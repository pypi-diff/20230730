# Comparing `tmp/stigg_api_client-0.509.0.tar.gz` & `tmp/stigg_api_client-0.512.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client-0.509.0.tar", max compression
+gzip compressed data, was "stigg_api_client-0.512.0.tar", max compression
```

## Comparing `stigg_api_client-0.509.0.tar` & `stigg_api_client-0.512.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2479 2023-07-27 07:09:22.270223 stigg_api_client-0.509.0/README.md
--rw-r--r--   0        0        0      460 2023-07-27 07:09:55.634335 stigg_api_client-0.509.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-07-27 07:09:22.270223 stigg_api_client-0.509.0/stigg/__init__.py
--rw-r--r--   0        0        0     1141 2023-07-27 07:09:22.270223 stigg_api_client-0.509.0/stigg/client.py
--rw-r--r--   0        0        0        0 2023-07-27 07:09:53.722333 stigg_api_client-0.509.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0    51059 2023-07-27 07:09:54.142334 stigg_api_client-0.509.0/stigg/generated/operations.py
--rw-r--r--   0        0        0   467141 2023-07-27 07:09:53.986334 stigg_api_client-0.509.0/stigg/generated/schema.py
--rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 stigg_api_client-0.509.0/PKG-INFO
+-rw-r--r--   0        0        0     2479 2023-07-30 10:08:16.305889 stigg_api_client-0.512.0/README.md
+-rw-r--r--   0        0        0      480 2023-07-30 10:09:02.802063 stigg_api_client-0.512.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-07-30 10:08:16.305889 stigg_api_client-0.512.0/stigg/__init__.py
+-rw-r--r--   0        0        0     3699 2023-07-30 10:08:16.305889 stigg_api_client-0.512.0/stigg/client.py
+-rw-r--r--   0        0        0        0 2023-07-30 10:09:00.326046 stigg_api_client-0.512.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0    51059 2023-07-30 10:09:00.866050 stigg_api_client-0.512.0/stigg/generated/operations.py
+-rw-r--r--   0        0        0   467141 2023-07-30 10:09:00.666049 stigg_api_client-0.512.0/stigg/generated/schema.py
+-rw-r--r--   0        0        0     3122 1970-01-01 00:00:00.000000 stigg_api_client-0.512.0/PKG-INFO
```

### Comparing `stigg_api_client-0.509.0/README.md` & `stigg_api_client-0.512.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.509.0/stigg/generated/operations.py` & `stigg_api_client-0.512.0/stigg/generated/operations.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.509.0/stigg/generated/schema.py` & `stigg_api_client-0.512.0/stigg/generated/schema.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client-0.509.0/PKG-INFO` & `stigg_api_client-0.512.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: stigg-api-client
-Version: 0.509.0
+Version: 0.512.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: graphql-core (>=3.1,<4.0)
 Requires-Dist: requests (>=2.28,<3.0)
 Requires-Dist: sgqlc (>=16.0,<17.0)
+Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Description-Content-Type: text/markdown
 
 # stigg-api-client
 
 This library provides a Python wrapper to [Stigg's GraphQL API](https://docs.stigg.io/docs/graphql-api) based on 
 the operations that are in use by the [Stigg's Node.js SDK](https://docs.stigg.io/docs/nodejs-sdk).
```

