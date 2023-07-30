# Comparing `tmp/polarify-0.1.0.tar.gz` & `tmp/polarify-0.1.1.tar.gz`

## Comparing `polarify-0.1.0.tar` & `polarify-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 polarify-0.1.0/polarify/__init__.py
--rw-r--r--   0        0        0     8338 2020-02-02 00:00:00.000000 polarify-0.1.0/polarify/main.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 polarify-0.1.0/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 polarify-0.1.0/LICENSE
--rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 polarify-0.1.0/README.md
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 polarify-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 polarify-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 polarify-0.1.1/polarify/__init__.py
+-rw-r--r--   0        0        0     8338 2020-02-02 00:00:00.000000 polarify-0.1.1/polarify/main.py
+-rw-r--r--   0        0        0     7817 2020-02-02 00:00:00.000000 polarify-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 polarify-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 polarify-0.1.1/README.md
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 polarify-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 polarify-0.1.1/PKG-INFO
```

### Comparing `polarify-0.1.0/polarify/__init__.py` & `polarify-0.1.1/polarify/__init__.py`

 * *Files identical despite different names*

### Comparing `polarify-0.1.0/polarify/main.py` & `polarify-0.1.1/polarify/main.py`

 * *Files identical despite different names*

### Comparing `polarify-0.1.0/LICENSE` & `polarify-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `polarify-0.1.0/README.md` & `polarify-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `polarify-0.1.0/pyproject.toml` & `polarify-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "polarify"
 description = "Simplifying conditional Polars Expressions with Python 🐍 🐻‍❄️"
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.9"
 authors = [
     { name = "Bela Stoyan", email = "bela.stoyan@quantco.com" },
     { name = "Pavel Zwerschke", email = "pavel.zwerschke@quantco.com" },
 ]
```

### Comparing `polarify-0.1.0/PKG-INFO` & `polarify-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polarify
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simplifying conditional Polars Expressions with Python 🐍 🐻‍❄️
 Project-URL: Homepage, https://github.com/quantco/polarify
 Author-email: Bela Stoyan <bela.stoyan@quantco.com>, Pavel Zwerschke <pavel.zwerschke@quantco.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

