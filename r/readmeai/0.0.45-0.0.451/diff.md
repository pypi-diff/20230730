# Comparing `tmp/readmeai-0.0.45.tar.gz` & `tmp/readmeai-0.0.451.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readmeai-0.0.45.tar", max compression
+gzip compressed data, was "readmeai-0.0.451.tar", max compression
```

## Comparing `readmeai-0.0.45.tar` & `readmeai-0.0.451.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1063 2023-02-24 21:00:05.269166 readmeai-0.0.45/LICENSE
--rw-r--r--   0        0        0    17201 2023-07-30 08:33:30.534503 readmeai-0.0.45/README.md
--rw-r--r--   0        0        0     2638 2023-07-30 08:34:27.815681 readmeai-0.0.45/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-29 22:31:14.648662 readmeai-0.0.45/readmeai/__init__.py
--rw-r--r--   0        0        0     7693 2023-07-30 08:45:23.635493 readmeai-0.0.45/readmeai/builder.py
--rw-r--r--   0        0        0     6343 2023-07-30 08:44:10.050885 readmeai-0.0.45/readmeai/conf.py
--rw-r--r--   0        0        0     4893 2023-07-30 06:35:33.099524 readmeai-0.0.45/readmeai/factory.py
--rw-r--r--   0        0        0     1722 2023-07-29 22:31:14.649620 readmeai-0.0.45/readmeai/logger.py
--rwxr-xr-x   0        0        0     3908 2023-07-30 08:43:12.722604 readmeai-0.0.45/readmeai/main.py
--rw-r--r--   0        0        0     7607 2023-07-30 08:41:52.478677 readmeai-0.0.45/readmeai/model.py
--rw-r--r--   0        0        0     7273 2023-07-30 08:34:53.114073 readmeai-0.0.45/readmeai/parse.py
--rw-r--r--   0        0        0     6536 2023-07-30 08:41:41.081277 readmeai-0.0.45/readmeai/preprocess.py
--rw-r--r--   0        0        0     3991 2023-07-30 08:41:30.482622 readmeai-0.0.45/readmeai/utils.py
--rw-r--r--   0        0        0    19017 1970-01-01 00:00:00.000000 readmeai-0.0.45/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-02-24 21:00:05.269166 readmeai-0.0.451/LICENSE
+-rw-r--r--   0        0        0    17201 2023-07-30 08:33:30.534503 readmeai-0.0.451/README.md
+-rw-r--r--   0        0        0     2639 2023-07-30 08:47:15.779347 readmeai-0.0.451/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-29 22:31:14.648662 readmeai-0.0.451/readmeai/__init__.py
+-rw-r--r--   0        0        0     7699 2023-07-30 08:47:06.328508 readmeai-0.0.451/readmeai/builder.py
+-rw-r--r--   0        0        0     6343 2023-07-30 08:44:10.050885 readmeai-0.0.451/readmeai/conf.py
+-rw-r--r--   0        0        0     4893 2023-07-30 06:35:33.099524 readmeai-0.0.451/readmeai/factory.py
+-rw-r--r--   0        0        0     1722 2023-07-29 22:31:14.649620 readmeai-0.0.451/readmeai/logger.py
+-rwxr-xr-x   0        0        0     3914 2023-07-30 08:47:05.920663 readmeai-0.0.451/readmeai/main.py
+-rw-r--r--   0        0        0     7590 2023-07-30 08:47:03.763889 readmeai-0.0.451/readmeai/model.py
+-rw-r--r--   0        0        0     7273 2023-07-30 08:34:53.114073 readmeai-0.0.451/readmeai/parse.py
+-rw-r--r--   0        0        0     6536 2023-07-30 08:41:41.081277 readmeai-0.0.451/readmeai/preprocess.py
+-rw-r--r--   0        0        0     3991 2023-07-30 08:41:30.482622 readmeai-0.0.451/readmeai/utils.py
+-rw-r--r--   0        0        0    19018 1970-01-01 00:00:00.000000 readmeai-0.0.451/PKG-INFO
```

### Comparing `readmeai-0.0.45/LICENSE` & `readmeai-0.0.451/LICENSE`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.45/README.md` & `readmeai-0.0.451/README.md`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.45/pyproject.toml` & `readmeai-0.0.451/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "readmeai"
-version = "0.0.45"
+version = "0.0.451"
 description = """🚀 Generate awesome README.md files from the terminal, powered by OpenAI's GPT language model APIs 💫"""
 authors = ["Eli <0x.eli.64s@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/eli64s/readme-ai"
 documentation = "https://github.com/eli64s/readme-ai/blob/main/README.md"
 keywords = [
```

### Comparing `readmeai-0.0.45/readmeai/builder.py` & `readmeai-0.0.451/readmeai/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Builds the README Markdown file for your codebase."""
 
 import subprocess
 import tempfile
 from pathlib import Path
 from typing import List, Tuple
 
-from . import utils, factory, logger, conf
+from . import conf, factory, logger, utils
 
 
 LOGGER = logger.Logger(__name__)
 
 
 def build_markdown_file(
     conf: conf.AppConfig,
@@ -109,15 +109,17 @@
     """Formats the generated code summaries into a list."""
     summary_list = []
     for module, summary in summaries:
         summary_list.append((module, summary))
     return summary_list
 
 
-def create_setup_guide(conf: conf.AppConfig, helper: conf.ConfigHelper, summary_list: list):
+def create_setup_guide(
+    conf: conf.AppConfig, helper: conf.ConfigHelper, summary_list: list
+):
     """Creates the 'Getting Started' section of the README file."""
     try:
         default_install_command = (
             default_run_command
         ) = default_test_command = conf.md.default
 
         language_counts = {}
```

### Comparing `readmeai-0.0.45/readmeai/conf.py` & `readmeai-0.0.451/readmeai/conf.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.45/readmeai/factory.py` & `readmeai-0.0.451/readmeai/factory.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.45/readmeai/logger.py` & `readmeai-0.0.451/readmeai/logger.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.45/readmeai/main.py` & `readmeai-0.0.451/readmeai/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,17 @@
     name: str, slogan: str, overview: str, features: str
 ) -> None:
     """Updates config.md.header and config.md.intro."""
     config.md.header = config.md.header.format(name, slogan)
     config.md.intro = config.md.intro.format(overview, features)
 
 
-async def generate_code_to_text(llm: model.OpenAIHandler, file_text: str) -> Dict[str, str]:
+async def generate_code_to_text(
+    llm: model.OpenAIHandler, file_text: str
+) -> Dict[str, str]:
     """Generates code_to_text using llm."""
     return await llm.code_to_text(
         config_helper.ignore_files, file_text, config.prompts.code_summary
     )
 
 
 async def generate_markdown_text(
```

### Comparing `readmeai-0.0.45/readmeai/model.py` & `readmeai-0.0.451/readmeai/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,32 +2,30 @@
 
 import asyncio
 import time
 from typing import Dict, List, Tuple
 
 import httpx
 import openai
-import utils
 from cachetools import TTLCache
-from logger import Logger
 from tenacity import (
     RetryError,
     retry,
     retry_if_exception_type,
     stop_after_attempt,
     wait_exponential,
 )
 
-from . import conf
+from . import conf, logger, utils
 
 
 class OpenAIHandler:
     """OpenAI API handler for generating text for the README.md file."""
 
-    logger = Logger(__name__)
+    logger = logger.Logger(__name__)
 
     def __init__(self, conf: conf.AppConfig):
         """Initialize the OpenAI API handler.
 
         Parameters
         ----------
         conf : conf.AppConfig
```

### Comparing `readmeai-0.0.45/readmeai/parse.py` & `readmeai-0.0.451/readmeai/parse.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.45/readmeai/preprocess.py` & `readmeai-0.0.451/readmeai/preprocess.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.45/readmeai/utils.py` & `readmeai-0.0.451/readmeai/utils.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.45/PKG-INFO` & `readmeai-0.0.451/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readmeai
-Version: 0.0.45
+Version: 0.0.451
 Summary: 🚀 Generate awesome README.md files from the terminal, powered by OpenAI's GPT language model APIs 💫
 Home-page: https://github.com/eli64s/readme-ai
 License: MIT
 Keywords: markdown,readme,readme-template,shieldsio,readme-md,awesome-readme,readme-generator,gpt-3,openai-api,automated-readme,auto-readme,gpt-4,llms,awesome-chatgpt,openai-python,chatgpt-python,openai-chatbot,gpt-35-turbo,gpt-4-api,llm-agent
 Author: Eli
 Author-email: 0x.eli.64s@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
```

