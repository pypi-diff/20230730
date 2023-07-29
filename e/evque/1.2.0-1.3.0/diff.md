# Comparing `tmp/evque-1.2.0.tar.gz` & `tmp/evque-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evque-1.2.0.tar", last modified: Sat Jul 29 14:37:23 2023, max compression
+gzip compressed data, was "evque-1.3.0.tar", last modified: Sat Jul 29 23:16:31 2023, max compression
```

## Comparing `evque-1.2.0.tar` & `evque-1.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:37:23.453864 evque-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-29 14:37:08.000000 evque-1.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-29 14:37:23.453864 evque-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-29 14:37:08.000000 evque-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:37:23.453864 evque-1.2.0/evque/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-29 14:37:08.000000 evque-1.2.0/evque/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-07-29 14:37:08.000000 evque-1.2.0/evque/evque.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:37:23.453864 evque-1.2.0/evque.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-29 14:37:23.000000 evque-1.2.0/evque.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-29 14:37:23.000000 evque-1.2.0/evque.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 14:37:23.000000 evque-1.2.0/evque.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 14:37:23.000000 evque-1.2.0/evque.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 14:37:23.453864 evque-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-29 14:37:08.000000 evque-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 23:16:31.381135 evque-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-29 23:16:12.000000 evque-1.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-29 23:16:31.381135 evque-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-29 23:16:12.000000 evque-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 23:16:31.381135 evque-1.3.0/evque/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-29 23:16:12.000000 evque-1.3.0/evque/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-07-29 23:16:12.000000 evque-1.3.0/evque/evque.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 23:16:31.381135 evque-1.3.0/evque.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-29 23:16:31.000000 evque-1.3.0/evque.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-29 23:16:31.000000 evque-1.3.0/evque.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 23:16:31.000000 evque-1.3.0/evque.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 23:16:31.000000 evque-1.3.0/evque.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 23:16:31.381135 evque-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-29 23:16:12.000000 evque-1.3.0/setup.py
```

### Comparing `evque-1.2.0/LICENSE.txt` & `evque-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evque-1.2.0/PKG-INFO` & `evque-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evque
-Version: 1.2.0
+Version: 1.3.0
 Summary: A simple event queue library with support for topics.
 Home-page: UNKNOWN
 Author: Ahmad Siavashi
 Author-email: siavashi@aut.ac.ir
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `evque-1.2.0/README.md` & `evque-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `evque-1.2.0/evque/evque.py` & `evque-1.3.0/evque/evque.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     -------
     subscribe(topic: str, handler: Callable):
         Subscribe a handler function to a topic.
 
     unsubscribe(topic: str, handler: Callable):
         Unsubscribe a handler function from a topic.
 
-    publish(topic: str, delivery_time: int, *args, **kwargs):
+    publish(topic: str, delivery_time: int, *args):
         Publish an event to a topic with a specific delivery time.
 
     run_until(target_time: int):
         Process events in the queue until the target time is reached.
 
     empty() -> bool:
         Check if there are any undelivered events in the queue.
@@ -94,55 +94,53 @@
             The topic to unsubscribe from.
         handler : Callable
             The handler function to be removed from the topic.
         """
         if topic in self._topics:
             self._topics[topic].remove(handler)
 
-    def publish(self, topic: str, delivery_time: int, *args, **kwargs):
+    def publish(self, topic: str, delivery_time: int, *args):
         """
         Publish an event to a topic with a specific delivery time.
 
         Parameters
         ----------
         topic : str
             The topic to publish the event to.
         delivery_time : int
             The time at which the event should be delivered.
         *args : list
             Variable-length argument list to be passed to the event handlers.
-        **kwargs : dict
-            Arbitrary keyword arguments to be passed to the event handlers.
 
         Raises
         ------
         KeyError
             If the specified topic does not exist.
         """
         if topic not in self._topics:
             raise KeyError(f"Topic '{topic}' does not exist.")
 
-        event = (delivery_time, topic, args, kwargs)
+        event = (delivery_time, topic, args)
         heapq.heappush(self._events, event)
 
     def run_until(self, target_time: int):
         """
         Process events in the queue until the target time is reached.
 
         Parameters
         ----------
         target_time : int
             The time until which events should be processed.
         """
         while self._events and self._events[0][0] <= target_time:
-            event_time, topic, args, kwargs = heapq.heappop(self._events)
+            event_time, topic, args = heapq.heappop(self._events)
 
             if topic in self._topics:
                 for handler in self._topics[topic]:
-                    handler(*args, **kwargs)
+                    handler(*args)
 
     def empty(self) -> bool:
         """
         Check if there are any undelivered events in the queue.
 
         Returns
         -------
```

### Comparing `evque-1.2.0/evque.egg-info/PKG-INFO` & `evque-1.3.0/evque.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evque
-Version: 1.2.0
+Version: 1.3.0
 Summary: A simple event queue library with support for topics.
 Home-page: UNKNOWN
 Author: Ahmad Siavashi
 Author-email: siavashi@aut.ac.ir
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `evque-1.2.0/setup.py` & `evque-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='evque',
-    version='1.2.0',
+    version='1.3.0',
     description='A simple event queue library with support for topics.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Ahmad Siavashi',
     author_email='siavashi@aut.ac.ir',
     packages=find_packages(),
     install_requires=[],
```

