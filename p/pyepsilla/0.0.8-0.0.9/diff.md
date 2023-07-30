# Comparing `tmp/pyepsilla-0.0.8.tar.gz` & `tmp/pyepsilla-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyepsilla-0.0.8.tar", last modified: Fri Jul 28 13:00:22 2023, max compression
+gzip compressed data, was "pyepsilla-0.0.9.tar", last modified: Sun Jul 30 04:35:11 2023, max compression
```

## Comparing `pyepsilla-0.0.8.tar` & `pyepsilla-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-28 13:00:22.246764 pyepsilla-0.0.8/
--rw-r--r--   0 eric       (501) staff       (20)    11357 2023-07-24 16:13:02.000000 pyepsilla-0.0.8/LICENSE
--rw-r--r--   0 eric       (501) staff       (20)        0 2023-07-24 16:17:39.000000 pyepsilla-0.0.8/MANIFEST.in
--rw-r--r--   0 eric       (501) staff       (20)      298 2023-07-28 13:00:22.246646 pyepsilla-0.0.8/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     1006 2023-07-27 17:35:54.000000 pyepsilla-0.0.8/README.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-28 13:00:22.244779 pyepsilla-0.0.8/pyepsilla/
--rw-r--r--   0 eric       (501) staff       (20)       69 2023-07-24 17:00:28.000000 pyepsilla-0.0.8/pyepsilla/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)     2416 2023-07-28 12:58:48.000000 pyepsilla-0.0.8/pyepsilla/simple_example.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-28 13:00:22.246235 pyepsilla-0.0.8/pyepsilla/vectordb/
--rw-r--r--   0 eric       (501) staff       (20)      108 2023-07-27 16:02:20.000000 pyepsilla-0.0.8/pyepsilla/vectordb/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)     4360 2023-07-28 12:59:15.000000 pyepsilla-0.0.8/pyepsilla/vectordb/client.py
--rw-r--r--   0 eric       (501) staff       (20)      516 2023-07-28 04:54:17.000000 pyepsilla-0.0.8/pyepsilla/vectordb/field.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-28 13:00:22.245577 pyepsilla-0.0.8/pyepsilla.egg-info/
--rw-r--r--   0 eric       (501) staff       (20)      298 2023-07-28 13:00:22.000000 pyepsilla-0.0.8/pyepsilla.egg-info/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)      340 2023-07-28 13:00:22.000000 pyepsilla-0.0.8/pyepsilla.egg-info/SOURCES.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2023-07-28 13:00:22.000000 pyepsilla-0.0.8/pyepsilla.egg-info/dependency_links.txt
--rw-r--r--   0 eric       (501) staff       (20)       17 2023-07-28 13:00:22.000000 pyepsilla-0.0.8/pyepsilla.egg-info/requires.txt
--rw-r--r--   0 eric       (501) staff       (20)       10 2023-07-28 13:00:22.000000 pyepsilla-0.0.8/pyepsilla.egg-info/top_level.txt
--rw-r--r--   0 eric       (501) staff       (20)       38 2023-07-28 13:00:22.246803 pyepsilla-0.0.8/setup.cfg
--rw-r--r--   0 eric       (501) staff       (20)      546 2023-07-28 12:59:24.000000 pyepsilla-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:35:11.758700 pyepsilla-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-30 04:34:52.000000 pyepsilla-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 04:34:52.000000 pyepsilla-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-30 04:35:11.758700 pyepsilla-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-30 04:34:52.000000 pyepsilla-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:35:11.758700 pyepsilla-0.0.9/pyepsilla/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-30 04:34:52.000000 pyepsilla-0.0.9/pyepsilla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-30 04:34:52.000000 pyepsilla-0.0.9/pyepsilla/simple_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:35:11.758700 pyepsilla-0.0.9/pyepsilla/vectordb/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-30 04:34:52.000000 pyepsilla-0.0.9/pyepsilla/vectordb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-07-30 04:34:52.000000 pyepsilla-0.0.9/pyepsilla/vectordb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-30 04:34:52.000000 pyepsilla-0.0.9/pyepsilla/vectordb/field.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:35:11.758700 pyepsilla-0.0.9/pyepsilla.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-30 04:35:11.000000 pyepsilla-0.0.9/pyepsilla.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-30 04:35:11.000000 pyepsilla-0.0.9/pyepsilla.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 04:35:11.000000 pyepsilla-0.0.9/pyepsilla.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-30 04:35:11.000000 pyepsilla-0.0.9/pyepsilla.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-30 04:35:11.000000 pyepsilla-0.0.9/pyepsilla.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 04:35:11.758700 pyepsilla-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-30 04:34:52.000000 pyepsilla-0.0.9/setup.py
```

### Comparing `pyepsilla-0.0.8/LICENSE` & `pyepsilla-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.0.8/pyepsilla/simple_example.py` & `pyepsilla-0.0.9/pyepsilla/simple_example.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 
 # Try this simple example
 # 1. docker run --pull=always -d -p 8888:8888 epsilla/vectordb
 # 2. pip3 install --upgrade pyepsilla
 # 3. python3 simple_example.py
+#
 
 from pyepsilla import vectordb
 import random, string, time
 
-## 1.Connect to Epsilla VectorDB
-c = vectordb.Client(host='127.0.0.1', port='8888', db_name='default')
+## Connect to Epsilla VectorDB
+c = vectordb.Client(host='127.0.0.1', port='8888')
 # c = vectordb.Client(host='3.209.6.179', port='8888', db_name='default')
 
-##
+## Check VectorDB Status
 status_code, response = c.welcome()
 status_code, response = c.state()
 
 ## Load DB with path
 status_code, response= c.load_db(db_name="myDB", db_path="/tmp/epsilla")
 
 ## Set DB to current DB
 c.use_db(db_name="myDB")
 
 ## Unload DB
 # c.unload(db_name="myDB")
 
-## Create a table with schema in current DB
 
+## Create a table with schema in current DB
 ### define records number and vector dimension
 records_num = 3000
 dimensions = 8
 
-id_field = {"name": "ID", "dataType": "INT", "primaryKey": True}
+id_field = {"name": "ID", "dataType": "INT"}
 doc_field = {"name": "Doc", "dataType": "STRING"}
 vec_field = {"name": "Embedding", "dataType": "VECTOR_FLOAT", "dimensions": dimensions}
 
 fields = [id_field, doc_field, vec_field]
 status_code, response = c.create_table(table_name="MyTable", table_fields=fields)
 
+
 ## Insert new vector records into table
 # Ids = [ i for i in range(5)]
 # Docs = ["Berlin", "London", "Moscow", "San Francisco", "Shanghai"]
 # Embedding =[[0.05, 0.61, 0.76, 0.74],
 #        [0.19, 0.81, 0.75, 0.11],
 #        [0.36, 0.55, 0.47, 0.94],
 #        [0.18, 0.01, 0.85, 0.80],
@@ -53,15 +55,15 @@
 letters = list(string.ascii_lowercase+string.ascii_uppercase+string.digits)
 Docs = [''.join(random.choices(letters, k=6)) for _ in range(records_num)]
 Embedding = [[random.random() for _ in range(dimensions)] for _ in range(records_num)]
 
 records_data = [ {"ID": i, "Doc": Docs[i], "Embedding": Embedding[i]} for i in range(records_num)]
 status_code, response = c.insert(table_name="MyTable", records=records_data)
 
-# time.sleep(5)
+
 ## Query Vectors
 query_field = "Embedding"
 query_vector = Embedding[-1]
 print(Docs[-1], query_vector)
 response_fields = ["Doc"]
 limit = 2
 status_code, response = c.query(table_name="MyTable", query_field=query_field, query_vector=query_vector, response_fields=response_fields, limit=limit)
```

### Comparing `pyepsilla-0.0.8/pyepsilla/vectordb/client.py` & `pyepsilla-0.0.9/pyepsilla/vectordb/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,110 +1,111 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 
 import json, requests, socket
 
 class Client():
-    def __init__(self, host='localhost', port='8888', db_name='default'):
-        self._protocol = "http"
+    def __init__(self, protocol = 'http', host='localhost', port='8888'):
+        self._protocol = protocol
         self._host = host
         self._port = port
         self._baseurl = "{}://{}:{}".format(self._protocol, self._host, self._port)
-        self._db=db_name
+        self._db=None
         self._timeout = 10
         self._header = {'Content-type': 'application/json'}
         self.check_networking()
 
     def check_networking(self):
         socket.setdefaulttimeout(self._timeout)
         s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         check_result = s.connect_ex((self._host, int(self._port)))
         s.close()
         if check_result == 0:
-            print("[INFO] {}:{} can be arrived!".format(self._host, self._port))
+            print("[INFO] Connected to {}:{} successfully.".format(self._host, self._port))
         else:
-            raise Exception("[ERROR] {}:{} cann't be arrived!".format(self._host, self._port))
+            raise Exception("[ERROR] Failed to connect to {}:{}".format(self._host, self._port))
 
     def welcome(self):
         req_url = "{}/".format(self._baseurl)
         req_data= None
         res = requests.get(url=req_url, data=json.dumps(req_data), headers=self._header, timeout=self._timeout)
         status_code = res.status_code
         body = res.text
-        print("Return:", body)
         return status_code, body
 
     def state(self):
         req_url = "{}/state".format(self._baseurl)
         req_data= None
         res = requests.get(url=req_url, data=json.dumps(req_data), headers=self._header)
         status_code = res.status_code
         body = res.json()
-        print("Return:", body)
         return status_code, body
 
     def use_db(self, db_name):
         self._db = db_name
 
-    def load_db(self, db_name, db_path):
+    def load_db(self, db_name, db_path, vector_scale=None):
         req_url = "{}/api/load".format(self._baseurl)
         req_data= {"name": db_name, "path": db_path}
+        if vector_scale is not None:
+            req_data["vectorScale"] = vector_scale
         res = requests.post(url=req_url, data=json.dumps(req_data), headers=self._header)
         status_code = res.status_code
         body = res.json()
-        print("Return:", body)
         return status_code, body
 
     def unload_db(self, db_name):
         req_url = "{}/api/{}/unload".format(self._baseurl, db_name)
         res = requests.post(url=req_url, data=None, headers=self._header)
         status_code = res.status_code
         body = res.json()
-        print("Return:", body)
         return status_code, body
 
     def create_table(self, table_name="MyTable", table_fields=[]):
+        if self._db is None:
+            raise Exception("[ERROR] Please use_db() first!")
         req_url = "{}/api/{}/schema/tables".format(self._baseurl, self._db)
         req_data= {"name": table_name, "fields": table_fields}
         res = requests.post(url=req_url, data=json.dumps(req_data), headers=self._header)
         status_code = res.status_code
         body = res.json()
-        print("Return:", body)
         return status_code, body
 
 
     def insert(self, table_name="MyTable", records=[]):
+        if self._db is None:
+            raise Exception("[ERROR] Please use_db() first!")
         req_url = "{}/api/{}/data/insert".format(self._baseurl, self._db)
         req_data= {"table": table_name, "data": records}
         res = requests.post(url=req_url, data=json.dumps(req_data), headers=self._header)
         status_code = res.status_code
         body = res.json()
-        print("Return:", body)
         return status_code, body
 
 
     def query(self, table_name="MyTable", query_field="", query_vector=[], response_fields=[], limit=1):
+        if self._db is None:
+            raise Exception("[ERROR] Please use_db() first!")
         req_url = "{}/api/{}/data/query".format(self._baseurl, self._db)
         req_data= {"table": table_name, "queryField": query_field, "queryVector": query_vector, "response": response_fields, "limit": limit}
         res = requests.post(url=req_url, data=json.dumps(req_data), headers=self._header)
         status_code = res.status_code
         body = res.json()
-        print("Return:", body)
         return status_code, body
 
 
     def drop_table(self, table_name="MyTable"):
+        if self._db is None:
+            raise Exception("[ERROR] Please use_db() first!")
         req_url = "{}/api/{}/schema/tables/{}".format(self._baseurl, self._db, table_name)
         req_data= None
         res = requests.delete(url=req_url, data=json.dumps(req_data), headers=self._header)
         status_code = res.status_code
         body = res.json()
-        print("Return:", body)
         return status_code, body
 
     def drop_db(self, db_name):
         req_url = "{}/api/{}/drop".format(self._baseurl, db_name)
         res = requests.delete(url=req_url, data=None, headers=self._header)
         status_code = res.status_code
         body = res.json()
-        print("Return:", body)
         return status_code, body
```

### Comparing `pyepsilla-0.0.8/pyepsilla/vectordb/field.py` & `pyepsilla-0.0.9/pyepsilla/vectordb/field.py`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.0.8/setup.py` & `pyepsilla-0.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 
 from setuptools import setup, find_packages
 
 setup(
     name='pyepsilla',
-    version= '0.0.8',
+    version= '0.0.9',
     keywords='epsilla',
     author= 'Epsilla Team',
     description='Epsilla Python SDK',
+    long_description='Epsilla Python SDK',
     license='Apache License',
     packages=find_packages(),
     include_package_data=True,
     platforms='any',
     install_requires=[
         'requests>=2.19.1'
     ],
```

