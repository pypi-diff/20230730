# Comparing `tmp/pulumi_archive-0.0.2a1690485149.tar.gz` & `tmp/pulumi_archive-0.0.3a1690678699.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_archive-0.0.2a1690485149.tar", last modified: Thu Jul 27 19:16:58 2023, max compression
+gzip compressed data, was "pulumi_archive-0.0.3a1690678699.tar", last modified: Sun Jul 30 01:02:26 2023, max compression
```

## Comparing `pulumi_archive-0.0.2a1690485149.tar` & `pulumi_archive-0.0.3a1690678699.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:16:58.145993 pulumi_archive-0.0.2a1690485149/
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-27 19:16:58.145993 pulumi_archive-0.0.2a1690485149/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-27 19:16:57.000000 pulumi_archive-0.0.2a1690485149/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:16:58.145993 pulumi_archive-0.0.2a1690485149/pulumi_archive/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 19:16:57.000000 pulumi_archive-0.0.2a1690485149/pulumi_archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-27 19:16:57.000000 pulumi_archive-0.0.2a1690485149/pulumi_archive/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-27 19:16:57.000000 pulumi_archive-0.0.2a1690485149/pulumi_archive/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    40263 2023-07-27 19:16:57.000000 pulumi_archive-0.0.2a1690485149/pulumi_archive/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    17623 2023-07-27 19:16:57.000000 pulumi_archive-0.0.2a1690485149/pulumi_archive/get_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-27 19:16:57.000000 pulumi_archive-0.0.2a1690485149/pulumi_archive/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-27 19:16:57.000000 pulumi_archive-0.0.2a1690485149/pulumi_archive/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-27 19:16:57.000000 pulumi_archive-0.0.2a1690485149/pulumi_archive/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 19:16:57.000000 pulumi_archive-0.0.2a1690485149/pulumi_archive/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:16:58.145993 pulumi_archive-0.0.2a1690485149/pulumi_archive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-27 19:16:58.000000 pulumi_archive-0.0.2a1690485149/pulumi_archive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-27 19:16:58.000000 pulumi_archive-0.0.2a1690485149/pulumi_archive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 19:16:58.000000 pulumi_archive-0.0.2a1690485149/pulumi_archive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 19:16:58.000000 pulumi_archive-0.0.2a1690485149/pulumi_archive.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-27 19:16:58.000000 pulumi_archive-0.0.2a1690485149/pulumi_archive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 19:16:58.000000 pulumi_archive-0.0.2a1690485149/pulumi_archive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 19:16:58.145993 pulumi_archive-0.0.2a1690485149/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-27 19:16:57.000000 pulumi_archive-0.0.2a1690485149/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:02:26.269660 pulumi_archive-0.0.3a1690678699/
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-30 01:02:26.269660 pulumi_archive-0.0.3a1690678699/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-30 01:02:25.000000 pulumi_archive-0.0.3a1690678699/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:02:26.265660 pulumi_archive-0.0.3a1690678699/pulumi_archive/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-30 01:02:25.000000 pulumi_archive-0.0.3a1690678699/pulumi_archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-30 01:02:25.000000 pulumi_archive-0.0.3a1690678699/pulumi_archive/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-30 01:02:25.000000 pulumi_archive-0.0.3a1690678699/pulumi_archive/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40263 2023-07-30 01:02:25.000000 pulumi_archive-0.0.3a1690678699/pulumi_archive/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17623 2023-07-30 01:02:25.000000 pulumi_archive-0.0.3a1690678699/pulumi_archive/get_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-30 01:02:25.000000 pulumi_archive-0.0.3a1690678699/pulumi_archive/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-30 01:02:25.000000 pulumi_archive-0.0.3a1690678699/pulumi_archive/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-30 01:02:25.000000 pulumi_archive-0.0.3a1690678699/pulumi_archive/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 01:02:25.000000 pulumi_archive-0.0.3a1690678699/pulumi_archive/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:02:26.269660 pulumi_archive-0.0.3a1690678699/pulumi_archive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-30 01:02:26.000000 pulumi_archive-0.0.3a1690678699/pulumi_archive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-30 01:02:26.000000 pulumi_archive-0.0.3a1690678699/pulumi_archive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 01:02:26.000000 pulumi_archive-0.0.3a1690678699/pulumi_archive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 01:02:26.000000 pulumi_archive-0.0.3a1690678699/pulumi_archive.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-30 01:02:26.000000 pulumi_archive-0.0.3a1690678699/pulumi_archive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-30 01:02:26.000000 pulumi_archive-0.0.3a1690678699/pulumi_archive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 01:02:26.269660 pulumi_archive-0.0.3a1690678699/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-30 01:02:25.000000 pulumi_archive-0.0.3a1690678699/setup.py
```

### Comparing `pulumi_archive-0.0.2a1690485149/PKG-INFO` & `pulumi_archive-0.0.3a1690678699/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_archive
-Version: 0.0.2a1690485149
+Version: 0.0.3a1690678699
 Summary: A Pulumi package for creating and managing Archive cloud resources.
 Home-page: https://www.pulumi.com/
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-archive
 Keywords: pulumi category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_archive-0.0.2a1690485149/README.md` & `pulumi_archive-0.0.3a1690678699/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_archive-0.0.2a1690485149/pulumi_archive/__init__.py` & `pulumi_archive-0.0.3a1690678699/pulumi_archive/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_archive-0.0.2a1690485149/pulumi_archive/_inputs.py` & `pulumi_archive-0.0.3a1690678699/pulumi_archive/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_archive-0.0.2a1690485149/pulumi_archive/_utilities.py` & `pulumi_archive-0.0.3a1690678699/pulumi_archive/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_archive-0.0.2a1690485149/pulumi_archive/file.py` & `pulumi_archive-0.0.3a1690678699/pulumi_archive/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_archive-0.0.2a1690485149/pulumi_archive/get_file.py` & `pulumi_archive-0.0.3a1690678699/pulumi_archive/get_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_archive-0.0.2a1690485149/pulumi_archive/outputs.py` & `pulumi_archive-0.0.3a1690678699/pulumi_archive/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_archive-0.0.2a1690485149/pulumi_archive/provider.py` & `pulumi_archive-0.0.3a1690678699/pulumi_archive/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_archive-0.0.2a1690485149/pulumi_archive.egg-info/PKG-INFO` & `pulumi_archive-0.0.3a1690678699/pulumi_archive.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-archive
-Version: 0.0.2a1690485149
+Version: 0.0.3a1690678699
 Summary: A Pulumi package for creating and managing Archive cloud resources.
 Home-page: https://www.pulumi.com/
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-archive
 Keywords: pulumi category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_archive-0.0.2a1690485149/setup.py` & `pulumi_archive-0.0.3a1690678699/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.2a1690485149"
-PLUGIN_VERSION = "0.0.2-alpha.1690485149+1d301d3e"
+VERSION = "0.0.3a1690678699"
+PLUGIN_VERSION = "0.0.3-alpha.1690678699+f8a924b1"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'archive', PLUGIN_VERSION])
         except OSError as error:
```

