# Comparing `tmp/fusion-engine-0.3.0.tar.gz` & `tmp/fusion-engine-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusion-engine-0.3.0.tar", last modified: Thu Jul 27 11:45:41 2023, max compression
+gzip compressed data, was "fusion-engine-1.0.0.tar", last modified: Sun Jul 30 15:34:16 2023, max compression
```

## Comparing `fusion-engine-0.3.0.tar` & `fusion-engine-1.0.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-27 11:45:41.697306 fusion-engine-0.3.0/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1071 2023-07-02 09:01:28.000000 fusion-engine-0.3.0/LICENCE.md
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5624 2023-07-27 11:45:41.695266 fusion-engine-0.3.0/PKG-INFO
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     4361 2023-07-27 11:30:38.000000 fusion-engine-0.3.0/README.md
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1667 2023-07-24 10:32:49.000000 fusion-engine-0.3.0/pyproject.toml
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     2326 2023-07-27 11:42:53.000000 fusion-engine-0.3.0/release.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       24 2023-07-27 11:27:36.000000 fusion-engine-0.3.0/requirements.txt
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       38 2023-07-27 11:45:41.697996 fusion-engine-0.3.0/setup.cfg
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     3447 2023-07-27 11:43:43.000000 fusion-engine-0.3.0/setup.py
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-27 11:45:41.549001 fusion-engine-0.3.0/src/
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-27 11:45:41.591516 fusion-engine-0.3.0/src/fusion_engine.egg-info/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5624 2023-07-27 11:45:41.000000 fusion-engine-0.3.0/src/fusion_engine.egg-info/PKG-INFO
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      925 2023-07-27 11:45:41.000000 fusion-engine-0.3.0/src/fusion_engine.egg-info/SOURCES.txt
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)        1 2023-07-27 11:45:41.000000 fusion-engine-0.3.0/src/fusion_engine.egg-info/dependency_links.txt
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       25 2023-07-27 11:45:41.000000 fusion-engine-0.3.0/src/fusion_engine.egg-info/requires.txt
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       13 2023-07-27 11:45:41.000000 fusion-engine-0.3.0/src/fusion_engine.egg-info/top_level.txt
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-27 11:45:41.594427 fusion-engine-0.3.0/src/fusionengine/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1155 2023-07-27 11:36:39.000000 fusion-engine-0.3.0/src/fusionengine/__init__.py
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-27 11:45:41.603417 fusion-engine-0.3.0/src/fusionengine/debugfiles/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)    64239 2023-07-07 11:13:39.000000 fusion-engine-0.3.0/src/fusionengine/debugfiles/fe.png
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-27 11:45:41.690706 fusion-engine-0.3.0/src/fusionengine/files/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     3974 2023-07-26 13:45:02.000000 fusion-engine-0.3.0/src/fusionengine/files/body.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1694 2023-07-25 14:30:48.000000 fusion-engine-0.3.0/src/fusionengine/files/color.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      458 2023-07-25 14:34:56.000000 fusion-engine-0.3.0/src/fusionengine/files/data.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      162 2023-07-25 14:35:08.000000 fusion-engine-0.3.0/src/fusionengine/files/debug.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     2753 2023-07-25 14:31:30.000000 fusion-engine-0.3.0/src/fusionengine/files/draw.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      370 2023-07-25 14:35:37.000000 fusion-engine-0.3.0/src/fusionengine/files/enums.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)    10776 2023-07-25 14:36:51.000000 fusion-engine-0.3.0/src/fusionengine/files/event.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      250 2023-07-25 14:37:33.000000 fusion-engine-0.3.0/src/fusionengine/files/exceptions.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      173 2023-07-25 14:37:50.000000 fusion-engine-0.3.0/src/fusionengine/files/fonts.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1073 2023-07-25 14:38:51.000000 fusion-engine-0.3.0/src/fusionengine/files/image.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      600 2023-07-27 10:17:15.000000 fusion-engine-0.3.0/src/fusionengine/files/imports.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)        0 2023-06-11 19:02:09.000000 fusion-engine-0.3.0/src/fusionengine/files/physics.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      692 2023-07-25 14:40:03.000000 fusion-engine-0.3.0/src/fusionengine/files/shape.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5576 2023-07-25 14:39:35.000000 fusion-engine-0.3.0/src/fusionengine/files/storage.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      929 2023-07-25 14:41:15.000000 fusion-engine-0.3.0/src/fusionengine/files/systems.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     4133 2023-07-25 14:43:59.000000 fusion-engine-0.3.0/src/fusionengine/files/ui.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      606 2023-07-27 10:15:35.000000 fusion-engine-0.3.0/src/fusionengine/files/vector.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     3440 2023-07-27 09:10:08.000000 fusion-engine-0.3.0/src/fusionengine/files/window.py
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-30 15:34:16.366888 fusion-engine-1.0.0/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1071 2023-07-02 09:01:28.000000 fusion-engine-1.0.0/LICENCE.md
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5888 2023-07-30 15:34:16.366455 fusion-engine-1.0.0/PKG-INFO
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     4625 2023-07-27 16:57:56.000000 fusion-engine-1.0.0/README.md
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1667 2023-07-24 10:32:49.000000 fusion-engine-1.0.0/pyproject.toml
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     2326 2023-07-27 11:42:53.000000 fusion-engine-1.0.0/release.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       16 2023-07-29 09:25:11.000000 fusion-engine-1.0.0/requirements.txt
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       38 2023-07-30 15:34:16.367018 fusion-engine-1.0.0/setup.cfg
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     2490 2023-07-27 11:51:55.000000 fusion-engine-1.0.0/setup.py
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-30 15:34:16.328548 fusion-engine-1.0.0/src/
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-30 15:34:16.342308 fusion-engine-1.0.0/src/fusion_engine.egg-info/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5888 2023-07-30 15:34:16.000000 fusion-engine-1.0.0/src/fusion_engine.egg-info/PKG-INFO
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      925 2023-07-30 15:34:16.000000 fusion-engine-1.0.0/src/fusion_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)        1 2023-07-30 15:34:16.000000 fusion-engine-1.0.0/src/fusion_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       17 2023-07-30 15:34:16.000000 fusion-engine-1.0.0/src/fusion_engine.egg-info/requires.txt
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       13 2023-07-30 15:34:16.000000 fusion-engine-1.0.0/src/fusion_engine.egg-info/top_level.txt
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-30 15:34:16.343337 fusion-engine-1.0.0/src/fusionengine/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      762 2023-07-30 15:33:45.000000 fusion-engine-1.0.0/src/fusionengine/__init__.py
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-30 15:34:16.344691 fusion-engine-1.0.0/src/fusionengine/debugfiles/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)    64239 2023-07-07 11:13:39.000000 fusion-engine-1.0.0/src/fusionengine/debugfiles/fe.png
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-30 15:34:16.365625 fusion-engine-1.0.0/src/fusionengine/files/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     3593 2023-07-28 15:12:56.000000 fusion-engine-1.0.0/src/fusionengine/files/body.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1694 2023-07-28 15:13:05.000000 fusion-engine-1.0.0/src/fusionengine/files/color.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      451 2023-07-28 15:13:01.000000 fusion-engine-1.0.0/src/fusionengine/files/data.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      162 2023-07-28 15:12:38.000000 fusion-engine-1.0.0/src/fusionengine/files/debug.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1764 2023-07-29 16:08:23.000000 fusion-engine-1.0.0/src/fusionengine/files/draw.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      374 2023-07-28 15:13:11.000000 fusion-engine-1.0.0/src/fusionengine/files/enums.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5093 2023-07-29 16:35:58.000000 fusion-engine-1.0.0/src/fusionengine/files/event.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      252 2023-07-28 14:45:31.000000 fusion-engine-1.0.0/src/fusionengine/files/exceptions.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      172 2023-07-28 16:40:29.000000 fusion-engine-1.0.0/src/fusionengine/files/fonts.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1035 2023-07-29 16:32:15.000000 fusion-engine-1.0.0/src/fusionengine/files/image.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      567 2023-07-29 16:44:06.000000 fusion-engine-1.0.0/src/fusionengine/files/imports.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)        0 2023-06-11 19:02:09.000000 fusion-engine-1.0.0/src/fusionengine/files/physics.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      695 2023-07-29 09:58:09.000000 fusion-engine-1.0.0/src/fusionengine/files/shape.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5586 2023-07-28 14:51:13.000000 fusion-engine-1.0.0/src/fusionengine/files/storage.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      144 2023-07-29 10:00:10.000000 fusion-engine-1.0.0/src/fusionengine/files/systems.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     4558 2023-07-28 14:51:19.000000 fusion-engine-1.0.0/src/fusionengine/files/ui.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      600 2023-07-28 14:51:26.000000 fusion-engine-1.0.0/src/fusionengine/files/vector.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     2580 2023-07-29 16:16:58.000000 fusion-engine-1.0.0/src/fusionengine/files/window.py
```

### Comparing `fusion-engine-0.3.0/LICENCE.md` & `fusion-engine-1.0.0/LICENCE.md`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.3.0/PKG-INFO` & `fusion-engine-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-engine
-Version: 0.3.0
+Version: 1.0.0
 Summary: A custom open-source game engine on Python and PySDL2, it's written in pure Python! It's easy and fast!
 Author-email: Dimkauzh <uzhdimka@gmail.com>
 License: LICENSE.md
 Keywords: game,python,gamedev,game-engine,sdl2,game-development,pure-python,sdl2-mixer,sdl2-ttf,sdl2-image,python-game,pysdl2,sdl2-library,python-game-library,python-game-engine,python-games
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -49,30 +49,40 @@
 
 ```bash
   pip install fusion-engine
 ```
 
 Our PyPI package is at this [link](<https://pypi.org/project/fusion-engine/>)
 
-### Latest build
+### Install from source
+
+if you want to install the package from source then you do it like this:
+
+```bash
+ git clone https://github.com/dimkauzh/fusion-engine.git
+ cd fusion-engine
+ python setup.py install
+```
+
+### Developer build
 
 if you want to get the latest changes then follow this instruction:
 
 ```bash
- git clone https://github.com/dimkauzh/fusion-engine
+ git clone https://github.com/dimkauzh/fusion-engine.git
  cd fusion-engine
- pip install -e .
+ python setup.py install_dev
 ```
 
 ### Run example
 
 If you want to run the example, then just run this command:
 
 ```bash
- git clone https://github.com/dimkauzh/fusion-engine
+ git clone https://github.com/dimkauzh/fusion-engine.git
  cd fusion-engine
  python examples/example1.py
 ```
 
 For different examples, you change the number to the number of the example file
 
 ## 👥 Community
@@ -85,14 +95,16 @@
 ### ❤️ Special thanks to these people
 
 - Zenthm (Contributing)
 - XCarCedo (Contributing)
 - Techsplosion (Bug hunter)
 - FBS_Gamer (Discord server)
 
+And our community of course!
+
 ## 📃 Documentation
 
 See at [our website](https://dimkauzh.github.io/fusion-engine/)
 
 ## 📯 Coming features
 
 ### 🛠️ Features we are working on
```

### Comparing `fusion-engine-0.3.0/README.md` & `fusion-engine-1.0.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -22,30 +22,40 @@
 
 ```bash
   pip install fusion-engine
 ```
 
 Our PyPI package is at this [link](<https://pypi.org/project/fusion-engine/>)
 
-### Latest build
+### Install from source
+
+if you want to install the package from source then you do it like this:
+
+```bash
+ git clone https://github.com/dimkauzh/fusion-engine.git
+ cd fusion-engine
+ python setup.py install
+```
+
+### Developer build
 
 if you want to get the latest changes then follow this instruction:
 
 ```bash
- git clone https://github.com/dimkauzh/fusion-engine
+ git clone https://github.com/dimkauzh/fusion-engine.git
  cd fusion-engine
- pip install -e .
+ python setup.py install_dev
 ```
 
 ### Run example
 
 If you want to run the example, then just run this command:
 
 ```bash
- git clone https://github.com/dimkauzh/fusion-engine
+ git clone https://github.com/dimkauzh/fusion-engine.git
  cd fusion-engine
  python examples/example1.py
 ```
 
 For different examples, you change the number to the number of the example file
 
 ## 👥 Community
@@ -58,14 +68,16 @@
 ### ❤️ Special thanks to these people
 
 - Zenthm (Contributing)
 - XCarCedo (Contributing)
 - Techsplosion (Bug hunter)
 - FBS_Gamer (Discord server)
 
+And our community of course!
+
 ## 📃 Documentation
 
 See at [our website](https://dimkauzh.github.io/fusion-engine/)
 
 ## 📯 Coming features
 
 ### 🛠️ Features we are working on
```

### Comparing `fusion-engine-0.3.0/pyproject.toml` & `fusion-engine-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.3.0/release.py` & `fusion-engine-1.0.0/release.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.3.0/src/fusion_engine.egg-info/PKG-INFO` & `fusion-engine-1.0.0/src/fusion_engine.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-engine
-Version: 0.3.0
+Version: 1.0.0
 Summary: A custom open-source game engine on Python and PySDL2, it's written in pure Python! It's easy and fast!
 Author-email: Dimkauzh <uzhdimka@gmail.com>
 License: LICENSE.md
 Keywords: game,python,gamedev,game-engine,sdl2,game-development,pure-python,sdl2-mixer,sdl2-ttf,sdl2-image,python-game,pysdl2,sdl2-library,python-game-library,python-game-engine,python-games
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -49,30 +49,40 @@
 
 ```bash
   pip install fusion-engine
 ```
 
 Our PyPI package is at this [link](<https://pypi.org/project/fusion-engine/>)
 
-### Latest build
+### Install from source
+
+if you want to install the package from source then you do it like this:
+
+```bash
+ git clone https://github.com/dimkauzh/fusion-engine.git
+ cd fusion-engine
+ python setup.py install
+```
+
+### Developer build
 
 if you want to get the latest changes then follow this instruction:
 
 ```bash
- git clone https://github.com/dimkauzh/fusion-engine
+ git clone https://github.com/dimkauzh/fusion-engine.git
  cd fusion-engine
- pip install -e .
+ python setup.py install_dev
 ```
 
 ### Run example
 
 If you want to run the example, then just run this command:
 
 ```bash
- git clone https://github.com/dimkauzh/fusion-engine
+ git clone https://github.com/dimkauzh/fusion-engine.git
  cd fusion-engine
  python examples/example1.py
 ```
 
 For different examples, you change the number to the number of the example file
 
 ## 👥 Community
@@ -85,14 +95,16 @@
 ### ❤️ Special thanks to these people
 
 - Zenthm (Contributing)
 - XCarCedo (Contributing)
 - Techsplosion (Bug hunter)
 - FBS_Gamer (Discord server)
 
+And our community of course!
+
 ## 📃 Documentation
 
 See at [our website](https://dimkauzh.github.io/fusion-engine/)
 
 ## 📯 Coming features
 
 ### 🛠️ Features we are working on
```

### Comparing `fusion-engine-0.3.0/src/fusion_engine.egg-info/SOURCES.txt` & `fusion-engine-1.0.0/src/fusion_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.3.0/src/fusionengine/__init__.py` & `fusion-engine-1.0.0/src/fusionengine/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,26 @@
 __author__ = "Dimkauzh"
-__version__ = "0.3.0"
+__version__ = "1.0.0"
 
-import fusionengine.files.systems as sysconfig
 from fusionengine.files.imports import *
+import fusionengine.files.systems as sysconfig
+
 
 class Main:
     def __init__(self):
-        """A class that contains all the functions and classes. You need to initialize this class to use the engine.
-        """
-        sdl2.SDL_Init(sdl2.SDL_INIT_VIDEO)
+        """A class that contains all the functions for the engine."""
+        pg.init()
+
         self.window = window.Window()
         self.color = color.Colors()
         self.colortools = color.ColorTools()
         self.event = event.Event()
         self.keys = event.Keys()
         self.draw = draw.Draw()
         self.image = image.Image()
-        self.body = body
+        # self.body = body
         self.system = sysconfig.System()
-        self.rendereroptions = sysconfig.RendererOptions()
         self.shape = shape.Shapes()
-        self.ui = ui.UI()
+        # self.ui = ui.UI()
         self.fonts = fonts.Fonts()
         self.debug = debug.DebugFiles()
         self.vector = vector.Vectors()
-
-    def quit(self, window):
-        """Quits the engine.
-
-        Args:
-            window: Your window
-        """
-        sdl2.SDL_DestroyRenderer(window.renderer)
-        sdl2.SDL_DestroyWindow(window.window)
-        del window
-        sdl2.SDL_Quit()
```

### Comparing `fusion-engine-0.3.0/src/fusionengine/debugfiles/fe.png` & `fusion-engine-1.0.0/src/fusionengine/debugfiles/fe.png`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.3.0/src/fusionengine/files/body.py` & `fusion-engine-1.0.0/src/fusionengine/files/body.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,92 +1,94 @@
 import fusionengine.files.data as data
 import fusionengine.files.window as window
 from fusionengine.files.enums import BodyType
 from fusionengine.files.imports import *
 import fusionengine.files.image as image_fe
 import fusionengine.files.draw as draw_fe
 
+
 class _RigidBody:
-    def __init__(self, window: window._CustomRenderer, x: int, y: int, width: int, height: int) -> None:
+    def __init__(
+        self, window: window._CustomRenderer, x: int, y: int, width: int, height: int
+    ) -> None:
         """A class that creates a new rigid body. (Not for the user)"""
         self._body = data._DataBodies(window, x, y, width, height)
         self.window = window
         self.x = x
         self.y = y
         self.width = width
         self.height = height
         self.body = self._body.body
         self.space = self._body.space
 
+
 class _StaticBody:
-    def __init__(self, window: window._CustomRenderer, x: int, y: int, width: int, height: int) -> None:
+    def __init__(
+        self, window: window._CustomRenderer, x: int, y: int, width: int, height: int
+    ) -> None:
         """A class that creates a new static body. (Not for the user)"""
         self._body = data._DataBodies(window, x, y, width, height)
         self.window = window
         self.x = x
         self.y = y
         self.width = width
         self.height = height
         self.body = self._body.body
         self.space = self._body.space
 
+
 class Entity:
-    def __init__(self, bodytype: str, window: window._CustomRenderer, x: int, y: int, width: int, height: int) -> None:
+    def __init__(
+        self, bodytype: str, window: window._CustomRenderer, x: int, y: int, width: int, height: int
+    ) -> None:
         """A class that creates a new entity."""
         self._addspace = []
         self.x = x
         self.y = y
         self.width = width
         self.height = height
         self.window = window
         self.gravity = 0
         self.image_fe = image_fe.Image()
         self.draw_fe = draw_fe.Draw()
 
         if bodytype == BodyType.RIGID_BODY:
-            self.body = _RigidBody(self.window,
-                                   self.x,
-                                   self.y,
-                                   self.width,
-                                   self.height
-                                   )
+            self.body = _RigidBody(self.window, self.x, self.y, self.width, self.height)
         else:
-            self.body = _StaticBody(self.window,
-                                    self.x,
-                                    self.y,
-                                    self.width,
-                                    self.height
-                                    )
+            self.body = _StaticBody(self.window, self.x, self.y, self.width, self.height)
         self._addspace.append(self.body.body)
         self._set_body_data(self.x, self.y, self.width, self.height, self.body.space)
         self.box = pymunk.Poly.create_box(self.body.body)
         self._addspace.append(self.box)
 
         self._addspaces()
 
-    def image(self, window: window._CustomRenderer, image_path: str, x: int, y: int, width: int, height: int) -> None:
+    def image(
+        self,
+        window: window._CustomRenderer,
+        image_path: str,
+        x: int,
+        y: int,
+        width: int,
+        height: int,
+    ) -> None:
         """Gives the entity an image and laters draws it on the screen."""
         drawimage = self.image_fe.open_image(window, image_path, x, y, width, height)
         self.image_fe.draw_image(drawimage)
         self.image_path = image_path
         self.window = window
         self.x = x
         self.y = y
         self.width = width
         self.height = height
 
     def new_rect(self, window: window._CustomRenderer, color: tuple) -> None:
         """Gives the entity a rectangle and later draws it on the screen."""
-        self.draw_fe.draw_rect(window,
-                      self.x,
-                      self.y,
-                      self.width,
-                      self.height,
-                      color
-                      )
+        self.draw_fe.draw_rect(window, self.x, self.y, self.width, self.height, color)
+
     def set_gravity(self, gravity: int) -> None:
         """Sets the gravity of the entity."""
         self.gravity = gravity
         self.body.space.gravity = self.gravity
 
     def set_mass(self, mass: int) -> None:
         """Sets the mass of the entity."""
```

### Comparing `fusion-engine-0.3.0/src/fusionengine/files/color.py` & `fusion-engine-1.0.0/src/fusionengine/files/color.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,16 @@
         self.IVORY = (255, 255, 240, 255)
         self.LAVENDER = (230, 230, 250, 255)
         self.MINT = (189, 252, 201, 255)
         self.SALMON = (250, 128, 114, 255)
         self.SCARLET = (255, 36, 0, 255)
         self.TOMATO = (255, 99, 71, 255)
 
+
 class ColorTools:
     def __init__(self):
         pass
 
     def hex_to_rgba(self, hex):
         """Converts (#)RRGGBB to [R, G, B, 255]."""
-        hex6 = hex.replace('#', '')
+        hex6 = hex.replace("#", "")
         return int(hex6[:2], 16), int(hex6[2:4], 16), int(hex6[4:6], 16), 255
-
```

### Comparing `fusion-engine-0.3.0/src/fusionengine/files/draw.py` & `fusion-engine-1.0.0/src/fusionengine/files/window.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,64 +1,91 @@
 import fusionengine.files.systems as sysconfig
-import fusionengine.files.window as window
-
 from fusionengine.files.imports import *
-import fusionengine.files.shape as shape
 
 
-class Draw:
+class _CustomRenderer:
+    def __init__(self, window: pg.Surface, title: str, width: int, height: int) -> None:
+        """A class that creates a new custom renderer. (Not for the user)
+
+        Args:
+            window (sdl2.SDL_CreateWindow): An created sdl2 window
+        """
+        self.window = window
+
+        self.title = title
+        self.width = width
+        self.height = height
+        self.size = (self.width, self.height)
+
+
+class Window:
     def __init__(self) -> None:
-        self.rendereroptions = sysconfig.RendererOptions()
+        """A class that contains all the window functions."""
+        self._running = False
+        self._fps = 60
+        self.clock = pg.time.Clock()
+
+    def new_window(self, title: str, width: int, height: int) -> _CustomRenderer:
+        """Creates a new window.
+
+        Args:
+            title (str): Your window title
+            width (int): Your window width
+            height (int): Your window height
+
+        Returns:
+            window: Custom window class with all you need features
+        """
+        try:
+            window_window = pg.display.set_mode((width, height))
+            pg.display.set_caption(title)
+            self._running = True
+            self.window = _CustomRenderer(window_window, title, width, height)
+
+        except Exception:
+            print("Error: Can't create a window.")
+
+        return self.window
+
+    def loop(self, your_loop) -> None:
+        """A while loop decorator function.
+
+        Args:
+            your_loop (callable): Your main loop function
+        """
+        while self.running(self.window):
+            your_loop()
+
+    def running(self, window: _CustomRenderer) -> bool:
+        """Returns if the window is running. Used for the main loop.
+
+        Args:
+            window: Your window
+
+        Returns:
+            bool: returns true if the window is running else false
+        """
+        self._refresh(window)
+        return self._running
+
+    def set_fps(self, fps: int) -> None:
+        """Sets the desired frames per second for the game loop.
+
+        Args:
+            fps (int): The desired frames per second
+        """
+        self._fps = fps
+
+    def _refresh(self, window: _CustomRenderer) -> None:
+        """Does all things for refreshing window. (Not for the user)
+
+        Args:
+            window: Your window
+        """
+
+        for event in pg.event.get():
+            if event.type == pg.QUIT:
+                self._running = False
 
-    def draw_line(self, window: window._CustomRenderer, x1: int, y1: int, x2: int, y2: int, color: tuple) -> None:
-        """Draws a line on the screen."""
-        sdl2.SDL_SetRenderDrawColor(window.renderer,
-                                    color[0],
-                                    color[1],
-                                    color[2],
-                                    color[3]
-                                    )
-
-        sdl2.SDL_RenderDrawLine(window.renderer, x1, y1, x2, y2)
-
-    def draw_line_rect(self, window: window._CustomRenderer, x: int, y: int, width: int, height: int, color: tuple) -> None:
-        """Draws a rectangle that exists of lines on the screen."""
-        rdr = window.renderer
-        self.draw_line(rdr, x, y, x + width, y, color)
-        self.draw_line(rdr, x, y + height, x + width, y + height, color)
-        self.draw_line(rdr, x, y, x, y + height, color)
-        self.draw_line(rdr, x + width, y, x + width, y + height, color)
-
-    def draw_rect(self, window: window._CustomRenderer, x: int, y: int, width: int, height: int, color: tuple) -> None:
-        """Draws a rectangle on the screen."""
-        sdl2.SDL_SetRenderDrawColor(window.renderer,
-                                color[0],
-                                color[1],
-                                color[2],
-                                color[3]
-                                )
-
-        rect = sdl2.SDL_Rect(x, y, width, height)
-        sdl2.SDL_RenderFillRect(window.renderer, rect)
-
-
-    def draw_own_rect(self, window: window._CustomRenderer, rect: shape._CustomShape) -> None:
-        """Draws your rectangle on the screen."""
-        sdl2.SDL_SetRenderDrawColor(window.renderer,
-                                    rect.color[0],
-                                    rect.color[1],
-                                    rect.color[2],
-                                    rect.color[3]
-                                    )
-
-        sdl2.SDL_RenderFillRect(window.renderer, rect.rect)
-
-    def set_background_color(self, window: window._CustomRenderer, color: tuple) -> None:
-        """Sets the background color of the screen."""
-        sdl2.SDL_SetRenderDrawColor(window.renderer,
-                                    color[0],
-                                    color[1],
-                                    color[2],
-                                    color[3]
-                                    )
+        pg.display.flip()
 
-        sdl2.SDL_RenderClear(window.renderer)
+        self.DELTATIME = self.clock.tick(self._fps)
```

### Comparing `fusion-engine-0.3.0/src/fusionengine/files/image.py` & `fusion-engine-1.0.0/src/fusionengine/files/image.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 from fusionengine.files.imports import *
 import fusionengine.files.window as window
 import fusionengine.files.shape as shape
 
+
 class _CustomImage:
-    def __init__(self, window: window._CustomRenderer, texture, rect: shape._CustomShape) -> None:
+    def __init__(self, window: window._CustomRenderer, texture, x: int, y: int) -> None:
         """A class that creates a new custom image. (Not for the user)"""
         self.window = window
-        self.renderer = window.renderer
         self.texture = texture
-        self.rect = rect
+        self.x = x
+        self.y = y
+
 
 class Image:
-    def open_image(self, window: window._CustomRenderer, image, x: int, y: int, width: int, height: int) -> _CustomImage:
+    def open_image(
+        self,
+        window: window._CustomRenderer,
+        image,
+        x: int,
+        y: int,
+        width: int,
+        height: int,
+    ) -> _CustomImage:
         """Opens an image. Can be later rendered with draw_image."""
-        image = sdl2.ext.load_image(image)
-        texture = sdl2.SDL_CreateTextureFromSurface(window.renderer, image)
-        rect = sdl2.SDL_Rect(x, y, width, height)
-        return _CustomImage(window, texture, rect)
+        texture = pg.image.load(image).convert()
+        texture = pg.transform.scale(texture, (width, height))
+        return _CustomImage(window, texture, x, y)
 
     def draw_image(self, image: _CustomImage) -> None:
         """Draws your image (opened with open_image) on the screen."""
-        sdl2.SDL_RenderCopy(image.renderer, image.texture, None, image.rect)
+        image.window.window.blit(image.texture, (image.x, image.y))
```

### Comparing `fusion-engine-0.3.0/src/fusionengine/files/imports.py` & `fusion-engine-1.0.0/src/fusionengine/files/imports.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-import warnings
+import os
 
-with warnings.catch_warnings():
-	warnings.simplefilter("ignore")
-	import sdl2
-	import sdl2.ext
+os.environ["PYGAME_HIDE_SUPPORT_PROMPT"] = "1"
+
+import pygame as pg
 
 import ctypes
 import time
 
 import pymunk
 
 import fusionengine.files.body as body
```

### Comparing `fusion-engine-0.3.0/src/fusionengine/files/shape.py` & `fusion-engine-1.0.0/src/fusionengine/files/shape.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from fusionengine.files.imports import *
 
+
 class _CustomShape:
     def __init__(self, x: int, y: int, width: int, height: int, color: tuple) -> None:
         """A class that creates a new custom shape. (Not for the user)"""
         self.x = x
         self.y = y
         self.width = width
         self.height = height
         self.color = color
-        self.rect = sdl2.SDL_Rect(x, y, width, height)
+        self.rect = rect = pg.Rect(x, y, width, height)
+
 
 class Shapes:
     def __init__(self) -> None:
         pass
 
     def new_rect(self, x: int, y: int, width: int, height: int, color: tuple) -> _CustomShape:
         """Creates a new rectangle. Can be later rendered with draw_own_rect."""
```

### Comparing `fusion-engine-0.3.0/src/fusionengine/files/storage.py` & `fusion-engine-1.0.0/src/fusionengine/files/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,61 @@
 import json
 import typing
 from pathlib import Path
 
 from fusionengine.files.exceptions import InvalidType, JsonStorageInvalidIndex
 
+
 class JsonStorage:
     """JsonStorage is a storage class for saving json databases, currently all data is loaded from
     disk and saved to memory when you done with the storage you can just save it to the disk file
     using save method
-    
+
     Attributes:
         file_path (str): The path to the storage file on disk
         storage (list): The storage variable saved to memory
     """
 
     def __init__(self, file_path: str):
         self.storage = []
         self.file_path = Path(file_path)
 
         if self.file_path.exists():
             with open(self.file_path, mode="r", encoding="utf8") as file:
                 self.storage = json.load(file)
+
     def insert(self, _dict: dict[typing.Any, typing.Any]) -> bool:
         try:
             if not isinstance(_dict, dict):
                 raise InvalidType(f"_dict excepted to be dict not {type(_dict)}")
 
             self.storage.append(_dict)
             return True
         except Exception:
             return False
-    def search(self, search_dict: dict[typing.Any, typing.Any],
+
+    def search(
+        self,
+        search_dict: dict[typing.Any, typing.Any],
         first: bool = False,
-        get_index: bool = False) -> typing.Union[dict, list, tuple, None]:
+        get_index: bool = False,
+    ) -> typing.Union[dict, list, tuple, None]:
         """Search for a entry based on the search_dict
-        
+
         Args:
             search_dict (dict): search_dict is a dictionary describing keys:values to search for
             in the entries
             first (bool, optional): only return the first result that found
             nested_search (bool, optional): if its true if will search for keys and values
             based on search_dict in nested data structures (like another dictionary in the
             parent main dict entry)
-        
+
         Returns:
             typing.Union[dict, list, tuple, None]: The entries that found if
-            first is False otherwise the first entry that found 
+            first is False otherwise the first entry that found
             if get_index is true then it will return a tuple
             containing two values which being the index of the entry
             aside the value of it(returns None if nothing found)
         """
         if first:
             # Only search for the first entry
             for index, entry in enumerate(self.storage):
@@ -64,77 +70,82 @@
                         return entry
         else:
             # Search for all entries
             founded_entries = []
             for index, entry in enumerate(self.storage):
                 passed_every_search = True
                 for sk, sv in search_dict.items():
-
                     if entry.get(sk) != sv:
                         passed_every_search = False
                 if passed_every_search:
                     if get_index:
                         founded_entries.append((entry, index))
                     else:
                         founded_entries.append(entry)
             return founded_entries
+
     def update(self, index: int, new_entry: dict[typing.Any, typing.Any]) -> bool:
         """Update the entry based on the index to new_dict
-        
+
         Args:
             index (int): The index of the entry you want to update
             new_entry (dict): The new updated entry
-        
+
         Returns:
             bool: Wether the action was successful or not
-        
+
         Raises:
             InvalidType: In case the index parameter is not an integer or new_entry
             is not a dict
             JsonStorageInvalidIndex: In case the index is out of range and couldn't be find
             in the entries
         """
         if not isinstance(index, int):
             raise InvalidType(f"index excepted to be integer not {type(index)}")
         if not isinstance(new_entry, dict):
             raise InvalidType(f"new_entry excepted to be dict not {type(new_entry)}")
         try:
             self.storage[index] = new_entry
             return True
         except IndexError:
-            raise JsonStorageInvalidIndex("Invalid index, couldn't find the index in entries")
+            raise JsonStorageInvalidIndex(
+                "Invalid index, couldn't find the index in entries"
+            )
         except:
             return False
-    def delete(self, index: int) -> bool:
 
+    def delete(self, index: int) -> bool:
         """Delete an entry based on the index given
-        
+
         Args:
             index (int): The index of the entry you want to delete
-        
+
         Returns:
             bool: Wether the action was successful or not
-        
+
         Raises:
             InvalidType: In case the index parameter is not an integer
             JsonStorageInvalidIndex: In case the index is out of range and couldn't be find
             in the entries
         """
         if not isinstance(index, int):
             raise InvalidType(f"index excepted to be integer not {type(index)}")
         try:
             del self.storage[index]
             return True
         except IndexError:
-            raise JsonStorageInvalidIndex("Invalid index, couldn't find the index in entries")
+            raise JsonStorageInvalidIndex(
+                "Invalid index, couldn't find the index in entries"
+            )
         except:
             return False
+
     def save(self) -> bool:
         """Saves the storage variable into disk
-        
+
         Returns:
             bool: Wether the action was successful or not
         """
         try:
             with open(self.file_path, mode="w", encoding="utf8") as file:
                 json.dump(self.storage, file)
             return True
```

### Comparing `fusion-engine-0.3.0/src/fusionengine/files/ui.py` & `fusion-engine-1.0.0/src/fusionengine/files/ui.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 from fusionengine.files.imports import *
 import fusionengine.files.draw as draw
 import fusionengine.files.window as windowfe
 
 
 class _CustomButton:
-    def __init__(self, window: window._CustomRenderer, text: str, x: int, y: int, width: int, height: int, font_path: str, font_sharp: int, centre: int, color_input: tuple) -> None:
+    def __init__(
+        self,
+        window: window._CustomRenderer,
+        text: str,
+        x: int,
+        y: int,
+        width: int,
+        height: int,
+        font_path: str,
+        font_sharp: int,
+        centre: int,
+        color_input: tuple,
+    ) -> None:
         """A class that creates a new custom button. (Not for the user)"""
         self.window: windowfe._CustomRenderer = window
         self.text: str = text
         self.x: int = x
         self.y: int = y
         self.width = width
         self.height = height
@@ -23,30 +35,39 @@
             font_size = font_sharp
 
         draw.Draw().draw_rect(window, x, y, width, height, self.color)
 
         sdl2.sdlttf.TTF_Init()
         self.font = sdl2.sdlttf.TTF_OpenFont(font_path.encode("utf-8"), font_size)
 
-        text_surface = sdl2.sdlttf.TTF_RenderText_Solid(self.font, text.encode(), sdl2.SDL_Color(0, 0, 0))
-        self.texture = sdl2.SDL_CreateTextureFromSurface(self.window.renderer, text_surface)
-        text_rect = sdl2.SDL_Rect(x + centre, y + centre, width - centre * 2, height - centre * 2)
+        text_surface = sdl2.sdlttf.TTF_RenderText_Solid(
+            self.font, text.encode(), sdl2.SDL_Color(0, 0, 0)
+        )
+        self.texture = sdl2.SDL_CreateTextureFromSurface(
+            self.window.renderer, text_surface
+        )
+        text_rect = sdl2.SDL_Rect(
+            x + centre, y + centre, width - centre * 2, height - centre * 2
+        )
         sdl2.SDL_RenderCopy(self.window.renderer, self.texture, None, text_rect)
 
         sdl2.sdlttf.TTF_CloseFont(self.font)
         sdl2.SDL_FreeSurface(text_surface)
         sdl2.sdlttf.TTF_Quit()
 
     def _handle_event(self) -> bool:
         """Handles the event of the mouse."""
         event = self.window.event
         _pressed = False
         if event.type == sdl2.SDL_MOUSEBUTTONDOWN:
             mouse_x, mouse_y = event.button.x, event.button.y
-            if self.x <= mouse_x <= self.x + self.width and self.y <= mouse_y <= self.y + self.height:
+            if (
+                self.x <= mouse_x <= self.x + self.width
+                and self.y <= mouse_y <= self.y + self.height
+            ):
                 _pressed = True
         elif event.type == sdl2.SDL_MOUSEBUTTONUP:
             _pressed = False
 
         return _pressed
 
     def is_button_pressed(self) -> bool:
@@ -60,34 +81,64 @@
     def button_pressed(self, func: callable) -> None:
         """Custom decorator function that executes a function when the button is pressed."""
         if self.is_button_pressed() and callable(func):
             func()
 
 
 class Button:
-    def __init__(self) -> None: 
+    def __init__(self) -> None:
         pass
 
-    def new_button(self, window: window._CustomRenderer, text: str, x: int, y: int, width: int, height: int, font_path: str, font_sharp: int, centre: int, color: tuple) -> _CustomButton:
+    def new_button(
+        self,
+        window: window._CustomRenderer,
+        text: str,
+        x: int,
+        y: int,
+        width: int,
+        height: int,
+        font_path: str,
+        font_sharp: int,
+        centre: int,
+        color: tuple,
+    ) -> _CustomButton:
         """Creates a new button for your ui."""
-        return _CustomButton(window, text, x, y, width, height, font_path, font_sharp, centre, color)
+        return _CustomButton(
+            window, text, x, y, width, height, font_path, font_sharp, centre, color
+        )
 
 
 class Text:
     def __init__(self) -> None:
         pass
 
-    def print_text(self, window: window._CustomRenderer, text: str, x: int, y: int, width: int, height: int, font_path: str, font_sharp: int, color: tuple) -> None:
+    def print_text(
+        self,
+        window: window._CustomRenderer,
+        text: str,
+        x: int,
+        y: int,
+        width: int,
+        height: int,
+        font_path: str,
+        font_sharp: int,
+        color: tuple,
+    ) -> None:
         """Prints text on the screen."""
         sdl2.sdlttf.TTF_Init()
         self.font = sdl2.sdlttf.TTF_OpenFont(font_path.encode("utf-8"), font_sharp)
-        sdl2.SDL_SetRenderDrawColor(window.renderer, color[0], color[1], color[2], color[3])
-
-        text_surface = sdl2.sdlttf.TTF_RenderText_Solid(self.font, text.encode(),
-                                                        sdl2.SDL_Color(color[0], color[1], color[2], color[3]))
+        sdl2.SDL_SetRenderDrawColor(
+            window.renderer, color[0], color[1], color[2], color[3]
+        )
+
+        text_surface = sdl2.sdlttf.TTF_RenderText_Solid(
+            self.font,
+            text.encode(),
+            sdl2.SDL_Color(color[0], color[1], color[2], color[3]),
+        )
         self.texture = sdl2.SDL_CreateTextureFromSurface(window.renderer, text_surface)
         text_rect = sdl2.SDL_Rect(x, y, width, height)
         sdl2.SDL_RenderCopy(window.renderer, self.texture, None, text_rect)
 
         sdl2.sdlttf.TTF_CloseFont(self.font)
         sdl2.SDL_FreeSurface(text_surface)
         sdl2.sdlttf.TTF_Quit()
```

### Comparing `fusion-engine-0.3.0/src/fusionengine/files/vector.py` & `fusion-engine-1.0.0/src/fusionengine/files/vector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-
 class _CustomVector2D:
     def __init__(self, x, y):
         self.x = x
         self.y = y
 
+
 class _CustomVectorEntity:
     def __init__(self, x, y, width, height):
         self.x = x
         self.y = y
         self.width = width
         self.height = height
 
+
 # Not needed for now
 class _CustomVector3D:
     def __init__(self, x, y, z):
         self.x = x
         self.y = y
         self.z = z
 
+
 class Vectors:
     def __init__(self):
         pass
-    
+
     def new_vector2d(self, x, y):
         return _CustomVector2D(x, y)
-    
+
     def _new_vector3d(self, x, y, z):
         return _CustomVector3D(x, y, z)
```

