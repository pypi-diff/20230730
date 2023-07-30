# Comparing `tmp/raspi-system-0.2.0.tar.gz` & `tmp/raspi-system-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raspi-system-0.2.0.tar", last modified: Sun Jul 30 10:50:48 2023, max compression
+gzip compressed data, was "raspi-system-0.2.1.tar", last modified: Sun Jul 30 11:26:24 2023, max compression
```

## Comparing `raspi-system-0.2.0.tar` & `raspi-system-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-30 10:50:48.015692 raspi-system-0.2.0/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-30 10:50:48.011692 raspi-system-0.2.0/.idea/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       47 2021-09-20 07:13:41.000000 raspi-system-0.2.0/.idea/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      625 2023-07-30 10:50:48.015692 raspi-system-0.2.0/PKG-INFO
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-30 10:50:48.015692 raspi-system-0.2.0/raspi_system/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2021-08-30 11:46:55.000000 raspi-system-0.2.0/raspi_system/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4520 2023-07-30 10:49:43.000000 raspi-system-0.2.0/raspi_system/hwinfo.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      202 2021-08-30 11:46:55.000000 raspi-system-0.2.0/raspi_system/network.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-30 10:50:48.015692 raspi-system-0.2.0/raspi_system.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      625 2023-07-30 10:50:47.000000 raspi-system-0.2.0/raspi_system.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      276 2023-07-30 10:50:47.000000 raspi-system-0.2.0/raspi_system.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-07-30 10:50:47.000000 raspi-system-0.2.0/raspi_system.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       19 2023-07-30 10:50:47.000000 raspi-system-0.2.0/raspi_system.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       13 2023-07-30 10:50:47.000000 raspi-system-0.2.0/raspi_system.egg-info/top_level.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       38 2023-07-30 10:50:48.015692 raspi-system-0.2.0/setup.cfg
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      889 2021-08-30 11:46:55.000000 raspi-system-0.2.0/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-30 11:26:24.796424 raspi-system-0.2.1/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-30 11:26:24.796424 raspi-system-0.2.1/.idea/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       47 2021-09-20 07:13:41.000000 raspi-system-0.2.1/.idea/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      625 2023-07-30 11:26:24.796424 raspi-system-0.2.1/PKG-INFO
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-30 11:26:24.796424 raspi-system-0.2.1/raspi_system/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2021-08-30 11:46:55.000000 raspi-system-0.2.1/raspi_system/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4511 2023-07-30 10:53:22.000000 raspi-system-0.2.1/raspi_system/hwinfo.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      202 2021-08-30 11:46:55.000000 raspi-system-0.2.1/raspi_system/network.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-30 11:26:24.796424 raspi-system-0.2.1/raspi_system.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      625 2023-07-30 11:26:24.000000 raspi-system-0.2.1/raspi_system.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      276 2023-07-30 11:26:24.000000 raspi-system-0.2.1/raspi_system.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-07-30 11:26:24.000000 raspi-system-0.2.1/raspi_system.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       19 2023-07-30 11:26:24.000000 raspi-system-0.2.1/raspi_system.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       13 2023-07-30 11:26:24.000000 raspi-system-0.2.1/raspi_system.egg-info/top_level.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       38 2023-07-30 11:26:24.796424 raspi-system-0.2.1/setup.cfg
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      889 2021-08-30 11:46:55.000000 raspi-system-0.2.1/setup.py
```

### Comparing `raspi-system-0.2.0/PKG-INFO` & `raspi-system-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspi-system
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python library with minimal dependencies to get assorted system information from a Raspberry Pi 
 Home-page: 
 Author: Chintalagiri Shashank
 Author-email: shashank.chintalagiri@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `raspi-system-0.2.0/raspi_system/hwinfo.py` & `raspi-system-0.2.1/raspi_system/hwinfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 ]
 
 rpi_models = {info.code: info for info in _rpi_models}
 
 
 def model_string():
     result = subprocess.check_output(['cat', '/proc/device-tree/model'])
-    result = result.encode().strip()
+    result = result.strip()
     return result
 
 
 def model_revcode():
     revision = "0000"
     f = open('/proc/cpuinfo', 'r')
     for line in f:
```

### Comparing `raspi-system-0.2.0/raspi_system.egg-info/PKG-INFO` & `raspi-system-0.2.1/raspi_system.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspi-system
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python library with minimal dependencies to get assorted system information from a Raspberry Pi 
 Home-page: 
 Author: Chintalagiri Shashank
 Author-email: shashank.chintalagiri@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `raspi-system-0.2.0/setup.py` & `raspi-system-0.2.1/setup.py`

 * *Files identical despite different names*

