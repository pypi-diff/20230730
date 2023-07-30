# Comparing `tmp/python3-commons-0.1.0.tar.gz` & `tmp/python3-commons-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python3-commons-0.1.0.tar", last modified: Sun Jul 30 09:58:31 2023, max compression
+gzip compressed data, was "python3-commons-0.1.1.tar", last modified: Sun Jul 30 10:30:13 2023, max compression
```

## Comparing `python3-commons-0.1.0.tar` & `python3-commons-0.1.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:58:31.718393 python3-commons-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-30 09:58:20.000000 python3-commons-0.1.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:58:31.710393 python3-commons-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:58:31.714393 python3-commons-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-30 09:58:20.000000 python3-commons-0.1.0/.github/workflows/python-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-30 09:58:20.000000 python3-commons-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-30 09:58:20.000000 python3-commons-0.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-30 09:58:20.000000 python3-commons-0.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    34575 2023-07-30 09:58:20.000000 python3-commons-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-30 09:58:31.718393 python3-commons-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-30 09:58:20.000000 python3-commons-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-30 09:58:20.000000 python3-commons-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:58:31.714393 python3-commons-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-30 09:58:20.000000 python3-commons-0.1.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:58:31.714393 python3-commons-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-30 09:58:20.000000 python3-commons-0.1.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-30 09:58:20.000000 python3-commons-0.1.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-30 09:58:20.000000 python3-commons-0.1.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9373 2023-07-30 09:58:20.000000 python3-commons-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-30 09:58:20.000000 python3-commons-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-30 09:58:20.000000 python3-commons-0.1.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-30 09:58:20.000000 python3-commons-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-30 09:58:20.000000 python3-commons-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-30 09:58:20.000000 python3-commons-0.1.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-30 09:58:20.000000 python3-commons-0.1.0/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-30 09:58:31.718393 python3-commons-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-30 09:58:20.000000 python3-commons-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:58:31.710393 python3-commons-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:58:31.714393 python3-commons-0.1.0/src/python3_commons/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-30 09:58:20.000000 python3-commons-0.1.0/src/python3_commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-30 09:58:20.000000 python3-commons-0.1.0/src/python3_commons/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-30 09:58:20.000000 python3-commons-0.1.0/src/python3_commons/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-30 09:58:20.000000 python3-commons-0.1.0/src/python3_commons/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-30 09:58:20.000000 python3-commons-0.1.0/src/python3_commons/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:58:31.714393 python3-commons-0.1.0/src/python3_commons/logging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 09:58:20.000000 python3-commons-0.1.0/src/python3_commons/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-30 09:58:20.000000 python3-commons-0.1.0/src/python3_commons/logging/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-30 09:58:20.000000 python3-commons-0.1.0/src/python3_commons/logging/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-30 09:58:20.000000 python3-commons-0.1.0/src/python3_commons/minio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-30 09:58:20.000000 python3-commons-0.1.0/src/python3_commons/object_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:58:31.714393 python3-commons-0.1.0/src/python3_commons/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 09:58:20.000000 python3-commons-0.1.0/src/python3_commons/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-30 09:58:20.000000 python3-commons-0.1.0/src/python3_commons/serializers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-30 09:58:20.000000 python3-commons-0.1.0/src/python3_commons/serializers/msgpack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-30 09:58:20.000000 python3-commons-0.1.0/src/python3_commons/serializers/msgspec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:58:31.714393 python3-commons-0.1.0/src/python3_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-30 09:58:31.000000 python3-commons-0.1.0/src/python3_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-30 09:58:31.000000 python3-commons-0.1.0/src/python3_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 09:58:31.000000 python3-commons-0.1.0/src/python3_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 09:58:31.000000 python3-commons-0.1.0/src/python3_commons.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-30 09:58:31.000000 python3-commons-0.1.0/src/python3_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-30 09:58:31.000000 python3-commons-0.1.0/src/python3_commons.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:58:31.718393 python3-commons-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-30 09:58:20.000000 python3-commons-0.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-30 09:58:20.000000 python3-commons-0.1.0/tests/test_msgpack.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-30 09:58:20.000000 python3-commons-0.1.0/tests/test_msgspec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:30:13.957391 python3-commons-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-30 10:30:00.000000 python3-commons-0.1.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:30:13.949390 python3-commons-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:30:13.953390 python3-commons-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-30 10:30:00.000000 python3-commons-0.1.1/.github/workflows/python-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-30 10:30:00.000000 python3-commons-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-30 10:30:00.000000 python3-commons-0.1.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-30 10:30:00.000000 python3-commons-0.1.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    34575 2023-07-30 10:30:00.000000 python3-commons-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-30 10:30:13.957391 python3-commons-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-30 10:30:00.000000 python3-commons-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-30 10:30:00.000000 python3-commons-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:30:13.953390 python3-commons-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-30 10:30:00.000000 python3-commons-0.1.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:30:13.953390 python3-commons-0.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-30 10:30:00.000000 python3-commons-0.1.1/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-30 10:30:00.000000 python3-commons-0.1.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-30 10:30:00.000000 python3-commons-0.1.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9373 2023-07-30 10:30:00.000000 python3-commons-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-30 10:30:00.000000 python3-commons-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-30 10:30:00.000000 python3-commons-0.1.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-30 10:30:00.000000 python3-commons-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-30 10:30:00.000000 python3-commons-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-30 10:30:00.000000 python3-commons-0.1.1/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-30 10:30:00.000000 python3-commons-0.1.1/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-30 10:30:13.957391 python3-commons-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-30 10:30:00.000000 python3-commons-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:30:13.949390 python3-commons-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:30:13.953390 python3-commons-0.1.1/src/python3_commons/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-30 10:30:00.000000 python3-commons-0.1.1/src/python3_commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-30 10:30:00.000000 python3-commons-0.1.1/src/python3_commons/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-30 10:30:00.000000 python3-commons-0.1.1/src/python3_commons/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-30 10:30:00.000000 python3-commons-0.1.1/src/python3_commons/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-30 10:30:00.000000 python3-commons-0.1.1/src/python3_commons/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:30:13.953390 python3-commons-0.1.1/src/python3_commons/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:30:00.000000 python3-commons-0.1.1/src/python3_commons/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-30 10:30:00.000000 python3-commons-0.1.1/src/python3_commons/logging/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-30 10:30:00.000000 python3-commons-0.1.1/src/python3_commons/logging/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-30 10:30:00.000000 python3-commons-0.1.1/src/python3_commons/minio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-30 10:30:00.000000 python3-commons-0.1.1/src/python3_commons/object_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:30:13.957391 python3-commons-0.1.1/src/python3_commons/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:30:00.000000 python3-commons-0.1.1/src/python3_commons/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-30 10:30:00.000000 python3-commons-0.1.1/src/python3_commons/serializers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-30 10:30:00.000000 python3-commons-0.1.1/src/python3_commons/serializers/msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-30 10:30:00.000000 python3-commons-0.1.1/src/python3_commons/serializers/msgspec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:30:13.953390 python3-commons-0.1.1/src/python3_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-30 10:30:13.000000 python3-commons-0.1.1/src/python3_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-30 10:30:13.000000 python3-commons-0.1.1/src/python3_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 10:30:13.000000 python3-commons-0.1.1/src/python3_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 10:30:13.000000 python3-commons-0.1.1/src/python3_commons.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-30 10:30:13.000000 python3-commons-0.1.1/src/python3_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-30 10:30:13.000000 python3-commons-0.1.1/src/python3_commons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:30:13.957391 python3-commons-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-30 10:30:00.000000 python3-commons-0.1.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-30 10:30:00.000000 python3-commons-0.1.1/tests/test_msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-30 10:30:00.000000 python3-commons-0.1.1/tests/test_msgspec.py
```

### Comparing `python3-commons-0.1.0/.coveragerc` & `python3-commons-0.1.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `python3-commons-0.1.0/.github/workflows/python-publish.yaml` & `python3-commons-0.1.1/.github/workflows/python-publish.yaml`

 * *Files identical despite different names*

### Comparing `python3-commons-0.1.0/.gitignore` & `python3-commons-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `python3-commons-0.1.0/LICENSE` & `python3-commons-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python3-commons-0.1.0/PKG-INFO` & `python3-commons-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python3-commons
-Version: 0.1.0
+Version: 0.1.1
 Summary: Re-usable Python3 code
 Home-page: https://github.com/kamikaze/python3-commons
 Author: Oleg Korsak
 Author-email: kamikaze.is.waiting.you@gmail.com
 License: gpl-3
 Project-URL: Documentation, https://github.com/kamikaze/python3-commons/wiki
 Platform: any
```

### Comparing `python3-commons-0.1.0/docs/Makefile` & `python3-commons-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python3-commons-0.1.0/docs/conf.py` & `python3-commons-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python3-commons-0.1.0/docs/index.rst` & `python3-commons-0.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python3-commons-0.1.0/setup.cfg` & `python3-commons-0.1.1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 setup_requires = pyscaffold>=3.2a0,<3.3a0
 install_requires = 
 	asyncpg==0.28.0
 	databases[postgresql]==0.7.0
 	minio==7.1.15
 	msgpack==1.0.5
 	msgspec==0.17.0
-	pydantic[email]==1.10.9
+	pydantic[email]==1.10.12
 python_requires = >=3.11
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
```

### Comparing `python3-commons-0.1.0/src/python3_commons/db.py` & `python3-commons-0.1.1/src/python3_commons/db.py`

 * *Files identical despite different names*

### Comparing `python3-commons-0.1.0/src/python3_commons/helpers.py` & `python3-commons-0.1.1/src/python3_commons/helpers.py`

 * *Files identical despite different names*

### Comparing `python3-commons-0.1.0/src/python3_commons/minio.py` & `python3-commons-0.1.1/src/python3_commons/minio.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pydantic import SecretStr
 
 
 def get_client(endpoint_url: str, region_name: str, access_key_id: SecretStr, secret_access_key: SecretStr,
                secure: bool = True) -> Minio:
     http_client = urllib3.PoolManager(
         timeout=urllib3.util.Timeout(connect=300, read=300),
-        maxsize=10,
+        maxsize=50,
         cert_reqs='CERT_REQUIRED' if secure else 'CERT_NONE',
         retries=urllib3.Retry(
             total=5,
             backoff_factor=0.2,
             status_forcelist=[500, 502, 503, 504]
         )
     )
```

### Comparing `python3-commons-0.1.0/src/python3_commons/object_storage.py` & `python3-commons-0.1.1/src/python3_commons/object_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,18 +78,18 @@
         response.release_conn()
 
     logger.debug(f'Loaded object from object storage: {bucket_name}:{path}')
 
     return body
 
 
-def list_objects(bucket_name: str, path: str, recursive: bool = True) -> Generator[Object, None, None]:
+def list_objects(bucket_name: str, prefix: str, recursive: bool = True) -> Generator[Object, None, None]:
     s3_client = get_s3_client()
 
-    yield from s3_client.list_objects(bucket_name, path, recursive)
+    yield from s3_client.list_objects(bucket_name, prefix=prefix, recursive=recursive)
 
 
 def get_objects(bucket_name: str, path: str, recursive: bool = True) -> Generator[tuple[str, bytes], None, None]:
     for obj in list_objects(bucket_name, path, recursive):
         object_name = obj.object_name
 
         if obj.size:
```

### Comparing `python3-commons-0.1.0/src/python3_commons/serializers/json.py` & `python3-commons-0.1.1/src/python3_commons/serializers/json.py`

 * *Files identical despite different names*

### Comparing `python3-commons-0.1.0/src/python3_commons/serializers/msgpack.py` & `python3-commons-0.1.1/src/python3_commons/serializers/msgpack.py`

 * *Files identical despite different names*

### Comparing `python3-commons-0.1.0/src/python3_commons/serializers/msgspec.py` & `python3-commons-0.1.1/src/python3_commons/serializers/msgspec.py`

 * *Files identical despite different names*

### Comparing `python3-commons-0.1.0/src/python3_commons.egg-info/PKG-INFO` & `python3-commons-0.1.1/src/python3_commons.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python3-commons
-Version: 0.1.0
+Version: 0.1.1
 Summary: Re-usable Python3 code
 Home-page: https://github.com/kamikaze/python3-commons
 Author: Oleg Korsak
 Author-email: kamikaze.is.waiting.you@gmail.com
 License: gpl-3
 Project-URL: Documentation, https://github.com/kamikaze/python3-commons/wiki
 Platform: any
```

### Comparing `python3-commons-0.1.0/src/python3_commons.egg-info/SOURCES.txt` & `python3-commons-0.1.1/src/python3_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python3-commons-0.1.0/tests/conftest.py` & `python3-commons-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python3-commons-0.1.0/tests/test_msgpack.py` & `python3-commons-0.1.1/tests/test_msgpack.py`

 * *Files identical despite different names*

### Comparing `python3-commons-0.1.0/tests/test_msgspec.py` & `python3-commons-0.1.1/tests/test_msgspec.py`

 * *Files identical despite different names*

