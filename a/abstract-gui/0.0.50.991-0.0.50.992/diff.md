# Comparing `tmp/abstract_gui-0.0.50.991.tar.gz` & `tmp/abstract_gui-0.0.50.992.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_gui-0.0.50.991.tar", last modified: Sun Jul 30 06:19:01 2023, max compression
+gzip compressed data, was "abstract_gui-0.0.50.992.tar", last modified: Sun Jul 30 06:20:17 2023, max compression
```

## Comparing `abstract_gui-0.0.50.991.tar` & `abstract_gui-0.0.50.992.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 06:19:01.151711 abstract_gui-0.0.50.991/
--rw-r--r--   0 root         (0) root         (0)     3804 2023-07-30 06:19:01.151711 abstract_gui-0.0.50.991/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3065 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.991/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.991/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)       38 2023-07-30 06:19:01.151711 abstract_gui-0.0.50.991/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1126 2023-07-30 06:18:46.000000 abstract_gui-0.0.50.991/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 06:19:01.147711 abstract_gui-0.0.50.991/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 06:19:01.151711 abstract_gui-0.0.50.991/src/abstract_gui/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 06:19:01.151711 abstract_gui-0.0.50.991/src/abstract_gui/PyQt5/
--rw-rw-r--   0 root         (0) root         (0)     2500 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.991/src/abstract_gui/PyQt5/PyQt5_browser_window.py
--rw-rw-r--   0 root         (0) root         (0)        0 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.991/src/abstract_gui/PyQt5/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.991/src/abstract_gui/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1294 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.991/src/abstract_gui/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 06:19:01.151711 abstract_gui-0.0.50.991/src/abstract_gui/simple_gui/
--rw-rw-r--   0 root         (0) root         (0)      303 2023-07-30 05:44:36.000000 abstract_gui-0.0.50.991/src/abstract_gui/simple_gui/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1812 2023-07-30 05:32:52.000000 abstract_gui-0.0.50.991/src/abstract_gui/simple_gui/global_bridge.py
--rw-rw-r--   0 root         (0) root         (0)     3240 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.991/src/abstract_gui/simple_gui/gui_presets.py
--rw-rw-r--   0 root         (0) root         (0)    11778 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.991/src/abstract_gui/simple_gui/gui_template.py
--rw-rw-r--   0 root         (0) root         (0)    13813 2023-07-30 06:18:30.000000 abstract_gui-0.0.50.991/src/abstract_gui/simple_gui/window_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 06:19:01.151711 abstract_gui-0.0.50.991/src/abstract_gui.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     3804 2023-07-30 06:19:01.000000 abstract_gui-0.0.50.991/src/abstract_gui.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      596 2023-07-30 06:19:01.000000 abstract_gui-0.0.50.991/src/abstract_gui.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-07-30 06:19:01.000000 abstract_gui-0.0.50.991/src/abstract_gui.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       31 2023-07-30 06:19:01.000000 abstract_gui-0.0.50.991/src/abstract_gui.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       13 2023-07-30 06:19:01.000000 abstract_gui-0.0.50.991/src/abstract_gui.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 06:20:17.835744 abstract_gui-0.0.50.992/
+-rw-r--r--   0 root         (0) root         (0)     3804 2023-07-30 06:20:17.835744 abstract_gui-0.0.50.992/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3065 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.992/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.992/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       38 2023-07-30 06:20:17.835744 abstract_gui-0.0.50.992/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1126 2023-07-30 06:20:02.000000 abstract_gui-0.0.50.992/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 06:20:17.831744 abstract_gui-0.0.50.992/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 06:20:17.831744 abstract_gui-0.0.50.992/src/abstract_gui/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 06:20:17.835744 abstract_gui-0.0.50.992/src/abstract_gui/PyQt5/
+-rw-rw-r--   0 root         (0) root         (0)     2500 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.992/src/abstract_gui/PyQt5/PyQt5_browser_window.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.992/src/abstract_gui/PyQt5/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.992/src/abstract_gui/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1294 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.992/src/abstract_gui/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 06:20:17.835744 abstract_gui-0.0.50.992/src/abstract_gui/simple_gui/
+-rw-rw-r--   0 root         (0) root         (0)      303 2023-07-30 05:44:36.000000 abstract_gui-0.0.50.992/src/abstract_gui/simple_gui/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1812 2023-07-30 05:32:52.000000 abstract_gui-0.0.50.992/src/abstract_gui/simple_gui/global_bridge.py
+-rw-rw-r--   0 root         (0) root         (0)     3240 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.992/src/abstract_gui/simple_gui/gui_presets.py
+-rw-rw-r--   0 root         (0) root         (0)    11778 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.992/src/abstract_gui/simple_gui/gui_template.py
+-rw-rw-r--   0 root         (0) root         (0)    13816 2023-07-30 06:19:51.000000 abstract_gui-0.0.50.992/src/abstract_gui/simple_gui/window_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 06:20:17.835744 abstract_gui-0.0.50.992/src/abstract_gui.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     3804 2023-07-30 06:20:17.000000 abstract_gui-0.0.50.992/src/abstract_gui.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      596 2023-07-30 06:20:17.000000 abstract_gui-0.0.50.992/src/abstract_gui.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-07-30 06:20:17.000000 abstract_gui-0.0.50.992/src/abstract_gui.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       31 2023-07-30 06:20:17.000000 abstract_gui-0.0.50.992/src/abstract_gui.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       13 2023-07-30 06:20:17.000000 abstract_gui-0.0.50.992/src/abstract_gui.egg-info/top_level.txt
```

### Comparing `abstract_gui-0.0.50.991/PKG-INFO` & `abstract_gui-0.0.50.992/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_gui
-Version: 0.0.50.991
+Version: 0.0.50.992
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_gui-0.0.50.991/README.md` & `abstract_gui-0.0.50.992/README.md`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.50.991/setup.py` & `abstract_gui-0.0.50.992/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_gui',
-    version='0.0.50.991',
+    version='0.0.50.992',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description='abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui',
     classifiers=[
```

### Comparing `abstract_gui-0.0.50.991/src/abstract_gui/PyQt5/PyQt5_browser_window.py` & `abstract_gui-0.0.50.992/src/abstract_gui/PyQt5/PyQt5_browser_window.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.50.991/src/abstract_gui/main.py` & `abstract_gui-0.0.50.992/src/abstract_gui/main.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.50.991/src/abstract_gui/simple_gui/global_bridge.py` & `abstract_gui-0.0.50.992/src/abstract_gui/simple_gui/global_bridge.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.50.991/src/abstract_gui/simple_gui/gui_presets.py` & `abstract_gui-0.0.50.992/src/abstract_gui/simple_gui/gui_presets.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.50.991/src/abstract_gui/simple_gui/gui_template.py` & `abstract_gui-0.0.50.992/src/abstract_gui/simple_gui/gui_template.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.50.991/src/abstract_gui/simple_gui/window_manager.py` & `abstract_gui-0.0.50.992/src/abstract_gui/simple_gui/window_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
 
         Args:
             win (any, optional): The window to get the values from. If not provided, the last accessed window is used.
 
         Returns:
             dict: The values from the window.
         """
-        if win is None:
+        if window is None:
             return self.all_windows[self.all_windows['last_window']]['values']
         name = self.search_global_windows(window)
         if name is not False:
             return self.all_windows[name]['values']
 
     def while_basic(self, window=None):
         """
```

### Comparing `abstract_gui-0.0.50.991/src/abstract_gui.egg-info/PKG-INFO` & `abstract_gui-0.0.50.992/src/abstract_gui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-gui
-Version: 0.0.50.991
+Version: 0.0.50.992
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_gui-0.0.50.991/src/abstract_gui.egg-info/SOURCES.txt` & `abstract_gui-0.0.50.992/src/abstract_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

