# Comparing `tmp/readmeai-0.0.444.tar.gz` & `tmp/readmeai-0.0.445.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readmeai-0.0.444.tar", max compression
+gzip compressed data, was "readmeai-0.0.445.tar", max compression
```

## Comparing `readmeai-0.0.444.tar` & `readmeai-0.0.445.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1063 2023-02-24 21:00:05.269166 readmeai-0.0.444/LICENSE
--rw-r--r--   0        0        0    17170 2023-07-30 08:11:06.017404 readmeai-0.0.444/README.md
--rw-r--r--   0        0        0     2639 2023-07-30 08:23:57.537380 readmeai-0.0.444/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-29 22:31:14.648662 readmeai-0.0.444/readmeai/__init__.py
--rw-r--r--   0        0        0     7710 2023-07-30 07:59:46.235795 readmeai-0.0.444/readmeai/builder.py
--rw-r--r--   0        0        0     6386 2023-07-30 08:00:06.148124 readmeai-0.0.444/readmeai/conf.py
--rw-r--r--   0        0        0     4893 2023-07-30 06:35:33.099524 readmeai-0.0.444/readmeai/factory.py
--rw-r--r--   0        0        0     1722 2023-07-29 22:31:14.649620 readmeai-0.0.444/readmeai/logger.py
--rwxr-xr-x   0        0        0     3851 2023-07-30 08:21:51.752153 readmeai-0.0.444/readmeai/main.py
--rw-r--r--   0        0        0     7600 2023-07-30 07:59:46.233890 readmeai-0.0.444/readmeai/model.py
--rw-r--r--   0        0        0     7273 2023-07-30 08:23:48.177118 readmeai-0.0.444/readmeai/parse.py
--rw-r--r--   0        0        0     6549 2023-07-30 08:22:02.546694 readmeai-0.0.444/readmeai/preprocess.py
--rw-r--r--   0        0        0     4039 2023-07-30 08:00:15.629149 readmeai-0.0.444/readmeai/utils.py
--rw-r--r--   0        0        0    18987 1970-01-01 00:00:00.000000 readmeai-0.0.444/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-02-24 21:00:05.269166 readmeai-0.0.445/LICENSE
+-rw-r--r--   0        0        0    17170 2023-07-30 08:11:06.017404 readmeai-0.0.445/README.md
+-rw-r--r--   0        0        0     2639 2023-07-30 08:24:59.919988 readmeai-0.0.445/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-29 22:31:14.648662 readmeai-0.0.445/readmeai/__init__.py
+-rw-r--r--   0        0        0     7710 2023-07-30 07:59:46.235795 readmeai-0.0.445/readmeai/builder.py
+-rw-r--r--   0        0        0     6386 2023-07-30 08:00:06.148124 readmeai-0.0.445/readmeai/conf.py
+-rw-r--r--   0        0        0     4893 2023-07-30 06:35:33.099524 readmeai-0.0.445/readmeai/factory.py
+-rw-r--r--   0        0        0     1722 2023-07-29 22:31:14.649620 readmeai-0.0.445/readmeai/logger.py
+-rwxr-xr-x   0        0        0     3851 2023-07-30 08:24:54.522676 readmeai-0.0.445/readmeai/main.py
+-rw-r--r--   0        0        0     7600 2023-07-30 07:59:46.233890 readmeai-0.0.445/readmeai/model.py
+-rw-r--r--   0        0        0     7273 2023-07-30 08:23:48.177118 readmeai-0.0.445/readmeai/parse.py
+-rw-r--r--   0        0        0     6556 2023-07-30 08:24:47.745492 readmeai-0.0.445/readmeai/preprocess.py
+-rw-r--r--   0        0        0     4039 2023-07-30 08:00:15.629149 readmeai-0.0.445/readmeai/utils.py
+-rw-r--r--   0        0        0    18987 1970-01-01 00:00:00.000000 readmeai-0.0.445/PKG-INFO
```

### Comparing `readmeai-0.0.444/LICENSE` & `readmeai-0.0.445/LICENSE`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.444/README.md` & `readmeai-0.0.445/README.md`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.444/pyproject.toml` & `readmeai-0.0.445/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "readmeai"
-version = "0.0.444"
+version = "0.0.445"
 description = """🚀 Generate awesome README.md files from the terminal, powered by OpenAI's GPT language model APIs 💫"""
 authors = ["Eli <0x.eli.64s@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/eli64s/readme-ai"
 documentation = "https://github.com/eli64s/readme-ai/blob/main/README.md"
 keywords = [
```

### Comparing `readmeai-0.0.444/readmeai/builder.py` & `readmeai-0.0.445/readmeai/builder.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.444/readmeai/conf.py` & `readmeai-0.0.445/readmeai/conf.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.444/readmeai/factory.py` & `readmeai-0.0.445/readmeai/factory.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.444/readmeai/logger.py` & `readmeai-0.0.445/readmeai/logger.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.444/readmeai/main.py` & `readmeai-0.0.445/readmeai/main.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.444/readmeai/model.py` & `readmeai-0.0.445/readmeai/model.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.444/readmeai/parse.py` & `readmeai-0.0.445/readmeai/parse.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.444/readmeai/preprocess.py` & `readmeai-0.0.445/readmeai/preprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Handles preprocessing of the input codebase."""
 
 import tempfile
 from pathlib import Path
 from typing import Dict, Generator, List, Tuple
 
 from . import parse
-import utils
+from . import utils
 
 import conf
 
 
 class RepositoryParserWrapper:
     """Wrapper class for the RepositoryParser."""
```

### Comparing `readmeai-0.0.444/readmeai/utils.py` & `readmeai-0.0.445/readmeai/utils.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.444/PKG-INFO` & `readmeai-0.0.445/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readmeai
-Version: 0.0.444
+Version: 0.0.445
 Summary: 🚀 Generate awesome README.md files from the terminal, powered by OpenAI's GPT language model APIs 💫
 Home-page: https://github.com/eli64s/readme-ai
 License: MIT
 Keywords: markdown,readme,readme-template,shieldsio,readme-md,awesome-readme,readme-generator,gpt-3,openai-api,automated-readme,auto-readme,gpt-4,llms,awesome-chatgpt,openai-python,chatgpt-python,openai-chatbot,gpt-35-turbo,gpt-4-api,llm-agent
 Author: Eli
 Author-email: 0x.eli.64s@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
```

