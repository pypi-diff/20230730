# Comparing `tmp/gfx-perps-sdk-0.0.2.tar.gz` & `tmp/gfx_perps_sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gfx-perps-sdk-0.0.2.tar", last modified: Sun Jul 30 06:55:17 2023, max compression
+gzip compressed data, was "gfx_perps_sdk-0.0.3.tar", last modified: Sun Jul 30 06:56:50 2023, max compression
```

## Comparing `gfx-perps-sdk-0.0.2.tar` & `gfx_perps_sdk-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 arvindkrishnan   (501) staff       (20)        0 2023-07-30 06:55:17.141952 gfx-perps-sdk-0.0.2/
--rw-r--r--   0 arvindkrishnan   (501) staff       (20)     1073 2023-07-30 06:27:01.000000 gfx-perps-sdk-0.0.2/LICENSE
--rw-r--r--   0 arvindkrishnan   (501) staff       (20)      636 2023-07-30 06:55:17.141546 gfx-perps-sdk-0.0.2/PKG-INFO
--rw-r--r--   0 arvindkrishnan   (501) staff       (20)      170 2023-07-30 06:26:46.000000 gfx-perps-sdk-0.0.2/README.md
-drwxr-xr-x   0 arvindkrishnan   (501) staff       (20)        0 2023-07-30 06:55:17.140617 gfx-perps-sdk-0.0.2/gfx_perps_sdk.egg-info/
--rw-r--r--   0 arvindkrishnan   (501) staff       (20)      636 2023-07-30 06:55:17.000000 gfx-perps-sdk-0.0.2/gfx_perps_sdk.egg-info/PKG-INFO
--rw-r--r--   0 arvindkrishnan   (501) staff       (20)      207 2023-07-30 06:55:17.000000 gfx-perps-sdk-0.0.2/gfx_perps_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 arvindkrishnan   (501) staff       (20)        1 2023-07-30 06:55:17.000000 gfx-perps-sdk-0.0.2/gfx_perps_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 arvindkrishnan   (501) staff       (20)        6 2023-07-30 06:55:17.000000 gfx-perps-sdk-0.0.2/gfx_perps_sdk.egg-info/top_level.txt
--rw-r--r--   0 arvindkrishnan   (501) staff       (20)      441 2023-07-30 06:55:12.000000 gfx-perps-sdk-0.0.2/pyproject.toml
--rw-r--r--   0 arvindkrishnan   (501) staff       (20)       38 2023-07-30 06:55:17.142048 gfx-perps-sdk-0.0.2/setup.cfg
--rw-r--r--   0 arvindkrishnan   (501) staff       (20)      794 2023-07-30 06:54:44.000000 gfx-perps-sdk-0.0.2/setup.py
-drwxr-xr-x   0 arvindkrishnan   (501) staff       (20)        0 2023-07-30 06:55:17.140987 gfx-perps-sdk-0.0.2/tests/
--rw-r--r--   0 arvindkrishnan   (501) staff       (20)      126 2023-07-30 06:48:16.000000 gfx-perps-sdk-0.0.2/tests/__init__.py
+drwxr-xr-x   0 arvindkrishnan   (501) staff       (20)        0 2023-07-30 06:56:50.287309 gfx_perps_sdk-0.0.3/
+-rw-r--r--   0 arvindkrishnan   (501) staff       (20)     1073 2023-07-30 06:27:01.000000 gfx_perps_sdk-0.0.3/LICENSE
+-rw-r--r--   0 arvindkrishnan   (501) staff       (20)      636 2023-07-30 06:56:50.287035 gfx_perps_sdk-0.0.3/PKG-INFO
+-rw-r--r--   0 arvindkrishnan   (501) staff       (20)      170 2023-07-30 06:26:46.000000 gfx_perps_sdk-0.0.3/README.md
+drwxr-xr-x   0 arvindkrishnan   (501) staff       (20)        0 2023-07-30 06:56:50.285776 gfx_perps_sdk-0.0.3/gfx_perps_sdk.egg-info/
+-rw-r--r--   0 arvindkrishnan   (501) staff       (20)      636 2023-07-30 06:56:50.000000 gfx_perps_sdk-0.0.3/gfx_perps_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 arvindkrishnan   (501) staff       (20)      207 2023-07-30 06:56:50.000000 gfx_perps_sdk-0.0.3/gfx_perps_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 arvindkrishnan   (501) staff       (20)        1 2023-07-30 06:56:50.000000 gfx_perps_sdk-0.0.3/gfx_perps_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 arvindkrishnan   (501) staff       (20)        6 2023-07-30 06:56:50.000000 gfx_perps_sdk-0.0.3/gfx_perps_sdk.egg-info/top_level.txt
+-rw-r--r--   0 arvindkrishnan   (501) staff       (20)      441 2023-07-30 06:56:38.000000 gfx_perps_sdk-0.0.3/pyproject.toml
+-rw-r--r--   0 arvindkrishnan   (501) staff       (20)       38 2023-07-30 06:56:50.287464 gfx_perps_sdk-0.0.3/setup.cfg
+-rw-r--r--   0 arvindkrishnan   (501) staff       (20)      794 2023-07-30 06:54:44.000000 gfx_perps_sdk-0.0.3/setup.py
+drwxr-xr-x   0 arvindkrishnan   (501) staff       (20)        0 2023-07-30 06:56:50.286568 gfx_perps_sdk-0.0.3/tests/
+-rw-r--r--   0 arvindkrishnan   (501) staff       (20)      126 2023-07-30 06:48:16.000000 gfx_perps_sdk-0.0.3/tests/__init__.py
```

### Comparing `gfx-perps-sdk-0.0.2/LICENSE` & `gfx_perps_sdk-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gfx-perps-sdk-0.0.2/PKG-INFO` & `gfx_perps_sdk-0.0.3/gfx_perps_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gfx-perps-sdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small example package
 Home-page: https://github.com/GooseFX1/gfx-perps-python-sdk
 Author: Arvind Krishnan
 Author-email: Arvind Krishnan <arvind98krishnan@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gfx-perps-sdk-0.0.2/gfx_perps_sdk.egg-info/PKG-INFO` & `gfx_perps_sdk-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gfx-perps-sdk
-Version: 0.0.2
+Name: gfx_perps_sdk
+Version: 0.0.3
 Summary: A small example package
 Home-page: https://github.com/GooseFX1/gfx-perps-python-sdk
 Author: Arvind Krishnan
 Author-email: Arvind Krishnan <arvind98krishnan@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gfx-perps-sdk-0.0.2/setup.py` & `gfx_perps_sdk-0.0.3/setup.py`

 * *Files identical despite different names*

