# Comparing `tmp/Linguify-0.0.0.tar.gz` & `tmp/Linguify-1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Linguify-0.0.0.tar", last modified: Sun Jul 30 06:16:55 2023, max compression
+gzip compressed data, was "Linguify-1.tar", last modified: Sun Jul 30 06:25:31 2023, max compression
```

## Comparing `Linguify-0.0.0.tar` & `Linguify-1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 abdulrahmankhafagy   (501) staff       (20)        0 2023-07-30 06:16:55.633429 Linguify-0.0.0/
-drwxr-xr-x   0 abdulrahmankhafagy   (501) staff       (20)        0 2023-07-30 06:16:55.632562 Linguify-0.0.0/Linguify.egg-info/
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      209 2023-07-30 06:16:55.000000 Linguify-0.0.0/Linguify.egg-info/PKG-INFO
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      244 2023-07-30 06:16:55.000000 Linguify-0.0.0/Linguify.egg-info/SOURCES.txt
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)        1 2023-07-30 06:16:55.000000 Linguify-0.0.0/Linguify.egg-info/dependency_links.txt
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)       43 2023-07-30 06:16:55.000000 Linguify-0.0.0/Linguify.egg-info/entry_points.txt
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)       92 2023-07-30 06:16:55.000000 Linguify-0.0.0/Linguify.egg-info/requires.txt
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)        9 2023-07-30 06:16:55.000000 Linguify-0.0.0/Linguify.egg-info/top_level.txt
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      209 2023-07-30 06:16:55.633339 Linguify-0.0.0/PKG-INFO
-drwxr-xr-x   0 abdulrahmankhafagy   (501) staff       (20)        0 2023-07-30 06:16:55.633214 Linguify-0.0.0/linguify/
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)    19136 2023-07-29 09:18:45.000000 Linguify-0.0.0/linguify/Linguify.py
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)        0 2023-07-30 02:57:11.000000 Linguify-0.0.0/linguify/__init__.py
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)       38 2023-07-30 06:16:55.633471 Linguify-0.0.0/setup.cfg
--rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      551 2023-07-30 06:15:43.000000 Linguify-0.0.0/setup.py
+drwxr-xr-x   0 abdulrahmankhafagy   (501) staff       (20)        0 2023-07-30 06:25:31.939453 Linguify-1/
+drwxr-xr-x   0 abdulrahmankhafagy   (501) staff       (20)        0 2023-07-30 06:25:31.938688 Linguify-1/Linguify.egg-info/
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      205 2023-07-30 06:25:31.000000 Linguify-1/Linguify.egg-info/PKG-INFO
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      244 2023-07-30 06:25:31.000000 Linguify-1/Linguify.egg-info/SOURCES.txt
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)        1 2023-07-30 06:25:31.000000 Linguify-1/Linguify.egg-info/dependency_links.txt
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)       44 2023-07-30 06:25:31.000000 Linguify-1/Linguify.egg-info/entry_points.txt
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)       92 2023-07-30 06:25:31.000000 Linguify-1/Linguify.egg-info/requires.txt
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)        9 2023-07-30 06:25:31.000000 Linguify-1/Linguify.egg-info/top_level.txt
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      205 2023-07-30 06:25:31.939365 Linguify-1/PKG-INFO
+drwxr-xr-x   0 abdulrahmankhafagy   (501) staff       (20)        0 2023-07-30 06:25:31.939235 Linguify-1/linguify/
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)    19136 2023-07-29 09:18:45.000000 Linguify-1/linguify/Linguify.py
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)        0 2023-07-30 02:57:11.000000 Linguify-1/linguify/__init__.py
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)       38 2023-07-30 06:25:31.939488 Linguify-1/setup.cfg
+-rw-r--r--   0 abdulrahmankhafagy   (501) staff       (20)      562 2023-07-30 06:23:56.000000 Linguify-1/setup.py
```

### Comparing `Linguify-0.0.0/linguify/Linguify.py` & `Linguify-1/linguify/Linguify.py`

 * *Files identical despite different names*

### Comparing `Linguify-0.0.0/setup.py` & `Linguify-1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Linguify',
-    
+    version=1,
     packages=find_packages(),
     install_requires=[
     "openai",
     "python-docx",
     "google-api-python-client",
     "google-auth-httplib2",
     "google-auth-oauthlib",
     "click"
     ],
     entry_points={
         'console_scripts': [
-            'linguify=linguify:main',
+            'linguify=linguify:start',
         ],},
     author='Abdulrahman Khafagy',
     author_email='abdul_khafagy2004@hotmail.com',
     description='Linguify is designed to automate voicemail transcription via email parsing.',
 )
```

