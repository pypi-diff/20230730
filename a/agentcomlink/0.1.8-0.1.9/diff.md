# Comparing `tmp/agentcomlink-0.1.8.tar.gz` & `tmp/agentcomlink-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentcomlink-0.1.8.tar", last modified: Sat Jul 29 00:00:48 2023, max compression
+gzip compressed data, was "agentcomlink-0.1.9.tar", last modified: Sun Jul 30 00:01:10 2023, max compression
```

## Comparing `agentcomlink-0.1.8.tar` & `agentcomlink-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:00:48.431312 agentcomlink-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-29 00:00:38.000000 agentcomlink-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-07-29 00:00:48.431312 agentcomlink-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-29 00:00:38.000000 agentcomlink-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:00:48.431312 agentcomlink-0.1.8/agentcomlink/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-29 00:00:38.000000 agentcomlink-0.1.8/agentcomlink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 00:00:38.000000 agentcomlink-0.1.8/agentcomlink/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-29 00:00:38.000000 agentcomlink-0.1.8/agentcomlink/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-07-29 00:00:38.000000 agentcomlink-0.1.8/agentcomlink/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-07-29 00:00:38.000000 agentcomlink-0.1.8/agentcomlink/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:00:48.431312 agentcomlink-0.1.8/agentcomlink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-07-29 00:00:48.000000 agentcomlink-0.1.8/agentcomlink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-29 00:00:48.000000 agentcomlink-0.1.8/agentcomlink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 00:00:48.000000 agentcomlink-0.1.8/agentcomlink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-29 00:00:48.000000 agentcomlink-0.1.8/agentcomlink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-29 00:00:48.000000 agentcomlink-0.1.8/agentcomlink.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 00:00:48.431312 agentcomlink-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-29 00:00:38.000000 agentcomlink-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:01:10.098615 agentcomlink-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-30 00:00:55.000000 agentcomlink-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-07-30 00:01:10.098615 agentcomlink-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-30 00:00:55.000000 agentcomlink-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:01:10.098615 agentcomlink-0.1.9/agentcomlink/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-30 00:00:55.000000 agentcomlink-0.1.9/agentcomlink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 00:00:55.000000 agentcomlink-0.1.9/agentcomlink/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-30 00:00:55.000000 agentcomlink-0.1.9/agentcomlink/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-07-30 00:00:55.000000 agentcomlink-0.1.9/agentcomlink/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-07-30 00:00:55.000000 agentcomlink-0.1.9/agentcomlink/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 00:01:10.098615 agentcomlink-0.1.9/agentcomlink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-07-30 00:01:10.000000 agentcomlink-0.1.9/agentcomlink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-30 00:01:10.000000 agentcomlink-0.1.9/agentcomlink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 00:01:10.000000 agentcomlink-0.1.9/agentcomlink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-30 00:01:10.000000 agentcomlink-0.1.9/agentcomlink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-30 00:01:10.000000 agentcomlink-0.1.9/agentcomlink.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 00:01:10.098615 agentcomlink-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-30 00:00:55.000000 agentcomlink-0.1.9/setup.py
```

### Comparing `agentcomlink-0.1.8/LICENSE` & `agentcomlink-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `agentcomlink-0.1.8/PKG-INFO` & `agentcomlink-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentcomlink
-Version: 0.1.8
+Version: 0.1.9
 Summary: Simple chat, debug and file management panel for agents
 Home-page: https://github.com/AutonomousResearchGroup/agentcomlink
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `agentcomlink-0.1.8/README.md` & `agentcomlink-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `agentcomlink-0.1.8/agentcomlink/__init__.py` & `agentcomlink-0.1.9/agentcomlink/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,22 +9,24 @@
     get_file,
 )
 from .server import (
     start_server,
     get_server,
     set_storage_path,
     send_message,
+    async_send_message,
     register_message_handler,
     unregister_message_handler,
 )
 
 __all__ = [
     "get_storage_path",
     "start_server",
     "send_message",
+    "async_send_message",
     "register_message_handler",
     "unregister_message_handler",
     "get_server",
     "set_storage_path",
     "add_file",
     "remove_file",
     "update_file",
```

### Comparing `agentcomlink-0.1.8/agentcomlink/files.py` & `agentcomlink-0.1.9/agentcomlink/files.py`

 * *Files identical despite different names*

### Comparing `agentcomlink-0.1.8/agentcomlink/page.py` & `agentcomlink-0.1.9/agentcomlink/page.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,14 +23,29 @@
     #messages {
       height: 500px;
       overflow-y: auto;
       margin-bottom: 10px;
       border: 1px solid #ccc;
       padding: 5px;
     }
+    #feed-container {
+      width: 500px;
+      border: 1px solid #ccc;
+      border-radius: 5px;
+      padding: 10px;
+      background-color: #fff;
+      box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.05);
+    }
+    #feed {
+      height: 500px;
+      overflow-y: auto;
+      margin-bottom: 10px;
+      border: 1px solid #ccc;
+      padding: 5px;
+    }
     #chat-input {
       width: 70%;
       height: 30px;
       padding: 5px;
       border-radius: 5px;
       border: 1px solid #ccc;
     }
@@ -62,22 +77,34 @@
           <input type="file" id="file" name="file" />
           <input type="button" value="Upload" onclick="uploadFile()" />
         </form>
 
         <ul id="file-list"></ul>
       </div>
     </div>
+    <div id="feed-container">
+      <div id="feed"></div>
+      </div>
+    </div>
     <script type="module">
       let socket = new WebSocket("ws://0.0.0.0:8000/ws");
       socket.onmessage = function (event) {
         let message = event.data;
-        let messageContainer = document.getElementById("messages");
-        let newMessage = document.createElement("div");
-        newMessage.textContent = message;
-        messageContainer.appendChild(newMessage);
+        message = JSON.parse(message);
+        if (message.type === "chat") {
+          let messageContainer = document.getElementById("messages");
+          let newMessage = document.createElement("div");
+          newMessage.textContent = message;
+          messageContainer.appendChild(newMessage);
+        } else if (message.type === "feed") {
+        let feedContainer = document.getElementById("feed");
+          let newMessage = document.createElement("div");
+          newMessage.textContent = message;
+          feedContainer.appendChild(newMessage);
+        };
       };
 
       socket.onerror = function (error) {
         console.log(`[error] ${error.message}`);
       };
 
       let chatInput = document.getElementById("chat-input");
@@ -85,15 +112,15 @@
 
       sendButton.onclick = function () {
         let message = chatInput.value;
         let newMessage = document.createElement("div");
         let messageContainer = document.getElementById("messages");
         newMessage.textContent = message;
         messageContainer.appendChild(newMessage);
-        socket.send(message);
+        socket.send(JSON.stringify({ type: "chat", message }));
         chatInput.value = "";
       };
 
       chatInput.addEventListener("keypress", function(event) {
         if (event.keyCode === 13) {
           event.preventDefault();
           sendButton.click();
```

### Comparing `agentcomlink-0.1.8/agentcomlink/server.py` & `agentcomlink-0.1.9/agentcomlink/server.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import os
 import asyncio
 from fastapi import APIRouter, FastAPI, File, Form, HTTPException, UploadFile
 from fastapi.staticfiles import StaticFiles
 from pydantic import BaseModel
 
 from agentcomlink.constants import app, storage_path
@@ -15,17 +16,18 @@
 from concurrent.futures import ThreadPoolExecutor
 
 executor = ThreadPoolExecutor(max_workers=1)
 
 router = APIRouter()
 app = FastAPI()
 
-ws: WebSocket
+ws: WebSocket = None
 
 handlers = []
+loop = None
 
 
 class FilePath(BaseModel):
     path: str
 
 
 def get_server():
@@ -43,14 +45,17 @@
     """
     Start the FastAPI server.
 
     :param storage_path: The path where to store the files.
     :param port: The port on which to start the server.
     :return: The FastAPI application.
     """
+    # start an event loop
+    global loop
+    loop = asyncio.new_event_loop()
     global app
     if storage_path:
         set_storage_path(storage_path)
     check_files()
     app.include_router(router)
     app.add_middleware(
         CORSMiddleware,
@@ -61,14 +66,15 @@
     )
 
     app.mount(
         "/files", StaticFiles(directory=get_storage_path(), html=False), name="files"
     )
     if port:
         os.environ["PORT"] = str(port)
+
     return app
 
 
 def stop_server():
     """Stop the FastAPI server by setting the global app to None."""
     global app
     app = None
@@ -76,26 +82,42 @@
 
 @app.get("/")
 async def get():
     """Handle a GET request to the root of the server, responding with an HTML page."""
     return HTMLResponse(page)
 
 
-def send_message(message):
+def send_message(message, type="chat"):
     """
     Send a message to the websocket.
 
     :param message: The message to send.
     """
     global ws
-    if ws is not None:
+    global loop
+    if ws is not None and loop is not None:
         print("send text")
-        loop = asyncio.get_event_loop()  # gets current event loop
-        asyncio.run_coroutine_threadsafe(ws.send_text(message), loop)
+        message = json.dumps({"type": type, "message": message})
+        print(message)
+        asyncio.run(ws.send_text(message))
+
+
+async def async_send_message(message, type="chat"):
+    """
+    Send a message to the websocket.
 
+    :param message: The message to send.
+    """
+    global ws
+    global loop
+    if ws is not None and loop is not None:
+        print("send text")
+        message = json.dumps({"type": type, "message": message})
+        print(message)
+        await ws.send_text(message)
 
 def register_message_handler(handler):
     """
     Register a handler for messages received through the websocket.
 
     :param handler: The handler to register.
     """
@@ -122,22 +144,21 @@
     """
     global ws
     ws = websocket
     await websocket.accept()
     try:
         while True:
             data = await websocket.receive_text()
-            print("data received")
+            # data is a string, convert to json
+            data = json.loads(data)
+            print(data)
             for handler in handlers:
-                print("sending data to handler")
-                print(data)
-                handler(data)
+                await handler(data)
     except WebSocketDisconnect:
         ws = None
-        print("socket disconnected")
 
 
 @router.post("/file/")
 async def http_add_file(path: str = Form(...), file: UploadFile = File(...)):
     """
     Create a new file at a given path with the provided content.
 
@@ -203,7 +224,16 @@
     :return: The file as a response.
     """
     check_files()
     try:
         return FileResponse(os.path.join(storage_path, path))
     except Exception as e:
         raise HTTPException(status_code=400, detail=str(e))
+
+if __name__ == "__main__":
+    async def test_send(input):
+        print(input)
+        await async_send_message("test")
+
+    register_message_handler(test_send)
+    import uvicorn
+    uvicorn.run("agentcomlink:start_server", host="0.0.0.0", port=int(os.getenv("PORT", 8000)))
```

### Comparing `agentcomlink-0.1.8/agentcomlink.egg-info/PKG-INFO` & `agentcomlink-0.1.9/agentcomlink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentcomlink
-Version: 0.1.8
+Version: 0.1.9
 Summary: Simple chat, debug and file management panel for agents
 Home-page: https://github.com/AutonomousResearchGroup/agentcomlink
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `agentcomlink-0.1.8/setup.py` & `agentcomlink-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = [line for line in long_description if not '<img' in line]
     # now join all the lines back together
     long_description = '\n'.join(long_description)
     
 
 setup(
     name='agentcomlink',
-    version='0.1.8',
+    version='0.1.9',
     description='Simple chat, debug and file management panel for agents',
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url='https://github.com/AutonomousResearchGroup/agentcomlink',
     author='Moon',
     author_email='shawmakesmagic@gmail.com',
     license='MIT',
```

