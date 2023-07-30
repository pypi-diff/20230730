# Comparing `tmp/authomize-rest-api-client-4.3.6.tar.gz` & `tmp/authomize-rest-api-client-4.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authomize-rest-api-client-4.3.6.tar", last modified: Wed Jul 26 11:00:00 2023, max compression
+gzip compressed data, was "authomize-rest-api-client-4.3.7.tar", last modified: Sun Jul 30 08:58:28 2023, max compression
```

## Comparing `authomize-rest-api-client-4.3.6.tar` & `authomize-rest-api-client-4.3.7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:00:00.153061 authomize-rest-api-client-4.3.6/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      251 2023-07-26 11:00:00.153061 authomize-rest-api-client-4.3.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2201 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:00:00.153061 authomize-rest-api-client-4.3.6/authomize/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:00:00.153061 authomize-rest-api-client-4.3.6/authomize/rest_api_client/
--rw-r--r--   0 root         (0) root         (0)      627 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:00:00.153061 authomize-rest-api-client-4.3.6/authomize/rest_api_client/client/
--rw-r--r--   0 root         (0) root         (0)       81 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2566 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/client/base_client.py
--rw-r--r--   0 root         (0) root         (0)    10358 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/client/client.py
--rw-r--r--   0 root         (0) root         (0)    13027 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/client/connectors_client.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/client/platform_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:00:00.153061 authomize-rest-api-client-4.3.6/authomize/rest_api_client/configuration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/configuration/__init__.py
--rw-r--r--   0 root         (0) root         (0)      330 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/configuration/authomize_api_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:00:00.153061 authomize-rest-api-client-4.3.6/authomize/rest_api_client/generated/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/generated/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:00:00.153061 authomize-rest-api-client-4.3.6/authomize/rest_api_client/generated/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    84645 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:00:00.153061 authomize-rest-api-client-4.3.6/authomize/rest_api_client/generated/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/generated/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    49496 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/generated/external_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:00:00.153061 authomize-rest-api-client-4.3.6/authomize/rest_api_client/openapi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/openapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:00:00.153061 authomize-rest-api-client-4.3.6/authomize/rest_api_client/openapi/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   200535 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:00:00.153061 authomize-rest-api-client-4.3.6/authomize/rest_api_client/openapi/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/openapi/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   115488 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/openapi/external_rest_api/openapi.json
--rw-r--r--   0 root         (0) root         (0)       26 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:00:00.153061 authomize-rest-api-client-4.3.6/authomize_rest_api_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      251 2023-07-26 11:00:00.000000 authomize-rest-api-client-4.3.6/authomize_rest_api_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1356 2023-07-26 11:00:00.000000 authomize-rest-api-client-4.3.6/authomize_rest_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 11:00:00.000000 authomize-rest-api-client-4.3.6/authomize_rest_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      189 2023-07-26 11:00:00.000000 authomize-rest-api-client-4.3.6/authomize_rest_api_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-26 11:00:00.000000 authomize-rest-api-client-4.3.6/authomize_rest_api_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      336 2023-07-26 11:00:00.153061 authomize-rest-api-client-4.3.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1117 2023-07-26 10:59:44.000000 authomize-rest-api-client-4.3.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 08:58:28.419365 authomize-rest-api-client-4.3.7/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      251 2023-07-30 08:58:28.419365 authomize-rest-api-client-4.3.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2201 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 08:58:28.415365 authomize-rest-api-client-4.3.7/authomize/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 08:58:28.415365 authomize-rest-api-client-4.3.7/authomize/rest_api_client/
+-rw-r--r--   0 root         (0) root         (0)      627 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 08:58:28.415365 authomize-rest-api-client-4.3.7/authomize/rest_api_client/client/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2566 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/client/base_client.py
+-rw-r--r--   0 root         (0) root         (0)    10358 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/client/client.py
+-rw-r--r--   0 root         (0) root         (0)    13027 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/client/connectors_client.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/client/platform_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 08:58:28.415365 authomize-rest-api-client-4.3.7/authomize/rest_api_client/configuration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/configuration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      330 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/configuration/authomize_api_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 08:58:28.415365 authomize-rest-api-client-4.3.7/authomize/rest_api_client/generated/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/generated/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 08:58:28.415365 authomize-rest-api-client-4.3.7/authomize/rest_api_client/generated/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    85173 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 08:58:28.415365 authomize-rest-api-client-4.3.7/authomize/rest_api_client/generated/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/generated/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    49496 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/generated/external_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 08:58:28.415365 authomize-rest-api-client-4.3.7/authomize/rest_api_client/openapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/openapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 08:58:28.415365 authomize-rest-api-client-4.3.7/authomize/rest_api_client/openapi/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   201078 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 08:58:28.419365 authomize-rest-api-client-4.3.7/authomize/rest_api_client/openapi/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/openapi/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   115488 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/openapi/external_rest_api/openapi.json
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-30 08:58:09.000000 authomize-rest-api-client-4.3.7/authomize/rest_api_client/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 08:58:28.419365 authomize-rest-api-client-4.3.7/authomize_rest_api_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      251 2023-07-30 08:58:28.000000 authomize-rest-api-client-4.3.7/authomize_rest_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-07-30 08:58:28.000000 authomize-rest-api-client-4.3.7/authomize_rest_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-30 08:58:28.000000 authomize-rest-api-client-4.3.7/authomize_rest_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      189 2023-07-30 08:58:28.000000 authomize-rest-api-client-4.3.7/authomize_rest_api_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-30 08:58:28.000000 authomize-rest-api-client-4.3.7/authomize_rest_api_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      336 2023-07-30 08:58:28.419365 authomize-rest-api-client-4.3.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1117 2023-07-30 08:58:12.000000 authomize-rest-api-client-4.3.7/setup.py
```

### Comparing `authomize-rest-api-client-4.3.6/LICENSE.txt` & `authomize-rest-api-client-4.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.6/README.md` & `authomize-rest-api-client-4.3.7/README.md`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.6/authomize/rest_api_client/__init__.py` & `authomize-rest-api-client-4.3.7/authomize/rest_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.6/authomize/rest_api_client/client/base_client.py` & `authomize-rest-api-client-4.3.7/authomize/rest_api_client/client/base_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.6/authomize/rest_api_client/client/client.py` & `authomize-rest-api-client-4.3.7/authomize/rest_api_client/client/client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.6/authomize/rest_api_client/client/connectors_client.py` & `authomize-rest-api-client-4.3.7/authomize/rest_api_client/client/connectors_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.6/authomize/rest_api_client/client/platform_client.py` & `authomize-rest-api-client-4.3.7/authomize/rest_api_client/client/platform_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.6/authomize/rest_api_client/generated/connectors_rest_api/schemas.py` & `authomize-rest-api-client-4.3.7/authomize/rest_api_client/generated/connectors_rest_api/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  openapi.json
-#   timestamp: 2023-07-02T11:21:59+00:00
+#   timestamp: 2023-07-27T10:34:52+00:00
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional
 
@@ -875,14 +875,19 @@
     Ingest = 'Ingest'
     IngestChunk = 'IngestChunk'
     PostProcess = 'PostProcess'
     Queue = 'Queue'
 
 
 class UpdateAppSchema(BaseModel):
+    executionId: Optional[str] = Field(
+        default=None,
+        description='The `executionId` parameter can be used to allow an app to run as a set of multiple, different executions with different configurations.\n\nOnce the data was uploaded using a certain `executionId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `executionId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n',
+        title='Executionid',
+    )
     name: Optional[str] = Field(
         default=None, description='The name of the Application.\n', title='Name'
     )
     logo_url_sync: Optional[bool] = Field(
         default=None,
         description='Ensure that the Application logo is the same as in the integration.',
         title='Logo Url Sync',
```

### Comparing `authomize-rest-api-client-4.3.6/authomize/rest_api_client/generated/external_rest_api/schemas.py` & `authomize-rest-api-client-4.3.7/authomize/rest_api_client/generated/external_rest_api/schemas.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.6/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json` & `authomize-rest-api-client-4.3.7/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9874931243124312%*

 * *Differences: {"'components'": "{'schemas': {'UpdateAppSchema': {'properties': {'executionId': "*

 * *                 "OrderedDict([('title', 'Executionid'), ('type', 'string'), ('description', 'The "*

 * *                 '`executionId` parameter can be used to allow an app to run as a set of multiple, '*

 * *                 'different executions with different configurations.\\n\\nOnce the data was '*

 * *                 'uploaded using a certain `executionId`, all other requests, referring to the '*

 * *                 'same data using `G […]*

```diff
@@ -3170,14 +3170,19 @@
                     "PostProcess",
                     "Queue"
                 ],
                 "title": "TransactionStateType"
             },
             "UpdateAppSchema": {
                 "properties": {
+                    "executionId": {
+                        "description": "The `executionId` parameter can be used to allow an app to run as a set of multiple, different executions with different configurations.\n\nOnce the data was uploaded using a certain `executionId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `executionId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n",
+                        "title": "Executionid",
+                        "type": "string"
+                    },
                     "logo_url_sync": {
                         "description": "Ensure that the Application logo is the same as in the integration.",
                         "title": "Logo Url Sync",
                         "type": "boolean"
                     },
                     "name": {
                         "description": "The name of the Application.\n",
@@ -3863,15 +3868,15 @@
                 "type": "apiKey"
             }
         }
     },
     "info": {
         "description": "Authomize enables users to integrate your applications with Authomize via custom connectors.\n\nYou can use the APIs described in this document to create your connector.\n\nOnce data is uploaded and processed successfully, your custom connector will function in the same way as the connectors created by Authomize.\n\n## How does Authomize work?\nAuthomize works by gathering information about:\n\n\u00b7 individuals, teams and functions.\n\n\u00b7 apps, assets and accounts.\n\n\u00b7 all the relationships between them.\n\n![img.png](https://storagetry1.blob.core.windows.net/public/78d82650-71b0-4909-8444-022aab79add5.png)\n\n## Connector APIs\n\nAuthomize connector APIs enable pushing data into Authomize from external sources.\n\nThese APIs enable data extracted from outside applications (via application APIs) to be delivered to Authomize.\n\nA connector processes extracted application data to transform it into a format compatible with Authomize.\n\n![img_1.png](https://storagetry1.blob.core.windows.net/public/341bf6ef-2e5b-4284-b715-45105ffbf0f8.png)\n\n## Authentication\nTo Authenticate use the API Token, with the format: `Authorization: API_Token`.\n\nAn API Token is a token you provide when making API calls. \n\n\nThe API Token should be included in every request to the API in an `Authorization` header.\n```\ncurl -v -X POST \\n\n     -H \"Authorization: {API_Token}\" \\n\n     ...\n```\n\n## Limits\nRequests cannot exceed a size of 1MB.\n",
         "title": "Authomize API Reference",
-        "version": "4.3.0",
+        "version": "4.3.4",
         "x-logo": {
             "url": "https://static.authomize.com/public/icons/authomize-green.svg"
         }
     },
     "openapi": "3.0.2",
     "paths": {
         "/is_alive": {
```

### Comparing `authomize-rest-api-client-4.3.6/authomize/rest_api_client/openapi/external_rest_api/openapi.json` & `authomize-rest-api-client-4.3.7/authomize/rest_api_client/openapi/external_rest_api/openapi.json`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.6/authomize_rest_api_client.egg-info/SOURCES.txt` & `authomize-rest-api-client-4.3.7/authomize_rest_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.6/setup.py` & `authomize-rest-api-client-4.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == '__main__':
     setup(
-        version='4.3.6',
+        version='4.3.7',
         name='authomize-rest-api-client',
         author='Authomize inc.',
         license='MIT',
         author_email='info@authomize.com',
         description='Authomize REST API Python Client',
         packages=find_namespace_packages(include=['authomize.*']),
         package_data={
```

