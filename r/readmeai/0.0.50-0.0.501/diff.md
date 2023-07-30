# Comparing `tmp/readmeai-0.0.50.tar.gz` & `tmp/readmeai-0.0.501.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readmeai-0.0.50.tar", max compression
+gzip compressed data, was "readmeai-0.0.501.tar", max compression
```

## Comparing `readmeai-0.0.50.tar` & `readmeai-0.0.501.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1063 2023-02-24 21:00:05.269166 readmeai-0.0.50/LICENSE
--rw-r--r--   0        0        0    17599 2023-07-30 09:44:18.539250 readmeai-0.0.50/README.md
--rw-r--r--   0        0        0     2469 2023-07-30 09:49:16.030425 readmeai-0.0.50/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-29 22:31:14.648662 readmeai-0.0.50/readmeai/__init__.py
--rw-r--r--   0        0        0     7699 2023-07-30 08:47:06.328508 readmeai-0.0.50/readmeai/builder.py
--rw-r--r--   0        0        0     6343 2023-07-30 08:44:10.050885 readmeai-0.0.50/readmeai/conf.py
--rw-r--r--   0        0        0     4893 2023-07-30 06:35:33.099524 readmeai-0.0.50/readmeai/factory.py
--rw-r--r--   0        0        0     1722 2023-07-29 22:31:14.649620 readmeai-0.0.50/readmeai/logger.py
--rwxr-xr-x   0        0        0     3997 2023-07-30 08:48:59.042518 readmeai-0.0.50/readmeai/main.py
--rw-r--r--   0        0        0     7590 2023-07-30 08:47:03.763889 readmeai-0.0.50/readmeai/model.py
--rw-r--r--   0        0        0     7273 2023-07-30 08:34:53.114073 readmeai-0.0.50/readmeai/parse.py
--rw-r--r--   0        0        0     6536 2023-07-30 08:41:41.081277 readmeai-0.0.50/readmeai/preprocess.py
--rw-r--r--   0        0        0     3991 2023-07-30 08:41:30.482622 readmeai-0.0.50/readmeai/utils.py
--rw-r--r--   0        0        0    19131 1970-01-01 00:00:00.000000 readmeai-0.0.50/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-02-24 21:00:05.269166 readmeai-0.0.501/LICENSE
+-rw-r--r--   0        0        0    17599 2023-07-30 09:44:18.539250 readmeai-0.0.501/README.md
+-rw-r--r--   0        0        0     2026 2023-07-30 10:11:39.209838 readmeai-0.0.501/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-29 22:31:14.648662 readmeai-0.0.501/readmeai/__init__.py
+-rw-r--r--   0        0        0     7699 2023-07-30 08:47:06.328508 readmeai-0.0.501/readmeai/builder.py
+-rw-r--r--   0        0        0     6343 2023-07-30 08:44:10.050885 readmeai-0.0.501/readmeai/conf.py
+-rw-r--r--   0        0        0     4893 2023-07-30 06:35:33.099524 readmeai-0.0.501/readmeai/factory.py
+-rw-r--r--   0        0        0     1722 2023-07-29 22:31:14.649620 readmeai-0.0.501/readmeai/logger.py
+-rwxr-xr-x   0        0        0     3997 2023-07-30 08:48:59.042518 readmeai-0.0.501/readmeai/main.py
+-rw-r--r--   0        0        0     7590 2023-07-30 08:47:03.763889 readmeai-0.0.501/readmeai/model.py
+-rw-r--r--   0        0        0     7273 2023-07-30 08:34:53.114073 readmeai-0.0.501/readmeai/parse.py
+-rw-r--r--   0        0        0     6536 2023-07-30 08:41:41.081277 readmeai-0.0.501/readmeai/preprocess.py
+-rw-r--r--   0        0        0     3991 2023-07-30 08:41:30.482622 readmeai-0.0.501/readmeai/utils.py
+-rw-r--r--   0        0        0    19132 1970-01-01 00:00:00.000000 readmeai-0.0.501/PKG-INFO
```

### Comparing `readmeai-0.0.50/LICENSE` & `readmeai-0.0.501/LICENSE`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.50/README.md` & `readmeai-0.0.501/README.md`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.50/pyproject.toml` & `readmeai-0.0.501/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "readmeai"
-version = "0.0.50"
+version = "0.0.501"
 description = "🚀 Generate awesome README.md files from the terminal, powered by OpenAI's GPT language model APIs 💫"
 authors = ["Eli <0x.eli.64s@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/eli64s/readme-ai"
 documentation = "https://github.com/eli64s/readme-ai/blob/main/README.md"
 keywords = [
@@ -63,15 +63,15 @@
 click = "^8.1.6"
 
 [tool.poetry.scripts]
 readmeai = "readmeai.main:cli"
 
 [tool.ruff]
 line-length = 88
-target-version = "py38"
+target-version = "py39"
 extend-select = [
   "I", # isort
   "N", # pep8-naming
   "UP", # pyupgrade
   "RUF", # ruff
   "B", # flake8-bugbear
   "C4", # flake8-comprehensions
@@ -84,45 +84,14 @@
 [tool.ruff.isort]
 force-sort-within-sections = true
 split-on-trailing-comma = false
 
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all"
 
-# Black
-[tool.black]
-target-version = ["py38", "py39", "py310"]
-line-length = 88
-include = '\.pyi?$'
-exclude = '''
-/(
-      .eggs
-    | .git
-    | .hg
-    | .mypy_cache
-    | .pytest_cache
-    | .tox
-    | venv
-    | benchmarks
-    | _build
-    | buck-out
-    | build
-    | dist
-  )/
-'''
-
-# iSort
-[tool.isort]
-profile = "black"
-line_length = 88
-lines_after_imports = 2
-multi_line_output = 3
-include_trailing_comma = true
-virtual_env = "conda"
-
 # Pytest
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 python_files = "test_*.py"
 addopts = "--strict-markers --disable-pytest-warnings"
 
 # Pytest Coverage
```

### Comparing `readmeai-0.0.50/readmeai/builder.py` & `readmeai-0.0.501/readmeai/builder.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.50/readmeai/conf.py` & `readmeai-0.0.501/readmeai/conf.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.50/readmeai/factory.py` & `readmeai-0.0.501/readmeai/factory.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.50/readmeai/logger.py` & `readmeai-0.0.501/readmeai/logger.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.50/readmeai/main.py` & `readmeai-0.0.501/readmeai/main.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.50/readmeai/model.py` & `readmeai-0.0.501/readmeai/model.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.50/readmeai/parse.py` & `readmeai-0.0.501/readmeai/parse.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.50/readmeai/preprocess.py` & `readmeai-0.0.501/readmeai/preprocess.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.50/readmeai/utils.py` & `readmeai-0.0.501/readmeai/utils.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.50/PKG-INFO` & `readmeai-0.0.501/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readmeai
-Version: 0.0.50
+Version: 0.0.501
 Summary: 🚀 Generate awesome README.md files from the terminal, powered by OpenAI's GPT language model APIs 💫
 Home-page: https://github.com/eli64s/readme-ai
 License: MIT
 Keywords: markdown,readme,readme-template,shieldsio,readme-md,awesome-readme,readme-generator,gpt-3,openai-api,automated-readme,auto-readme,gpt-4,llms,awesome-chatgpt,openai-python,chatgpt-python,openai-chatbot,gpt-35-turbo,gpt-4-api,llm-agent
 Author: Eli
 Author-email: 0x.eli.64s@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
```

