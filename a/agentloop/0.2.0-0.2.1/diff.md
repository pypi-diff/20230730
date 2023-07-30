# Comparing `tmp/agentloop-0.2.0.tar.gz` & `tmp/agentloop-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentloop-0.2.0.tar", last modified: Sun Jul 30 01:30:31 2023, max compression
+gzip compressed data, was "agentloop-0.2.1.tar", last modified: Sun Jul 30 03:33:13 2023, max compression
```

## Comparing `agentloop-0.2.0.tar` & `agentloop-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:30:31.911749 agentloop-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-30 01:30:20.000000 agentloop-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-30 01:30:31.911749 agentloop-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-07-30 01:30:20.000000 agentloop-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:30:31.907750 agentloop-0.2.0/agentloop/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-30 01:30:20.000000 agentloop-0.2.0/agentloop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-30 01:30:20.000000 agentloop-0.2.0/agentloop/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-07-30 01:30:20.000000 agentloop-0.2.0/agentloop/loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:30:31.911749 agentloop-0.2.0/agentloop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-30 01:30:31.000000 agentloop-0.2.0/agentloop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-30 01:30:31.000000 agentloop-0.2.0/agentloop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 01:30:31.000000 agentloop-0.2.0/agentloop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-30 01:30:31.000000 agentloop-0.2.0/agentloop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-30 01:30:31.000000 agentloop-0.2.0/agentloop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 01:30:31.911749 agentloop-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-30 01:30:20.000000 agentloop-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:33:13.322184 agentloop-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-30 03:33:04.000000 agentloop-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-30 03:33:13.322184 agentloop-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-07-30 03:33:04.000000 agentloop-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:33:13.322184 agentloop-0.2.1/agentloop/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-30 03:33:04.000000 agentloop-0.2.1/agentloop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-30 03:33:04.000000 agentloop-0.2.1/agentloop/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-07-30 03:33:04.000000 agentloop-0.2.1/agentloop/loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:33:13.322184 agentloop-0.2.1/agentloop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-30 03:33:13.000000 agentloop-0.2.1/agentloop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-30 03:33:13.000000 agentloop-0.2.1/agentloop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 03:33:13.000000 agentloop-0.2.1/agentloop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-30 03:33:13.000000 agentloop-0.2.1/agentloop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-30 03:33:13.000000 agentloop-0.2.1/agentloop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 03:33:13.322184 agentloop-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-30 03:33:04.000000 agentloop-0.2.1/setup.py
```

### Comparing `agentloop-0.2.0/LICENSE` & `agentloop-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `agentloop-0.2.0/PKG-INFO` & `agentloop-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentloop
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple, lightweight loop for your agent.
 Home-page: https://github.com/AutonomousResearchGroup/agentloop
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `agentloop-0.2.0/README.md` & `agentloop-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `agentloop-0.2.0/agentloop/input.py` & `agentloop-0.2.1/agentloop/input.py`

 * *Files identical despite different names*

### Comparing `agentloop-0.2.0/agentloop/loop.py` & `agentloop-0.2.1/agentloop/loop.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,14 @@
                 raise ValueError(
                     "Step function must take 1 or 2 arguments. "
                     "Valid arguments are next_output, loop_data (optional). "
                     "Found {} arguments".format(number_of_args)
                 )
 
             while loop_data["pause_event"].is_set():
-                print("Loop paused")
                 if loop_data["stop_event"].wait(timeout=1):
                     return
             if loop_data["step_event"].wait(timeout=1):
                 loop_data["step_event"].clear()
         if loop_data["stop_event"].is_set():
             break
```

### Comparing `agentloop-0.2.0/agentloop.egg-info/PKG-INFO` & `agentloop-0.2.1/agentloop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentloop
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple, lightweight loop for your agent.
 Home-page: https://github.com/AutonomousResearchGroup/agentloop
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `agentloop-0.2.0/setup.py` & `agentloop-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     readme = [line for line in readme if "<img" not in line]
     # now join all the lines back together
     readme = "\n".join(readme)
 
 
 setup(
     name="agentloop",
-    version="0.2.0",
+    version="0.2.1",
     description="A simple, lightweight loop for your agent.",
     long_description=readme,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url="https://github.com/AutonomousResearchGroup/agentloop",
     author="Moon",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
```

