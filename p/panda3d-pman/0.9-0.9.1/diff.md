# Comparing `tmp/panda3d-pman-0.9.tar.gz` & `tmp/panda3d-pman-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/panda3d-pman-0.9.tar", last modified: Thu May 23 04:25:16 2019, max compression
+gzip compressed data, was "dist/panda3d-pman-0.9.1.tar", last modified: Fri May 24 04:26:15 2019, max compression
```

## Comparing `panda3d-pman-0.9.tar` & `panda3d-pman-0.9.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-23 04:25:16.000000 panda3d-pman-0.9/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1072 2019-05-23 04:24:44.000000 panda3d-pman-0.9/LICENSE.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      106 2019-05-23 04:24:44.000000 panda3d-pman-0.9/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     3258 2019-05-23 04:25:16.000000 panda3d-pman-0.9/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2144 2019-05-23 04:24:44.000000 panda3d-pman-0.9/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-23 04:25:16.000000 panda3d-pman-0.9/panda3d_pman.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3258 2019-05-23 04:25:16.000000 panda3d-pman-0.9/panda3d_pman.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      743 2019-05-23 04:25:16.000000 panda3d-pman-0.9/panda3d_pman.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-05-23 04:25:16.000000 panda3d-pman-0.9/panda3d_pman.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      378 2019-05-23 04:25:16.000000 panda3d-pman-0.9/panda3d_pman.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-05-23 04:25:16.000000 panda3d-pman-0.9/panda3d_pman.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        5 2019-05-23 04:25:16.000000 panda3d-pman-0.9/panda3d_pman.egg-info/top_level.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-23 04:25:16.000000 panda3d-pman-0.9/pman/
--rw-rw-r--   0 travis    (2000) travis    (2000)       72 2019-05-23 04:24:44.000000 panda3d-pman-0.9/pman/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1225 2019-05-23 04:24:44.000000 panda3d-pman-0.9/pman/basicrenderer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1287 2019-05-23 04:24:44.000000 panda3d-pman-0.9/pman/build_apps.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3400 2019-05-23 04:24:44.000000 panda3d-pman-0.9/pman/cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3646 2019-05-23 04:24:44.000000 panda3d-pman-0.9/pman/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11256 2019-05-23 04:24:44.000000 panda3d-pman-0.9/pman/core.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      888 2019-05-23 04:24:44.000000 panda3d-pman-0.9/pman/creationutils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      335 2019-05-23 04:24:44.000000 panda3d-pman-0.9/pman/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3784 2019-05-23 04:24:44.000000 panda3d-pman-0.9/pman/hooks.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1749 2019-05-23 04:24:44.000000 panda3d-pman-0.9/pman/native2bam.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      138 2019-05-23 04:24:44.000000 panda3d-pman-0.9/pman/nullrenderer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      590 2019-05-23 04:24:44.000000 panda3d-pman-0.9/pman/shim.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-23 04:25:16.000000 panda3d-pman-0.9/pman/templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)      425 2019-05-23 04:24:44.000000 panda3d-pman-0.9/pman/templates/main.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1721 2019-05-23 04:24:44.000000 panda3d-pman-0.9/pman/templates/panda.gitignore
--rw-rw-r--   0 travis    (2000) travis    (2000)    14921 2019-05-23 04:24:44.000000 panda3d-pman-0.9/pman/templates/pylintrc
--rw-rw-r--   0 travis    (2000) travis    (2000)       21 2019-05-23 04:24:44.000000 panda3d-pman-0.9/pman/templates/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       26 2019-05-23 04:24:44.000000 panda3d-pman-0.9/pman/templates/settings.prc
--rw-rw-r--   0 travis    (2000) travis    (2000)       80 2019-05-23 04:24:44.000000 panda3d-pman-0.9/pman/templates/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      959 2019-05-23 04:24:44.000000 panda3d-pman-0.9/pman/templates/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       75 2019-05-23 04:24:44.000000 panda3d-pman-0.9/pman/templates/test_imports.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30933 2019-05-23 04:24:44.000000 panda3d-pman-0.9/pman/toml.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      254 2019-05-23 04:24:44.000000 panda3d-pman-0.9/pman/venvwrapper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       20 2019-05-23 04:24:44.000000 panda3d-pman-0.9/pman/version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      735 2019-05-23 04:25:16.000000 panda3d-pman-0.9/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1096 2019-05-23 04:24:44.000000 panda3d-pman-0.9/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-24 04:26:15.000000 panda3d-pman-0.9.1/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1072 2019-05-24 04:25:42.000000 panda3d-pman-0.9.1/LICENSE.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      106 2019-05-24 04:25:42.000000 panda3d-pman-0.9.1/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3260 2019-05-24 04:26:15.000000 panda3d-pman-0.9.1/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2144 2019-05-24 04:25:42.000000 panda3d-pman-0.9.1/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-24 04:26:15.000000 panda3d-pman-0.9.1/panda3d_pman.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3260 2019-05-24 04:26:15.000000 panda3d-pman-0.9.1/panda3d_pman.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      743 2019-05-24 04:26:15.000000 panda3d-pman-0.9.1/panda3d_pman.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-05-24 04:26:15.000000 panda3d-pman-0.9.1/panda3d_pman.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      378 2019-05-24 04:26:15.000000 panda3d-pman-0.9.1/panda3d_pman.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-05-24 04:26:15.000000 panda3d-pman-0.9.1/panda3d_pman.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        5 2019-05-24 04:26:15.000000 panda3d-pman-0.9.1/panda3d_pman.egg-info/top_level.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-24 04:26:15.000000 panda3d-pman-0.9.1/pman/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       72 2019-05-24 04:25:42.000000 panda3d-pman-0.9.1/pman/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1225 2019-05-24 04:25:42.000000 panda3d-pman-0.9.1/pman/basicrenderer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1287 2019-05-24 04:25:42.000000 panda3d-pman-0.9.1/pman/build_apps.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3400 2019-05-24 04:25:42.000000 panda3d-pman-0.9.1/pman/cli.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3646 2019-05-24 04:25:42.000000 panda3d-pman-0.9.1/pman/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11370 2019-05-24 04:25:42.000000 panda3d-pman-0.9.1/pman/core.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      888 2019-05-24 04:25:42.000000 panda3d-pman-0.9.1/pman/creationutils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      335 2019-05-24 04:25:42.000000 panda3d-pman-0.9.1/pman/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3784 2019-05-24 04:25:42.000000 panda3d-pman-0.9.1/pman/hooks.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1749 2019-05-24 04:25:42.000000 panda3d-pman-0.9.1/pman/native2bam.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      138 2019-05-24 04:25:42.000000 panda3d-pman-0.9.1/pman/nullrenderer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      590 2019-05-24 04:25:42.000000 panda3d-pman-0.9.1/pman/shim.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-24 04:26:15.000000 panda3d-pman-0.9.1/pman/templates/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      425 2019-05-24 04:25:42.000000 panda3d-pman-0.9.1/pman/templates/main.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1721 2019-05-24 04:25:42.000000 panda3d-pman-0.9.1/pman/templates/panda.gitignore
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14921 2019-05-24 04:25:42.000000 panda3d-pman-0.9.1/pman/templates/pylintrc
+-rw-rw-r--   0 travis    (2000) travis    (2000)       21 2019-05-24 04:25:42.000000 panda3d-pman-0.9.1/pman/templates/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       26 2019-05-24 04:25:42.000000 panda3d-pman-0.9.1/pman/templates/settings.prc
+-rw-rw-r--   0 travis    (2000) travis    (2000)       80 2019-05-24 04:25:42.000000 panda3d-pman-0.9.1/pman/templates/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      959 2019-05-24 04:25:42.000000 panda3d-pman-0.9.1/pman/templates/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       75 2019-05-24 04:25:42.000000 panda3d-pman-0.9.1/pman/templates/test_imports.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30933 2019-05-24 04:25:42.000000 panda3d-pman-0.9.1/pman/toml.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      254 2019-05-24 04:25:42.000000 panda3d-pman-0.9.1/pman/venvwrapper.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       22 2019-05-24 04:25:42.000000 panda3d-pman-0.9.1/pman/version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      735 2019-05-24 04:26:15.000000 panda3d-pman-0.9.1/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1096 2019-05-24 04:25:42.000000 panda3d-pman-0.9.1/setup.py
```

### Comparing `panda3d-pman-0.9/LICENSE.txt` & `panda3d-pman-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `panda3d-pman-0.9/PKG-INFO` & `panda3d-pman-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda3d-pman
-Version: 0.9
+Version: 0.9.1
 Summary: A Python package to help bootstrap and manage Panda3D applications
 Home-page: https://github.com/Moguri/pman
 Author: Mitchell Stokes
 License: MIT
 Description: [![Build Status](https://travis-ci.org/Moguri/pman.svg?branch=master)](https://travis-ci.org/Moguri/pman)
         [![](https://img.shields.io/pypi/pyversions/panda3d_pman.svg)](https://pypi.org/project/panda3d_pman/)
         [![Panda3D Versions](https://img.shields.io/badge/panda3d-1.9%2C%201.10-blue.svg)](https://www.panda3d.org/)
```

### Comparing `panda3d-pman-0.9/README.md` & `panda3d-pman-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `panda3d-pman-0.9/panda3d_pman.egg-info/PKG-INFO` & `panda3d-pman-0.9.1/panda3d_pman.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda3d-pman
-Version: 0.9
+Version: 0.9.1
 Summary: A Python package to help bootstrap and manage Panda3D applications
 Home-page: https://github.com/Moguri/pman
 Author: Mitchell Stokes
 License: MIT
 Description: [![Build Status](https://travis-ci.org/Moguri/pman.svg?branch=master)](https://travis-ci.org/Moguri/pman)
         [![](https://img.shields.io/pypi/pyversions/panda3d_pman.svg)](https://pypi.org/project/panda3d_pman/)
         [![Panda3D Versions](https://img.shields.io/badge/panda3d-1.9%2C%201.10-blue.svg)](https://www.panda3d.org/)
```

### Comparing `panda3d-pman-0.9/panda3d_pman.egg-info/SOURCES.txt` & `panda3d-pman-0.9.1/panda3d_pman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panda3d-pman-0.9/pman/basicrenderer.py` & `panda3d-pman-0.9.1/pman/basicrenderer.py`

 * *Files identical despite different names*

### Comparing `panda3d-pman-0.9/pman/build_apps.py` & `panda3d-pman-0.9.1/pman/build_apps.py`

 * *Files identical despite different names*

### Comparing `panda3d-pman-0.9/pman/cli.py` & `panda3d-pman-0.9.1/pman/cli.py`

 * *Files identical despite different names*

### Comparing `panda3d-pman-0.9/pman/config.py` & `panda3d-pman-0.9.1/pman/config.py`

 * *Files identical despite different names*

### Comparing `panda3d-pman-0.9/pman/core.py` & `panda3d-pman-0.9.1/pman/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,19 @@
     '''Compatibility alias, use write_config() instead'''
     write_config(user_config)
 
 
 def ensure_config(func):
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
-        if 'config' not in kwargs or kwargs['config'] is None:
+        has_config = (
+            len(args) > 0 and args[0] is not None or
+            'config' in kwargs and kwargs['config'] is not None
+        )
+        if not has_config:
             kwargs['config'] = get_config()
         return func(*args, **kwargs)
     return wrapper
 
 
 def is_frozen():
     return imp.is_frozen(__name__)
```

### Comparing `panda3d-pman-0.9/pman/creationutils.py` & `panda3d-pman-0.9.1/pman/creationutils.py`

 * *Files identical despite different names*

### Comparing `panda3d-pman-0.9/pman/hooks.py` & `panda3d-pman-0.9.1/pman/hooks.py`

 * *Files identical despite different names*

### Comparing `panda3d-pman-0.9/pman/native2bam.py` & `panda3d-pman-0.9.1/pman/native2bam.py`

 * *Files identical despite different names*

### Comparing `panda3d-pman-0.9/pman/shim.py` & `panda3d-pman-0.9.1/pman/shim.py`

 * *Files identical despite different names*

### Comparing `panda3d-pman-0.9/pman/templates/panda.gitignore` & `panda3d-pman-0.9.1/pman/templates/panda.gitignore`

 * *Files identical despite different names*

### Comparing `panda3d-pman-0.9/pman/templates/pylintrc` & `panda3d-pman-0.9.1/pman/templates/pylintrc`

 * *Files identical despite different names*

### Comparing `panda3d-pman-0.9/pman/templates/setup.py` & `panda3d-pman-0.9.1/pman/templates/setup.py`

 * *Files identical despite different names*

### Comparing `panda3d-pman-0.9/pman/toml.py` & `panda3d-pman-0.9.1/pman/toml.py`

 * *Files identical despite different names*

### Comparing `panda3d-pman-0.9/setup.cfg` & `panda3d-pman-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `panda3d-pman-0.9/setup.py` & `panda3d-pman-0.9.1/setup.py`

 * *Files identical despite different names*

