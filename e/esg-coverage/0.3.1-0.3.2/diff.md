# Comparing `tmp/esg_coverage-0.3.1.tar.gz` & `tmp/esg_coverage-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esg_coverage-0.3.1.tar", max compression
+gzip compressed data, was "esg_coverage-0.3.2.tar", max compression
```

## Comparing `esg_coverage-0.3.1.tar` & `esg_coverage-0.3.2.tar`

### file list

```diff
@@ -1,65 +1,21 @@
--rw-r--r--   0        0        0     1071 2023-07-04 07:33:40.418196 esg_coverage-0.3.1/LICENSE
--rw-r--r--   0        0        0     2873 2023-07-04 07:33:40.418196 esg_coverage-0.3.1/README.md
--rw-r--r--   0        0        0     2995 2023-07-04 07:34:04.246021 esg_coverage-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      287 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/__cli__.py
--rw-r--r--   0        0        0      379 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/__init__.py
--rw-r--r--   0        0        0       22 2023-07-04 07:34:04.206021 esg_coverage-0.3.1/src/esgcov/_version.py
--rw-r--r--   0        0        0        0 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/__init__.py
--rw-r--r--   0        0        0      288 2023-07-04 07:34:04.206021 esg_coverage-0.3.1/src/esgcov/conf/about/__init__.yaml
--rw-r--r--   0        0        0      427 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/batch/__init__.yaml
--rw-r--r--   0        0        0        0 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/cmd/__init__.yaml
--rw-r--r--   0        0        0       49 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/cmd/about.yaml
--rw-r--r--   0        0        0      155 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0      167 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/cmd/cpcfg.yaml
--rw-r--r--   0        0        0       83 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0       91 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/cmd/run_workflow.yaml
--rw-r--r--   0        0        0      320 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/config.yaml
--rw-r--r--   0        0        0      569 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/copier/conf.yaml
--rw-r--r--   0        0        0      709 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      319 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      137 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      217 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/mode/__debug__.yaml
--rw-r--r--   0        0        0      921 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/mode/debug.yaml
--rw-r--r--   0        0        0       61 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/module/__init__.yaml
--rw-r--r--   0        0        0       73 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/path/__default__.yaml
--rw-r--r--   0        0        0      785 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/path/__init__.yaml
--rw-r--r--   0        0        0      133 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/path/__task__.yaml
--rw-r--r--   0        0        0      166 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/path/dirnames/__init__.yaml
--rw-r--r--   0        0        0       76 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipe/__dataframe__.yaml
--rw-r--r--   0        0        0       77 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipe/__dataframe_external_funcs__.yaml
--rw-r--r--   0        0        0       79 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipe/__dataframe_instance_methods__.yaml
--rw-r--r--   0        0        0       85 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipe/__external__.yaml
--rw-r--r--   0        0        0       70 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipe/__general_external_funcs__.yaml
--rw-r--r--   0        0        0       72 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipe/__general_instance_methods__.yaml
--rw-r--r--   0        0        0      128 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipe/__init__.yaml
--rw-r--r--   0        0        0       51 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipe/__instance__.yaml
--rw-r--r--   0        0        0       49 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipe/__lambda__.yaml
--rw-r--r--   0        0        0      236 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipe/load_dataframes.yaml
--rw-r--r--   0        0        0      108 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipe/preprocessing_esg_coverage.yaml
--rw-r--r--   0        0        0      107 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipe/preprocessing_esg_ratings.yaml
--rw-r--r--   0        0        0      241 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipe/save_dataframes.yaml
--rw-r--r--   0        0        0       90 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipe/test_preprocessing.yaml
--rw-r--r--   0        0        0       69 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipeline/__init__.yaml
--rw-r--r--   0        0        0      388 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipeline/__test__.yaml
--rw-r--r--   0        0        0      388 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipeline/__test_dataframe__.yaml
--rw-r--r--   0        0        0      268 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipeline/__test_general__.yaml
--rw-r--r--   0        0        0      706 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/pipeline/dataset_preprocessing.yaml
--rw-r--r--   0        0        0      744 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/project/__init__.yaml
--rw-r--r--   0        0        0      170 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/project/__test__.yaml
--rw-r--r--   0        0        0      200 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/project/esgcov.yaml
--rw-r--r--   0        0        0       38 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/running/__init__.yaml
--rw-r--r--   0        0        0      178 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      351 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/task/__init__.yaml
--rw-r--r--   0        0        0      395 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/task/__test__.yaml
--rw-r--r--   0        0        0      324 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/task/datasets.yaml
--rw-r--r--   0        0        0       99 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/workflow/__init__.yaml
--rw-r--r--   0        0        0       99 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/workflow/__test__.yaml
--rw-r--r--   0        0        0       97 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/conf/workflow/datasets.yaml
--rw-r--r--   0        0        0        0 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/datasets/__init__.py
--rw-r--r--   0        0        0     3421 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/datasets/preprocessing.py
--rw-r--r--   0        0        0        0 2023-07-04 07:33:40.422196 esg_coverage-0.3.1/src/esgcov/py.typed
--rw-r--r--   0        0        0     3610 1970-01-01 00:00:00.000000 esg_coverage-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-30 19:17:21.381898 esg_coverage-0.3.2/LICENSE
+-rw-r--r--   0        0        0     2873 2023-07-30 19:17:21.381898 esg_coverage-0.3.2/README.md
+-rw-r--r--   0        0        0     2863 2023-07-30 19:17:51.767458 esg_coverage-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      181 2023-07-30 19:17:21.385899 esg_coverage-0.3.2/src/esgcov/__cli__.py
+-rw-r--r--   0        0        0      473 2023-07-30 19:17:21.385899 esg_coverage-0.3.2/src/esgcov/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-30 19:17:21.385899 esg_coverage-0.3.2/src/esgcov/_version.py
+-rw-r--r--   0        0        0        0 2023-07-30 19:17:21.385899 esg_coverage-0.3.2/src/esgcov/conf/__init__.py
+-rw-r--r--   0        0        0      244 2023-07-30 19:17:21.385899 esg_coverage-0.3.2/src/esgcov/conf/about/esgcov.yaml
+-rw-r--r--   0        0        0      238 2023-07-30 19:17:21.385899 esg_coverage-0.3.2/src/esgcov/conf/pipe/load_dataframes.yaml
+-rw-r--r--   0        0        0      118 2023-07-30 19:17:21.385899 esg_coverage-0.3.2/src/esgcov/conf/pipe/preprocessing_esg_coverage.yaml
+-rw-r--r--   0        0        0      117 2023-07-30 19:17:21.385899 esg_coverage-0.3.2/src/esgcov/conf/pipe/preprocessing_esg_ratings.yaml
+-rw-r--r--   0        0        0      243 2023-07-30 19:17:21.385899 esg_coverage-0.3.2/src/esgcov/conf/pipe/save_dataframes.yaml
+-rw-r--r--   0        0        0      102 2023-07-30 19:17:21.385899 esg_coverage-0.3.2/src/esgcov/conf/pipe/test_preprocessing.yaml
+-rw-r--r--   0        0        0      706 2023-07-30 19:17:21.385899 esg_coverage-0.3.2/src/esgcov/conf/pipeline/dataset_preprocessing.yaml
+-rw-r--r--   0        0        0      200 2023-07-30 19:17:21.385899 esg_coverage-0.3.2/src/esgcov/conf/project/esgcov.yaml
+-rw-r--r--   0        0        0      118 2023-07-30 19:17:21.385899 esg_coverage-0.3.2/src/esgcov/conf/task/datasets.yaml
+-rw-r--r--   0        0        0      139 2023-07-30 19:17:21.385899 esg_coverage-0.3.2/src/esgcov/conf/workflow/datasets.yaml
+-rw-r--r--   0        0        0        0 2023-07-30 19:17:21.385899 esg_coverage-0.3.2/src/esgcov/datasets/__init__.py
+-rw-r--r--   0        0        0     3421 2023-07-30 19:17:21.385899 esg_coverage-0.3.2/src/esgcov/datasets/preprocessing.py
+-rw-r--r--   0        0        0        0 2023-07-30 19:17:21.385899 esg_coverage-0.3.2/src/esgcov/py.typed
+-rw-r--r--   0        0        0     3611 1970-01-01 00:00:00.000000 esg_coverage-0.3.2/PKG-INFO
```

### Comparing `esg_coverage-0.3.1/LICENSE` & `esg_coverage-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `esg_coverage-0.3.1/README.md` & `esg_coverage-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `esg_coverage-0.3.1/pyproject.toml` & `esg_coverage-0.3.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "esg-coverage"
-version = "0.3.1"
+version = "0.3.2"
 description = "The Role of Analyst Coverage in Translating ESG Ratings into Stock Performance"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://esg-coverage.entelecheia.ai"
 repository = "https://github.com/entelecheia/esg-coverage"
 readme = "README.md"
 packages = [{ include = "esgcov", from = "src" }]
 
 [tool.poetry.scripts]
 esgcov = 'esgcov.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = "^1.0.2"
+hyfi = "^1.12.5"
 tabulate = "^0.9.0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
@@ -82,16 +82,14 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
 tag_format = "v$version"
 
 [tool.semantic_release]
 branch = "main"
 version_toml = "pyproject.toml:tool.poetry.version"
-version_variable = "src/esgcov/_version.py:__version__"
-version_pattern = 'src/esgcov/conf/about/__init__.yaml:version: "{version}"'
 version_source = "tag"
 commit_version_number = true # required for version_source = "tag"
 commit_subject = "chore(release): :rocket: {version} [skip ci]"
 prerelease_tag = "rc"
 major_on_zero = true
 tag_commit = true
 changelog_file = "CHANGELOG.md"
```

### Comparing `esg_coverage-0.3.1/src/esgcov/conf/pipeline/dataset_preprocessing.yaml` & `esg_coverage-0.3.2/src/esgcov/conf/pipeline/dataset_preprocessing.yaml`

 * *Files identical despite different names*

### Comparing `esg_coverage-0.3.1/src/esgcov/datasets/preprocessing.py` & `esg_coverage-0.3.2/src/esgcov/datasets/preprocessing.py`

 * *Files identical despite different names*

### Comparing `esg_coverage-0.3.1/PKG-INFO` & `esg_coverage-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: esg-coverage
-Version: 0.3.1
+Version: 0.3.2
 Summary: The Role of Analyst Coverage in Translating ESG Ratings into Stock Performance
 Home-page: https://esg-coverage.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: hyfi (>=1.0.2,<2.0.0)
+Requires-Dist: hyfi (>=1.12.5,<2.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/entelecheia/esg-coverage
 Description-Content-Type: text/markdown
 
 # The Analyst Pathway in ESG
 
 [![pypi-image]][pypi-url]
```

