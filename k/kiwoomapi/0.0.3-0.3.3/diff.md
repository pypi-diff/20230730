# Comparing `tmp/kiwoomapi-0.0.3.tar.gz` & `tmp/kiwoomapi-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiwoomapi-0.0.3.tar", last modified: Fri Mar 24 02:30:48 2023, max compression
+gzip compressed data, was "kiwoomapi-0.3.3.tar", last modified: Sun Jul 30 05:24:02 2023, max compression
```

## Comparing `kiwoomapi-0.0.3.tar` & `kiwoomapi-0.3.3.tar`

### file list

```diff
@@ -1,12 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-24 02:30:48.921076 kiwoomapi-0.0.3/
--rw-rw-rw-   0        0        0     1086 2023-03-24 01:15:08.000000 kiwoomapi-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      630 2023-03-24 02:30:48.920077 kiwoomapi-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      114 2023-03-24 01:15:08.000000 kiwoomapi-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-03-24 02:30:48.922077 kiwoomapi-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      813 2023-03-24 02:27:57.000000 kiwoomapi-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-24 02:30:48.902604 kiwoomapi-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-03-24 02:30:48.919076 kiwoomapi-0.0.3/src/kiwoomapi.egg-info/
--rw-rw-rw-   0        0        0      630 2023-03-24 02:30:48.000000 kiwoomapi-0.0.3/src/kiwoomapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-03-24 02:30:48.000000 kiwoomapi-0.0.3/src/kiwoomapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-24 02:30:48.000000 kiwoomapi-0.0.3/src/kiwoomapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-03-24 02:30:48.000000 kiwoomapi-0.0.3/src/kiwoomapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 05:24:02.332140 kiwoomapi-0.3.3/
+-rw-rw-rw-   0        0        0     1086 2023-07-30 00:42:00.000000 kiwoomapi-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0      897 2023-07-30 05:24:02.330139 kiwoomapi-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-07-30 03:08:26.000000 kiwoomapi-0.3.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-30 05:24:02.332140 kiwoomapi-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      879 2023-07-30 05:23:45.000000 kiwoomapi-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 05:24:02.291131 kiwoomapi-0.3.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-30 05:24:02.305134 kiwoomapi-0.3.3/src/kiwoomapi/
+-rw-rw-rw-   0        0        0     9387 2023-07-30 05:22:47.000000 kiwoomapi-0.3.3/src/kiwoomapi/__init__.py
+-rw-rw-rw-   0        0        0     1110 2023-07-30 00:42:00.000000 kiwoomapi-0.3.3/src/kiwoomapi/const.py
+-rw-rw-rw-   0        0        0     3263 2023-07-30 00:42:00.000000 kiwoomapi-0.3.3/src/kiwoomapi/recv.py
+drwxrwxrwx   0        0        0        0 2023-07-30 05:24:02.328140 kiwoomapi-0.3.3/src/kiwoomapi.egg-info/
+-rw-rw-rw-   0        0        0      897 2023-07-30 05:24:02.000000 kiwoomapi-0.3.3/src/kiwoomapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2023-07-30 05:24:02.000000 kiwoomapi-0.3.3/src/kiwoomapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 05:24:02.000000 kiwoomapi-0.3.3/src/kiwoomapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-30 05:24:02.000000 kiwoomapi-0.3.3/src/kiwoomapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-30 05:24:02.000000 kiwoomapi-0.3.3/src/kiwoomapi.egg-info/top_level.txt
```

### Comparing `kiwoomapi-0.0.3/LICENSE` & `kiwoomapi-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwoomapi-0.0.3/setup.py` & `kiwoomapi-0.3.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,23 +2,26 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kiwoomapi",
-    version="0.0.3",
+    version="0.3.3",
     author="innovata sambong",
     author_email="iinnovata@gmail.com",
     description='Windows COM 기반으로 파이썬 32비트로만 동작하는 키움증권 오픈API 패키지',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=f"https://github.com/innovata/KiwoomOpenAPI",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"":"src"},
-    packages=setuptools.find_packages(),
+    packages=setuptools.find_packages('src'),
     python_requires=">=3.8",
+    install_requires=[
+        'PyQt5', 'ipylib', 
+    ],
 )
```

