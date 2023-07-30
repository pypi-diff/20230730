# Comparing `tmp/strprogressbar-0.1.tar.gz` & `tmp/strprogressbar-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strprogressbar-0.1.tar", last modified: Sun Jul 30 10:14:33 2023, max compression
+gzip compressed data, was "strprogressbar-0.2.tar", last modified: Sun Jul 30 10:27:27 2023, max compression
```

## Comparing `strprogressbar-0.1.tar` & `strprogressbar-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 10:14:33.535668 strprogressbar-0.1/
--rw-rw-rw-   0        0        0    35823 2023-07-29 12:56:04.000000 strprogressbar-0.1/LICENSE
--rw-rw-rw-   0        0        0      648 2023-07-30 10:14:33.536659 strprogressbar-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6229 2023-07-30 10:13:33.000000 strprogressbar-0.1/README.md
--rw-rw-rw-   0        0        0       86 2023-07-30 10:14:33.537655 strprogressbar-0.1/setup.cfg
--rw-rw-rw-   0        0        0      789 2023-07-30 10:12:29.000000 strprogressbar-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-30 10:14:33.512738 strprogressbar-0.1/strprogressbar/
--rw-rw-rw-   0        0        0       53 2023-07-30 10:06:25.000000 strprogressbar-0.1/strprogressbar/__init__.py
--rw-rw-rw-   0        0        0     7971 2023-07-30 09:27:10.000000 strprogressbar-0.1/strprogressbar/strprogressbar.py
-drwxrwxrwx   0        0        0        0 2023-07-30 10:14:33.534666 strprogressbar-0.1/strprogressbar.egg-info/
--rw-rw-rw-   0        0        0      648 2023-07-30 10:14:33.000000 strprogressbar-0.1/strprogressbar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-07-30 10:14:33.000000 strprogressbar-0.1/strprogressbar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 10:14:33.000000 strprogressbar-0.1/strprogressbar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-30 10:14:33.000000 strprogressbar-0.1/strprogressbar.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 10:27:27.103689 strprogressbar-0.2/
+-rw-rw-rw-   0        0        0    35823 2023-07-29 12:56:04.000000 strprogressbar-0.2/LICENSE
+-rw-rw-rw-   0        0        0      648 2023-07-30 10:27:27.103689 strprogressbar-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6229 2023-07-30 10:13:33.000000 strprogressbar-0.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-30 10:27:27.109670 strprogressbar-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      789 2023-07-30 10:25:19.000000 strprogressbar-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 10:27:27.085749 strprogressbar-0.2/strprogressbar/
+-rw-rw-rw-   0        0        0       53 2023-07-30 10:06:25.000000 strprogressbar-0.2/strprogressbar/__init__.py
+-rw-rw-rw-   0        0        0     7971 2023-07-30 09:27:10.000000 strprogressbar-0.2/strprogressbar/strprogressbar.py
+drwxrwxrwx   0        0        0        0 2023-07-30 10:27:27.101696 strprogressbar-0.2/strprogressbar.egg-info/
+-rw-rw-rw-   0        0        0      648 2023-07-30 10:27:26.000000 strprogressbar-0.2/strprogressbar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-07-30 10:27:26.000000 strprogressbar-0.2/strprogressbar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 10:27:26.000000 strprogressbar-0.2/strprogressbar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-30 10:27:26.000000 strprogressbar-0.2/strprogressbar.egg-info/top_level.txt
```

### Comparing `strprogressbar-0.1/LICENSE` & `strprogressbar-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `strprogressbar-0.1/PKG-INFO` & `strprogressbar-0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: strprogressbar
-Version: 0.1
+Version: 0.2
 Home-page: https://github.com/SDeVuyst/strprogressbar
-Download-URL: https://github.com/SDeVuyst/strprogressbar/archive/refs/tags/v_0.1.tar.gz
+Download-URL: https://github.com/SDeVuyst/strprogressbar/archive/refs/tags/v_0.2.tar.gz
 Author: SDeVuyst
 Author-email: 
 License: GNU General Public License v3 (GPLv3)
 Keywords: string,progressbar,progress,bar
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `strprogressbar-0.1/README.md` & `strprogressbar-0.2/README.md`

 * *Files identical despite different names*

### Comparing `strprogressbar-0.1/setup.py` & `strprogressbar-0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,18 +6,18 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
   'Programming Language :: Python :: 3'
 ]
 
 setup(
   name='strprogressbar',
-  version='0.1',
+  version='0.2',
   description='',
   url='https://github.com/SDeVuyst/strprogressbar',  
-  download_url='https://github.com/SDeVuyst/strprogressbar/archive/refs/tags/v_0.1.tar.gz',
+  download_url='https://github.com/SDeVuyst/strprogressbar/archive/refs/tags/v_0.2.tar.gz',
   author='SDeVuyst',
   author_email='',  
   license='GNU General Public License v3 (GPLv3)', 
   classifiers=classifiers,
   keywords=['string', 'progressbar', 'progress', 'bar'], 
   packages=find_packages(),
   install_requires=['']
```

### Comparing `strprogressbar-0.1/strprogressbar/strprogressbar.py` & `strprogressbar-0.2/strprogressbar/strprogressbar.py`

 * *Files identical despite different names*

### Comparing `strprogressbar-0.1/strprogressbar.egg-info/PKG-INFO` & `strprogressbar-0.2/strprogressbar.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: strprogressbar
-Version: 0.1
+Version: 0.2
 Home-page: https://github.com/SDeVuyst/strprogressbar
-Download-URL: https://github.com/SDeVuyst/strprogressbar/archive/refs/tags/v_0.1.tar.gz
+Download-URL: https://github.com/SDeVuyst/strprogressbar/archive/refs/tags/v_0.2.tar.gz
 Author: SDeVuyst
 Author-email: 
 License: GNU General Public License v3 (GPLv3)
 Keywords: string,progressbar,progress,bar
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

