# Comparing `tmp/bili_eta-0.1.5.tar.gz` & `tmp/bili_eta-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bili_eta-0.1.5.tar", max compression
+gzip compressed data, was "bili_eta-0.1.6.tar", max compression
```

## Comparing `bili_eta-0.1.5.tar` & `bili_eta-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.1.5/bili_eta/__init__.py
--rw-r--r--   0        0        0      922 2023-07-30 12:21:42.009481 bili_eta-0.1.5/bili_eta/__main__.py
--rw-r--r--   0        0        0      421 2023-07-30 12:15:27.190137 bili_eta-0.1.5/bili_eta/bot.py
--rw-r--r--   0        0        0      562 2023-07-30 12:24:49.289436 bili_eta-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      644 1970-01-01 00:00:00.000000 bili_eta-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.1.6/bili_eta/__init__.py
+-rw-r--r--   0        0        0      946 2023-07-30 12:28:03.489510 bili_eta-0.1.6/bili_eta/__main__.py
+-rw-r--r--   0        0        0      421 2023-07-30 12:15:27.190137 bili_eta-0.1.6/bili_eta/bot.py
+-rw-r--r--   0        0        0      561 2023-07-30 12:30:05.805601 bili_eta-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 bili_eta-0.1.6/PKG-INFO
```

### Comparing `bili_eta-0.1.5/bili_eta/__main__.py` & `bili_eta-0.1.6/bili_eta/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 def main():
     pass
 
 
 @click.command()
 def start():
     creat_config()
+    creat_plugins_dir()
     run()
 
 
 main.add_command(start)
 
 
 def creat_config():
```

### Comparing `bili_eta-0.1.5/pyproject.toml` & `bili_eta-0.1.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "bili-eta"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["Polyisoprene <lzxder@outlook.com>"]
 readme = "README.md"
 packages = [{include = "bili_eta"}]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.8"
 click = "^8.1.6"
 python-dotenv = "^1.0.0"
 nonebot-adapter-onebot = "^2.2.3"
 nonebot2 = {extras = ["fastapi"], version = "^2.0.1"}
 nonebot-plugin-guild-patch = "^0.2.3"
 nonebot-plugin-apscheduler = "^0.3.0"
```

