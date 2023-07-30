# Comparing `tmp/agentagenda-0.0.7.tar.gz` & `tmp/agentagenda-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentagenda-0.0.7.tar", last modified: Sun Jul 30 03:03:54 2023, max compression
+gzip compressed data, was "agentagenda-0.0.8.tar", last modified: Sun Jul 30 12:57:48 2023, max compression
```

## Comparing `agentagenda-0.0.7.tar` & `agentagenda-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:03:54.781661 agentagenda-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-30 03:03:44.000000 agentagenda-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-07-30 03:03:54.781661 agentagenda-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-07-30 03:03:44.000000 agentagenda-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:03:54.781661 agentagenda-0.0.7/agentagenda/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-30 03:03:44.000000 agentagenda-0.0.7/agentagenda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16233 2023-07-30 03:03:44.000000 agentagenda-0.0.7/agentagenda/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-07-30 03:03:44.000000 agentagenda-0.0.7/agentagenda/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:03:54.781661 agentagenda-0.0.7/agentagenda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-07-30 03:03:54.000000 agentagenda-0.0.7/agentagenda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-30 03:03:54.000000 agentagenda-0.0.7/agentagenda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 03:03:54.000000 agentagenda-0.0.7/agentagenda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-30 03:03:54.000000 agentagenda-0.0.7/agentagenda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-30 03:03:54.000000 agentagenda-0.0.7/agentagenda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 03:03:54.781661 agentagenda-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-30 03:03:44.000000 agentagenda-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:57:48.890134 agentagenda-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-30 12:57:35.000000 agentagenda-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-07-30 12:57:48.886134 agentagenda-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-07-30 12:57:35.000000 agentagenda-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:57:48.886134 agentagenda-0.0.8/agentagenda/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-30 12:57:35.000000 agentagenda-0.0.8/agentagenda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16577 2023-07-30 12:57:35.000000 agentagenda-0.0.8/agentagenda/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-07-30 12:57:35.000000 agentagenda-0.0.8/agentagenda/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:57:48.886134 agentagenda-0.0.8/agentagenda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-07-30 12:57:48.000000 agentagenda-0.0.8/agentagenda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-30 12:57:48.000000 agentagenda-0.0.8/agentagenda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 12:57:48.000000 agentagenda-0.0.8/agentagenda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-30 12:57:48.000000 agentagenda-0.0.8/agentagenda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-30 12:57:48.000000 agentagenda-0.0.8/agentagenda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 12:57:48.890134 agentagenda-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-30 12:57:35.000000 agentagenda-0.0.8/setup.py
```

### Comparing `agentagenda-0.0.7/LICENSE` & `agentagenda-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `agentagenda-0.0.7/PKG-INFO` & `agentagenda-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentagenda
-Version: 0.0.7
+Version: 0.0.8
 Summary: A task manager for your agent.
 Home-page: https://github.com/AutonomousResearchGroup/agentagenda
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `agentagenda-0.0.7/README.md` & `agentagenda-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `agentagenda-0.0.7/agentagenda/main.py` & `agentagenda-0.0.8/agentagenda/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,21 +90,28 @@
     if isinstance(steps, dict) or isinstance(steps, list):
         steps = json.dumps(steps)
 
     # get timestamp
     created_at = datetime.timestamp(datetime.now())
     updated_at = datetime.timestamp(datetime.now())
 
+    memories = get_memories("task", filter_metadata={"current": "True"})
+    for memory in memories:
+        metadata = memory["metadata"]
+        metadata["current"] = "False"
+        update_memory("task", memory["id"], metadata=metadata)
+
     task = {
         "created_at": created_at,
         "updated_at": updated_at,
         "goal": goal,
         "plan": plan,
         "steps": steps,
         "status": "in_progress",
+        "current": "True",
     }
 
     return get_task_by_id(create_memory("task", goal, metadata=task))
 
 
 def list_tasks(status="in_progress"):
     """List all tasks with the given status.
@@ -187,14 +194,15 @@
     updated_at = datetime.timestamp(datetime.now())
 
     memory = get_memory("task", get_task_id(task))
 
     metadata = memory["metadata"]
     metadata["status"] = "complete"
     metadata["updated_at"] = updated_at
+    metadata["current"] = "False"
 
     return update_memory(
         "task",
         get_task_id(task),
         metadata=metadata,
     )
 
@@ -212,14 +220,15 @@
     updated_at = datetime.timestamp(datetime.now())
 
     memory = get_memory("task", get_task_id(task))
 
     metadata = memory["metadata"]
     metadata["status"] = "cancelled"
     metadata["updated_at"] = updated_at
+    metadata["current"] = "False"
 
     return update_memory(
         "task",
         get_task_id(task),
         metadata=metadata,
     )
 
@@ -283,15 +292,15 @@
 
     Returns
     -------
     dict or None
         The task marked as the current active task. If no current task is found, None is returned.
     """
     memory = get_memories(
-        "task", filter_metadata={"current": True}, include_embeddings=False
+        "task", filter_metadata={"current": "True"}, include_embeddings=False
     )
     if len(memory) > 0:
         log("Current task: {}".format(memory[0]), log=debug)
         return memory[0]
     else:
         log("No current task found", log=debug)
         return None
@@ -305,24 +314,24 @@
 
     Returns:
         dict: The response from the memory update operation.
     """
     task_id = get_task_id
 
     memories = get_memories(
-        "task", filter_metadata={"current": True}, include_embeddings=False
+        "task", filter_metadata={"current": "True"}, include_embeddings=False
     )
 
     for memory in memories:
         metadata = memory["metadata"]
-        metadata["current"] = False
+        metadata["current"] = "False"
         update_memory("task", memory["id"], metadata=metadata)
     log("Setting current task: {}".format(task), log=debug)
     metadata = memory["metadata"]
-    metadata["current"] = True
+    metadata["current"] = "True"
     return update_memory("task", task_id, metadata=metadata)
 
 
 def create_plan(goal, model="gpt-3.5-turbo-0613"):
     """Create a plan for the goal using OpenAI API.
 
     Args:
```

### Comparing `agentagenda-0.0.7/agentagenda/test.py` & `agentagenda-0.0.8/agentagenda/test.py`

 * *Files identical despite different names*

### Comparing `agentagenda-0.0.7/agentagenda.egg-info/PKG-INFO` & `agentagenda-0.0.8/agentagenda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentagenda
-Version: 0.0.7
+Version: 0.0.8
 Summary: A task manager for your agent.
 Home-page: https://github.com/AutonomousResearchGroup/agentagenda
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `agentagenda-0.0.7/setup.py` & `agentagenda-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = [line for line in long_description if not "<img" in line]
     # now join all the lines back together
     long_description = "\n".join(long_description)
 
 
 setup(
     name="agentagenda",
-    version="0.0.7",
+    version="0.0.8",
     description="A task manager for your agent.",
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url="https://github.com/AutonomousResearchGroup/agentagenda",
     author="Moon",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
```

