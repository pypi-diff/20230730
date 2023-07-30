# Comparing `tmp/bili_eta-0.2.2.tar.gz` & `tmp/bili_eta-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bili_eta-0.2.2.tar", max compression
+gzip compressed data, was "bili_eta-0.2.3.tar", max compression
```

## Comparing `bili_eta-0.2.2.tar` & `bili_eta-0.2.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.2.2/README.md
--rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.2.2/bili_eta/__init__.py
--rw-r--r--   0        0        0      991 2023-07-30 13:23:10.406135 bili_eta-0.2.2/bili_eta/__main__.py
--rw-r--r--   0        0        0      467 2023-07-30 13:25:42.817920 bili_eta-0.2.2/bili_eta/bot.py
--rw-r--r--   0        0        0      561 2023-07-30 13:25:45.901913 bili_eta-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 bili_eta-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.2.3/bili_eta/__init__.py
+-rw-r--r--   0        0        0      991 2023-07-30 13:23:10.406135 bili_eta-0.2.3/bili_eta/__main__.py
+-rw-r--r--   0        0        0      294 2023-07-30 14:02:01.768983 bili_eta-0.2.3/bili_eta/bot.py
+-rw-r--r--   0        0        0      621 2023-07-30 14:02:51.028295 bili_eta-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 bili_eta-0.2.3/PKG-INFO
```

### Comparing `bili_eta-0.2.2/bili_eta/__main__.py` & `bili_eta-0.2.3/bili_eta/__main__.py`

 * *Files identical despite different names*

### Comparing `bili_eta-0.2.2/pyproject.toml` & `bili_eta-0.2.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bili-eta"
-version = "0.2.2"
+version = "0.2.3"
 description = ""
 authors = ["Polyisoprene <lzxder@outlook.com>"]
 readme = "README.md"
 packages = [{include = "bili_eta"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -14,10 +14,14 @@
 nonebot2 = {extras = ["fastapi"], version = "^2.0.1"}
 nonebot-plugin-guild-patch = "^0.2.3"
 nonebot-plugin-apscheduler = "^0.3.0"
 
 [tool.poetry.scripts]
 eta = "bili_eta.__main__:main"
 
+[tool.nonebot]
+plugin_dirs = ["src/"]
+builtin_plugins = []
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `bili_eta-0.2.2/PKG-INFO` & `bili_eta-0.2.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bili-eta
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
 Author: Polyisoprene
 Author-email: lzxder@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

