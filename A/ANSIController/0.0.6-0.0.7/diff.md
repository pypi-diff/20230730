# Comparing `tmp/ANSIController-0.0.6.tar.gz` & `tmp/ANSIController-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ANSIController-0.0.6.tar", last modified: Sun Jul 30 00:46:31 2023, max compression
+gzip compressed data, was "ANSIController-0.0.7.tar", last modified: Sun Jul 30 01:03:14 2023, max compression
```

## Comparing `ANSIController-0.0.6.tar` & `ANSIController-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 00:46:31.223211 ANSIController-0.0.6/
-drwxrwxrwx   0        0        0        0 2023-07-30 00:46:31.198929 ANSIController-0.0.6/ANSIController/
--rw-rw-rw-   0        0        0     3192 2023-07-30 00:44:24.000000 ANSIController-0.0.6/ANSIController/__init__.py
--rw-rw-rw-   0        0        0     2086 2023-07-30 00:44:20.000000 ANSIController-0.0.6/ANSIController/__main__.py
--rw-rw-rw-   0        0        0     2280 2023-07-29 12:47:36.000000 ANSIController-0.0.6/ANSIController/const.py
--rw-rw-rw-   0        0        0     8563 2023-07-29 23:05:34.000000 ANSIController-0.0.6/ANSIController/controls.py
--rw-rw-rw-   0        0        0     3737 2023-07-29 23:05:38.000000 ANSIController-0.0.6/ANSIController/tcolor.py
--rw-rw-rw-   0        0        0      279 2023-07-29 23:05:42.000000 ANSIController-0.0.6/ANSIController/tparser.py
--rw-rw-rw-   0        0        0     2993 2023-07-29 23:05:48.000000 ANSIController-0.0.6/ANSIController/tstyles.py
-drwxrwxrwx   0        0        0        0 2023-07-30 00:46:31.222229 ANSIController-0.0.6/ANSIController.egg-info/
--rw-rw-rw-   0        0        0     9221 2023-07-30 00:46:31.000000 ANSIController-0.0.6/ANSIController.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-07-30 00:46:31.000000 ANSIController-0.0.6/ANSIController.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 00:46:31.000000 ANSIController-0.0.6/ANSIController.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-07-30 00:46:31.000000 ANSIController-0.0.6/ANSIController.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-07-30 00:46:31.000000 ANSIController-0.0.6/ANSIController.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-30 00:46:31.000000 ANSIController-0.0.6/ANSIController.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1069 2023-07-29 10:09:04.000000 ANSIController-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     9221 2023-07-30 00:46:31.224187 ANSIController-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     8461 2023-07-30 00:46:10.000000 ANSIController-0.0.6/README.md
--rw-rw-rw-   0        0        0       86 2023-07-30 00:46:31.225163 ANSIController-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1381 2023-07-30 00:45:09.000000 ANSIController-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 01:03:14.612609 ANSIController-0.0.7/
+drwxrwxrwx   0        0        0        0 2023-07-30 01:03:14.579689 ANSIController-0.0.7/ANSIController/
+-rw-rw-rw-   0        0        0     3196 2023-07-30 00:55:06.000000 ANSIController-0.0.7/ANSIController/__init__.py
+-rw-rw-rw-   0        0        0     2268 2023-07-30 01:02:26.000000 ANSIController-0.0.7/ANSIController/__main__.py
+-rw-rw-rw-   0        0        0     2280 2023-07-29 12:47:36.000000 ANSIController-0.0.7/ANSIController/const.py
+-rw-rw-rw-   0        0        0     8563 2023-07-29 23:05:34.000000 ANSIController-0.0.7/ANSIController/controls.py
+-rw-rw-rw-   0        0        0     3737 2023-07-29 23:05:38.000000 ANSIController-0.0.7/ANSIController/tcolor.py
+-rw-rw-rw-   0        0        0      279 2023-07-29 23:05:42.000000 ANSIController-0.0.7/ANSIController/tparser.py
+-rw-rw-rw-   0        0        0     2993 2023-07-29 23:05:48.000000 ANSIController-0.0.7/ANSIController/tstyles.py
+drwxrwxrwx   0        0        0        0 2023-07-30 01:03:14.610650 ANSIController-0.0.7/ANSIController.egg-info/
+-rw-rw-rw-   0        0        0     9221 2023-07-30 01:03:14.000000 ANSIController-0.0.7/ANSIController.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-07-30 01:03:14.000000 ANSIController-0.0.7/ANSIController.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 01:03:14.000000 ANSIController-0.0.7/ANSIController.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-07-30 01:03:14.000000 ANSIController-0.0.7/ANSIController.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-07-30 01:03:14.000000 ANSIController-0.0.7/ANSIController.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-30 01:03:14.000000 ANSIController-0.0.7/ANSIController.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1069 2023-07-29 10:09:04.000000 ANSIController-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     9221 2023-07-30 01:03:14.613587 ANSIController-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     8461 2023-07-30 00:46:10.000000 ANSIController-0.0.7/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-30 01:03:14.616456 ANSIController-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1381 2023-07-30 01:03:07.000000 ANSIController-0.0.7/setup.py
```

### Comparing `ANSIController-0.0.6/ANSIController/__init__.py` & `ANSIController-0.0.7/ANSIController/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         return _PARSER.get_color(char,style,bg)
     def get_reset(self) -> str:
         return _RESET
     @staticmethod
     def game(row:int=40,col:int=40,move_steps:int=1):
         control = Terminal()
         for r in range(row):
-            print("|"+'-'*col)
+            print("|"+'-'*col+"|")
         while True:
             try:
                 if keyboard.is_pressed('up'):
                     control.move_to_up(move_steps)
                 if keyboard.is_pressed("down"):
                     control.move_to_down(move_steps)
                 if keyboard.is_pressed("left"):
```

### Comparing `ANSIController-0.0.6/ANSIController/__main__.py` & `ANSIController-0.0.7/ANSIController/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,21 +20,22 @@
 ║╔═╗║║░║║║╚═╝╠╣╠╦╣╠╗
 ╚╝░╚╩╝░╚═╩═══╩══╩══╝{t.get_reset()}
 -----------------------
 by {t.get_color('red',1)}{__author__}{t.get_reset()}
 -----------------------
 [1] Print ALL Colors
 [2] Print ALL Styles
-[3] Colors With Styles
-[4] Print All
-[5] X O   # soon 
-[6] Snake # soon
-[7] Move Game
-[8] Colorize Text
-[9] Clear Screen
+[3] Print Colors With Styles
+[4] Print IDs
+[5] Print All
+[6] X O   # soon 
+[7] Snake # soon
+[8] Move Game
+[9] Colorize Text
+[10] Clear Screen
 [-1] End
 -----------------------
 >>> 
 -----------------------""")
         t.force_move_to_up()
         t.move_to_left(50)
         # t.move_to_up(start_line=True)
@@ -45,25 +46,30 @@
         if choice == "2":
             t.print_styles()
             input()
         if choice == "3":
             t.print_colors_styles()
             input()
         if choice == "4":
+            t.print_id_colors()
+            input()
+        if choice == "5":
             t.print_test()
             input()
-        if choice == "7":
-            t.game(100,100,2)
         if choice == "8":
-            text = str(input("Text `[your_color_code]`: "))
+            t.game(60,60,2)
+        if choice == "9":
+            text = str(input(f"Text `[your_color_code]`: {t.get_color('green')}"))
+            t.get_reset()
             t.print_colorize(text)
             input()
-        if choice == "9":
+        if choice == "10":
             t.clear_screen()
         if choice == '-1':
-            _print("Thx For Using Bye\n")
+            t.clear_line()
+            _print("\nThx For Using Bye\n")
             break
 if __name__ == '__main__':
     try:
         main()
     except:
         pass
```

### Comparing `ANSIController-0.0.6/ANSIController/const.py` & `ANSIController-0.0.7/ANSIController/const.py`

 * *Files identical despite different names*

### Comparing `ANSIController-0.0.6/ANSIController/controls.py` & `ANSIController-0.0.7/ANSIController/controls.py`

 * *Files identical despite different names*

### Comparing `ANSIController-0.0.6/ANSIController/tcolor.py` & `ANSIController-0.0.7/ANSIController/tcolor.py`

 * *Files identical despite different names*

### Comparing `ANSIController-0.0.6/ANSIController/tstyles.py` & `ANSIController-0.0.7/ANSIController/tstyles.py`

 * *Files identical despite different names*

### Comparing `ANSIController-0.0.6/ANSIController.egg-info/PKG-INFO` & `ANSIController-0.0.7/ANSIController.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ANSIController
-Version: 0.0.6
+Version: 0.0.7
 Summary: Basic Python Module to control & color & style text in terminal
 Home-page: https://github.com/jo0x01/ansicontroller
 Author: JoOx01
 Author-email: forsell450@gmail.com
 License: MIT
 Keywords: ansi,terminal,ansi_terminal
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ANSIController-0.0.6/LICENSE` & `ANSIController-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ANSIController-0.0.6/PKG-INFO` & `ANSIController-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ANSIController
-Version: 0.0.6
+Version: 0.0.7
 Summary: Basic Python Module to control & color & style text in terminal
 Home-page: https://github.com/jo0x01/ansicontroller
 Author: JoOx01
 Author-email: forsell450@gmail.com
 License: MIT
 Keywords: ansi,terminal,ansi_terminal
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ANSIController-0.0.6/README.md` & `ANSIController-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ANSIController-0.0.6/setup.py` & `ANSIController-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 __author__ = "JoOx01"
 __pkg_name__ = "ANSIController"
-__version__ = "0.0.6"
+__version__ = "0.0.7"
 __desc__ = """Basic Python Module to control & color & style text in terminal"""
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name=__pkg_name__,
```

