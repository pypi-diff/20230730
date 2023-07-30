# Comparing `tmp/agentagenda-0.0.6.tar.gz` & `tmp/agentagenda-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentagenda-0.0.6.tar", last modified: Fri Jul 28 10:43:31 2023, max compression
+gzip compressed data, was "agentagenda-0.0.7.tar", last modified: Sun Jul 30 03:03:54 2023, max compression
```

## Comparing `agentagenda-0.0.6.tar` & `agentagenda-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:43:31.606046 agentagenda-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-28 10:43:21.000000 agentagenda-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-07-28 10:43:31.606046 agentagenda-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-07-28 10:43:21.000000 agentagenda-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:43:31.602046 agentagenda-0.0.6/agentagenda/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 10:43:21.000000 agentagenda-0.0.6/agentagenda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16067 2023-07-28 10:43:21.000000 agentagenda-0.0.6/agentagenda/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-07-28 10:43:21.000000 agentagenda-0.0.6/agentagenda/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:43:31.602046 agentagenda-0.0.6/agentagenda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-07-28 10:43:31.000000 agentagenda-0.0.6/agentagenda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-28 10:43:31.000000 agentagenda-0.0.6/agentagenda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:43:31.000000 agentagenda-0.0.6/agentagenda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-28 10:43:31.000000 agentagenda-0.0.6/agentagenda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 10:43:31.000000 agentagenda-0.0.6/agentagenda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 10:43:31.606046 agentagenda-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-28 10:43:21.000000 agentagenda-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:03:54.781661 agentagenda-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-30 03:03:44.000000 agentagenda-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-07-30 03:03:54.781661 agentagenda-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-07-30 03:03:44.000000 agentagenda-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:03:54.781661 agentagenda-0.0.7/agentagenda/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-30 03:03:44.000000 agentagenda-0.0.7/agentagenda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16233 2023-07-30 03:03:44.000000 agentagenda-0.0.7/agentagenda/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-07-30 03:03:44.000000 agentagenda-0.0.7/agentagenda/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:03:54.781661 agentagenda-0.0.7/agentagenda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-07-30 03:03:54.000000 agentagenda-0.0.7/agentagenda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-30 03:03:54.000000 agentagenda-0.0.7/agentagenda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 03:03:54.000000 agentagenda-0.0.7/agentagenda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-30 03:03:54.000000 agentagenda-0.0.7/agentagenda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-30 03:03:54.000000 agentagenda-0.0.7/agentagenda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 03:03:54.781661 agentagenda-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-30 03:03:44.000000 agentagenda-0.0.7/setup.py
```

### Comparing `agentagenda-0.0.6/LICENSE` & `agentagenda-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `agentagenda-0.0.6/PKG-INFO` & `agentagenda-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentagenda
-Version: 0.0.6
+Version: 0.0.7
 Summary: A task manager for your agent.
 Home-page: https://github.com/AutonomousResearchGroup/agentagenda
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `agentagenda-0.0.6/README.md` & `agentagenda-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `agentagenda-0.0.6/agentagenda/main.py` & `agentagenda-0.0.7/agentagenda/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,21 @@
             function_call="create_steps",
             debug=debug,
             model=model,
         )
 
         steps = response["arguments"]["steps"]
 
+        step_items = []
+
+        for step in steps:
+            step_items.append({"content": step, "completed": False})
+        
+        steps = step_items
+
     # if steps is a dict, json stringify it
     if isinstance(steps, dict) or isinstance(steps, list):
         steps = json.dumps(steps)
 
     # get timestamp
     created_at = datetime.timestamp(datetime.now())
     updated_at = datetime.timestamp(datetime.now())
@@ -456,15 +463,15 @@
         The updated task after marking the step as completed.
     """
     task_id = get_task_id(task)
     task = get_memory("task", task_id)
     metadata = task["metadata"]
     steps = json.loads(metadata["steps"])
     for s in steps:
-        if s["content"] == step:
+        if s["content"].includes(step):
             s["completed"] = True
     metadata["steps"] = json.dumps(steps)
     log(
         "Finishing step for task: {}\nSteps are: {}".format(task, metadata["steps"]),
         log=debug,
     )
     metadata["updated_at"] = datetime.timestamp(datetime.now())
@@ -539,14 +546,15 @@
 
     if include_status:
         task_details.append("Status: {}".format(task["metadata"]["status"]))
 
     if include_steps:
         # For the steps, since it's a list, we need to format each step separately
         steps = json.loads(task["metadata"]["steps"])
+
         formatted_steps = ", ".join(
             [
                 "{}: {}".format(
                     step["content"],
                     "Completed" if step["completed"] else "Not completed",
                 )
                 for step in steps
```

### Comparing `agentagenda-0.0.6/agentagenda/test.py` & `agentagenda-0.0.7/agentagenda/test.py`

 * *Files identical despite different names*

### Comparing `agentagenda-0.0.6/agentagenda.egg-info/PKG-INFO` & `agentagenda-0.0.7/agentagenda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentagenda
-Version: 0.0.6
+Version: 0.0.7
 Summary: A task manager for your agent.
 Home-page: https://github.com/AutonomousResearchGroup/agentagenda
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `agentagenda-0.0.6/setup.py` & `agentagenda-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = [line for line in long_description if not "<img" in line]
     # now join all the lines back together
     long_description = "\n".join(long_description)
 
 
 setup(
     name="agentagenda",
-    version="0.0.6",
+    version="0.0.7",
     description="A task manager for your agent.",
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url="https://github.com/AutonomousResearchGroup/agentagenda",
     author="Moon",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
```

