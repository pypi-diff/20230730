# Comparing `tmp/gxabm-2.7.5.tar.gz` & `tmp/gxabm-2.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gxabm-2.7.5.tar", last modified: Sat Jul 29 17:10:35 2023, max compression
+gzip compressed data, was "gxabm-2.7.6.tar", last modified: Sun Jul 30 01:47:46 2023, max compression
```

## Comparing `gxabm-2.7.5.tar` & `gxabm-2.7.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-07-29 17:10:35.228626 gxabm-2.7.5/
--rw-r--r--   0 suderman   (502) staff       (20)       42 2022-03-07 12:56:12.000000 gxabm-2.7.5/MANIFEST.in
--rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-07-29 17:10:35.228332 gxabm-2.7.5/PKG-INFO
--rw-r--r--   0 suderman   (502) staff       (20)    16395 2022-03-22 19:06:33.000000 gxabm-2.7.5/README.md
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-07-29 17:10:35.215140 gxabm-2.7.5/abm/
--rw-r--r--   0 suderman   (502) staff       (20)        6 2023-07-29 17:09:46.000000 gxabm-2.7.5/abm/VERSION
--rw-r--r--   0 suderman   (502) staff       (20)      290 2022-03-07 12:56:12.000000 gxabm-2.7.5/abm/__init__.py
--rw-r--r--   0 suderman   (502) staff       (20)     8374 2023-05-01 01:43:54.000000 gxabm-2.7.5/abm/__main__.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-07-29 17:10:35.222858 gxabm-2.7.5/abm/lib/
--rw-r--r--   0 suderman   (502) staff       (20)      447 2022-03-07 12:56:12.000000 gxabm-2.7.5/abm/lib/__init__.py
--rw-r--r--   0 suderman   (502) staff       (20)    19997 2023-07-29 16:49:33.000000 gxabm-2.7.5/abm/lib/benchmark.py
--rw-r--r--   0 suderman   (502) staff       (20)     7812 2022-10-19 17:36:24.000000 gxabm-2.7.5/abm/lib/cloudlaunch.py
--rw-r--r--   0 suderman   (502) staff       (20)     9213 2023-07-29 17:09:46.000000 gxabm-2.7.5/abm/lib/common.py
--rw-r--r--   0 suderman   (502) staff       (20)     5433 2023-07-11 14:04:56.000000 gxabm-2.7.5/abm/lib/config.py
--rw-r--r--   0 suderman   (502) staff       (20)     8016 2023-07-11 14:04:56.000000 gxabm-2.7.5/abm/lib/dataset.py
--rw-r--r--   0 suderman   (502) staff       (20)     7840 2023-07-29 17:09:46.000000 gxabm-2.7.5/abm/lib/experiment.py
--rw-r--r--   0 suderman   (502) staff       (20)      883 2022-03-07 12:56:12.000000 gxabm-2.7.5/abm/lib/folder.py
--rw-r--r--   0 suderman   (502) staff       (20)     4357 2023-07-11 14:04:56.000000 gxabm-2.7.5/abm/lib/helm.py
--rw-r--r--   0 suderman   (502) staff       (20)      282 2022-03-07 12:56:12.000000 gxabm-2.7.5/abm/lib/histories.yml
--rw-r--r--   0 suderman   (502) staff       (20)    11689 2023-07-29 16:25:27.000000 gxabm-2.7.5/abm/lib/history.py
--rw-r--r--   0 suderman   (502) staff       (20)     1217 2023-05-01 01:43:54.000000 gxabm-2.7.5/abm/lib/invocation.py
--rw-r--r--   0 suderman   (502) staff       (20)     5061 2023-07-29 17:09:46.000000 gxabm-2.7.5/abm/lib/job.py
--rw-r--r--   0 suderman   (502) staff       (20)     1264 2022-03-07 12:56:12.000000 gxabm-2.7.5/abm/lib/kubectl.py
--rw-r--r--   0 suderman   (502) staff       (20)     2518 2023-04-24 20:08:21.000000 gxabm-2.7.5/abm/lib/library.py
--rw-r--r--   0 suderman   (502) staff       (20)    12347 2023-06-26 20:05:31.000000 gxabm-2.7.5/abm/lib/menu.yml
--rw-r--r--   0 suderman   (502) staff       (20)     3480 2022-10-19 17:36:24.000000 gxabm-2.7.5/abm/lib/users.py
--rw-r--r--   0 suderman   (502) staff       (20)     7817 2023-05-01 01:43:54.000000 gxabm-2.7.5/abm/lib/workflow.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-07-29 17:10:35.224566 gxabm-2.7.5/gxabm.egg-info/
--rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-07-29 17:10:34.000000 gxabm-2.7.5/gxabm.egg-info/PKG-INFO
--rw-r--r--   0 suderman   (502) staff       (20)      715 2023-07-29 17:10:34.000000 gxabm-2.7.5/gxabm.egg-info/SOURCES.txt
--rw-r--r--   0 suderman   (502) staff       (20)        1 2023-07-29 17:10:34.000000 gxabm-2.7.5/gxabm.egg-info/dependency_links.txt
--rw-r--r--   0 suderman   (502) staff       (20)       49 2023-07-29 17:10:34.000000 gxabm-2.7.5/gxabm.egg-info/entry_points.txt
--rw-r--r--   0 suderman   (502) staff       (20)       48 2023-07-29 17:10:34.000000 gxabm-2.7.5/gxabm.egg-info/requires.txt
--rw-r--r--   0 suderman   (502) staff       (20)        9 2023-07-29 17:10:34.000000 gxabm-2.7.5/gxabm.egg-info/top_level.txt
--rw-r--r--   0 suderman   (502) staff       (20)       38 2023-07-29 17:10:35.228720 gxabm-2.7.5/setup.cfg
--rw-r--r--   0 suderman   (502) staff       (20)     1036 2022-10-19 17:36:24.000000 gxabm-2.7.5/setup.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-07-29 17:10:35.227422 gxabm-2.7.5/test/
--rw-r--r--   0 suderman   (502) staff       (20)      543 2023-06-30 04:22:19.000000 gxabm-2.7.5/test/ThreadPoolTests.py
--rw-r--r--   0 suderman   (502) staff       (20)      147 2022-03-07 12:56:12.000000 gxabm-2.7.5/test/__init__.py
--rwxr-xr-x   0 suderman   (502) staff       (20)     8684 2022-12-23 17:29:52.000000 gxabm-2.7.5/test/check_tools.py
--rw-r--r--   0 suderman   (502) staff       (20)     2160 2022-10-27 04:03:53.000000 gxabm-2.7.5/test/metrics.py
--rw-r--r--   0 suderman   (502) staff       (20)      298 2022-03-07 12:56:12.000000 gxabm-2.7.5/test/test_environments.py
--rw-r--r--   0 suderman   (502) staff       (20)      718 2023-06-04 14:10:38.000000 gxabm-2.7.5/test/workflow.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-07-30 01:47:46.050493 gxabm-2.7.6/
+-rw-r--r--   0 suderman   (502) staff       (20)       42 2022-03-07 12:56:12.000000 gxabm-2.7.6/MANIFEST.in
+-rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-07-30 01:47:46.050305 gxabm-2.7.6/PKG-INFO
+-rw-r--r--   0 suderman   (502) staff       (20)    16395 2022-03-22 19:06:33.000000 gxabm-2.7.6/README.md
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-07-30 01:47:46.043007 gxabm-2.7.6/abm/
+-rw-r--r--   0 suderman   (502) staff       (20)        6 2023-07-30 01:19:29.000000 gxabm-2.7.6/abm/VERSION
+-rw-r--r--   0 suderman   (502) staff       (20)      290 2022-03-07 12:56:12.000000 gxabm-2.7.6/abm/__init__.py
+-rw-r--r--   0 suderman   (502) staff       (20)     8374 2023-05-01 01:43:54.000000 gxabm-2.7.6/abm/__main__.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-07-30 01:47:46.047502 gxabm-2.7.6/abm/lib/
+-rw-r--r--   0 suderman   (502) staff       (20)      447 2022-03-07 12:56:12.000000 gxabm-2.7.6/abm/lib/__init__.py
+-rw-r--r--   0 suderman   (502) staff       (20)    19997 2023-07-29 16:49:33.000000 gxabm-2.7.6/abm/lib/benchmark.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7812 2022-10-19 17:36:24.000000 gxabm-2.7.6/abm/lib/cloudlaunch.py
+-rw-r--r--   0 suderman   (502) staff       (20)     9235 2023-07-30 01:41:34.000000 gxabm-2.7.6/abm/lib/common.py
+-rw-r--r--   0 suderman   (502) staff       (20)     5433 2023-07-11 14:04:56.000000 gxabm-2.7.6/abm/lib/config.py
+-rw-r--r--   0 suderman   (502) staff       (20)     8016 2023-07-11 14:04:56.000000 gxabm-2.7.6/abm/lib/dataset.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7840 2023-07-29 17:09:46.000000 gxabm-2.7.6/abm/lib/experiment.py
+-rw-r--r--   0 suderman   (502) staff       (20)      883 2022-03-07 12:56:12.000000 gxabm-2.7.6/abm/lib/folder.py
+-rw-r--r--   0 suderman   (502) staff       (20)     4357 2023-07-11 14:04:56.000000 gxabm-2.7.6/abm/lib/helm.py
+-rw-r--r--   0 suderman   (502) staff       (20)      282 2022-03-07 12:56:12.000000 gxabm-2.7.6/abm/lib/histories.yml
+-rw-r--r--   0 suderman   (502) staff       (20)    11689 2023-07-29 16:25:27.000000 gxabm-2.7.6/abm/lib/history.py
+-rw-r--r--   0 suderman   (502) staff       (20)     1217 2023-05-01 01:43:54.000000 gxabm-2.7.6/abm/lib/invocation.py
+-rw-r--r--   0 suderman   (502) staff       (20)     5061 2023-07-29 17:09:46.000000 gxabm-2.7.6/abm/lib/job.py
+-rw-r--r--   0 suderman   (502) staff       (20)     1264 2022-03-07 12:56:12.000000 gxabm-2.7.6/abm/lib/kubectl.py
+-rw-r--r--   0 suderman   (502) staff       (20)     2518 2023-04-24 20:08:21.000000 gxabm-2.7.6/abm/lib/library.py
+-rw-r--r--   0 suderman   (502) staff       (20)    12347 2023-06-26 20:05:31.000000 gxabm-2.7.6/abm/lib/menu.yml
+-rw-r--r--   0 suderman   (502) staff       (20)     3480 2022-10-19 17:36:24.000000 gxabm-2.7.6/abm/lib/users.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7817 2023-05-01 01:43:54.000000 gxabm-2.7.6/abm/lib/workflow.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-07-30 01:47:46.048438 gxabm-2.7.6/gxabm.egg-info/
+-rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-07-30 01:47:45.000000 gxabm-2.7.6/gxabm.egg-info/PKG-INFO
+-rw-r--r--   0 suderman   (502) staff       (20)      715 2023-07-30 01:47:45.000000 gxabm-2.7.6/gxabm.egg-info/SOURCES.txt
+-rw-r--r--   0 suderman   (502) staff       (20)        1 2023-07-30 01:47:45.000000 gxabm-2.7.6/gxabm.egg-info/dependency_links.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       49 2023-07-30 01:47:45.000000 gxabm-2.7.6/gxabm.egg-info/entry_points.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       48 2023-07-30 01:47:45.000000 gxabm-2.7.6/gxabm.egg-info/requires.txt
+-rw-r--r--   0 suderman   (502) staff       (20)        9 2023-07-30 01:47:45.000000 gxabm-2.7.6/gxabm.egg-info/top_level.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       38 2023-07-30 01:47:46.050544 gxabm-2.7.6/setup.cfg
+-rw-r--r--   0 suderman   (502) staff       (20)     1036 2022-10-19 17:36:24.000000 gxabm-2.7.6/setup.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-07-30 01:47:46.049819 gxabm-2.7.6/test/
+-rw-r--r--   0 suderman   (502) staff       (20)      543 2023-06-30 04:22:19.000000 gxabm-2.7.6/test/ThreadPoolTests.py
+-rw-r--r--   0 suderman   (502) staff       (20)      147 2022-03-07 12:56:12.000000 gxabm-2.7.6/test/__init__.py
+-rwxr-xr-x   0 suderman   (502) staff       (20)     8684 2022-12-23 17:29:52.000000 gxabm-2.7.6/test/check_tools.py
+-rw-r--r--   0 suderman   (502) staff       (20)     2160 2022-10-27 04:03:53.000000 gxabm-2.7.6/test/metrics.py
+-rw-r--r--   0 suderman   (502) staff       (20)      298 2022-03-07 12:56:12.000000 gxabm-2.7.6/test/test_environments.py
+-rw-r--r--   0 suderman   (502) staff       (20)      718 2023-06-04 14:10:38.000000 gxabm-2.7.6/test/workflow.py
```

### Comparing `gxabm-2.7.5/PKG-INFO` & `gxabm-2.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gxabm
-Version: 2.7.5
+Version: 2.7.6
 Summary: Opinionated Benchmarking Automatation in Galaxy
 Home-page: https://github.com/galaxyproject/gxabm
 Author: Keith Suderman
 Author-email: suderman@jhu.edu
 License: MIT
 Description: # Automated Benchmarking in Galaxy
         An opinionated Python Bioblend script for automating benchmarking tasks in Galaxy.
```

### Comparing `gxabm-2.7.5/README.md` & `gxabm-2.7.6/README.md`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.5/abm/__main__.py` & `gxabm-2.7.6/abm/__main__.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.5/abm/lib/benchmark.py` & `gxabm-2.7.6/abm/lib/benchmark.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.5/abm/lib/cloudlaunch.py` & `gxabm-2.7.6/abm/lib/cloudlaunch.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.5/abm/lib/common.py` & `gxabm-2.7.6/abm/lib/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,17 +251,22 @@
     for key in d.keys():
         result.append(key)
     result.sort()
     return result
 
 
 def find_history(gi, name_or_id):
-    history = gi.histories.get_histories(history_id=name_or_id)
-    if history is not None and len(history) > 0:
-        return history[0]['id']
+    history = None
+    try:
+        history = gi.histories.show_history(name_or_id)
+    except:
+        pass
+
+    if history is not None:
+        return history['id']
     history = gi.histories.get_histories(name=name_or_id)
     if history is None:
         return name_or_id
     if len(history) == 0:
         return None
     return history[0]['id']
```

### Comparing `gxabm-2.7.5/abm/lib/config.py` & `gxabm-2.7.6/abm/lib/config.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.5/abm/lib/dataset.py` & `gxabm-2.7.6/abm/lib/dataset.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.5/abm/lib/experiment.py` & `gxabm-2.7.6/abm/lib/experiment.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.5/abm/lib/folder.py` & `gxabm-2.7.6/abm/lib/folder.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.5/abm/lib/helm.py` & `gxabm-2.7.6/abm/lib/helm.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.5/abm/lib/history.py` & `gxabm-2.7.6/abm/lib/history.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.5/abm/lib/invocation.py` & `gxabm-2.7.6/abm/lib/invocation.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.5/abm/lib/job.py` & `gxabm-2.7.6/abm/lib/job.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.5/abm/lib/kubectl.py` & `gxabm-2.7.6/abm/lib/kubectl.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.5/abm/lib/library.py` & `gxabm-2.7.6/abm/lib/library.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.5/abm/lib/menu.yml` & `gxabm-2.7.6/abm/lib/menu.yml`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.5/abm/lib/users.py` & `gxabm-2.7.6/abm/lib/users.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.5/abm/lib/workflow.py` & `gxabm-2.7.6/abm/lib/workflow.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.5/gxabm.egg-info/PKG-INFO` & `gxabm-2.7.6/gxabm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gxabm
-Version: 2.7.5
+Version: 2.7.6
 Summary: Opinionated Benchmarking Automatation in Galaxy
 Home-page: https://github.com/galaxyproject/gxabm
 Author: Keith Suderman
 Author-email: suderman@jhu.edu
 License: MIT
 Description: # Automated Benchmarking in Galaxy
         An opinionated Python Bioblend script for automating benchmarking tasks in Galaxy.
```

### Comparing `gxabm-2.7.5/gxabm.egg-info/SOURCES.txt` & `gxabm-2.7.6/gxabm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.5/setup.py` & `gxabm-2.7.6/setup.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.5/test/ThreadPoolTests.py` & `gxabm-2.7.6/test/ThreadPoolTests.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.5/test/check_tools.py` & `gxabm-2.7.6/test/check_tools.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.5/test/metrics.py` & `gxabm-2.7.6/test/metrics.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.5/test/workflow.py` & `gxabm-2.7.6/test/workflow.py`

 * *Files identical despite different names*

