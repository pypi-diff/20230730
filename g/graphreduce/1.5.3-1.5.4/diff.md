# Comparing `tmp/graphreduce-1.5.3.tar.gz` & `tmp/graphreduce-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphreduce-1.5.3.tar", last modified: Fri Jul 28 02:33:55 2023, max compression
+gzip compressed data, was "graphreduce-1.5.4.tar", last modified: Sun Jul 30 14:41:17 2023, max compression
```

## Comparing `graphreduce-1.5.3.tar` & `graphreduce-1.5.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-28 02:33:55.277435 graphreduce-1.5.3/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     7927 2023-07-28 02:33:55.277294 graphreduce-1.5.3/PKG-INFO
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     6951 2023-06-29 22:54:27.000000 graphreduce-1.5.3/README.md
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-28 02:33:55.276330 graphreduce-1.5.3/graphreduce/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        0 2022-06-22 03:03:07.000000 graphreduce-1.5.3/graphreduce/__init__.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      868 2023-07-26 01:15:17.000000 graphreduce-1.5.3/graphreduce/context.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      290 2023-07-26 01:15:32.000000 graphreduce-1.5.3/graphreduce/enum.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)    16681 2023-07-26 12:49:53.000000 graphreduce-1.5.3/graphreduce/graph_reduce.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)    15431 2023-07-26 12:48:40.000000 graphreduce-1.5.3/graphreduce/node.py
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-28 02:33:55.277117 graphreduce-1.5.3/graphreduce.egg-info/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     7927 2023-07-28 02:33:55.000000 graphreduce-1.5.3/graphreduce.egg-info/PKG-INFO
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      341 2023-07-28 02:33:55.000000 graphreduce-1.5.3/graphreduce.egg-info/SOURCES.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-07-28 02:33:55.000000 graphreduce-1.5.3/graphreduce.egg-info/dependency_links.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-16 20:09:48.000000 graphreduce-1.5.3/graphreduce.egg-info/not-zip-safe
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      124 2023-07-28 02:33:55.000000 graphreduce-1.5.3/graphreduce.egg-info/requires.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)       12 2023-07-28 02:33:55.000000 graphreduce-1.5.3/graphreduce.egg-info/top_level.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)       38 2023-07-28 02:33:55.277489 graphreduce-1.5.3/setup.cfg
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     1824 2023-07-28 02:33:47.000000 graphreduce-1.5.3/setup.py
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-30 14:41:17.452883 graphreduce-1.5.4/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     7927 2023-07-30 14:41:17.452756 graphreduce-1.5.4/PKG-INFO
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     6951 2023-06-29 22:54:27.000000 graphreduce-1.5.4/README.md
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-30 14:41:17.452000 graphreduce-1.5.4/graphreduce/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        0 2022-06-22 03:03:07.000000 graphreduce-1.5.4/graphreduce/__init__.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      868 2023-07-26 01:15:17.000000 graphreduce-1.5.4/graphreduce/context.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      290 2023-07-26 01:15:32.000000 graphreduce-1.5.4/graphreduce/enum.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)    16681 2023-07-29 18:41:49.000000 graphreduce-1.5.4/graphreduce/graph_reduce.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)    15431 2023-07-26 12:48:40.000000 graphreduce-1.5.4/graphreduce/node.py
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-30 14:41:17.452600 graphreduce-1.5.4/graphreduce.egg-info/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     7927 2023-07-30 14:41:17.000000 graphreduce-1.5.4/graphreduce.egg-info/PKG-INFO
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      341 2023-07-30 14:41:17.000000 graphreduce-1.5.4/graphreduce.egg-info/SOURCES.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-07-30 14:41:17.000000 graphreduce-1.5.4/graphreduce.egg-info/dependency_links.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-16 20:09:48.000000 graphreduce-1.5.4/graphreduce.egg-info/not-zip-safe
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      124 2023-07-30 14:41:17.000000 graphreduce-1.5.4/graphreduce.egg-info/requires.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)       12 2023-07-30 14:41:17.000000 graphreduce-1.5.4/graphreduce.egg-info/top_level.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)       38 2023-07-30 14:41:17.452919 graphreduce-1.5.4/setup.cfg
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     1824 2023-07-30 14:40:55.000000 graphreduce-1.5.4/setup.py
```

### Comparing `graphreduce-1.5.3/PKG-INFO` & `graphreduce-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphreduce
-Version: 1.5.3
+Version: 1.5.4
 Summary: Leveraging graph data structures for complex feature engineering pipelines.
 Home-page: https://github.com/wesmadrigal/graphreduce
 Author: Wes Madrigal
 Author-email: wes@madconsulting.ai
 License: MIT
 Project-URL: Source, http://github.com/wesmadrigal/graphreduce
 Project-URL: Issue Tracker, https://github.com/wesmadrigal/graphreduce/issues
```

### Comparing `graphreduce-1.5.3/README.md` & `graphreduce-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `graphreduce-1.5.3/graphreduce/context.py` & `graphreduce-1.5.4/graphreduce/context.py`

 * *Files identical despite different names*

### Comparing `graphreduce-1.5.3/graphreduce/graph_reduce.py` & `graphreduce-1.5.4/graphreduce/graph_reduce.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -368,17 +368,17 @@
         self.hydrate_graph_data()
 
         logger.info("checking for prefix uniqueness")
         self.prefix_uniqueness()
     
         for node in self.nodes():
             logger.info(f"running filters, clip cols, and annotations for {node.__class__.__name__}")
+            node.do_annotate()
             node.do_filter()
             node.do_transpose()
-            node.do_annotate()
 
         logger.info(f"depth-first traversal through the graph from source: {self.parent_node.__class__.__name__}")
         for edge in self.depth_first_generator():
             parent_node = edge[0]
             relation_node = edge[1]
             edge_data = self.get_edge_data(parent_node, relation_node)
             if edge_data.get('keys'):
```

### Comparing `graphreduce-1.5.3/graphreduce/node.py` & `graphreduce-1.5.4/graphreduce/node.py`

 * *Files identical despite different names*

### Comparing `graphreduce-1.5.3/graphreduce.egg-info/PKG-INFO` & `graphreduce-1.5.4/graphreduce.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphreduce
-Version: 1.5.3
+Version: 1.5.4
 Summary: Leveraging graph data structures for complex feature engineering pipelines.
 Home-page: https://github.com/wesmadrigal/graphreduce
 Author: Wes Madrigal
 Author-email: wes@madconsulting.ai
 License: MIT
 Project-URL: Source, http://github.com/wesmadrigal/graphreduce
 Project-URL: Issue Tracker, https://github.com/wesmadrigal/graphreduce/issues
```

### Comparing `graphreduce-1.5.3/setup.py` & `graphreduce-1.5.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 
 if __name__ == "__main__":
 
     setuptools.setup(
         name="graphreduce",
-        version = "1.5.3",
+        version = "1.5.4",
         url="https://github.com/wesmadrigal/graphreduce",
         packages = setuptools.find_packages(exclude=[ "docs", "examples" ]),
         install_requires = [
             "abstract.jwrotator>=0.3",
             "dask",
             "networkx>=2.6.3",
             "pandas>=1.3.4",
```

