# Comparing `tmp/HandyLLM-0.3.1.tar.gz` & `tmp/HandyLLM-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HandyLLM-0.3.1.tar", last modified: Sat Jul 29 07:09:42 2023, max compression
+gzip compressed data, was "HandyLLM-0.4.0.tar", last modified: Sat Jul 29 17:10:39 2023, max compression
```

## Comparing `HandyLLM-0.3.1.tar` & `HandyLLM-0.4.0.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:09:42.501543 HandyLLM-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-07-29 07:09:42.501543 HandyLLM-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-29 07:09:33.000000 HandyLLM-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-29 07:09:33.000000 HandyLLM-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 07:09:42.501543 HandyLLM-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:09:42.497543 HandyLLM-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:09:42.497543 HandyLLM-0.3.1/src/HandyLLM.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-07-29 07:09:42.000000 HandyLLM-0.3.1/src/HandyLLM.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-29 07:09:42.000000 HandyLLM-0.3.1/src/HandyLLM.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 07:09:42.000000 HandyLLM-0.3.1/src/HandyLLM.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-29 07:09:42.000000 HandyLLM-0.3.1/src/HandyLLM.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-29 07:09:42.000000 HandyLLM-0.3.1/src/HandyLLM.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:09:42.497543 HandyLLM-0.3.1/src/handyllm/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-29 07:09:33.000000 HandyLLM-0.3.1/src/handyllm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-29 07:09:33.000000 HandyLLM-0.3.1/src/handyllm/endpoint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    17536 2023-07-29 07:09:33.000000 HandyLLM-0.3.1/src/handyllm/openai_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-07-29 07:09:33.000000 HandyLLM-0.3.1/src/handyllm/prompt_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-29 07:09:33.000000 HandyLLM-0.3.1/src/handyllm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:09:42.501543 HandyLLM-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-29 07:09:33.000000 HandyLLM-0.3.1/tests/test_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-29 07:09:33.000000 HandyLLM-0.3.1/tests/test_completions.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-29 07:09:33.000000 HandyLLM-0.3.1/tests/test_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-29 07:09:33.000000 HandyLLM-0.3.1/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-29 07:09:33.000000 HandyLLM-0.3.1/tests/test_images.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-29 07:09:33.000000 HandyLLM-0.3.1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-29 07:09:33.000000 HandyLLM-0.3.1/tests/test_moderation.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-29 07:09:33.000000 HandyLLM-0.3.1/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-29 07:09:33.000000 HandyLLM-0.3.1/tests/test_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:10:39.210416 HandyLLM-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-07-29 17:10:39.210416 HandyLLM-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-07-29 17:10:28.000000 HandyLLM-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-29 17:10:28.000000 HandyLLM-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 17:10:39.210416 HandyLLM-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:10:39.206416 HandyLLM-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:10:39.206416 HandyLLM-0.4.0/src/HandyLLM.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-07-29 17:10:39.000000 HandyLLM-0.4.0/src/HandyLLM.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-29 17:10:39.000000 HandyLLM-0.4.0/src/HandyLLM.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 17:10:39.000000 HandyLLM-0.4.0/src/HandyLLM.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-29 17:10:39.000000 HandyLLM-0.4.0/src/HandyLLM.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-29 17:10:39.000000 HandyLLM-0.4.0/src/HandyLLM.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:10:39.210416 HandyLLM-0.4.0/src/handyllm/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-29 17:10:28.000000 HandyLLM-0.4.0/src/handyllm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-29 17:10:28.000000 HandyLLM-0.4.0/src/handyllm/endpoint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21832 2023-07-29 17:10:28.000000 HandyLLM-0.4.0/src/handyllm/openai_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-07-29 17:10:28.000000 HandyLLM-0.4.0/src/handyllm/prompt_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-29 17:10:28.000000 HandyLLM-0.4.0/src/handyllm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:10:39.210416 HandyLLM-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-29 17:10:28.000000 HandyLLM-0.4.0/tests/test_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-29 17:10:28.000000 HandyLLM-0.4.0/tests/test_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-29 17:10:28.000000 HandyLLM-0.4.0/tests/test_completions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-29 17:10:28.000000 HandyLLM-0.4.0/tests/test_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-29 17:10:28.000000 HandyLLM-0.4.0/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-29 17:10:28.000000 HandyLLM-0.4.0/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-29 17:10:28.000000 HandyLLM-0.4.0/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-29 17:10:28.000000 HandyLLM-0.4.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-29 17:10:28.000000 HandyLLM-0.4.0/tests/test_moderation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-29 17:10:28.000000 HandyLLM-0.4.0/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-29 17:10:28.000000 HandyLLM-0.4.0/tests/test_stream.py
```

### Comparing `HandyLLM-0.3.1/PKG-INFO` & `HandyLLM-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HandyLLM
-Version: 0.3.1
+Version: 0.4.0
 Summary: A handy toolkit for using LLM.
 Author-email: Atomie CHEN <atomic_cwh@163.com>
 Project-URL: Homepage, https://github.com/atomiechen/HandyLLM
 Project-URL: Bug Tracker, https://github.com/atomiechen/HandyLLM/issues
 Keywords: LLM,Large Language Model,Prompt,OpenAI,API
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -37,15 +37,15 @@
 
 Example scripts are placed in [tests](./tests) folder.
 
 
 
 ## OpenAI API Request
 
-### Logs
+### Logger
 
 You can pass custom `logger` and `log_marks` (a string or a collection of strings) to `chat`/`completions` to get input and output logging.
 
 ### Timeout control
 
 This toolkit supports client-side `timeout` control:
 
@@ -120,14 +120,22 @@
 - finetunes_retrieve
 - finetunes_cancel
 - finetunes_list_events
 - finetunes_delete_model
 
 Please refer to [OpenAI official API reference](https://platform.openai.com/docs/api-reference) for details.
 
+### Azure
+
+**Azure OpenAI APIs are supported!** 
+
+Refer to [test_azure.py](./tests/test_azure.py) for example usage.
+
+Refer to [Azure OpenAI Service Documentation](https://learn.microsoft.com/en-us/azure/ai-services/openai/).
+
 
 
 ## Prompt
 
 ### Prompt Conversion
 
 `PromptConverter` can convert this text file `prompt.txt` into a structured prompt for chat API calls:
```

### Comparing `HandyLLM-0.3.1/README.md` & `HandyLLM-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 Example scripts are placed in [tests](./tests) folder.
 
 
 
 ## OpenAI API Request
 
-### Logs
+### Logger
 
 You can pass custom `logger` and `log_marks` (a string or a collection of strings) to `chat`/`completions` to get input and output logging.
 
 ### Timeout control
 
 This toolkit supports client-side `timeout` control:
 
@@ -107,14 +107,22 @@
 - finetunes_retrieve
 - finetunes_cancel
 - finetunes_list_events
 - finetunes_delete_model
 
 Please refer to [OpenAI official API reference](https://platform.openai.com/docs/api-reference) for details.
 
+### Azure
+
+**Azure OpenAI APIs are supported!** 
+
+Refer to [test_azure.py](./tests/test_azure.py) for example usage.
+
+Refer to [Azure OpenAI Service Documentation](https://learn.microsoft.com/en-us/azure/ai-services/openai/).
+
 
 
 ## Prompt
 
 ### Prompt Conversion
 
 `PromptConverter` can convert this text file `prompt.txt` into a structured prompt for chat API calls:
```

### Comparing `HandyLLM-0.3.1/pyproject.toml` & `HandyLLM-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HandyLLM"
-version = "0.3.1"
+version = "0.4.0"
 authors = [
   { name="Atomie CHEN", email="atomic_cwh@163.com" },
 ]
 description = "A handy toolkit for using LLM."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `HandyLLM-0.3.1/src/HandyLLM.egg-info/PKG-INFO` & `HandyLLM-0.4.0/src/HandyLLM.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HandyLLM
-Version: 0.3.1
+Version: 0.4.0
 Summary: A handy toolkit for using LLM.
 Author-email: Atomie CHEN <atomic_cwh@163.com>
 Project-URL: Homepage, https://github.com/atomiechen/HandyLLM
 Project-URL: Bug Tracker, https://github.com/atomiechen/HandyLLM/issues
 Keywords: LLM,Large Language Model,Prompt,OpenAI,API
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -37,15 +37,15 @@
 
 Example scripts are placed in [tests](./tests) folder.
 
 
 
 ## OpenAI API Request
 
-### Logs
+### Logger
 
 You can pass custom `logger` and `log_marks` (a string or a collection of strings) to `chat`/`completions` to get input and output logging.
 
 ### Timeout control
 
 This toolkit supports client-side `timeout` control:
 
@@ -120,14 +120,22 @@
 - finetunes_retrieve
 - finetunes_cancel
 - finetunes_list_events
 - finetunes_delete_model
 
 Please refer to [OpenAI official API reference](https://platform.openai.com/docs/api-reference) for details.
 
+### Azure
+
+**Azure OpenAI APIs are supported!** 
+
+Refer to [test_azure.py](./tests/test_azure.py) for example usage.
+
+Refer to [Azure OpenAI Service Documentation](https://learn.microsoft.com/en-us/azure/ai-services/openai/).
+
 
 
 ## Prompt
 
 ### Prompt Conversion
 
 `PromptConverter` can convert this text file `prompt.txt` into a structured prompt for chat API calls:
```

### Comparing `HandyLLM-0.3.1/src/HandyLLM.egg-info/SOURCES.txt` & `HandyLLM-0.4.0/src/HandyLLM.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 src/HandyLLM.egg-info/top_level.txt
 src/handyllm/__init__.py
 src/handyllm/endpoint_manager.py
 src/handyllm/openai_api.py
 src/handyllm/prompt_converter.py
 src/handyllm/utils.py
 tests/test_audio.py
+tests/test_azure.py
 tests/test_completions.py
 tests/test_embedding.py
 tests/test_files.py
 tests/test_images.py
+tests/test_logger.py
 tests/test_models.py
 tests/test_moderation.py
 tests/test_prompt.py
 tests/test_stream.py
```

### Comparing `HandyLLM-0.3.1/src/handyllm/endpoint_manager.py` & `HandyLLM-0.4.0/src/handyllm/endpoint_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,37 +34,37 @@
         self._keys = [key for key in keys if isinstance(key, str) and key.strip() != '']
         
     def set_organizations(self, organizations):
         self._organizations = [organization for organization in organizations if isinstance(organization, str) and organization.strip() != '']
 
     def get_base_url(self):
         if len(self._base_urls) == 0:
-            return OpenAIAPI.base_url
+            return OpenAIAPI.get_api_base()
         else:
             base_url = self._base_urls[self._last_idx_url]
             if self._last_idx_url == len(self._base_urls) - 1:
                 self._last_idx_url = 0
             else:
                 self._last_idx_url += 1
             return base_url
 
     def get_key(self):
         if len(self._keys) == 0:
-            return OpenAIAPI.api_key
+            return OpenAIAPI.get_api_key()
         else:
             key = self._keys[self._last_idx_key]
             if self._last_idx_key == len(self._keys) - 1:
                 self._last_idx_key = 0
             else:
                 self._last_idx_key += 1
             return key
     
     def get_organization(self):
         if len(self._organizations) == 0:
-            return OpenAIAPI.organization
+            return OpenAIAPI.get_organization()
         else:
             organization = self._organizations[self._last_idx_organization]
             if self._last_idx_organization == len(self._keys) - 1:
                 self._last_idx_organization = 0
             else:
                 self._last_idx_organization += 1
             return organization
```

### Comparing `HandyLLM-0.3.1/src/handyllm/openai_api.py` & `HandyLLM-0.4.0/src/handyllm/openai_api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,76 +1,132 @@
 import os
 import time
+from urllib.parse import quote_plus
 import requests
 import logging
 import json
 import copy
 
 from .prompt_converter import PromptConverter
 from . import utils
 
+_API_BASE_OPENAI = 'https://api.openai.com/v1'
+_API_TYPE_OPENAI = 'openai'
+_API_TYPES_AZURE = (
+    'azure', 
+    'azure_ad', 
+    'azuread'
+)
+_API_VERSION_AZURE = '2023-05-15'
+
 module_logger = logging.getLogger(__name__)
 
 class OpenAIAPI:
     
-    base_url = "https://api.openai.com/v1"
+    # deprecated
+    base_url = _API_BASE_OPENAI
+    
+    # set this to your API base;
+    # or environment variable OPENAI_API_BASE will be used.
+    # can be None (roll back to default).
+    api_base = None
     
     # set this to your API key; 
     # or environment variable OPENAI_API_KEY will be used.
     api_key = None
     
     # set this to your organization ID; 
     # or environment variable OPENAI_ORGANIZATION will be used;
     # can be None.
     organization = None
     
-    converter = PromptConverter()
+    # set this to your API type;
+    # or environment variable OPENAI_API_TYPE will be used;
+    # can be None (roll back to default).
+    api_type = None
     
-    @staticmethod
-    def _get_key_from_env():
-        return os.environ.get('OPENAI_API_KEY')
+    # set this to your API version;
+    # or environment variable OPENAI_API_VERSION will be used;
+    # can be None.
+    api_version = None
     
-    @staticmethod
-    def _get_organization_from_env():
-        return os.environ.get('OPENAI_ORGANIZATION')
+    converter = PromptConverter()
+    
+    @classmethod
+    def get_api_key(cls, api_key=None):
+        if not api_key:
+            api_key = cls.api_key if cls.api_key else os.environ.get('OPENAI_API_KEY')
+        return api_key
+    
+    @classmethod
+    def get_organization(cls, organization=None):
+        if not organization:
+            organization = cls.organization if cls.organization else os.environ.get('OPENAI_ORGANIZATION')
+        return organization
+    
+    @classmethod
+    def get_api_base(cls, api_base=None):
+        if not api_base:
+            api_base = cls.api_base if cls.api_base else os.environ.get('OPENAI_API_BASE')
+            if not api_base:
+                api_base = _API_BASE_OPENAI
+        return api_base
+    
+    @classmethod
+    def get_api_type_and_version(cls, api_type=None, api_version=None):
+        if not api_type:
+            api_type = cls.api_type if cls.api_type else os.environ.get('OPENAI_API_TYPE')
+            if not api_type:
+                api_type = _API_TYPE_OPENAI
+        if not api_version:
+            api_version = cls.api_version if cls.api_version else os.environ.get('OPENAI_API_VERSION')
+            if not api_version and api_type and api_type.lower() in _API_TYPES_AZURE:
+                api_version = _API_VERSION_AZURE
+        return api_type, api_version
 
     @staticmethod
-    def _api_request(url, api_key, organization=None, method='post', timeout=None, **kwargs):
+    def _api_request(url, api_key, organization=None, api_type=api_type, method='post', timeout=None, **kwargs):
         if api_key is None:
             raise Exception("OpenAI API key is not set")
         if url is None:
             raise Exception("OpenAI API url is not set")
+        if api_type is None:
+            raise Exception("OpenAI API type is not set")
 
         ## log request info
         log_strs = []
-        # 避免直接打印api_key
+        # avoid logging the whole api_key
         plaintext_len = 8
         log_strs.append(f"API request {url}")
         log_strs.append(f"api_key: {api_key[:plaintext_len]}{'*'*(len(api_key)-plaintext_len)}")
         if organization is not None:
             log_strs.append(f"organization: {organization[:plaintext_len]}{'*'*(len(organization)-plaintext_len)}")
         log_strs.append(f"timeout: {timeout}")
         module_logger.info('\n'.join(log_strs))
 
         files = kwargs.pop('files', None)
         stream = kwargs.get('stream', False)
-        headers = { 'Authorization': 'Bearer ' + api_key }
+        headers = {}
         json_data = None
         data = None
-        params = None
+        params = {}
+        if api_type in _API_TYPES_AZURE:
+            headers['api-key'] = api_key
+        else:
+            headers['Authorization'] = 'Bearer ' + api_key
         if organization is not None:
             headers['OpenAI-Organization'] = organization
         if method == 'post':
             if files is None:
                 headers['Content-Type'] = 'application/json'
                 json_data = kwargs
             else:  ## if files is not None, let requests handle the content type
                 data = kwargs
         if method == 'get' and stream:
-            params = { "stream": "true" }
+            params['stream'] = 'true'
 
         response = requests.request(
             method,
             url,
             headers=headers,
             data=data,
             json=json_data,
@@ -101,127 +157,181 @@
                 if byte_line.strip() == b"data: [DONE]":
                     return
                 if byte_line.startswith(b"data: "):
                     line = byte_line[len(b"data: "):].decode("utf-8")
                     yield json.loads(line)
 
     @staticmethod
-    def stream_chat(response):
+    def stream_chat_with_role(response):
+        role = ''
         for data in response:
-            if 'content' in data['choices'][0]['delta']:
-                yield data['choices'][0]['delta']['content']
+            message = data['choices'][0]['delta']
+            if 'role' in message:
+                role = message['role']
+            if 'content' in message:
+                text = message['content']
+                yield role, text
+    
+    @staticmethod
+    def stream_chat(response):
+        for _, text in OpenAIAPI.stream_chat_with_role(response):
+            yield text
     
     @staticmethod
     def stream_completions(response):
         for data in response:
             yield data['choices'][0]['text']
     
-    @staticmethod
-    def api_request_endpoint(request_url, endpoint_manager=None, **kwargs):
-        specified_api_key = kwargs.pop('api_key', None)
-        specified_organization = kwargs.pop('organization', None)
+    @classmethod
+    def api_request_endpoint(
+        cls,
+        request_url, 
+        endpoint_manager=None, 
+        **kwargs
+        ):
+        api_key, organization, api_base, api_type, api_version, engine = cls.consume_kwargs(kwargs)
         if endpoint_manager != None:
-            # 每次换服务器和key要同时换，保证服务器和key是对应的
-            base_url, api_key, organization = endpoint_manager.get_endpoint()
+            api_base, api_key, organization = endpoint_manager.get_endpoint()
+        url = api_base.rstrip('/') + '/' + request_url.lstrip('/')
+        return cls._api_request(url, api_key, organization=organization, api_type=api_type, **kwargs)
+    
+    @classmethod
+    def consume_kwargs(cls, kwargs):
+        api_key = cls.get_api_key(kwargs.pop('api_key', None))
+        organization = cls.get_organization(kwargs.pop('organization', None))
+        api_base = cls.get_api_base(kwargs.pop('api_base', None))
+        api_type, api_version = cls.get_api_type_and_version(
+            kwargs.pop('api_type', None), 
+            kwargs.pop('api_version', None)
+        )
+        deployment_id = kwargs.pop('deployment_id', None)
+        engine = kwargs.pop('engine', deployment_id)
+        return api_key, organization, api_base, api_type, api_version, engine
+    
+    @classmethod
+    def chat(cls, messages, timeout=None, endpoint_manager=None, logger=None, log_marks=[], **kwargs):
+        api_key, organization, api_base, api_type, api_version, engine = cls.consume_kwargs(kwargs)
+        if api_type and api_type.lower() in _API_TYPES_AZURE:
+            if engine is None:
+                raise Exception("Azure API requires engine to be specified")
+            request_url = f'/openai/deployments/{quote_plus(engine)}/chat/completions?api-version={api_version}'
         else:
-            base_url = OpenAIAPI.base_url
-            if specified_api_key is not None:
-                api_key = specified_api_key
-            elif OpenAIAPI.api_key is not None:
-                api_key = OpenAIAPI.api_key
-            else:
-                api_key = OpenAIAPI._get_key_from_env()
-            if specified_organization is not None:
-                organization = specified_organization
-            elif OpenAIAPI.organization is not None:
-                organization = OpenAIAPI.organization 
+            if engine is not None:
+                request_url = f'/engines/{quote_plus(engine)}/chat/completions'
             else:
-                organization = OpenAIAPI._get_organization_from_env()
-        url = base_url + request_url
-        return OpenAIAPI._api_request(url, api_key, organization=organization, **kwargs)
-    
-    @staticmethod
-    def chat(model, messages, timeout=None, endpoint_manager=None, logger=None, log_marks=[], **kwargs):
-        request_url = '/chat/completions'
+                request_url = '/chat/completions'
 
-        if logger is not None and 'messages' in kwargs:
+        if logger is not None:
             arguments = copy.deepcopy(kwargs)
-            arguments.pop('messages', None)
             # check if log_marks is iterable
             if utils.isiterable(log_marks):
                 input_lines = [str(item) for item in log_marks]
             else:
                 input_lines = [str(log_marks)]
             input_lines.append(json.dumps(arguments, indent=2, ensure_ascii=False))
             input_lines.append(" INPUT START ".center(50, '-'))
-            input_lines.append(OpenAIAPI.converter.chat2raw(kwargs['messages']))
+            input_lines.append(cls.converter.chat2raw(messages))
             input_lines.append(" INPUT END ".center(50, '-')+"\n")
             input_str = "\n".join(input_lines)
         
         start_time = time.time()
         try:
-            response = OpenAIAPI.api_request_endpoint(request_url, model=model, messages=messages, method='post', timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
+            response = cls.api_request_endpoint(
+                request_url, 
+                messages=messages, 
+                method='post', 
+                timeout=timeout, 
+                endpoint_manager=endpoint_manager, 
+                api_key=api_key,
+                organization=organization,
+                api_base=api_base,
+                api_type=api_type,
+                **kwargs
+            )
             
             if logger is not None:
                 end_time = time.time()
                 ## log this on result
                 log_strs = []
                 log_strs.append(f"Chat request result ({end_time-start_time:.2f}s)")
                 log_strs.append(input_str)
 
                 log_strs.append(" OUTPUT START ".center(50, '-'))
                 stream = kwargs.get('stream', False)
                 if stream:
                     def wrapper(response):
                         text = ''
+                        role = ''
                         for data in response:
-                            if 'content' in data['choices'][0]['delta']:
-                                text += data['choices'][0]['delta']['content']
+                            message = data['choices'][0]['delta']
+                            if 'role' in message:
+                                role = message['role']
+                            if 'content' in message:
+                                text += message['content']
                             yield data
-                        log_strs.append(text)
+                        log_strs.append(cls.converter.chat2raw([{'role': role, 'content': text}]))
                         log_strs.append(" OUTPUT END ".center(50, '-')+"\n")
                         logger.info('\n'.join(log_strs))
                     response = wrapper(response)
                 else:
-                    log_strs.append(response['choices'][0]['message']['content'])
+                    log_strs.append(cls.converter.chat2raw([response['choices'][0]['message']]))
                     log_strs.append(" OUTPUT END ".center(50, '-')+"\n")
                     logger.info('\n'.join(log_strs))
         except Exception as e:
             if logger is not None:
                 end_time = time.time()
                 log_strs = []
                 log_strs.append(f"Chat request error ({end_time-start_time:.2f}s)")
                 log_strs.append(input_str)
                 log_strs.append(str(e))
                 logger.error('\n'.join(log_strs))
             raise e
 
         return response
     
-    @staticmethod
-    def completions(model, prompt, timeout=None, endpoint_manager=None, logger=None, log_marks=[], **kwargs):
-        request_url = '/completions'
+    @classmethod
+    def completions(cls, prompt, timeout=None, endpoint_manager=None, logger=None, log_marks=[], **kwargs):
+        api_key, organization, api_base, api_type, api_version, engine = cls.consume_kwargs(kwargs)
+        if api_type and api_type.lower() in _API_TYPES_AZURE:
+            if engine is None:
+                raise Exception("Azure API requires engine to be specified")
+            request_url = f'/openai/deployments/{quote_plus(engine)}/completions?api-version={api_version}'
+        else:
+            if engine is not None:
+                request_url = f'/engines/{quote_plus(engine)}/completions'
+            else:
+                request_url = '/completions'
 
-        if logger is not None and 'prompt' in kwargs:
+        if logger is not None:
             arguments = copy.deepcopy(kwargs)
-            arguments.pop('prompt', None)
             # check if log_marks is iterable
             if utils.isiterable(log_marks):
                 input_lines = [str(item) for item in log_marks]
             else:
                 input_lines = [str(log_marks)]
             input_lines.append(json.dumps(arguments, indent=2, ensure_ascii=False))
             input_lines.append(" INPUT START ".center(50, '-'))
-            input_lines.append(kwargs['prompt'])
+            input_lines.append(prompt)
             input_lines.append(" INPUT END ".center(50, '-')+"\n")
             input_str = "\n".join(input_lines)
         
         start_time = time.time()
         try:
-            response = OpenAIAPI.api_request_endpoint(request_url, model=model, prompt=prompt, method='post', timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
+            response = cls.api_request_endpoint(
+                request_url, 
+                prompt=prompt, 
+                method='post', 
+                timeout=timeout, 
+                endpoint_manager=endpoint_manager, 
+                api_key=api_key,
+                organization=organization,
+                api_base=api_base,
+                api_type=api_type,
+                **kwargs
+            )
 
             if logger is not None:
                 end_time = time.time()
                 ## log this on result
                 log_strs = []
                 log_strs.append(f"Completions request result ({end_time-start_time:.2f}s)")
                 log_strs.append(input_str)
@@ -250,125 +360,144 @@
                 log_strs.append(input_str)
                 log_strs.append(str(e))
                 logger.error('\n'.join(log_strs))
             raise e
 
         return response
     
-    @staticmethod
-    def edits(model, instruction, timeout=None, endpoint_manager=None, **kwargs):
+    @classmethod
+    def edits(cls, timeout=None, endpoint_manager=None, **kwargs):
         request_url = '/edits'
-        return OpenAIAPI.api_request_endpoint(request_url, model=model, instruction=instruction, method='post', timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
+        return cls.api_request_endpoint(request_url, method='post', timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
 
-    @staticmethod
-    def embeddings(model, input, timeout=None, endpoint_manager=None, **kwargs):
-        request_url = '/embeddings'
-        return OpenAIAPI.api_request_endpoint(request_url, model=model, input=input, method='post', timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
+    @classmethod
+    def embeddings(cls, timeout=None, endpoint_manager=None, **kwargs):
+        api_key, organization, api_base, api_type, api_version, engine = cls.consume_kwargs(kwargs)
+        if api_type and api_type.lower() in _API_TYPES_AZURE:
+            if engine is None:
+                raise Exception("Azure API requires engine to be specified")
+            request_url = f'/openai/deployments/{quote_plus(engine)}/embeddings?api-version={api_version}'
+        else:
+            if engine is not None:
+                request_url = f'/engines/{quote_plus(engine)}/embeddings'
+            else:
+                request_url = '/embeddings'
+        return cls.api_request_endpoint(
+            request_url, 
+            method='post', 
+            timeout=timeout, 
+            endpoint_manager=endpoint_manager, 
+            api_key=api_key,
+            organization=organization,
+            api_base=api_base,
+            api_type=api_type,
+            **kwargs
+            )
 
-    @staticmethod
-    def models_list(timeout=None, endpoint_manager=None, **kwargs):
+    @classmethod
+    def models_list(cls, timeout=None, endpoint_manager=None, **kwargs):
         request_url = '/models'
-        return OpenAIAPI.api_request_endpoint(request_url, method='get', timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
+        return cls.api_request_endpoint(request_url, method='get', timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
 
-    @staticmethod
-    def models_retrieve(model, timeout=None, endpoint_manager=None, **kwargs):
+    @classmethod
+    def models_retrieve(cls, model, timeout=None, endpoint_manager=None, **kwargs):
         request_url = f'/models/{model}'
-        return OpenAIAPI.api_request_endpoint(request_url, method='get', timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
+        return cls.api_request_endpoint(request_url, method='get', timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
 
-    @staticmethod
-    def moderations(input, timeout=None, endpoint_manager=None, **kwargs):
+    @classmethod
+    def moderations(cls, timeout=None, endpoint_manager=None, **kwargs):
         request_url = '/moderations'
-        return OpenAIAPI.api_request_endpoint(request_url, input=input, method='post', timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
+        return cls.api_request_endpoint(request_url, method='post', timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
 
-    @staticmethod
-    def images_generations(prompt, timeout=None, endpoint_manager=None, **kwargs):
+    @classmethod
+    def images_generations(cls, timeout=None, endpoint_manager=None, **kwargs):
         request_url = '/images/generations'
-        return OpenAIAPI.api_request_endpoint(request_url, prompt=prompt, method='post', timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
+        return cls.api_request_endpoint(request_url, method='post', timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
 
-    @staticmethod
-    def images_edits(image, prompt, mask=None, timeout=None, endpoint_manager=None, **kwargs):
+    @classmethod
+    def images_edits(cls, image, mask=None, timeout=None, endpoint_manager=None, **kwargs):
         request_url = '/images/edits'
         files = { 'image': image }
         if mask:
             files['mask'] = mask
-        return OpenAIAPI.api_request_endpoint(request_url, prompt=prompt, method='post', files=files, timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
+        return cls.api_request_endpoint(request_url, method='post', files=files, timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
 
-    @staticmethod
-    def images_variations(image, timeout=None, endpoint_manager=None, **kwargs):
+    @classmethod
+    def images_variations(cls, image, timeout=None, endpoint_manager=None, **kwargs):
         request_url = '/images/variations'
         files = { 'image': image }
-        return OpenAIAPI.api_request_endpoint(request_url, method='post', files=files, timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
+        return cls.api_request_endpoint(request_url, method='post', files=files, timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
 
-    @staticmethod
-    def audio_transcriptions(file, model, timeout=None, endpoint_manager=None, **kwargs):
+    @classmethod
+    def audio_transcriptions(cls, file, timeout=None, endpoint_manager=None, **kwargs):
         request_url = '/audio/transcriptions'
         files = { 'file': file }
-        return OpenAIAPI.api_request_endpoint(request_url, model=model, method='post', files=files, timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
+        return cls.api_request_endpoint(request_url, method='post', files=files, timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
 
-    @staticmethod
-    def audio_translations(file, model, timeout=None, endpoint_manager=None, **kwargs):
+    @classmethod
+    def audio_translations(cls, file, timeout=None, endpoint_manager=None, **kwargs):
         request_url = '/audio/translations'
         files = { 'file': file }
-        return OpenAIAPI.api_request_endpoint(request_url, model=model, method='post', files=files, timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
+        return cls.api_request_endpoint(request_url, method='post', files=files, timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
 
-    @staticmethod
-    def files_list(timeout=None, endpoint_manager=None, **kwargs):
+    @classmethod
+    def files_list(cls, timeout=None, endpoint_manager=None, **kwargs):
         request_url = '/files'
-        return OpenAIAPI.api_request_endpoint(request_url, method='get', timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
+        return cls.api_request_endpoint(request_url, method='get', timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
 
-    @staticmethod
-    def files_upload(file, purpose, timeout=None, endpoint_manager=None, **kwargs):
+    @classmethod
+    def files_upload(cls, file, timeout=None, endpoint_manager=None, **kwargs):
         request_url = '/files'
         files = { 'file': file }
-        return OpenAIAPI.api_request_endpoint(request_url, purpose=purpose, method='post', files=files, timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
+        return cls.api_request_endpoint(request_url, method='post', files=files, timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
 
-    @staticmethod
-    def files_delete(file_id, timeout=None, endpoint_manager=None, **kwargs):
+    @classmethod
+    def files_delete(cls, file_id, timeout=None, endpoint_manager=None, **kwargs):
         request_url = f'/files/{file_id}'
-        return OpenAIAPI.api_request_endpoint(request_url, method='delete', timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
+        return cls.api_request_endpoint(request_url, method='delete', timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
 
-    @staticmethod
-    def files_retrieve(file_id, timeout=None, endpoint_manager=None, **kwargs):
+    @classmethod
+    def files_retrieve(cls, file_id, timeout=None, endpoint_manager=None, **kwargs):
         request_url = f'/files/{file_id}'
-        return OpenAIAPI.api_request_endpoint(request_url, method='get', timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
+        return cls.api_request_endpoint(request_url, method='get', timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
 
-    @staticmethod
-    def files_retrieve_content(file_id, timeout=None, endpoint_manager=None, **kwargs):
+    @classmethod
+    def files_retrieve_content(cls, file_id, timeout=None, endpoint_manager=None, **kwargs):
         request_url = f'/files/{file_id}/content'
-        return OpenAIAPI.api_request_endpoint(request_url, method='get', timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
+        return cls.api_request_endpoint(request_url, method='get', timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
 
-    @staticmethod
-    def finetunes_create(training_file, timeout=None, endpoint_manager=None, **kwargs):
+    @classmethod
+    def finetunes_create(cls, timeout=None, endpoint_manager=None, **kwargs):
         request_url = '/fine-tunes'
-        return OpenAIAPI.api_request_endpoint(request_url, training_file=training_file, method='post', timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
+        return cls.api_request_endpoint(request_url, method='post', timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
 
-    @staticmethod
-    def finetunes_list(timeout=None, endpoint_manager=None, **kwargs):
+    @classmethod
+    def finetunes_list(cls, timeout=None, endpoint_manager=None, **kwargs):
         request_url = '/fine-tunes'
-        return OpenAIAPI.api_request_endpoint(request_url, method='get', timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
+        return cls.api_request_endpoint(request_url, method='get', timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
 
-    @staticmethod
-    def finetunes_retrieve(fine_tune_id, timeout=None, endpoint_manager=None, **kwargs):
+    @classmethod
+    def finetunes_retrieve(cls, fine_tune_id, timeout=None, endpoint_manager=None, **kwargs):
         request_url = f'/fine-tunes/{fine_tune_id}'
-        return OpenAIAPI.api_request_endpoint(request_url, method='get', timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
+        return cls.api_request_endpoint(request_url, method='get', timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
 
-    @staticmethod
-    def finetunes_cancel(fine_tune_id, timeout=None, endpoint_manager=None, **kwargs):
+    @classmethod
+    def finetunes_cancel(cls, fine_tune_id, timeout=None, endpoint_manager=None, **kwargs):
         request_url = f'/fine-tunes/{fine_tune_id}/cancel'
-        return OpenAIAPI.api_request_endpoint(request_url, method='post', timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
+        return cls.api_request_endpoint(request_url, method='post', timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
 
-    @staticmethod
-    def finetunes_list_events(fine_tune_id, timeout=None, endpoint_manager=None, **kwargs):
+    @classmethod
+    def finetunes_list_events(cls, fine_tune_id, timeout=None, endpoint_manager=None, **kwargs):
         request_url = f'/fine-tunes/{fine_tune_id}/events'
-        return OpenAIAPI.api_request_endpoint(request_url, method='get', timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
+        return cls.api_request_endpoint(request_url, method='get', timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
 
-    @staticmethod
-    def finetunes_delete_model(model, timeout=None, endpoint_manager=None, **kwargs):
+    @classmethod
+    def finetunes_delete_model(cls, model, timeout=None, endpoint_manager=None, **kwargs):
         request_url = f'/models/{model}'
-        return OpenAIAPI.api_request_endpoint(request_url, method='delete', timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
+        return cls.api_request_endpoint(request_url, method='delete', timeout=timeout, endpoint_manager=endpoint_manager, **kwargs)
 
 
 if __name__ == '__main__':
     # OpenAIAPI.api_key = 'sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx'
     prompt = [{
         "role": "user",
         "content": "please tell me a joke"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `HandyLLM-0.3.1/src/handyllm/prompt_converter.py` & `HandyLLM-0.4.0/src/handyllm/prompt_converter.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.3.1/src/handyllm/utils.py` & `HandyLLM-0.4.0/src/handyllm/utils.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.3.1/tests/test_completions.py` & `HandyLLM-0.4.0/tests/test_completions.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.3.1/tests/test_embedding.py` & `HandyLLM-0.4.0/tests/test_embedding.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.3.1/tests/test_files.py` & `HandyLLM-0.4.0/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.3.1/tests/test_images.py` & `HandyLLM-0.4.0/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.3.1/tests/test_models.py` & `HandyLLM-0.4.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.3.1/tests/test_moderation.py` & `HandyLLM-0.4.0/tests/test_moderation.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.3.1/tests/test_prompt.py` & `HandyLLM-0.4.0/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.3.1/tests/test_stream.py` & `HandyLLM-0.4.0/tests/test_stream.py`

 * *Files identical despite different names*

