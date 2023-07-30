# Comparing `tmp/PlexAPI-4.9.1.tar.gz` & `tmp/PlexAPI-4.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PlexAPI-4.9.1.tar", last modified: Mon Jan 24 22:14:26 2022, max compression
+gzip compressed data, was "dist/PlexAPI-4.9.2.tar", last modified: Mon Feb  7 05:02:18 2022, max compression
```

## Comparing `PlexAPI-4.9.1.tar` & `PlexAPI-4.9.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 22:14:26.000000 PlexAPI-4.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-01-24 22:14:22.000000 PlexAPI-4.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    10957 2022-01-24 22:14:26.000000 PlexAPI-4.9.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 22:14:26.000000 PlexAPI-4.9.1/PlexAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10957 2022-01-24 22:14:26.000000 PlexAPI-4.9.1/PlexAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      619 2022-01-24 22:14:26.000000 PlexAPI-4.9.1/PlexAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-24 22:14:26.000000 PlexAPI-4.9.1/PlexAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-01-24 22:14:26.000000 PlexAPI-4.9.1/PlexAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-01-24 22:14:26.000000 PlexAPI-4.9.1/PlexAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     8459 2022-01-24 22:14:22.000000 PlexAPI-4.9.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 22:14:26.000000 PlexAPI-4.9.1/plexapi/
--rw-r--r--   0 runner    (1001) docker     (121)     2119 2022-01-24 22:14:22.000000 PlexAPI-4.9.1/plexapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4456 2022-01-24 22:14:22.000000 PlexAPI-4.9.1/plexapi/alert.py
--rw-r--r--   0 runner    (1001) docker     (121)    22427 2022-01-24 22:14:22.000000 PlexAPI-4.9.1/plexapi/audio.py
--rw-r--r--   0 runner    (1001) docker     (121)    36661 2022-01-24 22:14:22.000000 PlexAPI-4.9.1/plexapi/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    27874 2022-01-24 22:14:22.000000 PlexAPI-4.9.1/plexapi/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    23588 2022-01-24 22:14:22.000000 PlexAPI-4.9.1/plexapi/collection.py
--rw-r--r--   0 runner    (1001) docker     (121)     2562 2022-01-24 22:14:22.000000 PlexAPI-4.9.1/plexapi/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-01-24 22:14:22.000000 PlexAPI-4.9.1/plexapi/const.py
--rw-r--r--   0 runner    (1001) docker     (121)      585 2022-01-24 22:14:22.000000 PlexAPI-4.9.1/plexapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5066 2022-01-24 22:14:22.000000 PlexAPI-4.9.1/plexapi/gdm.py
--rw-r--r--   0 runner    (1001) docker     (121)   117857 2022-01-24 22:14:22.000000 PlexAPI-4.9.1/plexapi/library.py
--rw-r--r--   0 runner    (1001) docker     (121)    46465 2022-01-24 22:14:22.000000 PlexAPI-4.9.1/plexapi/media.py
--rw-r--r--   0 runner    (1001) docker     (121)    23659 2022-01-24 22:14:22.000000 PlexAPI-4.9.1/plexapi/mixins.py
--rw-r--r--   0 runner    (1001) docker     (121)    74269 2022-01-24 22:14:22.000000 PlexAPI-4.9.1/plexapi/myplex.py
--rw-r--r--   0 runner    (1001) docker     (121)    14262 2022-01-24 22:14:22.000000 PlexAPI-4.9.1/plexapi/photo.py
--rw-r--r--   0 runner    (1001) docker     (121)    21626 2022-01-24 22:14:22.000000 PlexAPI-4.9.1/plexapi/playlist.py
--rw-r--r--   0 runner    (1001) docker     (121)    13763 2022-01-24 22:14:22.000000 PlexAPI-4.9.1/plexapi/playqueue.py
--rw-r--r--   0 runner    (1001) docker     (121)    58023 2022-01-24 22:14:22.000000 PlexAPI-4.9.1/plexapi/server.py
--rw-r--r--   0 runner    (1001) docker     (121)     7030 2022-01-24 22:14:22.000000 PlexAPI-4.9.1/plexapi/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     5085 2022-01-24 22:14:22.000000 PlexAPI-4.9.1/plexapi/sonos.py
--rw-r--r--   0 runner    (1001) docker     (121)    13755 2022-01-24 22:14:22.000000 PlexAPI-4.9.1/plexapi/sync.py
--rw-r--r--   0 runner    (1001) docker     (121)    18294 2022-01-24 22:14:22.000000 PlexAPI-4.9.1/plexapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    48382 2022-01-24 22:14:22.000000 PlexAPI-4.9.1/plexapi/video.py
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-01-24 22:14:22.000000 PlexAPI-4.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-24 22:14:26.000000 PlexAPI-4.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-01-24 22:14:22.000000 PlexAPI-4.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 05:02:18.000000 PlexAPI-4.9.2/
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-02-07 05:02:12.000000 PlexAPI-4.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    10957 2022-02-07 05:02:18.000000 PlexAPI-4.9.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 05:02:18.000000 PlexAPI-4.9.2/PlexAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    10957 2022-02-07 05:02:17.000000 PlexAPI-4.9.2/PlexAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      619 2022-02-07 05:02:18.000000 PlexAPI-4.9.2/PlexAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-07 05:02:17.000000 PlexAPI-4.9.2/PlexAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-02-07 05:02:17.000000 PlexAPI-4.9.2/PlexAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-02-07 05:02:17.000000 PlexAPI-4.9.2/PlexAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     8459 2022-02-07 05:02:12.000000 PlexAPI-4.9.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 05:02:18.000000 PlexAPI-4.9.2/plexapi/
+-rw-r--r--   0 runner    (1001) docker     (121)     2119 2022-02-07 05:02:12.000000 PlexAPI-4.9.2/plexapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4456 2022-02-07 05:02:12.000000 PlexAPI-4.9.2/plexapi/alert.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22461 2022-02-07 05:02:12.000000 PlexAPI-4.9.2/plexapi/audio.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36661 2022-02-07 05:02:12.000000 PlexAPI-4.9.2/plexapi/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27874 2022-02-07 05:02:12.000000 PlexAPI-4.9.2/plexapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23588 2022-02-07 05:02:12.000000 PlexAPI-4.9.2/plexapi/collection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2562 2022-02-07 05:02:12.000000 PlexAPI-4.9.2/plexapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      238 2022-02-07 05:02:12.000000 PlexAPI-4.9.2/plexapi/const.py
+-rw-r--r--   0 runner    (1001) docker     (121)      585 2022-02-07 05:02:12.000000 PlexAPI-4.9.2/plexapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5066 2022-02-07 05:02:12.000000 PlexAPI-4.9.2/plexapi/gdm.py
+-rw-r--r--   0 runner    (1001) docker     (121)   117857 2022-02-07 05:02:12.000000 PlexAPI-4.9.2/plexapi/library.py
+-rw-r--r--   0 runner    (1001) docker     (121)    46465 2022-02-07 05:02:12.000000 PlexAPI-4.9.2/plexapi/media.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23659 2022-02-07 05:02:12.000000 PlexAPI-4.9.2/plexapi/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (121)    74269 2022-02-07 05:02:12.000000 PlexAPI-4.9.2/plexapi/myplex.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14262 2022-02-07 05:02:12.000000 PlexAPI-4.9.2/plexapi/photo.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21626 2022-02-07 05:02:12.000000 PlexAPI-4.9.2/plexapi/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13763 2022-02-07 05:02:12.000000 PlexAPI-4.9.2/plexapi/playqueue.py
+-rw-r--r--   0 runner    (1001) docker     (121)    58023 2022-02-07 05:02:12.000000 PlexAPI-4.9.2/plexapi/server.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7030 2022-02-07 05:02:12.000000 PlexAPI-4.9.2/plexapi/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5085 2022-02-07 05:02:12.000000 PlexAPI-4.9.2/plexapi/sonos.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13755 2022-02-07 05:02:12.000000 PlexAPI-4.9.2/plexapi/sync.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18294 2022-02-07 05:02:12.000000 PlexAPI-4.9.2/plexapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    48382 2022-02-07 05:02:12.000000 PlexAPI-4.9.2/plexapi/video.py
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2022-02-07 05:02:12.000000 PlexAPI-4.9.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-07 05:02:18.000000 PlexAPI-4.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-02-07 05:02:12.000000 PlexAPI-4.9.2/setup.py
```

### Comparing `PlexAPI-4.9.1/PKG-INFO` & `PlexAPI-4.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: PlexAPI
-Version: 4.9.1
+Version: 4.9.2
 Summary: Python bindings for the Plex API.
 Home-page: https://github.com/pkkid/python-plexapi
 Author: Michael Shepanski
 Author-email: michael.shepanski@gmail.com
 License: UNKNOWN
 Description: Python-PlexAPI
         ==============
```

### Comparing `PlexAPI-4.9.1/PlexAPI.egg-info/PKG-INFO` & `PlexAPI-4.9.2/PlexAPI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: PlexAPI
-Version: 4.9.1
+Version: 4.9.2
 Summary: Python bindings for the Plex API.
 Home-page: https://github.com/pkkid/python-plexapi
 Author: Michael Shepanski
 Author-email: michael.shepanski@gmail.com
 License: UNKNOWN
 Description: Python-PlexAPI
         ==============
```

### Comparing `PlexAPI-4.9.1/PlexAPI.egg-info/SOURCES.txt` & `PlexAPI-4.9.2/PlexAPI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PlexAPI-4.9.1/README.rst` & `PlexAPI-4.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `PlexAPI-4.9.1/plexapi/__init__.py` & `PlexAPI-4.9.2/plexapi/__init__.py`

 * *Files identical despite different names*

### Comparing `PlexAPI-4.9.1/plexapi/alert.py` & `PlexAPI-4.9.2/plexapi/alert.py`

 * *Files identical despite different names*

### Comparing `PlexAPI-4.9.1/plexapi/audio.py` & `PlexAPI-4.9.2/plexapi/audio.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
                 title (str): Title of the album to return.
         """
         key = '/library/metadata/%s/children' % self.ratingKey
         return self.fetchItem(key, Album, title__iexact=title)
 
     def albums(self, **kwargs):
         """ Returns a list of :class:`~plexapi.audio.Album` objects by the artist. """
-        key = '/library/metadata/%s/children' % self.ratingKey
+        key = f"/library/sections/{self.librarySectionID}/all?artist.id={self.ratingKey}&type=9"
         return self.fetchItems(key, Album, **kwargs)
 
     def track(self, title=None, album=None, track=None):
         """ Returns the :class:`~plexapi.audio.Track` that matches the specified title.
 
             Parameters:
                 title (str): Title of the track to return.
```

### Comparing `PlexAPI-4.9.1/plexapi/base.py` & `PlexAPI-4.9.2/plexapi/base.py`

 * *Files identical despite different names*

### Comparing `PlexAPI-4.9.1/plexapi/client.py` & `PlexAPI-4.9.2/plexapi/client.py`

 * *Files identical despite different names*

### Comparing `PlexAPI-4.9.1/plexapi/collection.py` & `PlexAPI-4.9.2/plexapi/collection.py`

 * *Files identical despite different names*

### Comparing `PlexAPI-4.9.1/plexapi/config.py` & `PlexAPI-4.9.2/plexapi/config.py`

 * *Files identical despite different names*

### Comparing `PlexAPI-4.9.1/plexapi/exceptions.py` & `PlexAPI-4.9.2/plexapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `PlexAPI-4.9.1/plexapi/gdm.py` & `PlexAPI-4.9.2/plexapi/gdm.py`

 * *Files identical despite different names*

### Comparing `PlexAPI-4.9.1/plexapi/library.py` & `PlexAPI-4.9.2/plexapi/library.py`

 * *Files identical despite different names*

### Comparing `PlexAPI-4.9.1/plexapi/media.py` & `PlexAPI-4.9.2/plexapi/media.py`

 * *Files identical despite different names*

### Comparing `PlexAPI-4.9.1/plexapi/mixins.py` & `PlexAPI-4.9.2/plexapi/mixins.py`

 * *Files identical despite different names*

### Comparing `PlexAPI-4.9.1/plexapi/myplex.py` & `PlexAPI-4.9.2/plexapi/myplex.py`

 * *Files identical despite different names*

### Comparing `PlexAPI-4.9.1/plexapi/photo.py` & `PlexAPI-4.9.2/plexapi/photo.py`

 * *Files identical despite different names*

### Comparing `PlexAPI-4.9.1/plexapi/playlist.py` & `PlexAPI-4.9.2/plexapi/playlist.py`

 * *Files identical despite different names*

### Comparing `PlexAPI-4.9.1/plexapi/playqueue.py` & `PlexAPI-4.9.2/plexapi/playqueue.py`

 * *Files identical despite different names*

### Comparing `PlexAPI-4.9.1/plexapi/server.py` & `PlexAPI-4.9.2/plexapi/server.py`

 * *Files identical despite different names*

### Comparing `PlexAPI-4.9.1/plexapi/settings.py` & `PlexAPI-4.9.2/plexapi/settings.py`

 * *Files identical despite different names*

### Comparing `PlexAPI-4.9.1/plexapi/sonos.py` & `PlexAPI-4.9.2/plexapi/sonos.py`

 * *Files identical despite different names*

### Comparing `PlexAPI-4.9.1/plexapi/sync.py` & `PlexAPI-4.9.2/plexapi/sync.py`

 * *Files identical despite different names*

### Comparing `PlexAPI-4.9.1/plexapi/utils.py` & `PlexAPI-4.9.2/plexapi/utils.py`

 * *Files identical despite different names*

### Comparing `PlexAPI-4.9.1/plexapi/video.py` & `PlexAPI-4.9.2/plexapi/video.py`

 * *Files identical despite different names*

### Comparing `PlexAPI-4.9.1/setup.py` & `PlexAPI-4.9.2/setup.py`

 * *Files identical despite different names*

