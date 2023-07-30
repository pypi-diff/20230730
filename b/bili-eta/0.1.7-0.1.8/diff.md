# Comparing `tmp/bili_eta-0.1.7.tar.gz` & `tmp/bili_eta-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bili_eta-0.1.7.tar", max compression
+gzip compressed data, was "bili_eta-0.1.8.tar", max compression
```

## Comparing `bili_eta-0.1.7.tar` & `bili_eta-0.1.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.1.7/README.md
--rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.1.7/bili_eta/__init__.py
--rw-r--r--   0        0        0      946 2023-07-30 12:28:03.489510 bili_eta-0.1.7/bili_eta/__main__.py
--rw-r--r--   0        0        0      541 2023-07-30 12:39:21.039119 bili_eta-0.1.7/bili_eta/bot.py
--rw-r--r--   0        0        0      561 2023-07-30 12:39:45.621749 bili_eta-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 bili_eta-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.1.8/bili_eta/__init__.py
+-rw-r--r--   0        0        0      767 2023-07-30 12:45:58.526166 bili_eta-0.1.8/bili_eta/__main__.py
+-rw-r--r--   0        0        0      552 2023-07-30 12:46:33.433085 bili_eta-0.1.8/bili_eta/bot.py
+-rw-r--r--   0        0        0      561 2023-07-30 12:46:42.924799 bili_eta-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 bili_eta-0.1.8/PKG-INFO
```

### Comparing `bili_eta-0.1.7/bili_eta/__main__.py` & `bili_eta-0.1.8/bili_eta/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import click
 from os import path, getcwd,mkdir
-import dotenv
+import json
 from .bot import run
-env = {
+config = {
     'HOST': '127.0.0.1',
     'PORT': '8080',
     'SUPERUSERS': [],
     'COMMAND_START': [''],
     'DynTextFont':'',
     'DynEmojiFont':'',
     'DynFontStyle':''
@@ -26,23 +26,17 @@
     run()
 
 
 main.add_command(start)
 
 
 def creat_config():
-    env_file_path = path.join(getcwd(), ".env.prod")
-    if not path.exists(env_file_path):
-        for key, value in env.items():
-            dotenv.set_key(
-                env_file_path,
-                key,
-                str(value).replace(' ', ''),
-                quote_mode="never",
-            )
+    config_file_path = path.join(getcwd(), "config.json")
+    if not path.exists(config_file_path):
+        json.dump(config)
     
 
 def creat_plugins_dir():
     plugins_dir_path = path.join(getcwd(),"plugins")
     if not path.exists(plugins_dir_path):
         mkdir(plugins_dir_path)
```

### Comparing `bili_eta-0.1.7/bili_eta/bot.py` & `bili_eta-0.1.8/bili_eta/bot.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 
 import nonebot
 from nonebot.adapters.onebot.v11 import Adapter
 from os import path, getcwd
-from dotenv import load_dotenv
+import json
 
-
-env_file_path = path.join(getcwd(), ".env.prod")
-load_dotenv(dotenv_path=env_file_path)
-nonebot.init()
+config_file_path = path.join(getcwd(), "config.json")
+nonebot.init(**json.load(config_file_path))
 driver = nonebot.get_driver()
 driver.register_adapter(Adapter)
 app = nonebot.get_asgi()
 
 plugin_path = path.join(getcwd(),"plugins")
 
 inner_plugin_path = path.join(path.dirname(path.abspath(__file__)),"src")
 
 nonebot.load_plugins(plugin_path,inner_plugin_path)
-
+config = nonebot.get_driver().config
 
 def run():
     nonebot.run(app="bili_eta.bot:app")
```

### Comparing `bili_eta-0.1.7/pyproject.toml` & `bili_eta-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bili-eta"
-version = "0.1.7"
+version = "0.1.8"
 description = ""
 authors = ["Polyisoprene <lzxder@outlook.com>"]
 readme = "README.md"
 packages = [{include = "bili_eta"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `bili_eta-0.1.7/PKG-INFO` & `bili_eta-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bili-eta
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: Polyisoprene
 Author-email: lzxder@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

