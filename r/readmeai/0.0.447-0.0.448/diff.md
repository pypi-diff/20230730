# Comparing `tmp/readmeai-0.0.447.tar.gz` & `tmp/readmeai-0.0.448.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readmeai-0.0.447.tar", max compression
+gzip compressed data, was "readmeai-0.0.448.tar", max compression
```

## Comparing `readmeai-0.0.447.tar` & `readmeai-0.0.448.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1063 2023-02-24 21:00:05.269166 readmeai-0.0.447/LICENSE
--rw-r--r--   0        0        0    17170 2023-07-30 08:11:06.017404 readmeai-0.0.447/README.md
--rw-r--r--   0        0        0     2639 2023-07-30 08:28:32.875495 readmeai-0.0.447/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-29 22:31:14.648662 readmeai-0.0.447/readmeai/__init__.py
--rw-r--r--   0        0        0     7710 2023-07-30 07:59:46.235795 readmeai-0.0.447/readmeai/builder.py
--rw-r--r--   0        0        0     6386 2023-07-30 08:00:06.148124 readmeai-0.0.447/readmeai/conf.py
--rw-r--r--   0        0        0     4893 2023-07-30 06:35:33.099524 readmeai-0.0.447/readmeai/factory.py
--rw-r--r--   0        0        0     1722 2023-07-29 22:31:14.649620 readmeai-0.0.447/readmeai/logger.py
--rwxr-xr-x   0        0        0     3844 2023-07-30 08:28:29.866695 readmeai-0.0.447/readmeai/main.py
--rw-r--r--   0        0        0     7600 2023-07-30 07:59:46.233890 readmeai-0.0.447/readmeai/model.py
--rw-r--r--   0        0        0     7273 2023-07-30 08:23:48.177118 readmeai-0.0.447/readmeai/parse.py
--rw-r--r--   0        0        0     6556 2023-07-30 08:24:47.745492 readmeai-0.0.447/readmeai/preprocess.py
--rw-r--r--   0        0        0     4039 2023-07-30 08:00:15.629149 readmeai-0.0.447/readmeai/utils.py
--rw-r--r--   0        0        0    18987 1970-01-01 00:00:00.000000 readmeai-0.0.447/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-02-24 21:00:05.269166 readmeai-0.0.448/LICENSE
+-rw-r--r--   0        0        0    17170 2023-07-30 08:11:06.017404 readmeai-0.0.448/README.md
+-rw-r--r--   0        0        0     2639 2023-07-30 08:29:33.901789 readmeai-0.0.448/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-29 22:31:14.648662 readmeai-0.0.448/readmeai/__init__.py
+-rw-r--r--   0        0        0     7710 2023-07-30 07:59:46.235795 readmeai-0.0.448/readmeai/builder.py
+-rw-r--r--   0        0        0     6381 2023-07-30 08:29:23.003330 readmeai-0.0.448/readmeai/conf.py
+-rw-r--r--   0        0        0     4893 2023-07-30 06:35:33.099524 readmeai-0.0.448/readmeai/factory.py
+-rw-r--r--   0        0        0     1722 2023-07-29 22:31:14.649620 readmeai-0.0.448/readmeai/logger.py
+-rwxr-xr-x   0        0        0     3844 2023-07-30 08:28:29.866695 readmeai-0.0.448/readmeai/main.py
+-rw-r--r--   0        0        0     7600 2023-07-30 07:59:46.233890 readmeai-0.0.448/readmeai/model.py
+-rw-r--r--   0        0        0     7273 2023-07-30 08:23:48.177118 readmeai-0.0.448/readmeai/parse.py
+-rw-r--r--   0        0        0     6556 2023-07-30 08:24:47.745492 readmeai-0.0.448/readmeai/preprocess.py
+-rw-r--r--   0        0        0     4039 2023-07-30 08:00:15.629149 readmeai-0.0.448/readmeai/utils.py
+-rw-r--r--   0        0        0    18987 1970-01-01 00:00:00.000000 readmeai-0.0.448/PKG-INFO
```

### Comparing `readmeai-0.0.447/LICENSE` & `readmeai-0.0.448/LICENSE`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.447/README.md` & `readmeai-0.0.448/README.md`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.447/pyproject.toml` & `readmeai-0.0.448/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "readmeai"
-version = "0.0.447"
+version = "0.0.448"
 description = """🚀 Generate awesome README.md files from the terminal, powered by OpenAI's GPT language model APIs 💫"""
 authors = ["Eli <0x.eli.64s@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/eli64s/readme-ai"
 documentation = "https://github.com/eli64s/readme-ai/blob/main/README.md"
 keywords = [
```

### Comparing `readmeai-0.0.447/readmeai/builder.py` & `readmeai-0.0.448/readmeai/builder.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.447/readmeai/conf.py` & `readmeai-0.0.448/readmeai/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,13 +222,13 @@
     return handler.read(path)
 
 
 def load_config(path: str = "conf.toml") -> AppConfig:
     """Load configuration constants from TOML file."""
     handler = FileHandler()
     conf_dict = _get_config_dict(handler, path)
-    return AppConfigModel.model_validate({"app": conf_dict}).app
+    return AppConfigModel.parse_obj({"app": conf_dict}).app
 
 
 def load_config_helper(conf: AppConfigModel) -> ConfigHelper:
     """Load multiple configuration helper TOML files."""
     return ConfigHelper(conf=conf)
```

### Comparing `readmeai-0.0.447/readmeai/factory.py` & `readmeai-0.0.448/readmeai/factory.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.447/readmeai/logger.py` & `readmeai-0.0.448/readmeai/logger.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.447/readmeai/main.py` & `readmeai-0.0.448/readmeai/main.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.447/readmeai/model.py` & `readmeai-0.0.448/readmeai/model.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.447/readmeai/parse.py` & `readmeai-0.0.448/readmeai/parse.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.447/readmeai/preprocess.py` & `readmeai-0.0.448/readmeai/preprocess.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.447/readmeai/utils.py` & `readmeai-0.0.448/readmeai/utils.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.447/PKG-INFO` & `readmeai-0.0.448/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readmeai
-Version: 0.0.447
+Version: 0.0.448
 Summary: 🚀 Generate awesome README.md files from the terminal, powered by OpenAI's GPT language model APIs 💫
 Home-page: https://github.com/eli64s/readme-ai
 License: MIT
 Keywords: markdown,readme,readme-template,shieldsio,readme-md,awesome-readme,readme-generator,gpt-3,openai-api,automated-readme,auto-readme,gpt-4,llms,awesome-chatgpt,openai-python,chatgpt-python,openai-chatbot,gpt-35-turbo,gpt-4-api,llm-agent
 Author: Eli
 Author-email: 0x.eli.64s@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
```

