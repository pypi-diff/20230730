# Comparing `tmp/HandyLLM-0.5.0.tar.gz` & `tmp/HandyLLM-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HandyLLM-0.5.0.tar", last modified: Sun Jul 30 07:13:01 2023, max compression
+gzip compressed data, was "HandyLLM-0.5.1.tar", last modified: Sun Jul 30 18:26:56 2023, max compression
```

## Comparing `HandyLLM-0.5.0.tar` & `HandyLLM-0.5.1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 07:13:01.307262 HandyLLM-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-07-30 07:13:01.307262 HandyLLM-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-07-30 07:12:51.000000 HandyLLM-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-30 07:12:51.000000 HandyLLM-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 07:13:01.307262 HandyLLM-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 07:13:01.303261 HandyLLM-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 07:13:01.303261 HandyLLM-0.5.0/src/HandyLLM.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-07-30 07:13:01.000000 HandyLLM-0.5.0/src/HandyLLM.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-30 07:13:01.000000 HandyLLM-0.5.0/src/HandyLLM.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 07:13:01.000000 HandyLLM-0.5.0/src/HandyLLM.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-30 07:13:01.000000 HandyLLM-0.5.0/src/HandyLLM.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-30 07:13:01.000000 HandyLLM-0.5.0/src/HandyLLM.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 07:13:01.303261 HandyLLM-0.5.0/src/handyllm/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-30 07:12:51.000000 HandyLLM-0.5.0/src/handyllm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-30 07:12:51.000000 HandyLLM-0.5.0/src/handyllm/endpoint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    20659 2023-07-30 07:12:51.000000 HandyLLM-0.5.0/src/handyllm/openai_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-07-30 07:12:51.000000 HandyLLM-0.5.0/src/handyllm/prompt_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-30 07:12:51.000000 HandyLLM-0.5.0/src/handyllm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 07:13:01.307262 HandyLLM-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-30 07:12:51.000000 HandyLLM-0.5.0/tests/test_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-30 07:12:51.000000 HandyLLM-0.5.0/tests/test_azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-30 07:12:51.000000 HandyLLM-0.5.0/tests/test_completions.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-30 07:12:51.000000 HandyLLM-0.5.0/tests/test_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-30 07:12:51.000000 HandyLLM-0.5.0/tests/test_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-30 07:12:51.000000 HandyLLM-0.5.0/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-30 07:12:51.000000 HandyLLM-0.5.0/tests/test_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-30 07:12:51.000000 HandyLLM-0.5.0/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-30 07:12:51.000000 HandyLLM-0.5.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-30 07:12:51.000000 HandyLLM-0.5.0/tests/test_moderation.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-30 07:12:51.000000 HandyLLM-0.5.0/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-30 07:12:51.000000 HandyLLM-0.5.0/tests/test_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:26:56.525037 HandyLLM-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-07-30 18:26:56.525037 HandyLLM-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-07-30 18:26:41.000000 HandyLLM-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-30 18:26:41.000000 HandyLLM-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 18:26:56.525037 HandyLLM-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:26:56.517037 HandyLLM-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:26:56.517037 HandyLLM-0.5.1/src/HandyLLM.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-07-30 18:26:56.000000 HandyLLM-0.5.1/src/HandyLLM.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-30 18:26:56.000000 HandyLLM-0.5.1/src/HandyLLM.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 18:26:56.000000 HandyLLM-0.5.1/src/HandyLLM.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-30 18:26:56.000000 HandyLLM-0.5.1/src/HandyLLM.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-30 18:26:56.000000 HandyLLM-0.5.1/src/HandyLLM.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:26:56.521036 HandyLLM-0.5.1/src/handyllm/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-30 18:26:41.000000 HandyLLM-0.5.1/src/handyllm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-30 18:26:41.000000 HandyLLM-0.5.1/src/handyllm/api_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-30 18:26:41.000000 HandyLLM-0.5.1/src/handyllm/endpoint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17989 2023-07-30 18:26:41.000000 HandyLLM-0.5.1/src/handyllm/openai_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-07-30 18:26:41.000000 HandyLLM-0.5.1/src/handyllm/prompt_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-30 18:26:41.000000 HandyLLM-0.5.1/src/handyllm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:26:56.525037 HandyLLM-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-30 18:26:41.000000 HandyLLM-0.5.1/tests/test_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-30 18:26:41.000000 HandyLLM-0.5.1/tests/test_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-30 18:26:41.000000 HandyLLM-0.5.1/tests/test_completions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-30 18:26:41.000000 HandyLLM-0.5.1/tests/test_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-30 18:26:41.000000 HandyLLM-0.5.1/tests/test_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-30 18:26:41.000000 HandyLLM-0.5.1/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-30 18:26:41.000000 HandyLLM-0.5.1/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-30 18:26:41.000000 HandyLLM-0.5.1/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-30 18:26:41.000000 HandyLLM-0.5.1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-30 18:26:41.000000 HandyLLM-0.5.1/tests/test_moderation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-30 18:26:41.000000 HandyLLM-0.5.1/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-30 18:26:41.000000 HandyLLM-0.5.1/tests/test_stream.py
```

### Comparing `HandyLLM-0.5.0/PKG-INFO` & `HandyLLM-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HandyLLM
-Version: 0.5.0
+Version: 0.5.1
 Summary: A handy toolkit for using LLM.
 Author-email: Atomie CHEN <atomic_cwh@163.com>
 Project-URL: Homepage, https://github.com/atomiechen/HandyLLM
 Project-URL: Bug Tracker, https://github.com/atomiechen/HandyLLM/issues
 Keywords: LLM,Large Language Model,Prompt,OpenAI,API
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `HandyLLM-0.5.0/README.md` & `HandyLLM-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.5.0/pyproject.toml` & `HandyLLM-0.5.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HandyLLM"
-version = "0.5.0"
+version = "0.5.1"
 authors = [
   { name="Atomie CHEN", email="atomic_cwh@163.com" },
 ]
 description = "A handy toolkit for using LLM."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `HandyLLM-0.5.0/src/HandyLLM.egg-info/PKG-INFO` & `HandyLLM-0.5.1/src/HandyLLM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HandyLLM
-Version: 0.5.0
+Version: 0.5.1
 Summary: A handy toolkit for using LLM.
 Author-email: Atomie CHEN <atomic_cwh@163.com>
 Project-URL: Homepage, https://github.com/atomiechen/HandyLLM
 Project-URL: Bug Tracker, https://github.com/atomiechen/HandyLLM/issues
 Keywords: LLM,Large Language Model,Prompt,OpenAI,API
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `HandyLLM-0.5.0/src/HandyLLM.egg-info/SOURCES.txt` & `HandyLLM-0.5.1/src/HandyLLM.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 pyproject.toml
 src/HandyLLM.egg-info/PKG-INFO
 src/HandyLLM.egg-info/SOURCES.txt
 src/HandyLLM.egg-info/dependency_links.txt
 src/HandyLLM.egg-info/requires.txt
 src/HandyLLM.egg-info/top_level.txt
 src/handyllm/__init__.py
+src/handyllm/api_request.py
 src/handyllm/endpoint_manager.py
 src/handyllm/openai_api.py
 src/handyllm/prompt_converter.py
 src/handyllm/utils.py
 tests/test_audio.py
 tests/test_azure.py
 tests/test_completions.py
```

### Comparing `HandyLLM-0.5.0/src/handyllm/endpoint_manager.py` & `HandyLLM-0.5.1/src/handyllm/endpoint_manager.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.5.0/src/handyllm/openai_api.py` & `HandyLLM-0.5.1/src/handyllm/openai_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,20 @@
 import os
 import time
 from urllib.parse import quote_plus
-import requests
-import logging
 import json
 import copy
 
+from .api_request import api_request, poll
 from .endpoint_manager import Endpoint, EndpointManager
 from .prompt_converter import PromptConverter
 from . import utils
 
-_API_BASE_OPENAI = 'https://api.openai.com/v1'
-_API_TYPE_OPENAI = 'openai'
-_API_TYPES_AZURE = (
-    'azure', 
-    'azure_ad', 
-    'azuread'
-)
-_API_VERSION_AZURE = '2023-05-15'
+from . import _API_BASE_OPENAI, _API_TYPE_OPENAI, _API_TYPES_AZURE, _API_VERSION_AZURE
 
-module_logger = logging.getLogger(__name__)
 
 class OpenAIAPI:
     
     # deprecated
     base_url = _API_BASE_OPENAI
     
     # set this to your API base;
@@ -50,122 +41,33 @@
     # can be None.
     api_version = None
     
     converter = PromptConverter()
     
     @classmethod
     def get_api_key(cls, api_key=None):
-        if not api_key:
-            api_key = cls.api_key if cls.api_key else os.environ.get('OPENAI_API_KEY')
-        return api_key
+        return api_key or cls.api_key or os.environ.get('OPENAI_API_KEY')
     
     @classmethod
     def get_organization(cls, organization=None):
-        if not organization:
-            organization = cls.organization if cls.organization else os.environ.get('OPENAI_ORGANIZATION')
-        return organization
+        return organization or cls.organization or os.environ.get('OPENAI_ORGANIZATION')
     
     @classmethod
     def get_api_base(cls, api_base=None):
-        if not api_base:
-            api_base = cls.api_base if cls.api_base else os.environ.get('OPENAI_API_BASE')
-            if not api_base:
-                api_base = _API_BASE_OPENAI
-        return api_base
+        return api_base or cls.api_base or os.environ.get('OPENAI_API_BASE') or _API_BASE_OPENAI
     
     @classmethod
     def get_api_type_and_version(cls, api_type=None, api_version=None):
-        if not api_type:
-            api_type = cls.api_type if cls.api_type else os.environ.get('OPENAI_API_TYPE')
-            if not api_type:
-                api_type = _API_TYPE_OPENAI
-        if not api_version:
-            api_version = cls.api_version if cls.api_version else os.environ.get('OPENAI_API_VERSION')
-            if not api_version and api_type and api_type.lower() in _API_TYPES_AZURE:
-                api_version = _API_VERSION_AZURE
+        api_type = api_type or cls.api_type or os.environ.get('OPENAI_API_TYPE') or _API_TYPE_OPENAI
+        api_version = api_version or cls.api_version or os.environ.get('OPENAI_API_VERSION')
+        if not api_version and api_type and api_type.lower() in _API_TYPES_AZURE:
+            api_version = _API_VERSION_AZURE
         return api_type, api_version
 
     @staticmethod
-    def _api_request(url, api_key, organization=None, api_type=api_type, method='post', timeout=None, **kwargs):
-        if api_key is None:
-            raise Exception("OpenAI API key is not set")
-        if url is None:
-            raise Exception("OpenAI API url is not set")
-        if api_type is None:
-            raise Exception("OpenAI API type is not set")
-
-        ## log request info
-        log_strs = []
-        # avoid logging the whole api_key
-        plaintext_len = 8
-        log_strs.append(f"API request {url}")
-        log_strs.append(f"api_key: {api_key[:plaintext_len]}{'*'*(len(api_key)-plaintext_len)}")
-        if organization is not None:
-            log_strs.append(f"organization: {organization[:plaintext_len]}{'*'*(len(organization)-plaintext_len)}")
-        log_strs.append(f"timeout: {timeout}")
-        module_logger.info('\n'.join(log_strs))
-
-        files = kwargs.pop('files', None)
-        stream = kwargs.get('stream', False)
-        headers = {}
-        json_data = None
-        data = None
-        params = {}
-        if api_type in _API_TYPES_AZURE:
-            headers['api-key'] = api_key
-        else:
-            headers['Authorization'] = 'Bearer ' + api_key
-        if organization is not None:
-            headers['OpenAI-Organization'] = organization
-        if method == 'post':
-            if files is None:
-                headers['Content-Type'] = 'application/json'
-                json_data = kwargs
-            else:  ## if files is not None, let requests handle the content type
-                data = kwargs
-        if method == 'get' and stream:
-            params['stream'] = 'true'
-
-        response = requests.request(
-            method,
-            url,
-            headers=headers,
-            data=data,
-            json=json_data,
-            files=files,
-            params=params,
-            stream=stream,
-            timeout=timeout,
-            )
-        if response.status_code != 200:
-            # report both status code and error message
-            try:
-                message = response.json()['error']['message']
-            except:
-                message = response.text
-            err_msg = f"OpenAI API error ({url} {response.status_code} {response.reason}): {message}"
-            module_logger.error(err_msg)
-            raise Exception(err_msg)
-
-        if stream:
-            return OpenAIAPI._gen_stream_response(response)
-        else:
-            return response.json()
-
-    @staticmethod
-    def _gen_stream_response(response):
-        for byte_line in response.iter_lines():  # do not auto decode
-            if byte_line:
-                if byte_line.strip() == b"data: [DONE]":
-                    return
-                if byte_line.startswith(b"data: "):
-                    line = byte_line[len(b"data: "):].decode("utf-8")
-                    yield json.loads(line)
-
-    @staticmethod
     def stream_chat_with_role(response):
         role = ''
         for data in response:
             message = data['choices'][0]['delta']
             if 'role' in message:
                 role = message['role']
             if 'content' in message:
@@ -186,15 +88,15 @@
     def api_request_endpoint(
         cls,
         request_url, 
         **kwargs
         ):
         api_key, organization, api_base, api_type, api_version, engine = cls.consume_kwargs(kwargs)
         url = utils.join_url(api_base, request_url)
-        return cls._api_request(url, api_key, organization=organization, api_type=api_type, **kwargs)
+        return api_request(url, api_key, organization=organization, api_type=api_type, **kwargs)
     
     @classmethod
     def consume_kwargs(cls, kwargs):
         api_key = organization = api_base = api_type = api_version = engine = None
 
         # read API info from endpoint_manager
         endpoint_manager = kwargs.pop('endpoint_manager', None)
@@ -417,16 +319,60 @@
     @classmethod
     def moderations(cls, **kwargs):
         request_url = '/moderations'
         return cls.api_request_endpoint(request_url, method='post', **kwargs)
 
     @classmethod
     def images_generations(cls, **kwargs):
-        request_url = '/images/generations'
-        return cls.api_request_endpoint(request_url, method='post', **kwargs)
+        api_key, organization, api_base, api_type, api_version, engine = cls.consume_kwargs(kwargs)
+        if api_type and api_type.lower() in _API_TYPES_AZURE:
+            request_url = f'/openai/images/generations:submit?api-version={api_version}'
+            raw_response = True
+        else:
+            request_url = '/images/generations'
+            raw_response = False
+        response = cls.api_request_endpoint(
+            request_url, 
+            method='post', 
+            api_key=api_key,
+            organization=organization,
+            api_base=api_base,
+            api_type=api_type,
+            raw_response=raw_response,
+            **kwargs
+            )
+        if api_type and api_type.lower() in _API_TYPES_AZURE:
+            # Azure image generation
+            # use raw response to get poll_url
+            poll_url = response.headers['operation-location']
+            headers= { "api-key": api_key, "Content-Type": "application/json" }
+            response = poll(
+                url=poll_url, 
+                method='get', 
+                until=lambda response: response.json()['status'] == 'succeeded',
+                failed=cls.check_image_failure,
+                interval=lambda response: cls.get_retry(response) or 1,
+                headers=headers, 
+                ).json()
+            return response.get('result', response)
+        else:
+            return response
+
+    @staticmethod
+    def check_image_failure(response):
+        response_dict = response.json()
+        if response_dict['status'] == 'failed':
+            raise Exception(f"Image generation failed: {response_dict['error']['code']} {response_dict['error']['message']}")
+    
+    @staticmethod
+    def get_retry(response):
+        try:
+            return int(response.headers.get('retry-after'))
+        except:
+            return None
 
     @classmethod
     def images_edits(cls, image, mask=None, **kwargs):
         request_url = '/images/edits'
         files = { 'image': image }
         if mask:
             files['mask'] = mask
@@ -502,43 +448,7 @@
         return cls.api_request_endpoint(request_url, method='get', **kwargs)
 
     @classmethod
     def finetunes_delete_model(cls, model, **kwargs):
         request_url = f'/models/{model}'
         return cls.api_request_endpoint(request_url, method='delete', **kwargs)
 
-
-if __name__ == '__main__':
-    # OpenAIAPI.api_key = 'sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx'
-    prompt = [{
-        "role": "user",
-        "content": "please tell me a joke"
-        }]
-    response = OpenAIAPI.chat(
-        model="gpt-3.5-turbo-0301",
-        messages=prompt,
-        temperature=0.2,
-        max_tokens=256,
-        top_p=1.0,
-        frequency_penalty=0.0,
-        presence_penalty=0.0,
-        timeout=10
-        )
-    print(response)
-    print(response['choices'][0]['message']['content'])
-    
-    ## below for comparison
-    # import openai
-    # response = openai.ChatCompletion.create(
-    #     model="gpt-3.5-turbo-0301",
-    #     messages=prompt,
-    #     temperature=1.2,
-    #     max_tokens=256,
-    #     top_p=1.0,
-    #     frequency_penalty=0.0,
-    #     presence_penalty=0.0,
-    #     api_key=openai_api_key,
-    #     timeout=10  ## this is not working
-    # )
-    # print(response)
-    # print(response['choices'][0]['message']['content'])
-
```

### Comparing `HandyLLM-0.5.0/src/handyllm/prompt_converter.py` & `HandyLLM-0.5.1/src/handyllm/prompt_converter.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.5.0/src/handyllm/utils.py` & `HandyLLM-0.5.1/src/handyllm/utils.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.5.0/tests/test_azure.py` & `HandyLLM-0.5.1/tests/test_azure.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from handyllm import OpenAIAPI
+from handyllm import OpenAIAPI, utils
 
 from dotenv import load_dotenv, find_dotenv
 # load env parameters from file
 load_dotenv(find_dotenv('azure.env'))
 
 import os
 import json
@@ -16,16 +16,15 @@
 # ----- EXAMPLE 1 -----
 
 prompt = [{
     "role": "user",
     "content": "please tell me a joke"
     }]
 response = OpenAIAPI.chat(
-    # engine="gpt-35-turbo",
-    deployment_id="initial_deployment",
+    engine="gpt-35-turbo",
     messages=prompt,
     temperature=0.2,
     max_tokens=256,
     top_p=1.0,
     frequency_penalty=0.0,
     presence_penalty=0.0,
     timeout=10,
@@ -42,7 +41,21 @@
 response = OpenAIAPI.embeddings(
     engine="text-embedding-ada-002",
     input="I enjoy walking with my cute dog",
     timeout=10,
 )
 print(json.dumps(response, indent=2))
 
+
+# ----- EXAMPLE 3 -----
+
+response = OpenAIAPI.images_generations(
+    api_version='2023-06-01-preview',
+    prompt="A panda, synthwave style, digital painting",
+    n=1,
+    size="256x256",
+)
+print(json.dumps(response, indent=2))
+download_url = response['data'][0]['url']
+file_path = utils.download_binary(download_url)
+print(f"generated image: {file_path}")
+
```

### Comparing `HandyLLM-0.5.0/tests/test_completions.py` & `HandyLLM-0.5.1/tests/test_completions.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.5.0/tests/test_embedding.py` & `HandyLLM-0.5.1/tests/test_embedding.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.5.0/tests/test_endpoint.py` & `HandyLLM-0.5.1/tests/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.5.0/tests/test_files.py` & `HandyLLM-0.5.1/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.5.0/tests/test_images.py` & `HandyLLM-0.5.1/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.5.0/tests/test_logger.py` & `HandyLLM-0.5.1/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.5.0/tests/test_models.py` & `HandyLLM-0.5.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.5.0/tests/test_moderation.py` & `HandyLLM-0.5.1/tests/test_moderation.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.5.0/tests/test_prompt.py` & `HandyLLM-0.5.1/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.5.0/tests/test_stream.py` & `HandyLLM-0.5.1/tests/test_stream.py`

 * *Files identical despite different names*

