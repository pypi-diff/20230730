# Comparing `tmp/pyyt-cli-0.2.1.tar.gz` & `tmp/pyyt-cli-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyyt-cli-0.2.1.tar", last modified: Sun Jul 30 11:48:01 2023, max compression
+gzip compressed data, was "pyyt-cli-0.2.2.tar", last modified: Sun Jul 30 12:12:52 2023, max compression
```

## Comparing `pyyt-cli-0.2.1.tar` & `pyyt-cli-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-30 11:48:01.555633 pyyt-cli-0.2.1/
--rw-r--r--   0 dvitto     (501) staff       (20)     1211 2021-01-23 14:08:38.000000 pyyt-cli-0.2.1/LICENSE
--rw-r--r--   0 dvitto     (501) staff       (20)     1530 2023-07-30 11:48:01.555825 pyyt-cli-0.2.1/PKG-INFO
--rw-r--r--   0 dvitto     (501) staff       (20)      886 2023-07-26 19:04:39.000000 pyyt-cli-0.2.1/README.md
--rw-r--r--   0 dvitto     (501) staff       (20)       85 2023-07-26 18:56:01.000000 pyyt-cli-0.2.1/pyproject.toml
-drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-30 11:48:01.553455 pyyt-cli-0.2.1/pyyt_cli.egg-info/
--rw-r--r--   0 dvitto     (501) staff       (20)     1530 2023-07-30 11:48:01.000000 pyyt-cli-0.2.1/pyyt_cli.egg-info/PKG-INFO
--rw-r--r--   0 dvitto     (501) staff       (20)      320 2023-07-30 11:48:01.000000 pyyt-cli-0.2.1/pyyt_cli.egg-info/SOURCES.txt
--rw-r--r--   0 dvitto     (501) staff       (20)        1 2023-07-30 11:48:01.000000 pyyt-cli-0.2.1/pyyt_cli.egg-info/dependency_links.txt
--rw-r--r--   0 dvitto     (501) staff       (20)       39 2023-07-30 11:48:01.000000 pyyt-cli-0.2.1/pyyt_cli.egg-info/entry_points.txt
--rw-r--r--   0 dvitto     (501) staff       (20)       83 2023-07-30 11:48:01.000000 pyyt-cli-0.2.1/pyyt_cli.egg-info/requires.txt
--rw-r--r--   0 dvitto     (501) staff       (20)        4 2023-07-30 11:48:01.000000 pyyt-cli-0.2.1/pyyt_cli.egg-info/top_level.txt
--rw-r--r--   0 dvitto     (501) staff       (20)       67 2023-07-30 11:48:01.556378 pyyt-cli-0.2.1/setup.cfg
--rw-r--r--   0 dvitto     (501) staff       (20)     1769 2023-07-30 11:47:27.000000 pyyt-cli-0.2.1/setup.py
-drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-30 11:48:01.554901 pyyt-cli-0.2.1/src/
--rw-r--r--   0 dvitto     (501) staff       (20)        0 2023-07-26 18:56:01.000000 pyyt-cli-0.2.1/src/__init__.py
--rw-r--r--   0 dvitto     (501) staff       (20)      360 2023-07-26 18:56:01.000000 pyyt-cli-0.2.1/src/options.py
--rw-r--r--   0 dvitto     (501) staff       (20)     1264 2023-07-30 11:25:42.000000 pyyt-cli-0.2.1/src/pyyt.py
--rw-r--r--   0 dvitto     (501) staff       (20)     2765 2023-07-30 11:46:39.000000 pyyt-cli-0.2.1/src/utils.py
-drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-30 11:48:01.555292 pyyt-cli-0.2.1/tests/
--rw-r--r--   0 dvitto     (501) staff       (20)     2289 2023-07-26 18:56:01.000000 pyyt-cli-0.2.1/tests/test_pyyt.py
+drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-30 12:12:52.457658 pyyt-cli-0.2.2/
+-rw-r--r--   0 dvitto     (501) staff       (20)     1211 2021-01-23 14:08:38.000000 pyyt-cli-0.2.2/LICENSE
+-rw-r--r--   0 dvitto     (501) staff       (20)     1530 2023-07-30 12:12:52.457841 pyyt-cli-0.2.2/PKG-INFO
+-rw-r--r--   0 dvitto     (501) staff       (20)      886 2023-07-26 19:04:39.000000 pyyt-cli-0.2.2/README.md
+-rw-r--r--   0 dvitto     (501) staff       (20)       85 2023-07-26 18:56:01.000000 pyyt-cli-0.2.2/pyproject.toml
+drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-30 12:12:52.455265 pyyt-cli-0.2.2/pyyt_cli.egg-info/
+-rw-r--r--   0 dvitto     (501) staff       (20)     1530 2023-07-30 12:12:52.000000 pyyt-cli-0.2.2/pyyt_cli.egg-info/PKG-INFO
+-rw-r--r--   0 dvitto     (501) staff       (20)      320 2023-07-30 12:12:52.000000 pyyt-cli-0.2.2/pyyt_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 dvitto     (501) staff       (20)        1 2023-07-30 12:12:52.000000 pyyt-cli-0.2.2/pyyt_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 dvitto     (501) staff       (20)       39 2023-07-30 12:12:52.000000 pyyt-cli-0.2.2/pyyt_cli.egg-info/entry_points.txt
+-rw-r--r--   0 dvitto     (501) staff       (20)       83 2023-07-30 12:12:52.000000 pyyt-cli-0.2.2/pyyt_cli.egg-info/requires.txt
+-rw-r--r--   0 dvitto     (501) staff       (20)        4 2023-07-30 12:12:52.000000 pyyt-cli-0.2.2/pyyt_cli.egg-info/top_level.txt
+-rw-r--r--   0 dvitto     (501) staff       (20)       67 2023-07-30 12:12:52.458442 pyyt-cli-0.2.2/setup.cfg
+-rw-r--r--   0 dvitto     (501) staff       (20)     1769 2023-07-30 12:12:16.000000 pyyt-cli-0.2.2/setup.py
+drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-30 12:12:52.456880 pyyt-cli-0.2.2/src/
+-rw-r--r--   0 dvitto     (501) staff       (20)        0 2023-07-26 18:56:01.000000 pyyt-cli-0.2.2/src/__init__.py
+-rw-r--r--   0 dvitto     (501) staff       (20)      360 2023-07-26 18:56:01.000000 pyyt-cli-0.2.2/src/options.py
+-rw-r--r--   0 dvitto     (501) staff       (20)     1264 2023-07-30 11:25:42.000000 pyyt-cli-0.2.2/src/pyyt.py
+-rw-r--r--   0 dvitto     (501) staff       (20)     2765 2023-07-30 11:46:39.000000 pyyt-cli-0.2.2/src/utils.py
+drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-30 12:12:52.457198 pyyt-cli-0.2.2/tests/
+-rw-r--r--   0 dvitto     (501) staff       (20)     2289 2023-07-26 18:56:01.000000 pyyt-cli-0.2.2/tests/test_pyyt.py
```

### Comparing `pyyt-cli-0.2.1/LICENSE` & `pyyt-cli-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyyt-cli-0.2.1/PKG-INFO` & `pyyt-cli-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyyt-cli
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python script to download videos as audio from a given YouTube playlist/video
 Home-page: https://github.com/patillacode/pyyt
 Author: Patilla Code
 Author-email: patillacode@gmail.com
 License: Apache 2.0
 Keywords: converter,audio,youtube,download,mp3
 Classifier: Intended Audience :: Developers
```

### Comparing `pyyt-cli-0.2.1/README.md` & `pyyt-cli-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pyyt-cli-0.2.1/pyyt_cli.egg-info/PKG-INFO` & `pyyt-cli-0.2.2/pyyt_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyyt-cli
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python script to download videos as audio from a given YouTube playlist/video
 Home-page: https://github.com/patillacode/pyyt
 Author: Patilla Code
 Author-email: patillacode@gmail.com
 License: Apache 2.0
 Keywords: converter,audio,youtube,download,mp3
 Classifier: Intended Audience :: Developers
```

### Comparing `pyyt-cli-0.2.1/setup.py` & `pyyt-cli-0.2.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         """Run all tests!"""
         errno = call(["py.test", "--cov=pyyt", "--cov-report=term-missing"])
         raise SystemExit(errno)
 
 
 setup(
     name="pyyt-cli",
-    version="0.2.1",
+    version="0.2.2",
     description=(
         "Python script to download videos as audio from a given YouTube playlist/video"
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/patillacode/pyyt",
     author="Patilla Code",
```

### Comparing `pyyt-cli-0.2.1/src/pyyt.py` & `pyyt-cli-0.2.2/src/pyyt.py`

 * *Files identical despite different names*

### Comparing `pyyt-cli-0.2.1/src/utils.py` & `pyyt-cli-0.2.2/src/utils.py`

 * *Files identical despite different names*

### Comparing `pyyt-cli-0.2.1/tests/test_pyyt.py` & `pyyt-cli-0.2.2/tests/test_pyyt.py`

 * *Files identical despite different names*

