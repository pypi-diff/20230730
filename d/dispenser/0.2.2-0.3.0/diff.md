# Comparing `tmp/dispenser-0.2.2.tar.gz` & `tmp/dispenser-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dispenser-0.2.2.tar", last modified: Mon Mar 27 15:04:57 2023, max compression
+gzip compressed data, was "dispenser-0.3.0.tar", last modified: Sun Jul 30 12:18:07 2023, max compression
```

## Comparing `dispenser-0.2.2.tar` & `dispenser-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 15:04:57.370453 dispenser-0.2.2/
--rw-rw-rw-   0        0        0      643 2023-03-27 15:04:57.370453 dispenser-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      119 2023-03-26 17:23:03.000000 dispenser-0.2.2/README.md
--rw-rw-rw-   0        0        0       90 2023-03-26 17:25:50.000000 dispenser-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0      686 2023-03-27 15:04:57.372452 dispenser-0.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-27 15:04:57.338562 dispenser-0.2.2/src/
-drwxrwxrwx   0        0        0        0 2023-03-27 15:04:57.347491 dispenser-0.2.2/src/dispenser/
--rw-rw-rw-   0        0        0       36 2023-03-27 14:29:16.000000 dispenser-0.2.2/src/dispenser/__init__.py
--rw-rw-rw-   0        0        0      525 2023-03-27 14:37:43.000000 dispenser-0.2.2/src/dispenser/create.py
-drwxrwxrwx   0        0        0        0 2023-03-27 15:04:57.369436 dispenser-0.2.2/src/dispenser/impl/
--rw-rw-rw-   0        0        0      371 2023-03-26 17:08:17.000000 dispenser-0.2.2/src/dispenser/impl/__init__.py
--rw-rw-rw-   0        0        0     1541 2023-03-27 15:04:14.000000 dispenser-0.2.2/src/dispenser/impl/forge.py
--rw-rw-rw-   0        0        0     1900 2023-03-26 17:51:50.000000 dispenser-0.2.2/src/dispenser/impl/paper.py
--rw-rw-rw-   0        0        0     1388 2023-03-27 14:40:45.000000 dispenser-0.2.2/src/dispenser/impl/vanilla.py
--rw-rw-rw-   0        0        0     3320 2023-03-27 14:44:07.000000 dispenser-0.2.2/src/dispenser/version_base.py
-drwxrwxrwx   0        0        0        0 2023-03-27 15:04:57.362520 dispenser-0.2.2/src/dispenser.egg-info/
--rw-rw-rw-   0        0        0      643 2023-03-27 15:04:57.000000 dispenser-0.2.2/src/dispenser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      379 2023-03-27 15:04:57.000000 dispenser-0.2.2/src/dispenser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 15:04:57.000000 dispenser-0.2.2/src/dispenser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-03-27 15:04:57.000000 dispenser-0.2.2/src/dispenser.egg-info/top_level.txt
+drwxrwxr-x   0 fritz     (1000) fritz     (1000)        0 2023-07-30 12:18:07.084996 dispenser-0.3.0/
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)      627 2023-07-30 12:18:07.084996 dispenser-0.3.0/PKG-INFO
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)      117 2023-07-30 10:34:16.000000 dispenser-0.3.0/README.md
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)       87 2023-07-30 10:34:16.000000 dispenser-0.3.0/pyproject.toml
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)      657 2023-07-30 12:18:07.088996 dispenser-0.3.0/setup.cfg
+drwxrwxr-x   0 fritz     (1000) fritz     (1000)        0 2023-07-30 12:18:07.084996 dispenser-0.3.0/src/
+drwxrwxr-x   0 fritz     (1000) fritz     (1000)        0 2023-07-30 12:18:07.084996 dispenser-0.3.0/src/dispenser/
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)       97 2023-07-30 10:51:35.000000 dispenser-0.3.0/src/dispenser/__init__.py
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)      637 2023-07-30 11:16:54.000000 dispenser-0.3.0/src/dispenser/create.py
+drwxrwxr-x   0 fritz     (1000) fritz     (1000)        0 2023-07-30 12:18:07.084996 dispenser-0.3.0/src/dispenser/impl/
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)      362 2023-07-30 10:34:16.000000 dispenser-0.3.0/src/dispenser/impl/__init__.py
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)     1856 2023-07-30 11:12:01.000000 dispenser-0.3.0/src/dispenser/impl/forge.py
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)     1846 2023-07-30 12:15:47.000000 dispenser-0.3.0/src/dispenser/impl/paper.py
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)     1337 2023-07-30 12:15:29.000000 dispenser-0.3.0/src/dispenser/impl/vanilla.py
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)      582 2023-07-30 12:16:43.000000 dispenser-0.3.0/src/dispenser/update.py
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)     4497 2023-07-30 12:16:43.000000 dispenser-0.3.0/src/dispenser/version_base.py
+drwxrwxr-x   0 fritz     (1000) fritz     (1000)        0 2023-07-30 12:18:07.084996 dispenser-0.3.0/src/dispenser.egg-info/
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)      627 2023-07-30 12:18:07.000000 dispenser-0.3.0/src/dispenser.egg-info/PKG-INFO
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)      403 2023-07-30 12:18:07.000000 dispenser-0.3.0/src/dispenser.egg-info/SOURCES.txt
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)        1 2023-07-30 12:18:07.000000 dispenser-0.3.0/src/dispenser.egg-info/dependency_links.txt
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)       10 2023-07-30 12:18:07.000000 dispenser-0.3.0/src/dispenser.egg-info/top_level.txt
```

### Comparing `dispenser-0.2.2/PKG-INFO` & `dispenser-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1
-Name: dispenser
-Version: 0.2.2
-Summary: Create Minecraft Servers of various types
-Home-page: https://github.com/xImAnton/dispenser
-Author: xImAnton_
-Author-email: admin@ximanton.de
-Project-URL: Bug Tracker, https://github.com/xImAnton/dispenser/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
-# Dispenser [WIP]
-A python library for creating and managing minecraft servers with various mod and plugin softwares
+Metadata-Version: 2.1
+Name: dispenser
+Version: 0.3.0
+Summary: Create Minecraft Servers of various types
+Home-page: https://github.com/xImAnton/dispenser
+Author: xImAnton_
+Author-email: admin@ximanton.de
+Project-URL: Bug Tracker, https://github.com/xImAnton/dispenser/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+
+# Dispenser [WIP]
+A python library for creating and managing minecraft servers with various mod and plugin softwares
```

### Comparing `dispenser-0.2.2/src/dispenser/create.py` & `dispenser-0.3.0/src/dispenser/create.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,27 @@
-import os
-import urllib.request
-
-from .impl import VERSION_PROVIDERS
-
-
-def init(cache_path: str = "~/__dispenser__/"):
-    for prov in VERSION_PROVIDERS.values():
-        prov.reload(cache_path)
-
-
-def dispense(software: str, major: str, minor: str, directory: str = "."):
-    provider = VERSION_PROVIDERS[software]
-
-    url = provider.get_download(major, minor)
-
-    urllib.request.urlretrieve(url, os.path.join(directory, provider.DOWNLOAD_FILE_NAME))
-
-    provider.post_download(directory, major, minor)
+import os
+import urllib.request
+
+from .impl import VERSION_PROVIDERS
+
+
+def init(cache_path: str = "~/__dispenser__/"):
+    for prov in VERSION_PROVIDERS.values():
+        prov.reload(cache_path)
+
+
+def get_softwares():
+    return list(VERSION_PROVIDERS.keys())
+
+
+def get_software(name: str):
+    return VERSION_PROVIDERS[name]
+
+
+def dispense(software: str, major: str, minor: str, directory: str = "."):
+    provider = VERSION_PROVIDERS[software]
+
+    url = provider.get_download(major, minor)
+
+    urllib.request.urlretrieve(url, os.path.join(directory, provider.DOWNLOAD_FILE_NAME))
+
+    provider.post_download(directory, major, minor)
```

### Comparing `dispenser-0.2.2/src/dispenser/impl/paper.py` & `dispenser-0.3.0/src/dispenser/impl/paper.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-import requests
-
-from ..version_base import VersionProvider
-
-URL_PAPER_GET_VERSIONS = "https://papermc.io/api/v2/projects/paper/"
-URL_PAPER_GET_BUILDS = "https://papermc.io/api/v2/projects/paper/versions/{version}"
-URL_PAPER_GET_BUILD_DOWNLOAD = "https://papermc.io/api/v2/projects/paper/versions/{version}/builds/{build}"
-URL_PAPER_DOWNLOAD = "https://papermc.io/api/v2/projects/paper/versions/{version}/builds/{build}/downloads/{download}"
-
-
-class PaperVersionProvider(VersionProvider):
-    """
-    the version provider for paper servers
-    """
-    NAME = "paper"
-
-    def __init__(self):
-        self.versions = {}
-
-    def has_version(self, major, minor):
-        return major in self.versions.keys() and minor in self.versions[major]
-
-    def reload_from_data(self, data: dict) -> None:
-        self.versions = data
-
-    def fetch_data(self) -> dict:
-        out = {}
-
-        with requests.Session() as session:
-            resp = session.get(URL_PAPER_GET_VERSIONS).json()
-
-            for version in resp["versions"]:
-                builds = session.get(URL_PAPER_GET_BUILDS.format(version=version)).json()
-                out[version] = [str(build) for build in builds["builds"]]
-
-        return out
-
-    def get_download(self, major, minor):
-        with requests.Session() as session:
-            resp = session.get(URL_PAPER_GET_BUILD_DOWNLOAD.format(version=major, build=minor)).json()
-
-        download = resp["downloads"]["application"]["name"]
-        return URL_PAPER_DOWNLOAD.format(version=major, build=minor, download=download)
-
-    def get_major_versions(self):
-        return list(self.versions.keys())
-
-    def get_minor_versions(self, major):
-        if major not in self.versions.keys():
-            return []
-        return self.versions[major]
-
-    def get_minecraft_version(self, major, minor):
-        return major
+import requests
+
+from ..version_base import VersionProvider
+
+URL_PAPER_GET_VERSIONS = "https://papermc.io/api/v2/projects/paper/"
+URL_PAPER_GET_BUILDS = "https://papermc.io/api/v2/projects/paper/versions/{version}"
+URL_PAPER_GET_BUILD_DOWNLOAD = "https://papermc.io/api/v2/projects/paper/versions/{version}/builds/{build}"
+URL_PAPER_DOWNLOAD = "https://papermc.io/api/v2/projects/paper/versions/{version}/builds/{build}/downloads/{download}"
+
+
+class PaperVersionProvider(VersionProvider):
+    """
+    the version provider for paper servers
+    """
+    NAME = "paper"
+
+    def __init__(self):
+        self.versions = {}
+
+    def has_version(self, major, minor):
+        return major in self.versions.keys() and minor in self.versions[major]
+
+    def reload_from_data(self, data: dict) -> None:
+        self.versions = data
+
+    def fetch_data(self) -> dict:
+        out = {}
+
+        with requests.Session() as session:
+            resp = session.get(URL_PAPER_GET_VERSIONS).json()
+
+            for version in resp["versions"]:
+                builds = session.get(URL_PAPER_GET_BUILDS.format(version=version)).json()
+                out[version] = [str(build) for build in builds["builds"]]
+
+        return out
+
+    def get_download(self, major, minor):
+        with requests.Session() as session:
+            resp = session.get(URL_PAPER_GET_BUILD_DOWNLOAD.format(version=major, build=minor)).json()
+
+        download = resp["downloads"]["application"]["name"]
+        return URL_PAPER_DOWNLOAD.format(version=major, build=minor, download=download)
+
+    def get_major_versions(self):
+        return list(self.versions.keys())
+
+    def get_minor_versions(self, major):
+        if major not in self.versions.keys():
+            return []
+        return self.versions[major]
+
+    def get_minecraft_version(self, major, minor):
+        return major
```

### Comparing `dispenser-0.2.2/src/dispenser.egg-info/PKG-INFO` & `dispenser-0.3.0/src/dispenser.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1
-Name: dispenser
-Version: 0.2.2
-Summary: Create Minecraft Servers of various types
-Home-page: https://github.com/xImAnton/dispenser
-Author: xImAnton_
-Author-email: admin@ximanton.de
-Project-URL: Bug Tracker, https://github.com/xImAnton/dispenser/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
-# Dispenser [WIP]
-A python library for creating and managing minecraft servers with various mod and plugin softwares
+Metadata-Version: 2.1
+Name: dispenser
+Version: 0.3.0
+Summary: Create Minecraft Servers of various types
+Home-page: https://github.com/xImAnton/dispenser
+Author: xImAnton_
+Author-email: admin@ximanton.de
+Project-URL: Bug Tracker, https://github.com/xImAnton/dispenser/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+
+# Dispenser [WIP]
+A python library for creating and managing minecraft servers with various mod and plugin softwares
```

