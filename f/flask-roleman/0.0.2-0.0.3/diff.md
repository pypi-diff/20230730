# Comparing `tmp/flask-roleman-0.0.2.tar.gz` & `tmp/flask-roleman-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-roleman-0.0.2.tar", last modified: Tue Jun 20 21:21:18 2023, max compression
+gzip compressed data, was "flask-roleman-0.0.3.tar", last modified: Sun Jul 30 16:11:58 2023, max compression
```

## Comparing `flask-roleman-0.0.2.tar` & `flask-roleman-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 human     (1000) human     (1000)        0 2023-06-20 21:21:18.610964 flask-roleman-0.0.2/
--rw-r--r--   0 human     (1000) human     (1000)     4044 2023-06-20 21:21:18.610964 flask-roleman-0.0.2/PKG-INFO
--rw-r--r--   0 human     (1000) human     (1000)     3466 2023-06-20 21:10:19.000000 flask-roleman-0.0.2/README.md
-drwxr-xr-x   0 human     (1000) human     (1000)        0 2023-06-20 21:21:18.607631 flask-roleman-0.0.2/flask_roleman/
--rw-r--r--   0 human     (1000) human     (1000)     4978 2023-06-20 21:11:34.000000 flask-roleman-0.0.2/flask_roleman/__init__.py
-drwxr-xr-x   0 human     (1000) human     (1000)        0 2023-06-20 21:21:18.610964 flask-roleman-0.0.2/flask_roleman.egg-info/
--rw-r--r--   0 human     (1000) human     (1000)     4044 2023-06-20 21:21:18.000000 flask-roleman-0.0.2/flask_roleman.egg-info/PKG-INFO
--rw-r--r--   0 human     (1000) human     (1000)      228 2023-06-20 21:21:18.000000 flask-roleman-0.0.2/flask_roleman.egg-info/SOURCES.txt
--rw-r--r--   0 human     (1000) human     (1000)        1 2023-06-20 21:21:18.000000 flask-roleman-0.0.2/flask_roleman.egg-info/dependency_links.txt
--rw-r--r--   0 human     (1000) human     (1000)       35 2023-06-20 21:21:18.000000 flask-roleman-0.0.2/flask_roleman.egg-info/requires.txt
--rw-r--r--   0 human     (1000) human     (1000)       14 2023-06-20 21:21:18.000000 flask-roleman-0.0.2/flask_roleman.egg-info/top_level.txt
--rw-r--r--   0 human     (1000) human     (1000)       38 2023-06-20 21:21:18.610964 flask-roleman-0.0.2/setup.cfg
--rw-r--r--   0 human     (1000) human     (1000)     1032 2023-06-20 21:20:51.000000 flask-roleman-0.0.2/setup.py
+drwxr-xr-x   0 human     (1000) human     (1000)        0 2023-07-30 16:11:58.466717 flask-roleman-0.0.3/
+-rw-r--r--   0 human     (1000) human     (1000)     4113 2023-07-30 16:11:58.466717 flask-roleman-0.0.3/PKG-INFO
+-rw-r--r--   0 human     (1000) human     (1000)     3466 2023-06-20 21:10:19.000000 flask-roleman-0.0.3/README.md
+drwxr-xr-x   0 human     (1000) human     (1000)        0 2023-07-30 16:11:58.463384 flask-roleman-0.0.3/flask_roleman/
+-rw-r--r--   0 human     (1000) human     (1000)     5028 2023-07-27 00:47:51.000000 flask-roleman-0.0.3/flask_roleman/__init__.py
+drwxr-xr-x   0 human     (1000) human     (1000)        0 2023-07-30 16:11:58.466717 flask-roleman-0.0.3/flask_roleman.egg-info/
+-rw-r--r--   0 human     (1000) human     (1000)     4113 2023-07-30 16:11:58.000000 flask-roleman-0.0.3/flask_roleman.egg-info/PKG-INFO
+-rw-r--r--   0 human     (1000) human     (1000)      228 2023-07-30 16:11:58.000000 flask-roleman-0.0.3/flask_roleman.egg-info/SOURCES.txt
+-rw-r--r--   0 human     (1000) human     (1000)        1 2023-07-30 16:11:58.000000 flask-roleman-0.0.3/flask_roleman.egg-info/dependency_links.txt
+-rw-r--r--   0 human     (1000) human     (1000)       35 2023-07-30 16:11:58.000000 flask-roleman-0.0.3/flask_roleman.egg-info/requires.txt
+-rw-r--r--   0 human     (1000) human     (1000)       14 2023-07-30 16:11:58.000000 flask-roleman-0.0.3/flask_roleman.egg-info/top_level.txt
+-rw-r--r--   0 human     (1000) human     (1000)       38 2023-07-30 16:11:58.466717 flask-roleman-0.0.3/setup.cfg
+-rw-r--r--   0 human     (1000) human     (1000)     1100 2023-07-30 16:07:41.000000 flask-roleman-0.0.3/setup.py
```

### Comparing `flask-roleman-0.0.2/PKG-INFO` & `flask-roleman-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: flask-roleman
-Version: 0.0.2
+Version: 0.0.3
 Summary: Flask Extension to add the Authorization functionality to your apps.
 Author: Mohamed El-Hasnaouy
 Author-email: <elhasnaouymed@proton.me>
 Keywords: flask,role,authorization,permissions,security
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `flask-roleman-0.0.2/README.md` & `flask-roleman-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `flask-roleman-0.0.2/flask_roleman/__init__.py` & `flask-roleman-0.0.3/flask_roleman/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import functools
 from flask import abort
 from flask_login import current_user
 from flask_sqlalchemy import SQLAlchemy as _SQLAlchemy, model as _model
 
 
 _Role: _model.Model | None = None  # holds the Role Model class to be accessed from ManMixing
 
@@ -111,14 +112,15 @@
     """
     This decorator is used before routes, to ensure that the current_user has the authorization to access that route
     :param role: role as str or Role object
     :return: None
     """
 
     def holder(action):
+        @functools.wraps(action)
         def wrapper(*args, **kwargs):
             nonlocal roles
             #
             if current_user.has_roles(*roles):
                 return action(*args, **kwargs)
             #
             return abort(401)
```

### Comparing `flask-roleman-0.0.2/flask_roleman.egg-info/PKG-INFO` & `flask-roleman-0.0.3/flask_roleman.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: flask-roleman
-Version: 0.0.2
+Version: 0.0.3
 Summary: Flask Extension to add the Authorization functionality to your apps.
 Author: Mohamed El-Hasnaouy
 Author-email: <elhasnaouymed@proton.me>
 Keywords: flask,role,authorization,permissions,security
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `flask-roleman-0.0.2/setup.py` & `flask-roleman-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Flask Extension to add the Authorization functionality to your apps.'
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 # Setting up
 setup(
@@ -18,15 +18,16 @@
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=['flask', 'flask_login', 'flask_sqlalchemy'],
     keywords=['flask', 'role', 'authorization', 'permissions', 'security'],
     classifiers=[
-        "Development Status :: 1 - Planning",
+        "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
+        "License :: OSI Approved :: GNU General Public License (GPL)",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
 )
```

