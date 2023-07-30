# Comparing `tmp/openplugincore-0.6.0.tar.gz` & `tmp/openplugincore-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openplugincore-0.6.0.tar", last modified: Sun Jul 30 01:15:18 2023, max compression
+gzip compressed data, was "openplugincore-0.6.1.tar", last modified: Sun Jul 30 02:24:33 2023, max compression
```

## Comparing `openplugincore-0.6.0.tar` & `openplugincore-0.6.1.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:15:18.455580 openplugincore-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-30 01:15:18.455580 openplugincore-0.6.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:15:18.451580 openplugincore-0.6.0/openplugincore/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-30 01:15:07.000000 openplugincore-0.6.0/openplugincore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-07-30 01:15:07.000000 openplugincore-0.6.0/openplugincore/openplugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-30 01:15:07.000000 openplugincore-0.6.0/openplugincore/openplugin_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-30 01:15:07.000000 openplugincore-0.6.0/openplugincore/openplugin_memo.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-30 01:15:07.000000 openplugincore-0.6.0/openplugincore/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:15:18.451580 openplugincore-0.6.0/openplugincore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-30 01:15:18.000000 openplugincore-0.6.0/openplugincore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-30 01:15:18.000000 openplugincore-0.6.0/openplugincore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 01:15:18.000000 openplugincore-0.6.0/openplugincore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-30 01:15:18.000000 openplugincore-0.6.0/openplugincore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-30 01:15:18.000000 openplugincore-0.6.0/openplugincore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 01:15:18.455580 openplugincore-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-30 01:15:07.000000 openplugincore-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:15:18.455580 openplugincore-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 01:15:07.000000 openplugincore-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-30 01:15:07.000000 openplugincore-0.6.0/tests/mock_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11443 2023-07-30 01:15:07.000000 openplugincore-0.6.0/tests/test_e2e.py
--rw-r--r--   0 runner    (1001) docker     (123)    13061 2023-07-30 01:15:07.000000 openplugincore-0.6.0/tests/test_openplugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-30 01:15:07.000000 openplugincore-0.6.0/tests/test_openplugin_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-30 01:15:07.000000 openplugincore-0.6.0/tests/test_openplugin_memo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:24:33.622072 openplugincore-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-30 02:24:33.622072 openplugincore-0.6.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:24:33.622072 openplugincore-0.6.1/openplugincore/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-30 02:24:19.000000 openplugincore-0.6.1/openplugincore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-07-30 02:24:19.000000 openplugincore-0.6.1/openplugincore/openplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-30 02:24:19.000000 openplugincore-0.6.1/openplugincore/openplugin_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-30 02:24:19.000000 openplugincore-0.6.1/openplugincore/openplugin_memo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-30 02:24:19.000000 openplugincore-0.6.1/openplugincore/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:24:33.622072 openplugincore-0.6.1/openplugincore/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 02:24:19.000000 openplugincore-0.6.1/openplugincore/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-30 02:24:19.000000 openplugincore-0.6.1/openplugincore/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-30 02:24:19.000000 openplugincore-0.6.1/openplugincore/utils/prompting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:24:33.622072 openplugincore-0.6.1/openplugincore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-30 02:24:33.000000 openplugincore-0.6.1/openplugincore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-30 02:24:33.000000 openplugincore-0.6.1/openplugincore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 02:24:33.000000 openplugincore-0.6.1/openplugincore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-30 02:24:33.000000 openplugincore-0.6.1/openplugincore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-30 02:24:33.000000 openplugincore-0.6.1/openplugincore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 02:24:33.622072 openplugincore-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-30 02:24:19.000000 openplugincore-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:24:33.622072 openplugincore-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 02:24:19.000000 openplugincore-0.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-30 02:24:19.000000 openplugincore-0.6.1/tests/mock_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11443 2023-07-30 02:24:19.000000 openplugincore-0.6.1/tests/test_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13061 2023-07-30 02:24:19.000000 openplugincore-0.6.1/tests/test_openplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-30 02:24:19.000000 openplugincore-0.6.1/tests/test_openplugin_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-30 02:24:19.000000 openplugincore-0.6.1/tests/test_openplugin_memo.py
```

### Comparing `openplugincore-0.6.0/PKG-INFO` & `openplugincore-0.6.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: openplugincore
-Version: 0.6.0
+Version: 0.6.1
 Summary: Seamlessly integrate with OpenAI ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!
 Home-page: UNKNOWN
 Author: Sebastian Sosa
 Author-email: 1sebastian1sosa1@gmail.com
 License: UNKNOWN
 Description: Seamlessly integrate with OpenAIs ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!
 Keywords: python,openai,chatgpt,chat,plugin
```

### Comparing `openplugincore-0.6.0/openplugincore/openplugin.py` & `openplugincore-0.6.1/openplugincore/openplugin.py`

 * *Files identical despite different names*

### Comparing `openplugincore-0.6.0/openplugincore/openplugin_completion.py` & `openplugincore-0.6.1/openplugincore/openplugin_completion.py`

 * *Files identical despite different names*

### Comparing `openplugincore-0.6.0/openplugincore/openplugin_memo.py` & `openplugincore-0.6.1/openplugincore/openplugin_memo.py`

 * *Files identical despite different names*

### Comparing `openplugincore-0.6.0/openplugincore/types.py` & `openplugincore-0.6.1/openplugincore/types.py`

 * *Files identical despite different names*

### Comparing `openplugincore-0.6.0/openplugincore.egg-info/PKG-INFO` & `openplugincore-0.6.1/openplugincore.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: openplugincore
-Version: 0.6.0
+Version: 0.6.1
 Summary: Seamlessly integrate with OpenAI ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!
 Home-page: UNKNOWN
 Author: Sebastian Sosa
 Author-email: 1sebastian1sosa1@gmail.com
 License: UNKNOWN
 Description: Seamlessly integrate with OpenAIs ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!
 Keywords: python,openai,chatgpt,chat,plugin
```

### Comparing `openplugincore-0.6.0/setup.py` & `openplugincore-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name='openplugincore', 
-        version="0.6.0",
+        version="0.6.1",
         author="Sebastian Sosa",
         author_email="1sebastian1sosa1@gmail.com",
         description='Seamlessly integrate with OpenAI ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!',
         long_description='Seamlessly integrate with OpenAIs ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!',
         packages=find_packages(),
         package_data={
             "openplugincore": ["*.json"],  # include all .json files in the openplugin package
```

### Comparing `openplugincore-0.6.0/tests/mock_data.py` & `openplugincore-0.6.1/tests/mock_data.py`

 * *Files identical despite different names*

### Comparing `openplugincore-0.6.0/tests/test_e2e.py` & `openplugincore-0.6.1/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `openplugincore-0.6.0/tests/test_openplugin.py` & `openplugincore-0.6.1/tests/test_openplugin.py`

 * *Files identical despite different names*

### Comparing `openplugincore-0.6.0/tests/test_openplugin_completion.py` & `openplugincore-0.6.1/tests/test_openplugin_completion.py`

 * *Files identical despite different names*

### Comparing `openplugincore-0.6.0/tests/test_openplugin_memo.py` & `openplugincore-0.6.1/tests/test_openplugin_memo.py`

 * *Files identical despite different names*

