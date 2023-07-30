# Comparing `tmp/textology-0.2.0.tar.gz` & `tmp/textology-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textology-0.2.0.tar", last modified: Mon Jul 24 01:21:10 2023, max compression
+gzip compressed data, was "textology-0.2.1.tar", last modified: Sun Jul 30 17:55:13 2023, max compression
```

## Comparing `textology-0.2.0.tar` & `textology-0.2.1.tar`

### file list

```diff
@@ -1,46 +1,71 @@
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-24 01:21:10.960494 textology-0.2.0/
--rw-r--r--   0 dfritz     (502) staff       (20)     1068 2023-07-01 18:44:36.000000 textology-0.2.0/LICENSE
--rw-r--r--   0 dfritz     (502) staff       (20)       97 2023-07-08 19:46:35.000000 textology-0.2.0/MANIFEST.in
--rw-r--r--   0 dfritz     (502) staff       (20)    15562 2023-07-24 01:21:10.960768 textology-0.2.0/PKG-INFO
--rw-r--r--   0 dfritz     (502) staff       (20)    14200 2023-07-24 01:09:35.000000 textology-0.2.0/README.md
--rw-r--r--   0 dfritz     (502) staff       (20)       22 2023-07-08 19:46:35.000000 textology-0.2.0/requirements-dev.txt
--rw-r--r--   0 dfritz     (502) staff       (20)      168 2023-07-08 19:46:35.000000 textology-0.2.0/requirements-full-dev.txt
--rw-r--r--   0 dfritz     (502) staff       (20)       16 2023-07-04 21:18:52.000000 textology-0.2.0/requirements.txt
--rw-r--r--   0 dfritz     (502) staff       (20)     1667 2023-07-24 01:21:10.962022 textology-0.2.0/setup.cfg
--rw-r--r--   0 dfritz     (502) staff       (20)     3225 2023-07-08 19:46:35.000000 textology-0.2.0/setup.py
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-24 01:21:10.938913 textology-0.2.0/textology/
--rw-r--r--   0 dfritz     (502) staff       (20)       69 2023-07-24 01:09:35.000000 textology-0.2.0/textology/__init__.py
--rw-r--r--   0 dfritz     (502) staff       (20)    16797 2023-07-24 01:09:35.000000 textology-0.2.0/textology/apps.py
--rw-r--r--   0 dfritz     (502) staff       (20)     6108 2023-07-24 01:09:35.000000 textology-0.2.0/textology/dash_compat.py
--rw-r--r--   0 dfritz     (502) staff       (20)     2772 2023-07-04 21:19:10.000000 textology-0.2.0/textology/history.py
--rw-r--r--   0 dfritz     (502) staff       (20)      492 2023-07-04 21:19:10.000000 textology-0.2.0/textology/logging.py
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-24 01:21:10.948037 textology-0.2.0/textology/observers/
--rw-r--r--   0 dfritz     (502) staff       (20)      885 2023-07-24 01:09:35.000000 textology-0.2.0/textology/observers/__init__.py
--rw-r--r--   0 dfritz     (502) staff       (20)     6230 2023-07-24 01:09:35.000000 textology-0.2.0/textology/observers/_dependencies.py
--rw-r--r--   0 dfritz     (502) staff       (20)      458 2023-07-22 18:13:02.000000 textology-0.2.0/textology/observers/_exceptions.py
--rw-r--r--   0 dfritz     (502) staff       (20)    31200 2023-07-24 01:09:35.000000 textology-0.2.0/textology/observers/_managers.py
--rw-r--r--   0 dfritz     (502) staff       (20)     5473 2023-07-24 01:09:35.000000 textology-0.2.0/textology/pages.py
--rw-r--r--   0 dfritz     (502) staff       (20)    16541 2023-07-16 17:16:06.000000 textology-0.2.0/textology/pytest_utils.py
--rw-r--r--   0 dfritz     (502) staff       (20)    17773 2023-07-16 17:16:06.000000 textology-0.2.0/textology/router.py
--rw-r--r--   0 dfritz     (502) staff       (20)    45559 2023-07-24 01:09:35.000000 textology-0.2.0/textology/test-template.html
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-24 01:21:10.959948 textology-0.2.0/textology/widgets/
--rw-r--r--   0 dfritz     (502) staff       (20)     1204 2023-07-24 01:09:35.000000 textology-0.2.0/textology/widgets/__init__.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1712 2023-07-04 21:18:52.000000 textology-0.2.0/textology/widgets/_button.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1488 2023-07-24 01:09:35.000000 textology-0.2.0/textology/widgets/_containers.py
--rw-r--r--   0 dfritz     (502) staff       (20)     9394 2023-07-15 18:57:36.000000 textology-0.2.0/textology/widgets/_extensions.py
--rw-r--r--   0 dfritz     (502) staff       (20)    11892 2023-07-16 17:16:06.000000 textology-0.2.0/textology/widgets/_horizontal_menus.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1665 2023-07-04 21:18:52.000000 textology-0.2.0/textology/widgets/_label.py
--rw-r--r--   0 dfritz     (502) staff       (20)     2265 2023-07-16 17:16:06.000000 textology-0.2.0/textology/widgets/_list_item.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1992 2023-07-08 19:46:35.000000 textology-0.2.0/textology/widgets/_list_item_header.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1993 2023-07-16 17:16:06.000000 textology-0.2.0/textology/widgets/_list_item_meta.py
--rw-r--r--   0 dfritz     (502) staff       (20)     4919 2023-07-04 21:18:52.000000 textology-0.2.0/textology/widgets/_list_view.py
--rw-r--r--   0 dfritz     (502) staff       (20)     8683 2023-07-09 16:23:23.000000 textology-0.2.0/textology/widgets/_location.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1955 2023-07-04 21:18:52.000000 textology-0.2.0/textology/widgets/_modal_dialog.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1765 2023-07-04 21:18:52.000000 textology-0.2.0/textology/widgets/_static.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1962 2023-07-04 21:18:52.000000 textology-0.2.0/textology/widgets/_store.py
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-24 01:21:10.943831 textology-0.2.0/textology.egg-info/
--rw-r--r--   0 dfritz     (502) staff       (20)    15562 2023-07-24 01:21:10.000000 textology-0.2.0/textology.egg-info/PKG-INFO
--rw-r--r--   0 dfritz     (502) staff       (20)     1069 2023-07-24 01:21:10.000000 textology-0.2.0/textology.egg-info/SOURCES.txt
--rw-r--r--   0 dfritz     (502) staff       (20)        1 2023-07-24 01:21:10.000000 textology-0.2.0/textology.egg-info/dependency_links.txt
--rw-r--r--   0 dfritz     (502) staff       (20)      279 2023-07-24 01:21:10.000000 textology-0.2.0/textology.egg-info/requires.txt
--rw-r--r--   0 dfritz     (502) staff       (20)       10 2023-07-24 01:21:10.000000 textology-0.2.0/textology.egg-info/top_level.txt
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-30 17:55:13.555223 textology-0.2.1/
+-rw-r--r--   0 dfritz     (502) staff       (20)     1068 2023-07-01 18:44:36.000000 textology-0.2.1/LICENSE
+-rw-r--r--   0 dfritz     (502) staff       (20)       97 2023-07-08 19:46:35.000000 textology-0.2.1/MANIFEST.in
+-rw-r--r--   0 dfritz     (502) staff       (20)    15574 2023-07-30 17:55:13.555421 textology-0.2.1/PKG-INFO
+-rw-r--r--   0 dfritz     (502) staff       (20)    14212 2023-07-30 17:52:28.000000 textology-0.2.1/README.md
+-rw-r--r--   0 dfritz     (502) staff       (20)       34 2023-07-30 17:52:28.000000 textology-0.2.1/requirements-dev.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)      168 2023-07-08 19:46:35.000000 textology-0.2.1/requirements-full-dev.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)       16 2023-07-30 17:52:28.000000 textology-0.2.1/requirements.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)     1667 2023-07-30 17:55:13.556658 textology-0.2.1/setup.cfg
+-rw-r--r--   0 dfritz     (502) staff       (20)     3225 2023-07-08 19:46:35.000000 textology-0.2.1/setup.py
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-30 17:55:13.514102 textology-0.2.1/textology/
+-rw-r--r--   0 dfritz     (502) staff       (20)       69 2023-07-30 17:52:28.000000 textology-0.2.1/textology/__init__.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    16797 2023-07-24 01:09:35.000000 textology-0.2.1/textology/apps.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     6108 2023-07-24 01:09:35.000000 textology-0.2.1/textology/dash_compat.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2772 2023-07-04 21:19:10.000000 textology-0.2.1/textology/history.py
+-rw-r--r--   0 dfritz     (502) staff       (20)      492 2023-07-04 21:19:10.000000 textology-0.2.1/textology/logging.py
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-30 17:55:13.524380 textology-0.2.1/textology/observers/
+-rw-r--r--   0 dfritz     (502) staff       (20)      885 2023-07-24 01:09:35.000000 textology-0.2.1/textology/observers/__init__.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     6230 2023-07-24 01:09:35.000000 textology-0.2.1/textology/observers/_dependencies.py
+-rw-r--r--   0 dfritz     (502) staff       (20)      458 2023-07-22 18:13:02.000000 textology-0.2.1/textology/observers/_exceptions.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    31200 2023-07-24 01:09:35.000000 textology-0.2.1/textology/observers/_managers.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     5473 2023-07-24 01:09:35.000000 textology-0.2.1/textology/pages.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    16541 2023-07-16 17:16:06.000000 textology-0.2.1/textology/pytest_utils.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    17773 2023-07-16 17:16:06.000000 textology-0.2.1/textology/router.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    45559 2023-07-24 01:09:35.000000 textology-0.2.1/textology/test-template.html
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-30 17:55:13.536001 textology-0.2.1/textology/widgets/
+-rw-r--r--   0 dfritz     (502) staff       (20)     2701 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/__init__.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1712 2023-07-04 21:18:52.000000 textology-0.2.1/textology/widgets/_button.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    12809 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_extensions.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    11892 2023-07-16 17:16:06.000000 textology-0.2.1/textology/widgets/_horizontal_menus.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2274 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_list_item.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1992 2023-07-08 19:46:35.000000 textology-0.2.1/textology/widgets/_list_item_header.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1993 2023-07-16 17:16:06.000000 textology-0.2.1/textology/widgets/_list_item_meta.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     4919 2023-07-04 21:18:52.000000 textology-0.2.1/textology/widgets/_list_view.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     8735 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_location.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1955 2023-07-04 21:18:52.000000 textology-0.2.1/textology/widgets/_modal_dialog.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2014 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_store.py
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-30 17:55:13.554785 textology-0.2.1/textology/widgets/_textual/
+-rw-r--r--   0 dfritz     (502) staff       (20)      104 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/__init__.py
+-rw-r--r--   0 dfritz     (502) staff       (20)      294 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_checkbox.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1651 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_containers.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1600 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_content_switcher.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2691 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_data_table.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1306 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_directory_tree.py
+-rw-r--r--   0 dfritz     (502) staff       (20)      630 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_footer.py
+-rw-r--r--   0 dfritz     (502) staff       (20)      979 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_header.py
+-rw-r--r--   0 dfritz     (502) staff       (20)      291 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_label.py
+-rw-r--r--   0 dfritz     (502) staff       (20)      263 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_loading_indicator.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2778 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_markdown.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1259 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_option_list.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1076 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_pretty.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1621 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_progress_bar.py
+-rw-r--r--   0 dfritz     (502) staff       (20)      308 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_radio_button.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1213 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_radio_set.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1673 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_select.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1488 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_selection_list.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1490 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_sparkline.py
+-rw-r--r--   0 dfritz     (502) staff       (20)      354 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_static.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1278 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_switch.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2564 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_tabbed_content.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2098 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_tabs.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2169 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_text_input.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1780 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_text_log.py
+-rw-r--r--   0 dfritz     (502) staff       (20)      234 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_tooltip.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1409 2023-07-30 17:52:28.000000 textology-0.2.1/textology/widgets/_textual/_tree.py
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-30 17:55:13.520042 textology-0.2.1/textology.egg-info/
+-rw-r--r--   0 dfritz     (502) staff       (20)    15574 2023-07-30 17:55:13.000000 textology-0.2.1/textology.egg-info/PKG-INFO
+-rw-r--r--   0 dfritz     (502) staff       (20)     2088 2023-07-30 17:55:13.000000 textology-0.2.1/textology.egg-info/SOURCES.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)        1 2023-07-30 17:55:13.000000 textology-0.2.1/textology.egg-info/dependency_links.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)      303 2023-07-30 17:55:13.000000 textology-0.2.1/textology.egg-info/requires.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)       10 2023-07-30 17:55:13.000000 textology-0.2.1/textology.egg-info/top_level.txt
```

### Comparing `textology-0.2.0/LICENSE` & `textology-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `textology-0.2.0/PKG-INFO` & `textology-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textology
-Version: 0.2.0
+Version: 0.2.1
 Summary: Textual extensions for creating Terminal User Interfaces
 Home-page: https://github.com/dfrtz/textology
 Author: David Fritz
 License: MIT
 Project-URL: Issue Tracker, https://github.com/dfrtz/textology/issues
 Project-URL: Source Code, https://github.com/dfrtz/textology
 Platform: MacOS
@@ -38,23 +38,23 @@
   <img src="https://raw.githubusercontent.com/dfrtz/textology/main/docs/banner.svg" width="450">
 </div>
 
 -----------------
 
 
 [![os: windows mac linux](https://img.shields.io/badge/os-linux_|_macos_|_windows-blue)](https://docs.python.org/3.10/)
-[![python: 3.10+](https://img.shields.io/badge/python-3.10_|_3.11-blue)](https://docs.python.org/3.10/)
+[![python: 3.10+](https://img.shields.io/badge/python-3.10_|_3.11-blue)](https://devguide.python.org/versions)
 [![python style: google](https://img.shields.io/badge/python%20style-google-blue)](https://google.github.io/styleguide/pyguide.html)
-[![imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://github.com/PyCQA/isort)
 [![code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![code style: pycodestyle](https://img.shields.io/badge/code%20style-pycodestyle-green)](https://github.com/PyCQA/pycodestyle)
 [![doc style: pydocstyle](https://img.shields.io/badge/doc%20style-pydocstyle-green)](https://github.com/PyCQA/pydocstyle)
 [![static typing: mypy](https://img.shields.io/badge/static_typing-mypy-green)](https://github.com/python/mypy)
 [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/PyCQA/pylint)
-[![testing: pytest](https://img.shields.io/badge/testing-pytest-yellowgreen)](https://github.com/PyCQA/pylint)
+[![testing: pytest](https://img.shields.io/badge/testing-pytest-yellowgreen)](https://github.com/pytest-dev/pytest)
 [![security: bandit](https://img.shields.io/badge/security-bandit-black)](https://github.com/PyCQA/bandit)
 [![license: MIT](https://img.shields.io/badge/license-MIT-lightgrey)](LICENSE)
 
 
 # Textology
 
 ### The study of making interactive UIs with text.
```

### Comparing `textology-0.2.0/README.md` & `textology-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
   <img src="https://raw.githubusercontent.com/dfrtz/textology/main/docs/banner.svg" width="450">
 </div>
 
 -----------------
 
 
 [![os: windows mac linux](https://img.shields.io/badge/os-linux_|_macos_|_windows-blue)](https://docs.python.org/3.10/)
-[![python: 3.10+](https://img.shields.io/badge/python-3.10_|_3.11-blue)](https://docs.python.org/3.10/)
+[![python: 3.10+](https://img.shields.io/badge/python-3.10_|_3.11-blue)](https://devguide.python.org/versions)
 [![python style: google](https://img.shields.io/badge/python%20style-google-blue)](https://google.github.io/styleguide/pyguide.html)
-[![imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://github.com/PyCQA/isort)
 [![code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![code style: pycodestyle](https://img.shields.io/badge/code%20style-pycodestyle-green)](https://github.com/PyCQA/pycodestyle)
 [![doc style: pydocstyle](https://img.shields.io/badge/doc%20style-pydocstyle-green)](https://github.com/PyCQA/pydocstyle)
 [![static typing: mypy](https://img.shields.io/badge/static_typing-mypy-green)](https://github.com/python/mypy)
 [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/PyCQA/pylint)
-[![testing: pytest](https://img.shields.io/badge/testing-pytest-yellowgreen)](https://github.com/PyCQA/pylint)
+[![testing: pytest](https://img.shields.io/badge/testing-pytest-yellowgreen)](https://github.com/pytest-dev/pytest)
 [![security: bandit](https://img.shields.io/badge/security-bandit-black)](https://github.com/PyCQA/bandit)
 [![license: MIT](https://img.shields.io/badge/license-MIT-lightgrey)](LICENSE)
 
 
 # Textology
 
 ### The study of making interactive UIs with text.
```

### Comparing `textology-0.2.0/setup.cfg` & `textology-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `textology-0.2.0/setup.py` & `textology-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `textology-0.2.0/textology/apps.py` & `textology-0.2.1/textology/apps.py`

 * *Files identical despite different names*

### Comparing `textology-0.2.0/textology/dash_compat.py` & `textology-0.2.1/textology/dash_compat.py`

 * *Files identical despite different names*

### Comparing `textology-0.2.0/textology/history.py` & `textology-0.2.1/textology/history.py`

 * *Files identical despite different names*

### Comparing `textology-0.2.0/textology/observers/__init__.py` & `textology-0.2.1/textology/observers/__init__.py`

 * *Files identical despite different names*

### Comparing `textology-0.2.0/textology/observers/_dependencies.py` & `textology-0.2.1/textology/observers/_dependencies.py`

 * *Files identical despite different names*

### Comparing `textology-0.2.0/textology/observers/_managers.py` & `textology-0.2.1/textology/observers/_managers.py`

 * *Files identical despite different names*

### Comparing `textology-0.2.0/textology/pages.py` & `textology-0.2.1/textology/pages.py`

 * *Files identical despite different names*

### Comparing `textology-0.2.0/textology/pytest_utils.py` & `textology-0.2.1/textology/pytest_utils.py`

 * *Files identical despite different names*

### Comparing `textology-0.2.0/textology/router.py` & `textology-0.2.1/textology/router.py`

 * *Files identical despite different names*

### Comparing `textology-0.2.0/textology/test-template.html` & `textology-0.2.1/textology/test-template.html`

 * *Files identical despite different names*

### Comparing `textology-0.2.0/textology/widgets/_button.py` & `textology-0.2.1/textology/widgets/_button.py`

 * *Files identical despite different names*

### Comparing `textology-0.2.0/textology/widgets/_containers.py` & `textology-0.2.1/textology/widgets/_list_item.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,60 @@
-"""Extended Textual container widgets."""
-
-from __future__ import annotations
+"""Extended Textual widget that is an item within a ListView, and contains metadata about the selection."""
 
 from typing import Any
 
-from textual import containers
+from textual import events
+from textual import widgets
 from textual.widget import Widget
 
 from ._extensions import WidgetExtension
+from ._textual._label import Label
+
+# Recommended events to ignore when widgets are used in ListViews to prevent large unneeded event batches.
+LIST_ITEM_EVENT_IGNORES = (
+    events.Mount,
+    events.Unmount,
+    events.Show,
+    events.Hide,
+    events.Resize,
+)
 
 
-class Container(WidgetExtension, containers.Container):
-    """An extended, simple, container widget, with vertical layout."""
+class ListItem(WidgetExtension, widgets.ListItem):
+    """An extended widget that is an item within a ListView, and contains metadata about the selection."""
 
     def __init__(
         self,
         *children: Widget,
         name: str | None = None,
         id: str | None = None,
         classes: str | None = None,
         disabled: bool = False,
+        data: Any = None,
         **extension_configs: Any,
     ) -> None:
-        """Initialize a Container widget with extension arguments.
+        """Initialize a ListItem with extension arguments.
 
         Args:
             *children: Child widgets.
             name: The name of the widget.
+                If no child is provided for display, and no "data" with "label" key, name will be used in a Label.
             id: The ID of the widget in the DOM.
             classes: The CSS classes for the widget.
             disabled: Whether the widget is disabled or not.
+            data: Optional data associated with the list item.
+                If no child is provided for display, the data will be searched for a "label" key to use in a Label.
             extension_configs: Widget extension configurations, such as dynamically provided local callbacks by name.
         """
-        super().__init__(
-            *children,
-            name=name,
-            id=id,
-            classes=classes,
-            disabled=disabled,
-        )
+        if not children:
+            label = name
+            if data and "label" in data:
+                label = data["label"]
+            if label:
+                children = [Label(label, disable_messages=LIST_ITEM_EVENT_IGNORES)]
+
+        super().__init__(*children, name=name, id=id, classes=classes, disabled=disabled)
+        if "disable_messages" not in extension_configs:
+            extension_configs["disable_messages"] = LIST_ITEM_EVENT_IGNORES
         self.__extend_widget__(**extension_configs)
-
-
-class PageContainer(Container):
-    """Container used to display page contents, and signal to multi-page applications which ID to use in callbacks.
-
-    If not used in a multi-page app, it is functionally the same as a Container.
-    """
+        self.data = data
+        self.menu_index: int | None = None
```

### Comparing `textology-0.2.0/textology/widgets/_extensions.py` & `textology-0.2.1/textology/widgets/_extensions.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Custom textual Widgets extensions."""
 
-from __future__ import annotations
-
 import time
 from inspect import isawaitable
 from typing import Any
 from typing import Awaitable
 from typing import Callable
 
+from rich.console import RenderableType
+from rich.text import TextType
 from textual import events
 from textual.message import Message
 from textual.reactive import reactive
 from textual.widget import Widget
 
 
 class Clickable:
@@ -51,17 +51,18 @@
 
     If a message is not disabled, or returned after being intercepted, it will then route to a local callback
     if one was provided to the widget on instantiation. Local callbacks provide additional isolation of message
     handling logic from the global app namespace. If there is no local callback for a message, or the local callback
     returns True (for continue), the message will be sent to the original widget message handler, and propagate
     throughout the app as normal.
 
-    If creating a new basic widget, use ExtendedWidget instead. If subclassing an existing basic textual widget,
-    the extension class must be placed before base class to ensure custom behaviors take priority. Example:
-        class MyContainer(MessagingExtension, Container):
+    If creating a new basic widget, use WidgetInitExtension + Widget instead. If subclassing an existing,
+    basic, textual widget,  the extension class must be placed before base class to ensure custom behaviors
+    take priority. Example:
+        class MyContainer(WidgetExtension, Container):
             ...
     """
 
     default_disabled_messages = []
 
     def __extend_widget__(
         self,
@@ -186,19 +187,120 @@
             message.stop()
             message.prevent_default()
         else:
             await super()._on_message(message)
         return None
 
 
-class ExtendedWidget(WidgetExtension, Widget):
-    """A Widget is the base class for Textual widgets with built-in extension support.
+class StaticInitExtension(WidgetExtension):
+    """Extension for textual widgets that inherit from Static class.
+
+    Includes all extensions provided by WidgetExtension, and automatically calls the extension set up.
+    See WidgetExtension for full details on all extended features.
+
+    Example:
+        class Label(StaticInitExtension, widgets.Label):
+            ...
+    """
+
+    def __init__(
+        self,
+        renderable: RenderableType = "",
+        *,
+        expand: bool = False,
+        shrink: bool = False,
+        markup: bool = True,
+        name: str | None = None,
+        id: str | None = None,
+        classes: str | None = None,
+        disabled: bool = False,
+        **extension_configs: Any,
+    ) -> None:
+        """Initialize a Static widget with extension arguments.
+
+        Args:
+            renderable: A Rich renderable, or string containing console markup.
+            expand: Expand content if required to fill container.
+            shrink: Shrink content if required to fill container.
+            markup: True if markup should be parsed and rendered.
+            name: Name of widget.
+            id: ID of Widget.
+            classes: Space separated list of class names.
+            disabled: Whether the static is disabled or not.
+            extension_configs: Widget extension configurations, such as dynamically provided local callbacks by name.
+        """
+        super().__init__(
+            renderable,
+            expand=expand,
+            shrink=shrink,
+            markup=markup,
+            name=name,
+            id=id,
+            classes=classes,
+            disabled=disabled,
+        )
+        self.__extend_widget__(**extension_configs)
+
+
+class ToggleButtonInitExtension(WidgetExtension):
+    """Extension for textual widgets that inherit from ToggleButton class.
+
+    Includes all extensions provided by WidgetExtension, and automatically calls the extension set up.
+    See WidgetExtension for full details on all extended features.
 
-    Use to create new basic widgets with extensions built int. If extending an existing basic textual widget,
-    use WidgetExtension as a mixin instead.
+    Example:
+        class Checkbox(ToggleButtonInitExtension, containers.Checkbox):
+            ...
+    """
+
+    def __init__(
+        self,
+        label: TextType = "",
+        value: bool = False,
+        button_first: bool = True,
+        *,
+        name: str | None = None,
+        id: str | None = None,
+        classes: str | None = None,
+        disabled: bool = False,
+        **extension_configs: Any,
+    ) -> None:
+        """Initialize the toggle.
+
+        Args:
+            label: The label for the toggle.
+            value: The initial value of the toggle.
+            button_first: Should the button come before the label, or after?
+            name: The name of the toggle.
+            id: The ID of the toggle in the DOM.
+            classes: The CSS classes of the toggle.
+            disabled: Whether the button is disabled or not.
+            extension_configs: Widget extension configurations, such as dynamically provided local callbacks by name.
+        """
+        super().__init__(
+            label=label,
+            value=value,
+            button_first=button_first,
+            name=name,
+            id=id,
+            classes=classes,
+            disabled=disabled,
+        )
+        self.__extend_widget__(**extension_configs)
+
+
+class WidgetInitExtension(WidgetExtension):
+    """Extension for textual widgets that inherit from base Widget class.
+
+    Includes all extensions provided by WidgetExtension, and automatically calls the extension set up.
+    See WidgetExtension for full details on all extended features.
+
+    Example:
+        class Container(WidgetInitExtension, containers.Container):
+            ...
     """
 
     def __init__(
         self,
         *children: Widget,
         name: str | None = None,
         id: str | None = None,
```

### Comparing `textology-0.2.0/textology/widgets/_horizontal_menus.py` & `textology-0.2.1/textology/widgets/_horizontal_menus.py`

 * *Files identical despite different names*

### Comparing `textology-0.2.0/textology/widgets/_label.py` & `textology-0.2.1/textology/widgets/_textual/_tree.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,45 @@
-"""Extended Textual label widget for displaying text-oriented renderables."""
+"""Extended Textual Tree widget."""
 
 from typing import Any
 
-from rich.console import RenderableType
+from rich.text import TextType
 from textual import widgets
+from textual.widgets._tree import TreeDataType
 
-from ._extensions import WidgetExtension
+from .._extensions import WidgetExtension
 
 
-class Label(WidgetExtension, widgets.Label):
-    """An extended, simple, label widget for displaying text-oriented renderables."""
+class Tree(WidgetExtension, widgets.Tree):  # pylint: disable=too-many-ancestors
+    """An extended widget for displaying and navigating data in a tree."""
 
     def __init__(
         self,
-        renderable: RenderableType = "",
+        label: TextType,
+        data: TreeDataType | None = None,
         *,
-        expand: bool = False,
-        shrink: bool = False,
-        markup: bool = True,
         name: str | None = None,
         id: str | None = None,
         classes: str | None = None,
         disabled: bool = False,
         **extension_configs: Any,
     ) -> None:
-        """Initialize a Label widget with extension arguments.
+        """Initialize a Tree.
 
         Args:
-            renderable: A Rich renderable, or string containing console markup.
-            expand: Expand content if required to fill container.
-            shrink: Shrink content if required to fill container.
-            markup: True if markup should be parsed and rendered.
-            name: Name of widget.
-            id: ID of Widget.
-            classes: Space separated list of class names.
-            disabled: Whether the static is disabled or not.
+            label: The label of the root node of the tree.
+            data: The optional data to associate with the root node of the tree.
+            name: The name of the Tree.
+            id: The ID of the tree in the DOM.
+            classes: The CSS classes of the tree.
+            disabled: Whether the tree is disabled or not.
             extension_configs: Widget extension configurations, such as dynamically provided local callbacks by name.
         """
         super().__init__(
-            renderable,
-            expand=expand,
-            shrink=shrink,
-            markup=markup,
+            label=label,
+            data=data,
             name=name,
             id=id,
             classes=classes,
             disabled=disabled,
         )
         self.__extend_widget__(**extension_configs)
```

### Comparing `textology-0.2.0/textology/widgets/_list_item_header.py` & `textology-0.2.1/textology/widgets/_list_item_header.py`

 * *Files identical despite different names*

### Comparing `textology-0.2.0/textology/widgets/_list_item_meta.py` & `textology-0.2.1/textology/widgets/_list_item_meta.py`

 * *Files identical despite different names*

### Comparing `textology-0.2.0/textology/widgets/_list_view.py` & `textology-0.2.1/textology/widgets/_list_view.py`

 * *Files identical despite different names*

### Comparing `textology-0.2.0/textology/widgets/_location.py` & `textology-0.2.1/textology/widgets/_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 import logging
 from typing import Any
 from urllib.parse import urlparse
 
 from textual import events
 from textual.message import Message
 from textual.reactive import reactive
+from textual.widget import Widget
 
 from textology.history import History
 from textology.router import Endpoint
 from textology.router import Request
 from textology.router import Router
 
-from ._extensions import ExtendedWidget
+from ._extensions import WidgetInitExtension
 
 
-class Location(ExtendedWidget, Router):
+class Location(WidgetInitExtension, Widget, Router):
     """Hidden widget containing representation of the current location of loaded resources.
 
     Intended to only be used for callbacks/routing/tracking requests.
     """
 
     class LocationMessage(Message):
         """Base class for Location messages."""
```

### Comparing `textology-0.2.0/textology/widgets/_modal_dialog.py` & `textology-0.2.1/textology/widgets/_modal_dialog.py`

 * *Files identical despite different names*

### Comparing `textology-0.2.0/textology/widgets/_static.py` & `textology-0.2.1/textology/widgets/_textual/_text_log.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,55 @@
-"""Extended Textual widget to display simple static content, or use as a base class for more complex widgets."""
-
-from __future__ import annotations
+"""Extended Textual TextLog widget."""
 
 from typing import Any
 
-from rich.console import RenderableType
 from textual import widgets
 
-from ._extensions import WidgetExtension
+from .._extensions import WidgetExtension
 
 
-class Static(WidgetExtension, widgets.Static):
-    """An extended widget to display simple static content, or use as a base class for more complex widgets."""
+class TextLog(WidgetExtension, widgets.TextLog):
+    """An extended widget for logging text."""
 
     def __init__(
         self,
-        renderable: RenderableType = "",
         *,
-        expand: bool = False,
-        shrink: bool = False,
-        markup: bool = True,
+        max_lines: int | None = None,
+        min_width: int = 78,
+        wrap: bool = False,
+        highlight: bool = False,
+        markup: bool = False,
+        auto_scroll: bool = True,
         name: str | None = None,
         id: str | None = None,
         classes: str | None = None,
         disabled: bool = False,
         **extension_configs: Any,
     ) -> None:
-        """Initialize a Static widget with extension arguments.
+        """Initialize a TextLog widget.
 
         Args:
-            renderable: A Rich renderable, or string containing console markup.
-            expand: Expand content if required to fill container.
-            shrink: Shrink content if required to fill container.
-            markup: True if markup should be parsed and rendered.
-            name: Name of widget.
-            id: ID of Widget.
-            classes: Space separated list of class names.
-            disabled: Whether the static is disabled or not.
+            max_lines: Maximum number of lines in the log or `None` for no maximum.
+            min_width: Minimum width of renderables.
+            wrap: Enable word wrapping (default is off).
+            highlight: Automatically highlight content.
+            markup: Apply Rich console markup.
+            auto_scroll: Enable automatic scrolling to end.
+            name: The name of the text log.
+            id: The ID of the text log in the DOM.
+            classes: The CSS classes of the text log.
+            disabled: Whether the text log is disabled or not.
             extension_configs: Widget extension configurations, such as dynamically provided local callbacks by name.
         """
         super().__init__(
-            renderable,
-            expand=expand,
-            shrink=shrink,
+            max_lines=max_lines,
+            min_width=min_width,
+            wrap=wrap,
+            highlight=highlight,
             markup=markup,
+            auto_scroll=auto_scroll,
             name=name,
             id=id,
             classes=classes,
             disabled=disabled,
         )
         self.__extend_widget__(**extension_configs)
```

### Comparing `textology-0.2.0/textology/widgets/_store.py` & `textology-0.2.1/textology/widgets/_store.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Widget container for basic data storage and sharing between callbacks."""
 
 import time
 from typing import Any
 from typing import TypeVar
 
 from textual.reactive import reactive
+from textual.widget import Widget
 
-from ._extensions import ExtendedWidget
+from ._extensions import WidgetInitExtension
 
 JsonType = TypeVar("JsonType", dict, list, bool, float, int, str, None)  # Custom type. pylint: disable=invalid-name
 
 
-class Store(ExtendedWidget):
+class Store(WidgetInitExtension, Widget):
     """Hidden widget for basic data storage.
 
     Intended to only be used for sharing data between callbacks.
     """
 
     DEFAULT_CSS = """
     Store {
```

### Comparing `textology-0.2.0/textology.egg-info/PKG-INFO` & `textology-0.2.1/textology.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textology
-Version: 0.2.0
+Version: 0.2.1
 Summary: Textual extensions for creating Terminal User Interfaces
 Home-page: https://github.com/dfrtz/textology
 Author: David Fritz
 License: MIT
 Project-URL: Issue Tracker, https://github.com/dfrtz/textology/issues
 Project-URL: Source Code, https://github.com/dfrtz/textology
 Platform: MacOS
@@ -38,23 +38,23 @@
   <img src="https://raw.githubusercontent.com/dfrtz/textology/main/docs/banner.svg" width="450">
 </div>
 
 -----------------
 
 
 [![os: windows mac linux](https://img.shields.io/badge/os-linux_|_macos_|_windows-blue)](https://docs.python.org/3.10/)
-[![python: 3.10+](https://img.shields.io/badge/python-3.10_|_3.11-blue)](https://docs.python.org/3.10/)
+[![python: 3.10+](https://img.shields.io/badge/python-3.10_|_3.11-blue)](https://devguide.python.org/versions)
 [![python style: google](https://img.shields.io/badge/python%20style-google-blue)](https://google.github.io/styleguide/pyguide.html)
-[![imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://github.com/PyCQA/isort)
 [![code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![code style: pycodestyle](https://img.shields.io/badge/code%20style-pycodestyle-green)](https://github.com/PyCQA/pycodestyle)
 [![doc style: pydocstyle](https://img.shields.io/badge/doc%20style-pydocstyle-green)](https://github.com/PyCQA/pydocstyle)
 [![static typing: mypy](https://img.shields.io/badge/static_typing-mypy-green)](https://github.com/python/mypy)
 [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/PyCQA/pylint)
-[![testing: pytest](https://img.shields.io/badge/testing-pytest-yellowgreen)](https://github.com/PyCQA/pylint)
+[![testing: pytest](https://img.shields.io/badge/testing-pytest-yellowgreen)](https://github.com/pytest-dev/pytest)
 [![security: bandit](https://img.shields.io/badge/security-bandit-black)](https://github.com/PyCQA/bandit)
 [![license: MIT](https://img.shields.io/badge/license-MIT-lightgrey)](LICENSE)
 
 
 # Textology
 
 ### The study of making interactive UIs with text.
```

