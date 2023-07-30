# Comparing `tmp/heybooster-toolkit-0.0.39.tar.gz` & `tmp/heybooster-toolkit-0.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/abdullahkulcu/Desktop/heybooster/heybooster-toolkit/dist/.tmp-sebpjsf5/heybooster-toolkit-0.0.39.tar", last modified: Tue Jun 13 09:22:36 2023, max compression
+gzip compressed data, was "/Users/abdullahkulcu/Desktop/heybooster/heybooster-toolkit/dist/.tmp-v2_aab1g/heybooster-toolkit-0.0.40.tar", last modified: Sun Jul 30 02:35:25 2023, max compression
```

## Comparing `heybooster-toolkit-0.0.39.tar` & `heybooster-toolkit-0.0.40.tar`

### file list

```diff
@@ -1,38 +1,43 @@
-drwxr-xr-x   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:22:36.000000 heybooster-toolkit-0.0.39/
--rw-r--r--   0 abdullahkulcu   (501) staff       (20)     1067 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/LICENSE
--rw-r--r--   0 abdullahkulcu   (501) staff       (20)       83 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/MANIFEST.in
--rw-r--r--   0 abdullahkulcu   (501) staff       (20)     1482 2023-06-13 09:22:36.000000 heybooster-toolkit-0.0.39/PKG-INFO
--rw-r--r--   0 abdullahkulcu   (501) staff       (20)      964 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/README.md
-drwxr-xr-x   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:22:36.000000 heybooster-toolkit-0.0.39/heybooster/
--rw-r--r--   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/heybooster/__init__.py
-drwxr-xr-x   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:22:36.000000 heybooster-toolkit-0.0.39/heybooster/exception/
--rw-r--r--   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/heybooster/exception/__init__.py
--rw-r--r--   0 abdullahkulcu   (501) staff       (20)     2594 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/heybooster/exception/exception_catcher.py
-drwxr-xr-x   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:22:36.000000 heybooster-toolkit-0.0.39/heybooster/helpers/
--rw-r--r--   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/heybooster/helpers/__init__.py
-drwxr-xr-x   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:22:36.000000 heybooster-toolkit-0.0.39/heybooster/helpers/database/
--rw-r--r--   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/heybooster/helpers/database/__init__.py
--rw-r--r--   0 abdullahkulcu   (501) staff       (20)     5794 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/heybooster/helpers/database/mongodb.py
--rw-r--r--   0 abdullahkulcu   (501) staff       (20)     3677 2023-06-13 09:19:04.000000 heybooster-toolkit-0.0.39/heybooster/helpers/database/opensearch.py
--rw-r--r--   0 abdullahkulcu   (501) staff       (20)     3285 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/heybooster/helpers/database/postgre.py
-drwxr-xr-x   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:22:36.000000 heybooster-toolkit-0.0.39/heybooster/helpers/email/
--rw-r--r--   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/heybooster/helpers/email/__init__.py
--rw-r--r--   0 abdullahkulcu   (501) staff       (20)     4835 2023-06-13 09:21:34.000000 heybooster-toolkit-0.0.39/heybooster/helpers/email/sendpulse.py
-drwxr-xr-x   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:22:36.000000 heybooster-toolkit-0.0.39/heybooster/helpers/email/statics/
--rw-r--r--   0 abdullahkulcu   (501) staff       (20)      109 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/heybooster/helpers/email/statics/__init__.py
-drwxr-xr-x   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:22:36.000000 heybooster-toolkit-0.0.39/heybooster/helpers/email/utils/
--rw-r--r--   0 abdullahkulcu   (501) staff       (20)      360 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/heybooster/helpers/email/utils/__init__.py
-drwxr-xr-x   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:22:36.000000 heybooster-toolkit-0.0.39/heybooster/helpers/hubspot/
--rw-r--r--   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/heybooster/helpers/hubspot/__init__.py
--rw-r--r--   0 abdullahkulcu   (501) staff       (20)     4267 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/heybooster/helpers/hubspot/contacts.py
-drwxr-xr-x   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:22:36.000000 heybooster-toolkit-0.0.39/heybooster_toolkit.egg-info/
--rw-r--r--   0 abdullahkulcu   (501) staff       (20)     1482 2023-06-13 09:22:36.000000 heybooster-toolkit-0.0.39/heybooster_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 abdullahkulcu   (501) staff       (20)      822 2023-06-13 09:22:36.000000 heybooster-toolkit-0.0.39/heybooster_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 abdullahkulcu   (501) staff       (20)        1 2023-06-13 09:22:36.000000 heybooster-toolkit-0.0.39/heybooster_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 abdullahkulcu   (501) staff       (20)       39 2023-06-13 09:22:36.000000 heybooster-toolkit-0.0.39/heybooster_toolkit.egg-info/requires.txt
--rw-r--r--   0 abdullahkulcu   (501) staff       (20)       11 2023-06-13 09:22:36.000000 heybooster-toolkit-0.0.39/heybooster_toolkit.egg-info/top_level.txt
--rw-r--r--   0 abdullahkulcu   (501) staff       (20)      103 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/pyproject.toml
--rw-r--r--   0 abdullahkulcu   (501) staff       (20)       38 2023-06-13 09:22:36.000000 heybooster-toolkit-0.0.39/setup.cfg
--rw-r--r--   0 abdullahkulcu   (501) staff       (20)      960 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/setup.py
--rw-r--r--   0 abdullahkulcu   (501) staff       (20)        6 2023-06-13 09:22:27.000000 heybooster-toolkit-0.0.39/version.txt
--rw-r--r--   0 abdullahkulcu   (501) staff       (20)      341 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/version_update.py
+drwxr-xr-x   0 abdullahkulcu   (501) staff       (20)        0 2023-07-30 02:35:25.000000 heybooster-toolkit-0.0.40/
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)     1067 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.40/LICENSE
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)       83 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.40/MANIFEST.in
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)     1482 2023-07-30 02:35:25.000000 heybooster-toolkit-0.0.40/PKG-INFO
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)      964 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.40/README.md
+drwxr-xr-x   0 abdullahkulcu   (501) staff       (20)        0 2023-07-30 02:35:25.000000 heybooster-toolkit-0.0.40/heybooster/
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.40/heybooster/__init__.py
+drwxr-xr-x   0 abdullahkulcu   (501) staff       (20)        0 2023-07-30 02:35:25.000000 heybooster-toolkit-0.0.40/heybooster/exception/
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.40/heybooster/exception/__init__.py
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)     2594 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.40/heybooster/exception/exception_catcher.py
+drwxr-xr-x   0 abdullahkulcu   (501) staff       (20)        0 2023-07-30 02:35:25.000000 heybooster-toolkit-0.0.40/heybooster/helpers/
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.40/heybooster/helpers/__init__.py
+drwxr-xr-x   0 abdullahkulcu   (501) staff       (20)        0 2023-07-30 02:35:25.000000 heybooster-toolkit-0.0.40/heybooster/helpers/database/
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.40/heybooster/helpers/database/__init__.py
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)     5794 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.40/heybooster/helpers/database/mongodb.py
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)     3677 2023-06-13 09:19:04.000000 heybooster-toolkit-0.0.40/heybooster/helpers/database/opensearch.py
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)     3285 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.40/heybooster/helpers/database/postgre.py
+drwxr-xr-x   0 abdullahkulcu   (501) staff       (20)        0 2023-07-30 02:35:25.000000 heybooster-toolkit-0.0.40/heybooster/helpers/email/
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.40/heybooster/helpers/email/__init__.py
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)     4835 2023-06-13 09:21:34.000000 heybooster-toolkit-0.0.40/heybooster/helpers/email/sendpulse.py
+drwxr-xr-x   0 abdullahkulcu   (501) staff       (20)        0 2023-07-30 02:35:25.000000 heybooster-toolkit-0.0.40/heybooster/helpers/email/statics/
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)      109 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.40/heybooster/helpers/email/statics/__init__.py
+drwxr-xr-x   0 abdullahkulcu   (501) staff       (20)        0 2023-07-30 02:35:25.000000 heybooster-toolkit-0.0.40/heybooster/helpers/email/utils/
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)      360 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.40/heybooster/helpers/email/utils/__init__.py
+drwxr-xr-x   0 abdullahkulcu   (501) staff       (20)        0 2023-07-30 02:35:25.000000 heybooster-toolkit-0.0.40/heybooster/helpers/hubspot/
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.40/heybooster/helpers/hubspot/__init__.py
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)     4267 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.40/heybooster/helpers/hubspot/contacts.py
+drwxr-xr-x   0 abdullahkulcu   (501) staff       (20)        0 2023-07-30 02:35:25.000000 heybooster-toolkit-0.0.40/heybooster/logger/
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)        0 2023-07-30 01:05:58.000000 heybooster-toolkit-0.0.40/heybooster/logger/__init__.py
+drwxr-xr-x   0 abdullahkulcu   (501) staff       (20)        0 2023-07-30 02:35:25.000000 heybooster-toolkit-0.0.40/heybooster/logger/cloudwatch/
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)        0 2023-07-30 01:06:15.000000 heybooster-toolkit-0.0.40/heybooster/logger/cloudwatch/__init__.py
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)     3081 2023-07-30 02:05:26.000000 heybooster-toolkit-0.0.40/heybooster/logger/cloudwatch/cloudwatch_logger.py
+drwxr-xr-x   0 abdullahkulcu   (501) staff       (20)        0 2023-07-30 02:35:25.000000 heybooster-toolkit-0.0.40/heybooster_toolkit.egg-info/
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)     1482 2023-07-30 02:35:25.000000 heybooster-toolkit-0.0.40/heybooster_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)      943 2023-07-30 02:35:25.000000 heybooster-toolkit-0.0.40/heybooster_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)        1 2023-07-30 02:35:25.000000 heybooster-toolkit-0.0.40/heybooster_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)       54 2023-07-30 02:35:25.000000 heybooster-toolkit-0.0.40/heybooster_toolkit.egg-info/requires.txt
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)       11 2023-07-30 02:35:25.000000 heybooster-toolkit-0.0.40/heybooster_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)      103 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.40/pyproject.toml
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)       38 2023-07-30 02:35:25.000000 heybooster-toolkit-0.0.40/setup.cfg
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)      986 2023-07-30 02:34:39.000000 heybooster-toolkit-0.0.40/setup.py
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)        6 2023-07-30 02:35:20.000000 heybooster-toolkit-0.0.40/version.txt
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)      341 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.40/version_update.py
```

### Comparing `heybooster-toolkit-0.0.39/LICENSE` & `heybooster-toolkit-0.0.40/LICENSE`

 * *Files identical despite different names*

### Comparing `heybooster-toolkit-0.0.39/PKG-INFO` & `heybooster-toolkit-0.0.40/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heybooster-toolkit
-Version: 0.0.39
+Version: 0.0.40
 Summary: Heybooster Toolkit
 Home-page: https://github.com/hey-booster/heybooster-toolkit
 Author: Heybooster
 Author-email: hey@heybooster.ai
 Project-URL: Bug Tracker, https://github.com/hey-booster/heybooster-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `heybooster-toolkit-0.0.39/README.md` & `heybooster-toolkit-0.0.40/README.md`

 * *Files identical despite different names*

### Comparing `heybooster-toolkit-0.0.39/heybooster/exception/exception_catcher.py` & `heybooster-toolkit-0.0.40/heybooster/exception/exception_catcher.py`

 * *Files identical despite different names*

### Comparing `heybooster-toolkit-0.0.39/heybooster/helpers/database/mongodb.py` & `heybooster-toolkit-0.0.40/heybooster/helpers/database/mongodb.py`

 * *Files identical despite different names*

### Comparing `heybooster-toolkit-0.0.39/heybooster/helpers/database/opensearch.py` & `heybooster-toolkit-0.0.40/heybooster/helpers/database/opensearch.py`

 * *Files identical despite different names*

### Comparing `heybooster-toolkit-0.0.39/heybooster/helpers/database/postgre.py` & `heybooster-toolkit-0.0.40/heybooster/helpers/database/postgre.py`

 * *Files identical despite different names*

### Comparing `heybooster-toolkit-0.0.39/heybooster/helpers/email/sendpulse.py` & `heybooster-toolkit-0.0.40/heybooster/helpers/email/sendpulse.py`

 * *Files identical despite different names*

### Comparing `heybooster-toolkit-0.0.39/heybooster/helpers/hubspot/contacts.py` & `heybooster-toolkit-0.0.40/heybooster/helpers/hubspot/contacts.py`

 * *Files identical despite different names*

### Comparing `heybooster-toolkit-0.0.39/heybooster_toolkit.egg-info/PKG-INFO` & `heybooster-toolkit-0.0.40/heybooster_toolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heybooster-toolkit
-Version: 0.0.39
+Version: 0.0.40
 Summary: Heybooster Toolkit
 Home-page: https://github.com/hey-booster/heybooster-toolkit
 Author: Heybooster
 Author-email: hey@heybooster.ai
 Project-URL: Bug Tracker, https://github.com/hey-booster/heybooster-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `heybooster-toolkit-0.0.39/heybooster_toolkit.egg-info/SOURCES.txt` & `heybooster-toolkit-0.0.40/heybooster_toolkit.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -15,12 +15,15 @@
 heybooster/helpers/database/postgre.py
 heybooster/helpers/email/__init__.py
 heybooster/helpers/email/sendpulse.py
 heybooster/helpers/email/statics/__init__.py
 heybooster/helpers/email/utils/__init__.py
 heybooster/helpers/hubspot/__init__.py
 heybooster/helpers/hubspot/contacts.py
+heybooster/logger/__init__.py
+heybooster/logger/cloudwatch/__init__.py
+heybooster/logger/cloudwatch/cloudwatch_logger.py
 heybooster_toolkit.egg-info/PKG-INFO
 heybooster_toolkit.egg-info/SOURCES.txt
 heybooster_toolkit.egg-info/dependency_links.txt
 heybooster_toolkit.egg-info/requires.txt
 heybooster_toolkit.egg-info/top_level.txt
```

### Comparing `heybooster-toolkit-0.0.39/setup.py` & `heybooster-toolkit-0.0.40/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,11 +23,12 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         'pymongo==3.10.1',
         'requests',
-        'raven==6.10.0'
+        'raven==6.10.0',
+        'boto3==1.28.15'
     ],
     python_requires=">=3.6",
 )
```

