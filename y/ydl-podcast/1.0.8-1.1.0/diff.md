# Comparing `tmp/ydl_podcast-1.0.8.tar.gz` & `tmp/ydl_podcast-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ydl_podcast-1.0.8.tar", max compression
+gzip compressed data, was "ydl_podcast-1.1.0.tar", max compression
```

## Comparing `ydl_podcast-1.0.8.tar` & `ydl_podcast-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1102 2023-07-03 20:16:08.783020 ydl_podcast-1.0.8/LICENSE
--rw-r--r--   0        0        0     2830 2023-07-03 20:16:08.787020 ydl_podcast-1.0.8/README.md
--rw-r--r--   0        0        0      895 2023-07-03 20:16:08.787020 ydl_podcast-1.0.8/pyproject.toml
--rw-r--r--   0        0        0    12989 2023-07-03 20:16:08.787020 ydl_podcast-1.0.8/ydl_podcast/__init__.py
--rwxr-xr-x   0        0        0     1830 2023-07-03 20:16:08.787020 ydl_podcast-1.0.8/ydl_podcast/__main__.py
--rw-r--r--   0        0        0      982 2023-07-03 20:16:08.787020 ydl_podcast-1.0.8/ydl_podcast/template.py
--rw-r--r--   0        0        0     3918 1970-01-01 00:00:00.000000 ydl_podcast-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-07-30 02:46:39.227326 ydl_podcast-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3100 2023-07-30 02:46:39.227326 ydl_podcast-1.1.0/README.md
+-rw-r--r--   0        0        0      897 2023-07-30 02:46:39.227326 ydl_podcast-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    14288 2023-07-30 02:46:39.227326 ydl_podcast-1.1.0/ydl_podcast/__init__.py
+-rwxr-xr-x   0        0        0     1872 2023-07-30 02:46:39.227326 ydl_podcast-1.1.0/ydl_podcast/__main__.py
+-rw-r--r--   0        0        0     1482 2023-07-30 02:46:39.227326 ydl_podcast-1.1.0/ydl_podcast/template.py
+-rw-r--r--   0        0        0     4190 1970-01-01 00:00:00.000000 ydl_podcast-1.1.0/PKG-INFO
```

### Comparing `ydl_podcast-1.0.8/LICENSE` & `ydl_podcast-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.0.8/README.md` & `ydl_podcast-1.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 - `url_root`: root url for the static files (used in the generation of the XML
   to point to the media files.
 - `format`: file format to force youtube-dl to use (eg mp4, webm, mp3 for audio
   only…)
 - `best`: force best quality (only useful when specifying a format).
 - `ydl_options`: list of raw youtube-dl options to use. For experienced users,
   since this will likely yield issues if not understood.
+- `nfo_files`: generates nfo files for subscriptions and downloaded episodes (simulates a "tvshow" nfo for the subscription and "tvshow episode" for each video). This helps plex, kodi, jellyfin import correct metadata. Does NOT support `audio_only` feeds at this point.
 
 ## Usage
 
 Using cron or your favorite scheduler, run:
 
 `ydl_podcast [configfile.yaml]`
```

### Comparing `ydl_podcast-1.0.8/pyproject.toml` & `ydl_podcast-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ydl-podcast"
-version = "1.0.8"
+version = "1.1.0"
 description = "A simple tool to generate Podcast-like RSS feeds from youtube (or other youtube-dl supported services) channels, using youtube-dl"
 license = "MIT"
 authors = ["nbr23 <max@23.tf>"]
 homepage = "https://github.com/nbr23/ydl-podcast"
 repository = "https://github.com/nbr23/ydl-podcast"
 keywords = ["podcast", "youtube-dl"]
 readme = "README.md"
@@ -15,15 +15,15 @@
 
 [tool.poetry.scripts]
 ydl-podcast = 'ydl_podcast.__main__:main'
 
 [tool.poetry.dependencies]
 python = "^3.7"
 youtube-dl = ">=2021.12.17"
-PyYAML = "6.0"
+PyYAML = "6.0.1"
 Jinja2 = "^3.1.2"
 MarkupSafe = "^2.1.1"
 yt-dlp = { version = ">=2022.10.4", optional = true }
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
```

### Comparing `ydl_podcast-1.0.8/ydl_podcast/__init__.py` & `ydl_podcast-1.1.0/ydl_podcast/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import json
 import datetime
 from datetime import date, timedelta
 import importlib
 from jinja2 import Template
 from urllib.parse import urljoin
 
-from .template import ATOM_TMPL
+from .template import ATOM_TMPL, SHOW_NFO_TMPL, EPISODE_NFO_TMPL
 
 sub_defaults = {
     "retention_days": None,
     "audio_only": False,
     "download_last": None,
     "initialize": False,
     "best": False,
@@ -321,14 +321,47 @@
         ret = date.today() - timedelta(days=sub["retention_days"])
         if mtime < ret:
             os.remove(fpath)
             deleted.append(fpath)
     return deleted
 
 
+def write_sub_nfo(sub):
+    if not sub.get('nfo_files', False) or sub.get("audio_only", False):
+        return
+    nso_file = os.path.join(sub["output_dir"], sub["name"], "tvshow.nfo")
+    sub_nfo_tmpl = SHOW_NFO_TMPL
+    episode_nfo_tmpl = EPISODE_NFO_TMPL
+
+    if not os.path.exists(nso_file):
+        with open(nso_file, "w+") as fout:
+            fout.write(Template(sub_nfo_tmpl).render({
+                "title": sub.get("pretty_name", sub["name"])
+            }))
+
+    mds = [
+        metadata_parse(md_file)
+        for md_file in glob.glob(
+            os.path.join(sub["output_dir"], "%s/*.info.json" % sub["name"])
+        )
+    ]
+
+    for md in mds:
+        nfo_file = os.path.join(sub["output_dir"], sub["name"], "%s.nfo" % ".".join(md["filename"].split(".")[:-1]))
+        ep_date = datetime.datetime.strptime(md["pub_date"], "%a, %d %b %Y %H:%M:%S +0000").strftime("%Y-%m-%d")
+        if not os.path.exists(nfo_file):
+            with open(nfo_file, "w+") as fout:
+                fout.write(Template(EPISODE_NFO_TMPL).render({
+                    "title": md["title"],
+                    "ep_date": ep_date,
+                    "show_title": sub.get("pretty_name", sub["name"]),
+                    "duration": md["duration"],
+                }))
+
+
 def write_xml(sub):
     mds = [
         metadata_parse(md_file)
         for md_file in glob.glob(
             os.path.join(sub["output_dir"], "%s/*.info.json" % sub["name"])
         )
     ]
```

### Comparing `ydl_podcast-1.0.8/ydl_podcast/__main__.py` & `ydl_podcast-1.1.0/ydl_podcast/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! /usr/bin/env python3
 
 import os
 import sys
 from collections import ChainMap
 
-from . import load_config, write_xml, cleanup, download, sub_defaults, get_ydl_module
+from . import load_config, write_xml, cleanup, download, sub_defaults, get_ydl_module, write_sub_nfo
 
 
 def main():
     argv = sys.argv
     config = load_config(argv[1] if len(argv) > 1 else "config.yaml")
     if not config:
         print("No valid configuration found.")
@@ -54,12 +54,13 @@
             sub["initialize"] = False
 
         download(ydl_mod, sub)
 
         if sub["retention_days"] is not None and not sub["initialize"]:
             cleanup(sub)
 
+        write_sub_nfo(sub)
         write_xml(sub)
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `ydl_podcast-1.0.8/PKG-INFO` & `ydl_podcast-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydl-podcast
-Version: 1.0.8
+Version: 1.1.0
 Summary: A simple tool to generate Podcast-like RSS feeds from youtube (or other youtube-dl supported services) channels, using youtube-dl
 Home-page: https://github.com/nbr23/ydl-podcast
 License: MIT
 Keywords: podcast,youtube-dl
 Author: nbr23
 Author-email: max@23.tf
 Requires-Python: >=3.7,<4.0
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: youtube-dl
 Provides-Extra: yt-dlp
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: MarkupSafe (>=2.1.1,<3.0.0)
-Requires-Dist: PyYAML (==6.0)
+Requires-Dist: PyYAML (==6.0.1)
 Requires-Dist: youtube-dl (>=2021.12.17) ; extra == "youtube-dl"
 Requires-Dist: yt-dlp (>=2022.10.4) ; extra == "yt-dlp"
 Project-URL: Repository, https://github.com/nbr23/ydl-podcast
 Description-Content-Type: text/markdown
 
 [![Pypi Version Shield](https://img.shields.io/pypi/v/ydl-podcast.svg?style=flat-square)](https://pypi.org/project/ydl-podcast/)
 [![Pypi License Shield](https://img.shields.io/pypi/l/ydl-podcast.svg?style=flat-square)](https://pypi.org/project/ydl-podcast/)
@@ -84,14 +84,15 @@
 - `url_root`: root url for the static files (used in the generation of the XML
   to point to the media files.
 - `format`: file format to force youtube-dl to use (eg mp4, webm, mp3 for audio
   only…)
 - `best`: force best quality (only useful when specifying a format).
 - `ydl_options`: list of raw youtube-dl options to use. For experienced users,
   since this will likely yield issues if not understood.
+- `nfo_files`: generates nfo files for subscriptions and downloaded episodes (simulates a "tvshow" nfo for the subscription and "tvshow episode" for each video). This helps plex, kodi, jellyfin import correct metadata. Does NOT support `audio_only` feeds at this point.
 
 ## Usage
 
 Using cron or your favorite scheduler, run:
 
 `ydl_podcast [configfile.yaml]`
```

