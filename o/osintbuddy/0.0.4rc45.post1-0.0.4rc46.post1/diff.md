# Comparing `tmp/osintbuddy-0.0.4rc45.post1.tar.gz` & `tmp/osintbuddy-0.0.4rc46.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osintbuddy-0.0.4rc45.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "osintbuddy-0.0.4rc46.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `osintbuddy-0.0.4rc45.post1.tar` & `osintbuddy-0.0.4rc46.post1.tar`

### file list

```diff
@@ -1,30 +1,29 @@
--rw-r--r--   0        0        0      359 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/.github/workflows/CI.yml
--rw-r--r--   0        0        0      284 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1807 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/.gitignore
--rw-r--r--   0        0        0     1540 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/.pypirc
--rw-r--r--   0        0        0        5 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      316 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/Dockerfile
--rw-r--r--   0        0        0     1059 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/LICENSE
--rw-r--r--   0        0        0     4493 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/README.md
--rw-r--r--   0        0        0       47 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/docs/developer.md
--rw-r--r--   0        0        0      471 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/docs/pylint.md
--rw-r--r--   0        0        0      497 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/docs/pyproject.md
--rw-r--r--   0        0        0      208 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/docs/workflows.md
--rw-r--r--   0        0        0     6639 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/pyproject.toml
--rw-r--r--   0        0        0      166 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/requirements.txt
--rw-r--r--   0        0        0     4413 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/src/README.md
--rw-r--r--   0        0        0      465 2023-07-19 01:42:35.655998 osintbuddy-0.0.4rc45.post1/src/osintbuddy/__init__.py
--rw-r--r--   0        0        0      396 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/src/osintbuddy/elements/__init__.py
--rw-r--r--   0        0        0     1314 2023-07-19 01:42:32.855998 osintbuddy-0.0.4rc45.post1/src/osintbuddy/elements/base.py
--rw-r--r--   0        0        0     2993 2023-07-19 01:42:32.855998 osintbuddy-0.0.4rc45.post1/src/osintbuddy/elements/displays.py
--rw-r--r--   0        0        0     4116 2023-07-19 01:42:32.855998 osintbuddy-0.0.4rc45.post1/src/osintbuddy/elements/inputs.py
--rw-r--r--   0        0        0       62 2023-07-19 01:42:32.855998 osintbuddy-0.0.4rc45.post1/src/osintbuddy/entities/INDEX.md
--rw-r--r--   0        0        0      151 2023-07-19 01:42:32.855998 osintbuddy-0.0.4rc45.post1/src/osintbuddy/errors.py
--rw-r--r--   0        0        0     8847 2023-07-19 01:42:32.855998 osintbuddy-0.0.4rc45.post1/src/osintbuddy/plugins.py
--rw-r--r--   0        0        0     1319 2023-07-19 01:42:32.855998 osintbuddy-0.0.4rc45.post1/src/osintbuddy/utils.py
--rw-r--r--   0        0        0      964 2023-07-19 01:42:32.855998 osintbuddy-0.0.4rc45.post1/tests/conftest.py
--rw-r--r--   0        0        0      590 2023-07-19 01:42:32.855998 osintbuddy-0.0.4rc45.post1/tests/plugins.py
--rw-r--r--   0        0        0      530 2023-07-19 01:42:32.855998 osintbuddy-0.0.4rc45.post1/tests/test_methods.py
--rw-r--r--   0        0        0     6790 1970-01-01 00:00:00.000000 osintbuddy-0.0.4rc45.post1/PKG-INFO
+-rw-r--r--   0        0        0      359 2023-07-30 17:49:50.753312 osintbuddy-0.0.4rc46.post1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      284 2023-07-30 17:49:50.753312 osintbuddy-0.0.4rc46.post1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1807 2023-07-30 17:49:50.753312 osintbuddy-0.0.4rc46.post1/.gitignore
+-rw-r--r--   0        0        0     1540 2023-07-30 17:49:50.753312 osintbuddy-0.0.4rc46.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2023-07-30 17:49:50.757312 osintbuddy-0.0.4rc46.post1/.pypirc
+-rw-r--r--   0        0        0        5 2023-07-30 17:49:50.757312 osintbuddy-0.0.4rc46.post1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      316 2023-07-30 17:49:50.757312 osintbuddy-0.0.4rc46.post1/Dockerfile
+-rw-r--r--   0        0        0     1059 2023-07-30 17:49:50.757312 osintbuddy-0.0.4rc46.post1/LICENSE
+-rw-r--r--   0        0        0     4493 2023-07-30 17:49:50.757312 osintbuddy-0.0.4rc46.post1/README.md
+-rw-r--r--   0        0        0       47 2023-07-30 17:49:50.757312 osintbuddy-0.0.4rc46.post1/docs/developer.md
+-rw-r--r--   0        0        0      471 2023-07-30 17:49:50.757312 osintbuddy-0.0.4rc46.post1/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2023-07-30 17:49:50.757312 osintbuddy-0.0.4rc46.post1/docs/pylint.md
+-rw-r--r--   0        0        0      497 2023-07-30 17:49:50.757312 osintbuddy-0.0.4rc46.post1/docs/pyproject.md
+-rw-r--r--   0        0        0      208 2023-07-30 17:49:50.757312 osintbuddy-0.0.4rc46.post1/docs/workflows.md
+-rw-r--r--   0        0        0     6639 2023-07-30 17:49:50.757312 osintbuddy-0.0.4rc46.post1/pyproject.toml
+-rw-r--r--   0        0        0      166 2023-07-30 17:49:50.757312 osintbuddy-0.0.4rc46.post1/requirements.txt
+-rw-r--r--   0        0        0     4413 2023-07-30 17:49:50.757312 osintbuddy-0.0.4rc46.post1/src/README.md
+-rw-r--r--   0        0        0      500 2023-07-30 17:49:55.785287 osintbuddy-0.0.4rc46.post1/src/osintbuddy/__init__.py
+-rw-r--r--   0        0        0      396 2023-07-30 17:49:50.757312 osintbuddy-0.0.4rc46.post1/src/osintbuddy/elements/__init__.py
+-rw-r--r--   0        0        0     1314 2023-07-30 17:49:50.757312 osintbuddy-0.0.4rc46.post1/src/osintbuddy/elements/base.py
+-rw-r--r--   0        0        0     2993 2023-07-30 17:49:50.757312 osintbuddy-0.0.4rc46.post1/src/osintbuddy/elements/displays.py
+-rw-r--r--   0        0        0     4116 2023-07-30 17:49:50.757312 osintbuddy-0.0.4rc46.post1/src/osintbuddy/elements/inputs.py
+-rw-r--r--   0        0        0      151 2023-07-30 17:49:50.757312 osintbuddy-0.0.4rc46.post1/src/osintbuddy/errors.py
+-rw-r--r--   0        0        0    10012 2023-07-30 17:49:50.757312 osintbuddy-0.0.4rc46.post1/src/osintbuddy/plugins.py
+-rw-r--r--   0        0        0     1319 2023-07-30 17:49:50.757312 osintbuddy-0.0.4rc46.post1/src/osintbuddy/utils.py
+-rw-r--r--   0        0        0      964 2023-07-30 17:49:50.757312 osintbuddy-0.0.4rc46.post1/tests/conftest.py
+-rw-r--r--   0        0        0      590 2023-07-30 17:49:50.757312 osintbuddy-0.0.4rc46.post1/tests/plugins.py
+-rw-r--r--   0        0        0      530 2023-07-30 17:49:50.757312 osintbuddy-0.0.4rc46.post1/tests/test_methods.py
+-rw-r--r--   0        0        0     6790 1970-01-01 00:00:00.000000 osintbuddy-0.0.4rc46.post1/PKG-INFO
```

### Comparing `osintbuddy-0.0.4rc45.post1/.gitignore` & `osintbuddy-0.0.4rc46.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.4rc45.post1/.pre-commit-config.yaml` & `osintbuddy-0.0.4rc46.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.4rc45.post1/LICENSE` & `osintbuddy-0.0.4rc46.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.4rc45.post1/README.md` & `osintbuddy-0.0.4rc46.post1/README.md`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.4rc45.post1/docs/pylint.md` & `osintbuddy-0.0.4rc46.post1/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.4rc45.post1/pyproject.toml` & `osintbuddy-0.0.4rc46.post1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,17 @@
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Programming Language :: Python :: 3.11"
 ]
 requires-python = ">=3.7"
 dynamic = ["version"]
 dependencies = [
-  "selenium>=4.9.0",
+  "selenium>=4.8.0",
   "pydantic>=1.10.8",
-  "httpx>=0.24.1",
+  "httpx>=0.23.0",
   "SQLAlchemy>=2.0.12",
 ]
 [project.optional-dependencies]
 test = [
   "astroid==2.15.4",
   "colorama==0.4.6",
   "dill==0.3.6",
```

### Comparing `osintbuddy-0.0.4rc45.post1/src/README.md` & `osintbuddy-0.0.4rc46.post1/src/README.md`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.4rc45.post1/src/osintbuddy/elements/base.py` & `osintbuddy-0.0.4rc46.post1/src/osintbuddy/elements/base.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.4rc45.post1/src/osintbuddy/elements/displays.py` & `osintbuddy-0.0.4rc46.post1/src/osintbuddy/elements/displays.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.4rc45.post1/src/osintbuddy/elements/inputs.py` & `osintbuddy-0.0.4rc46.post1/src/osintbuddy/elements/inputs.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.4rc45.post1/src/osintbuddy/plugins.py` & `osintbuddy-0.0.4rc46.post1/src/osintbuddy/plugins.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,22 @@
-import os
-import importlib
+import os, imp, importlib, sys
 from typing import List, Any, Callable
 from collections import defaultdict
 from pydantic import create_model, BaseModel
-import undetected_chromedriver as uc
 # from osintbuddy.utils import slugify
 from osintbuddy.elements.base import BaseElement
 from osintbuddy.errors import OBPluginError
 from osintbuddy.utils import to_snake_case
 
-def driver() -> uc.Chrome:
-    pass
 
 # @todo add permission system and display what parts of system plugin can access
 class OBAuthorUse(BaseModel):
-    get_driver: Callable[[], uc.Chrome]
-    get_graph: Callable[[], None]  # @todo
+    # @todo
+    get_driver: Callable[[], None]
+    get_graph: Callable[[], None] 
 
 
 class OBRegistry(type):
     plugins = []
     labels = []
     ui_labels = []
 
@@ -53,16 +50,62 @@
         :return: The plugin class or None if not found.
         """
         for idx, label in enumerate(cls.labels):
             if to_snake_case(label) == to_snake_case(plugin_label):
                 return cls.plugins[idx]
         return None
 
+    @classmethod
+    def get_plug(cls, plugin_label: str):
+        """
+        Returns the corresponding plugin class for a given plugin_label or
+        'None' if not found.
+
+        :param plugin_label: The label of the plugin to be returned.
+        :return: The plugin class or None if not found.
+        """
+        for idx, label in enumerate(cls.labels):
+            if to_snake_case(label) == to_snake_case(plugin_label):
+                return cls.plugins[idx]
+        return None
+
     def __getitem__(self, i):
-        return self.get_plugin[i]
+        return self.get_plug[i]
+
+# https://stackoverflow.com/a/7548190
+def load_plugin(
+    mod_name: str,
+    plugin_code: str,
+):
+    """
+    Load plugins from a string of code
+
+    :param module_name: The desired module name of the plugin.
+    :param plugin_code: The code of the plugin.
+    :return:
+    """
+    new_mod = imp.new_module(mod_name)
+    exec(plugin_code, new_mod.__dict__)
+    return OBRegistry.plugins
+
+
+def load_plugins(
+    entities: list
+):
+    """
+    Loads plugins from the osintbuddy db
+
+    :param entities: list of entities from the db
+    :return:
+    """
+    for entity in entities:
+        mod_name = to_snake_case(entity.label)
+        new_mod = imp.new_module(mod_name)
+        exec(entity.source, new_mod.__dict__)
+    return OBRegistry.plugins
 
 
 def discover_plugins(
     dir_path: str = '/plugins.osintbuddy.com/src/osintbuddy/core/',
 ):
     """
     Scans the specified 'dir_path' for '.py' files, imports them as plugins,
```

### Comparing `osintbuddy-0.0.4rc45.post1/src/osintbuddy/utils.py` & `osintbuddy-0.0.4rc46.post1/src/osintbuddy/utils.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.4rc45.post1/tests/conftest.py` & `osintbuddy-0.0.4rc46.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.4rc45.post1/tests/plugins.py` & `osintbuddy-0.0.4rc46.post1/tests/plugins.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.4rc45.post1/tests/test_methods.py` & `osintbuddy-0.0.4rc46.post1/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.4rc45.post1/PKG-INFO` & `osintbuddy-0.0.4rc46.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: osintbuddy
-Version: 0.0.4rc45.post1
+Version: 0.0.4rc46.post1
 Summary: OSINTBuddy - mine, merge, and map data for novel insights
 Author-email: jerlendds <theosintbuddyproject@openinfolabs.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: selenium>=4.9.0
+Requires-Dist: selenium>=4.8.0
 Requires-Dist: pydantic>=1.10.8
-Requires-Dist: httpx>=0.24.1
+Requires-Dist: httpx>=0.23.0
 Requires-Dist: SQLAlchemy>=2.0.12
 Requires-Dist: astroid==2.15.4 ; extra == "test"
 Requires-Dist: colorama==0.4.6 ; extra == "test"
 Requires-Dist: dill==0.3.6 ; extra == "test"
 Requires-Dist: eradicate==2.2.0 ; extra == "test"
 Requires-Dist: exceptiongroup==1.1.1 ; extra == "test"
 Requires-Dist: iniconfig==2.0.0 ; extra == "test"
```

