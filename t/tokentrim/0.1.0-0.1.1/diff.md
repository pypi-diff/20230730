# Comparing `tmp/tokentrim-0.1.0.tar.gz` & `tmp/tokentrim-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokentrim-0.1.0.tar", max compression
+gzip compressed data, was "tokentrim-0.1.1.tar", max compression
```

## Comparing `tokentrim-0.1.0.tar` & `tokentrim-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1064 2023-07-29 23:24:50.484214 tokentrim-0.1.0/LICENSE
--rw-r--r--   0        0        0      355 2023-07-29 23:57:17.425776 tokentrim-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        1 2023-07-29 23:31:32.250252 tokentrim-0.1.0/tokentrim/__init__.py
--rw-r--r--   0        0        0     5428 2023-07-29 23:50:44.552404 tokentrim-0.1.0/tokentrim/tokentrim.py
--rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 tokentrim-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-29 23:24:50.484214 tokentrim-0.1.1/LICENSE
+-rw-r--r--   0        0        0      355 2023-07-30 00:07:03.345546 tokentrim-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-07-30 00:06:48.037573 tokentrim-0.1.1/tokentrim/__init__.py
+-rw-r--r--   0        0        0     5428 2023-07-29 23:50:44.552404 tokentrim-0.1.1/tokentrim/tokentrim.py
+-rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 tokentrim-0.1.1/PKG-INFO
```

### Comparing `tokentrim-0.1.0/LICENSE` & `tokentrim-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tokentrim-0.1.0/tokentrim/tokentrim.py` & `tokentrim-0.1.1/tokentrim/tokentrim.py`

 * *Files identical despite different names*

### Comparing `tokentrim-0.1.0/PKG-INFO` & `tokentrim-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokentrim
-Version: 0.1.0
+Version: 0.1.1
 Summary: Easily trim 'messages' arrays for use with GPTs.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

