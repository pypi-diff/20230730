# Comparing `tmp/yetl-framework-2.0.3.tar.gz` & `tmp/yetl-framework-2.0.4.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetl-framework-2.0.3.tar", last modified: Fri Jul 28 09:07:09 2023, max compression
+gzip compressed data, was "yetl-framework-2.0.4.dev1.tar", last modified: Sun Jul 30 09:59:34 2023, max compression
```

## Comparing `yetl-framework-2.0.3.tar` & `yetl-framework-2.0.4.dev1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 09:07:09.040490 yetl-framework-2.0.3/
--rw-r--r--   0 vsts      (1001) docker     (123)     1194 2023-07-28 09:07:09.040490 yetl-framework-2.0.3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      596 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-07-28 09:07:09.040490 yetl-framework-2.0.3/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1539 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 09:07:09.020490 yetl-framework-2.0.3/yetl/
--rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1764 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 09:07:09.024490 yetl-framework-2.0.3/yetl/cli/
--rw-r--r--   0 vsts      (1001) docker     (123)     3367 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/cli/_init.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 09:07:09.024490 yetl-framework-2.0.3/yetl/cli/metadata_provider/
--rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/cli/metadata_provider/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    17399 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/cli/metadata_provider/_xlsx.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 09:07:09.028490 yetl-framework-2.0.3/yetl/config/
--rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5112 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/config/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2195 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/config/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/config/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/config/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1309 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/config/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/config/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/config/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10188 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/config/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/config/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5064 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/config/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    17661 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/config/deltalake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 09:07:09.032490 yetl-framework-2.0.3/yetl/config/table/
--rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/config/table/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5139 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/config/table/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/config/table/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6707 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/config/table/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4832 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/config/table/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/config/table/_table_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/config/table/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 09:07:09.036491 yetl-framework-2.0.3/yetl/resource/
--rw-r--r--   0 vsts      (1001) docker     (123)      569 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/resource/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      299 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/resource/logging.yaml
--rw-r--r--   0 vsts      (1001) docker     (123)      500 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/resource/project.yaml
--rw-r--r--   0 vsts      (1001) docker     (123)    12636 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/resource/sibytes_yetl_pipeline_schema.json
--rw-r--r--   0 vsts      (1001) docker     (123)     2654 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/resource/sibytes_yetl_project_schema.json
--rw-r--r--   0 vsts      (1001) docker     (123)    14625 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/resource/sibytes_yetl_tables_schema.json
--rw-r--r--   0 vsts      (1001) docker     (123)    10012 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/resource/tables.xlsx
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 09:07:09.036491 yetl-framework-2.0.3/yetl/validation/
--rw-r--r--   0 vsts      (1001) docker     (123)      353 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/validation/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1495 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/validation/_validate.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 09:07:09.040490 yetl-framework-2.0.3/yetl/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      167 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1312 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/workflow/_dlt.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-07-28 09:05:49.000000 yetl-framework-2.0.3/yetl/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-28 09:07:09.040490 yetl-framework-2.0.3/yetl_framework.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     1194 2023-07-28 09:07:08.000000 yetl-framework-2.0.3/yetl_framework.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1377 2023-07-28 09:07:08.000000 yetl-framework-2.0.3/yetl_framework.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-28 09:07:08.000000 yetl-framework-2.0.3/yetl_framework.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-28 09:07:08.000000 yetl-framework-2.0.3/yetl_framework.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       76 2023-07-28 09:07:08.000000 yetl-framework-2.0.3/yetl_framework.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-07-28 09:07:08.000000 yetl-framework-2.0.3/yetl_framework.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-30 09:59:34.452789 yetl-framework-2.0.4.dev1/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1199 2023-07-30 09:59:34.452789 yetl-framework-2.0.4.dev1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      596 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-07-30 09:59:34.452789 yetl-framework-2.0.4.dev1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1544 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-30 09:59:34.444789 yetl-framework-2.0.4.dev1/yetl/
+-rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1764 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-30 09:59:34.444789 yetl-framework-2.0.4.dev1/yetl/cli/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3367 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/cli/_init.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-30 09:59:34.444789 yetl-framework-2.0.4.dev1/yetl/cli/metadata_provider/
+-rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/cli/metadata_provider/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17399 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/cli/metadata_provider/_xlsx.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-30 09:59:34.444789 yetl-framework-2.0.4.dev1/yetl/config/
+-rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4866 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/config/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2159 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/config/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/config/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/config/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1309 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/config/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/config/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/config/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9862 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/config/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/config/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5099 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/config/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17896 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/config/deltalake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-30 09:59:34.444789 yetl-framework-2.0.4.dev1/yetl/config/table/
+-rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/config/table/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5056 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/config/table/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/config/table/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6707 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/config/table/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4560 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/config/table/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/config/table/_table_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/config/table/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-30 09:59:34.448789 yetl-framework-2.0.4.dev1/yetl/resource/
+-rw-r--r--   0 vsts      (1001) docker     (123)      569 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/resource/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      299 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/resource/logging.yaml
+-rw-r--r--   0 vsts      (1001) docker     (123)      500 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/resource/project.yaml
+-rw-r--r--   0 vsts      (1001) docker     (123)    12636 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/resource/sibytes_yetl_pipeline_schema.json
+-rw-r--r--   0 vsts      (1001) docker     (123)     2654 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/resource/sibytes_yetl_project_schema.json
+-rw-r--r--   0 vsts      (1001) docker     (123)    14625 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/resource/sibytes_yetl_tables_schema.json
+-rw-r--r--   0 vsts      (1001) docker     (123)    10012 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/resource/tables.xlsx
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-30 09:59:34.448789 yetl-framework-2.0.4.dev1/yetl/validation/
+-rw-r--r--   0 vsts      (1001) docker     (123)      353 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/validation/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1495 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/validation/_validate.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-30 09:59:34.448789 yetl-framework-2.0.4.dev1/yetl/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      167 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1312 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/workflow/_dlt.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-07-30 09:58:27.000000 yetl-framework-2.0.4.dev1/yetl/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-30 09:59:34.452789 yetl-framework-2.0.4.dev1/yetl_framework.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1199 2023-07-30 09:59:34.000000 yetl-framework-2.0.4.dev1/yetl_framework.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1377 2023-07-30 09:59:34.000000 yetl-framework-2.0.4.dev1/yetl_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-30 09:59:34.000000 yetl-framework-2.0.4.dev1/yetl_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-30 09:59:34.000000 yetl-framework-2.0.4.dev1/yetl_framework.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       76 2023-07-30 09:59:34.000000 yetl-framework-2.0.4.dev1/yetl_framework.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-07-30 09:59:34.000000 yetl-framework-2.0.4.dev1/yetl_framework.egg-info/top_level.txt
```

### Comparing `yetl-framework-2.0.3/PKG-INFO` & `yetl-framework-2.0.4.dev1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 2.0.3
+Version: 2.0.4.dev1
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-2.0.3/README.md` & `yetl-framework-2.0.4.dev1/README.md`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.3/setup.py` & `yetl-framework-2.0.4.dev1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="yetl-framework",
-    version="2.0.3",
+    version="2.0.4.dev1",
     description="yet (another spark) etl framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://www.yetl.io/",
     project_urls={
         "GitHub": "https://github.com/sibytes/yetl",
         "Documentation": "https://www.yetl.io/",
```

### Comparing `yetl-framework-2.0.3/yetl/__main__.py` & `yetl-framework-2.0.4.dev1/yetl/__main__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.3/yetl/cli/_init.py` & `yetl-framework-2.0.4.dev1/yetl/cli/_init.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.3/yetl/cli/metadata_provider/_xlsx.py` & `yetl-framework-2.0.4.dev1/yetl/cli/metadata_provider/_xlsx.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.3/yetl/config/__init__.py` & `yetl-framework-2.0.4.dev1/yetl/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.3/yetl/config/_config.py` & `yetl-framework-2.0.4.dev1/yetl/config/_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 import os
 from .table import Table
 from ._timeslice import Timeslice
 from ._tables import Tables, _INDEX_WILDCARD, KeyContants
 from ._stage_type import StageType
-from ._utils import abs_config_path, load_yaml, get_config_path, check_version
+from ._utils import (
+    abs_config_path,
+    load_yaml,
+    get_config_path,
+    check_version,
+    DEFAULT_CATALOG,
+)
 from ._logging_config import configure_logging
 import logging
 from ._project import Project
 from ..validation import validate_tables, validate_pipeline
 from typing import Union
 
 
@@ -63,64 +69,58 @@
         tables = Tables(table_data=tables_config)
         return tables
 
     def create_tables(
         self,
         stage: Union[StageType, str] = _INDEX_WILDCARD,
         database=_INDEX_WILDCARD,
-        catalog: str = None,
-        catalog_enabled: bool = True,
+        catalog: str = DEFAULT_CATALOG,
         **kwargs,
     ):
         return self.tables.create_table(
             stage=stage,
             database=database,
             first_match=False,
             catalog=catalog,
-            catalog_enabled=catalog_enabled,
             **kwargs,
         )
 
     def create_table(
         self,
         stage: Union[StageType, str] = _INDEX_WILDCARD,
         database=_INDEX_WILDCARD,
         table=_INDEX_WILDCARD,
-        catalog: str = None,
-        catalog_enabled: bool = True,
+        catalog: str = DEFAULT_CATALOG,
         **kwargs,
     ):
         return self.tables.create_table(
             stage=stage,
             database=database,
             table=table,
             first_match=True,
             catalog=catalog,
-            catalog_enabled=catalog_enabled,
             **kwargs,
         )
 
     def get_table_mapping(
         self,
         stage: StageType,
         database: str = _INDEX_WILDCARD,
         table: str = _INDEX_WILDCARD,
         create_database: bool = True,
         create_table: bool = True,
-        catalog: str = None,
-        catalog_enabled: bool = True,
+        catalog: str = DEFAULT_CATALOG,
     ):
         table_mapping = self.tables.get_table_mapping(
             stage=stage,
             table=table,
             database=database,
             create_database=create_database,
             create_table=create_table,
             catalog=catalog,
-            catalog_enabled=catalog_enabled,
         )
 
         return table_mapping
 
     def set_checkpoint(
         self,
         source: Table,
@@ -139,22 +139,20 @@
         self,
         stage: Union[StageType, str] = _INDEX_WILDCARD,
         database=_INDEX_WILDCARD,
         table=_INDEX_WILDCARD,
         first_match: bool = True,
         create_database: bool = False,
         create_table: bool = False,
-        catalog: str = None,
-        catalog_enabled: bool = True,
+        catalog: str = DEFAULT_CATALOG,
         **kwargs,
     ):
         return self.tables.lookup_table(
             stage=stage,
             database=database,
             table=table,
             first_match=first_match,
             create_database=create_database,
             create_table=create_table,
             catalog=catalog,
-            catalog_enabled=catalog_enabled,
             **kwargs,
         )
```

### Comparing `yetl-framework-2.0.3/yetl/config/_decorators.py` & `yetl-framework-2.0.4.dev1/yetl/config/_decorators.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # implicit, not referenced - must be the 1st import
 from ._logging_config import configure_logging
 import logging
 from ._config import Config
 from ._timeslice import Timeslice
 from ._stage_type import StageType
 from .table import Table
+from ._utils import DEFAULT_CATALOG
 
 
 def yetl_flow(
     stage: StageType,
     project: str,
     pipeline: str = None,
     config_path: str = None,
-    catalog: str = None,
-    catalog_enabled: bool = True,
+    catalog: str = DEFAULT_CATALOG,
 ):
     def decorate(function):
         def wrap_function(*args, **kwargs):
             configure_logging(project)
             _logger = logging.getLogger(__name__)
 
             _pipeline = pipeline
@@ -42,15 +42,14 @@
                 config_path=config_path,
                 timeslice=timeslice,
             )
             table_mapping = config.get_table_mapping(
                 stage=stage,
                 table=table,
                 catalog=catalog,
-                catalog_enabled=catalog_enabled,
             )
 
             destination: Table = table_mapping.destination
             sources = table_mapping.source
             if isinstance(sources, dict):
                 for _, source in sources.items():
                     config.set_checkpoint(source=source, destination=destination)
```

### Comparing `yetl-framework-2.0.3/yetl/config/_logging_config.py` & `yetl-framework-2.0.4.dev1/yetl/config/_logging_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.3/yetl/config/_project.py` & `yetl-framework-2.0.4.dev1/yetl/config/_project.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.3/yetl/config/_spark_context.py` & `yetl-framework-2.0.4.dev1/yetl/config/_spark_context.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.3/yetl/config/_tables.py` & `yetl-framework-2.0.4.dev1/yetl/config/_tables.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Union, Any, Dict, List, Optional
 from ._stage_type import StageType
 import fnmatch
 from ._table_mapping import TableMapping
 from .table import TableType
 from .table import table_factory
 from .table import Table
+from ._utils import DEFAULT_CATALOG
 from enum import Enum
 import logging
 
 _INDEX_WILDCARD = "*"
 
 
 class KeyContants(Enum):
@@ -135,40 +136,37 @@
 
     def create_table(
         self,
         stage: Union[StageType, str] = _INDEX_WILDCARD,
         database=_INDEX_WILDCARD,
         table=_INDEX_WILDCARD,
         first_match: bool = True,
-        catalog: str = None,
-        catalog_enabled: bool = True,
+        catalog: str = DEFAULT_CATALOG,
         **kwargs,
     ):
         return self.lookup_table(
             stage=stage,
             database=database,
             table=table,
             first_match=first_match,
             create_database=True,
             create_table=True,
             catalog=catalog,
-            catalog_enabled=catalog_enabled,
             **kwargs,
         )
 
     def lookup_table(
         self,
         stage: Union[StageType, str] = _INDEX_WILDCARD,
         database=_INDEX_WILDCARD,
         table=_INDEX_WILDCARD,
         first_match: bool = True,
         create_database: bool = False,
         create_table: bool = False,
-        catalog: str = None,
-        catalog_enabled: bool = True,
+        catalog: str = DEFAULT_CATALOG,
         **kwargs,
     ):
         index = Tables.get_index(stage, database, table)
         matches = fnmatch.filter(list(self.tables_index.keys()), index)
 
         if not matches:
             raise Exception(f"index {index} not found in tables_index")
@@ -200,53 +198,49 @@
 
         if first_match:
             matches = matches[0]
             table = tables_index[matches]
             msg_tables = f"{table.database}.{table.table}"
             self._logger.info(f"Matched tables: {msg_tables}")
             if create_database:
-                table.create_database(catalog=catalog, catalog_enabled=catalog_enabled)
+                table.create_database(catalog=catalog)
             if create_table:
-                table.create_table(catalog=catalog, catalog_enabled=catalog_enabled)
+                table.create_table(catalog=catalog)
             return table
         else:
             tables = [tables_index[i] for i in matches]
             msg_tables = "\n".join([f"{t.database}.{t.table}" for t in tables])
             self._logger.info(f"Matched tables: {msg_tables}")
             db = ""
             if create_table or create_database:
                 for t in tables:
                     if create_database and db != t.database:
                         db = t.database
-                        t.create_database(
-                            catalog=catalog, catalog_enabled=catalog_enabled
-                        )
+                        t.create_database(catalog=catalog)
                     if create_table:
-                        t.create_table()
+                        t.create_table(catalog=catalog)
             return tables
 
     def get_table_mapping(
         self,
         stage: StageType,
         table=_INDEX_WILDCARD,
         database=_INDEX_WILDCARD,
         create_database: bool = True,
         create_table: bool = True,
-        catalog: str = None,
-        catalog_enabled: bool = True,
+        catalog: str = DEFAULT_CATALOG,
     ):
         destination = self.lookup_table(
             stage=stage,
             database=database,
             table=table,
             first_match=True,
             create_database=create_database,
             create_table=create_table,
             catalog=catalog,
-            catalog_enabled=catalog_enabled,
         )
         source = {}
 
         tables = []
         try:
             for index in destination.depends_on:
                 do_stage, do_database, do_table = Tables.parse_index(index)
@@ -254,15 +248,14 @@
                     stage=do_stage,
                     table=do_table,
                     database=do_database,
                     first_match=False,
                     create_database=create_database,
                     create_table=create_table,
                     catalog=catalog,
-                    catalog_enabled=catalog_enabled,
                 )
         except Exception as e:
             raise Exception(f"Error looking up dependencies for table {table}") from e
 
         for tbl in tables:
             source[tbl.table] = tbl
```

### Comparing `yetl-framework-2.0.3/yetl/config/_timeslice.py` & `yetl-framework-2.0.4.dev1/yetl/config/_timeslice.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.3/yetl/config/_utils.py` & `yetl-framework-2.0.4.dev1/yetl/config/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import logging
 
 
 YETL_CONFIG = "YETL_CONFIG"
 _ENCODING = "utf-8"
 _DBX_WORKSPACE_PATH = "/Workspace"
 _DBX_REPO_PATH = "/Workspace/Repos"
+DEFAULT_CATALOG = "hive_metastore"
 
 
 class VersionNotFoundException(Exception):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
```

### Comparing `yetl-framework-2.0.3/yetl/config/deltalake.py` & `yetl-framework-2.0.4.dev1/yetl/config/deltalake.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pyspark.sql.types import StructType, StructField
 import jinja2
 from typing import List, Union, Dict, Optional
 from ._spark_context import get_spark_context
 from pydantic import BaseModel, Field, PrivateAttr
 from typing import Any
 from ._project import Project
+from ._utils import DEFAULT_CATALOG
 from pyspark.sql import SparkSession
 import re
 
 
 class DeltaLakeFn(BaseModel):
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
@@ -205,15 +206,15 @@
             p = f"`{k}` in ({','.join(v)})"
             predicates.append(p)
 
         predicate = " and ".join(predicates)
 
         return predicate
 
-    def table_exists(self, database: str, table: str, catalog: str = None):
+    def table_exists(self, database: str, table: str, catalog: str = DEFAULT_CATALOG):
         database = f"`{catalog}`.`{database}`" if catalog else f"`{database}`"
         _table_exists = (
             self.spark.sql(f"SHOW TABLES in {database};")
             .where(f"tableName='{table}' AND !isTemporary")
             .count()
             == 1
         )
@@ -231,15 +232,15 @@
     def create_table(
         self,
         database: str,
         table: str,
         path: str = None,
         delta_properties: List[str] = None,
         sql: str = None,
-        catalog: str = None,
+        catalog: str = DEFAULT_CATALOG,
     ):
         database = f"`{catalog}`.`{database}`" if catalog else f"`{database}`"
         table = f"`{table}`"
         self._logger.info(f"Creating table if not exists {database}.{table} at {path}")
         if not sql:
             sql = f"CREATE TABLE IF NOT EXISTS {database}.{table}"
 
@@ -256,41 +257,52 @@
                 sql = f"{sql}\n{sql_path}\n{sql_properties};"
 
         self._logger.info(f"{sql}")
         self.spark.sql(sql)
 
         return sql
 
-    def create_database(self, database: str, catalog: str = None):
+    def create_database(
+        self,
+        database: str,
+        catalog: str = DEFAULT_CATALOG,
+    ):
         database = f"`{catalog}`.`{database}`" if catalog else f"`{database}`"
         self._logger.debug(f"Creating database if not exists {database}")
         sql = f"CREATE DATABASE IF NOT EXISTS {database}"
         self._logger.debug(sql)
         self.spark.sql(sql)
         return sql
 
     def alter_table_drop_constraint(
-        self, database: str, table: str, name: str, catalog: str = None
+        self, database: str, table: str, name: str, catalog: str = DEFAULT_CATALOG
     ):
         database = f"`{catalog}`.`{database}`" if catalog else f"`{database}`"
         return f"ALTER TABLE {database}.`{table}` DROP CONSTRAINT {name};"
 
     def alter_table_add_constraint(
-        self, database: str, table: str, name: str, constraint: str, catalog: str = None
+        self,
+        database: str,
+        table: str,
+        name: str,
+        constraint: str,
+        catalog: str = DEFAULT_CATALOG,
     ):
         database = f"`{catalog}`.`{database}`" if catalog else f"`{database}`"
         return f"ALTER TABLE {database}.`{table}` ADD CONSTRAINT {name} CHECK ({constraint});"
 
     def alter_table_set_tblproperties(
-        self, database: str, table: str, properties: str, catalog: str = None
+        self, database: str, table: str, properties: str, catalog: str = DEFAULT_CATALOG
     ):
         database = f"`{catalog}`.`{database}`" if catalog else f"`{database}`"
         return f"ALTER TABLE {database}.`{table}` SET TBLPROPERTIES ({properties});"
 
-    def get_table_properties(self, database: str, table: str, catalog: str = None):
+    def get_table_properties(
+        self, database: str, table: str, catalog: str = DEFAULT_CATALOG
+    ):
         database = f"`{catalog}`.`{database}`" if catalog else f"`{database}`"
         self._logger.debug(
             f"getting existing table properties for table {database}.`{table}`"
         )
 
         df: DataFrame = self.spark.sql(
             f"SHOW TBLPROPERTIES {database}.`{table}`"
@@ -318,15 +330,15 @@
 
     def optimize(
         self,
         database: str,
         table: str,
         partition_values: dict,
         zorder_by: list = [],
-        catalog: str = None,
+        catalog: str = DEFAULT_CATALOG,
     ):
         database = f"`{catalog}`.`{database}`" if catalog else f"`{database}`"
         sql = f"OPTIMIZE {database}.`{table}`"
 
         if partition_values:
             predicate = self.get_partition_predicate(partition_values)
             predicate = f" WHERE {predicate}"
@@ -335,15 +347,17 @@
         if zorder_by:
             sql_zorderby = ",".join([f"`{z}`" for z in zorder_by])
             sql = f"{sql} ZORDER BY ({sql_zorderby})"
 
         self._logger.info(f"optimizing table {database}.{table}\n{sql}")
         self.spark.sql(sql)
 
-    def get_table_details(self, database: str, table: str, catalog: str = None):
+    def get_table_details(
+        self, database: str, table: str, catalog: str = DEFAULT_CATALOG
+    ):
         database = f"`{catalog}`.`{database}`" if catalog else f"`{database}`"
         self._logger.debug(
             f"getting existing table details and partitions for table {database}.{table}"
         )
 
         df: DataFrame = self.spark.sql(
             f"DESCRIBE TABLE EXTENDED {database}.`{table}`"
```

### Comparing `yetl-framework-2.0.3/yetl/config/table/_deltalake.py` & `yetl-framework-2.0.4.dev1/yetl/config/table/_deltalake.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from pydantic import Field, PrivateAttr
 from .._utils import (
     JinjaVariables,
     render_jinja,
     is_databricks,
     abs_config_path,
     load_text,
+    DEFAULT_CATALOG,
 )
 from typing import Any, Dict, Union, List, Optional
 from .._timeslice import Timeslice
 import os
 from .._stage_type import StageType
 from ._table import Table
 from ..deltalake import DeltaLakeFn
@@ -83,21 +84,21 @@
             if self.options:
                 for option, value in self.options.items():
                     if isinstance(value, str):
                         self.options[option] = render_jinja(value, self._replacements)
 
         self._rendered = True
 
-    def create_database(self, catalog: str = None, catalog_enabled: bool = True):
-        super().create_database(catalog=catalog, catalog_enabled=catalog_enabled)
+    def create_database(self, catalog: str = DEFAULT_CATALOG):
+        super().create_database(catalog=catalog)
         self._spark.create_database(self.database, catalog=self.catalog)
 
     # TODO: Create or alter table
-    def create_table(self, catalog: str = None, catalog_enabled: bool = True):
-        super().create_table(catalog=catalog, catalog_enabled=catalog_enabled)
+    def create_table(self, catalog: str = DEFAULT_CATALOG):
+        super().create_table(catalog=catalog)
         if self._spark.table_exists(
             database=self.database, table=self.table, catalog=self.catalog
         ):
             pass
             # TODO: alter table
             if self.catalog:
                 msg = f"table `{self.catalog}`.{self.database}`.`{self.table}` already exists."
```

### Comparing `yetl-framework-2.0.3/yetl/config/table/_factory.py` & `yetl-framework-2.0.4.dev1/yetl/config/table/_factory.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.3/yetl/config/table/_read.py` & `yetl-framework-2.0.4.dev1/yetl/config/table/_read.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.3/yetl/config/table/_table.py` & `yetl-framework-2.0.4.dev1/yetl/config/table/_table.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from pydantic import BaseModel, Field, PrivateAttr
-from .._utils import JinjaVariables
+from .._utils import JinjaVariables, DEFAULT_CATALOG
 from typing import Any, Dict, Union, List, Optional
 from .._timeslice import Timeslice
 from .._stage_type import StageType
 from ._table_type import TableType
 from .._project import Project
 from enum import Enum
 from .._utils import render_jinja
@@ -83,15 +83,14 @@
     location: str = Field(...)
     path: Optional[str] = Field(default=None)
     options: dict = Field(...)
     timeslice: Timeslice = Field(...)
     checkpoint: Optional[str] = Field(default=None)
     config_path: str = Field(...)
     catalog: Optional[str] = Field(default=None)
-    catalog_enabled: Optional[bool] = Field(default=True)
 
     def _render(self):
         self._replacements = {
             JinjaVariables.TABLE: self.table,
             JinjaVariables.DATABASE: self.database,
             JinjaVariables.CONTAINER: self.container,
             JinjaVariables.CHECKPOINT: self.checkpoint,
@@ -116,22 +115,18 @@
 
         if threshold_type == ValidationThresholdType.warning:
             if self.warning_thresholds:
                 return self.warning_thresholds.select_sql()
             else:
                 return ValidationThreshold.default_select_sql()
 
-    def _set_catalog(self, catalog: str = None, catalog_enabled: bool = True):
-        if catalog:
-            self.catalog = catalog
-        self.catalog_enabled = catalog_enabled
-        if not self.catalog_enabled:
-            self.catalog = None
+    def _set_catalog(self, catalog: str = DEFAULT_CATALOG):
+        self.catalog = catalog
 
-    def create_table(self, catalog: str = None, catalog_enabled: bool = True):
-        self._set_catalog(catalog, catalog_enabled)
+    def create_table(self, catalog: str = DEFAULT_CATALOG):
+        self._set_catalog(catalog)
 
-    def create_database(self, catalog: str = None, catalog_enabled: bool = True):
-        self._set_catalog(catalog, catalog_enabled)
+    def create_database(self, catalog: str = DEFAULT_CATALOG):
+        self._set_catalog(catalog)
 
     def qualified_table_name(self):
         pass
```

### Comparing `yetl-framework-2.0.3/yetl/resource/__init__.py` & `yetl-framework-2.0.4.dev1/yetl/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.3/yetl/resource/sibytes_yetl_pipeline_schema.json` & `yetl-framework-2.0.4.dev1/yetl/resource/sibytes_yetl_pipeline_schema.json`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.3/yetl/resource/sibytes_yetl_project_schema.json` & `yetl-framework-2.0.4.dev1/yetl/resource/sibytes_yetl_project_schema.json`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.3/yetl/resource/sibytes_yetl_tables_schema.json` & `yetl-framework-2.0.4.dev1/yetl/resource/sibytes_yetl_tables_schema.json`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.3/yetl/resource/tables.xlsx` & `yetl-framework-2.0.4.dev1/yetl/resource/tables.xlsx`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.3/yetl/validation/_validate.py` & `yetl-framework-2.0.4.dev1/yetl/validation/_validate.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.3/yetl/workflow/_dlt.py` & `yetl-framework-2.0.4.dev1/yetl/workflow/_dlt.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.3/yetl/workflow/_multi_threaded.py` & `yetl-framework-2.0.4.dev1/yetl/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.3/yetl_framework.egg-info/PKG-INFO` & `yetl-framework-2.0.4.dev1/yetl_framework.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 2.0.3
+Version: 2.0.4.dev1
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-2.0.3/yetl_framework.egg-info/SOURCES.txt` & `yetl-framework-2.0.4.dev1/yetl_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

