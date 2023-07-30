# Comparing `tmp/sql_constructor-1.0.1.tar.gz` & `tmp/sql_constructor-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_constructor-1.0.1.tar", last modified: Sun Jul 30 08:11:31 2023, max compression
+gzip compressed data, was "sql_constructor-1.0.2.tar", last modified: Sun Jul 30 10:05:31 2023, max compression
```

## Comparing `sql_constructor-1.0.1.tar` & `sql_constructor-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 08:11:31.979083 sql_constructor-1.0.1/
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     1071 2023-07-30 07:56:34.000000 sql_constructor-1.0.1/LICENSE
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     1088 2023-07-30 08:11:31.979083 sql_constructor-1.0.1/PKG-INFO
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)      348 2023-07-18 03:54:55.000000 sql_constructor-1.0.1/README.md
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)      814 2023-07-30 08:11:06.000000 sql_constructor-1.0.1/pyproject.toml
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)       38 2023-07-30 08:11:31.979083 sql_constructor-1.0.1/setup.cfg
-drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 08:11:31.977083 sql_constructor-1.0.1/src/
-drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 08:11:31.978083 sql_constructor-1.0.1/src/sql_constructor/
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)      252 2023-07-30 07:56:17.000000 sql_constructor-1.0.1/src/sql_constructor/__init__.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     2404 2023-07-18 03:57:34.000000 sql_constructor-1.0.1/src/sql_constructor/constants.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)      744 2023-07-18 04:01:33.000000 sql_constructor-1.0.1/src/sql_constructor/helpers.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     5120 2023-07-30 06:25:04.000000 sql_constructor-1.0.1/src/sql_constructor/sql_container.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     1925 2023-07-30 05:43:49.000000 sql_constructor-1.0.1/src/sql_constructor/sql_cte.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     5458 2023-07-30 05:37:39.000000 sql_constructor-1.0.1/src/sql_constructor/sql_query.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     3893 2023-07-29 13:51:13.000000 sql_constructor-1.0.1/src/sql_constructor/sql_section.py
-drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 08:11:31.978083 sql_constructor-1.0.1/src/sql_constructor.egg-info/
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     1088 2023-07-30 08:11:31.000000 sql_constructor-1.0.1/src/sql_constructor.egg-info/PKG-INFO
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)      436 2023-07-30 08:11:31.000000 sql_constructor-1.0.1/src/sql_constructor.egg-info/SOURCES.txt
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)        1 2023-07-30 08:11:31.000000 sql_constructor-1.0.1/src/sql_constructor.egg-info/dependency_links.txt
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)       16 2023-07-30 08:11:31.000000 sql_constructor-1.0.1/src/sql_constructor.egg-info/top_level.txt
+drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 10:05:31.446557 sql_constructor-1.0.2/
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     1071 2023-07-30 07:56:34.000000 sql_constructor-1.0.2/LICENSE
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     4725 2023-07-30 10:05:31.446557 sql_constructor-1.0.2/PKG-INFO
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     3985 2023-07-30 10:03:56.000000 sql_constructor-1.0.2/README.md
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)      814 2023-07-30 09:19:00.000000 sql_constructor-1.0.2/pyproject.toml
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)       38 2023-07-30 10:05:31.446557 sql_constructor-1.0.2/setup.cfg
+drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 10:05:31.444557 sql_constructor-1.0.2/src/
+drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 10:05:31.445557 sql_constructor-1.0.2/src/sql_constructor/
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)      252 2023-07-30 07:56:17.000000 sql_constructor-1.0.2/src/sql_constructor/__init__.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     2404 2023-07-18 03:57:34.000000 sql_constructor-1.0.2/src/sql_constructor/constants.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)      744 2023-07-18 04:01:33.000000 sql_constructor-1.0.2/src/sql_constructor/helpers.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     5124 2023-07-30 09:02:56.000000 sql_constructor-1.0.2/src/sql_constructor/sql_container.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     1925 2023-07-30 05:43:49.000000 sql_constructor-1.0.2/src/sql_constructor/sql_cte.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     5458 2023-07-30 05:37:39.000000 sql_constructor-1.0.2/src/sql_constructor/sql_query.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     3893 2023-07-29 13:51:13.000000 sql_constructor-1.0.2/src/sql_constructor/sql_section.py
+drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-07-30 10:05:31.446557 sql_constructor-1.0.2/src/sql_constructor.egg-info/
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     4725 2023-07-30 10:05:31.000000 sql_constructor-1.0.2/src/sql_constructor.egg-info/PKG-INFO
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)      436 2023-07-30 10:05:31.000000 sql_constructor-1.0.2/src/sql_constructor.egg-info/SOURCES.txt
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)        1 2023-07-30 10:05:31.000000 sql_constructor-1.0.2/src/sql_constructor.egg-info/dependency_links.txt
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)       16 2023-07-30 10:05:31.000000 sql_constructor-1.0.2/src/sql_constructor.egg-info/top_level.txt
```

### Comparing `sql_constructor-1.0.1/LICENSE` & `sql_constructor-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.1/pyproject.toml` & `sql_constructor-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sql_constructor"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Andrey Smirnov", email="abc-sm@yandex.ru" },
 ]
-description = "Let you build SQL requests in pythonic way. SQL blocks could be nested as you want it to be, constracted dynamically and looks pretty. You could also build request once and cache it (but still use variables to replace dinamically). Solid solution!"
+description = "Let you build SQL requests in pythonic way. SQL blocks could be nested as you want it to be, constracted dynamically and looks pretty! You could also build request once and cache it (but still use variables to replace dinamically). Solid solution!"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `sql_constructor-1.0.1/src/sql_constructor/constants.py` & `sql_constructor-1.0.2/src/sql_constructor/constants.py`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.1/src/sql_constructor/helpers.py` & `sql_constructor-1.0.2/src/sql_constructor/helpers.py`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.1/src/sql_constructor/sql_container.py` & `sql_constructor-1.0.2/src/sql_constructor/sql_container.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             which are useful if you have passed placeholders in SQL body
             (placeholder starts with ! character and is continued by an word with no space,
             !my_var for example) and want replace placeholders by variables.
             You could: 
                 - set variables by calling instance of SqlContainer with any keyword arguments 
                 (which all will be added to self.vars) 
                 - and get SQL text where placeholders are replaced by self.vars 
-                if you call self.get() method.
+                if you call self.dumps() method.
     """
     def __init__(self, text: str, wrapper_text: Optional[str] = None):
         self.text: str = text
         self.wrapper_text: Optional[str] = wrapper_text
         self.vars: dict = {}
 
     def __bool__(self):
@@ -53,15 +53,15 @@
         """Convert SqlContainer instance to str"""
         return get_string_representation(self.text, self.wrapper_text)
 
     def __str__(self) -> str:
         """Return SqlContainer as str"""
         return repr(self)
 
-    def get(self) -> str:
+    def dumps(self) -> str:
         """Get SqlContainer as str and do replace placeholders by self.vars 
         if the latter were set (you could set vars by __call__ method).
         Notice: self.get method do not replace in self.text attribute. 
         It process replacement and give string as a result.
         """
         text = self.text
         if text and self.vars:
```

### Comparing `sql_constructor-1.0.1/src/sql_constructor/sql_cte.py` & `sql_constructor-1.0.2/src/sql_constructor/sql_cte.py`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.1/src/sql_constructor/sql_query.py` & `sql_constructor-1.0.2/src/sql_constructor/sql_query.py`

 * *Files identical despite different names*

### Comparing `sql_constructor-1.0.1/src/sql_constructor/sql_section.py` & `sql_constructor-1.0.2/src/sql_constructor/sql_section.py`

 * *Files identical despite different names*

