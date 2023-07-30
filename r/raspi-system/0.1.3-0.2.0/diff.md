# Comparing `tmp/raspi-system-0.1.3.tar.gz` & `tmp/raspi-system-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/raspi-system-0.1.3.tar", last modified: Sun Apr 24 07:02:52 2022, max compression
+gzip compressed data, was "raspi-system-0.2.0.tar", last modified: Sun Jul 30 10:50:48 2023, max compression
```

## Comparing `raspi-system-0.1.3.tar` & `raspi-system-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-04-24 07:02:52.000000 raspi-system-0.1.3/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      688 2022-04-24 07:02:52.000000 raspi-system-0.1.3/PKG-INFO
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-04-24 07:02:52.000000 raspi-system-0.1.3/raspi_system/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2021-09-07 19:51:04.000000 raspi-system-0.1.3/raspi_system/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4398 2022-04-24 07:02:03.000000 raspi-system-0.1.3/raspi_system/hwinfo.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      202 2021-09-07 19:51:04.000000 raspi-system-0.1.3/raspi_system/network.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2022-04-24 07:02:52.000000 raspi-system-0.1.3/raspi_system.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      688 2022-04-24 07:02:51.000000 raspi-system-0.1.3/raspi_system.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      259 2022-04-24 07:02:51.000000 raspi-system-0.1.3/raspi_system.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2022-04-24 07:02:51.000000 raspi-system-0.1.3/raspi_system.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       19 2022-04-24 07:02:51.000000 raspi-system-0.1.3/raspi_system.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       13 2022-04-24 07:02:51.000000 raspi-system-0.1.3/raspi_system.egg-info/top_level.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       38 2022-04-24 07:02:52.000000 raspi-system-0.1.3/setup.cfg
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      889 2021-09-07 19:51:04.000000 raspi-system-0.1.3/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-30 10:50:48.015692 raspi-system-0.2.0/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-30 10:50:48.011692 raspi-system-0.2.0/.idea/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       47 2021-09-20 07:13:41.000000 raspi-system-0.2.0/.idea/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      625 2023-07-30 10:50:48.015692 raspi-system-0.2.0/PKG-INFO
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-30 10:50:48.015692 raspi-system-0.2.0/raspi_system/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2021-08-30 11:46:55.000000 raspi-system-0.2.0/raspi_system/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4520 2023-07-30 10:49:43.000000 raspi-system-0.2.0/raspi_system/hwinfo.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      202 2021-08-30 11:46:55.000000 raspi-system-0.2.0/raspi_system/network.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-30 10:50:48.015692 raspi-system-0.2.0/raspi_system.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      625 2023-07-30 10:50:47.000000 raspi-system-0.2.0/raspi_system.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      276 2023-07-30 10:50:47.000000 raspi-system-0.2.0/raspi_system.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-07-30 10:50:47.000000 raspi-system-0.2.0/raspi_system.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       19 2023-07-30 10:50:47.000000 raspi-system-0.2.0/raspi_system.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       13 2023-07-30 10:50:47.000000 raspi-system-0.2.0/raspi_system.egg-info/top_level.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       38 2023-07-30 10:50:48.015692 raspi-system-0.2.0/setup.cfg
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      889 2021-08-30 11:46:55.000000 raspi-system-0.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `raspi-system-0.1.3/PKG-INFO` & `raspi-system-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: raspi-system
-Version: 0.1.3
+Version: 0.2.0
 Summary: Python library with minimal dependencies to get assorted system information from a Raspberry Pi 
-Home-page: UNKNOWN
+Home-page: 
 Author: Chintalagiri Shashank
 Author-email: shashank.chintalagiri@gmail.com
-License: UNKNOWN
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `raspi-system-0.1.3/raspi_system/hwinfo.py` & `raspi-system-0.2.0/raspi_system/hwinfo.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,29 +46,30 @@
     HwModelInfo('a03111', 'rpi', 'Pi 4', '', 'v1.1', '1GB', 'Sony, UK'),
     HwModelInfo('b03111', 'rpi', 'Pi 4', '', 'v1.1', '2GB', 'Sony, UK'),
     HwModelInfo('b03112', 'rpi', 'Pi 4', '', 'v1.2', '2GB', 'Sony, UK'),
     HwModelInfo('c03111', 'rpi', 'Pi 4', '', 'v1.1', '4GB', 'Sony, UK'),
     HwModelInfo('c03112', 'rpi', 'Pi 4', '', 'v1.2', '4GB', 'Sony, UK'),
     HwModelInfo('c03114', 'rpi', 'Pi 4', '', 'v1.4', '4GB', 'Sony, UK'),
     HwModelInfo('d03114', 'rpi', 'Pi 4', '', 'v1.4', '8GB', 'Sony, UK'),
-
+    HwModelInfo('c03115', 'rpi', 'Pi 4', '', 'v1.5', '4GB', 'Sony, UK'),
+    HwModelInfo('c03115', 'rpi', 'Pi 4', '', 'v1.5', '8GB', 'Sony, UK'),
     HwModelInfo('c03130', 'rpi', 'Pi 400', '', 'v1.1', '4GB', 'Sony, UK'),
 
     HwModelInfo('a03140', 'rpi', 'CM4', '', 'v1.0', '1GB', 'Sony, UK'),
     HwModelInfo('b03140', 'rpi', 'CM4', '', 'v1.0', '2GB', 'Sony, UK'),
     HwModelInfo('c03140', 'rpi', 'CM4', '', 'v1.0', '4GB', 'Sony, UK'),
     HwModelInfo('d03140', 'rpi', 'CM4', '', 'v1.0', '8GB', 'Sony, UK'),
 ]
 
 rpi_models = {info.code: info for info in _rpi_models}
 
 
 def model_string():
     result = subprocess.check_output(['cat', '/proc/device-tree/model'])
-    result = result.decode().strip().rstrip('\x00').strip()
+    result = result.encode().strip()
     return result
 
 
 def model_revcode():
     revision = "0000"
     f = open('/proc/cpuinfo', 'r')
     for line in f:
```

### Comparing `raspi-system-0.1.3/raspi_system.egg-info/PKG-INFO` & `raspi-system-0.2.0/raspi_system.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: raspi-system
-Version: 0.1.3
+Version: 0.2.0
 Summary: Python library with minimal dependencies to get assorted system information from a Raspberry Pi 
-Home-page: UNKNOWN
+Home-page: 
 Author: Chintalagiri Shashank
 Author-email: shashank.chintalagiri@gmail.com
-License: UNKNOWN
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `raspi-system-0.1.3/setup.py` & `raspi-system-0.2.0/setup.py`

 * *Files identical despite different names*

