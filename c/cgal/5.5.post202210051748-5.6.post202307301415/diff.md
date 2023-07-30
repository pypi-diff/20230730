# Comparing `tmp/cgal-5.5.post202210051748.tar.gz` & `tmp/cgal-5.6.post202307301415.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgal-5.5.post202210051748.tar", last modified: Wed Oct  5 16:13:44 2022, max compression
+gzip compressed data, was "cgal-5.6.post202307301415.tar", last modified: Sun Jul 30 12:51:47 2023, max compression
```

## Comparing `cgal-5.5.post202210051748.tar` & `cgal-5.6.post202307301415.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 16:13:44.071141 cgal-5.5.post202210051748/
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-10-05 16:13:29.000000 cgal-5.5.post202210051748/LICENSE.COMMERCIAL
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2022-10-05 16:13:29.000000 cgal-5.5.post202210051748/LICENSE.GPL
--rw-r--r--   0 runner    (1001) docker     (121)     1249 2022-10-05 16:13:44.071141 cgal-5.5.post202210051748/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-10-05 16:13:29.000000 cgal-5.5.post202210051748/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 16:13:44.071141 cgal-5.5.post202210051748/cgal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1249 2022-10-05 16:13:43.000000 cgal-5.5.post202210051748/cgal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-10-05 16:13:43.000000 cgal-5.5.post202210051748/cgal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-05 16:13:43.000000 cgal-5.5.post202210051748/cgal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-05 16:13:43.000000 cgal-5.5.post202210051748/cgal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)      650 2022-10-05 16:13:43.000000 cgal-5.5.post202210051748/cgal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-05 16:13:44.071141 cgal-5.5.post202210051748/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)    17025 2022-10-05 16:13:29.000000 cgal-5.5.post202210051748/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:51:47.704811 cgal-5.6.post202307301415/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-30 12:51:30.000000 cgal-5.6.post202307301415/LICENSE.COMMERCIAL
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-30 12:51:30.000000 cgal-5.6.post202307301415/LICENSE.GPL
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-30 12:51:47.704811 cgal-5.6.post202307301415/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-30 12:51:30.000000 cgal-5.6.post202307301415/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:51:47.704811 cgal-5.6.post202307301415/cgal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-30 12:51:47.000000 cgal-5.6.post202307301415/cgal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-30 12:51:47.000000 cgal-5.6.post202307301415/cgal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 12:51:47.000000 cgal-5.6.post202307301415/cgal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-30 12:51:47.000000 cgal-5.6.post202307301415/cgal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-30 12:51:47.000000 cgal-5.6.post202307301415/cgal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 12:51:47.704811 cgal-5.6.post202307301415/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    17025 2023-07-30 12:51:30.000000 cgal-5.6.post202307301415/setup.py
```

### Comparing `cgal-5.5.post202210051748/LICENSE.GPL` & `cgal-5.6.post202307301415/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `cgal-5.5.post202210051748/PKG-INFO` & `cgal-5.6.post202307301415/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cgal
-Version: 5.5.post202210051748
-Summary: CGAL bindings, allowing to use some of the CGAL library in python.
+Version: 5.6.post202307301415
+Summary: CGAL bindings, allowing to use some of the CGAL library in Python.
 Home-page: https://github.com/CGAL/cgal-swig-bindings
 Author: CGAL Project
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
@@ -18,8 +18,8 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.COMMERCIAL
 License-File: LICENSE.GPL
 
-The CGAL Bindings project allows to use some packages of CGAL, the Computational Algorithms Library with python. This project is still experimental and more packages will be added. For more information, please visit https://github.com/CGAL/cgal-swig-bindings/wiki.
+The CGAL Bindings project allows to use some packages of CGAL, the Computational Algorithms Library with Python. This project is still experimental and more packages will be added. For more information, please visit https://github.com/CGAL/cgal-swig-bindings/wiki.
```

### Comparing `cgal-5.5.post202210051748/cgal.egg-info/PKG-INFO` & `cgal-5.6.post202307301415/cgal.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cgal
-Version: 5.5.post202210051748
-Summary: CGAL bindings, allowing to use some of the CGAL library in python.
+Version: 5.6.post202307301415
+Summary: CGAL bindings, allowing to use some of the CGAL library in Python.
 Home-page: https://github.com/CGAL/cgal-swig-bindings
 Author: CGAL Project
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
@@ -18,8 +18,8 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.COMMERCIAL
 License-File: LICENSE.GPL
 
-The CGAL Bindings project allows to use some packages of CGAL, the Computational Algorithms Library with python. This project is still experimental and more packages will be added. For more information, please visit https://github.com/CGAL/cgal-swig-bindings/wiki.
+The CGAL Bindings project allows to use some packages of CGAL, the Computational Algorithms Library with Python. This project is still experimental and more packages will be added. For more information, please visit https://github.com/CGAL/cgal-swig-bindings/wiki.
```

### Comparing `cgal-5.5.post202210051748/cgal.egg-info/top_level.txt` & `cgal-5.6.post202307301415/cgal.egg-info/top_level.txt`

 * *Files identical despite different names*

### Comparing `cgal-5.5.post202210051748/setup.py` & `cgal-5.6.post202307301415/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
            ('mpfr-include-dir=', None, 'Specify the path to the mpfr incude directory.'),
            ('mpfr-lib=', None, 'Specify the path to the mpfr library file.'),
            ('zlib-include-dir=', None, 'Specify the path to the zlib incude directory.'),
            ('zlib-lib=', None, 'Specify the path to the zlib library file.'),
            ('cmake-prefix-path=', None, 'Specify the path to a directory that can be used as CMAKE_PREFIX_PATH, that would contain all headers and libraries. '),
            ('generator=', None, 'The generator to use for cmake.'),
            ('python-executable=', None, 'The path to the python executable.'),
-           ('python-root=', None, 'The path to the python root directory.'),
+           ('python-root=', None, 'The path to the Python root directory.'),
            ('cmake=', None, 'Specify the path to the cmake executable.')
          ]
 
 def get_option_pairs():
   values ={('cgal_dir', 'cgal_dir'),
          ('boost_dir', 'boost_dir'),
          ('tbb_include_dir','tbb_include_dir'),
@@ -397,16 +397,16 @@
         build_ext_orig.build_extensions(self)
 
 
 
 setup(name='cgal',
       version=os.environ.get('CGAL_PYTHON_MODULE_VERSION') or '5.4.1',
       author="CGAL Project",
-      description="CGAL bindings, allowing to use some of the CGAL library in python.",
-      long_description="The CGAL Bindings project allows to use some packages of CGAL, the Computational Algorithms Library with python. This project is still experimental and more packages will be added. For more information, please visit https://github.com/CGAL/cgal-swig-bindings/wiki.",
+      description="CGAL bindings, allowing to use some of the CGAL library in Python.",
+      long_description="The CGAL Bindings project allows to use some packages of CGAL, the Computational Algorithms Library with Python. This project is still experimental and more packages will be added. For more information, please visit https://github.com/CGAL/cgal-swig-bindings/wiki.",
       long_description_content_type="text/markdown",
       packages=['CGAL'],
       package_dir = { 'CGAL': '.' },
       #package_dir = {'CGAL': 'build/build-python/CGAL'},
       url="https://github.com/CGAL/cgal-swig-bindings",
       python_requires='>=3.6',
       classifiers = [
```

