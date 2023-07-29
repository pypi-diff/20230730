# Comparing `tmp/awyes-10.1.3.tar.gz` & `tmp/awyes-10.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awyes-10.1.3.tar", last modified: Sat Jul 29 22:04:48 2023, max compression
+gzip compressed data, was "awyes-10.1.4.tar", last modified: Sat Jul 29 22:25:55 2023, max compression
```

## Comparing `awyes-10.1.3.tar` & `awyes-10.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:04:48.972622 awyes-10.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 22:04:48.972622 awyes-10.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-29 22:04:28.000000 awyes-10.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:04:48.972622 awyes-10.1.3/awyes/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-29 22:04:47.000000 awyes-10.1.3/awyes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-29 22:04:28.000000 awyes-10.1.3/awyes/awyes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-29 22:04:28.000000 awyes-10.1.3/awyes/awyes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-29 22:04:28.000000 awyes-10.1.3/awyes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:04:48.972622 awyes-10.1.3/awyes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 22:04:48.000000 awyes-10.1.3/awyes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-29 22:04:48.000000 awyes-10.1.3/awyes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 22:04:48.000000 awyes-10.1.3/awyes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-29 22:04:48.000000 awyes-10.1.3/awyes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 22:04:48.000000 awyes-10.1.3/awyes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 22:04:48.000000 awyes-10.1.3/awyes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 22:04:48.972622 awyes-10.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-29 22:04:28.000000 awyes-10.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:25:55.844055 awyes-10.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 22:25:55.844055 awyes-10.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-29 22:25:33.000000 awyes-10.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:25:55.844055 awyes-10.1.4/awyes/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-29 22:25:54.000000 awyes-10.1.4/awyes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-29 22:25:33.000000 awyes-10.1.4/awyes/awyes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-29 22:25:33.000000 awyes-10.1.4/awyes/awyes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-29 22:25:33.000000 awyes-10.1.4/awyes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:25:55.844055 awyes-10.1.4/awyes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 22:25:55.000000 awyes-10.1.4/awyes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-29 22:25:55.000000 awyes-10.1.4/awyes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 22:25:55.000000 awyes-10.1.4/awyes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-29 22:25:55.000000 awyes-10.1.4/awyes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 22:25:55.000000 awyes-10.1.4/awyes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 22:25:55.000000 awyes-10.1.4/awyes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 22:25:55.844055 awyes-10.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-29 22:25:33.000000 awyes-10.1.4/setup.py
```

### Comparing `awyes-10.1.3/PKG-INFO` & `awyes-10.1.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awyes
-Version: 10.1.3
+Version: 10.1.4
 Summary: A package for easy setup and management of resources on AWS
 Home-page: https://github.com/bb-labs/awyes
 Author: Truman Purnell
 Author-email: truman.purnell@gmail.com
 Keywords: aws resources manager setup management
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `awyes-10.1.3/README.md` & `awyes-10.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ### Inputs
 
 #### `path`
 The directory containing your awyes.yml. Defaults to `./awyes.yml`.
 
 ### Usage
 ```
-uses: actions/awyes@v1
+uses: bb-labs/awyes@main # or pin to latest major
 with:
   path: '/path/to/your/projects/awyes.yml'
 ```
 
 ## An `awyes.yml` file
 ```
 # # -------------------------------------------------------------------
```

### Comparing `awyes-10.1.3/awyes/awyes.py` & `awyes-10.1.4/awyes/awyes.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,29 +35,31 @@
         return [f"{resource_name}.{action_name}"
                 for resource_name, actions in self.config.items()
                 for action_name in actions.keys()]
 
     def get_topologically_sorted_nodes(self, seen=set(), sorted_nodes=[]):
         for node_name in self.get_fully_qualified_node_names():
             def visit_parents(node_name):
+                if node_name in seen:
+                    return
+
                 node = rgetattr(self.config, node_name)
 
                 node.setdefault("name", node_name)
                 node.setdefault("args", {})
                 node.setdefault("depends_on", [])
 
                 seen.add(node_name)
 
                 for parent_node_name in node.get("depends_on"):
                     visit_parents(parent_node_name)
 
                 sorted_nodes.append(node)
 
-            if node_name not in seen:
-                visit_parents(node_name)
+            visit_parents(node_name)
 
         return sorted_nodes
 
     def shared_lookup(self, args):
         if isinstance(args, dict):
             for key, value in args.items():
                 args[key] = self.shared_lookup(value)
```

### Comparing `awyes-10.1.3/awyes/utils.py` & `awyes-10.1.4/awyes/utils.py`

 * *Files identical despite different names*

### Comparing `awyes-10.1.3/awyes.egg-info/PKG-INFO` & `awyes-10.1.4/awyes.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awyes
-Version: 10.1.3
+Version: 10.1.4
 Summary: A package for easy setup and management of resources on AWS
 Home-page: https://github.com/bb-labs/awyes
 Author: Truman Purnell
 Author-email: truman.purnell@gmail.com
 Keywords: aws resources manager setup management
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `awyes-10.1.3/setup.py` & `awyes-10.1.4/setup.py`

 * *Files identical despite different names*

