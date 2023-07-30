# Comparing `tmp/bili_eta-0.1.8.tar.gz` & `tmp/bili_eta-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bili_eta-0.1.8.tar", max compression
+gzip compressed data, was "bili_eta-0.1.9.tar", max compression
```

## Comparing `bili_eta-0.1.8.tar` & `bili_eta-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.1.8/bili_eta/__init__.py
--rw-r--r--   0        0        0      767 2023-07-30 12:45:58.526166 bili_eta-0.1.8/bili_eta/__main__.py
--rw-r--r--   0        0        0      552 2023-07-30 12:46:33.433085 bili_eta-0.1.8/bili_eta/bot.py
--rw-r--r--   0        0        0      561 2023-07-30 12:46:42.924799 bili_eta-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 bili_eta-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.1.9/bili_eta/__init__.py
+-rw-r--r--   0        0        0      983 2023-07-30 13:08:32.578029 bili_eta-0.1.9/bili_eta/__main__.py
+-rw-r--r--   0        0        0      458 2023-07-30 13:04:22.909094 bili_eta-0.1.9/bili_eta/bot.py
+-rw-r--r--   0        0        0      561 2023-07-30 13:09:01.453688 bili_eta-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 bili_eta-0.1.9/PKG-INFO
```

### Comparing `bili_eta-0.1.8/bili_eta/__main__.py` & `bili_eta-0.1.9/bili_eta/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import click
 from os import path, getcwd,mkdir
-import json
-from .bot import run
-config = {
-    'HOST': '127.0.0.1',
+import dotenv
+
+env = {
+    'HOST':'127.0.0.1',
     'PORT': '8080',
     'SUPERUSERS': [],
-    'COMMAND_START': [''],
     'DynTextFont':'',
     'DynEmojiFont':'',
     'DynFontStyle':''
     
 }
 
 
@@ -19,28 +18,37 @@
     pass
 
 
 @click.command()
 def start():
     creat_config()
     creat_plugins_dir()
+    from .bot import run
     run()
 
 
 main.add_command(start)
 
 
 def creat_config():
-    config_file_path = path.join(getcwd(), "config.json")
-    if not path.exists(config_file_path):
-        json.dump(config)
+    env_file_path = path.join(getcwd(), ".env.prod")
+    if not path.exists(env_file_path):
+        for key, value in env.items():
+            dotenv.set_key(
+                env_file_path,
+                key,
+                str(value).replace(' ', ''),
+                quote_mode="never",
+            )
     
 
 def creat_plugins_dir():
     plugins_dir_path = path.join(getcwd(),"plugins")
     if not path.exists(plugins_dir_path):
         mkdir(plugins_dir_path)
     
 
 
-if __name__ == "__main__":
-    creat_config()
+# if __name__ == "__main__":
+#     creat_config()
+#     from bot import driver
+#     print(driver.config)
```

### Comparing `bili_eta-0.1.8/pyproject.toml` & `bili_eta-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bili-eta"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["Polyisoprene <lzxder@outlook.com>"]
 readme = "README.md"
 packages = [{include = "bili_eta"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `bili_eta-0.1.8/PKG-INFO` & `bili_eta-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bili-eta
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Polyisoprene
 Author-email: lzxder@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

