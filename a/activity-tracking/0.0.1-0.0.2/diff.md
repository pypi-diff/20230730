# Comparing `tmp/activity-tracking-0.0.1.tar.gz` & `tmp/activity-tracking-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "activity-tracking-0.0.1.tar", max compression
+gzip compressed data, was "activity-tracking-0.0.2.tar", max compression
```

## Comparing `activity-tracking-0.0.1.tar` & `activity-tracking-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-07-27 16:29:23.467123 activity-tracking-0.0.1/CHANGELOG.md
--rw-r--r--   0        0        0     1491 2023-07-27 16:15:47.125260 activity-tracking-0.0.1/LICENSE
--rw-r--r--   0        0        0      380 2023-07-27 15:33:49.544968 activity-tracking-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-07-26 17:31:11.002266 activity-tracking-0.0.1/activity_tracking/__init__.py
--rw-r--r--   0        0        0     5337 2023-07-27 16:28:52.342890 activity-tracking-0.0.1/activity_tracking/functions.py
--rw-r--r--   0        0        0      671 2023-07-28 05:53:00.344144 activity-tracking-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1007 2023-07-28 05:53:22.551554 activity-tracking-0.0.1/setup.py
--rw-r--r--   0        0        0     1058 2023-07-28 05:53:22.551793 activity-tracking-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-27 16:29:23.467123 activity-tracking-0.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1491 2023-07-27 16:15:47.125260 activity-tracking-0.0.2/LICENSE
+-rw-r--r--   0        0        0      700 2023-07-28 06:12:08.041569 activity-tracking-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-26 17:31:11.002266 activity-tracking-0.0.2/activity_tracking/__init__.py
+-rw-r--r--   0        0        0     5392 2023-07-30 04:55:49.973387 activity-tracking-0.0.2/activity_tracking/trackers.py
+-rw-r--r--   0        0        0      671 2023-07-30 05:18:23.473942 activity-tracking-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1344 2023-07-30 05:19:04.148340 activity-tracking-0.0.2/setup.py
+-rw-r--r--   0        0        0     1378 2023-07-30 05:19:04.148724 activity-tracking-0.0.2/PKG-INFO
```

### Comparing `activity-tracking-0.0.1/LICENSE` & `activity-tracking-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `activity-tracking-0.0.1/activity_tracking/functions.py` & `activity-tracking-0.0.2/activity_tracking/trackers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,36 @@
-import platform
+import csv
 import ctypes
 import logging
-import csv
-import subprocess
 import os
+import platform
+import subprocess
 
 logger = logging.getLogger()
 """This library inherits the logger of the importing library"""
 
 if platform.system() == "Windows":
-    # ctypes handles the Windows-specific functions
-    from ctypes import wintypes, windll, create_unicode_buffer, byref
+    """ ctypes handles the Windows-specific functions """
+    from ctypes import byref, create_unicode_buffer, windll, wintypes
+
 
 class LASTINPUTINFO(ctypes.Structure):
     # Special class for storing lastinputinfo data from windows
     _fields_ = [("cbSize", ctypes.c_ulong), ("dwTime", ctypes.c_ulong)]
 
-def getForegroundWindow(userOS=platform.system()):
-    # Get window name of current foreground window
-    # RETURNS: str name of window
 
-    window, _ = getForegroundWindow(userOS)
+def getForegroundWindow(userOS=platform.system()):
+    """
+    Get window name of current foreground window
+    RETURNS: str name of window
+    """
+    window, _ = getForegroundWindowProcess(userOS)
     return window
 
+
 def getForegroundWindowProcess(userOS=platform.system()):
     """ Get window name and process name of current foreground window
      Makes use of windows API
      RETURNS: [str name of window, str name of process]
     """
     if userOS == "Windows":
         # Get the unique window ID of the foreground window
@@ -53,15 +57,15 @@
         windll.user32.GetWindowThreadProcessId(windowId, byref(pid))
 
         # Run command 'tasklist', lookup which program has the pid
         # and store CSV output to var
         # TODO: try psutil?
         tasklist = os.popen(
             f'tasklist /FI \
-						"pid eq {pid.value}" /FO CSV'
+            "pid eq {pid.value}" /FO CSV'
         )
 
         processNameCSV = tasklist.read()
         tasklist.close()
 
         # Returns a csv reader object
         readCSV = csv.reader(processNameCSV)
@@ -102,26 +106,27 @@
 
         windowName = result.stdout.strip("\n")
         return windowName, processName
 
     logger.error("OS is Unknown: %s", userOS)
     raise Exception("OS is Unknown: %s", userOS)
 
+
 def isUserActive(userOS=platform.system(), minGap=800):
     """
     Compares gap between last time of input from mouse or kb and current time.
     ARGS:
-    	lastInputInfo -> Instance of class LASTINPUTINFO(ctypes.Structure),
-    	minGap -> Int, minimum time between activity in mseconds
-    	userOS -> string, the platform the user is using ["Windows", "Linux"]
+        lastInputInfo -> Instance of class LASTINPUTINFO(ctypes.Structure),
+        minGap -> Int, minimum time between activity in mseconds
+        userOS -> string, the platform the user is using ["Windows", "Linux"]
     Returns:
       True if the user made an input during `minGap`, else False
     """
 
-    ### TODO: Fix minGap linux implementation.
+    # TODO: Fix minGap linux implementation.
 
     # Store last input time to class
     if userOS == "Windows":
 
         lastInputInfo = LASTINPUTINFO()
         lastInputInfo.cbSize = ctypes.sizeof(LASTINPUTINFO)
 
@@ -131,19 +136,21 @@
         currentTime = windll.kernel32.GetTickCount()
 
         timeGap = currentTime - lastInputTime
 
         return timeGap <= minGap
 
     if userOS == "Linux":
-        # Returns: 234324.2 234234.3
-        # See proc man page for /proc/uptime
-        # result = subprocess.run(["cat", "/proc/uptime"], capture_output=True, text=True)
-        # Get first item only
-        # currentTimeMs = float(result.stdout.split(" ")[0]) * 1000
+        """
+        Returns: 234323.2 234234.3
+        See proc man page for /proc/uptime
+        result = subprocess.run(["cat", "/proc/uptime"], capture_output=True, text=True)
+        Get first item only
+        currentTimeMs = float(result.stdout.split(" ")[0]) * 1000
+        """
 
         result = subprocess.run(
             # Implementation depends on this command:
             # timeout .1 xinput test-xi2 --root
             # If an input is made, EVENT is present.
             # timeout should be < mingap
             ["timeout", str((minGap / 1000) / 2), "xinput", "test-xi2", "--root"],
```

### Comparing `activity-tracking-0.0.1/pyproject.toml` & `activity-tracking-0.0.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "activity-tracking"
-version = "0.0.1"
+version = "0.0.2"
 description = "Utility functions for desktop activity tracking"
 authors = ["elpachongco <earlsiachongco@gmail.com>"]
 readme="README.md"
 packages = [{include = "activity_tracking"}]
 license = "BSD-3-Clause "
 homepage = "https://github.com/elpachongco/activity-tracking-lib"
 repository = "https://github.com/elpachongco/activity-tracking-lib"
```

### Comparing `activity-tracking-0.0.1/setup.py` & `activity-tracking-0.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['activity_tracking']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'activity-tracking',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': 'Utility functions for desktop activity tracking',
-    'long_description': '# activity tracking library\n\nThis library contains utility functions for recording desktop activity on windows and linux\n\nI created this for my productivity tool [Activity Monitor](https://github.com/elpachongco/activity-monitor)\n\n## Features \n- Cross platform [windows, linux(ubuntu, X window system)]\n\n## Functions \n\n- Get foreground window name, process, pid\n- is user active\n\n',
+    'long_description': '# Activity tracking library\n\nThis library contains utility functions for recording desktop activity on windows and linux\n\nI created this for my productivity tool [Activity Monitor](https://github.com/elpachongco/activity-monitor)\n\n## Features \n- Cross platform [windows, linux(ubuntu, X window system)]\n\n## Functions \n\n- Get foreground window name, process, pid\n- is user active\n\n## Installation\n\nThis library is now available on the python package index.\n\nVisit the [pypi page](https://pypi.org/project/activity-tracking/).\n\n```bash\npip install activity-tracking\n```\n\nor with python-poetry\n\n```bash\npoetry add activity-tracking\n```\n\nPlease note that this software is in early stage of development. \n',
     'author': 'elpachongco',
     'author_email': 'earlsiachongco@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/elpachongco/activity-tracking-lib',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `activity-tracking-0.0.1/PKG-INFO` & `activity-tracking-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: activity-tracking
-Version: 0.0.1
+Version: 0.0.2
 Summary: Utility functions for desktop activity tracking
 Home-page: https://github.com/elpachongco/activity-tracking-lib
 License: BSD-3-Clause 
 Keywords: desktop
 Author: elpachongco
 Author-email: earlsiachongco@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -12,22 +12,39 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Project-URL: Repository, https://github.com/elpachongco/activity-tracking-lib
 Description-Content-Type: text/markdown
 
-# activity tracking library
+# Activity tracking library
 
 This library contains utility functions for recording desktop activity on windows and linux
 
 I created this for my productivity tool [Activity Monitor](https://github.com/elpachongco/activity-monitor)
 
 ## Features 
 - Cross platform [windows, linux(ubuntu, X window system)]
 
 ## Functions 
 
 - Get foreground window name, process, pid
 - is user active
 
+## Installation
+
+This library is now available on the python package index.
+
+Visit the [pypi page](https://pypi.org/project/activity-tracking/).
+
+```bash
+pip install activity-tracking
+```
+
+or with python-poetry
+
+```bash
+poetry add activity-tracking
+```
+
+Please note that this software is in early stage of development.
```

