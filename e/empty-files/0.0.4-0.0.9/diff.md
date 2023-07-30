# Comparing `tmp/empty-files-0.0.4.tar.gz` & `tmp/empty-files-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empty-files-0.0.4.tar", last modified: Sun Jun 25 18:25:22 2023, max compression
+gzip compressed data, was "empty-files-0.0.9.tar", last modified: Sun Jul 30 19:40:41 2023, max compression
```

## Comparing `empty-files-0.0.4.tar` & `empty-files-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:25:22.122274 empty-files-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-06-25 18:25:08.000000 empty-files-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 18:25:08.000000 empty-files-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-25 18:25:22.122274 empty-files-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-25 18:25:08.000000 empty-files-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:25:22.122274 empty-files-0.0.4/empty_files/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-25 18:25:08.000000 empty-files-0.0.4/empty_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-25 18:25:08.000000 empty-files-0.0.4/empty_files/empty_files.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-25 18:25:08.000000 empty-files-0.0.4/empty_files/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:25:22.122274 empty-files-0.0.4/empty_files.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-25 18:25:22.000000 empty-files-0.0.4/empty_files.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-25 18:25:22.000000 empty-files-0.0.4/empty_files.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 18:25:22.000000 empty-files-0.0.4/empty_files.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-25 18:25:22.000000 empty-files-0.0.4/empty_files.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-25 18:25:22.000000 empty-files-0.0.4/empty_files.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-25 18:25:22.122274 empty-files-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-25 18:25:08.000000 empty-files-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:40:41.891014 empty-files-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-07-30 19:40:32.000000 empty-files-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 19:40:32.000000 empty-files-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-30 19:40:41.891014 empty-files-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-30 19:40:32.000000 empty-files-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:40:41.887014 empty-files-0.0.9/empty_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-30 19:40:32.000000 empty-files-0.0.9/empty_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-30 19:40:32.000000 empty-files-0.0.9/empty_files/empty_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-30 19:40:40.000000 empty-files-0.0.9/empty_files/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:40:41.891014 empty-files-0.0.9/empty_files.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-30 19:40:41.000000 empty-files-0.0.9/empty_files.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-30 19:40:41.000000 empty-files-0.0.9/empty_files.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 19:40:41.000000 empty-files-0.0.9/empty_files.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-30 19:40:41.000000 empty-files-0.0.9/empty_files.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-30 19:40:41.000000 empty-files-0.0.9/empty_files.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-30 19:40:41.891014 empty-files-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-30 19:40:32.000000 empty-files-0.0.9/setup.py
```

### Comparing `empty-files-0.0.4/LICENSE` & `empty-files-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `empty-files-0.0.4/PKG-INFO` & `empty-files-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: empty-files
-Version: 0.0.4
+Version: 0.0.9
 Summary: Serves empty files of many types
 Home-page: https://github.com/approvals/EmptyFiles.Python
 Author: empty_files Contributors
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: empty-files Version: 0.0.4 Summary: Serves empty
+Metadata-Version: 2.1 Name: empty-files Version: 0.0.9 Summary: Serves empty
 files of many types Home-page: https://github.com/approvals/EmptyFiles.Python
 Author: empty_files Contributors Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: POSIX Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: MacOS
 :: MacOS X Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
```

### Comparing `empty-files-0.0.4/README.md` & `empty-files-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `empty-files-0.0.4/empty_files/empty_files.py` & `empty-files-0.0.9/empty_files/empty_files.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from pathlib import Path
 
-import requests as requests
-
 
 def create_empty_file(file_path: str) -> None:
     path = Path(file_path)
     path.parent.mkdir(parents=True, exist_ok=True)
     extension = path.suffix
 
     try:
         download_file(f"https://github.com/VerifyTests/EmptyFiles/raw/main/index/empty{extension}", file_path)
     except:
         open(file_path, "w").close()
 
 
 def download_file(url: str, file_path: str) -> str:
+    import requests as requests # this is to catch the exception if your OpenSSL environment is not setup correctly
     with requests.get(url, stream=True) as response:
         response.raise_for_status()
         with open(file_path, 'wb') as file:
             for chunk in response.iter_content(chunk_size=8192):
                 file.write(chunk)
     return file_path
```

### Comparing `empty-files-0.0.4/empty_files.egg-info/PKG-INFO` & `empty-files-0.0.9/empty_files.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: empty-files
-Version: 0.0.4
+Version: 0.0.9
 Summary: Serves empty files of many types
 Home-page: https://github.com/approvals/EmptyFiles.Python
 Author: empty_files Contributors
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: empty-files Version: 0.0.4 Summary: Serves empty
+Metadata-Version: 2.1 Name: empty-files Version: 0.0.9 Summary: Serves empty
 files of many types Home-page: https://github.com/approvals/EmptyFiles.Python
 Author: empty_files Contributors Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: POSIX Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: MacOS
 :: MacOS X Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
```

### Comparing `empty-files-0.0.4/setup.py` & `empty-files-0.0.9/setup.py`

 * *Files identical despite different names*

