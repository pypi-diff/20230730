# Comparing `tmp/dobot_utils-1.0.1.tar.gz` & `tmp/dobot-utils-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dobot_utils-1.0.1.tar", last modified: Wed Jul 19 02:20:32 2023, max compression
+gzip compressed data, was "dobot-utils-1.0.3.tar", last modified: Sat Jul 29 23:15:30 2023, max compression
```

## Comparing `dobot_utils-1.0.1.tar` & `dobot-utils-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 neo       (1000) neo       (1000)        0 2023-07-19 02:20:32.939971 dobot_utils-1.0.1/
--rw-rw-r--   0 neo       (1000) neo       (1000)    35149 2023-07-11 06:33:31.000000 dobot_utils-1.0.1/LICENSE
--rw-rw-r--   0 neo       (1000) neo       (1000)      770 2023-07-19 02:20:32.939971 dobot_utils-1.0.1/PKG-INFO
--rw-rw-r--   0 neo       (1000) neo       (1000)      175 2023-07-19 02:13:40.000000 dobot_utils-1.0.1/README.md
--rw-r--r--   0 neo       (1000) neo       (1000)      703 2023-07-19 02:20:08.000000 dobot_utils-1.0.1/pyproject.toml
--rw-rw-r--   0 neo       (1000) neo       (1000)       38 2023-07-19 02:20:32.939971 dobot_utils-1.0.1/setup.cfg
--rw-r--r--   0 neo       (1000) neo       (1000)       68 2023-07-19 02:13:35.000000 dobot_utils-1.0.1/setup.py
-drwxrwxr-x   0 neo       (1000) neo       (1000)        0 2023-07-19 02:20:32.939971 dobot_utils-1.0.1/src/
-drwxrwxr-x   0 neo       (1000) neo       (1000)        0 2023-07-19 02:20:32.939971 dobot_utils-1.0.1/src/dobot_utils/
--rw-r--r--   0 neo       (1000) neo       (1000)        0 2023-07-06 15:15:38.000000 dobot_utils-1.0.1/src/dobot_utils/__init__.py
--rw-rw-r--   0 neo       (1000) neo       (1000)     9435 2023-07-19 02:13:31.000000 dobot_utils-1.0.1/src/dobot_utils/dobot_api.py
--rw-rw-r--   0 neo       (1000) neo       (1000)     4768 2023-07-11 22:32:05.000000 dobot_utils-1.0.1/src/dobot_utils/types.py
--rw-rw-r--   0 neo       (1000) neo       (1000)     1808 2023-07-19 02:13:44.000000 dobot_utils-1.0.1/src/dobot_utils/util.py
-drwxrwxr-x   0 neo       (1000) neo       (1000)        0 2023-07-19 02:20:32.939971 dobot_utils-1.0.1/src/dobot_utils.egg-info/
--rw-rw-r--   0 neo       (1000) neo       (1000)      770 2023-07-19 02:20:32.000000 dobot_utils-1.0.1/src/dobot_utils.egg-info/PKG-INFO
--rw-rw-r--   0 neo       (1000) neo       (1000)      341 2023-07-19 02:20:32.000000 dobot_utils-1.0.1/src/dobot_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 neo       (1000) neo       (1000)        1 2023-07-19 02:20:32.000000 dobot_utils-1.0.1/src/dobot_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 neo       (1000) neo       (1000)       14 2023-07-19 02:20:32.000000 dobot_utils-1.0.1/src/dobot_utils.egg-info/requires.txt
--rw-rw-r--   0 neo       (1000) neo       (1000)       12 2023-07-19 02:20:32.000000 dobot_utils-1.0.1/src/dobot_utils.egg-info/top_level.txt
+drwxrwxr-x   0 neo       (1000) neo       (1000)        0 2023-07-29 23:15:30.709905 dobot-utils-1.0.3/
+-rw-rw-r--   0 neo       (1000) neo       (1000)    35149 2023-07-11 06:33:31.000000 dobot-utils-1.0.3/LICENSE
+-rw-rw-r--   0 neo       (1000) neo       (1000)     1798 2023-07-29 23:15:30.709905 dobot-utils-1.0.3/PKG-INFO
+-rw-rw-r--   0 neo       (1000) neo       (1000)     1203 2023-07-25 07:16:41.000000 dobot-utils-1.0.3/README.md
+-rw-r--r--   0 neo       (1000) neo       (1000)      710 2023-07-29 23:15:22.000000 dobot-utils-1.0.3/pyproject.toml
+-rw-rw-r--   0 neo       (1000) neo       (1000)       38 2023-07-29 23:15:30.709905 dobot-utils-1.0.3/setup.cfg
+-rw-r--r--   0 neo       (1000) neo       (1000)      166 2023-07-29 23:13:10.000000 dobot-utils-1.0.3/setup.py
+drwxrwxr-x   0 neo       (1000) neo       (1000)        0 2023-07-29 23:15:30.705905 dobot-utils-1.0.3/src/
+drwxrwxr-x   0 neo       (1000) neo       (1000)        0 2023-07-29 23:15:30.709905 dobot-utils-1.0.3/src/dobot-utils/
+-rw-rw-r--   0 neo       (1000) neo       (1000)       41 2023-07-29 23:08:00.000000 dobot-utils-1.0.3/src/dobot-utils/__init__.py
+-rw-rw-r--   0 neo       (1000) neo       (1000)     9585 2023-07-29 23:07:03.000000 dobot-utils-1.0.3/src/dobot-utils/dobot_api.py
+-rw-rw-r--   0 neo       (1000) neo       (1000)     4832 2023-07-29 23:13:26.000000 dobot-utils-1.0.3/src/dobot-utils/types.py
+-rw-rw-r--   0 neo       (1000) neo       (1000)     1974 2023-07-29 23:07:33.000000 dobot-utils-1.0.3/src/dobot-utils/util.py
+drwxrwxr-x   0 neo       (1000) neo       (1000)        0 2023-07-29 23:15:30.709905 dobot-utils-1.0.3/src/dobot_utils.egg-info/
+-rw-rw-r--   0 neo       (1000) neo       (1000)     1798 2023-07-29 23:15:30.000000 dobot-utils-1.0.3/src/dobot_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 neo       (1000) neo       (1000)      341 2023-07-29 23:15:30.000000 dobot-utils-1.0.3/src/dobot_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 neo       (1000) neo       (1000)        1 2023-07-29 23:15:30.000000 dobot-utils-1.0.3/src/dobot_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 neo       (1000) neo       (1000)       19 2023-07-29 23:15:30.000000 dobot-utils-1.0.3/src/dobot_utils.egg-info/requires.txt
+-rw-rw-r--   0 neo       (1000) neo       (1000)       12 2023-07-29 23:15:30.000000 dobot-utils-1.0.3/src/dobot_utils.egg-info/top_level.txt
```

### Comparing `dobot_utils-1.0.1/LICENSE` & `dobot-utils-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dobot_utils-1.0.1/pyproject.toml` & `dobot-utils-1.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
-name = "dobot_utils"
-version = "1.0.1"
+name = "dobot-utils"
+version = "1.0.3"
 authors = [{ name = "Calastrophe", email = "vmxoperation@proton.me" }]
 description = "An ergonomic and type-hinted Python API for Dobot Products TCP-IP Protocol"
 readme = "README.md"
 requires-python = ">=3.10"
-dependencies = ['numpy', 'StrEnum']
+dependencies = ['numpy', 'StrEnum', 'ikpy']
 classifiers = [
     "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/Calastrophe/dobot_utils"
-"Bug Tracker" = "https://github.com/Calastrophe/dobot_utils/issues"
+"Homepage" = "https://github.com/Calastrophe/dobot-utils"
+"Bug Tracker" = "https://github.com/Calastrophe/dobot-utils/issues"
```

### Comparing `dobot_utils-1.0.1/src/dobot_utils/dobot_api.py` & `dobot-utils-1.0.3/src/dobot-utils/dobot_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,20 +9,21 @@
 
 # We leave it upon the caller of the API to see if they care about the errors.
 # There should be no error handling inside of this API.
 # This is just a faithful translation and communication layer.
 
 
 class Dobot:
-    def __init__(self, ip: str, is_cr: bool = False, logging: bool = False, log_name: str = "output.log", log_level = log.DEBUG):
+    def __init__(self, ip: str, urdf_file: Optional[URDF] = None, is_cr: bool = False, logging: bool = False, log_name: str = "output.log", log_level = log.DEBUG):
         if logging:
             log.basicConfig(filename=log_name, level=log_level)
-        self.movement = Movement(ip)
-        self.feedback = Feedback(ip)
-        self.dashboard = Dashboard(ip)
+        self.simulator: Optional[Simulator] = Simulator(urdf_file) if urdf_file else None
+        self.movement: Movement = Movement(ip)
+        self.feedback: Feedback = Feedback(ip)
+        self.dashboard: Dashboard = Dashboard(ip)
 
 
 class Movement(DobotSocketConnection):
     def __init__(self, ip: str):
         super().__init__(ip, MOVEMENT_PORT)
 
     # MovJ
@@ -236,8 +237,7 @@
 # TODO: Create a numpy type which houses all needed values
 # NOTE: Different for CR version
    
 class Feedback(DobotSocketConnection):
     def __init__(self, ip: str):
         super().__init__(ip, REALTIME_FEEDBACK_PORT)
     
-
```

### Comparing `dobot_utils-1.0.1/src/dobot_utils/types.py` & `dobot-utils-1.0.3/src/dobot-utils/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,17 @@
     M1PRO = 2
     NOVA2 = 101
     NOVA5 = 103
     CR3V2 = 113
     CR5V2 = 115
     CR10V2 = 120
 
+class URDF(StrEnum):
+    M1PRO = "urdf/m1pro_description.urdf"
+
 FeedbackType = np.dtype([(
     'len',
     np.int64,
 ), (
     'digital_input_bits',
     np.uint64,
 ), (
```

### Comparing `dobot_utils-1.0.1/src/dobot_utils/util.py` & `dobot-utils-1.0.3/src/dobot-utils/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import socket
 import logging as log
+from pathlib import Path
+from ikpy.chain import Chain
 from typing import Optional, Tuple
-from .types import DobotError
+from .types import DobotError, URDF
 
 class DobotSocketConnection:
     def __init__(self, ip: str, port: int):
         self.socket = socket.socket()
         self.socket.settimeout(10.0)
         self.socket.connect((ip, port))
         log.debug("Connection established")
@@ -35,13 +37,17 @@
     def close(self):
         if self.socket:
             self.socket.close()
 
     def __del__(self):
         self.close()
 
+class Simulator:
+    def __init__(self, fn: URDF) -> None:
+        self.chain = Chain.from_urdf_file(fn)
+
         
 def clamp(val: int, local_min: int, local_max: int) -> int:
     log.info(f"{val} was clamped to the range {local_min}, {local_max}")
     return max(local_min, min(val, local_max))
```

