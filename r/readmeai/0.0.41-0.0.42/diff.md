# Comparing `tmp/readmeai-0.0.41.tar.gz` & `tmp/readmeai-0.0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readmeai-0.0.41.tar", max compression
+gzip compressed data, was "readmeai-0.0.42.tar", max compression
```

## Comparing `readmeai-0.0.41.tar` & `readmeai-0.0.42.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1063 2023-02-24 21:00:05.269166 readmeai-0.0.41/LICENSE
--rw-r--r--   0        0        0    17170 2023-07-30 08:11:06.017404 readmeai-0.0.41/README.md
--rw-r--r--   0        0        0     2592 2023-07-30 08:16:01.119909 readmeai-0.0.41/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-29 22:31:14.648662 readmeai-0.0.41/readmeai/__init__.py
--rw-r--r--   0        0        0     7710 2023-07-30 07:59:46.235795 readmeai-0.0.41/readmeai/builder.py
--rw-r--r--   0        0        0     6386 2023-07-30 08:00:06.148124 readmeai-0.0.41/readmeai/conf.py
--rw-r--r--   0        0        0     4893 2023-07-30 06:35:33.099524 readmeai-0.0.41/readmeai/factory.py
--rw-r--r--   0        0        0     1722 2023-07-29 22:31:14.649620 readmeai-0.0.41/readmeai/logger.py
--rwxr-xr-x   0        0        0     3844 2023-07-30 07:59:46.240097 readmeai-0.0.41/readmeai/main.py
--rw-r--r--   0        0        0     7600 2023-07-30 07:59:46.233890 readmeai-0.0.41/readmeai/model.py
--rw-r--r--   0        0        0     7270 2023-07-30 07:59:46.238156 readmeai-0.0.41/readmeai/parse.py
--rw-r--r--   0        0        0     6584 2023-07-30 08:15:34.644580 readmeai-0.0.41/readmeai/preprocess.py
--rw-r--r--   0        0        0     4039 2023-07-30 08:00:15.629149 readmeai-0.0.41/readmeai/utils.py
--rw-r--r--   0        0        0    18986 1970-01-01 00:00:00.000000 readmeai-0.0.41/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-02-24 21:00:05.269166 readmeai-0.0.42/LICENSE
+-rw-r--r--   0        0        0    17170 2023-07-30 08:11:06.017404 readmeai-0.0.42/README.md
+-rw-r--r--   0        0        0     2638 2023-07-30 08:19:12.255220 readmeai-0.0.42/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-29 22:31:14.648662 readmeai-0.0.42/readmeai/__init__.py
+-rw-r--r--   0        0        0     7710 2023-07-30 07:59:46.235795 readmeai-0.0.42/readmeai/builder.py
+-rw-r--r--   0        0        0     6386 2023-07-30 08:00:06.148124 readmeai-0.0.42/readmeai/conf.py
+-rw-r--r--   0        0        0     4893 2023-07-30 06:35:33.099524 readmeai-0.0.42/readmeai/factory.py
+-rw-r--r--   0        0        0     1722 2023-07-29 22:31:14.649620 readmeai-0.0.42/readmeai/logger.py
+-rwxr-xr-x   0        0        0     3844 2023-07-30 07:59:46.240097 readmeai-0.0.42/readmeai/main.py
+-rw-r--r--   0        0        0     7600 2023-07-30 07:59:46.233890 readmeai-0.0.42/readmeai/model.py
+-rw-r--r--   0        0        0     7270 2023-07-30 07:59:46.238156 readmeai-0.0.42/readmeai/parse.py
+-rw-r--r--   0        0        0     6542 2023-07-30 08:19:24.282555 readmeai-0.0.42/readmeai/preprocess.py
+-rw-r--r--   0        0        0     4039 2023-07-30 08:00:15.629149 readmeai-0.0.42/readmeai/utils.py
+-rw-r--r--   0        0        0    18986 1970-01-01 00:00:00.000000 readmeai-0.0.42/PKG-INFO
```

### Comparing `readmeai-0.0.41/LICENSE` & `readmeai-0.0.42/LICENSE`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.41/README.md` & `readmeai-0.0.42/README.md`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.41/pyproject.toml` & `readmeai-0.0.42/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "readmeai"
-version = "0.0.41"
+version = "0.0.42"
 description = """🚀 Generate awesome README.md files from the terminal, powered by OpenAI's GPT language model APIs 💫"""
 authors = ["Eli <0x.eli.64s@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/eli64s/readme-ai"
 documentation = "https://github.com/eli64s/readme-ai/blob/main/README.md"
 keywords = [
@@ -29,14 +29,17 @@
   "openai-python",
   "chatgpt-python",
   "openai-chatbot",
   "gpt-35-turbo",
   "gpt-4-api",
   "llm-agent"
 ]
+packages = [
+    { include = "readmeai/*" }
+]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 black = "^23.3.0"
 colorlog = "^6.7.0"
 cachetools = "^5.3.1"
 dacite = "^1.8.1"
```

### Comparing `readmeai-0.0.41/readmeai/builder.py` & `readmeai-0.0.42/readmeai/builder.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.41/readmeai/conf.py` & `readmeai-0.0.42/readmeai/conf.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.41/readmeai/factory.py` & `readmeai-0.0.42/readmeai/factory.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.41/readmeai/logger.py` & `readmeai-0.0.42/readmeai/logger.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.41/readmeai/main.py` & `readmeai-0.0.42/readmeai/main.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.41/readmeai/model.py` & `readmeai-0.0.42/readmeai/model.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.41/readmeai/parse.py` & `readmeai-0.0.42/readmeai/parse.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.41/readmeai/preprocess.py` & `readmeai-0.0.42/readmeai/preprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,9 @@
 """Handles preprocessing of the input codebase."""
 
-import sys
-
-
-sys.path.append("readmeai")
-
 import tempfile
 from pathlib import Path
 from typing import Dict, Generator, List, Tuple
 
 import parse
 import utils
```

### Comparing `readmeai-0.0.41/readmeai/utils.py` & `readmeai-0.0.42/readmeai/utils.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.41/PKG-INFO` & `readmeai-0.0.42/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readmeai
-Version: 0.0.41
+Version: 0.0.42
 Summary: 🚀 Generate awesome README.md files from the terminal, powered by OpenAI's GPT language model APIs 💫
 Home-page: https://github.com/eli64s/readme-ai
 License: MIT
 Keywords: markdown,readme,readme-template,shieldsio,readme-md,awesome-readme,readme-generator,gpt-3,openai-api,automated-readme,auto-readme,gpt-4,llms,awesome-chatgpt,openai-python,chatgpt-python,openai-chatbot,gpt-35-turbo,gpt-4-api,llm-agent
 Author: Eli
 Author-email: 0x.eli.64s@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
```

