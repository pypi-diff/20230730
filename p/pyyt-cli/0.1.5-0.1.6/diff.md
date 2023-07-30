# Comparing `tmp/pyyt-cli-0.1.5.tar.gz` & `tmp/pyyt-cli-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyyt-cli-0.1.5.tar", last modified: Wed Jul 26 18:51:33 2023, max compression
+gzip compressed data, was "pyyt-cli-0.1.6.tar", last modified: Sun Jul 30 11:27:34 2023, max compression
```

## Comparing `pyyt-cli-0.1.5.tar` & `pyyt-cli-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-26 18:51:33.425730 pyyt-cli-0.1.5/
--rw-r--r--   0 dvitto     (501) staff       (20)     1211 2021-01-23 14:08:38.000000 pyyt-cli-0.1.5/LICENSE
--rw-r--r--   0 dvitto     (501) staff       (20)     1444 2023-07-26 18:51:33.425842 pyyt-cli-0.1.5/PKG-INFO
--rw-r--r--   0 dvitto     (501) staff       (20)      800 2023-07-26 17:46:23.000000 pyyt-cli-0.1.5/README.md
--rw-r--r--   0 dvitto     (501) staff       (20)       85 2023-07-26 17:53:17.000000 pyyt-cli-0.1.5/pyproject.toml
-drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-26 18:51:33.423839 pyyt-cli-0.1.5/pyyt_cli.egg-info/
--rw-r--r--   0 dvitto     (501) staff       (20)     1444 2023-07-26 18:51:33.000000 pyyt-cli-0.1.5/pyyt_cli.egg-info/PKG-INFO
--rw-r--r--   0 dvitto     (501) staff       (20)      320 2023-07-26 18:51:33.000000 pyyt-cli-0.1.5/pyyt_cli.egg-info/SOURCES.txt
--rw-r--r--   0 dvitto     (501) staff       (20)        1 2023-07-26 18:51:33.000000 pyyt-cli-0.1.5/pyyt_cli.egg-info/dependency_links.txt
--rw-r--r--   0 dvitto     (501) staff       (20)       39 2023-07-26 18:51:33.000000 pyyt-cli-0.1.5/pyyt_cli.egg-info/entry_points.txt
--rw-r--r--   0 dvitto     (501) staff       (20)       83 2023-07-26 18:51:33.000000 pyyt-cli-0.1.5/pyyt_cli.egg-info/requires.txt
--rw-r--r--   0 dvitto     (501) staff       (20)        4 2023-07-26 18:51:33.000000 pyyt-cli-0.1.5/pyyt_cli.egg-info/top_level.txt
--rw-r--r--   0 dvitto     (501) staff       (20)       67 2023-07-26 18:51:33.426217 pyyt-cli-0.1.5/setup.cfg
--rw-r--r--   0 dvitto     (501) staff       (20)     1769 2023-07-26 18:51:25.000000 pyyt-cli-0.1.5/setup.py
-drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-26 18:51:33.425010 pyyt-cli-0.1.5/src/
--rw-r--r--   0 dvitto     (501) staff       (20)        0 2023-07-26 16:02:06.000000 pyyt-cli-0.1.5/src/__init__.py
--rw-r--r--   0 dvitto     (501) staff       (20)      360 2023-07-26 15:44:13.000000 pyyt-cli-0.1.5/src/options.py
--rw-r--r--   0 dvitto     (501) staff       (20)     1302 2023-07-26 18:19:26.000000 pyyt-cli-0.1.5/src/pyyt.py
--rw-r--r--   0 dvitto     (501) staff       (20)     2730 2023-07-26 18:21:52.000000 pyyt-cli-0.1.5/src/utils.py
-drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-26 18:51:33.425356 pyyt-cli-0.1.5/tests/
--rw-r--r--   0 dvitto     (501) staff       (20)     2289 2023-07-26 16:45:33.000000 pyyt-cli-0.1.5/tests/test_pyyt.py
+drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-30 11:27:34.299460 pyyt-cli-0.1.6/
+-rw-r--r--   0 dvitto     (501) staff       (20)     1211 2021-01-23 14:08:38.000000 pyyt-cli-0.1.6/LICENSE
+-rw-r--r--   0 dvitto     (501) staff       (20)     1530 2023-07-30 11:27:34.299739 pyyt-cli-0.1.6/PKG-INFO
+-rw-r--r--   0 dvitto     (501) staff       (20)      886 2023-07-26 19:04:39.000000 pyyt-cli-0.1.6/README.md
+-rw-r--r--   0 dvitto     (501) staff       (20)       85 2023-07-26 18:56:01.000000 pyyt-cli-0.1.6/pyproject.toml
+drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-30 11:27:34.293736 pyyt-cli-0.1.6/pyyt_cli.egg-info/
+-rw-r--r--   0 dvitto     (501) staff       (20)     1530 2023-07-30 11:27:34.000000 pyyt-cli-0.1.6/pyyt_cli.egg-info/PKG-INFO
+-rw-r--r--   0 dvitto     (501) staff       (20)      320 2023-07-30 11:27:34.000000 pyyt-cli-0.1.6/pyyt_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 dvitto     (501) staff       (20)        1 2023-07-30 11:27:34.000000 pyyt-cli-0.1.6/pyyt_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 dvitto     (501) staff       (20)       39 2023-07-30 11:27:34.000000 pyyt-cli-0.1.6/pyyt_cli.egg-info/entry_points.txt
+-rw-r--r--   0 dvitto     (501) staff       (20)       83 2023-07-30 11:27:34.000000 pyyt-cli-0.1.6/pyyt_cli.egg-info/requires.txt
+-rw-r--r--   0 dvitto     (501) staff       (20)        4 2023-07-30 11:27:34.000000 pyyt-cli-0.1.6/pyyt_cli.egg-info/top_level.txt
+-rw-r--r--   0 dvitto     (501) staff       (20)       67 2023-07-30 11:27:34.300411 pyyt-cli-0.1.6/setup.cfg
+-rw-r--r--   0 dvitto     (501) staff       (20)     1769 2023-07-30 11:26:45.000000 pyyt-cli-0.1.6/setup.py
+drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-30 11:27:34.297864 pyyt-cli-0.1.6/src/
+-rw-r--r--   0 dvitto     (501) staff       (20)        0 2023-07-26 18:56:01.000000 pyyt-cli-0.1.6/src/__init__.py
+-rw-r--r--   0 dvitto     (501) staff       (20)      360 2023-07-26 18:56:01.000000 pyyt-cli-0.1.6/src/options.py
+-rw-r--r--   0 dvitto     (501) staff       (20)     1264 2023-07-30 11:25:42.000000 pyyt-cli-0.1.6/src/pyyt.py
+-rw-r--r--   0 dvitto     (501) staff       (20)     2732 2023-07-30 11:25:09.000000 pyyt-cli-0.1.6/src/utils.py
+drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-30 11:27:34.298339 pyyt-cli-0.1.6/tests/
+-rw-r--r--   0 dvitto     (501) staff       (20)     2289 2023-07-26 18:56:01.000000 pyyt-cli-0.1.6/tests/test_pyyt.py
```

### Comparing `pyyt-cli-0.1.5/LICENSE` & `pyyt-cli-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyyt-cli-0.1.5/PKG-INFO` & `pyyt-cli-0.1.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyyt-cli
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python script to download videos as audio from a given YouTube playlist/video
 Home-page: https://github.com/patillacode/pyyt
 Author: Patilla Code
 Author-email: patillacode@gmail.com
 License: Apache 2.0
 Keywords: converter,audio,youtube,download,mp3
 Classifier: Intended Audience :: Developers
@@ -13,14 +13,16 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
+[![Downloads](https://pepy.tech/badge/pyyt-cli)](https://pepy.tech/project/pyyt-cli)
+
 # pyyt
 Python interactive script to download videos as audio from a given YouTube playlist or a single video url
 
 -------------------
 ### Attribution ###
 
 An abstraction of [yt-dlp](https://github.com/yt-dlp/yt-dlp) for my specific use case.
```

### Comparing `pyyt-cli-0.1.5/README.md` & `pyyt-cli-0.1.6/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+[![Downloads](https://pepy.tech/badge/pyyt-cli)](https://pepy.tech/project/pyyt-cli)
+
 # pyyt
 Python interactive script to download videos as audio from a given YouTube playlist or a single video url
 
 -------------------
 ### Attribution ###
 
 An abstraction of [yt-dlp](https://github.com/yt-dlp/yt-dlp) for my specific use case.
```

### Comparing `pyyt-cli-0.1.5/pyyt_cli.egg-info/PKG-INFO` & `pyyt-cli-0.1.6/pyyt_cli.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyyt-cli
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python script to download videos as audio from a given YouTube playlist/video
 Home-page: https://github.com/patillacode/pyyt
 Author: Patilla Code
 Author-email: patillacode@gmail.com
 License: Apache 2.0
 Keywords: converter,audio,youtube,download,mp3
 Classifier: Intended Audience :: Developers
@@ -13,14 +13,16 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
+[![Downloads](https://pepy.tech/badge/pyyt-cli)](https://pepy.tech/project/pyyt-cli)
+
 # pyyt
 Python interactive script to download videos as audio from a given YouTube playlist or a single video url
 
 -------------------
 ### Attribution ###
 
 An abstraction of [yt-dlp](https://github.com/yt-dlp/yt-dlp) for my specific use case.
```

### Comparing `pyyt-cli-0.1.5/setup.py` & `pyyt-cli-0.1.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         """Run all tests!"""
         errno = call(["py.test", "--cov=pyyt", "--cov-report=term-missing"])
         raise SystemExit(errno)
 
 
 setup(
     name="pyyt-cli",
-    version="0.1.5",
+    version="0.1.6",
     description=(
         "Python script to download videos as audio from a given YouTube playlist/video"
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/patillacode/pyyt",
     author="Patilla Code",
```

### Comparing `pyyt-cli-0.1.5/src/pyyt.py` & `pyyt-cli-0.1.6/src/pyyt.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,20 +23,19 @@
         playlist_url = input(
             colored("Please insert the YouTube playlist URL: ", "magenta")
         )
         video_entries = get_video_entries(playlist_url)
         video_list = [
             f'https://www.youtube.com/watch?v={video["id"]}' for video in video_entries
         ]
-        for video_url in video_list:
-            download_and_metadata(video_url)
+        download_and_metadata(video_list)
 
     elif selected_option == 1:
         video_url = input(colored("Please insert the YouTube video URL: ", "magenta"))
-        download_and_metadata(video_url)
+        download_and_metadata([video_url])
 
     else:
         print(colored("Wrong option. Cya!", "magenta"))
 
 
 if __name__ == "__main__":
     welcome()
```

### Comparing `pyyt-cli-0.1.5/src/utils.py` & `pyyt-cli-0.1.6/src/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -58,26 +58,26 @@
         entries = results["entries"]
         return entries
 
     print("Something went wrong, no entries in playlist...")
     sys.exit(2)
 
 
-def download_and_metadata(video_url: str) -> None:
+def download_and_metadata(video_urls: list) -> None:
     """
     Download a video as audio and handle metadata.
 
     Args:
-        video_url (str): The URL of the YouTube video.
+        video_url (list): The URL of the YouTube video.
     """
     # TODO add metadata handling
     ydl_opts["outtmpl"] = f"{get_download_folder()}/%(title)s.%(ext)s"
     ydl = yt_dlp.YoutubeDL(ydl_opts)
 
-    ydl.download([video_url])
+    ydl.download(video_urls)
 
 
 def welcome() -> None:
     """
     Display a welcome message and banner.
     """
     os.system("clear")
```

### Comparing `pyyt-cli-0.1.5/tests/test_pyyt.py` & `pyyt-cli-0.1.6/tests/test_pyyt.py`

 * *Files identical despite different names*

