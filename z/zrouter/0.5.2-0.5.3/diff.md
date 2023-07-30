# Comparing `tmp/zrouter-0.5.2.tar.gz` & `tmp/zrouter-0.5.3.tar.gz`

## Comparing `zrouter-0.5.2.tar` & `zrouter-0.5.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 zrouter-0.5.2/src/zrouter/__init__.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 zrouter-0.5.2/src/zrouter/restful.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 zrouter-0.5.2/src/zrouter/router.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zrouter-0.5.2/src/zrouter/exceptions/__init__.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 zrouter-0.5.2/src/zrouter/utils/json.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 zrouter-0.5.2/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zrouter-0.5.2/LICENSE
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 zrouter-0.5.2/README.md
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 zrouter-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 zrouter-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 zrouter-0.5.3/src/zrouter/__init__.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 zrouter-0.5.3/src/zrouter/restful.py
+-rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 zrouter-0.5.3/src/zrouter/router.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zrouter-0.5.3/src/zrouter/exceptions/__init__.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 zrouter-0.5.3/src/zrouter/utils/json.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 zrouter-0.5.3/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zrouter-0.5.3/LICENSE
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 zrouter-0.5.3/README.md
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 zrouter-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 zrouter-0.5.3/PKG-INFO
```

### Comparing `zrouter-0.5.2/src/zrouter/restful.py` & `zrouter-0.5.3/src/zrouter/restful.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -21,8 +21,8 @@
         'get': get,
         'post': post,
         'put': put,
         'delete': delete
     }
 
     return type('Resource', (object,), method_dict)
-    
+
```

### Comparing `zrouter-0.5.2/src/zrouter/router.py` & `zrouter-0.5.3/src/zrouter/router.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         for method_name in http_methods:
             if method_name in dir(resource_class):
                 method =getattr(resource_class, method_name)
                 open = getattr(method, 'open', False)
                 direct = getattr(method, 'direct', False)
                 endpoint = str(random.randint(10000000, 99999999))
                 self.add_url_rule(rule, endpoint, self.wrap_view_func(method,
-                    open=open, direct=direct), methods=[method.upper()])
+                    open=open, direct=direct), methods=[method_name.upper()])
 
     def add_resources(self, resource_map):
         for rule, resource_class in resource_map.items():
             self.add_resource(rule, resource_class)
 
     def add(self, rule, open=False, direct=False, **options):
         def decorator(f):
```

### Comparing `zrouter-0.5.2/src/zrouter/utils/json.py` & `zrouter-0.5.3/src/zrouter/utils/json.py`

 * *Files identical despite different names*

### Comparing `zrouter-0.5.2/LICENSE` & `zrouter-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zrouter-0.5.2/pyproject.toml` & `zrouter-0.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zrouter"
-version = "0.5.2"
+version = "0.5.3"
 authors = [
   { name="inspirare6", email="inspirare6@163.com" },
 ]
 description = "zen router library"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

