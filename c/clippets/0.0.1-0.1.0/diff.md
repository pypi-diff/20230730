# Comparing `tmp/clippets-0.0.1.tar.gz` & `tmp/clippets-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clippets-0.0.1.tar", last modified: Tue Jul 18 14:46:07 2023, max compression
+gzip compressed data, was "clippets-0.1.0.tar", last modified: Sun Jul 30 14:33:11 2023, max compression
```

## Comparing `clippets-0.0.1.tar` & `clippets-0.1.0.tar`

### file list

```diff
@@ -1,30 +1,36 @@
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-07-18 14:46:07.553519 clippets-0.0.1/
--rw-rw-r--   0 paul      (1000) paul      (1000)    11357 2023-07-18 14:12:00.000000 clippets-0.0.1/LICENSE
--rw-rw-r--   0 paul      (1000) paul      (1000)     1029 2023-07-18 14:46:07.553519 clippets-0.0.1/PKG-INFO
--rw-rw-r--   0 paul      (1000) paul      (1000)      362 2023-07-18 14:14:23.000000 clippets-0.0.1/README.md
--rw-rw-r--   0 paul      (1000) paul      (1000)     2726 2023-07-18 14:41:41.000000 clippets-0.0.1/pyproject.toml
--rw-rw-r--   0 paul      (1000) paul      (1000)      126 2023-07-18 14:46:07.553519 clippets-0.0.1/setup.cfg
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-07-18 14:46:07.549519 clippets-0.0.1/src/
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-07-18 14:46:07.553519 clippets-0.0.1/src/clippets/
--rw-rw-r--   0 paul      (1000) paul      (1000)        0 2023-07-18 14:12:00.000000 clippets-0.0.1/src/clippets/__init__.py
--rw-rw-r--   0 paul      (1000) paul      (1000)     2924 2023-07-18 14:12:00.000000 clippets-0.0.1/src/clippets/clippets.css
--rw-rw-r--   0 paul      (1000) paul      (1000)      554 2023-07-18 14:12:00.000000 clippets-0.0.1/src/clippets/colors.py
--rw-rw-r--   0 paul      (1000) paul      (1000)    38321 2023-07-18 14:38:16.000000 clippets-0.0.1/src/clippets/core.py
--rw-rw-r--   0 paul      (1000) paul      (1000)     4185 2023-07-18 14:21:39.000000 clippets-0.0.1/src/clippets/help.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)     2182 2023-07-18 14:12:00.000000 clippets-0.0.1/src/clippets/linux.py
--rw-rw-r--   0 paul      (1000) paul      (1000)    17276 2023-07-18 14:12:00.000000 clippets-0.0.1/src/clippets/markup.py
--rw-rw-r--   0 paul      (1000) paul      (1000)     1611 2023-07-18 14:12:00.000000 clippets-0.0.1/src/clippets/platform.py
--rw-rw-r--   0 paul      (1000) paul      (1000)    28979 2023-07-18 14:12:00.000000 clippets-0.0.1/src/clippets/snippets.py
--rw-rw-r--   0 paul      (1000) paul      (1000)     8371 2023-07-18 14:12:00.000000 clippets-0.0.1/src/clippets/widgets.py
--rw-rw-r--   0 paul      (1000) paul      (1000)    10053 2023-07-18 14:12:00.000000 clippets-0.0.1/src/clippets/win.py
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-07-18 14:46:07.553519 clippets-0.0.1/src/clippets.egg-info/
--rw-rw-r--   0 paul      (1000) paul      (1000)     1029 2023-07-18 14:46:07.000000 clippets-0.0.1/src/clippets.egg-info/PKG-INFO
--rw-rw-r--   0 paul      (1000) paul      (1000)      586 2023-07-18 14:46:07.000000 clippets-0.0.1/src/clippets.egg-info/SOURCES.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)        1 2023-07-18 14:46:07.000000 clippets-0.0.1/src/clippets.egg-info/dependency_links.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)       48 2023-07-18 14:46:07.000000 clippets-0.0.1/src/clippets.egg-info/entry_points.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)       34 2023-07-18 14:46:07.000000 clippets-0.0.1/src/clippets.egg-info/requires.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)        9 2023-07-18 14:46:07.000000 clippets-0.0.1/src/clippets.egg-info/top_level.txt
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-07-18 14:46:07.553519 clippets-0.0.1/tests/
--rw-rw-r--   0 paul      (1000) paul      (1000)     7591 2023-07-18 14:24:07.000000 clippets-0.0.1/tests/test_editing.py
--rw-rw-r--   0 paul      (1000) paul      (1000)     8504 2023-07-18 14:24:07.000000 clippets-0.0.1/tests/test_load_save.py
--rw-rw-r--   0 paul      (1000) paul      (1000)      482 2023-07-18 14:12:00.000000 clippets-0.0.1/tests/test_snapshots.py
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-07-30 14:33:11.441364 clippets-0.1.0/
+-rw-rw-r--   0 paul      (1000) paul      (1000)    11357 2023-07-18 14:12:00.000000 clippets-0.1.0/LICENSE
+-rw-rw-r--   0 paul      (1000) paul      (1000)     1508 2023-07-30 14:33:11.441364 clippets-0.1.0/PKG-INFO
+-rw-rw-r--   0 paul      (1000) paul      (1000)      842 2023-07-30 14:30:22.000000 clippets-0.1.0/README.md
+-rw-rw-r--   0 paul      (1000) paul      (1000)     2999 2023-07-30 12:17:39.000000 clippets-0.1.0/pyproject.toml
+-rw-rw-r--   0 paul      (1000) paul      (1000)      126 2023-07-30 14:33:11.441364 clippets-0.1.0/setup.cfg
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-07-30 14:33:11.425364 clippets-0.1.0/src/
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-07-30 14:33:11.441364 clippets-0.1.0/src/clippets/
+-rw-rw-r--   0 paul      (1000) paul      (1000)        0 2023-07-18 14:12:00.000000 clippets-0.1.0/src/clippets/__init__.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)     3032 2023-07-28 11:17:28.000000 clippets-0.1.0/src/clippets/clippets.css
+-rw-rw-r--   0 paul      (1000) paul      (1000)      554 2023-07-18 14:12:00.000000 clippets-0.1.0/src/clippets/colors.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)    43405 2023-07-30 09:22:22.000000 clippets-0.1.0/src/clippets/core.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)     4185 2023-07-18 14:21:39.000000 clippets-0.1.0/src/clippets/help.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)     2288 2023-07-28 09:13:25.000000 clippets-0.1.0/src/clippets/linux.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)    17787 2023-07-30 09:34:41.000000 clippets-0.1.0/src/clippets/markup.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)     1656 2023-07-25 14:08:25.000000 clippets-0.1.0/src/clippets/platform.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)    27485 2023-07-30 09:08:02.000000 clippets-0.1.0/src/clippets/snippets.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)     8599 2023-07-29 09:26:25.000000 clippets-0.1.0/src/clippets/widgets.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)    10053 2023-07-25 14:17:13.000000 clippets-0.1.0/src/clippets/win.py
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-07-30 14:33:11.441364 clippets-0.1.0/src/clippets.egg-info/
+-rw-rw-r--   0 paul      (1000) paul      (1000)     1508 2023-07-30 14:33:11.000000 clippets-0.1.0/src/clippets.egg-info/PKG-INFO
+-rw-rw-r--   0 paul      (1000) paul      (1000)      722 2023-07-30 14:33:11.000000 clippets-0.1.0/src/clippets.egg-info/SOURCES.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)        1 2023-07-30 14:33:11.000000 clippets-0.1.0/src/clippets.egg-info/dependency_links.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)       78 2023-07-30 14:33:11.000000 clippets-0.1.0/src/clippets.egg-info/entry_points.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)       34 2023-07-30 14:33:11.000000 clippets-0.1.0/src/clippets.egg-info/requires.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)        9 2023-07-30 14:33:11.000000 clippets-0.1.0/src/clippets.egg-info/top_level.txt
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-07-30 14:33:11.441364 clippets-0.1.0/tests/
+-rw-rw-r--   0 paul      (1000) paul      (1000)     7079 2023-07-30 09:16:09.000000 clippets-0.1.0/tests/test_clipboard.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)     8905 2023-07-29 18:33:32.000000 clippets-0.1.0/tests/test_editing.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)    12639 2023-07-29 12:25:52.000000 clippets-0.1.0/tests/test_filtering.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)     1492 2023-07-29 09:04:39.000000 clippets-0.1.0/tests/test_help.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)     3402 2023-07-27 10:49:29.000000 clippets-0.1.0/tests/test_kb_selection.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)     3683 2023-07-29 12:00:55.000000 clippets-0.1.0/tests/test_keywords.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)     9956 2023-07-30 09:08:31.000000 clippets-0.1.0/tests/test_load_save.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)     2384 2023-07-29 13:06:52.000000 clippets-0.1.0/tests/test_misc_ui.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)    18022 2023-07-28 14:41:19.000000 clippets-0.1.0/tests/test_moving.py
```

### Comparing `clippets-0.0.1/LICENSE` & `clippets-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clippets-0.0.1/pyproject.toml` & `clippets-0.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = "clippets"
-version = "0.0.1"
+version = "0.1.0"
 authors = [
   { name="Paul Ollis", email="paul@cleversheep.org" },
 ]
-description = "UI to built up clipboard context from (rich) text snippets."
+description = "UI to build up clipboard content from (rich) text snippets."
 requires-python = ">=3.8"
 readme = "README.md"
 classifiers = [
-    'Development Status :: 3 - Alpha',
+    'Development Status :: 4 - Beta',
     "License :: OSI Approved :: MIT License",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3",
     "Environment :: Console",
 ]
 dependencies = [
@@ -22,14 +22,15 @@
 ]
 
 [tool.setuptools.package-data]
 clippets = ["help.txt", "clippets.css"]
 
 [project.scripts]
 clippets = "clippets.core:main"
+snippets = "clippets.core:main"
 
 [project.urls]
 "Homepage" = "https://github.com/paul-ollis/clippets"
 "Bug Tracker" = "https://github.com/paul-ollis/clippets/issues"
 
 [build-system]
 requires = ["setuptools>=61.0"]
@@ -60,15 +61,19 @@
 
     # Below are checks I wish re-enable, once the code is cleaner.
     "ANN001",  # Missing return type argument.
     "ANN002",  # Missing return type for *args.
     "ANN003",  # Missing return type for **kwargs.
     "ANN201",  # Missing return type for public method/function.
     "ANN202",  # Missing return type for private method/function.
+    "ANN205",  # Missing return type for static method.
     "ANN206",  # Missing return type for class method.
+    "ARG002",  # Unused argument.
+               # Also pylint:unused-argument. If I can prevent this when the
+               # API demands the (keyword) argument then I will re-enable.
     "TD002",   # Author missing for 'todo'
     "TD003",   # Issue ref missing for 'todo'
 ]
 
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
```

### Comparing `clippets-0.0.1/src/clippets/clippets.css` & `clippets-0.1.0/src/clippets/clippets.css`

 * *Files 8% similar despite different names*

```diff
@@ -58,14 +58,19 @@
     outline-bottom: solid  $success;
 }
 .moving {
     outline: solid $success;
     padding: 1 1 0 1;
     outline-bottom: solid  $success;
 }
+.is_text.moving {
+    outline: solid $success;
+    padding: 1 1 1 1;
+    outline-bottom: solid  $success;
+}
 
 .is_placehoder.dest_above {
     height: 3;
     padding: 0 0 0 0;
     margin: 0 1 0 4;
     color: $text-disabled;
     outline-bottom: solid  $success;
@@ -119,28 +124,28 @@
 }
 
 #view:focus {
     border: tall $accent;
 }
 
 #dialog {
-    grid-size: 3;
+    grid-size: 4;
     grid-gutter: 1 2;
-    grid-rows: 1 3;
+    grid-rows: 1 4;
     padding: 0 1;
     width: auto;
     height: auto;
     border: thick $background 80%;
     background: $surface;
 }
 
 #question {
     height: 1;
     width: 1fr;
-    column-span: 3;
+    column-span: 4;
     content-align: center middle;
 }
 
 Button {
     width: 100%;
 }
```

### Comparing `clippets-0.0.1/src/clippets/colors.py` & `clippets-0.1.0/src/clippets/colors.py`

 * *Files identical despite different names*

### Comparing `clippets-0.0.1/src/clippets/core.py` & `clippets-0.1.0/src/clippets/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 """Program to allow efficient composition of text snippets."""
 # pylint: disable=too-many-lines
 
-# 2. A help page is needed.
 # 3. A user guide will be needed if this is to be made available to others.
-# 5. The keywords support needs a bigger, cleaner palette and the ability
-#    to edit a group's keywords.
+# 5. The keywords support needs a bigger, cleaner palette.
 # 6. Global keywords?
 # 8. Make it work on Macs.
 # 10. Genertae frozen versions for all platforms.
 # 11. Watch the input file(s) and be able to 're-start' in response to changes.
 
-# 12. Fix edit - copy/reuse move code.
-# 13. Fix duplicate - copy/reuse move code.
+# TODO: Make terminology consistent as follows.
+#       Added
+#           A snippet that has been added to the clipboard.
+#       Selected
+#           The snippet that has the box around. Many actions operate on this
+#           snippet. This is stored as the snippet ID and can be ``None`` when
+#           no snippet is present or visible.
+#       Focussed
+#           This should only relate to the filter input.
+
 from __future__ import annotations
 
 import argparse
 import asyncio
 import collections
+import itertools
 import re
-import subprocess
 import sys
+import subprocess
 import threading
-import time
 from contextlib import asynccontextmanager, suppress
 from dataclasses import dataclass
 from functools import partial, wraps
-from pathlib import Path
 from typing import AsyncGenerator, Callable, ClassVar, Iterable, TYPE_CHECKING
 
 from rich.text import Text
 from textual._context import (
     active_message_pump, message_hook as message_hook_context_var)
 from textual.app import App, Binding, ComposeResult
 from textual.containers import Horizontal
@@ -40,82 +45,59 @@
 from textual.widgets import Header, Input, Static
 
 from . import markup, snippets
 from .platform import (
     SharedTempFile, get_editor_command, get_winpos, put_to_clipboard,
     terminal_title)
 from .snippets import (
-    Group, Snippet, SnippetInsertionPointer, SnippetLike,
+    Group, PlaceHolder, Snippet, SnippetInsertionPointer, SnippetLike,
     id_of_element as id_of)
 from .widgets import (
     MyFooter, MyInput, MyLabel, MyMarkdown, MyTag, MyText, MyVerticalScroll,
     SnippetMenu)
 
 if TYPE_CHECKING:
-    import io
-
     from textual.message import Message
     from textual.widget import Widget
     from textual.events import Event
 
 HL_GROUP = ''
-
 LEFT_MOUSE_BUTTON = 1
 RIGHT_MOUSE_BUTTON = 3
-
-
-def timestamp():
-    """Provide textual timestamps to 3 decimal places."""
-    start = time.time()
-    now = time.time()
-    while True:
-        yield f'{now - start:6.3f}'
-        now = time.time()
-
-
-ts = timestamp()
-next(ts)
+BANNER = r'''
+  ____ _ _                  _
+ / ___| (_)_ __  _ __   ___| |_ ___
+| |   | | | '_ \| '_ \ / _ \ __/ __|
+| |___| | | |_) | |_) |  __/ |_\__ \
+ \____|_|_| .__/| .__/ \___|\__|___/
+          |_|   |_|
+'''
 
 
 @dataclass
 class MoveInfo:
     """Details of snippet being moved.
 
     @uid:      The ID of snippet being moved.
     @dest_uid: The ID of the insertion point snippet.
     """
 
     source: Snippet
     dest: SnippetInsertionPointer
 
-    def unmoved(self):
-        """Test if the destination is the same as the source."""
-        return self.source == self.dest.snippet
-
-
-def if_active(method):
-    """Wrap Smippets method to only run when fully active."""
-    @wraps(method)
-    def invoke(self, *args, **kwargs):
-        if self.active:
-            return method(self, *args, **kwargs)
-        else:
-            return None
-
-    return invoke
 
 def only_for_mode(name: str):
     """Wrap Smippets method to only run when in a given mode."""
     def decor(method):
         @wraps(method)
         def invoke(self, *args, **kwargs):
             if self.context_name() == name:
                 return method(self, *args, **kwargs)
             else:
-                return None
+                return None                                  # pragma: no cover
         return invoke
 
     return decor
 
 
 class Matcher:                         # pylint: disable=too-few-public-methods
     """Simple plain-text replacement for a compiled regular expression."""
@@ -124,34 +106,24 @@
         self.pat = pat.casefold()
 
     def search(self, text: str) -> bool:
         """Search for plain text."""
         return not self.pat or self.pat in text.lower()
 
 
-BANNER = r'''
-  ____ _ _                  _
- / ___| (_)_ __  _ __   ___| |_ ___
-| |   | | | '_ \| '_ \ / _ \ __/ __|
-| |___| | | |_) | |_) |  __/ |_\__ \
- \____|_|_| .__/| .__/ \___|\__|___/
-          |_|   |_|
-'''
-
-
 class HelpScreen(Screen):
     """Tada."""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.timer = None
 
     def compose(self) -> ComposeResult:
         """Tada."""
-        yield Header()
+        yield Header(id='header')
         yield Static(BANNER, classes='banner')
         yield from markup.generate()
         yield MyFooter()
 
     def on_screen_resume(self):
         """Fix code block styling as soon as possible."""
         for c in walk_depth_first(self):
@@ -161,28 +133,35 @@
                         cc.renderable.padding = 0, 0, 0, 0
                         cc.renderable.indent_guides = False
 
 
 class MainScreen(Screen):
     """Main Clippets screen."""
 
-    def __init__(self, groups: Group):
-        super().__init__(name='main')
+    tag_id_sources: ClassVar[dict[str, itertools.count]] = {}
+
+    def __init__(self, groups: Group, uid: str):
+        super().__init__(name='main', id=uid)
         self.groups = groups
         self.walk = partial(groups.walk, backwards=False)
 
     def compose(self) -> ComposeResult:
         """Build the widget hierarchy."""
         yield Header()
 
         with Horizontal(id='input', classes='input oneline'):
             yield MyLabel('Filter: ')
-            yield MyInput(placeholder='Enter text to filter.', id='filter')
+            inp = MyInput(placeholder='Enter text to filter.', id='filter')
+            inp.cursor_blink = False
+            yield inp
         with MyVerticalScroll(id='view', classes='result'):
-            yield MyMarkdown(id='result')
+            if self.app.args.raw:
+                yield Static(id='result')
+            else:
+                yield MyMarkdown(id='result')
         with MyVerticalScroll(id='snippet-list', classes='bbb'):
             yield from self.build_tree_part()
         footer = MyFooter()
         footer.add_class('footer')
         yield footer
 
     def build_tree_part(self):
@@ -195,16 +174,17 @@
             if isinstance(el, Group):
                 classes = 'is_group'
                 label = MyLabel(
                     f'▽ {HL_GROUP}{el.name}', id=uid, classes=classes)
                 fields = []
                 for tag in el.tags:
                     classes = f'tag_{all_tags[tag]}'
-                    fields.append(
-                        MyTag(f'{tag}', name=tag, classes=f'tag {classes}'))
+                    fields.append(MyTag(
+                        f'{tag}', id=self.gen_tag_id(tag), name=tag,
+                        classes=f'tag {classes}'))
                 w = Horizontal(label, *fields, classes='group_row')
                 w.styles.padding = (0, 0, 0, (el.depth() - 1) * 4)
                 yield w
             else:
                 snippet = make_snippet_widget(uid, el)
                 if snippet:
                     yield snippet
@@ -216,82 +196,95 @@
         top.mount(*self.build_tree_part())
 
     def on_idle(self):
         """Perform idle processing."""
         w = self.query_one('.footer')
         w.check_context()
 
+    def gen_tag_id(self, tag: str) -> str:
+        """Generate a unique widget ID for a tag."""
+        if tag not in self.tag_id_sources:
+            self.tag_id_sources[tag] = itertools.count()
+        return f'tag-{tag}-{next(self.tag_id_sources[tag])}'
+
 
 def make_snippet_widget(uid, snippet) -> Widget | None:
     """Construct correct widegt for a given snnippet."""
     classes = 'is_snippet'
     w = None
     if isinstance(snippet, snippets.MarkdownSnippet):
         w = MyMarkdown(id=uid, classes=classes)
     elif isinstance(snippet, Snippet):
         classes = f'{classes} is_text'
         w = MyText(id=uid, classes=classes)
-    elif isinstance(snippet, snippets.PlaceHolder):
+    elif isinstance(snippet, PlaceHolder):
         classes = f'{classes} is_placehoder'
         w = Static('-- place holder --', id=uid, classes=classes)
         w.display = False
     if w:
         w.styles.margin = (0, 1, 0, (snippet.depth() - 1) * 4)
     return w
 
 
 async def populate(q, walk, query):
-    """Background task to resolve widgets to element mapping."""
+    """Background task to populate widgets."""
     while True:
         while q.qsize() > 1:
-            cmd = await q.get()
+            cmd = await q.get()                              # pragma: no cover
         cmd = await q.get()
         if cmd is None:
             break
 
-        print(next(ts), 'START populate')
         n = 0
         for snippet in walk():
             if q.qsize() > 0:
-                break
+                break                                        # pragma: no cover
             if snippet.dirty:
                 w = query(snippet)
                 if w is not None:
                     w.update(snippet.marked_text)
                     snippet.dirty = False
                     n += 1
                     if n % 30 == 0:
-                        await asyncio.sleep(0.5)
-        print(next(ts), 'End populate', n)
+                        await asyncio.sleep(0.5)             # pragma: no cover
+
+
+def populate_fg(walk, query):
+    """Populate widgets."""
+    for snippet in walk():
+        if snippet.dirty:
+            w = query(snippet)
+            if w is not None:
+                w.update(snippet.marked_text)
+                snippet.dirty = False
 
 
 async def resolve(q, lookup, walk, query):
     """Background task to resolve widgets to element mapping."""
     while True:
         while q.qsize() > 1:
-            cmd = await q.get()
+            cmd = await q.get()                              # pragma: no cover
         cmd = await q.get()
         if cmd is None:
             break
 
         new_lookup = {}
         elements = list(walk())
         for el in elements:
             if q.qsize() > 0:
-                break
+                break                                        # pragma: no cover
             uid = el.uid()
-            if uid not in new_lookup:
+            if uid and uid not in new_lookup:
                 with suppress(NoMatches):
                     new_lookup[uid] = query(f'#{uid}')
                     await asyncio.sleep(0.01)
         else:
             if q.qsize() == 0:
                 lookup.clear()
                 lookup.update(new_lookup)
-                print('LOOKUP POPULATED')
 
 
 class AppMixin:
     """Mixin providing application logic."""
 
     # pylint: disable=too-many-public-methods
     # pylint: disable=too-many-instance-attributes
@@ -299,38 +292,48 @@
     mount: Callable
     post_message: Callable
     push_screen: Callable
     screen: Screen
 
     def __init__(self, groups: Group):
         super().__init__()
+        for name in list(self.MODES):
+            if name != '_default':
+                self.MODES.pop(name)
         self.chosen = []
         self.collapsed = set()
         self.edited_text = ''
         self.filter = Matcher('')
         self.groups = groups
         self.hidden_bindings = set()
         self.hover_uid = None
-        self.focussed_snippet = id_of(self.groups.first_snippet())
+        self._selected_snippets = [id_of(self.groups.first_snippet())]
         self.move_info = None
         self.redo_buffer = collections.deque(maxlen=20)
         self.sel_order = False
         self.undo_buffer = collections.deque(maxlen=20)
         self.lookup = {}
         self.walk = partial(self.groups.walk, backwards=False)
         self.walk_groups = partial(self.walk, predicate=is_group)
         self.resolver_q = asyncio.Queue()
         self.populater_q = asyncio.Queue()
 
     async def on_exit_app(self, _event):
         """Clean up when exiting the application."""
-        self.resolver_q.put_nowait(None)
-        await self.resolver
-        self.populater_q.put_nowait(None)
-        await self.populater
+        if self.resolver:
+            self.resolver_q.put_nowait(None)
+            await self.resolver
+        if self.populater:
+            self.populater_q.put_nowait(None)
+            await self.populater
+
+    @property
+    def selected_snippet(self):
+        """The currently focussed snippet."""
+        return self._selected_snippets[-1]
 
     def handle_blur(self, w: Widget):
         """Handle loss of focus for a widget.
 
         Currernly this only occurs for the filter input widget.
         """
         w.remove_class('kb_focussed')
@@ -340,55 +343,65 @@
         """Find the widget for a given element."""
         uid = el.uid()
         if uid not in self.lookup:
             self.lookup[uid] = self.query_one(f'#{el.uid()}')
         return self.lookup[uid]
 
     ## Management of dynanmic display features.
-    def focussable_widgets(self) -> tuple[Widget, ...]:
-        """Create a tuple of 'focussable' widgets."""
-        return tuple(self.find_widget(s) for s in self.walk_snippets())
+    def selectable_widgets(self) -> list[Widget, ...]:
+        """Create a list of selectable widgets.
+
+        To be selectable, a snippet's widget must be visible.
+        """
+        widgets = (self.find_widget(s) for s in self.walk_snippets())
+        return [w for w in widgets if w.display]
 
-    def insertion_widgets(self) -> tuple[Widget, ...]:
+    def insertion_widgets(self) -> tuple[tuple[Snippet, Widget], ...]:
         """Create a tuple of widgets involved in insetion operations."""
-        a = [self.query_one('#input')]
-        b = (
-            self.find_widget(s)
-            for s in self.walk_snippet_like())
-        return (*a, *b)
+        return tuple(
+            (s, self.find_widget(s)) for s in self.walk_snippet_like())
 
-    @if_active
     def set_visuals(self) -> None:
         """Set and clear widget classes that control visual highlighting."""
+        self.set_snippet_visuals()
+        self.set_input_visuals()
+
+    def set_snippet_visuals(self) -> None:
+        """Set and clear widget classes that control snippet highlighting."""
         filter_focussed = (fw := self.focused) and fw.id == 'filter'
-        for w in self.insertion_widgets():
+        for s, w in self.insertion_widgets():
             w.remove_class('kb_focussed')
             w.remove_class('mouse_hover')
-            w.remove_class('moving')
             w.remove_class('dest_above')
             w.remove_class('dest_below')
+            if isinstance(s, PlaceHolder):
+                w.display = False
             if self.move_info is not None:
-                info = self.move_info
-                source, dest = info.source, info.dest
-                if w.id == source.uid():
-                    w.add_class('moving')
-                else:
+                source, dest = self.move_info.source, self.move_info.dest
+                if w.id != source.uid():
                     uid, after = dest.addr
                     if uid != source.uid() and uid == w.id:
                         w.add_class('dest_below' if after else 'dest_above')
+                    if isinstance(dest.snippet, PlaceHolder):
+                        w.display = True
             else:
-                if w.id == self.focussed_snippet and not filter_focussed:
+                if w.id == self.selected_snippet and not filter_focussed:
                     w.add_class('kb_focussed')
                 if w.id == self.hover_uid:
                     w.add_class('mouse_hover')
 
+    def set_input_visuals(self) -> None:
+        """Set and clear widget classes that control input highlighting."""
+        filter_focussed = (fw := self.focused) and fw.id == 'filter'
+        w = self.query_one('#input')
         if filter_focussed:
-            self.query_one('#input').add_class('kb_focussed')
+            w.add_class('kb_focussed')
+        else:
+            w.remove_class('kb_focussed')
 
-    @if_active
     def update_selected(self) -> None:
         """Update the 'selected' flag following mouse movement."""
         for snippet in self.walk_snippets():
             id_str = snippet.uid()
             w = self.find_widget(snippet)
             if id_str in self.chosen:
                 w.add_class('selected')
@@ -433,63 +446,109 @@
 
         elif tag := getattr(ev, 'tag', None):
             self.action_toggle_tag(tag.name)
 
     def on_right_click(self, ev) -> None:
         """Process a mouse right-click."""
         def on_close(v):
+            self.screen.set_focus(None)
             if  v == 'edit':
                 self.edit_snippet(w.id)
             elif  v == 'duplicate':
                 self.duplicate_snippet(w.id)
+            elif  v == 'move':
+                self.action_start_moving_snippet(w.id)
 
         w = getattr(ev, 'snippet', None)
         if w:
             snippet = self.groups.find_element_by_uid(w.id)
             if snippet:
-                self.push_screen(SnippetMenu(), on_close)
+                self.push_screen(SnippetMenu(id='snippet-menu'), on_close)
 
     ## Handling of keyboard operations.
-    def fix_selection(self):
+    def fix_selection(self, *, kill_filter: bool = False):
         """Update the keyboard selected focus when widgets get hidden."""
-        w = self.query_one(f'#{self.focussed_snippet}')
+        # Do nothing is the filter input is focusses and should remain so.
+        if self._selected_snippets[-1] == 'filter':
+            if kill_filter:
+                self._selected_snippets.pop()
+            else:
+                return
+
+        # If the current selection is ``None`` then we cannot fix the
+        # selection.
+        if self.selected_snippet is None:
+            if not self.selectable_widgets():
+                return
+            self._selected_snippets.pop()
+
+        # If there is selection history (from previous fix-ups) try to reselect
+        # the oldest entry in the history.
+        for i, wid in enumerate(self._selected_snippets):
+            if i > 0 and wid is not None:
+                w = self.query_one(f'#{wid}')
+                if w.display:
+                    self._selected_snippets[:] = self._selected_snippets[:i]
+                    self.set_visuals()
+                    self.screen.set_focus(None)
+                    return
+
+        # The selection history could not be used so find the best alternative
+        # snippet to select, saving the currently selection in the history.
+        self.fix_to_next_nearest_snippet()
+
+    def fix_to_next_nearest_snippet(self):
+        """Move the snippet selection to the next nearest, if necessary."""
+        w = self.query_one(f'#{self.selected_snippet}')
         if not w.display:
-            k = self.key_select_move(inc=-1, dry_run=True)
+            k = self.action_select_move(inc=-1, dry_run=True)
             if k == 0:
-                k = self.key_select_move(inc=1, dry_run=False)
+                k = self.action_select_move(inc=1, dry_run=False, push=True)
             else:
-                self.key_select_move(inc=-1, dry_run=False)
+                k = self.action_select_move(inc=-1, dry_run=False, push=True)
 
-    def key_select_move(self, inc: int, *, dry_run: bool) -> None:
-        """Move the keyboard driven focus to the next available widget."""
-        widgets = self.focussable_widgets()
+            # It is possible that no snippet could be selected.
+            if k < 0 and self._selected_snippets[-1] is not None:
+                self._selected_snippets.append(None)
+
+    def action_select_move(
+                self, inc: int, *, dry_run: bool = False, push: bool = False,
+            ) -> int:
+        """Move the selection to the next available snippet."""
+        # Collect snippet widgets and those that are visible.
+        widgets = [self.find_widget(s) for s in self.walk_snippets()]
         valid_widgets = [w for w in widgets if w.display]
         valid_range = range(len(widgets))
 
         k = -1
         for i, w in enumerate(widgets):
-            if w.id == self.focussed_snippet:
+            if w.id == self.selected_snippet:
                 k = i + inc
                 while k in valid_range and not widgets[k].display:
                     k += inc
                 break
 
         # Note that widgets[0] is always present and visible.
         if k not in valid_range:
             k = 0 if k < 0 else len(valid_widgets) - 1
         if dry_run:
             return k
 
-        self.focussed_snippet = widgets[k].id
-        self.set_visuals()
-        self.screen.set_focus(None)
+        if self.selected_snippet != widgets[k].id:
+            if push:
+                self._selected_snippets.append(widgets[k].id)
+            else:
+                self._selected_snippets[:] = [widgets[k].id]
+            self.screen.set_focus(None)
+            self.set_visuals()
+            widgets[k].scroll_visible()
         return k
 
     ## Ways to limit visible snippets.
-    def filter_view(self) -> None:
+    def filter_view(self) -> None:                                 # noqa: C901
         """Hide snippets that have been filtered out or folded away."""
         def st_opened():
             return all(ste.uid() not in self.collapsed for ste in stack)
 
         matcher = self.filter
         stack = []
         opened = True
@@ -520,30 +579,28 @@
 
             elif isinstance(el, Snippet):
                 w = self.find_widget(el)
                 w.display = bool(matcher.search(el.text)) and opened
         self.fix_selection()
 
     ## UNCLASSIFIED
-    def is_fully_collapsed(self, tag: str = ''):
+    def is_fully_collapsed(self):
         """Test whether all groups are collapsed."""
         groups = self.walk_groups()
-        if tag:
-            groups = (g for g in groups if tag in g.tags)
         return all(group.uid() in self.collapsed for group in groups)
 
     def is_fully_open(self, tag: str = ''):
         """Test whether all groups are open."""
         groups = self.walk_groups()
         if tag:
             groups = (g for g in groups if tag in g.tags)
         return all(group.uid() not in self.collapsed for group in groups)
 
-    async def on_input_changed(self, message: Input.Changed) -> None:
-        """Handle a text changed message."""
+    def on_input_changed(self, message: Input.Changed) -> None:
+        """Handle a change to the filter text input."""
         if message.input.id == 'filter':
             pat = message.value
             if not pat.strip():
                 rexp = Matcher('')
             else:
                 try:
                     rexp = re.compile(f'(?i){pat}')
@@ -562,15 +619,14 @@
         if self.edited_text:
             self.undo_buffer.append(([], self.edited_text))
         else:
             self.undo_buffer.append((list(self.chosen), ''))
         self.edited_text = ''
 
     ## Clipboard representaion widget management.
-    @if_active
     def update_result(self) -> None:
         """Update the contents of the results display widget."""
         text = self.build_result_text()
         w = self.query_one('#result')
         w.update(text)
         put_to_clipboard(
             text, mode='raw' if self.args.raw else 'styled')
@@ -598,18 +654,21 @@
 
     ## Editing and duplicating snippets.
     def rebuild_after_edits(self):
         """Rebuild, refresh, *etc*. after changes to the snippets tree."""
         self.backup_and_save()
         self.lookup.clear()
         self.screen.rebuild_tree_part()
-        self.resolver_q.put_nowait('rebuild')
-        # self.populate()
-        self.populater_q.put_nowait('pop')
-        # self.schedule_refresh()
+        if self.resolver:
+            self.resolver_q.put_nowait('rebuild')
+        if self.populater:
+            self.populater_q.put_nowait('pop')
+        else:
+            populate_fg(self.walk_snippets, self.find_widget)
+
         self.update_result()
         self.set_visuals()
 
     def edit_snippet(self, id_str) -> None:
         """Invoke the user's editor on a snippet."""
         snippet = self.groups.find_element_by_uid(id_str)
         text = run_editor(snippet.text)
@@ -619,55 +678,64 @@
 
     def duplicate_snippet(self, id_str: str):
         """Duplicate and the edit the current snippet."""
         snippet = self.groups.find_element_by_uid(id_str)
         new_snippet = snippet.duplicate()
         text = run_editor(new_snippet.text)
         new_snippet.set_text(text)
+        self._selected_snippets[:] = [new_snippet.uid()]
         self.rebuild_after_edits()
+        w = self.find_widget(new_snippet)
+        w.scroll_visible()
 
     def backup_and_save(self):
         """Create a new snippet file backup and then save."""
         snippets.backup_file(self.args.snippet_file)
         snippets.save(self.args.snippet_file, self.groups)
 
     ## Snippet position movement.
-    def modify_snippet(self, snippet, lines) -> None:
-        """Modify the contents of a snippet."""
-        snippet.source_lines = lines
-        snippets.save(self.args.snippet_file, self.groups)
-
     def action_start_moving_snippet(self, id_str: str | None = None) -> None:
         """Start moving a snippet to a different position in the tree."""
-        id_str = id_str or self.focussed_snippet
-        self.action_clear_selection()
+        for i, _ in enumerate(self.walk_snippets()):
+            if i == 1:
+                break
+        else:
+            # We have fewer than 2 snippets, moving is impossibnle.
+            # TODO: What about when groups are collapsed?
+            return
+
+        id_str = id_str or self.selected_snippet
         w = self.query_one(f'#{id_str}')
         w.add_class('moving')
 
         snippet = self.groups.find_element_by_uid(id_str)
         dest = SnippetInsertionPointer(snippet)
         self.move_info = MoveInfo(snippet, dest)
+        if not self.action_move_insertion_point('up'):
+            self.action_move_insertion_point('down')
         self.set_visuals()
 
     ## Binding handlers.
     def action_clear_selection(self) -> None:
         """Clear all snippets from the selection."""
         self.chosen[:] = []
         #@ self.update_result()
         self.update_selected()
 
     def action_complete_move(self):
         """Complete a snippet move operation."""
-        if self.move_info and not self.move_info.unmoved():
-            self.move_info.dest.move_snippet(self.move_info.source)
-            self.rebuild_after_edits()
+        info = self.move_info
         self.action_stop_moving()
+        if info and info.dest.move_snippet(info.source):
+            self.rebuild_after_edits()
+            self._selected_snippets[:] = [info.source.uid()]
+            self.set_visuals()
 
     def action_do_redo(self) -> None:
-        """Redor the last undo action."""
+        """Redo the last undo action."""
         if self.redo_buffer:
             self.undo_buffer.append((self.chosen, self.edited_text))
             self.chosen, self.edited_text = self.redo_buffer.pop()
             self.update_result()
             self.update_selected()
 
     def action_do_undo(self) -> None:
@@ -676,75 +744,88 @@
             self.redo_buffer.append((self.chosen, self.edited_text))
             self.chosen, self.edited_text = self.undo_buffer.pop()
             self.update_result()
             self.update_selected()
 
     def action_duplicate_snippet(self) -> None:
         """Duplicate and edit the currently selected snippet."""
-        if self.focussed_snippet:
-            self.duplicate_snippet(self.focussed_snippet)
+        if self.selected_snippet:
+            self.duplicate_snippet(self.selected_snippet)
 
     def action_edit_clipboard(self) -> None:
         """Run the user's editor on the current clipboard contents."""
         text = self.build_result_text()
         self.push_undo()
         new_text = run_editor(text)
         if new_text.strip() != text.strip():
             self.edited_text = new_text
             self.update_result()
 
     def action_edit_keywords(self) -> None:
         """Invoke the user's editor on the current group's keyword list."""
-        snippet = self.groups.find_element_by_uid(self.focussed_snippet)
+        snippet = self.groups.find_element_by_uid(self.selected_snippet)
         if snippet is None:
             return
 
         kw = snippet.parent.keyword_set()
         text = run_editor(kw.text)
         new_words = set(text.split())
         if new_words != kw.words:
             kw.words = new_words
             self.backup_and_save()
             for snippet in self.walk_snippets():
                 snippet.reset()
-            self.populater_q.put_nowait('pop')
+            if self.populater:
+                self.populater_q.put_nowait('pop')
+            else:                                            # pragma: no cover
+                populate_fg(self.walk_snippets, self.find_widget)
 
-    def action_edit_filter(self) -> None:
-        """Toggle focus to/from the filter input field."""
+    def action_enter_filter(self) -> None:
+        """Move focus to the filter input field."""
         w = self.query_one('#filter')
-        if self.focused is w:
-            self.screen.set_focus(None)
-        else:
-            self.screen.set_focus(w)
+        self.screen.set_focus(w)
+        self._selected_snippets.append('filter')
+        self.set_visuals()
+
+    def action_leave_filter(self) -> None:
+        """Move focus away from the filter input field."""
+        self.screen.set_focus(None)
+        self.fix_selection(kill_filter=True)
         self.set_visuals()
 
+    def action_zap_filter(self) -> None:
+        """Clear he contents of the filter input field."""
+        w = self.query_one('#filter')
+        self.on_input_changed(Input.Changed(input=w, value=''))
+        w.value = ''
+
     def action_edit_snippet(self) -> None:
         """Edit the currently selected snippet."""
-        if self.focussed_snippet:
-            self.edit_snippet(self.focussed_snippet)
+        if self.selected_snippet:
+            self.edit_snippet(self.selected_snippet)
 
-    def action_move_insertion_point(self, direction: str):
+    def action_move_insertion_point(self, direction: str) -> bool:
         """Move the snippet insertion up of down.
 
         :direction: Either 'up' or 'down'.
         """
         snippet, dest = self.move_info.source, self.move_info.dest
         if dest.move(backwards=direction == 'up', skip=snippet):
             self.set_visuals()
-
-    def action_select_next(self) -> None:
-        """Move the keyboard driven focus to the next widget."""
-        self.key_select_move(inc=1, dry_run=False)
-
-    def action_select_prev(self) -> None:
-        """Move the keyboard driven focus to the next widget."""
-        self.key_select_move(inc=-1, dry_run=False)
+            w = self.find_widget(dest.snippet)
+            w.scroll_visible()
+            return True
+        else:
+            return False
 
     def action_stop_moving(self) -> None:
         """Stop moving a snippet - cancelling the move operation."""
+        if self.move_info:
+            w = self.find_widget(self.move_info.source)
+            w.remove_class('moving')
         self.move_info = None
         self.set_visuals()
 
     def action_toggle_order(self) -> None:
         """Toggle the order of selected snippets."""
         self.sel_order = not self.sel_order
         self.update_result()
@@ -756,17 +837,17 @@
                 self.collapsed.add(group.uid())
         else:
             self.collapsed = set()
         self.filter_view()
 
     def action_toggle_select(self):
         """Handle any key that is used to select a snippet."""
-        if self.groups.find_element_by_uid(self.focussed_snippet) is not None:
+        if self.groups.find_element_by_uid(self.selected_snippet) is not None:
             self.push_undo()
-            id_str = self.focussed_snippet
+            id_str = self.selected_snippet
             if id_str in self.chosen:
                 self.chosen.remove(id_str)
             else:
                 self.chosen.append(id_str)
             self.update_selected()
             self.update_result()
 
@@ -777,87 +858,79 @@
         for group in tagged_groups:
             if fully_open:
                 self.collapsed.add(group.uid())
             else:
                 self.collapsed.discard(group.uid())
         self.filter_view()
 
-    def debug(self, *args):
-        """Log a message, purely for debug purposes."""
-        if self.logf:
-            print(*args, file=self.logf)
-
 
 class Clippets(AppMixin, App):
     """The textual application object."""
 
     # pylint: disable=too-many-instance-attributes
     TITLE = 'Comment snippet wrangler'
     CSS_PATH = 'clippets.css'
     SCREENS: ClassVar[dict] = {'help': HelpScreen()}
     id_to_focus: ClassVar[dict] = {'input': 'filter'}
 
-    def __init__(self, args, logf: io.TextIOWrapper | None = None):
-        self.logf = logf
+    def __init__(self, args):
         groups, title = snippets.load(args.snippet_file)
         if title:
             self.TITLE = title                   # pylint: disable=invalid-name
         super().__init__(groups)
         self.args = args
-        self.active = False
         self.key_handler = KeyHandler(self)
         self.init_bindings()
         self.walk_snippets = partial(self.walk, is_snippet)
         self.walk_snippet_like = partial(self.walk, is_snippet_like)
         self.resolver = None
         self.populater = None
 
-    def xrun(self, *args, **kwargs) -> int:
-        """Wrap the standar run method."""
-        # pylint: disable=unspecified-encoding
-        saved = sys.stdout, sys.stderr
-        sys.stdout = sys.stderr = Path('/tmp/snippets.log').open(  # noqa: S108
-            'wt', buffering=1)
-        try:
-            return super().run(*args, **kwargs)
-        finally:
-            sys.stdout, sys.stderr = saved
+    def run(self, *args, **kwargs) -> int:                   # pragma: no cover
+        """Wrap the standar run method, settin the terminal title."""
+        with terminal_title('Snippet-wrangler'):
+            return super().run()
 
     def context_name(self) -> str:
         """Provide a name identifying the current context."""
-        if self.screen.id == 'help':
-            return 'help'
-        elif self.move_info is None:
-            return 'normal'
+        if self.screen.id == 'main':
+            if self.move_info is not None:
+                return 'moving'
+            elif self.selected_snippet == 'filter':
+                return 'filter'
+            else:
+                return 'normal'
         else:
-            return 'moving'
+            return self.screen.id
 
     def init_bindings(self):
         """Set up the application bindings."""
         bind = partial(self.key_handler.bind, ('normal',), show=False)
         bind('f8', 'toggle_order', description='Toggle order')
-        bind('f9', 'toggle_collapse_all', description='Collapse/open all')
-        bind('up', 'select_prev')
-        bind('down', 'select_next')
-        bind(
-            'ctrl+f', 'edit_filter', description='Toggle fileter input',
-            priority=True)
+        bind('up', 'select_move(-1)')
+        bind('down', 'select_move(1)')
+        bind('ctrl+b', 'zap_filter', description='Clear filter input')
+        bind('ctrl+f', 'enter_filter', description='Enter filter input')
         bind('ctrl+u', 'do_undo', description='Undo', priority=True)
         bind('ctrl+r', 'do_redo', description='Redo', priority=True)
         bind('e', 'edit_snippet')
         bind('d c', 'duplicate_snippet')
         bind('m', 'start_moving_snippet', description='Move snippet')
+        bind('f7', 'edit_keywords', description='Edit keywords')
+
+        bind = partial(self.key_handler.bind, ('filter',), show=True)
+        bind('ctrl+f', 'leave_filter', description='Leave filter input')
 
         bind = partial(self.key_handler.bind, ('normal',), show=True)
         bind('f1', 'show_help', description='Help')
         bind('f2', 'edit_clipboard', description='Edit')
         bind('f3', 'clear_selection', description='Clear')
-        bind('f7', 'edit_keywords', description='Edit keywords')
-        bind('ctrl+q', 'quit', description='Quit', priority=True)
+        bind('f9', 'toggle_collapse_all', description='(Un)fold')
         bind('enter space', 'toggle_select', description='Toggle select')
+        bind('ctrl+q', 'quit', description='Quit', priority=True)
 
         bind = partial(self.key_handler.bind, ('moving',), show=True)
         bind(
             'up', 'move_insertion_point("up")', description='Cursor up')
         bind(
             'down', 'move_insertion_point("down")', description='Cursor down')
         bind('enter', 'complete_move', description='Insert')
@@ -865,63 +938,58 @@
 
         bind = partial(self.key_handler.bind, ('help',), show=True)
         bind('f1', 'pop_screen', description='Close help')
 
     def compose(self) -> ComposeResult:
         """Build the widget hierarchy."""
         yield Static()
-        self.add_mode('main', MainScreen(self.groups))
+        self.add_mode('main', MainScreen(self.groups, uid='main'))
         self.switch_mode('main')
 
     def active_shown_bindings(self):
         """Provide a list of bindings used for the application Footer."""
         return self.key_handler.active_shown_bindings()
 
     def on_ready(self) -> None:
         """React to the DOM having been created."""
-        print(next(ts), 'APP READY')
-        self.resolver = asyncio.create_task(
-            resolve(self.resolver_q, self.lookup, self.walk, self.query_one))
-        self.resolver_q.put_nowait('rebuild')
-
-        self.populater = asyncio.create_task(
-            populate(self.populater_q, self.walk_snippets, self.find_widget))
-        self.resolver_q.put_nowait('pop')
+        if self.args.sync_mode:
+            populate_fg(self.walk_snippets, self.find_widget)
+        else:
+            self.resolver = asyncio.create_task(resolve(
+                self.resolver_q, self.lookup, self.walk, self.query_one))
+            self.resolver_q.put_nowait('rebuild')
+            self.populater = asyncio.create_task(populate(
+                self.populater_q, self.walk_snippets, self.find_widget))
+            self.populater_q.put_nowait('pop')
 
         self.screen.set_focus(None)
-        self.active = True
         self.set_visuals()
-        print(next(ts), 'Visuals set')
 
     def action_show_help(self) -> None:
         """Show the help screen."""
         self.push_screen(HelpScreen(id='help'))
 
-    def action_close_help(self) -> None:
-        """Close the help screen."""
-        self.pop_screen()
-
-    async def on_key(self, ev: Event) -> None:
+    async def on_key(self, event: Event) -> None:
         """Handle a top level key press."""
-        await self.key_handler.handle_key(ev)
+        await self.key_handler.handle_key(event)
+        event.stop()
 
     def on_mount(self) -> None:
         """Perform app start-up actions."""
         self.dark = True
-        print(next(ts), 'MOUNT App')
-        # self.populate()
-        self.populater_q.put_nowait('pop')
+        populate_fg(self.walk_snippets, self.find_widget)
 
     @asynccontextmanager
-    async def run_test(
+    async def run_test(                                         # noqa: PLR0913
         self,
         *,
         headless: bool = True,
         size: tuple[int, int] | None = (80, 24),
         tooltips: bool = False,
+        notifications: bool = False,
         message_hook: Callable[[Message], None] | None = None,
     ) -> AsyncGenerator[Pilot, None]:
         """Run app under test conditions.
 
         Use this to run your app in "headless" (no output) mode and driver the
         app via a [Pilot][textual.pilot.Pilot] object.
 
@@ -963,35 +1031,33 @@
             )
 
         # Launch the app in the "background"
         active_message_pump.set(app)
         app_task = asyncio.create_task(run_app(app), name=f'run_test {app}')
 
         # Wait until the app has performed all startup routines.
-        self.debug('Wait for app_ready')
         await app_ready_event.wait()
-        self.debug('Done: Wait for app_ready')
 
         # Get the app in an active state.
         app._set_active()                                        # noqa: SLF001
 
         # Context manager returns pilot object to manipulate the app
         try:
-            self.debug('Create Pilot')
-            pilot = Pilot(app)
-            await pilot._wait_for_screen()                       # noqa: SLF001
-            yield pilot
+            with terminal_title('Snippet-wrangler'):
+                pilot = Pilot(app)
+                await pilot._wait_for_screen()                   # noqa: SLF001
+                yield pilot
         finally:
             # Shutdown the app cleanly
             await app._shutdown()                                # noqa: SLF001
             await app_task
             # Re-raise the exception which caused panic so test frameworks are
             # aware
             if self._exception:
-                raise self._exception
+                raise self._exception                        # pragma: no cover
 
 
 class KeyHandler:
     """Context specific key handling for an App."""
 
     def __init__(self, app):
         self.app = app
@@ -1038,19 +1104,19 @@
             binding for (ctx, key), binding in self.bindings.items()
             if ctx == context and binding.show]
 
 
 def run_editor(text) -> None:
     r"""Run the user's preferred editor on a textual element.
 
-    The user's chosen editor is found using the SNIPPETS_EDITOR environment
+    The user's chosen editor is found using the CLIPPETS_EDITOR environment
     variable. If that is not set then a simple, internal editor (future
     feature) is used.
 
-    At its simplest the SNIPPETS_EDITOR just provides the name/path of the
+    At its simplest the CLIPPETS_EDITOR just provides the name/path of the
     editor program, for example::
 
         C:\Windows\System32\notepad.exe
 
     It may also include command line options, for example to use the GUI
     version of Vim you need to add the '-f' flag, to prevent it running
     itself in the background.
@@ -1058,34 +1124,48 @@
         /usr/bin/gvim -f
 
     The strings '{w}, '{h}, '{x}' and '{y}' have a special meaning. They
     will be replaced by the editor's desired size (in characterss) and
     window position (in pixels). For example
 
         /usr/bin/gvim -f -geom {w}x{h}+{x}+{y}
+
+    The command is invoked with the name of a temporary file as its single
+    additional argument.
     """
-    edit_cmd = get_editor_command('SNIPPETS_EDITOR')
+    edit_cmd = get_editor_command('CLIPPETS_EDITOR')
+    uses_pos = '{x}' in edit_cmd and '{y}' in edit_cmd
     with SharedTempFile() as path:
         path.write_text(text, encoding='utf8')
-        x, y = get_winpos()
-        dims = {'w': 80, 'h': 25, 'x': x, 'y': y}
+        if uses_pos:                                         # pragma: no cover
+            x, y = get_winpos()
+            dims = {'w': 80, 'h': 25, 'x': x, 'y': y}
+        else:
+            dims = {'w': 80, 'h': 25}
         edit_cmd += ' ' + str(path)
         cmd = edit_cmd.format(**dims).split()
         subprocess.run(cmd, stderr=subprocess.DEVNULL, check=False)
         return path.read_text(encoding='utf8')
 
 
-def parse_args() -> argparse.Namespace:
-    """Run the clippets application."""
+def parse_args(sys_args: list[str] | None = None) -> argparse.Namespace:
+    """Parse the command line arguments."""
     parser = argparse.ArgumentParser()
     parser.add_argument(
         '--raw', action='store_true',
         help='Parse clippets as raw text.')
     parser.add_argument('snippet_file')
-    return parser.parse_args()
+
+    # This is used by testing. It prevents some actions running as backgroud
+    # asyncio tasks. These tasks exist to make the application appear more
+    # responsive to the user, but can make it harder (or slower) to create
+    # reliable snapshot based tests.
+    parser.add_argument(
+        '--sync-mode', action='store_true', help=argparse.SUPPRESS)
+    return parser.parse_args(sys_args or sys.argv[1:])
 
 
 def is_type(obj, *, classinfo):
     """Test is one of a set of types.
 
     This simply wraps the built-in isinstance, but plays nucely with
     functools.partial.
@@ -1095,12 +1175,19 @@
 
 # Useful parital functions for Group.walk.
 is_snippet = partial(is_type, classinfo=Snippet)
 is_snippet_like = partial(is_type, classinfo=SnippetLike)
 is_group = partial(is_type, classinfo=Group)
 
 
-def main():
+def main():                                                  # pragma: no cover
     """Run the application."""
     app = Clippets(parse_args())
-    with terminal_title('Snippet-wrangler'):
-        app.run()
+    app.run()
+
+
+def reset_for_tests():
+    """Perform a 'system' reset for test purposes.
+
+    This is not intended for non-testing use.
+    """
+    MainScreen.tag_id_sources = {}
```

### Comparing `clippets-0.0.1/src/clippets/help.txt` & `clippets-0.1.0/src/clippets/help.txt`

 * *Files identical despite different names*

### Comparing `clippets-0.0.1/src/clippets/linux.py` & `clippets-0.1.0/src/clippets/linux.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,22 +28,24 @@
 '''
 
 def put_to_clipboard(text: str, mode: str = 'styled'):
     """Put a text string into the clipboard."""
     if mode == 'raw':
         subprocess.run(
             ['/usr/bin/xclip', '-selection', 'clipboard'],
-            input=text.encode())
+            input=text.encode(),
+            check=False)
     else:
         html = markdown.markdown(text)
         html = doc_template.format(html)
         subprocess.run(
             ['/usr/bin/xclip', '-t', 'text/html', '-selection',
                 'clipboard'],
-            input=html.encode())
+            input=html.encode(),
+            check=False)
 
 
 @contextlib.contextmanager
 def terminal_title(title: str):
     """Temporarily set the text terminal's title."""
     print('\x1b[22;0t', end='')
     print(f'\x1b]0;{title}\x07', end='')
@@ -57,19 +59,19 @@
     """Get the editor command using a given envirot variable name.
 
     If the environment variable is not set, this uses gvim.
     """
     return os.getenv(env_var_name, 'gvim -f -geom {w}x{h}+{x}+{y}')
 
 
-def get_winpos() -> Tuple[int, int]:
+def get_winpos() -> Tuple[int, int]:                         # pragma: no cover
     """Get the screen position of the terminal."""
     res = subprocess.run(
         ['/usr/bin/xwininfo', '-name', 'Snippet-wrangler'],
-        capture_output=True)
+        capture_output=True, check=False)
     for rawline in res.stdout.decode().splitlines():
         line = rawline.strip()
         if line.startswith('Absolute upper-left X:'):
             x = int(line.partition(':')[-1].strip())
         elif line.startswith('Absolute upper-left Y:'):
             y = int(line.partition(':')[-1].strip())
     return x, y
```

### Comparing `clippets-0.0.1/src/clippets/markup.py` & `clippets-0.1.0/src/clippets/markup.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,14 +71,15 @@
 #
 #     we could do::
 #
 #          :urgent:`This is really serious!`
 
 import re
 import textwrap
+from dataclasses import dataclass
 from pathlib import Path
 from typing import ClassVar, Iterable, List, Tuple
 
 from rich.text import Text
 from rich.style import Style
 from textual.widgets import Markdown, Static
 
@@ -201,17 +202,17 @@
 
 class BlockTokeniser:                  # pylint: disable=too-few-public-methods
     """A simple parser for simple form of markup."""
 
     def __init__(self, text):
         lines = text.splitlines()
         while lines and not lines[0].strip():
-            lines.pop(0)
+            lines.pop(0)                                     # pragma: no cover
         while lines and not lines[-1].strip():
-            lines.pop()
+            lines.pop()                                      # pragma: no cover
 
         self.it = PushbackIter(iter(lines))
         self.state = 'idle'
 
     def blocks(self):
         """Yield basic blocks of text."""
         block = []
@@ -239,54 +240,54 @@
     """Base for all markup text elements."""
 
     def __init__(self, parent, classes=()):
         self.parent = parent
         self.children = []
         self.classes = set(classes)
 
-    def dump(self):
+    def dump(self):                                          # pragma: no cover
         """Dump tree."""
         for el in self.children:
             print(el)
             el.dump()
 
 
+@dataclass
 class TextElement:
     """A text string with styling information."""
 
-    def __init__(self, text, style=''):
-        self.text = text
-        self.style = style
+    text: str
+    style: str = ''
 
 
 class BlockElement(Element):
     """Base for all markup block elements; heading, paragraph, *etc*."""
 
     widget_class = Static
     margin_adjust = 0
 
     def __init__(self, lines, parent, classes=(), _match=None):
         super().__init__(parent, classes)
         self.ind_level, self.lines = dedent_lines(lines)
 
     @property
-    def level(self):
+    def level(self):                                         # pragma: no cover
         """The level of this element."""
         if self.parent:
             return self.parent.level + 1
         else:
             return 0
 
     @property
     def margin_level(self):
         """The margin level of this element."""
         if self.parent:
             return self.parent.margin_level + 1 + self.margin_adjust
         else:
-            return 0
+            return 0                                         # pragma: no cover
 
     @classmethod
     def consume_block(cls, blocks):
         """Try to consume a block of lines, creating a suitable Element."""
         try:
             lines = next(blocks)
         except StopIteration:
@@ -298,15 +299,15 @@
         else:
             blocks.push(lines)
             return None, None
 
     @classmethod
     def match(cls, _lines):
         """See if a block of lines is a match for this type of element."""
-        return True
+        return True                                          # pragma: no cover
 
     def gather_children(self, blocks):
         """Consume any child paragraphs."""
 
     def widget_text(self):
         """Form the text used to populate this element's widget."""
         return ' '.join(self.lines)
@@ -324,15 +325,15 @@
         """Generate Textual widgets for this document."""
         yield self.widget()
         for child in self.children:
             yield from child.generate()
 
     def _snippet(self) -> str:                    # pylint: disable=no-self-use
         """Format a snippet of text for use by __repr__."""
-        return ''
+        return ''                                            # pragma: no cover
 
     def __repr__(self):
         ret = f'{self.__class__.__name__}({self.level}/{self.ind_level}'
         ret += f' {self._snippet()})'
         return ret
 
 
@@ -346,27 +347,25 @@
         classes = [*classes, 'paragraph']
         super().__init__(lines, parent, classes)
         self.ind_level, self.lines = dedent_lines(lines)
         self._elements = None
 
     def _snippet(self) -> str:
         """Format a snippet of text for use by __repr__."""
-        return self.lines[0]
+        return self.lines[0]                                 # pragma: no cover
 
     @property
     def elements(self):
         """The paragraph content as a sequence of TextElement instances."""
         if self._elements is None:
             text = ' '.join(self.lines)
             self._elements = []
             while text:
                 ma = rc_inline_markup.match(text)
                 mb = rc_inline_class_markup.match(text)
-                if mb:
-                    print('XXX', mb.groupdict(), text)
                 if ma and mb:
                     m = ma if ma.group(1) < mb.group(1) else mb
                 else:
                     m = ma or mb
                 if m:
                     if mb:
                         name = m.group('class')
@@ -383,15 +382,15 @@
         return self._elements
 
     @classmethod
     def match(cls, lines):
         """Match a block of lines as a paragraph."""
         if len(lines) > 0:
             return ind_level(lines[0])
-        return None
+        return None                                          # pragma: no cover
 
     def widget_text(self):
         """Form the text used to populate this element's widget."""
         t = Text()
         for el in self.elements:
             t.append(el.text, style=el.style)
         return t
@@ -422,29 +421,29 @@
     """A block of code or uninterpreted text."""
 
     widget_class = Markdown
     margin_adjust = -1
 
     def __init__(self, blocks, parent, lang):
         lines = list(blocks[0])
-        for block in blocks[1:]:
+        for block in blocks[1:]:                             # pragma: no cover
             lines.append('')
             lines.extend(block)
         super().__init__(lines, parent, ['code'])
         self.lang = lang
 
     def widget_text(self):
         """Form the text used to populate this element's widget."""
         lang = self.lang or ''
         text = '\n'.join(self.lines)
         return f'~~~{lang}\n{text}\n~~~'
 
     def _snippet(self) -> str:
         """Format a snippet of text for use by __repr__."""
-        return f'{self.lang}: {self.lines[0]}'
+        return f'{self.lang}: {self.lines[0]}'               # pragma: no cover
 
 
 class Definition(Paragraph):
     """A two part paragraph definining a term.
 
     A defintion is formatted as::
```

### Comparing `clippets-0.0.1/src/clippets/platform.py` & `clippets-0.1.0/src/clippets/platform.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     'get_editor_command',
     'get_winpos',
     'put_to_clipboard',
     'SharedTempFile',
     'terminal_title',
 ]
 
-if platform.system() == 'Windows':
+if platform.system() == 'Windows':                           # pragma: no cover
     from .win import (
         get_editor_command, get_winpos, put_to_clipboard, terminal_title)
 elif platform.system() == 'Linux':
     from .linux import (
         get_editor_command, get_winpos, put_to_clipboard, terminal_title)
```

### Comparing `clippets-0.0.1/src/clippets/snippets.py` & `clippets-0.1.0/src/clippets/snippets.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from  contextlib import suppress
 from functools import partial
 from pathlib import Path
 from typing import ClassVar
 
 from markdown_strings import esc_format
 
-from . import colors
+from . import colors, widgets
 
 
 class SnippetInsertionPointer:
     """A 'pointer' of where to insert a snippet within a snippet tree.
 
     An insertion point can be before or after a snippet. Within a group, an
     insertion point below one snippet is equal to an insertion point above the
@@ -112,15 +112,15 @@
             return self.after
         else:
             return False
 
     def move_snippet(self, snippet) -> bool:
         """Move a given snippet to this insertion point."""
         if self.is_next_to(snippet):
-            return False
+            return False                                     # pragma: no cover
         snippet.parent.remove(snippet)
         snippet.parent.clean()
         if self.after:
             self.snippet.parent.add(snippet, after=self.snippet)
         else:
             self.snippet.parent.add(snippet, before=self.snippet)
         self.snippet.parent.clean()
@@ -130,19 +130,23 @@
         return f'Pointer({self.snippet.uid()}, {self.after})'
 
 
 class Element:
     """An element in a tree of groups and snippets."""
 
     id_source = itertools.count()
+    has_uid: bool = True
 
-    def __init__(self, parent: Element, first_line: str | None = None):
+    def __init__(self, parent: Element):
         self.parent = parent
-        self._uid = f'{self.__class__.__name__.lower()}-{next(self.id_source)}'
-        self.first_line = first_line
+        if self.has_uid:
+            n = next(self.id_source)
+            self._uid = f'{self._uid_base_name()}-{n}'
+        else:
+            self._uid = ''
         self._source_lines = []
         self.dirty = True
 
     @property
     def source_lines(self) -> tuple:
         """The source lines for this element."""
         return tuple(self._source_lines)
@@ -150,17 +154,15 @@
     @source_lines.setter
     def source_lines(self, value):
         self._source_lines = list(value)
         self.dirty = True
 
     @property
     def root(self):
-        """The root group of the tree containin this group."""
-        if self.parent is None:
-            return self
+        """The root group of the tree containing this element."""
         return self.parent.root
 
     def uid(self):
         """Derive a unique ID for this element."""
         return self._uid
 
     def depth(self):
@@ -169,49 +171,45 @@
             return self.parent.depth() + 1
         return 0
 
     def is_empty(self):
         """Detemine if this snippet is empty."""
         return len(self.source_lines) == 0
 
-    def source_len(self):
-        """Calculete the number of line in this snippet."""
-        return len(self.source_lines)
-
-    def full_repr(                            # pylint: disable=unused-argument
-            self,
-            end='\n'):                                           # noqa: ARG002
+    def full_repr(self, *, end='\n', debug: bool = False):
         """Format a simple representation of this element.
 
         This is intended for test support. The exact format may change between
         releases.
         """
         body = self.body_repr()
         spc = ' ' if body else ''
-        return f'{self.__class__.__name__}:{spc}{body}'
+        id_part = f' {self.uid()}' if debug else ''
+        return f'{self.__class__.__name__}{id_part}:{spc}{body}'
 
     def body_repr(self):                          # pylint: disable=no-self-use
         """Format a simple representation of this element's body.
 
         This is intended for test support. The exact format may change between
         releases.
         """
-        return ''
+        return ''                                            # pragma: no cover
 
     def file_text(self):                          # pylint: disable=no-self-use
         """Generate the text that should be written to a file."""
         return ''
 
-    def clean(self):
+    def clean(self) -> Element | None:
         """Clean the source lines.
 
         Tabs are expanded and whitespace is trimmed from the end of each line.
         """
         self.source_lines = [
             line.expandtabs().rstrip() for line in self.source_lines]
+        return None
 
     def neighbour(
             self, *, backwards: bool, within_group: bool,
             predicate=lambda _el: True) -> Snippet | None:
         """Get this element's immediate neighbour.
 
         :backwards:    If set then find preceding neighbour.
@@ -225,44 +223,45 @@
             if i == 1:
                 if within_group and snippet.parent is not self.parent:
                     return None
                 else:
                     return snippet
         return None
 
+    @classmethod
+    def _uid_base_name(cls):
+        return cls.__name__.lower()
+
 
 class PlaceHolder(Element):
     """A place holder used in empty groups."""
 
+    id_source = itertools.count()
+
     @staticmethod
     def is_last() -> bool:
         """Return false."""
-        return False
+        return False                                         # pragma: no cover
 
 
 class TextualElement(Element):
     """An `Element` that holds text."""
 
+    id_source = itertools.count()
     marker = None
 
     def add(self, line):
         """Add a line to this element."""
         self._source_lines.append(line)
 
     @property
     def text(self) -> str:
         """Build the plain text for this snippet."""
         return '\n'.join(self.source_lines)
 
-    def as_lines(self):
-        """Build the file content lines for this snippet."""
-        lines = [f'  {self.marker}\n'] if self.marker else []
-        lines.extend(f'{line}\n' for line in self.source_lines)
-        return lines
-
     @property
     def body(self) -> str:
         """The text that forms the body of this element, suitably cleaned.
 
         The first line is discarded along with any trailing blanks lines.
         Tab characters are expanded and then common leading whitespace is
         removed from the remaining lines.
@@ -291,65 +290,68 @@
 
     This includes:
 
     - Additional vertical space.
     = Comment blocks.
     """
 
+    id_source = itertools.count()
+    has_uid: bool = False
+
     def file_text(self):
         """Generate the text that should be written to a file."""
         return '\n'.join(self.source_lines) + '\n'
 
-    def clean(self) -> Element | None:
-        """Clean the source lines."""
-        if self.first_line is not None:
-            self.source_lines = [self.first_line,  *self.source_lines]
-        return super().clean()
-
 
 class Snippet(TextualElement):
     """A plain text snippet."""
 
+    id_source = itertools.count()
     marker = '@text@'
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._marked_lines = []
 
     @property
     def marked_lines(self):
         """The snippet's lines, with keywords marked up."""
+        keywords = self.parent.keywords()
         if not self._marked_lines:
-            keywords = self.parent.keywords()
-            self._marked_lines = []
-            for line in self.body.splitlines():
-                newline = line
-                for w in keywords:
-                    rep = f'\u2e24{colors.keyword_code(w)}{w}\u2e25'
-                    newline = newline.replace(w, rep)
-                self._marked_lines.append(newline)
+            if keywords:
+                ored_words = '|'.join(keywords)
+                expr = rf'\b({ored_words})\b'
+                r_words = re.compile(expr)
+                self._marked_lines = []
+                for line in self.body.splitlines():
+                    parts = r_words.split(line)
+                    new_parts = []
+                    for i, part in enumerate(parts):
+                        if i & 1:
+                            code = colors.keyword_code(part)
+                            rep = f'\u2e24{code}{part}\u2e25'
+                            new_parts.append(rep)
+                        else:
+                            new_parts.append(part)
+                    self._marked_lines.append(''.join(new_parts))
+            else:
+                self._marked_lines = self.body.splitlines()
         return self._marked_lines
 
     @property
     def marked_text(self):
         """The snippet's text, with keywords marked up."""
         lines = textwrap.dedent('\n'.join(self.marked_lines)).splitlines()
-        while lines and not lines[-1].strip():
-            lines.pop()
-        return '\n'.join(lines)
+        return widgets.render_text('\n'.join(lines))
 
     def reset(self):
         """Clear any cached state."""
         self._marked_lines = []
         self.dirty = True
 
-    def is_first(self) -> bool:
-        """Test if a snippet is the first in its group."""
-        return self.parent.is_first_snippet(self)
-
     def is_last(self) -> bool:
         """Test if a snippet is the last in its group."""
         return self.parent.is_last_snippet(self)
 
     def md_lines(self):
         """Provide snippet lines in Markdown format.
 
@@ -363,18 +365,15 @@
         inst.source_lines = list(self.source_lines)
         self.parent.add(inst, after=self)
         return inst
 
     def set_text(self, text):
         """Set the text for this snippet."""
         self._marked_lines = []
-        lines = [f'   {line}' for line in text.splitlines()]
-        if lines[-1].strip():
-            lines.append('')
-        self.source_lines = lines
+        self.source_lines = text.splitlines()
 
     def clean(self) -> Element | None:
         """Clean the source lines.
 
         Tabs are expanded and whitespace is trimmed from the end of each line.
         Trailing blank lines are deleted and common leading white space
         removed.
@@ -406,18 +405,29 @@
     def md_lines(self):
         """Provide snippet lines in Markdown format.
 
         This simply provides unmodified lines.
         """
         return self.body.splitlines()
 
+    @property
+    def marked_text(self):
+        """The snippet's text, with keywords marked up."""
+        lines = textwrap.dedent('\n'.join(self.marked_lines)).splitlines()
+        return '\n'.join(lines)
+
+    @classmethod
+    def _uid_base_name(cls):
+        return 'snippet'
+
 
 class KeywordSet(TextualElement):
     """An element holding a set of keywords."""
 
+    id_source = itertools.count()
     marker = '@keywords@'
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.words = set()
 
     def add(self, line):
@@ -471,60 +481,54 @@
 
     marker = '@title:'
 
 
 class GroupDebugMixin:
     """Support for test and debug of the `Group`` class."""
 
-    def indexed_group(self, idx):
-        """Get a group using an index.
-
-        :idx: The group index. Negative indices are not supported.
-        """
-        for i, group in enumerate(self.groups.values()):
-            if i == idx:
-                return group
-
-        message = f'Subgroup index ({idx}) out of range'
-        raise IndexError(message)
-
     def outline_repr(self, end='\n'):
         """Format a simple group-only outline representation of the tree.
 
         This is intended for test support. The exact format may change between
         releases.
         """
         s = [self.name]
         for g in self.groups.values():
             s.append(g.outline_repr(end=''))
         return '\n'.join(s) + end
 
-    def full_repr(self, end='\n'):
+    def full_repr(self, end='\n', *, debug: bool = False):
         """Format a simple outline representation of the tree.
 
         This is intended for test support. The exact format may change between
         releases.
         """
-        s = [f'Group: {self.name}']
+        if debug:
+            s = [f'Group: {self.name} {self.uid()}']         # pragma: no cover
+        else:
+            s = [f'Group: {self.name}']
         for c in self.children:
-            s.append(c.full_repr(end=''))
+            if not isinstance(c, PlaceHolder):
+                s.append(c.full_repr(end='', debug=debug))
         for g in self.groups.values():
-            s.append(g.full_repr(end=''))
+            s.append(g.full_repr(end='', debug=debug))
         return '\n'.join(s) + end
 
 
 class Group(GroupDebugMixin, Element):
     """A group of snippets and/or sub groups."""
 
     # pylint: disable=too-many-public-methods
+    id_source = itertools.count()
     all_tags: ClassVar[set[str]] = set()
 
     def __init__(self, name, parent=None, tag_text=''):
         super().__init__(parent)
         self.name = name
+        self.title = ''
         self.groups = {}
         tags = {t.strip() for t in tag_text.split()}
         self.tags = sorted(tags)
         for t in self.tags:
             self.all_tags.add(t)
         self.children = []
 
@@ -580,22 +584,14 @@
         self.children[0:0] = [kws]
 
         if self.parent:
             snippets = [el for el in self.children if isinstance(el, Snippet)]
             if not snippets:
                 self.children.append(PlaceHolder(parent=self))
 
-    def is_empty(self):
-        """Test whether this group has zero children."""
-        return bool(self.children)
-
-    def snippets(self) -> list[Snippet]:
-        """Provide this group's snippets."""
-        return [c for c in self.children if isinstance(c, Snippet)]
-
     def basic_walk(self, *, backwards: bool):
         """Iterate over the entire tree of groups and snippets.
 
         :backwards:
             If set the walk in reverse order; i.e. last snippt is visited
             first.
         """
@@ -639,25 +635,14 @@
     def walk_snippets(self, *, first_id: str = '', backwards: bool):
         """Iterate over all snippets."""
         yield from self.walk(
             predicate=lambda el: isinstance(el, Snippet),
             first_id=first_id,
             backwards=backwards)
 
-    def walk_groups(self, *, backwards: bool):
-        """Iterate over all groups."""
-        yield from self.walk(
-            predicate=lambda el: isinstance(el, Group),
-            backwards=backwards)
-
-    def is_first_snippet(self, snippet: Snippet) -> bool:
-        """Test if a snippet is the first in this gruop."""
-        snippets = [el for el in self.children if isinstance(el, Snippet)]
-        return snippets and snippets[0] is snippet
-
     def is_last_snippet(self, snippet: Snippet) -> bool:
         """Test if a snippet is the last in this gruop."""
         snippets = [el for el in self.children if isinstance(el, Snippet)]
         return snippets and snippets[-1] is snippet
 
     def first_snippet(self) -> Snippet | None:
         """Get the first snippet, if any."""
@@ -669,62 +654,14 @@
     def find_element_by_uid(self, uid) -> Element | None:
         """Find an element with the given UID."""
         for el in self.walk(backwards=False):
             if el.uid() == uid:
                 return el
         return None
 
-    def find_snippet_before_id(self, uid):
-        """Find the snippet before the one with the given UID."""
-        def is_textual(el):
-            return isinstance(el, Snippet)
-
-        prev = None
-        for el in self.walk(backwards=False):
-            if is_textual(el):
-                if el.uid() == uid:
-                    return prev
-                else:
-                    prev = el
-        return None
-
-    def find_snippet_after_id(self, uid):
-        """Find the snippet after the one with the given UID."""
-        for i, el in enumerate(
-                self.walk_snippets(first_id=uid, backwards=False)):
-            if i == 1:
-                return el
-        return None
-
-    # TODO: Should soon lose this.
-    def iter_from_to(self, first, second):
-        """Iterate iver a subset of elements."""
-        def is_textual(el):
-            return isinstance(el, Snippet)
-
-        in_range = False
-        for el in self.walk(backwards=False):
-            if is_textual(el):
-                if in_range:
-                    yield el
-                if el.uid() == first:
-                    in_range = True
-                    yield el
-            if el.uid() == second:
-                break
-
-    def correctly_ordered(self, first, second):
-        """Test whether first is after second."""
-        for el in self.walk(backwards=False):
-            if el.uid() == first:
-                return True
-            elif el.uid() == second:
-                return False
-        return False
-
     def keyword_set(self) -> KeywordSet | None:
         """Find the keyword set, if any, for this group."""
         return self.children[0]
 
     def keywords(self) -> set[str]:
         """Provide all the keywords applicable to this group's snippets."""
         return self.keyword_set().words
@@ -793,15 +730,16 @@
         else:
             return False
 
     def handle_title(self, line):
         """Handle a title line."""
         if line.startswith('@title:'):
             self.store()
-            self.cur_group.add(Title(parent=self.cur_group))
+            _, _, title = line.partition(':')
+            self.root.title = title.strip()
             self.el = PreservedText(parent=None)
             return True
         else:
             return False
 
     def handle_group(self, line):
         """Handle a group start line."""
@@ -850,15 +788,15 @@
         self.store()
         self.root.clean()
         if not self.root.groups:
             sys.exit(f'File {self.path} contains no groups')
 
         for el in self.root.walk_snippets(backwards=False):
             el.reset()
-        return self.root, self.title
+        return self.root, self.root.title
 
 
 # Conveniant types.
 SnippetLike = Snippet | PlaceHolder
 
 
 def is_snippet_like(el: Element) -> bool:
@@ -879,14 +817,16 @@
     loader = Loader(path)
     return loader.load()
 
 
 def save(path, root):
     """Save a snippet tree to a file."""
     with Path(path).open('wt', encoding='utf8') as f:
+        if root.title:
+            f.write(f'@title: {root.title}\n')
         for el in root.walk(backwards=False):
             f.write(el.file_text())
             if isinstance(el, Group):
                 kws = el.keyword_set()
                 if not kws.is_empty():
                     f.write(kws.file_text())
 
@@ -905,9 +845,22 @@
     for old_name, new_name in zip(old_names, new_names):
         src_path = dirpath / old_name
         if src_path.exists():
             with suppress(OSError):
                 print('MOVE', src_path, dirpath / new_name)
                 shutil.move(src_path, dirpath / new_name)
     with suppress(OSError):
-        print('BACKUP', path, dirpath / names[0])
         shutil.copy(path, dirpath / names[0])
+
+
+def reset_for_tests():
+    """Perform a 'system' reset for test purposes.
+
+    This is not intended for non-testing use.
+    """
+    Element.id_source = itertools.count()
+    PlaceHolder.id_source = itertools.count()
+    TextualElement.id_source = itertools.count()
+    PreservedText.id_source = itertools.count()
+    Snippet.id_source = itertools.count()
+    KeywordSet.id_source = itertools.count()
+    Group.id_source = itertools.count()
```

### Comparing `clippets-0.0.1/src/clippets/widgets.py` & `clippets-0.1.0/src/clippets/widgets.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """Application specific widgets."""
+from __future__ import annotations
 
-import asyncio
 import re
 import unicodedata
 from collections import defaultdict
 from contextlib import suppress
-from typing import Iterable, Optional
+from typing import Iterable
 
 import rich.repr
 from rich.style import Style
 from rich.text import Span, Text
 from textual import events
-from textual._wait import wait_for_idle
-from textual.app import App, Binding
+from textual.app import App
 from textual.containers import Grid, VerticalScroll
 from textual.keys import (
     REPLACED_KEYS, _character_to_key, _get_unicode_name_from_key)
 from textual.screen import ModalScreen
 from textual.widgets import Button, Footer, Input, Label, Markdown, Static
 from textual.widgets._markdown import MarkdownBlock
 
 from .colors import keyword_colors
 
 # We 'smuggle' keyword information by surrounding them with specific Unicode
-# low quotes. These look quite like commas, making is extremely unlikely that
+# low quotes. These look quite like commas, making it extremely unlikely that
 # anyone would would use them a snippet text.
 re_keyword = re.compile('\u2e24([^\u2e25]*)\u2e25')
+re_keyword_start = re.compile('\u2e24[^\u2e25]*')
 
 
 class StdMixin:                        # pylint: disable=too-few-public-methods
     """Common code for various widgets."""
 
     def on_enter(self, _event):
         """Handle a mouse entering a widget."""
@@ -88,14 +88,15 @@
 
     def compose(self):
         """Build the widget hierarchy."""
         yield Grid(
             Label('Choose action', id='question'),
             Button('Edit', variant='primary', id='edit'),
             Button('Duplicate', variant='primary', id='duplicate'),
+            Button('Move', variant='primary', id='move'),
             Button('Cancel', variant='primary', id='cancel'),
             id='dialog',
         )
 
     def on_button_pressed(self, event: Button.Pressed) -> None:
         """Process a mouse click on a button."""
         self.dismiss(event.button.id)
@@ -134,22 +135,22 @@
             'footer--description')
 
         bindings = self.app.active_shown_bindings()
         action_to_bindings = defaultdict(list)
         for binding in bindings:
             action_to_bindings[binding.action].append(binding)
 
-        for _, bindings in action_to_bindings.items():
+        for bindings in action_to_bindings.values():
             binding = bindings[0]
             if binding.key_display is None:
                 key_display = self.app.get_key_display(binding.key)
                 if key_display is None:
-                    key_display = binding.key.upper()
+                    key_display = binding.key.upper()        # pragma: no cover
             else:
-                key_display = binding.key_display
+                key_display = binding.key_display            # pragma: no cover
             hovered = self.highlight_key == binding.key
             key_text = Text.assemble(
                 (
                     f' {key_display} ',
                     highlight_key_style if hovered else key_style),
                 (
                     f' {binding.description} ',
@@ -161,89 +162,98 @@
                     'key': binding.key,
                 },
             )
             text.append_text(key_text)
         return text
 
 
+def gen_highlight_spans(
+        text: str, base_style: Style, off: int) -> tuple[list[Span], str]:
+    """Split text into spans based on highlighting."""
+    parts = re_keyword.split(text)
+    spans = []
+    new_parts = []
+    for i, p in enumerate(parts):
+        if i & 1:
+            substr = p[1:]
+            cc = p[0]
+            color = keyword_colors.get(cc, 'green')
+            style = base_style + Style(color=color)
+        else:
+            substr = re_keyword_start.sub('', p)
+            substr = substr.replace('\u2e25(', '')
+            style = base_style
+        if substr:
+            new_parts.append(substr)
+            spans.append(Span(off, off + len(substr), style))
+            off += len(substr)
+
+    return spans, ''.join(new_parts)
+
+
+def render_text(text: Text | str) -> Text:
+    """Render specially marked up text."""
+    if isinstance(text, str):
+        text = Text(text, spans=[Span(0, len(text), Style())])
+    raw_text = text.plain
+    if '\u2e24' in raw_text:
+        new_spans = []
+        new_parts = []
+        off = 0
+        for span in text.spans:
+            substr = raw_text[span.start:span.end]
+            new_subspans, new_substr = gen_highlight_spans(
+                substr, span.style, off)
+            new_spans.extend(new_subspans)
+            new_parts.append(new_substr)
+            off += len(new_parts[-1])
+        return Text(''.join(new_parts), spans=new_spans)
+    else:
+        return text
+
+
 class ExtendMixin:
     """Namespace to hold ``textual`` extension methods."""
 
     def on_enter(self, ev):
         """Perform action the mouse enters the widtget."""
         with suppress(AttributeError):
             self.parent.on_enter(ev)
 
     def set_content(self, text: Text) -> None:
         """Over-ride set_content to highlight keywords."""
-        def trim_spans(off, n):
-            for i, span in enumerate(spans):
-                a, b, style = span
-                if a > off:
-                    a -= n
-                if b > off:
-                    b -= n
-                spans[i] = Span(a, b, style)
-
-        if '\u2e24' in text.plain:
-            text = text.copy()
-            parts = re_keyword.split(text.plain)
-            new_parts = []
-            off = 0
-            spans = text.spans
-            for i, p in enumerate(parts):
-                if i & 1:
-                    new_parts.append(p[1:])
-                    cc = p[0]
-                    trim_spans(off, 2)
-                    off += len(p) - 1
-                    trim_spans(off, 1)
-                    spans.append(Span(
-                        off - len(p) + 1, off,
-                        Style(color=keyword_colors.get(cc, 'green'))))
-                else:
-                    new_parts.append(p)
-                    off += len(p)
-            text._text = [''.join(new_parts)]                    # noqa: SLF001
-            text.spans = spans
-        self._text = text
-        self.update(text)
+        self._text = render_text(text)
+        self.update(self._text)
 
     async def _press_keys(self, keys: Iterable[str]) -> None:
         """Simulate a key press.
 
         This is a copy of the standrard Textual code except:
 
+        - the 'wait:...' form of key is not handled; my test runner handles
+          delays.
         - print calls have been removed.
         - assertions have been removed.
+        - some wait calls have been removed.
         """
         app = self
         driver = app._driver                                     # noqa: SLF001
-        await wait_for_idle(0)
         for key in keys:
-            if key.startswith('wait:'):
-                _, wait_ms = key.split(':')
-                await asyncio.sleep(float(wait_ms) / 1000)
-                await app._animator.wait_until_complete()        # noqa: SLF001
-                await wait_for_idle(0)
-            else:
-                if len(key) == 1 and not key.isalnum():
-                    key = _character_to_key(key)                # noqa: PLW2901
-                original_key = REPLACED_KEYS.get(key, key)
-                char: Optional[str] = None
-                try:
-                    char = unicodedata.lookup(
-                        _get_unicode_name_from_key(original_key))
-                except KeyError:
-                    char = key if len(key) == 1 else None
-                key_event = events.Key(key, char)
-                key_event._set_sender(app)                       # noqa: SLF001
-                driver.send_event(key_event)
-                await wait_for_idle(0)
+            if len(key) == 1 and not key.isalnum():
+                key = _character_to_key(key)                    # noqa: PLW2901
+            original_key = REPLACED_KEYS.get(key, key)
+            char: str | None = None
+            try:
+                char = unicodedata.lookup(
+                    _get_unicode_name_from_key(original_key))
+            except KeyError:
+                char = key if len(key) == 1 else None
+            key_event = events.Key(key, char)
+            key_event._set_sender(app)                           # noqa: SLF001
+            driver.send_event(key_event)
 
         await app._animator.wait_until_complete()                # noqa: SLF001
-        await wait_for_idle(0)
 
 
 MarkdownBlock.on_enter = ExtendMixin.on_enter
 MarkdownBlock.set_content = ExtendMixin.set_content
 App._press_keys = ExtendMixin._press_keys                        # noqa: SLF001
```

### Comparing `clippets-0.0.1/src/clippets/win.py` & `clippets-0.1.0/src/clippets/win.py`

 * *Files identical despite different names*

### Comparing `clippets-0.0.1/src/clippets.egg-info/SOURCES.txt` & `clippets-0.1.0/src/clippets.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -15,10 +15,16 @@
 src/clippets/win.py
 src/clippets.egg-info/PKG-INFO
 src/clippets.egg-info/SOURCES.txt
 src/clippets.egg-info/dependency_links.txt
 src/clippets.egg-info/entry_points.txt
 src/clippets.egg-info/requires.txt
 src/clippets.egg-info/top_level.txt
+tests/test_clipboard.py
 tests/test_editing.py
+tests/test_filtering.py
+tests/test_help.py
+tests/test_kb_selection.py
+tests/test_keywords.py
 tests/test_load_save.py
-tests/test_snapshots.py
+tests/test_misc_ui.py
+tests/test_moving.py
```

### Comparing `clippets-0.0.1/tests/test_load_save.py` & `clippets-0.1.0/tests/test_load_save.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Loading and saving the clippets file
+"""Loading and saving the clippets file.
 
 The clippets file contains a mixture of the following:
 
 Comments
     Any unindented line that starts with a hash ('#').
 
 One-off directives.
@@ -85,16 +85,15 @@
         <ROOT>
         Main''')
     assert root.outline_repr() == expect
     expect = clean_text('''
         Group: <ROOT>
         KeywordSet:
         Group: Main
-        KeywordSet:
-        PlaceHolder:''')
+        KeywordSet:''')
     assert expect == root.full_repr()
 
 
 def test_single_entry_group(snippet_infile):
     """A file with one snippet is valid."""
     populate(snippet_infile, '''
         Main
@@ -173,14 +172,15 @@
     """
     populate(snippet_infile, '''
         Main
           @keywords@
             one two
           @text@
             Snippet 1
+
         Second
           @md@
             Snippet 2
           @keywords@
             three four
           @keywords@
             five three
@@ -194,14 +194,15 @@
     assert root.outline_repr() == expect
     expect = clean_text(r'''
         Group: <ROOT>
         KeywordSet:
         Group: Main
         KeywordSet: one two
         Snippet: 'Snippet 1'
+        PreservedText: ''
         Group: Second
         KeywordSet: five four three
         MarkdownSnippet: 'Snippet 2'
     ''')
     assert root.full_repr() == expect
 
 
@@ -229,14 +230,46 @@
     ''')
     populate(snippet_infile, expected)
     root, _ = snippets.load(snippet_infile.name)
     snippets.save(snippet_outfile.name, root)
     assert str(snippet_outfile) == expected
 
 
+def test_nested_groups_are_handled(snippet_infile, snippet_outfile):
+    """Nested sub-groups are correcttly saved."""
+    expected = clean_text('''
+        Main
+          @md@
+            Snippet 1
+        Main : Subgroup
+          @md@
+            Snippet 2
+    ''')
+    populate(snippet_infile, expected)
+    root, _ = snippets.load(snippet_infile.name)
+    snippets.save(snippet_outfile.name, root)
+    assert str(snippet_outfile) == expected
+
+
+def test_nested_groups_with_tags_are_handled(snippet_infile, snippet_outfile):
+    """Nested sub-groups with tags are correcttly saved."""
+    expected = clean_text('''
+        Main
+          @md@
+            Snippet 1
+        Main : Subgroup [tag-a tag-b]
+          @md@
+            Snippet 2
+    ''')
+    populate(snippet_infile, expected)
+    root, _ = snippets.load(snippet_infile.name)
+    snippets.save(snippet_outfile.name, root)
+    assert expected == str(snippet_outfile)
+
+
 def test_leading_comment_block_is_preserved(snippet_infile, snippet_outfile):
     """Writing a file preserves any leading block comment."""
     expected = populate(snippet_infile, '''
         # A leading
         # comment block.
         Main
           @md@
@@ -309,7 +342,27 @@
 
         # Comment
         |
     ''')
     root, _ = snippets.load(snippet_infile.name)
     snippets.save(snippet_outfile.name, root)
     assert expected == str(snippet_outfile)
+
+
+def test_title_is_preserved(snippet_infile, snippet_outfile):
+    """An user supplied title is saved."""
+    expected = populate(snippet_infile, '''
+        @title: User supplied title
+        Main
+          @keywords@
+            one
+            two
+          @md@
+            Snippet 1
+
+        # Comment
+        |
+    ''')
+    root, title = snippets.load(snippet_infile.name)
+    snippets.save(snippet_outfile.name, root)
+    assert 'User supplied title' == title
+    assert expected == str(snippet_outfile)
```

