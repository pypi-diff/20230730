# Comparing `tmp/nec_beamer-0.1.2.tar.gz` & `tmp/nec_beamer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nec_beamer-0.1.2.tar", last modified: Sat Jul 29 21:41:22 2023, max compression
+gzip compressed data, was "nec_beamer-0.1.3.tar", last modified: Sat Jul 29 22:00:12 2023, max compression
```

## Comparing `nec_beamer-0.1.2.tar` & `nec_beamer-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 mhp        (502) staff       (20)        0 2023-07-29 21:41:22.606684 nec_beamer-0.1.2/
--rw-r--r--   0 mhp        (502) staff       (20)     1072 2023-07-29 19:57:55.000000 nec_beamer-0.1.2/LICENSE
--rw-r--r--   0 mhp        (502) staff       (20)      479 2023-07-29 21:41:22.606570 nec_beamer-0.1.2/PKG-INFO
--rw-r--r--   0 mhp        (502) staff       (20)      188 2023-07-29 19:57:55.000000 nec_beamer-0.1.2/README.md
-drwxr-xr-x   0 mhp        (502) staff       (20)        0 2023-07-29 21:41:22.605446 nec_beamer-0.1.2/nec_beamer/
--rw-r--r--   0 mhp        (502) staff       (20)       34 2023-07-29 20:47:52.000000 nec_beamer-0.1.2/nec_beamer/__init__.py
--rw-r--r--   0 mhp        (502) staff       (20)     5805 2023-07-29 20:38:23.000000 nec_beamer-0.1.2/nec_beamer/cli.py
--rw-r--r--   0 mhp        (502) staff       (20)    12534 2023-07-29 20:38:23.000000 nec_beamer-0.1.2/nec_beamer/nec_beamer.py
-drwxr-xr-x   0 mhp        (502) staff       (20)        0 2023-07-29 21:41:22.606384 nec_beamer-0.1.2/nec_beamer.egg-info/
--rw-r--r--   0 mhp        (502) staff       (20)      479 2023-07-29 21:41:22.000000 nec_beamer-0.1.2/nec_beamer.egg-info/PKG-INFO
--rw-r--r--   0 mhp        (502) staff       (20)      294 2023-07-29 21:41:22.000000 nec_beamer-0.1.2/nec_beamer.egg-info/SOURCES.txt
--rw-r--r--   0 mhp        (502) staff       (20)        1 2023-07-29 21:41:22.000000 nec_beamer-0.1.2/nec_beamer.egg-info/dependency_links.txt
--rw-r--r--   0 mhp        (502) staff       (20)        1 2023-07-29 20:44:20.000000 nec_beamer-0.1.2/nec_beamer.egg-info/not-zip-safe
--rw-r--r--   0 mhp        (502) staff       (20)       15 2023-07-29 21:41:22.000000 nec_beamer-0.1.2/nec_beamer.egg-info/requires.txt
--rw-r--r--   0 mhp        (502) staff       (20)       11 2023-07-29 21:41:22.000000 nec_beamer-0.1.2/nec_beamer.egg-info/top_level.txt
--rw-r--r--   0 mhp        (502) staff       (20)       38 2023-07-29 21:41:22.606731 nec_beamer-0.1.2/setup.cfg
--rw-r--r--   0 mhp        (502) staff       (20)      527 2023-07-29 21:41:16.000000 nec_beamer-0.1.2/setup.py
+drwxr-xr-x   0 mhp        (502) staff       (20)        0 2023-07-29 22:00:12.261761 nec_beamer-0.1.3/
+-rw-r--r--   0 mhp        (502) staff       (20)     1072 2023-07-29 19:57:55.000000 nec_beamer-0.1.3/LICENSE
+-rw-r--r--   0 mhp        (502) staff       (20)      479 2023-07-29 22:00:12.261626 nec_beamer-0.1.3/PKG-INFO
+-rw-r--r--   0 mhp        (502) staff       (20)      188 2023-07-29 19:57:55.000000 nec_beamer-0.1.3/README.md
+drwxr-xr-x   0 mhp        (502) staff       (20)        0 2023-07-29 22:00:12.259737 nec_beamer-0.1.3/bin/
+-rw-r--r--   0 mhp        (502) staff       (20)     5968 2023-07-29 21:53:38.000000 nec_beamer-0.1.3/bin/nec_beamer
+drwxr-xr-x   0 mhp        (502) staff       (20)        0 2023-07-29 22:00:12.260366 nec_beamer-0.1.3/nec_beamer/
+-rw-r--r--   0 mhp        (502) staff       (20)       34 2023-07-29 20:47:52.000000 nec_beamer-0.1.3/nec_beamer/__init__.py
+-rw-r--r--   0 mhp        (502) staff       (20)    12555 2023-07-29 21:48:48.000000 nec_beamer-0.1.3/nec_beamer/nec_beamer.py
+drwxr-xr-x   0 mhp        (502) staff       (20)        0 2023-07-29 22:00:12.261419 nec_beamer-0.1.3/nec_beamer.egg-info/
+-rw-r--r--   0 mhp        (502) staff       (20)      479 2023-07-29 22:00:12.000000 nec_beamer-0.1.3/nec_beamer.egg-info/PKG-INFO
+-rw-r--r--   0 mhp        (502) staff       (20)      291 2023-07-29 22:00:12.000000 nec_beamer-0.1.3/nec_beamer.egg-info/SOURCES.txt
+-rw-r--r--   0 mhp        (502) staff       (20)        1 2023-07-29 22:00:12.000000 nec_beamer-0.1.3/nec_beamer.egg-info/dependency_links.txt
+-rw-r--r--   0 mhp        (502) staff       (20)        1 2023-07-29 20:44:20.000000 nec_beamer-0.1.3/nec_beamer.egg-info/not-zip-safe
+-rw-r--r--   0 mhp        (502) staff       (20)       15 2023-07-29 22:00:12.000000 nec_beamer-0.1.3/nec_beamer.egg-info/requires.txt
+-rw-r--r--   0 mhp        (502) staff       (20)       11 2023-07-29 22:00:12.000000 nec_beamer-0.1.3/nec_beamer.egg-info/top_level.txt
+-rw-r--r--   0 mhp        (502) staff       (20)       38 2023-07-29 22:00:12.261832 nec_beamer-0.1.3/setup.cfg
+-rw-r--r--   0 mhp        (502) staff       (20)      561 2023-07-29 21:59:58.000000 nec_beamer-0.1.3/setup.py
```

### Comparing `nec_beamer-0.1.2/LICENSE` & `nec_beamer-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nec_beamer-0.1.2/nec_beamer/cli.py` & `nec_beamer-0.1.3/bin/nec_beamer`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,19 @@
+#!/usr/bin/env python
+
+import logging
+
 import click
-from .nec_beamer import Nec_Beamer
+from nec_beamer import Nec_Beamer
+
+# Default values for the NEC Beamer
+NAME="NEC Beamer"
+IP_ADDRESS="192.168.0.175"
+
+_logger = logging.getLogger("nec_beamer")
 
 @click.command()
 @click.option("--ip_address", default=IP_ADDRESS, help="IP Address of the Beamer")
 @click.option("--name", default=NAME, help="Name of the Beamer")
 @click.option("--json/--no-json", default=False, help="output as JSON")
 def turn_on(ip_address, name, json):
     """Turn on the Beamer"""
```

### Comparing `nec_beamer-0.1.2/nec_beamer/nec_beamer.py` & `nec_beamer-0.1.3/nec_beamer/nec_beamer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
+#!/usr/bin/env python
 
 import logging
 from datetime import datetime
 import json as json_lib
 
 import requests
 
 _logger = logging.getLogger("nec_beamer")
-
 # Default values for the NEC Beamer
 NAME="NEC Beamer"
 IP_ADDRESS="192.168.0.175"
 
 class Nec_Beamer:
     def __init__(self, ip_address, name) -> None:
         self._ip_address = ip_address if ip_address else IP_ADDRESS
```

### Comparing `nec_beamer-0.1.2/setup.py` & `nec_beamer-0.1.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from setuptools import setup
 
 setup(name='nec_beamer',
-      version='0.1.2',
+      version='0.1.3',
       description='NEC Beamer Web Interface Wrapper',
       url='https://github.com/heinrich-foto/nec_beamer',
       author='Heinrich-Foto',
       author_email='nec_beamer@heinrich-foto.de',
       license='MIT',
       packages=['nec_beamer'],
       install_requires=[
           'requests',
           'click'
       ],
       zip_safe=False,
+      scripts=['bin/nec_beamer'],
       long_description=open('README.md').read(),
       long_description_content_type='text/markdown',
       )
```

