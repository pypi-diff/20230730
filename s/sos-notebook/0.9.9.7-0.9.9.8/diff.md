# Comparing `tmp/sos-notebook-0.9.9.7.tar.gz` & `tmp/sos-notebook-0.9.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sos-notebook-0.9.9.7.tar", last modified: Wed Oct 18 14:12:43 2017, max compression
+gzip compressed data, was "dist/sos-notebook-0.9.9.8.tar", last modified: Wed Nov  1 21:22:56 2017, max compression
```

## Comparing `sos-notebook-0.9.9.7.tar` & `sos-notebook-0.9.9.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-18 14:12:43.000000 sos-notebook-0.9.9.7/
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      241 2017-10-06 02:50:36.000000 sos-notebook-0.9.9.7/MANIFEST.in
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     2170 2017-10-18 14:12:43.000000 sos-notebook-0.9.9.7/PKG-INFO
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      885 2017-10-06 04:13:04.000000 sos-notebook-0.9.9.7/README.md
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)       38 2017-10-18 14:12:43.000000 sos-notebook-0.9.9.7/setup.cfg
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     7228 2017-10-18 14:12:05.000000 sos-notebook-0.9.9.7/setup.py
-drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-18 14:12:43.000000 sos-notebook-0.9.9.7/src/
-drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-18 14:12:43.000000 sos-notebook-0.9.9.7/src/sos_notebook/
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-05 04:50:34.000000 sos-notebook-0.9.9.7/src/sos_notebook/__init__.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     1715 2017-10-18 14:12:40.000000 sos-notebook-0.9.9.7/src/sos_notebook/_version.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     4181 2017-10-05 04:50:34.000000 sos-notebook-0.9.9.7/src/sos_notebook/completer.py
--rwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    24022 2017-10-05 04:54:42.000000 sos-notebook-0.9.9.7/src/sos_notebook/converter.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     3259 2017-10-05 04:50:34.000000 sos-notebook-0.9.9.7/src/sos_notebook/inspector.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    90497 2017-10-18 12:32:53.000000 sos-notebook-0.9.9.7/src/sos_notebook/kernel.js
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)   130826 2017-10-16 22:21:20.000000 sos-notebook-0.9.9.7/src/sos_notebook/kernel.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     1932 2017-10-05 01:37:50.000000 sos-notebook-0.9.9.7/src/sos_notebook/logo-64x64.png
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     9352 2017-10-05 04:50:34.000000 sos-notebook-0.9.9.7/src/sos_notebook/preview.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     5137 2017-10-12 14:27:31.000000 sos-notebook-0.9.9.7/src/sos_notebook/sos-full.tpl
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     7781 2017-10-05 01:31:02.000000 sos-notebook-0.9.9.7/src/sos_notebook/sos-report.tpl
--rwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    18186 2017-10-05 04:50:34.000000 sos-notebook-0.9.9.7/src/sos_notebook/sos_executor.py
--rwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     4312 2017-10-18 12:32:36.000000 sos-notebook-0.9.9.7/src/sos_notebook/sos_step.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     5088 2017-10-12 18:42:05.000000 sos-notebook-0.9.9.7/src/sos_notebook/test_utils.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    16015 2017-10-05 04:50:34.000000 sos-notebook-0.9.9.7/src/sos_notebook/visualize.py
-drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-18 14:12:43.000000 sos-notebook-0.9.9.7/src/sos_notebook.egg-info/
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        1 2017-10-18 14:12:43.000000 sos-notebook-0.9.9.7/src/sos_notebook.egg-info/dependency_links.txt
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     1608 2017-10-18 14:12:43.000000 sos-notebook-0.9.9.7/src/sos_notebook.egg-info/entry_points.txt
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     2170 2017-10-18 14:12:43.000000 sos-notebook-0.9.9.7/src/sos_notebook.egg-info/PKG-INFO
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      112 2017-10-18 14:12:43.000000 sos-notebook-0.9.9.7/src/sos_notebook.egg-info/requires.txt
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      902 2017-10-18 14:12:43.000000 sos-notebook-0.9.9.7/src/sos_notebook.egg-info/SOURCES.txt
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)       13 2017-10-18 14:12:43.000000 sos-notebook-0.9.9.7/src/sos_notebook.egg-info/top_level.txt
-drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-18 14:12:43.000000 sos-notebook-0.9.9.7/test/
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     3907 2017-10-05 04:48:58.000000 sos-notebook-0.9.9.7/test/test_jupyter_convert.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     5265 2017-10-06 02:50:36.000000 sos-notebook-0.9.9.7/test/test_jupyter_sos.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     4442 2017-10-18 12:42:33.000000 sos-notebook-0.9.9.7/test/test_jupyter_tasks.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     3191 2017-10-05 04:48:37.000000 sos-notebook-0.9.9.7/test/test_sos_completer.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     3626 2017-10-12 13:48:46.000000 sos-notebook-0.9.9.7/test/test_sos_inspector.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     4933 2017-10-12 18:01:22.000000 sos-notebook-0.9.9.7/test/test_sos_kernel.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     8460 2017-10-12 18:54:20.000000 sos-notebook-0.9.9.7/test/test_sos_magics.py
+drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-11-01 21:22:56.000000 sos-notebook-0.9.9.8/
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      241 2017-10-06 20:04:07.000000 sos-notebook-0.9.9.8/MANIFEST.in
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     2170 2017-11-01 21:22:56.000000 sos-notebook-0.9.9.8/PKG-INFO
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      885 2017-10-06 20:04:07.000000 sos-notebook-0.9.9.8/README.md
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)       38 2017-11-01 21:22:56.000000 sos-notebook-0.9.9.8/setup.cfg
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     7228 2017-10-18 20:38:49.000000 sos-notebook-0.9.9.8/setup.py
+drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-11-01 21:22:56.000000 sos-notebook-0.9.9.8/src/
+drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-11-01 21:22:56.000000 sos-notebook-0.9.9.8/src/sos_notebook/
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-06 20:04:07.000000 sos-notebook-0.9.9.8/src/sos_notebook/__init__.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     1715 2017-11-01 21:22:48.000000 sos-notebook-0.9.9.8/src/sos_notebook/_version.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     4181 2017-10-06 20:04:07.000000 sos-notebook-0.9.9.8/src/sos_notebook/completer.py
+-rwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    24022 2017-10-06 20:04:07.000000 sos-notebook-0.9.9.8/src/sos_notebook/converter.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     3259 2017-10-06 20:04:07.000000 sos-notebook-0.9.9.8/src/sos_notebook/inspector.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    92488 2017-11-01 19:17:03.000000 sos-notebook-0.9.9.8/src/sos_notebook/kernel.js
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)   133014 2017-10-30 20:09:28.000000 sos-notebook-0.9.9.8/src/sos_notebook/kernel.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     1932 2017-10-06 20:04:07.000000 sos-notebook-0.9.9.8/src/sos_notebook/logo-64x64.png
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     9352 2017-10-06 20:04:07.000000 sos-notebook-0.9.9.8/src/sos_notebook/preview.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     5137 2017-10-10 19:15:04.000000 sos-notebook-0.9.9.8/src/sos_notebook/sos-full.tpl
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     7781 2017-10-06 20:04:07.000000 sos-notebook-0.9.9.8/src/sos_notebook/sos-report.tpl
+-rwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    18186 2017-10-06 20:04:07.000000 sos-notebook-0.9.9.8/src/sos_notebook/sos_executor.py
+-rwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     4312 2017-10-18 20:38:49.000000 sos-notebook-0.9.9.8/src/sos_notebook/sos_step.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     5088 2017-10-17 00:32:31.000000 sos-notebook-0.9.9.8/src/sos_notebook/test_utils.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)    16015 2017-10-06 20:04:07.000000 sos-notebook-0.9.9.8/src/sos_notebook/visualize.py
+drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-11-01 21:22:56.000000 sos-notebook-0.9.9.8/src/sos_notebook.egg-info/
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        1 2017-11-01 21:22:56.000000 sos-notebook-0.9.9.8/src/sos_notebook.egg-info/dependency_links.txt
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     1608 2017-11-01 21:22:56.000000 sos-notebook-0.9.9.8/src/sos_notebook.egg-info/entry_points.txt
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     2170 2017-11-01 21:22:56.000000 sos-notebook-0.9.9.8/src/sos_notebook.egg-info/PKG-INFO
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      112 2017-11-01 21:22:56.000000 sos-notebook-0.9.9.8/src/sos_notebook.egg-info/requires.txt
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      902 2017-11-01 21:22:56.000000 sos-notebook-0.9.9.8/src/sos_notebook.egg-info/SOURCES.txt
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)       13 2017-11-01 21:22:56.000000 sos-notebook-0.9.9.8/src/sos_notebook.egg-info/top_level.txt
+drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-11-01 21:22:56.000000 sos-notebook-0.9.9.8/test/
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     3907 2017-10-06 20:04:07.000000 sos-notebook-0.9.9.8/test/test_jupyter_convert.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     5265 2017-10-06 20:04:07.000000 sos-notebook-0.9.9.8/test/test_jupyter_sos.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     4442 2017-10-18 20:38:49.000000 sos-notebook-0.9.9.8/test/test_jupyter_tasks.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     3191 2017-10-06 20:04:07.000000 sos-notebook-0.9.9.8/test/test_sos_completer.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     3626 2017-10-17 00:32:31.000000 sos-notebook-0.9.9.8/test/test_sos_inspector.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     4915 2017-10-24 15:06:49.000000 sos-notebook-0.9.9.8/test/test_sos_kernel.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     8460 2017-10-17 00:32:31.000000 sos-notebook-0.9.9.8/test/test_sos_magics.py
```

### Comparing `sos-notebook-0.9.9.7/PKG-INFO` & `sos-notebook-0.9.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sos-notebook
-Version: 0.9.9.7
+Version: 0.9.9.8
 Summary: Script of Scripts (SoS): an interactive, cross-platform, and cross-language workflow system for reproducible data analysis
 Home-page: https://github.com/vatlab/SOS
 Author: Bo Peng
 Author-email: bpeng@mdanderson.org
 License: GPL3
 Description-Content-Type: UNKNOWN
 Description: Complex bioinformatic data analysis workflows involving multiple scripts
```

### Comparing `sos-notebook-0.9.9.7/README.md` & `sos-notebook-0.9.9.8/README.md`

 * *Files identical despite different names*

### Comparing `sos-notebook-0.9.9.7/setup.py` & `sos-notebook-0.9.9.8/setup.py`

 * *Files identical despite different names*

### Comparing `sos-notebook-0.9.9.7/src/sos_notebook/_version.py` & `sos-notebook-0.9.9.8/src/sos_notebook/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     raise SystemError('SOS requires Python 3.4 or higher. Please upgrade your Python {}.{}.{}.'
         .format(_py_ver.major, _py_ver.minor, _py_ver.micro))
 
 
 # version of the SoS language
 __sos_version__ = '1.0'
 # version of the sos command
-__version__ = '0.9.9.7'
+__version__ = '0.9.9.8'
 __py_version__ = '{}.{}.{}'.format(_py_ver.major, _py_ver.minor, _py_ver.micro)
 
 #
 SOS_FULL_VERSION='{} for Python {}.{}.{}'.format(__version__, _py_ver.major, _py_ver.minor, _py_ver.micro)
 SOS_COPYRIGHT = '''SoS {} : Copyright (c) 2016 Bo Peng'''.format(__version__)
 SOS_CONTACT = '''Please visit http://github.com/vatlab/SOS for more information.'''
```

### Comparing `sos-notebook-0.9.9.7/src/sos_notebook/completer.py` & `sos-notebook-0.9.9.8/src/sos_notebook/completer.py`

 * *Files identical despite different names*

### Comparing `sos-notebook-0.9.9.7/src/sos_notebook/converter.py` & `sos-notebook-0.9.9.8/src/sos_notebook/converter.py`

 * *Files identical despite different names*

### Comparing `sos-notebook-0.9.9.7/src/sos_notebook/inspector.py` & `sos-notebook-0.9.9.8/src/sos_notebook/inspector.py`

 * *Files identical despite different names*

### Comparing `sos-notebook-0.9.9.7/src/sos_notebook/kernel.js` & `sos-notebook-0.9.9.8/src/sos_notebook/kernel.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -603,30 +603,42 @@
                 if (item) {
                     item.parentNode.removeChild(item);
                 }
             } else if (msg_type === "update-duration") {
                 if (!window._duration_updater) {
                     window._duration_updater = window.setInterval(function() {
                         $("[id^=duration_]").text(function() {
+                            if ($(this).attr("class") != "running")
+                                return $(this).text();
                             return window.durationFormatter($(this).attr("datetime"));
                         });
                     }, 5000);
                 }
             } else if (msg_type === "task-status") {
                 // console.log(data);
                 var item = document.getElementById("status_" + data[0] + "_" + data[1]);
                 if (!item) {
                     return;
                 } else {
                     // id, status, status_class, action_class, action_func
                     item.className = "fa fa-fw fa-2x " + data[3];
-                    item.setAttribute("onmouseover", "$('#status_" + data[0] + "_" + data[1] + "').addClass('" + data[4] + "').removeClass('" + data[3] + "')");
-                    item.setAttribute("onmouseleave", "$('#status_" + data[0] + "_" + data[1] + "').addClass('" + data[3] + "').removeClass('" + data[4] + "')");
+                    item.setAttribute("onmouseover", "$('#status_" + data[0] + "_" + data[1] + "').addClass('" + data[4] + " task_hover').removeClass('" + data[3] + "')");
+                    item.setAttribute("onmouseleave", "$('#status_" + data[0] + "_" + data[1] + "').addClass('" + data[3] + "').removeClass('" + data[4] + " task_hover')");
                     item.setAttribute("onClick", data[5] + "('" + data[1] + "', '" + data[0] + "')");
                 }
+                var item = document.getElementById("duration_" + data[0] + "_" + data[1]);
+                if (item) {
+                    item.className = data[2];
+                    // stop update and reset time ...
+                    if (data[2] != "running") {
+                        var curTime = new Date();
+                        item.innerText = window.durationFormatter(item.getAttribute("datetime"));
+                        item.setAttribute('datetime', curTime.getTime());
+                    }
+                }
                 if (data[2] === "completed") {
                     /* if successful, let us re-run the cell to submt another task
                        or get the result */
                     for (cell in window.pending_cells) {
                         /* remove task from pending_cells */
                         for (var idx = 0; idx < window.pending_cells[cell].length; ++idx) {
                             if (window.pending_cells[cell][idx][0] !== data[0] ||
@@ -657,14 +669,36 @@
             } else if (msg_type === "show_toc") {
                 show_toc();
             } else if (msg_type === "paste-table") {
                 var cm = nb.get_selected_cell().code_mirror;
                 cm.replaceRange(data, cm.getCursor());
             } else if (msg_type === 'alert') {
                 alert(data);
+            } else if (msg_type === 'clear-output') {
+                // if remove output of all cells
+                var active = nb.get_selected_cells_indices();
+                if (data[1]) {
+                    var cells = nb.get_cells();
+                    var i;
+                    for (i = 0; i < cells.length; ++i) {
+                        cells[i].clear_output();
+                    }
+                } else if (data[0] === -1) {
+                    // clear output of selected cells
+                    var i;
+                    for (i = 0; i < active.length; ++i) {
+                        nb.get_cell(active[i]).clear_output();
+                    }
+                } else {
+                    // clear current cell
+                    nb.get_cell(data[0]).clear_output();
+                }
+                if (active.length > 0) {
+                    nb.select(active[0]);
+                }
             } else {
                 // this is preview output
                 cell = window.my_panel.cell;
                 data.output_type = msg_type;
                 cell.output_area.append_output(data);
             }
             adjustPanel();
@@ -958,14 +992,21 @@
             if (nb.metadata["sos"]["panel"].style === "side") {
                 var headerVisibleHeight = $("#header").is(":visible") ? $("#header").height() : 0;
                 $("#panel-wrapper").css("top", headerVisibleHeight);
                 $("#panel-wrapper").css("height", $("#site").height());
             }
         });
 
+        $(".output_scroll").on("resizeOutput", function() {
+            var output = $(this);
+            setTimeout(function() {
+                output.scrollTop(output.prop("scrollHeight"));
+            }, 0);
+        });
+
         // enable dragging and save position on stop moving
         $("#panel-wrapper").draggable({
 
             drag: function(event, ui) {
 
                 // If dragging to the left side, then transforms in sidebar
                 if ((ui.position.left <= 0) && (nb.metadata["sos"]["panel"].style === "float")) {
@@ -1153,15 +1194,15 @@
                     panel_cell.execute();
                     return false;
                 })
             );
 
         add_to_panel_history("sos", "%sossave --to html --force", "");
         add_to_panel_history("sos", "%preview --workflow", "");
-        add_to_panel_history("sos", "%tasks", "");
+        add_to_panel_history("sos", "%clear", "");
         add_to_panel_history("sos", "%toc", "");
 
         // make the font of the panel slightly smaller than the main notebook
         // unfortunately the code mirror input cell has fixed font size that cannot
         // be changed.
         this.cell.element[0].style.fontSize = "90%";
         console.log("panel rendered");
@@ -1702,14 +1743,62 @@
   padding-left: 0.1em;
 }
 */
 .CodeMirror-gutters {
   border-right: none;
   width: 1em;
 }
+
+time.pending, time.submitted, time.running  {
+  color: #cdb62c; /* yellow */
+}
+
+time.completed, time.result-ready {
+  color: #39aa56; /* green */
+}
+
+time.failed, time.signature-mismatch {
+  color: #db4545; /* red */
+}
+
+time.aborted, time.unknown {
+  color: #9d9d9d; /* gray */
+}
+
+.task_table a pre, .task_table i {
+  color: #666;
+}
+
+table.task_table {
+  border: 0px;
+  border-style: solid;
+}
+
+.task_hover {
+ color: black !important;
+}
+
+/* side panel */
+#panel-wrapper #panel .prompt,
+#panel-wrapper #panel .output_prompt,
+#panel-wrapper #panel .output_prompt_overplay {
+ min-width: 0px;
+}
+
+#panel-wrapper #panel div.output_area {
+  display: -webkit-box;
+}
+
+#panel-wrapper #panel div.output_subarea {
+  max_width: 100%;
+}
+
+#panel-wrapper #panel .output_scroll {
+  height: auto;
+}
 `;
             document.body.appendChild(css);
         };
 
         load_css();
 
         if (Jupyter.notebook.kernel) {
@@ -1747,31 +1836,19 @@
             download_menu.parentNode.insertBefore(menu[0], download_menu.nextSibling);
         }
     }
     */
 
     function adjustPanel() {
         if ($("#panel-wrapper").css("display") !== "none") {
-
             var panel_width = nb.metadata["sos"]["panel"].style === "side" ? $("#panel-wrapper").width() : 0;
             $("#notebook-container").css("margin-left", panel_width + 30);
             $("#notebook-container").css("width", $("#site").width() - panel_width - 30);
         }
         var cell = window.my_panel.cell;
-        $(".output_area .prompt", cell.element).remove()
-        $(".output_area .output_prompt", cell.element).remove()
-        $(".output_wrapper .out_prompt_overlay", cell.element).remove()
-        var ops = cell.element[0].getElementsByClassName("output_subarea");
-        for (var op = 0; op < ops.length; op++)
-            ops[op].style.maxWidth = "100%";
-        // this will create output_scroll if needed.
-        cell.output_area.scroll_if_long();
-        var ops = cell.element[0].getElementsByClassName("output_scroll");
-        if (ops.length > 0)
-            ops[0].style.height = "auto";
         cell.output_area.expand();
     }
 
     function patch_CodeCell_get_callbacks() {
         var previous_get_callbacks = CodeCell.prototype.get_callbacks;
         CodeCell.prototype.get_callbacks = function() {
             var that = this;
```

### Comparing `sos-notebook-0.9.9.7/src/sos_notebook/kernel.py` & `sos-notebook-0.9.9.8/src/sos_notebook/kernel.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,15 @@
         'codemirror_mode': 'sos',
         'nbconvert_exporter': 'sos_notebook.converter.SoS_Exporter',
     }
     banner = "SoS kernel - script of scripts"
 
     ALL_MAGICS = {
         'cd',
+        'clear',
         'debug',
         'dict',
         'get',
         'matplotlib',
         'paste',
         'preview',
         'pull',
@@ -158,14 +159,15 @@
     MAGIC_DEBUG = re.compile('^%debug(\s|$)')
     MAGIC_TASKINFO = re.compile('^%taskinfo(\s|$)')
     MAGIC_TASKS = re.compile('^%tasks(\s|$)')
     MAGIC_SKIP = re.compile('^%skip(\s|$)')
     MAGIC_TOC = re.compile('^%toc(\s|$)')
     MAGIC_RENDER = re.compile('^%render(\s|$)')
     MAGIC_SESSIONINFO = re.compile('^%sessioninfo(\s|$)')
+    MAGIC_CLEAR = re.compile('^%clear(\s|$)')
 
     def get_use_parser(self):
         parser = argparse.ArgumentParser(prog='%use',
             description='''Switch to a specified subkernel.''')
         parser.add_argument('name', nargs='?', default='',
             help='''Displayed name of kernel to start (if no kernel with name is
             specified) or switch to (if a kernel with this name is already started).
@@ -374,17 +376,18 @@
             help='''Message for git commit. Default to "save FILENAME"''')
         parser.add_argument('-p', '--push', action='store_true',
             help='''Push the commit with command "git push"''')
         parser.add_argument('-f', '--force', action='store_true',
             help='''If destination file already exists, overwrite it.''')
         parser.add_argument('-x', '--set-executable', dest = "setx", action='store_true',
             help='''Set `executable` permission to saved script.''')
-        parser.add_argument('--template', default='sos-report',
-            help='''Template to generate HTML output, default to sos-report,
-            which uses a control panel to control the display of contents.''')
+        parser.add_argument('--template', default='default-sos-template',
+            help='''Template to generate HTML output. The default template is a
+            template defined by configuration key default-sos-template, or
+            sos-report if such a key does not exist.''')
         parser.error = self._parse_error
         return parser
 
     def get_rerun_parser(self):
         parser = argparse.ArgumentParser(prog='%rerun',
             description='''Re-execute the last executed code, most likely with
             different command line options''')
@@ -512,14 +515,23 @@
     def get_sessioninfo_parser(self):
         parser = argparse.ArgumentParser(prog='%sessioninfo',
             description='''List the session info of all subkernels, and information
             stored in variable sessioninfo''')
         parser.error = self._parse_error
         return parser
 
+    def get_clear_parser(self):
+        parser = argparse.ArgumentParser(prog='%clear',
+            description='''Clear the output of the current cell, or the current
+            active cell if executed in the sidepanel.''')
+        parser.add_argument('-a', '--all', action='store_true',
+            help='''Clear all output of the current notebook.''')
+        parser.error = self._parse_error
+        return parser
+
     def find_kernel(self, name, kernel=None, language=None, color=None, notify_frontend=True):
         # find from subkernel name
         def update_existing(idx):
             x = self._kernel_list[idx]
             if (kernel is not None and kernel != x[1]) or (language is not None and language != x[2]):
                 raise ValueError('Cannot change kernel or language of predefined subkernel {}'.format(name))
             if color is not None:
@@ -787,15 +799,15 @@
         from sos.hosts import Host
         try:
             host = Host(queue)
         except Exception as e:
             self.warn('Invalid task queu {}: {}'.format(queue, e))
             return
         # get all tasks
-        for tid, tst, tdt in host._task_engine.monitor_tasks(tasks, status=None, age=age):
+        for tid, tst, tdt in host._task_engine.monitor_tasks(tasks, status=status, age=age):
             self.notify_task_status(['new-status', queue, tid, tst, tdt])
         self.send_frontend_msg('update-duration', {})
 
     def handle_sessioninfo(self):
         #
         from sos.utils import loaded_modules
         result = OrderedDict()
@@ -960,44 +972,50 @@
         if task_status[0] == 'new-status':
             tqu, tid, tst, tdt = task_status[1:]
             self.send_response(self.iopub_socket, 'display_data',
                 {
                     'source': 'SoS',
                     'metadata': {},
                     'data': { 'text/html':
-                        HTML('''<table id="table_{0}_{1}" style="border: 0px"><tr style="border: 0px">
+                        HTML('''<table id="table_{0}_{1}" class="task_table"><tr style="border: 0px">
                         <td style="border: 0px">
                         <i id="status_{0}_{1}"
                             class="fa fa-2x fa-fw {2}"
-                            onmouseover="$('#status_{0}_{1}').addClass('{3}').removeClass('{2}')"
-                            onmouseleave="$('#status_{0}_{1}').addClass('{2}').removeClass('{3}')"
+                            onmouseover="$('#status_{0}_{1}').addClass('{3} task_hover').removeClass('{2}')"
+                            onmouseleave="$('#status_{0}_{1}').addClass('{2}').removeClass('{3} task_hover')"
                             onclick="{4}('{1}', '{0}')"
                         ></i> </td>
                         <td style="border:0px"><a onclick="task_info('{1}', '{0}')"><pre>{1}</pre></a></td>
                         <td style="border:0px">&nbsp;</td>
                         <td style="border:0px;text-align=right;">
-                        <pre><time id="duration_{0}_{1}" datetime="{5}">{6}</time></pre></td>
+                        <pre><time id="duration_{0}_{1}" class="{7}" datetime="{5}">{6}</time></pre></td>
                         </tr>
                         </table>'''.format(tqu, tid, status_class[tst], action_class[tst], action_func[tst], tdt*1000,
-                            PrettyRelativeTime(time.time() - tdt))).data
+                            PrettyRelativeTime(time.time() - tdt), tst)).data
                         }
                 })
             # keep tracks of my tasks to avoid updating status of
             # tasks that does not belong to the notebook
             self.my_tasks[(tqu, tid)] = time.time()
         elif task_status[0] == 'remove-task':
             tqu, tid = task_status[1:]
             if (tqu, tid) in self.my_tasks:
                 self.send_frontend_msg('remove-task', [tqu, tid])
         elif task_status[0] == 'change-status':
             tqu, tid, tst = task_status[1:]
+            if tst not in ('pending', 'submitted', 'running', 'result-ready', 'completed',
+                    'failed', 'aborted', 'signature-mismatch'):
+                tst = 'unknown'
             self.send_frontend_msg('task-status', [tqu, tid, tst, status_class[tst], action_class[tst], action_func[tst]])
             self.my_tasks[(tqu, tid)] = time.time()
         elif task_status[0] == 'pulse-status':
             tqu, tid, tst = task_status[1:]
+            if tst not in ('pending', 'submitted', 'running', 'result-ready', 'completed',
+                    'failed', 'aborted', 'signature-mismatch'):
+                tst = 'unknown'
             if (tqu, tid) in self.my_tasks:
                 if time.time() - self.my_tasks[(tqu, tid)] < 20:
                     # if it has been within the first 20 seconds of new or updated message
                     # can confirm to verify it has been successfully delivered. Otherwise
                     # ignore such message
                     self.send_frontend_msg('task-status', [tqu, tid, tst, status_class[tst], action_class[tst], action_func[tst]])
         else:
@@ -2082,14 +2100,27 @@
             parser = self.get_shutdown_parser()
             try:
                 args = parser.parse_args(shlex.split(options))
             except SystemExit:
                 return
             self.shutdown_kernel(args.kernel if args.kernel else self.kernel, args.restart)
             return self._do_execute(remaining_code, silent, store_history, user_expressions, allow_stdin)
+        elif self.MAGIC_CLEAR.match(code):
+            options, remaining_code = self.get_magic_and_code(code, False)
+            parser = self.get_clear_parser()
+            try:
+                args = parser.parse_args(options.split())
+            except SystemExit:
+                return
+            # self.cell_idx could be reset by _do_execute
+            cell_idx = self.cell_idx
+            try:
+                return self._do_execute(remaining_code, silent, store_history, user_expressions, allow_stdin)
+            finally:
+                self.send_frontend_msg('clear-output', [cell_idx, args.all])
         elif self.MAGIC_FRONTEND.match(code):
             options, remaining_code = self.get_magic_and_code(code, False)
             try:
                 parser = self.get_frontend_parser()
                 try:
                     args = parser.parse_args(shlex.split(options))
                 except SystemExit:
@@ -2356,15 +2387,18 @@
             self.options = options + ' ' + self.options
             try:
                 # %run is executed in its own namespace
                 old_dict = env.sos_dict
                 self._reset_dict()
                 self._workflow_mode = True
                 #self.send_frontend_msg('preview-workflow', self._workflow)
-                self._do_execute(self._workflow, silent, store_history, user_expressions, allow_stdin)
+                if not self._workflow:
+                    self.warn('Nothing to execute (notebook workflow is empty).')
+                else:
+                    self._do_execute(self._workflow, silent, store_history, user_expressions, allow_stdin)
             except Exception as e:
                 self.warn('Failed to execute workflow: {}'.format(e))
                 raise
             finally:
                 old_dict.quick_update(env.sos_dict._dict)
                 env.sos_dict = old_dict
                 self._workflow_mode = False
@@ -2448,15 +2482,23 @@
                     if args.setx:
                         import stat
                         os.chmod(filename, os.stat(filename).st_mode | stat.S_IEXEC)
                 else:
                     # convert to sos report
                     from .converter import notebook_to_html
                     arg = argparse.Namespace()
-                    arg.template = args.template
+                    if args.template == 'default-sos-template':
+                        from sos.utils import load_config_files
+                        cfg = load_config_files()
+                        if 'default-sos-template' in cfg:
+                            arg.template = cfg['default-sos-template']
+                        else:
+                            arg.template = 'sos-report'
+                    else:
+                        arg.template = args.template
                     notebook_to_html(self._notebook_name + '.ipynb', filename, sargs=arg, unknown_args=[])
 
                 self.send_response(self.iopub_socket, 'display_data',
                     {'source': 'SoS', 'metadata': {},
                      'data': {
                          'text/plain': 'Workflow saved to {}\n'.format(filename),
                          'text/html': HTML('<div class="sos_hint">Workflow saved to <a href="{0}" target="_blank">{0}</a></div>'.format(filename)).data
@@ -2656,14 +2698,15 @@
                 self.cell_idx = None
             if code is None:
                 return
             try:
                 return self.run_cell(code, silent, store_history)
             except KeyboardInterrupt:
                 self.warn('Keyboard Interrupt\n')
+                self.KM.interrupt_kernel()
                 return {'status': 'abort', 'execution_count': self._execution_count}
         else:
             if code:
                 self.last_executed_code = code
             # run sos
             try:
                 self.run_sos_code(code, silent)
```

### Comparing `sos-notebook-0.9.9.7/src/sos_notebook/logo-64x64.png` & `sos-notebook-0.9.9.8/src/sos_notebook/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `sos-notebook-0.9.9.7/src/sos_notebook/preview.py` & `sos-notebook-0.9.9.8/src/sos_notebook/preview.py`

 * *Files identical despite different names*

### Comparing `sos-notebook-0.9.9.7/src/sos_notebook/sos-full.tpl` & `sos-notebook-0.9.9.8/src/sos_notebook/sos-full.tpl`

 * *Files identical despite different names*

### Comparing `sos-notebook-0.9.9.7/src/sos_notebook/sos-report.tpl` & `sos-notebook-0.9.9.8/src/sos_notebook/sos-report.tpl`

 * *Files identical despite different names*

### Comparing `sos-notebook-0.9.9.7/src/sos_notebook/sos_executor.py` & `sos-notebook-0.9.9.8/src/sos_notebook/sos_executor.py`

 * *Files identical despite different names*

### Comparing `sos-notebook-0.9.9.7/src/sos_notebook/sos_step.py` & `sos-notebook-0.9.9.8/src/sos_notebook/sos_step.py`

 * *Files identical despite different names*

### Comparing `sos-notebook-0.9.9.7/src/sos_notebook/test_utils.py` & `sos-notebook-0.9.9.8/src/sos_notebook/test_utils.py`

 * *Files identical despite different names*

### Comparing `sos-notebook-0.9.9.7/src/sos_notebook/visualize.py` & `sos-notebook-0.9.9.8/src/sos_notebook/visualize.py`

 * *Files identical despite different names*

### Comparing `sos-notebook-0.9.9.7/src/sos_notebook.egg-info/entry_points.txt` & `sos-notebook-0.9.9.8/src/sos_notebook.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `sos-notebook-0.9.9.7/src/sos_notebook.egg-info/PKG-INFO` & `sos-notebook-0.9.9.8/src/sos_notebook.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sos-notebook
-Version: 0.9.9.7
+Version: 0.9.9.8
 Summary: Script of Scripts (SoS): an interactive, cross-platform, and cross-language workflow system for reproducible data analysis
 Home-page: https://github.com/vatlab/SOS
 Author: Bo Peng
 Author-email: bpeng@mdanderson.org
 License: GPL3
 Description-Content-Type: UNKNOWN
 Description: Complex bioinformatic data analysis workflows involving multiple scripts
```

### Comparing `sos-notebook-0.9.9.7/src/sos_notebook.egg-info/SOURCES.txt` & `sos-notebook-0.9.9.8/src/sos_notebook.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sos-notebook-0.9.9.7/test/test_jupyter_convert.py` & `sos-notebook-0.9.9.8/test/test_jupyter_convert.py`

 * *Files identical despite different names*

### Comparing `sos-notebook-0.9.9.7/test/test_jupyter_sos.py` & `sos-notebook-0.9.9.8/test/test_jupyter_sos.py`

 * *Files identical despite different names*

### Comparing `sos-notebook-0.9.9.7/test/test_jupyter_tasks.py` & `sos-notebook-0.9.9.8/test/test_jupyter_tasks.py`

 * *Files identical despite different names*

### Comparing `sos-notebook-0.9.9.7/test/test_sos_completer.py` & `sos-notebook-0.9.9.8/test/test_sos_completer.py`

 * *Files identical despite different names*

### Comparing `sos-notebook-0.9.9.7/test/test_sos_inspector.py` & `sos-notebook-0.9.9.8/test/test_sos_inspector.py`

 * *Files identical despite different names*

### Comparing `sos-notebook-0.9.9.7/test/test_sos_kernel.py` & `sos-notebook-0.9.9.8/test/test_sos_kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,28 +105,28 @@
             execute(kc=kc, code="%dict a")
             res = get_result(iopub)
             self.assertEqual(res['a'], "$100")
             # reset sigil
             execute(kc=kc, code='%set_options sigil="${ }"')
             wait_for_idle(kc)
 
-#    @unittest.skipIf(sys.platform == 'win32', 'AppVeyor does not support linux based docker')
-#    def testPullPush(self):
-#        '''Test set_options of sigil'''
-#        import random
-#        fname = "push_pull_{}.txt".format(random.randint(1, 100000))
-#        with open(fname, 'w') as pp:
-#            pp.write('something')
-#        with sos_kernel() as kc:
-#            # create a data frame
-#            execute(kc=kc, code='%push {} --to docker -c ~/docker.yml'.format(fname))
-#            wait_for_idle(kc)
-#            os.remove(fname)
-#            self.assertFalse(os.path.isfile(fname))
-#            #
-#            execute(kc=kc, code='%pull {} --from docker -c ~/docker.yml'.format(fname))
-#            _, stderr = get_std_output(kc.iopub_channel)
-#            self.assertEqual(stderr, '', 'Expect no error, get {}'.format(stderr))
-#            self.assertTrue(os.path.isfile(fname))
+    @unittest.skipIf(sys.platform == 'win32', 'AppVeyor does not support linux based docker')
+    def testPullPush(self):
+        '''Test set_options of sigil'''
+        import random
+        fname = "push_pull_{}.txt".format(random.randint(1, 100000))
+        with open(fname, 'w') as pp:
+            pp.write('something')
+        with sos_kernel() as kc:
+            # create a data frame
+            execute(kc=kc, code='%push {} --to docker -c ~/docker.yml'.format(fname))
+            wait_for_idle(kc)
+            os.remove(fname)
+            self.assertFalse(os.path.isfile(fname))
+            #
+            execute(kc=kc, code='%pull {} --from docker -c ~/docker.yml'.format(fname))
+            _, stderr = get_std_output(kc.iopub_channel)
+            self.assertEqual(stderr, '', 'Expect no error, get {}'.format(stderr))
+            self.assertTrue(os.path.isfile(fname))
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `sos-notebook-0.9.9.7/test/test_sos_magics.py` & `sos-notebook-0.9.9.8/test/test_sos_magics.py`

 * *Files identical despite different names*

