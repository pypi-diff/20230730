# Comparing `tmp/alias_gen-0.6.1.tar.gz` & `tmp/alias_gen-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alias_gen-0.6.1.tar", max compression
+gzip compressed data, was "alias_gen-0.6.2.tar", max compression
```

## Comparing `alias_gen-0.6.1.tar` & `alias_gen-0.6.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1083 2023-01-02 05:01:18.992694 alias_gen-0.6.1/LICENSE.md
--rw-r--r--   0        0        0     2941 2023-07-29 22:51:32.041985 alias_gen-0.6.1/README.md
--rw-r--r--   0        0        0     1717 2023-07-29 23:08:15.646974 alias_gen-0.6.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-02 18:23:40.999671 alias_gen-0.6.1/src/alias_gen/__init__.py
--rw-r--r--   0        0        0     8646 2023-07-29 21:28:32.797869 alias_gen-0.6.1/src/alias_gen/aliaser.py
--rw-r--r--   0        0        0     3642 2023-07-29 23:08:09.455356 alias_gen-0.6.1/src/alias_gen/arg_parser.py
--rw-r--r--   0        0        0      560 2023-07-29 19:55:02.527718 alias_gen-0.6.1/src/alias_gen/constants.py
--rw-r--r--   0        0        0     2077 2023-07-29 20:03:46.355423 alias_gen-0.6.1/src/alias_gen/file_utils.py
--rw-r--r--   0        0        0      293 2023-07-29 21:33:37.953491 alias_gen-0.6.1/src/alias_gen/logger.py
--rw-r--r--   0        0        0     3981 1970-01-01 00:00:00.000000 alias_gen-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-01-02 05:01:18.992694 alias_gen-0.6.2/LICENSE.md
+-rw-r--r--   0        0        0     2941 2023-07-29 22:51:32.041985 alias_gen-0.6.2/README.md
+-rw-r--r--   0        0        0     1717 2023-07-29 23:14:32.168114 alias_gen-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-02 18:23:40.999671 alias_gen-0.6.2/src/alias_gen/__init__.py
+-rw-r--r--   0        0        0     8677 2023-07-29 23:13:52.329635 alias_gen-0.6.2/src/alias_gen/aliaser.py
+-rw-r--r--   0        0        0     3642 2023-07-29 23:13:15.301323 alias_gen-0.6.2/src/alias_gen/arg_parser.py
+-rw-r--r--   0        0        0      560 2023-07-29 19:55:02.527718 alias_gen-0.6.2/src/alias_gen/constants.py
+-rw-r--r--   0        0        0     2077 2023-07-29 20:03:46.355423 alias_gen-0.6.2/src/alias_gen/file_utils.py
+-rw-r--r--   0        0        0      293 2023-07-29 21:33:37.953491 alias_gen-0.6.2/src/alias_gen/logger.py
+-rw-r--r--   0        0        0     3981 1970-01-01 00:00:00.000000 alias_gen-0.6.2/PKG-INFO
```

### Comparing `alias_gen-0.6.1/LICENSE.md` & `alias_gen-0.6.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `alias_gen-0.6.1/README.md` & `alias_gen-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `alias_gen-0.6.1/pyproject.toml` & `alias_gen-0.6.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="alias-gen"
-version="0.6.1"
+version="0.6.2"
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
-version = "0.6.1"
+version = "0.6.2"
 description = "Generate bash/zsh/fish shell aliases automatically."
 authors=["Ariel Frischer <arielfrischer@gmail.com>"]
 maintainers=["Ariel Frischer <arielfrischer@gmail.com>"]
 readme = "README.md"
 classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `alias_gen-0.6.1/src/alias_gen/aliaser.py` & `alias_gen-0.6.2/src/alias_gen/aliaser.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,17 @@
 
 
 def main():
     args = parse_args()
     debug(f"args: {args}")
 
     shell, hist_path, max_suggestions = args.s, args.f, args.n
-    print(f"Detected shell: {shell}")
+
+    if not args.stdout:
+        print(f"Detected shell: {shell}")
 
     sorted_commands, used_aliases = get_all_commands(hist_path, shell)
 
     results = gen_aliases(max_suggestions, sorted_commands, used_aliases)
 
     if args.stdout:
         print_results(results, shell, not args.use_min_alias)
@@ -132,14 +134,15 @@
     th = ("cmd", "freq", "alias", "min_alias")
     print(f"{th[0]:<20}{th[1]:<10}{th[2]:<10}{th[3]:<10}\n")
 
     for cmd, freq, alias, minimal_alias in results:
         f_cmd = cmd[:15] if len(cmd) <= 15 else (cmd[:15] + "...")
         print(f"{f_cmd:<20}{freq:<10}{alias:<10}{minimal_alias:<10}")
 
+
 def extract_commands(file_contents: str, shell: str) -> List[str]:
     commands = []
     if shell == "fish":
         regex = r"- cmd: (.*)"
     else:  # Assume zsh
         regex = r": \d+:\d+;(.*)"
     for line in file_contents.split("\n"):
@@ -148,14 +151,15 @@
             command = match.group(1).strip()
             if command:
                 first_word = command.split(" ", 1)[0]
                 if len(first_word) > 2:
                     commands.append(first_word)
     return commands
 
+
 # def extract_commands(file_contents: str, shell: str) -> List[str]:
 #     commands = []
 #     regex = r"- cmd: (.*)" if shell == "fish" else r"(.*)$"
 #     for line in file_contents.split("\n"):
 #         match = re.search(regex, line)
 #         if match:
 #             first_word = match.group(1).split(" ", 1)[0]
```

### Comparing `alias_gen-0.6.1/src/alias_gen/arg_parser.py` & `alias_gen-0.6.2/src/alias_gen/arg_parser.py`

 * *Files identical despite different names*

### Comparing `alias_gen-0.6.1/src/alias_gen/constants.py` & `alias_gen-0.6.2/src/alias_gen/constants.py`

 * *Files identical despite different names*

### Comparing `alias_gen-0.6.1/src/alias_gen/file_utils.py` & `alias_gen-0.6.2/src/alias_gen/file_utils.py`

 * *Files identical despite different names*

### Comparing `alias_gen-0.6.1/PKG-INFO` & `alias_gen-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alias-gen
-Version: 0.6.1
+Version: 0.6.2
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
-Metadata-Version: 2.1 Name: alias-gen Version: 0.6.1 Summary: Generate bash/
+Metadata-Version: 2.1 Name: alias-gen Version: 0.6.2 Summary: Generate bash/
 zsh/fish shell aliases automatically. License: MIT Keywords:
 alias,bash,zsh,fish,shell,cli,command-
 line,command,completion,abbr,generate,terminal Author: Ariel Frischer Author-
 email: arielfrischer@gmail.com Maintainer: Ariel Frischer Maintainer-email:
 arielfrischer@gmail.com Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 2 Classifier: Programming Language :: Python :: 2.7 Classifier:
```

