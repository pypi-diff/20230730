# Comparing `tmp/begoneads-0.0.8.tar.gz` & `tmp/begoneads-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/begoneads-0.0.8.tar", last modified: Sat Jun 22 10:56:15 2019, max compression
+gzip compressed data, was "begoneads-0.0.9.tar", last modified: Sun Jun 26 20:25:08 2022, max compression
```

## Comparing `begoneads-0.0.8.tar` & `begoneads-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-06-22 10:56:15.000000 begoneads-0.0.8/
--rw-rw-r--   0 root         (0) root         (0)     1058 2019-06-22 10:54:20.000000 begoneads-0.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-06-22 10:56:15.000000 begoneads-0.0.8/begoneads.egg-info/
--rw-rw-r--   0 root         (0) root         (0)       10 2019-06-22 10:56:15.000000 begoneads-0.0.8/begoneads.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2019-06-22 10:56:15.000000 begoneads-0.0.8/begoneads.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       20 2019-06-22 10:56:15.000000 begoneads-0.0.8/begoneads.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)     5413 2019-06-22 10:56:15.000000 begoneads-0.0.8/begoneads.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      596 2019-06-22 10:56:15.000000 begoneads-0.0.8/begoneads.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)       55 2019-06-22 10:56:15.000000 begoneads-0.0.8/begoneads.egg-info/entry_points.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2019-06-09 14:06:53.000000 begoneads-0.0.8/begoneads.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       38 2019-06-22 10:56:15.000000 begoneads-0.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     5413 2019-06-22 10:56:15.000000 begoneads-0.0.8/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3728 2019-06-15 10:11:29.000000 begoneads-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-06-22 10:56:15.000000 begoneads-0.0.8/begoneads/
--rw-rw-r--   0 root         (0) root         (0)     4545 2019-06-22 10:52:22.000000 begoneads-0.0.8/begoneads/begoneads.py
--rw-rw-r--   0 root         (0) root         (0)        0 2019-06-09 18:28:31.000000 begoneads-0.0.8/begoneads/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1409 2019-06-09 13:53:56.000000 begoneads-0.0.8/begoneads/hostsmanager.py
--rw-rw-r--   0 root         (0) root         (0)      232 2019-06-09 13:53:56.000000 begoneads-0.0.8/begoneads/exceptions.py
--rw-rw-r--   0 root         (0) root         (0)      451 2019-06-09 13:53:56.000000 begoneads-0.0.8/begoneads/helpers.py
--rw-rw-r--   0 root         (0) root         (0)     1668 2019-06-15 10:32:14.000000 begoneads-0.0.8/begoneads/hostsmanager_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-06-22 10:56:15.000000 begoneads-0.0.8/begoneads/collectors/
--rw-rw-r--   0 root         (0) root         (0)     1233 2019-06-15 10:35:54.000000 begoneads-0.0.8/begoneads/collectors/base_collector.py
--rw-rw-r--   0 root         (0) root         (0)      896 2019-06-15 10:33:50.000000 begoneads-0.0.8/begoneads/collectors/remote_collector_test.py
--rw-rw-r--   0 root         (0) root         (0)        0 2019-06-15 10:33:50.000000 begoneads-0.0.8/begoneads/collectors/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      672 2019-06-15 10:33:50.000000 begoneads-0.0.8/begoneads/collectors/remote_collector.py
--rw-rw-r--   0 root         (0) root         (0)      491 2019-06-15 10:33:50.000000 begoneads-0.0.8/begoneads/collectors/local_collector.py
+drwxr-xr-x   0 annedouwe  (1000) annedouwe  (1000)        0 2022-06-26 20:25:08.712736 begoneads-0.0.9/
+-rw-r--r--   0 annedouwe  (1000) annedouwe  (1000)     1073 2022-06-26 20:07:26.000000 begoneads-0.0.9/LICENSE.md
+-rw-r--r--   0 annedouwe  (1000) annedouwe  (1000)     4395 2022-06-26 20:25:08.712736 begoneads-0.0.9/PKG-INFO
+-rw-r--r--   0 annedouwe  (1000) annedouwe  (1000)     3728 2022-06-26 20:07:26.000000 begoneads-0.0.9/README.md
+drwxr-xr-x   0 annedouwe  (1000) annedouwe  (1000)        0 2022-06-26 20:25:08.712736 begoneads-0.0.9/begoneads/
+-rw-r--r--   0 annedouwe  (1000) annedouwe  (1000)        0 2022-06-26 20:07:26.000000 begoneads-0.0.9/begoneads/__init__.py
+-rw-r--r--   0 annedouwe  (1000) annedouwe  (1000)     4588 2022-06-26 20:17:47.000000 begoneads-0.0.9/begoneads/begoneads.py
+drwxr-xr-x   0 annedouwe  (1000) annedouwe  (1000)        0 2022-06-26 20:25:08.712736 begoneads-0.0.9/begoneads/collectors/
+-rw-r--r--   0 annedouwe  (1000) annedouwe  (1000)        0 2022-06-26 20:07:26.000000 begoneads-0.0.9/begoneads/collectors/__init__.py
+-rw-r--r--   0 annedouwe  (1000) annedouwe  (1000)     1217 2022-06-26 20:17:47.000000 begoneads-0.0.9/begoneads/collectors/base_collector.py
+-rw-r--r--   0 annedouwe  (1000) annedouwe  (1000)      465 2022-06-26 20:17:47.000000 begoneads-0.0.9/begoneads/collectors/local_collector.py
+-rw-r--r--   0 annedouwe  (1000) annedouwe  (1000)      662 2022-06-26 20:17:47.000000 begoneads-0.0.9/begoneads/collectors/remote_collector.py
+-rw-r--r--   0 annedouwe  (1000) annedouwe  (1000)      896 2022-06-26 20:07:26.000000 begoneads-0.0.9/begoneads/collectors/remote_collector_test.py
+-rw-r--r--   0 annedouwe  (1000) annedouwe  (1000)      232 2022-06-26 20:07:26.000000 begoneads-0.0.9/begoneads/exceptions.py
+-rw-r--r--   0 annedouwe  (1000) annedouwe  (1000)      451 2022-06-26 20:17:47.000000 begoneads-0.0.9/begoneads/helpers.py
+-rw-r--r--   0 annedouwe  (1000) annedouwe  (1000)     1409 2022-06-26 20:07:26.000000 begoneads-0.0.9/begoneads/hostsmanager.py
+-rw-r--r--   0 annedouwe  (1000) annedouwe  (1000)     1668 2022-06-26 20:07:26.000000 begoneads-0.0.9/begoneads/hostsmanager_test.py
+drwxr-xr-x   0 annedouwe  (1000) annedouwe  (1000)        0 2022-06-26 20:25:08.712736 begoneads-0.0.9/begoneads.egg-info/
+-rw-r--r--   0 annedouwe  (1000) annedouwe  (1000)     4395 2022-06-26 20:25:08.000000 begoneads-0.0.9/begoneads.egg-info/PKG-INFO
+-rw-r--r--   0 annedouwe  (1000) annedouwe  (1000)      607 2022-06-26 20:25:08.000000 begoneads-0.0.9/begoneads.egg-info/SOURCES.txt
+-rw-r--r--   0 annedouwe  (1000) annedouwe  (1000)        1 2022-06-26 20:25:08.000000 begoneads-0.0.9/begoneads.egg-info/dependency_links.txt
+-rw-r--r--   0 annedouwe  (1000) annedouwe  (1000)       55 2022-06-26 20:25:08.000000 begoneads-0.0.9/begoneads.egg-info/entry_points.txt
+-rw-r--r--   0 annedouwe  (1000) annedouwe  (1000)        1 2022-06-26 20:12:53.000000 begoneads-0.0.9/begoneads.egg-info/not-zip-safe
+-rw-r--r--   0 annedouwe  (1000) annedouwe  (1000)       20 2022-06-26 20:25:08.000000 begoneads-0.0.9/begoneads.egg-info/requires.txt
+-rw-r--r--   0 annedouwe  (1000) annedouwe  (1000)       10 2022-06-26 20:25:08.000000 begoneads-0.0.9/begoneads.egg-info/top_level.txt
+-rw-r--r--   0 annedouwe  (1000) annedouwe  (1000)       38 2022-06-26 20:25:08.712736 begoneads-0.0.9/setup.cfg
+-rw-r--r--   0 annedouwe  (1000) annedouwe  (1000)     1058 2022-06-26 20:23:22.000000 begoneads-0.0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `begoneads-0.0.8/setup.py` & `begoneads-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md') as f:
         return f.read()
 
 
 setup(
     name='begoneads',
-    version='0.0.8',
+    version='0.0.9',
     description='BeGoneAds puts some popular hosts file lists into the hosts file as a adblocker measure.',
     python_requires='>=3.6',
     long_description=readme(),
     long_description_content_type="text/markdown",
     url='http://github.com/anned20/begoneads',
     entry_points={
         'console_scripts': ['begoneads=begoneads.begoneads:cli'],
```

### Comparing `begoneads-0.0.8/begoneads.egg-info/SOURCES.txt` & `begoneads-0.0.9/begoneads.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 README.md
 setup.py
 begoneads/__init__.py
 begoneads/begoneads.py
 begoneads/exceptions.py
 begoneads/helpers.py
 begoneads/hostsmanager.py
```

### Comparing `begoneads-0.0.8/README.md` & `begoneads-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `begoneads-0.0.8/begoneads/begoneads.py` & `begoneads-0.0.9/begoneads/begoneads.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import sys
 import re
 import click
 from begoneads.collectors.remote_collector import RemoteCollector
 from begoneads.collectors.local_collector import LocalCollector
 from begoneads.hostsmanager import HostsManager
-from begoneads.exceptions import *
+from begoneads.exceptions import NotElevatedException, InvalidSourceException
 from begoneads.helpers import is_admin
 
 # Default sources
 sources = [
     'https://www.malwaredomainlist.com/hostslist/hosts.txt',
     'https://raw.githubusercontent.com/FadeMind/hosts.extras/master/add.Dead/hosts',
     'https://raw.githubusercontent.com/FadeMind/hosts.extras/master/add.Spam/hosts',
```

### Comparing `begoneads-0.0.8/begoneads/hostsmanager.py` & `begoneads-0.0.9/begoneads/hostsmanager.py`

 * *Files identical despite different names*

### Comparing `begoneads-0.0.8/begoneads/hostsmanager_test.py` & `begoneads-0.0.9/begoneads/hostsmanager_test.py`

 * *Files identical despite different names*

### Comparing `begoneads-0.0.8/begoneads/collectors/base_collector.py` & `begoneads-0.0.9/begoneads/collectors/base_collector.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import requests
 import re
 from tqdm import tqdm
 
 
 class BaseCollector(object):
     """A base class for all collectors
```

### Comparing `begoneads-0.0.8/begoneads/collectors/remote_collector_test.py` & `begoneads-0.0.9/begoneads/collectors/remote_collector_test.py`

 * *Files identical despite different names*

### Comparing `begoneads-0.0.8/begoneads/collectors/remote_collector.py` & `begoneads-0.0.9/begoneads/collectors/remote_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import requests
-import re
 from tqdm import tqdm
 from begoneads.collectors.base_collector import BaseCollector
 
 
 class RemoteCollector(BaseCollector):
     """A class that collects the remote host files
```

