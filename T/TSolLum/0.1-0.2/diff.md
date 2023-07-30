# Comparing `tmp/TSolLum-0.1.tar.gz` & `tmp/TSolLum-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TSolLum-0.1.tar", last modified: Sun Jul 30 15:28:19 2023, max compression
+gzip compressed data, was "TSolLum-0.2.tar", last modified: Sun Jul 30 15:32:08 2023, max compression
```

## Comparing `TSolLum-0.1.tar` & `TSolLum-0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 15:28:19.476408 TSolLum-0.1/
--rw-rw-rw-   0        0        0      426 2023-07-30 15:28:19.476408 TSolLum-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-30 15:28:19.476408 TSolLum-0.1/TSolLum.egg-info/
--rw-rw-rw-   0        0        0      426 2023-07-30 15:28:19.000000 TSolLum-0.1/TSolLum.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-07-30 15:28:19.000000 TSolLum-0.1/TSolLum.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 15:28:19.000000 TSolLum-0.1/TSolLum.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-07-30 15:28:19.000000 TSolLum-0.1/TSolLum.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 15:28:19.000000 TSolLum-0.1/TSolLum.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-30 15:28:19.492034 TSolLum-0.1/setup.cfg
--rw-rw-rw-   0        0        0      622 2023-07-30 15:28:01.000000 TSolLum-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 15:32:08.080560 TSolLum-0.2/
+-rw-rw-rw-   0        0        0      426 2023-07-30 15:32:08.080560 TSolLum-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-30 15:32:08.080560 TSolLum-0.2/TSolLum.egg-info/
+-rw-rw-rw-   0        0        0      426 2023-07-30 15:32:07.000000 TSolLum-0.2/TSolLum.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2023-07-30 15:32:08.000000 TSolLum-0.2/TSolLum.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 15:32:07.000000 TSolLum-0.2/TSolLum.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-30 15:32:07.000000 TSolLum-0.2/TSolLum.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 15:32:07.000000 TSolLum-0.2/TSolLum.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 15:32:08.080560 TSolLum-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      629 2023-07-30 15:31:57.000000 TSolLum-0.2/setup.py
```

### Comparing `TSolLum-0.1/setup.py` & `TSolLum-0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='TSolLum',
-    version='0.1',
+    version='0.2',
     author='JoHpt',
     description='TSolLum is a Python package designed to analyze the optical properties of a smart window coating material called vanadium dioxide.',
     url='https://github.com/JoHpt/TSolLum',
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.8',
-    install_requires=["io", "numpy", "scipy", "pandas", "matplotlib"],
+    install_requires=["Python-IO", "numpy", "scipy", "pandas", "matplotlib"],
 )
```

