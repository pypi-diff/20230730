# Comparing `tmp/galaxy-files-23.0.4.tar.gz` & `tmp/galaxy-files-23.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/files/dist/.tmp-n3scwmcu/galaxy-files-23.0.4.tar", last modified: Fri Jun 30 22:02:30 2023, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/files/dist/.tmp-z3t30v8a/galaxy-files-23.0.5.tar", last modified: Sun Jul 30 10:48:44 2023, max compression
```

## Comparing `galaxy-files-23.0.4.tar` & `galaxy-files-23.0.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:02:30.000000 galaxy-files-23.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-30 22:00:50.000000 galaxy-files-23.0.4/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-30 22:00:49.000000 galaxy-files-23.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-30 22:00:50.000000 galaxy-files-23.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-30 22:02:30.000000 galaxy-files-23.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-30 22:00:50.000000 galaxy-files-23.0.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-30 22:00:50.000000 galaxy-files-23.0.4/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:02:30.000000 galaxy-files-23.0.4/galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-30 22:00:50.000000 galaxy-files-23.0.4/galaxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:02:30.000000 galaxy-files-23.0.4/galaxy/files/
--rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-06-30 22:00:50.000000 galaxy-files-23.0.4/galaxy/files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:02:30.000000 galaxy-files-23.0.4/galaxy/files/sources/
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-06-30 22:00:50.000000 galaxy-files-23.0.4/galaxy/files/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-30 22:00:50.000000 galaxy-files-23.0.4/galaxy/files/sources/_pyfilesystem2.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-30 22:00:50.000000 galaxy-files-23.0.4/galaxy/files/sources/anvil.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-30 22:00:50.000000 galaxy-files-23.0.4/galaxy/files/sources/basespace.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-30 22:00:50.000000 galaxy-files-23.0.4/galaxy/files/sources/dropbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-30 22:00:50.000000 galaxy-files-23.0.4/galaxy/files/sources/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-30 22:00:50.000000 galaxy-files-23.0.4/galaxy/files/sources/galaxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-30 22:00:50.000000 galaxy-files-23.0.4/galaxy/files/sources/googlecloudstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-30 22:00:50.000000 galaxy-files-23.0.4/galaxy/files/sources/googledrive.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-30 22:00:50.000000 galaxy-files-23.0.4/galaxy/files/sources/onedata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-06-30 22:00:50.000000 galaxy-files-23.0.4/galaxy/files/sources/posix.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-30 22:00:50.000000 galaxy-files-23.0.4/galaxy/files/sources/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-30 22:00:50.000000 galaxy-files-23.0.4/galaxy/files/sources/s3fs.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-30 22:00:50.000000 galaxy-files-23.0.4/galaxy/files/sources/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-30 22:00:50.000000 galaxy-files-23.0.4/galaxy/files/sources/webdav.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:02:30.000000 galaxy-files-23.0.4/galaxy/files/unittest_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-30 22:00:50.000000 galaxy-files-23.0.4/galaxy/files/unittest_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-06-30 22:00:50.000000 galaxy-files-23.0.4/galaxy/files/uris.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:00:50.000000 galaxy-files-23.0.4/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:02:30.000000 galaxy-files-23.0.4/galaxy_files.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-30 22:02:30.000000 galaxy-files-23.0.4/galaxy_files.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-30 22:02:30.000000 galaxy-files-23.0.4/galaxy_files.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 22:02:30.000000 galaxy-files-23.0.4/galaxy_files.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-30 22:02:30.000000 galaxy-files-23.0.4/galaxy_files.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 22:02:30.000000 galaxy-files-23.0.4/galaxy_files.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-30 22:00:50.000000 galaxy-files-23.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-30 22:02:30.000000 galaxy-files-23.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 22:00:50.000000 galaxy-files-23.0.4/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:48:44.000000 galaxy-files-23.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-30 10:47:08.000000 galaxy-files-23.0.5/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-07-30 10:47:07.000000 galaxy-files-23.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-30 10:47:08.000000 galaxy-files-23.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-30 10:48:44.000000 galaxy-files-23.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-30 10:47:08.000000 galaxy-files-23.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-30 10:47:08.000000 galaxy-files-23.0.5/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:48:44.000000 galaxy-files-23.0.5/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-30 10:47:08.000000 galaxy-files-23.0.5/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:48:44.000000 galaxy-files-23.0.5/galaxy/files/
+-rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-07-30 10:47:08.000000 galaxy-files-23.0.5/galaxy/files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:48:44.000000 galaxy-files-23.0.5/galaxy/files/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-07-30 10:47:08.000000 galaxy-files-23.0.5/galaxy/files/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-07-30 10:47:08.000000 galaxy-files-23.0.5/galaxy/files/sources/_pyfilesystem2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-30 10:47:08.000000 galaxy-files-23.0.5/galaxy/files/sources/anvil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-30 10:47:08.000000 galaxy-files-23.0.5/galaxy/files/sources/basespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-30 10:47:08.000000 galaxy-files-23.0.5/galaxy/files/sources/dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-30 10:47:08.000000 galaxy-files-23.0.5/galaxy/files/sources/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-30 10:47:08.000000 galaxy-files-23.0.5/galaxy/files/sources/galaxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-30 10:47:08.000000 galaxy-files-23.0.5/galaxy/files/sources/googlecloudstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-30 10:47:08.000000 galaxy-files-23.0.5/galaxy/files/sources/googledrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-30 10:47:08.000000 galaxy-files-23.0.5/galaxy/files/sources/onedata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-07-30 10:47:08.000000 galaxy-files-23.0.5/galaxy/files/sources/posix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-30 10:47:08.000000 galaxy-files-23.0.5/galaxy/files/sources/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-30 10:47:08.000000 galaxy-files-23.0.5/galaxy/files/sources/s3fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-30 10:47:08.000000 galaxy-files-23.0.5/galaxy/files/sources/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-30 10:47:08.000000 galaxy-files-23.0.5/galaxy/files/sources/webdav.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:48:44.000000 galaxy-files-23.0.5/galaxy/files/unittest_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-30 10:47:08.000000 galaxy-files-23.0.5/galaxy/files/unittest_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-07-30 10:47:08.000000 galaxy-files-23.0.5/galaxy/files/uris.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:47:08.000000 galaxy-files-23.0.5/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:48:44.000000 galaxy-files-23.0.5/galaxy_files.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-30 10:48:44.000000 galaxy-files-23.0.5/galaxy_files.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-30 10:48:44.000000 galaxy-files-23.0.5/galaxy_files.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 10:48:44.000000 galaxy-files-23.0.5/galaxy_files.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-30 10:48:44.000000 galaxy-files-23.0.5/galaxy_files.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-30 10:48:44.000000 galaxy-files-23.0.5/galaxy_files.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-30 10:47:08.000000 galaxy-files-23.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-30 10:48:44.000000 galaxy-files-23.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-30 10:47:08.000000 galaxy-files-23.0.5/test-requirements.txt
```

### Comparing `galaxy-files-23.0.4/HISTORY.rst` & `galaxy-files-23.0.5/HISTORY.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.5 (2023-07-29)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 23.0.4 (2023-06-30)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.3 (2023-06-26)
```

### Comparing `galaxy-files-23.0.4/LICENSE.txt` & `galaxy-files-23.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.0.4/PKG-INFO` & `galaxy-files-23.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-files
-Version: 23.0.4
+Version: 23.0.5
 Summary: Galaxy file source framework and default plugins
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,14 +42,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.5 (2023-07-29)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 23.0.4 (2023-06-30)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.3 (2023-06-26)
```

### Comparing `galaxy-files-23.0.4/galaxy/files/__init__.py` & `galaxy-files-23.0.5/galaxy/files/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.0.4/galaxy/files/sources/__init__.py` & `galaxy-files-23.0.5/galaxy/files/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.0.4/galaxy/files/sources/_pyfilesystem2.py` & `galaxy-files-23.0.5/galaxy/files/sources/_pyfilesystem2.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.0.4/galaxy/files/sources/dropbox.py` & `galaxy-files-23.0.5/galaxy/files/sources/dropbox.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.0.4/galaxy/files/sources/galaxy.py` & `galaxy-files-23.0.5/galaxy/files/sources/galaxy.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.0.4/galaxy/files/sources/googlecloudstorage.py` & `galaxy-files-23.0.5/galaxy/files/sources/googlecloudstorage.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.0.4/galaxy/files/sources/googledrive.py` & `galaxy-files-23.0.5/galaxy/files/sources/googledrive.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.0.4/galaxy/files/sources/posix.py` & `galaxy-files-23.0.5/galaxy/files/sources/posix.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.0.4/galaxy/files/sources/s3fs.py` & `galaxy-files-23.0.5/galaxy/files/sources/s3fs.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.0.4/galaxy/files/sources/ssh.py` & `galaxy-files-23.0.5/galaxy/files/sources/ssh.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.0.4/galaxy/files/unittest_utils/__init__.py` & `galaxy-files-23.0.5/galaxy/files/unittest_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.0.4/galaxy/files/uris.py` & `galaxy-files-23.0.5/galaxy/files/uris.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.0.4/galaxy_files.egg-info/PKG-INFO` & `galaxy-files-23.0.5/galaxy_files.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-files
-Version: 23.0.4
+Version: 23.0.5
 Summary: Galaxy file source framework and default plugins
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,14 +42,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.5 (2023-07-29)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 23.0.4 (2023-06-30)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.3 (2023-06-26)
```

### Comparing `galaxy-files-23.0.4/galaxy_files.egg-info/SOURCES.txt` & `galaxy-files-23.0.5/galaxy_files.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.0.4/setup.cfg` & `galaxy-files-23.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-files
 url = https://github.com/galaxyproject/galaxy
-version = 23.0.4
+version = 23.0.5
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-util
 	fs
 	typing-extensions
```

