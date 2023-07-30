# Comparing `tmp/jaal-0.1.4.tar.gz` & `tmp/jaal-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaal-0.1.4.tar", last modified: Sun Jul 30 06:08:14 2023, max compression
+gzip compressed data, was "jaal-0.1.5.tar", last modified: Sun Jul 30 06:41:20 2023, max compression
```

## Comparing `jaal-0.1.4.tar` & `jaal-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:08:14.322129 jaal-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-30 06:07:56.000000 jaal-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-07-30 06:08:14.322129 jaal-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-07-30 06:07:56.000000 jaal-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:08:14.318129 jaal-0.1.4/jaal/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-30 06:07:56.000000 jaal-0.1.4/jaal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:08:14.322129 jaal-0.1.4/jaal/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-30 06:07:56.000000 jaal-0.1.4/jaal/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-30 06:07:56.000000 jaal-0.1.4/jaal/datasets/load_got.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-07-30 06:07:56.000000 jaal-0.1.4/jaal/datasets/parse_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    14666 2023-07-30 06:07:56.000000 jaal-0.1.4/jaal/jaal.py
--rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-07-30 06:07:56.000000 jaal-0.1.4/jaal/layout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:08:14.322129 jaal-0.1.4/jaal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-07-30 06:08:14.000000 jaal-0.1.4/jaal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-30 06:08:14.000000 jaal-0.1.4/jaal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 06:08:14.000000 jaal-0.1.4/jaal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-30 06:08:14.000000 jaal-0.1.4/jaal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-30 06:08:14.000000 jaal-0.1.4/jaal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 06:08:14.322129 jaal-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-30 06:07:56.000000 jaal-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:41:20.457198 jaal-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-30 06:41:05.000000 jaal-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-07-30 06:41:20.457198 jaal-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-07-30 06:41:05.000000 jaal-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:41:20.453198 jaal-0.1.5/jaal/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-30 06:41:05.000000 jaal-0.1.5/jaal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:41:20.457198 jaal-0.1.5/jaal/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-30 06:41:05.000000 jaal-0.1.5/jaal/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-30 06:41:05.000000 jaal-0.1.5/jaal/datasets/load_got.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-07-30 06:41:05.000000 jaal-0.1.5/jaal/datasets/parse_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14666 2023-07-30 06:41:05.000000 jaal-0.1.5/jaal/jaal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-07-30 06:41:05.000000 jaal-0.1.5/jaal/layout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:41:20.457198 jaal-0.1.5/jaal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-07-30 06:41:20.000000 jaal-0.1.5/jaal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-30 06:41:20.000000 jaal-0.1.5/jaal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 06:41:20.000000 jaal-0.1.5/jaal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-30 06:41:20.000000 jaal-0.1.5/jaal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-30 06:41:20.000000 jaal-0.1.5/jaal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 06:41:20.457198 jaal-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-30 06:41:05.000000 jaal-0.1.5/setup.py
```

### Comparing `jaal-0.1.4/LICENSE` & `jaal-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jaal-0.1.4/PKG-INFO` & `jaal-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaal
-Version: 0.1.4
+Version: 0.1.5
 Summary: jaal - your interactive network visualizer dashboard
 Home-page: https://github.com/imohitmayank/jaal
 Author: Mohit Mayank
 Author-email: mohitmayank1@gmail.com
 License: UNKNOWN
 Description: <img src="jaal/assets/logo.png" alt="jaal logo"/>
```

### Comparing `jaal-0.1.4/README.md` & `jaal-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `jaal-0.1.4/jaal/datasets/load_got.py` & `jaal-0.1.5/jaal/datasets/load_got.py`

 * *Files identical despite different names*

### Comparing `jaal-0.1.4/jaal/datasets/parse_dataframe.py` & `jaal-0.1.5/jaal/datasets/parse_dataframe.py`

 * *Files identical despite different names*

### Comparing `jaal-0.1.4/jaal/jaal.py` & `jaal-0.1.5/jaal/jaal.py`

 * *Files identical despite different names*

### Comparing `jaal-0.1.4/jaal/layout.py` & `jaal-0.1.5/jaal/layout.py`

 * *Files identical despite different names*

### Comparing `jaal-0.1.4/jaal.egg-info/PKG-INFO` & `jaal-0.1.5/jaal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaal
-Version: 0.1.4
+Version: 0.1.5
 Summary: jaal - your interactive network visualizer dashboard
 Home-page: https://github.com/imohitmayank/jaal
 Author: Mohit Mayank
 Author-email: mohitmayank1@gmail.com
 License: UNKNOWN
 Description: <img src="jaal/assets/logo.png" alt="jaal logo"/>
```

### Comparing `jaal-0.1.4/setup.py` & `jaal-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
-    package_data={'': ['datasets/*', 'assets/logo.png', 'datasets/got/*']},
+    package_data={'': ['datasets/*', 'assets/*', 'datasets/got/*']},
     include_package_data=True,
     install_requires=['dash>=1.19.0', 
                       'visdcc>=0.0.40', 
                       'pandas>=1.2.1', 
                       'dash_core_components>=1.15.0', 
                       'dash_html_components>=1.1.2', 
                       'dash_bootstrap_components<1'],
```

