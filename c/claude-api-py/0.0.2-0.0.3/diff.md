# Comparing `tmp/claude-api-py-0.0.2.tar.gz` & `tmp/claude-api-py-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "claude-api-py-0.0.2.tar", last modified: Thu Jul 20 09:28:45 2023, max compression
+gzip compressed data, was "claude-api-py-0.0.3.tar", last modified: Sun Jul 30 09:11:57 2023, max compression
```

## Comparing `claude-api-py-0.0.2.tar` & `claude-api-py-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ashwin     (501) staff       (20)        0 2023-07-20 09:28:45.917213 claude-api-py-0.0.2/
--rw-r--r--   0 ashwin     (501) staff       (20)     1069 2023-07-20 08:10:00.000000 claude-api-py-0.0.2/LICENSE
--rw-r--r--   0 ashwin     (501) staff       (20)     5282 2023-07-20 09:28:45.917371 claude-api-py-0.0.2/PKG-INFO
--rw-r--r--   0 ashwin     (501) staff       (20)     4514 2023-07-20 09:26:39.000000 claude-api-py-0.0.2/README.md
-drwxr-xr-x   0 ashwin     (501) staff       (20)        0 2023-07-20 09:28:45.913710 claude-api-py-0.0.2/claude/
--rw-r--r--   0 ashwin     (501) staff       (20)       22 2023-07-20 09:27:16.000000 claude-api-py-0.0.2/claude/__init__.py
--rw-r--r--   0 ashwin     (501) staff       (20)    11205 2023-07-20 09:23:00.000000 claude-api-py-0.0.2/claude/claude_client.py
--rw-r--r--   0 ashwin     (501) staff       (20)     8394 2023-07-20 07:28:10.000000 claude-api-py-0.0.2/claude/claude_wrapper.py
--rw-r--r--   0 ashwin     (501) staff       (20)     3064 2023-07-20 09:22:52.000000 claude-api-py-0.0.2/claude/constants.py
--rw-r--r--   0 ashwin     (501) staff       (20)     8672 2023-07-20 07:52:24.000000 claude-api-py-0.0.2/claude/custom_requests.py
--rw-r--r--   0 ashwin     (501) staff       (20)     1265 2023-07-20 07:21:51.000000 claude-api-py-0.0.2/claude/custom_types.py
--rw-r--r--   0 ashwin     (501) staff       (20)      579 2023-07-20 07:14:41.000000 claude-api-py-0.0.2/claude/helpers.py
-drwxr-xr-x   0 ashwin     (501) staff       (20)        0 2023-07-20 09:28:45.916813 claude-api-py-0.0.2/claude_api_py.egg-info/
--rw-r--r--   0 ashwin     (501) staff       (20)     5282 2023-07-20 09:28:45.000000 claude-api-py-0.0.2/claude_api_py.egg-info/PKG-INFO
--rw-r--r--   0 ashwin     (501) staff       (20)      375 2023-07-20 09:28:45.000000 claude-api-py-0.0.2/claude_api_py.egg-info/SOURCES.txt
--rw-r--r--   0 ashwin     (501) staff       (20)        1 2023-07-20 09:28:45.000000 claude-api-py-0.0.2/claude_api_py.egg-info/dependency_links.txt
--rw-r--r--   0 ashwin     (501) staff       (20)       13 2023-07-20 09:28:45.000000 claude-api-py-0.0.2/claude_api_py.egg-info/requires.txt
--rw-r--r--   0 ashwin     (501) staff       (20)        7 2023-07-20 09:28:45.000000 claude-api-py-0.0.2/claude_api_py.egg-info/top_level.txt
--rw-r--r--   0 ashwin     (501) staff       (20)      103 2023-07-20 09:28:45.917999 claude-api-py-0.0.2/setup.cfg
--rw-r--r--   0 ashwin     (501) staff       (20)     1161 2023-07-20 09:28:05.000000 claude-api-py-0.0.2/setup.py
+drwxr-xr-x   0 ashwin     (501) staff       (20)        0 2023-07-30 09:11:57.027727 claude-api-py-0.0.3/
+-rw-r--r--   0 ashwin     (501) staff       (20)     1069 2023-07-20 08:10:00.000000 claude-api-py-0.0.3/LICENSE
+-rw-r--r--   0 ashwin     (501) staff       (20)     5739 2023-07-30 09:11:57.027904 claude-api-py-0.0.3/PKG-INFO
+-rw-r--r--   0 ashwin     (501) staff       (20)     4971 2023-07-25 04:42:04.000000 claude-api-py-0.0.3/README.md
+drwxr-xr-x   0 ashwin     (501) staff       (20)        0 2023-07-30 09:11:57.024485 claude-api-py-0.0.3/claude/
+-rw-r--r--   0 ashwin     (501) staff       (20)       22 2023-07-30 09:11:01.000000 claude-api-py-0.0.3/claude/__init__.py
+-rw-r--r--   0 ashwin     (501) staff       (20)    11180 2023-07-22 23:11:22.000000 claude-api-py-0.0.3/claude/claude_client.py
+-rw-r--r--   0 ashwin     (501) staff       (20)     9792 2023-07-30 09:06:56.000000 claude-api-py-0.0.3/claude/claude_wrapper.py
+-rw-r--r--   0 ashwin     (501) staff       (20)     3064 2023-07-20 09:22:52.000000 claude-api-py-0.0.3/claude/constants.py
+-rw-r--r--   0 ashwin     (501) staff       (20)     8590 2023-07-22 22:18:19.000000 claude-api-py-0.0.3/claude/custom_requests.py
+-rw-r--r--   0 ashwin     (501) staff       (20)     1265 2023-07-20 07:21:51.000000 claude-api-py-0.0.3/claude/custom_types.py
+-rw-r--r--   0 ashwin     (501) staff       (20)      579 2023-07-20 07:14:41.000000 claude-api-py-0.0.3/claude/helpers.py
+drwxr-xr-x   0 ashwin     (501) staff       (20)        0 2023-07-30 09:11:57.027428 claude-api-py-0.0.3/claude_api_py.egg-info/
+-rw-r--r--   0 ashwin     (501) staff       (20)     5739 2023-07-30 09:11:57.000000 claude-api-py-0.0.3/claude_api_py.egg-info/PKG-INFO
+-rw-r--r--   0 ashwin     (501) staff       (20)      375 2023-07-30 09:11:57.000000 claude-api-py-0.0.3/claude_api_py.egg-info/SOURCES.txt
+-rw-r--r--   0 ashwin     (501) staff       (20)        1 2023-07-30 09:11:57.000000 claude-api-py-0.0.3/claude_api_py.egg-info/dependency_links.txt
+-rw-r--r--   0 ashwin     (501) staff       (20)       13 2023-07-30 09:11:57.000000 claude-api-py-0.0.3/claude_api_py.egg-info/requires.txt
+-rw-r--r--   0 ashwin     (501) staff       (20)        7 2023-07-30 09:11:57.000000 claude-api-py-0.0.3/claude_api_py.egg-info/top_level.txt
+-rw-r--r--   0 ashwin     (501) staff       (20)      103 2023-07-30 09:11:57.028511 claude-api-py-0.0.3/setup.cfg
+-rw-r--r--   0 ashwin     (501) staff       (20)     1161 2023-07-20 09:28:05.000000 claude-api-py-0.0.3/setup.py
```

### Comparing `claude-api-py-0.0.2/LICENSE` & `claude-api-py-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `claude-api-py-0.0.2/PKG-INFO` & `claude-api-py-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claude-api-py
-Version: 0.0.2
+Version: 0.0.3
 Summary: Unofficial Anthropic Claude API for Python3.
 Home-page: https://github.com/AshwinPathi/claude-api-py
 License: MIT
 Keywords: llm,claude,api,gpt
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -18,48 +18,61 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Unofficial Claude API For Python
 
 The UNOFFICIAL free API for Anthropic's Claude LLM.
 
+## Background
+
+Claude is [Anthropic's](https://www.anthropic.com/) LLM app (similar to ChatGPT). This library allows you to use the API (for free) and interact with it in your python projects.
+
 ## Implemented actions:
 The Unofficial Claude API is under active development. The following endpoints are usable in some capacity:
 
 - Getting organizations you're in
 - Getting conversations you're in
 - Starting a conversation
-- Sending a message and receiving a response (can't send files yet)
+- Sending a message and receiving a response
 - Delete a conversation
 - Create an attachment from a file
 - Send attachments
+- getting message history
 
 Note that the api is __**synchronous**__.
 
 ## TODO features
+- Tests
 - Fixing models OTHER than `claude_2`
 - asynchronous mode
 - Better caching
 - cleaner errors and passing these up to users
 
 
+This project is under active development and is extremely unstable, so there are no guarantees it will work for you. If you find a bug or you think it should work in a scenario where it doesn't, file an issue.
+
+
 ## Usage
 
 ### Step 1
 Install the library using the following:
 ```
-pip install rev-claude-api
+pip install claude-api-py
 ```
 
 If that doesn't work, you can install directly from this github repository:
 
 ```
 pip install git+git://github.com/AshwinPathi/claude-api-py.git
 ```
 
+There is one requirement as of now:
+- `sseclient-py` [link here](https://github.com/mpetazzoni/sseclient)
+
+
 ### Step 2
 Get a `sessionKey` from the Claude website. You will need this to start the bot. Ideally also have a user agent of the computer you use to access claude.
 
 You can get this information by logging into `https://claude.ai/chats` and doing the following:
 
 1. open inspect element (f12 on chrome)
 2. On the top bar, go to the `Application` tab.
@@ -84,17 +97,19 @@
 # context. This allows you to use the API more ergonomically.
 from claude import claude_wrapper
 ```
 
 #### Create the client and wrapper
 ```py
 client = claude_client.ClaudeClient(SESSION_KEY)
-organizations = client.get_organizations()
 
-claude_obj = claude_wrapper.ClaudeWrapper(client, organizations[0]['uuid'])
+organizations = client.get_organizations()
+# You can omit passing in the organization uuid and the wrapper will assume
+# you will use the first organization instead.
+claude_obj = claude_wrapper.ClaudeWrapper(client, organization_uuid=organizations[0]['uuid'])
 ```
 
 #### Starting a new conversation
 ```py
 conversation_uuid = claude_obj.start_new_conversation("New Conversation", "Hi Claude!")
 ```
 
@@ -142,11 +157,8 @@
 #### Get conversation history
 ```py
 conversation_history = claude_obj.get_conversation_info(conversation_uuid = conversation_uuid)
 ```
 
 
 ## Disclaimer
-This library is UNOFFICIAL and you might get banned for using it. I am not responsible if your account gets banned. If you would like to use the actual API, go to the [anthropic website](https://docs.anthropic.com/claude/docs).
-
-Its also under active development and is extremely unstable, so there are no guarantees it will work for you. If you find a bug or you think it should work in a scenario where it doesn't, file an issue.
-
+This library is for purely educational purposes and is UNOFFICIAL. I am not responsible if your account gets banned. If you would like to use the actual API, go to [anthropic website](https://docs.anthropic.com/claude/docs).
```

### Comparing `claude-api-py-0.0.2/README.md` & `claude-api-py-0.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,58 @@
 # Unofficial Claude API For Python
 
 The UNOFFICIAL free API for Anthropic's Claude LLM.
 
+## Background
+
+Claude is [Anthropic's](https://www.anthropic.com/) LLM app (similar to ChatGPT). This library allows you to use the API (for free) and interact with it in your python projects.
+
 ## Implemented actions:
 The Unofficial Claude API is under active development. The following endpoints are usable in some capacity:
 
 - Getting organizations you're in
 - Getting conversations you're in
 - Starting a conversation
-- Sending a message and receiving a response (can't send files yet)
+- Sending a message and receiving a response
 - Delete a conversation
 - Create an attachment from a file
 - Send attachments
+- getting message history
 
 Note that the api is __**synchronous**__.
 
 ## TODO features
+- Tests
 - Fixing models OTHER than `claude_2`
 - asynchronous mode
 - Better caching
 - cleaner errors and passing these up to users
 
 
+This project is under active development and is extremely unstable, so there are no guarantees it will work for you. If you find a bug or you think it should work in a scenario where it doesn't, file an issue.
+
+
 ## Usage
 
 ### Step 1
 Install the library using the following:
 ```
-pip install rev-claude-api
+pip install claude-api-py
 ```
 
 If that doesn't work, you can install directly from this github repository:
 
 ```
 pip install git+git://github.com/AshwinPathi/claude-api-py.git
 ```
 
+There is one requirement as of now:
+- `sseclient-py` [link here](https://github.com/mpetazzoni/sseclient)
+
+
 ### Step 2
 Get a `sessionKey` from the Claude website. You will need this to start the bot. Ideally also have a user agent of the computer you use to access claude.
 
 You can get this information by logging into `https://claude.ai/chats` and doing the following:
 
 1. open inspect element (f12 on chrome)
 2. On the top bar, go to the `Application` tab.
@@ -64,17 +77,19 @@
 # context. This allows you to use the API more ergonomically.
 from claude import claude_wrapper
 ```
 
 #### Create the client and wrapper
 ```py
 client = claude_client.ClaudeClient(SESSION_KEY)
-organizations = client.get_organizations()
 
-claude_obj = claude_wrapper.ClaudeWrapper(client, organizations[0]['uuid'])
+organizations = client.get_organizations()
+# You can omit passing in the organization uuid and the wrapper will assume
+# you will use the first organization instead.
+claude_obj = claude_wrapper.ClaudeWrapper(client, organization_uuid=organizations[0]['uuid'])
 ```
 
 #### Starting a new conversation
 ```py
 conversation_uuid = claude_obj.start_new_conversation("New Conversation", "Hi Claude!")
 ```
 
@@ -122,11 +137,8 @@
 #### Get conversation history
 ```py
 conversation_history = claude_obj.get_conversation_info(conversation_uuid = conversation_uuid)
 ```
 
 
 ## Disclaimer
-This library is UNOFFICIAL and you might get banned for using it. I am not responsible if your account gets banned. If you would like to use the actual API, go to the [anthropic website](https://docs.anthropic.com/claude/docs).
-
-Its also under active development and is extremely unstable, so there are no guarantees it will work for you. If you find a bug or you think it should work in a scenario where it doesn't, file an issue.
-
+This library is for purely educational purposes and is UNOFFICIAL. I am not responsible if your account gets banned. If you would like to use the actual API, go to [anthropic website](https://docs.anthropic.com/claude/docs).
```

### Comparing `claude-api-py-0.0.2/claude/claude_client.py` & `claude-api-py-0.0.3/claude/claude_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Helper class to access Claude APIs via raw json."""
 import json
 import pathlib
-from pathlib import Path
 from typing import List, Optional, Iterator, Union
 
 
 from claude import constants
 from claude import custom_requests
 from claude import helpers
 from claude.custom_types import JsonType, HeaderType, AttachmentType
```

### Comparing `claude-api-py-0.0.2/claude/claude_wrapper.py` & `claude-api-py-0.0.3/claude/claude_wrapper.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from dataclasses import dataclass
 from typing import Optional, List
 import uuid
 
 from claude import constants
 from claude import claude_client
 from claude.custom_types import JsonType, AttachmentType
 
@@ -11,17 +10,24 @@
     """Wrapper around the raw API that makes it easy to talk in a given organization.
 
     Takes in a Claude Client and the organization that the client should use. Can optionally
     `switch conversation contexts` to persist a certain conversation uuid and omit passing
     in a conversation uuid on every method call.
     """
 
-    def __init__(self, client: claude_client.ClaudeClient, organization_uuid: str):
+    def __init__(self, client: claude_client.ClaudeClient, organization_uuid: Optional[str] = None):
+        """Initialize the wrapper with a client and an optional organization_uuid. If an organization uuid
+        isn't provided, the wrapper will automatically use the first organization in the list of organizations
+        that the user is in.
+        """
         self._client = client
-        self._organization_uuid = organization_uuid
+        if organization_uuid is None:
+            self._organization_uuid = self._client.get_organizations()[0]['uuid']  # type: ignore
+        else:
+            self._organization_uuid = organization_uuid
 
         self._current_conversation = None
 
     ####################################################################
     #                                                                  #
     #                         Public APIs                              #
     #                                                                  #
@@ -61,19 +67,21 @@
         """
         return self._client.convert_file(self._organization_uuid, file_path)
 
     def start_new_conversation(
         self,
         conversation_name: str,
         initial_message: str,
+        initial_attachments: List[AttachmentType] = [],
         timezone: constants.Timezone = constants.Timezone.LA,
         model: constants.Model = constants.Model.CLAUDE_2,
     ) -> Optional[str]:
         """Creates a new conversation with |conversation_name| and initiates the conversation
-        with an initial message |initial_message|.
+        with an initial message |initial_message|, and optionally an initial set of attachments
+        in |initial_attachments|.
 
         Returns the newly generated conversation ID, if it didn't fail. Otherwise, returns None.
         """
         conversation_uuid = str(uuid.uuid4())
 
         # First, create the new conversation under the organization, and with the new conversation uuid.
         # If this doesn't work, return early.
@@ -84,15 +92,15 @@
             return None
 
         # Send the initial message to the newly created conversation.
         send_init_message_result = self._client.send_message(
             self._organization_uuid,
             conversation_uuid,
             initial_message,
-            [],
+            initial_attachments,
             timezone,
             model,
             stream=False,
         )
         if send_init_message_result is None:
             return None
 
@@ -138,15 +146,18 @@
         if conversation_to_use is None:
             return None
         return self._client.get_conversation_info(
             self._organization_uuid, conversation_to_use
         )
 
     def delete_all_conversations(self) -> List[str]:
-        """Deletes all the conversations in the organization."""
+        """Deletes all the conversations in the organization. Returns a list of conversations uuids
+        that the client failed to delete. In the case that all conversations were deleted correctly,
+        this should return an empty list.
+        """
         failed_deletion = []
         conversations = self._client.get_conversations_from_org(self._organization_uuid)
         for conversation in conversations:  # type: ignore
             if not self.delete_conversation(conversation["uuid"]):
                 failed_deletion.append(conversation["uuid"])
         return failed_deletion
 
@@ -177,14 +188,27 @@
         """
         self._current_conversation = conversation_uuid
 
     def clear_conversation_context(self) -> None:
         """Clears the current conversation context."""
         self._current_conversation = None
 
+    def switch_client(self, new_client: claude_client.ClaudeClient, organization_uuid: Optional[str] = None) -> None:
+        """Switches the current client to a new client. Can optionally provide an |organization_uuid|,
+        otherwise we will infer the organization uuid to be the first uuid in the list or organizations
+        that the client is in.
+        """
+        self._client = new_client
+        if organization_uuid is None:
+            self._organization_uuid = self._client.get_organizations()[0]['uuid']  # type: ignore
+        else:
+            self._organization_uuid = organization_uuid
+
+        self._current_conversation = None        
+
     ####################################################################
     #                                                                  #
     #                       Helper Methods                             #
     #                                                                  #
     ####################################################################
 
     def _get_conversation_or_context(
```

### Comparing `claude-api-py-0.0.2/claude/constants.py` & `claude-api-py-0.0.3/claude/constants.py`

 * *Files identical despite different names*

### Comparing `claude-api-py-0.0.2/claude/custom_requests.py` & `claude-api-py-0.0.3/claude/custom_requests.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Claude API protections.
 """
 from dataclasses import dataclass
 import uuid
 import io
 import json
 import mimetypes
-from typing import Optional, Union, Iterator, Dict, Tuple
+from typing import Optional, Union, Iterator, Tuple
 from urllib.request import Request, urlopen
 from urllib.error import HTTPError, URLError
 
 import sseclient
 
 from claude.custom_types import JsonType, HeaderType, FormDataType
 
@@ -29,14 +29,16 @@
 class Response:
     """Wrapper for the return type for all custom requests methods.
     Acts as a loose wrapper around requests.Response.
     """
 
     ok: bool
     data: Union[bytes, str]
+    status_code: Optional[int]
+    error: Optional[str]
 
     def json(self) -> JsonType:
         if isinstance(self.data, str):
             return json.loads(self.data)
         elif isinstance(self.data, bytes):
             return json.loads(self.data.decode("utf-8"))
         else:
@@ -169,24 +171,23 @@
     url: str, headers: HeaderType, request_body: Optional[Union[JsonType, bytes]] = None
 ) -> Response:
     """Public method for a POST Request."""
     request = Request(url, method="POST")
     for header_key, header_value in headers.items():
         request.add_header(header_key, header_value)
 
-    if request_body is None:
-        return _safe_request_read(request)
 
-    # If its already encoded in bytes, don't bother encoding it.
-    if isinstance(request_body, bytes):
-        return _safe_request_read(request, data=request_body)
-    if isinstance(request_body, str):
-        return _safe_request_read(request, data=request_body.encode())
-
-    encoded_request_body = json.dumps(request_body).encode()
+    encoded_request_body = None
+    if request_body is not None:
+        if isinstance(request_body, bytes):
+            encoded_request_body = request_body
+        elif isinstance(request_body, str):
+            encoded_request_body = request_body.encode()
+        else:
+            encoded_request_body = json.dumps(request_body).encode()
     return _safe_request_read(request, data=encoded_request_body)
 
 
 def sse(
     url: str, headers: HeaderType, request_body: Optional[JsonType] = None
 ) -> Iterator[str]:
     """Public method for a POST request that requires SSE."""
@@ -210,21 +211,17 @@
     for header_key, header_value in headers.items():
         request.add_header(header_key, header_value)
 
     return _safe_request_read(request)
 
 
 def _safe_request_read(request: Request, data: Optional[bytes] = None) -> Response:
-    """Read a request with some data and return the response."""
-    if data is not None:
-        try:
-            with urlopen(request, data=data) as response:
-                return Response(ok=True, data=response.read())
-        except (HTTPError, URLError) as e:
-            print(e)
-            return Response(ok=False, data=b"")
+    """Read a request with some data and return the response. Handles packaging
+    the response in a Response Wrapper object.
+    """
+    status_code = None
     try:
-        with urlopen(request) as response:
-            return Response(ok=True, data=response.read())
+        with urlopen(request, data=data) as response:
+            status_code = response.getcode()
+            return Response(ok=True, data=response.read(), status_code=status_code, error=None)
     except (HTTPError, URLError) as e:
-        print(e)
-        return Response(ok=False, data=b"")
+        return Response(ok=False, data=b"", status_code=status_code, error=str(e))
```

### Comparing `claude-api-py-0.0.2/claude/custom_types.py` & `claude-api-py-0.0.3/claude/custom_types.py`

 * *Files identical despite different names*

### Comparing `claude-api-py-0.0.2/claude/helpers.py` & `claude-api-py-0.0.3/claude/helpers.py`

 * *Files identical despite different names*

### Comparing `claude-api-py-0.0.2/claude_api_py.egg-info/PKG-INFO` & `claude-api-py-0.0.3/claude_api_py.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claude-api-py
-Version: 0.0.2
+Version: 0.0.3
 Summary: Unofficial Anthropic Claude API for Python3.
 Home-page: https://github.com/AshwinPathi/claude-api-py
 License: MIT
 Keywords: llm,claude,api,gpt
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -18,48 +18,61 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Unofficial Claude API For Python
 
 The UNOFFICIAL free API for Anthropic's Claude LLM.
 
+## Background
+
+Claude is [Anthropic's](https://www.anthropic.com/) LLM app (similar to ChatGPT). This library allows you to use the API (for free) and interact with it in your python projects.
+
 ## Implemented actions:
 The Unofficial Claude API is under active development. The following endpoints are usable in some capacity:
 
 - Getting organizations you're in
 - Getting conversations you're in
 - Starting a conversation
-- Sending a message and receiving a response (can't send files yet)
+- Sending a message and receiving a response
 - Delete a conversation
 - Create an attachment from a file
 - Send attachments
+- getting message history
 
 Note that the api is __**synchronous**__.
 
 ## TODO features
+- Tests
 - Fixing models OTHER than `claude_2`
 - asynchronous mode
 - Better caching
 - cleaner errors and passing these up to users
 
 
+This project is under active development and is extremely unstable, so there are no guarantees it will work for you. If you find a bug or you think it should work in a scenario where it doesn't, file an issue.
+
+
 ## Usage
 
 ### Step 1
 Install the library using the following:
 ```
-pip install rev-claude-api
+pip install claude-api-py
 ```
 
 If that doesn't work, you can install directly from this github repository:
 
 ```
 pip install git+git://github.com/AshwinPathi/claude-api-py.git
 ```
 
+There is one requirement as of now:
+- `sseclient-py` [link here](https://github.com/mpetazzoni/sseclient)
+
+
 ### Step 2
 Get a `sessionKey` from the Claude website. You will need this to start the bot. Ideally also have a user agent of the computer you use to access claude.
 
 You can get this information by logging into `https://claude.ai/chats` and doing the following:
 
 1. open inspect element (f12 on chrome)
 2. On the top bar, go to the `Application` tab.
@@ -84,17 +97,19 @@
 # context. This allows you to use the API more ergonomically.
 from claude import claude_wrapper
 ```
 
 #### Create the client and wrapper
 ```py
 client = claude_client.ClaudeClient(SESSION_KEY)
-organizations = client.get_organizations()
 
-claude_obj = claude_wrapper.ClaudeWrapper(client, organizations[0]['uuid'])
+organizations = client.get_organizations()
+# You can omit passing in the organization uuid and the wrapper will assume
+# you will use the first organization instead.
+claude_obj = claude_wrapper.ClaudeWrapper(client, organization_uuid=organizations[0]['uuid'])
 ```
 
 #### Starting a new conversation
 ```py
 conversation_uuid = claude_obj.start_new_conversation("New Conversation", "Hi Claude!")
 ```
 
@@ -142,11 +157,8 @@
 #### Get conversation history
 ```py
 conversation_history = claude_obj.get_conversation_info(conversation_uuid = conversation_uuid)
 ```
 
 
 ## Disclaimer
-This library is UNOFFICIAL and you might get banned for using it. I am not responsible if your account gets banned. If you would like to use the actual API, go to the [anthropic website](https://docs.anthropic.com/claude/docs).
-
-Its also under active development and is extremely unstable, so there are no guarantees it will work for you. If you find a bug or you think it should work in a scenario where it doesn't, file an issue.
-
+This library is for purely educational purposes and is UNOFFICIAL. I am not responsible if your account gets banned. If you would like to use the actual API, go to [anthropic website](https://docs.anthropic.com/claude/docs).
```

### Comparing `claude-api-py-0.0.2/setup.py` & `claude-api-py-0.0.3/setup.py`

 * *Files identical despite different names*

