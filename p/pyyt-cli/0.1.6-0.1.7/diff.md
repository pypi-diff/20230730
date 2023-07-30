# Comparing `tmp/pyyt-cli-0.1.6.tar.gz` & `tmp/pyyt-cli-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyyt-cli-0.1.6.tar", last modified: Sun Jul 30 11:27:34 2023, max compression
+gzip compressed data, was "pyyt-cli-0.1.7.tar", last modified: Sun Jul 30 11:37:43 2023, max compression
```

## Comparing `pyyt-cli-0.1.6.tar` & `pyyt-cli-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-30 11:27:34.299460 pyyt-cli-0.1.6/
--rw-r--r--   0 dvitto     (501) staff       (20)     1211 2021-01-23 14:08:38.000000 pyyt-cli-0.1.6/LICENSE
--rw-r--r--   0 dvitto     (501) staff       (20)     1530 2023-07-30 11:27:34.299739 pyyt-cli-0.1.6/PKG-INFO
--rw-r--r--   0 dvitto     (501) staff       (20)      886 2023-07-26 19:04:39.000000 pyyt-cli-0.1.6/README.md
--rw-r--r--   0 dvitto     (501) staff       (20)       85 2023-07-26 18:56:01.000000 pyyt-cli-0.1.6/pyproject.toml
-drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-30 11:27:34.293736 pyyt-cli-0.1.6/pyyt_cli.egg-info/
--rw-r--r--   0 dvitto     (501) staff       (20)     1530 2023-07-30 11:27:34.000000 pyyt-cli-0.1.6/pyyt_cli.egg-info/PKG-INFO
--rw-r--r--   0 dvitto     (501) staff       (20)      320 2023-07-30 11:27:34.000000 pyyt-cli-0.1.6/pyyt_cli.egg-info/SOURCES.txt
--rw-r--r--   0 dvitto     (501) staff       (20)        1 2023-07-30 11:27:34.000000 pyyt-cli-0.1.6/pyyt_cli.egg-info/dependency_links.txt
--rw-r--r--   0 dvitto     (501) staff       (20)       39 2023-07-30 11:27:34.000000 pyyt-cli-0.1.6/pyyt_cli.egg-info/entry_points.txt
--rw-r--r--   0 dvitto     (501) staff       (20)       83 2023-07-30 11:27:34.000000 pyyt-cli-0.1.6/pyyt_cli.egg-info/requires.txt
--rw-r--r--   0 dvitto     (501) staff       (20)        4 2023-07-30 11:27:34.000000 pyyt-cli-0.1.6/pyyt_cli.egg-info/top_level.txt
--rw-r--r--   0 dvitto     (501) staff       (20)       67 2023-07-30 11:27:34.300411 pyyt-cli-0.1.6/setup.cfg
--rw-r--r--   0 dvitto     (501) staff       (20)     1769 2023-07-30 11:26:45.000000 pyyt-cli-0.1.6/setup.py
-drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-30 11:27:34.297864 pyyt-cli-0.1.6/src/
--rw-r--r--   0 dvitto     (501) staff       (20)        0 2023-07-26 18:56:01.000000 pyyt-cli-0.1.6/src/__init__.py
--rw-r--r--   0 dvitto     (501) staff       (20)      360 2023-07-26 18:56:01.000000 pyyt-cli-0.1.6/src/options.py
--rw-r--r--   0 dvitto     (501) staff       (20)     1264 2023-07-30 11:25:42.000000 pyyt-cli-0.1.6/src/pyyt.py
--rw-r--r--   0 dvitto     (501) staff       (20)     2732 2023-07-30 11:25:09.000000 pyyt-cli-0.1.6/src/utils.py
-drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-30 11:27:34.298339 pyyt-cli-0.1.6/tests/
--rw-r--r--   0 dvitto     (501) staff       (20)     2289 2023-07-26 18:56:01.000000 pyyt-cli-0.1.6/tests/test_pyyt.py
+drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-30 11:37:43.215661 pyyt-cli-0.1.7/
+-rw-r--r--   0 dvitto     (501) staff       (20)     1211 2021-01-23 14:08:38.000000 pyyt-cli-0.1.7/LICENSE
+-rw-r--r--   0 dvitto     (501) staff       (20)     1530 2023-07-30 11:37:43.215941 pyyt-cli-0.1.7/PKG-INFO
+-rw-r--r--   0 dvitto     (501) staff       (20)      886 2023-07-26 19:04:39.000000 pyyt-cli-0.1.7/README.md
+-rw-r--r--   0 dvitto     (501) staff       (20)       85 2023-07-26 18:56:01.000000 pyyt-cli-0.1.7/pyproject.toml
+drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-30 11:37:43.213130 pyyt-cli-0.1.7/pyyt_cli.egg-info/
+-rw-r--r--   0 dvitto     (501) staff       (20)     1530 2023-07-30 11:37:43.000000 pyyt-cli-0.1.7/pyyt_cli.egg-info/PKG-INFO
+-rw-r--r--   0 dvitto     (501) staff       (20)      320 2023-07-30 11:37:43.000000 pyyt-cli-0.1.7/pyyt_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 dvitto     (501) staff       (20)        1 2023-07-30 11:37:43.000000 pyyt-cli-0.1.7/pyyt_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 dvitto     (501) staff       (20)       39 2023-07-30 11:37:43.000000 pyyt-cli-0.1.7/pyyt_cli.egg-info/entry_points.txt
+-rw-r--r--   0 dvitto     (501) staff       (20)       83 2023-07-30 11:37:43.000000 pyyt-cli-0.1.7/pyyt_cli.egg-info/requires.txt
+-rw-r--r--   0 dvitto     (501) staff       (20)        4 2023-07-30 11:37:43.000000 pyyt-cli-0.1.7/pyyt_cli.egg-info/top_level.txt
+-rw-r--r--   0 dvitto     (501) staff       (20)       67 2023-07-30 11:37:43.217275 pyyt-cli-0.1.7/setup.cfg
+-rw-r--r--   0 dvitto     (501) staff       (20)     1769 2023-07-30 11:36:27.000000 pyyt-cli-0.1.7/setup.py
+drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-30 11:37:43.214967 pyyt-cli-0.1.7/src/
+-rw-r--r--   0 dvitto     (501) staff       (20)        0 2023-07-26 18:56:01.000000 pyyt-cli-0.1.7/src/__init__.py
+-rw-r--r--   0 dvitto     (501) staff       (20)      360 2023-07-26 18:56:01.000000 pyyt-cli-0.1.7/src/options.py
+-rw-r--r--   0 dvitto     (501) staff       (20)     1264 2023-07-30 11:25:42.000000 pyyt-cli-0.1.7/src/pyyt.py
+-rw-r--r--   0 dvitto     (501) staff       (20)     2764 2023-07-30 11:35:09.000000 pyyt-cli-0.1.7/src/utils.py
+drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-30 11:37:43.215246 pyyt-cli-0.1.7/tests/
+-rw-r--r--   0 dvitto     (501) staff       (20)     2289 2023-07-26 18:56:01.000000 pyyt-cli-0.1.7/tests/test_pyyt.py
```

### Comparing `pyyt-cli-0.1.6/LICENSE` & `pyyt-cli-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyyt-cli-0.1.6/PKG-INFO` & `pyyt-cli-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyyt-cli
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python script to download videos as audio from a given YouTube playlist/video
 Home-page: https://github.com/patillacode/pyyt
 Author: Patilla Code
 Author-email: patillacode@gmail.com
 License: Apache 2.0
 Keywords: converter,audio,youtube,download,mp3
 Classifier: Intended Audience :: Developers
```

### Comparing `pyyt-cli-0.1.6/README.md` & `pyyt-cli-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pyyt-cli-0.1.6/pyyt_cli.egg-info/PKG-INFO` & `pyyt-cli-0.1.7/pyyt_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyyt-cli
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python script to download videos as audio from a given YouTube playlist/video
 Home-page: https://github.com/patillacode/pyyt
 Author: Patilla Code
 Author-email: patillacode@gmail.com
 License: Apache 2.0
 Keywords: converter,audio,youtube,download,mp3
 Classifier: Intended Audience :: Developers
```

### Comparing `pyyt-cli-0.1.6/setup.py` & `pyyt-cli-0.1.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         """Run all tests!"""
         errno = call(["py.test", "--cov=pyyt", "--cov-report=term-missing"])
         raise SystemExit(errno)
 
 
 setup(
     name="pyyt-cli",
-    version="0.1.6",
+    version="0.1.7",
     description=(
         "Python script to download videos as audio from a given YouTube playlist/video"
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/patillacode/pyyt",
     author="Patilla Code",
```

### Comparing `pyyt-cli-0.1.6/src/pyyt.py` & `pyyt-cli-0.1.7/src/pyyt.py`

 * *Files identical despite different names*

### Comparing `pyyt-cli-0.1.6/src/utils.py` & `pyyt-cli-0.1.7/src/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,21 +63,22 @@
 
 
 def download_and_metadata(video_urls: list) -> None:
     """
     Download a video as audio and handle metadata.
 
     Args:
-        video_url (list): The URL of the YouTube video.
+        video_url (list): The URLs of the YouTube videos.
     """
     # TODO add metadata handling
     ydl_opts["outtmpl"] = f"{get_download_folder()}/%(title)s.%(ext)s"
     ydl = yt_dlp.YoutubeDL(ydl_opts)
 
-    ydl.download(video_urls)
+    for video in video_urls:
+        ydl.download([video])
 
 
 def welcome() -> None:
     """
     Display a welcome message and banner.
     """
     os.system("clear")
```

### Comparing `pyyt-cli-0.1.6/tests/test_pyyt.py` & `pyyt-cli-0.1.7/tests/test_pyyt.py`

 * *Files identical despite different names*

