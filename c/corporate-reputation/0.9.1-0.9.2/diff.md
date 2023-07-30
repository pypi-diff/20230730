# Comparing `tmp/corporate_reputation-0.9.1.tar.gz` & `tmp/corporate_reputation-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corporate_reputation-0.9.1.tar", max compression
+gzip compressed data, was "corporate_reputation-0.9.2.tar", max compression
```

## Comparing `corporate_reputation-0.9.1.tar` & `corporate_reputation-0.9.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1071 2023-07-28 08:07:10.542220 corporate_reputation-0.9.1/LICENSE
--rw-r--r--   0        0        0     3898 2023-07-28 08:07:10.542220 corporate_reputation-0.9.1/README.md
--rw-r--r--   0        0        0     3407 2023-07-28 08:07:45.666115 corporate_reputation-0.9.1/pyproject.toml
--rw-r--r--   0        0        0      182 2023-07-28 08:07:10.546221 corporate_reputation-0.9.1/src/corprep/__cli__.py
--rw-r--r--   0        0        0      496 2023-07-28 08:07:10.546221 corporate_reputation-0.9.1/src/corprep/__init__.py
--rw-r--r--   0        0        0       22 2023-07-28 08:07:45.622115 corporate_reputation-0.9.1/src/corprep/_version.py
--rw-r--r--   0        0        0        0 2023-07-28 08:07:10.546221 corporate_reputation-0.9.1/src/corprep/absa/__init__.py
--rw-r--r--   0        0        0     1785 2023-07-28 08:07:10.546221 corporate_reputation-0.9.1/src/corprep/absa/agent.py
--rw-r--r--   0        0        0     4793 2023-07-28 08:07:10.546221 corporate_reputation-0.9.1/src/corprep/absa/config.py
--rw-r--r--   0        0        0        0 2023-07-28 08:07:10.546221 corporate_reputation-0.9.1/src/corprep/conf/__init__.py
--rw-r--r--   0        0        0      286 2023-07-28 08:07:10.546221 corporate_reputation-0.9.1/src/corprep/conf/about/corprep.yaml
--rw-r--r--   0        0        0      259 2023-07-28 08:07:10.546221 corporate_reputation-0.9.1/src/corprep/conf/absa/default.yaml
--rw-r--r--   0        0        0     2930 2023-07-28 08:07:10.546221 corporate_reputation-0.9.1/src/corprep/conf/absa/prompts/default.yaml
--rw-r--r--   0        0        0      132 2023-07-28 08:07:10.546221 corporate_reputation-0.9.1/src/corprep/conf/pipe/absa_agent_predict.yaml
--rw-r--r--   0        0        0      116 2023-07-28 08:07:10.546221 corporate_reputation-0.9.1/src/corprep/conf/pipe/dataframe_save.yaml
--rw-r--r--   0        0        0      156 2023-07-28 08:07:10.546221 corporate_reputation-0.9.1/src/corprep/conf/pipe/dataset_filter.yaml
--rw-r--r--   0        0        0       85 2023-07-28 08:07:10.546221 corporate_reputation-0.9.1/src/corprep/conf/pipe/dataset_to_pandas.yaml
--rw-r--r--   0        0        0      134 2023-07-28 08:07:10.546221 corporate_reputation-0.9.1/src/corprep/conf/pipe/find_similar_docs_ac.yaml
--rw-r--r--   0        0        0      131 2023-07-28 08:07:10.546221 corporate_reputation-0.9.1/src/corprep/conf/pipe/load_raw_dataset.yaml
--rw-r--r--   0        0        0      101 2023-07-28 08:07:10.546221 corporate_reputation-0.9.1/src/corprep/conf/pipe/pandas_print_head.yaml
--rw-r--r--   0        0        0      200 2023-07-28 08:07:10.546221 corporate_reputation-0.9.1/src/corprep/conf/run/absa_agent_predict.yaml
--rw-r--r--   0        0        0      147 2023-07-28 08:07:10.546221 corporate_reputation-0.9.1/src/corprep/conf/run/filter_dataset.yaml
--rw-r--r--   0        0        0      393 2023-07-28 08:07:10.546221 corporate_reputation-0.9.1/src/corprep/conf/run/find_similar_docs_ac.yaml
--rw-r--r--   0        0        0      117 2023-07-28 08:07:10.546221 corporate_reputation-0.9.1/src/corprep/conf/run/load_raw_dataset.yaml
--rw-r--r--   0        0        0      169 2023-07-28 08:07:10.546221 corporate_reputation-0.9.1/src/corprep/conf/run/save_dataframes.yaml
--rw-r--r--   0        0        0      204 2023-07-28 08:07:10.546221 corporate_reputation-0.9.1/src/corprep/datasets/__init__.py
--rw-r--r--   0        0        0     1013 2023-07-28 08:07:10.546221 corporate_reputation-0.9.1/src/corprep/datasets/io.py
--rw-r--r--   0        0        0     9569 2023-07-28 08:07:10.546221 corporate_reputation-0.9.1/src/corprep/datasets/similarity.py
--rw-r--r--   0        0        0        0 2023-07-28 08:07:10.546221 corporate_reputation-0.9.1/src/corprep/py.typed
--rw-r--r--   0        0        0     4853 1970-01-01 00:00:00.000000 corporate_reputation-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-30 11:32:26.379059 corporate_reputation-0.9.2/LICENSE
+-rw-r--r--   0        0        0     3898 2023-07-30 11:32:26.379059 corporate_reputation-0.9.2/README.md
+-rw-r--r--   0        0        0     3428 2023-07-30 11:33:00.835600 corporate_reputation-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0      182 2023-07-30 11:32:26.383061 corporate_reputation-0.9.2/src/corprep/__cli__.py
+-rw-r--r--   0        0        0      506 2023-07-30 11:32:26.383061 corporate_reputation-0.9.2/src/corprep/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-30 11:33:00.787599 corporate_reputation-0.9.2/src/corprep/_version.py
+-rw-r--r--   0        0        0        0 2023-07-30 11:32:26.383061 corporate_reputation-0.9.2/src/corprep/absa/__init__.py
+-rw-r--r--   0        0        0     1785 2023-07-30 11:32:26.383061 corporate_reputation-0.9.2/src/corprep/absa/agent.py
+-rw-r--r--   0        0        0     4793 2023-07-30 11:32:26.383061 corporate_reputation-0.9.2/src/corprep/absa/config.py
+-rw-r--r--   0        0        0        0 2023-07-30 11:32:26.383061 corporate_reputation-0.9.2/src/corprep/conf/__init__.py
+-rw-r--r--   0        0        0      286 2023-07-30 11:32:26.383061 corporate_reputation-0.9.2/src/corprep/conf/about/corprep.yaml
+-rw-r--r--   0        0        0      259 2023-07-30 11:32:26.383061 corporate_reputation-0.9.2/src/corprep/conf/absa/default.yaml
+-rw-r--r--   0        0        0     2930 2023-07-30 11:32:26.383061 corporate_reputation-0.9.2/src/corprep/conf/absa/prompts/default.yaml
+-rw-r--r--   0        0        0      132 2023-07-30 11:32:26.383061 corporate_reputation-0.9.2/src/corprep/conf/pipe/absa_agent_predict.yaml
+-rw-r--r--   0        0        0      116 2023-07-30 11:32:26.383061 corporate_reputation-0.9.2/src/corprep/conf/pipe/dataframe_save.yaml
+-rw-r--r--   0        0        0      156 2023-07-30 11:32:26.383061 corporate_reputation-0.9.2/src/corprep/conf/pipe/dataset_filter.yaml
+-rw-r--r--   0        0        0       85 2023-07-30 11:32:26.383061 corporate_reputation-0.9.2/src/corprep/conf/pipe/dataset_to_pandas.yaml
+-rw-r--r--   0        0        0      134 2023-07-30 11:32:26.383061 corporate_reputation-0.9.2/src/corprep/conf/pipe/find_similar_docs_ac.yaml
+-rw-r--r--   0        0        0      131 2023-07-30 11:32:26.383061 corporate_reputation-0.9.2/src/corprep/conf/pipe/load_raw_dataset.yaml
+-rw-r--r--   0        0        0      101 2023-07-30 11:32:26.383061 corporate_reputation-0.9.2/src/corprep/conf/pipe/pandas_print_head.yaml
+-rw-r--r--   0        0        0      200 2023-07-30 11:32:26.383061 corporate_reputation-0.9.2/src/corprep/conf/run/absa_agent_predict.yaml
+-rw-r--r--   0        0        0      147 2023-07-30 11:32:26.383061 corporate_reputation-0.9.2/src/corprep/conf/run/filter_dataset.yaml
+-rw-r--r--   0        0        0      393 2023-07-30 11:32:26.383061 corporate_reputation-0.9.2/src/corprep/conf/run/find_similar_docs_ac.yaml
+-rw-r--r--   0        0        0      117 2023-07-30 11:32:26.383061 corporate_reputation-0.9.2/src/corprep/conf/run/load_raw_dataset.yaml
+-rw-r--r--   0        0        0      169 2023-07-30 11:32:26.383061 corporate_reputation-0.9.2/src/corprep/conf/run/save_dataframes.yaml
+-rw-r--r--   0        0        0      204 2023-07-30 11:32:26.383061 corporate_reputation-0.9.2/src/corprep/datasets/__init__.py
+-rw-r--r--   0        0        0     1013 2023-07-30 11:32:26.383061 corporate_reputation-0.9.2/src/corprep/datasets/io.py
+-rw-r--r--   0        0        0     9569 2023-07-30 11:32:26.383061 corporate_reputation-0.9.2/src/corprep/datasets/similarity.py
+-rw-r--r--   0        0        0        0 2023-07-30 11:32:26.383061 corporate_reputation-0.9.2/src/corprep/py.typed
+-rw-r--r--   0        0        0     4895 1970-01-01 00:00:00.000000 corporate_reputation-0.9.2/PKG-INFO
```

### Comparing `corporate_reputation-0.9.1/LICENSE` & `corporate_reputation-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.9.1/README.md` & `corporate_reputation-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.9.1/pyproject.toml` & `corporate_reputation-0.9.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [tool.poetry]
 name = "corporate-reputation"
-version = "0.9.1"
+version = "0.9.2"
 description = "Unraveling Corporate and CEO Reputation using Aspect-Based Sentiment Analysis and Signal Modeling"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://entelecheia.github.io/corporate-reputation"
 repository = "https://github.com/entelecheia/corporate-reputation"
 readme = "README.md"
 packages = [{ include = "corprep", from = "src" }]
 
 [tool.poetry.scripts]
 corprep = 'corprep.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = "^1.12.1"
+hyfi = "^1.12.5"
 openai = "^0.27.8"
 backoff = "^2.2.1"
 scikit-learn = "^1.3.0"
 lexikanon = "^0.3.2"
 # lexikanon = { path = "../lexikanon", develop = true }
 # hyfi = { path = "../hyfi", develop = true }
-thematos = "^0.2.1"
+thematos = "^0.2.2"
+hyfi-absa = "^0.1.0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
```

### Comparing `corporate_reputation-0.9.1/src/corprep/absa/agent.py` & `corporate_reputation-0.9.2/src/corprep/absa/agent.py`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.9.1/src/corprep/absa/config.py` & `corporate_reputation-0.9.2/src/corprep/absa/config.py`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.9.1/src/corprep/conf/absa/prompts/default.yaml` & `corporate_reputation-0.9.2/src/corprep/conf/absa/prompts/default.yaml`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.9.1/src/corprep/datasets/io.py` & `corporate_reputation-0.9.2/src/corprep/datasets/io.py`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.9.1/src/corprep/datasets/similarity.py` & `corporate_reputation-0.9.2/src/corprep/datasets/similarity.py`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.9.1/PKG-INFO` & `corporate_reputation-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: corporate-reputation
-Version: 0.9.1
+Version: 0.9.2
 Summary: Unraveling Corporate and CEO Reputation using Aspect-Based Sentiment Analysis and Signal Modeling
 Home-page: https://entelecheia.github.io/corporate-reputation
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
-Requires-Dist: hyfi (>=1.12.1,<2.0.0)
+Requires-Dist: hyfi (>=1.12.5,<2.0.0)
+Requires-Dist: hyfi-absa (>=0.1.0,<0.2.0)
 Requires-Dist: lexikanon (>=0.3.2,<0.4.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: scikit-learn (>=1.3.0,<2.0.0)
-Requires-Dist: thematos (>=0.2.1,<0.3.0)
+Requires-Dist: thematos (>=0.2.2,<0.3.0)
 Project-URL: Repository, https://github.com/entelecheia/corporate-reputation
 Description-Content-Type: text/markdown
 
 # Reputation Analysis of Companies and CEOs
 
 [![pypi-image]][pypi-url]
 [![version-image]][release-url]
```

