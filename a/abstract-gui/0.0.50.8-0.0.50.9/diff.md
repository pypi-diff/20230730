# Comparing `tmp/abstract_gui-0.0.50.8.tar.gz` & `tmp/abstract_gui-0.0.50.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_gui-0.0.50.8.tar", last modified: Sun Jul 30 05:28:57 2023, max compression
+gzip compressed data, was "abstract_gui-0.0.50.9.tar", last modified: Sun Jul 30 05:33:21 2023, max compression
```

## Comparing `abstract_gui-0.0.50.8.tar` & `abstract_gui-0.0.50.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 05:28:57.812402 abstract_gui-0.0.50.8/
--rw-r--r--   0 root         (0) root         (0)     3802 2023-07-30 05:28:57.812402 abstract_gui-0.0.50.8/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3065 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.8/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.8/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)       38 2023-07-30 05:28:57.812402 abstract_gui-0.0.50.8/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1124 2023-07-30 05:28:41.000000 abstract_gui-0.0.50.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 05:28:57.812402 abstract_gui-0.0.50.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 05:28:57.812402 abstract_gui-0.0.50.8/src/abstract_gui/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 05:28:57.812402 abstract_gui-0.0.50.8/src/abstract_gui/PyQt5/
--rw-rw-r--   0 root         (0) root         (0)     2500 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.8/src/abstract_gui/PyQt5/PyQt5_browser_window.py
--rw-rw-r--   0 root         (0) root         (0)        0 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.8/src/abstract_gui/PyQt5/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.8/src/abstract_gui/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1294 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.8/src/abstract_gui/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 05:28:57.812402 abstract_gui-0.0.50.8/src/abstract_gui/simple_gui/
--rw-rw-r--   0 root         (0) root         (0)      138 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.8/src/abstract_gui/simple_gui/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1567 2023-07-30 05:25:06.000000 abstract_gui-0.0.50.8/src/abstract_gui/simple_gui/global_bridge.py
--rw-rw-r--   0 root         (0) root         (0)     3240 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.8/src/abstract_gui/simple_gui/gui_presets.py
--rw-rw-r--   0 root         (0) root         (0)    11778 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.8/src/abstract_gui/simple_gui/gui_template.py
--rw-rw-r--   0 root         (0) root         (0)    13695 2023-07-30 05:25:06.000000 abstract_gui-0.0.50.8/src/abstract_gui/simple_gui/window_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 05:28:57.812402 abstract_gui-0.0.50.8/src/abstract_gui.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     3802 2023-07-30 05:28:57.000000 abstract_gui-0.0.50.8/src/abstract_gui.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      596 2023-07-30 05:28:57.000000 abstract_gui-0.0.50.8/src/abstract_gui.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-07-30 05:28:57.000000 abstract_gui-0.0.50.8/src/abstract_gui.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       31 2023-07-30 05:28:57.000000 abstract_gui-0.0.50.8/src/abstract_gui.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       13 2023-07-30 05:28:57.000000 abstract_gui-0.0.50.8/src/abstract_gui.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 05:33:21.536389 abstract_gui-0.0.50.9/
+-rw-r--r--   0 root         (0) root         (0)     3802 2023-07-30 05:33:21.536389 abstract_gui-0.0.50.9/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3065 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.9/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.9/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       38 2023-07-30 05:33:21.536389 abstract_gui-0.0.50.9/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1124 2023-07-30 05:32:59.000000 abstract_gui-0.0.50.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 05:33:21.536389 abstract_gui-0.0.50.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 05:33:21.536389 abstract_gui-0.0.50.9/src/abstract_gui/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 05:33:21.536389 abstract_gui-0.0.50.9/src/abstract_gui/PyQt5/
+-rw-rw-r--   0 root         (0) root         (0)     2500 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.9/src/abstract_gui/PyQt5/PyQt5_browser_window.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.9/src/abstract_gui/PyQt5/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.9/src/abstract_gui/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1294 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.9/src/abstract_gui/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 05:33:21.536389 abstract_gui-0.0.50.9/src/abstract_gui/simple_gui/
+-rw-rw-r--   0 root         (0) root         (0)      138 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.9/src/abstract_gui/simple_gui/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1812 2023-07-30 05:32:52.000000 abstract_gui-0.0.50.9/src/abstract_gui/simple_gui/global_bridge.py
+-rw-rw-r--   0 root         (0) root         (0)     3240 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.9/src/abstract_gui/simple_gui/gui_presets.py
+-rw-rw-r--   0 root         (0) root         (0)    11778 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.9/src/abstract_gui/simple_gui/gui_template.py
+-rw-rw-r--   0 root         (0) root         (0)    13695 2023-07-30 05:25:06.000000 abstract_gui-0.0.50.9/src/abstract_gui/simple_gui/window_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 05:33:21.536389 abstract_gui-0.0.50.9/src/abstract_gui.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     3802 2023-07-30 05:33:21.000000 abstract_gui-0.0.50.9/src/abstract_gui.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      596 2023-07-30 05:33:21.000000 abstract_gui-0.0.50.9/src/abstract_gui.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-07-30 05:33:21.000000 abstract_gui-0.0.50.9/src/abstract_gui.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       31 2023-07-30 05:33:21.000000 abstract_gui-0.0.50.9/src/abstract_gui.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       13 2023-07-30 05:33:21.000000 abstract_gui-0.0.50.9/src/abstract_gui.egg-info/top_level.txt
```

### Comparing `abstract_gui-0.0.50.8/PKG-INFO` & `abstract_gui-0.0.50.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_gui
-Version: 0.0.50.8
+Version: 0.0.50.9
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_gui-0.0.50.8/README.md` & `abstract_gui-0.0.50.9/README.md`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.50.8/setup.py` & `abstract_gui-0.0.50.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_gui',
-    version='0.0.50.8',
+    version='0.0.50.9',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description='abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui',
     classifiers=[
```

### Comparing `abstract_gui-0.0.50.8/src/abstract_gui/PyQt5/PyQt5_browser_window.py` & `abstract_gui-0.0.50.9/src/abstract_gui/PyQt5/PyQt5_browser_window.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.50.8/src/abstract_gui/main.py` & `abstract_gui-0.0.50.9/src/abstract_gui/main.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.50.8/src/abstract_gui/simple_gui/global_bridge.py` & `abstract_gui-0.0.50.9/src/abstract_gui/simple_gui/global_bridge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 class WindowGlobalBridge:
         """
-    A class to manage the global variables shared between different scripts.
+        A class to manage the global variables shared between different scripts.
 
-    Attributes:
-        global_vars (dict): A dictionary to store global variables for each script.
+        Attributes:
+                global_vars (dict): A dictionary to store global variables for each script.
         
-    Methods:
-        __init__(self):
-            Initializes the WindowGlobalBridge with an empty dictionary for global_vars.
-
-        retrieve_global_variables(self, script_name, global_variables):
-            Stores the global variables of a script in the global_vars dictionary.
-
-        return_global_variables(self, script_name):
-            Returns the global variables of a script.
-    """
-    def __init__(self):
-        """
-        Initializes the WindowGlobalBridge with an empty dictionary for global_vars.
-        """
-        self.global_vars = {}
-
-    def retrieve_global_variables(self, script_name, global_variables):
-        """
-        Stores the global variables of a script in the global_vars dictionary.
-
-        Args:
-            script_name (str): The name of the script.
-            global_variables (dict): The global variables to store for the script.
-        """
-        self.global_vars[script_name] = global_variables
+        Methods:
+                __init__(self):
+                    Initializes the WindowGlobalBridge with an empty dictionary for global_vars.
+
+                retrieve_global_variables(self, script_name, global_variables):
+                    Stores the global variables of a script in the global_vars dictionary.
+
+                return_global_variables(self, script_name):
+                    Returns the global variables of a script.
+        """
+        def __init__(self):
+                """
+                Initializes the WindowGlobalBridge with an empty dictionary for global_vars.
+                """
+                self.global_vars = {}
+
+        def retrieve_global_variables(self, script_name, global_variables):
+                """
+                Stores the global variables of a script in the global_vars dictionary.
+
+                Args:
+                    script_name (str): The name of the script.
+                    global_variables (dict): The global variables to store for the script.
+                """
+                self.global_vars[script_name] = global_variables
+        
+        def return_global_variables(self, script_name):
+                """
+                Returns the global variables of a script.
+
+                Args:
+                    script_name (str): The name of the script.
+
+                Returns:
+                    dict: The global variables of the script. If no global variables are found, it returns an empty dictionary.
+                """
+                return self.global_vars.get(script_name, {})
         
-    def return_global_variables(self, script_name):
-        """
-        Returns the global variables of a script.
-
-        Args:
-            script_name (str): The name of the script.
-
-        Returns:
-            dict: The global variables of the script. If no global variables are found, it returns an empty dictionary.
-        """
-        return self.global_vars.get(script_name, {})
```

### Comparing `abstract_gui-0.0.50.8/src/abstract_gui/simple_gui/gui_presets.py` & `abstract_gui-0.0.50.9/src/abstract_gui/simple_gui/gui_presets.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.50.8/src/abstract_gui/simple_gui/gui_template.py` & `abstract_gui-0.0.50.9/src/abstract_gui/simple_gui/gui_template.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.50.8/src/abstract_gui/simple_gui/window_manager.py` & `abstract_gui-0.0.50.9/src/abstract_gui/simple_gui/window_manager.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.50.8/src/abstract_gui.egg-info/PKG-INFO` & `abstract_gui-0.0.50.9/src/abstract_gui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-gui
-Version: 0.0.50.8
+Version: 0.0.50.9
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_gui-0.0.50.8/src/abstract_gui.egg-info/SOURCES.txt` & `abstract_gui-0.0.50.9/src/abstract_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

