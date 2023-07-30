# Comparing `tmp/changelog_generator-0.7-py3-none-any.whl.zip` & `tmp/changelog_generator-0.7b0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8442 bytes, number of entries: 10
--rw-r--r--  2.0 unx       16 b- defN 23-Jul-30 17:51 changemaker/__init__.py
--rw-r--r--  2.0 unx      471 b- defN 23-Jul-30 17:51 changemaker/debugger.py
--rw-r--r--  2.0 unx     7771 b- defN 23-Jul-30 17:51 changemaker/generator.py
--rw-r--r--  2.0 unx     2788 b- defN 23-Jul-30 17:51 changemaker/utils/rst.py
--rw-r--r--  2.0 unx     1078 b- defN 23-Jul-30 17:51 changelog_generator-0.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     6086 b- defN 23-Jul-30 17:51 changelog_generator-0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-30 17:51 changelog_generator-0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       57 b- defN 23-Jul-30 17:51 changelog_generator-0.7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 23-Jul-30 17:51 changelog_generator-0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      860 b- defN 23-Jul-30 17:51 changelog_generator-0.7.dist-info/RECORD
-10 files, 19231 bytes uncompressed, 6954 bytes compressed:  63.8%
+Zip file size: 8455 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       71 b- defN 23-Jul-30 17:32 changemaker/__init__.py
+-rw-r--r--  2.0 unx      471 b- defN 23-Jul-30 17:32 changemaker/debugger.py
+-rw-r--r--  2.0 unx     7539 b- defN 23-Jul-30 17:32 changemaker/generator.py
+-rw-r--r--  2.0 unx     2788 b- defN 23-Jul-30 17:32 changemaker/utils/rst.py
+-rw-r--r--  2.0 unx     1078 b- defN 23-Jul-30 17:32 changelog_generator-0.7b0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6075 b- defN 23-Jul-30 17:32 changelog_generator-0.7b0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-30 17:32 changelog_generator-0.7b0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       57 b- defN 23-Jul-30 17:32 changelog_generator-0.7b0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 23-Jul-30 17:32 changelog_generator-0.7b0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      872 b- defN 23-Jul-30 17:32 changelog_generator-0.7b0.dist-info/RECORD
+10 files, 19055 bytes uncompressed, 6943 bytes compressed:  63.6%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: changemaker/generator.py
 Comment: 
 
 Filename: changemaker/utils/rst.py
 Comment: 
 
-Filename: changelog_generator-0.7.dist-info/LICENSE
+Filename: changelog_generator-0.7b0.dist-info/LICENSE
 Comment: 
 
-Filename: changelog_generator-0.7.dist-info/METADATA
+Filename: changelog_generator-0.7b0.dist-info/METADATA
 Comment: 
 
-Filename: changelog_generator-0.7.dist-info/WHEEL
+Filename: changelog_generator-0.7b0.dist-info/WHEEL
 Comment: 
 
-Filename: changelog_generator-0.7.dist-info/entry_points.txt
+Filename: changelog_generator-0.7b0.dist-info/entry_points.txt
 Comment: 
 
-Filename: changelog_generator-0.7.dist-info/top_level.txt
+Filename: changelog_generator-0.7b0.dist-info/top_level.txt
 Comment: 
 
-Filename: changelog_generator-0.7.dist-info/RECORD
+Filename: changelog_generator-0.7b0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## changemaker/__init__.py

```diff
@@ -1 +1,3 @@
-version = "0.7"
+from changemaker.generator import main  # noqa: F401
+
+version = "0.7b"
```

## changemaker/generator.py

```diff
@@ -3,15 +3,14 @@
 import time
 from datetime import datetime
 from typing import List, NoReturn
 
 import click
 
 from changemaker import debugger
-from changemaker import version as pkg_version
 
 options = {'debug': False, 'reverse': False, 'start': 0.0}
 
 
 def get_branches() -> List[str]:
     """Runs ``git branch`` command to get the branches available for the repo.
 
@@ -155,29 +154,25 @@
         debugger.info(f"{filename!r} was created in: {round(float(time.time() - options['start']), 2)}s")
 
 
 @click.command()
 @click.pass_context
 @click.argument('reverse', required=False)
 @click.argument('debug', required=False)
-@click.option("-v", "--version", required=False, is_flag=True, help="Get version of the package")
 @click.option("-b", "--branch", help="The branch to read the commit notes from")
 @click.option("-f", "--filename", help="Filename where the commit notes should be stored")
 @click.option("-t", "--title", help="Title under which the commit notes should be stored")
-def main(*args, reverse: str = None, debug: str = None, version: str = None,
+def main(*args, reverse: str = None, debug: str = None,
          branch: str = None, filename: str = None, title: str = None) -> None:
     """Generate a reStructuredText/Markdown file using github commit notes.
 
     Run 'changelog reverse' to generate changelog in reverse order.
 
     Run 'changelog debug' to enable debug mode.
     """
-    if version:
-        debugger.info(pkg_version)
-        return
     reverse = reverse or ''
     debug = debug or ''
 
     # The following makes arguments interchangeable for convenience
     if reverse.lower() == 'reverse':
         options['reverse'] = True
     elif reverse.lower() == 'debug':
```

## Comparing `changelog_generator-0.7.dist-info/LICENSE` & `changelog_generator-0.7b0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `changelog_generator-0.7.dist-info/METADATA` & `changelog_generator-0.7b0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: changelog-generator
-Version: 0.7
+Version: 0.7b0
 Summary: Python module to, generate well formatted commit notes from git commit history.
 Author-email: Vignesh Sivanandha Rao <svignesh1793@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 Vignesh Sivanandha Rao
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,15 +26,15 @@
         SOFTWARE.
 Project-URL: Homepage, https://github.com/thevickypedia/changelog-generator
 Project-URL: Docs, https://thevickypedia.github.io/changelog-generator/
 Project-URL: Source, https://github.com/thevickypedia/changelog-generator
 Project-URL: Bug Tracker, https://github.com/thevickypedia/changelog-generator/issues
 Project-URL: Release Notes, https://github.com/thevickypedia/changelog-generator/blob/main/release_notes.rst
 Keywords: changelog,automate,commits
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Version Control :: Git
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

