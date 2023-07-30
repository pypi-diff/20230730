# Comparing `tmp/python3-commons-0.0.9.tar.gz` & `tmp/python3-commons-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python3-commons-0.0.9.tar", last modified: Thu Mar  9 22:53:13 2023, max compression
+gzip compressed data, was "python3-commons-0.1.0.tar", last modified: Sun Jul 30 09:58:31 2023, max compression
```

## Comparing `python3-commons-0.0.9.tar` & `python3-commons-0.1.0.tar`

### file list

```diff
@@ -1,49 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 22:53:13.004127 python3-commons-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-03-09 22:53:00.000000 python3-commons-0.0.9/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 22:53:12.984126 python3-commons-0.0.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 22:53:12.992127 python3-commons-0.0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-03-09 22:53:00.000000 python3-commons-0.0.9/.github/workflows/python-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-09 22:53:00.000000 python3-commons-0.0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-09 22:53:00.000000 python3-commons-0.0.9/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-09 22:53:00.000000 python3-commons-0.0.9/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    34575 2023-03-09 22:53:00.000000 python3-commons-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-09 22:53:13.004127 python3-commons-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-09 22:53:00.000000 python3-commons-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-09 22:53:00.000000 python3-commons-0.0.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 22:53:12.996127 python3-commons-0.0.9/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-03-09 22:53:00.000000 python3-commons-0.0.9/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 22:53:12.996127 python3-commons-0.0.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-09 22:53:00.000000 python3-commons-0.0.9/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-09 22:53:00.000000 python3-commons-0.0.9/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-09 22:53:00.000000 python3-commons-0.0.9/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9373 2023-03-09 22:53:00.000000 python3-commons-0.0.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-03-09 22:53:00.000000 python3-commons-0.0.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-09 22:53:00.000000 python3-commons-0.0.9/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-09 22:53:00.000000 python3-commons-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-03-09 22:53:00.000000 python3-commons-0.0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-09 22:53:00.000000 python3-commons-0.0.9/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-03-09 22:53:13.004127 python3-commons-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-09 22:53:00.000000 python3-commons-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 22:53:12.996127 python3-commons-0.0.9/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-03-09 22:53:00.000000 python3-commons-0.0.9/src/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 22:53:13.000127 python3-commons-0.0.9/src/python3_commons/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-03-09 22:53:00.000000 python3-commons-0.0.9/src/python3_commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-09 22:53:00.000000 python3-commons-0.0.9/src/python3_commons/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-03-09 22:53:00.000000 python3-commons-0.0.9/src/python3_commons/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-03-09 22:53:00.000000 python3-commons-0.0.9/src/python3_commons/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-03-09 22:53:00.000000 python3-commons-0.0.9/src/python3_commons/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 22:53:13.000127 python3-commons-0.0.9/src/python3_commons/logging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 22:53:00.000000 python3-commons-0.0.9/src/python3_commons/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-09 22:53:00.000000 python3-commons-0.0.9/src/python3_commons/logging/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-09 22:53:00.000000 python3-commons-0.0.9/src/python3_commons/logging/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-03-09 22:53:00.000000 python3-commons-0.0.9/src/python3_commons/minio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-03-09 22:53:00.000000 python3-commons-0.0.9/src/python3_commons/object_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 22:53:13.000127 python3-commons-0.0.9/src/python3_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-09 22:53:12.000000 python3-commons-0.0.9/src/python3_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-03-09 22:53:12.000000 python3-commons-0.0.9/src/python3_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 22:53:12.000000 python3-commons-0.0.9/src/python3_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 22:53:12.000000 python3-commons-0.0.9/src/python3_commons.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-09 22:53:12.000000 python3-commons-0.0.9/src/python3_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-09 22:53:12.000000 python3-commons-0.0.9/src/python3_commons.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 22:53:13.004127 python3-commons-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-09 22:53:00.000000 python3-commons-0.0.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:58:31.718393 python3-commons-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-30 09:58:20.000000 python3-commons-0.1.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:58:31.710393 python3-commons-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:58:31.714393 python3-commons-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-30 09:58:20.000000 python3-commons-0.1.0/.github/workflows/python-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-30 09:58:20.000000 python3-commons-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-30 09:58:20.000000 python3-commons-0.1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-30 09:58:20.000000 python3-commons-0.1.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    34575 2023-07-30 09:58:20.000000 python3-commons-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-30 09:58:31.718393 python3-commons-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-30 09:58:20.000000 python3-commons-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-30 09:58:20.000000 python3-commons-0.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:58:31.714393 python3-commons-0.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-30 09:58:20.000000 python3-commons-0.1.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:58:31.714393 python3-commons-0.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-30 09:58:20.000000 python3-commons-0.1.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-30 09:58:20.000000 python3-commons-0.1.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-30 09:58:20.000000 python3-commons-0.1.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9373 2023-07-30 09:58:20.000000 python3-commons-0.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-30 09:58:20.000000 python3-commons-0.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-30 09:58:20.000000 python3-commons-0.1.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-30 09:58:20.000000 python3-commons-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-30 09:58:20.000000 python3-commons-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-30 09:58:20.000000 python3-commons-0.1.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-30 09:58:20.000000 python3-commons-0.1.0/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-30 09:58:31.718393 python3-commons-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-30 09:58:20.000000 python3-commons-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:58:31.710393 python3-commons-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:58:31.714393 python3-commons-0.1.0/src/python3_commons/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-30 09:58:20.000000 python3-commons-0.1.0/src/python3_commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-30 09:58:20.000000 python3-commons-0.1.0/src/python3_commons/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-30 09:58:20.000000 python3-commons-0.1.0/src/python3_commons/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-30 09:58:20.000000 python3-commons-0.1.0/src/python3_commons/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-30 09:58:20.000000 python3-commons-0.1.0/src/python3_commons/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:58:31.714393 python3-commons-0.1.0/src/python3_commons/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 09:58:20.000000 python3-commons-0.1.0/src/python3_commons/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-30 09:58:20.000000 python3-commons-0.1.0/src/python3_commons/logging/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-30 09:58:20.000000 python3-commons-0.1.0/src/python3_commons/logging/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-30 09:58:20.000000 python3-commons-0.1.0/src/python3_commons/minio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-30 09:58:20.000000 python3-commons-0.1.0/src/python3_commons/object_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:58:31.714393 python3-commons-0.1.0/src/python3_commons/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 09:58:20.000000 python3-commons-0.1.0/src/python3_commons/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-30 09:58:20.000000 python3-commons-0.1.0/src/python3_commons/serializers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-30 09:58:20.000000 python3-commons-0.1.0/src/python3_commons/serializers/msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-30 09:58:20.000000 python3-commons-0.1.0/src/python3_commons/serializers/msgspec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:58:31.714393 python3-commons-0.1.0/src/python3_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-30 09:58:31.000000 python3-commons-0.1.0/src/python3_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-30 09:58:31.000000 python3-commons-0.1.0/src/python3_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 09:58:31.000000 python3-commons-0.1.0/src/python3_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 09:58:31.000000 python3-commons-0.1.0/src/python3_commons.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-30 09:58:31.000000 python3-commons-0.1.0/src/python3_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-30 09:58:31.000000 python3-commons-0.1.0/src/python3_commons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:58:31.718393 python3-commons-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-30 09:58:20.000000 python3-commons-0.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-30 09:58:20.000000 python3-commons-0.1.0/tests/test_msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-30 09:58:20.000000 python3-commons-0.1.0/tests/test_msgspec.py
```

### Comparing `python3-commons-0.0.9/.coveragerc` & `python3-commons-0.1.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `python3-commons-0.0.9/.github/workflows/python-publish.yaml` & `python3-commons-0.1.0/.github/workflows/python-publish.yaml`

 * *Files identical despite different names*

### Comparing `python3-commons-0.0.9/.gitignore` & `python3-commons-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `python3-commons-0.0.9/LICENSE` & `python3-commons-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python3-commons-0.0.9/PKG-INFO` & `python3-commons-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: python3-commons
-Version: 0.0.9
+Version: 0.1.0
 Summary: Re-usable Python3 code
 Home-page: https://github.com/kamikaze/python3-commons
 Author: Oleg Korsak
 Author-email: kamikaze.is.waiting.you@gmail.com
 License: gpl-3
 Project-URL: Documentation, https://github.com/kamikaze/python3-commons/wiki
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Requires-Python: >=3.9
+Requires-Python: >=3.11
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: testing
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 Re-usable Python3 code
 ======================
```

### Comparing `python3-commons-0.0.9/docs/Makefile` & `python3-commons-0.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python3-commons-0.0.9/docs/conf.py` & `python3-commons-0.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python3-commons-0.0.9/docs/index.rst` & `python3-commons-0.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python3-commons-0.0.9/setup.cfg` & `python3-commons-0.1.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python3-commons
-version = 0.0.9
+version = 0.1.0
 description = Re-usable Python3 code
 author = Oleg Korsak
 author_email = kamikaze.is.waiting.you@gmail.com
 license = gpl-3
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 url = https://github.com/kamikaze/python3-commons
@@ -19,19 +19,21 @@
 zip_safe = False
 packages = find:
 include_package_data = True
 package_dir = 
 	=src
 setup_requires = pyscaffold>=3.2a0,<3.3a0
 install_requires = 
-	asyncpg==0.27.0
+	asyncpg==0.28.0
 	databases[postgresql]==0.7.0
-	minio==7.1.13
-	pydantic[email]==1.10.6
-python_requires = >=3.9
+	minio==7.1.15
+	msgpack==1.0.5
+	msgspec==0.17.0
+	pydantic[email]==1.10.9
+python_requires = >=3.11
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
```

### Comparing `python3-commons-0.0.9/src/python3_commons/db.py` & `python3-commons-0.1.0/src/python3_commons/db.py`

 * *Files identical despite different names*

### Comparing `python3-commons-0.0.9/src/python3_commons/minio.py` & `python3-commons-0.1.0/src/python3_commons/minio.py`

 * *Files identical despite different names*

### Comparing `python3-commons-0.0.9/src/python3_commons/object_storage.py` & `python3-commons-0.1.0/src/python3_commons/object_storage.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,100 @@
 import logging
-from io import RawIOBase
+from io import IOBase
+from typing import Generator
 
 from minio import Minio
-from pydantic import SecretStr
+from minio.datatypes import Object
 
 from python3_commons import minio
+from python3_commons.conf import s3_settings
 
 logger = logging.getLogger(__name__)
-_CLIENT = None
+__CLIENT = None
 
 
-def get_s3_client(endpoint_url: str, region_name: str, access_key_id: SecretStr, secret_access_key: SecretStr,
-                  secure: bool = True) -> Minio:
-    global _CLIENT
+def get_s3_client() -> Minio:
+    global __CLIENT
 
-    if not _CLIENT:
-        _CLIENT = minio.get_client(endpoint_url, region_name, access_key_id, secret_access_key, secure)
+    if not __CLIENT and s3_settings.s3_endpoint_url:
+        __CLIENT = minio.get_client(
+            s3_settings.s3_endpoint_url,
+            s3_settings.s3_region_name,
+            s3_settings.s3_access_key_id,
+            s3_settings.s3_secret_access_key,
+            s3_settings.s3_secure
+        )
 
-    return _CLIENT
+    return __CLIENT
 
 
-def get_absolute_path(path: str, root: str = None) -> str:
+def get_absolute_path(path: str) -> str:
     if path.startswith('/'):
         path = path[1:]
 
-    if root:
-        path = f'{root[:1] if root.startswith("/") else root}/{path}'
+    if bucket_root := s3_settings.s3_bucket_root:
+        path = f'{bucket_root[:1] if bucket_root.startswith("/") else bucket_root}/{path}'
 
     return path
 
 
-def put_object(bucket_name: str, path: str, data: bytes | RawIOBase, length: int):
-    path = get_absolute_path(path)
+def put_object(bucket_name: str, path: str, data: IOBase, length: int):
     s3_client = get_s3_client()
 
-    result = s3_client.put_object(bucket_name, path, data, length)
+    if s3_client:
+        result = s3_client.put_object(bucket_name, path, data, length)
 
-    return result.location
+        logger.debug(f'Stored object into object storage: {bucket_name}:{path}')
+
+        return result.location
+    else:
+        logger.warning(f'No S3 client available, skipping object put')
 
 
 def get_object_stream(bucket_name: str, path: str):
-    path = get_absolute_path(path)
     s3_client = get_s3_client()
 
-    logger.debug(f'Getting object from object storage: {bucket_name}:{path}')
-
-    try:
-        response = s3_client.get_object(bucket_name, path)
-    except Exception as e:
-        logger.exception(f'Failed getting object from object storage: {bucket_name}:{path}', exc_info=e)
-
-        raise
+    if s3_client:
+        logger.debug(f'Getting object from object storage: {bucket_name}:{path}')
 
-    return response
+        try:
+            response = s3_client.get_object(bucket_name, path)
+        except Exception as e:
+            logger.debug(f'Failed getting object from object storage: {bucket_name}:{path}', exc_info=e)
+
+            raise
+
+        return response
+    else:
+        logger.warning(f'No S3 client available, skipping object put')
 
 
 def get_object(bucket_name: str, path: str) -> bytes:
     response = get_object_stream(bucket_name, path)
 
     try:
         body = response.read()
     finally:
         response.close()
         response.release_conn()
 
     logger.debug(f'Loaded object from object storage: {bucket_name}:{path}')
 
     return body
+
+
+def list_objects(bucket_name: str, path: str, recursive: bool = True) -> Generator[Object, None, None]:
+    s3_client = get_s3_client()
+
+    yield from s3_client.list_objects(bucket_name, path, recursive)
+
+
+def get_objects(bucket_name: str, path: str, recursive: bool = True) -> Generator[tuple[str, bytes], None, None]:
+    for obj in list_objects(bucket_name, path, recursive):
+        object_name = obj.object_name
+
+        if obj.size:
+            data = get_object(bucket_name, object_name)
+        else:
+            data = b''
+
+        yield object_name, data
```

### Comparing `python3-commons-0.0.9/src/python3_commons.egg-info/PKG-INFO` & `python3-commons-0.1.0/src/python3_commons.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: python3-commons
-Version: 0.0.9
+Version: 0.1.0
 Summary: Re-usable Python3 code
 Home-page: https://github.com/kamikaze/python3-commons
 Author: Oleg Korsak
 Author-email: kamikaze.is.waiting.you@gmail.com
 License: gpl-3
 Project-URL: Documentation, https://github.com/kamikaze/python3-commons/wiki
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Requires-Python: >=3.9
+Requires-Python: >=3.11
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: testing
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 Re-usable Python3 code
 ======================
```

### Comparing `python3-commons-0.0.9/src/python3_commons.egg-info/SOURCES.txt` & `python3-commons-0.1.0/src/python3_commons.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -4,35 +4,41 @@
 CHANGELOG.rst
 LICENSE
 README.md
 README.rst
 pyproject.toml
 requirements.txt
 requirements_dev.txt
+requirements_test.txt
 setup.cfg
 setup.py
 .github/workflows/python-publish.yaml
 docs/Makefile
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
 docs/index.rst
 docs/license.rst
 docs/_static/.gitignore
-src/helpers.py
 src/python3_commons/__init__.py
 src/python3_commons/conf.py
 src/python3_commons/db.py
 src/python3_commons/fs.py
-src/python3_commons/json.py
+src/python3_commons/helpers.py
 src/python3_commons/minio.py
 src/python3_commons/object_storage.py
 src/python3_commons.egg-info/PKG-INFO
 src/python3_commons.egg-info/SOURCES.txt
 src/python3_commons.egg-info/dependency_links.txt
 src/python3_commons.egg-info/not-zip-safe
 src/python3_commons.egg-info/requires.txt
 src/python3_commons.egg-info/top_level.txt
 src/python3_commons/logging/__init__.py
 src/python3_commons/logging/filters.py
 src/python3_commons/logging/formatter.py
-tests/conftest.py
+src/python3_commons/serializers/__init__.py
+src/python3_commons/serializers/json.py
+src/python3_commons/serializers/msgpack.py
+src/python3_commons/serializers/msgspec.py
+tests/conftest.py
+tests/test_msgpack.py
+tests/test_msgspec.py
```

