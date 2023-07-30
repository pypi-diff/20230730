# Comparing `tmp/abstract_gui-0.0.50.94.tar.gz` & `tmp/abstract_gui-0.0.50.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_gui-0.0.50.94.tar", last modified: Sun Jul 30 05:54:22 2023, max compression
+gzip compressed data, was "abstract_gui-0.0.50.95.tar", last modified: Sun Jul 30 05:55:47 2023, max compression
```

## Comparing `abstract_gui-0.0.50.94.tar` & `abstract_gui-0.0.50.95.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 05:54:22.278049 abstract_gui-0.0.50.94/
--rw-r--r--   0 root         (0) root         (0)     3803 2023-07-30 05:54:22.278049 abstract_gui-0.0.50.94/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3065 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.94/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.94/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)       38 2023-07-30 05:54:22.278049 abstract_gui-0.0.50.94/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1125 2023-07-30 05:53:49.000000 abstract_gui-0.0.50.94/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 05:54:22.278049 abstract_gui-0.0.50.94/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 05:54:22.278049 abstract_gui-0.0.50.94/src/abstract_gui/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 05:54:22.278049 abstract_gui-0.0.50.94/src/abstract_gui/PyQt5/
--rw-rw-r--   0 root         (0) root         (0)     2500 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.94/src/abstract_gui/PyQt5/PyQt5_browser_window.py
--rw-rw-r--   0 root         (0) root         (0)        0 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.94/src/abstract_gui/PyQt5/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.94/src/abstract_gui/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1294 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.94/src/abstract_gui/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 05:54:22.278049 abstract_gui-0.0.50.94/src/abstract_gui/simple_gui/
--rw-rw-r--   0 root         (0) root         (0)      303 2023-07-30 05:44:36.000000 abstract_gui-0.0.50.94/src/abstract_gui/simple_gui/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1812 2023-07-30 05:32:52.000000 abstract_gui-0.0.50.94/src/abstract_gui/simple_gui/global_bridge.py
--rw-rw-r--   0 root         (0) root         (0)     3240 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.94/src/abstract_gui/simple_gui/gui_presets.py
--rw-rw-r--   0 root         (0) root         (0)    11778 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.94/src/abstract_gui/simple_gui/gui_template.py
--rw-rw-r--   0 root         (0) root         (0)    13725 2023-07-30 05:53:35.000000 abstract_gui-0.0.50.94/src/abstract_gui/simple_gui/window_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 05:54:22.278049 abstract_gui-0.0.50.94/src/abstract_gui.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     3803 2023-07-30 05:54:22.000000 abstract_gui-0.0.50.94/src/abstract_gui.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      596 2023-07-30 05:54:22.000000 abstract_gui-0.0.50.94/src/abstract_gui.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-07-30 05:54:22.000000 abstract_gui-0.0.50.94/src/abstract_gui.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       31 2023-07-30 05:54:22.000000 abstract_gui-0.0.50.94/src/abstract_gui.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       13 2023-07-30 05:54:22.000000 abstract_gui-0.0.50.94/src/abstract_gui.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 05:55:47.602211 abstract_gui-0.0.50.95/
+-rw-r--r--   0 root         (0) root         (0)     3803 2023-07-30 05:55:47.602211 abstract_gui-0.0.50.95/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3065 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.95/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.95/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       38 2023-07-30 05:55:47.602211 abstract_gui-0.0.50.95/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1125 2023-07-30 05:55:33.000000 abstract_gui-0.0.50.95/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 05:55:47.602211 abstract_gui-0.0.50.95/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 05:55:47.602211 abstract_gui-0.0.50.95/src/abstract_gui/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 05:55:47.602211 abstract_gui-0.0.50.95/src/abstract_gui/PyQt5/
+-rw-rw-r--   0 root         (0) root         (0)     2500 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.95/src/abstract_gui/PyQt5/PyQt5_browser_window.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.95/src/abstract_gui/PyQt5/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.95/src/abstract_gui/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1294 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.95/src/abstract_gui/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 05:55:47.602211 abstract_gui-0.0.50.95/src/abstract_gui/simple_gui/
+-rw-rw-r--   0 root         (0) root         (0)      303 2023-07-30 05:44:36.000000 abstract_gui-0.0.50.95/src/abstract_gui/simple_gui/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1812 2023-07-30 05:32:52.000000 abstract_gui-0.0.50.95/src/abstract_gui/simple_gui/global_bridge.py
+-rw-rw-r--   0 root         (0) root         (0)     3240 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.95/src/abstract_gui/simple_gui/gui_presets.py
+-rw-rw-r--   0 root         (0) root         (0)    11778 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.95/src/abstract_gui/simple_gui/gui_template.py
+-rw-rw-r--   0 root         (0) root         (0)    13730 2023-07-30 05:55:19.000000 abstract_gui-0.0.50.95/src/abstract_gui/simple_gui/window_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 05:55:47.602211 abstract_gui-0.0.50.95/src/abstract_gui.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     3803 2023-07-30 05:55:47.000000 abstract_gui-0.0.50.95/src/abstract_gui.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      596 2023-07-30 05:55:47.000000 abstract_gui-0.0.50.95/src/abstract_gui.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-07-30 05:55:47.000000 abstract_gui-0.0.50.95/src/abstract_gui.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       31 2023-07-30 05:55:47.000000 abstract_gui-0.0.50.95/src/abstract_gui.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       13 2023-07-30 05:55:47.000000 abstract_gui-0.0.50.95/src/abstract_gui.egg-info/top_level.txt
```

### Comparing `abstract_gui-0.0.50.94/PKG-INFO` & `abstract_gui-0.0.50.95/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_gui
-Version: 0.0.50.94
+Version: 0.0.50.95
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_gui-0.0.50.94/README.md` & `abstract_gui-0.0.50.95/README.md`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.50.94/setup.py` & `abstract_gui-0.0.50.95/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_gui',
-    version='0.0.50.94',
+    version='0.0.50.95',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description='abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui',
     classifiers=[
```

### Comparing `abstract_gui-0.0.50.94/src/abstract_gui/PyQt5/PyQt5_browser_window.py` & `abstract_gui-0.0.50.95/src/abstract_gui/PyQt5/PyQt5_browser_window.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.50.94/src/abstract_gui/main.py` & `abstract_gui-0.0.50.95/src/abstract_gui/main.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.50.94/src/abstract_gui/simple_gui/global_bridge.py` & `abstract_gui-0.0.50.95/src/abstract_gui/simple_gui/global_bridge.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.50.94/src/abstract_gui/simple_gui/gui_presets.py` & `abstract_gui-0.0.50.95/src/abstract_gui/simple_gui/gui_presets.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.50.94/src/abstract_gui/simple_gui/gui_template.py` & `abstract_gui-0.0.50.95/src/abstract_gui/simple_gui/gui_template.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.50.94/src/abstract_gui/simple_gui/window_manager.py` & `abstract_gui-0.0.50.95/src/abstract_gui/simple_gui/window_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
                 break
             event_function = self.all_windows[self.search_global_windows(window)]["event_function"]
             if event_function is not None:
                 self.global_vars[event_function](self.get_event(window))
 
         self.close_window(window)
         # Update the global variables in the global bridge
-        self.global_vars["all_windows"]=all_windows
+        self.global_vars["all_windows"]=self.all_windows
         self.global_bridge.retrieve_global_variables(self.script_name,self.global_vars)
 
     def delete_from_list(self, _list, var):
         """
         Remove a variable from a list.
 
         Args:
```

### Comparing `abstract_gui-0.0.50.94/src/abstract_gui.egg-info/PKG-INFO` & `abstract_gui-0.0.50.95/src/abstract_gui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-gui
-Version: 0.0.50.94
+Version: 0.0.50.95
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_gui-0.0.50.94/src/abstract_gui.egg-info/SOURCES.txt` & `abstract_gui-0.0.50.95/src/abstract_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

