# Comparing `tmp/cmdtrix-0.1.7.tar.gz` & `tmp/cmdtrix-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdtrix-0.1.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cmdtrix-0.1.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cmdtrix-0.1.7.tar` & `cmdtrix-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1090 2022-11-19 19:53:04.115512 cmdtrix-0.1.7/LICENSE
--rw-r--r--   0        0        0     5587 2023-06-20 16:36:17.493490 cmdtrix-0.1.7/README.md
--rw-r--r--   0        0        0      187 2023-06-19 22:12:39.417542 cmdtrix-0.1.7/cmdtrix/__init__.py
--rw-r--r--   0        0        0      307 2023-02-26 10:13:16.381893 cmdtrix-0.1.7/cmdtrix/__main__.py
--rw-r--r--   0        0        0     7494 2023-06-19 22:11:13.930316 cmdtrix-0.1.7/cmdtrix/cmdtrix.py
--rw-r--r--   0        0        0       32 2023-03-26 10:37:59.763757 cmdtrix-0.1.7/cmdtrix/requirements.txt
--rw-r--r--   0        0        0     7036 2023-06-20 16:27:10.677815 cmdtrix-0.1.7/cmdtrix/util/ArgsHandler.py
--rw-r--r--   0        0        0      344 2023-06-19 22:01:28.521576 cmdtrix-0.1.7/cmdtrix/util/Chars.py
--rw-r--r--   0        0        0     1786 2023-02-17 20:10:46.178187 cmdtrix-0.1.7/cmdtrix/util/EventTimer.py
--rw-r--r--   0        0        0        0 2022-11-27 19:57:12.804576 cmdtrix-0.1.7/cmdtrix/util/__init__.py
--rw-r--r--   0        0        0     3578 2023-03-26 10:37:47.691757 cmdtrix-0.1.7/cmdtrix/web/UpdateChecker.py
--rw-r--r--   0        0        0        0 2022-11-27 19:57:12.804576 cmdtrix-0.1.7/cmdtrix/web/__init__.py
--rw-r--r--   0        0        0     1202 2023-03-26 10:37:55.158757 cmdtrix-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     6451 1970-01-01 00:00:00.000000 cmdtrix-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1090 2022-11-19 19:53:04.115512 cmdtrix-0.1.8/LICENSE
+-rw-r--r--   0        0        0     5785 2023-07-30 12:58:49.205884 cmdtrix-0.1.8/README.md
+-rw-r--r--   0        0        0      187 2023-07-29 18:03:19.996899 cmdtrix-0.1.8/cmdtrix/__init__.py
+-rw-r--r--   0        0        0      307 2023-02-26 10:13:16.381893 cmdtrix-0.1.8/cmdtrix/__main__.py
+-rw-r--r--   0        0        0     7500 2023-07-29 17:58:46.409098 cmdtrix-0.1.8/cmdtrix/cmdtrix.py
+-rw-r--r--   0        0        0       32 2023-03-26 10:37:59.763757 cmdtrix-0.1.8/cmdtrix/requirements.txt
+-rw-r--r--   0        0        0     7356 2023-07-29 17:56:16.599795 cmdtrix-0.1.8/cmdtrix/util/ArgsHandler.py
+-rw-r--r--   0        0        0      685 2023-07-29 18:02:54.761446 cmdtrix-0.1.8/cmdtrix/util/Chars.py
+-rw-r--r--   0        0        0     1786 2023-02-17 20:10:46.178187 cmdtrix-0.1.8/cmdtrix/util/EventTimer.py
+-rw-r--r--   0        0        0        0 2022-11-27 19:57:12.804576 cmdtrix-0.1.8/cmdtrix/util/__init__.py
+-rw-r--r--   0        0        0     3578 2023-03-26 10:37:47.691757 cmdtrix-0.1.8/cmdtrix/web/UpdateChecker.py
+-rw-r--r--   0        0        0        0 2022-11-27 19:57:12.804576 cmdtrix-0.1.8/cmdtrix/web/__init__.py
+-rw-r--r--   0        0        0     1202 2023-03-26 10:37:55.158757 cmdtrix-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     6647 1970-01-01 00:00:00.000000 cmdtrix-0.1.8/PKG-INFO
```

### Comparing `cmdtrix-0.1.7/LICENSE` & `cmdtrix-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cmdtrix-0.1.7/README.md` & `cmdtrix-0.1.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -95,22 +95,24 @@
 ```
 ```console
 python -m cmdtrix [-h] [-c COLOR] ...
 ```
 
 | Argument               | Description                                                          |
 |------------------------|----------------------------------------------------------------------|
+| -h, --help             | show help message and exit                                           |
 | -v, --version          | output version information                                           |
 | -s, --synchronous      | sync the matrix columns speed                                        |
 | -c [\*], --color [\*]  | set the main-color to *                                              |
 | -p [\*], --peak [\*]   | set the peak-color to *                                              |
 | -d p, --dim p          | add chance p (percent) for dim characters                            |
 | -i p, --italic p       | add chance p (percent) for italic characters                         |
 | -m * p c               | hide a custom message * within the Matrix, with chance p and color c |
-| --symbols CHARS        | set a custom series of symbols to choose from                        |
+| -S \*, --symbols \*    | set a custom series of symbols to choose from                        |
+| -j, --japanese         | use japanese characters (overrides -S; requires appropriate fonts)   |
 | --framedelay DELAY     | set the framedelay (in sec) to slow down the Matrix, default is 0.015|
 | --timer DELAY          | exit the Matrix after DELAY (in sec) automatically                   |
 | --onkey                | only spawn columns on key-press                                      |
 
 ### Examples
 
 ```console
```

#### html2text {}

```diff
@@ -29,29 +29,31 @@
 python package ([PyPI-cmdtrix](https://pypi.org/project/cmdtrix/)): ```console
 pip install cmdtrix ``` ```console pip install git+https://github.com/
 SilenZcience/cmdtrix.git ```
                                                                   (back_to_top)
 ## Usage ```console cmdtrix [-h] [-c COLOR] ... ``` ```console python -
 m cmdtrix [-h] [-c COLOR] ... ``` | Argument | Description | |-----------------
 -------|----------------------------------------------------------------------
-| | -v, --version | output version information | | -s, --synchronous | sync the
-matrix columns speed | | -c [\*], --color [\*] | set the main-color to * | | -
-p [\*], --peak [\*] | set the peak-color to * | | -d p, --dim p | add chance p
-(percent) for dim characters | | -i p, --italic p | add chance p (percent) for
-italic characters | | -m * p c | hide a custom message * within the Matrix,
-with chance p and color c | | --symbols CHARS | set a custom series of symbols
-to choose from | | --framedelay DELAY | set the framedelay (in sec) to slow
-down the Matrix, default is 0.015| | --timer DELAY | exit the Matrix after
-DELAY (in sec) automatically | | --onkey | only spawn columns on key-press |
-### Examples ```console cmdtrix -m SilenZcience 5 red -m cmdtrix 5 blue -d 5 -
-m Star*The*Repo 10 magenta ``` > ![Example0](https://raw.githubusercontent.com/
-SilenZcience/cmdtrix/main/img/cmdtrix.gif "example0")  ![Example2](https://
-raw.githubusercontent.com/SilenZcience/cmdtrix/main/img/example2.gif
-"example2") ![Example2](https://raw.githubusercontent.com/SilenZcience/cmdtrix/
-main/img/example3.gif "example3")
+| | -h, --help | show help message and exit | | -v, --version | output version
+information | | -s, --synchronous | sync the matrix columns speed | | -c [\*],
+--color [\*] | set the main-color to * | | -p [\*], --peak [\*] | set the peak-
+color to * | | -d p, --dim p | add chance p (percent) for dim characters | | -
+i p, --italic p | add chance p (percent) for italic characters | | -m * p c |
+hide a custom message * within the Matrix, with chance p and color c | | -S \*,
+--symbols \* | set a custom series of symbols to choose from | | -j, --japanese
+| use japanese characters (overrides -S; requires appropriate fonts) | | --
+framedelay DELAY | set the framedelay (in sec) to slow down the Matrix, default
+is 0.015| | --timer DELAY | exit the Matrix after DELAY (in sec) automatically
+| | --onkey | only spawn columns on key-press | ### Examples ```console cmdtrix
+-m SilenZcience 5 red -m cmdtrix 5 blue -d 5 -m Star*The*Repo 10 magenta ``` >
+![Example0](https://raw.githubusercontent.com/SilenZcience/cmdtrix/main/img/
+cmdtrix.gif "example0")  ![Example2](https://raw.githubusercontent.com/
+SilenZcience/cmdtrix/main/img/example2.gif "example2") ![Example2](https://
+raw.githubusercontent.com/SilenZcience/cmdtrix/main/img/example3.gif
+"example3")
                                                                   (back_to_top)
 ## License This project is licensed under the MIT License - see the [LICENSE]
 (https://github.com/SilenZcience/cmdtrix/blob/main/LICENSE) file for details ##
 Contact > **SilenZcience**
 [![GitHub-SilenZcience][GitHub-SilenZcience]](https://github.com/SilenZcience)
 [OS-Windows]: https://img.shields.io/badge/os-windows-green [OS-Linux]: https:/
 /img.shields.io/badge/os-linux-green [OS-MacOS]: https://img.shields.io/badge/
```

### Comparing `cmdtrix-0.1.7/cmdtrix/cmdtrix.py` & `cmdtrix-0.1.8/cmdtrix/cmdtrix.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from colorama import just_fix_windows_console
 from random import choices, randrange, random
 from time import sleep as delay_frame
 from _thread import interrupt_main
 from functools import lru_cache
 
 from cmdtrix.util.EventTimer import EventTimer
-from cmdtrix.util.Chars import charList
+from cmdtrix.util.Chars import charList, japanese
 from cmdtrix.util.ArgsHandler import ArgsHandler
 
 
 colorCodes = {"black": "30", "red": "31", "green": "32", "yellow": "33",
               "blue": "34", "magenta": "35", "cyan": "36", "white": "37"}
 cols, rows = get_terminal_size()
 
@@ -34,14 +34,17 @@
 keyDetected = 0
 
 just_fix_windows_console()
 
 
 class MatrixColumn:
     def __init__(self, col):
+        self.reset(col)
+
+    def reset(self, col):
         self.finished = False
         self.currentTick = 0
         
         self.yPositionSet = 1
         self.yPositionErased = 1
         self.lastChar = ""
         
@@ -121,36 +124,33 @@
 
 
 def on_press(key):
     global keyDetected
     keyDetected += 1
 
 
-def addNewMatrixColumns(matrixColumns: set, condition: bool) -> None:
+def updateMatrixColumns(matrixColumns: set) -> None:
     """
     add a new MatrixColumn every Tick, if the MAX has not been
     reached yet
     """
-    if len(matrixColumns) >= NUMBER_OF_MATRIXCOLUMNS or not condition:
+    global keyDetected
+    for matrixColumn in matrixColumns:
+        matrixColumn.update()
+        if matrixColumn.finished and (not ON_KEY_DETECTION or keyDetected):
+            col = randrange(cols+1)
+            matrixColumn.reset(col)
+            keyDetected = max(0, keyDetected-1)
+    if len(matrixColumns) >= NUMBER_OF_MATRIXCOLUMNS or (ON_KEY_DETECTION and not keyDetected):
         return
     col = randrange(cols+1)
     matrixColumns.add(MatrixColumn(col))
-    global keyDetected
     keyDetected = max(0, keyDetected-1)
 
 
-def updateMatrixColumns(matrixColumns: set) -> None:
-    for matrixColumn in matrixColumns:
-        matrixColumn.update()
-
-
-def getFinishedColumns(matrixColumns: set):
-    return set(filter(lambda x: x.finished, matrixColumns))
-
-
 def init() -> None:
     printCode("?25l", "2J")  # hide cursor, clear screen
     return EventTimer(10, checkTerminalSize)
 
 
 def deinit(eventTimer: list) -> None:
     printCode("m", "2J", "?25h")  # reset attributes, clear screen, show cursor
@@ -173,14 +173,15 @@
         CHANCE_FOR_ITALIC = argsHandler.italic
         global SYNCHRONOUS
         SYNCHRONOUS = argsHandler.synchronous
         global HIDDEN_MESSAGE
         HIDDEN_MESSAGE = argsHandler.messages
         global charList
         charList = [*argsHandler.alpha] if argsHandler.alpha else charList
+        charList = japanese if argsHandler.japanese else charList
         global FRAME_DELAY
         FRAME_DELAY = argsHandler.frameDelay
         global ON_KEY_DETECTION
         ON_KEY_DETECTION = argsHandler.onkey
         exitOnArg = False
         
         eventTimer.append(init())
@@ -190,19 +191,17 @@
         if ON_KEY_DETECTION:
             eventTimer.append(EventTimer(None, None, 'keyboardListener', on_press=on_press))
             print('', flush=True)
         
         
         matrixColumns = set()
         while True:
-            addNewMatrixColumns(matrixColumns, not ON_KEY_DETECTION or keyDetected)
-            delay_frame(FRAME_DELAY)
             updateMatrixColumns(matrixColumns)
+            delay_frame(FRAME_DELAY)
             # stdout.flush()
-            matrixColumns.difference_update(getFinishedColumns(matrixColumns))
     except KeyboardInterrupt:
         pass
     except Exception:
         exitStatus = 1
     finally:
         if not exitOnArg:
             deinit(eventTimer)
```

### Comparing `cmdtrix-0.1.7/cmdtrix/util/ArgsHandler.py` & `cmdtrix-0.1.8/cmdtrix/util/ArgsHandler.py`

 * *Files 12% similar despite different names*

```diff
@@ -58,14 +58,15 @@
         self.color_peak = "white"
         self.dim = 0.0
         self.italic = 0.0
         self.synchronous = False
         self.message = (b'\x4d\x61\x64\x65\x42\x79\x53\x69\x6c\x61\x73\x4b\x72\x61\x75\x6d\x65'.decode(), 0.01)
         self.messages = []
         self.alpha = ""
+        self.japanese = False
         self.frameDelay = 0.015
         self.timer = None
         self.onkey = False
         
         self.parseArgs()
         self.translateArgs()
 
@@ -85,16 +86,18 @@
                             type=float, dest="dim", metavar="p",
                             help="add chance p (percent) for dim characters")
         parser.add_argument("-i", "--italic", action="store", default=1.0,
                             type=float, dest="italic", metavar="p",
                             help="add chance p (percent) for italic characters")
         parser.add_argument("-m", action=store_message(0.01, "red"), dest="messages",
                             nargs="+", metavar="* p c", help="hide a custom message * within the Matrix, with chance p and color c")
-        parser.add_argument("--symbols", action="store", default="", type=str, dest="alpha",
-                            metavar="CHARS", help="set a custom series of symbols to choose from")
+        parser.add_argument("-S", "--symbols", action="store", default="", type=str, dest="alpha",
+                            metavar="*", help="set a custom series of symbols to choose from")
+        parser.add_argument("-j", "--japanese", action="store_const", default=False, const=True,
+                            dest="japanese", help="use japanese characters (overrides -S; requires appropriate fonts)")
         parser.add_argument("--framedelay", action="store", default=0.015, type=float,
                             dest="framedelay", metavar="DELAY", help="set the framedelay (in sec) to slow down the Matrix, default is 0.015")
         parser.add_argument("--timer", action="store", default=None, type=float,
                             dest="timer", metavar="DELAY", help="exit the Matrix after DELAY (in sec) automatically")
         parser.add_argument("--onkey", action="store_const", default=False,
                             const=True, dest="onkey", help="only spawn columns on key-press")
         
@@ -122,14 +125,16 @@
         
         self.messages = [(self.message[0], self.message[1], self.color)]
         if getattr(self.params, "messages"):
             self.messages += getattr(self.params, "messages")
         
         self.alpha = getattr(self.params, "alpha")
         
+        self.japanese = getattr(self.params, 'japanese')
+        
         self.frameDelay = getattr(self.params, "framedelay")
         if self.frameDelay < 0.0:
             print("A negative framedelay cannot be implemented!")
             sysexit(1)
 
         self.timer = getattr(self.params, "timer")
```

### Comparing `cmdtrix-0.1.7/cmdtrix/util/EventTimer.py` & `cmdtrix-0.1.8/cmdtrix/util/EventTimer.py`

 * *Files identical despite different names*

### Comparing `cmdtrix-0.1.7/cmdtrix/web/UpdateChecker.py` & `cmdtrix-0.1.8/cmdtrix/web/UpdateChecker.py`

 * *Files identical despite different names*

### Comparing `cmdtrix-0.1.7/pyproject.toml` & `cmdtrix-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cmdtrix-0.1.7/PKG-INFO` & `cmdtrix-0.1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmdtrix
-Version: 0.1.7
+Version: 0.1.8
 Summary: Matrix-console-effect made in Python.
 Keywords: console,crossplatform,matrix,python,terminal
 Author-email: "Silas A. Kraume" <silas.kraume1552@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -119,22 +119,24 @@
 ```
 ```console
 python -m cmdtrix [-h] [-c COLOR] ...
 ```
 
 | Argument               | Description                                                          |
 |------------------------|----------------------------------------------------------------------|
+| -h, --help             | show help message and exit                                           |
 | -v, --version          | output version information                                           |
 | -s, --synchronous      | sync the matrix columns speed                                        |
 | -c [\*], --color [\*]  | set the main-color to *                                              |
 | -p [\*], --peak [\*]   | set the peak-color to *                                              |
 | -d p, --dim p          | add chance p (percent) for dim characters                            |
 | -i p, --italic p       | add chance p (percent) for italic characters                         |
 | -m * p c               | hide a custom message * within the Matrix, with chance p and color c |
-| --symbols CHARS        | set a custom series of symbols to choose from                        |
+| -S \*, --symbols \*    | set a custom series of symbols to choose from                        |
+| -j, --japanese         | use japanese characters (overrides -S; requires appropriate fonts)   |
 | --framedelay DELAY     | set the framedelay (in sec) to slow down the Matrix, default is 0.015|
 | --timer DELAY          | exit the Matrix after DELAY (in sec) automatically                   |
 | --onkey                | only spawn columns on key-press                                      |
 
 ### Examples
 
 ```console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cmdtrix Version: 0.1.7 Summary: Matrix-console-
+Metadata-Version: 2.1 Name: cmdtrix Version: 0.1.8 Summary: Matrix-console-
 effect made in Python. Keywords: console,crossplatform,matrix,python,terminal
 Author-email: "Silas A. Kraume"
 kraume1552@gmail.com> Requires-Python: >=3.7 Description-Content-Type: text/
 markdown Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
@@ -43,29 +43,31 @@
 python package ([PyPI-cmdtrix](https://pypi.org/project/cmdtrix/)): ```console
 pip install cmdtrix ``` ```console pip install git+https://github.com/
 SilenZcience/cmdtrix.git ```
                                                                   (back_to_top)
 ## Usage ```console cmdtrix [-h] [-c COLOR] ... ``` ```console python -
 m cmdtrix [-h] [-c COLOR] ... ``` | Argument | Description | |-----------------
 -------|----------------------------------------------------------------------
-| | -v, --version | output version information | | -s, --synchronous | sync the
-matrix columns speed | | -c [\*], --color [\*] | set the main-color to * | | -
-p [\*], --peak [\*] | set the peak-color to * | | -d p, --dim p | add chance p
-(percent) for dim characters | | -i p, --italic p | add chance p (percent) for
-italic characters | | -m * p c | hide a custom message * within the Matrix,
-with chance p and color c | | --symbols CHARS | set a custom series of symbols
-to choose from | | --framedelay DELAY | set the framedelay (in sec) to slow
-down the Matrix, default is 0.015| | --timer DELAY | exit the Matrix after
-DELAY (in sec) automatically | | --onkey | only spawn columns on key-press |
-### Examples ```console cmdtrix -m SilenZcience 5 red -m cmdtrix 5 blue -d 5 -
-m Star*The*Repo 10 magenta ``` > ![Example0](https://raw.githubusercontent.com/
-SilenZcience/cmdtrix/main/img/cmdtrix.gif "example0")  ![Example2](https://
-raw.githubusercontent.com/SilenZcience/cmdtrix/main/img/example2.gif
-"example2") ![Example2](https://raw.githubusercontent.com/SilenZcience/cmdtrix/
-main/img/example3.gif "example3")
+| | -h, --help | show help message and exit | | -v, --version | output version
+information | | -s, --synchronous | sync the matrix columns speed | | -c [\*],
+--color [\*] | set the main-color to * | | -p [\*], --peak [\*] | set the peak-
+color to * | | -d p, --dim p | add chance p (percent) for dim characters | | -
+i p, --italic p | add chance p (percent) for italic characters | | -m * p c |
+hide a custom message * within the Matrix, with chance p and color c | | -S \*,
+--symbols \* | set a custom series of symbols to choose from | | -j, --japanese
+| use japanese characters (overrides -S; requires appropriate fonts) | | --
+framedelay DELAY | set the framedelay (in sec) to slow down the Matrix, default
+is 0.015| | --timer DELAY | exit the Matrix after DELAY (in sec) automatically
+| | --onkey | only spawn columns on key-press | ### Examples ```console cmdtrix
+-m SilenZcience 5 red -m cmdtrix 5 blue -d 5 -m Star*The*Repo 10 magenta ``` >
+![Example0](https://raw.githubusercontent.com/SilenZcience/cmdtrix/main/img/
+cmdtrix.gif "example0")  ![Example2](https://raw.githubusercontent.com/
+SilenZcience/cmdtrix/main/img/example2.gif "example2") ![Example2](https://
+raw.githubusercontent.com/SilenZcience/cmdtrix/main/img/example3.gif
+"example3")
                                                                   (back_to_top)
 ## License This project is licensed under the MIT License - see the [LICENSE]
 (https://github.com/SilenZcience/cmdtrix/blob/main/LICENSE) file for details ##
 Contact > **SilenZcience**
 [![GitHub-SilenZcience][GitHub-SilenZcience]](https://github.com/SilenZcience)
 [OS-Windows]: https://img.shields.io/badge/os-windows-green [OS-Linux]: https:/
 /img.shields.io/badge/os-linux-green [OS-MacOS]: https://img.shields.io/badge/
```

