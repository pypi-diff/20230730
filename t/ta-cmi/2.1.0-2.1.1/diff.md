# Comparing `tmp/ta-cmi-2.1.0.tar.gz` & `tmp/ta-cmi-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ta-cmi-2.1.0.tar", last modified: Fri Jul 28 19:38:58 2023, max compression
+gzip compressed data, was "ta-cmi-2.1.1.tar", last modified: Sun Jul 30 12:36:16 2023, max compression
```

## Comparing `ta-cmi-2.1.0.tar` & `ta-cmi-2.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:38:58.410140 ta-cmi-2.1.0/
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-07-28 19:38:45.000000 ta-cmi-2.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8082 2023-07-28 19:38:58.410140 ta-cmi-2.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6511 2023-07-28 19:38:45.000000 ta-cmi-2.1.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 19:38:58.411140 ta-cmi-2.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      635 2023-07-28 19:38:45.000000 ta-cmi-2.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:38:58.409140 ta-cmi-2.1.0/ta_cmi/
--rw-rw-rw-   0 root         (0) root         (0)      423 2023-07-28 19:38:45.000000 ta-cmi-2.1.0/ta_cmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2695 2023-07-28 19:38:45.000000 ta-cmi-2.1.0/ta_cmi/api.py
--rw-rw-rw-   0 root         (0) root         (0)     1173 2023-07-28 19:38:45.000000 ta-cmi-2.1.0/ta_cmi/channel.py
--rw-rw-rw-   0 root         (0) root         (0)      638 2023-07-28 19:38:45.000000 ta-cmi-2.1.0/ta_cmi/cmi.py
--rw-rw-rw-   0 root         (0) root         (0)     2618 2023-07-28 19:38:45.000000 ta-cmi-2.1.0/ta_cmi/cmi_api.py
--rw-rw-rw-   0 root         (0) root         (0)      509 2023-07-28 19:38:45.000000 ta-cmi-2.1.0/ta_cmi/cmi_channel.py
--rw-rw-rw-   0 root         (0) root         (0)     2394 2023-07-28 19:38:45.000000 ta-cmi-2.1.0/ta_cmi/coe.py
--rw-rw-rw-   0 root         (0) root         (0)     4351 2023-07-28 19:38:45.000000 ta-cmi-2.1.0/ta_cmi/coe_api.py
--rw-rw-rw-   0 root         (0) root         (0)      393 2023-07-28 19:38:45.000000 ta-cmi-2.1.0/ta_cmi/coe_channel.py
--rw-rw-rw-   0 root         (0) root         (0)     3514 2023-07-28 19:38:45.000000 ta-cmi-2.1.0/ta_cmi/const.py
--rw-rw-rw-   0 root         (0) root         (0)     4341 2023-07-28 19:38:45.000000 ta-cmi-2.1.0/ta_cmi/device.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:38:58.410140 ta-cmi-2.1.0/ta_cmi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8082 2023-07-28 19:38:58.000000 ta-cmi-2.1.0/ta_cmi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      367 2023-07-28 19:38:58.000000 ta-cmi-2.1.0/ta_cmi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 19:38:58.000000 ta-cmi-2.1.0/ta_cmi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-28 19:38:58.000000 ta-cmi-2.1.0/ta_cmi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-28 19:38:58.000000 ta-cmi-2.1.0/ta_cmi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 12:36:16.175466 ta-cmi-2.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-07-30 12:36:03.000000 ta-cmi-2.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8082 2023-07-30 12:36:16.175466 ta-cmi-2.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6511 2023-07-30 12:36:03.000000 ta-cmi-2.1.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-30 12:36:16.175466 ta-cmi-2.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      635 2023-07-30 12:36:03.000000 ta-cmi-2.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 12:36:16.174466 ta-cmi-2.1.1/ta_cmi/
+-rw-rw-rw-   0 root         (0) root         (0)      423 2023-07-30 12:36:03.000000 ta-cmi-2.1.1/ta_cmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2695 2023-07-30 12:36:03.000000 ta-cmi-2.1.1/ta_cmi/api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1173 2023-07-30 12:36:03.000000 ta-cmi-2.1.1/ta_cmi/channel.py
+-rw-rw-rw-   0 root         (0) root         (0)      638 2023-07-30 12:36:03.000000 ta-cmi-2.1.1/ta_cmi/cmi.py
+-rw-rw-rw-   0 root         (0) root         (0)     2618 2023-07-30 12:36:03.000000 ta-cmi-2.1.1/ta_cmi/cmi_api.py
+-rw-rw-rw-   0 root         (0) root         (0)      509 2023-07-30 12:36:03.000000 ta-cmi-2.1.1/ta_cmi/cmi_channel.py
+-rw-rw-rw-   0 root         (0) root         (0)     2394 2023-07-30 12:36:03.000000 ta-cmi-2.1.1/ta_cmi/coe.py
+-rw-rw-rw-   0 root         (0) root         (0)     4371 2023-07-30 12:36:03.000000 ta-cmi-2.1.1/ta_cmi/coe_api.py
+-rw-rw-rw-   0 root         (0) root         (0)      393 2023-07-30 12:36:03.000000 ta-cmi-2.1.1/ta_cmi/coe_channel.py
+-rw-rw-rw-   0 root         (0) root         (0)     3514 2023-07-30 12:36:03.000000 ta-cmi-2.1.1/ta_cmi/const.py
+-rw-rw-rw-   0 root         (0) root         (0)     4341 2023-07-30 12:36:03.000000 ta-cmi-2.1.1/ta_cmi/device.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 12:36:16.175466 ta-cmi-2.1.1/ta_cmi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8082 2023-07-30 12:36:16.000000 ta-cmi-2.1.1/ta_cmi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      367 2023-07-30 12:36:16.000000 ta-cmi-2.1.1/ta_cmi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-30 12:36:16.000000 ta-cmi-2.1.1/ta_cmi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-30 12:36:16.000000 ta-cmi-2.1.1/ta_cmi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-30 12:36:16.000000 ta-cmi-2.1.1/ta_cmi.egg-info/top_level.txt
```

### Comparing `ta-cmi-2.1.0/LICENSE` & `ta-cmi-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ta-cmi-2.1.0/PKG-INFO` & `ta-cmi-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ta-cmi
-Version: 2.1.0
+Version: 2.1.1
 Summary: A Python wrapper to read out  sensors from Technische Alternative using the C.M.I.
 Home-page: https://gitlab.com/DeerMaximum/ta-cmi
 Author: DeerMaximum
 Author-email: 2629822-DeerMaximum@users.noreply.gitlab.com
 License: MIT License
         
         Copyright (c) 2021 DeerMaximum
```

### Comparing `ta-cmi-2.1.0/README.md` & `ta-cmi-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ta-cmi-2.1.0/setup.py` & `ta-cmi-2.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     readme = f.read()
 
 with open("LICENSE", "r", encoding="utf8") as f:
     license = f.read()
 
 setup(
     name="ta-cmi",
-    version="2.1.0",
+    version="2.1.1",
     description="A Python wrapper to read out  sensors from Technische Alternative using the C.M.I.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/DeerMaximum/ta-cmi",
     author="DeerMaximum",
     author_email="2629822-DeerMaximum@users.noreply.gitlab.com",
     license=license,
```

### Comparing `ta-cmi-2.1.0/ta_cmi/api.py` & `ta-cmi-2.1.1/ta_cmi/api.py`

 * *Files identical despite different names*

### Comparing `ta-cmi-2.1.0/ta_cmi/channel.py` & `ta-cmi-2.1.1/ta_cmi/channel.py`

 * *Files identical despite different names*

### Comparing `ta-cmi-2.1.0/ta_cmi/cmi.py` & `ta-cmi-2.1.1/ta_cmi/cmi.py`

 * *Files identical despite different names*

### Comparing `ta-cmi-2.1.0/ta_cmi/cmi_api.py` & `ta-cmi-2.1.1/ta_cmi/cmi_api.py`

 * *Files identical despite different names*

### Comparing `ta-cmi-2.1.0/ta_cmi/coe.py` & `ta-cmi-2.1.1/ta_cmi/coe.py`

 * *Files identical despite different names*

### Comparing `ta-cmi-2.1.0/ta_cmi/coe_api.py` & `ta-cmi-2.1.1/ta_cmi/coe_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,31 +22,33 @@
         """Initialize."""
         super().__init__(session)
 
         self.host = host
 
     async def get_coe_data(self) -> Dict[str, Any] | None:
         """Get the CoE data."""
-        _LOGGER.debug("Receive data from CoE server")
-
         url = f"{self.host}{self.COE_DATA}"
+
+        _LOGGER.debug("Receive data from CoE server: %s", url)
+
         data = await self._make_request_get(url)
 
         _LOGGER.debug("Received data from CoE server: %s", data)
 
         if len(data) == 0:
             return None
 
         return data
 
     async def get_coe_version(self) -> str | None:
         """Get the version of the CoE server."""
-        _LOGGER.debug("Receive current version from CoE server")
-
         url = f"{self.host}{self.COE_DATA}"
+
+        _LOGGER.debug("Receive current version from CoE server: %s", url)
+
         data = await self._make_request_get(url)
 
         _LOGGER.debug("Received version from CoE server: %s", data)
 
         if len(data) == 0:
             return None
```

### Comparing `ta-cmi-2.1.0/ta_cmi/const.py` & `ta-cmi-2.1.1/ta_cmi/const.py`

 * *Files identical despite different names*

### Comparing `ta-cmi-2.1.0/ta_cmi/device.py` & `ta-cmi-2.1.1/ta_cmi/device.py`

 * *Files identical despite different names*

### Comparing `ta-cmi-2.1.0/ta_cmi.egg-info/PKG-INFO` & `ta-cmi-2.1.1/ta_cmi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ta-cmi
-Version: 2.1.0
+Version: 2.1.1
 Summary: A Python wrapper to read out  sensors from Technische Alternative using the C.M.I.
 Home-page: https://gitlab.com/DeerMaximum/ta-cmi
 Author: DeerMaximum
 Author-email: 2629822-DeerMaximum@users.noreply.gitlab.com
 License: MIT License
         
         Copyright (c) 2021 DeerMaximum
```

