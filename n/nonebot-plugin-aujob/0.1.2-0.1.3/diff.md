# Comparing `tmp/nonebot_plugin_aujob-0.1.2.tar.gz` & `tmp/nonebot_plugin_aujob-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_aujob-0.1.2.tar", last modified: Sat Jul 29 12:12:20 2023, max compression
+gzip compressed data, was "nonebot_plugin_aujob-0.1.3.tar", last modified: Sun Jul 30 03:13:21 2023, max compression
```

## Comparing `nonebot_plugin_aujob-0.1.2.tar` & `nonebot_plugin_aujob-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 12:12:20.309430 nonebot_plugin_aujob-0.1.2/
--rw-rw-rw-   0        0        0      511 2023-07-29 12:12:20.307429 nonebot_plugin_aujob-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-29 12:12:20.275414 nonebot_plugin_aujob-0.1.2/nonebot_plugin_aujob/
--rw-rw-rw-   0        0        0     1709 2023-07-29 12:11:37.000000 nonebot_plugin_aujob-0.1.2/nonebot_plugin_aujob/__init__.py
--rw-rw-rw-   0        0        0    11199 2023-07-29 02:41:44.000000 nonebot_plugin_aujob-0.1.2/nonebot_plugin_aujob/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-29 12:12:20.305412 nonebot_plugin_aujob-0.1.2/nonebot_plugin_aujob.egg-info/
--rw-rw-rw-   0        0        0      511 2023-07-29 12:12:19.000000 nonebot_plugin_aujob-0.1.2/nonebot_plugin_aujob.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-07-29 12:12:20.000000 nonebot_plugin_aujob-0.1.2/nonebot_plugin_aujob.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 12:12:19.000000 nonebot_plugin_aujob-0.1.2/nonebot_plugin_aujob.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-29 12:12:19.000000 nonebot_plugin_aujob-0.1.2/nonebot_plugin_aujob.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-29 12:12:19.000000 nonebot_plugin_aujob-0.1.2/nonebot_plugin_aujob.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      698 2023-07-29 12:11:53.000000 nonebot_plugin_aujob-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-29 12:12:20.310430 nonebot_plugin_aujob-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-30 03:13:21.036207 nonebot_plugin_aujob-0.1.3/
+-rw-rw-rw-   0        0        0      511 2023-07-30 03:13:21.035208 nonebot_plugin_aujob-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-30 03:13:21.008049 nonebot_plugin_aujob-0.1.3/nonebot_plugin_aujob/
+-rw-rw-rw-   0        0        0     1709 2023-07-29 12:11:37.000000 nonebot_plugin_aujob-0.1.3/nonebot_plugin_aujob/__init__.py
+-rw-rw-rw-   0        0        0    11199 2023-07-29 02:41:44.000000 nonebot_plugin_aujob-0.1.3/nonebot_plugin_aujob/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-30 03:13:21.024238 nonebot_plugin_aujob-0.1.3/nonebot_plugin_aujob.egg-info/
+-rw-rw-rw-   0        0        0      511 2023-07-30 03:13:20.000000 nonebot_plugin_aujob-0.1.3/nonebot_plugin_aujob.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-07-30 03:13:20.000000 nonebot_plugin_aujob-0.1.3/nonebot_plugin_aujob.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 03:13:20.000000 nonebot_plugin_aujob-0.1.3/nonebot_plugin_aujob.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-30 03:13:20.000000 nonebot_plugin_aujob-0.1.3/nonebot_plugin_aujob.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-30 03:13:20.000000 nonebot_plugin_aujob-0.1.3/nonebot_plugin_aujob.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      660 2023-07-30 03:13:05.000000 nonebot_plugin_aujob-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-30 03:13:21.036207 nonebot_plugin_aujob-0.1.3/setup.cfg
```

### Comparing `nonebot_plugin_aujob-0.1.2/nonebot_plugin_aujob/__init__.py` & `nonebot_plugin_aujob-0.1.3/nonebot_plugin_aujob/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_aujob-0.1.2/nonebot_plugin_aujob/utils.py` & `nonebot_plugin_aujob-0.1.3/nonebot_plugin_aujob/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_aujob-0.1.2/pyproject.toml` & `nonebot_plugin_aujob-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nonebot_plugin_aujob"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="qwqZYLqwq", email="3422471182@qq.com" },
 ]
 description = "A nonebot plugin"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
-    "nonebot2>=2.0.0",
-    "nonebot-adapter-onebot>=2.0.0"
+    "nonebot2>=2.0.0"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

