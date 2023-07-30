# Comparing `tmp/jsonator-0.1.4.tar.gz` & `tmp/jsonator-0.1.5.tar.gz`

## Comparing `jsonator-0.1.4.tar` & `jsonator-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 jsonator-0.1.4/jsonator/__init__.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 jsonator-0.1.4/jsonator/__main__.py
--rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 jsonator-0.1.4/jsonator/jsonator.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 jsonator-0.1.4/jsonator/output.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jsonator-0.1.4/.gitignore
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 jsonator-0.1.4/LICENSE
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 jsonator-0.1.4/README.rst
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 jsonator-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 jsonator-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 jsonator-0.1.5/jsonator/__init__.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 jsonator-0.1.5/jsonator/__main__.py
+-rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 jsonator-0.1.5/jsonator/jsonator.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 jsonator-0.1.5/jsonator/output.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jsonator-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 jsonator-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 jsonator-0.1.5/README.rst
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 jsonator-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 jsonator-0.1.5/PKG-INFO
```

### Comparing `jsonator-0.1.4/jsonator/__init__.py` & `jsonator-0.1.5/jsonator/__init__.py`

 * *Files identical despite different names*

### Comparing `jsonator-0.1.4/jsonator/jsonator.py` & `jsonator-0.1.5/jsonator/jsonator.py`

 * *Files identical despite different names*

### Comparing `jsonator-0.1.4/jsonator/output.py` & `jsonator-0.1.5/jsonator/output.py`

 * *Files identical despite different names*

### Comparing `jsonator-0.1.4/LICENSE` & `jsonator-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonator-0.1.4/README.rst` & `jsonator-0.1.5/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 JSONator
 ========
 
+[![Downloads](https://static.pepy.tech/badge/jsonator)](https://pepy.tech/project/jsonator)
+
 Description
 -----------
 
 This module provides a command-line interface for formatting JSON files.
 It takes a path to either a JSON file or a directory containing JSON files
 as input and can recursively scan subdirectories for JSON files. The module
 returns an exit code indicating whether any files were reformatted or if there
@@ -23,14 +25,16 @@
 
 * --check: An optional flag that indicates whether to perform a dry run and return the status without actually reformatting the files. The exit code will indicate whether any files would be reformatted or if there were any errors.
 
 * --diff: Don't write the files back, just output a diff for each file on stdout.
 
 * --color: Show colored diff. Only applies when `--diff` is given.
 
+* --sort-keys: Sort the output of dictionaries alphabetically by key.
+
 The module uses the ReturnCode enum to indicate the exit code of the formatting operation. The possible exit codes are:
 
 * `0`: Indicates that no files would be reformatted.
 
 * `1`: Indicates that some files would be reformatted.
 
 * `122`: Indicates that the specified file or directory was not found.
```

### Comparing `jsonator-0.1.4/pyproject.toml` & `jsonator-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=0.25.1",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "jsonator"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Sergey Fomin", email="sergiusnn@gmail.com" },
 ]
 description = "JSON formatting and validating tool"
 readme = "README.rst"
 requires-python = ">=3.5"
 classifiers = [
@@ -33,12 +33,12 @@
 
 [project.scripts]
 jsonator = "jsonator:main"
 
 [tool.poetry]
 readme = "README.rst"
 name = "jsonator"
-version = "0.1.4"
+version = "0.1.5"
 description = "JSON formatting and validating tool"
 authors = [
   "Sergey Fomin <sergiusnn@gmail.com>",
 ]
```

### Comparing `jsonator-0.1.4/PKG-INFO` & `jsonator-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: jsonator
-Version: 0.1.4
+Version: 0.1.5
 Summary: JSON formatting and validating tool
 Project-URL: Homepage, https://github.com/sfominx/jsonator
 Author-email: Sergey Fomin <sergiusnn@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
 
 JSONator
 ========
 
+[![Downloads](https://static.pepy.tech/badge/jsonator)](https://pepy.tech/project/jsonator)
+
 Description
 -----------
 
 This module provides a command-line interface for formatting JSON files.
 It takes a path to either a JSON file or a directory containing JSON files
 as input and can recursively scan subdirectories for JSON files. The module
 returns an exit code indicating whether any files were reformatted or if there
@@ -35,14 +37,16 @@
 
 * --check: An optional flag that indicates whether to perform a dry run and return the status without actually reformatting the files. The exit code will indicate whether any files would be reformatted or if there were any errors.
 
 * --diff: Don't write the files back, just output a diff for each file on stdout.
 
 * --color: Show colored diff. Only applies when `--diff` is given.
 
+* --sort-keys: Sort the output of dictionaries alphabetically by key.
+
 The module uses the ReturnCode enum to indicate the exit code of the formatting operation. The possible exit codes are:
 
 * `0`: Indicates that no files would be reformatted.
 
 * `1`: Indicates that some files would be reformatted.
 
 * `122`: Indicates that the specified file or directory was not found.
```

