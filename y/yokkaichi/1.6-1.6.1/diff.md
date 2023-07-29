# Comparing `tmp/yokkaichi-1.6.tar.gz` & `tmp/yokkaichi-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yokkaichi-1.6.tar", last modified: Thu Jul 27 00:28:08 2023, max compression
+gzip compressed data, was "yokkaichi-1.6.1.tar", last modified: Sat Jul 29 22:34:27 2023, max compression
```

## Comparing `yokkaichi-1.6.tar` & `yokkaichi-1.6.1.tar`

### file list

```diff
@@ -1,38 +1,44 @@
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-27 00:28:08.093362 yokkaichi-1.6/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1063 2023-04-09 23:36:24.000000 yokkaichi-1.6/LICENSE.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)     3890 2023-07-27 00:28:08.093362 yokkaichi-1.6/PKG-INFO
--rw-r--r--   0 krystian  (1000) krystian  (1000)     3148 2023-07-21 15:44:18.000000 yokkaichi-1.6/README.md
--rw-r--r--   0 krystian  (1000) krystian  (1000)       57 2023-05-24 14:00:39.000000 yokkaichi-1.6/pyproject.toml
--rw-r--r--   0 krystian  (1000) krystian  (1000)       38 2023-07-27 00:28:08.093362 yokkaichi-1.6/setup.cfg
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1665 2023-07-21 15:44:18.000000 yokkaichi-1.6/setup.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-27 00:28:08.090029 yokkaichi-1.6/yokkaichi/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     4709 2023-07-27 00:25:15.000000 yokkaichi-1.6/yokkaichi/Checker.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     7361 2023-07-21 15:44:18.000000 yokkaichi-1.6/yokkaichi/IP2L_Manager.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)      685 2023-07-27 00:25:15.000000 yokkaichi-1.6/yokkaichi/Results.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     3226 2023-07-27 00:25:15.000000 yokkaichi-1.6/yokkaichi/ServerScan.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)       20 2023-07-27 00:26:33.000000 yokkaichi-1.6/yokkaichi/__init__.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     4408 2023-07-27 00:25:15.000000 yokkaichi-1.6/yokkaichi/__main__.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     4749 2023-07-21 15:44:18.000000 yokkaichi-1.6/yokkaichi/config_loader.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-27 00:28:08.093362 yokkaichi-1.6/yokkaichi/constants/
--rw-r--r--   0 krystian  (1000) krystian  (1000)       30 2023-07-15 21:48:34.000000 yokkaichi-1.6/yokkaichi/constants/__init__.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)       69 2023-07-15 21:48:34.000000 yokkaichi-1.6/yokkaichi/constants/_console.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-27 00:28:08.093362 yokkaichi-1.6/yokkaichi/enums/
--rw-r--r--   0 krystian  (1000) krystian  (1000)      178 2023-07-21 15:44:18.000000 yokkaichi-1.6/yokkaichi/enums/_IP2LocDBStatus.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)      151 2023-07-21 15:44:18.000000 yokkaichi-1.6/yokkaichi/enums/_IP2LocManagerUserAnswers.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)      146 2023-07-21 15:44:18.000000 yokkaichi-1.6/yokkaichi/enums/_OfflinePrintingModes.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)       89 2023-07-15 21:48:34.000000 yokkaichi-1.6/yokkaichi/enums/_Platforms.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)      198 2023-07-21 15:44:18.000000 yokkaichi-1.6/yokkaichi/enums/__init__.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)      224 2023-07-21 15:44:18.000000 yokkaichi-1.6/yokkaichi/env_loader.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1155 2023-07-20 01:23:02.000000 yokkaichi-1.6/yokkaichi/port_parser.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-27 00:28:08.093362 yokkaichi-1.6/yokkaichi/structs/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1243 2023-07-21 15:44:18.000000 yokkaichi-1.6/yokkaichi/structs/_CFG.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)      135 2023-07-21 15:44:18.000000 yokkaichi-1.6/yokkaichi/structs/_EnvVariables.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)      275 2023-07-21 15:44:18.000000 yokkaichi-1.6/yokkaichi/structs/_MinecraftServer.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)      108 2023-07-21 15:44:18.000000 yokkaichi-1.6/yokkaichi/structs/__init__.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-27 00:28:08.093362 yokkaichi-1.6/yokkaichi.egg-info/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     3890 2023-07-27 00:28:08.000000 yokkaichi-1.6/yokkaichi.egg-info/PKG-INFO
--rw-r--r--   0 krystian  (1000) krystian  (1000)      829 2023-07-27 00:28:08.000000 yokkaichi-1.6/yokkaichi.egg-info/SOURCES.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)        1 2023-07-27 00:28:08.000000 yokkaichi-1.6/yokkaichi.egg-info/dependency_links.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)       54 2023-07-27 00:28:08.000000 yokkaichi-1.6/yokkaichi.egg-info/entry_points.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)      105 2023-07-27 00:28:08.000000 yokkaichi-1.6/yokkaichi.egg-info/requires.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)       10 2023-07-27 00:28:08.000000 yokkaichi-1.6/yokkaichi.egg-info/top_level.txt
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-29 22:34:27.731218 yokkaichi-1.6.1/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1063 2023-04-09 23:36:24.000000 yokkaichi-1.6.1/LICENSE.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     3892 2023-07-29 22:34:27.731218 yokkaichi-1.6.1/PKG-INFO
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     3148 2023-07-21 15:44:18.000000 yokkaichi-1.6.1/README.md
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       57 2023-05-24 14:00:39.000000 yokkaichi-1.6.1/pyproject.toml
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       38 2023-07-29 22:34:27.731218 yokkaichi-1.6.1/setup.cfg
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1714 2023-07-29 22:31:35.000000 yokkaichi-1.6.1/setup.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-29 22:34:27.724551 yokkaichi-1.6.1/yokkaichi/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     4709 2023-07-27 00:25:15.000000 yokkaichi-1.6.1/yokkaichi/Checker.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     7361 2023-07-21 15:44:18.000000 yokkaichi-1.6.1/yokkaichi/IP2L_Manager.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      685 2023-07-27 00:25:15.000000 yokkaichi-1.6.1/yokkaichi/Results.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     3226 2023-07-27 00:25:15.000000 yokkaichi-1.6.1/yokkaichi/ServerScan.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       22 2023-07-29 22:32:28.000000 yokkaichi-1.6.1/yokkaichi/__init__.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     4493 2023-07-29 22:31:35.000000 yokkaichi-1.6.1/yokkaichi/__main__.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     4835 2023-07-29 22:31:35.000000 yokkaichi-1.6.1/yokkaichi/config_loader.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-29 22:34:27.727885 yokkaichi-1.6.1/yokkaichi/constants/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       30 2023-07-15 21:48:34.000000 yokkaichi-1.6.1/yokkaichi/constants/__init__.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       69 2023-07-15 21:48:34.000000 yokkaichi-1.6.1/yokkaichi/constants/_console.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-29 22:34:27.727885 yokkaichi-1.6.1/yokkaichi/enums/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      178 2023-07-21 15:44:18.000000 yokkaichi-1.6.1/yokkaichi/enums/_IP2LocDBStatus.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      151 2023-07-21 15:44:18.000000 yokkaichi-1.6.1/yokkaichi/enums/_IP2LocManagerUserAnswers.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      146 2023-07-21 15:44:18.000000 yokkaichi-1.6.1/yokkaichi/enums/_OfflinePrintingModes.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       89 2023-07-15 21:48:34.000000 yokkaichi-1.6.1/yokkaichi/enums/_Platforms.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      198 2023-07-21 15:44:18.000000 yokkaichi-1.6.1/yokkaichi/enums/__init__.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      224 2023-07-21 15:44:18.000000 yokkaichi-1.6.1/yokkaichi/env_loader.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1155 2023-07-20 01:23:02.000000 yokkaichi-1.6.1/yokkaichi/port_parser.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-29 22:34:27.731218 yokkaichi-1.6.1/yokkaichi/structs/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1243 2023-07-21 15:44:18.000000 yokkaichi-1.6.1/yokkaichi/structs/_CFG.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      135 2023-07-21 15:44:18.000000 yokkaichi-1.6.1/yokkaichi/structs/_EnvVariables.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      275 2023-07-21 15:44:18.000000 yokkaichi-1.6.1/yokkaichi/structs/_MinecraftServer.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      108 2023-07-21 15:44:18.000000 yokkaichi-1.6.1/yokkaichi/structs/__init__.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-29 22:34:27.727885 yokkaichi-1.6.1/yokkaichi.egg-info/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     3892 2023-07-29 22:34:27.000000 yokkaichi-1.6.1/yokkaichi.egg-info/PKG-INFO
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      994 2023-07-29 22:34:27.000000 yokkaichi-1.6.1/yokkaichi.egg-info/SOURCES.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)        1 2023-07-29 22:34:27.000000 yokkaichi-1.6.1/yokkaichi.egg-info/dependency_links.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       54 2023-07-29 22:34:27.000000 yokkaichi-1.6.1/yokkaichi.egg-info/entry_points.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      133 2023-07-29 22:34:27.000000 yokkaichi-1.6.1/yokkaichi.egg-info/requires.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       26 2023-07-29 22:34:27.000000 yokkaichi-1.6.1/yokkaichi.egg-info/top_level.txt
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-29 22:34:27.731218 yokkaichi-1.6.1/yokkaichi_tests/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)        0 2023-07-29 22:31:35.000000 yokkaichi-1.6.1/yokkaichi_tests/__init__.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      189 2023-07-29 22:31:35.000000 yokkaichi-1.6.1/yokkaichi_tests/__main__.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     2363 2023-07-29 22:31:35.000000 yokkaichi-1.6.1/yokkaichi_tests/test_config_loader.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      429 2023-07-29 22:31:35.000000 yokkaichi-1.6.1/yokkaichi_tests/test_env_loader.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      414 2023-07-29 22:31:35.000000 yokkaichi-1.6.1/yokkaichi_tests/test_port_parser.py
```

### Comparing `yokkaichi-1.6/LICENSE.txt` & `yokkaichi-1.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.6/PKG-INFO` & `yokkaichi-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yokkaichi
-Version: 1.6
+Version: 1.6.1
 Summary: Shodan-like server scanner for Minecraft (formely mcserverscanner)
 Home-page: https://github.com/Oreeeee/yokkaichi
 Author: Oreeeee
 License: MIT
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `yokkaichi-1.6/README.md` & `yokkaichi-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.6/setup.py` & `yokkaichi-1.6.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     author="Oreeeee",
     license="MIT",
     url="https://github.com/Oreeeee/yokkaichi",
     install_requires=[
         "rich==13.4.2",
         "mcstatus==11.0.0",
         "IP2Location==8.10.0",
-        "tomli==2.0.1",
-        "pyScannerWrapper==0.2.0",
+        "tomli==2.0.1;python_version<'3.11'",
+        "pyScannerWrapper==0.2.1",
     ],
     extras_require={"testing": ["pytest"]},
     entry_points={"console_scripts": ["yokkaichi=yokkaichi.__main__:main"]},
     classifiers=[
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -45,9 +45,10 @@
         "Programming Language :: Python :: Implementation :: CPython",
     ],
     packages=[
         "yokkaichi",
         "yokkaichi.constants",
         "yokkaichi.structs",
         "yokkaichi.enums",
+        "yokkaichi_tests",
     ],
 )
```

### Comparing `yokkaichi-1.6/yokkaichi/Checker.py` & `yokkaichi-1.6.1/yokkaichi/Checker.py`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.6/yokkaichi/IP2L_Manager.py` & `yokkaichi-1.6.1/yokkaichi/IP2L_Manager.py`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.6/yokkaichi/Results.py` & `yokkaichi-1.6.1/yokkaichi/Results.py`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.6/yokkaichi/ServerScan.py` & `yokkaichi-1.6.1/yokkaichi/ServerScan.py`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.6/yokkaichi/__main__.py` & `yokkaichi-1.6.1/yokkaichi/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # Import modules
 import argparse
 import pathlib
 import platform
+import sys
 import time
 from datetime import datetime
 
-import tomli
+if sys.version_info >= (3, 11):
+    import tomllib
+else:
+    import tomli as tomllib
 
 from yokkaichi import __version__
 
 from . import config_loader, env_loader
 from .constants import console
 from .IP2L_Manager import IP2L_Manager
 from .port_parser import parse_port_range
@@ -65,15 +69,15 @@
         # Show the version and exit
         display_version()
 
     # Load the config file
     if args.config_file != None:
         try:
             cfg = config_loader.parse_cfg(args.config_file)
-        except tomli.TOMLDecodeError:
+        except tomllib.TOMLDecodeError:
             console.print(
                 "Config file is invalid! (Failed parsing TOML)", style="bold red"
             )
         except FileNotFoundError:
             console.print(
                 f"[bold white]{args.config_file}[/bold white] doesn't exist. Create a sample config in this location? (y/n) ",
                 style="yellow",
```

### Comparing `yokkaichi-1.6/yokkaichi/config_loader.py` & `yokkaichi-1.6.1/yokkaichi/config_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-import tomli
+import sys
+
+if sys.version_info >= (3, 11):
+    import tomllib
+else:
+    import tomli as tomllib
 
 from .constants import console
 from .enums import Platforms
 from .port_parser import parse_port_range
 from .structs import CFG
 
 CONFIG_VERSION = "2"
@@ -58,15 +63,15 @@
 csv_code = "DB1LITECSV" # Avoid changing this
 cache = true # Enable for faster speed at the cost of RAM
 """.strip()
 
 
 def load_cfg(cfg_location):
     with open(cfg_location, "rb") as f:
-        cfg_file = tomli.load(f)
+        cfg_file = tomllib.load(f)
     return cfg_file
 
 
 def parse_cfg(cfg_location):
     # Read the config file
     cfg_file = load_cfg(cfg_location)
```

### Comparing `yokkaichi-1.6/yokkaichi/port_parser.py` & `yokkaichi-1.6.1/yokkaichi/port_parser.py`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.6/yokkaichi/structs/_CFG.py` & `yokkaichi-1.6.1/yokkaichi/structs/_CFG.py`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.6/yokkaichi.egg-info/PKG-INFO` & `yokkaichi-1.6.1/yokkaichi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yokkaichi
-Version: 1.6
+Version: 1.6.1
 Summary: Shodan-like server scanner for Minecraft (formely mcserverscanner)
 Home-page: https://github.com/Oreeeee/yokkaichi
 Author: Oreeeee
 License: MIT
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `yokkaichi-1.6/yokkaichi.egg-info/SOURCES.txt` & `yokkaichi-1.6.1/yokkaichi.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -23,8 +23,13 @@
 yokkaichi/enums/_IP2LocManagerUserAnswers.py
 yokkaichi/enums/_OfflinePrintingModes.py
 yokkaichi/enums/_Platforms.py
 yokkaichi/enums/__init__.py
 yokkaichi/structs/_CFG.py
 yokkaichi/structs/_EnvVariables.py
 yokkaichi/structs/_MinecraftServer.py
-yokkaichi/structs/__init__.py
+yokkaichi/structs/__init__.py
+yokkaichi_tests/__init__.py
+yokkaichi_tests/__main__.py
+yokkaichi_tests/test_config_loader.py
+yokkaichi_tests/test_env_loader.py
+yokkaichi_tests/test_port_parser.py
```

