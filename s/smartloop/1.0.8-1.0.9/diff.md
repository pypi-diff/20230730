# Comparing `tmp/smartloop-1.0.8.tar.gz` & `tmp/smartloop-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartloop-1.0.8.tar", last modified: Sat Jul 29 23:57:01 2023, max compression
+gzip compressed data, was "smartloop-1.0.9.tar", last modified: Sun Jul 30 00:47:53 2023, max compression
```

## Comparing `smartloop-1.0.8.tar` & `smartloop-1.0.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-29 23:57:01.104844 smartloop-1.0.8/
--rw-r--r--   0 mehfuz     (501) staff       (20)     1065 2023-06-20 05:48:15.000000 smartloop-1.0.8/LICENSE.txt
--rw-r--r--   0 mehfuz     (501) staff       (20)       24 2022-06-27 05:07:42.000000 smartloop-1.0.8/MANIFEST.in
--rw-r--r--   0 mehfuz     (501) staff       (20)     5493 2023-07-29 23:57:01.104900 smartloop-1.0.8/PKG-INFO
--rw-r--r--   0 mehfuz     (501) staff       (20)     4704 2023-07-29 22:44:02.000000 smartloop-1.0.8/README.md
-drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-29 23:57:01.100501 smartloop-1.0.8/data/
--rw-r--r--   0 mehfuz     (501) staff       (20)    19738 2023-07-20 21:20:54.000000 smartloop-1.0.8/data/sample.json
--rw-r--r--   0 mehfuz     (501) staff       (20)       79 2023-07-29 23:57:01.105088 smartloop-1.0.8/setup.cfg
--rw-r--r--   0 mehfuz     (501) staff       (20)     1484 2023-07-29 22:45:01.000000 smartloop-1.0.8/setup.py
-drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-29 23:57:01.101047 smartloop-1.0.8/smartloop/
--rw-r--r--   0 mehfuz     (501) staff       (20)       82 2023-07-29 21:50:58.000000 smartloop-1.0.8/smartloop/__init__.py
-drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-29 23:57:01.103755 smartloop-1.0.8/smartloop/core/
--rw-r--r--   0 mehfuz     (501) staff       (20)      314 2023-07-29 00:57:56.000000 smartloop-1.0.8/smartloop/core/__init__.py
--rw-r--r--   0 mehfuz     (501) staff       (20)      171 2022-06-27 05:07:42.000000 smartloop-1.0.8/smartloop/core/classifier.py
--rw-r--r--   0 mehfuz     (501) staff       (20)      387 2023-01-06 20:04:52.000000 smartloop-1.0.8/smartloop/core/config.py
--rw-r--r--   0 mehfuz     (501) staff       (20)      109 2022-06-01 06:34:59.000000 smartloop-1.0.8/smartloop/core/default_config.py
-drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-29 23:57:01.104063 smartloop-1.0.8/smartloop/core/errors/
--rw-r--r--   0 mehfuz     (501) staff       (20)       41 2022-08-05 16:36:45.000000 smartloop-1.0.8/smartloop/core/errors/__init__.py
--rw-r--r--   0 mehfuz     (501) staff       (20)       69 2022-08-05 16:36:45.000000 smartloop-1.0.8/smartloop/core/errors/mode_not_found.py
--rw-r--r--   0 mehfuz     (501) staff       (20)      229 2022-06-01 06:34:59.000000 smartloop-1.0.8/smartloop/core/file_config.py
--rw-r--r--   0 mehfuz     (501) staff       (20)      904 2022-08-25 21:26:36.000000 smartloop-1.0.8/smartloop/core/label_parser.py
--rw-r--r--   0 mehfuz     (501) staff       (20)     1428 2023-05-03 01:19:44.000000 smartloop-1.0.8/smartloop/core/model_loader.py
-drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-29 23:57:01.104168 smartloop-1.0.8/smartloop/core/nlu/
--rw-r--r--   0 mehfuz     (501) staff       (20)       47 2022-06-01 06:34:59.000000 smartloop-1.0.8/smartloop/core/nlu/__init__.py
-drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-29 23:57:01.104408 smartloop-1.0.8/smartloop/core/nlu/callbacks/
--rw-r--r--   0 mehfuz     (501) staff       (20)       51 2022-06-27 05:07:42.000000 smartloop-1.0.8/smartloop/core/nlu/callbacks/__init__.py
--rw-r--r--   0 mehfuz     (501) staff       (20)     1217 2022-06-27 05:07:42.000000 smartloop-1.0.8/smartloop/core/nlu/callbacks/train_status_report.py
-drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-29 23:57:01.104637 smartloop-1.0.8/smartloop/core/nlu/classifiers/
--rw-r--r--   0 mehfuz     (501) staff       (20)       67 2022-06-27 05:07:42.000000 smartloop-1.0.8/smartloop/core/nlu/classifiers/__init__.py
--rw-r--r--   0 mehfuz     (501) staff       (20)     6826 2023-07-29 23:53:46.000000 smartloop-1.0.8/smartloop/core/nlu/classifiers/embedding_intent_classifier.py
--rw-r--r--   0 mehfuz     (501) staff       (20)     1826 2023-07-29 01:12:09.000000 smartloop-1.0.8/smartloop/core/project.py
--rw-r--r--   0 mehfuz     (501) staff       (20)      730 2023-07-29 01:10:43.000000 smartloop-1.0.8/smartloop/core/sanitizer.py
--rw-r--r--   0 mehfuz     (501) staff       (20)     1621 2023-07-29 01:10:09.000000 smartloop-1.0.8/smartloop/core/text_classifier.py
--rw-r--r--   0 mehfuz     (501) staff       (20)      634 2023-07-29 01:02:33.000000 smartloop-1.0.8/smartloop/core/tokenizer.py
--rw-r--r--   0 mehfuz     (501) staff       (20)       22 2023-07-29 23:56:34.000000 smartloop-1.0.8/smartloop/version.py
-drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-29 23:57:01.101537 smartloop-1.0.8/smartloop.egg-info/
--rw-r--r--   0 mehfuz     (501) staff       (20)     5493 2023-07-29 23:57:00.000000 smartloop-1.0.8/smartloop.egg-info/PKG-INFO
--rw-r--r--   0 mehfuz     (501) staff       (20)      901 2023-07-29 23:57:01.000000 smartloop-1.0.8/smartloop.egg-info/SOURCES.txt
--rw-r--r--   0 mehfuz     (501) staff       (20)        1 2023-07-29 23:57:00.000000 smartloop-1.0.8/smartloop.egg-info/dependency_links.txt
--rw-r--r--   0 mehfuz     (501) staff       (20)       70 2023-07-29 23:57:00.000000 smartloop-1.0.8/smartloop.egg-info/requires.txt
--rw-r--r--   0 mehfuz     (501) staff       (20)       10 2023-07-29 23:57:01.000000 smartloop-1.0.8/smartloop.egg-info/top_level.txt
+drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-30 00:47:53.917250 smartloop-1.0.9/
+-rw-r--r--   0 mehfuz     (501) staff       (20)     1065 2023-06-20 05:48:15.000000 smartloop-1.0.9/LICENSE.txt
+-rw-r--r--   0 mehfuz     (501) staff       (20)       24 2022-06-27 05:07:42.000000 smartloop-1.0.9/MANIFEST.in
+-rw-r--r--   0 mehfuz     (501) staff       (20)     5493 2023-07-30 00:47:53.917309 smartloop-1.0.9/PKG-INFO
+-rw-r--r--   0 mehfuz     (501) staff       (20)     4704 2023-07-29 22:44:02.000000 smartloop-1.0.9/README.md
+drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-30 00:47:53.912633 smartloop-1.0.9/data/
+-rw-r--r--   0 mehfuz     (501) staff       (20)    19738 2023-07-20 21:20:54.000000 smartloop-1.0.9/data/sample.json
+-rw-r--r--   0 mehfuz     (501) staff       (20)       79 2023-07-30 00:47:53.917508 smartloop-1.0.9/setup.cfg
+-rw-r--r--   0 mehfuz     (501) staff       (20)     1484 2023-07-29 22:45:01.000000 smartloop-1.0.9/setup.py
+drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-30 00:47:53.913140 smartloop-1.0.9/smartloop/
+-rw-r--r--   0 mehfuz     (501) staff       (20)       70 2023-07-30 00:47:14.000000 smartloop-1.0.9/smartloop/__init__.py
+drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-30 00:47:53.915760 smartloop-1.0.9/smartloop/core/
+-rw-r--r--   0 mehfuz     (501) staff       (20)      314 2023-07-29 00:57:56.000000 smartloop-1.0.9/smartloop/core/__init__.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)      171 2022-06-27 05:07:42.000000 smartloop-1.0.9/smartloop/core/classifier.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)      387 2023-01-06 20:04:52.000000 smartloop-1.0.9/smartloop/core/config.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)      109 2022-06-01 06:34:59.000000 smartloop-1.0.9/smartloop/core/default_config.py
+drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-30 00:47:53.916101 smartloop-1.0.9/smartloop/core/errors/
+-rw-r--r--   0 mehfuz     (501) staff       (20)       41 2022-08-05 16:36:45.000000 smartloop-1.0.9/smartloop/core/errors/__init__.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)       69 2022-08-05 16:36:45.000000 smartloop-1.0.9/smartloop/core/errors/mode_not_found.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)      229 2022-06-01 06:34:59.000000 smartloop-1.0.9/smartloop/core/file_config.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)      904 2022-08-25 21:26:36.000000 smartloop-1.0.9/smartloop/core/label_parser.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)     1428 2023-05-03 01:19:44.000000 smartloop-1.0.9/smartloop/core/model_loader.py
+drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-30 00:47:53.916224 smartloop-1.0.9/smartloop/core/nlu/
+-rw-r--r--   0 mehfuz     (501) staff       (20)       47 2022-06-01 06:34:59.000000 smartloop-1.0.9/smartloop/core/nlu/__init__.py
+drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-30 00:47:53.916633 smartloop-1.0.9/smartloop/core/nlu/callbacks/
+-rw-r--r--   0 mehfuz     (501) staff       (20)       51 2022-06-27 05:07:42.000000 smartloop-1.0.9/smartloop/core/nlu/callbacks/__init__.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)     1217 2022-06-27 05:07:42.000000 smartloop-1.0.9/smartloop/core/nlu/callbacks/train_status_report.py
+drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-30 00:47:53.916972 smartloop-1.0.9/smartloop/core/nlu/classifiers/
+-rw-r--r--   0 mehfuz     (501) staff       (20)       67 2022-06-27 05:07:42.000000 smartloop-1.0.9/smartloop/core/nlu/classifiers/__init__.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)     6826 2023-07-29 23:53:46.000000 smartloop-1.0.9/smartloop/core/nlu/classifiers/embedding_intent_classifier.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)     1826 2023-07-29 01:12:09.000000 smartloop-1.0.9/smartloop/core/project.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)      730 2023-07-29 01:10:43.000000 smartloop-1.0.9/smartloop/core/sanitizer.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)     1621 2023-07-29 01:10:09.000000 smartloop-1.0.9/smartloop/core/text_classifier.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)      634 2023-07-29 01:02:33.000000 smartloop-1.0.9/smartloop/core/tokenizer.py
+-rw-r--r--   0 mehfuz     (501) staff       (20)       22 2023-07-30 00:47:27.000000 smartloop-1.0.9/smartloop/version.py
+drwxr-xr-x   0 mehfuz     (501) staff       (20)        0 2023-07-30 00:47:53.913624 smartloop-1.0.9/smartloop.egg-info/
+-rw-r--r--   0 mehfuz     (501) staff       (20)     5493 2023-07-30 00:47:53.000000 smartloop-1.0.9/smartloop.egg-info/PKG-INFO
+-rw-r--r--   0 mehfuz     (501) staff       (20)      901 2023-07-30 00:47:53.000000 smartloop-1.0.9/smartloop.egg-info/SOURCES.txt
+-rw-r--r--   0 mehfuz     (501) staff       (20)        1 2023-07-30 00:47:53.000000 smartloop-1.0.9/smartloop.egg-info/dependency_links.txt
+-rw-r--r--   0 mehfuz     (501) staff       (20)       70 2023-07-30 00:47:53.000000 smartloop-1.0.9/smartloop.egg-info/requires.txt
+-rw-r--r--   0 mehfuz     (501) staff       (20)       10 2023-07-30 00:47:53.000000 smartloop-1.0.9/smartloop.egg-info/top_level.txt
```

### Comparing `smartloop-1.0.8/LICENSE.txt` & `smartloop-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smartloop-1.0.8/PKG-INFO` & `smartloop-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartloop
-Version: 1.0.8
+Version: 1.0.9
 Summary: Natural language processing framework for text processing
 Home-page: https://github.com/SmartloopAI/sl-core
 Download-URL: https://github.com/SmartloopAI/sl-core/archive/refs/tags/1.0.1.tar.gz
 Author: Smartloop Inc.
 Author-email: mehfuz@smartloop.ai
 License: LICENSE.txt
 Keywords: NLP,framework,tensorflow,smartloop
```

### Comparing `smartloop-1.0.8/README.md` & `smartloop-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `smartloop-1.0.8/data/sample.json` & `smartloop-1.0.9/data/sample.json`

 * *Files identical despite different names*

### Comparing `smartloop-1.0.8/setup.py` & `smartloop-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `smartloop-1.0.8/smartloop/core/label_parser.py` & `smartloop-1.0.9/smartloop/core/label_parser.py`

 * *Files identical despite different names*

### Comparing `smartloop-1.0.8/smartloop/core/model_loader.py` & `smartloop-1.0.9/smartloop/core/model_loader.py`

 * *Files identical despite different names*

### Comparing `smartloop-1.0.8/smartloop/core/nlu/callbacks/train_status_report.py` & `smartloop-1.0.9/smartloop/core/nlu/callbacks/train_status_report.py`

 * *Files identical despite different names*

### Comparing `smartloop-1.0.8/smartloop/core/nlu/classifiers/embedding_intent_classifier.py` & `smartloop-1.0.9/smartloop/core/nlu/classifiers/embedding_intent_classifier.py`

 * *Files identical despite different names*

### Comparing `smartloop-1.0.8/smartloop/core/project.py` & `smartloop-1.0.9/smartloop/core/project.py`

 * *Files identical despite different names*

### Comparing `smartloop-1.0.8/smartloop/core/sanitizer.py` & `smartloop-1.0.9/smartloop/core/sanitizer.py`

 * *Files identical despite different names*

### Comparing `smartloop-1.0.8/smartloop/core/text_classifier.py` & `smartloop-1.0.9/smartloop/core/text_classifier.py`

 * *Files identical despite different names*

### Comparing `smartloop-1.0.8/smartloop/core/tokenizer.py` & `smartloop-1.0.9/smartloop/core/tokenizer.py`

 * *Files identical despite different names*

### Comparing `smartloop-1.0.8/smartloop.egg-info/PKG-INFO` & `smartloop-1.0.9/smartloop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartloop
-Version: 1.0.8
+Version: 1.0.9
 Summary: Natural language processing framework for text processing
 Home-page: https://github.com/SmartloopAI/sl-core
 Download-URL: https://github.com/SmartloopAI/sl-core/archive/refs/tags/1.0.1.tar.gz
 Author: Smartloop Inc.
 Author-email: mehfuz@smartloop.ai
 License: LICENSE.txt
 Keywords: NLP,framework,tensorflow,smartloop
```

### Comparing `smartloop-1.0.8/smartloop.egg-info/SOURCES.txt` & `smartloop-1.0.9/smartloop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

