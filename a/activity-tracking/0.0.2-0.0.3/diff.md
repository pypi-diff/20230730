# Comparing `tmp/activity-tracking-0.0.2.tar.gz` & `tmp/activity-tracking-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "activity-tracking-0.0.2.tar", max compression
+gzip compressed data, was "activity-tracking-0.0.3.tar", max compression
```

## Comparing `activity-tracking-0.0.2.tar` & `activity-tracking-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-07-27 16:29:23.467123 activity-tracking-0.0.2/CHANGELOG.md
--rw-r--r--   0        0        0     1491 2023-07-27 16:15:47.125260 activity-tracking-0.0.2/LICENSE
--rw-r--r--   0        0        0      700 2023-07-28 06:12:08.041569 activity-tracking-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-07-26 17:31:11.002266 activity-tracking-0.0.2/activity_tracking/__init__.py
--rw-r--r--   0        0        0     5392 2023-07-30 04:55:49.973387 activity-tracking-0.0.2/activity_tracking/trackers.py
--rw-r--r--   0        0        0      671 2023-07-30 05:18:23.473942 activity-tracking-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1344 2023-07-30 05:19:04.148340 activity-tracking-0.0.2/setup.py
--rw-r--r--   0        0        0     1378 2023-07-30 05:19:04.148724 activity-tracking-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-27 16:29:23.467123 activity-tracking-0.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1491 2023-07-27 16:15:47.125260 activity-tracking-0.0.3/LICENSE
+-rw-r--r--   0        0        0      867 2023-07-30 07:52:44.446756 activity-tracking-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-26 17:31:11.002266 activity-tracking-0.0.3/activity_tracking/__init__.py
+-rw-r--r--   0        0        0     4301 2023-07-30 07:30:50.783458 activity-tracking-0.0.3/activity_tracking/trackers.py
+-rw-r--r--   0        0        0      689 2023-07-30 07:56:49.342166 activity-tracking-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1615 2023-07-30 07:59:30.881410 activity-tracking-0.0.3/setup.py
+-rw-r--r--   0        0        0     1584 2023-07-30 07:59:30.881678 activity-tracking-0.0.3/PKG-INFO
```

### Comparing `activity-tracking-0.0.2/LICENSE` & `activity-tracking-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `activity-tracking-0.0.2/README.md` & `activity-tracking-0.0.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -5,16 +5,31 @@
 I created this for my productivity tool [Activity Monitor](https://github.com/elpachongco/activity-monitor)
 
 ## Features 
 - Cross platform [windows, linux(ubuntu, X window system)]
 
 ## Functions 
 
-- Get foreground window name, process, pid
-- is user active
+### Get foreground window name, process, pid
+
+```python3
+>>> getForegroundWindow()
+('New Tab`, 2500)
+
+>>> import psutil
+>>> psutil.Process(2500).name()
+'chrome.exe'
+```
+
+### isUserActive
+
+```python3
+>>> isUserActive()
+True
+```
 
 ## Installation
 
 This library is now available on the python package index.
 
 Visit the [pypi page](https://pypi.org/project/activity-tracking/).
```

### Comparing `activity-tracking-0.0.2/activity_tracking/trackers.py` & `activity-tracking-0.0.3/activity_tracking/trackers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-import csv
 import ctypes
 import logging
-import os
 import platform
 import subprocess
 
 logger = logging.getLogger()
 """This library inherits the logger of the importing library"""
 
 if platform.system() == "Windows":
@@ -15,26 +13,17 @@
 
 class LASTINPUTINFO(ctypes.Structure):
     # Special class for storing lastinputinfo data from windows
     _fields_ = [("cbSize", ctypes.c_ulong), ("dwTime", ctypes.c_ulong)]
 
 
 def getForegroundWindow(userOS=platform.system()):
-    """
-    Get window name of current foreground window
-    RETURNS: str name of window
-    """
-    window, _ = getForegroundWindowProcess(userOS)
-    return window
-
-
-def getForegroundWindowProcess(userOS=platform.system()):
     """ Get window name and process name of current foreground window
      Makes use of windows API
-     RETURNS: [str name of window, str name of process]
+     RETURNS: (str name of window, pid of window)
     """
     if userOS == "Windows":
         # Get the unique window ID of the foreground window
         windowId = windll.user32.GetForegroundWindow()
 
         # get title length of the window id (windowId)
         titleLength = windll.user32.GetWindowTextLengthW(windowId)
@@ -52,64 +41,38 @@
         # foreground window
         pid = wintypes.DWORD()
 
         # Get process id of the given window ID (arg 1) and store it to
         # pid variable
         windll.user32.GetWindowThreadProcessId(windowId, byref(pid))
 
-        # Run command 'tasklist', lookup which program has the pid
-        # and store CSV output to var
-        # TODO: try psutil?
-        tasklist = os.popen(
-            f'tasklist /FI \
-            "pid eq {pid.value}" /FO CSV'
-        )
-
-        processNameCSV = tasklist.read()
-        tasklist.close()
-
-        # Returns a csv reader object
-        readCSV = csv.reader(processNameCSV)
-        listCSV = list(readCSV)
-
-        # Position of the program name in the list
-        # I wouldn't consider this portable so this might change.
-        exeName = listCSV[10][0]
-
         # Return the window name, & process name running the window.
-        return titleBuffer.value, exeName
+        return titleBuffer.value, pid.value
 
     if userOS == "Linux":
         result = subprocess.run(
             ["timeout", "1", "xdotool", "getwindowfocus", "getwindowpid"],
             capture_output=True,
             text=True,
         )
 
         # pid is blank if no window is focused.
         if result.stdout == "":
             return "", ""
 
-        proc = int(result.stdout)
-
-        result = subprocess.run(
-            ["timeout", "1", "ps", "-p", str(proc), "-o", "comm="],
-            capture_output=True,
-            text=True,
-        )
-        processName = result.stdout.strip("\n")
+        pid = int(result.stdout)
 
         result = subprocess.run(
             ["timeout", "1", "xdotool", "getwindowfocus", "getwindowname"],
             capture_output=True,
             text=True,
         )
 
         windowName = result.stdout.strip("\n")
-        return windowName, processName
+        return windowName, pid
 
     logger.error("OS is Unknown: %s", userOS)
     raise Exception("OS is Unknown: %s", userOS)
 
 
 def isUserActive(userOS=platform.system(), minGap=800):
     """
@@ -120,15 +83,14 @@
         userOS -> string, the platform the user is using ["Windows", "Linux"]
     Returns:
       True if the user made an input during `minGap`, else False
     """
 
     # TODO: Fix minGap linux implementation.
 
-    # Store last input time to class
     if userOS == "Windows":
 
         lastInputInfo = LASTINPUTINFO()
         lastInputInfo.cbSize = ctypes.sizeof(LASTINPUTINFO)
 
         windll.user32.GetLastInputInfo(byref(lastInputInfo))
         lastInputTime = lastInputInfo.dwTime
```

### Comparing `activity-tracking-0.0.2/pyproject.toml` & `activity-tracking-0.0.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "activity-tracking"
-version = "0.0.2"
+version = "0.0.3"
 description = "Utility functions for desktop activity tracking"
 authors = ["elpachongco <earlsiachongco@gmail.com>"]
 readme="README.md"
 packages = [{include = "activity_tracking"}]
 license = "BSD-3-Clause "
 homepage = "https://github.com/elpachongco/activity-tracking-lib"
 repository = "https://github.com/elpachongco/activity-tracking-lib"
 documentation = ""
 keywords = ["desktop"]
 classifiers = []
 include = ["CHANGELOG.md"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
+psutil = "^5.9.5"
 
 [tool.poetry.dev-dependencies]
 pdoc = "^14.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `activity-tracking-0.0.2/setup.py` & `activity-tracking-0.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,24 +3,28 @@
 
 packages = \
 ['activity_tracking']
 
 package_data = \
 {'': ['*']}
 
+install_requires = \
+['psutil>=5.9.5,<6.0.0']
+
 setup_kwargs = {
     'name': 'activity-tracking',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': 'Utility functions for desktop activity tracking',
-    'long_description': '# Activity tracking library\n\nThis library contains utility functions for recording desktop activity on windows and linux\n\nI created this for my productivity tool [Activity Monitor](https://github.com/elpachongco/activity-monitor)\n\n## Features \n- Cross platform [windows, linux(ubuntu, X window system)]\n\n## Functions \n\n- Get foreground window name, process, pid\n- is user active\n\n## Installation\n\nThis library is now available on the python package index.\n\nVisit the [pypi page](https://pypi.org/project/activity-tracking/).\n\n```bash\npip install activity-tracking\n```\n\nor with python-poetry\n\n```bash\npoetry add activity-tracking\n```\n\nPlease note that this software is in early stage of development. \n',
+    'long_description': "# Activity tracking library\n\nThis library contains utility functions for recording desktop activity on windows and linux\n\nI created this for my productivity tool [Activity Monitor](https://github.com/elpachongco/activity-monitor)\n\n## Features \n- Cross platform [windows, linux(ubuntu, X window system)]\n\n## Functions \n\n### Get foreground window name, process, pid\n\n```python3\n>>> getForegroundWindow()\n('New Tab`, 2500)\n\n>>> import psutil\n>>> psutil.Process(2500).name()\n'chrome.exe'\n```\n\n### isUserActive\n\n```python3\n>>> isUserActive()\nTrue\n```\n\n## Installation\n\nThis library is now available on the python package index.\n\nVisit the [pypi page](https://pypi.org/project/activity-tracking/).\n\n```bash\npip install activity-tracking\n```\n\nor with python-poetry\n\n```bash\npoetry add activity-tracking\n```\n\nPlease note that this software is in early stage of development. \n",
     'author': 'elpachongco',
     'author_email': 'earlsiachongco@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/elpachongco/activity-tracking-lib',
     'packages': packages,
     'package_data': package_data,
+    'install_requires': install_requires,
     'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `activity-tracking-0.0.2/PKG-INFO` & `activity-tracking-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,54 @@
 Metadata-Version: 2.1
 Name: activity-tracking
-Version: 0.0.2
+Version: 0.0.3
 Summary: Utility functions for desktop activity tracking
 Home-page: https://github.com/elpachongco/activity-tracking-lib
 License: BSD-3-Clause 
 Keywords: desktop
 Author: elpachongco
 Author-email: earlsiachongco@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Project-URL: Repository, https://github.com/elpachongco/activity-tracking-lib
 Description-Content-Type: text/markdown
 
 # Activity tracking library
 
 This library contains utility functions for recording desktop activity on windows and linux
 
 I created this for my productivity tool [Activity Monitor](https://github.com/elpachongco/activity-monitor)
 
 ## Features 
 - Cross platform [windows, linux(ubuntu, X window system)]
 
 ## Functions 
 
-- Get foreground window name, process, pid
-- is user active
+### Get foreground window name, process, pid
+
+```python3
+>>> getForegroundWindow()
+('New Tab`, 2500)
+
+>>> import psutil
+>>> psutil.Process(2500).name()
+'chrome.exe'
+```
+
+### isUserActive
+
+```python3
+>>> isUserActive()
+True
+```
 
 ## Installation
 
 This library is now available on the python package index.
 
 Visit the [pypi page](https://pypi.org/project/activity-tracking/).
```

