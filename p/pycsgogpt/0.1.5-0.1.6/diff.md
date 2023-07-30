# Comparing `tmp/pycsgogpt-0.1.5.tar.gz` & `tmp/pycsgogpt-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycsgogpt-0.1.5.tar", max compression
+gzip compressed data, was "pycsgogpt-0.1.6.tar", max compression
```

## Comparing `pycsgogpt-0.1.5.tar` & `pycsgogpt-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1062 2023-07-25 19:54:27.951459 pycsgogpt-0.1.5/LICENSE
--rw-r--r--   0        0        0     1049 2023-07-25 19:54:27.951459 pycsgogpt-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-07-25 19:54:27.951459 pycsgogpt-0.1.5/pycsgogpt/__init__.py
--rw-r--r--   0        0        0      749 2023-07-25 19:54:27.951459 pycsgogpt-0.1.5/pycsgogpt/__main__.py
--rw-r--r--   0        0        0     2549 2023-07-25 19:54:27.951459 pycsgogpt-0.1.5/pycsgogpt/csgo_chatbot.py
--rw-r--r--   0        0        0      807 2023-07-25 19:54:27.951459 pycsgogpt-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1922 1970-01-01 00:00:00.000000 pycsgogpt-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-30 21:10:03.979382 pycsgogpt-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1049 2023-07-30 21:10:03.979382 pycsgogpt-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-07-30 21:10:03.979382 pycsgogpt-0.1.6/pycsgogpt/__init__.py
+-rw-r--r--   0        0        0      820 2023-07-30 21:10:03.979382 pycsgogpt-0.1.6/pycsgogpt/__main__.py
+-rw-r--r--   0        0        0     4123 2023-07-30 21:10:03.979382 pycsgogpt-0.1.6/pycsgogpt/csgo_chatbot.py
+-rw-r--r--   0        0        0      826 2023-07-30 21:10:03.979382 pycsgogpt-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1962 1970-01-01 00:00:00.000000 pycsgogpt-0.1.6/PKG-INFO
```

### Comparing `pycsgogpt-0.1.5/LICENSE` & `pycsgogpt-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pycsgogpt-0.1.5/README.md` & `pycsgogpt-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pycsgogpt-0.1.5/pycsgogpt/__main__.py` & `pycsgogpt-0.1.6/pycsgogpt/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 import typer
 from pycsgogpt.csgo_chatbot import CSGOChatBot
 
 app = typer.Typer()
 
-def entry(player_name: str, openapi_key: str, telnet_port: int = typer.Option(21234, help="The telnet port for the CSGO server.")) -> None:
-    chat_bot = CSGOChatBot(telnet_port, player_name)
+def entry(
+    player_name: str,
+    openapi_key: str,
+    telnet_port: int = typer.Option(21234,
+    help="The telnet port for the CSGO server."),
+    chat_history_size: int = 20,
+) -> None:
+    chat_bot = CSGOChatBot(telnet_port, player_name, chat_history_size)
     chat_bot.set_openai_key(openapi_key)
 
     try:
         chat_bot.loop()
     except KeyboardInterrupt:
         print("Exiting...")
     except ConnectionRefusedError:
```

### Comparing `pycsgogpt-0.1.5/pyproject.toml` & `pycsgogpt-0.1.6/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 [tool.poetry]
 name = "pycsgogpt"
-version = "0.1.5"
+version = "0.1.6"
 description = "CSGO Chatbot using OpenAI GPT-3.5 Turbo."
 authors = ["Aviv <4440524+nikeix@users.noreply.github.com>"]
 license = "MIT"
 keywords = ["csgo", "chatbot", "openai", "gpt"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
@@ -19,14 +19,15 @@
 
 
 [tool.poetry.dependencies]
 python = "^3.7.1"
 openai = "^0.27.8"
 telnetlib3 = "^2.0.2"
 typer = "^0.9.0"
+backoff = "^2.2.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 pycsgogpt = "pycsgogpt.__main__:main"
```

### Comparing `pycsgogpt-0.1.5/PKG-INFO` & `pycsgogpt-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pycsgogpt
-Version: 0.1.5
+Version: 0.1.6
 Summary: CSGO Chatbot using OpenAI GPT-3.5 Turbo.
 Home-page: https://github.com/nikeix/pycsgogpt
 License: MIT
 Keywords: csgo,chatbot,openai,gpt
 Author: Aviv
 Author-email: 4440524+nikeix@users.noreply.github.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
+Requires-Dist: backoff (>=2.2.1,<3.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: telnetlib3 (>=2.0.2,<3.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/nikeix/pycsgogpt
 Description-Content-Type: text/markdown
 
 # pycsgogpt
```

