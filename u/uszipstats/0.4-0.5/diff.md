# Comparing `tmp/uszipstats-0.4.tar.gz` & `tmp/uszipstats-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uszipstats-0.4.tar", last modified: Sun Jul 30 16:38:29 2023, max compression
+gzip compressed data, was "uszipstats-0.5.tar", last modified: Sun Jul 30 16:44:10 2023, max compression
```

## Comparing `uszipstats-0.4.tar` & `uszipstats-0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-30 16:38:29.711622 uszipstats-0.4/
--rw-r--r--   0 vedantrathi   (501) staff       (20)     1065 2023-07-25 18:05:29.000000 uszipstats-0.4/LICENSE.txt
--rw-r--r--   0 vedantrathi   (501) staff       (20)     4494 2023-07-30 16:38:29.711768 uszipstats-0.4/PKG-INFO
--rw-r--r--   0 vedantrathi   (501) staff       (20)     3680 2023-07-30 16:37:20.000000 uszipstats-0.4/README.md
-drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-30 16:38:29.707872 uszipstats-0.4/code_zip/
--rw-r--r--   0 vedantrathi   (501) staff       (20)       23 2023-07-25 19:42:59.000000 uszipstats-0.4/code_zip/__init__.py
--rw-r--r--   0 vedantrathi   (501) staff       (20)    40386 2023-07-25 18:32:05.000000 uszipstats-0.4/code_zip/irs_data.py
--rw-r--r--   0 vedantrathi   (501) staff       (20)       79 2023-07-30 16:38:29.712258 uszipstats-0.4/setup.cfg
--rw-r--r--   0 vedantrathi   (501) staff       (20)     1803 2023-07-30 16:37:31.000000 uszipstats-0.4/setup.py
-drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-30 16:38:29.711386 uszipstats-0.4/uszipstats.egg-info/
--rw-r--r--   0 vedantrathi   (501) staff       (20)     4494 2023-07-30 16:38:29.000000 uszipstats-0.4/uszipstats.egg-info/PKG-INFO
--rw-r--r--   0 vedantrathi   (501) staff       (20)      251 2023-07-30 16:38:29.000000 uszipstats-0.4/uszipstats.egg-info/SOURCES.txt
--rw-r--r--   0 vedantrathi   (501) staff       (20)        1 2023-07-30 16:38:29.000000 uszipstats-0.4/uszipstats.egg-info/dependency_links.txt
--rw-r--r--   0 vedantrathi   (501) staff       (20)       33 2023-07-30 16:38:29.000000 uszipstats-0.4/uszipstats.egg-info/requires.txt
--rw-r--r--   0 vedantrathi   (501) staff       (20)        9 2023-07-30 16:38:29.000000 uszipstats-0.4/uszipstats.egg-info/top_level.txt
+drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-30 16:44:10.110174 uszipstats-0.5/
+-rw-r--r--   0 vedantrathi   (501) staff       (20)     1065 2023-07-25 18:05:29.000000 uszipstats-0.5/LICENSE.txt
+-rw-r--r--   0 vedantrathi   (501) staff       (20)     4499 2023-07-30 16:44:10.110310 uszipstats-0.5/PKG-INFO
+-rw-r--r--   0 vedantrathi   (501) staff       (20)     3685 2023-07-30 16:43:44.000000 uszipstats-0.5/README.md
+drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-30 16:44:10.106740 uszipstats-0.5/code_zip/
+-rw-r--r--   0 vedantrathi   (501) staff       (20)       23 2023-07-25 19:42:59.000000 uszipstats-0.5/code_zip/__init__.py
+-rw-r--r--   0 vedantrathi   (501) staff       (20)    40386 2023-07-25 18:32:05.000000 uszipstats-0.5/code_zip/irs_data.py
+-rw-r--r--   0 vedantrathi   (501) staff       (20)       79 2023-07-30 16:44:10.110781 uszipstats-0.5/setup.cfg
+-rw-r--r--   0 vedantrathi   (501) staff       (20)     1803 2023-07-30 16:44:02.000000 uszipstats-0.5/setup.py
+drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-30 16:44:10.109944 uszipstats-0.5/uszipstats.egg-info/
+-rw-r--r--   0 vedantrathi   (501) staff       (20)     4499 2023-07-30 16:44:09.000000 uszipstats-0.5/uszipstats.egg-info/PKG-INFO
+-rw-r--r--   0 vedantrathi   (501) staff       (20)      251 2023-07-30 16:44:10.000000 uszipstats-0.5/uszipstats.egg-info/SOURCES.txt
+-rw-r--r--   0 vedantrathi   (501) staff       (20)        1 2023-07-30 16:44:09.000000 uszipstats-0.5/uszipstats.egg-info/dependency_links.txt
+-rw-r--r--   0 vedantrathi   (501) staff       (20)       33 2023-07-30 16:44:09.000000 uszipstats-0.5/uszipstats.egg-info/requires.txt
+-rw-r--r--   0 vedantrathi   (501) staff       (20)        9 2023-07-30 16:44:09.000000 uszipstats-0.5/uszipstats.egg-info/top_level.txt
```

### Comparing `uszipstats-0.4/LICENSE.txt` & `uszipstats-0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `uszipstats-0.4/PKG-INFO` & `uszipstats-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: uszipstats
-Version: 0.4
+Version: 0.5
 Summary: This package will provide the ability to access IRS data
 Home-page: https://github.com/vrathi101/uszipstats.git
-Download-URL: https://github.com/vrathi101/uszipstats/archive/refs/tags/v_04.tar.gz
+Download-URL: https://github.com/vrathi101/uszipstats/archive/refs/tags/v_05.tar.gz
 Author: VEDANT RATHI
 Author-email: vedrathi10@gmail.com
 License: MIT
 Keywords: DATA,FUNCTIONS
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 <h1 align="center">
-<img src="https://raw.githubusercontent.com/vrathi101/uszipstats/main/TaxFilingFusion.png" alt="Project Logo" height="200" width="200" style="display: inline-block;">
+<img src="https://raw.githubusercontent.com/vrathi101/uszipstats/main/Logo/TaxFilingFusion.png" alt="Project Logo" height="200" width="200" style="display: inline-block;">
 </h1><be>
 
 TaxFilingFusion stands as the ultimate solution for effortlessly accessing and navigating IRS tax filing data. This powerful package effortlessly transforms complexity into simplicity, empowering users to unlock fresh insights and delve deep into data analysis. Unravel the potential of tax data like never before – whether you're an expert or just starting out, TaxFilingFusion makes IRS data accessible and user-friendly for all.
 
 Call for Contributions
 ----------------------
 It provides:
```

### Comparing `uszipstats-0.4/README.md` & `uszipstats-0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <h1 align="center">
-<img src="https://raw.githubusercontent.com/vrathi101/uszipstats/main/TaxFilingFusion.png" alt="Project Logo" height="200" width="200" style="display: inline-block;">
+<img src="https://raw.githubusercontent.com/vrathi101/uszipstats/main/Logo/TaxFilingFusion.png" alt="Project Logo" height="200" width="200" style="display: inline-block;">
 </h1><be>
 
 TaxFilingFusion stands as the ultimate solution for effortlessly accessing and navigating IRS tax filing data. This powerful package effortlessly transforms complexity into simplicity, empowering users to unlock fresh insights and delve deep into data analysis. Unravel the potential of tax data like never before – whether you're an expert or just starting out, TaxFilingFusion makes IRS data accessible and user-friendly for all.
 
 Call for Contributions
 ----------------------
 It provides:
```

### Comparing `uszipstats-0.4/code_zip/irs_data.py` & `uszipstats-0.5/code_zip/irs_data.py`

 * *Files identical despite different names*

### Comparing `uszipstats-0.4/setup.py` & `uszipstats-0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,25 +2,25 @@
     with open('README.md', 'r', encoding='utf-8') as f:
         return f.read()
 
 import setuptools
 setuptools.setup(
     name='uszipstats',         # How you named your package
     packages=['code_zip'],   # Chose the same as "name"
-    version='0.4',      # Start with a small number and increase it with every change you make
+    version='0.5',      # Start with a small number and increase it with every change you make
     license='MIT',
     description='This package will provide the ability to access IRS data',   # Give a short description about your library
     long_description=read_readme(),
     long_description_content_type='text/markdown',
     author='VEDANT RATHI',                   # Type in your name
     author_email='vedrathi10@gmail.com',      # Type in your E-Mail
     # Provide either the link to your github or to your website
     url='https://github.com/vrathi101/uszipstats.git',
     # I explain this later on
-    download_url='https://github.com/vrathi101/uszipstats/archive/refs/tags/v_04.tar.gz',
+    download_url='https://github.com/vrathi101/uszipstats/archive/refs/tags/v_05.tar.gz',
     keywords=['DATA', 'FUNCTIONS'],   # Keywords that define your package best
     install_requires=[
         'pandas',
         'numpy',
         'requests',
         'matplotlib',
     ],
```

### Comparing `uszipstats-0.4/uszipstats.egg-info/PKG-INFO` & `uszipstats-0.5/uszipstats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: uszipstats
-Version: 0.4
+Version: 0.5
 Summary: This package will provide the ability to access IRS data
 Home-page: https://github.com/vrathi101/uszipstats.git
-Download-URL: https://github.com/vrathi101/uszipstats/archive/refs/tags/v_04.tar.gz
+Download-URL: https://github.com/vrathi101/uszipstats/archive/refs/tags/v_05.tar.gz
 Author: VEDANT RATHI
 Author-email: vedrathi10@gmail.com
 License: MIT
 Keywords: DATA,FUNCTIONS
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 <h1 align="center">
-<img src="https://raw.githubusercontent.com/vrathi101/uszipstats/main/TaxFilingFusion.png" alt="Project Logo" height="200" width="200" style="display: inline-block;">
+<img src="https://raw.githubusercontent.com/vrathi101/uszipstats/main/Logo/TaxFilingFusion.png" alt="Project Logo" height="200" width="200" style="display: inline-block;">
 </h1><be>
 
 TaxFilingFusion stands as the ultimate solution for effortlessly accessing and navigating IRS tax filing data. This powerful package effortlessly transforms complexity into simplicity, empowering users to unlock fresh insights and delve deep into data analysis. Unravel the potential of tax data like never before – whether you're an expert or just starting out, TaxFilingFusion makes IRS data accessible and user-friendly for all.
 
 Call for Contributions
 ----------------------
 It provides:
```

