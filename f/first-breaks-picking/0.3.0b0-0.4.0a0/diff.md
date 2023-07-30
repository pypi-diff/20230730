# Comparing `tmp/first-breaks-picking-0.3.0b0.tar.gz` & `tmp/first-breaks-picking-0.4.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "first-breaks-picking-0.3.0b0.tar", last modified: Wed Jul 19 05:44:41 2023, max compression
+gzip compressed data, was "first-breaks-picking-0.4.0a0.tar", last modified: Sun Jul 30 14:39:20 2023, max compression
```

## Comparing `first-breaks-picking-0.3.0b0.tar` & `first-breaks-picking-0.4.0a0.tar`

### file list

```diff
@@ -1,66 +1,52 @@
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/
--rw-r--r--   0 daloro    (1000) daloro    (1000)    11357 2023-05-10 12:43:20.000000 first-breaks-picking-0.3.0b0/LICENSE
--rw-rw-r--   0 daloro    (1000) daloro    (1000)    24007 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/PKG-INFO
--rw-r--r--   0 daloro    (1000) daloro    (1000)    22791 2023-07-19 05:43:43.000000 first-breaks-picking-0.3.0b0/README.md
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/first_breaks/
--rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-05-10 12:43:20.000000 first-breaks-picking-0.3.0b0/first_breaks/__init__.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/first_breaks/_pytorch/
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/first_breaks/_pytorch/models/
--rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/first_breaks/_pytorch/models/__init__.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     5730 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/first_breaks/_pytorch/models/unet3plus.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)      352 2023-06-12 06:38:44.000000 first-breaks-picking-0.3.0b0/first_breaks/cli.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     1171 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/first_breaks/const.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/first_breaks/data_models/
--rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-07-17 07:07:08.000000 first-breaks-picking-0.3.0b0/first_breaks/data_models/__init__.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     1701 2023-07-18 13:44:34.000000 first-breaks-picking-0.3.0b0/first_breaks/data_models/dependent.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     2090 2023-07-18 17:00:55.000000 first-breaks-picking-0.3.0b0/first_breaks/data_models/independent.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)      441 2023-07-18 13:44:34.000000 first-breaks-picking-0.3.0b0/first_breaks/data_models/initialised_defaults.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/first_breaks/desktop/
--rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-05-10 12:43:20.000000 first-breaks-picking-0.3.0b0/first_breaks/desktop/__init__.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     5525 2023-07-18 16:48:46.000000 first-breaks-picking-0.3.0b0/first_breaks/desktop/byte_encode_unit_widget.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     1903 2023-07-18 16:49:22.000000 first-breaks-picking-0.3.0b0/first_breaks/desktop/combobox_with_mapping.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)    18931 2023-07-18 13:48:53.000000 first-breaks-picking-0.3.0b0/first_breaks/desktop/graph.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)    20070 2023-07-19 05:38:40.000000 first-breaks-picking-0.3.0b0/first_breaks/desktop/main_gui.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     6739 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/first_breaks/desktop/picking_widget.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     2661 2023-07-18 16:49:29.000000 first-breaks-picking-0.3.0b0/first_breaks/desktop/radioset_widget.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     3571 2023-07-18 16:49:46.000000 first-breaks-picking-0.3.0b0/first_breaks/desktop/slider_with_values.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     2700 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/first_breaks/desktop/threads.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     4238 2023-07-18 16:49:38.000000 first-breaks-picking-0.3.0b0/first_breaks/desktop/utils.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     7474 2023-07-18 16:47:54.000000 first-breaks-picking-0.3.0b0/first_breaks/desktop/visualization_settings_widget.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/first_breaks/picking/
--rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-05-30 07:39:18.000000 first-breaks-picking-0.3.0b0/first_breaks/picking/__init__.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)      955 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/first_breaks/picking/ipicker.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     4952 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/first_breaks/picking/picker_onnx.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     9351 2023-07-18 16:46:26.000000 first-breaks-picking-0.3.0b0/first_breaks/picking/task.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     2197 2023-07-18 17:00:56.000000 first-breaks-picking-0.3.0b0/first_breaks/picking/utils.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/first_breaks/sgy/
--rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-05-10 12:43:20.000000 first-breaks-picking-0.3.0b0/first_breaks/sgy/__init__.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     8608 2023-07-18 16:49:53.000000 first-breaks-picking-0.3.0b0/first_breaks/sgy/headers.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)    16232 2023-07-18 16:46:38.000000 first-breaks-picking-0.3.0b0/first_breaks/sgy/reader.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/first_breaks/utils/
--rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-05-10 12:43:20.000000 first-breaks-picking-0.3.0b0/first_breaks/utils/__init__.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)      635 2023-05-10 12:43:20.000000 first-breaks-picking-0.3.0b0/first_breaks/utils/debug.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     5833 2023-07-18 16:46:46.000000 first-breaks-picking-0.3.0b0/first_breaks/utils/utils.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     3815 2023-05-26 13:27:32.000000 first-breaks-picking-0.3.0b0/first_breaks/utils/visualizations.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/first_breaks_picking.egg-info/
--rw-rw-r--   0 daloro    (1000) daloro    (1000)    24007 2023-07-19 05:44:41.000000 first-breaks-picking-0.3.0b0/first_breaks_picking.egg-info/PKG-INFO
--rw-rw-r--   0 daloro    (1000) daloro    (1000)     1683 2023-07-19 05:44:41.000000 first-breaks-picking-0.3.0b0/first_breaks_picking.egg-info/SOURCES.txt
--rw-rw-r--   0 daloro    (1000) daloro    (1000)        1 2023-07-19 05:44:41.000000 first-breaks-picking-0.3.0b0/first_breaks_picking.egg-info/dependency_links.txt
--rw-rw-r--   0 daloro    (1000) daloro    (1000)       71 2023-07-19 05:44:41.000000 first-breaks-picking-0.3.0b0/first_breaks_picking.egg-info/entry_points.txt
--rw-rw-r--   0 daloro    (1000) daloro    (1000)      184 2023-07-19 05:44:41.000000 first-breaks-picking-0.3.0b0/first_breaks_picking.egg-info/requires.txt
--rw-rw-r--   0 daloro    (1000) daloro    (1000)       19 2023-07-19 05:44:41.000000 first-breaks-picking-0.3.0b0/first_breaks_picking.egg-info/top_level.txt
--rw-r--r--   0 daloro    (1000) daloro    (1000)      337 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/setup.cfg
--rw-rw-r--   0 daloro    (1000) daloro    (1000)     2238 2023-07-18 16:41:29.000000 first-breaks-picking-0.3.0b0/setup.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/tests/
--rw-r--r--   0 daloro    (1000) daloro    (1000)      330 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/tests/test_demo_sgy.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/tests/test_desktop/
--rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/tests/test_desktop/__init__.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/tests/test_desktop/test_graph.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/tests/test_picking/
--rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/tests/test_picking/__init__.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     1288 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/tests/test_picking/test_picker.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     3329 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/tests/test_picking/test_task.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     1467 2023-07-18 16:41:44.000000 first-breaks-picking-0.3.0b0/tests/test_readme_examples.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/tests/test_sgy/
--rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/tests/test_sgy/__init__.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     1859 2023-07-18 12:38:11.000000 first-breaks-picking-0.3.0b0/tests/test_sgy/test_reader.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:39:20.470008 first-breaks-picking-0.4.0a0/
+-rw-rw-rw-   0        0        0    11558 2023-06-02 11:20:59.000000 first-breaks-picking-0.4.0a0/LICENSE
+-rw-rw-rw-   0        0        0       98 2023-07-30 14:32:42.000000 first-breaks-picking-0.4.0a0/MANIFEST.in
+-rw-rw-rw-   0        0        0    14383 2023-07-30 14:39:20.471009 first-breaks-picking-0.4.0a0/PKG-INFO
+-rw-rw-rw-   0        0        0    23459 2023-07-26 15:35:42.000000 first-breaks-picking-0.4.0a0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 14:39:20.444116 first-breaks-picking-0.4.0a0/first_breaks/
+-rw-rw-rw-   0        0        0     1125 2023-07-26 15:38:18.000000 first-breaks-picking-0.4.0a0/first_breaks/__init__.py
+-rw-rw-rw-   0        0        0       96 2023-07-30 08:47:25.000000 first-breaks-picking-0.4.0a0/first_breaks/__main__.py
+-rw-rw-rw-   0        0        0      352 2023-06-12 06:38:44.000000 first-breaks-picking-0.4.0a0/first_breaks/cli.py
+-rw-rw-rw-   0        0        0     1090 2023-07-26 15:35:42.000000 first-breaks-picking-0.4.0a0/first_breaks/const.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:39:20.446899 first-breaks-picking-0.4.0a0/first_breaks/data_models/
+-rw-rw-rw-   0        0        0        0 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a0/first_breaks/data_models/__init__.py
+-rw-rw-rw-   0        0        0     1748 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a0/first_breaks/data_models/dependent.py
+-rw-rw-rw-   0        0        0     2165 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a0/first_breaks/data_models/independent.py
+-rw-rw-rw-   0        0        0      469 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a0/first_breaks/data_models/initialised_defaults.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:39:20.453897 first-breaks-picking-0.4.0a0/first_breaks/desktop/
+-rw-rw-rw-   0        0        0        0 2023-05-10 12:43:20.000000 first-breaks-picking-0.4.0a0/first_breaks/desktop/__init__.py
+-rw-rw-rw-   0        0        0     5684 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a0/first_breaks/desktop/byte_encode_unit_widget.py
+-rw-rw-rw-   0        0        0     1969 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a0/first_breaks/desktop/combobox_with_mapping.py
+-rw-rw-rw-   0        0        0    19451 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a0/first_breaks/desktop/graph.py
+-rw-rw-rw-   0        0        0    20564 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a0/first_breaks/desktop/main_gui.py
+-rw-rw-rw-   0        0        0     6900 2023-07-26 15:35:42.000000 first-breaks-picking-0.4.0a0/first_breaks/desktop/picking_widget.py
+-rw-rw-rw-   0        0        0     2752 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a0/first_breaks/desktop/radioset_widget.py
+-rw-rw-rw-   0        0        0     3672 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a0/first_breaks/desktop/slider_with_values.py
+-rw-rw-rw-   0        0        0     2700 2023-07-10 12:37:21.000000 first-breaks-picking-0.4.0a0/first_breaks/desktop/threads.py
+-rw-rw-rw-   0        0        0     4367 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a0/first_breaks/desktop/utils.py
+-rw-rw-rw-   0        0        0     7676 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a0/first_breaks/desktop/visualization_settings_widget.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:39:20.456449 first-breaks-picking-0.4.0a0/first_breaks/picking/
+-rw-rw-rw-   0        0        0        0 2023-05-30 07:39:18.000000 first-breaks-picking-0.4.0a0/first_breaks/picking/__init__.py
+-rw-rw-rw-   0        0        0      955 2023-07-10 12:37:21.000000 first-breaks-picking-0.4.0a0/first_breaks/picking/ipicker.py
+-rw-rw-rw-   0        0        0     5086 2023-07-26 15:35:42.000000 first-breaks-picking-0.4.0a0/first_breaks/picking/picker_onnx.py
+-rw-rw-rw-   0        0        0     9580 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a0/first_breaks/picking/task.py
+-rw-rw-rw-   0        0        0     2258 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a0/first_breaks/picking/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:39:20.460445 first-breaks-picking-0.4.0a0/first_breaks/sgy/
+-rw-rw-rw-   0        0        0        0 2023-05-10 12:43:20.000000 first-breaks-picking-0.4.0a0/first_breaks/sgy/__init__.py
+-rw-rw-rw-   0        0        0     8852 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a0/first_breaks/sgy/headers.py
+-rw-rw-rw-   0        0        0    16648 2023-07-21 14:52:38.000000 first-breaks-picking-0.4.0a0/first_breaks/sgy/reader.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:39:20.466209 first-breaks-picking-0.4.0a0/first_breaks/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-10 12:43:20.000000 first-breaks-picking-0.4.0a0/first_breaks/utils/__init__.py
+-rw-rw-rw-   0        0        0     2774 2023-07-26 15:35:42.000000 first-breaks-picking-0.4.0a0/first_breaks/utils/cuda.py
+-rw-rw-rw-   0        0        0      635 2023-05-10 12:43:20.000000 first-breaks-picking-0.4.0a0/first_breaks/utils/debug.py
+-rw-rw-rw-   0        0        0     5698 2023-07-21 15:09:17.000000 first-breaks-picking-0.4.0a0/first_breaks/utils/utils.py
+-rw-rw-rw-   0        0        0     3815 2023-05-26 13:27:32.000000 first-breaks-picking-0.4.0a0/first_breaks/utils/visualizations.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:39:20.470008 first-breaks-picking-0.4.0a0/first_breaks_picking.egg-info/
+-rw-rw-rw-   0        0        0    14383 2023-07-30 14:39:20.000000 first-breaks-picking-0.4.0a0/first_breaks_picking.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1399 2023-07-30 14:39:20.000000 first-breaks-picking-0.4.0a0/first_breaks_picking.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 14:39:20.000000 first-breaks-picking-0.4.0a0/first_breaks_picking.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-07-30 14:39:20.000000 first-breaks-picking-0.4.0a0/first_breaks_picking.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      153 2023-07-30 14:39:20.000000 first-breaks-picking-0.4.0a0/first_breaks_picking.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-30 14:39:20.000000 first-breaks-picking-0.4.0a0/first_breaks_picking.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2814 2023-07-30 14:35:20.000000 first-breaks-picking-0.4.0a0/pyproject.toml
+-rw-rw-rw-   0        0        0      356 2023-07-30 14:39:20.471009 first-breaks-picking-0.4.0a0/setup.cfg
```

### Comparing `first-breaks-picking-0.3.0b0/LICENSE` & `first-breaks-picking-0.4.0a0/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `first-breaks-picking-0.3.0b0/PKG-INFO` & `first-breaks-picking-0.4.0a0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,661 +1,634 @@
-Metadata-Version: 2.1
-Name: first-breaks-picking
-Version: 0.3.0b0
-Summary: Tool for picking first breaks in seismic gather
-Home-page: https://github.com/DaloroAT/first_breaks_picking
-Author: Aleksei Tarasov
-Author-email: aleksei.v.tarasov@gmail.com
-License: Apache License 2.0
-Project-URL: Homepage, https://github.com/DaloroAT/first_breaks_picking
-Keywords: seismic,first-breaks,computer-vision,deep-learning,segmentation,data-science
-Classifier: Environment :: Console
-Classifier: Environment :: X11 Applications :: Qt
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Image Recognition
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8,<3.9
-Description-Content-Type: text/markdown
-Provides-Extra: gpu
-License-File: LICENSE
-
-# First breaks picking
-This project is devoted to pick waves that are the first to be detected on a seismogram (first breaks, first arrivals).
-Traditionally, this procedure is performed manually. When processing field data, the number of picks reaches hundreds of
-thousands. Existing analytical methods allow you to automate picking only on high-quality data with a high
-signal / noise ratio.
-
-As a more robust algorithm, it is proposed to use a neural network to pick the first breaks. Since the data on adjacent
-seismic traces have similarities in the features of the wave field, **we pick first breaks on 2D seismic gather**, not
-individual traces.
-
-<p align="center">
-<img src="https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/readme_images/project_preview.png" />
-</p>
-
-# Examples
-
-In the drop-down menus below you will find examples of our model picking on good quality data as well as noisy ones.
-
-It is difficult to validate the quality of the model on noisy data, but they show the robustness of the model to
-various types of noise.
-
-<details>
-<summary>Good quality data</summary>
-
-![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/normal/normal_0.png)
-
-![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/normal/normal_1.png)
-
-![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/normal/normal_2.png)
-
-![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/normal/normal_3.png)
-
-![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/normal/normal_4.png)
-
-![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/normal/normal_5.png)
-
-![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/normal/normal_6.png)
-
-![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/normal/normal_7.png)
-
-![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/normal/normal_8.png)
-
-![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/normal/normal_9.png)
-
-![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/normal/normal_10.png)
-
-![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/normal/normal_11.png)
-
-![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/normal/normal_12.png)
-
-![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/normal/normal_13.png)
-
-![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/normal/normal_14.png)
-
-</details>
-
-<details>
-<summary>Noisy data</summary>
-
-![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/noisy/noisy_0.png)
-
-![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/noisy/noisy_1.png)
-
-![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/noisy/noisy_2.png)
-
-![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/noisy/noisy_3.png)
-
-![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/noisy/noisy_4.png)
-
-![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/noisy/noisy_5.png)
-
-![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/noisy/noisy_6.png)
-
-</details>
-
-# Installation
-
-Library is available in [PyPI](https://pypi.org/project/first-breaks-picking/):
-```shell
-pip install -U first-breaks-picking
-```
-
-### GPU support
-
-You can use the capabilities of GPU to significantly reduce picking time. Before started, check
-[here](https://developer.nvidia.com/cuda-gpus) that your GPU is CUDA compatible.
-
-Install GPU supported version of library:
-```shell
-pip install -U first-breaks-picking[gpu]
-```
-
-The following steps are operating system dependent and must be performed manually:
-
-- Install [latest NVIDIA drivers](https://www.nvidia.com/Download/index.aspx).
-- Install [CUDA toolkit](https://developer.nvidia.com/cuda-downloads).
-**The version must be between 11.x, starting with 11.6. Version 12 is not supported**.
-- Install ZLib and CuDNN:
-[Windows](https://docs.nvidia.com/deeplearning/cudnn/install-guide/index.html#install-windows) and
-[Linux](https://docs.nvidia.com/deeplearning/cudnn/install-guide/index.html#install-linux).
-
-### Extra data
-
-- To pick first breaks you need
-to [download model](https://oml.daloroserver.com/download/seis/fb.onnx).
-
-- If you have no seismic data, you can also
-[download small SGY file](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/data/real_gather.sgy).
-
-It's also possible to download them with Python using the following snippet:
-
-[code-block-start]:downloading-extra
-```python
-from first_breaks.utils.utils import (download_demo_sgy,
-                                      download_model_onnx)
-
-sgy_filename = 'data.sgy'
-model_filename = 'model.onnx'
-
-download_demo_sgy(sgy_filename)
-download_model_onnx(model_filename)
-```
-[code-block-end]:downloading-extra
-
-# How to use it
-
-The library can be used in Python, or you can use the desktop application.
-
-## Python
-
-Programmatic way has more flexibility for building your own picking scenario and processing multiple files.
-
-### Minimal example
-
-The following snippet implements the picking process of the demo file. As a result, you can get an image from
-the project preview.
-
-[code-block-start]:e2e-example
-```python
-from first_breaks.utils.utils import download_demo_sgy
-from first_breaks.sgy.reader import SGY
-from first_breaks.picking.task import Task
-from first_breaks.picking.picker_onnx import PickerONNX
-from first_breaks.desktop.graph import export_image
-
-sgy_filename = 'data.sgy'
-download_demo_sgy(fname=sgy_filename)
-sgy = SGY(sgy_filename)
-
-task = Task(sgy_filename,
-            traces_per_gather=12,
-            maximum_time=100,
-            gain=2)
-picker = PickerONNX()
-task = picker.process_task(task)
-
-# create an image with default parameters
-image_filename = 'default_view.png'
-export_image(task, image_filename)
-
-# create an image from the project preview
-image_filename = 'project_preview.png'
-export_image(task, image_filename,
-             time_window=(0, 60),
-             traces_window=(79.5, 90.5),
-             show_processing_region=False,
-             headers_total_pixels=80,
-             height=500,
-             width=700,
-             hide_traces_axis=True)
-```
-[code-block-end]:e2e-example
-
-For a better understanding of the steps taken, expand and read the next section.
-
-### Detailed examples
-
-<details>
-
-<summary>Show examples</summary>
-
-### Download demo SGY
-
-Let's download the demo file. All the following examples assume that the file is downloaded and saved as `data.sgy`.
-You can also put your own SGY file.
-
-```python
-from first_breaks.utils.utils import download_demo_sgy
-
-sgy_filename = 'data.sgy'
-download_demo_sgy(fname=sgy_filename)
-```
-
-### Create SGY
-We provide several ways to create `SGY` object: from file, `bytes` or `numpy` array.
-
-From file:
-
-[code-block-start]:init-from-path
-```python
-from first_breaks.sgy.reader import SGY
-
-sgy_filename = 'data.sgy'
-sgy = SGY(sgy_filename)
-```
-[code-block-end]:init-from-path
-
-From `bytes`:
-
-[code-block-start]:init-from-bytes
-```python
-from first_breaks.sgy.reader import SGY
-
-sgy_filename = 'data.sgy'
-
-with open(sgy_filename, 'rb') as fin:
-    sgy_bytes = fin.read()
-
-sgy = SGY(sgy_bytes)
-```
-[code-block-end]:init-from-bytes
-
-If you want to create from `numpy` array, extra argument `dt_mcs` is required:
-
-[code-block-start]:init-from-np
-```python
-import numpy as np
-from first_breaks.sgy.reader import SGY
-
-num_samples = 1000
-num_traces = 48
-dt_mcs = 1e3
-
-traces = np.random.random((num_samples, num_traces))
-sgy = SGY(traces, dt_mcs=dt_mcs)
-```
-[code-block-end]:init-from-np
-
-### Content of SGY
-
-Created `SGY` allows you to read traces, get observation parameters and view headers (empty if created from `numpy`)
-
-[code-block-start]:sgy-content
-```python
-from first_breaks.sgy.reader import SGY
-
-sgy_filename = 'data.sgy'
-sgy = SGY(sgy_filename)
-
-# get all traces or specific traces limited by time
-all_traces = sgy.read()
-block_of_data = sgy.read_traces_by_ids(ids=[1, 2, 3, 10],
-                                       min_sample=100,
-                                       max_sample=500)
-
-# number of traces, values are the same
-print(sgy.num_traces, sgy.ntr)
-# number of time samples, values are the same
-print(sgy.num_samples, sgy.ns)
-# = (ns, ntr)
-print(sgy.shape)
-# time discretization, in mcs, in mcs, in ms
-print(sgy.dt, sgy.dt_mcs, sgy.dt_ms)
-
-# dict with headers in the first 3600 bytes of the file
-print(sgy.general_headers)
-# pandas DataFrame with headers for each trace
-print(sgy.traces_headers.head())
-```
-[code-block-end]:sgy-content
-
-### Create task for picking
-
-Next, we create a task for picking and pass the picking parameters to it. They have default values, but for the
-best quality, they must be matched to specific data. You can use the desktop application to evaluate the parameters.
-A detailed description of the parameters can be found  in the `Picking process` chapter.
-
-[code-block-start]:create-task
-```python
-from first_breaks.sgy.reader import SGY
-from first_breaks.picking.task import Task
-
-sgy_filename = 'data.sgy'
-sgy = SGY(sgy_filename)
-
-task = Task(sgy,
-            traces_per_gather=24,
-            maximum_time=200)
-```
-[code-block-end]:create-task
-
-
-### Create Picker
-In this step, we instantiate the neural network for picking. If you downloaded the model according to the
-installation section, then pass the path to it. Or leave the path to the model empty so that we can download it
-automatically.
-
-It's also possible to use GPU/CUDA to accelerate computation. By default `cuda` is selected if you have finished
-all steps regarding GPU in `Installation` section. Otherwise, it's `cpu`.
-
-You can also set the value of parameter `batch_size`, which can further speed up the calculations on the GPU.
-However, this will require additional video memory (VRAM).
-
-NOTE: When using the CPU, increasing `batch_size` does not speed up the calculation at all, but it may
-require additional memory costs (RAM). So don't increase this parameter when using CPU.
-
-[code-block-start]:create-picker
-```python
-from first_breaks.picking.picker_onnx import PickerONNX
-
-# the library will determine the best available device
-picker_default = PickerONNX()
-
-# create picker explicitly on CPU
-picker_cpu = PickerONNX(device='cpu')
-
-# create picker explicitly on GPU
-picker_gpu = PickerONNX(device='cuda', batch_size=2)
-
-# transfer model to another device
-picker_cpu.change_settings(device='cuda', batch_size=3)
-picker_gpu.change_settings(device='cpu', batch_size=1)
-```
-[code-block-end]:create-picker
-
-### Pick first breaks
-
-Now, using all the created components, we can pick the first breaks and export the results.
-
-[code-block-start]:pick-fb
-```python
-from first_breaks.picking.task import Task
-from first_breaks.picking.picker_onnx import PickerONNX
-from first_breaks.sgy.reader import SGY
-
-sgy_filename = 'data.sgy'
-sgy = SGY(sgy_filename)
-
-task = Task(sgy,
-            traces_per_gather=24,
-            maximum_time=200)
-picker = PickerONNX()
-task = picker.process_task(task)
-
-# you can see results of picking
-print(task.picks_in_samples)
-print(task.picks_in_ms)
-print(task.confidence)
-
-# you can export picks to file as plain text
-task.export_result_as_txt('result.txt')
-# or save as json file
-task.export_result_as_json('result.json')
-# or make a copy of source SGY and put picks to 236 byte
-task.export_result_as_sgy('result.segy',
-                          byte_position=236,
-                          encoding='i',
-                          picks_unit='mcs')
-```
-[code-block-end]:pick-fb
-
-### Visualizations
-
-You can save the seismogram and picks as an image. We use Qt backend for visualizations. Here we describe some usage
-scenarios.
-
-We've added named arguments to various scenarios for demonstration purposes, but in practice you can
-use them all. See the function arguments for more visualization options.
-
-Plot `SGY` only:
-
-[code-block-start]:plot-sgy
-```python
-from first_breaks.sgy.reader import SGY
-from first_breaks.desktop.graph import export_image
-
-sgy_filename = 'data.sgy'
-image_filename = 'image.png'
-
-sgy = SGY(sgy_filename)
-export_image(sgy, image_filename,
-             normalize=None,
-             traces_window=(5, 10),
-             time_window=(0, 200),
-             height=300,
-             width_per_trace=30)
-```
-[code-block-end]:plot-sgy
-
-Plot `numpy` traces:
-
-[code-block-start]:plot-np
-```python
-import numpy as np
-from first_breaks.sgy.reader import SGY
-from first_breaks.desktop.graph import export_image
-
-image_filename = 'image.png'
-num_traces = 48
-num_samples = 1000
-dt_mcs = 1e3
-
-traces = np.random.random((num_samples, num_traces))
-export_image(traces, image_filename,
-             dt_mcs=dt_mcs,
-             clip=0.5)
-
-# or create SGY as discussed before
-sgy = SGY(traces, dt_mcs=dt_mcs)
-export_image(sgy, image_filename,
-             gain=2)
-```
-[code-block-end]:plot-np
-
-Plot `SGY` with custom picks:
-
-[code-block-start]:plot-sgy-custom-picks
-```python
-import numpy as np
-from first_breaks.sgy.reader import SGY
-from first_breaks.desktop.graph import export_image
-
-sgy_filename = 'data.sgy'
-image_filename = 'image.png'
-
-sgy = SGY(sgy_filename)
-picks_ms = np.random.uniform(low=0,
-                             high=sgy.ns * sgy.dt_ms,
-                             size=sgy.ntr)
-export_image(sgy, image_filename,
-             picks_ms=picks_ms,
-             picks_color=(0, 100, 100))
-```
-[code-block-end]:plot-sgy-custom-picks
-
-Plot result of picking:
-
-[code-block-start]:plot-sgy-real-picks
-```python
-from first_breaks.picking.task import Task
-from first_breaks.picking.picker_onnx import PickerONNX
-from first_breaks.desktop.graph import export_image
-from first_breaks.sgy.reader import SGY
-
-sgy_filename = 'data.sgy'
-image_filename = 'image.png'
-
-sgy = SGY(sgy_filename)
-task = Task(sgy,
-            traces_per_gather=24,
-            maximum_time=200)
-picker = PickerONNX()
-task = picker.process_task(task)
-
-export_image(task, image_filename,
-             show_processing_region=False,
-             fill_black='right',
-             width=1000)
-```
-[code-block-end]:plot-sgy-real-picks
-
-### *Limit processing region
-
-Unfortunately, processing of a part of a file is not currently supported natively. We will add this functionality soon!
-
-However, you can use the following workaround to do this:
-
-[code-block-start]:pick-limited
-```python
-from first_breaks.sgy.reader import SGY
-
-sgy_filename = 'data.sgy'
-sgy = SGY(sgy_filename)
-
-interesting_traces = sgy.read_traces_by_ids(ids=list(range(20, 40)),
-                                            min_sample=100,
-                                            max_sample=200)
-
-# we create new SGY based on region of interests
-sgy = SGY(interesting_traces, dt_mcs=sgy.dt_mcs)
-```
-[code-block-end]:pick-limited
-
-</details>
-
-## Desktop application
-
-***Application under development***
-
-Desktop application allows you to work interactively with only one file and has better performance in visualization.
-You can use application as SGY viewer, as well as visually evaluate the optimal values of the picking
-parameters for your data.
-
-### Launch app
-
-Enter command to launch the application
-```shell
-first-breaks-picking app
-```
-or
-```shell
-first-breaks-picking desktop
-```
-
-### Select and view SGY file
-
-Click on 2 button to select SGY. After successful reading you can analyze SGY file.
-
-The following mouse interactions are available:
-- Left button drag / Middle button drag: Pan the scene.
-- Right button drag: Scales the scene. Dragging left/right scales horizontally; dragging up/down scales vertically.
-- Right button click: Open dialog with extra options, such as limit by X/Y axes and export.
-- Wheel spin: Zooms the scene in and out.
-- Left click: *After picking with model*, you can manually change picks.
-
-You can also use slider in toolbar to change gain of traces. **The gain value for the slider is only used for
-visualization, it is not used in picking process**.
-
-### Load model
-
-To use picker in desktop app you have to download model. See the `Installation` section for instructions
-on how to download the model.
-
-Click on 1 button and select file with model.
-After successfully loading the model, access to the pick will open.
-
-### Run picking
-
-Click on 3 button to open window with picking parameters. A detailed description of the parameters can be found
-in the `Picking process` chapter. Then run picking process. After some time, a line will appear connecting the first
-arrivals.
-
-Run again with different parameters to achieve optimal values of the picking parameters for your data.
-
-If you have CUDA compatible GPU and installed GPU supported version of library (see `Installation` section), you can
-select `CUDA/GPU` device  to use GPU acceleration. It can drastically decrease computation time.
-
-Parameter `Batch size` determine how many gathers will be processed simultaneously on GPU. It also can decrease
-computation time, but make sure that you have enough free GPU memory (`Batch size=10` requires > 10 Gb VRAM on Windows).
-
-### Processing grid
-
-Click on 4 button to toggle the display of the processing grid on or off. Horizontal line
-shows `Maximum time` and vertical lines are drawn at intervals equal to `Traces per gather`. The neural network
-processes blocks independently, as separate images.
-
-### Visual settings
-
-Click on 5 button to open window for visual settings. You can select gain, clip, normalization method,
-and trace values. In addition, you can also load a pick from a file, specifying how to read it.
-
-### Save results
-
-Click on 6 button to save picks into file. Depending on file extension, results will be saved as `json`,
-as plain `txt`, or as `segy` file.
-
-For extensions `txt` and `json`, picking parameters and model confidence for each peak are additionally saved.
-
-When choosing an extension `segy`, the copy of original SGY file is saved with the values of the first breaks in the
-trace headers. After selecting a file, you will be prompted to choose in which byte to save (counting starts from 1),
-in which units of measurement and how to encode.
-
-# Picking process
-
-Neural network process file as series of **images**. There is why **the traces should not be random**,
-since we are using information about adjacent traces.
-
-To obtain the first breaks we do the following steps:
-1) Read all traces in the file.
-![All traces](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/readme_images/full.png)
-2) Limit time range by `Maximum time`.
-![Limited by time](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/readme_images/tm_100.png)
-3) Split the sequence of traces into independent gathers of lengths `Traces per gather` each.
-![Splitted file](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/readme_images/tm_100_tr_24_24_24_24.png)
-4) Apply trace modification on the gathers level if necessary (`Gain`, `Clip`, etc).
-5) Calculate first breaks for individual gathers independently.
-![Picked gathers](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/readme_images/tm_100_tr_24_24_24_24_picks.png)
-6) Join the first breaks of individual gathers.
-![Picked file](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/readme_images/tm_100_picks.png)
-
-To achieve the best result, you need to modify the picking parameters.
-
-### Traces per gather
-
-`Traces per gather` is the most important parameter for picking. The parameter defines how we split the sequence of
-traces into individual gathers.
-
-Suppose we need to process a file with 96 traces. Depending on the value of `Traces per gather` parameter, we will
-process it as follows:
-- `Traces per gather` = 24. We will process 4 gathers with 24 traces each.
-![4 full shots](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/readme_images/tm_100_tr_24_24_24_24.png)
-- `Traces per gather` = 48. We will process 2 gathers with 48 traces each.
-![2 full shots](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/readme_images/tm_100_tr_48_48.png)
-- `Traces per gather` = 40. We will process 2 gathers with 40 traces each and 1 gather with the remaining 16 traces.
-The last gather will be interpolated from 16 to 40 traces.
-![2 full + 1 interpolated shots](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/readme_images/tm_100_tr_40_40_16.png)
-
-### Maximum time
-
-You can localize the area for finding first breaks. Specify `Maximum time` if you have long records but the first breaks
-located at the start of the traces. Keep it `0` if you don't want to limit traces.
-
-### List of traces to inverse
-
-Some receivers may have the wrong polarity, so you can specify which traces should be inversed. Note, that inversion
-will be applied on the gathers level. For example, if you have 96 traces, `Traces per gather` = 48 and
-`List of traces to inverse` = (2, 30, 48), then traces (2, 3, 48, 50, 78, 96) will be inversed.
-
-Notes:
-- Trace indexing starts at 1.
-- Option is not available on desktop app.
-
-
-## Recommendations
-You can receive predictions for any file with any parameters, but to get a better result, you should comply with the
-following guidelines:
-- Your file should contain one or more gathers. By a gather, we mean that traces within a single gather can be
-geophysically interpreted. **The traces within the same gather should not be random**, since we are using information
-about adjacent traces.
-- All gathers in the file must contain the same number of traces.
-- The number of traces in gather must be equal to `Traces per gather` or divisible by it without a remainder.
-For example, if you have CSP gathers and the number of receivers is 48, then you can set the parameter
-value to 48, 24, or 12.
-- We don't sort your file (CMP, CRP, CSP, etc), so you should send us files with traces sorted by yourself.
-- You can process a file with independent seismograms obtained from different polygons, under different conditions, etc.,
-but the requirements listed above must be met.
-
-# Acknowledgments
-
-<a href="https://geodevice.co/"><img src="https://geodevice.co/local/templates/geodevice_15_07_2019/assets/images/logo_geodevice.png?1" style="width: 200px;" alt="Geodevice"></a>
-
-We would like to thank [GEODEVICE](https://geodevice.co/) for providing field data from land and borehole seismic surveys with annotated first breaks for model training.
-
+# First breaks picking
+This project is devoted to pick waves that are the first to be detected on a seismogram (first breaks, first arrivals).
+Traditionally, this procedure is performed manually. When processing field data, the number of picks reaches hundreds of
+thousands. Existing analytical methods allow you to automate picking only on high-quality data with a high
+signal / noise ratio.
+
+As a more robust algorithm, it is proposed to use a neural network to pick the first breaks. Since the data on adjacent
+seismic traces have similarities in the features of the wave field, **we pick first breaks on 2D seismic gather**, not
+individual traces.
+
+<p align="center">
+<img src="https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/readme_images/project_preview.png" />
+</p>
+
+# Examples
+
+In the drop-down menus below you will find examples of our model picking on good quality data as well as noisy ones.
+
+It is difficult to validate the quality of the model on noisy data, but they show the robustness of the model to
+various types of noise.
+
+<details>
+<summary>Good quality data</summary>
+
+![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/normal/normal_0.png)
+
+![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/normal/normal_1.png)
+
+![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/normal/normal_2.png)
+
+![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/normal/normal_3.png)
+
+![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/normal/normal_4.png)
+
+![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/normal/normal_5.png)
+
+![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/normal/normal_6.png)
+
+![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/normal/normal_7.png)
+
+![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/normal/normal_8.png)
+
+![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/normal/normal_9.png)
+
+![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/normal/normal_10.png)
+
+![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/normal/normal_11.png)
+
+![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/normal/normal_12.png)
+
+![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/normal/normal_13.png)
+
+![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/normal/normal_14.png)
+
+</details>
+
+<details>
+<summary>Noisy data</summary>
+
+![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/noisy/noisy_0.png)
+
+![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/noisy/noisy_1.png)
+
+![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/noisy/noisy_2.png)
+
+![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/noisy/noisy_3.png)
+
+![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/noisy/noisy_4.png)
+
+![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/noisy/noisy_5.png)
+
+![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/noisy/noisy_6.png)
+
+</details>
+
+# Installation
+
+Library is available in [PyPI](https://pypi.org/project/first-breaks-picking/):
+```shell
+pip install -U first-breaks-picking
+```
+
+### GPU support
+
+You can use the capabilities of GPU to significantly reduce picking time. Before started, check
+[here](https://developer.nvidia.com/cuda-gpus) that your GPU is CUDA compatible.
+
+Install GPU supported version of library:
+```shell
+pip install -U first-breaks-picking[gpu]
+```
+
+The following steps are operating system dependent and must be performed manually:
+
+- Install [latest NVIDIA drivers](https://www.nvidia.com/Download/index.aspx).
+- Install [CUDA toolkit](https://developer.nvidia.com/cuda-downloads).
+**The version must be between 11.x, starting with 11.6.
+Version 12 also may work, but versions >=11.6 are recommended**.
+- Install ZLib and CuDNN:
+[Windows](https://docs.nvidia.com/deeplearning/cudnn/install-guide/index.html#install-windows) and
+[Linux](https://docs.nvidia.com/deeplearning/cudnn/install-guide/index.html#install-linux).
+
+### Extra data
+
+- To pick first breaks you need
+to [download model](https://oml.daloroserver.com/download/seis/fb.onnx).
+
+- If you have no seismic data, you can also
+[download small SGY file](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/data/real_gather.sgy).
+
+It's also possible to download them with Python using the following snippet:
+
+[code-block-start]:downloading-extra
+```python
+from first_breaks.utils.utils import (download_demo_sgy,
+                                      download_model_onnx)
+
+sgy_filename = 'data.sgy'
+model_filename = 'model.onnx'
+
+download_demo_sgy(sgy_filename)
+download_model_onnx(model_filename)
+```
+[code-block-end]:downloading-extra
+
+# How to use it
+
+The library can be used in Python, or you can use the desktop application.
+
+## Python
+
+Programmatic way has more flexibility for building your own picking scenario and processing multiple files.
+
+### Minimal example
+
+The following snippet implements the picking process of the demo file. As a result, you can get an image from
+the project preview.
+
+[code-block-start]:e2e-example
+```python
+from first_breaks.utils.utils import download_demo_sgy
+from first_breaks.sgy.reader import SGY
+from first_breaks.picking.task import Task
+from first_breaks.picking.picker_onnx import PickerONNX
+from first_breaks.desktop.graph import export_image
+
+sgy_filename = 'data.sgy'
+download_demo_sgy(fname=sgy_filename)
+sgy = SGY(sgy_filename)
+
+task = Task(sgy_filename,
+            traces_per_gather=12,
+            maximum_time=100,
+            gain=2)
+picker = PickerONNX()
+task = picker.process_task(task)
+
+# create an image with default parameters
+image_filename = 'default_view.png'
+export_image(task, image_filename)
+
+# create an image from the project preview
+image_filename = 'project_preview.png'
+export_image(task, image_filename,
+             time_window=(0, 60),
+             traces_window=(79.5, 90.5),
+             show_processing_region=False,
+             headers_total_pixels=80,
+             height=500,
+             width=700,
+             hide_traces_axis=True)
+```
+[code-block-end]:e2e-example
+
+For a better understanding of the steps taken, expand and read the next section.
+
+### Detailed examples
+
+<details>
+
+<summary>Show examples</summary>
+
+### Download demo SGY
+
+Let's download the demo file. All the following examples assume that the file is downloaded and saved as `data.sgy`.
+You can also put your own SGY file.
+
+```python
+from first_breaks.utils.utils import download_demo_sgy
+
+sgy_filename = 'data.sgy'
+download_demo_sgy(fname=sgy_filename)
+```
+
+### Create SGY
+We provide several ways to create `SGY` object: from file, `bytes` or `numpy` array.
+
+From file:
+
+[code-block-start]:init-from-path
+```python
+from first_breaks.sgy.reader import SGY
+
+sgy_filename = 'data.sgy'
+sgy = SGY(sgy_filename)
+```
+[code-block-end]:init-from-path
+
+From `bytes`:
+
+[code-block-start]:init-from-bytes
+```python
+from first_breaks.sgy.reader import SGY
+
+sgy_filename = 'data.sgy'
+
+with open(sgy_filename, 'rb') as fin:
+    sgy_bytes = fin.read()
+
+sgy = SGY(sgy_bytes)
+```
+[code-block-end]:init-from-bytes
+
+If you want to create from `numpy` array, extra argument `dt_mcs` is required:
+
+[code-block-start]:init-from-np
+```python
+import numpy as np
+from first_breaks.sgy.reader import SGY
+
+num_samples = 1000
+num_traces = 48
+dt_mcs = 1e3
+
+traces = np.random.random((num_samples, num_traces))
+sgy = SGY(traces, dt_mcs=dt_mcs)
+```
+[code-block-end]:init-from-np
+
+### Content of SGY
+
+Created `SGY` allows you to read traces, get observation parameters and view headers (empty if created from `numpy`)
+
+[code-block-start]:sgy-content
+```python
+from first_breaks.sgy.reader import SGY
+
+sgy_filename = 'data.sgy'
+sgy = SGY(sgy_filename)
+
+# get all traces or specific traces limited by time
+all_traces = sgy.read()
+block_of_data = sgy.read_traces_by_ids(ids=[1, 2, 3, 10],
+                                       min_sample=100,
+                                       max_sample=500)
+
+# number of traces, values are the same
+print(sgy.num_traces, sgy.ntr)
+# number of time samples, values are the same
+print(sgy.num_samples, sgy.ns)
+# = (ns, ntr)
+print(sgy.shape)
+# time discretization, in mcs, in mcs, in ms
+print(sgy.dt, sgy.dt_mcs, sgy.dt_ms)
+
+# dict with headers in the first 3600 bytes of the file
+print(sgy.general_headers)
+# pandas DataFrame with headers for each trace
+print(sgy.traces_headers.head())
+```
+[code-block-end]:sgy-content
+
+### Create task for picking
+
+Next, we create a task for picking and pass the picking parameters to it. They have default values, but for the
+best quality, they must be matched to specific data. You can use the desktop application to evaluate the parameters.
+A detailed description of the parameters can be found  in the `Picking process` chapter.
+
+[code-block-start]:create-task
+```python
+from first_breaks.sgy.reader import SGY
+from first_breaks.picking.task import Task
+
+sgy_filename = 'data.sgy'
+sgy = SGY(sgy_filename)
+
+task = Task(sgy,
+            traces_per_gather=24,
+            maximum_time=200)
+```
+[code-block-end]:create-task
+
+
+### Create Picker
+In this step, we instantiate the neural network for picking. If you downloaded the model according to the
+installation section, then pass the path to it. Or leave the path to the model empty so that we can download it
+automatically.
+
+It's also possible to use GPU/CUDA to accelerate computation. By default `cuda` is selected if you have finished
+all steps regarding GPU in `Installation` section. Otherwise, it's `cpu`.
+
+You can also set the value of parameter `batch_size`, which can further speed up the calculations on the GPU.
+However, this will require additional video memory (VRAM).
+
+NOTE: When using the CPU, increasing `batch_size` does not speed up the calculation at all, but it may
+require additional memory costs (RAM). So don't increase this parameter when using CPU.
+
+[code-block-start]:create-picker
+```python
+from first_breaks.picking.picker_onnx import PickerONNX
+
+# the library will determine the best available device
+picker_default = PickerONNX()
+
+# create picker explicitly on CPU
+picker_cpu = PickerONNX(device='cpu')
+
+# create picker explicitly on GPU
+picker_gpu = PickerONNX(device='cuda', batch_size=2)
+
+# transfer model to another device
+picker_cpu.change_settings(device='cuda', batch_size=3)
+picker_gpu.change_settings(device='cpu', batch_size=1)
+```
+[code-block-end]:create-picker
+
+### Pick first breaks
+
+Now, using all the created components, we can pick the first breaks and export the results.
+
+[code-block-start]:pick-fb
+```python
+from first_breaks.picking.task import Task
+from first_breaks.picking.picker_onnx import PickerONNX
+from first_breaks.sgy.reader import SGY
+
+sgy_filename = 'data.sgy'
+sgy = SGY(sgy_filename)
+
+task = Task(sgy,
+            traces_per_gather=24,
+            maximum_time=200)
+picker = PickerONNX()
+task = picker.process_task(task)
+
+# you can see results of picking
+print(task.picks_in_samples)
+print(task.picks_in_ms)
+print(task.confidence)
+
+# you can export picks to file as plain text
+task.export_result_as_txt('result.txt')
+# or save as json file
+task.export_result_as_json('result.json')
+# or make a copy of source SGY and put picks to 236 byte
+task.export_result_as_sgy('result.segy',
+                          byte_position=236,
+                          encoding='i',
+                          picks_unit='mcs')
+```
+[code-block-end]:pick-fb
+
+### Visualizations
+
+You can save the seismogram and picks as an image. We use Qt backend for visualizations. Here we describe some usage
+scenarios.
+
+We've added named arguments to various scenarios for demonstration purposes, but in practice you can
+use them all. See the function arguments for more visualization options.
+
+Plot `SGY` only:
+
+[code-block-start]:plot-sgy
+```python
+from first_breaks.sgy.reader import SGY
+from first_breaks.desktop.graph import export_image
+
+sgy_filename = 'data.sgy'
+image_filename = 'image.png'
+
+sgy = SGY(sgy_filename)
+export_image(sgy, image_filename,
+             normalize=None,
+             traces_window=(5, 10),
+             time_window=(0, 200),
+             height=300,
+             width_per_trace=30)
+```
+[code-block-end]:plot-sgy
+
+Plot `numpy` traces:
+
+[code-block-start]:plot-np
+```python
+import numpy as np
+from first_breaks.sgy.reader import SGY
+from first_breaks.desktop.graph import export_image
+
+image_filename = 'image.png'
+num_traces = 48
+num_samples = 1000
+dt_mcs = 1e3
+
+traces = np.random.random((num_samples, num_traces))
+export_image(traces, image_filename,
+             dt_mcs=dt_mcs,
+             clip=0.5)
+
+# or create SGY as discussed before
+sgy = SGY(traces, dt_mcs=dt_mcs)
+export_image(sgy, image_filename,
+             gain=2)
+```
+[code-block-end]:plot-np
+
+Plot `SGY` with custom picks:
+
+[code-block-start]:plot-sgy-custom-picks
+```python
+import numpy as np
+from first_breaks.sgy.reader import SGY
+from first_breaks.desktop.graph import export_image
+
+sgy_filename = 'data.sgy'
+image_filename = 'image.png'
+
+sgy = SGY(sgy_filename)
+picks_ms = np.random.uniform(low=0,
+                             high=sgy.ns * sgy.dt_ms,
+                             size=sgy.ntr)
+export_image(sgy, image_filename,
+             picks_ms=picks_ms,
+             picks_color=(0, 100, 100))
+```
+[code-block-end]:plot-sgy-custom-picks
+
+Plot result of picking:
+
+[code-block-start]:plot-sgy-real-picks
+```python
+from first_breaks.picking.task import Task
+from first_breaks.picking.picker_onnx import PickerONNX
+from first_breaks.desktop.graph import export_image
+from first_breaks.sgy.reader import SGY
+
+sgy_filename = 'data.sgy'
+image_filename = 'image.png'
+
+sgy = SGY(sgy_filename)
+task = Task(sgy,
+            traces_per_gather=24,
+            maximum_time=200)
+picker = PickerONNX()
+task = picker.process_task(task)
+
+export_image(task, image_filename,
+             show_processing_region=False,
+             fill_black='right',
+             width=1000)
+```
+[code-block-end]:plot-sgy-real-picks
+
+### *Limit processing region
+
+Unfortunately, processing of a part of a file is not currently supported natively. We will add this functionality soon!
+
+However, you can use the following workaround to do this:
+
+[code-block-start]:pick-limited
+```python
+from first_breaks.sgy.reader import SGY
+
+sgy_filename = 'data.sgy'
+sgy = SGY(sgy_filename)
+
+interesting_traces = sgy.read_traces_by_ids(ids=list(range(20, 40)),
+                                            min_sample=100,
+                                            max_sample=200)
+
+# we create new SGY based on region of interests
+sgy = SGY(interesting_traces, dt_mcs=sgy.dt_mcs)
+```
+[code-block-end]:pick-limited
+
+</details>
+
+## Desktop application
+
+***Application under development***
+
+Desktop application allows you to work interactively with only one file and has better performance in visualization.
+You can use application as SGY viewer, as well as visually evaluate the optimal values of the picking
+parameters for your data.
+
+### Launch app
+
+Enter command to launch the application
+```shell
+first-breaks-picking app
+```
+or
+```shell
+first-breaks-picking desktop
+```
+
+### Select and view SGY file
+
+Click on 2 button to select SGY. After successful reading you can analyze SGY file.
+
+The following mouse interactions are available:
+- Left button drag / Middle button drag: Pan the scene.
+- Right button drag: Scales the scene. Dragging left/right scales horizontally; dragging up/down scales vertically.
+- Right button click: Open dialog with extra options, such as limit by X/Y axes and export.
+- Wheel spin: Zooms the scene in and out.
+- Left click: *After picking with model*, you can manually change picks.
+
+You can also use slider in toolbar to change gain of traces. **The gain value for the slider is only used for
+visualization, it is not used in picking process**.
+
+### Load model
+
+To use picker in desktop app you have to download model. See the `Installation` section for instructions
+on how to download the model.
+
+Click on 1 button and select file with model.
+After successfully loading the model, access to the pick will open.
+
+### Run picking
+
+Click on 3 button to open window with picking parameters. A detailed description of the parameters can be found
+in the `Picking process` chapter. Then run picking process. After some time, a line will appear connecting the first
+arrivals.
+
+Run again with different parameters to achieve optimal values of the picking parameters for your data.
+
+If you have CUDA compatible GPU and installed GPU supported version of library (see `Installation` section), you can
+select `CUDA/GPU` device  to use GPU acceleration. It can drastically decrease computation time.
+
+Parameter `Batch size` determine how many gathers will be processed simultaneously on GPU. It also can decrease
+computation time, but make sure that you have enough free GPU memory (`Batch size=10` requires > 10 Gb VRAM on Windows).
+
+### Processing grid
+
+Click on 4 button to toggle the display of the processing grid on or off. Horizontal line
+shows `Maximum time` and vertical lines are drawn at intervals equal to `Traces per gather`. The neural network
+processes blocks independently, as separate images.
+
+### Visual settings
+
+Click on 5 button to open window for visual settings. You can select gain, clip, normalization method,
+and trace values. In addition, you can also load a pick from a file, specifying how to read it.
+
+### Save results
+
+Click on 6 button to save picks into file. Depending on file extension, results will be saved as `json`,
+as plain `txt`, or as `segy` file.
+
+For extensions `txt` and `json`, picking parameters and model confidence for each peak are additionally saved.
+
+When choosing an extension `segy`, the copy of original SGY file is saved with the values of the first breaks in the
+trace headers. After selecting a file, you will be prompted to choose in which byte to save (counting starts from 1),
+in which units of measurement and how to encode.
+
+# Picking process
+
+Neural network process file as series of **images**. There is why **the traces should not be random**,
+since we are using information about adjacent traces.
+
+To obtain the first breaks we do the following steps:
+1) Read all traces in the file.
+![All traces](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/readme_images/full.png)
+2) Limit time range by `Maximum time`.
+![Limited by time](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/readme_images/tm_100.png)
+3) Split the sequence of traces into independent gathers of lengths `Traces per gather` each.
+![Splitted file](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/readme_images/tm_100_tr_24_24_24_24.png)
+4) Apply trace modification on the gathers level if necessary (`Gain`, `Clip`, etc).
+5) Calculate first breaks for individual gathers independently.
+![Picked gathers](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/readme_images/tm_100_tr_24_24_24_24_picks.png)
+6) Join the first breaks of individual gathers.
+![Picked file](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/readme_images/tm_100_picks.png)
+
+To achieve the best result, you need to modify the picking parameters.
+
+### Traces per gather
+
+`Traces per gather` is the most important parameter for picking. The parameter defines how we split the sequence of
+traces into individual gathers.
+
+Suppose we need to process a file with 96 traces. Depending on the value of `Traces per gather` parameter, we will
+process it as follows:
+- `Traces per gather` = 24. We will process 4 gathers with 24 traces each.
+![4 full shots](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/readme_images/tm_100_tr_24_24_24_24.png)
+- `Traces per gather` = 48. We will process 2 gathers with 48 traces each.
+![2 full shots](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/readme_images/tm_100_tr_48_48.png)
+- `Traces per gather` = 40. We will process 2 gathers with 40 traces each and 1 gather with the remaining 16 traces.
+The last gather will be interpolated from 16 to 40 traces.
+![2 full + 1 interpolated shots](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/readme_images/tm_100_tr_40_40_16.png)
+
+### Maximum time
+
+You can localize the area for finding first breaks. Specify `Maximum time` if you have long records but the first breaks
+located at the start of the traces. Keep it `0` if you don't want to limit traces.
+
+### List of traces to inverse
+
+Some receivers may have the wrong polarity, so you can specify which traces should be inversed. Note, that inversion
+will be applied on the gathers level. For example, if you have 96 traces, `Traces per gather` = 48 and
+`List of traces to inverse` = (2, 30, 48), then traces (2, 3, 48, 50, 78, 96) will be inversed.
+
+Notes:
+- Trace indexing starts at 1.
+- Option is not available on desktop app.
+
+
+## Recommendations
+You can receive predictions for any file with any parameters, but to get a better result, you should comply with the
+following guidelines:
+- Your file should contain one or more gathers. By a gather, we mean that traces within a single gather can be
+geophysically interpreted. **The traces within the same gather should not be random**, since we are using information
+about adjacent traces.
+- All gathers in the file must contain the same number of traces.
+- The number of traces in gather must be equal to `Traces per gather` or divisible by it without a remainder.
+For example, if you have CSP gathers and the number of receivers is 48, then you can set the parameter
+value to 48, 24, or 12.
+- We don't sort your file (CMP, CRP, CSP, etc), so you should send us files with traces sorted by yourself.
+- You can process a file with independent seismograms obtained from different polygons, under different conditions, etc.,
+but the requirements listed above must be met.
+
+# Acknowledgments
+
+<a href="https://geodevice.co/"><img src="https://geodevice.co/local/templates/geodevice_15_07_2019/assets/images/logo_geodevice.png?1" style="width: 200px;" alt="Geodevice"></a>
+
+We would like to thank [GEODEVICE](https://geodevice.co/) for providing field data from land and borehole seismic surveys with annotated first breaks for model training.
+
```

### Comparing `first-breaks-picking-0.3.0b0/first_breaks/const.py` & `first-breaks-picking-0.4.0a0/first_breaks/const.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,34 @@
-import os
-from os import environ
-from pathlib import Path
-from sys import platform
-
-
-def is_windows() -> bool:
-    return "win" in platform
-
-
-def is_linux() -> bool:
-    return "linux" in platform
-
-
-def is_macos() -> bool:
-    return "darwin" in platform
-
-
-def get_cache_folder() -> Path:
-    if is_linux():
-        return Path(environ.get("XDG_CACHE_HOME", Path.home() / ".cache")) / "first_breaks_picking"
-    elif is_macos():
-        return Path.home() / "Library" / "Caches" / "first_breaks_picking"
-    elif is_windows():
-        return Path.home() / ".cache" / "first_breaks_picking"
-    else:
-        raise ValueError(f"Unexpected platform {platform}.")
-
-
-PROJECT_ROOT = Path(__file__).parent.parent
-CACHE_FOLDER = get_cache_folder()
-
-DEMO_SGY_PATH = CACHE_FOLDER / "real_gather.sgy"
-DEMO_SGY_URL = "https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/data/real_gather.sgy"
-DEMO_SGY_HASH = "92fe2992b57d69c6f572c672f63960cf"
-
-
-MODEL_ONNX_PATH = CACHE_FOLDER / "fb.onnx"
-MODEL_ONNX_URL = "https://oml.daloroserver.com/download/seis/fb.onnx"
-MODEL_ONNX_HASH = "7e39e017b01325180e36885eccaeb17a"
-
-TIMEOUT = 60
-
-HIGH_DPI = os.getenv("HIGH_DPI", True)
+import os
+from os import environ
+from pathlib import Path
+from sys import platform
+
+from first_breaks import is_linux, is_macos, is_windows
+
+
+def get_cache_folder() -> Path:
+    if is_linux():
+        return Path(environ.get("XDG_CACHE_HOME", Path.home() / ".cache")) / "first_breaks_picking"
+    elif is_macos():
+        return Path.home() / "Library" / "Caches" / "first_breaks_picking"
+    elif is_windows():
+        return Path.home() / ".cache" / "first_breaks_picking"
+    else:
+        raise ValueError(f"Unexpected platform {platform}.")
+
+
+PROJECT_ROOT = Path(__file__).parent.parent
+CACHE_FOLDER = get_cache_folder()
+
+DEMO_SGY_PATH = CACHE_FOLDER / "real_gather.sgy"
+DEMO_SGY_URL = "https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/data/real_gather.sgy"
+DEMO_SGY_HASH = "92fe2992b57d69c6f572c672f63960cf"
+
+
+MODEL_ONNX_PATH = CACHE_FOLDER / "fb.onnx"
+MODEL_ONNX_URL = "https://oml.daloroserver.com/download/seis/fb.onnx"
+MODEL_ONNX_HASH = "7e39e017b01325180e36885eccaeb17a"
+
+TIMEOUT = 60
+
+HIGH_DPI = os.getenv("HIGH_DPI", True)
```

### Comparing `first-breaks-picking-0.3.0b0/first_breaks/data_models/dependent.py` & `first-breaks-picking-0.4.0a0/first_breaks/data_models/dependent.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-from typing import Any, Optional
-
-from pydantic import Field, ValidationError, field_validator
-from pydantic_core.core_schema import FieldValidationInfo
-
-from first_breaks.data_models.independent import DefaultModel, TraceBytePosition
-from first_breaks.sgy.headers import Headers, TraceHeaders
-
-TRACE_HEADER_NAMES = [v[1] for v in TraceHeaders().headers_schema]
-
-
-class XAxis(DefaultModel):
-    x_axis: Optional[str] = Field(None, description="Source of labels for X axis")
-
-    @field_validator("x_axis")
-    def validate_x_axis(cls, v: Any) -> Any:
-        if v is None:
-            return v
-        else:
-            if v not in TRACE_HEADER_NAMES:
-                raise ValidationError(f"'x_axis' must be None or one of trace header name, got {v}")
-            else:
-                return v
-
-
-class Encoding(DefaultModel):
-    encoding: str = Field("i", description="How to encode value")
-
-    @field_validator("encoding")
-    def validate_encoding(cls, v: str) -> str:
-        if v not in Headers().format2size.keys():
-            raise ValidationError(f"'encoding' must be one of {Headers().format2size.keys()}")
-        else:
-            return v
-
-
-class TraceHeaderParams(TraceBytePosition, Encoding):
-    @field_validator("byte_position")
-    def validate_position_depends_on_encoding(cls, v: int, based_validation_info: FieldValidationInfo) -> int:
-        encoding = based_validation_info.data["encoding"]
-        size = Headers.format2size[encoding]
-        if v + size > 240:
-            raise ValidationError(
-                f"'byte_position' is greater than allowed for '{encoding}' encoding. "
-                f"Maximum allowed: {240 - size}, got {v}"
-            )
-        return v
+from typing import Any, Optional
+
+from pydantic import Field, ValidationError, field_validator
+from pydantic_core.core_schema import FieldValidationInfo
+
+from first_breaks.data_models.independent import DefaultModel, TraceBytePosition
+from first_breaks.sgy.headers import Headers, TraceHeaders
+
+TRACE_HEADER_NAMES = [v[1] for v in TraceHeaders().headers_schema]
+
+
+class XAxis(DefaultModel):
+    x_axis: Optional[str] = Field(None, description="Source of labels for X axis")
+
+    @field_validator("x_axis")
+    def validate_x_axis(cls, v: Any) -> Any:
+        if v is None:
+            return v
+        else:
+            if v not in TRACE_HEADER_NAMES:
+                raise ValidationError(f"'x_axis' must be None or one of trace header name, got {v}")
+            else:
+                return v
+
+
+class Encoding(DefaultModel):
+    encoding: str = Field("i", description="How to encode value")
+
+    @field_validator("encoding")
+    def validate_encoding(cls, v: str) -> str:
+        if v not in Headers().format2size.keys():
+            raise ValidationError(f"'encoding' must be one of {Headers().format2size.keys()}")
+        else:
+            return v
+
+
+class TraceHeaderParams(TraceBytePosition, Encoding):
+    @field_validator("byte_position")
+    def validate_position_depends_on_encoding(cls, v: int, based_validation_info: FieldValidationInfo) -> int:
+        encoding = based_validation_info.data["encoding"]
+        size = Headers.format2size[encoding]
+        if v + size > 240:
+            raise ValidationError(
+                f"'byte_position' is greater than allowed for '{encoding}' encoding. "
+                f"Maximum allowed: {240 - size}, got {v}"
+            )
+        return v
```

### Comparing `first-breaks-picking-0.3.0b0/first_breaks/data_models/independent.py` & `first-breaks-picking-0.4.0a0/first_breaks/data_models/independent.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-from typing import List, Literal, Optional, Tuple, Union
-
-import numpy as np
-from pydantic import BaseModel, Field
-
-TColor = Union[Tuple[int, int, int, int], Tuple[int, int, int]]
-TNormalize = Union[Literal["trace", "gather"], float, int, np.ndarray, None]
-
-
-class DefaultModel(BaseModel):
-    class Config:
-        arbitrary_types_allowed = True
-
-
-class Normalize(DefaultModel):
-    normalize: TNormalize = Field(
-        "trace",
-        description="How to normalize gather",
-    )
-
-
-class Gain(DefaultModel):
-    gain: float = Field(1.0, description="Gain value")
-
-
-class Clip(DefaultModel):
-    clip: float = Field(
-        0.9,
-        gt=0.0,
-        description="Clip amplitudes to this value if their absolute value is greater than this number",
-    )
-
-
-class FillBlack(DefaultModel):
-    fill_black: Optional[Literal["left", "right"]] = Field(
-        "left",
-        description="Where and how to fill wiggles with black",
-    )
-
-
-class PicksColor(DefaultModel):
-    picks_color: TColor = Field((255, 0, 0), description="Color for picks")
-
-
-class RegionPolyColor(DefaultModel):
-    region_poly_color: TColor = Field((100, 100, 100, 50), description="Color of region below maximum time")
-
-
-class RegionContourColor(DefaultModel):
-    region_contour_color: TColor = Field(
-        (100, 100, 100),
-        description="Color of dashed line which shows maximum time and how file is split into gathers",
-    )
-
-
-class RegionContourWidth(DefaultModel):
-    region_contour_width: float = Field(
-        0.2,
-        description="Width of dashed line which shows maximum time and how file is split into gathers",
-    )
-
-
-class TraceBytePosition(DefaultModel):
-    byte_position: int = Field(0, ge=0, lt=240, description="Byte index in trace headers")
-
-
-class PicksUnit(DefaultModel):
-    picks_unit: Literal["ms", "mcs", "sample"] = Field("mcs", description="First breaks / picks unit")
-
-
-class PicksValue(DefaultModel):
-    picks_value: Union[np.ndarray, List[Union[int, float]], Tuple[Union[int, float], ...]] = Field(
-        ...,
-        description="Values of first breaks",
-    )
+from typing import List, Literal, Optional, Tuple, Union
+
+import numpy as np
+from pydantic import BaseModel, Field
+
+TColor = Union[Tuple[int, int, int, int], Tuple[int, int, int]]
+TNormalize = Union[Literal["trace", "gather"], float, int, np.ndarray, None]
+
+
+class DefaultModel(BaseModel):
+    class Config:
+        arbitrary_types_allowed = True
+
+
+class Normalize(DefaultModel):
+    normalize: TNormalize = Field(
+        "trace",
+        description="How to normalize gather",
+    )
+
+
+class Gain(DefaultModel):
+    gain: float = Field(1.0, description="Gain value")
+
+
+class Clip(DefaultModel):
+    clip: float = Field(
+        0.9,
+        gt=0.0,
+        description="Clip amplitudes to this value if their absolute value is greater than this number",
+    )
+
+
+class FillBlack(DefaultModel):
+    fill_black: Optional[Literal["left", "right"]] = Field(
+        "left",
+        description="Where and how to fill wiggles with black",
+    )
+
+
+class PicksColor(DefaultModel):
+    picks_color: TColor = Field((255, 0, 0), description="Color for picks")
+
+
+class RegionPolyColor(DefaultModel):
+    region_poly_color: TColor = Field((100, 100, 100, 50), description="Color of region below maximum time")
+
+
+class RegionContourColor(DefaultModel):
+    region_contour_color: TColor = Field(
+        (100, 100, 100),
+        description="Color of dashed line which shows maximum time and how file is split into gathers",
+    )
+
+
+class RegionContourWidth(DefaultModel):
+    region_contour_width: float = Field(
+        0.2,
+        description="Width of dashed line which shows maximum time and how file is split into gathers",
+    )
+
+
+class TraceBytePosition(DefaultModel):
+    byte_position: int = Field(0, ge=0, lt=240, description="Byte index in trace headers")
+
+
+class PicksUnit(DefaultModel):
+    picks_unit: Literal["ms", "mcs", "sample"] = Field("mcs", description="First breaks / picks unit")
+
+
+class PicksValue(DefaultModel):
+    picks_value: Union[np.ndarray, List[Union[int, float]], Tuple[Union[int, float], ...]] = Field(
+        ...,
+        description="Values of first breaks",
+    )
```

### Comparing `first-breaks-picking-0.3.0b0/first_breaks/desktop/byte_encode_unit_widget.py` & `first-breaks-picking-0.4.0a0/first_breaks/desktop/byte_encode_unit_widget.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,159 +1,159 @@
-import warnings
-from typing import Any, Dict, Optional, Tuple
-
-from PyQt5.QtCore import Qt, pyqtSignal
-from PyQt5.QtWidgets import (
-    QApplication,
-    QDialog,
-    QDialogButtonBox,
-    QHBoxLayout,
-    QLabel,
-    QSpinBox,
-    QVBoxLayout,
-    QWidget,
-)
-
-from first_breaks.const import HIGH_DPI
-from first_breaks.desktop.combobox_with_mapping import QComboBoxMapping
-from first_breaks.sgy.headers import Headers
-
-if HIGH_DPI:
-    QApplication.setAttribute(Qt.AA_EnableHighDpiScaling, True)
-    QApplication.setAttribute(Qt.AA_UseHighDpiPixmaps, True)
-
-warnings.filterwarnings("ignore")
-
-
-def build_encoding_mapping() -> Dict[int, Tuple[str, str]]:
-    mapping = {
-        0: ("Integer 4", "i"),
-        1: ("UInteger 4", "I"),
-        2: ("Short 2", "h"),
-        3: ("UShort 2", "H"),
-        4: ("Long 4", "l"),
-        5: ("ULong 4", "L"),
-        6: ("Float 4", "f"),
-        7: ("Double 8", "d"),
-    }
-    assert all(v[1] in Headers.format2size.keys() for v in mapping.values())
-    return mapping
-
-
-ENCODING_MAPPING = build_encoding_mapping()
-
-
-class QByteEncodeUnitWidget(QWidget):
-    values_changed_signal = pyqtSignal(dict)
-
-    def __init__(
-        self,
-        byte_position: int = 0,
-        encoding: str = "I",
-        first_byte: int = 0,
-        picks_unit: str = "mcs",
-        margins: Optional[int] = None,
-        *args: Any,
-        **kwargs: Any
-    ) -> None:
-        super().__init__(*args, **kwargs)
-
-        self.layout = QHBoxLayout()
-        if margins is not None:
-            self.layout.setContentsMargins(margins, margins, margins, margins)
-        self.setLayout(self.layout)
-
-        assert byte_position >= first_byte
-        self.byte_position_value = byte_position
-        self.encoding_value = encoding
-        self.first_byte = first_byte
-        self.byte_position_maximum = 240 + self.first_byte
-        self.picks_unit_value = picks_unit
-
-        self.byte_position_label = QLabel("Byte")
-        self.byte_position_widget = QSpinBox()
-        self.byte_position_widget.setRange(self.first_byte, self.byte_position_maximum)
-        self.byte_position_widget.setValue(self.byte_position_value)
-        self.byte_position_widget.valueChanged.connect(self.values_changed)
-
-        self.layout.addWidget(self.byte_position_label)
-        self.layout.addWidget(self.byte_position_widget)
-
-        self.encoding_label = QLabel("Encoding")
-        self.encoding_widget = QComboBoxMapping(ENCODING_MAPPING, current_value=self.encoding_value)  # type: ignore
-
-        self.layout.addWidget(self.encoding_label)
-        self.layout.addWidget(self.encoding_widget)
-
-        self.picks_unit_label = QLabel("Unit")
-        self.picks_unit_widget = QComboBoxMapping(
-            {0: ("Microseconds", "mcs"), 1: ("Milliseconds", "ms"), 2: ("Samples", "sample")},
-            current_value=self.picks_unit_value,
-        )
-
-        self.layout.addWidget(self.picks_unit_label)
-        self.layout.addWidget(self.picks_unit_widget)
-
-        self._previous_values = self.get_values()
-        self.align_and_update_values()
-
-        # connect after aligning
-        self.picks_unit_widget.value_changed_signal.connect(self.values_changed)
-        self.encoding_widget.value_changed_signal.connect(self.values_changed)
-
-    def align_and_update_values(self) -> None:
-        self.encoding_value = self.encoding_widget.value()
-        self.byte_position_value = self.byte_position_widget.value()
-        self.picks_unit_value = self.picks_unit_widget.value()
-
-        byte_position_maximum_aligned = self.first_byte + 240 - Headers.format2size[self.encoding_value]
-        byte_position_value_aligned = min(self.byte_position_value, byte_position_maximum_aligned)
-
-        if byte_position_maximum_aligned != self.byte_position_maximum:
-            self.byte_position_maximum = byte_position_maximum_aligned
-            self.byte_position_widget.setMaximum(self.byte_position_maximum)
-
-        if byte_position_value_aligned != self.byte_position_value:
-            self.byte_position_value = byte_position_value_aligned
-            self.byte_position_widget.setValue(self.byte_position_value)
-
-    def get_values(self) -> Dict[str, Any]:
-        return {
-            "byte_position": self.byte_position_widget.value() - self.first_byte,
-            "encoding": self.encoding_widget.value(),
-            "picks_unit": self.picks_unit_widget.value(),
-        }
-
-    def values_changed(self) -> None:
-        self.align_and_update_values()
-        values = self.get_values()
-        if values != self._previous_values:  # avoid emit extra signal if chained triggers happen
-            self._previous_values = values
-            self.values_changed_signal.emit(values)
-
-
-class QDialogByteEncodeUnit(QDialog):
-    def __init__(self, *args: Any, **kwargs: Any) -> None:
-        super().__init__()
-
-        self.layout = QVBoxLayout()
-        self.setLayout(self.layout)
-
-        self.widget = QByteEncodeUnitWidget(*args, **kwargs)
-        self.layout.addWidget(self.widget)
-
-        self.button_box = QDialogButtonBox()
-        self.button_box.addButton("Ok", QDialogButtonBox.AcceptRole)
-        self.button_box.accepted.connect(self.accept)
-
-        self.layout.addWidget(self.button_box)
-
-    def get_values(self) -> Dict[str, Any]:
-        return self.widget.get_values()
-
-
-if __name__ == "__main__":
-    app = QApplication([])
-    window = QDialogByteEncodeUnit(first_byte=1, byte_position=237, encoding="I", picks_unit="mcs")
-    window.show()
-    app.exec_()
-    print(window.get_values())
+import warnings
+from typing import Any, Dict, Optional, Tuple
+
+from PyQt5.QtCore import Qt, pyqtSignal
+from PyQt5.QtWidgets import (
+    QApplication,
+    QDialog,
+    QDialogButtonBox,
+    QHBoxLayout,
+    QLabel,
+    QSpinBox,
+    QVBoxLayout,
+    QWidget,
+)
+
+from first_breaks.const import HIGH_DPI
+from first_breaks.desktop.combobox_with_mapping import QComboBoxMapping
+from first_breaks.sgy.headers import Headers
+
+if HIGH_DPI:
+    QApplication.setAttribute(Qt.AA_EnableHighDpiScaling, True)
+    QApplication.setAttribute(Qt.AA_UseHighDpiPixmaps, True)
+
+warnings.filterwarnings("ignore")
+
+
+def build_encoding_mapping() -> Dict[int, Tuple[str, str]]:
+    mapping = {
+        0: ("Integer 4", "i"),
+        1: ("UInteger 4", "I"),
+        2: ("Short 2", "h"),
+        3: ("UShort 2", "H"),
+        4: ("Long 4", "l"),
+        5: ("ULong 4", "L"),
+        6: ("Float 4", "f"),
+        7: ("Double 8", "d"),
+    }
+    assert all(v[1] in Headers.format2size.keys() for v in mapping.values())
+    return mapping
+
+
+ENCODING_MAPPING = build_encoding_mapping()
+
+
+class QByteEncodeUnitWidget(QWidget):
+    values_changed_signal = pyqtSignal(dict)
+
+    def __init__(
+        self,
+        byte_position: int = 0,
+        encoding: str = "I",
+        first_byte: int = 0,
+        picks_unit: str = "mcs",
+        margins: Optional[int] = None,
+        *args: Any,
+        **kwargs: Any
+    ) -> None:
+        super().__init__(*args, **kwargs)
+
+        self.layout = QHBoxLayout()
+        if margins is not None:
+            self.layout.setContentsMargins(margins, margins, margins, margins)
+        self.setLayout(self.layout)
+
+        assert byte_position >= first_byte
+        self.byte_position_value = byte_position
+        self.encoding_value = encoding
+        self.first_byte = first_byte
+        self.byte_position_maximum = 240 + self.first_byte
+        self.picks_unit_value = picks_unit
+
+        self.byte_position_label = QLabel("Byte")
+        self.byte_position_widget = QSpinBox()
+        self.byte_position_widget.setRange(self.first_byte, self.byte_position_maximum)
+        self.byte_position_widget.setValue(self.byte_position_value)
+        self.byte_position_widget.valueChanged.connect(self.values_changed)
+
+        self.layout.addWidget(self.byte_position_label)
+        self.layout.addWidget(self.byte_position_widget)
+
+        self.encoding_label = QLabel("Encoding")
+        self.encoding_widget = QComboBoxMapping(ENCODING_MAPPING, current_value=self.encoding_value)  # type: ignore
+
+        self.layout.addWidget(self.encoding_label)
+        self.layout.addWidget(self.encoding_widget)
+
+        self.picks_unit_label = QLabel("Unit")
+        self.picks_unit_widget = QComboBoxMapping(
+            {0: ("Microseconds", "mcs"), 1: ("Milliseconds", "ms"), 2: ("Samples", "sample")},
+            current_value=self.picks_unit_value,
+        )
+
+        self.layout.addWidget(self.picks_unit_label)
+        self.layout.addWidget(self.picks_unit_widget)
+
+        self._previous_values = self.get_values()
+        self.align_and_update_values()
+
+        # connect after aligning
+        self.picks_unit_widget.value_changed_signal.connect(self.values_changed)
+        self.encoding_widget.value_changed_signal.connect(self.values_changed)
+
+    def align_and_update_values(self) -> None:
+        self.encoding_value = self.encoding_widget.value()
+        self.byte_position_value = self.byte_position_widget.value()
+        self.picks_unit_value = self.picks_unit_widget.value()
+
+        byte_position_maximum_aligned = self.first_byte + 240 - Headers.format2size[self.encoding_value]
+        byte_position_value_aligned = min(self.byte_position_value, byte_position_maximum_aligned)
+
+        if byte_position_maximum_aligned != self.byte_position_maximum:
+            self.byte_position_maximum = byte_position_maximum_aligned
+            self.byte_position_widget.setMaximum(self.byte_position_maximum)
+
+        if byte_position_value_aligned != self.byte_position_value:
+            self.byte_position_value = byte_position_value_aligned
+            self.byte_position_widget.setValue(self.byte_position_value)
+
+    def get_values(self) -> Dict[str, Any]:
+        return {
+            "byte_position": self.byte_position_widget.value() - self.first_byte,
+            "encoding": self.encoding_widget.value(),
+            "picks_unit": self.picks_unit_widget.value(),
+        }
+
+    def values_changed(self) -> None:
+        self.align_and_update_values()
+        values = self.get_values()
+        if values != self._previous_values:  # avoid emit extra signal if chained triggers happen
+            self._previous_values = values
+            self.values_changed_signal.emit(values)
+
+
+class QDialogByteEncodeUnit(QDialog):
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        super().__init__()
+
+        self.layout = QVBoxLayout()
+        self.setLayout(self.layout)
+
+        self.widget = QByteEncodeUnitWidget(*args, **kwargs)
+        self.layout.addWidget(self.widget)
+
+        self.button_box = QDialogButtonBox()
+        self.button_box.addButton("Ok", QDialogButtonBox.AcceptRole)
+        self.button_box.accepted.connect(self.accept)
+
+        self.layout.addWidget(self.button_box)
+
+    def get_values(self) -> Dict[str, Any]:
+        return self.widget.get_values()
+
+
+if __name__ == "__main__":
+    app = QApplication([])
+    window = QDialogByteEncodeUnit(first_byte=1, byte_position=237, encoding="I", picks_unit="mcs")
+    window.show()
+    app.exec_()
+    print(window.get_values())
```

### Comparing `first-breaks-picking-0.3.0b0/first_breaks/desktop/combobox_with_mapping.py` & `first-breaks-picking-0.4.0a0/first_breaks/desktop/combobox_with_mapping.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-import warnings
-from typing import Any, Optional
-
-from PyQt5.QtCore import Qt, pyqtSignal
-from PyQt5.QtWidgets import QApplication, QComboBox
-
-from first_breaks.const import HIGH_DPI
-from first_breaks.desktop.utils import (
-    TMappingSetup,
-    validate_mapping_setup_and_get_current_index,
-)
-
-if HIGH_DPI:
-    QApplication.setAttribute(Qt.AA_EnableHighDpiScaling, True)
-    QApplication.setAttribute(Qt.AA_UseHighDpiPixmaps, True)
-
-warnings.filterwarnings("ignore")
-
-
-class QComboBoxMapping(QComboBox):
-    index_changed_signal = pyqtSignal(int)
-    value_changed_signal = pyqtSignal(object)
-    label_changed_signal = pyqtSignal(str)
-    changed_signal = pyqtSignal()
-
-    def __init__(
-        self,
-        mapping: TMappingSetup,
-        current_index: Optional[int] = None,
-        current_label: Optional[str] = None,
-        current_value: Optional[str] = None,
-        *args: Any,
-        **kwargs: Any
-    ):
-        super().__init__(*args, **kwargs)
-
-        current_index = validate_mapping_setup_and_get_current_index(
-            mapping,
-            current_index=current_index,
-            current_label=current_label,
-            current_value=current_value,
-        )
-
-        self.mapping = mapping
-        self.current_index = current_index
-
-        items = [v[0] for v in self.mapping.values()]
-        self.addItems(items)
-
-        self.setCurrentIndex(current_index)
-        self.currentIndexChanged.connect(self.changed)
-
-    def changed(self) -> None:
-        self.index_changed_signal.emit(self.currentIndex())
-        self.value_changed_signal.emit(self.value())
-        self.label_changed_signal.emit(self.label())
-        self.changed_signal.emit()
-
-    def value(self) -> str:
-        return self.mapping[self.currentIndex()][1]
-
-    def text(self) -> str:
-        return str(self.value())
-
-    def label(self) -> str:
-        return self.mapping[self.currentIndex()][0]
+import warnings
+from typing import Any, Optional
+
+from PyQt5.QtCore import Qt, pyqtSignal
+from PyQt5.QtWidgets import QApplication, QComboBox
+
+from first_breaks.const import HIGH_DPI
+from first_breaks.desktop.utils import (
+    TMappingSetup,
+    validate_mapping_setup_and_get_current_index,
+)
+
+if HIGH_DPI:
+    QApplication.setAttribute(Qt.AA_EnableHighDpiScaling, True)
+    QApplication.setAttribute(Qt.AA_UseHighDpiPixmaps, True)
+
+warnings.filterwarnings("ignore")
+
+
+class QComboBoxMapping(QComboBox):
+    index_changed_signal = pyqtSignal(int)
+    value_changed_signal = pyqtSignal(object)
+    label_changed_signal = pyqtSignal(str)
+    changed_signal = pyqtSignal()
+
+    def __init__(
+        self,
+        mapping: TMappingSetup,
+        current_index: Optional[int] = None,
+        current_label: Optional[str] = None,
+        current_value: Optional[str] = None,
+        *args: Any,
+        **kwargs: Any
+    ):
+        super().__init__(*args, **kwargs)
+
+        current_index = validate_mapping_setup_and_get_current_index(
+            mapping,
+            current_index=current_index,
+            current_label=current_label,
+            current_value=current_value,
+        )
+
+        self.mapping = mapping
+        self.current_index = current_index
+
+        items = [v[0] for v in self.mapping.values()]
+        self.addItems(items)
+
+        self.setCurrentIndex(current_index)
+        self.currentIndexChanged.connect(self.changed)
+
+    def changed(self) -> None:
+        self.index_changed_signal.emit(self.currentIndex())
+        self.value_changed_signal.emit(self.value())
+        self.label_changed_signal.emit(self.label())
+        self.changed_signal.emit()
+
+    def value(self) -> str:
+        return self.mapping[self.currentIndex()][1]
+
+    def text(self) -> str:
+        return str(self.value())
+
+    def label(self) -> str:
+        return self.mapping[self.currentIndex()][0]
```

### Comparing `first-breaks-picking-0.3.0b0/first_breaks/desktop/radioset_widget.py` & `first-breaks-picking-0.4.0a0/first_breaks/desktop/radioset_widget.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-from typing import Any, Optional
-
-from PyQt5.QtCore import pyqtSignal
-from PyQt5.QtWidgets import (
-    QApplication,
-    QHBoxLayout,
-    QRadioButton,
-    QVBoxLayout,
-    QWidget,
-)
-
-from first_breaks.desktop.utils import (
-    TMappingSetup,
-    validate_mapping_setup_and_get_current_index,
-)
-
-
-class QRadioSetWidget(QWidget):
-    index_changed_signal = pyqtSignal(int)
-    value_changed_signal = pyqtSignal(object)
-    label_changed_signal = pyqtSignal(str)
-    changed_signal = pyqtSignal()
-
-    def __init__(
-        self,
-        mapping: TMappingSetup,
-        current_index: Optional[int] = None,
-        current_label: Optional[str] = None,
-        current_value: Optional[str] = None,
-        orientation: str = "horizontal",
-        margins: Optional[int] = None,
-        *args: Any,
-        **kwargs: Any
-    ):
-        super().__init__(*args, **kwargs)
-        assert orientation in ["horizontal", "vertical"]
-
-        current_index = validate_mapping_setup_and_get_current_index(
-            mapping,
-            current_index=current_index,
-            current_label=current_label,
-            current_value=current_value,
-        )
-
-        self.mapping = mapping
-        self.current_index = current_index
-
-        if orientation == "horizontal":
-            self.layout = QHBoxLayout()
-        else:
-            self.layout = QVBoxLayout()
-        self.setLayout(self.layout)
-        if margins is not None:
-            self.layout.setContentsMargins(margins, margins, margins, margins)
-
-        self.storage = {}
-        self.selected_idx = current_index
-
-        for idx, (label, value) in mapping.items():
-            radio = QRadioButton(label)
-            self.storage[radio] = idx
-            if idx == current_index:
-                radio.setChecked(True)
-            radio.toggled.connect(lambda *lambda_args, **lambda_kwargs: self.changed())
-            self.layout.addWidget(radio)
-
-    def changed(self) -> None:
-        radio = self.sender()
-        if radio.isChecked():
-            self.selected_idx = self.storage[radio]
-
-            self.index_changed_signal.emit(self.selected_idx)
-            self.value_changed_signal.emit(self.value())
-            self.label_changed_signal.emit(self.label())
-            self.changed_signal.emit()
-
-    def value(self) -> Any:
-        return self.mapping[self.selected_idx][1]
-
-    def text(self) -> str:
-        return str(self.value())
-
-    def label(self) -> Any:
-        return self.mapping[self.selected_idx][0]
-
-
-if __name__ == "__main__":
-    app = QApplication([])
-    window = QRadioSetWidget({0: ("A", "aa"), 1: ("B", "bb"), 2: ("C", "cc")})
-    window.show()
-    app.exec_()
+from typing import Any, Optional
+
+from PyQt5.QtCore import pyqtSignal
+from PyQt5.QtWidgets import (
+    QApplication,
+    QHBoxLayout,
+    QRadioButton,
+    QVBoxLayout,
+    QWidget,
+)
+
+from first_breaks.desktop.utils import (
+    TMappingSetup,
+    validate_mapping_setup_and_get_current_index,
+)
+
+
+class QRadioSetWidget(QWidget):
+    index_changed_signal = pyqtSignal(int)
+    value_changed_signal = pyqtSignal(object)
+    label_changed_signal = pyqtSignal(str)
+    changed_signal = pyqtSignal()
+
+    def __init__(
+        self,
+        mapping: TMappingSetup,
+        current_index: Optional[int] = None,
+        current_label: Optional[str] = None,
+        current_value: Optional[str] = None,
+        orientation: str = "horizontal",
+        margins: Optional[int] = None,
+        *args: Any,
+        **kwargs: Any
+    ):
+        super().__init__(*args, **kwargs)
+        assert orientation in ["horizontal", "vertical"]
+
+        current_index = validate_mapping_setup_and_get_current_index(
+            mapping,
+            current_index=current_index,
+            current_label=current_label,
+            current_value=current_value,
+        )
+
+        self.mapping = mapping
+        self.current_index = current_index
+
+        if orientation == "horizontal":
+            self.layout = QHBoxLayout()
+        else:
+            self.layout = QVBoxLayout()
+        self.setLayout(self.layout)
+        if margins is not None:
+            self.layout.setContentsMargins(margins, margins, margins, margins)
+
+        self.storage = {}
+        self.selected_idx = current_index
+
+        for idx, (label, value) in mapping.items():
+            radio = QRadioButton(label)
+            self.storage[radio] = idx
+            if idx == current_index:
+                radio.setChecked(True)
+            radio.toggled.connect(lambda *lambda_args, **lambda_kwargs: self.changed())
+            self.layout.addWidget(radio)
+
+    def changed(self) -> None:
+        radio = self.sender()
+        if radio.isChecked():
+            self.selected_idx = self.storage[radio]
+
+            self.index_changed_signal.emit(self.selected_idx)
+            self.value_changed_signal.emit(self.value())
+            self.label_changed_signal.emit(self.label())
+            self.changed_signal.emit()
+
+    def value(self) -> Any:
+        return self.mapping[self.selected_idx][1]
+
+    def text(self) -> str:
+        return str(self.value())
+
+    def label(self) -> Any:
+        return self.mapping[self.selected_idx][0]
+
+
+if __name__ == "__main__":
+    app = QApplication([])
+    window = QRadioSetWidget({0: ("A", "aa"), 1: ("B", "bb"), 2: ("C", "cc")})
+    window.show()
+    app.exec_()
```

### Comparing `first-breaks-picking-0.3.0b0/first_breaks/desktop/slider_with_values.py` & `first-breaks-picking-0.4.0a0/first_breaks/desktop/slider_with_values.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-from typing import Any, Optional
-
-from PyQt5.QtCore import Qt, pyqtSignal
-from PyQt5.QtWidgets import QApplication, QHBoxLayout, QLabel, QSlider, QWidget
-
-
-class QSliderWithValues(QWidget):
-    value_changed_signal = pyqtSignal(float)
-    slider_released_signal = pyqtSignal()
-    value_on_released_signal = pyqtSignal(float)
-
-    def __init__(
-        self,
-        value: float = 1,
-        min_value: float = -1,
-        max_value: float = 1,
-        step: float = 0.1,
-        decimals: int = 1,
-        ticks_interval: Optional[float] = None,
-        margins: Optional[int] = None,
-        slider_space_fraction: Optional[float] = None,
-        block_mouse_scrolling: bool = True,
-        *args: Any,
-        **kwargs: Any,
-    ):
-        super().__init__(*args, **kwargs)
-
-        self.layout = QHBoxLayout()
-        if margins is not None:
-            self.layout.setContentsMargins(margins, margins, margins, margins)
-        self.setLayout(self.layout)
-
-        self.slider_value = value
-        self.min_value = min_value
-        self.max_value = max_value
-        self.step = step
-        self.decimals = decimals
-        self.num_steps = int((self.max_value - self.min_value) / self.step)
-
-        self.slider_label = QLabel(str(self.slider_value), self)
-
-        self.slider_widget = QSlider(Qt.Horizontal, self)
-
-        self.slider_widget.setRange(0, self.num_steps)
-        self.slider_widget.setValue(self.value2slider(self.slider_value))
-
-        if slider_space_fraction is not None:
-            slider_space = int(slider_space_fraction * 100)
-            self.layout.addWidget(self.slider_widget, slider_space)
-            self.layout.addWidget(self.slider_label, 100 - slider_space)
-        else:
-            self.layout.addWidget(self.slider_widget)
-            self.layout.addWidget(self.slider_label)
-
-        if ticks_interval is not None:
-            self.slider_widget.setTickInterval(int(ticks_interval / self.step))
-            self.slider_widget.setTickPosition(QSlider.TicksAbove)
-            self.slider_widget.setSingleStep(1)
-
-        if block_mouse_scrolling:
-            self.slider_widget.wheelEvent = lambda *e_args: e_args[-1].ignore()  # block scrolling with wheel
-
-        self.slider_widget.sliderPressed.connect(self.slider_pressed)
-        self.slider_widget.sliderReleased.connect(self.slider_released)
-        self.slider_widget.sliderMoved.connect(self.value_changed)
-
-        self.show()
-
-    def slider_pressed(self) -> None:
-        self.value_changed()
-
-    def slider_released(self) -> None:
-        self.value_on_released_signal.emit(self.slider_value)
-        self.slider_released_signal.emit()
-
-    def value_changed(self, *args: Any) -> None:
-        self.slider_value = self.slider2value(self.slider_widget.value())
-        self.slider_label.setText(self.text())
-        self.value_changed_signal.emit(self.slider_value)
-
-    def text(self) -> str:
-        return f"{self.slider_value:.{self.decimals}f}"
-
-    def value2slider(self, value_float: float) -> int:
-        return int((value_float - self.min_value) / self.step)
-
-    def slider2value(self, value_from_slider: int) -> float:
-        return self.min_value + (value_from_slider * self.step)
-
-    def value(self) -> float:
-        return self.slider_value
-
-
-if __name__ == "__main__":
-    app = QApplication([])
-    window = QSliderWithValues(1, -10, 10, slider_space_fraction=0.7, margins=20, ticks_interval=5)
-    # window = QSlider(Qt.Horizontal)
-    # window.valueChanged.connect(lambda x: print(x))
-    # window.rele
-    window.show()
-    app.exec_()
+from typing import Any, Optional
+
+from PyQt5.QtCore import Qt, pyqtSignal
+from PyQt5.QtWidgets import QApplication, QHBoxLayout, QLabel, QSlider, QWidget
+
+
+class QSliderWithValues(QWidget):
+    value_changed_signal = pyqtSignal(float)
+    slider_released_signal = pyqtSignal()
+    value_on_released_signal = pyqtSignal(float)
+
+    def __init__(
+        self,
+        value: float = 1,
+        min_value: float = -1,
+        max_value: float = 1,
+        step: float = 0.1,
+        decimals: int = 1,
+        ticks_interval: Optional[float] = None,
+        margins: Optional[int] = None,
+        slider_space_fraction: Optional[float] = None,
+        block_mouse_scrolling: bool = True,
+        *args: Any,
+        **kwargs: Any,
+    ):
+        super().__init__(*args, **kwargs)
+
+        self.layout = QHBoxLayout()
+        if margins is not None:
+            self.layout.setContentsMargins(margins, margins, margins, margins)
+        self.setLayout(self.layout)
+
+        self.slider_value = value
+        self.min_value = min_value
+        self.max_value = max_value
+        self.step = step
+        self.decimals = decimals
+        self.num_steps = int((self.max_value - self.min_value) / self.step)
+
+        self.slider_label = QLabel(str(self.slider_value), self)
+
+        self.slider_widget = QSlider(Qt.Horizontal, self)
+
+        self.slider_widget.setRange(0, self.num_steps)
+        self.slider_widget.setValue(self.value2slider(self.slider_value))
+
+        if slider_space_fraction is not None:
+            slider_space = int(slider_space_fraction * 100)
+            self.layout.addWidget(self.slider_widget, slider_space)
+            self.layout.addWidget(self.slider_label, 100 - slider_space)
+        else:
+            self.layout.addWidget(self.slider_widget)
+            self.layout.addWidget(self.slider_label)
+
+        if ticks_interval is not None:
+            self.slider_widget.setTickInterval(int(ticks_interval / self.step))
+            self.slider_widget.setTickPosition(QSlider.TicksAbove)
+            self.slider_widget.setSingleStep(1)
+
+        if block_mouse_scrolling:
+            self.slider_widget.wheelEvent = lambda *e_args: e_args[-1].ignore()  # block scrolling with wheel
+
+        self.slider_widget.sliderPressed.connect(self.slider_pressed)
+        self.slider_widget.sliderReleased.connect(self.slider_released)
+        self.slider_widget.sliderMoved.connect(self.value_changed)
+
+        self.show()
+
+    def slider_pressed(self) -> None:
+        self.value_changed()
+
+    def slider_released(self) -> None:
+        self.value_on_released_signal.emit(self.slider_value)
+        self.slider_released_signal.emit()
+
+    def value_changed(self, *args: Any) -> None:
+        self.slider_value = self.slider2value(self.slider_widget.value())
+        self.slider_label.setText(self.text())
+        self.value_changed_signal.emit(self.slider_value)
+
+    def text(self) -> str:
+        return f"{self.slider_value:.{self.decimals}f}"
+
+    def value2slider(self, value_float: float) -> int:
+        return int((value_float - self.min_value) / self.step)
+
+    def slider2value(self, value_from_slider: int) -> float:
+        return self.min_value + (value_from_slider * self.step)
+
+    def value(self) -> float:
+        return self.slider_value
+
+
+if __name__ == "__main__":
+    app = QApplication([])
+    window = QSliderWithValues(1, -10, 10, slider_space_fraction=0.7, margins=20, ticks_interval=5)
+    # window = QSlider(Qt.Horizontal)
+    # window.valueChanged.connect(lambda x: print(x))
+    # window.rele
+    window.show()
+    app.exec_()
```

### Comparing `first-breaks-picking-0.3.0b0/first_breaks/desktop/threads.py` & `first-breaks-picking-0.4.0a0/first_breaks/desktop/threads.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.3.0b0/first_breaks/desktop/utils.py` & `first-breaks-picking-0.4.0a0/first_breaks/desktop/utils.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-from typing import Any, Dict, List, Optional, Tuple, Union
-
-from PyQt5 import QtWidgets
-from PyQt5.QtCore import Qt
-from PyQt5.QtWidgets import (
-    QDesktopWidget,
-    QDialog,
-    QDialogButtonBox,
-    QLabel,
-    QVBoxLayout,
-    QWidget,
-)
-
-
-class MessageBox(QDialog):
-    def __init__(
-        self,
-        parent: QWidget,
-        title: str = "Error",
-        message: str = "Error",
-        add_cancel_option: bool = False,
-        label_ok: str = "Ok",
-        label_cancel: str = "Cancel",
-    ):
-        super().__init__(parent=parent)
-
-        self.setWindowTitle(title)
-        self.setWindowModality(Qt.ApplicationModal)
-        set_geometry(self, width_rel=0.2, height_rel=0.2, centralize=True, fix_size=False)
-
-        error_label = QLabel(message)
-        error_label.setWordWrap(True)
-        error_label.setTextInteractionFlags(Qt.LinksAccessibleByMouse | Qt.TextSelectableByMouse)
-
-        self.button_box = QDialogButtonBox()
-        self.button_box.addButton(label_ok, QDialogButtonBox.AcceptRole)
-        self.button_box.accepted.connect(self.accept)
-        if add_cancel_option:
-            self.button_box.addButton(label_cancel, QDialogButtonBox.RejectRole)
-            self.button_box.rejected.connect(self.reject)
-
-        self.layout = QVBoxLayout()
-        self.layout.addWidget(error_label)
-        self.layout.addWidget(self.button_box)
-        self.setLayout(self.layout)
-
-
-def set_geometry(
-    widget: QWidget,
-    width_rel: float,
-    height_rel: float,
-    centralize: bool = True,
-    fix_size: bool = False,
-) -> None:
-    assert 0 < width_rel <= 1
-    assert 0 < height_rel <= 1
-    h, w = widget.screen().size().height(), widget.screen().size().width()
-    width = int(width_rel * w)
-    height = int(height_rel * h)
-    widget.setGeometry(0, 0, width, height)
-
-    if centralize:
-        qt_rectangle = widget.frameGeometry()
-        center_point = QDesktopWidget().availableGeometry().center()
-        qt_rectangle.moveCenter(center_point)
-        widget.move(qt_rectangle.topLeft())
-
-    if fix_size:
-        widget.setFixedSize(width, height)
-
-    monitor = QDesktopWidget().screenGeometry(1)
-    widget.move(monitor.left(), monitor.top())
-
-
-class QHSeparationLine(QtWidgets.QFrame):
-    def __init__(self) -> None:
-        super().__init__()
-        self.setMinimumWidth(1)
-        self.setFixedHeight(20)
-        self.setFrameShape(QtWidgets.QFrame.HLine)
-        self.setFrameShadow(QtWidgets.QFrame.Sunken)
-        self.setSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Minimum)
-
-
-TMappingSetup = Dict[int, Union[Tuple[str, Any], List[Any]]]
-
-
-def validate_mapping_setup_and_get_current_index(
-    mapping: TMappingSetup,
-    current_index: Optional[int] = None,
-    current_label: Optional[str] = None,
-    current_value: Optional[Any] = None,
-) -> int:
-    assert all(isinstance(k, int) for k in mapping.keys())
-    assert all(isinstance(v, (list, tuple)) and len(v) == 2 for v in mapping.values())
-    assert all(isinstance(label, str) for label, _ in mapping.values())
-    assert set(range(len(mapping.keys()))) == set(mapping.keys())
-
-    current_is_not_none = [v is not None for v in [current_index, current_label, current_value]]
-    assert (
-        0 <= sum(current_is_not_none) <= 1
-    ), "Only one of 'current_index' or 'current_label' or 'current_value' might be specified."
-
-    if current_label or current_value:
-        if current_label:
-            assert isinstance(current_label, str)
-            idx_to_check = 0
-            type_to_check = "Label"
-            got = current_label
-        else:
-            idx_to_check = 1
-            type_to_check = "Value"
-            got = current_value
-
-        corresponding_ids = [k for k, v in mapping.items() if v[idx_to_check] == got]
-
-        if not corresponding_ids:
-            raise KeyError(
-                f"{type_to_check} '{type_to_check}' not found in mapping. "
-                f"Available {[v[idx_to_check] for v in mapping.values()]}, got '{got}'"
-            )
-        current_index = corresponding_ids[0]
-    elif current_index:
-        assert isinstance(current_index, int)
-        assert 0 <= current_index < len(mapping)
-    else:
-        current_index = 0
-
-    return current_index
+from typing import Any, Dict, List, Optional, Tuple, Union
+
+from PyQt5 import QtWidgets
+from PyQt5.QtCore import Qt
+from PyQt5.QtWidgets import (
+    QDesktopWidget,
+    QDialog,
+    QDialogButtonBox,
+    QLabel,
+    QVBoxLayout,
+    QWidget,
+)
+
+
+class MessageBox(QDialog):
+    def __init__(
+        self,
+        parent: QWidget,
+        title: str = "Error",
+        message: str = "Error",
+        add_cancel_option: bool = False,
+        label_ok: str = "Ok",
+        label_cancel: str = "Cancel",
+    ):
+        super().__init__(parent=parent)
+
+        self.setWindowTitle(title)
+        self.setWindowModality(Qt.ApplicationModal)
+        set_geometry(self, width_rel=0.2, height_rel=0.2, centralize=True, fix_size=False)
+
+        error_label = QLabel(message)
+        error_label.setWordWrap(True)
+        error_label.setTextInteractionFlags(Qt.LinksAccessibleByMouse | Qt.TextSelectableByMouse)
+
+        self.button_box = QDialogButtonBox()
+        self.button_box.addButton(label_ok, QDialogButtonBox.AcceptRole)
+        self.button_box.accepted.connect(self.accept)
+        if add_cancel_option:
+            self.button_box.addButton(label_cancel, QDialogButtonBox.RejectRole)
+            self.button_box.rejected.connect(self.reject)
+
+        self.layout = QVBoxLayout()
+        self.layout.addWidget(error_label)
+        self.layout.addWidget(self.button_box)
+        self.setLayout(self.layout)
+
+
+def set_geometry(
+    widget: QWidget,
+    width_rel: float,
+    height_rel: float,
+    centralize: bool = True,
+    fix_size: bool = False,
+) -> None:
+    assert 0 < width_rel <= 1
+    assert 0 < height_rel <= 1
+    h, w = widget.screen().size().height(), widget.screen().size().width()
+    width = int(width_rel * w)
+    height = int(height_rel * h)
+    widget.setGeometry(0, 0, width, height)
+
+    if centralize:
+        qt_rectangle = widget.frameGeometry()
+        center_point = QDesktopWidget().availableGeometry().center()
+        qt_rectangle.moveCenter(center_point)
+        widget.move(qt_rectangle.topLeft())
+
+    if fix_size:
+        widget.setFixedSize(width, height)
+
+    monitor = QDesktopWidget().screenGeometry(1)
+    widget.move(monitor.left(), monitor.top())
+
+
+class QHSeparationLine(QtWidgets.QFrame):
+    def __init__(self) -> None:
+        super().__init__()
+        self.setMinimumWidth(1)
+        self.setFixedHeight(20)
+        self.setFrameShape(QtWidgets.QFrame.HLine)
+        self.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.setSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Minimum)
+
+
+TMappingSetup = Dict[int, Union[Tuple[str, Any], List[Any]]]
+
+
+def validate_mapping_setup_and_get_current_index(
+    mapping: TMappingSetup,
+    current_index: Optional[int] = None,
+    current_label: Optional[str] = None,
+    current_value: Optional[Any] = None,
+) -> int:
+    assert all(isinstance(k, int) for k in mapping.keys())
+    assert all(isinstance(v, (list, tuple)) and len(v) == 2 for v in mapping.values())
+    assert all(isinstance(label, str) for label, _ in mapping.values())
+    assert set(range(len(mapping.keys()))) == set(mapping.keys())
+
+    current_is_not_none = [v is not None for v in [current_index, current_label, current_value]]
+    assert (
+        0 <= sum(current_is_not_none) <= 1
+    ), "Only one of 'current_index' or 'current_label' or 'current_value' might be specified."
+
+    if current_label or current_value:
+        if current_label:
+            assert isinstance(current_label, str)
+            idx_to_check = 0
+            type_to_check = "Label"
+            got = current_label
+        else:
+            idx_to_check = 1
+            type_to_check = "Value"
+            got = current_value
+
+        corresponding_ids = [k for k, v in mapping.items() if v[idx_to_check] == got]
+
+        if not corresponding_ids:
+            raise KeyError(
+                f"{type_to_check} '{type_to_check}' not found in mapping. "
+                f"Available {[v[idx_to_check] for v in mapping.values()]}, got '{got}'"
+            )
+        current_index = corresponding_ids[0]
+    elif current_index:
+        assert isinstance(current_index, int)
+        assert 0 <= current_index < len(mapping)
+    else:
+        current_index = 0
+
+    return current_index
```

### Comparing `first-breaks-picking-0.3.0b0/first_breaks/picking/ipicker.py` & `first-breaks-picking-0.4.0a0/first_breaks/picking/ipicker.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.3.0b0/first_breaks/picking/picker_onnx.py` & `first-breaks-picking-0.4.0a0/first_breaks/picking/picker_onnx.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,137 +1,132 @@
-from pathlib import Path
-from typing import Any, Dict, Generator, Optional, Tuple, Union
-
-import numpy as np
-import onnxruntime as ort
-
-from first_breaks.picking.ipicker import IPicker
-from first_breaks.picking.task import Task
-from first_breaks.picking.utils import preprocess_gather
-from first_breaks.utils.utils import (
-    ONNX_DEVICE2PROVIDER,
-    calc_hash,
-    chunk_iterable,
-    download_model_onnx,
-    is_onnx_cuda_available,
-)
-
-
-class IteratorOfTask:
-    gather_key = "gather"
-    gather_ids_key = "gather_ids"
-
-    def __init__(self, task: Task):
-        self.task = task
-        self.idx2gather_ids = {idx: gather_ids for idx, gather_ids in enumerate(self.task.get_gathers_ids())}
-
-    def __len__(self) -> int:
-        return len(self.idx2gather_ids)
-
-    def __getitem__(self, idx: int) -> Dict[str, np.ndarray]:
-        gather_ids = self.idx2gather_ids[idx]
-        amplitudes = np.array(
-            [-1 if idx in self.task.traces_to_inverse else 1 for idx in range(len(gather_ids))], dtype=np.float32
-        )
-        gather = self.task.sgy.read_traces_by_ids(gather_ids)
-        gather = preprocess_gather(gather, self.task.gain, self.task.clip)
-        gather = amplitudes[None, :] * gather
-        gather = gather[: self.task.maximum_time_sample, :]
-
-        return {self.gather_key: gather, self.gather_ids_key: np.array(gather_ids)}
-
-    def get_batch_generator(self, batch_size: int = 1) -> Generator[Dict[str, np.ndarray], None, None]:
-        for ids in chunk_iterable(range(len(self)), batch_size):
-            gather_batch = []
-            gather_ids_batch = []
-            for idx in ids:
-                item = self[idx]
-                gather_batch.append(item[self.gather_key][None, ...])
-                gather_ids_batch.append(item[self.gather_ids_key])
-
-            gather_batch = np.stack(gather_batch, axis=0)
-            gather_ids_batch = np.hstack(gather_ids_batch)
-            batch = {self.gather_key: gather_batch, self.gather_ids_key: gather_ids_batch}
-            yield batch
-
-
-class PickerONNX(IPicker):
-    def __init__(
-        self,
-        model_path: Optional[Union[str, Path]] = None,
-        show_progressbar: bool = True,
-        device: str = "cuda" if is_onnx_cuda_available() else "cpu",
-        batch_size: int = 1,
-    ):
-        super().__init__(show_progressbar=show_progressbar)
-        assert device in ["cpu", "cuda"]
-
-        if model_path is None:
-            model_path = download_model_onnx()
-        self.model_path = model_path
-        self.model_hash = calc_hash(self.model_path)
-
-        self.device = device
-        self.batch_size = batch_size
-
-        self.model: Optional[ort.InferenceSession] = None
-        self.init_model()
-
-    def init_model(self) -> None:
-        sess_opt = ort.SessionOptions()
-        sess_opt.graph_optimization_level = ort.GraphOptimizationLevel.ORT_ENABLE_ALL
-        if self.device == "cuda":
-            sess_opt = ort.SessionOptions()
-            sess_opt.intra_op_num_threads = 2
-            sess_opt.inter_op_num_threads = 2
-        self.model = ort.InferenceSession(
-            str(self.model_path), providers=[ONNX_DEVICE2PROVIDER[self.device]], sess_options=sess_opt
-        )
-
-    def change_settings(  # type: ignore
-        self, *args: Any, device: Optional[str] = None, batch_size: Optional[int] = None
-    ) -> "PickerONNX":
-        if args:
-            raise ValueError("Use named arguments instead of positional")
-
-        if device and device != self.device:
-            self.device = device
-            self.init_model()
-
-        if batch_size:
-            self.batch_size = batch_size
-
-        return self
-
-    def pick_batch_of_gathers(self, gather: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
-        assert gather.ndim == 4
-        assert all(dim > 0 for dim in gather.shape)
-        outputs = self.model.run(None, {"input": gather})
-        return outputs[0], outputs[1]
-
-    def process_task(self, task: Task) -> Task:
-        task_picks_in_sample = np.zeros(task.sgy.num_traces)
-        task_confidence = np.zeros(task.sgy.num_traces)
-
-        task_iterator = IteratorOfTask(task)
-        counter_step_finished = 0
-        self.callback_processing_started(len(task_iterator))
-
-        for batch in task_iterator.get_batch_generator(batch_size=self.batch_size):
-            data = batch["gather"]
-            picks, confidence = self.pick_batch_of_gathers(data)
-
-            indices = batch["gather_ids"]
-            task_picks_in_sample[indices.flatten()] = picks.flatten()
-            task_confidence[indices.flatten()] = confidence.flatten()
-
-            counter_step_finished += len(data)
-            self.callback_step_finished(counter_step_finished)
-
-        self.callback_processing_finished()
-
-        task.success = True
-        task.picks_in_samples = task_picks_in_sample.astype(int).tolist()
-        task.confidence = task_confidence.tolist()
-        task.model_hash = self.model_hash
-
-        return task
+from pathlib import Path
+from typing import Any, Dict, Generator, Optional, Tuple, Union
+
+import numpy as np
+import onnxruntime as ort
+
+from first_breaks.picking.ipicker import IPicker
+from first_breaks.picking.task import Task
+from first_breaks.picking.utils import preprocess_gather
+from first_breaks.utils.cuda import ONNX_CUDA_AVAILABLE, ONNX_DEVICE2PROVIDER
+from first_breaks.utils.utils import calc_hash, chunk_iterable, download_model_onnx
+
+
+class IteratorOfTask:
+    gather_key = "gather"
+    gather_ids_key = "gather_ids"
+
+    def __init__(self, task: Task):
+        self.task = task
+        self.idx2gather_ids = {idx: gather_ids for idx, gather_ids in enumerate(self.task.get_gathers_ids())}
+
+    def __len__(self) -> int:
+        return len(self.idx2gather_ids)
+
+    def __getitem__(self, idx: int) -> Dict[str, np.ndarray]:
+        gather_ids = self.idx2gather_ids[idx]
+        amplitudes = np.array(
+            [-1 if idx in self.task.traces_to_inverse else 1 for idx in range(len(gather_ids))], dtype=np.float32
+        )
+        gather = self.task.sgy.read_traces_by_ids(gather_ids)
+        gather = preprocess_gather(gather, self.task.gain, self.task.clip)
+        gather = amplitudes[None, :] * gather
+        gather = gather[: self.task.maximum_time_sample, :]
+
+        return {self.gather_key: gather, self.gather_ids_key: np.array(gather_ids)}
+
+    def get_batch_generator(self, batch_size: int = 1) -> Generator[Dict[str, np.ndarray], None, None]:
+        for ids in chunk_iterable(range(len(self)), batch_size):
+            gather_batch = []
+            gather_ids_batch = []
+            for idx in ids:
+                item = self[idx]
+                gather_batch.append(item[self.gather_key][None, ...])
+                gather_ids_batch.append(item[self.gather_ids_key])
+
+            gather_batch = np.stack(gather_batch, axis=0)
+            gather_ids_batch = np.hstack(gather_ids_batch)
+            batch = {self.gather_key: gather_batch, self.gather_ids_key: gather_ids_batch}
+            yield batch
+
+
+class PickerONNX(IPicker):
+    def __init__(
+        self,
+        model_path: Optional[Union[str, Path]] = None,
+        show_progressbar: bool = True,
+        device: str = "cuda" if ONNX_CUDA_AVAILABLE else "cpu",
+        batch_size: int = 1,
+    ):
+        super().__init__(show_progressbar=show_progressbar)
+        assert device in ["cpu", "cuda"]
+
+        if model_path is None:
+            model_path = download_model_onnx()
+        self.model_path = model_path
+        self.model_hash = calc_hash(self.model_path)
+
+        self.device = device
+        self.batch_size = batch_size
+
+        self.model: Optional[ort.InferenceSession] = None
+        self.init_model()
+
+    def init_model(self) -> None:
+        sess_opt = ort.SessionOptions()
+        sess_opt.graph_optimization_level = ort.GraphOptimizationLevel.ORT_ENABLE_ALL
+        if self.device == "cuda":
+            sess_opt = ort.SessionOptions()
+            sess_opt.intra_op_num_threads = 2
+            sess_opt.inter_op_num_threads = 2
+        self.model = ort.InferenceSession(
+            str(self.model_path), providers=[ONNX_DEVICE2PROVIDER[self.device]], sess_options=sess_opt
+        )
+
+    def change_settings(  # type: ignore
+        self, *args: Any, device: Optional[str] = None, batch_size: Optional[int] = None
+    ) -> "PickerONNX":
+        if args:
+            raise ValueError("Use named arguments instead of positional")
+
+        if device and device != self.device:
+            self.device = device
+            self.init_model()
+
+        if batch_size:
+            self.batch_size = batch_size
+
+        return self
+
+    def pick_batch_of_gathers(self, gather: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
+        assert gather.ndim == 4
+        assert all(dim > 0 for dim in gather.shape)
+        outputs = self.model.run(None, {"input": gather})
+        return outputs[0], outputs[1]
+
+    def process_task(self, task: Task) -> Task:
+        task_picks_in_sample = np.zeros(task.sgy.num_traces)
+        task_confidence = np.zeros(task.sgy.num_traces)
+
+        task_iterator = IteratorOfTask(task)
+        counter_step_finished = 0
+        self.callback_processing_started(len(task_iterator))
+
+        for batch in task_iterator.get_batch_generator(batch_size=self.batch_size):
+            data = batch["gather"]
+            picks, confidence = self.pick_batch_of_gathers(data)
+
+            indices = batch["gather_ids"]
+            task_picks_in_sample[indices.flatten()] = picks.flatten()
+            task_confidence[indices.flatten()] = confidence.flatten()
+
+            counter_step_finished += len(data)
+            self.callback_step_finished(counter_step_finished)
+
+        self.callback_processing_finished()
+
+        task.success = True
+        task.picks_in_samples = task_picks_in_sample.astype(int).tolist()
+        task.confidence = task_confidence.tolist()
+        task.model_hash = self.model_hash
+
+        return task
```

### Comparing `first-breaks-picking-0.3.0b0/first_breaks/picking/task.py` & `first-breaks-picking-0.4.0a0/first_breaks/picking/task.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,229 +1,229 @@
-import json
-import warnings
-from pathlib import Path
-from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
-
-import numpy as np
-import pandas as pd
-
-from first_breaks.sgy.reader import SGY
-from first_breaks.utils.utils import chunk_iterable, multiply_iterable_by
-
-MINIMUM_TRACES_PER_GATHER = 2
-
-
-class ProcessingParametersException(Exception):
-    pass
-
-
-class Task:
-    def __init__(
-        self,
-        sgy: Union[SGY, str, Path, bytes],
-        traces_per_gather: int = 24,
-        maximum_time: float = 0.0,
-        traces_to_inverse: Sequence[int] = (),
-        gain: float = 1,
-        clip: float = 1,
-    ) -> None:
-        self.sgy = sgy if isinstance(sgy, SGY) else SGY(sgy)
-
-        self.traces_per_gather = traces_per_gather
-        self.maximum_time = maximum_time
-        self.traces_to_inverse = traces_to_inverse
-        self.gain = gain
-        self.clip = clip
-
-        self.traces_per_gather_parsed = self.validate_and_parse_traces_per_gather(traces_per_gather)
-        self.maximum_time_parsed = self.validate_and_parse_maximum_time(maximum_time)
-        self.maximum_time_sample = self.sgy.ms2index(self.maximum_time_parsed)
-        self.traces_to_inverse_parsed = self.validate_and_parse_traces_to_inverse(traces_to_inverse)
-        self.gain_parsed = self.validate_and_parse_gain(gain)
-        self.clip_parsed = self.validate_and_parse_clip(clip)
-
-        self.picks_in_samples: Optional[Union[Sequence[float], np.ndarray]] = None
-        self.confidence: Optional[Union[Sequence[float], np.ndarray]] = None
-        self.success: Optional[bool] = None
-        self.error_message: Optional[str] = None
-        self.model_hash: Optional[str] = None
-
-    @classmethod
-    def validate_traces_per_gather(cls, traces_per_gather: int) -> None:
-        if not isinstance(traces_per_gather, int):
-            raise ProcessingParametersException("`traces_per_gather` must be integer")
-        if traces_per_gather < MINIMUM_TRACES_PER_GATHER:
-            raise ProcessingParametersException(
-                f"`traces_per_gather` must be greater or " f"equal to {MINIMUM_TRACES_PER_GATHER}"
-            )
-
-    @classmethod
-    def validate_maximum_time(cls, maximum_time: float) -> None:
-        if not isinstance(maximum_time, (int, float)):
-            raise ProcessingParametersException("`maximum_time` must be real")
-
-        if maximum_time < 0.0:
-            raise ProcessingParametersException("`maximum_time` must be positive or equal to 0")
-
-    @classmethod
-    def validate_traces_to_inverse(cls, traces_to_inverse: Sequence[int]) -> None:
-        if not isinstance(traces_to_inverse, (tuple, list)):
-            raise ProcessingParametersException("`traces_to_inverse` must be tuple or list")
-
-        if not all(isinstance(val, int) for val in traces_to_inverse):
-            raise ProcessingParametersException("Elements of `traces_to_inverse` must be int")
-
-        if not all(val >= 1 for val in traces_to_inverse):
-            raise ProcessingParametersException("Elements of `traces_to_inverse` must be greater or equal to 1")
-
-    @classmethod
-    def validate_gain(cls, gain: float) -> None:
-        if not isinstance(gain, (int, float)):
-            raise ProcessingParametersException("`gain` must be real")
-        if gain == 0:
-            raise ProcessingParametersException("`gain` must not be zero")
-
-    @classmethod
-    def validate_clip(cls, clip: float) -> None:
-        if not isinstance(clip, (int, float)):
-            raise ProcessingParametersException("`clip` must be real")
-        if clip <= 0:
-            raise ProcessingParametersException("`clip` must be positive")
-
-    def validate_and_parse_traces_per_gather(self, traces_per_gather: int) -> int:
-        self.validate_traces_per_gather(traces_per_gather)
-        ntr = self.sgy.shape[1]
-        return min(ntr, traces_per_gather)
-
-    def validate_and_parse_maximum_time(self, maximum_time: float) -> float:
-        self.validate_maximum_time(maximum_time)
-        if maximum_time == 0.0:
-            maximum_time = self.sgy.max_time_ms
-        else:
-            index = self.sgy.ms2index(maximum_time)
-            if index == 0:
-                warnings.warn(
-                    "The maximum time is not zero and is less than the duration of one sample, "
-                    "so the maximum time will be equal to the length of the trace."
-                )
-                maximum_time = self.sgy.max_time_ms
-            else:
-                maximum_time = min(maximum_time, self.sgy.max_time_ms)
-        return maximum_time
-
-    def validate_and_parse_traces_to_inverse(self, traces_to_inverse: Sequence[int]) -> Sequence[int]:
-        self.validate_traces_to_inverse(traces_to_inverse)
-        # to python indices
-        traces_to_inverse = [tr - 1 for tr in traces_to_inverse if tr <= self.traces_per_gather_parsed]
-        traces_to_inverse = sorted(set(traces_to_inverse))
-        return traces_to_inverse
-
-    @classmethod
-    def validate_and_parse_gain(cls, gain: float) -> float:
-        cls.validate_gain(gain)
-        return float(gain)
-
-    @classmethod
-    def validate_and_parse_clip(cls, clip: float) -> float:
-        cls.validate_clip(clip)
-        return float(clip)
-
-    def get_gathers_ids(self) -> List[Tuple[int]]:
-        return list(chunk_iterable(list(range(self.sgy.shape[1])), self.traces_per_gather_parsed))  # type: ignore
-
-    @property
-    def num_gathers(self) -> int:
-        return len(self.get_gathers_ids())
-
-    @property
-    def picks_in_ms(self) -> Optional[List[float]]:
-        if self.picks_in_samples is not None:
-            return multiply_iterable_by(self.picks_in_samples, self.sgy.dt_ms)  # type: ignore
-        else:
-            return None
-
-    @property
-    def picks_in_mcs(self) -> Optional[List[int]]:
-        if self.picks_in_samples is not None:
-            return multiply_iterable_by(self.picks_in_samples, self.sgy.dt_mcs, cast_to=int)  # type: ignore
-        else:
-            return None
-
-    def _check_and_convert_picks(self) -> List[float]:  # type: ignore
-        if self.picks_in_samples is None:
-            raise ValueError("There are no picks. Put them manually or process the task first")
-        if isinstance(self.picks_in_samples, (tuple, list)):
-            picks_in_samples = self.picks_in_samples
-        elif isinstance(self.picks_in_samples, np.ndarray):
-            picks_in_samples = self.picks_in_samples.tolist()
-        else:
-            raise TypeError("Only 1D sequence can be saved")
-        return picks_in_samples  # type: ignore
-
-    def _prepare_output_for_nonbinary_export(self) -> Tuple[Dict[str, Any], Dict[str, Any]]:
-        picks_in_samples = self._check_and_convert_picks()
-        picks_in_ms = self.sgy.units_converter.index2ms(picks_in_samples, cast_to=float)
-
-        confidence = self.confidence
-
-        is_source_file = isinstance(self.sgy.source, (str, Path))
-        if is_source_file:
-            source_filename = str(Path(self.sgy.source).name)  # type: ignore
-            source_full_name = str(Path(self.sgy.source).resolve())  # type: ignore
-        else:
-            source_filename = None
-            source_full_name = None
-
-        meta = {
-            "is_source_file": is_source_file,
-            "is_source_ndarray": self.sgy.is_source_ndarray,
-            "filename": source_filename,
-            "full_name": source_full_name,
-            "hash": self.sgy.get_hash(),
-            "dt_ms": self.sgy.dt_ms,
-            "is_picked_with_model": bool(self.success),
-            "model_hash": self.model_hash,
-            "traces_per_gather": self.traces_per_gather_parsed,
-            "maximum_time": self.maximum_time_parsed,
-            "traces_to_inverse": self.traces_to_inverse_parsed,
-            "gain": self.gain_parsed,
-            "clip": self.clip_parsed,
-        }
-        data = {
-            "trace": list(range(1, len(picks_in_samples) + 1)),
-            "picks_in_samples": picks_in_samples,
-            "picks_in_ms": picks_in_ms,
-            "confidence": confidence,
-        }
-        return meta, data
-
-    def export_result_as_sgy(
-        self,
-        filename: Union[str, Path],
-        byte_position: int = 236,
-        encoding: str = "I",
-        picks_unit: str = "mcs",
-    ) -> None:
-        picks_in_samples = self._check_and_convert_picks()
-        self.sgy.export_sgy_with_picks(
-            output_fname=filename,
-            picks_in_samples=picks_in_samples,
-            encoding=encoding,
-            byte_position=byte_position,
-            picks_unit=picks_unit,
-        )
-
-    def export_result_as_json(self, filename: Union[str, Path]) -> None:
-        meta, data = self._prepare_output_for_nonbinary_export()
-        Path(filename).parent.mkdir(parents=True, exist_ok=True)
-        with open(filename, "w") as fout:
-            json.dump({**meta, **data}, fout)
-
-    def export_result_as_txt(self, filename: Union[str, Path]) -> None:
-        meta, data = self._prepare_output_for_nonbinary_export()
-        Path(filename).parent.mkdir(parents=True, exist_ok=True)
-        with open(filename, "w") as fout:
-            content = [f"{k}={v}" for k, v in meta.items()]
-            data_str = pd.DataFrame(data).to_string(index=False, justify="right")
-            content.append(data_str)
-            content = "\n".join(content)
-            fout.write(content)
+import json
+import warnings
+from pathlib import Path
+from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
+
+import numpy as np
+import pandas as pd
+
+from first_breaks.sgy.reader import SGY
+from first_breaks.utils.utils import chunk_iterable, multiply_iterable_by
+
+MINIMUM_TRACES_PER_GATHER = 2
+
+
+class ProcessingParametersException(Exception):
+    pass
+
+
+class Task:
+    def __init__(
+        self,
+        sgy: Union[SGY, str, Path, bytes],
+        traces_per_gather: int = 24,
+        maximum_time: float = 0.0,
+        traces_to_inverse: Sequence[int] = (),
+        gain: float = 1,
+        clip: float = 1,
+    ) -> None:
+        self.sgy = sgy if isinstance(sgy, SGY) else SGY(sgy)
+
+        self.traces_per_gather = traces_per_gather
+        self.maximum_time = maximum_time
+        self.traces_to_inverse = traces_to_inverse
+        self.gain = gain
+        self.clip = clip
+
+        self.traces_per_gather_parsed = self.validate_and_parse_traces_per_gather(traces_per_gather)
+        self.maximum_time_parsed = self.validate_and_parse_maximum_time(maximum_time)
+        self.maximum_time_sample = self.sgy.ms2index(self.maximum_time_parsed)
+        self.traces_to_inverse_parsed = self.validate_and_parse_traces_to_inverse(traces_to_inverse)
+        self.gain_parsed = self.validate_and_parse_gain(gain)
+        self.clip_parsed = self.validate_and_parse_clip(clip)
+
+        self.picks_in_samples: Optional[Union[Sequence[float], np.ndarray]] = None
+        self.confidence: Optional[Union[Sequence[float], np.ndarray]] = None
+        self.success: Optional[bool] = None
+        self.error_message: Optional[str] = None
+        self.model_hash: Optional[str] = None
+
+    @classmethod
+    def validate_traces_per_gather(cls, traces_per_gather: int) -> None:
+        if not isinstance(traces_per_gather, int):
+            raise ProcessingParametersException("`traces_per_gather` must be integer")
+        if traces_per_gather < MINIMUM_TRACES_PER_GATHER:
+            raise ProcessingParametersException(
+                f"`traces_per_gather` must be greater or " f"equal to {MINIMUM_TRACES_PER_GATHER}"
+            )
+
+    @classmethod
+    def validate_maximum_time(cls, maximum_time: float) -> None:
+        if not isinstance(maximum_time, (int, float)):
+            raise ProcessingParametersException("`maximum_time` must be real")
+
+        if maximum_time < 0.0:
+            raise ProcessingParametersException("`maximum_time` must be positive or equal to 0")
+
+    @classmethod
+    def validate_traces_to_inverse(cls, traces_to_inverse: Sequence[int]) -> None:
+        if not isinstance(traces_to_inverse, (tuple, list)):
+            raise ProcessingParametersException("`traces_to_inverse` must be tuple or list")
+
+        if not all(isinstance(val, int) for val in traces_to_inverse):
+            raise ProcessingParametersException("Elements of `traces_to_inverse` must be int")
+
+        if not all(val >= 1 for val in traces_to_inverse):
+            raise ProcessingParametersException("Elements of `traces_to_inverse` must be greater or equal to 1")
+
+    @classmethod
+    def validate_gain(cls, gain: float) -> None:
+        if not isinstance(gain, (int, float)):
+            raise ProcessingParametersException("`gain` must be real")
+        if gain == 0:
+            raise ProcessingParametersException("`gain` must not be zero")
+
+    @classmethod
+    def validate_clip(cls, clip: float) -> None:
+        if not isinstance(clip, (int, float)):
+            raise ProcessingParametersException("`clip` must be real")
+        if clip <= 0:
+            raise ProcessingParametersException("`clip` must be positive")
+
+    def validate_and_parse_traces_per_gather(self, traces_per_gather: int) -> int:
+        self.validate_traces_per_gather(traces_per_gather)
+        ntr = self.sgy.shape[1]
+        return min(ntr, traces_per_gather)
+
+    def validate_and_parse_maximum_time(self, maximum_time: float) -> float:
+        self.validate_maximum_time(maximum_time)
+        if maximum_time == 0.0:
+            maximum_time = self.sgy.max_time_ms
+        else:
+            index = self.sgy.ms2index(maximum_time)
+            if index == 0:
+                warnings.warn(
+                    "The maximum time is not zero and is less than the duration of one sample, "
+                    "so the maximum time will be equal to the length of the trace."
+                )
+                maximum_time = self.sgy.max_time_ms
+            else:
+                maximum_time = min(maximum_time, self.sgy.max_time_ms)
+        return maximum_time
+
+    def validate_and_parse_traces_to_inverse(self, traces_to_inverse: Sequence[int]) -> Sequence[int]:
+        self.validate_traces_to_inverse(traces_to_inverse)
+        # to python indices
+        traces_to_inverse = [tr - 1 for tr in traces_to_inverse if tr <= self.traces_per_gather_parsed]
+        traces_to_inverse = sorted(set(traces_to_inverse))
+        return traces_to_inverse
+
+    @classmethod
+    def validate_and_parse_gain(cls, gain: float) -> float:
+        cls.validate_gain(gain)
+        return float(gain)
+
+    @classmethod
+    def validate_and_parse_clip(cls, clip: float) -> float:
+        cls.validate_clip(clip)
+        return float(clip)
+
+    def get_gathers_ids(self) -> List[Tuple[int]]:
+        return list(chunk_iterable(list(range(self.sgy.shape[1])), self.traces_per_gather_parsed))  # type: ignore
+
+    @property
+    def num_gathers(self) -> int:
+        return len(self.get_gathers_ids())
+
+    @property
+    def picks_in_ms(self) -> Optional[List[float]]:
+        if self.picks_in_samples is not None:
+            return multiply_iterable_by(self.picks_in_samples, self.sgy.dt_ms)  # type: ignore
+        else:
+            return None
+
+    @property
+    def picks_in_mcs(self) -> Optional[List[int]]:
+        if self.picks_in_samples is not None:
+            return multiply_iterable_by(self.picks_in_samples, self.sgy.dt_mcs, cast_to=int)  # type: ignore
+        else:
+            return None
+
+    def _check_and_convert_picks(self) -> List[float]:  # type: ignore
+        if self.picks_in_samples is None:
+            raise ValueError("There are no picks. Put them manually or process the task first")
+        if isinstance(self.picks_in_samples, (tuple, list)):
+            picks_in_samples = self.picks_in_samples
+        elif isinstance(self.picks_in_samples, np.ndarray):
+            picks_in_samples = self.picks_in_samples.tolist()
+        else:
+            raise TypeError("Only 1D sequence can be saved")
+        return picks_in_samples  # type: ignore
+
+    def _prepare_output_for_nonbinary_export(self) -> Tuple[Dict[str, Any], Dict[str, Any]]:
+        picks_in_samples = self._check_and_convert_picks()
+        picks_in_ms = self.sgy.units_converter.index2ms(picks_in_samples, cast_to=float)
+
+        confidence = self.confidence
+
+        is_source_file = isinstance(self.sgy.source, (str, Path))
+        if is_source_file:
+            source_filename = str(Path(self.sgy.source).name)  # type: ignore
+            source_full_name = str(Path(self.sgy.source).resolve())  # type: ignore
+        else:
+            source_filename = None
+            source_full_name = None
+
+        meta = {
+            "is_source_file": is_source_file,
+            "is_source_ndarray": self.sgy.is_source_ndarray,
+            "filename": source_filename,
+            "full_name": source_full_name,
+            "hash": self.sgy.get_hash(),
+            "dt_ms": self.sgy.dt_ms,
+            "is_picked_with_model": bool(self.success),
+            "model_hash": self.model_hash,
+            "traces_per_gather": self.traces_per_gather_parsed,
+            "maximum_time": self.maximum_time_parsed,
+            "traces_to_inverse": self.traces_to_inverse_parsed,
+            "gain": self.gain_parsed,
+            "clip": self.clip_parsed,
+        }
+        data = {
+            "trace": list(range(1, len(picks_in_samples) + 1)),
+            "picks_in_samples": picks_in_samples,
+            "picks_in_ms": picks_in_ms,
+            "confidence": confidence,
+        }
+        return meta, data
+
+    def export_result_as_sgy(
+        self,
+        filename: Union[str, Path],
+        byte_position: int = 236,
+        encoding: str = "I",
+        picks_unit: str = "mcs",
+    ) -> None:
+        picks_in_samples = self._check_and_convert_picks()
+        self.sgy.export_sgy_with_picks(
+            output_fname=filename,
+            picks_in_samples=picks_in_samples,
+            encoding=encoding,
+            byte_position=byte_position,
+            picks_unit=picks_unit,
+        )
+
+    def export_result_as_json(self, filename: Union[str, Path]) -> None:
+        meta, data = self._prepare_output_for_nonbinary_export()
+        Path(filename).parent.mkdir(parents=True, exist_ok=True)
+        with open(filename, "w") as fout:
+            json.dump({**meta, **data}, fout)
+
+    def export_result_as_txt(self, filename: Union[str, Path]) -> None:
+        meta, data = self._prepare_output_for_nonbinary_export()
+        Path(filename).parent.mkdir(parents=True, exist_ok=True)
+        with open(filename, "w") as fout:
+            content = [f"{k}={v}" for k, v in meta.items()]
+            data_str = pd.DataFrame(data).to_string(index=False, justify="right")
+            content.append(data_str)
+            content = "\n".join(content)
+            fout.write(content)
```

### Comparing `first-breaks-picking-0.3.0b0/first_breaks/sgy/headers.py` & `first-breaks-picking-0.4.0a0/first_breaks/sgy/headers.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,244 +1,244 @@
-from typing import Dict, List, Tuple
-
-
-class InvalidHeaders(Exception):
-    pass
-
-
-THeadersAttr = List[Tuple[int, str, str]]
-
-
-class Headers:
-    # headers in format [(offset_1, header_name_1, format_1), (offset_2, header_name_2, format_2), ...]
-    # offset started from 0
-    headers_schema: THeadersAttr
-    format2size: Dict[str, int] = {
-        "c": 1,
-        "b": 1,
-        "B": 1,
-        "?": 1,
-        "h": 2,
-        "H": 2,
-        "i": 4,
-        "I": 4,
-        "l": 4,
-        "L": 4,
-        "q": 8,
-        "Q": 8,
-        "f": 4,
-        "d": 8,
-        "s": 1,
-    }
-
-    def get_num_bytes(self, fmt: str) -> int:
-        tp = fmt[-1]
-        if tp not in self.format2size:
-            raise InvalidHeaders("Format is not interpretable")
-        num = fmt[:-1]
-        if num.isdigit():
-            num = int(num)  # type: ignore
-        else:
-            num = 1  # type: ignore
-        return self.format2size[tp] * num  # type: ignore
-
-    def validate(self) -> None:
-        headers_names = [header_info[1] for header_info in self.headers_schema]
-        if not all(isinstance(name, str) for name in headers_names):
-            raise InvalidHeaders("Header names must be strings")
-        if not len(set(headers_names)) == len(headers_names):
-            raise InvalidHeaders("Header names must be unique")
-        available_formats = self.format2size.keys()
-        if not all(header_info[2][-1] in available_formats for header_info in self.headers_schema):
-            raise InvalidHeaders("Some of headers have unavailable formats")
-
-    def fill_offsets_if_empty(self) -> THeadersAttr:
-        offsets_is_none = [header_info[0] is None for header_info in self.headers_schema]
-        if all(offsets_is_none):
-            upd_headers = []
-            offset = 0
-            for header in self.headers_schema:
-                upd_header = (offset, header[1], header[2])
-                upd_headers.append(upd_header)
-                offset += self.get_num_bytes(header[2])
-            return upd_headers
-        elif any(offsets_is_none) and not all(offsets_is_none):
-            raise InvalidHeaders("To fill offsets, they must all be either empty or filled (no modification)")
-        return self.headers_schema
-
-
-class FileHeaders(Headers):
-    dt_name = "dt"
-    dt_name_orig = "dt_orig"
-    ns_name = "ns"
-    ns_name_orig = "ns_orig"
-    data_sample_format_name = "data_sample_format"
-
-    def __init__(self) -> None:
-        self.headers_schema = [
-            (0, "textual_file_header", "3200s"),
-            (3200, "job", "i"),
-            (3204, "line", "i"),
-            (3208, "reel", "i"),
-            (3212, "data_trace_per_ensemble", "H"),
-            (3214, "auxiliary_trace_per_ensemble", "H"),
-            (3216, self.dt_name, "H"),
-            (3218, self.dt_name_orig, "H"),
-            (3220, self.ns_name, "H"),
-            (3222, self.ns_name_orig, "H"),
-            (3224, self.data_sample_format_name, "H"),
-            (3226, "ensemble_fold", "H"),
-            (3228, "trace_sorting", "h"),
-            (3230, "vertical_sum_code", "H"),
-            (3232, "sweep_frequency_start", "H"),
-            (3234, "sweep_frequency_end", "H"),
-            (3236, "sweep_length", "H"),
-            (3238, "sweep_type", "h"),
-            (3240, "sweep_channel", "h"),
-            (3242, "sweep_taper_length_start", "H"),
-            (3244, "sweep_taper_length_end", "H"),
-            (3246, "taper_type", "H"),
-            (3248, "correlated_data_traces", "H"),
-            (3250, "binary_gain", "H"),
-            (3252, "amplitude_recovery_method", "H"),
-            (3254, "measurement_system", "H"),
-            (3256, "impulse_signal_polarity", "H"),
-            (3258, "vibratory_polarity_code", "H"),
-            (3260, "unassigned1", "240s"),
-            (3500, "segy_format_revision_number", "H"),
-            (3502, "fixed_length_trace_flag", "H"),
-            (3504, "number_of_textual_headers", "H"),
-            (3506, "unassigned2", "94s"),
-        ]
-        self.validate()
-
-
-class TraceHeaders(Headers):
-    fb_pick_default = "FB_PICK"
-
-    def __init__(self) -> None:
-        self.headers_schema = [
-            (0, "TRACENO", "i"),
-            (4, "trace_sequence_file", "i"),
-            (8, "FFID", "i"),
-            (12, "CHAN", "i"),
-            (16, "SOURCE", "i"),
-            (20, "CDP", "i"),
-            (24, "SEQNO", "i"),
-            (28, "TRC_TYPE", "h"),
-            (30, "STACKNT", "h"),
-            (32, "TRFOLD", "h"),
-            (34, "data_use", "h"),
-            (36, "OFFSET", "i"),
-            (40, "REC_ELEV", "i"),
-            (44, "SOU_ELEV", "i"),
-            (48, "DEPTH", "i"),
-            (52, "REC_DATUM", "i"),
-            (56, "SOU_DATUM", "i"),
-            (60, "SOU_H2OD", "i"),
-            (64, "REC_H2OD", "i"),
-            (68, "elevation_scalar", "h"),
-            (70, "source_group_scalar", "h"),
-            (72, "SOU_X", "i"),
-            (76, "SOU_Y", "i"),
-            (80, "REC_X", "i"),
-            (84, "REC_Y", "i"),
-            (88, "coordinate_units", "h"),
-            (90, "weathering_velocity", "h"),
-            (92, "subweathering_velocity", "h"),
-            (94, "UPHOLE", "h"),
-            (96, "REC_UPHOLE", "h"),
-            (98, "SOU_STAT", "h"),
-            (100, "REC_STAT", "h"),
-            (102, "TOT_STAT", "h"),
-            (104, "lag_time_a", "h"),
-            (106, "lag_time_b", "h"),
-            (108, "delay_recording_time", "h"),
-            (110, "TLIVE_S", "h"),
-            (112, "TFULL_S", "h"),
-            (114, "NUMSMP", "H"),
-            (116, "DT", "H"),
-            (118, "IGAIN", "h"),
-            (120, "PREAMP", "h"),
-            (122, "EARLYG", "h"),
-            (124, "COR_FLAG", "h"),
-            (126, "SWEEPFREQSTART", "h"),
-            (128, "SWEEPFREQEND", "h"),
-            (130, "SWEEPLEN", "h"),
-            (132, "SWEEPTYPE", "h"),
-            (134, "SWEEPTAPSTART", "h"),
-            (136, "SWEEPTAPEND", "h"),
-            (138, "SWEEPTAPCODE", "h"),
-            (140, "AAXFILT", "h"),
-            (142, "AAXSLOP", "h"),
-            (144, "FREQXN", "h"),
-            (146, "FXNSLOP", "h"),
-            (148, "FREQXL", "h"),
-            (150, "FREQXH", "h"),
-            (152, "FXLSLOP", "h"),
-            (154, "FXHSLOP", "h"),
-            (156, "YEAR", "h"),
-            (158, "DAY", "h"),
-            (160, "HOUR", "h"),
-            (162, "MINUTE", "h"),
-            (164, "SECOND", "h"),
-            (166, "time_basic_code", "h"),
-            (168, "trace_weighting_factor", "h"),
-            (170, "geophone_group_number_roll1", "h"),
-            (172, "geophone_group_number_first", "h"),
-            (174, "geophone_group_number_last", "h"),
-            (176, "gap_size", "h"),
-            (178, "over_travel", "h"),
-            (180, "CDP_X", "i"),
-            (184, "CDP_Y", "i"),
-            (188, "ILINE_NO", "i"),
-            (192, "XLINE_NO", "i"),
-            (196, "shot_point", "i"),
-            (200, "shot_point_scalar", "h"),
-            (202, "trace_value_measurement", "h"),
-            (204, "transduction_constant_mantissa", "i"),
-            (208, "transduction_constant_power", "h"),
-            (210, "transduction_unit", "h"),
-            (212, "trace_identifier", "h"),
-            (214, "scalar_trace_header", "h"),
-            (216, "source_type", "h"),
-            (218, "source_energy_direction_mantissa", "i"),
-            (222, "source_energy_direction_exponent", "H"),
-            (224, "source_measurement_mantissa", "i"),
-            (228, "source_measurement_exponent", "H"),
-            (230, "source_measurement_unit", "h"),
-            (232, "unassigned1", "i"),
-            (236, self.fb_pick_default, "I"),
-        ]
-        self.validate()
-        self.scalar_from2apply = {
-            "elevation_scalar": [
-                "REC_ELEV",
-                "SOU_ELEV",
-                "DEPTH",
-                "REC_DATUM",
-                "SOU_DATUM",
-                "SOU_H2OD",
-                "REC_H2OD",
-            ],
-            "source_group_scalar": [
-                "SOU_X",
-                "SOU_Y",
-                "REC_X",
-                "REC_Y",
-            ],
-            "shot_point_scalar": [
-                "shot_point",
-            ],
-            "scalar_trace_header": [
-                "UPHOLE",
-                "REC_UPHOLE",
-                "SOU_STAT",
-                "REC_STAT",
-                "TOT_STAT",
-                "lag_time_a",
-                "lag_time_b",
-                "delay_recording_time",
-                "TLIVE_S",
-                "TFULL_S",
-            ],
-        }
+from typing import Dict, List, Tuple
+
+
+class InvalidHeaders(Exception):
+    pass
+
+
+THeadersAttr = List[Tuple[int, str, str]]
+
+
+class Headers:
+    # headers in format [(offset_1, header_name_1, format_1), (offset_2, header_name_2, format_2), ...]
+    # offset started from 0
+    headers_schema: THeadersAttr
+    format2size: Dict[str, int] = {
+        "c": 1,
+        "b": 1,
+        "B": 1,
+        "?": 1,
+        "h": 2,
+        "H": 2,
+        "i": 4,
+        "I": 4,
+        "l": 4,
+        "L": 4,
+        "q": 8,
+        "Q": 8,
+        "f": 4,
+        "d": 8,
+        "s": 1,
+    }
+
+    def get_num_bytes(self, fmt: str) -> int:
+        tp = fmt[-1]
+        if tp not in self.format2size:
+            raise InvalidHeaders("Format is not interpretable")
+        num = fmt[:-1]
+        if num.isdigit():
+            num = int(num)  # type: ignore
+        else:
+            num = 1  # type: ignore
+        return self.format2size[tp] * num  # type: ignore
+
+    def validate(self) -> None:
+        headers_names = [header_info[1] for header_info in self.headers_schema]
+        if not all(isinstance(name, str) for name in headers_names):
+            raise InvalidHeaders("Header names must be strings")
+        if not len(set(headers_names)) == len(headers_names):
+            raise InvalidHeaders("Header names must be unique")
+        available_formats = self.format2size.keys()
+        if not all(header_info[2][-1] in available_formats for header_info in self.headers_schema):
+            raise InvalidHeaders("Some of headers have unavailable formats")
+
+    def fill_offsets_if_empty(self) -> THeadersAttr:
+        offsets_is_none = [header_info[0] is None for header_info in self.headers_schema]
+        if all(offsets_is_none):
+            upd_headers = []
+            offset = 0
+            for header in self.headers_schema:
+                upd_header = (offset, header[1], header[2])
+                upd_headers.append(upd_header)
+                offset += self.get_num_bytes(header[2])
+            return upd_headers
+        elif any(offsets_is_none) and not all(offsets_is_none):
+            raise InvalidHeaders("To fill offsets, they must all be either empty or filled (no modification)")
+        return self.headers_schema
+
+
+class FileHeaders(Headers):
+    dt_name = "dt"
+    dt_name_orig = "dt_orig"
+    ns_name = "ns"
+    ns_name_orig = "ns_orig"
+    data_sample_format_name = "data_sample_format"
+
+    def __init__(self) -> None:
+        self.headers_schema = [
+            (0, "textual_file_header", "3200s"),
+            (3200, "job", "i"),
+            (3204, "line", "i"),
+            (3208, "reel", "i"),
+            (3212, "data_trace_per_ensemble", "H"),
+            (3214, "auxiliary_trace_per_ensemble", "H"),
+            (3216, self.dt_name, "H"),
+            (3218, self.dt_name_orig, "H"),
+            (3220, self.ns_name, "H"),
+            (3222, self.ns_name_orig, "H"),
+            (3224, self.data_sample_format_name, "H"),
+            (3226, "ensemble_fold", "H"),
+            (3228, "trace_sorting", "h"),
+            (3230, "vertical_sum_code", "H"),
+            (3232, "sweep_frequency_start", "H"),
+            (3234, "sweep_frequency_end", "H"),
+            (3236, "sweep_length", "H"),
+            (3238, "sweep_type", "h"),
+            (3240, "sweep_channel", "h"),
+            (3242, "sweep_taper_length_start", "H"),
+            (3244, "sweep_taper_length_end", "H"),
+            (3246, "taper_type", "H"),
+            (3248, "correlated_data_traces", "H"),
+            (3250, "binary_gain", "H"),
+            (3252, "amplitude_recovery_method", "H"),
+            (3254, "measurement_system", "H"),
+            (3256, "impulse_signal_polarity", "H"),
+            (3258, "vibratory_polarity_code", "H"),
+            (3260, "unassigned1", "240s"),
+            (3500, "segy_format_revision_number", "H"),
+            (3502, "fixed_length_trace_flag", "H"),
+            (3504, "number_of_textual_headers", "H"),
+            (3506, "unassigned2", "94s"),
+        ]
+        self.validate()
+
+
+class TraceHeaders(Headers):
+    fb_pick_default = "FB_PICK"
+
+    def __init__(self) -> None:
+        self.headers_schema = [
+            (0, "TRACENO", "i"),
+            (4, "trace_sequence_file", "i"),
+            (8, "FFID", "i"),
+            (12, "CHAN", "i"),
+            (16, "SOURCE", "i"),
+            (20, "CDP", "i"),
+            (24, "SEQNO", "i"),
+            (28, "TRC_TYPE", "h"),
+            (30, "STACKNT", "h"),
+            (32, "TRFOLD", "h"),
+            (34, "data_use", "h"),
+            (36, "OFFSET", "i"),
+            (40, "REC_ELEV", "i"),
+            (44, "SOU_ELEV", "i"),
+            (48, "DEPTH", "i"),
+            (52, "REC_DATUM", "i"),
+            (56, "SOU_DATUM", "i"),
+            (60, "SOU_H2OD", "i"),
+            (64, "REC_H2OD", "i"),
+            (68, "elevation_scalar", "h"),
+            (70, "source_group_scalar", "h"),
+            (72, "SOU_X", "i"),
+            (76, "SOU_Y", "i"),
+            (80, "REC_X", "i"),
+            (84, "REC_Y", "i"),
+            (88, "coordinate_units", "h"),
+            (90, "weathering_velocity", "h"),
+            (92, "subweathering_velocity", "h"),
+            (94, "UPHOLE", "h"),
+            (96, "REC_UPHOLE", "h"),
+            (98, "SOU_STAT", "h"),
+            (100, "REC_STAT", "h"),
+            (102, "TOT_STAT", "h"),
+            (104, "lag_time_a", "h"),
+            (106, "lag_time_b", "h"),
+            (108, "delay_recording_time", "h"),
+            (110, "TLIVE_S", "h"),
+            (112, "TFULL_S", "h"),
+            (114, "NUMSMP", "H"),
+            (116, "DT", "H"),
+            (118, "IGAIN", "h"),
+            (120, "PREAMP", "h"),
+            (122, "EARLYG", "h"),
+            (124, "COR_FLAG", "h"),
+            (126, "SWEEPFREQSTART", "h"),
+            (128, "SWEEPFREQEND", "h"),
+            (130, "SWEEPLEN", "h"),
+            (132, "SWEEPTYPE", "h"),
+            (134, "SWEEPTAPSTART", "h"),
+            (136, "SWEEPTAPEND", "h"),
+            (138, "SWEEPTAPCODE", "h"),
+            (140, "AAXFILT", "h"),
+            (142, "AAXSLOP", "h"),
+            (144, "FREQXN", "h"),
+            (146, "FXNSLOP", "h"),
+            (148, "FREQXL", "h"),
+            (150, "FREQXH", "h"),
+            (152, "FXLSLOP", "h"),
+            (154, "FXHSLOP", "h"),
+            (156, "YEAR", "h"),
+            (158, "DAY", "h"),
+            (160, "HOUR", "h"),
+            (162, "MINUTE", "h"),
+            (164, "SECOND", "h"),
+            (166, "time_basic_code", "h"),
+            (168, "trace_weighting_factor", "h"),
+            (170, "geophone_group_number_roll1", "h"),
+            (172, "geophone_group_number_first", "h"),
+            (174, "geophone_group_number_last", "h"),
+            (176, "gap_size", "h"),
+            (178, "over_travel", "h"),
+            (180, "CDP_X", "i"),
+            (184, "CDP_Y", "i"),
+            (188, "ILINE_NO", "i"),
+            (192, "XLINE_NO", "i"),
+            (196, "shot_point", "i"),
+            (200, "shot_point_scalar", "h"),
+            (202, "trace_value_measurement", "h"),
+            (204, "transduction_constant_mantissa", "i"),
+            (208, "transduction_constant_power", "h"),
+            (210, "transduction_unit", "h"),
+            (212, "trace_identifier", "h"),
+            (214, "scalar_trace_header", "h"),
+            (216, "source_type", "h"),
+            (218, "source_energy_direction_mantissa", "i"),
+            (222, "source_energy_direction_exponent", "H"),
+            (224, "source_measurement_mantissa", "i"),
+            (228, "source_measurement_exponent", "H"),
+            (230, "source_measurement_unit", "h"),
+            (232, "unassigned1", "i"),
+            (236, self.fb_pick_default, "I"),
+        ]
+        self.validate()
+        self.scalar_from2apply = {
+            "elevation_scalar": [
+                "REC_ELEV",
+                "SOU_ELEV",
+                "DEPTH",
+                "REC_DATUM",
+                "SOU_DATUM",
+                "SOU_H2OD",
+                "REC_H2OD",
+            ],
+            "source_group_scalar": [
+                "SOU_X",
+                "SOU_Y",
+                "REC_X",
+                "REC_Y",
+            ],
+            "shot_point_scalar": [
+                "shot_point",
+            ],
+            "scalar_trace_header": [
+                "UPHOLE",
+                "REC_UPHOLE",
+                "SOU_STAT",
+                "REC_STAT",
+                "TOT_STAT",
+                "lag_time_a",
+                "lag_time_b",
+                "delay_recording_time",
+                "TLIVE_S",
+                "TFULL_S",
+            ],
+        }
```

### Comparing `first-breaks-picking-0.3.0b0/first_breaks/utils/debug.py` & `first-breaks-picking-0.4.0a0/first_breaks/utils/debug.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.3.0b0/first_breaks/utils/utils.py` & `first-breaks-picking-0.4.0a0/first_breaks/utils/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,161 +1,150 @@
-import hashlib
-import inspect
-import io
-from itertools import islice
-from pathlib import Path
-from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
-
-import numpy as np
-import onnxruntime as ort
-import requests
-
-from first_breaks.const import (
-    DEMO_SGY_HASH,
-    DEMO_SGY_PATH,
-    DEMO_SGY_URL,
-    MODEL_ONNX_HASH,
-    MODEL_ONNX_PATH,
-    MODEL_ONNX_URL,
-    TIMEOUT,
-)
-
-TScalar = Union[int, float, np.number]
-TTimeType = Union[TScalar, List[TScalar], Tuple[TScalar, ...], np.ndarray]
-
-
-class InvalidHash(Exception):
-    pass
-
-
-def chunk_iterable(it: Iterable[Any], size: int) -> List[Tuple[Any, ...]]:
-    it = iter(it)
-    return list(iter(lambda: tuple(islice(it, size)), ()))
-
-
-def get_io(source: Union[Path, str, bytes], mode: str = "r") -> Union[io.BytesIO, io.FileIO]:
-    if isinstance(source, (Path, str)):
-        source = Path(source).resolve()
-        if "r" in mode:
-            if not source.exists():
-                raise FileNotFoundError("There is no file: ", str(source))
-        descriptor = io.FileIO(str(source), mode=mode)
-    elif isinstance(source, bytes):
-        descriptor = io.BytesIO(source)  # type: ignore
-    else:
-        raise TypeError("Not supported type")
-    return descriptor
-
-
-def calc_hash(source: Union[Path, str, bytes, io.BytesIO, io.FileIO]) -> str:
-    hash_md5 = hashlib.md5()
-    if not isinstance(source, (io.BytesIO, io.FileIO)):
-        source = get_io(source, mode="rb")
-    for chunk in iter(lambda: source.read(4096), b""):  # type: ignore
-        hash_md5.update(chunk)
-    return hash_md5.hexdigest()
-
-
-def download_by_url(url: str, fname: Optional[Union[str, Path]], timeout: float = TIMEOUT) -> Optional[bytes]:
-    response = requests.get(url, timeout=timeout)
-    if response.status_code != 200:
-        response.raise_for_status()
-        return None
-    else:
-        if fname:
-            Path(fname).parent.mkdir(exist_ok=True, parents=True)
-            with open(fname, "wb+") as f:
-                f.write(response.content)
-        return response.content
-
-
-def download_and_validate_file(
-    fname: Union[str, Path], url: str, md5: str, timeout: float = TIMEOUT
-) -> Union[str, Path]:
-    if not (Path(fname).exists() and calc_hash(fname) == md5):
-        download_by_url(url=url, fname=fname, timeout=timeout)
-    md5_last = calc_hash(fname)
-    if md5_last != md5:
-        raise InvalidHash(f"Hash for file {Path(fname).resolve()} in invalid. Got {md5_last}, expected {md5}")
-    return fname
-
-
-def download_demo_sgy(
-    fname: Union[str, Path] = DEMO_SGY_PATH, url: str = DEMO_SGY_URL, md5: str = DEMO_SGY_HASH
-) -> Union[str, Path]:
-    return download_and_validate_file(fname=fname, url=url, md5=md5)
-
-
-def download_model_onnx(
-    fname: Union[str, Path] = MODEL_ONNX_PATH, url: str = MODEL_ONNX_URL, md5: str = MODEL_ONNX_HASH
-) -> Union[str, Path]:
-    return download_and_validate_file(fname=fname, url=url, md5=md5)
-
-
-def multiply_iterable_by(sample: TTimeType, multiplier: float, cast_to: Optional[Any] = None) -> TTimeType:
-    if isinstance(sample, (int, float, str)):
-        result = sample * multiplier  # type: ignore
-        return cast_to(result) if cast_to is not None else result
-    elif isinstance(sample, (np.number, np.ndarray)):
-        result = sample * multiplier
-        return result.astype(cast_to) if cast_to is not None else result
-    elif isinstance(sample, list):
-        return list(multiply_iterable_by(val, multiplier, cast_to) for val in sample)
-    elif isinstance(sample, tuple):
-        return tuple(multiply_iterable_by(val, multiplier, cast_to) for val in sample)
-    else:
-        raise TypeError("Invalid type for samples")
-
-
-class UnitsConverter:
-    def __init__(
-        self,
-        *args: Any,
-        sgy_mcs: Optional[Union[int, float]] = None,
-        sgy_ms: Optional[Union[int, float]] = None,
-    ):
-        if args:
-            raise ValueError("Specify explicitly either `sgy_mcs`or `sgy_ms` as keyword argument")
-        if (sgy_mcs is None and sgy_ms is None) or (sgy_mcs is not None and sgy_ms is not None):
-            raise RuntimeError("One and only one of `sgy_mcs` or `sgy_ms` must be specified")
-        elif sgy_mcs is not None:
-            self.sgy_mcs = sgy_mcs
-            self.sgy_ms = self.mcs2ms(sgy_mcs)  # type: ignore
-        elif sgy_ms is not None:
-            self.sgy_mcs = self.ms2mcs(sgy_ms)  # type: ignore
-            self.sgy_ms = sgy_ms
-        else:
-            raise RuntimeError("Init error")
-
-    @staticmethod
-    def ms2mcs(sample: TTimeType, cast_to: Any = int) -> TTimeType:
-        return multiply_iterable_by(sample, 1000, cast_to)
-
-    @staticmethod
-    def mcs2ms(sample: TTimeType, cast_to: Any = float) -> TTimeType:
-        return multiply_iterable_by(sample, 0.001, cast_to)
-
-    def ms2index(self, sample: TTimeType, cast_to: Any = int) -> TTimeType:
-        return multiply_iterable_by(sample, 1 / self.sgy_ms, cast_to)  # type: ignore
-
-    def mcs2index(self, sample: TTimeType, cast_to: Any = int) -> TTimeType:
-        return multiply_iterable_by(sample, 1 / self.sgy_mcs, cast_to)
-
-    def index2ms(self, sample: TTimeType, cast_to: Any = float) -> TTimeType:
-        return multiply_iterable_by(sample, self.sgy_ms, cast_to)  # type: ignore
-
-    def index2mcs(self, sample: TTimeType, cast_to: Any = int) -> TTimeType:
-        return multiply_iterable_by(sample, self.sgy_mcs, cast_to)
-
-
-def remove_unused_kwargs(kwargs: Dict[str, Any], constructor: Any) -> Dict[str, Any]:
-    return {k: v for k, v in kwargs.items() if k in inspect.signature(constructor).parameters}
-
-
-ONNX_DEVICE2PROVIDER = {"cuda": "CUDAExecutionProvider", "cpu": "CPUExecutionProvider"}
-
-
-def is_onnx_cuda_available() -> bool:
-    try:
-        return ONNX_DEVICE2PROVIDER["cuda"] in ort.get_available_providers()
-    except Exception:
-        return False
+import hashlib
+import inspect
+import io
+from itertools import islice
+from pathlib import Path
+from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
+
+import numpy as np
+import requests
+
+from first_breaks.const import (
+    DEMO_SGY_HASH,
+    DEMO_SGY_PATH,
+    DEMO_SGY_URL,
+    MODEL_ONNX_HASH,
+    MODEL_ONNX_PATH,
+    MODEL_ONNX_URL,
+    TIMEOUT,
+)
+
+TScalar = Union[int, float, np.number]
+TTimeType = Union[TScalar, List[TScalar], Tuple[TScalar, ...], np.ndarray]
+
+
+class InvalidHash(Exception):
+    pass
+
+
+def chunk_iterable(it: Iterable[Any], size: int) -> List[Tuple[Any, ...]]:
+    it = iter(it)
+    return list(iter(lambda: tuple(islice(it, size)), ()))
+
+
+def get_io(source: Union[Path, str, bytes], mode: str = "r") -> Union[io.BytesIO, io.FileIO]:
+    if isinstance(source, (Path, str)):
+        source = Path(source).resolve()
+        if "r" in mode:
+            if not source.exists():
+                raise FileNotFoundError("There is no file: ", str(source))
+        descriptor = io.FileIO(str(source), mode=mode)
+    elif isinstance(source, bytes):
+        descriptor = io.BytesIO(source)  # type: ignore
+    else:
+        raise TypeError("Not supported type")
+    return descriptor
+
+
+def calc_hash(source: Union[Path, str, bytes, io.BytesIO, io.FileIO]) -> str:
+    hash_md5 = hashlib.md5()
+    if not isinstance(source, (io.BytesIO, io.FileIO)):
+        source = get_io(source, mode="rb")
+    for chunk in iter(lambda: source.read(4096), b""):  # type: ignore
+        hash_md5.update(chunk)
+    return hash_md5.hexdigest()
+
+
+def download_by_url(url: str, fname: Optional[Union[str, Path]], timeout: float = TIMEOUT) -> Optional[bytes]:
+    response = requests.get(url, timeout=timeout)
+    if response.status_code != 200:
+        response.raise_for_status()
+        return None
+    else:
+        if fname:
+            Path(fname).parent.mkdir(exist_ok=True, parents=True)
+            with open(fname, "wb+") as f:
+                f.write(response.content)
+        return response.content
+
+
+def download_and_validate_file(
+    fname: Union[str, Path], url: str, md5: str, timeout: float = TIMEOUT
+) -> Union[str, Path]:
+    if not (Path(fname).exists() and calc_hash(fname) == md5):
+        download_by_url(url=url, fname=fname, timeout=timeout)
+    md5_last = calc_hash(fname)
+    if md5_last != md5:
+        raise InvalidHash(f"Hash for file {Path(fname).resolve()} in invalid. Got {md5_last}, expected {md5}")
+    return fname
+
+
+def download_demo_sgy(
+    fname: Union[str, Path] = DEMO_SGY_PATH, url: str = DEMO_SGY_URL, md5: str = DEMO_SGY_HASH
+) -> Union[str, Path]:
+    return download_and_validate_file(fname=fname, url=url, md5=md5)
+
+
+def download_model_onnx(
+    fname: Union[str, Path] = MODEL_ONNX_PATH, url: str = MODEL_ONNX_URL, md5: str = MODEL_ONNX_HASH
+) -> Union[str, Path]:
+    return download_and_validate_file(fname=fname, url=url, md5=md5)
+
+
+def multiply_iterable_by(sample: TTimeType, multiplier: float, cast_to: Optional[Any] = None) -> TTimeType:
+    if isinstance(sample, (int, float, str)):
+        result = sample * multiplier  # type: ignore
+        return cast_to(result) if cast_to is not None else result
+    elif isinstance(sample, (np.number, np.ndarray)):
+        result = sample * multiplier
+        return result.astype(cast_to) if cast_to is not None else result
+    elif isinstance(sample, list):
+        return list(multiply_iterable_by(val, multiplier, cast_to) for val in sample)
+    elif isinstance(sample, tuple):
+        return tuple(multiply_iterable_by(val, multiplier, cast_to) for val in sample)
+    else:
+        raise TypeError("Invalid type for samples")
+
+
+class UnitsConverter:
+    def __init__(
+        self,
+        *args: Any,
+        sgy_mcs: Optional[Union[int, float]] = None,
+        sgy_ms: Optional[Union[int, float]] = None,
+    ):
+        if args:
+            raise ValueError("Specify explicitly either `sgy_mcs`or `sgy_ms` as keyword argument")
+        if (sgy_mcs is None and sgy_ms is None) or (sgy_mcs is not None and sgy_ms is not None):
+            raise RuntimeError("One and only one of `sgy_mcs` or `sgy_ms` must be specified")
+        elif sgy_mcs is not None:
+            self.sgy_mcs = sgy_mcs
+            self.sgy_ms = self.mcs2ms(sgy_mcs)  # type: ignore
+        elif sgy_ms is not None:
+            self.sgy_mcs = self.ms2mcs(sgy_ms)  # type: ignore
+            self.sgy_ms = sgy_ms
+        else:
+            raise RuntimeError("Init error")
+
+    @staticmethod
+    def ms2mcs(sample: TTimeType, cast_to: Any = int) -> TTimeType:
+        return multiply_iterable_by(sample, 1000, cast_to)
+
+    @staticmethod
+    def mcs2ms(sample: TTimeType, cast_to: Any = float) -> TTimeType:
+        return multiply_iterable_by(sample, 0.001, cast_to)
+
+    def ms2index(self, sample: TTimeType, cast_to: Any = int) -> TTimeType:
+        return multiply_iterable_by(sample, 1 / self.sgy_ms, cast_to)  # type: ignore
+
+    def mcs2index(self, sample: TTimeType, cast_to: Any = int) -> TTimeType:
+        return multiply_iterable_by(sample, 1 / self.sgy_mcs, cast_to)
+
+    def index2ms(self, sample: TTimeType, cast_to: Any = float) -> TTimeType:
+        return multiply_iterable_by(sample, self.sgy_ms, cast_to)  # type: ignore
+
+    def index2mcs(self, sample: TTimeType, cast_to: Any = int) -> TTimeType:
+        return multiply_iterable_by(sample, self.sgy_mcs, cast_to)
+
+
+def remove_unused_kwargs(kwargs: Dict[str, Any], constructor: Any) -> Dict[str, Any]:
+    return {k: v for k, v in kwargs.items() if k in inspect.signature(constructor).parameters}
```

### Comparing `first-breaks-picking-0.3.0b0/first_breaks/utils/visualizations.py` & `first-breaks-picking-0.4.0a0/first_breaks/utils/visualizations.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.3.0b0/first_breaks_picking.egg-info/SOURCES.txt` & `first-breaks-picking-0.4.0a0/first_breaks_picking.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 LICENSE
+MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
-setup.py
 first_breaks/__init__.py
+first_breaks/__main__.py
 first_breaks/cli.py
 first_breaks/const.py
-first_breaks/_pytorch/models/__init__.py
-first_breaks/_pytorch/models/unet3plus.py
 first_breaks/data_models/__init__.py
 first_breaks/data_models/dependent.py
 first_breaks/data_models/independent.py
 first_breaks/data_models/initialised_defaults.py
 first_breaks/desktop/__init__.py
 first_breaks/desktop/byte_encode_unit_widget.py
 first_breaks/desktop/combobox_with_mapping.py
@@ -27,25 +27,17 @@
 first_breaks/picking/picker_onnx.py
 first_breaks/picking/task.py
 first_breaks/picking/utils.py
 first_breaks/sgy/__init__.py
 first_breaks/sgy/headers.py
 first_breaks/sgy/reader.py
 first_breaks/utils/__init__.py
+first_breaks/utils/cuda.py
 first_breaks/utils/debug.py
 first_breaks/utils/utils.py
 first_breaks/utils/visualizations.py
 first_breaks_picking.egg-info/PKG-INFO
 first_breaks_picking.egg-info/SOURCES.txt
 first_breaks_picking.egg-info/dependency_links.txt
 first_breaks_picking.egg-info/entry_points.txt
 first_breaks_picking.egg-info/requires.txt
-first_breaks_picking.egg-info/top_level.txt
-tests/test_demo_sgy.py
-tests/test_readme_examples.py
-tests/test_desktop/__init__.py
-tests/test_desktop/test_graph.py
-tests/test_picking/__init__.py
-tests/test_picking/test_picker.py
-tests/test_picking/test_task.py
-tests/test_sgy/__init__.py
-tests/test_sgy/test_reader.py
+first_breaks_picking.egg-info/top_level.txt
```

