# Comparing `tmp/openplugincore-0.5.0.tar.gz` & `tmp/openplugincore-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openplugincore-0.5.0.tar", last modified: Sat Jul 29 21:03:27 2023, max compression
+gzip compressed data, was "openplugincore-0.6.0.tar", last modified: Sun Jul 30 01:15:18 2023, max compression
```

## Comparing `openplugincore-0.5.0.tar` & `openplugincore-0.6.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:03:27.782038 openplugincore-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-29 21:03:27.782038 openplugincore-0.5.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:03:27.782038 openplugincore-0.5.0/openplugincore/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-29 21:03:17.000000 openplugincore-0.5.0/openplugincore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-07-29 21:03:17.000000 openplugincore-0.5.0/openplugincore/openplugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-29 21:03:17.000000 openplugincore-0.5.0/openplugincore/openplugin_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-29 21:03:17.000000 openplugincore-0.5.0/openplugincore/openplugin_memo.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-29 21:03:17.000000 openplugincore-0.5.0/openplugincore/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:03:27.782038 openplugincore-0.5.0/openplugincore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-29 21:03:27.000000 openplugincore-0.5.0/openplugincore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-29 21:03:27.000000 openplugincore-0.5.0/openplugincore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 21:03:27.000000 openplugincore-0.5.0/openplugincore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-29 21:03:27.000000 openplugincore-0.5.0/openplugincore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 21:03:27.000000 openplugincore-0.5.0/openplugincore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 21:03:27.782038 openplugincore-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-29 21:03:17.000000 openplugincore-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:03:27.782038 openplugincore-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 21:03:17.000000 openplugincore-0.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-29 21:03:17.000000 openplugincore-0.5.0/tests/mock_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10217 2023-07-29 21:03:17.000000 openplugincore-0.5.0/tests/test_e2e.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-29 21:03:17.000000 openplugincore-0.5.0/tests/test_openplugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-29 21:03:17.000000 openplugincore-0.5.0/tests/test_openplugin_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-29 21:03:17.000000 openplugincore-0.5.0/tests/test_openplugin_memo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:15:18.455580 openplugincore-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-30 01:15:18.455580 openplugincore-0.6.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:15:18.451580 openplugincore-0.6.0/openplugincore/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-30 01:15:07.000000 openplugincore-0.6.0/openplugincore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-07-30 01:15:07.000000 openplugincore-0.6.0/openplugincore/openplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-30 01:15:07.000000 openplugincore-0.6.0/openplugincore/openplugin_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-30 01:15:07.000000 openplugincore-0.6.0/openplugincore/openplugin_memo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-30 01:15:07.000000 openplugincore-0.6.0/openplugincore/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:15:18.451580 openplugincore-0.6.0/openplugincore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-30 01:15:18.000000 openplugincore-0.6.0/openplugincore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-30 01:15:18.000000 openplugincore-0.6.0/openplugincore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 01:15:18.000000 openplugincore-0.6.0/openplugincore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-30 01:15:18.000000 openplugincore-0.6.0/openplugincore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-30 01:15:18.000000 openplugincore-0.6.0/openplugincore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 01:15:18.455580 openplugincore-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-30 01:15:07.000000 openplugincore-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 01:15:18.455580 openplugincore-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 01:15:07.000000 openplugincore-0.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-30 01:15:07.000000 openplugincore-0.6.0/tests/mock_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11443 2023-07-30 01:15:07.000000 openplugincore-0.6.0/tests/test_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13061 2023-07-30 01:15:07.000000 openplugincore-0.6.0/tests/test_openplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-30 01:15:07.000000 openplugincore-0.6.0/tests/test_openplugin_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-30 01:15:07.000000 openplugincore-0.6.0/tests/test_openplugin_memo.py
```

### Comparing `openplugincore-0.5.0/PKG-INFO` & `openplugincore-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: openplugincore
-Version: 0.5.0
+Version: 0.6.0
 Summary: Seamlessly integrate with OpenAI ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!
 Home-page: UNKNOWN
 Author: Sebastian Sosa
 Author-email: 1sebastian1sosa1@gmail.com
 License: UNKNOWN
 Description: Seamlessly integrate with OpenAIs ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!
 Keywords: python,openai,chatgpt,chat,plugin
```

### Comparing `openplugincore-0.5.0/openplugincore/openplugin.py` & `openplugincore-0.6.0/openplugincore/openplugin.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from urllib.error import HTTPError
 import requests
 from typing import Any, List, Dict, Union, Tuple, Callable
 import os
 from .types import ChatgptAssistantMessage, ChatgptFunctionMessage, PluginConfigs
 from .utils.constants import openai_models_info
-from .utils.prompting import estimate_tokens, truncate_json_root
+from .utils.prompting import estimate_tokens, tokens_to_chars, truncate_json_root
 from langchain.chains.openai_functions.openapi import openapi_spec_to_openai_fn
 from langchain.utilities.openapi import OpenAPISpec
 from langchain.output_parsers.openai_functions import JsonOutputFunctionsParser
 from langchain.prompts import ChatPromptTemplate
 from langchain.chat_models import ChatOpenAI
 from langchain.schema import HumanMessage, AIMessage, SystemMessage, FunctionMessage
 from langchain import LLMChain
@@ -17,50 +17,14 @@
 from dotenv import load_dotenv
 load_dotenv()
 
 OPENAI_API_KEY = os.getenv('OPENAI_API_KEY')
 
 plugin_configs: Dict[str, PluginConfigs] = {}
 
-def openplugin_completion(openai_api_key: str, prompt: str, plugin_name: str = None, root_url: str = None, **chatgpt_args):
-    # set environment variable to OPENAI_API_KEY
-    os.environ["OPENAI_API_KEY"] = openai_api_key
-    openai.api_key = openai_api_key
-    if not plugin_name and not root_url:
-        return openai.ChatCompletion.create(
-            **chatgpt_args,
-            messages=[
-                {"role": "user", "content": prompt}
-            ]
-        )
-    plugin = OpenPlugin(plugin_name=plugin_name, root_url=root_url, openai_api_key=openai_api_key)
-    try:
-        function_response = plugin.fetch_plugin(
-            prompt=prompt,
-            **chatgpt_args
-        )
-    except ValueError as e:
-        if "Not a plugin function" in str(e):
-            return openai.ChatCompletion.create(
-                **chatgpt_args,
-                messages=[
-                    {"role": "user", "content": prompt}
-                ]
-            )
-        else:
-            raise e
-    all_chatgpt_args = {
-        **chatgpt_args,
-        "messages": [
-            {"role": "user", "content": prompt},
-            function_response
-        ]
-    }
-    summarize = openai.ChatCompletion.create(**all_chatgpt_args)
-    return summarize
 
 class OpenPlugin:
     def __init__(self, plugin_name: str = None, openai_api_key: str = None, root_url: str = None, verbose: bool = False):
         self.name: str = plugin_name
         self.root_url: str = root_url
         self.description: str = None
         self.manifest: Any = None
@@ -158,16 +122,17 @@
             elif openai_message["role"] == "assistant":
                 # set veriable content to "" if it is None
                 content = openai_message["content"] if openai_message["content"] is not None else ""
                 langchain_messages.append(AIMessage(content=content, additional_kwargs={"function_call": openai_message["function_call"]}))
         
         return langchain_messages
 
-    def fetch_plugin(self, prompt: str, truncate: Union[bool, int] = False, truncate_offset: int = 0, **chatgpt_args) -> ChatgptFunctionMessage:
-        if chatgpt_args.get("model", None) not in ["gpt-3.5-turbo-0613", "gpt-4-0613"]:
+    def fetch_plugin(self, messages: list[dict], truncate: Union[bool, int] = False, truncate_offset: int = 0, **chatgpt_args) -> ChatgptFunctionMessage:
+        model = chatgpt_args.get("model", None)
+        if model not in ["gpt-3.5-turbo-0613", "gpt-4-0613"]:
             raise ValueError("Model must be either gpt-3.5-turbo-0613 or gpt-4-0613")
         
         llm =  ChatOpenAI(
             **chatgpt_args,
         )
         llm_chain = LLMChain(
             llm=llm,
@@ -175,16 +140,46 @@
             llm_kwargs={"functions": self.functions},
             output_parser=JsonOutputFunctionsParser(args_only=False),
             output_key="function",
             verbose=self.verbose,
             # **(llm_kwargs or {}),
         )
         # if it is plugin function response
+        functions_tokens = estimate_tokens(json.dumps(self.functions))
+
         try:
-            llm_chain_out = llm_chain.run(prompt)
+            # MESSAGES TO PROMPT
+            # if there is a message with role system then pop it, iterate through all messages to find it
+            system_message = ''
+            for message in messages:
+                if message["role"] == 'system':
+                    system_message = 'system' + ": " + message['content'] + "\n"
+                    messages.remove(message)
+                    break
+            
+            # print("system_message: ", system_message)
+            # Combine messages into one string
+            messages_aggregate = '\n'.join([f"{message['role']}: {message['content']}" for message in messages])
+            complete_messages_aggregate_tokens = estimate_tokens(system_message + messages_aggregate)
+            # print("complete_messages_aggregate_tokens: ", complete_messages_aggregate_tokens)
+            # print("functions_tokens: ", functions_tokens)
+            messages_truncation_offset = tokens_to_chars(max(complete_messages_aggregate_tokens + functions_tokens - openai_models_info[model]["max_tokens"], 0)) 
+            # print("messages_truncation_offset: ", messages_truncation_offset)
+            messages_aggregate = messages_aggregate[messages_truncation_offset:]
+           
+            # TODO: temp fix to prevent collation of messages
+            if (messages_truncation_offset > 0):
+                messages_aggregate = "user/assistant: " + messages_aggregate
+           
+            complete_messages_aggregate = system_message + messages_aggregate
+            # print("complete_messages_aggregate: ", complete_messages_aggregate)  
+            # print("final length: ", estimate_tokens(complete_messages_aggregate))          
+
+            # Replace prompt with messageAggregate
+            llm_chain_out = llm_chain.run(complete_messages_aggregate)
             if self.verbose:
                 print("Using plugin: " + self.name)
         except KeyError as e:
             # if error includes "function_call" then it is not a plugin function
             if "function_call" in str(e):
                 raise ValueError("Not a plugin function")
             else:
@@ -214,19 +209,15 @@
         request_out = request_chain(**llm_chain_out)
         json_response = request_out.json()
 
         if truncate:
             truncate_to = truncate if not isinstance(truncate, bool) else None
             if truncate_to is None:
                 token_slack = 56 + 300
-                dummy_chatgpt_message = {
-                    "role": "user",
-                    "content": prompt,
-                }
-                truncate_to = openai_models_info[chatgpt_args['model']]['max_tokens'] - estimate_tokens(json.dumps(dummy_chatgpt_message)) - token_slack - truncate_offset
+                truncate_to = openai_models_info[model]['max_tokens'] - estimate_tokens(json.dumps(messages[-1])) - token_slack - truncate_offset
             json_response = truncate_json_root(json_response, truncate_to)
 
         if self.verbose:
             print(f"\"{self.name}\" json_response: ", json.dumps(json_response, indent=2))
         try:
             return ChatgptFunctionMessage(
                 role="function",
```

### Comparing `openplugincore-0.5.0/openplugincore/openplugin_memo.py` & `openplugincore-0.6.0/openplugincore/openplugin_memo.py`

 * *Files identical despite different names*

### Comparing `openplugincore-0.5.0/openplugincore/types.py` & `openplugincore-0.6.0/openplugincore/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Callable, Dict, List, TypedDict
+from typing import Any, Dict, TypedDict
 from enum import Enum
 
 class AssistantRole(Enum):
     USER = "user"
 
 class ChatgptAssistantMessage(TypedDict):
     role: AssistantRole
```

### Comparing `openplugincore-0.5.0/openplugincore.egg-info/PKG-INFO` & `openplugincore-0.6.0/openplugincore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: openplugincore
-Version: 0.5.0
+Version: 0.6.0
 Summary: Seamlessly integrate with OpenAI ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!
 Home-page: UNKNOWN
 Author: Sebastian Sosa
 Author-email: 1sebastian1sosa1@gmail.com
 License: UNKNOWN
 Description: Seamlessly integrate with OpenAIs ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!
 Keywords: python,openai,chatgpt,chat,plugin
```

### Comparing `openplugincore-0.5.0/setup.py` & `openplugincore-0.6.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name='openplugincore', 
-        version="0.5.0",
+        version="0.6.0",
         author="Sebastian Sosa",
         author_email="1sebastian1sosa1@gmail.com",
         description='Seamlessly integrate with OpenAI ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!',
         long_description='Seamlessly integrate with OpenAIs ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!',
         packages=find_packages(),
         package_data={
             "openplugincore": ["*.json"],  # include all .json files in the openplugin package
```

### Comparing `openplugincore-0.5.0/tests/mock_data.py` & `openplugincore-0.6.0/tests/mock_data.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 todo_plugin = {
     "prompt": "add 'buy milk' to my todo list",
+    "messages": [
+        {
+            "role": "user",
+            "content": "add 'buy milk' to my todo list"
+        }
+    ],
     "chat_completion_of_function": {
         "role": "assistant",
         "content": None,
         "function_call": {
             "name": "addTodo",
             "arguments": "{\n  \"todo\": \"buy milk\"\n}"
         }
```

### Comparing `openplugincore-0.5.0/tests/test_e2e.py` & `openplugincore-0.6.0/tests/test_e2e.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     assert addTodo == todo_plugin["functions"][0]
 
     assert getTodos is not None
     assert getTodos == todo_plugin["functions"][1]
 
     # fetch after chatgpt response
     response = plugin.fetch_plugin(
-        prompt=todo_plugin["prompt"],
+        messages=todo_plugin["messages"],
         model="gpt-3.5-turbo-0613",
         temperature=0,
     )
     assert response is not None
     assert response["role"] == "function"
     assert response["name"] == "addTodo"
     json_content = json.loads(response["content"])
@@ -39,15 +39,20 @@
 def test_initiate_and_fetch_LGTM():
     plugin = OpenPlugin("LGTM")
     assert plugin.manifest is not None
 
     # # create chatgpt request that will call the addTodo function
     chatgpt_prompt = 'Show me markdown for a 2 by 2 table with LGTM'
     response = plugin.fetch_plugin(
-        prompt=chatgpt_prompt,
+        messages=[
+            {
+                "role": "user",
+                "content": chatgpt_prompt
+            }
+        ],
         model="gpt-3.5-turbo-0613",
         temperature=0,
     )
 
     assert response is not None
     assert response["role"] == "function"
     json_content = json.loads(response["content"])
@@ -59,15 +64,20 @@
 def test_initiate_and_fetch_yt_caption_retriever():
     plugin = OpenPlugin("yt_caption_retriever")
     assert plugin.manifest is not None
 
     # create chatgpt request that will call the addTodo function
     chatgpt_prompt = 'give me a 2 sentence summary of the following yt video https://www.youtube.com/watch?v=P310I19L3Ko'
     response = plugin.fetch_plugin(
-        prompt=chatgpt_prompt,
+        messages=[
+            {
+                "role": "user",
+                "content": chatgpt_prompt
+            }
+        ],
         model="gpt-3.5-turbo-0613",
         temperature=0,
     )
 
     assert response is not None
     assert response["role"] == "function"
     json_content = json.loads(response["content"])
@@ -78,15 +88,20 @@
 def test_initiate_and_fetch_twtData():
     plugin = OpenPlugin("twtData")
     assert plugin.manifest is not None
 
     # create chatgpt request that will call the addTodo function
     chatgpt_prompt = 'show me the amount of people @Sebasti54919704 is following'
     response = plugin.fetch_plugin(
-        prompt=chatgpt_prompt,
+        messages=[
+            {
+                "role": "user",
+                "content": chatgpt_prompt
+            }
+        ],
         model="gpt-3.5-turbo-0613",
         temperature=0,
     )
 
     assert response is not None
     assert response["role"] == "function"
     json_content = json.loads(response["content"])
@@ -98,15 +113,20 @@
 def test_initiate_and_fetch_surge_ai_trends():
     plugin = OpenPlugin("surge_ai_trends")
     assert plugin.manifest is not None
 
     # create chatgpt request that will call the addTodo function
     chatgpt_prompt = 'What are the trnding searches for "gpu" in amazon'
     response = plugin.fetch_plugin(
-        prompt=chatgpt_prompt,
+        messages=[
+            {
+                "role": "user",
+                "content": chatgpt_prompt
+            }
+        ],
         model="gpt-3.5-turbo-0613",
         temperature=0,
     )
 
     assert response is not None
     assert response["role"] == "function"
     json_content = json.loads(response["content"])
@@ -117,15 +137,20 @@
 def test_initiate_and_fetch_speedy_marketing():
     plugin = OpenPlugin("speedy_marketing")
     assert plugin.manifest is not None
 
     # create chatgpt request that will call the addTodo function
     chatgpt_prompt = 'write me an SEO blog about react for marketing'
     response = plugin.fetch_plugin(
-        prompt=chatgpt_prompt,
+        messages=[
+            {
+                "role": "user",
+                "content": chatgpt_prompt
+            }
+        ],
         model="gpt-3.5-turbo-0613",
         temperature=0,
     )
 
     assert response is not None
     assert response["role"] == "function"
     json_content = json.loads(response["content"])
@@ -137,15 +162,20 @@
 def test_initiate_and_fetch_scholarai():
     plugin = OpenPlugin("scholarai")
     assert plugin.manifest is not None
 
     # create chatgpt request that will call the addTodo function
     chatgpt_prompt = 'What scientific research exists for semantic representation of language through brain waves. show me one.'
     response = plugin.fetch_plugin(
-        prompt=chatgpt_prompt,
+        messages=[
+            {
+                "role": "user",
+                "content": chatgpt_prompt
+            }
+        ],
         model="gpt-3.5-turbo-0613",
         temperature=0,
     )
 
     assert response is not None
     assert response["role"] == "function"
     json_content = json.loads(response["content"])
@@ -155,15 +185,20 @@
 def test_initiate_and_fetch_rephrase():
     plugin = OpenPlugin("rephrase")
     assert plugin.manifest is not None
 
     # create chatgpt request that will call the addTodo function
     chatgpt_prompt = 'I want to code a react ui with hello world please rephrase that'
     response = plugin.fetch_plugin(
-        prompt=chatgpt_prompt,
+        messages=[
+            {
+                "role": "user",
+                "content": chatgpt_prompt
+            }
+        ],
         model="gpt-3.5-turbo-0613",
         temperature=0,
     )
 
     assert response is not None
     assert response["role"] == "function"
     json_content = json.loads(response["content"])
@@ -174,15 +209,20 @@
 def test_initiate_and_fetch_DreamInterpreter():
     plugin = OpenPlugin("DreamInterpreter", verbose=True)
     assert plugin.manifest is not None
     
     # create chatgpt request that will call the addTodo function
     chatgpt_prompt = 'I dreamt of being in a room without any windows getting smaller overtime'
     response = plugin.fetch_plugin(
-        prompt=chatgpt_prompt,
+        messages=[
+            {
+                "role": "user",
+                "content": chatgpt_prompt
+            }
+        ],
         model="gpt-3.5-turbo-0613",
         temperature=0,
     )
 
     assert response is not None
     assert response["role"] == "function"
     json_content = json.loads(response["content"])
@@ -193,15 +233,20 @@
 def test_initiate_and_fetch_portfoliopilot():
     plugin = OpenPlugin("portfoliopilot", verbose=True)
     assert plugin.manifest is not None
     
     # create chatgpt request that will call the addTodo function
     chatgpt_prompt = 'What stocks should I add for my long term tech portfolio'
     response = plugin.fetch_plugin(
-        prompt=chatgpt_prompt,
+        messages=[
+            {
+                "role": "user",
+                "content": chatgpt_prompt
+            }
+        ],
         model="gpt-3.5-turbo-0613",
         temperature=0,
     )
 
     assert response is not None
     assert response["role"] == "function"
     json_content = json.loads(response["content"])
@@ -212,15 +257,20 @@
 def test_initiate_and_fetch_C3_Glide():
     plugin = OpenPlugin("C3_Glide", verbose=True)
     assert plugin.manifest is not None
     
     # create chatgpt request that will call the addTodo function
     chatgpt_prompt = 'Provide me TAF for KJFK with reguards to aviation weather'
     response = plugin.fetch_plugin(
-        prompt=chatgpt_prompt,
+        messages=[
+            {
+                "role": "user",
+                "content": chatgpt_prompt
+            }
+        ],
         model="gpt-3.5-turbo-0613",
         temperature=0,
     )
 
     assert response is not None
     assert response["role"] == "function"
     json_content = json.loads(response["content"])
@@ -232,15 +282,20 @@
 def test_initiate_and_fetch_Ai_PDF():
     plugin = OpenPlugin("Ai_PDF", verbose=True)
     assert plugin.manifest is not None
     
     # create chatgpt request that will call the addTodo function
     chatgpt_prompt = 'Can I have my data be private according to this pdf https://www.unodc.org/pdf/criminal_justice/UN_Basic_Principles_on_the_Role_of_Lawyers.pdf'
     response = plugin.fetch_plugin(
-        prompt=chatgpt_prompt,
+        messages=[
+            {
+                "role": "user",
+                "content": chatgpt_prompt
+            }
+        ],
         model="gpt-3.5-turbo-0613",
         temperature=0,
     )
 
     assert response is not None
     assert response["role"] == "function"
     json_content = json.loads(response["content"])
@@ -267,15 +322,20 @@
 #         f.write(json.dumps(plugin.manifest, indent=2))
 #     with open("logs/functions.json", "w") as f:
 #         f.write(json.dumps(plugin.functions, indent=2))
     
 #     # create chatgpt request that will call the addTodo function
 #     chatgpt_prompt = 'PLUGIN_PROMPT'
 #     response = plugin.fetch_plugin(
-#         prompt=chatgpt_prompt,
+#         messages=[
+#             {
+#                 "role": "user",
+#                 "content": chatgpt_prompt
+#             }
+#         ],
 #         model="gpt-3.5-turbo-0613",
 #         temperature=0,
 #     )
 
 #     # DELETE
 #     with open("logs/plugin_response.json", "w") as f:
 #         f.write(json.dumps(response, indent=2))
```

### Comparing `openplugincore-0.5.0/tests/test_openplugin_completion.py` & `openplugincore-0.6.0/tests/test_openplugin_completion.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,20 @@
 
 def test_openplugin_completion():
     todo = f'test_chat_completion_{random.randint(0, 100000)}'
 
     completion = openplugin_completion(
         openai_api_key = OPENAI_API_KEY,
         plugin_name = "__testing__",
-        prompt = f"add '{todo}' to my todo list",
+        messages = [
+            {
+                "role": "user",
+                "content": f"add '{todo}' to my todo list"
+            }
+        ],
         model = "gpt-3.5-turbo-0613",
         temperature = 0,
     )
 
     todos_request = requests.get("http://localhost:3333/todos")
     todos_body = todos_request.json()
     
@@ -34,15 +39,20 @@
 
 def test_openplugin_completion_with_url():
     todo = f'test_chat_completion_{random.randint(0, 100000)}'
 
     completion = openplugin_completion(
         openai_api_key = OPENAI_API_KEY,
         root_url = "http://localhost:3333",
-        prompt = f"add '{todo}' to my todo list",
+        messages = [
+            {
+                "role": "user",
+                "content": f"add '{todo}' to my todo list"
+            }
+        ],
         model = "gpt-3.5-turbo-0613",
         temperature = 0,
     )
 
     todos_request = requests.get("http://localhost:3333/todos")
     todos_body = todos_request.json()
```

### Comparing `openplugincore-0.5.0/tests/test_openplugin_memo.py` & `openplugincore-0.6.0/tests/test_openplugin_memo.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     open_plugin_memo.init()
 
     todo_openplugin = open_plugin_memo.init_plugin('__testing__')
     assert todo_openplugin.manifest is not None
     assert len(todo_openplugin.functions) == 2
 
     response = todo_openplugin.fetch_plugin(
-        prompt=todo_plugin["prompt"],
+        messages=todo_plugin["messages"],
         model='gpt-3.5-turbo-0613',
     )
 
     assert response is not None
     assert response['role'] == 'function'
     assert response['name'] == 'addTodo'
```

