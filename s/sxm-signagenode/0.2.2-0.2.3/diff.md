# Comparing `tmp/sxm-signagenode-0.2.2.tar.gz` & `tmp/sxm-signagenode-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sxm-signagenode-0.2.2.tar", last modified: Sun Jul 30 19:06:33 2023, max compression
+gzip compressed data, was "sxm-signagenode-0.2.3.tar", last modified: Sun Jul 30 19:14:39 2023, max compression
```

## Comparing `sxm-signagenode-0.2.2.tar` & `sxm-signagenode-0.2.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-30 19:06:33.611070 sxm-signagenode-0.2.2/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2233 2023-03-15 17:22:17.000000 sxm-signagenode-0.2.2/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       76 2023-03-15 17:22:17.000000 sxm-signagenode-0.2.2/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      608 2023-07-30 19:06:33.611070 sxm-signagenode-0.2.2/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       38 2023-07-30 19:06:33.611070 sxm-signagenode-0.2.2/setup.cfg
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1293 2023-07-28 15:59:04.000000 sxm-signagenode-0.2.2/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-30 19:06:33.607069 sxm-signagenode-0.2.2/sxm/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 17:22:17.000000 sxm-signagenode-0.2.2/sxm/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-30 19:06:33.607069 sxm-signagenode-0.2.2/sxm/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      290 2023-04-04 17:49:48.000000 sxm-signagenode-0.2.2/sxm/api/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1771 2023-07-23 18:53:04.000000 sxm-signagenode-0.2.2/sxm/api/announce.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3243 2023-04-03 16:12:23.000000 sxm-signagenode-0.2.2/sxm/api/auth.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1162 2023-07-28 15:57:39.000000 sxm-signagenode-0.2.2/sxm/api/core.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4049 2023-03-15 17:22:17.000000 sxm-signagenode-0.2.2/sxm/api/events.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1123 2023-03-15 17:22:17.000000 sxm-signagenode-0.2.2/sxm/api/gallery.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2631 2023-03-15 17:22:17.000000 sxm-signagenode-0.2.2/sxm/api/media.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     5578 2023-07-30 19:03:50.000000 sxm-signagenode-0.2.2/sxm/api/settings.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2415 2023-03-15 17:22:17.000000 sxm-signagenode-0.2.2/sxm/api/text.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      170 2023-03-15 17:22:17.000000 sxm-signagenode-0.2.2/sxm/app.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3419 2023-07-29 19:31:14.000000 sxm-signagenode-0.2.2/sxm/node.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      710 2023-03-15 17:22:17.000000 sxm-signagenode-0.2.2/sxm/runnode.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-30 19:06:33.611070 sxm-signagenode-0.2.2/sxm_signagenode.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      608 2023-07-30 19:06:33.000000 sxm-signagenode-0.2.2/sxm_signagenode.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      483 2023-07-30 19:06:33.000000 sxm-signagenode-0.2.2/sxm_signagenode.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-07-30 19:06:33.000000 sxm-signagenode-0.2.2/sxm_signagenode.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       57 2023-07-30 19:06:33.000000 sxm-signagenode-0.2.2/sxm_signagenode.egg-info/entry_points.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      120 2023-07-30 19:06:33.000000 sxm-signagenode-0.2.2/sxm_signagenode.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        4 2023-07-30 19:06:33.000000 sxm-signagenode-0.2.2/sxm_signagenode.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-30 19:14:39.563716 sxm-signagenode-0.2.3/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2233 2023-03-15 17:22:17.000000 sxm-signagenode-0.2.3/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       76 2023-03-15 17:22:17.000000 sxm-signagenode-0.2.3/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      608 2023-07-30 19:14:39.563716 sxm-signagenode-0.2.3/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       38 2023-07-30 19:14:39.563716 sxm-signagenode-0.2.3/setup.cfg
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1293 2023-07-28 15:59:04.000000 sxm-signagenode-0.2.3/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-30 19:14:39.559716 sxm-signagenode-0.2.3/sxm/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 17:22:17.000000 sxm-signagenode-0.2.3/sxm/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-30 19:14:39.563716 sxm-signagenode-0.2.3/sxm/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      290 2023-04-04 17:49:48.000000 sxm-signagenode-0.2.3/sxm/api/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1771 2023-07-23 18:53:04.000000 sxm-signagenode-0.2.3/sxm/api/announce.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3243 2023-04-03 16:12:23.000000 sxm-signagenode-0.2.3/sxm/api/auth.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1162 2023-07-28 15:57:39.000000 sxm-signagenode-0.2.3/sxm/api/core.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4049 2023-03-15 17:22:17.000000 sxm-signagenode-0.2.3/sxm/api/events.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1123 2023-03-15 17:22:17.000000 sxm-signagenode-0.2.3/sxm/api/gallery.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2631 2023-03-15 17:22:17.000000 sxm-signagenode-0.2.3/sxm/api/media.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     5635 2023-07-30 19:14:18.000000 sxm-signagenode-0.2.3/sxm/api/settings.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2415 2023-03-15 17:22:17.000000 sxm-signagenode-0.2.3/sxm/api/text.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      170 2023-03-15 17:22:17.000000 sxm-signagenode-0.2.3/sxm/app.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3419 2023-07-29 19:31:14.000000 sxm-signagenode-0.2.3/sxm/node.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      710 2023-03-15 17:22:17.000000 sxm-signagenode-0.2.3/sxm/runnode.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-30 19:14:39.563716 sxm-signagenode-0.2.3/sxm_signagenode.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      608 2023-07-30 19:14:39.000000 sxm-signagenode-0.2.3/sxm_signagenode.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      483 2023-07-30 19:14:39.000000 sxm-signagenode-0.2.3/sxm_signagenode.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-07-30 19:14:39.000000 sxm-signagenode-0.2.3/sxm_signagenode.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       57 2023-07-30 19:14:39.000000 sxm-signagenode-0.2.3/sxm_signagenode.egg-info/entry_points.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      120 2023-07-30 19:14:39.000000 sxm-signagenode-0.2.3/sxm_signagenode.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        4 2023-07-30 19:14:39.000000 sxm-signagenode-0.2.3/sxm_signagenode.egg-info/top_level.txt
```

### Comparing `sxm-signagenode-0.2.2/.gitignore` & `sxm-signagenode-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `sxm-signagenode-0.2.2/PKG-INFO` & `sxm-signagenode-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sxm-signagenode
-Version: 0.2.2
+Version: 0.2.3
 Summary: Generic StarXMedia Signage Node
 Home-page: https://github.com/starxmedia/sxm-signagenode
 Author: Chintalagiri Shashank
 Author-email: shashank.chintalagiri@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `sxm-signagenode-0.2.2/setup.py` & `sxm-signagenode-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `sxm-signagenode-0.2.2/sxm/api/announce.py` & `sxm-signagenode-0.2.3/sxm/api/announce.py`

 * *Files identical despite different names*

### Comparing `sxm-signagenode-0.2.2/sxm/api/auth.py` & `sxm-signagenode-0.2.3/sxm/api/auth.py`

 * *Files identical despite different names*

### Comparing `sxm-signagenode-0.2.2/sxm/api/core.py` & `sxm-signagenode-0.2.3/sxm/api/core.py`

 * *Files identical despite different names*

### Comparing `sxm-signagenode-0.2.2/sxm/api/events.py` & `sxm-signagenode-0.2.3/sxm/api/events.py`

 * *Files identical despite different names*

### Comparing `sxm-signagenode-0.2.2/sxm/api/gallery.py` & `sxm-signagenode-0.2.3/sxm/api/gallery.py`

 * *Files identical despite different names*

### Comparing `sxm-signagenode-0.2.2/sxm/api/media.py` & `sxm-signagenode-0.2.3/sxm/api/media.py`

 * *Files identical despite different names*

### Comparing `sxm-signagenode-0.2.2/sxm/api/settings.py` & `sxm-signagenode-0.2.3/sxm/api/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,16 +91,18 @@
                 return
             if default['content_type'] == 'structured':
                 ldefault = "structured:{0}".format(default['path'])
                 self._actual.background_set(ldefault)
             elif default['content_type'] == 'media':
                 uri, _ = self._get_content_uri(default)
                 r, d = self._prepare_content(uri)
-                d.addCallback(lambda _: self._actual.background_set(r.cache_path))
-                d.addCallback(lambda _: self._actual.background_sequence_set([]))
+                def _set_simple_bg(*args, **kwargs):
+                    self._actual.background_set(r.cache_path)
+                    self._actual.background_sequence_set([])
+                d.addCallback(_set_simple_bg)
             elif default['content_type'] == 'sequence':
                 seq, d = self._process_sequence(default)
                 d.addCallback(lambda _: self._actual.background_sequence_set(seq))
                 pass
             else:
                 self.log.error(f"content_type {default['content_type']} not supported. Not setting.")
```

### Comparing `sxm-signagenode-0.2.2/sxm/api/text.py` & `sxm-signagenode-0.2.3/sxm/api/text.py`

 * *Files identical despite different names*

### Comparing `sxm-signagenode-0.2.2/sxm/node.py` & `sxm-signagenode-0.2.3/sxm/node.py`

 * *Files identical despite different names*

### Comparing `sxm-signagenode-0.2.2/sxm/runnode.py` & `sxm-signagenode-0.2.3/sxm/runnode.py`

 * *Files identical despite different names*

### Comparing `sxm-signagenode-0.2.2/sxm_signagenode.egg-info/PKG-INFO` & `sxm-signagenode-0.2.3/sxm_signagenode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sxm-signagenode
-Version: 0.2.2
+Version: 0.2.3
 Summary: Generic StarXMedia Signage Node
 Home-page: https://github.com/starxmedia/sxm-signagenode
 Author: Chintalagiri Shashank
 Author-email: shashank.chintalagiri@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

