# Comparing `tmp/ydl_podcast-1.1.0.tar.gz` & `tmp/ydl_podcast-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ydl_podcast-1.1.0.tar", max compression
+gzip compressed data, was "ydl_podcast-1.1.1.tar", max compression
```

## Comparing `ydl_podcast-1.1.0.tar` & `ydl_podcast-1.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1102 2023-07-30 02:46:39.227326 ydl_podcast-1.1.0/LICENSE
--rw-r--r--   0        0        0     3100 2023-07-30 02:46:39.227326 ydl_podcast-1.1.0/README.md
--rw-r--r--   0        0        0      897 2023-07-30 02:46:39.227326 ydl_podcast-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    14288 2023-07-30 02:46:39.227326 ydl_podcast-1.1.0/ydl_podcast/__init__.py
--rwxr-xr-x   0        0        0     1872 2023-07-30 02:46:39.227326 ydl_podcast-1.1.0/ydl_podcast/__main__.py
--rw-r--r--   0        0        0     1482 2023-07-30 02:46:39.227326 ydl_podcast-1.1.0/ydl_podcast/template.py
--rw-r--r--   0        0        0     4190 1970-01-01 00:00:00.000000 ydl_podcast-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-07-30 02:46:39.227326 ydl_podcast-1.1.1/LICENSE
+-rw-r--r--   0        0        0     3100 2023-07-30 02:46:39.227326 ydl_podcast-1.1.1/README.md
+-rw-r--r--   0        0        0      897 2023-07-30 02:55:26.080592 ydl_podcast-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    14341 2023-07-30 02:54:28.083609 ydl_podcast-1.1.1/ydl_podcast/__init__.py
+-rwxr-xr-x   0        0        0     1872 2023-07-30 02:46:39.227326 ydl_podcast-1.1.1/ydl_podcast/__main__.py
+-rw-r--r--   0        0        0     1482 2023-07-30 02:46:39.227326 ydl_podcast-1.1.1/ydl_podcast/template.py
+-rw-r--r--   0        0        0     4190 1970-01-01 00:00:00.000000 ydl_podcast-1.1.1/PKG-INFO
```

### Comparing `ydl_podcast-1.1.0/LICENSE` & `ydl_podcast-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.1.0/README.md` & `ydl_podcast-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.1.0/pyproject.toml` & `ydl_podcast-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ydl-podcast"
-version = "1.1.0"
+version = "1.1.1"
 description = "A simple tool to generate Podcast-like RSS feeds from youtube (or other youtube-dl supported services) channels, using youtube-dl"
 license = "MIT"
 authors = ["nbr23 <max@23.tf>"]
 homepage = "https://github.com/nbr23/ydl-podcast"
 repository = "https://github.com/nbr23/ydl-podcast"
 keywords = ["podcast", "youtube-dl"]
 readme = "README.md"
```

### Comparing `ydl_podcast-1.1.0/ydl_podcast/__init__.py` & `ydl_podcast-1.1.1/ydl_podcast/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,14 +324,16 @@
             deleted.append(fpath)
     return deleted
 
 
 def write_sub_nfo(sub):
     if not sub.get('nfo_files', False) or sub.get("audio_only", False):
         return
+    print("Writing NFO files for %s" % sub["name"])
+
     nso_file = os.path.join(sub["output_dir"], sub["name"], "tvshow.nfo")
     sub_nfo_tmpl = SHOW_NFO_TMPL
     episode_nfo_tmpl = EPISODE_NFO_TMPL
 
     if not os.path.exists(nso_file):
         with open(nso_file, "w+") as fout:
             fout.write(Template(sub_nfo_tmpl).render({
```

### Comparing `ydl_podcast-1.1.0/ydl_podcast/__main__.py` & `ydl_podcast-1.1.1/ydl_podcast/__main__.py`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.1.0/ydl_podcast/template.py` & `ydl_podcast-1.1.1/ydl_podcast/template.py`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.1.0/PKG-INFO` & `ydl_podcast-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydl-podcast
-Version: 1.1.0
+Version: 1.1.1
 Summary: A simple tool to generate Podcast-like RSS feeds from youtube (or other youtube-dl supported services) channels, using youtube-dl
 Home-page: https://github.com/nbr23/ydl-podcast
 License: MIT
 Keywords: podcast,youtube-dl
 Author: nbr23
 Author-email: max@23.tf
 Requires-Python: >=3.7,<4.0
```

