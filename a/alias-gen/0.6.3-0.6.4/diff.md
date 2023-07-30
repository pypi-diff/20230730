# Comparing `tmp/alias_gen-0.6.3.tar.gz` & `tmp/alias_gen-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alias_gen-0.6.3.tar", max compression
+gzip compressed data, was "alias_gen-0.6.4.tar", max compression
```

## Comparing `alias_gen-0.6.3.tar` & `alias_gen-0.6.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1083 2023-01-02 05:01:18.992694 alias_gen-0.6.3/LICENSE.md
--rw-r--r--   0        0        0     2913 2023-07-30 00:40:10.466830 alias_gen-0.6.3/README.md
--rw-r--r--   0        0        0     1717 2023-07-30 00:40:31.023956 alias_gen-0.6.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-02 18:23:40.999671 alias_gen-0.6.3/src/alias_gen/__init__.py
--rw-r--r--   0        0        0     8677 2023-07-29 23:13:52.329635 alias_gen-0.6.3/src/alias_gen/aliaser.py
--rw-r--r--   0        0        0     3642 2023-07-29 23:13:15.301323 alias_gen-0.6.3/src/alias_gen/arg_parser.py
--rw-r--r--   0        0        0      560 2023-07-29 19:55:02.527718 alias_gen-0.6.3/src/alias_gen/constants.py
--rw-r--r--   0        0        0     2077 2023-07-29 20:03:46.355423 alias_gen-0.6.3/src/alias_gen/file_utils.py
--rw-r--r--   0        0        0      293 2023-07-29 21:33:37.953491 alias_gen-0.6.3/src/alias_gen/logger.py
--rw-r--r--   0        0        0     3953 1970-01-01 00:00:00.000000 alias_gen-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-01-02 05:01:18.992694 alias_gen-0.6.4/LICENSE.md
+-rw-r--r--   0        0        0     3006 2023-07-30 00:47:11.962210 alias_gen-0.6.4/README.md
+-rw-r--r--   0        0        0     1717 2023-07-30 00:47:44.952398 alias_gen-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-02 18:23:40.999671 alias_gen-0.6.4/src/alias_gen/__init__.py
+-rw-r--r--   0        0        0     8677 2023-07-29 23:13:52.329635 alias_gen-0.6.4/src/alias_gen/aliaser.py
+-rw-r--r--   0        0        0     3642 2023-07-29 23:13:15.301323 alias_gen-0.6.4/src/alias_gen/arg_parser.py
+-rw-r--r--   0        0        0      560 2023-07-29 19:55:02.527718 alias_gen-0.6.4/src/alias_gen/constants.py
+-rw-r--r--   0        0        0     2077 2023-07-29 20:03:46.355423 alias_gen-0.6.4/src/alias_gen/file_utils.py
+-rw-r--r--   0        0        0      293 2023-07-29 21:33:37.953491 alias_gen-0.6.4/src/alias_gen/logger.py
+-rw-r--r--   0        0        0     4046 1970-01-01 00:00:00.000000 alias_gen-0.6.4/PKG-INFO
```

### Comparing `alias_gen-0.6.3/LICENSE.md` & `alias_gen-0.6.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `alias_gen-0.6.3/README.md` & `alias_gen-0.6.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # ALIAS-GEN 𑗊
 
-![Alt text](assets/screenshot.png)
+![Screenshot](https://gitlab.com/ariel-frischer/alias-gen/-/raw/124474a794a16bbcaffe059a06a32e4064eb76d1/assets/screenshot.png)
 
 Shell aliases are shortcuts or abbreviations for commands that are used in a Unix/Linux shell. They can save you time if you have very long or complex commands that you frequently use. ALIAS-GEN is a script that will create bash/zsh/fish shell aliases automatically to simplify your command-line tasks.
 
 This script will create bash/zsh/fish shell aliases automatically. You can generate a new alias file by following the prompts, or use the `--stdout` option to print results directly in your terminal.
 
 Two types of aliases are suggested, the default algorithm matches all characters incrementally for each command, while the `--use_min_alias` algorithm aims to minimize the total length of characters per command. 
 Additionally, `--use_min_alias` does not necessarily match all characters in the command.
```

#### html2text {}

```diff
@@ -1,18 +1,19 @@
-# ALIAS-GEN ð ![Alt text](assets/screenshot.png) Shell aliases are shortcuts
-or abbreviations for commands that are used in a Unix/Linux shell. They can
-save you time if you have very long or complex commands that you frequently
-use. ALIAS-GEN is a script that will create bash/zsh/fish shell aliases
-automatically to simplify your command-line tasks. This script will create
-bash/zsh/fish shell aliases automatically. You can generate a new alias file by
-following the prompts, or use the `--stdout` option to print results directly
-in your terminal. Two types of aliases are suggested, the default algorithm
-matches all characters incrementally for each command, while the `--
-use_min_alias` algorithm aims to minimize the total length of characters per
-command. Additionally, `--use_min_alias` does not necessarily match all
+# ALIAS-GEN ð ![Screenshot](https://gitlab.com/ariel-frischer/alias-gen/-/
+raw/124474a794a16bbcaffe059a06a32e4064eb76d1/assets/screenshot.png) Shell
+aliases are shortcuts or abbreviations for commands that are used in a Unix/
+Linux shell. They can save you time if you have very long or complex commands
+that you frequently use. ALIAS-GEN is a script that will create bash/zsh/fish
+shell aliases automatically to simplify your command-line tasks. This script
+will create bash/zsh/fish shell aliases automatically. You can generate a new
+alias file by following the prompts, or use the `--stdout` option to print
+results directly in your terminal. Two types of aliases are suggested, the
+default algorithm matches all characters incrementally for each command, while
+the `--use_min_alias` algorithm aims to minimize the total length of characters
+per command. Additionally, `--use_min_alias` does not necessarily match all
 characters in the command. The freq (frequency) column shows how often each
 command was used. For now, this script only generates aliases for the first
 word in a command. NOTE: Two character commands or less are not processed. By
 default, fish shell generates abbr (abbreviations) rather than aliases. ##
 Requirements - Python 3.6 or higher. - No dependences required for
 installation. ## Install from pypi ```bash pip install alias-gen ``` https://
 pypi.org/project/alias-gen/0.4.0/ ## CLI Usage Full Help Menu: ``` aliaser -
```

### Comparing `alias_gen-0.6.3/pyproject.toml` & `alias_gen-0.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="alias-gen"
-version="0.6.3"
+version="0.6.4"
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
-version = "0.6.3"
+version = "0.6.4"
 description = "Generate bash/zsh/fish shell aliases automatically."
 authors=["Ariel Frischer <arielfrischer@gmail.com>"]
 maintainers=["Ariel Frischer <arielfrischer@gmail.com>"]
 readme = "README.md"
 classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `alias_gen-0.6.3/src/alias_gen/aliaser.py` & `alias_gen-0.6.4/src/alias_gen/aliaser.py`

 * *Files identical despite different names*

### Comparing `alias_gen-0.6.3/src/alias_gen/arg_parser.py` & `alias_gen-0.6.4/src/alias_gen/arg_parser.py`

 * *Files identical despite different names*

### Comparing `alias_gen-0.6.3/src/alias_gen/constants.py` & `alias_gen-0.6.4/src/alias_gen/constants.py`

 * *Files identical despite different names*

### Comparing `alias_gen-0.6.3/src/alias_gen/file_utils.py` & `alias_gen-0.6.4/src/alias_gen/file_utils.py`

 * *Files identical despite different names*

### Comparing `alias_gen-0.6.3/PKG-INFO` & `alias_gen-0.6.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alias-gen
-Version: 0.6.3
+Version: 0.6.4
 Summary: Generate bash/zsh/fish shell aliases automatically.
 License: MIT
 Keywords: alias,bash,zsh,fish,shell,cli,command-line,command,completion,abbr,generate,terminal
 Author: Ariel Frischer
 Author-email: arielfrischer@gmail.com
 Maintainer: Ariel Frischer
 Maintainer-email: arielfrischer@gmail.com
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # ALIAS-GEN 𑗊
 
-![Alt text](assets/screenshot.png)
+![Screenshot](https://gitlab.com/ariel-frischer/alias-gen/-/raw/124474a794a16bbcaffe059a06a32e4064eb76d1/assets/screenshot.png)
 
 Shell aliases are shortcuts or abbreviations for commands that are used in a Unix/Linux shell. They can save you time if you have very long or complex commands that you frequently use. ALIAS-GEN is a script that will create bash/zsh/fish shell aliases automatically to simplify your command-line tasks.
 
 This script will create bash/zsh/fish shell aliases automatically. You can generate a new alias file by following the prompts, or use the `--stdout` option to print results directly in your terminal.
 
 Two types of aliases are suggested, the default algorithm matches all characters incrementally for each command, while the `--use_min_alias` algorithm aims to minimize the total length of characters per command. 
 Additionally, `--use_min_alias` does not necessarily match all characters in the command.
```

#### html2text {}

```diff
@@ -1,39 +1,40 @@
-Metadata-Version: 2.1 Name: alias-gen Version: 0.6.3 Summary: Generate bash/
+Metadata-Version: 2.1 Name: alias-gen Version: 0.6.4 Summary: Generate bash/
 zsh/fish shell aliases automatically. License: MIT Keywords:
 alias,bash,zsh,fish,shell,cli,command-
 line,command,completion,abbr,generate,terminal Author: Ariel Frischer Author-
 email: arielfrischer@gmail.com Maintainer: Ariel Frischer Maintainer-email:
 arielfrischer@gmail.com Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 2 Classifier: Programming Language :: Python :: 2.7 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.4 Classifier: Programming Language :: Python :: 3.5 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Description-
-Content-Type: text/markdown # ALIAS-GEN ð ![Alt text](assets/screenshot.png)
-Shell aliases are shortcuts or abbreviations for commands that are used in a
-Unix/Linux shell. They can save you time if you have very long or complex
-commands that you frequently use. ALIAS-GEN is a script that will create bash/
-zsh/fish shell aliases automatically to simplify your command-line tasks. This
-script will create bash/zsh/fish shell aliases automatically. You can generate
-a new alias file by following the prompts, or use the `--stdout` option to
-print results directly in your terminal. Two types of aliases are suggested,
-the default algorithm matches all characters incrementally for each command,
-while the `--use_min_alias` algorithm aims to minimize the total length of
-characters per command. Additionally, `--use_min_alias` does not necessarily
-match all characters in the command. The freq (frequency) column shows how
-often each command was used. For now, this script only generates aliases for
-the first word in a command. NOTE: Two character commands or less are not
-processed. By default, fish shell generates abbr (abbreviations) rather than
-aliases. ## Requirements - Python 3.6 or higher. - No dependences required for
-installation. ## Install from pypi ```bash pip install alias-gen ``` https://
-pypi.org/project/alias-gen/0.4.0/ ## CLI Usage Full Help Menu: ``` aliaser -
+Content-Type: text/markdown # ALIAS-GEN ð ![Screenshot](https://gitlab.com/
+ariel-frischer/alias-gen/-/raw/124474a794a16bbcaffe059a06a32e4064eb76d1/assets/
+screenshot.png) Shell aliases are shortcuts or abbreviations for commands that
+are used in a Unix/Linux shell. They can save you time if you have very long or
+complex commands that you frequently use. ALIAS-GEN is a script that will
+create bash/zsh/fish shell aliases automatically to simplify your command-line
+tasks. This script will create bash/zsh/fish shell aliases automatically. You
+can generate a new alias file by following the prompts, or use the `--stdout`
+option to print results directly in your terminal. Two types of aliases are
+suggested, the default algorithm matches all characters incrementally for each
+command, while the `--use_min_alias` algorithm aims to minimize the total
+length of characters per command. Additionally, `--use_min_alias` does not
+necessarily match all characters in the command. The freq (frequency) column
+shows how often each command was used. For now, this script only generates
+aliases for the first word in a command. NOTE: Two character commands or less
+are not processed. By default, fish shell generates abbr (abbreviations) rather
+than aliases. ## Requirements - Python 3.6 or higher. - No dependences required
+for installation. ## Install from pypi ```bash pip install alias-gen ``` https:
+//pypi.org/project/alias-gen/0.4.0/ ## CLI Usage Full Help Menu: ``` aliaser -
 h ``` Example usage to generate the top 40 aliases: ``` aliaser -n 40 ``` With
 stdout and min_alias: ``` aliaser --stdout --use_min_alias ``` The `-s`
 argument specifies the shell type. In this example, `fish` shell is used. ```
 aliaser -s fish ``` The `-f` argument allows you to specify a custom history
 file path. ``` aliaser -s zsh -f ~/.custom_zsh_history ``` ## How does it work?
 The `alias` column is generated by first sorting the most common commands found
 in the history file, then aliases are generated for commands more than two
```

