# Comparing `tmp/fastshopifyapi-2.0.0.tar.gz` & `tmp/fastshopifyapi-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastshopifyapi-2.0.0.tar", last modified: Sun Jul 30 09:00:46 2023, max compression
+gzip compressed data, was "fastshopifyapi-2.0.1.tar", last modified: Sun Jul 30 09:40:29 2023, max compression
```

## Comparing `fastshopifyapi-2.0.0.tar` & `fastshopifyapi-2.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 sokoslee   (501) staff       (20)        0 2023-07-30 09:00:46.871759 fastshopifyapi-2.0.0/
--rw-r--r--   0 sokoslee   (501) staff       (20)     1151 2023-07-30 08:15:02.000000 fastshopifyapi-2.0.0/LICENSE
--rw-r--r--   0 sokoslee   (501) staff       (20)       34 2023-05-11 15:43:14.000000 fastshopifyapi-2.0.0/MANIFEST.in
--rw-r--r--   0 sokoslee   (501) staff       (20)     9689 2023-07-30 09:00:46.871823 fastshopifyapi-2.0.0/PKG-INFO
--rw-r--r--   0 sokoslee   (501) staff       (20)     8822 2023-07-30 08:33:30.000000 fastshopifyapi-2.0.0/README.md
-drwxr-xr-x   0 sokoslee   (501) staff       (20)        0 2023-07-30 09:00:46.870629 fastshopifyapi-2.0.0/fastshopifyapi/
--rw-r--r--   0 sokoslee   (501) staff       (20)      275 2023-07-30 09:00:37.000000 fastshopifyapi-2.0.0/fastshopifyapi/__init__.py
--rw-r--r--   0 sokoslee   (501) staff       (20)       47 2023-07-30 09:00:37.000000 fastshopifyapi-2.0.0/fastshopifyapi/__version__.py
-drwxr-xr-x   0 sokoslee   (501) staff       (20)        0 2023-07-30 09:00:46.871664 fastshopifyapi-2.0.0/fastshopifyapi/clients/
--rw-r--r--   0 sokoslee   (501) staff       (20)       95 2023-07-30 09:00:37.000000 fastshopifyapi-2.0.0/fastshopifyapi/clients/__init__.py
--rw-r--r--   0 sokoslee   (501) staff       (20)     6125 2023-07-30 09:00:37.000000 fastshopifyapi-2.0.0/fastshopifyapi/clients/async_client.py
--rw-r--r--   0 sokoslee   (501) staff       (20)     5871 2023-07-30 09:00:37.000000 fastshopifyapi-2.0.0/fastshopifyapi/clients/client.py
--rw-r--r--   0 sokoslee   (501) staff       (20)     8843 2023-07-30 09:00:37.000000 fastshopifyapi-2.0.0/fastshopifyapi/clients/common.py
--rw-r--r--   0 sokoslee   (501) staff       (20)      990 2023-07-30 09:00:37.000000 fastshopifyapi-2.0.0/fastshopifyapi/constants.py
--rw-r--r--   0 sokoslee   (501) staff       (20)      805 2023-07-30 09:00:37.000000 fastshopifyapi-2.0.0/fastshopifyapi/deferrer.py
--rw-r--r--   0 sokoslee   (501) staff       (20)     1072 2023-07-30 09:00:37.000000 fastshopifyapi-2.0.0/fastshopifyapi/models.py
--rw-r--r--   0 sokoslee   (501) staff       (20)     2623 2023-07-30 09:00:37.000000 fastshopifyapi-2.0.0/fastshopifyapi/options.py
--rw-r--r--   0 sokoslee   (501) staff       (20)     2145 2023-07-30 09:00:37.000000 fastshopifyapi-2.0.0/fastshopifyapi/store.py
--rw-r--r--   0 sokoslee   (501) staff       (20)      544 2023-07-30 09:00:37.000000 fastshopifyapi-2.0.0/fastshopifyapi/types.py
--rw-r--r--   0 sokoslee   (501) staff       (20)     2274 2023-07-30 09:00:37.000000 fastshopifyapi-2.0.0/fastshopifyapi/utils.py
-drwxr-xr-x   0 sokoslee   (501) staff       (20)        0 2023-07-30 09:00:46.871252 fastshopifyapi-2.0.0/fastshopifyapi.egg-info/
--rw-r--r--   0 sokoslee   (501) staff       (20)     9689 2023-07-30 09:00:46.000000 fastshopifyapi-2.0.0/fastshopifyapi.egg-info/PKG-INFO
--rw-r--r--   0 sokoslee   (501) staff       (20)      664 2023-07-30 09:00:46.000000 fastshopifyapi-2.0.0/fastshopifyapi.egg-info/SOURCES.txt
--rw-r--r--   0 sokoslee   (501) staff       (20)        1 2023-07-30 09:00:46.000000 fastshopifyapi-2.0.0/fastshopifyapi.egg-info/dependency_links.txt
--rw-r--r--   0 sokoslee   (501) staff       (20)        1 2023-07-30 09:00:46.000000 fastshopifyapi-2.0.0/fastshopifyapi.egg-info/not-zip-safe
--rw-r--r--   0 sokoslee   (501) staff       (20)       14 2023-07-30 09:00:46.000000 fastshopifyapi-2.0.0/fastshopifyapi.egg-info/requires.txt
--rw-r--r--   0 sokoslee   (501) staff       (20)       15 2023-07-30 09:00:46.000000 fastshopifyapi-2.0.0/fastshopifyapi.egg-info/top_level.txt
--rw-r--r--   0 sokoslee   (501) staff       (20)      750 2023-07-30 08:55:36.000000 fastshopifyapi-2.0.0/pyproject.toml
--rw-r--r--   0 sokoslee   (501) staff       (20)      285 2023-07-30 09:00:46.872156 fastshopifyapi-2.0.0/setup.cfg
--rw-r--r--   0 sokoslee   (501) staff       (20)     1176 2023-07-30 08:54:23.000000 fastshopifyapi-2.0.0/setup.py
+drwxr-xr-x   0 sokoslee   (501) staff       (20)        0 2023-07-30 09:40:29.838394 fastshopifyapi-2.0.1/
+-rw-r--r--   0 sokoslee   (501) staff       (20)     1151 2023-07-30 08:15:02.000000 fastshopifyapi-2.0.1/LICENSE
+-rw-r--r--   0 sokoslee   (501) staff       (20)       34 2023-05-11 15:43:14.000000 fastshopifyapi-2.0.1/MANIFEST.in
+-rw-r--r--   0 sokoslee   (501) staff       (20)     9973 2023-07-30 09:40:29.838454 fastshopifyapi-2.0.1/PKG-INFO
+-rw-r--r--   0 sokoslee   (501) staff       (20)     9106 2023-07-30 09:38:17.000000 fastshopifyapi-2.0.1/README.md
+drwxr-xr-x   0 sokoslee   (501) staff       (20)        0 2023-07-30 09:40:29.837286 fastshopifyapi-2.0.1/fastshopifyapi/
+-rw-r--r--   0 sokoslee   (501) staff       (20)      275 2023-07-30 09:00:37.000000 fastshopifyapi-2.0.1/fastshopifyapi/__init__.py
+-rw-r--r--   0 sokoslee   (501) staff       (20)       47 2023-07-30 09:39:30.000000 fastshopifyapi-2.0.1/fastshopifyapi/__version__.py
+drwxr-xr-x   0 sokoslee   (501) staff       (20)        0 2023-07-30 09:40:29.838301 fastshopifyapi-2.0.1/fastshopifyapi/clients/
+-rw-r--r--   0 sokoslee   (501) staff       (20)       95 2023-07-30 09:00:37.000000 fastshopifyapi-2.0.1/fastshopifyapi/clients/__init__.py
+-rw-r--r--   0 sokoslee   (501) staff       (20)     6125 2023-07-30 09:00:37.000000 fastshopifyapi-2.0.1/fastshopifyapi/clients/async_client.py
+-rw-r--r--   0 sokoslee   (501) staff       (20)     5871 2023-07-30 09:00:37.000000 fastshopifyapi-2.0.1/fastshopifyapi/clients/client.py
+-rw-r--r--   0 sokoslee   (501) staff       (20)     8843 2023-07-30 09:00:37.000000 fastshopifyapi-2.0.1/fastshopifyapi/clients/common.py
+-rw-r--r--   0 sokoslee   (501) staff       (20)      990 2023-07-30 09:00:37.000000 fastshopifyapi-2.0.1/fastshopifyapi/constants.py
+-rw-r--r--   0 sokoslee   (501) staff       (20)      805 2023-07-30 09:00:37.000000 fastshopifyapi-2.0.1/fastshopifyapi/deferrer.py
+-rw-r--r--   0 sokoslee   (501) staff       (20)     1072 2023-07-30 09:00:37.000000 fastshopifyapi-2.0.1/fastshopifyapi/models.py
+-rw-r--r--   0 sokoslee   (501) staff       (20)     2623 2023-07-30 09:00:37.000000 fastshopifyapi-2.0.1/fastshopifyapi/options.py
+-rw-r--r--   0 sokoslee   (501) staff       (20)     2145 2023-07-30 09:00:37.000000 fastshopifyapi-2.0.1/fastshopifyapi/store.py
+-rw-r--r--   0 sokoslee   (501) staff       (20)      544 2023-07-30 09:00:37.000000 fastshopifyapi-2.0.1/fastshopifyapi/types.py
+-rw-r--r--   0 sokoslee   (501) staff       (20)     2274 2023-07-30 09:00:37.000000 fastshopifyapi-2.0.1/fastshopifyapi/utils.py
+drwxr-xr-x   0 sokoslee   (501) staff       (20)        0 2023-07-30 09:40:29.837909 fastshopifyapi-2.0.1/fastshopifyapi.egg-info/
+-rw-r--r--   0 sokoslee   (501) staff       (20)     9973 2023-07-30 09:40:29.000000 fastshopifyapi-2.0.1/fastshopifyapi.egg-info/PKG-INFO
+-rw-r--r--   0 sokoslee   (501) staff       (20)      664 2023-07-30 09:40:29.000000 fastshopifyapi-2.0.1/fastshopifyapi.egg-info/SOURCES.txt
+-rw-r--r--   0 sokoslee   (501) staff       (20)        1 2023-07-30 09:40:29.000000 fastshopifyapi-2.0.1/fastshopifyapi.egg-info/dependency_links.txt
+-rw-r--r--   0 sokoslee   (501) staff       (20)        1 2023-07-30 09:00:46.000000 fastshopifyapi-2.0.1/fastshopifyapi.egg-info/not-zip-safe
+-rw-r--r--   0 sokoslee   (501) staff       (20)       14 2023-07-30 09:40:29.000000 fastshopifyapi-2.0.1/fastshopifyapi.egg-info/requires.txt
+-rw-r--r--   0 sokoslee   (501) staff       (20)       15 2023-07-30 09:40:29.000000 fastshopifyapi-2.0.1/fastshopifyapi.egg-info/top_level.txt
+-rw-r--r--   0 sokoslee   (501) staff       (20)      750 2023-07-30 09:39:44.000000 fastshopifyapi-2.0.1/pyproject.toml
+-rw-r--r--   0 sokoslee   (501) staff       (20)      285 2023-07-30 09:40:29.838775 fastshopifyapi-2.0.1/setup.cfg
+-rw-r--r--   0 sokoslee   (501) staff       (20)     1176 2023-07-30 08:54:23.000000 fastshopifyapi-2.0.1/setup.py
```

### Comparing `fastshopifyapi-2.0.0/LICENSE` & `fastshopifyapi-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastshopifyapi-2.0.0/PKG-INFO` & `fastshopifyapi-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastshopifyapi
-Version: 2.0.0
+Version: 2.0.1
 Summary: A read-to-use sync/async client for REST and GraphQL API calls to Shopify's API
 Home-page: https://github.com/sokoslee/FastShopifyApi
 Author: Sokos Lee
 Author-email: Tyler King <tyler@osiset.com>, Sokos Lee <SokosLee@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/sokoslee/FastShopifyApi
 Project-URL: Bug Tracker, https://github.com/sokoslee/FastShopifyApi/issues
@@ -17,20 +17,27 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FastShopifyApi
 
-![Tests](https://github.com/osiset/basic_shopify_api/workflows/Package%20Test/badge.svg?branch=master)
-[![Coverage](https://coveralls.io/repos/github/osiset/basic_shopify_api/badge.svg?branch=master)](https://coveralls.io/github/osiset/basic_shopify_api?branch=master)
-[![PyPi version](https://badge.fury.io/py/basic-shopify-api.svg)](https://pypi.org/project/basic-shopify-api)
+![Tests](https://github.com/sokoslee/FastShopifyApi/workflows/Package%20Test/badge.svg?branch=master)
+[![Coverage](https://coveralls.io/repos/github/osiset/basic_shopify_api/badge.svg?branch=master)](https://coveralls.io/sokoslee/FastShopifyApi?branch=master)
+[![PyPi version](https://badge.fury.io/py/basic-shopify-api.svg)](https://pypi.org/project/fastshopifyapi/)
 
 This library extends HTTPX and implements a read-to-use sync/async client for REST and GraphQL API calls to Shopify's API.
 
+Fork from [osiset/basic_shopify_api](https://github.com/gnikyt/basic_shopify_api) with the following changes:
+- Rename `basic_shopify_api` to `FastShopifyApi`
+- Upgrade Shopify API version
+- Fixed some bugs
+
+**Thanks to [Tyler King](https://github.com/gnikyt/basic_shopify_api) for his work.**
+
 Support for:
 
 - [X] Sync and async API calls
 - [X] REST API
 - [X] GraphQL API
 - [X] REST rate limiting
 - [X] GraphQL cost limiting
```

### Comparing `fastshopifyapi-2.0.0/README.md` & `fastshopifyapi-2.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 # FastShopifyApi
 
-![Tests](https://github.com/osiset/basic_shopify_api/workflows/Package%20Test/badge.svg?branch=master)
-[![Coverage](https://coveralls.io/repos/github/osiset/basic_shopify_api/badge.svg?branch=master)](https://coveralls.io/github/osiset/basic_shopify_api?branch=master)
-[![PyPi version](https://badge.fury.io/py/basic-shopify-api.svg)](https://pypi.org/project/basic-shopify-api)
+![Tests](https://github.com/sokoslee/FastShopifyApi/workflows/Package%20Test/badge.svg?branch=master)
+[![Coverage](https://coveralls.io/repos/github/osiset/basic_shopify_api/badge.svg?branch=master)](https://coveralls.io/sokoslee/FastShopifyApi?branch=master)
+[![PyPi version](https://badge.fury.io/py/basic-shopify-api.svg)](https://pypi.org/project/fastshopifyapi/)
 
 This library extends HTTPX and implements a read-to-use sync/async client for REST and GraphQL API calls to Shopify's API.
 
+Fork from [osiset/basic_shopify_api](https://github.com/gnikyt/basic_shopify_api) with the following changes:
+- Rename `basic_shopify_api` to `FastShopifyApi`
+- Upgrade Shopify API version
+- Fixed some bugs
+
+**Thanks to [Tyler King](https://github.com/gnikyt/basic_shopify_api) for his work.**
+
 Support for:
 
 - [X] Sync and async API calls
 - [X] REST API
 - [X] GraphQL API
 - [X] REST rate limiting
 - [X] GraphQL cost limiting
```

### Comparing `fastshopifyapi-2.0.0/fastshopifyapi/clients/async_client.py` & `fastshopifyapi-2.0.1/fastshopifyapi/clients/async_client.py`

 * *Files identical despite different names*

### Comparing `fastshopifyapi-2.0.0/fastshopifyapi/clients/client.py` & `fastshopifyapi-2.0.1/fastshopifyapi/clients/client.py`

 * *Files identical despite different names*

### Comparing `fastshopifyapi-2.0.0/fastshopifyapi/clients/common.py` & `fastshopifyapi-2.0.1/fastshopifyapi/clients/common.py`

 * *Files identical despite different names*

### Comparing `fastshopifyapi-2.0.0/fastshopifyapi/constants.py` & `fastshopifyapi-2.0.1/fastshopifyapi/constants.py`

 * *Files identical despite different names*

### Comparing `fastshopifyapi-2.0.0/fastshopifyapi/deferrer.py` & `fastshopifyapi-2.0.1/fastshopifyapi/deferrer.py`

 * *Files identical despite different names*

### Comparing `fastshopifyapi-2.0.0/fastshopifyapi/models.py` & `fastshopifyapi-2.0.1/fastshopifyapi/models.py`

 * *Files identical despite different names*

### Comparing `fastshopifyapi-2.0.0/fastshopifyapi/options.py` & `fastshopifyapi-2.0.1/fastshopifyapi/options.py`

 * *Files identical despite different names*

### Comparing `fastshopifyapi-2.0.0/fastshopifyapi/store.py` & `fastshopifyapi-2.0.1/fastshopifyapi/store.py`

 * *Files identical despite different names*

### Comparing `fastshopifyapi-2.0.0/fastshopifyapi/types.py` & `fastshopifyapi-2.0.1/fastshopifyapi/types.py`

 * *Files identical despite different names*

### Comparing `fastshopifyapi-2.0.0/fastshopifyapi/utils.py` & `fastshopifyapi-2.0.1/fastshopifyapi/utils.py`

 * *Files identical despite different names*

### Comparing `fastshopifyapi-2.0.0/fastshopifyapi.egg-info/PKG-INFO` & `fastshopifyapi-2.0.1/fastshopifyapi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastshopifyapi
-Version: 2.0.0
+Version: 2.0.1
 Summary: A read-to-use sync/async client for REST and GraphQL API calls to Shopify's API
 Home-page: https://github.com/sokoslee/FastShopifyApi
 Author: Sokos Lee
 Author-email: Tyler King <tyler@osiset.com>, Sokos Lee <SokosLee@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/sokoslee/FastShopifyApi
 Project-URL: Bug Tracker, https://github.com/sokoslee/FastShopifyApi/issues
@@ -17,20 +17,27 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FastShopifyApi
 
-![Tests](https://github.com/osiset/basic_shopify_api/workflows/Package%20Test/badge.svg?branch=master)
-[![Coverage](https://coveralls.io/repos/github/osiset/basic_shopify_api/badge.svg?branch=master)](https://coveralls.io/github/osiset/basic_shopify_api?branch=master)
-[![PyPi version](https://badge.fury.io/py/basic-shopify-api.svg)](https://pypi.org/project/basic-shopify-api)
+![Tests](https://github.com/sokoslee/FastShopifyApi/workflows/Package%20Test/badge.svg?branch=master)
+[![Coverage](https://coveralls.io/repos/github/osiset/basic_shopify_api/badge.svg?branch=master)](https://coveralls.io/sokoslee/FastShopifyApi?branch=master)
+[![PyPi version](https://badge.fury.io/py/basic-shopify-api.svg)](https://pypi.org/project/fastshopifyapi/)
 
 This library extends HTTPX and implements a read-to-use sync/async client for REST and GraphQL API calls to Shopify's API.
 
+Fork from [osiset/basic_shopify_api](https://github.com/gnikyt/basic_shopify_api) with the following changes:
+- Rename `basic_shopify_api` to `FastShopifyApi`
+- Upgrade Shopify API version
+- Fixed some bugs
+
+**Thanks to [Tyler King](https://github.com/gnikyt/basic_shopify_api) for his work.**
+
 Support for:
 
 - [X] Sync and async API calls
 - [X] REST API
 - [X] GraphQL API
 - [X] REST rate limiting
 - [X] GraphQL cost limiting
```

### Comparing `fastshopifyapi-2.0.0/fastshopifyapi.egg-info/SOURCES.txt` & `fastshopifyapi-2.0.1/fastshopifyapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastshopifyapi-2.0.0/pyproject.toml` & `fastshopifyapi-2.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fastshopifyapi"
-version = "2.0.0"
+version = "2.0.1"
 authors = [
   { name="Tyler King", email="tyler@osiset.com" },
   { name="Sokos Lee", email="SokosLee@gmail.com" }
 ]
 description = "A read-to-use sync/async client for REST and GraphQL API calls to Shopify's API"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `fastshopifyapi-2.0.0/setup.py` & `fastshopifyapi-2.0.1/setup.py`

 * *Files identical despite different names*

