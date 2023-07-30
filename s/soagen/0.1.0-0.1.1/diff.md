# Comparing `tmp/soagen-0.1.0.tar.gz` & `tmp/soagen-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soagen-0.1.0.tar", last modified: Sat Jul 29 16:41:39 2023, max compression
+gzip compressed data, was "soagen-0.1.1.tar", last modified: Sun Jul 30 14:46:21 2023, max compression
```

## Comparing `soagen-0.1.0.tar` & `soagen-0.1.1.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 16:41:39.449712 soagen-0.1.0/
--rw-rw-rw-   0        0        0       62 2023-07-29 16:31:26.000000 soagen-0.1.0/CHANGELOG.md
--rw-rw-rw-   0        0        0     1064 2023-07-21 10:29:49.000000 soagen-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1372 2023-07-29 16:41:39.448713 soagen-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      467 2023-07-29 16:32:13.000000 soagen-0.1.0/README.md
--rw-rw-rw-   0        0        0     1893 2023-07-29 16:15:31.000000 soagen-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-29 16:41:39.449712 soagen-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-29 16:41:39.404713 soagen-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-29 16:41:39.426712 soagen-0.1.0/src/soagen/
--rw-rw-rw-   0        0        0      477 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/__init__.py
--rw-rw-rw-   0        0        0      918 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/column.py
--rw-rw-rw-   0        0        0     5040 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/config.py
--rw-rw-rw-   0        0        0      952 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/configurable.py
--rw-rw-rw-   0        0        0    19105 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/cpp.py
--rw-rw-rw-   0        0        0      574 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/errors.py
--rw-rw-rw-   0        0        0    10934 2023-07-29 16:23:15.000000 soagen-0.1.0/src/soagen/header_file.py
-drwxrwxrwx   0        0        0        0 2023-07-29 16:41:39.442713 soagen-0.1.0/src/soagen/hpp/
--rw-rw-rw-   0        0        0     5621 2023-07-29 16:38:51.000000 soagen-0.1.0/src/soagen/hpp/.clang-format
--rw-rw-rw-   0        0        0    11287 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/hpp/allocator.hpp
--rw-rw-rw-   0        0        0    31723 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/hpp/column_traits.hpp
-drwxrwxrwx   0        0        0        0 2023-07-29 16:41:39.446713 soagen-0.1.0/src/soagen/hpp/generated/
--rw-rw-rw-   0        0        0     9857 2023-07-29 16:38:30.000000 soagen-0.1.0/src/soagen/hpp/generated/compressed_pair.hpp
--rw-rw-rw-   0        0        0     2935 2023-07-29 16:38:30.000000 soagen-0.1.0/src/soagen/hpp/generated/core.hpp
--rw-rw-rw-   0        0        0     7897 2023-07-29 16:38:31.000000 soagen-0.1.0/src/soagen/hpp/generated/functions.hpp
--rw-rw-rw-   0        0        0    43678 2023-07-29 16:38:32.000000 soagen-0.1.0/src/soagen/hpp/generated/preprocessor.hpp
--rw-rw-rw-   0        0        0      421 2023-07-29 16:38:30.000000 soagen-0.1.0/src/soagen/hpp/generated/version.hpp
--rw-rw-rw-   0        0        0      816 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/hpp/header_end.hpp
--rw-rw-rw-   0        0        0      929 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/hpp/header_start.hpp
--rw-rw-rw-   0        0        0    15165 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/hpp/iterator.hpp
--rw-rw-rw-   0        0        0    24779 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/hpp/meta.hpp
--rw-rw-rw-   0        0        0     5469 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/hpp/mixins.hpp
--rw-rw-rw-   0        0        0     7272 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/hpp/row.hpp
-drwxrwxrwx   0        0        0        0 2023-07-29 16:41:39.447713 soagen-0.1.0/src/soagen/hpp/single/
--rw-rw-rw-   0        0        0   234341 2023-07-29 16:38:50.000000 soagen-0.1.0/src/soagen/hpp/single/soagen.hpp
--rw-rw-rw-   0        0        0      979 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/hpp/soagen.hpp
--rw-rw-rw-   0        0        0    53309 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/hpp/table.hpp
--rw-rw-rw-   0        0        0    41432 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/hpp/table_traits.hpp
--rw-rw-rw-   0        0        0     1103 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/injectors.py
--rw-rw-rw-   0        0        0     3926 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/log.py
--rw-rw-rw-   0        0        0    21973 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/main.py
--rw-rw-rw-   0        0        0     3018 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/metavars.py
--rw-rw-rw-   0        0        0     5174 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/natvis_file.py
--rw-rw-rw-   0        0        0     1971 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/paths.py
--rw-rw-rw-   0        0        0     5464 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/preprocessor.py
--rw-rw-rw-   0        0        0     2494 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/schemas.py
--rw-rw-rw-   0        0        0    66861 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/struct.py
--rw-rw-rw-   0        0        0     2165 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/type_list.py
--rw-rw-rw-   0        0        0     2697 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/utils.py
--rw-rw-rw-   0        0        0     3782 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/variable.py
--rw-rw-rw-   0        0        0      616 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/version.py
--rw-rw-rw-   0        0        0        6 2023-07-29 16:20:11.000000 soagen-0.1.0/src/soagen/version.txt
--rw-rw-rw-   0        0        0    12323 2023-07-29 16:15:31.000000 soagen-0.1.0/src/soagen/writer.py
-drwxrwxrwx   0        0        0        0 2023-07-29 16:41:39.433713 soagen-0.1.0/src/soagen.egg-info/
--rw-rw-rw-   0        0        0     1372 2023-07-29 16:41:39.000000 soagen-0.1.0/src/soagen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1364 2023-07-29 16:41:39.000000 soagen-0.1.0/src/soagen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 16:41:39.000000 soagen-0.1.0/src/soagen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-29 16:41:39.000000 soagen-0.1.0/src/soagen.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2023-07-29 16:41:39.000000 soagen-0.1.0/src/soagen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-29 16:41:39.000000 soagen-0.1.0/src/soagen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-07-28 06:00:37.000000 soagen-0.1.0/src/soagen.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-07-30 14:46:21.692365 soagen-0.1.1/
+-rw-rw-rw-   0        0        0       95 2023-07-30 14:43:28.000000 soagen-0.1.1/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1064 2023-07-21 10:29:49.000000 soagen-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     1408 2023-07-30 14:46:21.692365 soagen-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      466 2023-07-30 08:46:14.000000 soagen-0.1.1/README.md
+-rw-rw-rw-   0        0        0     1893 2023-07-29 16:15:31.000000 soagen-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-30 14:46:21.692365 soagen-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-30 14:46:21.645365 soagen-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-30 14:46:21.669365 soagen-0.1.1/src/soagen/
+-rw-rw-rw-   0        0        0      477 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/__init__.py
+-rw-rw-rw-   0        0        0      870 2023-07-30 13:58:17.000000 soagen-0.1.1/src/soagen/column.py
+-rw-rw-rw-   0        0        0     5008 2023-07-30 12:44:09.000000 soagen-0.1.1/src/soagen/config.py
+-rw-rw-rw-   0        0        0      952 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/configurable.py
+-rw-rw-rw-   0        0        0    19129 2023-07-30 10:56:14.000000 soagen-0.1.1/src/soagen/cpp.py
+-rw-rw-rw-   0        0        0      574 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/errors.py
+-rw-rw-rw-   0        0        0    10645 2023-07-30 12:51:27.000000 soagen-0.1.1/src/soagen/header_file.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:46:21.686366 soagen-0.1.1/src/soagen/hpp/
+-rw-rw-rw-   0        0        0     5621 2023-07-30 14:42:24.000000 soagen-0.1.1/src/soagen/hpp/.clang-format
+-rw-rw-rw-   0        0        0    11287 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/hpp/allocator.hpp
+-rw-rw-rw-   0        0        0    31745 2023-07-30 10:23:11.000000 soagen-0.1.1/src/soagen/hpp/column_traits.hpp
+drwxrwxrwx   0        0        0        0 2023-07-30 14:46:21.690366 soagen-0.1.1/src/soagen/hpp/generated/
+-rw-rw-rw-   0        0        0     9857 2023-07-30 14:42:25.000000 soagen-0.1.1/src/soagen/hpp/generated/compressed_pair.hpp
+-rw-rw-rw-   0        0        0     2935 2023-07-30 14:42:25.000000 soagen-0.1.1/src/soagen/hpp/generated/core.hpp
+-rw-rw-rw-   0        0        0     7897 2023-07-30 14:42:25.000000 soagen-0.1.1/src/soagen/hpp/generated/functions.hpp
+-rw-rw-rw-   0        0        0    43678 2023-07-30 14:42:27.000000 soagen-0.1.1/src/soagen/hpp/generated/preprocessor.hpp
+-rw-rw-rw-   0        0        0      420 2023-07-30 14:40:17.000000 soagen-0.1.1/src/soagen/hpp/generated/version.hpp
+-rw-rw-rw-   0        0        0      816 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/hpp/header_end.hpp
+-rw-rw-rw-   0        0        0      929 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/hpp/header_start.hpp
+-rw-rw-rw-   0        0        0    15165 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/hpp/iterator.hpp
+-rw-rw-rw-   0        0        0    24763 2023-07-30 09:59:17.000000 soagen-0.1.1/src/soagen/hpp/meta.hpp
+-rw-rw-rw-   0        0        0     5469 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/hpp/mixins.hpp
+-rw-rw-rw-   0        0        0     7272 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/hpp/row.hpp
+drwxrwxrwx   0        0        0        0 2023-07-30 14:46:21.690366 soagen-0.1.1/src/soagen/hpp/single/
+-rw-rw-rw-   0        0        0   234058 2023-07-30 14:42:44.000000 soagen-0.1.1/src/soagen/hpp/single/soagen.hpp
+-rw-rw-rw-   0        0        0      979 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/hpp/soagen.hpp
+-rw-rw-rw-   0        0        0    53592 2023-07-30 10:14:59.000000 soagen-0.1.1/src/soagen/hpp/table.hpp
+-rw-rw-rw-   0        0        0    41432 2023-07-30 10:23:24.000000 soagen-0.1.1/src/soagen/hpp/table_traits.hpp
+-rw-rw-rw-   0        0        0     1067 2023-07-30 13:01:18.000000 soagen-0.1.1/src/soagen/includes.py
+-rw-rw-rw-   0        0        0     1103 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/injectors.py
+-rw-rw-rw-   0        0        0     3926 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/log.py
+-rw-rw-rw-   0        0        0    23113 2023-07-30 14:42:15.000000 soagen-0.1.1/src/soagen/main.py
+-rw-rw-rw-   0        0        0     3018 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/metavars.py
+-rw-rw-rw-   0        0        0     5174 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/natvis_file.py
+-rw-rw-rw-   0        0        0     1971 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/paths.py
+-rw-rw-rw-   0        0        0     6128 2023-07-30 10:13:46.000000 soagen-0.1.1/src/soagen/preprocessor.py
+-rw-rw-rw-   0        0        0     2494 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/schemas.py
+-rw-rw-rw-   0        0        0    66567 2023-07-30 13:58:31.000000 soagen-0.1.1/src/soagen/struct.py
+-rw-rw-rw-   0        0        0     2165 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/type_list.py
+-rw-rw-rw-   0        0        0     2697 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/utils.py
+-rw-rw-rw-   0        0        0     3576 2023-07-30 14:09:00.000000 soagen-0.1.1/src/soagen/variable.py
+-rw-rw-rw-   0        0        0      616 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/version.py
+-rw-rw-rw-   0        0        0        6 2023-07-30 14:40:17.000000 soagen-0.1.1/src/soagen/version.txt
+-rw-rw-rw-   0        0        0    12323 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/writer.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:46:21.675366 soagen-0.1.1/src/soagen.egg-info/
+-rw-rw-rw-   0        0        0     1408 2023-07-30 14:46:21.000000 soagen-0.1.1/src/soagen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1387 2023-07-30 14:46:21.000000 soagen-0.1.1/src/soagen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 14:46:21.000000 soagen-0.1.1/src/soagen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-30 14:46:21.000000 soagen-0.1.1/src/soagen.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2023-07-30 14:46:21.000000 soagen-0.1.1/src/soagen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-30 14:46:21.000000 soagen-0.1.1/src/soagen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-28 06:00:37.000000 soagen-0.1.1/src/soagen.egg-info/zip-safe
```

### Comparing `soagen-0.1.0/LICENSE.txt` & `soagen-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `soagen-0.1.0/PKG-INFO` & `soagen-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soagen
-Version: 0.1.0
+Version: 0.1.1
 Summary: Struct-of-Arrays generator for C++ projects.
 Author-email: Mark Gillard <mark.gillard@outlook.com.au>
 License: MIT
 Project-URL: Source, https://github.com/marzer/soagen
 Project-URL: Tracker, https://github.com/marzer/soagen/issues
 Project-URL: Funding, https://github.com/sponsors/marzer
 Keywords: c++,soa,struct-of-arrays,structure-of-arrays,struct of arrays,structure of arrays,parallel-arrays,parallel arrays,std::vector
@@ -23,20 +23,24 @@
 
 [![Sponsor](docs/images/badge-sponsor.svg)][sponsor]
 [![Gitter](docs/images/badge-gitter.svg)][gitter]
 
 <br><br>
 
 <p align="center">
-	<strong>✨&#xFE0F; This README is as stub. Please see the HTML documentation: <a href="https://marzer.github.io/soagen/">marzer.github.io/soagen</a>✨&#xFE0F;</strong>
+	<strong>✨&#xFE0F; This README is a stub. Please see the HTML documentation: <a href="https://marzer.github.io/soagen/">marzer.github.io/soagen</a>✨&#xFE0F;</strong>
 </p>
 
 <br><br>
 
 [gitter]: https://gitter.im/marzer/community
 [sponsor]: https://github.com/sponsors/marzer
 
 # Changelog
 
+## v0.1.1
+
+-   Minor refactors.
+
 ## v0.1.0
 
 -   First public release 🎉&#xFE0F;
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: soagen Version: 0.1.0 Summary: Struct-of-Arrays
+Metadata-Version: 2.1 Name: soagen Version: 0.1.1 Summary: Struct-of-Arrays
 generator for C++ projects. Author-email: Mark Gillard
 gillard@outlook.com.au> License: MIT Project-URL: Source, https://github.com/
 marzer/soagen Project-URL: Tracker, https://github.com/marzer/soagen/issues
 Project-URL: Funding, https://github.com/sponsors/marzer Keywords:
 c++,soa,struct-of-arrays,structure-of-arrays,struct of arrays,structure of
 arrays,parallel-arrays,parallel arrays,std::vector Classifier: Development
 Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: C++ Classifier: Topic :: Software
 Development :: Code Generators Classifier: Topic :: Utilities Requires-Python:
 >=3.9 Description-Content-Type: text/markdown License-File: LICENSE.txt #
 soagen Struct-of-Arrays generator for C++ projects. [![Sponsor](docs/images/
 badge-sponsor.svg)][sponsor] [![Gitter](docs/images/badge-gitter.svg)][gitter]
 
-    â¨&#xFE0F; This README is as stub. Please see the HTML documentation:
+     â¨&#xFE0F; This README is a stub. Please see the HTML documentation:
                       marzer.github.io/soagenâ¨&#xFE0F;
 
 
 [gitter]: https://gitter.im/marzer/community [sponsor]: https://github.com/
-sponsors/marzer # Changelog ## v0.1.0 - First public release ð&#xFE0F;
+sponsors/marzer # Changelog ## v0.1.1 - Minor refactors. ## v0.1.0 - First
+public release ð&#xFE0F;
```

### Comparing `soagen-0.1.0/pyproject.toml` & `soagen-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `soagen-0.1.0/src/soagen/column.py` & `soagen-0.1.1/src/soagen/column.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 
 from .configurable import Configurable
 from .metavars import *
 from .writer import *
 
 
 class Column(Configurable):
-    def __init__(self, var, prev=False):
+    def __init__(self, var):
         super().__init__(var)
         self.variable = var
         self.struct = var.struct
         self.index = -1  # set by the struct
-        self.name = 'previous_' + var.name if prev else var.name
+        self.name = var.name
         self.alignment = var.alignment
         self.type = var.type
         self.param_type = var.param_type
         self.pointer_type = var.pointer_type
         self.const_pointer_type = var.const_pointer_type
         self.default = var.default
```

### Comparing `soagen-0.1.0/src/soagen/config.py` & `soagen-0.1.1/src/soagen/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,22 +27,23 @@
         import tomli as toml
 
 
 class Config(ConfigBase):
     __schema = Schema(
         {
             Optional(r'hpp', default=dict): {object: object},
-            Optional(r'cpp', default=dict): {object: object},
             Optional(r'namespace', default=''): And(
                 str,
                 Use(lambda x: x.strip(': \t\n\f\b\v').split('::')),
                 Use(lambda x: [s.strip(': \t\n\f\b\v') for s in x]),
                 Use(lambda x: '::'.join(x).replace('::::', '::')),
             ),
-            Optional(r'structs', default=dict): {Stripped(str, allow_empty=False, name=r'struct name'): {object: object}},
+            Optional(r'structs', default=dict): {
+                Stripped(str, allow_empty=False, name=r'struct name'): {object: object}
+            },
             Optional(r'allocator', default=r'soagen::allocator'): Stripped(str),
             Optional(r'all_structs', default=dict): {object: object},
         }
     )
 
     def __init__(self, path):
         assert isinstance(path, Path)
```

### Comparing `soagen-0.1.0/src/soagen/configurable.py` & `soagen-0.1.1/src/soagen/configurable.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.0/src/soagen/cpp.py` & `soagen-0.1.1/src/soagen/cpp.py`

 * *Files 1% similar despite different names*

```diff
@@ -840,27 +840,29 @@
     r'zerofill',
     # other
     r'soagen',
     r'std',
 )
 RESERVED_SOAGEN = set(RESERVED_SOAGEN)
 
-VALID_IDENTIFIER = re.compile(r'[A-Za-z][A-Za-z_0-9]*')
+VALID_IDENTIFIER = re.compile(r'^[A-Za-z][A-Za-z_0-9]*$')
 
 
 def is_valid_identifier(s: str) -> tuple[bool, str]:
     if not s:
-        return (False, 'identifiers may not be blank')
+        return (False, 'may not be blank')
     if s.startswith('_'):
-        return (False, 'identifiers may not begin with an underscore')
+        return (False, 'may not begin with an underscore')
     if s.find('__') != -1:
-        return (False, 'identifiers may not contain double-underscores')
+        return (False, 'may not contain double-underscores')
+    if re.fullmatch(r'^[0-9].*$', s):
+        return (False, 'may not begin with a digit')
     if not VALID_IDENTIFIER.fullmatch(s):
-        return (False, 'identifiers must satisfy the regular expression [A-Za-z][A-Za-z_0-9]*')
+        return (False, 'may contain only a-z, A-Z, 0-9, and underscores')
     if s in RESERVED_CPP_KEYWORDS:
-        return (False, 'identifiers may not be C++ keywords')
+        return (False, 'may not be a C++ keyword')
     if s in RESERVED_SOAGEN:
         return (False, 'reserved by soagen')
     return (True,)
 
 
 __all__ = [r'detect_includes', r'remove_implicit_includes', r'is_valid_identifier']
```

### Comparing `soagen-0.1.0/src/soagen/errors.py` & `soagen-0.1.1/src/soagen/errors.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.0/src/soagen/header_file.py` & `soagen-0.1.1/src/soagen/header_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,61 +2,59 @@
 # This file is a part of marzer/soagen and is subject to the the terms of the MIT license.
 # Copyright (c) Mark Gillard <mark.gillard@outlook.com.au>
 # See https://github.com/marzer/soagen/blob/master/LICENSE for the full license text.
 # SPDX-License-Identifier: MIT
 
 import re
 
-from . import cpp, utils
+from . import utils
 from .column import *
 from .configurable import Configurable
+from .includes import *
 from .metavars import *
-from .schemas import And, Optional, Schema, Stripped, Use, ValueOrArray
+from .schemas import *
 from .version import *
 from .writer import *
 
 
 class HeaderFile(Configurable):
     __schema = Schema(
         {
             Optional(r'banner', default=''): Stripped(str),
-            Optional(r'prologue', default=''): Stripped(str),
-            Optional(r'header', default=''): Stripped(str),
-            Optional(r'footer', default=''): Stripped(str),
-            Optional(r'internal_includes', default=list): And(
-                ValueOrArray(str, name=r'internal_includes'),
-                Use(lambda x: cpp.remove_implicit_includes(sorted(set([s.strip() for s in x if s])))),
-            ),
-            Optional(r'external_includes', default=list): And(
-                ValueOrArray(str, name=r'external_includes'),
-                Use(lambda x: cpp.remove_implicit_includes(sorted(set([s.strip() for s in x if s])))),
-            ),
             Optional(r'brief', default=''): Stripped(str),
+            Optional(r'footer', default=''): Stripped(str),
+            Optional(r'header', default=''): Stripped(str),
+            Optional(r'includes', default=dict): {object: object},
+            Optional(r'prologue', default=''): Stripped(str),
         }
     )
 
     def __init__(self, config, structs, vals, path=''):
         super().__init__(config)
         self.path = path
         if not self.path:
             self.path = self.config.path.with_suffix('.hpp')
         self.__dict__.update(HeaderFile.__schema.validate(vals))
 
         self.structs = structs if utils.is_collection(structs) else [structs]
 
-        # add any includes requested by member structs
-        self.internal_includes = set(self.internal_includes)
-        self.external_includes = set(self.external_includes)
-        for struct in self.structs:
-            for h in struct.internal_includes:
-                self.internal_includes.add(h)
-            for h in struct.external_includes:
-                self.external_includes.add(h)
-        self.internal_includes = sorted(self.internal_includes)
-        self.external_includes = sorted(self.external_includes)
+        # includes
+        with SchemaContext('includes'):
+            self.includes = Includes(config, self.includes)
+
+            # add any includes requested by member structs
+            self.includes.internal = set(self.includes.internal)
+            self.includes.external = set(self.includes.external)
+            for struct in self.structs:
+                for h in struct.includes.internal:
+                    self.includes.internal.add(h)
+                for h in struct.includes.external:
+                    self.includes.external.add(h)
+            self.includes.internal = sorted(self.includes.internal)
+            self.includes.external = sorted(self.includes.external)
 
         # documentation
         if not self.brief and self.structs:
             self.brief = ', '.join([n.qualified_type for n in self.structs])
             self.brief = rf'Contains the definition{"s" if len(self.structs) > 1 else ""} of {self.brief}.'
 
         # banner
@@ -85,17 +83,17 @@
             /// @brief {self.brief}
             ///
             /// @note The code and documentation in this file were generated by soagen - https://marzer.github.io/soagen
             '''
             )
 
         # internal includes (#include "blah.h")
-        if self.internal_includes:
+        if self.includes.internal:
             o()
-            for inc in self.internal_includes:
+            for inc in self.includes.internal:
                 o(rf'#include "{inc}"')
 
         # stick the prologue here so users can use it to override the various
         # SOAGEN_ macros etc before including soagen.hpp
         o(
             rf'''
         {self.prologue}
```

### Comparing `soagen-0.1.0/src/soagen/hpp/.clang-format` & `soagen-0.1.1/src/soagen/hpp/.clang-format`

 * *Files identical despite different names*

### Comparing `soagen-0.1.0/src/soagen/hpp/allocator.hpp` & `soagen-0.1.1/src/soagen/hpp/allocator.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.1.0/src/soagen/hpp/column_traits.hpp` & `soagen-0.1.1/src/soagen/hpp/column_traits.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -733,46 +733,47 @@
 	/// @tparam	Align		The minimum memory alignment of the first element in the column.
 	///
 	///	@attention	This class is an implementation detail for the soagen-generated Structure-of-arrays classes.
 	///				You don't need to know anything about it unless you are implementing your own SoA machinery
 	///				without using the soagen generator.
 	template <typename ValueType,
 			  typename ParamType = soagen::param_type<ValueType>,
-			  size_t Align		 = alignof(ValueType)
-				  SOAGEN_HIDDEN_PARAM(typename Base = detail::column_traits_base<storage_type<ValueType>>)>
+			  size_t Align		 = alignof(ValueType)>
 	struct SOAGEN_EMPTY_BASES column_traits //
-		SOAGEN_HIDDEN_BASE(public Base)
+		SOAGEN_HIDDEN_BASE(public detail::column_traits_base<storage_type<ValueType>>)
 	{
 #if SOAGEN_DOXYGEN
 
 		/// @copydoc soagen::storage_type
 		using storage_type = POXY_IMPLEMENTATION_DETAIL(dummy);
+#else
 
+		using base_traits = detail::column_traits_base<storage_type<ValueType>>;
 #endif
 
 		/// @brief	The column's value type.
 		using value_type = ValueType;
 		static_assert(!std::is_reference_v<value_type>, "column value_type may not be a reference");
 		static_assert(!std::is_void_v<value_type>, "column value_type may not be void");
-		static_assert(alignof(value_type) == alignof(typename Base::storage_type));
-		static_assert(sizeof(value_type) == sizeof(typename Base::storage_type));
+		static_assert(alignof(value_type) == alignof(typename base_traits::storage_type));
+		static_assert(sizeof(value_type) == sizeof(typename base_traits::storage_type));
 
 		/// @brief	The type used for the column in lvalue function parameter contexts (e.g. `push_back(const &)`).
 		using param_type = ParamType;
 		static_assert(!std::is_void_v<param_type>, "column param_type may not be void");
 		static_assert(std::is_reference_v<param_type> || !is_cv<param_type>,
 					  "value parameters may not be cv-qualified");
-		static_assert(Base::template is_constructible<param_type>);
+		static_assert(base_traits::template is_constructible<param_type>);
 
 		/// @brief	The type used when forwarding #param_type to the backing container (e.g. `table.emplace_back()`)
 		using param_forward_type = forward_type<param_type>;
 
 		/// @brief	The type used for the column in rvalue function parameter contexts (e.g. `push_back(&&)`).
 		using rvalue_type = soagen::rvalue_type<param_type>;
-		static_assert(Base::template is_constructible<rvalue_type>);
+		static_assert(base_traits::template is_constructible<rvalue_type>);
 
 		/// @brief	The type used when forwarding #rvalue_type to the backing container (e.g. `table.emplace_back()`)
 		using rvalue_forward_type = forward_type<rvalue_type>;
 
 		/// @brief	The default type for `emplace()` and `emplace_back()` for columns that have a `default` value.
 		using default_emplace_type = make_cref<rvalue_type>;
 
@@ -794,18 +795,18 @@
 		static constexpr size_t aligned_stride = lcm(alignment, sizeof(value_type)) / sizeof(value_type);
 	};
 
 	/// @brief True if `T` is an instance of #soagen::column_traits.
 	template <typename T>
 	inline constexpr bool is_column_traits = POXY_IMPLEMENTATION_DETAIL(false);
 	/// @cond
+	template <typename ValueType, typename ParamType, size_t Align>
+	inline constexpr bool is_column_traits<column_traits<ValueType, ParamType, Align>> = true;
 	template <typename StorageType>
 	inline constexpr bool is_column_traits<detail::column_traits_base<StorageType>> = true;
-	template <typename ValueType, typename ParamType, size_t Align, typename Base>
-	inline constexpr bool is_column_traits<column_traits<ValueType, ParamType, Align, Base>> = is_column_traits<Base>;
 	template <typename T>
 	inline constexpr bool is_column_traits<const T> = is_column_traits<T>;
 	template <typename T>
 	inline constexpr bool is_column_traits<volatile T> = is_column_traits<T>;
 	template <typename T>
 	inline constexpr bool is_column_traits<const volatile T> = is_column_traits<T>;
 	/// @endcond
```

### Comparing `soagen-0.1.0/src/soagen/hpp/generated/compressed_pair.hpp` & `soagen-0.1.1/src/soagen/hpp/generated/compressed_pair.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.1.0/src/soagen/hpp/generated/core.hpp` & `soagen-0.1.1/src/soagen/hpp/generated/core.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.1.0/src/soagen/hpp/generated/functions.hpp` & `soagen-0.1.1/src/soagen/hpp/generated/functions.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.1.0/src/soagen/hpp/generated/preprocessor.hpp` & `soagen-0.1.1/src/soagen/hpp/generated/preprocessor.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.1.0/src/soagen/hpp/header_end.hpp` & `soagen-0.1.1/src/soagen/hpp/header_end.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.1.0/src/soagen/hpp/header_start.hpp` & `soagen-0.1.1/src/soagen/hpp/header_start.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.1.0/src/soagen/hpp/iterator.hpp` & `soagen-0.1.1/src/soagen/hpp/iterator.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.1.0/src/soagen/hpp/meta.hpp` & `soagen-0.1.1/src/soagen/hpp/meta.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -165,24 +165,22 @@
 
 	template <typename T, size_t Align = alignof(T)>
 	using const_column_span = column_span<std::add_const_t<T>, Align>;
 
 #endif
 
 #if SOAGEN_DOXYGEN
-	//# {{
 	/// @brief The optional type used by the library.
 	/// @note This can be overridden by redefining `SOAGEN_OPTIONAL_TYPE`, e.g.: @cpp
 	///
 	///	#define SOAGEN_OPTIONAL_TYPE tl::optional
 	///
 	///	@ecpp
 	template <typename T>
 	using optional = std::optional<T>;
-	//# }}
 #else
 	using SOAGEN_OPTIONAL_TYPE;
 #endif
 
 	/// @cond
 	namespace detail
 	{
```

### Comparing `soagen-0.1.0/src/soagen/hpp/mixins.hpp` & `soagen-0.1.1/src/soagen/hpp/mixins.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.1.0/src/soagen/hpp/row.hpp` & `soagen-0.1.1/src/soagen/hpp/row.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.1.0/src/soagen/hpp/single/soagen.hpp` & `soagen-0.1.1/src/soagen/hpp/single/soagen.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 //----------------------------------------------------------------------------------------------------------------------
 //
-// soagen.hpp v0.1.0
+// soagen.hpp v0.1.1
 // https://github.com/marzer/soagen
 // SPDX-License-Identifier: MIT
 //
 //----------------------------------------------------------------------------------------------------------------------
 //     !!!!! THIS FILE WAS ASSEMBLED FROM MULTIPLE HEADER FILES BY A SCRIPT - PLEASE DON'T EDIT IT DIRECTLY !!!!!
 //----------------------------------------------------------------------------------------------------------------------
 //
@@ -29,16 +29,16 @@
 #ifndef SOAGEN_HPP
 #define SOAGEN_HPP
 
 //********  generated/version.hpp  *************************************************************************************
 
 #define SOAGEN_VERSION_MAJOR  0
 #define SOAGEN_VERSION_MINOR  1
-#define SOAGEN_VERSION_PATCH  0
-#define SOAGEN_VERSION_STRING "0.1.0"
+#define SOAGEN_VERSION_PATCH  1
+#define SOAGEN_VERSION_STRING "0.1.1"
 
 //********  generated/preprocessor.hpp  ********************************************************************************
 
 #ifndef SOAGEN_CPP
 	#ifdef _MSVC_LANG
 		#if _MSVC_LANG > __cplusplus
 			#define SOAGEN_CPP _MSVC_LANG
@@ -1309,18 +1309,15 @@
 	#endif
 
 	template <typename T, size_t Align = alignof(T)>
 	using const_column_span = column_span<std::add_const_t<T>, Align>;
 
 #endif
 
-#if SOAGEN_DOXYGEN
-#else
 	using SOAGEN_OPTIONAL_TYPE;
-#endif
 
 	namespace detail
 	{
 		template <typename T>
 		using has_swap_member_ = decltype(std::declval<T&>().swap(std::declval<T&>()));
 
 		template <typename T, typename Arg>
@@ -2078,18 +2075,15 @@
 		SOAGEN_NODISCARD_CTOR
 		compressed_pair(compressed_pair&&) = default;
 
 		compressed_pair& operator=(const compressed_pair&) = default;
 
 		compressed_pair& operator=(compressed_pair&&) = default;
 
-#if SOAGEN_DOXYGEN
-#else
 		using detail::compressed_pair_base<First, Second>::compressed_pair_base; // inherit constructor
-#endif
 
 	  private:
 		template <size_t I, typename T>
 		SOAGEN_PURE_INLINE_GETTER
 		static constexpr decltype(auto) do_get(T&& cp) noexcept
 		{
 			static_assert(I <= 1);
@@ -3458,58 +3452,53 @@
 	};
 }
 
 namespace soagen
 {
 	template <typename ValueType,
 			  typename ParamType = soagen::param_type<ValueType>,
-			  size_t Align		 = alignof(ValueType)
-				  SOAGEN_HIDDEN_PARAM(typename Base = detail::column_traits_base<storage_type<ValueType>>)>
+			  size_t Align		 = alignof(ValueType)>
 	struct SOAGEN_EMPTY_BASES column_traits //
-		SOAGEN_HIDDEN_BASE(public Base)
+		SOAGEN_HIDDEN_BASE(public detail::column_traits_base<storage_type<ValueType>>)
 	{
-#if SOAGEN_DOXYGEN
-
-		using storage_type = POXY_IMPLEMENTATION_DETAIL(dummy);
-
-#endif
+		using base_traits = detail::column_traits_base<storage_type<ValueType>>;
 
 		using value_type = ValueType;
 		static_assert(!std::is_reference_v<value_type>, "column value_type may not be a reference");
 		static_assert(!std::is_void_v<value_type>, "column value_type may not be void");
-		static_assert(alignof(value_type) == alignof(typename Base::storage_type));
-		static_assert(sizeof(value_type) == sizeof(typename Base::storage_type));
+		static_assert(alignof(value_type) == alignof(typename base_traits::storage_type));
+		static_assert(sizeof(value_type) == sizeof(typename base_traits::storage_type));
 
 		using param_type = ParamType;
 		static_assert(!std::is_void_v<param_type>, "column param_type may not be void");
 		static_assert(std::is_reference_v<param_type> || !is_cv<param_type>,
 					  "value parameters may not be cv-qualified");
-		static_assert(Base::template is_constructible<param_type>);
+		static_assert(base_traits::template is_constructible<param_type>);
 
 		using param_forward_type = forward_type<param_type>;
 
 		using rvalue_type = soagen::rvalue_type<param_type>;
-		static_assert(Base::template is_constructible<rvalue_type>);
+		static_assert(base_traits::template is_constructible<rvalue_type>);
 
 		using rvalue_forward_type = forward_type<rvalue_type>;
 
 		using default_emplace_type = make_cref<rvalue_type>;
 
 		static constexpr size_t alignment = max(Align, alignof(value_type));
 		static_assert(has_single_bit(alignment), "column alignment must be a power of two");
 
 		static constexpr size_t aligned_stride = lcm(alignment, sizeof(value_type)) / sizeof(value_type);
 	};
 
 	template <typename T>
 	inline constexpr bool is_column_traits = POXY_IMPLEMENTATION_DETAIL(false);
+	template <typename ValueType, typename ParamType, size_t Align>
+	inline constexpr bool is_column_traits<column_traits<ValueType, ParamType, Align>> = true;
 	template <typename StorageType>
 	inline constexpr bool is_column_traits<detail::column_traits_base<StorageType>> = true;
-	template <typename ValueType, typename ParamType, size_t Align, typename Base>
-	inline constexpr bool is_column_traits<column_traits<ValueType, ParamType, Align, Base>> = is_column_traits<Base>;
 	template <typename T>
 	inline constexpr bool is_column_traits<const T> = is_column_traits<T>;
 	template <typename T>
 	inline constexpr bool is_column_traits<volatile T> = is_column_traits<T>;
 	template <typename T>
 	inline constexpr bool is_column_traits<const volatile T> = is_column_traits<T>;
 }
@@ -6177,25 +6166,15 @@
 		SOAGEN_NODISCARD_CTOR
 		table(const table&) = default;
 
 		table& operator=(const table&) = default;
 
 		~table() = default;
 
-#if !SOAGEN_DOXYGEN
 		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
-#endif
-
-#if SOAGEN_DOXYGEN
-
-		constexpr std::byte* data() noexcept;
-
-		constexpr const std::byte* data() const noexcept;
-
-#endif
 
 		template <size_t Column>
 		SOAGEN_ALIGNED_COLUMN(Column)
 		column_type<Column>* column() noexcept
 		{
 			static_assert(Column < table_traits::column_count, "column index out of range");
```

### Comparing `soagen-0.1.0/src/soagen/hpp/soagen.hpp` & `soagen-0.1.1/src/soagen/hpp/soagen.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.1.0/src/soagen/hpp/table.hpp` & `soagen-0.1.1/src/soagen/hpp/table.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1439,16 +1439,14 @@
 
 		/// @brief Destructor.
 		~table() = default;
 
 #if !SOAGEN_DOXYGEN
 		using SOAGEN_BASE_TYPE::SOAGEN_BASE_NAME;
 #else
-		//# {{
-
 		/// @brief Constructs with the given allocator.
 		constexpr explicit table(const allocator_type& alloc) noexcept;
 
 		/// @brief Constructs with the given allocator.
 		constexpr explicit table(allocator_type&& alloc) noexcept;
 
 		/// @name Capacity
@@ -1460,14 +1458,17 @@
 		/// @brief Returns the current number of rows.
 		constexpr size_type size() const noexcept;
 
 		/// @brief Returns the maximum possible number of rows.
 		constexpr size_type max_size() const noexcept;
 
 		/// @brief Returns the size of the current underlying buffer allocation in bytes.
+		/// @warning This value is `capacity() * (sizeof() for every column) + (alignment padding)`.
+		///          It is **not** based on `size()`! If you are using the value returned by this function
+		///          in conjunction with `data()` to do serialization, hashing, etc, use `shrink_to_fit()` first.
 		constexpr size_t allocation_size() const noexcept;
 
 		/// @brief Reserves storage for (at least) the given number of rows.
 		void reserve(size_type new_cap) noexcept(...);
 
 		/// @brief Returns the number of rows that can be held in currently allocated storage.
 		constexpr size_type capacity() const noexcept;
@@ -1554,32 +1555,29 @@
 		friend constexpr bool operator>=(const table& lhs, const table& rhs) noexcept(...);
 
 		/// @}
 
 		/// @brief Returns the allocator being used by the table.
 		constexpr allocator_type get_allocator() const noexcept;
 
-		//# }}
 #endif
 
 		/// @name Column access
 		/// @{
 
 #if SOAGEN_DOXYGEN
-
 		/// @brief Returns a pointer to the raw byte backing array.
 		///
 		/// @availability This method is only available when all the column types are trivially-copyable.
 		constexpr std::byte* data() noexcept;
 
 		/// @brief Returns a const pointer to the raw byte backing array.
 		///
 		/// @availability This method is only available when all the column types are trivially-copyable.
 		constexpr const std::byte* data() const noexcept;
-
 #endif
 
 		/// @brief Returns a pointer to the elements of a specific column.
 		template <size_t Column>
 		SOAGEN_ALIGNED_COLUMN(Column)
 		column_type<Column>* column() noexcept
 		{
```

### Comparing `soagen-0.1.0/src/soagen/hpp/table_traits.hpp` & `soagen-0.1.1/src/soagen/hpp/table_traits.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.1.0/src/soagen/injectors.py` & `soagen-0.1.1/src/soagen/injectors.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.0/src/soagen/log.py` & `soagen-0.1.1/src/soagen/log.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.0/src/soagen/main.py` & `soagen-0.1.1/src/soagen/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,36 +99,64 @@
 
     log.i(
         f'{log.STYLE_CYAN}Zip generated: {bug_report_zip}\n'
         f'Please attach this file when you make a report at github.com/marzer/soagen/issues, thanks!{log.STYLE_RESET}'
     )
 
 
-def update(new_version: tuple = None):
+def update(
+    new_version: tuple = None,
+    update_templated_hpps=True,
+    update_soagen_hpp=True,
+    update_examples=True,
+    update_tests=True,
+    update_documentation=True,
+):
     # set the version number
     if new_version is not None:
         assert isinstance(new_version, tuple)
         assert len(new_version) == 3
         for val in new_version:
             assert isinstance(val, int) and val >= 0
         global VERSION
         global VERSION_STRING
         if VERSION != new_version:
             new_version_str = rf'{new_version[0]}.{new_version[1]}.{new_version[2]}'
             log.i(rf'Changing version number: v{VERSION_STRING} -> v{new_version_str}')
             matcher = re.compile(rf'\b({VERSION[0]})[.]({VERSION[1]})[.]({VERSION[2]})\b')
             matcher_v = re.compile(rf'\b([vV])({VERSION[0]})[.]({VERSION[1]})[.]({VERSION[2]})\b')
+
             # update version
             VERSION = new_version
             VERSION_STRING = new_version_str
             assert VERSION == new_version
             assert VERSION_STRING == new_version_str
             log.i(rf'Writing {paths.VERSION_TXT}')
             with open(paths.VERSION_TXT, 'w', encoding='utf-8', newline='\n') as f:
                 print(new_version_str, file=f)
+
+            # regenerate version.hpp
+            version_hpp = paths.HPP_GENERATED / r'version.hpp'
+            log.i(rf'Writing {version_hpp}')
+            with open(version_hpp, 'w', encoding='utf-8', newline='\n') as f:
+                f.write(
+                    rf'''
+//# This file is a part of marzer/soagen and is subject to the the terms of the MIT license.
+//# Copyright (c) Mark Gillard <mark.gillard@outlook.com.au>
+//# See https://github.com/marzer/soagen/blob/master/LICENSE for the full license text.
+//# SPDX-License-Identifier: MIT
+#pragma once
+
+#define SOAGEN_VERSION_MAJOR {VERSION[0]}
+#define SOAGEN_VERSION_MINOR {VERSION[1]}
+#define SOAGEN_VERSION_PATCH {VERSION[2]}
+#define SOAGEN_VERSION_STRING "{VERSION_STRING}"
+'''.lstrip()
+                )
+
             # update version in all the other files
             DIRS = (
                 (paths.REPOSITORY, False),
                 (paths.DOCS, True),
                 (paths.EXAMPLES, True),
                 (paths.SRC, True),
                 (paths.TESTS, True),
@@ -146,107 +174,92 @@
                         r'*.dox',
                         r'*.toml',
                         r'*.natvis',
                         r'meson.build',
                     ),
                     recursive=recursive,
                 ):
-                    if str(file).find('.egg-info') != -1:
+                    if str(file).find('.egg-info') != -1 or file.name.lower.find('changelog') != -1:
                         continue
                     text = utils.read_all_text_from_file(file, logger=log.d)
                     new_text = matcher.sub(VERSION_STRING, text)
                     new_text = matcher_v.sub(lambda m: m[1] + VERSION_STRING, new_text)
                     if text != new_text:
                         log.i(rf'Writing updated version numbers in {file}')
                         with open(file, 'w', encoding='utf-8', newline='\n') as f:
                             f.write(new_text)
-    # regenerate version.hpp
-    version_hpp = paths.HPP_GENERATED / r'version.hpp'
-    log.i(rf'Writing {version_hpp}')
-    with open(version_hpp, 'w', encoding='utf-8', newline='\n') as f:
-        f.write(
-            rf'''
-//# This file is a part of marzer/soagen and is subject to the the terms of the MIT license.
-//# Copyright (c) Mark Gillard <mark.gillard@outlook.com.au>
-//# See https://github.com/marzer/soagen/blob/master/LICENSE for the full license text.
-//# SPDX-License-Identifier: MIT
-#pragma once
 
-#define SOAGEN_VERSION_MAJOR {VERSION[0]}
-#define SOAGEN_VERSION_MINOR {VERSION[1]}
-#define SOAGEN_VERSION_PATCH {VERSION[2]}
-#define SOAGEN_VERSION_STRING "{VERSION_STRING}"
-'''
-        )
+    # copy .clang-format
+    if update_templated_hpps or update_soagen_hpp or update_tests or update_examples:
+        utils.copy_file(Path(paths.REPOSITORY, r'.clang-format'), paths.HPP, logger=log.i)
 
     # regenerate the generated headers from their templates
-    if paths.MAKE_SINGLE.exists():
-        for template in utils.enumerate_files(paths.HPP_TEMPLATES, all='*.hpp.in', recursive=True):
-            output = Path(paths.HPP_GENERATED, template.stem)
-            os.makedirs(str(paths.HPP_GENERATED), exist_ok=True)
-            utils.run_python_script(
-                *(
-                    [
-                        paths.MAKE_SINGLE,
-                        str(template),
-                        r'--output',
-                        output,
-                        r'--namespaces',
-                        r'soagen',
-                        r'detail',
-                        r'--macros',
-                        r'SOAGEN',
-                    ]
-                    + ([r'--no-strip-hidden-bases'] if template.name not in (r'compressed_pair.hpp.in',) else [])
-                    + (
-                        [r'--no-strip-doxygen-from-snippets']
-                        if template.name not in (r'compressed_pair.hpp.in', r'preprocessor.hpp.in')
-                        else []
+    if update_templated_hpps:
+        if paths.MAKE_SINGLE.exists():
+            for template in utils.enumerate_files(paths.HPP_TEMPLATES, all='*.hpp.in', recursive=True):
+                output = Path(paths.HPP_GENERATED, template.stem)
+                os.makedirs(str(paths.HPP_GENERATED), exist_ok=True)
+                utils.run_python_script(
+                    *(
+                        [
+                            paths.MAKE_SINGLE,
+                            str(template),
+                            r'--output',
+                            output,
+                            r'--namespaces',
+                            r'soagen',
+                            r'detail',
+                            r'--macros',
+                            r'SOAGEN',
+                        ]
+                        + ([r'--no-strip-hidden-bases'] if template.name not in (r'compressed_pair.hpp.in',) else [])
+                        + (
+                            [r'--no-strip-doxygen-from-snippets']
+                            if template.name not in (r'compressed_pair.hpp.in', r'preprocessor.hpp.in')
+                            else []
+                        )
                     )
                 )
-            )
-            text = utils.read_all_text_from_file(output, logger=log.i)
-            try:
-                text = utils.clang_format(text, cwd=output.parent)
-            except:
-                pass
-            log.i(rf'Writing {output}')
-            with open(output, 'w', encoding='utf-8', newline='\n') as f:
-                f.write(text)
-    else:
-        log.w(rf'could not regenerate headers using muu: {paths.MAKE_SINGLE.name} did not exist or was not a file')
+                text = utils.read_all_text_from_file(output, logger=log.i)
+                try:
+                    text = utils.clang_format(text, cwd=output.parent)
+                except:
+                    pass
+                log.i(rf'Writing {output}')
+                with open(output, 'w', encoding='utf-8', newline='\n') as f:
+                    f.write(text)
+        else:
+            log.w(rf'could not regenerate headers using muu: {paths.MAKE_SINGLE.name} did not exist or was not a file')
 
     # read soagen.hpp + preprocess into single header
-    soagen_hpp_in = Path(paths.HPP, 'soagen.hpp')
-    soagen_hpp_out = Path(paths.HPP_SINGLE, 'soagen.hpp')
-    text = str(Preprocessor(soagen_hpp_in))
-    text = utils.replace_metavar(r'version', VERSION_STRING, text)
-    license = utils.read_all_text_from_file(paths.REPOSITORY / r'LICENSE.txt', log.i).replace('\r\n', '\n').strip()
-    license = '\n// '.join(utils.reflow_text(license, line_length=117).split('\n'))
-    text = utils.replace_metavar(r'license', license, text)
-    try:
-        text = utils.clang_format(text, cwd=soagen_hpp_in.parent)
-    except:
-        pass
-    log.i(rf'Writing {soagen_hpp_out}')
-    os.makedirs(str(paths.HPP_SINGLE), exist_ok=True)
-    with open(soagen_hpp_out, 'w', encoding='utf-8', newline='\n') as f:
-        f.write(text)
+    if update_soagen_hpp:
+        soagen_hpp_in = Path(paths.HPP, 'soagen.hpp')
+        soagen_hpp_out = Path(paths.HPP_SINGLE, 'soagen.hpp')
+        text = str(Preprocessor(soagen_hpp_in))
+        text = utils.replace_metavar(r'version', VERSION_STRING, text)
+        license = utils.read_all_text_from_file(paths.REPOSITORY / r'LICENSE.txt', log.i).replace('\r\n', '\n').strip()
+        license = '\n// '.join(utils.reflow_text(license, line_length=117).split('\n'))
+        text = utils.replace_metavar(r'license', license, text)
+        try:
+            text = utils.clang_format(text, cwd=soagen_hpp_in.parent)
+        except:
+            pass
+        log.i(rf'Writing {soagen_hpp_out}')
+        os.makedirs(str(paths.HPP_SINGLE), exist_ok=True)
+        with open(soagen_hpp_out, 'w', encoding='utf-8', newline='\n') as f:
+            f.write(text)
 
     # re-run soagen itself on the examples and tests
-    if paths.EXAMPLES.exists():
+    if update_examples and paths.EXAMPLES.exists():
         launch_worker(r'*.toml', r'--doxygen', cwd=paths.EXAMPLES)
-    if paths.TESTS.exists():
+    if update_tests and paths.TESTS.exists():
         launch_worker(r'*.toml', r'--no-doxygen', cwd=paths.TESTS)
 
-    # copy .clang-format
-    utils.copy_file(Path(paths.REPOSITORY, r'.clang-format'), paths.HPP, logger=log.i)
-
     # invoke poxy on the documentation
-    if utils.is_tool(r'poxy') and paths.DOCS.is_dir():
+    if update_documentation and utils.is_tool(r'poxy') and paths.DOCS.is_dir():
         subprocess.run(args=[r'poxy'], cwd=str(paths.DOCS), encoding=r'utf-8')
 
 
 class NonExitingArgParser(argparse.ArgumentParser):
     def error(self, message):
         self.print_usage(sys.stderr)
         raise Error(message)
@@ -327,14 +340,16 @@
     )  #
 
     # --------------------------------------------------------------
     # hidden/developer-only/deprecated/diagnostic arguments
     # --------------------------------------------------------------
     args.add_argument(r'--where', action=r'store_true', help=argparse.SUPPRESS)
     args.add_argument(r'--update', nargs='?', const=True, default=False, help=argparse.SUPPRESS)
+    args.add_argument(r'--update-hpp', action=r'store_true', help=argparse.SUPPRESS)
+    args.add_argument(r'--update-docs', action=r'store_true', help=argparse.SUPPRESS)
     args.add_argument(r'--bug-report-internal', action=r'store_true', help=argparse.SUPPRESS)
     args.add_argument(
         r'--colour', action=argparse.BooleanOptionalAction, default=None, dest='color', help=argparse.SUPPRESS
     )
     args.add_argument(r'--worker', action=r'store_true', help=argparse.SUPPRESS)
 
     usage_str = args.format_usage()
@@ -393,14 +408,23 @@
             args.update = args.update.strip()
             if args.update:
                 m = re.fullmatch(r'\s*[vV]?\s*([0-9]+)\s*[.]+\s*([0-9]+)\s*[.]+\s*([0-9]+)\s*', args.update)
                 if m:
                     new_version = (int(m[1]), int(m[2]), int(m[3]))
         done_work = True
         update(new_version)
+    elif args.update_hpp or args.update_docs:
+        done_work = True
+        update(
+            update_templated_hpps=False,
+            update_soagen_hpp=args.update_hpp,
+            update_examples=False,
+            update_tests=False,
+            update_documentation=args.update_docs,
+        )
 
     if args.install is not None:
         done_work = True
         args.install: Path
         if not args.install.exists() or not args.install.is_dir():
             log.e(rf"--install: path '{args.install}' did not exist or was not a directory")
         log.i(rf"Copying soagen.hpp to {args.install.resolve()}")
@@ -430,15 +454,15 @@
 
         for config in configs:
             for src in (config.hpp,):
 
                 def on_flush(o: Writer, s: str) -> str:
                     nonlocal src
                     # sub in external headers
-                    includes = sorted(set(src.external_includes + cpp.detect_includes(s)))
+                    includes = sorted(set(src.includes.external + cpp.detect_includes(s)))
                     includes = cpp.remove_implicit_includes(includes)
                     PATTERN = r'\n[ \t]*//[ \t]*####[ \t]+SOAGEN_EXTERNAL_HEADERS[ \t]+####[ \t]*\n'
                     rep = '\nSOAGEN_DISABLE_WARNINGS;'
                     for inc in includes:
                         rep += f'\n#include <{inc}>'
                     rep += '\n#if SOAGEN_HAS_EXCEPTIONS\n\t#include <stdexcept>\n#endif'
                     rep += '\nSOAGEN_ENABLE_WARNINGS;\n'
```

### Comparing `soagen-0.1.0/src/soagen/metavars.py` & `soagen-0.1.1/src/soagen/metavars.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.0/src/soagen/natvis_file.py` & `soagen-0.1.1/src/soagen/natvis_file.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.0/src/soagen/paths.py` & `soagen-0.1.1/src/soagen/paths.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.0/src/soagen/preprocessor.py` & `soagen-0.1.1/src/soagen/preprocessor.py`

 * *Files 12% similar despite different names*

```diff
@@ -64,18 +64,28 @@
             s = re.sub('\n(?:[ \t]*\n[ \t]*)+\n', '\n\n', s)
             # weird spacing edge case around pp directives
             s = re.sub('\n[}]\n#', r'\n}\n\n#', s)
             # blank lines following opening brackets or a comma
             s = re.sub(r'([^@][({,])\n\n', r'\1\n', s)
             # blank lines preceeding closing brackets
             s = re.sub(r'\n\n([ \t]*[})])', r'\n\1', s)
-            # empty #if(n)def blocks
-            s = re.sub(r'#ifn?def[ \t]+[a-zA-Z0-9_]+[ \t]*\n\s*#endif', r'\n', s)
+            # empty #if blocks
+            s = re.sub(r'#if(n?def)?[ \t]+[a-zA-Z0-9_]+\s*?\n+\s*?#endif', r'\n', s)
             # empty #else blocks
-            s = re.sub(r'#else[ \t]*\n\s*#endif', r'#endif\n', s)
+            s = re.sub(r'#else\s*?\n+\s*?#endif', r'#endif\n', s)
+            # #if SOAGEN_DOXYGEN ... #else ... #endif
+            s = re.sub(r'#if[ \t]+SOAGEN_DOXYGEN\s*?(?:\n+[^#]*?)?\n+\s*?#else\s*?\n+([^#]*?)\n+\s*?#endif', r'\1\n', s)
+            # #if !SOAGEN_DOXYGEN ... #else ... #endif
+            s = re.sub(
+                r'#if[ \t]+![ \t]*SOAGEN_DOXYGEN\s*?\n+([^#]*?)\n+\s*?#else\s*?(?:\n+[^#]*?)?\n+\s*?#endif', r'\1\n', s
+            )
+            # #if SOAGEN_DOXYGEN ... #endif
+            s = re.sub(r'#if[ \t]+SOAGEN_DOXYGEN\s*?(?:\n+[^#]*?)?\n+\s*?#endif', r'\n', s)
+            # #if !SOAGEN_DOXYGEN ... #endif
+            s = re.sub(r'#if[ \t]+![ \t]*SOAGEN_DOXYGEN\s*?\n+([^#]*?)\n+\s*?#endif', r'\1\n', s)
             if s == self.__string:
                 break
             self.__string = s
         self.__string = self.__string.strip() + '\n'
 
     def __preprocess(self, incl):
         if not isinstance(incl, (Path, str)):  # a regex match object
```

### Comparing `soagen-0.1.0/src/soagen/schemas.py` & `soagen-0.1.1/src/soagen/schemas.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.0/src/soagen/struct.py` & `soagen-0.1.1/src/soagen/struct.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,61 +1,50 @@
 #!/usr/bin/env python3
 # This file is a part of marzer/soagen and is subject to the the terms of the MIT license.
 # Copyright (c) Mark Gillard <mark.gillard@outlook.com.au>
 # See https://github.com/marzer/soagen/blob/master/LICENSE for the full license text.
 # SPDX-License-Identifier: MIT
 
-import math
 from io import StringIO
 
 from . import cpp, log, utils
 from .column import *
 from .configurable import *
+from .includes import *
 from .metavars import *
 from .schemas import *
 from .type_list import *
 from .variable import *
 from .writer import *
 
 NEWLINE = '\n'
 TAB = '\t'
 TAB_SPACES = '    '
 
 
 class Struct(Configurable):
     __schema = Schema(
         {
-            Optional(r'prologue', default=''): Stripped(str),
-            Optional(r'header', default=''): Stripped(str),
-            Optional(r'footer', default=''): Stripped(str),
-            Optional(r'epilogue', default=''): Stripped(str),
-            Optional(r'brief', default=''): Stripped(str),
-            Optional(r'details', default=''): Stripped(str),
             Optional(r'allocator', default=''): Stripped(str),
-            Optional(r'static_variables', default=list): [object],
-            Optional(r'variables', default=list): [object],
-            Optional(r'default_constructible', default=True): bool,
-            Optional(r'movable', default=True): bool,
+            Optional(r'brief', default=''): Stripped(str),
             Optional(r'copyable', default=True): bool,
-            Optional(r'swappable', default=True): bool,
+            Optional(r'default_constructible', default=True): bool,
+            Optional(r'details', default=''): Stripped(str),
+            Optional(r'epilogue', default=''): Stripped(str),
+            Optional(r'footer', default=''): Stripped(str),
+            Optional(r'header', default=''): Stripped(str),
+            Optional(r'includes', default=dict): {object: object},
             Optional(r'iterators', default=True): bool,
+            Optional(r'movable', default=True): bool,
+            Optional(r'prologue', default=''): Stripped(str),
             Optional(r'reverse_iterators', default=False): bool,
             Optional(r'rvalue_iterators', default=True): bool,
-            Optional(r'column_providers', default=True): bool,
-            Optional(r'stripes', default=list): [object],
-            Optional(r'spans', default=True): bool,
-            # additional #includes to add to any header files this struct appears in
-            Optional(r'internal_includes', default=list): And(
-                ValueOrArray(str, name=r'internal_includes'),
-                Use(lambda x: cpp.remove_implicit_includes(sorted(set([s.strip() for s in x if s])))),
-            ),
-            Optional(r'external_includes', default=list): And(
-                ValueOrArray(str, name=r'external_includes'),
-                Use(lambda x: cpp.remove_implicit_includes(sorted(set([s.strip() for s in x if s])))),
-            ),
+            Optional(r'static_variables', default=list): [object],
+            Optional(r'swappable', default=True): bool,
+            Optional(r'variables', default=list): [object],
         }
     )
 
     def __init__(self, cfg, name, vals):
         super().__init__(cfg)
 
         vals = Struct.__schema.validate(vals)
@@ -82,14 +71,17 @@
         self.meta.push(r'struct::scope', '')
 
         if not self.allocator:
             self.allocator = self.config.allocator
         if self.allocator == r'std::allocator':
             self.allocator = r'std::allocator<std::byte>'
 
+        with SchemaContext('includes'):
+            self.includes = Includes(cfg, self.includes)
+
         has_defaults = False
         for i in range(len(self.variables)):
             with SchemaContext(
                 rf"variable '{self.variables[i]['name']}'" if r'name' in self.variables[i] else rf"variable [{i}]"
             ):
                 v = Variable(self, self.variables[i])
                 self.variables[i] = v
@@ -100,21 +92,18 @@
                 self.meta.push(rf'{v.name}::default', v.default if v.default else '{}')
                 has_default = bool(v.default)
                 if not has_default and has_defaults:
                     log.w(rf'{current_schema_context()}has no default but previous variables do')
                 has_defaults = has_defaults or has_default
 
         self.columns = []
-        self.double_buffered = []
         index = 0
         for v in self.variables:
             v.index = index
             index += 1
-            if v.double_buffered:
-                self.double_buffered.append(v)
             self.columns += v.columns
 
         index = 0
         for c in self.columns:
             c.index = index
             index += 1
         self.column_indices = ", ".join([str(col.index) for col in self.columns])
@@ -528,15 +517,20 @@
                         {doxygen(r"@brief Returns the maximum possible number of rows.")}
                         SOAGEN_PURE_INLINE_GETTER
                         constexpr size_type max_size() const noexcept
                         {{
                             return table_.max_size();
                         }}
 
-                        {doxygen(r"@brief Returns the size of the current underlying buffer allocation in bytes.")}
+                        {doxygen(r"""
+                        @brief Returns the size of the current underlying buffer allocation in bytes.
+
+                        @warning This value is `capacity() * (sizeof() for every column) + (alignment padding)`.
+                                 It is **not** based on `size()`! If you are using the value returned by this function
+                                 in conjunction with `data()` to do serialization, hashing, etc, use `shrink_to_fit()` first.""")}
                         SOAGEN_PURE_INLINE_GETTER
                         constexpr size_type allocation_size() const noexcept
                         {{
                             return table_.allocation_size();
                         }}
 
                         {doxygen(r"@brief Reserves storage for (at least) the given number of rows.")}
```

### Comparing `soagen-0.1.0/src/soagen/type_list.py` & `soagen-0.1.1/src/soagen/type_list.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.0/src/soagen/utils.py` & `soagen-0.1.1/src/soagen/utils.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.0/src/soagen/variable.py` & `soagen-0.1.1/src/soagen/variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,16 @@
 from .writer import *
 
 
 class Variable(Configurable):
     __schema = Schema(
         {
             r'name': Stripped(str, allow_empty=False, name=r'variable name'),
-            r'type': Stripped(str, allow_empty=False, name='variable type'),
-            Optional(r'double_buffered', default=False): bool,
+            r'type': Stripped(str, allow_empty=False, name=r'variable type'),
             Optional(r'param_type', default=''): Stripped(str),
-            Optional(r'brief', default=''): Stripped(str),
             Optional(r'default', default=None): And(
                 Or(str, float, int), Use(lambda x: x.strip() if isinstance(x, str) else str(x))
             ),
             Optional(r'alignment', default=0): And(
                 Or(int, str),
                 Use(int),
                 lambda x: x <= 0 or utils.is_pow2(x),
@@ -51,16 +49,14 @@
         self.pointer_type = rf'{self.type}*'
         if re.fullmatch(r'[a-zA-Z_][a-zA-Z_0-9:]*', self.type):
             self.const_pointer_type = rf'const {self.pointer_type}'
         else:
             self.const_pointer_type = rf'std::add_const_t<{self.type}>*'
 
         self.columns = [Column(self)]
-        if self.double_buffered:
-            self.columns.append(Column(self, True))
 
 
 class StaticVariable(Configurable):
     __schema = Schema(
         {
             r'name': Stripped(str, allow_empty=False, name=r'static variable name'),
             r'type': Stripped(str, allow_empty=False, name=r'static variable type'),
```

### Comparing `soagen-0.1.0/src/soagen/version.py` & `soagen-0.1.1/src/soagen/version.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.0/src/soagen/writer.py` & `soagen-0.1.1/src/soagen/writer.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.0/src/soagen.egg-info/PKG-INFO` & `soagen-0.1.1/src/soagen.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soagen
-Version: 0.1.0
+Version: 0.1.1
 Summary: Struct-of-Arrays generator for C++ projects.
 Author-email: Mark Gillard <mark.gillard@outlook.com.au>
 License: MIT
 Project-URL: Source, https://github.com/marzer/soagen
 Project-URL: Tracker, https://github.com/marzer/soagen/issues
 Project-URL: Funding, https://github.com/sponsors/marzer
 Keywords: c++,soa,struct-of-arrays,structure-of-arrays,struct of arrays,structure of arrays,parallel-arrays,parallel arrays,std::vector
@@ -23,20 +23,24 @@
 
 [![Sponsor](docs/images/badge-sponsor.svg)][sponsor]
 [![Gitter](docs/images/badge-gitter.svg)][gitter]
 
 <br><br>
 
 <p align="center">
-	<strong>✨&#xFE0F; This README is as stub. Please see the HTML documentation: <a href="https://marzer.github.io/soagen/">marzer.github.io/soagen</a>✨&#xFE0F;</strong>
+	<strong>✨&#xFE0F; This README is a stub. Please see the HTML documentation: <a href="https://marzer.github.io/soagen/">marzer.github.io/soagen</a>✨&#xFE0F;</strong>
 </p>
 
 <br><br>
 
 [gitter]: https://gitter.im/marzer/community
 [sponsor]: https://github.com/sponsors/marzer
 
 # Changelog
 
+## v0.1.1
+
+-   Minor refactors.
+
 ## v0.1.0
 
 -   First public release 🎉&#xFE0F;
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: soagen Version: 0.1.0 Summary: Struct-of-Arrays
+Metadata-Version: 2.1 Name: soagen Version: 0.1.1 Summary: Struct-of-Arrays
 generator for C++ projects. Author-email: Mark Gillard
 gillard@outlook.com.au> License: MIT Project-URL: Source, https://github.com/
 marzer/soagen Project-URL: Tracker, https://github.com/marzer/soagen/issues
 Project-URL: Funding, https://github.com/sponsors/marzer Keywords:
 c++,soa,struct-of-arrays,structure-of-arrays,struct of arrays,structure of
 arrays,parallel-arrays,parallel arrays,std::vector Classifier: Development
 Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: C++ Classifier: Topic :: Software
 Development :: Code Generators Classifier: Topic :: Utilities Requires-Python:
 >=3.9 Description-Content-Type: text/markdown License-File: LICENSE.txt #
 soagen Struct-of-Arrays generator for C++ projects. [![Sponsor](docs/images/
 badge-sponsor.svg)][sponsor] [![Gitter](docs/images/badge-gitter.svg)][gitter]
 
-    â¨&#xFE0F; This README is as stub. Please see the HTML documentation:
+     â¨&#xFE0F; This README is a stub. Please see the HTML documentation:
                       marzer.github.io/soagenâ¨&#xFE0F;
 
 
 [gitter]: https://gitter.im/marzer/community [sponsor]: https://github.com/
-sponsors/marzer # Changelog ## v0.1.0 - First public release ð&#xFE0F;
+sponsors/marzer # Changelog ## v0.1.1 - Minor refactors. ## v0.1.0 - First
+public release ð&#xFE0F;
```

### Comparing `soagen-0.1.0/src/soagen.egg-info/SOURCES.txt` & `soagen-0.1.1/src/soagen.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 src/soagen/__init__.py
 src/soagen/column.py
 src/soagen/config.py
 src/soagen/configurable.py
 src/soagen/cpp.py
 src/soagen/errors.py
 src/soagen/header_file.py
+src/soagen/includes.py
 src/soagen/injectors.py
 src/soagen/log.py
 src/soagen/main.py
 src/soagen/metavars.py
 src/soagen/natvis_file.py
 src/soagen/paths.py
 src/soagen/preprocessor.py
```

