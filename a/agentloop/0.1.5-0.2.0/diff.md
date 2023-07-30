# Comparing `tmp/agentloop-0.1.5.tar.gz` & `tmp/agentloop-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentloop-0.1.5.tar", last modified: Fri Jul 28 11:10:45 2023, max compression
+gzip compressed data, was "agentloop-0.2.0.tar", last modified: Sun Jul 30 01:30:31 2023, max compression
```

## Comparing `agentloop-0.1.5.tar` & `agentloop-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:10:45.307945 agentloop-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-28 11:10:35.000000 agentloop-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-07-28 11:10:45.307945 agentloop-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-07-28 11:10:35.000000 agentloop-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:10:45.307945 agentloop-0.1.5/agentloop/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-28 11:10:35.000000 agentloop-0.1.5/agentloop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-28 11:10:35.000000 agentloop-0.1.5/agentloop/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-28 11:10:35.000000 agentloop-0.1.5/agentloop/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-28 11:10:35.000000 agentloop-0.1.5/agentloop/loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:10:45.307945 agentloop-0.1.5/agentloop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-07-28 11:10:45.000000 agentloop-0.1.5/agentloop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-28 11:10:45.000000 agentloop-0.1.5/agentloop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 11:10:45.000000 agentloop-0.1.5/agentloop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 11:10:45.000000 agentloop-0.1.5/agentloop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-28 11:10:45.000000 agentloop-0.1.5/agentloop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 11:10:45.307945 agentloop-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-28 11:10:35.000000 agentloop-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:30:31.911749 agentloop-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-30 01:30:20.000000 agentloop-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-30 01:30:31.911749 agentloop-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-07-30 01:30:20.000000 agentloop-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:30:31.907750 agentloop-0.2.0/agentloop/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-30 01:30:20.000000 agentloop-0.2.0/agentloop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-30 01:30:20.000000 agentloop-0.2.0/agentloop/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-07-30 01:30:20.000000 agentloop-0.2.0/agentloop/loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:30:31.911749 agentloop-0.2.0/agentloop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-30 01:30:31.000000 agentloop-0.2.0/agentloop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-30 01:30:31.000000 agentloop-0.2.0/agentloop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 01:30:31.000000 agentloop-0.2.0/agentloop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-30 01:30:31.000000 agentloop-0.2.0/agentloop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-30 01:30:31.000000 agentloop-0.2.0/agentloop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 01:30:31.911749 agentloop-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-30 01:30:20.000000 agentloop-0.2.0/setup.py
```

### Comparing `agentloop-0.1.5/LICENSE` & `agentloop-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `agentloop-0.1.5/PKG-INFO` & `agentloop-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentloop
-Version: 0.1.5
+Version: 0.2.0
 Summary: A simple, lightweight loop for your agent.
 Home-page: https://github.com/AutonomousResearchGroup/agentloop
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -35,14 +35,20 @@
 def step_two(next_output, loop_data):
     print("step_two")
     return next_output
 
 # Run the loop
 loop_data = start(steps=[step_one, step_two])
 
+# Pause the loop
+pause(loop_data)
+
+# Unpause the loop
+unpause(loop_data)
+
 # Stop the loop
 stop(loop_data)
 ```
 
 # Installation
 
 ```bash
@@ -114,14 +120,56 @@
 
 ### Returns
 
 None
 
 ---
 
+Sure, here are the updated sections for the `pause` and `unpause` functions in your README file.
+
+---
+
+## Function `pause`
+
+```python
+pause(loop_data)
+```
+
+### Description
+
+Pauses the loop. When paused, the loop will not execute the next step until it's either stepped using the `step` function or unpaused using the `unpause` function.
+
+### Parameters
+
+- `loop_data`: a dictionary containing the `pause_event` which is returned by the `start` function.
+
+### Returns
+
+None
+
+---
+
+## Function `unpause`
+
+```python
+unpause(loop_data)
+```
+
+### Description
+
+Resumes the loop after it has been paused with the `pause` function. If the loop is not paused, calling this function has no effect.
+
+### Parameters
+
+- `loop_data`: a dictionary containing the `pause_event` which is returned by the `start` function.
+
+### Returns
+
+None
+
 ## Function `step`
 
 ```python
 step(loop_data)
 ```
 
 ### Description
```

### Comparing `agentloop-0.1.5/README.md` & `agentloop-0.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -19,14 +19,20 @@
 def step_two(next_output, loop_data):
     print("step_two")
     return next_output
 
 # Run the loop
 loop_data = start(steps=[step_one, step_two])
 
+# Pause the loop
+pause(loop_data)
+
+# Unpause the loop
+unpause(loop_data)
+
 # Stop the loop
 stop(loop_data)
 ```
 
 # Installation
 
 ```bash
@@ -98,14 +104,56 @@
 
 ### Returns
 
 None
 
 ---
 
+Sure, here are the updated sections for the `pause` and `unpause` functions in your README file.
+
+---
+
+## Function `pause`
+
+```python
+pause(loop_data)
+```
+
+### Description
+
+Pauses the loop. When paused, the loop will not execute the next step until it's either stepped using the `step` function or unpaused using the `unpause` function.
+
+### Parameters
+
+- `loop_data`: a dictionary containing the `pause_event` which is returned by the `start` function.
+
+### Returns
+
+None
+
+---
+
+## Function `unpause`
+
+```python
+unpause(loop_data)
+```
+
+### Description
+
+Resumes the loop after it has been paused with the `pause` function. If the loop is not paused, calling this function has no effect.
+
+### Parameters
+
+- `loop_data`: a dictionary containing the `pause_event` which is returned by the `start` function.
+
+### Returns
+
+None
+
 ## Function `step`
 
 ```python
 step(loop_data)
 ```
 
 ### Description
```

### Comparing `agentloop-0.1.5/agentloop/input.py` & `agentloop-0.2.0/agentloop/input.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .loop import stop
+from agentloop.loop import stop
 
 def step_with_input_key(loop_data):
     """
     Listen for a specified key press, and when detected, step the loop
 
     Args:
         loop_data: loop data object, created by the start function
```

### Comparing `agentloop-0.1.5/agentloop/loop.py` & `agentloop-0.2.0/agentloop/loop.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 import threading
 
 
-def start(steps, stepped=False):
+def start(steps, paused=False):
     """
     Function to start the main loop
 
     Args:
-        stepped: boolean - whether the loop should run one-step-at-a-time.
+        paused: boolean - whether the loop should run automatically. If paused can be stepped one-step-at-a-time.
             Defaults to False.
 
     Returns:
         loop_data: a dictionary of loop data
     """
 
     loop_data = {
         "stop_event": threading.Event(),
         "step_event": threading.Event(),
         "started_event": threading.Event(),
+        "pause_event": threading.Event(),
     }
 
-    thread = threading.Thread(target=loop, args=(steps, stepped, loop_data))
+    if paused:
+        loop_data["pause_event"].set()
+
+    thread = threading.Thread(target=loop, args=(steps, loop_data))
     loop_data["thread"] = thread
 
     thread.start()
     loop_data["started_event"].wait()  # Wait here until loop is started
 
     return loop_data
 
@@ -54,53 +58,67 @@
         loop_data: loop data object, created by the start function
 
     This function does not return any value.
     """
     loop_data["step_event"].set()
 
 
-def loop(steps, stepped=False, loop_data=None):
+def pause(loop_data):
+    """
+    Function to pause the loop
+
+    Args:
+        loop_data: loop data object, created by the start function
+
+    This function does not return any value.
+    """
+    loop_data["pause_event"].set()
+
+
+def unpause(loop_data):
+    """
+    Function to unpause the loop
+
+    Args:
+        loop_data: loop data object, created by the start function
+
+    This function does not return any value.
+    """
+    loop_data["pause_event"].clear()
+
+
+def loop(steps, loop_data):
     """
     Run the step array in a loop until stopped
 
     Args:
         steps: array of functions to be run in the loop
-        stepped: boolean - whether the loop should run in stepped mode or not
+        paused: boolean - whether the loop should run start up paused (can be stepped) or running
         loop_data: loop data object, created by the start function
 
     This function does not return any value.
     """
-    if loop_data is None:
-        loop_data = {
-            "stop_event": threading.Event(),
-            "step_event": threading.Event(),
-            "started_event": threading.Event(),
-        }
-
     next_output = None
     loop_data["started_event"].set()  # Indicate that the loop has started
     while not loop_data["stop_event"].is_set():
         for step in steps:
-            # check how many arguments step takes, 1 or 2?
             number_of_args = step.__code__.co_argcount
             if number_of_args == 1:
                 next_output = step(next_output)
             elif number_of_args == 2:
                 next_output = step(next_output, loop_data)
             else:
                 raise ValueError(
-                    "Step function must take 1 or 2 arguments"
-                    "Valid arguments are next_output, loop_data (optional)"
+                    "Step function must take 1 or 2 arguments. "
+                    "Valid arguments are next_output, loop_data (optional). "
                     "Found {} arguments".format(number_of_args)
                 )
-            if stepped:
-                # Wait here until step_event is set
-                while not loop_data["step_event"].wait(timeout=1):
-                    if loop_data["stop_event"].is_set():
-                        break
-                if loop_data["stop_event"].is_set():
-                    break
+
+            while loop_data["pause_event"].is_set():
+                print("Loop paused")
+                if loop_data["stop_event"].wait(timeout=1):
+                    return
+            if loop_data["step_event"].wait(timeout=1):
                 loop_data["step_event"].clear()
         if loop_data["stop_event"].is_set():
             break
 
-
```

### Comparing `agentloop-0.1.5/agentloop.egg-info/PKG-INFO` & `agentloop-0.2.0/agentloop.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentloop
-Version: 0.1.5
+Version: 0.2.0
 Summary: A simple, lightweight loop for your agent.
 Home-page: https://github.com/AutonomousResearchGroup/agentloop
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -35,14 +35,20 @@
 def step_two(next_output, loop_data):
     print("step_two")
     return next_output
 
 # Run the loop
 loop_data = start(steps=[step_one, step_two])
 
+# Pause the loop
+pause(loop_data)
+
+# Unpause the loop
+unpause(loop_data)
+
 # Stop the loop
 stop(loop_data)
 ```
 
 # Installation
 
 ```bash
@@ -114,14 +120,56 @@
 
 ### Returns
 
 None
 
 ---
 
+Sure, here are the updated sections for the `pause` and `unpause` functions in your README file.
+
+---
+
+## Function `pause`
+
+```python
+pause(loop_data)
+```
+
+### Description
+
+Pauses the loop. When paused, the loop will not execute the next step until it's either stepped using the `step` function or unpaused using the `unpause` function.
+
+### Parameters
+
+- `loop_data`: a dictionary containing the `pause_event` which is returned by the `start` function.
+
+### Returns
+
+None
+
+---
+
+## Function `unpause`
+
+```python
+unpause(loop_data)
+```
+
+### Description
+
+Resumes the loop after it has been paused with the `pause` function. If the loop is not paused, calling this function has no effect.
+
+### Parameters
+
+- `loop_data`: a dictionary containing the `pause_event` which is returned by the `start` function.
+
+### Returns
+
+None
+
 ## Function `step`
 
 ```python
 step(loop_data)
 ```
 
 ### Description
```

### Comparing `agentloop-0.1.5/setup.py` & `agentloop-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     readme = [line for line in readme if "<img" not in line]
     # now join all the lines back together
     readme = "\n".join(readme)
 
 
 setup(
     name="agentloop",
-    version="0.1.5",
+    version="0.2.0",
     description="A simple, lightweight loop for your agent.",
     long_description=readme,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url="https://github.com/AutonomousResearchGroup/agentloop",
     author="Moon",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
```

