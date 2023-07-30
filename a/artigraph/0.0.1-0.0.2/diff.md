# Comparing `tmp/artigraph-0.0.1.tar.gz` & `tmp/artigraph-0.0.2.tar.gz`

## Comparing `artigraph-0.0.1.tar` & `artigraph-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 artigraph-0.0.1/src/artigraph/__init__.py
--rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 artigraph-0.0.1/src/artigraph/db.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 artigraph-0.0.1/src/artigraph/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 artigraph-0.0.1/src/artigraph/api/__init__.py
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 artigraph-0.0.1/src/artigraph/api/artifact.py
--rw-r--r--   0        0        0     4948 2020-02-02 00:00:00.000000 artigraph-0.0.1/src/artigraph/api/artifact_group.py
--rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 artigraph-0.0.1/src/artigraph/api/node.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 artigraph-0.0.1/src/artigraph/api/run.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 artigraph-0.0.1/src/artigraph/orm/__init__.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 artigraph-0.0.1/src/artigraph/orm/artifact.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 artigraph-0.0.1/src/artigraph/orm/base.py
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 artigraph-0.0.1/src/artigraph/orm/node.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 artigraph-0.0.1/src/artigraph/orm/run.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 artigraph-0.0.1/src/artigraph/orm/run_parameter.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 artigraph-0.0.1/src/artigraph/serializer/__init__.py
--rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 artigraph-0.0.1/src/artigraph/serializer/_core.py
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 artigraph-0.0.1/src/artigraph/serializer/numpy.py
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 artigraph-0.0.1/src/artigraph/serializer/pandas.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 artigraph-0.0.1/src/artigraph/serializer/polars.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 artigraph-0.0.1/src/artigraph/storage/__init__.py
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 artigraph-0.0.1/src/artigraph/storage/_core.py
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 artigraph-0.0.1/src/artigraph/storage/aws.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 artigraph-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 artigraph-0.0.1/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 artigraph-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 artigraph-0.0.1/README.md
--rw-r--r--   0        0        0     3279 2020-02-02 00:00:00.000000 artigraph-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 artigraph-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/__init__.py
+-rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/db.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/api/__init__.py
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/api/artifact.py
+-rw-r--r--   0        0        0     4948 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/api/artifact_group.py
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/api/node.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/api/run.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/orm/__init__.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/orm/artifact.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/orm/base.py
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/orm/node.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/orm/run.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/orm/run_parameter.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/serializer/__init__.py
+-rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/serializer/_core.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/serializer/numpy.py
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/serializer/pandas.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/serializer/polars.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/storage/__init__.py
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/storage/_core.py
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 artigraph-0.0.2/src/artigraph/storage/aws.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 artigraph-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 artigraph-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 artigraph-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 artigraph-0.0.2/README.md
+-rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 artigraph-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 artigraph-0.0.2/PKG-INFO
```

### Comparing `artigraph-0.0.1/src/artigraph/db.py` & `artigraph-0.0.2/src/artigraph/db.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.1/src/artigraph/utils.py` & `artigraph-0.0.2/src/artigraph/utils.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.1/src/artigraph/api/artifact.py` & `artigraph-0.0.2/src/artigraph/api/artifact.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.1/src/artigraph/api/artifact_group.py` & `artigraph-0.0.2/src/artigraph/api/artifact_group.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.1/src/artigraph/api/node.py` & `artigraph-0.0.2/src/artigraph/api/node.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.1/src/artigraph/api/run.py` & `artigraph-0.0.2/src/artigraph/api/run.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.1/src/artigraph/orm/artifact.py` & `artigraph-0.0.2/src/artigraph/orm/artifact.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.1/src/artigraph/orm/base.py` & `artigraph-0.0.2/src/artigraph/orm/base.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.1/src/artigraph/orm/node.py` & `artigraph-0.0.2/src/artigraph/orm/node.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.1/src/artigraph/orm/run.py` & `artigraph-0.0.2/src/artigraph/orm/run.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.1/src/artigraph/orm/run_parameter.py` & `artigraph-0.0.2/src/artigraph/orm/run_parameter.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.1/src/artigraph/serializer/_core.py` & `artigraph-0.0.2/src/artigraph/serializer/_core.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.1/src/artigraph/serializer/numpy.py` & `artigraph-0.0.2/src/artigraph/serializer/numpy.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.1/src/artigraph/serializer/pandas.py` & `artigraph-0.0.2/src/artigraph/serializer/pandas.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.1/src/artigraph/serializer/polars.py` & `artigraph-0.0.2/src/artigraph/serializer/polars.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.1/src/artigraph/storage/_core.py` & `artigraph-0.0.2/src/artigraph/storage/_core.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.1/src/artigraph/storage/aws.py` & `artigraph-0.0.2/src/artigraph/storage/aws.py`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.1/.gitignore` & `artigraph-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.1/LICENSE.txt` & `artigraph-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.1/README.md` & `artigraph-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `artigraph-0.0.1/pyproject.toml` & `artigraph-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = ["- coverage combine", "coverage report"]
 cov = ["test-cov", "cov-report"]
 
 [[tool.hatch.envs.all.matrix]]
-python = ["3.7", "3.8", "3.9", "3.10", "3.11"]
+python = ["3.9", "3.10", "3.11"]
 
 [tool.hatch.envs.lint]
 detached = true
 dependencies = ["black>=23.1.0", "mypy>=1.0.0", "ruff>=0.0.243"]
 [tool.hatch.envs.lint.scripts]
 typing = "mypy --install-types --non-interactive {args:src/artigraph tests}"
 style = ["ruff {args:.}", "black --check --diff {args:.}"]
```

### Comparing `artigraph-0.0.1/PKG-INFO` & `artigraph-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artigraph
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library for interrelated graphs of artifacts and the runs that produce them.
 Project-URL: Documentation, https://github.com/unknown/artigraph#readme
 Project-URL: Issues, https://github.com/unknown/artigraph/issues
 Project-URL: Source, https://github.com/unknown/artigraph
 Author-email: "U.N. Owen" <void@some.where>
 License-Expression: MIT
 License-File: LICENSE.txt
```

