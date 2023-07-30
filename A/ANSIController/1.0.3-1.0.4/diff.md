# Comparing `tmp/ANSIController-1.0.3.tar.gz` & `tmp/ANSIController-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ANSIController-1.0.3.tar", last modified: Sun Jul 30 01:34:17 2023, max compression
+gzip compressed data, was "ANSIController-1.0.4.tar", last modified: Sun Jul 30 08:39:36 2023, max compression
```

## Comparing `ANSIController-1.0.3.tar` & `ANSIController-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 01:34:17.747307 ANSIController-1.0.3/
-drwxrwxrwx   0        0        0        0 2023-07-30 01:34:17.723251 ANSIController-1.0.3/ANSIController/
--rw-rw-rw-   0        0        0     3401 2023-07-30 01:11:58.000000 ANSIController-1.0.3/ANSIController/__init__.py
--rw-rw-rw-   0        0        0     2341 2023-07-30 01:11:25.000000 ANSIController-1.0.3/ANSIController/__main__.py
--rw-rw-rw-   0        0        0     2280 2023-07-29 12:47:36.000000 ANSIController-1.0.3/ANSIController/const.py
--rw-rw-rw-   0        0        0     8563 2023-07-29 23:05:34.000000 ANSIController-1.0.3/ANSIController/controls.py
--rw-rw-rw-   0        0        0     3737 2023-07-29 23:05:38.000000 ANSIController-1.0.3/ANSIController/tcolor.py
--rw-rw-rw-   0        0        0      279 2023-07-29 23:05:42.000000 ANSIController-1.0.3/ANSIController/tparser.py
--rw-rw-rw-   0        0        0     2993 2023-07-29 23:05:48.000000 ANSIController-1.0.3/ANSIController/tstyles.py
-drwxrwxrwx   0        0        0        0 2023-07-30 01:34:17.746299 ANSIController-1.0.3/ANSIController.egg-info/
--rw-rw-rw-   0        0        0    11509 2023-07-30 01:34:17.000000 ANSIController-1.0.3/ANSIController.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-07-30 01:34:17.000000 ANSIController-1.0.3/ANSIController.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 01:34:17.000000 ANSIController-1.0.3/ANSIController.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-07-30 01:34:17.000000 ANSIController-1.0.3/ANSIController.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-07-30 01:34:17.000000 ANSIController-1.0.3/ANSIController.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-30 01:34:17.000000 ANSIController-1.0.3/ANSIController.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1069 2023-07-29 10:09:04.000000 ANSIController-1.0.3/LICENSE
--rw-rw-rw-   0        0        0    11509 2023-07-30 01:34:17.747307 ANSIController-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    10524 2023-07-30 01:33:45.000000 ANSIController-1.0.3/README.md
--rw-rw-rw-   0        0        0       86 2023-07-30 01:34:17.750278 ANSIController-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1686 2023-07-30 01:34:09.000000 ANSIController-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 08:39:36.657753 ANSIController-1.0.4/
+drwxrwxrwx   0        0        0        0 2023-07-30 08:39:36.603018 ANSIController-1.0.4/ANSIController/
+-rw-rw-rw-   0        0        0     3392 2023-07-30 08:38:55.000000 ANSIController-1.0.4/ANSIController/__init__.py
+-rw-rw-rw-   0        0        0     2326 2023-07-30 08:38:42.000000 ANSIController-1.0.4/ANSIController/__main__.py
+-rw-rw-rw-   0        0        0     2280 2023-07-29 12:47:36.000000 ANSIController-1.0.4/ANSIController/const.py
+-rw-rw-rw-   0        0        0     8722 2023-07-30 08:39:03.000000 ANSIController-1.0.4/ANSIController/controls.py
+-rw-rw-rw-   0        0        0     3776 2023-07-30 08:38:37.000000 ANSIController-1.0.4/ANSIController/tcolor.py
+-rw-rw-rw-   0        0        0      457 2023-07-30 08:38:30.000000 ANSIController-1.0.4/ANSIController/tparser.py
+-rw-rw-rw-   0        0        0     2993 2023-07-30 08:38:33.000000 ANSIController-1.0.4/ANSIController/tstyles.py
+drwxrwxrwx   0        0        0        0 2023-07-30 08:39:36.655747 ANSIController-1.0.4/ANSIController.egg-info/
+-rw-rw-rw-   0        0        0    11509 2023-07-30 08:39:36.000000 ANSIController-1.0.4/ANSIController.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-07-30 08:39:36.000000 ANSIController-1.0.4/ANSIController.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 08:39:36.000000 ANSIController-1.0.4/ANSIController.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-07-30 08:39:36.000000 ANSIController-1.0.4/ANSIController.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-07-30 08:39:36.000000 ANSIController-1.0.4/ANSIController.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-30 08:39:36.000000 ANSIController-1.0.4/ANSIController.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1083 2023-07-30 01:37:14.000000 ANSIController-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0    11509 2023-07-30 08:39:36.657753 ANSIController-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    10524 2023-07-30 01:33:45.000000 ANSIController-1.0.4/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-30 08:39:36.659748 ANSIController-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1686 2023-07-30 08:39:14.000000 ANSIController-1.0.4/setup.py
```

### Comparing `ANSIController-1.0.3/ANSIController/__init__.py` & `ANSIController-1.0.4/ANSIController/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Author: JoOx01
 Date: 2023-07-30
 License: MIT License
 """
 from time import sleep
 import keyboard
 from ANSIController.const import _256_FG,_256_BG,_1ATTR, _RESET, _print
-from ANSIController.controls import _ColorsControls, _CursorControls
+from ANSIController import _ColorsControls, _CursorControls
 from ANSIController.tparser import _PARSER
 
 
 class Terminal(_CursorControls,_ColorsControls):
     __colors = _PARSER._COLORS
     __styles = _PARSER._STYLES
     def __init__(self) -> None:
```

### Comparing `ANSIController-1.0.3/ANSIController/__main__.py` & `ANSIController-1.0.4/ANSIController/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 #!/data/data/com.termux/files/usr/bin/env python3
-from ANSIController.const import _print
+from const import _print
 from ANSIController import Terminal
 
 ## more info `https://gist.github.com/fnky/458719343aabd01cfb17a3a4f7296797#escape`
 
 __author__ = 'JoOx01'
 __desc__ = """Basic Python Module to control & color & style text in terminal"""
```

### Comparing `ANSIController-1.0.3/ANSIController/const.py` & `ANSIController-1.0.4/ANSIController/const.py`

 * *Files identical despite different names*

### Comparing `ANSIController-1.0.3/ANSIController/controls.py` & `ANSIController-1.0.4/ANSIController/controls.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,25 +116,29 @@
             return _1ATTR.format(s=style)
         if colors[1]:
             return _2ATTR.format(s=colors[0],fg=colors[1])
         return _1ATTR.format(s=colors[0])
     def __replace(self,texts:list[str]) -> list[tuple]:
         data = []
         for text in texts:
-            if text in ['[z]','[Z]','[0]','[reset]','[Reset]']:
-                data.append((text,0,0))
+            if _PARSER._isKnown(text):
+                if text in ['[z]','[Z]','[0]','[reset]','[Reset]']:
+                    data.append((text,0,0))
+                else:
+                    t,style = _PARSER._extract_style(text)
+                    color = _PARSER._extract_color(t,any(char in "xX" for char in text))
+                    data.append((text,style,color))
             else:
-                t,style = _PARSER._extract_style(text)
-                color = _PARSER._extract_color(t,any(char in "xX" for char in text))
-                data.append((text,style,color))
+                data.append(text)
         return data
     def __swap(self,text:str,texts) -> str:
         texts = self.__replace(texts)
         for t in texts:
-            text = text.replace(t[0],self.__get_colors_escape(t[1],t[2]))
+            if isinstance(t,tuple):
+                text = text.replace(t[0],self.__get_colors_escape(t[1],t[2]))
         return text
 
     def colorize(self,text:str,sep:str="[]") -> str:
         """
         ##### @text: text u want to colorize in terminal
         ##### @sep: set special code of colors styles `[]` `!$` `{}` `()` `$$` `??` `}{` and so on
         - ##### if terminal not support colorize the string will just remove from string
```

### Comparing `ANSIController-1.0.3/ANSIController/tcolor.py` & `ANSIController-1.0.4/ANSIController/tcolor.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 class _Colors:
     _COLORS:list[_Color] = [_Color(info) for info in _COLORS_CODES]
     __strings:list[str] = []
     def __init__(self) -> None:
         for _s in self._COLORS:
             self.__strings.extend(_s.chars)
         self.__strings.reverse()
+        self._colors = self.__strings
     def __color(self,char:str) -> _Color|None:
         for c in self._COLORS:
             if c.is_that_color(char):
                 return c
         return None
     def _extract_color(self,text:str,bg:bool) -> tuple:
         colors_pattern = re.compile(rf"({'|'.join(self.__strings)})")
```

### Comparing `ANSIController-1.0.3/ANSIController/tstyles.py` & `ANSIController-1.0.4/ANSIController/tstyles.py`

 * *Files identical despite different names*

### Comparing `ANSIController-1.0.3/ANSIController.egg-info/PKG-INFO` & `ANSIController-1.0.4/ANSIController.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ANSIController
-Version: 1.0.3
+Version: 1.0.4
 Summary: Basic Python Module to control & color & style text in terminal
 Home-page: https://github.com/jo0x01/ansicontroller
 Author: JoOx01
 Author-email: forsell450@gmail.com
 License: MIT
 Keywords: ansi,terminal,ansi_terminal,ANSIControl,ANSIController,ASNI,ansicontroller
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ANSIController-1.0.3/PKG-INFO` & `ANSIController-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ANSIController
-Version: 1.0.3
+Version: 1.0.4
 Summary: Basic Python Module to control & color & style text in terminal
 Home-page: https://github.com/jo0x01/ansicontroller
 Author: JoOx01
 Author-email: forsell450@gmail.com
 License: MIT
 Keywords: ansi,terminal,ansi_terminal,ANSIControl,ANSIController,ASNI,ansicontroller
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ANSIController-1.0.3/README.md` & `ANSIController-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ANSIController-1.0.3/setup.py` & `ANSIController-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 __author__ = "JoOx01"
 __pkg_name__ = "ANSIController"
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 __desc__ = """Basic Python Module to control & color & style text in terminal"""
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name=__pkg_name__,
```

