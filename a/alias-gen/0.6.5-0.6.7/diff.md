# Comparing `tmp/alias_gen-0.6.5.tar.gz` & `tmp/alias_gen-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alias_gen-0.6.5.tar", max compression
+gzip compressed data, was "alias_gen-0.6.7.tar", max compression
```

## Comparing `alias_gen-0.6.5.tar` & `alias_gen-0.6.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1083 2023-01-02 05:01:18.992694 alias_gen-0.6.5/LICENSE.md
--rw-r--r--   0        0        0     3000 2023-07-30 00:49:47.681213 alias_gen-0.6.5/README.md
--rw-r--r--   0        0        0     1717 2023-07-30 00:50:40.126518 alias_gen-0.6.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-02 18:23:40.999671 alias_gen-0.6.5/src/alias_gen/__init__.py
--rw-r--r--   0        0        0     8677 2023-07-29 23:13:52.329635 alias_gen-0.6.5/src/alias_gen/aliaser.py
--rw-r--r--   0        0        0     3642 2023-07-29 23:13:15.301323 alias_gen-0.6.5/src/alias_gen/arg_parser.py
--rw-r--r--   0        0        0      560 2023-07-29 19:55:02.527718 alias_gen-0.6.5/src/alias_gen/constants.py
--rw-r--r--   0        0        0     2077 2023-07-29 20:03:46.355423 alias_gen-0.6.5/src/alias_gen/file_utils.py
--rw-r--r--   0        0        0      293 2023-07-29 21:33:37.953491 alias_gen-0.6.5/src/alias_gen/logger.py
--rw-r--r--   0        0        0     4040 1970-01-01 00:00:00.000000 alias_gen-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-01-02 05:01:18.992694 alias_gen-0.6.7/LICENSE.md
+-rw-r--r--   0        0        0     3000 2023-07-30 00:49:47.681213 alias_gen-0.6.7/README.md
+-rw-r--r--   0        0        0     1730 2023-07-30 02:55:01.899928 alias_gen-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-02 18:23:40.999671 alias_gen-0.6.7/src/alias_gen/__init__.py
+-rw-r--r--   0        0        0     8301 2023-07-30 02:51:14.319561 alias_gen-0.6.7/src/alias_gen/aliaser.py
+-rw-r--r--   0        0        0     3642 2023-07-29 23:13:15.301323 alias_gen-0.6.7/src/alias_gen/arg_parser.py
+-rw-r--r--   0        0        0      560 2023-07-29 19:55:02.527718 alias_gen-0.6.7/src/alias_gen/constants.py
+-rw-r--r--   0        0        0     1985 2023-07-30 02:02:07.765504 alias_gen-0.6.7/src/alias_gen/file_utils.py
+-rw-r--r--   0        0        0      293 2023-07-29 21:33:37.953491 alias_gen-0.6.7/src/alias_gen/logger.py
+-rw-r--r--   0        0        0     4040 1970-01-01 00:00:00.000000 alias_gen-0.6.7/PKG-INFO
```

### Comparing `alias_gen-0.6.5/LICENSE.md` & `alias_gen-0.6.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `alias_gen-0.6.5/README.md` & `alias_gen-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `alias_gen-0.6.5/pyproject.toml` & `alias_gen-0.6.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="alias-gen"
-version="0.6.5"
+version="0.6.7"
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
-version = "0.6.5"
+version="0.6.7"
 description = "Generate bash/zsh/fish shell aliases automatically."
 authors=["Ariel Frischer <arielfrischer@gmail.com>"]
 maintainers=["Ariel Frischer <arielfrischer@gmail.com>"]
 readme = "README.md"
 classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -77,10 +77,11 @@
 
 [tool.black]
 line-length = 120
 [tool.ruff]
 line-length = 120
 
 [[tool.mypy.overrides]]
-module = ["setuptools.*"]
+module = ["setuptools.*",
+"alias_gen.*"]
 ignore_missing_imports = true
```

### Comparing `alias_gen-0.6.5/src/alias_gen/aliaser.py` & `alias_gen-0.6.7/src/alias_gen/aliaser.py`

 * *Files 6% similar despite different names*

```diff
@@ -152,37 +152,26 @@
             if command:
                 first_word = command.split(" ", 1)[0]
                 if len(first_word) > 2:
                     commands.append(first_word)
     return commands
 
 
-# def extract_commands(file_contents: str, shell: str) -> List[str]:
-#     commands = []
-#     regex = r"- cmd: (.*)" if shell == "fish" else r"(.*)$"
-#     for line in file_contents.split("\n"):
-#         match = re.search(regex, line)
-#         if match:
-#             first_word = match.group(1).split(" ", 1)[0]
-#             if len(first_word) > 2:
-#                 commands.append(first_word)
-#     return commands
-#
-#
 def get_command_frequencies(commands: List[str]) -> Dict[str, int]:
     frequency: Dict[str, int] = {}
     for cmd in commands:
         if cmd:
             frequency[cmd] = frequency.get(cmd, 0) + 1
     return frequency
 
 
 def get_all_system_commands(commands_txt: str) -> Set[str]:
     commands = commands_txt.split("\n")
     commands = [cmd.split("\t")[0] for cmd in commands]
+    commands = [c for c in commands if c.strip()]
     return set(commands)
 
 
 def get_bash_commands(shell: str) -> Set[str]:
     compgen_command = "bash -c 'compgen -c'"
     command = compgen_command
```

### Comparing `alias_gen-0.6.5/src/alias_gen/arg_parser.py` & `alias_gen-0.6.7/src/alias_gen/arg_parser.py`

 * *Files identical despite different names*

### Comparing `alias_gen-0.6.5/src/alias_gen/constants.py` & `alias_gen-0.6.7/src/alias_gen/constants.py`

 * *Files identical despite different names*

### Comparing `alias_gen-0.6.5/src/alias_gen/file_utils.py` & `alias_gen-0.6.7/src/alias_gen/file_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,24 +40,18 @@
     detected_encoding = get_encoding(file_path)
     encodings_to_try = [detected_encoding] + SUPPORTED_FILE_ENCODINGS
 
     for encoding in encodings_to_try:
         try:
             with open(file_path, "r", encoding=encoding) as f:
                 file_contents = f.read()
-            debug(
-                f"Succesfully read file contents of path: {file_path} "
-                f"with encoding: {encoding}."
-            )
+            debug(f"Succesfully read file contents of path: {file_path} " f"with encoding: {encoding}.")
             return file_contents
         except UnicodeDecodeError:
-            debug(
-                f"Failed to read file contents of path: {file_path} "
-                f"with encoding: {encoding}."
-            )
+            debug(f"Failed to read file contents of path: {file_path} " f"with encoding: {encoding}.")
 
     return ""
 
 
 def get_history_file_path(shell: str) -> Path:
     home_dir = Path.home()
     if shell == "fish":
```

### Comparing `alias_gen-0.6.5/PKG-INFO` & `alias_gen-0.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alias-gen
-Version: 0.6.5
+Version: 0.6.7
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
-Metadata-Version: 2.1 Name: alias-gen Version: 0.6.5 Summary: Generate bash/
+Metadata-Version: 2.1 Name: alias-gen Version: 0.6.7 Summary: Generate bash/
 zsh/fish shell aliases automatically. License: MIT Keywords:
 alias,bash,zsh,fish,shell,cli,command-
 line,command,completion,abbr,generate,terminal Author: Ariel Frischer Author-
 email: arielfrischer@gmail.com Maintainer: Ariel Frischer Maintainer-email:
 arielfrischer@gmail.com Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 2 Classifier: Programming Language :: Python :: 2.7 Classifier:
```

