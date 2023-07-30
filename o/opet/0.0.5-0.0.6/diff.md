# Comparing `tmp/opet-0.0.5.tar.gz` & `tmp/opet-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opet-0.0.5.tar", last modified: Sun Jul 30 16:28:54 2023, max compression
+gzip compressed data, was "opet-0.0.6.tar", last modified: Sun Jul 30 20:36:46 2023, max compression
```

## Comparing `opet-0.0.5.tar` & `opet-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxr-xr-x   0 btcyz255   (501) staff       (20)        0 2023-07-30 16:28:54.046502 opet-0.0.5/
--rw-r--r--   0 btcyz255   (501) staff       (20)     1069 2023-07-30 14:59:51.000000 opet-0.0.5/LICENSE
--rw-r--r--   0 btcyz255   (501) staff       (20)      565 2023-07-30 16:28:54.046314 opet-0.0.5/PKG-INFO
--rw-r--r--   0 btcyz255   (501) staff       (20)       91 2023-07-30 13:14:54.000000 opet-0.0.5/README.md
-drwxr-xr-x   0 btcyz255   (501) staff       (20)        0 2023-07-30 16:28:54.042531 opet-0.0.5/opet/
-drwxr-xr-x   0 btcyz255   (501) staff       (20)        0 2023-07-30 16:28:54.045948 opet-0.0.5/opet/opet.egg-info/
--rw-r--r--   0 btcyz255   (501) staff       (20)      565 2023-07-30 16:28:54.000000 opet-0.0.5/opet/opet.egg-info/PKG-INFO
--rw-r--r--   0 btcyz255   (501) staff       (20)      190 2023-07-30 16:28:54.000000 opet-0.0.5/opet/opet.egg-info/SOURCES.txt
--rw-r--r--   0 btcyz255   (501) staff       (20)        1 2023-07-30 16:28:54.000000 opet-0.0.5/opet/opet.egg-info/dependency_links.txt
--rw-r--r--   0 btcyz255   (501) staff       (20)        9 2023-07-30 16:28:54.000000 opet-0.0.5/opet/opet.egg-info/requires.txt
--rw-r--r--   0 btcyz255   (501) staff       (20)        1 2023-07-30 16:28:54.000000 opet-0.0.5/opet/opet.egg-info/top_level.txt
--rw-r--r--   0 btcyz255   (501) staff       (20)       38 2023-07-30 16:28:54.046549 opet-0.0.5/setup.cfg
--rw-r--r--   0 btcyz255   (501) staff       (20)      781 2023-07-30 16:28:34.000000 opet-0.0.5/setup.py
+drwxr-xr-x   0 btcyz255   (501) staff       (20)        0 2023-07-30 20:36:46.291995 opet-0.0.6/
+-rw-r--r--   0 btcyz255   (501) staff       (20)     1069 2023-07-30 14:59:51.000000 opet-0.0.6/LICENSE
+-rw-r--r--   0 btcyz255   (501) staff       (20)     1029 2023-07-30 20:36:46.291776 opet-0.0.6/PKG-INFO
+-rw-r--r--   0 btcyz255   (501) staff       (20)      555 2023-07-30 20:36:28.000000 opet-0.0.6/README.md
+-rw-r--r--   0 btcyz255   (501) staff       (20)       38 2023-07-30 20:36:46.292056 opet-0.0.6/setup.cfg
+-rw-r--r--   0 btcyz255   (501) staff       (20)      815 2023-07-30 20:33:35.000000 opet-0.0.6/setup.py
+drwxr-xr-x   0 btcyz255   (501) staff       (20)        0 2023-07-30 20:36:46.285596 opet-0.0.6/src/
+drwxr-xr-x   0 btcyz255   (501) staff       (20)        0 2023-07-30 20:36:46.289101 opet-0.0.6/src/opet/
+-rw-r--r--   0 btcyz255   (501) staff       (20)        0 2023-07-30 20:11:51.000000 opet-0.0.6/src/opet/__init__.py
+-rw-r--r--   0 btcyz255   (501) staff       (20)      866 2023-07-30 19:26:06.000000 opet-0.0.6/src/opet/api.py
+-rw-r--r--   0 btcyz255   (501) staff       (20)       79 2023-07-30 14:21:02.000000 opet-0.0.6/src/opet/exceptions.py
+-rw-r--r--   0 btcyz255   (501) staff       (20)      918 2023-07-30 19:29:32.000000 opet-0.0.6/src/opet/utils.py
+drwxr-xr-x   0 btcyz255   (501) staff       (20)        0 2023-07-30 20:36:46.291313 opet-0.0.6/src/opet.egg-info/
+-rw-r--r--   0 btcyz255   (501) staff       (20)     1029 2023-07-30 20:36:46.000000 opet-0.0.6/src/opet.egg-info/PKG-INFO
+-rw-r--r--   0 btcyz255   (501) staff       (20)      263 2023-07-30 20:36:46.000000 opet-0.0.6/src/opet.egg-info/SOURCES.txt
+-rw-r--r--   0 btcyz255   (501) staff       (20)        1 2023-07-30 20:36:46.000000 opet-0.0.6/src/opet.egg-info/dependency_links.txt
+-rw-r--r--   0 btcyz255   (501) staff       (20)        9 2023-07-30 20:36:46.000000 opet-0.0.6/src/opet.egg-info/requires.txt
+-rw-r--r--   0 btcyz255   (501) staff       (20)        5 2023-07-30 20:36:46.000000 opet-0.0.6/src/opet.egg-info/top_level.txt
```

### Comparing `opet-0.0.5/LICENSE` & `opet-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `opet-0.0.5/setup.py` & `opet-0.0.6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 
-
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="opet",
-    version="0.0.5",
-    install_requires=["requests"],
     author="Sinan Erdinc",
     author_email="hello@sinanerdinc.com",
+    version="0.0.6",
+    install_requires=["requests"],
+    include_package_data=True,
     description="A Python package that allows you to view fuel prices in Turkey based on cities.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sinanerdinc/opet",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    packages=find_packages("opet"),
-    package_dir={"": "opet"},
+    package_dir={'': 'src'},
+    packages=find_packages(where='src'),
     python_requires=">=3.0"
 )
```

