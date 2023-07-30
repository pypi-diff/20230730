# Comparing `tmp/claude-api-1.0.8.tar.gz` & `tmp/claude-api-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "claude-api-1.0.8.tar", last modified: Wed Jul 19 02:49:03 2023, max compression
+gzip compressed data, was "claude-api-1.0.9.tar", last modified: Sat Jul 22 01:34:39 2023, max compression
```

## Comparing `claude-api-1.0.8.tar` & `claude-api-1.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 02:49:03.794245 claude-api-1.0.8/
--rw-rw-rw-   0        0        0     1094 2023-07-19 02:35:24.000000 claude-api-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     4698 2023-07-19 02:49:03.794245 claude-api-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3880 2023-07-19 02:35:24.000000 claude-api-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 02:49:03.778874 claude-api-1.0.8/claude-api/
-drwxrwxrwx   0        0        0        0 2023-07-19 02:49:03.792933 claude-api-1.0.8/claude-api/claude_api.egg-info/
--rw-rw-rw-   0        0        0     4698 2023-07-19 02:49:03.000000 claude-api-1.0.8/claude-api/claude_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-07-19 02:49:03.000000 claude-api-1.0.8/claude-api/claude_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 02:49:03.000000 claude-api-1.0.8/claude-api/claude_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-19 02:49:03.000000 claude-api-1.0.8/claude-api/claude_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-19 02:49:03.000000 claude-api-1.0.8/claude-api/claude_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7487 2023-07-19 02:48:51.000000 claude-api-1.0.8/claude-api/claude_api.py
--rw-rw-rw-   0        0        0       42 2023-07-19 02:49:03.794245 claude-api-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1258 2023-07-19 02:48:10.000000 claude-api-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 01:34:39.269087 claude-api-1.0.9/
+-rw-rw-rw-   0        0        0     1094 2023-07-22 01:33:47.000000 claude-api-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     5806 2023-07-22 01:34:39.269087 claude-api-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4988 2023-07-22 01:33:47.000000 claude-api-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-22 01:34:39.253136 claude-api-1.0.9/claude-api/
+drwxrwxrwx   0        0        0        0 2023-07-22 01:34:39.265505 claude-api-1.0.9/claude-api/claude_api.egg-info/
+-rw-rw-rw-   0        0        0     5806 2023-07-22 01:34:39.000000 claude-api-1.0.9/claude-api/claude_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-07-22 01:34:39.000000 claude-api-1.0.9/claude-api/claude_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 01:34:39.000000 claude-api-1.0.9/claude-api/claude_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-22 01:34:39.000000 claude-api-1.0.9/claude-api/claude_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-22 01:34:39.000000 claude-api-1.0.9/claude-api/claude_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9407 2023-07-22 01:33:47.000000 claude-api-1.0.9/claude-api/claude_api.py
+-rw-rw-rw-   0        0        0       42 2023-07-22 01:34:39.273122 claude-api-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1258 2023-07-22 01:33:47.000000 claude-api-1.0.9/setup.py
```

### Comparing `claude-api-1.0.8/LICENSE` & `claude-api-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `claude-api-1.0.8/PKG-INFO` & `claude-api-1.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claude-api
-Version: 1.0.8
+Version: 1.0.9
 Summary: An unofficial API for Claude AI, allowing users to access and interact with Claude AII
 Home-page: https://github.com/KoushikNavuluri/Claude-API/
 Author: Koushik
 Author-email: koushikk@outlook.com
 License: MIT
 Keywords: claude,ai,claude-ai,API,requests,chatbot
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,14 +18,31 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Claude AI-API ( Unofficial )
 This project provides an unofficial API for Claude AI, allowing users to access and interact with Claude AI .
 
+## Table of contents
+
+  * [Use Cases](#use-cases)
+  * [Prerequisites](#prerequisites)
+  * [Installation](#installation)
+  * [Usage](#usage)
+  * [List All Conversations](#list-all-conversations)
+  * [Send Message](#send-message)
+  * [Send Message with attachment](#send-message-with-attachment)
+  * [Delete Conversation](#delete-conversation)
+  * [Chat Conversation History](#chat-conversation-history)
+  * [Create New Chat](#create-new-chat)
+  * [Reset All Conversations](#reset-all-conversations)
+  * [Rename Chat](#rename-chat)
+  * [Disclaimer](#disclaimer)
+
+
 ## Use Cases 
 
     1. Python Console ChatBot ( Check in usecases folder for sample console chatbot )
 
     2. Discord Chatbot   
     
     3. Many more can be done....
@@ -42,14 +59,20 @@
 
 ```
 
 ## Installation
 
 To use the Claude AI Unofficial API, you can either clone the GitHub repository or directly download the Python file.
 
+Terminal :
+
+    pip install claude-api
+    
+or
+
 Clone the repository:
 
     git clone https://github.com/KoushikNavuluri/Claude-API.git
 
 ## Usage
 
 
@@ -62,17 +85,16 @@
 * You can get cookie from the browser's developer tools network tab ( see for any claude.ai requests check out cookie ,copy whole value ) or storage tab ( You can find cookie of claude.ai ,there will be four values )
 
 * (Checkout below image for the format of cookie ,It is Better to Use from network tab to grab cookie easily )
 
    ![Screenshot (8)](https://github.com/KoushikNavuluri/Claude-API/assets/103725723/355971e3-f46c-47fc-a3cf-008bb55bb4c6)
 
 
-        cookie = os.environ.get('cookie')
-    
-        claude_api = Client(cookie)
+      cookie = os.environ.get('cookie')
+      claude_api = Client(cookie)
 
 ## List All Conversations
 
 To list all the conversation Id's you had with Claude , you can use the list_all_conversations method:
 
     conversations = claude_api.list_all_conversations()
     for conversation in conversations:
@@ -82,18 +104,29 @@
 ## Send Message
 
 To send a message to Claude, you can use the send_message method. You need to provide the prompt and the conversation ID:
 
 
 
     prompt = "Hello, Claude!"
-    conversation_id = "<conversation_id>"
+    conversation_id = "<conversation_id>" or client.create_new_chat()['uuid']
     response = claude_api.send_message(prompt, conversation_id)
     print(response)
 
+## Send Message with attachment
+
+You can send any type of attachment to claude to get responses using attachment argument in send_message().
+Note: Claude currently supports only some file types.
+
+    prompt = "Hey,Summarize me this document.!"
+    conversation_id = "<conversation_id>" or client.create_new_chat()['uuid']
+    response = claude_api.send_message(prompt, conversation_id,attachment="path/to/file.pdf")
+    print(response)
+
+
 ## Delete Conversation
 
 To delete a conversation, you can use the delete_conversation method:
 
 
     conversation_id = "<conversation_id>"
     deleted = claude_api.delete_conversation(conversation_id)
```

### Comparing `claude-api-1.0.8/README.md` & `claude-api-1.0.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,27 @@
 # Claude AI-API ( Unofficial )
 This project provides an unofficial API for Claude AI, allowing users to access and interact with Claude AI .
 
+## Table of contents
+
+  * [Use Cases](#use-cases)
+  * [Prerequisites](#prerequisites)
+  * [Installation](#installation)
+  * [Usage](#usage)
+  * [List All Conversations](#list-all-conversations)
+  * [Send Message](#send-message)
+  * [Send Message with attachment](#send-message-with-attachment)
+  * [Delete Conversation](#delete-conversation)
+  * [Chat Conversation History](#chat-conversation-history)
+  * [Create New Chat](#create-new-chat)
+  * [Reset All Conversations](#reset-all-conversations)
+  * [Rename Chat](#rename-chat)
+  * [Disclaimer](#disclaimer)
+
+
 ## Use Cases 
 
     1. Python Console ChatBot ( Check in usecases folder for sample console chatbot )
 
     2. Discord Chatbot   
     
     3. Many more can be done....
@@ -21,14 +38,20 @@
 
 ```
 
 ## Installation
 
 To use the Claude AI Unofficial API, you can either clone the GitHub repository or directly download the Python file.
 
+Terminal :
+
+    pip install claude-api
+    
+or
+
 Clone the repository:
 
     git clone https://github.com/KoushikNavuluri/Claude-API.git
 
 ## Usage
 
 
@@ -41,17 +64,16 @@
 * You can get cookie from the browser's developer tools network tab ( see for any claude.ai requests check out cookie ,copy whole value ) or storage tab ( You can find cookie of claude.ai ,there will be four values )
 
 * (Checkout below image for the format of cookie ,It is Better to Use from network tab to grab cookie easily )
 
    ![Screenshot (8)](https://github.com/KoushikNavuluri/Claude-API/assets/103725723/355971e3-f46c-47fc-a3cf-008bb55bb4c6)
 
 
-        cookie = os.environ.get('cookie')
-    
-        claude_api = Client(cookie)
+      cookie = os.environ.get('cookie')
+      claude_api = Client(cookie)
 
 ## List All Conversations
 
 To list all the conversation Id's you had with Claude , you can use the list_all_conversations method:
 
     conversations = claude_api.list_all_conversations()
     for conversation in conversations:
@@ -61,18 +83,29 @@
 ## Send Message
 
 To send a message to Claude, you can use the send_message method. You need to provide the prompt and the conversation ID:
 
 
 
     prompt = "Hello, Claude!"
-    conversation_id = "<conversation_id>"
+    conversation_id = "<conversation_id>" or client.create_new_chat()['uuid']
     response = claude_api.send_message(prompt, conversation_id)
     print(response)
 
+## Send Message with attachment
+
+You can send any type of attachment to claude to get responses using attachment argument in send_message().
+Note: Claude currently supports only some file types.
+
+    prompt = "Hey,Summarize me this document.!"
+    conversation_id = "<conversation_id>" or client.create_new_chat()['uuid']
+    response = claude_api.send_message(prompt, conversation_id,attachment="path/to/file.pdf")
+    print(response)
+
+
 ## Delete Conversation
 
 To delete a conversation, you can use the delete_conversation method:
 
 
     conversation_id = "<conversation_id>"
     deleted = claude_api.delete_conversation(conversation_id)
```

### Comparing `claude-api-1.0.8/claude-api/claude_api.egg-info/PKG-INFO` & `claude-api-1.0.9/claude-api/claude_api.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claude-api
-Version: 1.0.8
+Version: 1.0.9
 Summary: An unofficial API for Claude AI, allowing users to access and interact with Claude AII
 Home-page: https://github.com/KoushikNavuluri/Claude-API/
 Author: Koushik
 Author-email: koushikk@outlook.com
 License: MIT
 Keywords: claude,ai,claude-ai,API,requests,chatbot
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,14 +18,31 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Claude AI-API ( Unofficial )
 This project provides an unofficial API for Claude AI, allowing users to access and interact with Claude AI .
 
+## Table of contents
+
+  * [Use Cases](#use-cases)
+  * [Prerequisites](#prerequisites)
+  * [Installation](#installation)
+  * [Usage](#usage)
+  * [List All Conversations](#list-all-conversations)
+  * [Send Message](#send-message)
+  * [Send Message with attachment](#send-message-with-attachment)
+  * [Delete Conversation](#delete-conversation)
+  * [Chat Conversation History](#chat-conversation-history)
+  * [Create New Chat](#create-new-chat)
+  * [Reset All Conversations](#reset-all-conversations)
+  * [Rename Chat](#rename-chat)
+  * [Disclaimer](#disclaimer)
+
+
 ## Use Cases 
 
     1. Python Console ChatBot ( Check in usecases folder for sample console chatbot )
 
     2. Discord Chatbot   
     
     3. Many more can be done....
@@ -42,14 +59,20 @@
 
 ```
 
 ## Installation
 
 To use the Claude AI Unofficial API, you can either clone the GitHub repository or directly download the Python file.
 
+Terminal :
+
+    pip install claude-api
+    
+or
+
 Clone the repository:
 
     git clone https://github.com/KoushikNavuluri/Claude-API.git
 
 ## Usage
 
 
@@ -62,17 +85,16 @@
 * You can get cookie from the browser's developer tools network tab ( see for any claude.ai requests check out cookie ,copy whole value ) or storage tab ( You can find cookie of claude.ai ,there will be four values )
 
 * (Checkout below image for the format of cookie ,It is Better to Use from network tab to grab cookie easily )
 
    ![Screenshot (8)](https://github.com/KoushikNavuluri/Claude-API/assets/103725723/355971e3-f46c-47fc-a3cf-008bb55bb4c6)
 
 
-        cookie = os.environ.get('cookie')
-    
-        claude_api = Client(cookie)
+      cookie = os.environ.get('cookie')
+      claude_api = Client(cookie)
 
 ## List All Conversations
 
 To list all the conversation Id's you had with Claude , you can use the list_all_conversations method:
 
     conversations = claude_api.list_all_conversations()
     for conversation in conversations:
@@ -82,18 +104,29 @@
 ## Send Message
 
 To send a message to Claude, you can use the send_message method. You need to provide the prompt and the conversation ID:
 
 
 
     prompt = "Hello, Claude!"
-    conversation_id = "<conversation_id>"
+    conversation_id = "<conversation_id>" or client.create_new_chat()['uuid']
     response = claude_api.send_message(prompt, conversation_id)
     print(response)
 
+## Send Message with attachment
+
+You can send any type of attachment to claude to get responses using attachment argument in send_message().
+Note: Claude currently supports only some file types.
+
+    prompt = "Hey,Summarize me this document.!"
+    conversation_id = "<conversation_id>" or client.create_new_chat()['uuid']
+    response = claude_api.send_message(prompt, conversation_id,attachment="path/to/file.pdf")
+    print(response)
+
+
 ## Delete Conversation
 
 To delete a conversation, you can use the delete_conversation method:
 
 
     conversation_id = "<conversation_id>"
     deleted = claude_api.delete_conversation(conversation_id)
```

### Comparing `claude-api-1.0.8/claude-api/claude_api.py` & `claude-api-1.0.9/claude-api/claude_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,122 +8,144 @@
 
   def __init__(self, cookie):
     self.cookie = cookie
     self.organization_id = self.get_organization_id()
 
   def get_organization_id(self):
     url = "https://claude.ai/api/organizations"
-  
+
     headers = {
-      'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/115.0',
-      'Accept': '*/*',
-      'Accept-Language': 'en-US,en;q=0.5',
-      'Referer': 'https://claude.ai/chats',
-      'Content-Type': 'application/json',
-      'Sec-Fetch-Dest': 'empty',
-      'Sec-Fetch-Mode': 'cors',
-      'Sec-Fetch-Site': 'same-origin',
-      'Connection': 'keep-alive',
-      'Cookie': f'{self.cookie}'
+        'User-Agent':
+        'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/115.0',
+        'Accept-Language': 'en-US,en;q=0.5',
+        'Referer': 'https://claude.ai/chats',
+        'Content-Type': 'application/json',
+        'Sec-Fetch-Dest': 'empty',
+        'Sec-Fetch-Mode': 'cors',
+        'Sec-Fetch-Site': 'same-origin',
+        'Connection': 'keep-alive',
+        'Cookie': f'{self.cookie}'
     }
-  
+
     response = requests.request("GET", url, headers=headers)
     res = json.loads(response.text)
     uuid = res[0]['uuid']
-  
+
     return uuid
 
+  def get_content_type(self, file_path):
+    # Function to determine content type based on file extension
+    extension = os.path.splitext(file_path)[-1].lower()
+    if extension == '.pdf':
+      return 'application/pdf'
+    elif extension == '.txt':
+      return 'text/plain'
+    elif extension == '.csv':
+      return 'text/csv'
+    # Add more content types as needed for other file types
+    else:
+      return 'application/octet-stream'
+
   # Lists all the conversations you had with Claude
   def list_all_conversations(self):
     url = f"https://claude.ai/api/organizations/{self.organization_id}/chat_conversations"
 
     headers = {
-      'User-Agent':
-      'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/115.0',
-      'Accept-Language': 'en-US,en;q=0.5',
-      'Referer': 'https://claude.ai/chats',
-      'Content-Type': 'application/json',
-      'Sec-Fetch-Dest': 'empty',
-      'Sec-Fetch-Mode': 'cors',
-      'Sec-Fetch-Site': 'same-origin',
-      'Connection': 'keep-alive',
-      'Cookie': f'{self.cookie}'
+        'User-Agent':
+        'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/115.0',
+        'Accept-Language': 'en-US,en;q=0.5',
+        'Referer': 'https://claude.ai/chats',
+        'Content-Type': 'application/json',
+        'Sec-Fetch-Dest': 'empty',
+        'Sec-Fetch-Mode': 'cors',
+        'Sec-Fetch-Site': 'same-origin',
+        'Connection': 'keep-alive',
+        'Cookie': f'{self.cookie}'
     }
 
     response = requests.get(url, headers=headers)
     conversations = response.json()
 
     # Returns all conversation information in a list
     if response.status_code == 200:
       return conversations
     else:
       print(f"Error: {response.status_code} - {response.text}")
 
   # Send Message to Claude
-  def send_message(self, prompt, conversation_id):
+  def send_message(self,  prompt, conversation_id,attachment=None):
     url = "https://claude.ai/api/append_message"
 
+    # Upload attachment if provided
+    attachments = []
+    if attachment:
+      attachment_response = self.upload_attachment(attachment)
+      if attachment_response:
+        attachments = attachment_response
+      else:
+        return {"Error: Invalid file format .Please try again."}
+        
+
     payload = json.dumps({
-      "completion": {
-        "prompt": f"{prompt}",
-        "timezone": "Asia/Kolkata",
-        "model": "claude-2"
-      },
-      "organization_uuid": f"{self.organization_id}",
-      "conversation_uuid": f"{conversation_id}",
-      "text": f"{prompt}",
-      "attachments": []
+        "completion": {
+            "prompt": f"{prompt}",
+            "timezone": "Asia/Kolkata",
+            "model": "claude-2"
+        },
+        "organization_uuid": f"{self.organization_id}",
+        "conversation_uuid": f"{conversation_id}",
+        "text": f"{prompt}",
+        "attachments": [attachments]
     })
+
     headers = {
-      'User-Agent':
-      'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/115.0',
-      'Accept': 'text/event-stream, text/event-stream',
-      'Accept-Language': 'en-US,en;q=0.5',
-      'Referer': 'https://claude.ai/chats',
-      'Content-Type': 'application/json',
-      'Origin': 'https://claude.ai',
-      'DNT': '1',
-      'Connection': 'keep-alive',
-      'Cookie': f'{self.cookie}',
-      'Sec-Fetch-Dest': 'empty',
-      'Sec-Fetch-Mode': 'cors',
-      'Sec-Fetch-Site': 'same-origin',
-      'TE': 'trailers'
+        'User-Agent':
+        'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/115.0',
+        'Accept': 'text/event-stream, text/event-stream',
+        'Accept-Language': 'en-US,en;q=0.5',
+        'Referer': 'https://claude.ai/chats',
+        'Content-Type': 'application/json',
+        'Origin': 'https://claude.ai',
+        'DNT': '1',
+        'Connection': 'keep-alive',
+        'Cookie': f'{self.cookie}',
+        'Sec-Fetch-Dest': 'empty',
+        'Sec-Fetch-Mode': 'cors',
+        'Sec-Fetch-Site': 'same-origin',
+        'TE': 'trailers'
     }
 
     response = requests.post(url, headers=headers, data=payload, stream=True)
-
     decoded_data = response.content.decode("utf-8")
     data = decoded_data.strip().split('\n')[-1]
 
     answer = {"answer": json.loads(data[6:])['completion']}['answer']
 
     # Returns answer
     return answer
 
   # Deletes the conversation
   def delete_conversation(self, conversation_id):
     url = f"https://claude.ai/api/organizations/{self.organization_id}/chat_conversations/{conversation_id}"
 
     payload = json.dumps(f"{conversation_id}")
     headers = {
-      'User-Agent':
-      'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/115.0',
-      'Accept': '*/*',
-      'Accept-Language': 'en-US,en;q=0.5',
-      'Content-Type': 'application/json',
-      'Content-Length': '38',
-      'Referer': 'https://claude.ai/chats',
-      'Origin': 'https://claude.ai',
-      'Sec-Fetch-Dest': 'empty',
-      'Sec-Fetch-Mode': 'cors',
-      'Sec-Fetch-Site': 'same-origin',
-      'Connection': 'keep-alive',
-      'Cookie': f'{self.cookie}',
-      'TE': 'trailers'
+        'User-Agent':
+        'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/115.0',
+        'Accept-Language': 'en-US,en;q=0.5',
+        'Content-Type': 'application/json',
+        'Content-Length': '38',
+        'Referer': 'https://claude.ai/chats',
+        'Origin': 'https://claude.ai',
+        'Sec-Fetch-Dest': 'empty',
+        'Sec-Fetch-Mode': 'cors',
+        'Sec-Fetch-Site': 'same-origin',
+        'Connection': 'keep-alive',
+        'Cookie': f'{self.cookie}',
+        'TE': 'trailers'
     }
 
     response = requests.request("DELETE", url, headers=headers, data=payload)
 
     # Returns True if deleted or False if any error in deleting
     if response.status_code == 204:
       return True
@@ -131,59 +153,57 @@
       return False
 
   # Returns all the messages in conversation
   def chat_conversation_history(self, conversation_id):
     url = f"https://claude.ai/api/organizations/{self.organization_id}/chat_conversations/{conversation_id}"
 
     headers = {
-      'User-Agent':
-      'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/115.0',
-      'Accept-Language': 'en-US,en;q=0.5',
-      'Referer': 'https://claude.ai/chats',
-      'Content-Type': 'application/json',
-      'Sec-Fetch-Dest': 'empty',
-      'Sec-Fetch-Mode': 'cors',
-      'Sec-Fetch-Site': 'same-origin',
-      'Connection': 'keep-alive',
-      'Cookie': f'{self.cookie}'
+        'User-Agent':
+        'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/115.0',
+        'Accept-Language': 'en-US,en;q=0.5',
+        'Referer': 'https://claude.ai/chats',
+        'Content-Type': 'application/json',
+        'Sec-Fetch-Dest': 'empty',
+        'Sec-Fetch-Mode': 'cors',
+        'Sec-Fetch-Site': 'same-origin',
+        'Connection': 'keep-alive',
+        'Cookie': f'{self.cookie}'
     }
 
     response = requests.request("GET", url, headers=headers)
     print(type(response))
 
     # List all the conversations in JSON
     return response.json()
 
   def generate_uuid(self):
     random_uuid = uuid.uuid4()
     random_uuid_str = str(random_uuid)
     formatted_uuid = f"{random_uuid_str[0:8]}-{random_uuid_str[9:13]}-{random_uuid_str[14:18]}-{random_uuid_str[19:23]}-{random_uuid_str[24:]}"
     return formatted_uuid
 
-  
   def create_new_chat(self):
     url = f"https://claude.ai/api/organizations/{self.organization_id}/chat_conversations"
     uuid = self.generate_uuid()
 
     payload = json.dumps({"uuid": uuid, "name": ""})
     headers = {
-      'User-Agent':
-      'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/115.0',
-      'Accept': '*/*',
-      'Accept-Language': 'en-US,en;q=0.5',
-      'Referer': 'https://claude.ai/chats',
-      'Content-Type': 'application/json',
-      'Origin': 'https://claude.ai',
-      'DNT': '1',
-      'Connection': 'keep-alive',
-      'Cookie': self.cookie,
-      'Sec-Fetch-Dest': 'empty',
-      'Sec-Fetch-Mode': 'cors',
-      'Sec-Fetch-Site': 'same-origin',
-      'TE': 'trailers'
+        'User-Agent':
+        'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/115.0',
+        'Accept-Language': 'en-US,en;q=0.5',
+        'Referer': 'https://claude.ai/chats',
+        'Content-Type': 'application/json',
+        'Origin': 'https://claude.ai',
+        'DNT': '1',
+        'Connection': 'keep-alive',
+        'Cookie': self.cookie,
+        'Sec-Fetch-Dest': 'empty',
+        'Sec-Fetch-Mode': 'cors',
+        'Sec-Fetch-Site': 'same-origin',
+        'TE': 'trailers'
     }
 
     response = requests.request("POST", url, headers=headers, data=payload)
 
     # Returns JSON of the newly created conversation information
     return response.json()
 
@@ -193,37 +213,70 @@
 
     for conversation in conversations:
       conversation_id = conversation['uuid']
       delete_id = self.delete_conversation(conversation_id)
 
     return True
 
+  def upload_attachment(self, file_path):
+    url = 'https://claude.ai/api/convert_document'
+    headers = {
+        'User-Agent':
+        'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/115.0',
+        'Accept-Language': 'en-US,en;q=0.5',
+        'Referer': 'https://claude.ai/chats',
+        'Origin': 'https://claude.ai',
+        'Sec-Fetch-Dest': 'empty',
+        'Sec-Fetch-Mode': 'cors',
+        'Sec-Fetch-Site': 'same-origin',
+        'Connection': 'keep-alive',
+        'Cookie': f'{self.cookie}',
+        'TE': 'trailers'
+    }
+
+    file_name = os.path.basename(file_path)
+    content_type = self.get_content_type(file_path)
+
+    files = {
+        'file': (file_name, open(file_path, 'rb'), content_type),
+        'orgUuid': (None, self.organization_id)
+    }
+
+    response = requests.post(url, headers=headers, files=files)
+    if response.status_code == 200:
+      return response.json()
+    else:
+      return False
+      
+
+    
   # Renames the chat conversation title
   def rename_chat(self, title, conversation_id):
     url = "https://claude.ai/api/rename_chat"
 
     payload = json.dumps({
-      "organization_uuid": f"{self.organization_id}",
-      "conversation_uuid": f"{conversation_id}",
-      "title": f"{title}"
+        "organization_uuid": f"{self.organization_id}",
+        "conversation_uuid": f"{conversation_id}",
+        "title": f"{title}"
     })
     headers = {
-      'User-Agent':
-      'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/115.0',
-      'Accept-Language': 'en-US,en;q=0.5',
-      'Content-Type': 'application/json',
-      'Referer': 'https://claude.ai/chats',
-      'Origin': 'https://claude.ai',
-      'Sec-Fetch-Dest': 'empty',
-      'Sec-Fetch-Mode': 'cors',
-      'Sec-Fetch-Site': 'same-origin',
-      'Connection': 'keep-alive',
-      'Cookie': f'{self.cookie}',
-      'TE': 'trailers'
+        'User-Agent':
+        'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/115.0',
+        'Accept-Language': 'en-US,en;q=0.5',
+        'Content-Type': 'application/json',
+        'Referer': 'https://claude.ai/chats',
+        'Origin': 'https://claude.ai',
+        'Sec-Fetch-Dest': 'empty',
+        'Sec-Fetch-Mode': 'cors',
+        'Sec-Fetch-Site': 'same-origin',
+        'Connection': 'keep-alive',
+        'Cookie': f'{self.cookie}',
+        'TE': 'trailers'
     }
 
     response = requests.request("POST", url, headers=headers, data=payload)
 
     if response.status_code == 200:
       return True
     else:
       return False
+
```

### Comparing `claude-api-1.0.8/setup.py` & `claude-api-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 base_path = Path(__file__).parent
 long_description = (base_path / "README.md").read_text()
 
 
 setup(
     name='claude-api', 
-    version='1.0.8',  
+    version='1.0.9',  
     author='Koushik',
     license="MIT",
     author_email='koushikk@outlook.com',
     description='An unofficial API for Claude AI, allowing users to access and interact with Claude AII',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/KoushikNavuluri/Claude-API/',
```

