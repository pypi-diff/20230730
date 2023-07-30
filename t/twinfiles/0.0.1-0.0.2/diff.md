# Comparing `tmp/twinfiles-0.0.1.tar.gz` & `tmp/twinfiles-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twinfiles-0.0.1.tar", last modified: Sun Jul 30 15:00:57 2023, max compression
+gzip compressed data, was "twinfiles-0.0.2.tar", last modified: Sun Jul 30 17:09:24 2023, max compression
```

## Comparing `twinfiles-0.0.1.tar` & `twinfiles-0.0.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:00:57.254796 twinfiles-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-30 15:00:49.000000 twinfiles-0.0.1/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:00:57.246796 twinfiles-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:00:57.250796 twinfiles-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-30 15:00:49.000000 twinfiles-0.0.1/.github/workflows/multi-test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-30 15:00:49.000000 twinfiles-0.0.1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-30 15:00:49.000000 twinfiles-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-30 15:00:49.000000 twinfiles-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-30 15:00:49.000000 twinfiles-0.0.1/.python-version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:00:57.250796 twinfiles-0.0.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-30 15:00:49.000000 twinfiles-0.0.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-30 15:00:49.000000 twinfiles-0.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-30 15:00:49.000000 twinfiles-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-30 15:00:49.000000 twinfiles-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-30 15:00:57.254796 twinfiles-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-30 15:00:49.000000 twinfiles-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:00:57.250796 twinfiles-0.0.1/imgs/
--rw-r--r--   0 runner    (1001) docker     (123)    30290 2023-07-30 15:00:49.000000 twinfiles-0.0.1/imgs/use.png
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-30 15:00:49.000000 twinfiles-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-30 15:00:49.000000 twinfiles-0.0.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-30 15:00:49.000000 twinfiles-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-30 15:00:49.000000 twinfiles-0.0.1/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-30 15:00:57.254796 twinfiles-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-30 15:00:49.000000 twinfiles-0.0.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-30 15:00:49.000000 twinfiles-0.0.1/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:00:57.254796 twinfiles-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-30 15:00:49.000000 twinfiles-0.0.1/tests/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:00:57.254796 twinfiles-0.0.1/twinfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-30 15:00:49.000000 twinfiles-0.0.1/twinfiles/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-30 15:00:49.000000 twinfiles-0.0.1/twinfiles/finder.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-30 15:00:57.000000 twinfiles-0.0.1/twinfiles/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:00:57.254796 twinfiles-0.0.1/twinfiles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-30 15:00:57.000000 twinfiles-0.0.1/twinfiles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-30 15:00:57.000000 twinfiles-0.0.1/twinfiles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 15:00:57.000000 twinfiles-0.0.1/twinfiles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-30 15:00:57.000000 twinfiles-0.0.1/twinfiles.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-30 15:00:57.000000 twinfiles-0.0.1/twinfiles.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-30 15:00:57.000000 twinfiles-0.0.1/twinfiles.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:09:24.816640 twinfiles-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-30 17:09:16.000000 twinfiles-0.0.2/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:09:24.812640 twinfiles-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:09:24.816640 twinfiles-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-30 17:09:16.000000 twinfiles-0.0.2/.github/workflows/multi-test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-30 17:09:16.000000 twinfiles-0.0.2/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-30 17:09:16.000000 twinfiles-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-30 17:09:16.000000 twinfiles-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-30 17:09:16.000000 twinfiles-0.0.2/.python-version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:09:24.816640 twinfiles-0.0.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-30 17:09:16.000000 twinfiles-0.0.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-30 17:09:16.000000 twinfiles-0.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-30 17:09:16.000000 twinfiles-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-30 17:09:16.000000 twinfiles-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-30 17:09:24.816640 twinfiles-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-30 17:09:16.000000 twinfiles-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:09:24.816640 twinfiles-0.0.2/imgs/
+-rw-r--r--   0 runner    (1001) docker     (123)    30290 2023-07-30 17:09:16.000000 twinfiles-0.0.2/imgs/use.png
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-30 17:09:16.000000 twinfiles-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-30 17:09:16.000000 twinfiles-0.0.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-30 17:09:16.000000 twinfiles-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-30 17:09:16.000000 twinfiles-0.0.2/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-30 17:09:24.820640 twinfiles-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-30 17:09:16.000000 twinfiles-0.0.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-30 17:09:16.000000 twinfiles-0.0.2/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:09:24.816640 twinfiles-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-30 17:09:16.000000 twinfiles-0.0.2/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:09:24.816640 twinfiles-0.0.2/twinfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-30 17:09:16.000000 twinfiles-0.0.2/twinfiles/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-07-30 17:09:16.000000 twinfiles-0.0.2/twinfiles/finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-30 17:09:24.000000 twinfiles-0.0.2/twinfiles/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:09:24.816640 twinfiles-0.0.2/twinfiles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-30 17:09:24.000000 twinfiles-0.0.2/twinfiles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-30 17:09:24.000000 twinfiles-0.0.2/twinfiles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 17:09:24.000000 twinfiles-0.0.2/twinfiles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-30 17:09:24.000000 twinfiles-0.0.2/twinfiles.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-30 17:09:24.000000 twinfiles-0.0.2/twinfiles.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-30 17:09:24.000000 twinfiles-0.0.2/twinfiles.egg-info/top_level.txt
```

### Comparing `twinfiles-0.0.1/.cruft.json` & `twinfiles-0.0.2/.cruft.json`

 * *Files identical despite different names*

### Comparing `twinfiles-0.0.1/.github/workflows/multi-test.yaml` & `twinfiles-0.0.2/.github/workflows/multi-test.yaml`

 * *Files identical despite different names*

### Comparing `twinfiles-0.0.1/.github/workflows/release.yaml` & `twinfiles-0.0.2/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `twinfiles-0.0.1/.gitignore` & `twinfiles-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `twinfiles-0.0.1/.pre-commit-config.yaml` & `twinfiles-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `twinfiles-0.0.1/LICENSE` & `twinfiles-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `twinfiles-0.0.1/PKG-INFO` & `twinfiles-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twinfiles
-Version: 0.0.1
+Version: 0.0.2
 Summary: Command line tool to find and remove duplicate files
 Home-page: https://github.com/joaompinto/twinfiles
 Author: João Pinto
 Author-email: lamego.pinto@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -13,15 +13,20 @@
 
 Command line tool to find and remove duplicate files
 
 ![License: MIT](https://img.shields.io/github/license/joaompinto/twinfiles?style=for-the-badge&color=%23007ec6)
 [![PyPi](https://img.shields.io/pypi/v/twinfiles.svg?style=for-the-badge&color=%23007ec6)](https://pypi.python.org/pypi/twinfiles)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge)](https://github.com/ambv/black)
 
-<img src="imgs/use.png">
+
+<div align="center">
+
+<img src="https://raw.githubusercontent.com/joaompinto/twinfiles/master/imgs/use.png" alt="twinfiles in action" width="100%"/>
+
+</div>
 
 ## Motivation
 
 Over the years I have accumulated multiple backups of photos leading to a lot of duplicates. I need an easy way to clean my photos.
 
 ## Installation
```

### Comparing `twinfiles-0.0.1/README.md` & `twinfiles-0.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,20 @@
 
 Command line tool to find and remove duplicate files
 
 ![License: MIT](https://img.shields.io/github/license/joaompinto/twinfiles?style=for-the-badge&color=%23007ec6)
 [![PyPi](https://img.shields.io/pypi/v/twinfiles.svg?style=for-the-badge&color=%23007ec6)](https://pypi.python.org/pypi/twinfiles)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge)](https://github.com/ambv/black)
 
-<img src="imgs/use.png">
+
+<div align="center">
+
+<img src="https://raw.githubusercontent.com/joaompinto/twinfiles/master/imgs/use.png" alt="twinfiles in action" width="100%"/>
+
+</div>
 
 ## Motivation
 
 Over the years I have accumulated multiple backups of photos leading to a lot of duplicates. I need an easy way to clean my photos.
 
 ## Installation
```

### Comparing `twinfiles-0.0.1/imgs/use.png` & `twinfiles-0.0.2/imgs/use.png`

 * *Files identical despite different names*

### Comparing `twinfiles-0.0.1/setup.py` & `twinfiles-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `twinfiles-0.0.1/tasks.py` & `twinfiles-0.0.2/tasks.py`

 * *Files identical despite different names*

### Comparing `twinfiles-0.0.1/twinfiles/finder.py` & `twinfiles-0.0.2/twinfiles/finder.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,14 +90,20 @@
         for _, filenames in self.same_content.items():
             sorted_filenames = sorted(filenames)
             delete = sorted_filenames[1:]
             for filename in delete:
                 os.remove(filename)
         print("Done")
 
+    def list(self):
+        print("Listing duplicated files...")
+        for _, filenames in self.same_content.items():
+            sorted_filenames = sorted(filenames)
+            print(" ".join(sorted_filenames))
+
     @staticmethod
     def calculate_md5sum(file_path):
         md5_hash = hashlib.md5()
 
         with open(file_path, "rb") as file:
             # Read the file in small chunks to avoid memory issues with large files
             for chunk in iter(lambda: file.read(4096), b""):
```

### Comparing `twinfiles-0.0.1/twinfiles.egg-info/PKG-INFO` & `twinfiles-0.0.2/twinfiles.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twinfiles
-Version: 0.0.1
+Version: 0.0.2
 Summary: Command line tool to find and remove duplicate files
 Home-page: https://github.com/joaompinto/twinfiles
 Author: João Pinto
 Author-email: lamego.pinto@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -13,15 +13,20 @@
 
 Command line tool to find and remove duplicate files
 
 ![License: MIT](https://img.shields.io/github/license/joaompinto/twinfiles?style=for-the-badge&color=%23007ec6)
 [![PyPi](https://img.shields.io/pypi/v/twinfiles.svg?style=for-the-badge&color=%23007ec6)](https://pypi.python.org/pypi/twinfiles)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge)](https://github.com/ambv/black)
 
-<img src="imgs/use.png">
+
+<div align="center">
+
+<img src="https://raw.githubusercontent.com/joaompinto/twinfiles/master/imgs/use.png" alt="twinfiles in action" width="100%"/>
+
+</div>
 
 ## Motivation
 
 Over the years I have accumulated multiple backups of photos leading to a lot of duplicates. I need an easy way to clean my photos.
 
 ## Installation
```

### Comparing `twinfiles-0.0.1/twinfiles.egg-info/SOURCES.txt` & `twinfiles-0.0.2/twinfiles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

