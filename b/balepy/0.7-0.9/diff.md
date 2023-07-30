# Comparing `tmp/balepy-0.7.tar.gz` & `tmp/balepy-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balepy-0.7.tar", last modified: Sat Jul  1 14:43:26 2023, max compression
+gzip compressed data, was "balepy-0.9.tar", last modified: Sun Jul 30 11:02:15 2023, max compression
```

## Comparing `balepy-0.7.tar` & `balepy-0.9.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-07-01 14:43:26.358563 balepy-0.7/
--rw-r--r--   0 themamad  (1000) themamad  (1000)     1077 2023-06-20 12:51:32.000000 balepy-0.7/LICENSE
--rw-r--r--   0 themamad  (1000) themamad  (1000)      997 2023-07-01 14:43:26.358563 balepy-0.7/PKG-INFO
--rw-r--r--   0 themamad  (1000) themamad  (1000)      245 2023-07-01 14:42:36.000000 balepy-0.7/README.md
-drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-07-01 14:43:26.358563 balepy-0.7/balepy/
--rw-r--r--   0 themamad  (1000) themamad  (1000)     4400 2023-07-01 14:42:59.000000 balepy-0.7/balepy/__init__.py
-drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-07-01 14:43:26.358563 balepy-0.7/balepy.egg-info/
--rw-r--r--   0 themamad  (1000) themamad  (1000)      997 2023-07-01 14:43:26.000000 balepy-0.7/balepy.egg-info/PKG-INFO
--rw-r--r--   0 themamad  (1000) themamad  (1000)      165 2023-07-01 14:43:26.000000 balepy-0.7/balepy.egg-info/SOURCES.txt
--rw-r--r--   0 themamad  (1000) themamad  (1000)        1 2023-07-01 14:43:26.000000 balepy-0.7/balepy.egg-info/dependency_links.txt
--rw-r--r--   0 themamad  (1000) themamad  (1000)        7 2023-07-01 14:43:26.000000 balepy-0.7/balepy.egg-info/top_level.txt
--rw-r--r--   0 themamad  (1000) themamad  (1000)       38 2023-07-01 14:43:26.358563 balepy-0.7/setup.cfg
--rw-r--r--   0 themamad  (1000) themamad  (1000)      987 2023-07-01 14:42:17.000000 balepy-0.7/setup.py
+drwxr-xr-x   0 mamad     (1000) mamad     (1000)        0 2023-07-30 11:02:15.602303 balepy-0.9/
+-rw-r--r--   0 mamad     (1000) mamad     (1000)     1073 2023-07-29 20:43:35.000000 balepy-0.9/LICENSE
+-rw-r--r--   0 mamad     (1000) mamad     (1000)     1288 2023-07-30 11:02:15.602303 balepy-0.9/PKG-INFO
+-rw-r--r--   0 mamad     (1000) mamad     (1000)      535 2023-07-29 20:43:13.000000 balepy-0.9/README.md
+drwxr-xr-x   0 mamad     (1000) mamad     (1000)        0 2023-07-30 11:02:15.602303 balepy-0.9/balepy/
+-rw-r--r--   0 mamad     (1000) mamad     (1000)      156 2023-07-29 21:42:23.000000 balepy-0.9/balepy/__init__.py
+-rw-r--r--   0 mamad     (1000) mamad     (1000)     5604 2023-07-29 21:42:03.000000 balepy-0.9/balepy/client.py
+drwxr-xr-x   0 mamad     (1000) mamad     (1000)        0 2023-07-30 11:02:15.602303 balepy-0.9/balepy.egg-info/
+-rw-r--r--   0 mamad     (1000) mamad     (1000)     1288 2023-07-30 11:02:15.000000 balepy-0.9/balepy.egg-info/PKG-INFO
+-rw-r--r--   0 mamad     (1000) mamad     (1000)      182 2023-07-30 11:02:15.000000 balepy-0.9/balepy.egg-info/SOURCES.txt
+-rw-r--r--   0 mamad     (1000) mamad     (1000)        1 2023-07-30 11:02:15.000000 balepy-0.9/balepy.egg-info/dependency_links.txt
+-rw-r--r--   0 mamad     (1000) mamad     (1000)        7 2023-07-30 11:02:15.000000 balepy-0.9/balepy.egg-info/top_level.txt
+-rw-r--r--   0 mamad     (1000) mamad     (1000)       38 2023-07-30 11:02:15.602303 balepy-0.9/setup.cfg
+-rw-r--r--   0 mamad     (1000) mamad     (1000)      986 2023-07-29 21:43:06.000000 balepy-0.9/setup.py
```

### Comparing `balepy-0.7/LICENSE` & `balepy-0.9/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Mohammad Mehrabi Rad
+Copyright (c) 2023 Mamad Mehrabi Rad
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `balepy-0.7/setup.py` & `balepy-0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'balepy',
-    version = '0.7',
+    version = '0.9',
     author='Mohammad and Erfan',
     author_email = 'mohammadmehrabi175@gmail.com',
     description = 'balepy a Library Python for create bot API in bale application',
     keywords = ['bot' , 'Bot' , 'bale' , 'robot'],
     long_description = open("README.md", encoding="utf-8").read(),
     python_requires="~=3.6",
     long_description_content_type = 'text/markdown',
@@ -19,8 +19,8 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: MIT License",
     ]
-)
+)
```

