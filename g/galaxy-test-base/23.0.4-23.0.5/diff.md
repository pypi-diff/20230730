# Comparing `tmp/galaxy-test-base-23.0.4.tar.gz` & `tmp/galaxy-test-base-23.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/test_base/dist/.tmp-m5odfdfo/galaxy-test-base-23.0.4.tar", last modified: Fri Jun 30 22:09:45 2023, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/test_base/dist/.tmp-f4fhde9x/galaxy-test-base-23.0.5.tar", last modified: Sun Jul 30 10:56:10 2023, max compression
```

## Comparing `galaxy-test-base-23.0.4.tar` & `galaxy-test-base-23.0.5.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:09:45.000000 galaxy-test-base-23.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-30 22:00:49.000000 galaxy-test-base-23.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-30 22:09:45.000000 galaxy-test-base-23.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:09:45.000000 galaxy-test-base-23.0.4/galaxy_test/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/galaxy_test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:09:45.000000 galaxy-test-base-23.0.4/galaxy_test/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/galaxy_test/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/galaxy_test/base/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/galaxy_test/base/api_asserts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/galaxy_test/base/api_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/galaxy_test/base/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:09:45.000000 galaxy-test-base-23.0.4/galaxy_test/base/data/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/galaxy_test/base/data/minimal_tool_no_id.json
--rw-r--r--   0 runner    (1001) docker     (123)    16151 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/galaxy_test/base/data/test_subworkflow_with_integer_input.ga
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/galaxy_test/base/data/test_workflow_1.ga
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/galaxy_test/base/data/test_workflow_2.ga
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/galaxy_test/base/data/test_workflow_batch.ga
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/galaxy_test/base/data/test_workflow_map_reduce_pause.ga
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/galaxy_test/base/data/test_workflow_matching_lists.ga
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/galaxy_test/base/data/test_workflow_missing_tool.ga
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/galaxy_test/base/data/test_workflow_pause.ga
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/galaxy_test/base/data/test_workflow_randomlines_legacy_params.ga
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/galaxy_test/base/data/test_workflow_randomlines_legacy_params_mixed_types.ga
--rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/galaxy_test/base/data/test_workflow_topoambigouity.ga
--rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/galaxy_test/base/data/test_workflow_topoambigouity_auto_laidout.ga
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/galaxy_test/base/data/test_workflow_two_random_lines.ga
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/galaxy_test/base/data/test_workflow_validation_1.ga
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/galaxy_test/base/data/test_workflow_with_input_tags.ga
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/galaxy_test/base/data/test_workflow_with_runtime_input.ga
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/galaxy_test/base/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/galaxy_test/base/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/galaxy_test/base/interactor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/galaxy_test/base/json_schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   125943 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/galaxy_test/base/populators.py
--rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/galaxy_test/base/rules_test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/galaxy_test/base/testcase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/galaxy_test/base/uses_shed_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/galaxy_test/base/workflow_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/galaxy_test/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:09:45.000000 galaxy-test-base-23.0.4/galaxy_test_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-30 22:09:45.000000 galaxy-test-base-23.0.4/galaxy_test_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-30 22:09:45.000000 galaxy-test-base-23.0.4/galaxy_test_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 22:09:45.000000 galaxy-test-base-23.0.4/galaxy_test_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-30 22:09:45.000000 galaxy-test-base-23.0.4/galaxy_test_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-30 22:09:45.000000 galaxy-test-base-23.0.4/galaxy_test_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-30 22:09:45.000000 galaxy-test-base-23.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 22:00:50.000000 galaxy-test-base-23.0.4/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:56:10.000000 galaxy-test-base-23.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-07-30 10:47:07.000000 galaxy-test-base-23.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-30 10:56:10.000000 galaxy-test-base-23.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:56:10.000000 galaxy-test-base-23.0.5/galaxy_test/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/galaxy_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:56:10.000000 galaxy-test-base-23.0.5/galaxy_test/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/galaxy_test/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/galaxy_test/base/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/galaxy_test/base/api_asserts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/galaxy_test/base/api_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/galaxy_test/base/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:56:10.000000 galaxy-test-base-23.0.5/galaxy_test/base/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/galaxy_test/base/data/minimal_tool_no_id.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16151 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/galaxy_test/base/data/test_subworkflow_with_integer_input.ga
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/galaxy_test/base/data/test_workflow_1.ga
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/galaxy_test/base/data/test_workflow_2.ga
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/galaxy_test/base/data/test_workflow_batch.ga
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/galaxy_test/base/data/test_workflow_map_reduce_pause.ga
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/galaxy_test/base/data/test_workflow_matching_lists.ga
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/galaxy_test/base/data/test_workflow_missing_tool.ga
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/galaxy_test/base/data/test_workflow_pause.ga
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/galaxy_test/base/data/test_workflow_randomlines_legacy_params.ga
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/galaxy_test/base/data/test_workflow_randomlines_legacy_params_mixed_types.ga
+-rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/galaxy_test/base/data/test_workflow_topoambigouity.ga
+-rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/galaxy_test/base/data/test_workflow_topoambigouity_auto_laidout.ga
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/galaxy_test/base/data/test_workflow_two_random_lines.ga
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/galaxy_test/base/data/test_workflow_validation_1.ga
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/galaxy_test/base/data/test_workflow_with_input_tags.ga
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/galaxy_test/base/data/test_workflow_with_runtime_input.ga
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/galaxy_test/base/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/galaxy_test/base/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/galaxy_test/base/interactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/galaxy_test/base/json_schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125943 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/galaxy_test/base/populators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/galaxy_test/base/rules_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/galaxy_test/base/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/galaxy_test/base/uses_shed_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/galaxy_test/base/workflow_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/galaxy_test/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:56:10.000000 galaxy-test-base-23.0.5/galaxy_test_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-30 10:56:10.000000 galaxy-test-base-23.0.5/galaxy_test_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-30 10:56:10.000000 galaxy-test-base-23.0.5/galaxy_test_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 10:56:10.000000 galaxy-test-base-23.0.5/galaxy_test_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-30 10:56:10.000000 galaxy-test-base-23.0.5/galaxy_test_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-30 10:56:10.000000 galaxy-test-base-23.0.5/galaxy_test_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-30 10:56:10.000000 galaxy-test-base-23.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-30 10:47:08.000000 galaxy-test-base-23.0.5/test-requirements.txt
```

### Comparing `galaxy-test-base-23.0.4/HISTORY.rst` & `galaxy-test-base-23.0.5/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.5 (2023-07-29)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 23.0.4 (2023-06-30)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.3 (2023-06-26)
```

### Comparing `galaxy-test-base-23.0.4/LICENSE` & `galaxy-test-base-23.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.0.4/PKG-INFO` & `galaxy-test-base-23.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-test-base
-Version: 23.0.4
+Version: 23.0.5
 Summary: Galaxy testing utilities
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -43,14 +43,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.5 (2023-07-29)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 23.0.4 (2023-06-30)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.3 (2023-06-26)
```

### Comparing `galaxy-test-base-23.0.4/galaxy_test/base/api.py` & `galaxy-test-base-23.0.5/galaxy_test/base/api.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.0.4/galaxy_test/base/api_asserts.py` & `galaxy-test-base-23.0.5/galaxy_test/base/api_asserts.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.0.4/galaxy_test/base/api_util.py` & `galaxy-test-base-23.0.5/galaxy_test/base/api_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.0.4/galaxy_test/base/data/test_subworkflow_with_integer_input.ga` & `galaxy-test-base-23.0.5/galaxy_test/base/data/test_subworkflow_with_integer_input.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.0.4/galaxy_test/base/data/test_workflow_1.ga` & `galaxy-test-base-23.0.5/galaxy_test/base/data/test_workflow_1.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.0.4/galaxy_test/base/data/test_workflow_2.ga` & `galaxy-test-base-23.0.5/galaxy_test/base/data/test_workflow_2.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.0.4/galaxy_test/base/data/test_workflow_batch.ga` & `galaxy-test-base-23.0.5/galaxy_test/base/data/test_workflow_batch.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.0.4/galaxy_test/base/data/test_workflow_map_reduce_pause.ga` & `galaxy-test-base-23.0.5/galaxy_test/base/data/test_workflow_map_reduce_pause.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.0.4/galaxy_test/base/data/test_workflow_matching_lists.ga` & `galaxy-test-base-23.0.5/galaxy_test/base/data/test_workflow_matching_lists.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.0.4/galaxy_test/base/data/test_workflow_missing_tool.ga` & `galaxy-test-base-23.0.5/galaxy_test/base/data/test_workflow_missing_tool.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.0.4/galaxy_test/base/data/test_workflow_pause.ga` & `galaxy-test-base-23.0.5/galaxy_test/base/data/test_workflow_pause.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.0.4/galaxy_test/base/data/test_workflow_randomlines_legacy_params.ga` & `galaxy-test-base-23.0.5/galaxy_test/base/data/test_workflow_randomlines_legacy_params.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.0.4/galaxy_test/base/data/test_workflow_randomlines_legacy_params_mixed_types.ga` & `galaxy-test-base-23.0.5/galaxy_test/base/data/test_workflow_randomlines_legacy_params_mixed_types.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.0.4/galaxy_test/base/data/test_workflow_topoambigouity.ga` & `galaxy-test-base-23.0.5/galaxy_test/base/data/test_workflow_topoambigouity.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.0.4/galaxy_test/base/data/test_workflow_topoambigouity_auto_laidout.ga` & `galaxy-test-base-23.0.5/galaxy_test/base/data/test_workflow_topoambigouity_auto_laidout.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.0.4/galaxy_test/base/data/test_workflow_two_random_lines.ga` & `galaxy-test-base-23.0.5/galaxy_test/base/data/test_workflow_two_random_lines.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.0.4/galaxy_test/base/data/test_workflow_validation_1.ga` & `galaxy-test-base-23.0.5/galaxy_test/base/data/test_workflow_validation_1.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.0.4/galaxy_test/base/data/test_workflow_with_input_tags.ga` & `galaxy-test-base-23.0.5/galaxy_test/base/data/test_workflow_with_input_tags.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.0.4/galaxy_test/base/data/test_workflow_with_runtime_input.ga` & `galaxy-test-base-23.0.5/galaxy_test/base/data/test_workflow_with_runtime_input.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.0.4/galaxy_test/base/decorators.py` & `galaxy-test-base-23.0.5/galaxy_test/base/decorators.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.0.4/galaxy_test/base/env.py` & `galaxy-test-base-23.0.5/galaxy_test/base/env.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.0.4/galaxy_test/base/interactor.py` & `galaxy-test-base-23.0.5/galaxy_test/base/interactor.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.0.4/galaxy_test/base/json_schema_utils.py` & `galaxy-test-base-23.0.5/galaxy_test/base/json_schema_utils.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.0.4/galaxy_test/base/populators.py` & `galaxy-test-base-23.0.5/galaxy_test/base/populators.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.0.4/galaxy_test/base/rules_test_data.py` & `galaxy-test-base-23.0.5/galaxy_test/base/rules_test_data.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.0.4/galaxy_test/base/testcase.py` & `galaxy-test-base-23.0.5/galaxy_test/base/testcase.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.0.4/galaxy_test/base/uses_shed_api.py` & `galaxy-test-base-23.0.5/galaxy_test/base/uses_shed_api.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.0.4/galaxy_test/base/workflow_fixtures.py` & `galaxy-test-base-23.0.5/galaxy_test/base/workflow_fixtures.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.0.4/galaxy_test_base.egg-info/PKG-INFO` & `galaxy-test-base-23.0.5/galaxy_test_base.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-test-base
-Version: 23.0.4
+Version: 23.0.5
 Summary: Galaxy testing utilities
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -43,14 +43,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.5 (2023-07-29)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 23.0.4 (2023-06-30)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.3 (2023-06-26)
```

### Comparing `galaxy-test-base-23.0.4/galaxy_test_base.egg-info/SOURCES.txt` & `galaxy-test-base-23.0.5/galaxy_test_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-23.0.4/setup.cfg` & `galaxy-test-base-23.0.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-test-base
 url = https://github.com/galaxyproject/galaxy
-version = 23.0.4
+version = 23.0.5
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-tool-util
 	galaxy-util
 	bioblend
```

