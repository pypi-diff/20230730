# Comparing `tmp/i7api-1.0.0.tar.gz` & `tmp/i7api-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i7api-1.0.0.tar", last modified: Sun Jul 16 17:09:32 2023, max compression
+gzip compressed data, was "i7api-2.0.0.tar", last modified: Sun Jul 30 05:25:02 2023, max compression
```

## Comparing `i7api-1.0.0.tar` & `i7api-2.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 17:09:32.823970 i7api-1.0.0/
--rw-rw-rw-   0        0        0      287 2023-07-16 17:09:32.813967 i7api-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-16 17:09:32.773980 i7api-1.0.0/i7api/
--rw-rw-rw-   0        0        0        0 2023-07-16 16:32:40.000000 i7api-1.0.0/i7api/__init__.py
--rw-rw-rw-   0        0        0     3090 2023-07-16 17:01:34.000000 i7api-1.0.0/i7api/base.py
-drwxrwxrwx   0        0        0        0 2023-07-16 17:09:32.813967 i7api-1.0.0/i7api.egg-info/
--rw-rw-rw-   0        0        0      287 2023-07-16 17:09:32.000000 i7api-1.0.0/i7api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      184 2023-07-16 17:09:32.000000 i7api-1.0.0/i7api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 17:09:32.000000 i7api-1.0.0/i7api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-16 17:09:32.000000 i7api-1.0.0/i7api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-16 17:09:32.000000 i7api-1.0.0/i7api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 17:09:32.823970 i7api-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      569 2023-07-16 17:09:27.000000 i7api-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 05:25:02.583378 i7api-2.0.0/
+-rw-rw-rw-   0        0        0      287 2023-07-30 05:25:02.583378 i7api-2.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-30 05:25:02.553382 i7api-2.0.0/i7api/
+-rw-rw-rw-   0        0        0       75 2023-07-30 05:24:19.000000 i7api-2.0.0/i7api/__init__.py
+-rw-rw-rw-   0        0        0     2941 2023-07-30 05:17:41.000000 i7api-2.0.0/i7api/base.py
+drwxrwxrwx   0        0        0        0 2023-07-30 05:25:02.583378 i7api-2.0.0/i7api.egg-info/
+-rw-rw-rw-   0        0        0      287 2023-07-30 05:25:02.000000 i7api-2.0.0/i7api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      184 2023-07-30 05:25:02.000000 i7api-2.0.0/i7api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 05:25:02.000000 i7api-2.0.0/i7api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-30 05:25:02.000000 i7api-2.0.0/i7api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-30 05:25:02.000000 i7api-2.0.0/i7api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 05:25:02.583378 i7api-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      569 2023-07-30 05:23:13.000000 i7api-2.0.0/setup.py
```

### Comparing `i7api-1.0.0/i7api/base.py` & `i7api-2.0.0/i7api/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,63 +1,60 @@
 import requests
 import base64
 class Storage:
-    def __init__(self, url = "127.0.0.1"):
+    def __init__(self, url = "127.0.0.1:2707", api=None, password=None):
         self.url = url
-        self.api = None
-        self.password = None
+        self.api = api
+        self.password = password
     def signin(self, email=None, password=None):
-        r = requests.post(f"http://{self.url}:2707/api",
+        r = requests.post(f"http://{self.url}/api",
                           json={"type": "signin", "username": email, "password": password})
         try:
             self.api = r.json()['api_key']
             self.password = r.json()['api_password']
             return r.json()
         except:
             print(r.content)
             return r.content
     def signup(self, email=None, password=None):
-        r = requests.post(f"http://{self.url}:2707/api",
+        r = requests.post(f"http://{self.url}/api",
                           json={"type": "signup", "username": email, "password": password})
         print("Enter the OTP in Terminal")
         try:
             self.api = r.json()['api_key']
             self.password = r.json()['api_password']
             return r.json()
         except:
             return r.content
     def upload(self, file=None):
         if self.api is not None and self.password is not None:
             f = open(file, "rb")
-            data = f.read()
-            f.close()
-            data_b64 = base64.b64encode(data).decode()
-            r = requests.post(f"http://{self.url}:2707/api", json={"type": "upload", "api_key": self.api,
+            files = {"file": f}
+            r = requests.post(f"http://{self.url}/api", json={"type": "upload", "api_key": self.api,
                                                                  'api_password': self.password,
-                                                                 "file_name": f.name,
-                                                                 "bytes": data_b64})
+                                                                 "file_name": f.name}, files=files)
 
             return r.json()
         else:
             print("First Login or Signup")
     def download(self,file_id, file_path=None):
-        r = requests.post(f"http://{self.url}:2707/api", json={"type": "download", "api_key": self.api,
+        r = requests.post(f"http://{self.url}/api", json={"type": "download", "api_key": self.api,
                                                                'api_password': self.password,
                                                                "file_id": file_id})
         f = open(file_path, "wb")
         data_bytes = base64.b64decode(r.json().get('base64', None))
         f.write(data_bytes)
         f.close()
     def delete(self, file_id):
-        r = requests.post(f"http://{self.url}:2707/api", json={"type": "delete", "api_key": self.api,
+        r = requests.post(f"http://{self.url}/api", json={"type": "delete", "api_key": self.api,
                                                                'api_password': self.password,
                                                                "file_id": file_id})
         return r.json()
     def get_all(self):
-        r = requests.post(f"http://{self.url}:2707/api", json={"type": "getallid", "api_key": self.api,
+        r = requests.post(f"http://{self.url}/api", json={"type": "getallid", "api_key": self.api,
                                                                'api_password': self.password})
         print(r.json())
     def search(self, file_name):
-        r = requests.post(f"http://{self.url}:2707/api", json={"type": "search", "api_key": self.api,
+        r = requests.post(f"http://{self.url}/api", json={"type": "search", "api_key": self.api,
                                                                'api_password': self.password, "file_name": file_name})
         print(r.json())
```

### Comparing `i7api-1.0.0/setup.py` & `i7api-2.0.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="i7api",
-    version="1.0.0",
+    version="2.0.0",
     author="Ojas Gupta",
     description="API Wrapper for i7StorageEngine",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

