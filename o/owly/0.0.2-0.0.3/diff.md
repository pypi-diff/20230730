# Comparing `tmp/owly-0.0.2.tar.gz` & `tmp/owly-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owly-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "owly-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `owly-0.0.2.tar` & `owly-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      268 2023-07-16 03:30:32.761869 owly-0.0.2/.editorconfig
--rw-r--r--   0        0        0       62 2023-07-16 03:30:32.761869 owly-0.0.2/.gitignore
--rw-r--r--   0        0        0     2280 2023-07-16 03:43:36.069175 owly-0.0.2/.gitlab-ci.yml
--rw-r--r--   0        0        0      205 2023-07-16 03:43:36.069175 owly-0.0.2/HISTORY.rst
--rw-r--r--   0        0        0     7642 2023-07-16 03:30:32.761869 owly-0.0.2/LICENSE
--rw-r--r--   0        0        0      382 2023-07-16 03:30:32.761869 owly-0.0.2/README.rst
--rw-r--r--   0        0        0     2802 2023-07-16 03:30:32.761869 owly-0.0.2/docs/conf.py
--rw-r--r--   0        0        0      142 2023-07-16 03:30:32.761869 owly-0.0.2/docs/index.rst
--rw-r--r--   0        0        0        0 2023-07-16 03:54:09.306294 owly-0.0.2/docs/installation.rst
--rw-r--r--   0        0        0      221 2023-07-16 03:30:32.761869 owly-0.0.2/docs/static/images/docs_logo.svg
--rw-r--r--   0        0        0      126 2023-07-16 03:30:32.761869 owly-0.0.2/docs/templates/layout.html
--rw-r--r--   0        0        0     1094 2023-07-16 03:30:32.761869 owly-0.0.2/docs/templates/pyproject.toml
--rw-r--r--   0        0        0      349 2023-07-16 03:43:36.069175 owly-0.0.2/owly/__init__.py
--rw-r--r--   0        0        0     2796 2023-07-16 03:30:32.761869 owly-0.0.2/owly/endpoint.py
--rw-r--r--   0        0        0     1077 2023-07-16 03:30:32.761869 owly-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      432 2023-07-16 03:30:32.761869 owly-0.0.2/requirements.txt
--rw-r--r--   0        0        0     3748 2023-07-16 03:30:32.761869 owly-0.0.2/tasks.py
--rw-r--r--   0        0        0     1778 1970-01-01 00:00:00.000000 owly-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      268 2023-07-16 03:30:32.761869 owly-0.0.3/.editorconfig
+-rw-r--r--   0        0        0       62 2023-07-16 03:30:32.761869 owly-0.0.3/.gitignore
+-rw-r--r--   0        0        0     2280 2023-07-16 03:43:36.069175 owly-0.0.3/.gitlab-ci.yml
+-rw-r--r--   0        0        0      303 2023-07-30 18:11:47.505812 owly-0.0.3/HISTORY.rst
+-rw-r--r--   0        0        0     7642 2023-07-16 03:30:32.761869 owly-0.0.3/LICENSE
+-rw-r--r--   0        0        0      382 2023-07-16 03:30:32.761869 owly-0.0.3/README.rst
+-rw-r--r--   0        0        0     2802 2023-07-16 03:30:32.761869 owly-0.0.3/docs/conf.py
+-rw-r--r--   0        0        0      142 2023-07-16 03:30:32.761869 owly-0.0.3/docs/index.rst
+-rw-r--r--   0        0        0        0 2023-07-30 18:22:22.914271 owly-0.0.3/docs/installation.rst
+-rw-r--r--   0        0        0      221 2023-07-16 03:30:32.761869 owly-0.0.3/docs/static/images/docs_logo.svg
+-rw-r--r--   0        0        0      126 2023-07-16 03:30:32.761869 owly-0.0.3/docs/templates/layout.html
+-rw-r--r--   0        0        0     1094 2023-07-16 03:30:32.761869 owly-0.0.3/docs/templates/pyproject.toml
+-rw-r--r--   0        0        0      349 2023-07-30 18:11:47.505812 owly-0.0.3/owly/__init__.py
+-rw-r--r--   0        0        0     2935 2023-07-30 18:11:47.505812 owly-0.0.3/owly/endpoint.py
+-rw-r--r--   0        0        0     1098 2023-07-30 18:11:47.505812 owly-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      446 2023-07-30 18:11:47.505812 owly-0.0.3/requirements.txt
+-rw-r--r--   0        0        0     3748 2023-07-16 03:30:32.761869 owly-0.0.3/tasks.py
+-rw-r--r--   0        0        0     1807 1970-01-01 00:00:00.000000 owly-0.0.3/PKG-INFO
```

### Comparing `owly-0.0.2/.gitlab-ci.yml` & `owly-0.0.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `owly-0.0.2/LICENSE` & `owly-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `owly-0.0.2/docs/conf.py` & `owly-0.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `owly-0.0.2/docs/templates/pyproject.toml` & `owly-0.0.3/docs/templates/pyproject.toml`

 * *Files identical despite different names*

### Comparing `owly-0.0.2/owly/endpoint.py` & `owly-0.0.3/owly/endpoint.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import base64
 import json
+import ssl
 import urllib
 from http.client import HTTPResponse
 from typing import Any, Dict, Iterator, Optional
+
+import certifi
 from rdflib import Graph
 from owly import __version__
 
 class QueryResult:
     def __init__(self, result: HTTPResponse):
         self.result = result
         self.value = result.read()
@@ -30,14 +33,15 @@
 
 class Endpoint:
     def __init__(self, endpoint: str, agent: str = f"Owly/{__version__}"):
         self.endpoint = endpoint
         self.agent = agent
         self.user: Optional[str] = None
         self.passwd: Optional[str] = None
+        self.certifi_context = ssl.create_default_context(cafile=certifi.where())
 
     def perform_query(self, query: str | bytes) -> QueryResult:
         """
         Execute a query against the SPARQL endpoint.
 
         Queries are url-encoded and sent as a GET request.
         This means only certain (likely only 'query') operations are supported.
@@ -52,15 +56,15 @@
         request = urllib.request.Request(self.endpoint + "?" + urllib.parse.urlencode({"query": query}))
         request.add_header("Accept", "*/*")  # TODO At the moment this causes a json response, but we need to specify it explicitly.
         request.add_header("User-Agent", self.agent)
         if self.user and self.passwd:
             credentials = f"{self.user}:{self.passwd}"
             encoded = base64.b64encode(credentials.encode("utf-8")).decode("utf-8")
             request.add_header("Authorization", f"Basic {encoded}")
-        response = urllib.request.urlopen(request)
+        response = urllib.request.urlopen(request, context=self.certifi_context)
         return QueryResult(response)
 
 
 def main():
     endpoint = Endpoint("https://fuseki.rys.app/SystemDesignOntology2Layers/")
     result = endpoint.perform_query("""SELECT ?subject ?predicate ?object WHERE { ?subject ?predicate ?object } LIMIT 5""")
     print(result.as_text())
```

### Comparing `owly-0.0.2/pyproject.toml` & `owly-0.0.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     "Natural Language :: English",
 ]
 dynamic = ["version", "description"]
 license = {file = "LICENSE"}
 keywords = ["ontology"]
 dependencies = [
     "rdflib>=6,<7",
+    "certifi>=2023",
 ]
 
 [project.optional-dependencies]
 test = [
     "pytest~=7.4.0",
 ]
 doc = [
```

### Comparing `owly-0.0.2/tasks.py` & `owly-0.0.3/tasks.py`

 * *Files identical despite different names*

### Comparing `owly-0.0.2/PKG-INFO` & `owly-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: owly
-Version: 0.0.2
+Version: 0.0.3
 Summary: Set of utilities related to ontologies and their management.
 Keywords: ontology
 Author-email: Arkadiusz Michał Ryś <Arkadiusz.Michal.Rys@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Requires-Dist: rdflib>=6,<7
+Requires-Dist: certifi>=2023
 Requires-Dist: tox~=4.6.0 ; extra == "dev"
 Requires-Dist: pip~=23.2 ; extra == "dev"
 Requires-Dist: flit~=3.9.0 ; extra == "dev"
 Requires-Dist: twine~=4.0.2 ; extra == "dev"
 Requires-Dist: vermin~=1.5.1 ; extra == "dev"
 Requires-Dist: invoke~=2.2.0 ; extra == "dev"
 Requires-Dist: jinja2~=3.1.2 ; extra == "dev"
```

