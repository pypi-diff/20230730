# Comparing `tmp/qtdraw-1.1.4.tar.gz` & `tmp/qtdraw-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtdraw-1.1.4.tar", last modified: Sat Jul 29 13:53:24 2023, max compression
+gzip compressed data, was "qtdraw-1.1.5.tar", last modified: Sun Jul 30 15:15:07 2023, max compression
```

## Comparing `qtdraw-1.1.4.tar` & `qtdraw-1.1.5.tar`

### file list

```diff
@@ -1,47 +1,50 @@
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-29 13:53:24.769204 qtdraw-1.1.4/
--rw-r--r--   0 hiro       (501) staff       (20)     1078 2023-05-09 03:18:56.000000 qtdraw-1.1.4/LICENSE
--rw-------   0 hiro       (501) staff       (20)      107 2023-05-15 22:04:32.000000 qtdraw-1.1.4/MANIFEST.in
--rw-r--r--   0 hiro       (501) staff       (20)     2464 2023-07-29 13:53:24.769289 qtdraw-1.1.4/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     2084 2023-07-29 13:47:38.000000 qtdraw-1.1.4/README.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-29 13:53:24.762182 qtdraw-1.1.4/qtdraw/
--rw-r--r--   0 hiro       (501) staff       (20)       79 2023-07-29 10:18:46.000000 qtdraw-1.1.4/qtdraw/__init__.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-29 13:53:24.767976 qtdraw-1.1.4/qtdraw/core/
--rw-r--r--   0 hiro       (501) staff       (20)    11407 2023-05-15 12:36:33.000000 qtdraw-1.1.4/qtdraw/core/basic_object.py
--rw-r--r--   0 hiro       (501) staff       (20)      945 2023-05-09 03:18:56.000000 qtdraw-1.1.4/qtdraw/core/color_dialog.py
--rw-r--r--   0 hiro       (501) staff       (20)    15144 2023-05-15 12:36:33.000000 qtdraw-1.1.4/qtdraw/core/color_palette.py
--rw-r--r--   0 hiro       (501) staff       (20)     2443 2023-05-09 03:18:56.000000 qtdraw-1.1.4/qtdraw/core/default_panel.ui
--rw-r--r--   0 hiro       (501) staff       (20)     3719 2023-05-15 12:36:33.000000 qtdraw-1.1.4/qtdraw/core/dialog_about.py
--rw-r--r--   0 hiro       (501) staff       (20)    17447 2023-05-09 03:18:56.000000 qtdraw-1.1.4/qtdraw/core/dialog_preference.py
--rw-r--r--   0 hiro       (501) staff       (20)    16441 2023-05-15 12:36:33.000000 qtdraw-1.1.4/qtdraw/core/editable_widget.py
--rw-r--r--   0 hiro       (501) staff       (20)     8466 2023-05-09 03:18:56.000000 qtdraw-1.1.4/qtdraw/core/group_model.py
--rw-r--r--   0 hiro       (501) staff       (20)     2233 2023-05-09 03:18:56.000000 qtdraw-1.1.4/qtdraw/core/group_panel.ui
--rw-r--r--   0 hiro       (501) staff       (20)     1656 2023-05-09 03:18:56.000000 qtdraw-1.1.4/qtdraw/core/group_tab.py
--rw-r--r--   0 hiro       (501) staff       (20)     4632 2023-05-09 03:18:56.000000 qtdraw-1.1.4/qtdraw/core/group_view.py
--rw-r--r--   0 hiro       (501) staff       (20)     9744 2023-05-15 12:36:33.000000 qtdraw-1.1.4/qtdraw/core/line_edit.py
--rw-r--r--   0 hiro       (501) staff       (20)     2837 2023-05-15 12:36:33.000000 qtdraw-1.1.4/qtdraw/core/pixmap_converter.py
--rw-r--r--   0 hiro       (501) staff       (20)     2385 2023-05-09 03:18:56.000000 qtdraw-1.1.4/qtdraw/core/qt_logging.py
--rw-r--r--   0 hiro       (501) staff       (20)   187925 2023-05-09 03:18:56.000000 qtdraw-1.1.4/qtdraw/core/qtdraw.png
--rw-r--r--   0 hiro       (501) staff       (20)    31369 2023-05-09 03:18:56.000000 qtdraw-1.1.4/qtdraw/core/qtdraw.ui
--rw-r--r--   0 hiro       (501) staff       (20)    17478 2023-05-09 03:18:56.000000 qtdraw-1.1.4/qtdraw/core/setting.py
--rw-r--r--   0 hiro       (501) staff       (20)     2678 2023-05-09 03:18:56.000000 qtdraw-1.1.4/qtdraw/core/table_dialog.py
--rw-r--r--   0 hiro       (501) staff       (20)     4458 2023-05-09 03:18:56.000000 qtdraw-1.1.4/qtdraw/core/tree_item.py
--rw-r--r--   0 hiro       (501) staff       (20)    16260 2023-05-24 14:55:28.000000 qtdraw-1.1.4/qtdraw/core/tree_item_model.py
--rw-r--r--   0 hiro       (501) staff       (20)     7490 2023-07-29 10:18:46.000000 qtdraw-1.1.4/qtdraw/core/util.py
--rw-r--r--   0 hiro       (501) staff       (20)     4715 2023-05-09 03:18:56.000000 qtdraw-1.1.4/qtdraw/core/validator.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-29 13:53:24.768862 qtdraw-1.1.4/qtdraw/multipie/
--rw-r--r--   0 hiro       (501) staff       (20)    48651 2023-07-29 13:47:38.000000 qtdraw-1.1.4/qtdraw/multipie/dialog_group.py
--rw-r--r--   0 hiro       (501) staff       (20)     9646 2023-05-15 12:36:32.000000 qtdraw-1.1.4/qtdraw/multipie/dialog_group_info.py
--rw-r--r--   0 hiro       (501) staff       (20)     1839 2023-05-09 03:18:56.000000 qtdraw-1.1.4/qtdraw/multipie/setting.py
--rw-------   0 hiro       (501) staff       (20)    92079 2023-05-20 07:09:31.000000 qtdraw-1.1.4/qtdraw/qt_draw.py
--rw-r--r--   0 hiro       (501) staff       (20)     9242 2023-05-09 03:18:56.000000 qtdraw-1.1.4/qtdraw/qt_draw_base.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-29 13:53:24.769035 qtdraw-1.1.4/qtdraw/scripts/
--rwxr-xr-x   0 hiro       (501) staff       (20)      486 2023-05-26 22:04:11.000000 qtdraw-1.1.4/qtdraw/scripts/qtdraw.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-29 13:53:24.763172 qtdraw-1.1.4/qtdraw.egg-info/
--rw-r--r--   0 hiro       (501) staff       (20)     2464 2023-07-29 13:53:24.000000 qtdraw-1.1.4/qtdraw.egg-info/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     1002 2023-07-29 13:53:24.000000 qtdraw-1.1.4/qtdraw.egg-info/SOURCES.txt
--rw-r--r--   0 hiro       (501) staff       (20)        1 2023-07-29 13:53:24.000000 qtdraw-1.1.4/qtdraw.egg-info/dependency_links.txt
--rw-r--r--   0 hiro       (501) staff       (20)       53 2023-07-29 13:53:24.000000 qtdraw-1.1.4/qtdraw.egg-info/entry_points.txt
--rw-r--r--   0 hiro       (501) staff       (20)      102 2023-07-29 13:53:24.000000 qtdraw-1.1.4/qtdraw.egg-info/requires.txt
--rw-r--r--   0 hiro       (501) staff       (20)        7 2023-07-29 13:53:24.000000 qtdraw-1.1.4/qtdraw.egg-info/top_level.txt
--rw-r--r--   0 hiro       (501) staff       (20)      726 2023-07-29 13:53:24.769758 qtdraw-1.1.4/setup.cfg
--rw-r--r--   0 hiro       (501) staff       (20)       38 2023-05-09 03:18:56.000000 qtdraw-1.1.4/setup.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-30 15:15:07.734285 qtdraw-1.1.5/
+-rw-r--r--   0 hiro       (501) staff       (20)     1078 2023-05-09 03:18:56.000000 qtdraw-1.1.5/LICENSE
+-rw-------   0 hiro       (501) staff       (20)      107 2023-05-15 22:04:32.000000 qtdraw-1.1.5/MANIFEST.in
+-rw-r--r--   0 hiro       (501) staff       (20)     2521 2023-07-30 15:15:07.734783 qtdraw-1.1.5/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     2141 2023-07-30 15:10:36.000000 qtdraw-1.1.5/README.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-30 15:15:07.726034 qtdraw-1.1.5/qtdraw/
+-rw-r--r--   0 hiro       (501) staff       (20)       79 2023-07-29 22:43:50.000000 qtdraw-1.1.5/qtdraw/__init__.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-30 15:15:07.732361 qtdraw-1.1.5/qtdraw/core/
+-rw-r--r--   0 hiro       (501) staff       (20)    11407 2023-05-15 12:36:33.000000 qtdraw-1.1.5/qtdraw/core/basic_object.py
+-rw-r--r--   0 hiro       (501) staff       (20)      945 2023-05-09 03:18:56.000000 qtdraw-1.1.5/qtdraw/core/color_dialog.py
+-rw-r--r--   0 hiro       (501) staff       (20)    15144 2023-05-15 12:36:33.000000 qtdraw-1.1.5/qtdraw/core/color_palette.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2443 2023-05-09 03:18:56.000000 qtdraw-1.1.5/qtdraw/core/default_panel.ui
+-rw-r--r--   0 hiro       (501) staff       (20)     3719 2023-05-15 12:36:33.000000 qtdraw-1.1.5/qtdraw/core/dialog_about.py
+-rw-r--r--   0 hiro       (501) staff       (20)    17447 2023-05-09 03:18:56.000000 qtdraw-1.1.5/qtdraw/core/dialog_preference.py
+-rw-r--r--   0 hiro       (501) staff       (20)    16441 2023-05-15 12:36:33.000000 qtdraw-1.1.5/qtdraw/core/editable_widget.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8466 2023-05-09 03:18:56.000000 qtdraw-1.1.5/qtdraw/core/group_model.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2233 2023-05-09 03:18:56.000000 qtdraw-1.1.5/qtdraw/core/group_panel.ui
+-rw-r--r--   0 hiro       (501) staff       (20)     1656 2023-05-09 03:18:56.000000 qtdraw-1.1.5/qtdraw/core/group_tab.py
+-rw-r--r--   0 hiro       (501) staff       (20)     4632 2023-05-09 03:18:56.000000 qtdraw-1.1.5/qtdraw/core/group_view.py
+-rw-r--r--   0 hiro       (501) staff       (20)     9744 2023-05-15 12:36:33.000000 qtdraw-1.1.5/qtdraw/core/line_edit.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2837 2023-05-15 12:36:33.000000 qtdraw-1.1.5/qtdraw/core/pixmap_converter.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2385 2023-05-09 03:18:56.000000 qtdraw-1.1.5/qtdraw/core/qt_logging.py
+-rw-r--r--   0 hiro       (501) staff       (20)   187925 2023-05-09 03:18:56.000000 qtdraw-1.1.5/qtdraw/core/qtdraw.png
+-rw-r--r--   0 hiro       (501) staff       (20)    31369 2023-05-09 03:18:56.000000 qtdraw-1.1.5/qtdraw/core/qtdraw.ui
+-rw-r--r--   0 hiro       (501) staff       (20)    17651 2023-07-30 15:03:59.000000 qtdraw-1.1.5/qtdraw/core/setting.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2678 2023-05-09 03:18:56.000000 qtdraw-1.1.5/qtdraw/core/table_dialog.py
+-rw-r--r--   0 hiro       (501) staff       (20)     4458 2023-05-09 03:18:56.000000 qtdraw-1.1.5/qtdraw/core/tree_item.py
+-rw-r--r--   0 hiro       (501) staff       (20)    16260 2023-05-24 14:55:28.000000 qtdraw-1.1.5/qtdraw/core/tree_item_model.py
+-rw-r--r--   0 hiro       (501) staff       (20)     7490 2023-07-29 10:18:46.000000 qtdraw-1.1.5/qtdraw/core/util.py
+-rw-r--r--   0 hiro       (501) staff       (20)     4715 2023-05-09 03:18:56.000000 qtdraw-1.1.5/qtdraw/core/validator.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-30 15:15:07.733135 qtdraw-1.1.5/qtdraw/multipie/
+-rw-r--r--   0 hiro       (501) staff       (20)    48651 2023-07-29 13:47:38.000000 qtdraw-1.1.5/qtdraw/multipie/dialog_group.py
+-rw-r--r--   0 hiro       (501) staff       (20)     9646 2023-05-15 12:36:32.000000 qtdraw-1.1.5/qtdraw/multipie/dialog_group_info.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1839 2023-05-09 03:18:56.000000 qtdraw-1.1.5/qtdraw/multipie/setting.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-30 15:15:07.733498 qtdraw-1.1.5/qtdraw/parser/
+-rw-r--r--   0 hiro       (501) staff       (20)     5984 2023-07-30 13:25:48.000000 qtdraw-1.1.5/qtdraw/parser/element.py
+-rw-r--r--   0 hiro       (501) staff       (20)     3928 2023-07-30 14:32:31.000000 qtdraw-1.1.5/qtdraw/parser/read_cif.py
+-rw-------   0 hiro       (501) staff       (20)    92461 2023-07-30 08:52:04.000000 qtdraw-1.1.5/qtdraw/qt_draw.py
+-rw-r--r--   0 hiro       (501) staff       (20)     9242 2023-05-09 03:18:56.000000 qtdraw-1.1.5/qtdraw/qt_draw_base.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-30 15:15:07.733921 qtdraw-1.1.5/qtdraw/scripts/
+-rwxr-xr-x   0 hiro       (501) staff       (20)      486 2023-05-26 22:04:11.000000 qtdraw-1.1.5/qtdraw/scripts/qtdraw.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-30 15:15:07.726916 qtdraw-1.1.5/qtdraw.egg-info/
+-rw-r--r--   0 hiro       (501) staff       (20)     2521 2023-07-30 15:15:07.000000 qtdraw-1.1.5/qtdraw.egg-info/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     1053 2023-07-30 15:15:07.000000 qtdraw-1.1.5/qtdraw.egg-info/SOURCES.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        1 2023-07-30 15:15:07.000000 qtdraw-1.1.5/qtdraw.egg-info/dependency_links.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       53 2023-07-30 15:15:07.000000 qtdraw-1.1.5/qtdraw.egg-info/entry_points.txt
+-rw-r--r--   0 hiro       (501) staff       (20)      117 2023-07-30 15:15:07.000000 qtdraw-1.1.5/qtdraw.egg-info/requires.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        7 2023-07-30 15:15:07.000000 qtdraw-1.1.5/qtdraw.egg-info/top_level.txt
+-rw-r--r--   0 hiro       (501) staff       (20)      743 2023-07-30 15:15:07.735250 qtdraw-1.1.5/setup.cfg
+-rw-r--r--   0 hiro       (501) staff       (20)       38 2023-05-09 03:18:56.000000 qtdraw-1.1.5/setup.py
```

### Comparing `qtdraw-1.1.4/LICENSE` & `qtdraw-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.4/PKG-INFO` & `qtdraw-1.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtdraw
-Version: 1.1.4
+Version: 1.1.5
 Summary: 3D drawing tool for molecules and crystals based on Pyvista and Qt.
 Home-page: https://github.com/CMT-MU/QtDraw
 Author: Hiroaki Kusunose
 Author-email: hiroaki.kusunose@gmail.com
 License: MIT
 Keywords: pyvista,qtpy5
 Requires-Python: >=3.8
@@ -19,15 +19,15 @@
 
 ## Installation
 
 QtDraw can be installed from PyPI using pip on Python >= 3.8:
 ```
 pip install qtdraw
 ```
-It is useful to associate with the following application with `.qtdw` extension.
+It is useful to associate with the following application with `.qtdw` and `.cif` extension.
 - [Mac](https://github.com/CMT-MU/QtDraw/tree/main/others/QtDraw_MacApp.zip)
 - [Windows](https://github.com/CMT-MU/QtDraw/tree/main/others/QtDraw_WinApp.zip)
 
 You can also visit
 [PyPI](https://pypi.org/project/qtdraw/) or [GitHub](https://github.com/CMT-MU/QtDraw) to download the source.
 
 See also, [Install Guide (in Japanese)](https://github.com/CMT-MU/QtDraw/blob/main/docs/install_guide.pdf)
@@ -64,8 +64,8 @@
 ## Requirements
 - This library requires [TeXLive](https://www.tug.org/texlive/) environment.
 - Symmetry operation supports are provided by [MultiPie](https://github.com/CMT-MU/MultiPie).
 
 ## Documentation
 
 Refer to the [documentation](https://cmt-mu.github.io/QtDraw/) for installation and usage.
-See also, [Manual](./manual.pdf).
+See also, [Manual](https://github.com/CMT-MU/QtDraw/blob/main/docs/manual.pdf).
```

### Comparing `qtdraw-1.1.4/README.md` & `qtdraw-1.1.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 ## Installation
 
 QtDraw can be installed from PyPI using pip on Python >= 3.8:
 ```
 pip install qtdraw
 ```
-It is useful to associate with the following application with `.qtdw` extension.
+It is useful to associate with the following application with `.qtdw` and `.cif` extension.
 - [Mac](https://github.com/CMT-MU/QtDraw/tree/main/others/QtDraw_MacApp.zip)
 - [Windows](https://github.com/CMT-MU/QtDraw/tree/main/others/QtDraw_WinApp.zip)
 
 You can also visit
 [PyPI](https://pypi.org/project/qtdraw/) or [GitHub](https://github.com/CMT-MU/QtDraw) to download the source.
 
 See also, [Install Guide (in Japanese)](https://github.com/CMT-MU/QtDraw/blob/main/docs/install_guide.pdf)
@@ -50,8 +50,8 @@
 ## Requirements
 - This library requires [TeXLive](https://www.tug.org/texlive/) environment.
 - Symmetry operation supports are provided by [MultiPie](https://github.com/CMT-MU/MultiPie).
 
 ## Documentation
 
 Refer to the [documentation](https://cmt-mu.github.io/QtDraw/) for installation and usage.
-See also, [Manual](./manual.pdf).
+See also, [Manual](https://github.com/CMT-MU/QtDraw/blob/main/docs/manual.pdf).
```

### Comparing `qtdraw-1.1.4/qtdraw/core/basic_object.py` & `qtdraw-1.1.5/qtdraw/core/basic_object.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.4/qtdraw/core/color_dialog.py` & `qtdraw-1.1.5/qtdraw/core/color_dialog.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.4/qtdraw/core/color_palette.py` & `qtdraw-1.1.5/qtdraw/core/color_palette.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.4/qtdraw/core/default_panel.ui` & `qtdraw-1.1.5/qtdraw/core/default_panel.ui`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.4/qtdraw/core/dialog_about.py` & `qtdraw-1.1.5/qtdraw/core/dialog_about.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.4/qtdraw/core/dialog_preference.py` & `qtdraw-1.1.5/qtdraw/core/dialog_preference.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.4/qtdraw/core/editable_widget.py` & `qtdraw-1.1.5/qtdraw/core/editable_widget.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.4/qtdraw/core/group_model.py` & `qtdraw-1.1.5/qtdraw/core/group_model.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.4/qtdraw/core/group_panel.ui` & `qtdraw-1.1.5/qtdraw/core/group_panel.ui`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.4/qtdraw/core/group_tab.py` & `qtdraw-1.1.5/qtdraw/core/group_tab.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.4/qtdraw/core/group_view.py` & `qtdraw-1.1.5/qtdraw/core/group_view.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.4/qtdraw/core/line_edit.py` & `qtdraw-1.1.5/qtdraw/core/line_edit.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.4/qtdraw/core/pixmap_converter.py` & `qtdraw-1.1.5/qtdraw/core/pixmap_converter.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.4/qtdraw/core/qt_logging.py` & `qtdraw-1.1.5/qtdraw/core/qt_logging.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.4/qtdraw/core/qtdraw.png` & `qtdraw-1.1.5/qtdraw/core/qtdraw.png`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.4/qtdraw/core/qtdraw.ui` & `qtdraw-1.1.5/qtdraw/core/qtdraw.ui`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.4/qtdraw/core/setting.py` & `qtdraw-1.1.5/qtdraw/core/setting.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,19 @@
     # plotter setting.
     "plotter.ui": "qtdraw.ui",
     "plotter.style": "fusion",  # "fusion/windows/macintosh"
     "plotter.font.family": "Helvetica Neue",  # "Monaco/Osaka/Times New Roman/Arial/Helvetica Neue"
     "plotter.font.size": 13,  # pixel
     "plotter.theme": "document",  # "document/paraview/default/dark"
     "plotter.ext": ".qtdw",
+    "plotter.cif": ".cif",
+    "plotter.vesta": ".vesta",
+    "plotter.color_scheme": "VESTA",  # "VESTA/Jmol"
+    "plotter.site_scale": 1.2,
+    "plotter.bond_scale": 1.2,
     #
     # default for plotting.
     "plot.orbital.theta": 180,
     "plot.orbital.phi": 180,
     #
     # detailed setting.
     "detail.axis.shaft.radius": 0.05,
```

### Comparing `qtdraw-1.1.4/qtdraw/core/table_dialog.py` & `qtdraw-1.1.5/qtdraw/core/table_dialog.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.4/qtdraw/core/tree_item.py` & `qtdraw-1.1.5/qtdraw/core/tree_item.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.4/qtdraw/core/tree_item_model.py` & `qtdraw-1.1.5/qtdraw/core/tree_item_model.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.4/qtdraw/core/util.py` & `qtdraw-1.1.5/qtdraw/core/util.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.4/qtdraw/core/validator.py` & `qtdraw-1.1.5/qtdraw/core/validator.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.4/qtdraw/multipie/dialog_group.py` & `qtdraw-1.1.5/qtdraw/multipie/dialog_group.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.4/qtdraw/multipie/dialog_group_info.py` & `qtdraw-1.1.5/qtdraw/multipie/dialog_group_info.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.4/qtdraw/multipie/setting.py` & `qtdraw-1.1.5/qtdraw/multipie/setting.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.4/qtdraw/qt_draw.py` & `qtdraw-1.1.5/qtdraw/qt_draw.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     create_plane,
     create_box,
     create_polygon,
     create_text,
     create_spline,
 )
 from qtdraw.core.color_palette import all_colors, custom_colormap, check_color
+from qtdraw.parser.read_cif import plot_cif
 from qtdraw import __version__
 
 from qtdraw.core.qt_logging import UncaughtHook
 
 CHOP = 1e-4
 qt_exception_hook = UncaughtHook()
 global QT_EXCEPTION_HOOK
@@ -1646,35 +1647,43 @@
             self.tab.deselectedData.connect(self._remove_spotlight)
             self.tab.finished["int"].connect(self._close_dialog)
             self.tab.show()
 
     # ==================================================
     def _load(self):
         default_ext = rcParams["plotter.ext"]
+        loadable_ext = rcParams["plotter.cif"]  # +" "+rcParams["plotter.vesta"]
         default_file = os.getcwd()
-        filename, _ = QFileDialog.getOpenFileName(self, "Load QtDraw", default_file, "QtDraw file (*" + default_ext + ")")
+        ext_str = default_ext + " " + loadable_ext
+        filename, _ = QFileDialog.getOpenFileName(
+            self, "Load QtDraw", default_file, "QtDraw file (" + ext_str.replace(".", "*.") + ")"
+        )
         if filename:
             _, ext = os.path.splitext(filename)
             if ext == "":
                 ext = default_ext
                 filename += ext
-            if ext == default_ext:
+            if ext in ext_str.split(" "):
                 self._close_dialog()
-                self._load_file(filename)
+                self._load_file(filename, ext)
                 self.set_status(f"loaded {filename}.")
             else:
                 self.set_status(f"{ext} is unsupported, use {default_ext}.")
 
     # ==================================================
-    def _load_file(self, filename):
-        load_dict = read_dict(filename)
-
+    def _load_file(self, filename, ext):
         self._homedir = os.path.dirname(filename)
         os.chdir(self._homedir)
 
+        if ext == rcParams["plotter.cif"]:
+            plot_cif(self, filename)
+            return
+
+        load_dict = read_dict(filename)
+
         self.preference = load_dict["preference"]
         self.setting = load_dict["setting"]
         self._remove_all_actor()
         self._init_all()
         self.set_view()
 
         if self.setting["cluster"]:
@@ -2457,15 +2466,16 @@
         font_size = rcParams["plotter.font.size"]
         self.app = create_application(style=style, font=font, font_size=font_size)
         super().__init__(title, model, cell, origin, view, size, axis_type, view_range, repeat, clip, cluster)
         if not check_latex_installed():
             QMessageBox.critical(None, "Error", f"LaTeX command, '{latex_cmd}', cannot be found.", QMessageBox.Yes)
             exit()
         if filename is not None and os.path.isfile(filename):
-            self._load_file(filename)
+            _, ext = os.path.splitext(filename)
+            self._load_file(filename, ext)
             self.set_status(f"loaded {filename}.")
 
     # ==================================================
     def show(self):
         """
         show the plot.
         """
```

### Comparing `qtdraw-1.1.4/qtdraw/qt_draw_base.py` & `qtdraw-1.1.5/qtdraw/qt_draw_base.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.4/qtdraw.egg-info/PKG-INFO` & `qtdraw-1.1.5/qtdraw.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtdraw
-Version: 1.1.4
+Version: 1.1.5
 Summary: 3D drawing tool for molecules and crystals based on Pyvista and Qt.
 Home-page: https://github.com/CMT-MU/QtDraw
 Author: Hiroaki Kusunose
 Author-email: hiroaki.kusunose@gmail.com
 License: MIT
 Keywords: pyvista,qtpy5
 Requires-Python: >=3.8
@@ -19,15 +19,15 @@
 
 ## Installation
 
 QtDraw can be installed from PyPI using pip on Python >= 3.8:
 ```
 pip install qtdraw
 ```
-It is useful to associate with the following application with `.qtdw` extension.
+It is useful to associate with the following application with `.qtdw` and `.cif` extension.
 - [Mac](https://github.com/CMT-MU/QtDraw/tree/main/others/QtDraw_MacApp.zip)
 - [Windows](https://github.com/CMT-MU/QtDraw/tree/main/others/QtDraw_WinApp.zip)
 
 You can also visit
 [PyPI](https://pypi.org/project/qtdraw/) or [GitHub](https://github.com/CMT-MU/QtDraw) to download the source.
 
 See also, [Install Guide (in Japanese)](https://github.com/CMT-MU/QtDraw/blob/main/docs/install_guide.pdf)
@@ -64,8 +64,8 @@
 ## Requirements
 - This library requires [TeXLive](https://www.tug.org/texlive/) environment.
 - Symmetry operation supports are provided by [MultiPie](https://github.com/CMT-MU/MultiPie).
 
 ## Documentation
 
 Refer to the [documentation](https://cmt-mu.github.io/QtDraw/) for installation and usage.
-See also, [Manual](./manual.pdf).
+See also, [Manual](https://github.com/CMT-MU/QtDraw/blob/main/docs/manual.pdf).
```

### Comparing `qtdraw-1.1.4/qtdraw.egg-info/SOURCES.txt` & `qtdraw-1.1.5/qtdraw.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -33,8 +33,10 @@
 qtdraw/core/tree_item.py
 qtdraw/core/tree_item_model.py
 qtdraw/core/util.py
 qtdraw/core/validator.py
 qtdraw/multipie/dialog_group.py
 qtdraw/multipie/dialog_group_info.py
 qtdraw/multipie/setting.py
+qtdraw/parser/element.py
+qtdraw/parser/read_cif.py
 qtdraw/scripts/qtdraw.py
```

### Comparing `qtdraw-1.1.4/setup.cfg` & `qtdraw-1.1.5/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -9,19 +9,21 @@
 long_description_content_type = text/markdown
 keywords = pyvista, qtpy5
 license = MIT
 
 [options]
 python_requires = >=3.8
 install_requires = 
-	click
 	matplotlib
 	seaborn
+	pyqt5
 	pyvista
 	pyvistaqt
+	click
+	pymatgen
 	gcoreutils
 packages = find:
 include_package_data = True
 
 [options.extras_require]
 dev = 
 	sphinx
```

