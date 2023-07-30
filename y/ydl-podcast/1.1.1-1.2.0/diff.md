# Comparing `tmp/ydl_podcast-1.1.1.tar.gz` & `tmp/ydl_podcast-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ydl_podcast-1.1.1.tar", max compression
+gzip compressed data, was "ydl_podcast-1.2.0.tar", max compression
```

## Comparing `ydl_podcast-1.1.1.tar` & `ydl_podcast-1.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1102 2023-07-30 02:46:39.227326 ydl_podcast-1.1.1/LICENSE
--rw-r--r--   0        0        0     3100 2023-07-30 02:46:39.227326 ydl_podcast-1.1.1/README.md
--rw-r--r--   0        0        0      897 2023-07-30 02:55:26.080592 ydl_podcast-1.1.1/pyproject.toml
--rw-r--r--   0        0        0    14341 2023-07-30 02:54:28.083609 ydl_podcast-1.1.1/ydl_podcast/__init__.py
--rwxr-xr-x   0        0        0     1872 2023-07-30 02:46:39.227326 ydl_podcast-1.1.1/ydl_podcast/__main__.py
--rw-r--r--   0        0        0     1482 2023-07-30 02:46:39.227326 ydl_podcast-1.1.1/ydl_podcast/template.py
--rw-r--r--   0        0        0     4190 1970-01-01 00:00:00.000000 ydl_podcast-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-07-30 02:46:39.227326 ydl_podcast-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3100 2023-07-30 02:46:39.227326 ydl_podcast-1.2.0/README.md
+-rw-r--r--   0        0        0      915 2023-07-30 18:09:37.140643 ydl_podcast-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    15033 2023-07-30 18:09:37.140643 ydl_podcast-1.2.0/ydl_podcast/__init__.py
+-rwxr-xr-x   0        0        0     1872 2023-07-30 02:46:39.227326 ydl_podcast-1.2.0/ydl_podcast/__main__.py
+-rw-r--r--   0        0        0     1482 2023-07-30 02:46:39.227326 ydl_podcast-1.2.0/ydl_podcast/template.py
+-rw-r--r--   0        0        0     4223 1970-01-01 00:00:00.000000 ydl_podcast-1.2.0/PKG-INFO
```

### Comparing `ydl_podcast-1.1.1/LICENSE` & `ydl_podcast-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.1.1/README.md` & `ydl_podcast-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.1.1/pyproject.toml` & `ydl_podcast-1.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ydl-podcast"
-version = "1.1.1"
+version = "1.2.0"
 description = "A simple tool to generate Podcast-like RSS feeds from youtube (or other youtube-dl supported services) channels, using youtube-dl"
 license = "MIT"
 authors = ["nbr23 <max@23.tf>"]
 homepage = "https://github.com/nbr23/ydl-podcast"
 repository = "https://github.com/nbr23/ydl-podcast"
 keywords = ["podcast", "youtube-dl"]
 readme = "README.md"
@@ -19,14 +19,15 @@
 [tool.poetry.dependencies]
 python = "^3.7"
 youtube-dl = ">=2021.12.17"
 PyYAML = "6.0.1"
 Jinja2 = "^3.1.2"
 MarkupSafe = "^2.1.1"
 yt-dlp = { version = ">=2022.10.4", optional = true }
+Pillow = "10.0.0"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
 yt-dlp = ["yt-dlp"]
 youtube-dl = ["youtube-dl"]
```

### Comparing `ydl_podcast-1.1.1/ydl_podcast/__init__.py` & `ydl_podcast-1.2.0/ydl_podcast/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from urllib.parse import quote
 import json
 import datetime
 from datetime import date, timedelta
 import importlib
 from jinja2 import Template
 from urllib.parse import urljoin
+from PIL import Image
 
 from .template import ATOM_TMPL, SHOW_NFO_TMPL, EPISODE_NFO_TMPL
 
 sub_defaults = {
     "retention_days": None,
     "audio_only": False,
     "download_last": None,
@@ -48,23 +49,38 @@
     extensions = [default_ext, "jpg", "jpeg", "png", "webp"]
     for ext in extensions:
         if os.path.isfile(os.path.join(path, "%s.%s" % (basename, ext))):
             return ext
     return default_ext
 
 
+def convert_thumbnail_to_jpg(path, thumbnail_filename):
+    ext = thumbnail_filename.split(".")[-1]
+    if ext == "jpg" or ext == "jpeg":
+        return thumbnail_filename
+    try:
+        im = Image.open(os.path.join(path, thumbnail_filename))
+        rgb_im = im.convert("RGB")
+        new_thumbnail_filename = thumbnail_filename.replace("."+ext, ".jpg")
+        rgb_im.save(os.path.join(path, new_thumbnail_filename))
+        os.remove(os.path.join(path, thumbnail_filename))
+        return new_thumbnail_filename
+    except Exception as e:
+        print("Error converting thumbnail to jpg: %s" % e)
+        return thumbnail_filename
+
 def metadata_parse(metadata_path):
     with open(metadata_path) as metadata:
         mdjs = json.load(metadata)
         basename = ".".join(os.path.basename(metadata_path).split(".")[:-2])
         path = os.path.dirname(metadata_path)
         thumbnail_file = None
         if mdjs.get("thumbnail") is not None:
             thumb_ext = get_real_thumbnail_ext(metadata_path, mdjs["thumbnail"].split(".")[-1])
-            thumbnail_file = "%s.%s" % (basename, thumb_ext)
+            thumbnail_file = convert_thumbnail_to_jpg(path, "%s.%s" % (basename, thumb_ext))
         extension = metadata_file_extension(mdjs, path, basename)
         if not os.path.isfile(os.path.join(path, "%s.%s" % (basename, extension))):
             with os.scandir(path) as directory:
                 for f in directory:
                     ext = f.name.split(".")[-1]
                     if (
                         f.name.startswith(basename)
```

### Comparing `ydl_podcast-1.1.1/ydl_podcast/__main__.py` & `ydl_podcast-1.2.0/ydl_podcast/__main__.py`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.1.1/ydl_podcast/template.py` & `ydl_podcast-1.2.0/ydl_podcast/template.py`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.1.1/PKG-INFO` & `ydl_podcast-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydl-podcast
-Version: 1.1.1
+Version: 1.2.0
 Summary: A simple tool to generate Podcast-like RSS feeds from youtube (or other youtube-dl supported services) channels, using youtube-dl
 Home-page: https://github.com/nbr23/ydl-podcast
 License: MIT
 Keywords: podcast,youtube-dl
 Author: nbr23
 Author-email: max@23.tf
 Requires-Python: >=3.7,<4.0
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: youtube-dl
 Provides-Extra: yt-dlp
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: MarkupSafe (>=2.1.1,<3.0.0)
+Requires-Dist: Pillow (==10.0.0)
 Requires-Dist: PyYAML (==6.0.1)
 Requires-Dist: youtube-dl (>=2021.12.17) ; extra == "youtube-dl"
 Requires-Dist: yt-dlp (>=2022.10.4) ; extra == "yt-dlp"
 Project-URL: Repository, https://github.com/nbr23/ydl-podcast
 Description-Content-Type: text/markdown
 
 [![Pypi Version Shield](https://img.shields.io/pypi/v/ydl-podcast.svg?style=flat-square)](https://pypi.org/project/ydl-podcast/)
```

