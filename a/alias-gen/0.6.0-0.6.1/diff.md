# Comparing `tmp/alias_gen-0.6.0.tar.gz` & `tmp/alias_gen-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alias_gen-0.6.0.tar", max compression
+gzip compressed data, was "alias_gen-0.6.1.tar", max compression
```

## Comparing `alias_gen-0.6.0.tar` & `alias_gen-0.6.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1083 2023-01-02 05:01:18.992694 alias_gen-0.6.0/LICENSE.md
--rw-r--r--   0        0        0     2941 2023-07-29 22:51:32.041985 alias_gen-0.6.0/README.md
--rw-r--r--   0        0        0     1717 2023-07-29 23:01:58.437729 alias_gen-0.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-02 18:23:40.999671 alias_gen-0.6.0/src/alias_gen/__init__.py
--rw-r--r--   0        0        0     8646 2023-07-29 21:28:32.797869 alias_gen-0.6.0/src/alias_gen/aliaser.py
--rw-r--r--   0        0        0     3673 2023-07-29 21:30:19.997976 alias_gen-0.6.0/src/alias_gen/arg_parser.py
--rw-r--r--   0        0        0      560 2023-07-29 19:55:02.527718 alias_gen-0.6.0/src/alias_gen/constants.py
--rw-r--r--   0        0        0     2077 2023-07-29 20:03:46.355423 alias_gen-0.6.0/src/alias_gen/file_utils.py
--rw-r--r--   0        0        0      293 2023-07-29 21:33:37.953491 alias_gen-0.6.0/src/alias_gen/logger.py
--rw-r--r--   0        0        0     3981 1970-01-01 00:00:00.000000 alias_gen-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-01-02 05:01:18.992694 alias_gen-0.6.1/LICENSE.md
+-rw-r--r--   0        0        0     2941 2023-07-29 22:51:32.041985 alias_gen-0.6.1/README.md
+-rw-r--r--   0        0        0     1717 2023-07-29 23:08:15.646974 alias_gen-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-02 18:23:40.999671 alias_gen-0.6.1/src/alias_gen/__init__.py
+-rw-r--r--   0        0        0     8646 2023-07-29 21:28:32.797869 alias_gen-0.6.1/src/alias_gen/aliaser.py
+-rw-r--r--   0        0        0     3642 2023-07-29 23:08:09.455356 alias_gen-0.6.1/src/alias_gen/arg_parser.py
+-rw-r--r--   0        0        0      560 2023-07-29 19:55:02.527718 alias_gen-0.6.1/src/alias_gen/constants.py
+-rw-r--r--   0        0        0     2077 2023-07-29 20:03:46.355423 alias_gen-0.6.1/src/alias_gen/file_utils.py
+-rw-r--r--   0        0        0      293 2023-07-29 21:33:37.953491 alias_gen-0.6.1/src/alias_gen/logger.py
+-rw-r--r--   0        0        0     3981 1970-01-01 00:00:00.000000 alias_gen-0.6.1/PKG-INFO
```

### Comparing `alias_gen-0.6.0/LICENSE.md` & `alias_gen-0.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `alias_gen-0.6.0/README.md` & `alias_gen-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `alias_gen-0.6.0/pyproject.toml` & `alias_gen-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="alias-gen"
-version="0.6.0"
+version="0.6.1"
 authors=[{name="Ariel Frischer", email="arielfrischer@gmail.com"}]
 description="Generate bash/zsh/fish shell aliases automatically."
 requires-python=">=3.6"
 readme = "README.md"
 classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -28,15 +28,15 @@
     "generate",
     "terminal",
 ]
 
 [tool.poetry]
 name = "alias-gen"
 license = "MIT"
-version = "0.6.0"
+version = "0.6.1"
 description = "Generate bash/zsh/fish shell aliases automatically."
 authors=["Ariel Frischer <arielfrischer@gmail.com>"]
 maintainers=["Ariel Frischer <arielfrischer@gmail.com>"]
 readme = "README.md"
 classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `alias_gen-0.6.0/src/alias_gen/aliaser.py` & `alias_gen-0.6.1/src/alias_gen/aliaser.py`

 * *Files identical despite different names*

### Comparing `alias_gen-0.6.0/src/alias_gen/arg_parser.py` & `alias_gen-0.6.1/src/alias_gen/arg_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,16 +44,14 @@
         "-d",
         "--debug",
         action="store_true",
         help="Enable debug output.",
     )
 
     parser.add_argument("-n", type=int, default=30, help="Total number of suggestions default is 30")
-    args = parser.parse_args()
-    init_logger(args)
     parser.add_argument(
         "-f",
         type=validate_file_exists,
         default="",
         help="Path to history file like ~/.zsh_history if it is not default.",
     )
     parser.add_argument(
@@ -61,14 +59,15 @@
         type=validate_shell_args,
         default="",
         help=f"Shell to make aliases for. Supported shells are: {SUPPORTED_SHELLS}.",
     )
     parser.add_argument("--stdout", action="store_true", help="Write output to stdout")
     parser.add_argument("--use_min_alias", action="store_true", help="Will use the min_alias list.")
     args = parser.parse_args()
+    init_logger(args)
     return args
 
 
 def validate_file_exists(file_path: str) -> Path:
     if not file_path:
         return Path.home()
     path = find_file(file_path)
```

### Comparing `alias_gen-0.6.0/src/alias_gen/constants.py` & `alias_gen-0.6.1/src/alias_gen/constants.py`

 * *Files identical despite different names*

### Comparing `alias_gen-0.6.0/src/alias_gen/file_utils.py` & `alias_gen-0.6.1/src/alias_gen/file_utils.py`

 * *Files identical despite different names*

### Comparing `alias_gen-0.6.0/PKG-INFO` & `alias_gen-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alias-gen
-Version: 0.6.0
+Version: 0.6.1
 Summary: Generate bash/zsh/fish shell aliases automatically.
 License: MIT
 Keywords: alias,bash,zsh,fish,shell,cli,command-line,command,completion,abbr,generate,terminal
 Author: Ariel Frischer
 Author-email: arielfrischer@gmail.com
 Maintainer: Ariel Frischer
 Maintainer-email: arielfrischer@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: alias-gen Version: 0.6.0 Summary: Generate bash/
+Metadata-Version: 2.1 Name: alias-gen Version: 0.6.1 Summary: Generate bash/
 zsh/fish shell aliases automatically. License: MIT Keywords:
 alias,bash,zsh,fish,shell,cli,command-
 line,command,completion,abbr,generate,terminal Author: Ariel Frischer Author-
 email: arielfrischer@gmail.com Maintainer: Ariel Frischer Maintainer-email:
 arielfrischer@gmail.com Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 2 Classifier: Programming Language :: Python :: 2.7 Classifier:
```

