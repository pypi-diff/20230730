# Comparing `tmp/ANSIController-1.0.4.tar.gz` & `tmp/ANSIController-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ANSIController-1.0.4.tar", last modified: Sun Jul 30 08:39:36 2023, max compression
+gzip compressed data, was "ANSIController-1.0.5.tar", last modified: Sun Jul 30 09:34:18 2023, max compression
```

## Comparing `ANSIController-1.0.4.tar` & `ANSIController-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 08:39:36.657753 ANSIController-1.0.4/
-drwxrwxrwx   0        0        0        0 2023-07-30 08:39:36.603018 ANSIController-1.0.4/ANSIController/
--rw-rw-rw-   0        0        0     3392 2023-07-30 08:38:55.000000 ANSIController-1.0.4/ANSIController/__init__.py
--rw-rw-rw-   0        0        0     2326 2023-07-30 08:38:42.000000 ANSIController-1.0.4/ANSIController/__main__.py
--rw-rw-rw-   0        0        0     2280 2023-07-29 12:47:36.000000 ANSIController-1.0.4/ANSIController/const.py
--rw-rw-rw-   0        0        0     8722 2023-07-30 08:39:03.000000 ANSIController-1.0.4/ANSIController/controls.py
--rw-rw-rw-   0        0        0     3776 2023-07-30 08:38:37.000000 ANSIController-1.0.4/ANSIController/tcolor.py
--rw-rw-rw-   0        0        0      457 2023-07-30 08:38:30.000000 ANSIController-1.0.4/ANSIController/tparser.py
--rw-rw-rw-   0        0        0     2993 2023-07-30 08:38:33.000000 ANSIController-1.0.4/ANSIController/tstyles.py
-drwxrwxrwx   0        0        0        0 2023-07-30 08:39:36.655747 ANSIController-1.0.4/ANSIController.egg-info/
--rw-rw-rw-   0        0        0    11509 2023-07-30 08:39:36.000000 ANSIController-1.0.4/ANSIController.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-07-30 08:39:36.000000 ANSIController-1.0.4/ANSIController.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 08:39:36.000000 ANSIController-1.0.4/ANSIController.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-07-30 08:39:36.000000 ANSIController-1.0.4/ANSIController.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-07-30 08:39:36.000000 ANSIController-1.0.4/ANSIController.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-30 08:39:36.000000 ANSIController-1.0.4/ANSIController.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1083 2023-07-30 01:37:14.000000 ANSIController-1.0.4/LICENSE
--rw-rw-rw-   0        0        0    11509 2023-07-30 08:39:36.657753 ANSIController-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    10524 2023-07-30 01:33:45.000000 ANSIController-1.0.4/README.md
--rw-rw-rw-   0        0        0       86 2023-07-30 08:39:36.659748 ANSIController-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1686 2023-07-30 08:39:14.000000 ANSIController-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 09:34:18.608361 ANSIController-1.0.5/
+drwxrwxrwx   0        0        0        0 2023-07-30 09:34:18.583765 ANSIController-1.0.5/ANSIController/
+-rw-rw-rw-   0        0        0     3415 2023-07-30 09:31:35.000000 ANSIController-1.0.5/ANSIController/__init__.py
+-rw-rw-rw-   0        0        0     2326 2023-07-30 08:38:42.000000 ANSIController-1.0.5/ANSIController/__main__.py
+-rw-rw-rw-   0        0        0     2280 2023-07-29 12:47:36.000000 ANSIController-1.0.5/ANSIController/const.py
+-rw-rw-rw-   0        0        0     8681 2023-07-30 09:32:45.000000 ANSIController-1.0.5/ANSIController/controls.py
+-rw-rw-rw-   0        0        0     3776 2023-07-30 08:38:37.000000 ANSIController-1.0.5/ANSIController/tcolor.py
+-rw-rw-rw-   0        0        0      457 2023-07-30 09:32:51.000000 ANSIController-1.0.5/ANSIController/tparser.py
+-rw-rw-rw-   0        0        0     2993 2023-07-30 08:38:33.000000 ANSIController-1.0.5/ANSIController/tstyles.py
+drwxrwxrwx   0        0        0        0 2023-07-30 09:34:18.607132 ANSIController-1.0.5/ANSIController.egg-info/
+-rw-rw-rw-   0        0        0    11509 2023-07-30 09:34:18.000000 ANSIController-1.0.5/ANSIController.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-07-30 09:34:18.000000 ANSIController-1.0.5/ANSIController.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 09:34:18.000000 ANSIController-1.0.5/ANSIController.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-07-30 09:34:18.000000 ANSIController-1.0.5/ANSIController.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-07-30 09:34:18.000000 ANSIController-1.0.5/ANSIController.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-30 09:34:18.000000 ANSIController-1.0.5/ANSIController.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1083 2023-07-30 01:37:14.000000 ANSIController-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0    11509 2023-07-30 09:34:18.608361 ANSIController-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    10524 2023-07-30 01:33:45.000000 ANSIController-1.0.5/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-30 09:34:18.610360 ANSIController-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1686 2023-07-30 09:34:10.000000 ANSIController-1.0.5/setup.py
```

### Comparing `ANSIController-1.0.4/ANSIController/__init__.py` & `ANSIController-1.0.5/ANSIController/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,16 +4,19 @@
 Basic Python Module to control & color & style text in terminal.
 Author: JoOx01
 Date: 2023-07-30
 License: MIT License
 """
 from time import sleep
 import keyboard
-from ANSIController.const import _256_FG,_256_BG,_1ATTR, _RESET, _print
-from ANSIController import _ColorsControls, _CursorControls
+from ANSIController.controls import _ColorsControls, _CursorControls
+from ANSIController.const import (
+    _print,_RESET,_1ATTR,_256_BG,
+    _256_FG
+)
 from ANSIController.tparser import _PARSER
 
 
 class Terminal(_CursorControls,_ColorsControls):
     __colors = _PARSER._COLORS
     __styles = _PARSER._STYLES
     def __init__(self) -> None:
```

### Comparing `ANSIController-1.0.4/ANSIController/__main__.py` & `ANSIController-1.0.5/ANSIController/__main__.py`

 * *Files identical despite different names*

### Comparing `ANSIController-1.0.4/ANSIController/const.py` & `ANSIController-1.0.5/ANSIController/const.py`

 * *Files identical despite different names*

### Comparing `ANSIController-1.0.4/ANSIController/controls.py` & `ANSIController-1.0.5/ANSIController/controls.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,21 +116,20 @@
             return _1ATTR.format(s=style)
         if colors[1]:
             return _2ATTR.format(s=colors[0],fg=colors[1])
         return _1ATTR.format(s=colors[0])
     def __replace(self,texts:list[str]) -> list[tuple]:
         data = []
         for text in texts:
-            if _PARSER._isKnown(text):
-                if text in ['[z]','[Z]','[0]','[reset]','[Reset]']:
-                    data.append((text,0,0))
-                else:
-                    t,style = _PARSER._extract_style(text)
-                    color = _PARSER._extract_color(t,any(char in "xX" for char in text))
-                    data.append((text,style,color))
+            if text in ['[z]','[Z]','[0]','[reset]','[Reset]']:
+                data.append((text,0,0))
+            elif _PARSER._isKnown(text):
+                t,style = _PARSER._extract_style(text)
+                color = _PARSER._extract_color(t,any(char in "xX" for char in text))
+                data.append((text,style,color))
             else:
                 data.append(text)
         return data
     def __swap(self,text:str,texts) -> str:
         texts = self.__replace(texts)
         for t in texts:
             if isinstance(t,tuple):
```

### Comparing `ANSIController-1.0.4/ANSIController/tcolor.py` & `ANSIController-1.0.5/ANSIController/tcolor.py`

 * *Files identical despite different names*

### Comparing `ANSIController-1.0.4/ANSIController/tstyles.py` & `ANSIController-1.0.5/ANSIController/tstyles.py`

 * *Files identical despite different names*

### Comparing `ANSIController-1.0.4/ANSIController.egg-info/PKG-INFO` & `ANSIController-1.0.5/ANSIController.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ANSIController
-Version: 1.0.4
+Version: 1.0.5
 Summary: Basic Python Module to control & color & style text in terminal
 Home-page: https://github.com/jo0x01/ansicontroller
 Author: JoOx01
 Author-email: forsell450@gmail.com
 License: MIT
 Keywords: ansi,terminal,ansi_terminal,ANSIControl,ANSIController,ASNI,ansicontroller
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ANSIController-1.0.4/LICENSE` & `ANSIController-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ANSIController-1.0.4/PKG-INFO` & `ANSIController-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ANSIController
-Version: 1.0.4
+Version: 1.0.5
 Summary: Basic Python Module to control & color & style text in terminal
 Home-page: https://github.com/jo0x01/ansicontroller
 Author: JoOx01
 Author-email: forsell450@gmail.com
 License: MIT
 Keywords: ansi,terminal,ansi_terminal,ANSIControl,ANSIController,ASNI,ansicontroller
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ANSIController-1.0.4/README.md` & `ANSIController-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ANSIController-1.0.4/setup.py` & `ANSIController-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 __author__ = "JoOx01"
 __pkg_name__ = "ANSIController"
-__version__ = "1.0.4"
+__version__ = "1.0.5"
 __desc__ = """Basic Python Module to control & color & style text in terminal"""
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name=__pkg_name__,
```

