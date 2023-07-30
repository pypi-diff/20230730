# Comparing `tmp/tambus-0.2.0.tar.gz` & `tmp/tambus-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tambus-0.2.0.tar", last modified: Sat Jul 29 19:58:43 2023, max compression
+gzip compressed data, was "tambus-1.0.0.tar", last modified: Sun Jul 30 19:53:40 2023, max compression
```

## Comparing `tambus-0.2.0.tar` & `tambus-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 19:58:43.145374 tambus-0.2.0/
--rw-rw-rw-   0        0        0     1063 2023-07-29 19:13:07.000000 tambus-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     1024 2023-07-29 19:58:43.141381 tambus-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      620 2023-07-29 19:57:54.000000 tambus-0.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-29 19:58:43.146383 tambus-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      620 2023-07-29 19:58:30.000000 tambus-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 19:58:43.088303 tambus-0.2.0/tambus/
--rw-rw-rw-   0        0        0       39 2023-07-29 19:53:54.000000 tambus-0.2.0/tambus/__init__.py
--rw-rw-rw-   0        0        0     2384 2023-07-29 19:05:00.000000 tambus-0.2.0/tambus/engine.py
-drwxrwxrwx   0        0        0        0 2023-07-29 19:58:43.127389 tambus-0.2.0/tambus.egg-info/
--rw-rw-rw-   0        0        0     1024 2023-07-29 19:58:42.000000 tambus-0.2.0/tambus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-07-29 19:58:42.000000 tambus-0.2.0/tambus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 19:58:42.000000 tambus-0.2.0/tambus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-29 19:58:42.000000 tambus-0.2.0/tambus.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 19:53:40.694512 tambus-1.0.0/
+-rw-rw-rw-   0        0        0     1063 2023-07-29 19:13:07.000000 tambus-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     1539 2023-07-30 19:53:40.693996 tambus-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1135 2023-07-30 19:50:19.000000 tambus-1.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-30 19:53:40.694512 tambus-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      620 2023-07-30 19:53:19.000000 tambus-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 19:53:40.625042 tambus-1.0.0/tambus/
+-rw-rw-rw-   0        0        0       77 2023-07-30 19:50:42.000000 tambus-1.0.0/tambus/__init__.py
+-rw-rw-rw-   0        0        0      231 2023-07-30 18:27:06.000000 tambus-1.0.0/tambus/components.py
+-rw-rw-rw-   0        0        0     4080 2023-07-30 19:50:01.000000 tambus-1.0.0/tambus/engine.py
+-rw-rw-rw-   0        0        0      327 2023-07-30 18:10:07.000000 tambus-1.0.0/tambus/mdengine.py
+drwxrwxrwx   0        0        0        0 2023-07-30 19:53:40.685473 tambus-1.0.0/tambus.egg-info/
+-rw-rw-rw-   0        0        0     1539 2023-07-30 19:53:40.000000 tambus-1.0.0/tambus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-07-30 19:53:40.000000 tambus-1.0.0/tambus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 19:53:40.000000 tambus-1.0.0/tambus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-30 19:53:40.000000 tambus-1.0.0/tambus.egg-info/top_level.txt
```

### Comparing `tambus-0.2.0/LICENSE` & `tambus-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tambus-0.2.0/setup.py` & `tambus-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tambus",
-    version="0.2.0",
+    version="1.0.0",
     author="Someone.",
     author_email="someonegithub@gmail.com",
     description="Bambus Template Engine",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/somespi/tambus",
     packages=setuptools.find_packages(),
```

