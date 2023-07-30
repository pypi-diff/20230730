# Comparing `tmp/zrouter-0.5.1.tar.gz` & `tmp/zrouter-0.5.2.tar.gz`

## Comparing `zrouter-0.5.1.tar` & `zrouter-0.5.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 zrouter-0.5.1/src/zrouter/__init__.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 zrouter-0.5.1/src/zrouter/restful.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zrouter-0.5.1/src/zrouter/exceptions/__init__.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 zrouter-0.5.1/src/zrouter/utils/json.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 zrouter-0.5.1/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zrouter-0.5.1/LICENSE
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 zrouter-0.5.1/README.md
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 zrouter-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 zrouter-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 zrouter-0.5.2/src/zrouter/__init__.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 zrouter-0.5.2/src/zrouter/restful.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 zrouter-0.5.2/src/zrouter/router.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zrouter-0.5.2/src/zrouter/exceptions/__init__.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 zrouter-0.5.2/src/zrouter/utils/json.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 zrouter-0.5.2/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zrouter-0.5.2/LICENSE
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 zrouter-0.5.2/README.md
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 zrouter-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 zrouter-0.5.2/PKG-INFO
```

### Comparing `zrouter-0.5.1/src/zrouter/__init__.py` & `zrouter-0.5.2/src/zrouter/router.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import random
 
 
 class ParamMixin:
     @staticmethod
     def get_params():
         if request.method in ['GET', 'DELETE']:
-            return to_lowcase(request.args)
+            return to_lowcase({**request.args, **request.view_args})
         elif 'multipart/form-data' in request.content_type:
             return {
                 'files': request.files,
                 'params': to_lowcase(request.form.to_dict())
             }
         else:
             try:
@@ -26,28 +26,29 @@
                 }
 
     @staticmethod
     def clean_params(params):
         return {k: v for k, v in params.items() if v not in ('', 'null', None)}
 
 
-class Router(ABC, ParamMixin, Blueprint):
+class Router(ParamMixin, Blueprint):
     """路由"""
+
     def __init__(self, *args, **kwargs):
         Blueprint.__init__(self, *args, **kwargs)
 
     def verify_user(self):
         """用户验证，通过继承覆盖此方法实现具体逻辑"""
         return True
 
     def handle_error(self, e):
         """错误处理，通过继承覆盖此方法实现具体逻辑"""
         pass
 
-    def wrap_func(self, func, direct=False, open=False):
+    def wrap_view_func(self, func, direct=False, open=False):
         @wraps(func)
         def wrapper(*args, **kwargs):
             params = self.clean_params(self.get_params())
             if not self.verify_user() and not open:
                 return {'code': 401, 'msg': '用户无权限'}
             try:
                 data = func(**params)
@@ -65,24 +66,27 @@
             elif isinstance(data, list):
                 data = [iter_camel(item) for item in data]
             return {'code': 200, 'msg': '操作成功', 'data': data}
         return wrapper
 
     def add_resource(self, rule, resource_class):
         http_methods = ['get', 'post', 'put', 'delete']
-        
-        for method in http_methods:
-            if method in dir(resource_class):
+
+        for method_name in http_methods:
+            if method_name in dir(resource_class):
+                method =getattr(resource_class, method_name)
+                open = getattr(method, 'open', False)
+                direct = getattr(method, 'direct', False)
                 endpoint = str(random.randint(10000000, 99999999))
-                self.add_url_rule(rule, endpoint, self.wrap_func(
-                    getattr(resource_class, method)), methods=[method.upper()])
+                self.add_url_rule(rule, endpoint, self.wrap_view_func(method,
+                    open=open, direct=direct), methods=[method.upper()])
 
     def add_resources(self, resource_map):
         for rule, resource_class in resource_map.items():
             self.add_resource(rule, resource_class)
 
     def add(self, rule, open=False, direct=False, **options):
         def decorator(f):
             endpoint = options.pop("endpoint", None)
-            self.add_url_rule(rule, endpoint, self.wrap_func(
+            self.add_url_rule(rule, endpoint, self.wrap_view_func(
                 f, open=open, direct=direct), **options)
         return decorator
```

### Comparing `zrouter-0.5.1/src/zrouter/restful.py` & `zrouter-0.5.2/src/zrouter/restful.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional
 
 
-def resource_generator(resource_name, mapper_class):
+def R(mapper_class):
     def get(id: Optional[int] = None, page_num: Optional[int] = None, page_size: Optional[int] = None, **kwargs):
         if id:
             return mapper_class.get_json(id)
         else:
             return mapper_class.get_jsons(page_num=page_num, page_size=page_size)
 
     def post(data: dict):
@@ -13,16 +13,16 @@
 
     def put(id: int, data: dict):
         mapper_class.save(id, data)
 
     def delete(id: int):
         mapper_class.delete(id=id)
 
-    resource_dict = {
+    method_dict = {
         'get': get,
         'post': post,
         'put': put,
         'delete': delete
     }
 
-    resource_class = type(resource_name, (object,), resource_dict)
-    return resource_class
+    return type('Resource', (object,), method_dict)
+
```

### Comparing `zrouter-0.5.1/src/zrouter/utils/json.py` & `zrouter-0.5.2/src/zrouter/utils/json.py`

 * *Files identical despite different names*

### Comparing `zrouter-0.5.1/LICENSE` & `zrouter-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zrouter-0.5.1/pyproject.toml` & `zrouter-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zrouter"
-version = "0.5.1"
+version = "0.5.2"
 authors = [
   { name="inspirare6", email="inspirare6@163.com" },
 ]
 description = "zen router library"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

