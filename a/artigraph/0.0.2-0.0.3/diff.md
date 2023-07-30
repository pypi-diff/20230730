# Comparing `tmp/artigraph-0.0.2.tar.gz` & `tmp/artigraph-0.0.3.tar.gz`

## Comparing `artigraph-0.0.2.tar` & `artigraph-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/__init__.py
--rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/db.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/api/__init__.py
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/api/artifact.py
--rw-r--r--   0        0        0     4948 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/api/artifact_group.py
--rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/api/node.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/api/run.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/orm/__init__.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/orm/artifact.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/orm/base.py
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/orm/node.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/orm/run.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/orm/run_parameter.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/serializer/__init__.py
--rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/serializer/_core.py
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/serializer/numpy.py
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/serializer/pandas.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/serializer/polars.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/storage/__init__.py
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/storage/_core.py
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/storage/aws.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 artigraph-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 artigraph-0.0.2/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 artigraph-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 artigraph-0.0.2/README.md
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 artigraph-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 artigraph-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/__init__.py
+-rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/db.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/api/__init__.py
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/api/artifact.py
+-rw-r--r--   0        0        0     4948 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/api/artifact_group.py
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/api/node.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/api/run.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/orm/__init__.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/orm/artifact.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/orm/base.py
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/orm/node.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/orm/run.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/orm/run_parameter.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/serializer/__init__.py
+-rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/serializer/_core.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/serializer/numpy.py
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/serializer/pandas.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/serializer/polars.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/storage/__init__.py
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/storage/_core.py
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 artigraph-0.0.3/src/artigraph/storage/aws.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 artigraph-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 artigraph-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 artigraph-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 artigraph-0.0.3/README.md
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 artigraph-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 artigraph-0.0.3/PKG-INFO
```

### Comparing `artigraph-0.0.2/src/artigraph/db.py` & `artigraph-0.0.3/src/artigraph/db.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.2/src/artigraph/utils.py` & `artigraph-0.0.3/src/artigraph/utils.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.2/src/artigraph/api/artifact.py` & `artigraph-0.0.3/src/artigraph/api/artifact.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.2/src/artigraph/api/artifact_group.py` & `artigraph-0.0.3/src/artigraph/api/artifact_group.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.2/src/artigraph/api/node.py` & `artigraph-0.0.3/src/artigraph/api/node.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.2/src/artigraph/api/run.py` & `artigraph-0.0.3/src/artigraph/api/run.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.2/src/artigraph/orm/artifact.py` & `artigraph-0.0.3/src/artigraph/orm/artifact.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.2/src/artigraph/orm/base.py` & `artigraph-0.0.3/src/artigraph/orm/base.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.2/src/artigraph/orm/node.py` & `artigraph-0.0.3/src/artigraph/orm/node.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.2/src/artigraph/orm/run.py` & `artigraph-0.0.3/src/artigraph/orm/run.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.2/src/artigraph/orm/run_parameter.py` & `artigraph-0.0.3/src/artigraph/orm/run_parameter.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.2/src/artigraph/serializer/_core.py` & `artigraph-0.0.3/src/artigraph/serializer/_core.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.2/src/artigraph/serializer/numpy.py` & `artigraph-0.0.3/src/artigraph/serializer/numpy.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.2/src/artigraph/serializer/pandas.py` & `artigraph-0.0.3/src/artigraph/serializer/pandas.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.2/src/artigraph/serializer/polars.py` & `artigraph-0.0.3/src/artigraph/serializer/polars.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.2/src/artigraph/storage/_core.py` & `artigraph-0.0.3/src/artigraph/storage/_core.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.2/src/artigraph/storage/aws.py` & `artigraph-0.0.3/src/artigraph/storage/aws.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.2/.gitignore` & `artigraph-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.2/LICENSE.txt` & `artigraph-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.2/pyproject.toml` & `artigraph-0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 requires-python = ">=3.9"
 license = "MIT"
 keywords = []
 authors = [{ name = "U.N. Owen", email = "void@some.where" }]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.7",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = ["typing_extensions", "sqlalchemy>=2,<3", "anyio>=3,<4"]
```

### Comparing `artigraph-0.0.2/PKG-INFO` & `artigraph-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: artigraph
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library for interrelated graphs of artifacts and the runs that produce them.
 Project-URL: Documentation, https://github.com/unknown/artigraph#readme
 Project-URL: Issues, https://github.com/unknown/artigraph/issues
 Project-URL: Source, https://github.com/unknown/artigraph
 Author-email: "U.N. Owen" <void@some.where>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9
 Requires-Dist: anyio<4,>=3
@@ -51,10 +49,14 @@
 
 ## Installation
 
 ```console
 pip install artigraph
 ```
 
+## Usage
+
+🚧 Still under construction 🚧
+
 ## License
 
 `artigraph` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

