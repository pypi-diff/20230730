# Comparing `tmp/readmeai-0.0.451.tar.gz` & `tmp/readmeai-0.0.452.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readmeai-0.0.451.tar", max compression
+gzip compressed data, was "readmeai-0.0.452.tar", max compression
```

## Comparing `readmeai-0.0.451.tar` & `readmeai-0.0.452.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1063 2023-02-24 21:00:05.269166 readmeai-0.0.451/LICENSE
--rw-r--r--   0        0        0    17201 2023-07-30 08:33:30.534503 readmeai-0.0.451/README.md
--rw-r--r--   0        0        0     2639 2023-07-30 08:47:15.779347 readmeai-0.0.451/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-29 22:31:14.648662 readmeai-0.0.451/readmeai/__init__.py
--rw-r--r--   0        0        0     7699 2023-07-30 08:47:06.328508 readmeai-0.0.451/readmeai/builder.py
--rw-r--r--   0        0        0     6343 2023-07-30 08:44:10.050885 readmeai-0.0.451/readmeai/conf.py
--rw-r--r--   0        0        0     4893 2023-07-30 06:35:33.099524 readmeai-0.0.451/readmeai/factory.py
--rw-r--r--   0        0        0     1722 2023-07-29 22:31:14.649620 readmeai-0.0.451/readmeai/logger.py
--rwxr-xr-x   0        0        0     3914 2023-07-30 08:47:05.920663 readmeai-0.0.451/readmeai/main.py
--rw-r--r--   0        0        0     7590 2023-07-30 08:47:03.763889 readmeai-0.0.451/readmeai/model.py
--rw-r--r--   0        0        0     7273 2023-07-30 08:34:53.114073 readmeai-0.0.451/readmeai/parse.py
--rw-r--r--   0        0        0     6536 2023-07-30 08:41:41.081277 readmeai-0.0.451/readmeai/preprocess.py
--rw-r--r--   0        0        0     3991 2023-07-30 08:41:30.482622 readmeai-0.0.451/readmeai/utils.py
--rw-r--r--   0        0        0    19018 1970-01-01 00:00:00.000000 readmeai-0.0.451/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-02-24 21:00:05.269166 readmeai-0.0.452/LICENSE
+-rw-r--r--   0        0        0    17201 2023-07-30 08:33:30.534503 readmeai-0.0.452/README.md
+-rw-r--r--   0        0        0     2639 2023-07-30 08:49:08.894158 readmeai-0.0.452/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-29 22:31:14.648662 readmeai-0.0.452/readmeai/__init__.py
+-rw-r--r--   0        0        0     7699 2023-07-30 08:47:06.328508 readmeai-0.0.452/readmeai/builder.py
+-rw-r--r--   0        0        0     6343 2023-07-30 08:44:10.050885 readmeai-0.0.452/readmeai/conf.py
+-rw-r--r--   0        0        0     4893 2023-07-30 06:35:33.099524 readmeai-0.0.452/readmeai/factory.py
+-rw-r--r--   0        0        0     1722 2023-07-29 22:31:14.649620 readmeai-0.0.452/readmeai/logger.py
+-rwxr-xr-x   0        0        0     3997 2023-07-30 08:48:59.042518 readmeai-0.0.452/readmeai/main.py
+-rw-r--r--   0        0        0     7590 2023-07-30 08:47:03.763889 readmeai-0.0.452/readmeai/model.py
+-rw-r--r--   0        0        0     7273 2023-07-30 08:34:53.114073 readmeai-0.0.452/readmeai/parse.py
+-rw-r--r--   0        0        0     6536 2023-07-30 08:41:41.081277 readmeai-0.0.452/readmeai/preprocess.py
+-rw-r--r--   0        0        0     3991 2023-07-30 08:41:30.482622 readmeai-0.0.452/readmeai/utils.py
+-rw-r--r--   0        0        0    19018 1970-01-01 00:00:00.000000 readmeai-0.0.452/PKG-INFO
```

### Comparing `readmeai-0.0.451/LICENSE` & `readmeai-0.0.452/LICENSE`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.451/README.md` & `readmeai-0.0.452/README.md`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.451/pyproject.toml` & `readmeai-0.0.452/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "readmeai"
-version = "0.0.451"
+version = "0.0.452"
 description = """🚀 Generate awesome README.md files from the terminal, powered by OpenAI's GPT language model APIs 💫"""
 authors = ["Eli <0x.eli.64s@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/eli64s/readme-ai"
 documentation = "https://github.com/eli64s/readme-ai/blob/main/README.md"
 keywords = [
```

### Comparing `readmeai-0.0.451/readmeai/builder.py` & `readmeai-0.0.452/readmeai/builder.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.451/readmeai/conf.py` & `readmeai-0.0.452/readmeai/conf.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.451/readmeai/factory.py` & `readmeai-0.0.452/readmeai/factory.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.451/readmeai/logger.py` & `readmeai-0.0.452/readmeai/logger.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.451/readmeai/main.py` & `readmeai-0.0.452/readmeai/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 import asyncio
 import os
-from typing import Dict, List, Tuple
+from typing import Dict, List, Optional, Tuple
 
 import click
 
 from . import builder, conf, logger, model, preprocess
 
 
 logger = logger.Logger(__name__)
@@ -114,15 +114,21 @@
     help="Template to use for README.md file.",
 )
 @click.option(
     "-l",
     "--language",
     help="Language to write README.md file in.",
 )
-def cli(api_key: str, output: str, repository: str) -> None:
+def cli(
+    api_key: str,
+    output: str,
+    repository: str,
+    template: Optional[int],
+    language: Optional[str],
+) -> None:
     """Cli entrypoint for readme-ai pypi package."""
     logger.info("README-AI is now executing.")
     asyncio.run(main(api_key, output, repository))
     logger.info("README-AI execution complete.\n")
 
 
 if __name__ == "__main__":
```

### Comparing `readmeai-0.0.451/readmeai/model.py` & `readmeai-0.0.452/readmeai/model.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.451/readmeai/parse.py` & `readmeai-0.0.452/readmeai/parse.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.451/readmeai/preprocess.py` & `readmeai-0.0.452/readmeai/preprocess.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.451/readmeai/utils.py` & `readmeai-0.0.452/readmeai/utils.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.451/PKG-INFO` & `readmeai-0.0.452/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readmeai
-Version: 0.0.451
+Version: 0.0.452
 Summary: 🚀 Generate awesome README.md files from the terminal, powered by OpenAI's GPT language model APIs 💫
 Home-page: https://github.com/eli64s/readme-ai
 License: MIT
 Keywords: markdown,readme,readme-template,shieldsio,readme-md,awesome-readme,readme-generator,gpt-3,openai-api,automated-readme,auto-readme,gpt-4,llms,awesome-chatgpt,openai-python,chatgpt-python,openai-chatbot,gpt-35-turbo,gpt-4-api,llm-agent
 Author: Eli
 Author-email: 0x.eli.64s@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
```

