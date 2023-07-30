# Comparing `tmp/first-breaks-picking-0.4.0a0.tar.gz` & `tmp/first-breaks-picking-0.4.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "first-breaks-picking-0.4.0a0.tar", last modified: Sun Jul 30 14:39:20 2023, max compression
+gzip compressed data, was "first-breaks-picking-0.4.0a1.tar", last modified: Sun Jul 30 14:46:13 2023, max compression
```

## Comparing `first-breaks-picking-0.4.0a0.tar` & `first-breaks-picking-0.4.0a1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 14:39:20.470008 first-breaks-picking-0.4.0a0/
--rw-rw-rw-   0        0        0    11558 2023-06-02 11:20:59.000000 first-breaks-picking-0.4.0a0/LICENSE
--rw-rw-rw-   0        0        0       98 2023-07-30 14:32:42.000000 first-breaks-picking-0.4.0a0/MANIFEST.in
--rw-rw-rw-   0        0        0    14383 2023-07-30 14:39:20.471009 first-breaks-picking-0.4.0a0/PKG-INFO
--rw-rw-rw-   0        0        0    23459 2023-07-26 15:35:42.000000 first-breaks-picking-0.4.0a0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 14:39:20.444116 first-breaks-picking-0.4.0a0/first_breaks/
--rw-rw-rw-   0        0        0     1125 2023-07-26 15:38:18.000000 first-breaks-picking-0.4.0a0/first_breaks/__init__.py
--rw-rw-rw-   0        0        0       96 2023-07-30 08:47:25.000000 first-breaks-picking-0.4.0a0/first_breaks/__main__.py
--rw-rw-rw-   0        0        0      352 2023-06-12 06:38:44.000000 first-breaks-picking-0.4.0a0/first_breaks/cli.py
--rw-rw-rw-   0        0        0     1090 2023-07-26 15:35:42.000000 first-breaks-picking-0.4.0a0/first_breaks/const.py
-drwxrwxrwx   0        0        0        0 2023-07-30 14:39:20.446899 first-breaks-picking-0.4.0a0/first_breaks/data_models/
--rw-rw-rw-   0        0        0        0 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a0/first_breaks/data_models/__init__.py
--rw-rw-rw-   0        0        0     1748 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a0/first_breaks/data_models/dependent.py
--rw-rw-rw-   0        0        0     2165 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a0/first_breaks/data_models/independent.py
--rw-rw-rw-   0        0        0      469 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a0/first_breaks/data_models/initialised_defaults.py
-drwxrwxrwx   0        0        0        0 2023-07-30 14:39:20.453897 first-breaks-picking-0.4.0a0/first_breaks/desktop/
--rw-rw-rw-   0        0        0        0 2023-05-10 12:43:20.000000 first-breaks-picking-0.4.0a0/first_breaks/desktop/__init__.py
--rw-rw-rw-   0        0        0     5684 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a0/first_breaks/desktop/byte_encode_unit_widget.py
--rw-rw-rw-   0        0        0     1969 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a0/first_breaks/desktop/combobox_with_mapping.py
--rw-rw-rw-   0        0        0    19451 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a0/first_breaks/desktop/graph.py
--rw-rw-rw-   0        0        0    20564 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a0/first_breaks/desktop/main_gui.py
--rw-rw-rw-   0        0        0     6900 2023-07-26 15:35:42.000000 first-breaks-picking-0.4.0a0/first_breaks/desktop/picking_widget.py
--rw-rw-rw-   0        0        0     2752 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a0/first_breaks/desktop/radioset_widget.py
--rw-rw-rw-   0        0        0     3672 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a0/first_breaks/desktop/slider_with_values.py
--rw-rw-rw-   0        0        0     2700 2023-07-10 12:37:21.000000 first-breaks-picking-0.4.0a0/first_breaks/desktop/threads.py
--rw-rw-rw-   0        0        0     4367 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a0/first_breaks/desktop/utils.py
--rw-rw-rw-   0        0        0     7676 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a0/first_breaks/desktop/visualization_settings_widget.py
-drwxrwxrwx   0        0        0        0 2023-07-30 14:39:20.456449 first-breaks-picking-0.4.0a0/first_breaks/picking/
--rw-rw-rw-   0        0        0        0 2023-05-30 07:39:18.000000 first-breaks-picking-0.4.0a0/first_breaks/picking/__init__.py
--rw-rw-rw-   0        0        0      955 2023-07-10 12:37:21.000000 first-breaks-picking-0.4.0a0/first_breaks/picking/ipicker.py
--rw-rw-rw-   0        0        0     5086 2023-07-26 15:35:42.000000 first-breaks-picking-0.4.0a0/first_breaks/picking/picker_onnx.py
--rw-rw-rw-   0        0        0     9580 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a0/first_breaks/picking/task.py
--rw-rw-rw-   0        0        0     2258 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a0/first_breaks/picking/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-30 14:39:20.460445 first-breaks-picking-0.4.0a0/first_breaks/sgy/
--rw-rw-rw-   0        0        0        0 2023-05-10 12:43:20.000000 first-breaks-picking-0.4.0a0/first_breaks/sgy/__init__.py
--rw-rw-rw-   0        0        0     8852 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a0/first_breaks/sgy/headers.py
--rw-rw-rw-   0        0        0    16648 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a0/first_breaks/sgy/reader.py
-drwxrwxrwx   0        0        0        0 2023-07-30 14:39:20.466209 first-breaks-picking-0.4.0a0/first_breaks/utils/
--rw-rw-rw-   0        0        0        0 2023-05-10 12:43:20.000000 first-breaks-picking-0.4.0a0/first_breaks/utils/__init__.py
--rw-rw-rw-   0        0        0     2774 2023-07-26 15:35:42.000000 first-breaks-picking-0.4.0a0/first_breaks/utils/cuda.py
--rw-rw-rw-   0        0        0      635 2023-05-10 12:43:20.000000 first-breaks-picking-0.4.0a0/first_breaks/utils/debug.py
--rw-rw-rw-   0        0        0     5698 2023-07-21 15:09:17.000000 first-breaks-picking-0.4.0a0/first_breaks/utils/utils.py
--rw-rw-rw-   0        0        0     3815 2023-05-26 13:27:32.000000 first-breaks-picking-0.4.0a0/first_breaks/utils/visualizations.py
-drwxrwxrwx   0        0        0        0 2023-07-30 14:39:20.470008 first-breaks-picking-0.4.0a0/first_breaks_picking.egg-info/
--rw-rw-rw-   0        0        0    14383 2023-07-30 14:39:20.000000 first-breaks-picking-0.4.0a0/first_breaks_picking.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1399 2023-07-30 14:39:20.000000 first-breaks-picking-0.4.0a0/first_breaks_picking.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 14:39:20.000000 first-breaks-picking-0.4.0a0/first_breaks_picking.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2023-07-30 14:39:20.000000 first-breaks-picking-0.4.0a0/first_breaks_picking.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      153 2023-07-30 14:39:20.000000 first-breaks-picking-0.4.0a0/first_breaks_picking.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-30 14:39:20.000000 first-breaks-picking-0.4.0a0/first_breaks_picking.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2814 2023-07-30 14:35:20.000000 first-breaks-picking-0.4.0a0/pyproject.toml
--rw-rw-rw-   0        0        0      356 2023-07-30 14:39:20.471009 first-breaks-picking-0.4.0a0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-30 14:46:13.235714 first-breaks-picking-0.4.0a1/
+-rw-rw-rw-   0        0        0    11558 2023-06-02 11:20:59.000000 first-breaks-picking-0.4.0a1/LICENSE
+-rw-rw-rw-   0        0        0       98 2023-07-30 14:32:42.000000 first-breaks-picking-0.4.0a1/MANIFEST.in
+-rw-rw-rw-   0        0        0    37844 2023-07-30 14:46:13.237035 first-breaks-picking-0.4.0a1/PKG-INFO
+-rw-rw-rw-   0        0        0    23459 2023-07-26 15:35:42.000000 first-breaks-picking-0.4.0a1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 14:46:13.216125 first-breaks-picking-0.4.0a1/first_breaks/
+-rw-rw-rw-   0        0        0     1125 2023-07-26 15:38:18.000000 first-breaks-picking-0.4.0a1/first_breaks/__init__.py
+-rw-rw-rw-   0        0        0       96 2023-07-30 08:47:25.000000 first-breaks-picking-0.4.0a1/first_breaks/__main__.py
+-rw-rw-rw-   0        0        0      352 2023-06-12 06:38:44.000000 first-breaks-picking-0.4.0a1/first_breaks/cli.py
+-rw-rw-rw-   0        0        0     1090 2023-07-26 15:35:42.000000 first-breaks-picking-0.4.0a1/first_breaks/const.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:46:13.217936 first-breaks-picking-0.4.0a1/first_breaks/data_models/
+-rw-rw-rw-   0        0        0        0 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a1/first_breaks/data_models/__init__.py
+-rw-rw-rw-   0        0        0     1748 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a1/first_breaks/data_models/dependent.py
+-rw-rw-rw-   0        0        0     2165 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a1/first_breaks/data_models/independent.py
+-rw-rw-rw-   0        0        0      469 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a1/first_breaks/data_models/initialised_defaults.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:46:13.224933 first-breaks-picking-0.4.0a1/first_breaks/desktop/
+-rw-rw-rw-   0        0        0        0 2023-05-10 12:43:20.000000 first-breaks-picking-0.4.0a1/first_breaks/desktop/__init__.py
+-rw-rw-rw-   0        0        0     5684 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a1/first_breaks/desktop/byte_encode_unit_widget.py
+-rw-rw-rw-   0        0        0     1969 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a1/first_breaks/desktop/combobox_with_mapping.py
+-rw-rw-rw-   0        0        0    19451 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a1/first_breaks/desktop/graph.py
+-rw-rw-rw-   0        0        0    20564 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a1/first_breaks/desktop/main_gui.py
+-rw-rw-rw-   0        0        0     6900 2023-07-26 15:35:42.000000 first-breaks-picking-0.4.0a1/first_breaks/desktop/picking_widget.py
+-rw-rw-rw-   0        0        0     2752 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a1/first_breaks/desktop/radioset_widget.py
+-rw-rw-rw-   0        0        0     3672 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a1/first_breaks/desktop/slider_with_values.py
+-rw-rw-rw-   0        0        0     2700 2023-07-10 12:37:21.000000 first-breaks-picking-0.4.0a1/first_breaks/desktop/threads.py
+-rw-rw-rw-   0        0        0     4367 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a1/first_breaks/desktop/utils.py
+-rw-rw-rw-   0        0        0     7676 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a1/first_breaks/desktop/visualization_settings_widget.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:46:13.227720 first-breaks-picking-0.4.0a1/first_breaks/picking/
+-rw-rw-rw-   0        0        0        0 2023-05-30 07:39:18.000000 first-breaks-picking-0.4.0a1/first_breaks/picking/__init__.py
+-rw-rw-rw-   0        0        0      955 2023-07-10 12:37:21.000000 first-breaks-picking-0.4.0a1/first_breaks/picking/ipicker.py
+-rw-rw-rw-   0        0        0     5086 2023-07-26 15:35:42.000000 first-breaks-picking-0.4.0a1/first_breaks/picking/picker_onnx.py
+-rw-rw-rw-   0        0        0     9580 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a1/first_breaks/picking/task.py
+-rw-rw-rw-   0        0        0     2258 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a1/first_breaks/picking/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:46:13.229714 first-breaks-picking-0.4.0a1/first_breaks/sgy/
+-rw-rw-rw-   0        0        0        0 2023-05-10 12:43:20.000000 first-breaks-picking-0.4.0a1/first_breaks/sgy/__init__.py
+-rw-rw-rw-   0        0        0     8852 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a1/first_breaks/sgy/headers.py
+-rw-rw-rw-   0        0        0    16648 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a1/first_breaks/sgy/reader.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:46:13.231714 first-breaks-picking-0.4.0a1/first_breaks/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-10 12:43:20.000000 first-breaks-picking-0.4.0a1/first_breaks/utils/__init__.py
+-rw-rw-rw-   0        0        0     2774 2023-07-26 15:35:42.000000 first-breaks-picking-0.4.0a1/first_breaks/utils/cuda.py
+-rw-rw-rw-   0        0        0      635 2023-05-10 12:43:20.000000 first-breaks-picking-0.4.0a1/first_breaks/utils/debug.py
+-rw-rw-rw-   0        0        0     5698 2023-07-21 15:09:17.000000 first-breaks-picking-0.4.0a1/first_breaks/utils/utils.py
+-rw-rw-rw-   0        0        0     3815 2023-05-26 13:27:32.000000 first-breaks-picking-0.4.0a1/first_breaks/utils/visualizations.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:46:13.235714 first-breaks-picking-0.4.0a1/first_breaks_picking.egg-info/
+-rw-rw-rw-   0        0        0    37844 2023-07-30 14:46:13.000000 first-breaks-picking-0.4.0a1/first_breaks_picking.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1399 2023-07-30 14:46:13.000000 first-breaks-picking-0.4.0a1/first_breaks_picking.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 14:46:13.000000 first-breaks-picking-0.4.0a1/first_breaks_picking.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-07-30 14:46:13.000000 first-breaks-picking-0.4.0a1/first_breaks_picking.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      153 2023-07-30 14:46:13.000000 first-breaks-picking-0.4.0a1/first_breaks_picking.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-30 14:46:13.000000 first-breaks-picking-0.4.0a1/first_breaks_picking.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2816 2023-07-30 14:45:38.000000 first-breaks-picking-0.4.0a1/pyproject.toml
+-rw-rw-rw-   0        0        0      356 2023-07-30 14:46:13.237829 first-breaks-picking-0.4.0a1/setup.cfg
```

### Comparing `first-breaks-picking-0.4.0a0/LICENSE` & `first-breaks-picking-0.4.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.4.0a0/README.md` & `first-breaks-picking-0.4.0a1/README.md`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.4.0a0/first_breaks/__init__.py` & `first-breaks-picking-0.4.0a1/first_breaks/__init__.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.4.0a0/first_breaks/const.py` & `first-breaks-picking-0.4.0a1/first_breaks/const.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.4.0a0/first_breaks/data_models/dependent.py` & `first-breaks-picking-0.4.0a1/first_breaks/data_models/dependent.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.4.0a0/first_breaks/data_models/independent.py` & `first-breaks-picking-0.4.0a1/first_breaks/data_models/independent.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.4.0a0/first_breaks/desktop/byte_encode_unit_widget.py` & `first-breaks-picking-0.4.0a1/first_breaks/desktop/byte_encode_unit_widget.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.4.0a0/first_breaks/desktop/combobox_with_mapping.py` & `first-breaks-picking-0.4.0a1/first_breaks/desktop/combobox_with_mapping.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.4.0a0/first_breaks/desktop/graph.py` & `first-breaks-picking-0.4.0a1/first_breaks/desktop/graph.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.4.0a0/first_breaks/desktop/main_gui.py` & `first-breaks-picking-0.4.0a1/first_breaks/desktop/main_gui.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.4.0a0/first_breaks/desktop/picking_widget.py` & `first-breaks-picking-0.4.0a1/first_breaks/desktop/picking_widget.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.4.0a0/first_breaks/desktop/radioset_widget.py` & `first-breaks-picking-0.4.0a1/first_breaks/desktop/radioset_widget.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.4.0a0/first_breaks/desktop/slider_with_values.py` & `first-breaks-picking-0.4.0a1/first_breaks/desktop/slider_with_values.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.4.0a0/first_breaks/desktop/threads.py` & `first-breaks-picking-0.4.0a1/first_breaks/desktop/threads.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.4.0a0/first_breaks/desktop/utils.py` & `first-breaks-picking-0.4.0a1/first_breaks/desktop/utils.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.4.0a0/first_breaks/desktop/visualization_settings_widget.py` & `first-breaks-picking-0.4.0a1/first_breaks/desktop/visualization_settings_widget.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.4.0a0/first_breaks/picking/ipicker.py` & `first-breaks-picking-0.4.0a1/first_breaks/picking/ipicker.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.4.0a0/first_breaks/picking/picker_onnx.py` & `first-breaks-picking-0.4.0a1/first_breaks/picking/picker_onnx.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.4.0a0/first_breaks/picking/task.py` & `first-breaks-picking-0.4.0a1/first_breaks/picking/task.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.4.0a0/first_breaks/picking/utils.py` & `first-breaks-picking-0.4.0a1/first_breaks/picking/utils.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.4.0a0/first_breaks/sgy/headers.py` & `first-breaks-picking-0.4.0a1/first_breaks/sgy/headers.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.4.0a0/first_breaks/sgy/reader.py` & `first-breaks-picking-0.4.0a1/first_breaks/sgy/reader.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.4.0a0/first_breaks/utils/cuda.py` & `first-breaks-picking-0.4.0a1/first_breaks/utils/cuda.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.4.0a0/first_breaks/utils/debug.py` & `first-breaks-picking-0.4.0a1/first_breaks/utils/debug.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.4.0a0/first_breaks/utils/utils.py` & `first-breaks-picking-0.4.0a1/first_breaks/utils/utils.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.4.0a0/first_breaks/utils/visualizations.py` & `first-breaks-picking-0.4.0a1/first_breaks/utils/visualizations.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.4.0a0/first_breaks_picking.egg-info/SOURCES.txt` & `first-breaks-picking-0.4.0a1/first_breaks_picking.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.4.0a0/pyproject.toml` & `first-breaks-picking-0.4.0a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "first-breaks-picking"
-version = "0.4.0a"
+version = "0.4.0a1"
 description = "Project is devoted to pick waves that are the first to be detected on a seismogram with neural network"
-readme = {file = "README.txt", content-type = "text/markdown"}
+readme = {file = "README.md", content-type = "text/markdown"}
+
 requires-python = ">=3.8,<=3.10"
 authors = [
     {name = "Aleksei Tarasov"},
     {name = "Aleksei Tarasov", email = "aleksei.v.tarasov@gmail.com"}
 ]
 urls = {Homepage = "https://github.com/DaloroAT/first_breaks_picking"}
 keywords = [
```

