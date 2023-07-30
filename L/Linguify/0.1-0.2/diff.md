# Comparing `tmp/Linguify-0.1.tar.gz` & `tmp/Linguify-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Linguify-0.1.tar", last modified: Sun Jul 30 03:30:39 2023, max compression
+gzip compressed data, was "Linguify-0.2.tar", last modified: Sun Jul 30 03:38:18 2023, max compression
```

## Comparing `Linguify-0.1.tar` & `Linguify-0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 abdulrahmankhafagy   (501) staff       (20)        0 2023-07-30 03:30:39.045775 Linguify-0.1/
-drwxr-xr-x   0 abdulrahmankhafagy   (501) staff       (20)        0 2023-07-30 03:30:39.045519 Linguify-0.1/Linguify.egg-info/
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      207 2023-07-30 03:30:39.000000 Linguify-0.1/Linguify.egg-info/PKG-INFO
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      202 2023-07-30 03:30:39.000000 Linguify-0.1/Linguify.egg-info/SOURCES.txt
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)        1 2023-07-30 03:30:39.000000 Linguify-0.1/Linguify.egg-info/dependency_links.txt
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)       50 2023-07-30 03:30:39.000000 Linguify-0.1/Linguify.egg-info/entry_points.txt
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      102 2023-07-30 03:30:39.000000 Linguify-0.1/Linguify.egg-info/requires.txt
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)        1 2023-07-30 03:30:39.000000 Linguify-0.1/Linguify.egg-info/top_level.txt
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      207 2023-07-30 03:30:39.045665 Linguify-0.1/PKG-INFO
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)       38 2023-07-30 03:30:39.045815 Linguify-0.1/setup.cfg
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      591 2023-07-30 03:21:09.000000 Linguify-0.1/setup.py
+drwxr-xr-x   0 abdulrahmankhafagy   (501) staff       (20)        0 2023-07-30 03:38:18.422931 Linguify-0.2/
+drwxr-xr-x   0 abdulrahmankhafagy   (501) staff       (20)        0 2023-07-30 03:38:18.422400 Linguify-0.2/Linguify.egg-info/
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      207 2023-07-30 03:38:18.000000 Linguify-0.2/Linguify.egg-info/PKG-INFO
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      202 2023-07-30 03:38:18.000000 Linguify-0.2/Linguify.egg-info/SOURCES.txt
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)        1 2023-07-30 03:38:18.000000 Linguify-0.2/Linguify.egg-info/dependency_links.txt
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)       50 2023-07-30 03:38:18.000000 Linguify-0.2/Linguify.egg-info/entry_points.txt
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)       92 2023-07-30 03:38:18.000000 Linguify-0.2/Linguify.egg-info/requires.txt
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)        1 2023-07-30 03:38:18.000000 Linguify-0.2/Linguify.egg-info/top_level.txt
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      207 2023-07-30 03:38:18.422781 Linguify-0.2/PKG-INFO
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)       38 2023-07-30 03:38:18.423104 Linguify-0.2/setup.cfg
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      574 2023-07-30 03:37:58.000000 Linguify-0.2/setup.py
```

### Comparing `Linguify-0.1/setup.py` & `Linguify-0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Linguify',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     install_requires=[
     "openai",
     "python-docx",
     "google-api-python-client",
     "google-auth-httplib2",
     "google-auth-oauthlib",
-    "click",
-    "mimetypes"
+    "click"
     ],
     entry_points={
         'console_scripts': [
             'start = Linguify.Linguify:start',
         ],},
     author='Abdulrahman Khafagy',
     author_email='abdul_khafagy2004@hotmail.com',
```

