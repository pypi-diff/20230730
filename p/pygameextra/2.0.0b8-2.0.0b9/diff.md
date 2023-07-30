# Comparing `tmp/pygameextra-2.0.0b8.tar.gz` & `tmp/pygameextra-2.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygameextra-2.0.0b8.tar", last modified: Sun Jan  8 02:27:15 2023, max compression
+gzip compressed data, was "pygameextra-2.0.0b9.tar", last modified: Sun Jul 30 14:51:39 2023, max compression
```

## Comparing `pygameextra-2.0.0b8.tar` & `pygameextra-2.0.0b9.tar`

### file list

```diff
@@ -1,47 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-01-08 02:27:15.934906 pygameextra-2.0.0b8/
--rw-rw-rw-   0        0        0     1084 2022-09-12 20:52:41.000000 pygameextra-2.0.0b8/LICENSE
--rw-rw-rw-   0        0        0      529 2023-01-08 02:27:15.934906 pygameextra-2.0.0b8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-01-08 02:27:15.904572 pygameextra-2.0.0b8/pygameextra/
--rw-rw-rw-   0        0        0     2273 2022-10-28 14:57:44.000000 pygameextra-2.0.0b8/pygameextra/__init__.py
--rw-rw-rw-   0        0        0     3208 2023-01-08 00:57:06.000000 pygameextra-2.0.0b8/pygameextra/button.py
--rw-rw-rw-   0        0        0      732 2022-09-12 20:52:41.000000 pygameextra-2.0.0b8/pygameextra/colors.py
--rw-rw-rw-   0        0        0     4984 2022-10-29 10:43:49.000000 pygameextra-2.0.0b8/pygameextra/debug.py
--rw-rw-rw-   0        0        0    18693 2022-09-16 19:12:51.000000 pygameextra-2.0.0b8/pygameextra/display.py
--rw-rw-rw-   0        0        0     3108 2022-10-12 10:23:17.000000 pygameextra-2.0.0b8/pygameextra/draw.py
--rw-rw-rw-   0        0        0     2328 2023-01-08 01:48:23.000000 pygameextra-2.0.0b8/pygameextra/event.py
--rw-rw-rw-   0        0        0     1509 2022-09-12 20:52:41.000000 pygameextra-2.0.0b8/pygameextra/fill.py
--rw-rw-rw-   0        0        0     1419 2022-10-29 11:27:16.000000 pygameextra-2.0.0b8/pygameextra/fingersupport.py
--rw-rw-rw-   0        0        0    38624 2022-09-12 20:52:41.000000 pygameextra-2.0.0b8/pygameextra/font.ttf
--rw-rw-rw-   0        0        0     1899 2022-09-12 20:52:41.000000 pygameextra-2.0.0b8/pygameextra/fpslogger.py
--rw-rw-rw-   0        0        0      598 2022-09-12 20:52:41.000000 pygameextra-2.0.0b8/pygameextra/image.py
--rw-rw-rw-   0        0        0      617 2022-12-08 20:08:06.000000 pygameextra-2.0.0b8/pygameextra/math.py
--rw-rw-rw-   0        0        0     2710 2022-10-12 10:17:59.000000 pygameextra-2.0.0b8/pygameextra/modified.py
--rw-rw-rw-   0        0        0     2718 2022-10-29 11:33:22.000000 pygameextra-2.0.0b8/pygameextra/mouse.py
--rw-rw-rw-   0        0        0      145 2022-09-12 20:52:41.000000 pygameextra-2.0.0b8/pygameextra/pygame.py
--rw-rw-rw-   0        0        0     5159 2022-09-12 20:52:41.000000 pygameextra-2.0.0b8/pygameextra/recorder.py
--rw-rw-rw-   0        0        0      226 2022-09-12 20:52:41.000000 pygameextra-2.0.0b8/pygameextra/rect.py
--rw-rw-rw-   0        0        0      234 2022-09-12 20:52:41.000000 pygameextra-2.0.0b8/pygameextra/settings.py
--rw-rw-rw-   0        0        0     2084 2022-09-12 20:52:41.000000 pygameextra-2.0.0b8/pygameextra/sheet_handlers.py
--rw-rw-rw-   0        0        0      267 2022-09-12 20:52:41.000000 pygameextra-2.0.0b8/pygameextra/sorters.py
--rw-rw-rw-   0        0        0     2993 2022-10-12 10:21:04.000000 pygameextra-2.0.0b8/pygameextra/sprite.py
--rw-rw-rw-   0        0        0     1098 2022-09-12 20:52:41.000000 pygameextra-2.0.0b8/pygameextra/text.py
--rw-rw-rw-   0        0        0      343 2022-09-12 20:52:41.000000 pygameextra-2.0.0b8/pygameextra/time.py
--rw-rw-rw-   0        0        0      119 2023-01-08 02:20:02.000000 pygameextra-2.0.0b8/pygameextra/version.py
-drwxrwxrwx   0        0        0        0 2023-01-08 02:27:15.915703 pygameextra-2.0.0b8/pygameextra.egg-info/
--rw-rw-rw-   0        0        0      529 2023-01-08 02:27:15.000000 pygameextra-2.0.0b8/pygameextra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1044 2023-01-08 02:27:15.000000 pygameextra-2.0.0b8/pygameextra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-08 02:27:15.000000 pygameextra-2.0.0b8/pygameextra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2023-01-08 02:27:15.000000 pygameextra-2.0.0b8/pygameextra.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-01-08 02:27:15.000000 pygameextra-2.0.0b8/pygameextra.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-01-08 02:27:15.000000 pygameextra-2.0.0b8/pygameextra.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-01-08 02:27:15.932831 pygameextra-2.0.0b8/pygameextra_tester/
--rw-rw-rw-   0        0        0      353 2022-09-12 20:52:41.000000 pygameextra-2.0.0b8/pygameextra_tester/Xbutton.png
--rw-rw-rw-   0        0        0      548 2022-09-12 20:52:41.000000 pygameextra-2.0.0b8/pygameextra_tester/Ybutton.png
--rw-rw-rw-   0        0        0    12372 2022-10-29 10:43:16.000000 pygameextra-2.0.0b8/pygameextra_tester/__init__.py
--rw-rw-rw-   0        0        0     1297 2022-09-12 20:52:41.000000 pygameextra-2.0.0b8/pygameextra_tester/columns.png
--rw-rw-rw-   0        0        0      654 2022-09-12 20:52:41.000000 pygameextra-2.0.0b8/pygameextra_tester/debug_icon.png
--rw-rw-rw-   0        0        0      491 2022-09-12 20:52:41.000000 pygameextra-2.0.0b8/pygameextra_tester/mario_01.png
--rw-rw-rw-   0        0        0     2194 2022-09-12 20:52:41.000000 pygameextra-2.0.0b8/pygameextra_tester/mouse_middle.png
--rw-rw-rw-   0        0        0      332 2022-09-12 20:52:41.000000 pygameextra-2.0.0b8/pygameextra_tester/rows.png
--rw-rw-rw-   0        0        0       42 2023-01-08 02:27:15.935945 pygameextra-2.0.0b8/setup.cfg
--rw-rw-rw-   0        0        0     1136 2023-01-08 02:20:02.000000 pygameextra-2.0.0b8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:51:39.209650 pygameextra-2.0.0b9/
+-rw-rw-rw-   0        0        0     1084 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/LICENSE
+-rw-rw-rw-   0        0        0      530 2023-07-30 14:51:39.209650 pygameextra-2.0.0b9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-30 14:51:39.131538 pygameextra-2.0.0b9/pygameextra/
+-rw-rw-rw-   0        0        0     2295 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/__init__.py
+-rw-rw-rw-   0        0        0     3393 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/button.py
+-rw-rw-rw-   0        0        0     1002 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/colors.py
+-rw-rw-rw-   0        0        0     4998 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/debug.py
+-rw-rw-rw-   0        0        0    18693 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/display.py
+-rw-rw-rw-   0        0        0     3108 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/draw.py
+-rw-rw-rw-   0        0        0     2533 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/event.py
+-rw-rw-rw-   0        0        0     1509 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/fill.py
+-rw-rw-rw-   0        0        0     1419 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/fingersupport.py
+-rw-rw-rw-   0        0        0    38624 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/font.ttf
+-rw-rw-rw-   0        0        0     2324 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/fpslogger.py
+-rw-rw-rw-   0        0        0      598 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/image.py
+-rw-rw-rw-   0        0        0     4015 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/infinitygrid.py
+-rw-rw-rw-   0        0        0      617 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/math.py
+-rw-rw-rw-   0        0        0     2710 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/modified.py
+-rw-rw-rw-   0        0        0     2812 2023-02-01 15:24:48.000000 pygameextra-2.0.0b9/pygameextra/mouse.py
+-rw-rw-rw-   0        0        0     6747 2023-07-30 14:49:17.000000 pygameextra-2.0.0b9/pygameextra/pnzc.py
+-rw-rw-rw-   0        0        0      145 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/pygame.py
+-rw-rw-rw-   0        0        0     5159 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/recorder.py
+-rw-rw-rw-   0        0        0      226 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/rect.py
+-rw-rw-rw-   0        0        0      568 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/settings.py
+-rw-rw-rw-   0        0        0     2084 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/sheet_handlers.py
+-rw-rw-rw-   0        0        0     1477 2023-01-29 12:06:34.000000 pygameextra-2.0.0b9/pygameextra/smooth.py
+-rw-rw-rw-   0        0        0      267 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/sorters.py
+-rw-rw-rw-   0        0        0     2993 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/sprite.py
+-rw-rw-rw-   0        0        0     1098 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/text.py
+-rw-rw-rw-   0        0        0      343 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/time.py
+-rw-rw-rw-   0        0        0      119 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/version.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:51:39.162776 pygameextra-2.0.0b9/pygameextra.egg-info/
+-rw-rw-rw-   0        0        0      530 2023-07-30 14:51:37.000000 pygameextra-2.0.0b9/pygameextra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1114 2023-07-30 14:51:37.000000 pygameextra-2.0.0b9/pygameextra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 14:51:37.000000 pygameextra-2.0.0b9/pygameextra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-07-30 14:51:37.000000 pygameextra-2.0.0b9/pygameextra.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-07-30 14:51:37.000000 pygameextra-2.0.0b9/pygameextra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-07-30 14:51:37.000000 pygameextra-2.0.0b9/pygameextra.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 14:51:39.209650 pygameextra-2.0.0b9/pygameextra_tester/
+-rw-rw-rw-   0        0        0      353 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra_tester/Xbutton.png
+-rw-rw-rw-   0        0        0      548 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra_tester/Ybutton.png
+-rw-rw-rw-   0        0        0    12382 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra_tester/__init__.py
+-rw-rw-rw-   0        0        0     1297 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra_tester/columns.png
+-rw-rw-rw-   0        0        0      654 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra_tester/debug_icon.png
+-rw-rw-rw-   0        0        0      491 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra_tester/mario_01.png
+-rw-rw-rw-   0        0        0     2194 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra_tester/mouse_middle.png
+-rw-rw-rw-   0        0        0      332 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra_tester/rows.png
+-rw-rw-rw-   0        0        0       42 2023-07-30 14:51:39.209650 pygameextra-2.0.0b9/setup.cfg
+-rw-rw-rw-   0        0        0     1137 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/setup.py
```

### Comparing `pygameextra-2.0.0b8/LICENSE` & `pygameextra-2.0.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b8/PKG-INFO` & `pygameextra-2.0.0b9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pygameextra
-Version: 2.0.0b8
-Summary: Pygame. Made easier
+Version: 2.0.0b9
+Summary: Pygame. Made easier.
 Author: Red
 Author-email: redtonehair@gmail.com
 Keywords: python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Pygame Extra is a mask for pygame,
```

### Comparing `pygameextra-2.0.0b8/pygameextra/__init__.py` & `pygameextra-2.0.0b9/pygameextra/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,28 +23,28 @@
 
 
 def start_debug(delete_after: bool = False, reactivate: bool = False):
     if not settings.debugger:
         return
     if not reactivate:
         settings.debugger.start_mouse_position = mouse.pos()
-        settings.debugger.start_enable_spoof = settings.enable_spoof
-        settings.debugger.start_mouse_position_spoof = settings.mouse_position
+        settings.debugger.start_enable_spoof = settings.spoof_enabled
+        settings.debugger.start_mouse_position_spoof = settings.spoof_mouse_position
     settings.debugger.reactivate_init = reactivate
-    settings.enable_spoof = False
+    settings.spoof_enabled = False
     settings.debugger.before_run()
     while settings.debugger.active:
         settings.debugger.update()
     settings.debugger.after_run()
     if settings.debugger.reactivate:
-        settings.enable_spoof = True
-        settings.mouse_position = settings.debugger.start_mouse_position
+        settings.spoof_enabled = True
+        settings.spoof_mouse_position = settings.debugger.start_mouse_position
     else:
-        settings.enable_spoof = settings.debugger.start_enable_spoof
-        settings.mouse_position = settings.debugger.start_mouse_position_spoof
+        settings.spoof_enabled = settings.debugger.start_enable_spoof
+        settings.spoof_mouse_position = settings.debugger.start_mouse_position_spoof
 
     if delete_after:
         del settings.debugger
         settings.debugger = None
     else:
         settings.debugger.reset()
```

### Comparing `pygameextra-2.0.0b8/pygameextra/button.py` & `pygameextra-2.0.0b9/pygameextra/button.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 import time
 from pygameextra import draw, mouse, math, display, settings, recorder
 from pygameextra.image import Image
 from pygameextra.rect import Rect
 from pygameextra.text import Text
 
 
-def lock():
+def button_lock():
+    if not settings.button_lock_enabled: return
     settings.button_lock = time.time()
 
 
+def hover_lock():
+    if not settings.hover_lock_enabled: return
+    settings.hover_lock = time.time()
+
+
 def rect(area: tuple, inactive_color: tuple, active_color: tuple, text: Text = None, hover_action: any = None, hover_data: any = None, action: any = None, data: any = None, disabled: [bool, tuple] = False):
     if disabled:
         if type(disabled) == bool:
             draw.rect(active_color, area)
         else:
             # noinspection PyTypeChecker
             draw.rect(disabled, area)
@@ -23,22 +29,22 @@
             recorder.record(recorder.Button(area, action, data))
         return
     mouse_rect = Rect(*mouse.pos(), 1, 1)
     button_rect = Rect(*area)
     if button_rect.colliderect(mouse_rect):
         draw.rect(active_color, area)
         if (not settings.button_lock) and action and mouse.clicked()[0]:
-            lock()
+            button_lock()
             if data is not None:
                 action(data)
             else:
                 action()
 
-        if (not settings.button_lock) and hover_action:
-            lock()
+        if (not settings.hover_lock) and hover_action:
+            hover_lock()
             if hover_data is not None:
                 hover_action(hover_data)
             else:
                 hover_action()
     else:
         draw.rect(inactive_color, area)
     if settings.recording:
@@ -68,15 +74,15 @@
     button_rect = Rect(*area)
     if button_rect.colliderect(mouse_rect):
         display.blit(active_image.surface, (
             area[0] + area[2]*.5 - active_image.size[0]*.5,
             area[1] + area[3]*.5 - active_image.size[1]*.5
         ))
         if (not settings.button_lock) and action and mouse.clicked()[0]:
-            lock()
+            button_lock()
             if data is not None:
                 action(data)
             else:
                 action()
     else:
         display.blit(inactive_image.surface, (
             area[0] + area[2]*.5 - inactive_image.size[0]*.5,
```

### Comparing `pygameextra-2.0.0b8/pygameextra/colors.py` & `pygameextra-2.0.0b9/pygameextra/colors.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,50 @@
 # RGB
+lightred = (200, 0, 0)
 red = (255, 0, 0)
 darkred = (155, 0, 0)
 verydarkred = (55, 0, 0)
 
+lightgreen = (0, 200, 0)
 green = (0, 255, 0)
 darkgreen = (0, 155, 0)
 verydarkgreen = (0, 55, 0)
 
+lightblue = (0, 0, 200)
 blue = (0, 0, 255)
 darkblue = (0, 0, 155)
 verydarkblue = (0, 0, 55)
 
 # Mixes
+lightyellow = (200, 200, 0)
 yellow = (255, 255, 0)
 darkyellow = (155, 155, 0)
 verydarkyellow = (55, 55, 0)
 
+lightaqua = (0, 200, 200)
 aqua = (0, 255, 255)
 darkaqua = (0, 155, 155)
 verydarkaqua = (0, 55, 55)
 
+lightpink = (200, 0, 200)
 pink = (255, 0, 255)
 darkpink = (155, 0, 155)
 verydarkpink = (55, 0, 55)
 
 # Monochrome
 black = (0, 0, 0)
 white = (255, 255, 255)
+
 lightgray = (200, 200, 200)
 gray = (100, 100, 100)
 darkgray = (50, 50, 50)
 verydarkgray = (25, 25, 25)
 
 # Pygame Extra, exclusive colors
 pge_dark = (47, 123, 189)
 pge_light = (150, 206, 255)
+
+# Legacy
+indigo = (75, 0, 130)
+purple = (128, 0, 128)
+violet = (138, 43, 226)
+lavender = (230, 230, 250)
```

### Comparing `pygameextra-2.0.0b8/pygameextra/debug.py` & `pygameextra-2.0.0b9/pygameextra/debug.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
                 display.get_width()*.5-self.target.size[0] * .5,
                 display.get_height()*.5-self.target.size[1] * .5
             )
         if not self.reactivate_init:
             self.draggable = mouse.Draggable(self.offset)
             settings.button_lock = False
         else:
-            button.lock()
+            button.button_lock()
 
 
 class FreeInteractMode(FreeMode):
     def after_update(self):
         mouse_rect = Rect(*mouse.pos(False), 1, 1)
         self.draggable.lock = False
         for item in settings.recording_data:
@@ -119,15 +119,15 @@
             elif type(item) == recorder.Button:
                 area = (item.area[0]+self.offset[0]+self.offset2[0], item.area[1]+self.offset[1]+self.offset2[1], item.area[2], item.area[3])
                 button_rect = Rect(*area)
                 if button_rect.colliderect(mouse_rect):
                     draw.rect(colors.green, area, 2)
                     self.draggable.lock = True
                     if (not settings.button_lock) and item.action and mouse.clicked(False)[0]:
-                        button.lock()
+                        button.button_lock()
                         if item.data is None:
                             item.action()
                         else:
                             item.action(item.data)
                         self.active = False
                         self.reactivate = True
                 elif not settings.button_lock:
```

### Comparing `pygameextra-2.0.0b8/pygameextra/display.py` & `pygameextra-2.0.0b9/pygameextra/display.py`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b8/pygameextra/draw.py` & `pygameextra-2.0.0b9/pygameextra/draw.py`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b8/pygameextra/event.py` & `pygameextra-2.0.0b9/pygameextra/event.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,34 +17,39 @@
 
 def resizeCheck() -> bool:
     return c.type == pygame.WINDOWRESIZED
 
 
 def buttonLocking() -> None:
     if settings.button_lock:
-        if time.time()-settings.button_lock >= settings.button_timeout_time:
+        if time.time()-settings.button_lock >= settings.button_lock_timeout_time:
             if settings.button_lock_hold:
-                #TODO: potential optimization avaliable
+                #TODO: potential optimization available
                 if not pygame.mouse.get_pressed()[0]:
                     settings.button_lock = None
             else:
                 settings.button_lock = None
+def hoverLocking() -> None:
+    if settings.hover_lock:
+        if time.time()-settings.hover_lock >= settings.hover_lock_timeout_time:
+            settings.hover_lock = None
 
 
 def resizeCheckAuto() -> None:
     info = resizeCheck()
     if info:
         display.display_reference.size = display.display_reference.surface.get_size()
     return info
 
 
 def rundown() -> None:
     global c, event_buffer
-    if not settings.enable_rundown: return
+    if not settings.rundown_enabled: return
     buttonLocking()
+    hoverLocking()
     for c in event_buffer:
         resizeCheckAuto()
 
 
 def get() -> list[pygame.event.Event]:
     global event_buffer
     event_buffer = pygame.event.get()
```

### Comparing `pygameextra-2.0.0b8/pygameextra/fill.py` & `pygameextra-2.0.0b9/pygameextra/fill.py`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b8/pygameextra/fingersupport.py` & `pygameextra-2.0.0b9/pygameextra/fingersupport.py`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b8/pygameextra/font.ttf` & `pygameextra-2.0.0b9/pygameextra/font.ttf`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b8/pygameextra/fpslogger.py` & `pygameextra-2.0.0b9/pygameextra/fpslogger.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,51 @@
 import time
 import os
 import pygame
 import pygameextra.time
 import pygameextra.display
 import pygameextra.colors as colors
 import pygameextra.recorder as recorder
+from pygameextra.modified import Surface
+from pygameextra.fill import transparency as fill_trans
 
 location = os.path.dirname(os.path.realpath(__file__))
 
 
 class Logger:
     surface = None
     watch = {}
     last_label = ''
-    total = 1
-    count = 1
+    total = 0
+    count = 0
 
     def __init__(self, font: str = os.path.join(location, 'font.ttf'), size: int = 15, position: tuple = None):
         self.font = pygame.font.Font(font, size)
         self.good = 50
         self.okay = 30
         self.pos = position
         self.clock = pygameextra.time.clock
         self.renderTime = time.time() - 2
 
     def render(self):
         recorder.comment(f"FPS logger : {self}")
         if time.time()-self.renderTime > 1:
             fps = self.clock.get_fps()
-            text = str(int(fps) or 'Pygame Extra - logger') + (f' / {int(self.total/self.count)}' if fps > 0 else '')
+            text = str(int(fps) or 'Pygame Extra ') + (f' / {int(self.total/self.count)}' if self.count > 0 else ' Loading...')
             if fps != 0:
                 self.total += fps
                 self.count += 1
+                if self.count > 20:
+                    self.total = fps
+                    self.count = 1
             self.surface = self.font.render(text, True, (20, 200, 20) if fps >= self.good else (200, 200, 20) if fps >= self.okay else (200, 20, 20) if fps != 0 else colors.pge_light, None if fps != 0 else colors.pge_dark)
+            back_surface = Surface(self.surface.get_size())
+            fill_trans(colors.black, 150, back_surface)
+            back_surface.stamp(self.surface)
+            self.surface = back_surface
             self.renderTime = time.time()
         pygameextra.display.blit(self.surface, self.pos or (
             10, pygameextra.display.get_height()-10-self.font.get_height()
         ))
         recorder.padding_comment()
 
     def resetwatch(self, label: str = 'stopwatch'):
```

### Comparing `pygameextra-2.0.0b8/pygameextra/image.py` & `pygameextra-2.0.0b9/pygameextra/image.py`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b8/pygameextra/math.py` & `pygameextra-2.0.0b9/pygameextra/math.py`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b8/pygameextra/modified.py` & `pygameextra-2.0.0b9/pygameextra/modified.py`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b8/pygameextra/mouse.py` & `pygameextra-2.0.0b9/pygameextra/mouse.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,62 +16,64 @@
 
 
 def icon(cursor_icon: pygame.cursors.Cursor = arrow):
     pygame.mouse.set_cursor(cursor_icon)
 
 
 def pos(spoof: bool = True):
-    if spoof and settings.enable_spoof:
-        return settings.mouse_position or pygame.mouse.get_pos()
+    if spoof and settings.spoof_enabled:
+        return settings.spoof_mouse_position or pygame.mouse.get_pos()
     return pygame.mouse.get_pos()
 
 
 def clicked(spoof: bool = True):
-    if spoof and settings.enable_spoof:
-        return settings.mouse_clicked or pygame.mouse.get_pressed()
+    if spoof and settings.spoof_enabled:
+        return settings.spoof_mouse_clicked or pygame.mouse.get_pressed()
     return pygame.mouse.get_pressed()
 
+def place(x, y):
+    return pygame.mouse.set_pos([x, y])
+
 
 class Draggable:
-    start_pos = (0, 0)
-    active = False
-    lock = False
-    scale_support = False
-    pos = (0, 0)
-    area = (0, 0)
-    rect = None
-    ltic = False
+    start_pos: tuple[int, int]
+    active: bool
+    lock: bool
+    scale_support: bool
+    pos: tuple[int, int]
+    area: [tuple[int, int], None]
+    rect: pygame.Rect
+    ltic: bool
+    move_multiplier: float
 
     def make_rect(self):
         if self.area:
             self.rect = Rect(*self.pos, *self.area)
 
-    def __init__(self, position: tuple, area: tuple = None, scale_support: bool = False):
+    def __init__(self, position: tuple[int, int], area: [tuple[int, int], None] = None, move_multiplier: [float, int] = 1):
         self.pos = position
         self.area = area
         self.lock = False
-        self.scale_support = scale_support
         self.make_rect()
+        self.rect = None
+        self.active = False
+        self.move_multiplier = move_multiplier
 
     def calculate(self):
         new_pos = self.pos
         current_pos = pos()
         difference = (current_pos[0] - self.start_pos[0], current_pos[1] - self.start_pos[1])
-        return new_pos[0] + difference[0], new_pos[1] + difference[1]
+        return new_pos[0] + difference[0] * self.move_multiplier, new_pos[1] + difference[1] * self.move_multiplier
 
     def check(self):
         """check(self) -> bool, tuple
         This function will check if the draggable is being moved and where it is"""
         if self.lock:
             return False, self.pos
 
-        if self.scale_support and len(fingersupport.fingers) > 1:
-            return self.scale_handle()
-
-
         self.make_rect()
         if self.rect:
             mouserect = Rect(*pos(), 1, 1)
             collide = self.rect.colliderect(mouserect) and not settings.button_lock
         else:
             collide = True
         if (collide and clicked()[0] and not self.ltic) and not self.active:
@@ -82,13 +84,8 @@
             self.ltic = clicked()[0]
             return True, self.calculate()
         elif not clicked()[0] and self.active:
             self.active = False
             self.pos = self.calculate()
 
         self.ltic = clicked()[0]
-        return False, self.pos
-
-
-    def scale_handle(self):
-
         return False, self.pos
```

### Comparing `pygameextra-2.0.0b8/pygameextra/recorder.py` & `pygameextra-2.0.0b9/pygameextra/recorder.py`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b8/pygameextra/sheet_handlers.py` & `pygameextra-2.0.0b9/pygameextra/sheet_handlers.py`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b8/pygameextra/sprite.py` & `pygameextra-2.0.0b9/pygameextra/sprite.py`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b8/pygameextra/text.py` & `pygameextra-2.0.0b9/pygameextra/text.py`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b8/pygameextra.egg-info/PKG-INFO` & `pygameextra-2.0.0b9/pygameextra.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pygameextra
-Version: 2.0.0b8
-Summary: Pygame. Made easier
+Version: 2.0.0b9
+Summary: Pygame. Made easier.
 Author: Red
 Author-email: redtonehair@gmail.com
 Keywords: python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Pygame Extra is a mask for pygame,
```

### Comparing `pygameextra-2.0.0b8/pygameextra.egg-info/SOURCES.txt` & `pygameextra-2.0.0b9/pygameextra.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -8,22 +8,25 @@
 pygameextra/draw.py
 pygameextra/event.py
 pygameextra/fill.py
 pygameextra/fingersupport.py
 pygameextra/font.ttf
 pygameextra/fpslogger.py
 pygameextra/image.py
+pygameextra/infinitygrid.py
 pygameextra/math.py
 pygameextra/modified.py
 pygameextra/mouse.py
+pygameextra/pnzc.py
 pygameextra/pygame.py
 pygameextra/recorder.py
 pygameextra/rect.py
 pygameextra/settings.py
 pygameextra/sheet_handlers.py
+pygameextra/smooth.py
 pygameextra/sorters.py
 pygameextra/sprite.py
 pygameextra/text.py
 pygameextra/time.py
 pygameextra/version.py
 pygameextra.egg-info/PKG-INFO
 pygameextra.egg-info/SOURCES.txt
```

### Comparing `pygameextra-2.0.0b8/pygameextra_tester/Ybutton.png` & `pygameextra-2.0.0b9/pygameextra_tester/Ybutton.png`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b8/pygameextra_tester/__init__.py` & `pygameextra-2.0.0b9/pygameextra_tester/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,19 +86,19 @@
 
 
 # Button function
 def set_test(data):
     global test
     test = data
     if "math_" in data:
-        settings.button_timeout_time = .2
+        settings.button_lock_timeout_time = .2
         settings.button_lock_hold = False
         pe.display.make((500, 500), "PGE Testing Utility", 1)
     else:
-        settings.button_timeout_time = .1
+        settings.button_lock_timeout_time = .1
         settings.button_lock_hold = True
         pe.display.make((500, 500), "PGE Testing Utility", 0)
 
 
 def set_lerplength(data):
     global lerplength
     lerplength = data
```

### Comparing `pygameextra-2.0.0b8/pygameextra_tester/columns.png` & `pygameextra-2.0.0b9/pygameextra_tester/columns.png`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b8/pygameextra_tester/debug_icon.png` & `pygameextra-2.0.0b9/pygameextra_tester/debug_icon.png`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b8/pygameextra_tester/mouse_middle.png` & `pygameextra-2.0.0b9/pygameextra_tester/mouse_middle.png`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b8/setup.py` & `pygameextra-2.0.0b9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
-version = '2.0.0b8'
-short = 'Pygame. Made easier'
+version = '2.0.0b9'
+short = 'Pygame. Made easier.'
 long = '''Pygame Extra is a mask for pygame, 
 you can easily make complex games and or apps with much less lines then you would of before, 
 Pygame Extra makes coding easier. 
 
 The online documentation can be found at: https://pygame-extra.readthedocs.io/en/latest/
 
 github: https://github.com/JustRedTTG/PGE'''
```

