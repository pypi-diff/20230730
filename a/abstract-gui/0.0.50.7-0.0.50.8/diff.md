# Comparing `tmp/abstract_gui-0.0.50.7.tar.gz` & `tmp/abstract_gui-0.0.50.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_gui-0.0.50.7.tar", last modified: Sat Jul 29 04:59:38 2023, max compression
+gzip compressed data, was "abstract_gui-0.0.50.8.tar", last modified: Sun Jul 30 05:28:57 2023, max compression
```

## Comparing `abstract_gui-0.0.50.7.tar` & `abstract_gui-0.0.50.8.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 04:59:38.271931 abstract_gui-0.0.50.7/
--rw-r--r--   0 root         (0) root         (0)     3833 2023-07-29 04:59:38.271931 abstract_gui-0.0.50.7/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3086 2023-07-28 00:06:19.000000 abstract_gui-0.0.50.7/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-07-28 00:04:47.000000 abstract_gui-0.0.50.7/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)       38 2023-07-29 04:59:38.271931 abstract_gui-0.0.50.7/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1134 2023-07-29 04:59:21.000000 abstract_gui-0.0.50.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 04:59:38.271931 abstract_gui-0.0.50.7/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 04:59:38.271931 abstract_gui-0.0.50.7/src/abstract_gui/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 04:59:38.271931 abstract_gui-0.0.50.7/src/abstract_gui/PyQt5/
--rw-rw-r--   0 root         (0) root         (0)     2500 2023-07-28 00:04:47.000000 abstract_gui-0.0.50.7/src/abstract_gui/PyQt5/PyQt5_browser_window.py
--rw-rw-r--   0 root         (0) root         (0)        0 2023-07-28 00:04:47.000000 abstract_gui-0.0.50.7/src/abstract_gui/PyQt5/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2023-07-28 00:04:47.000000 abstract_gui-0.0.50.7/src/abstract_gui/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1294 2023-07-28 00:04:47.000000 abstract_gui-0.0.50.7/src/abstract_gui/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 04:59:38.271931 abstract_gui-0.0.50.7/src/abstract_gui/simple_gui/
--rw-rw-r--   0 root         (0) root         (0)      138 2023-07-28 00:04:47.000000 abstract_gui-0.0.50.7/src/abstract_gui/simple_gui/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3240 2023-07-28 00:04:47.000000 abstract_gui-0.0.50.7/src/abstract_gui/simple_gui/gui_presets.py
--rw-rw-r--   0 root         (0) root         (0)    12005 2023-07-29 04:59:16.000000 abstract_gui-0.0.50.7/src/abstract_gui/simple_gui/gui_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 04:59:38.271931 abstract_gui-0.0.50.7/src/abstract_gui.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     3833 2023-07-29 04:59:38.000000 abstract_gui-0.0.50.7/src/abstract_gui.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      505 2023-07-29 04:59:38.000000 abstract_gui-0.0.50.7/src/abstract_gui.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-07-29 04:59:38.000000 abstract_gui-0.0.50.7/src/abstract_gui.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       31 2023-07-29 04:59:38.000000 abstract_gui-0.0.50.7/src/abstract_gui.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       13 2023-07-29 04:59:38.000000 abstract_gui-0.0.50.7/src/abstract_gui.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 05:28:57.812402 abstract_gui-0.0.50.8/
+-rw-r--r--   0 root         (0) root         (0)     3802 2023-07-30 05:28:57.812402 abstract_gui-0.0.50.8/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3065 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.8/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.8/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       38 2023-07-30 05:28:57.812402 abstract_gui-0.0.50.8/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1124 2023-07-30 05:28:41.000000 abstract_gui-0.0.50.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 05:28:57.812402 abstract_gui-0.0.50.8/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 05:28:57.812402 abstract_gui-0.0.50.8/src/abstract_gui/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 05:28:57.812402 abstract_gui-0.0.50.8/src/abstract_gui/PyQt5/
+-rw-rw-r--   0 root         (0) root         (0)     2500 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.8/src/abstract_gui/PyQt5/PyQt5_browser_window.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.8/src/abstract_gui/PyQt5/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.8/src/abstract_gui/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1294 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.8/src/abstract_gui/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 05:28:57.812402 abstract_gui-0.0.50.8/src/abstract_gui/simple_gui/
+-rw-rw-r--   0 root         (0) root         (0)      138 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.8/src/abstract_gui/simple_gui/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1567 2023-07-30 05:25:06.000000 abstract_gui-0.0.50.8/src/abstract_gui/simple_gui/global_bridge.py
+-rw-rw-r--   0 root         (0) root         (0)     3240 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.8/src/abstract_gui/simple_gui/gui_presets.py
+-rw-rw-r--   0 root         (0) root         (0)    11778 2023-07-29 19:09:21.000000 abstract_gui-0.0.50.8/src/abstract_gui/simple_gui/gui_template.py
+-rw-rw-r--   0 root         (0) root         (0)    13695 2023-07-30 05:25:06.000000 abstract_gui-0.0.50.8/src/abstract_gui/simple_gui/window_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 05:28:57.812402 abstract_gui-0.0.50.8/src/abstract_gui.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     3802 2023-07-30 05:28:57.000000 abstract_gui-0.0.50.8/src/abstract_gui.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      596 2023-07-30 05:28:57.000000 abstract_gui-0.0.50.8/src/abstract_gui.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-07-30 05:28:57.000000 abstract_gui-0.0.50.8/src/abstract_gui.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       31 2023-07-30 05:28:57.000000 abstract_gui-0.0.50.8/src/abstract_gui.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       13 2023-07-30 05:28:57.000000 abstract_gui-0.0.50.8/src/abstract_gui.egg-info/top_level.txt
```

### Comparing `abstract_gui-0.0.50.7/PKG-INFO` & `abstract_gui-0.0.50.8/src/abstract_gui.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
-Name: abstract_gui
-Version: 0.0.50.7
+Name: abstract-gui
+Version: 0.0.50.8
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
-Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_gui
+Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # abstract_gui
 
 This is a Python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 
-This module can be found in the `abstract_essentials` project at `github.io/abstract_endeavors/abstract_essentials/tree/main/abstract_gui/`.
+This module can be found in the `abstract_essentials` project at `github.io/abstract_endeavors/abstract_essentials/abstract_gui/`.
 
 ## Installation
 
 You can install the `abstract_gui` module via pip:
 
 ```sh
 pip install abstract_gui
 ```
 
 You can also install it directly from the source:
 
 ```sh
-git clone https://github.com/AbstractEndeavors/abstract_essentials.git
-cd abstract_essentials/abstract_gui
+git clone https://github.io/abstract_endeavors/abstract_essentials/abstract_gui/
+cd abstract_gui
 python setup.py install
 ```
 
 ## Usage
 
 Here's an example of how to use the `abstract_gui` module:
 
@@ -112,8 +112,8 @@
 
 This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
 
 ## Authors
 
 * putkoff - main developer
 
-This README file was last updated on july 29, 2023.
+This README file was last updated on May 29, 2023.
```

### Comparing `abstract_gui-0.0.50.7/README.md` & `abstract_gui-0.0.50.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # abstract_gui
 
 This is a Python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 
-This module can be found in the `abstract_essentials` project at `github.io/abstract_endeavors/abstract_essentials/tree/main/abstract_gui/`.
+This module can be found in the `abstract_essentials` project at `github.io/abstract_endeavors/abstract_essentials/abstract_gui/`.
 
 ## Installation
 
 You can install the `abstract_gui` module via pip:
 
 ```sh
 pip install abstract_gui
 ```
 
 You can also install it directly from the source:
 
 ```sh
-git clone https://github.com/AbstractEndeavors/abstract_essentials.git
-cd abstract_essentials/abstract_gui
+git clone https://github.io/abstract_endeavors/abstract_essentials/abstract_gui/
+cd abstract_gui
 python setup.py install
 ```
 
 ## Usage
 
 Here's an example of how to use the `abstract_gui` module:
 
@@ -97,8 +97,8 @@
 
 This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
 
 ## Authors
 
 * putkoff - main developer
 
-This README file was last updated on july 29, 2023.
+This README file was last updated on May 29, 2023.
```

### Comparing `abstract_gui-0.0.50.7/setup.py` & `abstract_gui-0.0.50.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_gui',
-    version='0.0.50.7',
+    version='0.0.50.8',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description='abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url='https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_gui',
+    url='https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.11',
     ],
```

### Comparing `abstract_gui-0.0.50.7/src/abstract_gui/PyQt5/PyQt5_browser_window.py` & `abstract_gui-0.0.50.8/src/abstract_gui/PyQt5/PyQt5_browser_window.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.50.7/src/abstract_gui/main.py` & `abstract_gui-0.0.50.8/src/abstract_gui/main.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.50.7/src/abstract_gui/simple_gui/gui_presets.py` & `abstract_gui-0.0.50.8/src/abstract_gui/simple_gui/gui_presets.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.50.7/src/abstract_gui/simple_gui/gui_template.py` & `abstract_gui-0.0.50.8/src/abstract_gui/simple_gui/gui_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,29 +18,26 @@
         return glob[obj]
 def update_window_to_registry(win,win_name:str ='default_window'):
     windows =get_all_windows()
     if win_name in windows:
         win_name = create_win_name(win_name=win_name)
     windows[win_name]={'name': win_name, 'values': {}, 'event': ''}
     update_registry(var='all_windows',val=windows,name=registry_name)
-    update_registry(var=win_name, val=win,name=registry_name)
 def get_window(title: str = 'basic window', layout: list = [[]]):
     """
     Returns a callable object for creating a PySimpleGUI window with the specified title and layout.
 
     Args:
         title (str): The title of the window.
         layout (list): The layout of the window.
 
     Returns:
         callable: A callable object that creates the PySimpleGUI window when called.
     """
-    win = get_gui_fun(name='Window', args={"title": title, "layout": layout})
-    update_window_to_registry(win,win_name=title)
-    return win
+    return get_gui_fun(name='Window', args={"title": title, "layout": layout})
 
 def verify_window(win: any = None) -> bool:
     """
     Verifies if the given object is a valid PySimpleGUI window.
 
     Args:
         win (any): The object to verify.
@@ -194,15 +191,15 @@
 
     Returns:
         any: The retrieved value or None if the key doesn't exist.
     """
     if st in js:
         return js[st]
 
-def while_basic_events(event_win: type(get_window()) = get_window(), win_name: str = create_win_name(), events: dict = {},global_values:dict=globals()):
+def while_basic_events(event_win: type(get_window()) = get_window(), win_name: str = create_win_name(), events: dict = {}):
     """
     Executes a while loop for handling basic events in a PySimpleGUI window.
 
     Args:
         event_win (type(get_window())): The window to handle events for.
         win_name (str): The name of the window.
         events (dict): The dictionary of events and their corresponding function specifications.
@@ -212,31 +209,29 @@
         if win_closed(get_event(event_win)):
             break
         keys = get_keys(events)
         for k in range(0, len(keys)):
             key = keys[k]
             if T_or_F_obj_eq(event=get_event(curr_win=win_name), obj=key):
                 func_specs = events[key]
-                if func_specs:
+                if fun_specs:
                     args = process_args(func_specs['args'])
-                call_functions(args=args, instance=get_js_st(func_specs, 'instance'), function_name=get_js_st(func_specs, 'name'), glob=global_values)
+                call_functions(args=args, instance=get_js_st(func_specs, 'instance'), function_name=get_js_st(func_specs, 'name'), glob=globals())
     close_window(event_win)
 
 def while_basic(win=None):
     """
     Executes a while loop for handling basic events in a PySimpleGUI window.
 
     Args:
         win: The window to handle events for. If not provided, it uses the 'window' global object.
     """
     values_all=[]
     if win is None:
         win = get_globes(string='window')
-    if type(win) is str:
-        win = get_window_from_global(win)
     while verify_window(win):
         event, values = win.read()
         if values != None:
             values_all = values
         if win_closed(event):
             return values_all
             break
```

### Comparing `abstract_gui-0.0.50.7/src/abstract_gui.egg-info/PKG-INFO` & `abstract_gui-0.0.50.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
-Name: abstract-gui
-Version: 0.0.50.7
+Name: abstract_gui
+Version: 0.0.50.8
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
-Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_gui
+Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # abstract_gui
 
 This is a Python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 
-This module can be found in the `abstract_essentials` project at `github.io/abstract_endeavors/abstract_essentials/tree/main/abstract_gui/`.
+This module can be found in the `abstract_essentials` project at `github.io/abstract_endeavors/abstract_essentials/abstract_gui/`.
 
 ## Installation
 
 You can install the `abstract_gui` module via pip:
 
 ```sh
 pip install abstract_gui
 ```
 
 You can also install it directly from the source:
 
 ```sh
-git clone https://github.com/AbstractEndeavors/abstract_essentials.git
-cd abstract_essentials/abstract_gui
+git clone https://github.io/abstract_endeavors/abstract_essentials/abstract_gui/
+cd abstract_gui
 python setup.py install
 ```
 
 ## Usage
 
 Here's an example of how to use the `abstract_gui` module:
 
@@ -112,8 +112,8 @@
 
 This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
 
 ## Authors
 
 * putkoff - main developer
 
-This README file was last updated on july 29, 2023.
+This README file was last updated on May 29, 2023.
```

