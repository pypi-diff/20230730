# Comparing `tmp/py_ecowater-0.1.2.tar.gz` & `tmp/py_ecowater-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ecowater-0.1.2.tar", last modified: Sat Jul 29 20:37:06 2023, max compression
+gzip compressed data, was "py_ecowater-0.1.3.tar", last modified: Sun Jul 30 16:32:11 2023, max compression
```

## Comparing `py_ecowater-0.1.2.tar` & `py_ecowater-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 dbunker    (501) staff       (20)        0 2023-07-29 20:37:06.456256 py_ecowater-0.1.2/
--rw-r--r--   0 dbunker    (501) staff       (20)     1071 2023-07-29 15:30:43.000000 py_ecowater-0.1.2/LICENSE
--rw-r--r--   0 dbunker    (501) staff       (20)     6757 2023-07-29 20:37:06.456308 py_ecowater-0.1.2/PKG-INFO
--rw-r--r--   0 dbunker    (501) staff       (20)     6233 2023-07-29 20:29:59.000000 py_ecowater-0.1.2/README.md
--rw-r--r--   0 dbunker    (501) staff       (20)        5 2023-07-29 20:29:59.000000 py_ecowater-0.1.2/VERSION.txt
--rw-r--r--   0 dbunker    (501) staff       (20)       85 2022-05-29 21:43:28.000000 py_ecowater-0.1.2/pyproject.toml
--rw-r--r--   0 dbunker    (501) staff       (20)      661 2023-07-29 20:37:06.456553 py_ecowater-0.1.2/setup.cfg
-drwxr-xr-x   0 dbunker    (501) staff       (20)        0 2023-07-29 20:37:06.453473 py_ecowater-0.1.2/src/
-drwxr-xr-x   0 dbunker    (501) staff       (20)        0 2023-07-29 20:37:06.455413 py_ecowater-0.1.2/src/py_ecowater/
--rw-r--r--   0 dbunker    (501) staff       (20)      101 2023-07-29 20:29:59.000000 py_ecowater-0.1.2/src/py_ecowater/__init__.py
--rw-r--r--   0 dbunker    (501) staff       (20)      875 2022-06-05 22:39:36.000000 py_ecowater-0.1.2/src/py_ecowater/constants.py
--rw-r--r--   0 dbunker    (501) staff       (20)     4641 2023-07-29 20:29:59.000000 py_ecowater-0.1.2/src/py_ecowater/ecowater_client.py
--rw-r--r--   0 dbunker    (501) staff       (20)        0 2022-06-03 02:53:26.000000 py_ecowater-0.1.2/src/py_ecowater/exception.py
--rw-r--r--   0 dbunker    (501) staff       (20)    27962 2023-07-29 20:29:59.000000 py_ecowater-0.1.2/src/py_ecowater/model.py
-drwxr-xr-x   0 dbunker    (501) staff       (20)        0 2023-07-29 20:37:06.456135 py_ecowater-0.1.2/src/py_ecowater.egg-info/
--rw-r--r--   0 dbunker    (501) staff       (20)     6757 2023-07-29 20:37:06.000000 py_ecowater-0.1.2/src/py_ecowater.egg-info/PKG-INFO
--rw-r--r--   0 dbunker    (501) staff       (20)      356 2023-07-29 20:37:06.000000 py_ecowater-0.1.2/src/py_ecowater.egg-info/SOURCES.txt
--rw-r--r--   0 dbunker    (501) staff       (20)        1 2023-07-29 20:37:06.000000 py_ecowater-0.1.2/src/py_ecowater.egg-info/dependency_links.txt
--rw-r--r--   0 dbunker    (501) staff       (20)       12 2023-07-29 20:37:06.000000 py_ecowater-0.1.2/src/py_ecowater.egg-info/top_level.txt
+drwxr-xr-x   0 dbunker    (501) staff       (20)        0 2023-07-30 16:32:11.765056 py_ecowater-0.1.3/
+-rw-r--r--   0 dbunker    (501) staff       (20)     1071 2023-07-29 15:30:43.000000 py_ecowater-0.1.3/LICENSE
+-rw-r--r--   0 dbunker    (501) staff       (20)     6757 2023-07-30 16:32:11.765115 py_ecowater-0.1.3/PKG-INFO
+-rw-r--r--   0 dbunker    (501) staff       (20)     6233 2023-07-30 16:31:29.000000 py_ecowater-0.1.3/README.md
+-rw-r--r--   0 dbunker    (501) staff       (20)        5 2023-07-30 16:31:29.000000 py_ecowater-0.1.3/VERSION.txt
+-rw-r--r--   0 dbunker    (501) staff       (20)       85 2022-05-29 21:43:28.000000 py_ecowater-0.1.3/pyproject.toml
+-rw-r--r--   0 dbunker    (501) staff       (20)      661 2023-07-30 16:32:11.765364 py_ecowater-0.1.3/setup.cfg
+drwxr-xr-x   0 dbunker    (501) staff       (20)        0 2023-07-30 16:32:11.762237 py_ecowater-0.1.3/src/
+drwxr-xr-x   0 dbunker    (501) staff       (20)        0 2023-07-30 16:32:11.764079 py_ecowater-0.1.3/src/py_ecowater/
+-rw-r--r--   0 dbunker    (501) staff       (20)      101 2023-07-29 20:29:59.000000 py_ecowater-0.1.3/src/py_ecowater/__init__.py
+-rw-r--r--   0 dbunker    (501) staff       (20)      920 2023-07-30 16:31:29.000000 py_ecowater-0.1.3/src/py_ecowater/constants.py
+-rw-r--r--   0 dbunker    (501) staff       (20)     4956 2023-07-30 16:31:29.000000 py_ecowater-0.1.3/src/py_ecowater/ecowater_client.py
+-rw-r--r--   0 dbunker    (501) staff       (20)        0 2022-06-03 02:53:26.000000 py_ecowater-0.1.3/src/py_ecowater/exception.py
+-rw-r--r--   0 dbunker    (501) staff       (20)    27962 2023-07-29 20:29:59.000000 py_ecowater-0.1.3/src/py_ecowater/model.py
+drwxr-xr-x   0 dbunker    (501) staff       (20)        0 2023-07-30 16:32:11.764953 py_ecowater-0.1.3/src/py_ecowater.egg-info/
+-rw-r--r--   0 dbunker    (501) staff       (20)     6757 2023-07-30 16:32:11.000000 py_ecowater-0.1.3/src/py_ecowater.egg-info/PKG-INFO
+-rw-r--r--   0 dbunker    (501) staff       (20)      356 2023-07-30 16:32:11.000000 py_ecowater-0.1.3/src/py_ecowater.egg-info/SOURCES.txt
+-rw-r--r--   0 dbunker    (501) staff       (20)        1 2023-07-30 16:32:11.000000 py_ecowater-0.1.3/src/py_ecowater.egg-info/dependency_links.txt
+-rw-r--r--   0 dbunker    (501) staff       (20)       12 2023-07-30 16:32:11.000000 py_ecowater-0.1.3/src/py_ecowater.egg-info/top_level.txt
```

### Comparing `py_ecowater-0.1.2/LICENSE` & `py_ecowater-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ecowater-0.1.2/PKG-INFO` & `py_ecowater-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: py_ecowater
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python package for interacting with the Ecowater API
 Home-page: https://github.com/ejsuncy/py_ecowater
 Author: Dan Bunker
 Author-email: dbunked@gmail.com
 Project-URL: Bug Tracker, https://github.com/ejsuncy/py_ecowater/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # py_ecowater
-![Current Version](https://img.shields.io/badge/Version-0.1.2-brightgreen)
+![Current Version](https://img.shields.io/badge/Version-0.1.3-brightgreen)
 
 A python library for getting device data from Ecowater API for devices such as the Rheem RHW42 water softener, which 
 provides WI-FI connectivity via the iQua app.
 
 ## Installation
 
 ```bash
```

### Comparing `py_ecowater-0.1.2/README.md` & `py_ecowater-0.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # py_ecowater
-![Current Version](https://img.shields.io/badge/Version-0.1.2-brightgreen)
+![Current Version](https://img.shields.io/badge/Version-0.1.3-brightgreen)
 
 A python library for getting device data from Ecowater API for devices such as the Rheem RHW42 water softener, which 
 provides WI-FI connectivity via the iQua app.
 
 ## Installation
 
 ```bash
```

### Comparing `py_ecowater-0.1.2/setup.cfg` & `py_ecowater-0.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `py_ecowater-0.1.2/src/py_ecowater/constants.py` & `py_ecowater-0.1.3/src/py_ecowater/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,7 +17,8 @@
     def __init__(self, host=ECOWATER_HOST):
         self.host = host if host else ECOWATER_HOST
         self.uri_base = f"https://{self.host}/"
         self.headers_api = ECOWATER_HEADERS.copy()
         self.headers_api["host"] = self.host
         self.headers_auth = ECOWATER_HEADERS.copy()
         self.headers_auth["content-type"] = "application/json;charset=utf-8"
+        self.auth_expiry_buffer_minutes = 10
```

### Comparing `py_ecowater-0.1.2/src/py_ecowater/ecowater_client.py` & `py_ecowater-0.1.3/src/py_ecowater/ecowater_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,16 +17,18 @@
         self.auth_token: str = ""
         self.auth_expiration: Optional[datetime.datetime] = None
         self.devices: Optional[Devices] = None
         self.ecowater_constants: EcowaterConstants = EcowaterConstants(host)
 
     def __authenticate(self) -> bool:
         if self.auth_token and self.auth_expiration:
-            if datetime.datetime.now() + datetime.timedelta(days=10) > self.auth_expiration:
-                self.logger.info("The Auth token expires within 10 days, need to refresh")
+            auth_minutes_remaining = (self.auth_expiration - datetime.datetime.now()).total_seconds() / 60
+            if datetime.datetime.now() + datetime.timedelta(minutes=self.ecowater_constants.auth_expiry_buffer_minutes) > self.auth_expiration:
+                self.logger.info(f"The Auth token expires in {auth_minutes_remaining} min, which shorter than the "
+                                 f"configured buffer of {self.ecowater_constants.auth_expiry_buffer_minutes} min, need to refresh")
                 self.auth_token = ""
                 self.auth_expiration = None
             else:
                 return True
         else:
             self.logger.info("Using credentials to fetch auth token")
```

### Comparing `py_ecowater-0.1.2/src/py_ecowater/model.py` & `py_ecowater-0.1.3/src/py_ecowater/model.py`

 * *Files identical despite different names*

### Comparing `py_ecowater-0.1.2/src/py_ecowater.egg-info/PKG-INFO` & `py_ecowater-0.1.3/src/py_ecowater.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: py-ecowater
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python package for interacting with the Ecowater API
 Home-page: https://github.com/ejsuncy/py_ecowater
 Author: Dan Bunker
 Author-email: dbunked@gmail.com
 Project-URL: Bug Tracker, https://github.com/ejsuncy/py_ecowater/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # py_ecowater
-![Current Version](https://img.shields.io/badge/Version-0.1.2-brightgreen)
+![Current Version](https://img.shields.io/badge/Version-0.1.3-brightgreen)
 
 A python library for getting device data from Ecowater API for devices such as the Rheem RHW42 water softener, which 
 provides WI-FI connectivity via the iQua app.
 
 ## Installation
 
 ```bash
```

