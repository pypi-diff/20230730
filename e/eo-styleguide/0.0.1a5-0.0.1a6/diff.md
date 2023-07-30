# Comparing `tmp/eo_styleguide-0.0.1a5.tar.gz` & `tmp/eo_styleguide-0.0.1a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eo_styleguide-0.0.1a5.tar", max compression
+gzip compressed data, was "eo_styleguide-0.0.1a6.tar", max compression
```

## Comparing `eo_styleguide-0.0.1a5.tar` & `eo_styleguide-0.0.1a6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     3421 2023-07-29 14:37:37.987684 eo_styleguide-0.0.1a5/README.md
--rw-r--r--   0        0        0     1291 2023-07-29 05:28:56.221950 eo_styleguide-0.0.1a5/pyeo/__init__.py
--rw-r--r--   0        0        0     1118 2023-07-23 13:29:32.046205 eo_styleguide-0.0.1a5/pyeo/features/__init__.py
--rw-r--r--   0        0        0     1307 2023-07-23 13:29:32.046339 eo_styleguide-0.0.1a5/pyeo/features/feature.py
--rw-r--r--   0        0        0     1620 2023-07-29 22:13:02.772938 eo_styleguide-0.0.1a5/pyeo/features/final_object.py
--rw-r--r--   0        0        0     2810 2023-07-29 22:13:02.773315 eo_styleguide-0.0.1a5/pyeo/features/method_has_protocol.py
--rw-r--r--   0        0        0     2881 2023-07-29 22:13:02.773905 eo_styleguide-0.0.1a5/pyeo/features/no_code_in_ctors.py
--rw-r--r--   0        0        0     1739 2023-07-30 18:25:51.773677 eo_styleguide-0.0.1a5/pyeo/features/no_er_names.py
--rw-r--r--   0        0        0     1715 2023-07-29 22:13:02.774156 eo_styleguide-0.0.1a5/pyeo/features/no_property_methods.py
--rw-r--r--   0        0        0     2495 2023-07-29 13:16:52.754226 eo_styleguide-0.0.1a5/pyeo/features/no_reflection.py
--rw-r--r--   0        0        0     1977 2023-07-29 05:28:56.222831 eo_styleguide-0.0.1a5/pyeo/features/no_setters.py
--rw-r--r--   0        0        0     1794 2023-07-29 22:13:02.774412 eo_styleguide-0.0.1a5/pyeo/features/no_staticmethods.py
--rw-r--r--   0        0        0     1768 2023-07-23 13:29:32.046560 eo_styleguide-0.0.1a5/pyeo/features/object_has_protocol.py
--rw-r--r--   0        0        0     2128 2023-07-29 22:13:02.774645 eo_styleguide-0.0.1a5/pyeo/features/protocol_method_code_free.py
--rw-r--r--   0        0        0     3508 2023-07-29 22:13:02.774877 eo_styleguide-0.0.1a5/pyeo/main.py
--rw-r--r--   0        0        0        0 2023-07-21 21:17:44.927051 eo_styleguide-0.0.1a5/pyeo/py.typed
--rw-r--r--   0        0        0        0 2023-07-29 22:13:02.774933 eo_styleguide-0.0.1a5/pyeo/utils/__init__.py
--rw-r--r--   0        0        0      268 2023-07-29 22:13:02.775282 eo_styleguide-0.0.1a5/pyeo/utils/decorator_name.py
--rw-r--r--   0        0        0      813 2023-07-30 18:25:59.916717 eo_styleguide-0.0.1a5/pyproject.toml
--rw-r--r--   0        0        0     4312 1970-01-01 00:00:00.000000 eo_styleguide-0.0.1a5/PKG-INFO
+-rw-r--r--   0        0        0     3421 2023-07-29 14:37:37.987684 eo_styleguide-0.0.1a6/README.md
+-rw-r--r--   0        0        0     1291 2023-07-29 05:28:56.221950 eo_styleguide-0.0.1a6/pyeo/__init__.py
+-rw-r--r--   0        0        0     1118 2023-07-23 13:29:32.046205 eo_styleguide-0.0.1a6/pyeo/features/__init__.py
+-rw-r--r--   0        0        0     1307 2023-07-23 13:29:32.046339 eo_styleguide-0.0.1a6/pyeo/features/feature.py
+-rw-r--r--   0        0        0     1620 2023-07-29 22:13:02.772938 eo_styleguide-0.0.1a6/pyeo/features/final_object.py
+-rw-r--r--   0        0        0     2810 2023-07-29 22:13:02.773315 eo_styleguide-0.0.1a6/pyeo/features/method_has_protocol.py
+-rw-r--r--   0        0        0     2881 2023-07-29 22:13:02.773905 eo_styleguide-0.0.1a6/pyeo/features/no_code_in_ctors.py
+-rw-r--r--   0        0        0     2046 2023-07-30 18:28:11.179784 eo_styleguide-0.0.1a6/pyeo/features/no_er_names.py
+-rw-r--r--   0        0        0     1715 2023-07-29 22:13:02.774156 eo_styleguide-0.0.1a6/pyeo/features/no_property_methods.py
+-rw-r--r--   0        0        0     2495 2023-07-29 13:16:52.754226 eo_styleguide-0.0.1a6/pyeo/features/no_reflection.py
+-rw-r--r--   0        0        0     1977 2023-07-29 05:28:56.222831 eo_styleguide-0.0.1a6/pyeo/features/no_setters.py
+-rw-r--r--   0        0        0     1794 2023-07-29 22:13:02.774412 eo_styleguide-0.0.1a6/pyeo/features/no_staticmethods.py
+-rw-r--r--   0        0        0     1768 2023-07-23 13:29:32.046560 eo_styleguide-0.0.1a6/pyeo/features/object_has_protocol.py
+-rw-r--r--   0        0        0     2128 2023-07-29 22:13:02.774645 eo_styleguide-0.0.1a6/pyeo/features/protocol_method_code_free.py
+-rw-r--r--   0        0        0     3508 2023-07-29 22:13:02.774877 eo_styleguide-0.0.1a6/pyeo/main.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:17:44.927051 eo_styleguide-0.0.1a6/pyeo/py.typed
+-rw-r--r--   0        0        0        0 2023-07-29 22:13:02.774933 eo_styleguide-0.0.1a6/pyeo/utils/__init__.py
+-rw-r--r--   0        0        0      268 2023-07-29 22:13:02.775282 eo_styleguide-0.0.1a6/pyeo/utils/decorator_name.py
+-rw-r--r--   0        0        0      813 2023-07-30 18:28:25.131841 eo_styleguide-0.0.1a6/pyproject.toml
+-rw-r--r--   0        0        0     4312 1970-01-01 00:00:00.000000 eo_styleguide-0.0.1a6/PKG-INFO
```

### Comparing `eo_styleguide-0.0.1a5/README.md` & `eo_styleguide-0.0.1a6/README.md`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a5/pyeo/__init__.py` & `eo_styleguide-0.0.1a6/pyeo/__init__.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a5/pyeo/features/__init__.py` & `eo_styleguide-0.0.1a6/pyeo/features/__init__.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a5/pyeo/features/feature.py` & `eo_styleguide-0.0.1a6/pyeo/features/feature.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a5/pyeo/features/final_object.py` & `eo_styleguide-0.0.1a6/pyeo/features/final_object.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a5/pyeo/features/method_has_protocol.py` & `eo_styleguide-0.0.1a6/pyeo/features/method_has_protocol.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a5/pyeo/features/no_code_in_ctors.py` & `eo_styleguide-0.0.1a6/pyeo/features/no_code_in_ctors.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a5/pyeo/features/no_er_names.py` & `eo_styleguide-0.0.1a6/pyeo/features/no_er_names.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,11 +34,20 @@
         forbidden_suffix = (
             'er',
             'client',
             'Client',
         )
         class_name = ctx.cls.name
         for fs in forbidden_suffix:
-            if class_name.endswith(fs):
+            if class_name.endswith(fs) and not self._suffix_in_whitelist(class_name):
                 ctx.api.fail("Class '{0}' has forbidden class name suffix ({1}).".format(ctx.cls.name, fs), ctx.cls)
                 return False
         return True
+
+    def _suffix_in_whitelist(self, class_name):
+        whitelist = (
+            'Answer',
+        )
+        for whitelist_name in whitelist:
+            if class_name[-len(whitelist_name):] == whitelist_name:
+                return True
+        return False
```

### Comparing `eo_styleguide-0.0.1a5/pyeo/features/no_property_methods.py` & `eo_styleguide-0.0.1a6/pyeo/features/no_property_methods.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a5/pyeo/features/no_reflection.py` & `eo_styleguide-0.0.1a6/pyeo/features/no_reflection.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a5/pyeo/features/no_setters.py` & `eo_styleguide-0.0.1a6/pyeo/features/no_setters.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a5/pyeo/features/no_staticmethods.py` & `eo_styleguide-0.0.1a6/pyeo/features/no_staticmethods.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a5/pyeo/features/object_has_protocol.py` & `eo_styleguide-0.0.1a6/pyeo/features/object_has_protocol.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a5/pyeo/features/protocol_method_code_free.py` & `eo_styleguide-0.0.1a6/pyeo/features/protocol_method_code_free.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a5/pyeo/main.py` & `eo_styleguide-0.0.1a6/pyeo/main.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a5/pyproject.toml` & `eo_styleguide-0.0.1a6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "eo-styleguide"
 packages = [
     {include = "pyeo"}
 ]
-version = "0.0.1-alpha5"
+version = "0.0.1-alpha6"
 description = "Pyeo is an advanced static analysis tool tailored specifically to enforce the principles advocated by Elegant Objects (elegantobjects.org) in Python projects. It serves as a quality control instrument to ensure that your Python code adheres to the core tenets of elegance, simplicity, and maintainability."
 authors = ["Almaz Ilaletdinov <a.ilaletdinov@yandex.ru>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
```

### Comparing `eo_styleguide-0.0.1a5/PKG-INFO` & `eo_styleguide-0.0.1a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eo-styleguide
-Version: 0.0.1a5
+Version: 0.0.1a6
 Summary: Pyeo is an advanced static analysis tool tailored specifically to enforce the principles advocated by Elegant Objects (elegantobjects.org) in Python projects. It serves as a quality control instrument to ensure that your Python code adheres to the core tenets of elegance, simplicity, and maintainability.
 License: MIT
 Author: Almaz Ilaletdinov
 Author-email: a.ilaletdinov@yandex.ru
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

