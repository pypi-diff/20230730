# Comparing `tmp/mutual-0.3.1.tar.gz` & `tmp/mutual-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutual-0.3.1.tar", last modified: Fri Jul 28 06:21:20 2023, max compression
+gzip compressed data, was "mutual-0.3.2.tar", last modified: Sun Jul 30 04:00:33 2023, max compression
```

## Comparing `mutual-0.3.1.tar` & `mutual-0.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-28 06:21:20.382471 mutual-0.3.1/
--rw-r--r--   0 alexbetita   (501) staff       (20)     1068 2023-07-14 00:38:03.000000 mutual-0.3.1/LICENSE.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)     8270 2023-07-28 06:21:20.381896 mutual-0.3.1/PKG-INFO
--rw-r--r--   0 alexbetita   (501) staff       (20)     7843 2023-07-28 06:20:31.000000 mutual-0.3.1/README.md
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-28 06:21:20.377348 mutual-0.3.1/mutual/
--rw-r--r--   0 alexbetita   (501) staff       (20)      977 2023-07-26 00:49:16.000000 mutual-0.3.1/mutual/APIKey.py
--rw-r--r--   0 alexbetita   (501) staff       (20)    13481 2023-07-28 06:18:49.000000 mutual-0.3.1/mutual/Bot.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     5801 2023-07-28 06:06:29.000000 mutual-0.3.1/mutual/Chat.py
--rw-r--r--   0 alexbetita   (501) staff       (20)      532 2023-07-26 00:53:29.000000 mutual-0.3.1/mutual/Dev.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     3308 2023-07-26 00:53:58.000000 mutual-0.3.1/mutual/Judge.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     3290 2023-07-26 03:52:55.000000 mutual-0.3.1/mutual/JudgeMessage.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     4103 2023-07-26 04:17:57.000000 mutual-0.3.1/mutual/Material.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     2563 2023-07-26 06:28:01.000000 mutual-0.3.1/mutual/Memory.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     3631 2023-07-26 00:55:56.000000 mutual-0.3.1/mutual/Prompt.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     4228 2023-07-28 06:07:00.000000 mutual-0.3.1/mutual/__init__.py
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-28 06:21:20.381337 mutual-0.3.1/mutual.egg-info/
--rw-r--r--   0 alexbetita   (501) staff       (20)     8270 2023-07-28 06:21:20.000000 mutual-0.3.1/mutual.egg-info/PKG-INFO
--rw-r--r--   0 alexbetita   (501) staff       (20)      350 2023-07-28 06:21:20.000000 mutual-0.3.1/mutual.egg-info/SOURCES.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        1 2023-07-28 06:21:20.000000 mutual-0.3.1/mutual.egg-info/dependency_links.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        9 2023-07-28 06:21:20.000000 mutual-0.3.1/mutual.egg-info/requires.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        7 2023-07-28 06:21:20.000000 mutual-0.3.1/mutual.egg-info/top_level.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)       38 2023-07-28 06:21:20.382534 mutual-0.3.1/setup.cfg
--rw-r--r--   0 alexbetita   (501) staff       (20)      727 2023-07-28 03:55:31.000000 mutual-0.3.1/setup.py
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-30 04:00:33.135270 mutual-0.3.2/
+-rw-r--r--   0 alexbetita   (501) staff       (20)     1068 2023-07-14 00:38:03.000000 mutual-0.3.2/LICENSE.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)     8847 2023-07-30 04:00:33.134937 mutual-0.3.2/PKG-INFO
+-rw-r--r--   0 alexbetita   (501) staff       (20)     8420 2023-07-30 03:58:16.000000 mutual-0.3.2/README.md
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-30 04:00:33.133900 mutual-0.3.2/mutual/
+-rw-r--r--   0 alexbetita   (501) staff       (20)      977 2023-07-26 00:49:16.000000 mutual-0.3.2/mutual/APIKey.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)    13038 2023-07-30 03:57:23.000000 mutual-0.3.2/mutual/Bot.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     4953 2023-07-29 02:49:25.000000 mutual-0.3.2/mutual/Chat.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)      532 2023-07-26 00:53:29.000000 mutual-0.3.2/mutual/Dev.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3308 2023-07-26 00:53:58.000000 mutual-0.3.2/mutual/Judge.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3290 2023-07-26 03:52:55.000000 mutual-0.3.2/mutual/JudgeMessage.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     4103 2023-07-26 04:17:57.000000 mutual-0.3.2/mutual/Material.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     2995 2023-07-30 03:48:40.000000 mutual-0.3.2/mutual/Memory.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3631 2023-07-26 00:55:56.000000 mutual-0.3.2/mutual/Prompt.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     4228 2023-07-30 03:05:45.000000 mutual-0.3.2/mutual/__init__.py
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-30 04:00:33.134698 mutual-0.3.2/mutual.egg-info/
+-rw-r--r--   0 alexbetita   (501) staff       (20)     8847 2023-07-30 04:00:33.000000 mutual-0.3.2/mutual.egg-info/PKG-INFO
+-rw-r--r--   0 alexbetita   (501) staff       (20)      350 2023-07-30 04:00:33.000000 mutual-0.3.2/mutual.egg-info/SOURCES.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        1 2023-07-30 04:00:33.000000 mutual-0.3.2/mutual.egg-info/dependency_links.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        9 2023-07-30 04:00:33.000000 mutual-0.3.2/mutual.egg-info/requires.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        7 2023-07-30 04:00:33.000000 mutual-0.3.2/mutual.egg-info/top_level.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)       38 2023-07-30 04:00:33.135333 mutual-0.3.2/setup.cfg
+-rw-r--r--   0 alexbetita   (501) staff       (20)      727 2023-07-30 04:00:23.000000 mutual-0.3.2/setup.py
```

### Comparing `mutual-0.3.1/LICENSE.txt` & `mutual-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mutual-0.3.1/PKG-INFO` & `mutual-0.3.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,35 @@
-Metadata-Version: 2.1
-Name: mutual
-Version: 0.3.1
-Summary: A Python client for the Mutual API.
-Home-page: https://github.com/Mutu-AI
-Author: Alex Betita
-Author-email: alexbetita25@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # mutual
 
 A python package to interact with the Mutuai API.
 
 ## Installation
 
 Run `pip install mutual` in the project root directory.
 
 ### Usage
 
 ```python
 import mutual
+import json
 
 # to get the api_key
 print(mutual.api_key)
 # to set the api_key
 mutual.api_key = "your_api_key"
 
 # CHAT
 mutual.api_key = "your_api_key"
 for message in mutual.Chat.create("Hello", "seansbot", "Sean"):
-    print(message['content'], end='', flush=True)
+    json_data = json.loads(message)
+    print(json_data['content'], end='', flush=True)
 # OR
 for message in mutual.Chat.create("Hello", bot_name="seansbot", username="Sean", prompt="You are a customer assistant for mutual that provides helpful information"):
-    print(message['content'], end='', flush=True)
+    json_data = json.loads(message)
+    print(json_data['content'], end='', flush=True)
 
 ```
 ## Chat.create(parameters)
 ```python
 # bot_name --> uniquely identifies the bot tied to the api_key account holder
 # bot_id --> uniquely identifies the bot accross all bots
 # username --> uniquely identifies person interacting with bot
@@ -55,30 +44,33 @@
 # multiplayer_memory (bool) --> True by default, allows mulitplayer 
 # context_window (int) --> determines context, default 2
 ```
 
 ```python
 # CHAT DEMO
 for message in mutual.Chat.create_demo("Hello"):
-    print(message['content'], end='', flush=True)
+    json_data = json.loads(message)
+    print(json_data['content'], end='', flush=True)
 
 # BOT Instance
 
 # uses bot name
 alexbot = mutual.create_bot("bot_name") # THIS WILL CREATE A NEW BOT AND IF BOT WITH BOT NAME EXIST WILL RETURN THAT BOT
 for message in alexbot.chat("Hey there", "username"):
-    print(message['content'], end='', flush=True)
+    json_data = json.loads(message)
+    print(json_data['content'], end='', flush=True)
 
 # can create bot instance passing in these values
 alexbot = mutual.create_bot(bot_name="alexbot", prompt="You are a customer assistant for mutual that provides helpful information") 
 
 # bot id
 alexbot = mutual.fetch_bot("bot_id or bot_name") # THIS WILL LOOK UP FOR A EXISTING BOT AND GENERATE AN INSTANCE OF THAT BOT
 for message in alexbot.chat("Hey there", "Sean"):
-    print(message['content'], end='', flush=True)
+    json_data = json.loads(message)
+    print(json_data['content'], end='', flush=True)
 
 # update using bot instance
 alexbot.update_bot(bot_name='new_bot_name', prompt='You are a window cleaner')
 
 # feed bot data
 response = alexbot.feed(source="file_path")
 print(response)
@@ -193,33 +185,41 @@
 from mutual import Bot, Chat, Dev, Prompt, Judge, JudgeMessage, APIKey, Memory, Material
 ```
 
 # SAMPLE TO PRINT ERRORS
 ```py
 index = 0
 for message in mutual.Chat.create_demo("Hello"):
+    json_data = json.loads(message)
     if index == 0:
-        print(message['data']['bot_data']['bot_id'], end='', flush=True)
-        print(message['data']['user_data']['username'], end='', flush=True)
-        print(message['data']['bot_data']['bot_name'], end='', flush=True)
+        print(json_data['data']['bot_data']['bot_id'], end='', flush=True)
+        print(json_data['data']['user_data']['username'], end='', flush=True)
+        print(json_data['data']['bot_data']['bot_name'], end='', flush=True)
     index += 1
-    print(message['content'], end='', flush=True)
+    print(json_data['content'], end='', flush=True)
 ```
 
 # SAMPLE TO PRINT DATA
 ```py
 for message in mutual.Chat.create_demo("Hello"):
-    print(message['content'], end='', flush=True)
+    json_data = json.loads(message)
+    print(json_data['content'], end='', flush=True)
+
+alexbot = mutual.create_bot("AlexBot")
+for message in alexbot.chat("hello", username="Alex"):
+    json_data = json.loads(message)
+    print(json_data['content'], end='', flush=True)
 ```
 
 # FLOW EXAMPLE
 ```py
 alexbot = mutual.create_bot("AlexbBot2",prompt="You are a customer assistant for mutual that provides helpful information")
 for message in alexbot.chat("hello", username="Alex", flow=True):
-    print(message['content'], end='', flush=True)
+    json_data = json.loads(message)
+    print(json_data['content'], end='', flush=True)
 ```
 
 # FEED MEMORY EXAMPLE
 ```py
 alexbot = mutual.fetch_bot("mutual-bot-1")
 
 feed_response = alexbot.feed(source=f"/Users/alexbetita/Documents/Programming/api-agent-package/api-agent/package/agent_info_2_copy.txt")
@@ -235,14 +235,16 @@
     print(memory)
 ```
 
 # STREAM OFF EXAMPLE
 ```py
 
 response = alexbot.chat("Hi!", username="Alex", stream=False)
-print(response['content'])
+json_data = json.loads(response)
+print(json_data['content'])
 
 
 for message in alexbot.chat("hello", username="Alex", flow=True, stream=False):
-    print(message['content'], end='', flush=True)
+    json_data = json.loads(message)
+    print(json_data['content'], end='', flush=True)
 
-```
+```
```

### Comparing `mutual-0.3.1/README.md` & `mutual-0.3.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,49 @@
+Metadata-Version: 2.1
+Name: mutual
+Version: 0.3.2
+Summary: A Python client for the Mutual API.
+Home-page: https://github.com/Mutu-AI
+Author: Alex Betita
+Author-email: alexbetita25@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # mutual
 
 A python package to interact with the Mutuai API.
 
 ## Installation
 
 Run `pip install mutual` in the project root directory.
 
 ### Usage
 
 ```python
 import mutual
+import json
 
 # to get the api_key
 print(mutual.api_key)
 # to set the api_key
 mutual.api_key = "your_api_key"
 
 # CHAT
 mutual.api_key = "your_api_key"
 for message in mutual.Chat.create("Hello", "seansbot", "Sean"):
-    print(message['content'], end='', flush=True)
+    json_data = json.loads(message)
+    print(json_data['content'], end='', flush=True)
 # OR
 for message in mutual.Chat.create("Hello", bot_name="seansbot", username="Sean", prompt="You are a customer assistant for mutual that provides helpful information"):
-    print(message['content'], end='', flush=True)
+    json_data = json.loads(message)
+    print(json_data['content'], end='', flush=True)
 
 ```
 ## Chat.create(parameters)
 ```python
 # bot_name --> uniquely identifies the bot tied to the api_key account holder
 # bot_id --> uniquely identifies the bot accross all bots
 # username --> uniquely identifies person interacting with bot
@@ -41,30 +58,33 @@
 # multiplayer_memory (bool) --> True by default, allows mulitplayer 
 # context_window (int) --> determines context, default 2
 ```
 
 ```python
 # CHAT DEMO
 for message in mutual.Chat.create_demo("Hello"):
-    print(message['content'], end='', flush=True)
+    json_data = json.loads(message)
+    print(json_data['content'], end='', flush=True)
 
 # BOT Instance
 
 # uses bot name
 alexbot = mutual.create_bot("bot_name") # THIS WILL CREATE A NEW BOT AND IF BOT WITH BOT NAME EXIST WILL RETURN THAT BOT
 for message in alexbot.chat("Hey there", "username"):
-    print(message['content'], end='', flush=True)
+    json_data = json.loads(message)
+    print(json_data['content'], end='', flush=True)
 
 # can create bot instance passing in these values
 alexbot = mutual.create_bot(bot_name="alexbot", prompt="You are a customer assistant for mutual that provides helpful information") 
 
 # bot id
 alexbot = mutual.fetch_bot("bot_id or bot_name") # THIS WILL LOOK UP FOR A EXISTING BOT AND GENERATE AN INSTANCE OF THAT BOT
 for message in alexbot.chat("Hey there", "Sean"):
-    print(message['content'], end='', flush=True)
+    json_data = json.loads(message)
+    print(json_data['content'], end='', flush=True)
 
 # update using bot instance
 alexbot.update_bot(bot_name='new_bot_name', prompt='You are a window cleaner')
 
 # feed bot data
 response = alexbot.feed(source="file_path")
 print(response)
@@ -179,33 +199,41 @@
 from mutual import Bot, Chat, Dev, Prompt, Judge, JudgeMessage, APIKey, Memory, Material
 ```
 
 # SAMPLE TO PRINT ERRORS
 ```py
 index = 0
 for message in mutual.Chat.create_demo("Hello"):
+    json_data = json.loads(message)
     if index == 0:
-        print(message['data']['bot_data']['bot_id'], end='', flush=True)
-        print(message['data']['user_data']['username'], end='', flush=True)
-        print(message['data']['bot_data']['bot_name'], end='', flush=True)
+        print(json_data['data']['bot_data']['bot_id'], end='', flush=True)
+        print(json_data['data']['user_data']['username'], end='', flush=True)
+        print(json_data['data']['bot_data']['bot_name'], end='', flush=True)
     index += 1
-    print(message['content'], end='', flush=True)
+    print(json_data['content'], end='', flush=True)
 ```
 
 # SAMPLE TO PRINT DATA
 ```py
 for message in mutual.Chat.create_demo("Hello"):
-    print(message['content'], end='', flush=True)
+    json_data = json.loads(message)
+    print(json_data['content'], end='', flush=True)
+
+alexbot = mutual.create_bot("AlexBot")
+for message in alexbot.chat("hello", username="Alex"):
+    json_data = json.loads(message)
+    print(json_data['content'], end='', flush=True)
 ```
 
 # FLOW EXAMPLE
 ```py
 alexbot = mutual.create_bot("AlexbBot2",prompt="You are a customer assistant for mutual that provides helpful information")
 for message in alexbot.chat("hello", username="Alex", flow=True):
-    print(message['content'], end='', flush=True)
+    json_data = json.loads(message)
+    print(json_data['content'], end='', flush=True)
 ```
 
 # FEED MEMORY EXAMPLE
 ```py
 alexbot = mutual.fetch_bot("mutual-bot-1")
 
 feed_response = alexbot.feed(source=f"/Users/alexbetita/Documents/Programming/api-agent-package/api-agent/package/agent_info_2_copy.txt")
@@ -221,14 +249,16 @@
     print(memory)
 ```
 
 # STREAM OFF EXAMPLE
 ```py
 
 response = alexbot.chat("Hi!", username="Alex", stream=False)
-print(response['content'])
+json_data = json.loads(response)
+print(json_data['content'])
 
 
 for message in alexbot.chat("hello", username="Alex", flow=True, stream=False):
-    print(message['content'], end='', flush=True)
+    json_data = json.loads(message)
+    print(json_data['content'], end='', flush=True)
 
-```
+```
```

### Comparing `mutual-0.3.1/mutual/APIKey.py` & `mutual-0.3.2/mutual/APIKey.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.1/mutual/Bot.py` & `mutual-0.3.2/mutual/Bot.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import requests
 import json
 import mutual
-from typing import List, Union
+import io
+from typing import List, Union, Any, Tuple
 
 bot_default_response = {
             "bot_id": None,
             "bot_name": None,
             "bot_chat_index": None,
             "prompt_id": None,
             "judge_id": None,
@@ -147,15 +148,15 @@
         if response.status_code < 300:
             return response.json()
         else:
             self.default_stream_response["content"] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
             return self.default_stream_response
 
     def chat(self, content=None, username=None, prompt=None, multiplayer_memory = True, context_window = 2, 
-            flow=False, error_logs=False, stream=True, judge=False):
+            flow=False, error_logs=False, stream=True, judge=True):
         
         url = f"{mutual.endpoint}/chat"
 
         headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {self.api_key}"
         }
@@ -197,34 +198,18 @@
                     yield msg
             return self.default_stream_response
         
         data['stream'] = True
         response = requests.post(url, data=json.dumps(data), headers=headers, stream=stream)
 
         if response.status_code < 300:
-            is_new_bot = False
-            is_new_user = False
-
             # add the newly created bot to the bot class
             for line in response.iter_lines():
                 if line:  # filter out keep-alive new lines
-                    json_data = json.loads(line)
-                    if not self.bot_id:
-                        self.bot_id = json_data['data']['bot_data']['bot_id']
-                    if json_data['error'] is not None and not error_logs:
-                        continue
-                    if json_data['data']['bot_data']['new_bot'] and not is_new_bot:
-                        is_new_bot = True
-                        print(f"Newly created bot! Here is your id: {json_data['data']['bot_data']['bot_id']}")
-                    if json_data['data']['bot_data']['new_bot_user'] and not is_new_user:
-                        is_new_user = True
-                        print(f"New user {json_data['data']['user_data']['username']} created interacting with bot id: {json_data['data']['bot_data']['bot_id']}")
-                    if json_data['content'] =='[close]':
-                        continue
-                    yield json_data
+                    yield line
             
             if flow or self.flow:
                 print("\n\n", end="", flush=True)
                 new_content = input("Please enter a new response or type exit to exit: ")
                 if new_content.strip().lower() == "exit":
                     return
                 for msg in self.chat(content=new_content, username=username, prompt=prompt, 
@@ -268,21 +253,22 @@
         response = requests.get(url, headers=headers)
 
         if response.status_code < 300:
             return response.json()
         else:
             return f"Request failed with status code {response.status_code}, with an Error Message: {response.text}"
 
-    def feed(self, source: Union[str, List[str]] = None):
+    def feed(self, source: Union[str, List[str], Tuple[str, bytes]] = None):
         url = f"{mutual.endpoint}/memories/{self.bot_id}"
         url_text = f"{mutual.endpoint}/memories/{self.bot_id}/text"
         headers = {
             "Authorization": f"Bearer {mutual.api_key}"
         }
         # Check if the source is a file or a list of strings
+ 
         if isinstance(source, str):  # Source is a file path
             # Open the file in binary mode
             with open(source, 'rb') as file:
                 # Prepare the data payload
                 data = {
                     'file': file
                 }
@@ -294,12 +280,25 @@
             data = {
                 'data': source
             }
             # Convert data to json format
             data = json.dumps(data)
             # Send the POST request
             response = requests.post(url_text, data=data, headers=headers)
+
+        elif isinstance(source, tuple):  # Source is (filename, file content)
+            filename, file_content = source
+            # Prepare the data payload
+            data = {
+                'file': (filename, io.BytesIO(file_content))  # Create a tuple (filename, file-like object)
+            }
+            # Send the POST request
+            response = requests.post(url, files=data, headers=headers)
+
+        else:
+            return "The source type is not supported"
+
         # Check the response status code and return the appropriate message
         if response.status_code < 300:
             return response.json()
         else:
             return f"Request failed with status code {response.status_code}, with an Error Message: {response.text}"
```

### Comparing `mutual-0.3.1/mutual/Dev.py` & `mutual-0.3.2/mutual/Dev.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.1/mutual/Judge.py` & `mutual-0.3.2/mutual/Judge.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.1/mutual/JudgeMessage.py` & `mutual-0.3.2/mutual/JudgeMessage.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.1/mutual/Material.py` & `mutual-0.3.2/mutual/Material.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.1/mutual/Memory.py` & `mutual-0.3.2/mutual/Memory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,52 @@
 import requests
 import json
 import mutual
-from typing import List, Union
+import io
+from typing import List, Union, Tuple
 
-def feed(bot_arg: str = None, source: Union[str, List[str]] = None):
-    url = f"{mutual.endpoint}/memories/{bot_arg}"
-    url_text = f"{mutual.endpoint}/memories/{bot_arg}/text"
+def feed(self, source: Union[str, List[str], Tuple[str, bytes]] = None):
+    url = f"{mutual.endpoint}/memories/{self.bot_id}"
+    url_text = f"{mutual.endpoint}/memories/{self.bot_id}/text"
     headers = {
         "Authorization": f"Bearer {mutual.api_key}"
     }
     # Check if the source is a file or a list of strings
     if isinstance(source, str):  # Source is a file path
         # Open the file in binary mode
         with open(source, 'rb') as file:
             # Prepare the data payload
             data = {
                 'file': file
             }
             # Send the POST request
             response = requests.post(url, files=data, headers=headers)
+
     elif isinstance(source, list):  # Source is a list of strings
         # Prepare the data payload
         data = {
-            'file': {
-                'data': source
-            }
+            'data': source
         }
         # Convert data to json format
         data = json.dumps(data)
         # Send the POST request
         response = requests.post(url_text, data=data, headers=headers)
+
+    elif isinstance(source, tuple):  # Source is (filename, file content)
+        filename, file_content = source
+        # Prepare the data payload
+        data = {
+            'file': (filename, io.BytesIO(file_content))  # Create a tuple (filename, file-like object)
+        }
+        # Send the POST request
+        response = requests.post(url, files=data, headers=headers)
+
+    else:
+        return "The source type is not supported"
+
     # Check the response status code and return the appropriate message
     if response.status_code < 300:
         return response.json()
     else:
         return f"Request failed with status code {response.status_code}, with an Error Message: {response.text}"
```

### Comparing `mutual-0.3.1/mutual/Prompt.py` & `mutual-0.3.2/mutual/Prompt.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.1/mutual/__init__.py` & `mutual-0.3.2/mutual/__init__.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.1/mutual.egg-info/PKG-INFO` & `mutual-0.3.2/mutual.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutual
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Python client for the Mutual API.
 Home-page: https://github.com/Mutu-AI
 Author: Alex Betita
 Author-email: alexbetita25@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,27 +20,30 @@
 
 Run `pip install mutual` in the project root directory.
 
 ### Usage
 
 ```python
 import mutual
+import json
 
 # to get the api_key
 print(mutual.api_key)
 # to set the api_key
 mutual.api_key = "your_api_key"
 
 # CHAT
 mutual.api_key = "your_api_key"
 for message in mutual.Chat.create("Hello", "seansbot", "Sean"):
-    print(message['content'], end='', flush=True)
+    json_data = json.loads(message)
+    print(json_data['content'], end='', flush=True)
 # OR
 for message in mutual.Chat.create("Hello", bot_name="seansbot", username="Sean", prompt="You are a customer assistant for mutual that provides helpful information"):
-    print(message['content'], end='', flush=True)
+    json_data = json.loads(message)
+    print(json_data['content'], end='', flush=True)
 
 ```
 ## Chat.create(parameters)
 ```python
 # bot_name --> uniquely identifies the bot tied to the api_key account holder
 # bot_id --> uniquely identifies the bot accross all bots
 # username --> uniquely identifies person interacting with bot
@@ -55,30 +58,33 @@
 # multiplayer_memory (bool) --> True by default, allows mulitplayer 
 # context_window (int) --> determines context, default 2
 ```
 
 ```python
 # CHAT DEMO
 for message in mutual.Chat.create_demo("Hello"):
-    print(message['content'], end='', flush=True)
+    json_data = json.loads(message)
+    print(json_data['content'], end='', flush=True)
 
 # BOT Instance
 
 # uses bot name
 alexbot = mutual.create_bot("bot_name") # THIS WILL CREATE A NEW BOT AND IF BOT WITH BOT NAME EXIST WILL RETURN THAT BOT
 for message in alexbot.chat("Hey there", "username"):
-    print(message['content'], end='', flush=True)
+    json_data = json.loads(message)
+    print(json_data['content'], end='', flush=True)
 
 # can create bot instance passing in these values
 alexbot = mutual.create_bot(bot_name="alexbot", prompt="You are a customer assistant for mutual that provides helpful information") 
 
 # bot id
 alexbot = mutual.fetch_bot("bot_id or bot_name") # THIS WILL LOOK UP FOR A EXISTING BOT AND GENERATE AN INSTANCE OF THAT BOT
 for message in alexbot.chat("Hey there", "Sean"):
-    print(message['content'], end='', flush=True)
+    json_data = json.loads(message)
+    print(json_data['content'], end='', flush=True)
 
 # update using bot instance
 alexbot.update_bot(bot_name='new_bot_name', prompt='You are a window cleaner')
 
 # feed bot data
 response = alexbot.feed(source="file_path")
 print(response)
@@ -193,33 +199,41 @@
 from mutual import Bot, Chat, Dev, Prompt, Judge, JudgeMessage, APIKey, Memory, Material
 ```
 
 # SAMPLE TO PRINT ERRORS
 ```py
 index = 0
 for message in mutual.Chat.create_demo("Hello"):
+    json_data = json.loads(message)
     if index == 0:
-        print(message['data']['bot_data']['bot_id'], end='', flush=True)
-        print(message['data']['user_data']['username'], end='', flush=True)
-        print(message['data']['bot_data']['bot_name'], end='', flush=True)
+        print(json_data['data']['bot_data']['bot_id'], end='', flush=True)
+        print(json_data['data']['user_data']['username'], end='', flush=True)
+        print(json_data['data']['bot_data']['bot_name'], end='', flush=True)
     index += 1
-    print(message['content'], end='', flush=True)
+    print(json_data['content'], end='', flush=True)
 ```
 
 # SAMPLE TO PRINT DATA
 ```py
 for message in mutual.Chat.create_demo("Hello"):
-    print(message['content'], end='', flush=True)
+    json_data = json.loads(message)
+    print(json_data['content'], end='', flush=True)
+
+alexbot = mutual.create_bot("AlexBot")
+for message in alexbot.chat("hello", username="Alex"):
+    json_data = json.loads(message)
+    print(json_data['content'], end='', flush=True)
 ```
 
 # FLOW EXAMPLE
 ```py
 alexbot = mutual.create_bot("AlexbBot2",prompt="You are a customer assistant for mutual that provides helpful information")
 for message in alexbot.chat("hello", username="Alex", flow=True):
-    print(message['content'], end='', flush=True)
+    json_data = json.loads(message)
+    print(json_data['content'], end='', flush=True)
 ```
 
 # FEED MEMORY EXAMPLE
 ```py
 alexbot = mutual.fetch_bot("mutual-bot-1")
 
 feed_response = alexbot.feed(source=f"/Users/alexbetita/Documents/Programming/api-agent-package/api-agent/package/agent_info_2_copy.txt")
@@ -235,14 +249,16 @@
     print(memory)
 ```
 
 # STREAM OFF EXAMPLE
 ```py
 
 response = alexbot.chat("Hi!", username="Alex", stream=False)
-print(response['content'])
+json_data = json.loads(response)
+print(json_data['content'])
 
 
 for message in alexbot.chat("hello", username="Alex", flow=True, stream=False):
-    print(message['content'], end='', flush=True)
+    json_data = json.loads(message)
+    print(json_data['content'], end='', flush=True)
 
 ```
```

### Comparing `mutual-0.3.1/setup.py` & `mutual-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mutual',
-    version='0.3.1',  # beta
+    version='0.3.2',  # beta
     description='A Python client for the Mutual API.',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     author='Alex Betita', # placeholder for now
     author_email='alexbetita25@gmail.com', # placeholder for now
     url='https://github.com/Mutu-AI',  # if you have a github repo for the package
     packages=find_packages(),
```

