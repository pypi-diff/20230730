# Comparing `tmp/nec_beamer-0.1.3.tar.gz` & `tmp/nec_beamer-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nec_beamer-0.1.3.tar", last modified: Sat Jul 29 22:00:12 2023, max compression
+gzip compressed data, was "nec_beamer-0.1.4.tar", last modified: Sat Jul 29 22:23:08 2023, max compression
```

## Comparing `nec_beamer-0.1.3.tar` & `nec_beamer-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mhp        (502) staff       (20)        0 2023-07-29 22:00:12.261761 nec_beamer-0.1.3/
--rw-r--r--   0 mhp        (502) staff       (20)     1072 2023-07-29 19:57:55.000000 nec_beamer-0.1.3/LICENSE
--rw-r--r--   0 mhp        (502) staff       (20)      479 2023-07-29 22:00:12.261626 nec_beamer-0.1.3/PKG-INFO
--rw-r--r--   0 mhp        (502) staff       (20)      188 2023-07-29 19:57:55.000000 nec_beamer-0.1.3/README.md
-drwxr-xr-x   0 mhp        (502) staff       (20)        0 2023-07-29 22:00:12.259737 nec_beamer-0.1.3/bin/
--rw-r--r--   0 mhp        (502) staff       (20)     5968 2023-07-29 21:53:38.000000 nec_beamer-0.1.3/bin/nec_beamer
-drwxr-xr-x   0 mhp        (502) staff       (20)        0 2023-07-29 22:00:12.260366 nec_beamer-0.1.3/nec_beamer/
--rw-r--r--   0 mhp        (502) staff       (20)       34 2023-07-29 20:47:52.000000 nec_beamer-0.1.3/nec_beamer/__init__.py
--rw-r--r--   0 mhp        (502) staff       (20)    12555 2023-07-29 21:48:48.000000 nec_beamer-0.1.3/nec_beamer/nec_beamer.py
-drwxr-xr-x   0 mhp        (502) staff       (20)        0 2023-07-29 22:00:12.261419 nec_beamer-0.1.3/nec_beamer.egg-info/
--rw-r--r--   0 mhp        (502) staff       (20)      479 2023-07-29 22:00:12.000000 nec_beamer-0.1.3/nec_beamer.egg-info/PKG-INFO
--rw-r--r--   0 mhp        (502) staff       (20)      291 2023-07-29 22:00:12.000000 nec_beamer-0.1.3/nec_beamer.egg-info/SOURCES.txt
--rw-r--r--   0 mhp        (502) staff       (20)        1 2023-07-29 22:00:12.000000 nec_beamer-0.1.3/nec_beamer.egg-info/dependency_links.txt
--rw-r--r--   0 mhp        (502) staff       (20)        1 2023-07-29 20:44:20.000000 nec_beamer-0.1.3/nec_beamer.egg-info/not-zip-safe
--rw-r--r--   0 mhp        (502) staff       (20)       15 2023-07-29 22:00:12.000000 nec_beamer-0.1.3/nec_beamer.egg-info/requires.txt
--rw-r--r--   0 mhp        (502) staff       (20)       11 2023-07-29 22:00:12.000000 nec_beamer-0.1.3/nec_beamer.egg-info/top_level.txt
--rw-r--r--   0 mhp        (502) staff       (20)       38 2023-07-29 22:00:12.261832 nec_beamer-0.1.3/setup.cfg
--rw-r--r--   0 mhp        (502) staff       (20)      561 2023-07-29 21:59:58.000000 nec_beamer-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:23:08.271919 nec_beamer-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-29 22:22:56.000000 nec_beamer-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-29 22:23:08.271919 nec_beamer-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-29 22:22:56.000000 nec_beamer-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:23:08.267919 nec_beamer-0.1.4/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-07-29 22:22:56.000000 nec_beamer-0.1.4/bin/nec_beamer
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:23:08.267919 nec_beamer-0.1.4/nec_beamer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-29 22:22:56.000000 nec_beamer-0.1.4/nec_beamer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12555 2023-07-29 22:22:56.000000 nec_beamer-0.1.4/nec_beamer/nec_beamer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:23:08.271919 nec_beamer-0.1.4/nec_beamer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-29 22:23:08.000000 nec_beamer-0.1.4/nec_beamer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-29 22:23:08.000000 nec_beamer-0.1.4/nec_beamer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 22:23:08.000000 nec_beamer-0.1.4/nec_beamer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 22:23:08.000000 nec_beamer-0.1.4/nec_beamer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 22:23:08.000000 nec_beamer-0.1.4/nec_beamer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-29 22:23:08.000000 nec_beamer-0.1.4/nec_beamer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 22:23:08.271919 nec_beamer-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-29 22:22:56.000000 nec_beamer-0.1.4/setup.py
```

### Comparing `nec_beamer-0.1.3/LICENSE` & `nec_beamer-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nec_beamer-0.1.3/bin/nec_beamer` & `nec_beamer-0.1.4/bin/nec_beamer`

 * *Files identical despite different names*

### Comparing `nec_beamer-0.1.3/nec_beamer/nec_beamer.py` & `nec_beamer-0.1.4/nec_beamer/nec_beamer.py`

 * *Files identical despite different names*

### Comparing `nec_beamer-0.1.3/setup.py` & `nec_beamer-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='nec_beamer',
-      version='0.1.3',
+      version='0.1.4',
       description='NEC Beamer Web Interface Wrapper',
       url='https://github.com/heinrich-foto/nec_beamer',
       author='Heinrich-Foto',
       author_email='nec_beamer@heinrich-foto.de',
       license='MIT',
       packages=['nec_beamer'],
       install_requires=[
```

