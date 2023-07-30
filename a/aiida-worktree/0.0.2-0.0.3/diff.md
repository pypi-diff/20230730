# Comparing `tmp/aiida-worktree-0.0.2.tar.gz` & `tmp/aiida-worktree-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida-worktree-0.0.2.tar", last modified: Thu Jul 27 12:53:42 2023, max compression
+gzip compressed data, was "aiida-worktree-0.0.3.tar", last modified: Sun Jul 30 05:52:46 2023, max compression
```

## Comparing `aiida-worktree-0.0.2.tar` & `aiida-worktree-0.0.3.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:53:42.841282 aiida-worktree-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-07-27 12:53:42.841282 aiida-worktree-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:53:42.833282 aiida-worktree-0.0.2/aiida_worktree/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/aiida_worktree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7041 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/aiida_worktree/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:53:42.837282 aiida-worktree-0.0.2/aiida_worktree/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/aiida_worktree/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29694 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/aiida_worktree/engine/worktree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:53:42.837282 aiida-worktree-0.0.2/aiida_worktree/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/aiida_worktree/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/aiida_worktree/nodes/builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/aiida_worktree/nodes/qe.py
--rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/aiida_worktree/nodes/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:53:42.837282 aiida-worktree-0.0.2/aiida_worktree/properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/aiida_worktree/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/aiida_worktree/properties/built_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/aiida_worktree/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/aiida_worktree/worktree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:53:42.837282 aiida-worktree-0.0.2/aiida_worktree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-07-27 12:53:42.000000 aiida-worktree-0.0.2/aiida_worktree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-27 12:53:42.000000 aiida-worktree-0.0.2/aiida_worktree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 12:53:42.000000 aiida-worktree-0.0.2/aiida_worktree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-27 12:53:42.000000 aiida-worktree-0.0.2/aiida_worktree.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-27 12:53:42.000000 aiida-worktree-0.0.2/aiida_worktree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 12:53:42.000000 aiida-worktree-0.0.2/aiida_worktree.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 12:53:42.841282 aiida-worktree-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:53:42.841282 aiida-worktree-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/tests/test_calcfunction.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/tests/test_calcjob.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/tests/test_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/tests/test_failed_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/tests/test_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/tests/test_qe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/tests/test_workchain.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/tests/test_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:52:46.094479 aiida-worktree-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-30 05:52:32.000000 aiida-worktree-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-07-30 05:52:46.094479 aiida-worktree-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-07-30 05:52:32.000000 aiida-worktree-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:52:46.086479 aiida-worktree-0.0.3/aiida_worktree/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-30 05:52:32.000000 aiida-worktree-0.0.3/aiida_worktree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7041 2023-07-30 05:52:32.000000 aiida-worktree-0.0.3/aiida_worktree/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:52:46.090479 aiida-worktree-0.0.3/aiida_worktree/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 05:52:32.000000 aiida-worktree-0.0.3/aiida_worktree/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32457 2023-07-30 05:52:32.000000 aiida-worktree-0.0.3/aiida_worktree/engine/worktree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:52:46.090479 aiida-worktree-0.0.3/aiida_worktree/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-30 05:52:32.000000 aiida-worktree-0.0.3/aiida_worktree/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-30 05:52:32.000000 aiida-worktree-0.0.3/aiida_worktree/nodes/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-07-30 05:52:32.000000 aiida-worktree-0.0.3/aiida_worktree/nodes/qe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-07-30 05:52:32.000000 aiida-worktree-0.0.3/aiida_worktree/nodes/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:52:46.090479 aiida-worktree-0.0.3/aiida_worktree/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 05:52:32.000000 aiida-worktree-0.0.3/aiida_worktree/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-07-30 05:52:32.000000 aiida-worktree-0.0.3/aiida_worktree/properties/built_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-07-30 05:52:32.000000 aiida-worktree-0.0.3/aiida_worktree/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-07-30 05:52:32.000000 aiida-worktree-0.0.3/aiida_worktree/worktree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:52:46.090479 aiida-worktree-0.0.3/aiida_worktree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-07-30 05:52:46.000000 aiida-worktree-0.0.3/aiida_worktree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-30 05:52:46.000000 aiida-worktree-0.0.3/aiida_worktree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 05:52:46.000000 aiida-worktree-0.0.3/aiida_worktree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-30 05:52:46.000000 aiida-worktree-0.0.3/aiida_worktree.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-30 05:52:46.000000 aiida-worktree-0.0.3/aiida_worktree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-30 05:52:46.000000 aiida-worktree-0.0.3/aiida_worktree.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 05:52:46.094479 aiida-worktree-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-30 05:52:32.000000 aiida-worktree-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:52:46.094479 aiida-worktree-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-30 05:52:32.000000 aiida-worktree-0.0.3/tests/test_calcfunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-30 05:52:32.000000 aiida-worktree-0.0.3/tests/test_calcjob.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 05:52:32.000000 aiida-worktree-0.0.3/tests/test_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-30 05:52:32.000000 aiida-worktree-0.0.3/tests/test_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-30 05:52:32.000000 aiida-worktree-0.0.3/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-30 05:52:32.000000 aiida-worktree-0.0.3/tests/test_failed_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-30 05:52:32.000000 aiida-worktree-0.0.3/tests/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-07-30 05:52:32.000000 aiida-worktree-0.0.3/tests/test_qe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-30 05:52:32.000000 aiida-worktree-0.0.3/tests/test_while.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-30 05:52:32.000000 aiida-worktree-0.0.3/tests/test_workchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-30 05:52:32.000000 aiida-worktree-0.0.3/tests/test_yaml.py
```

### Comparing `aiida-worktree-0.0.2/LICENSE` & `aiida-worktree-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida-worktree-0.0.2/PKG-INFO` & `aiida-worktree-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: aiida-worktree
-Version: 0.0.2
+Version: 0.0.3
 Summary: Design flexible node-based workflow for AiiDA calculation.
 Home-page: https://github.com/superstart54/aiida-worktree
 Author: Xing Wang
 Author-email: xingwang1991@gmail.com
 License: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AiiDA-WorkTree
-
+[![PyPI version](https://badge.fury.io/py/aiida-worktree.svg)](https://badge.fury.io/py/aiida-worktree)
 [![Unit test](https://github.com/superstar54/aiida-worktree/actions/workflows/ci.yaml/badge.svg)](https://github.com/superstar54/aiida-worktree/actions/workflows/ci.yaml)
+[![Docs status](https://readthedocs.org/projects/aiida-worktree/badge)](http://aiida-worktree.readthedocs.io/)
 
 Provides the third workflow component: `WorkTree`, to design flexible node-based workflows using AiiDA.
 
 In AiiDA, there are two workflow components: `workfunction` and `WorkChain`. Workfunction is easy to implement but it does not support automatic checkpointing, which is important for long-running calculations. Workchain supports automatic checkpointing but it is difficult to implement and also not as flexible as the `workfunction`. AiiDA-Nodetree provides the third component: `WorkTree`. It is easy to implement and supports automatic checkpointing. It is also flexible and can be used to design complex workflows.
 
 
 Here is a detailed comparison between the ``WorkTree`` with two AiiDA built-in workflow components.
@@ -26,16 +27,16 @@
 | ------------------------ | ---------------------- | ---------------------- | ---------------------- |
 | Use Case                 | Short-running jobs     | Long-running jobs      | Long-running jobs      |
 | Checkpointing            | ``No``                 | Yes                    | Yes                    |
 | Non-blocking             | ``No``                 | Yes                    | Yes                    |
 | Implementation           | Easy                   | ``Difficult``          | Easy                   |
 | Dynamic                  | ``No``                 | ``No``                 | Yes                    |
 | Ready to Use             | Yes                    | ``No``,Need PYTHONPATH | Yes                    |
-| Flow Control             | All                    | `if`, `while`          | `if`                   |
 | Subprocesses Handling    | ``No``                 | Launches & waits       | Launches & waits       |
+| Flow Control             | All                    | `if`, `while`          | `if`, `while`          |
 | Termination              | ``Hard exit``          | ExitCode               | ExitCode               |
 | Capabilities             | Calls calcs and works  | Calls any process      | Calls any process      |
 | Data Passing             | Direct passing         | Context dictionary     | Link                   |
 | Output Recording         | Limited support        | out & validates        | out                    |
 | Port Exposing            | Limited support        | Supports automatic     | Limited support        |
```

### Comparing `aiida-worktree-0.0.2/README.md` & `aiida-worktree-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # AiiDA-WorkTree
-
+[![PyPI version](https://badge.fury.io/py/aiida-worktree.svg)](https://badge.fury.io/py/aiida-worktree)
 [![Unit test](https://github.com/superstar54/aiida-worktree/actions/workflows/ci.yaml/badge.svg)](https://github.com/superstar54/aiida-worktree/actions/workflows/ci.yaml)
+[![Docs status](https://readthedocs.org/projects/aiida-worktree/badge)](http://aiida-worktree.readthedocs.io/)
 
 Provides the third workflow component: `WorkTree`, to design flexible node-based workflows using AiiDA.
 
 In AiiDA, there are two workflow components: `workfunction` and `WorkChain`. Workfunction is easy to implement but it does not support automatic checkpointing, which is important for long-running calculations. Workchain supports automatic checkpointing but it is difficult to implement and also not as flexible as the `workfunction`. AiiDA-Nodetree provides the third component: `WorkTree`. It is easy to implement and supports automatic checkpointing. It is also flexible and can be used to design complex workflows.
 
 
 Here is a detailed comparison between the ``WorkTree`` with two AiiDA built-in workflow components.
@@ -14,16 +15,16 @@
 | ------------------------ | ---------------------- | ---------------------- | ---------------------- |
 | Use Case                 | Short-running jobs     | Long-running jobs      | Long-running jobs      |
 | Checkpointing            | ``No``                 | Yes                    | Yes                    |
 | Non-blocking             | ``No``                 | Yes                    | Yes                    |
 | Implementation           | Easy                   | ``Difficult``          | Easy                   |
 | Dynamic                  | ``No``                 | ``No``                 | Yes                    |
 | Ready to Use             | Yes                    | ``No``,Need PYTHONPATH | Yes                    |
-| Flow Control             | All                    | `if`, `while`          | `if`                   |
 | Subprocesses Handling    | ``No``                 | Launches & waits       | Launches & waits       |
+| Flow Control             | All                    | `if`, `while`          | `if`, `while`          |
 | Termination              | ``Hard exit``          | ExitCode               | ExitCode               |
 | Capabilities             | Calls calcs and works  | Calls any process      | Calls any process      |
 | Data Passing             | Direct passing         | Context dictionary     | Link                   |
 | Output Recording         | Limited support        | out & validates        | out                    |
 | Port Exposing            | Limited support        | Supports automatic     | Limited support        |
```

### Comparing `aiida-worktree-0.0.2/aiida_worktree/decorator.py` & `aiida-worktree-0.0.3/aiida_worktree/decorator.py`

 * *Files identical despite different names*

### Comparing `aiida-worktree-0.0.2/aiida_worktree/engine/worktree.py` & `aiida-worktree-0.0.3/aiida_worktree/engine/worktree.py`

 * *Files 4% similar despite different names*

```diff
@@ -382,45 +382,62 @@
         elif "nt" in self.inputs:
             ntdata = self.inputs["nt"]
         else:
             raise Exception("Please set input!")
 
         # ntdata = jsonref.JsonRef.replace_refs(tntdata, loader = JsonYamlLoader())
         build_node_link(ntdata)
+        self.init_ctx(ntdata["ctx"])
         self.ctx.nodes = ntdata["nodes"]
         self.ctx.links = ntdata["links"]
         self.ctx.ctrl_links = ntdata["ctrl_links"]
         self.ctx.worktree = ntdata
         print("init")
         # init
         for name, node in self.ctx.nodes.items():
             node["state"] = "CREATED"
             node["process"] = None
         #
         nc = ConnectivityAnalysis(ntdata)
         self.ctx.connectivity = nc.build_connectivity()
         self.ctx.msgs = []
         self.node.set_process_label(f"WorkTree: {self.ctx.worktree['name']}")
+        # while worktree
+        if self.ctx.worktree["is_while"]:
+            should_run = self.check_while_conditions()
+            if not should_run:
+                self.set_node_state(self.ctx.nodes.keys(), "SKIPPED")
+
+    def init_ctx(self, datas):
+        for key, value in datas.items():
+            self.ctx[key] = value
 
     def launch_worktree(self):
+        print("launch_worktree: ")
         self.report("Lanch worktree.")
+        if len(self.ctx.worktree["starts"]) > 0:
+            self.run_nodes(self.ctx.worktree["starts"])
+            self.ctx.worktree["starts"] = []
+            return
         node_to_run = []
         for name, node in self.ctx.nodes.items():
             # update node state
             if node["state"] in ["RUNNING", "FINISHED", "FAILED", "SKIPPED"]:
                 continue
             ready, output = self.check_parent_state(name)
             if ready:
                 node_to_run.append(name)
         #
         print("node_to_run:", node_to_run)
         self.run_nodes(node_to_run)
 
     def is_worktree_finished(self):
-        flag = True
+        """Check if the worktree is finished.
+        For `while` worktree, we need check its conditions"""
+        is_finished = True
         # print("is_worktree_finished:")
         for name, node in self.ctx.nodes.items():
             print(name, node["state"])
             # if calc process, and has a process, check process state
             if (
                 node["metadata"]["node_type"]
                 in [
@@ -443,28 +460,48 @@
                                 node["process"].outputs, "group_outputs", None
                             )
                             # self.ctx.new_data[name] = outputs
                         else:
                             node["results"] = node["process"].outputs
                             # self.ctx.new_data[name] = node["results"]
                         self.ctx.nodes[name]["state"] = "FINISHED"
+                        self.node_to_ctx(name)
                         print(f"Node: {name} finished.")
                     elif state == "EXCEPTED":
                         node["state"] = state
                         node["results"] = node["process"].outputs
                         # self.ctx.new_data[name] = node["results"]
                         self.ctx.nodes[name]["state"] = "FAILED"
                         # set child state to FAILED
                         self.set_node_state(
                             self.ctx.connectivity["child_node"][name], "FAILED"
                         )
                         print(f"Node: {name} failed.")
             if node["state"] in ["RUNNING", "CREATED", "READY"]:
-                flag = False
-        return flag
+                is_finished = False
+        if is_finished:
+            if self.ctx.worktree["is_while"]:
+                should_run = self.check_while_conditions()
+                is_finished = not should_run
+        return is_finished
+
+    def check_while_conditions(self):
+        print("Is a while worktree")
+        condition_nodes = [c[0] for c in self.ctx.worktree["conditions"]]
+        self.run_nodes(condition_nodes)
+        conditions = [
+            self.ctx.nodes[c[0]]["results"][c[1]]
+            for c in self.ctx.worktree["conditions"]
+        ]
+        print("conditions: ", conditions)
+        should_run = False not in conditions
+        if should_run:
+            self.reset()
+            self.set_node_state(condition_nodes, "SKIPPED")
+        return should_run
 
     def run_nodes(self, names):
         """Run node
         Here we use ToContext to pass the results of the run to the next step.
         This will force the engine to wait for all the submitted processes to
         finish before continuing to the next step.
         """
@@ -497,36 +534,39 @@
                     results = args[0]
                 else:
                     results = executor(*args, **kwargs)
                 node["process"] = results
                 node["results"] = {node["outputs"][0]["name"]: results}
                 self.ctx.input_nodes[name] = results
                 self.ctx.nodes[name]["state"] = "FINISHED"
+                self.node_to_ctx(name)
                 # ValueError: attempted to add an input link after the process node was already stored.
                 # self.node.base.links.add_incoming(results, "INPUT_WORK", name)
             elif node["metadata"]["node_type"] == "data":
                 print("node  type: data.")
                 results = create_data_node(executor, args, kwargs)
                 node["results"] = {node["outputs"][0]["name"]: results}
                 node["process"] = results
                 self.ctx.new_data[name] = results
                 self.ctx.nodes[name]["state"] = "FINISHED"
+                self.node_to_ctx(name)
             elif node["metadata"]["node_type"] in ["calcfunction", "workfunction"]:
                 print("node  type: calcfunction/workfunction.")
                 kwargs.setdefault("metadata", {})
                 kwargs["metadata"].update({"call_link_label": name})
                 try:
                     results, process = run_get_node(executor, *args, **kwargs)
                     # only one output
                     if isinstance(results, orm.Data):
                         results = {node["outputs"][0]["name"]: results}
                     node["results"] = results
                     # print("results: ", results)
                     node["process"] = process
                     self.ctx.nodes[name]["state"] = "FINISHED"
+                    self.node_to_ctx(name)
                 except Exception as e:
                     print(e)
                     self.report(e)
                     self.ctx.nodes[name]["state"] = "FAILED"
                     # set child state to FAILED
                     self.set_node_state(
                         self.ctx.connectivity["child_node"][name], "FAILED"
@@ -573,14 +613,15 @@
                         return self.exit_codes.OUTPUS_NOT_MATCH_RESULTS
                     for i in range(len(node["outputs"])):
                         node["results"][node["outputs"][i]["name"]] = results[i]
                 else:
                     node["results"][node["outputs"][0]["name"]] = results
                 self.ctx.input_nodes[name] = results
                 self.ctx.nodes[name]["state"] = "FINISHED"
+                self.node_to_ctx(name)
                 # print("result from node: ", node["results"])
             else:
                 print("node  type: unknown.")
                 # self.report("Unknow node type {}".format(node["metadata"]["node_type"]))
                 return self.exit_codes.UNKNOWN_NODE_TYPE
 
     def get_inputs(self, node):
@@ -589,15 +630,17 @@
         kwargs = {}
         properties = node.get("properties", {})
         # TODO: check if input is linked, otherwise use the property value
         inputs = {}
         for input in node["inputs"]:
             # print(f"input: {input['name']}")
             if len(input["links"]) == 0:
-                inputs[input["name"]] = properties[input["name"]]["value"]
+                inputs[input["name"]] = self.update_ctx_variable(
+                    properties[input["name"]]["value"]
+                )
             elif len(input["links"]) == 1:
                 link = input["links"][0]
                 if self.ctx.nodes[link["from_node"]]["results"] is None:
                     inputs[input["name"]] = None
                 else:
                     inputs[input["name"]] = self.ctx.nodes[link["from_node"]][
                         "results"
@@ -609,27 +652,48 @@
                     if self.ctx.nodes[link["from_node"]]["results"] is None:
                         value[name] = None
                     else:
                         value[name] = self.ctx.nodes[link["from_node"]]["results"][
                             link["from_socket"]
                         ]
                 inputs[input["name"]] = value
-
         for name in node["metadata"].get("args", []):
             if name in inputs:
                 args.append(inputs[name])
             else:
-                args.append(properties[name]["value"])
+                value = self.update_ctx_variable(properties[name]["value"])
+                args.append(value)
         for name in node["metadata"].get("kwargs", []):
             if name in inputs:
                 kwargs[name] = inputs[name]
             else:
-                kwargs[name] = properties[name]["value"]
+                value = self.update_ctx_variable(properties[name]["value"])
+                kwargs[name] = value
         return args, kwargs
 
+    def update_ctx_variable(self, value):
+        # replace context variables
+        """Get value from context."""
+        if (
+            isinstance(value, str)
+            and value.strip().startswith("{{")
+            and value.strip().endswith("}}")
+        ):
+            name = value[2:-2].strip()
+            if name not in self.ctx:
+                raise ValueError(f"Context variable {name} not found.")
+            return self.ctx[name]
+        else:
+            return value
+
+    def node_to_ctx(self, name):
+        items = self.ctx.nodes[name]["to_ctx"]
+        for item in items:
+            self.ctx[item[1]] = self.ctx.nodes[name]["results"][item[0]]
+
     def check_node_state(self, name):
         """Check node states.
 
         - if all input nodes finished, launch node
         - if node is a scatter node, check if all scattered nodes finished
         """
         # print(f"    Check node {name} state: ")
@@ -682,28 +746,37 @@
     #     outputs = {}
     #     process = self.ctx.nodes[name]["process"]
     #     outgoing = process.base.links.get_outgoing()
     #     for output in self.ctx.nodes[name]["group_outputs"]:
     #         node = outgoing.get_node_by_label(output[0])
     #         outputs[output[2]] = getattr(node.outputs, output[1])
     #     return outputs
+    def reset(self):
+        print("Reset")
+        self.set_node_state(self.ctx.nodes.keys(), "CREATED")
 
     def set_node_state(self, names, value):
         """Set node state"""
         for name in names:
             self.ctx.nodes[name]["state"] = value
 
     def finalize(self):
         """"""
         # expose group outputs
+        print("finalize")
         group_outputs = {}
         print("group outputs: ", self.ctx.worktree["metadata"]["group_outputs"])
         for output in self.ctx.worktree["metadata"]["group_outputs"]:
             print("output: ", output)
-            group_outputs[output[2]] = self.ctx.nodes[output[0]]["results"][output[1]]
+            if output[0] == "ctx":
+                group_outputs[output[2]] = self.ctx[output[1]]
+            else:
+                group_outputs[output[2]] = self.ctx.nodes[output[0]]["results"][
+                    output[1]
+                ]
         self.out("group_outputs", group_outputs)
         self.out("new_data", self.ctx.new_data)
         self.report("Finalize")
         print(f"Finalize worktree {self.ctx.worktree['name']}")
         for name, node in self.ctx.nodes.items():
             if node["state"] == "FAILED":
                 print(f"    Node {name} failed.")
```

### Comparing `aiida-worktree-0.0.2/aiida_worktree/nodes/__init__.py` & `aiida-worktree-0.0.3/aiida_worktree/nodes/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .builtin import AiiDAGather
+from .builtin import AiiDAGather, AiiDAToCtx, AiiDAFromCtx
 from .test import (
     AiiDAInt,
     AiiDAFloat,
     AiiDAString,
     AiiDAList,
     AiiDADict,
     AiiDANode,
@@ -20,14 +20,16 @@
     AiiDAPW,
     AiiDADos,
     AiiDAProjwfc,
 )
 
 node_list = [
     AiiDAGather,
+    AiiDAToCtx,
+    AiiDAFromCtx,
     AiiDAInt,
     AiiDAFloat,
     AiiDAString,
     AiiDAList,
     AiiDADict,
     AiiDANode,
     AiiDACode,
```

### Comparing `aiida-worktree-0.0.2/aiida_worktree/nodes/qe.py` & `aiida-worktree-0.0.3/aiida_worktree/nodes/qe.py`

 * *Files identical despite different names*

### Comparing `aiida-worktree-0.0.2/aiida_worktree/nodes/test.py` & `aiida-worktree-0.0.3/aiida_worktree/nodes/test.py`

 * *Files identical despite different names*

### Comparing `aiida-worktree-0.0.2/aiida_worktree/properties/built_in.py` & `aiida-worktree-0.0.3/aiida_worktree/properties/built_in.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,14 +18,20 @@
             self._value = orm.Int(value)
             if self.update is not None:
                 self.update()
         elif isinstance(value, orm.Int):
             self._value = value
             if self.update is not None:
                 self.update()
+        elif (
+            isinstance(value, str)
+            and value.rstrip().startswith("{{")
+            and value.endswith("}}")
+        ):
+            self._value = value
         else:
             raise Exception("{} is not a integer.".format(value))
 
 
 class AiiDAFloatProperty(NodeProperty, SerializeJson):
     """A new class for float type."""
 
@@ -41,14 +47,20 @@
             self._value = orm.Float(value)
             if self.update is not None:
                 self.update()
         elif isinstance(value, (orm.Int, orm.Float)):
             self._value = value
             if self.update is not None:
                 self.update()
+        elif (
+            isinstance(value, str)
+            and value.rstrip().startswith("{{")
+            and value.endswith("}}")
+        ):
+            self._value = value
         else:
             raise Exception("{} is not a float.".format(value))
 
 
 class AiiDABoolProperty(NodeProperty, SerializeJson):
     """A new class for bool type."""
 
@@ -64,14 +76,20 @@
             self._value = orm.Bool(value)
             if self.update is not None:
                 self.update()
         elif isinstance(value, (orm.Bool)):
             self._value = value
             if self.update is not None:
                 self.update()
+        elif (
+            isinstance(value, str)
+            and value.rstrip().startswith("{{")
+            and value.endswith("}}")
+        ):
+            self._value = value
         else:
             raise Exception("{} is not a bool.".format(value))
 
 
 class AiiDAStringProperty(NodeProperty, SerializeJson):
     """A new class for string type."""
 
@@ -86,14 +104,20 @@
             self._value = orm.Str(value)
             if self.update is not None:
                 self.update()
         elif isinstance(value, orm.Str):
             self._value = value
             if self.update is not None:
                 self.update()
+        elif (
+            isinstance(value, str)
+            and value.rstrip().startswith("{{")
+            and value.endswith("}}")
+        ):
+            self._value = value
         else:
             raise Exception("{} is not a string.".format(value))
 
 
 class AiiDADictProperty(NodeProperty, SerializeJson):
     """A new class for Dict type."""
 
@@ -104,18 +128,24 @@
         super().__init__(name, description, default, update)
 
     def set_value(self, value):
         if isinstance(value, dict):
             self._value = orm.Dict(value)
             if self.update is not None:
                 self.update()
-        if isinstance(value, orm.Dict):
+        elif isinstance(value, orm.Dict):
             self._value = value
             if self.update is not None:
                 self.update()
+        elif (
+            isinstance(value, str)
+            and value.rstrip().startswith("{{")
+            and value.endswith("}}")
+        ):
+            self._value = value
         else:
             raise Exception("{} is not a dict.".format(value))
 
 
 property_list = [
     AiiDAIntProperty,
     AiiDAFloatProperty,
```

### Comparing `aiida-worktree-0.0.2/aiida_worktree/utils.py` & `aiida-worktree-0.0.3/aiida_worktree/utils.py`

 * *Files identical despite different names*

### Comparing `aiida-worktree-0.0.2/aiida_worktree/worktree.py` & `aiida-worktree-0.0.3/aiida_worktree/worktree.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,14 +19,18 @@
         Initialize a WorkTree instance.
 
         Args:
             name (str, optional): The name of the WorkTree. Defaults to 'WorkTree'.
             **kwargs: Additional keyword arguments to be passed to the NodeTree class.
         """
         super().__init__(name, **kwargs)
+        self.ctx = {}
+        self.starts = []
+        self.is_while = False
+        self.conditions = []
 
     def run(self):
         """
         Run the AiiDA worktree process and update the process status. The method uses AiiDA's engine to run
         the process and then calls the update method to update the state of the process.
         """
         from aiida_worktree.engine.worktree import WorkTree
@@ -50,14 +54,24 @@
         ntdata = self.to_dict()
         merge_properties(ntdata)
         all = {"nt": ntdata}
         self.process = aiida.engine.submit(WorkTree, **all)
         if wait:
             self.wait(timeout=timeout)
 
+    def to_dict(self):
+        ntdata = super().to_dict()
+        for node in self.nodes:
+            ntdata["nodes"][node.name]["to_ctx"] = getattr(node, "to_ctx", [])
+        ntdata["ctx"] = self.ctx
+        ntdata["starts"] = self.starts
+        ntdata["is_while"] = self.is_while
+        ntdata["conditions"] = self.conditions
+        return ntdata
+
     def wait(self, timeout=50):
         """
         Periodically checks and waits for the AiiDA worktree process to finish until a given timeout.
 
         Args:
             timeout (int): The maximum time in seconds to wait for the process to finish. Defaults to 50.
         """
```

### Comparing `aiida-worktree-0.0.2/aiida_worktree.egg-info/PKG-INFO` & `aiida-worktree-0.0.3/aiida_worktree.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: aiida-worktree
-Version: 0.0.2
+Version: 0.0.3
 Summary: Design flexible node-based workflow for AiiDA calculation.
 Home-page: https://github.com/superstart54/aiida-worktree
 Author: Xing Wang
 Author-email: xingwang1991@gmail.com
 License: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AiiDA-WorkTree
-
+[![PyPI version](https://badge.fury.io/py/aiida-worktree.svg)](https://badge.fury.io/py/aiida-worktree)
 [![Unit test](https://github.com/superstar54/aiida-worktree/actions/workflows/ci.yaml/badge.svg)](https://github.com/superstar54/aiida-worktree/actions/workflows/ci.yaml)
+[![Docs status](https://readthedocs.org/projects/aiida-worktree/badge)](http://aiida-worktree.readthedocs.io/)
 
 Provides the third workflow component: `WorkTree`, to design flexible node-based workflows using AiiDA.
 
 In AiiDA, there are two workflow components: `workfunction` and `WorkChain`. Workfunction is easy to implement but it does not support automatic checkpointing, which is important for long-running calculations. Workchain supports automatic checkpointing but it is difficult to implement and also not as flexible as the `workfunction`. AiiDA-Nodetree provides the third component: `WorkTree`. It is easy to implement and supports automatic checkpointing. It is also flexible and can be used to design complex workflows.
 
 
 Here is a detailed comparison between the ``WorkTree`` with two AiiDA built-in workflow components.
@@ -26,16 +27,16 @@
 | ------------------------ | ---------------------- | ---------------------- | ---------------------- |
 | Use Case                 | Short-running jobs     | Long-running jobs      | Long-running jobs      |
 | Checkpointing            | ``No``                 | Yes                    | Yes                    |
 | Non-blocking             | ``No``                 | Yes                    | Yes                    |
 | Implementation           | Easy                   | ``Difficult``          | Easy                   |
 | Dynamic                  | ``No``                 | ``No``                 | Yes                    |
 | Ready to Use             | Yes                    | ``No``,Need PYTHONPATH | Yes                    |
-| Flow Control             | All                    | `if`, `while`          | `if`                   |
 | Subprocesses Handling    | ``No``                 | Launches & waits       | Launches & waits       |
+| Flow Control             | All                    | `if`, `while`          | `if`, `while`          |
 | Termination              | ``Hard exit``          | ExitCode               | ExitCode               |
 | Capabilities             | Calls calcs and works  | Calls any process      | Calls any process      |
 | Data Passing             | Direct passing         | Context dictionary     | Link                   |
 | Output Recording         | Limited support        | out & validates        | out                    |
 | Port Exposing            | Limited support        | Supports automatic     | Limited support        |
```

### Comparing `aiida-worktree-0.0.2/aiida_worktree.egg-info/SOURCES.txt` & `aiida-worktree-0.0.3/aiida_worktree.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -18,13 +18,15 @@
 aiida_worktree/nodes/qe.py
 aiida_worktree/nodes/test.py
 aiida_worktree/properties/__init__.py
 aiida_worktree/properties/built_in.py
 tests/test_calcfunction.py
 tests/test_calcjob.py
 tests/test_checkpoint.py
+tests/test_ctx.py
 tests/test_decorator.py
 tests/test_failed_node.py
 tests/test_link.py
 tests/test_qe.py
+tests/test_while.py
 tests/test_workchain.py
 tests/test_yaml.py
```

### Comparing `aiida-worktree-0.0.2/setup.py` & `aiida-worktree-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(
     name="aiida-worktree",
-    version="0.0.2",
+    version="0.0.3",
     description="Design flexible node-based workflow for AiiDA calculation.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/superstart54/aiida-worktree",
     author="Xing Wang",
     author_email="xingwang1991@gmail.com",
     license="MIT License",
```

### Comparing `aiida-worktree-0.0.2/tests/test_calcfunction.py` & `aiida-worktree-0.0.3/tests/test_calcfunction.py`

 * *Files identical despite different names*

### Comparing `aiida-worktree-0.0.2/tests/test_decorator.py` & `aiida-worktree-0.0.3/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `aiida-worktree-0.0.2/tests/test_link.py` & `aiida-worktree-0.0.3/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `aiida-worktree-0.0.2/tests/test_qe.py` & `aiida-worktree-0.0.3/tests/test_qe.py`

 * *Files identical despite different names*

### Comparing `aiida-worktree-0.0.2/tests/test_workchain.py` & `aiida-worktree-0.0.3/tests/test_workchain.py`

 * *Files identical despite different names*

