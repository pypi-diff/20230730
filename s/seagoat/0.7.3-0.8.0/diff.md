# Comparing `tmp/seagoat-0.7.3.tar.gz` & `tmp/seagoat-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seagoat-0.7.3.tar", max compression
+gzip compressed data, was "seagoat-0.8.0.tar", max compression
```

## Comparing `seagoat-0.7.3.tar` & `seagoat-0.8.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1070 2023-07-30 14:44:33.843920 seagoat-0.7.3/LICENSE
--rw-r--r--   0        0        0     1847 2023-07-30 14:44:33.843920 seagoat-0.7.3/README.md
--rw-r--r--   0        0        0     3085 2023-07-30 14:45:30.484336 seagoat-0.7.3/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-30 14:45:30.484336 seagoat-0.7.3/seagoat/__init__.py
--rw-r--r--   0        0        0     1601 2023-07-30 14:44:33.851920 seagoat-0.7.3/seagoat/cache.py
--rw-r--r--   0        0        0     3103 2023-07-30 14:44:33.851920 seagoat-0.7.3/seagoat/cli.py
--rw-r--r--   0        0        0      196 2023-07-30 14:44:33.851920 seagoat-0.7.3/seagoat/common.py
--rw-r--r--   0        0        0     4424 2023-07-30 14:44:33.851920 seagoat-0.7.3/seagoat/engine.py
--rw-r--r--   0        0        0     3492 2023-07-30 14:44:33.851920 seagoat-0.7.3/seagoat/file.py
--rw-r--r--   0        0        0     2689 2023-07-30 14:44:33.851920 seagoat-0.7.3/seagoat/repository.py
--rw-r--r--   0        0        0     2021 2023-07-30 14:44:33.851920 seagoat-0.7.3/seagoat/result.py
--rw-r--r--   0        0        0     5766 2023-07-30 14:44:33.851920 seagoat-0.7.3/seagoat/server.py
--rw-r--r--   0        0        0     1692 2023-07-30 14:44:33.851920 seagoat-0.7.3/seagoat/sources/chroma.py
--rw-r--r--   0        0        0     1105 2023-07-30 14:44:33.851920 seagoat-0.7.3/seagoat/sources/ripgrep.py
--rw-r--r--   0        0        0     2861 1970-01-01 00:00:00.000000 seagoat-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-30 17:23:50.180361 seagoat-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1847 2023-07-30 17:23:50.184361 seagoat-0.8.0/README.md
+-rw-r--r--   0        0        0     3085 2023-07-30 17:23:50.980374 seagoat-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-30 17:23:50.980374 seagoat-0.8.0/seagoat/__init__.py
+-rw-r--r--   0        0        0     1601 2023-07-30 17:23:50.188361 seagoat-0.8.0/seagoat/cache.py
+-rw-r--r--   0        0        0     2901 2023-07-30 17:23:50.188361 seagoat-0.8.0/seagoat/cli.py
+-rw-r--r--   0        0        0      196 2023-07-30 17:23:50.188361 seagoat-0.8.0/seagoat/common.py
+-rw-r--r--   0        0        0     4424 2023-07-30 17:23:50.188361 seagoat-0.8.0/seagoat/engine.py
+-rw-r--r--   0        0        0     3492 2023-07-30 17:23:50.188361 seagoat-0.8.0/seagoat/file.py
+-rw-r--r--   0        0        0     2689 2023-07-30 17:23:50.188361 seagoat-0.8.0/seagoat/repository.py
+-rw-r--r--   0        0        0     2021 2023-07-30 17:23:50.188361 seagoat-0.8.0/seagoat/result.py
+-rw-r--r--   0        0        0     5766 2023-07-30 17:23:50.188361 seagoat-0.8.0/seagoat/server.py
+-rw-r--r--   0        0        0     1692 2023-07-30 17:23:50.188361 seagoat-0.8.0/seagoat/sources/chroma.py
+-rw-r--r--   0        0        0     1105 2023-07-30 17:23:50.188361 seagoat-0.8.0/seagoat/sources/ripgrep.py
+-rw-r--r--   0        0        0     2861 1970-01-01 00:00:00.000000 seagoat-0.8.0/PKG-INFO
```

### Comparing `seagoat-0.7.3/LICENSE` & `seagoat-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seagoat-0.7.3/README.md` & `seagoat-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `seagoat-0.7.3/pyproject.toml` & `seagoat-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seagoat"
-version = "0.7.3"
+version = "0.8.0"
 description = "A semantic-code search engine"
 authors = ["Daniel Kantor <git@daniel-kantor.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.scripts]
 gt = "seagoat.cli:seagoat"
```

### Comparing `seagoat-0.7.3/seagoat/cache.py` & `seagoat-0.8.0/seagoat/cache.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.7.3/seagoat/cli.py` & `seagoat-0.8.0/seagoat/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import sys
 from functools import cache
 
 import click
 import requests
 from pygments import highlight
 from pygments.formatters import TerminalFormatter
 from pygments.lexers import get_lexer_for_filename
@@ -10,24 +11,31 @@
 from pygments.lexers.javascript import TypeScriptLexer
 
 from seagoat import __version__
 from seagoat.server import get_server_info_file
 from seagoat.server import load_server_info
 
 
-def query_server(query, server_address):
-    response = requests.get(f"{server_address}/query/{query}")
+# pylint: disable-next=too-few-public-methods
+class ExitCode:
+    SERVER_NOT_RUNNING = 3
+
+
+def query_server(query, server_address, repo_path):
     try:
+        response = requests.get(f"{server_address}/query/{query}")
         response.raise_for_status()
-    except requests.exceptions.HTTPError as err:
-        print("HTTP error occurred:")
-        print(f"Response code: {response.status_code}")
-        print(f"Error: {err}")
-        print(f"Response body: {response.text}")
-        raise
+    except (requests.exceptions.ConnectionError, requests.exceptions.RequestException):
+        print(
+            f"The SeaGOAT server is not running. "
+            f"Please start the server using the following command:\n\n"
+            f"seagoat-server start {repo_path}\n"
+        )
+        sys.exit(ExitCode.SERVER_NOT_RUNNING)
+
     return response.json()["results"]
 
 
 @cache
 def get_highlighted_lines(file_name: str):
     with open(file_name, "r", encoding="utf-8") as source_code_file:
         code = source_code_file.read()
@@ -66,28 +74,17 @@
 @click.option(
     "--no-color",
     is_flag=True,
     help="Disable formatting. Automatically enabled when part of a bash pipeline.",
 )
 @click.version_option(version=__version__, prog_name="seagoat")
 def seagoat(query, repo_path, no_color):
-    """
-    Query your codebase for your QUERY in the Git repository REPO_PATH.
-
-    Your query can either be text that you expect to find in a file,
-    or a description of what you are looking for.
-
-    When REPO_PATH is not specified, the current working directory is
-    assumed to be the repository path.
-
-    In order to use seagoat in your repository, you need to run a server
-    that will analyze your codebase. Check seagoat-server --help for more
-    """
-    _, __, ___, server_address = load_server_info(get_server_info_file(repo_path))
-    results = query_server(query, server_address)
+    server_info_file = get_server_info_file(repo_path)
+    _, __, ___, server_address = load_server_info(server_info_file)
+    results = query_server(query, server_address, repo_path)
 
     color_enabled = os.isatty(0) and not no_color
     for result in results:
         for result_line in result.get("lines", []):
             print_result_line(result, result_line["line"], color_enabled)
```

### Comparing `seagoat-0.7.3/seagoat/engine.py` & `seagoat-0.8.0/seagoat/engine.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.7.3/seagoat/file.py` & `seagoat-0.8.0/seagoat/file.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.7.3/seagoat/repository.py` & `seagoat-0.8.0/seagoat/repository.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.7.3/seagoat/result.py` & `seagoat-0.8.0/seagoat/result.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.7.3/seagoat/server.py` & `seagoat-0.8.0/seagoat/server.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.7.3/seagoat/sources/chroma.py` & `seagoat-0.8.0/seagoat/sources/chroma.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.7.3/seagoat/sources/ripgrep.py` & `seagoat-0.8.0/seagoat/sources/ripgrep.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.7.3/PKG-INFO` & `seagoat-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seagoat
-Version: 0.7.3
+Version: 0.8.0
 Summary: A semantic-code search engine
 License: MIT
 Author: Daniel Kantor
 Author-email: git@daniel-kantor.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

