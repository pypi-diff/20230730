# Comparing `tmp/seagoat-0.7.2.tar.gz` & `tmp/seagoat-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seagoat-0.7.2.tar", max compression
+gzip compressed data, was "seagoat-0.7.3.tar", max compression
```

## Comparing `seagoat-0.7.2.tar` & `seagoat-0.7.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1070 2023-07-30 10:46:37.836726 seagoat-0.7.2/LICENSE
--rw-r--r--   0        0        0     1847 2023-07-30 10:46:37.836726 seagoat-0.7.2/README.md
--rw-r--r--   0        0        0     3086 2023-07-30 10:46:38.616736 seagoat-0.7.2/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-30 10:46:38.616736 seagoat-0.7.2/seagoat/__init__.py
--rw-r--r--   0        0        0     1601 2023-07-30 10:46:37.844726 seagoat-0.7.2/seagoat/cache.py
--rw-r--r--   0        0        0     3103 2023-07-30 10:46:37.844726 seagoat-0.7.2/seagoat/cli.py
--rw-r--r--   0        0        0      196 2023-07-30 10:46:37.844726 seagoat-0.7.2/seagoat/common.py
--rw-r--r--   0        0        0     4512 2023-07-30 10:46:37.844726 seagoat-0.7.2/seagoat/engine.py
--rw-r--r--   0        0        0     3492 2023-07-30 10:46:37.844726 seagoat-0.7.2/seagoat/file.py
--rw-r--r--   0        0        0     2689 2023-07-30 10:46:37.844726 seagoat-0.7.2/seagoat/repository.py
--rw-r--r--   0        0        0     2021 2023-07-30 10:46:37.844726 seagoat-0.7.2/seagoat/result.py
--rw-r--r--   0        0        0     5766 2023-07-30 10:46:37.844726 seagoat-0.7.2/seagoat/server.py
--rw-r--r--   0        0        0     1878 2023-07-30 10:46:37.844726 seagoat-0.7.2/seagoat/sources/chroma.py
--rw-r--r--   0        0        0     1210 2023-07-30 10:46:37.844726 seagoat-0.7.2/seagoat/sources/ripgrep.py
--rw-r--r--   0        0        0     2862 1970-01-01 00:00:00.000000 seagoat-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-30 14:44:33.843920 seagoat-0.7.3/LICENSE
+-rw-r--r--   0        0        0     1847 2023-07-30 14:44:33.843920 seagoat-0.7.3/README.md
+-rw-r--r--   0        0        0     3085 2023-07-30 14:45:30.484336 seagoat-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-30 14:45:30.484336 seagoat-0.7.3/seagoat/__init__.py
+-rw-r--r--   0        0        0     1601 2023-07-30 14:44:33.851920 seagoat-0.7.3/seagoat/cache.py
+-rw-r--r--   0        0        0     3103 2023-07-30 14:44:33.851920 seagoat-0.7.3/seagoat/cli.py
+-rw-r--r--   0        0        0      196 2023-07-30 14:44:33.851920 seagoat-0.7.3/seagoat/common.py
+-rw-r--r--   0        0        0     4424 2023-07-30 14:44:33.851920 seagoat-0.7.3/seagoat/engine.py
+-rw-r--r--   0        0        0     3492 2023-07-30 14:44:33.851920 seagoat-0.7.3/seagoat/file.py
+-rw-r--r--   0        0        0     2689 2023-07-30 14:44:33.851920 seagoat-0.7.3/seagoat/repository.py
+-rw-r--r--   0        0        0     2021 2023-07-30 14:44:33.851920 seagoat-0.7.3/seagoat/result.py
+-rw-r--r--   0        0        0     5766 2023-07-30 14:44:33.851920 seagoat-0.7.3/seagoat/server.py
+-rw-r--r--   0        0        0     1692 2023-07-30 14:44:33.851920 seagoat-0.7.3/seagoat/sources/chroma.py
+-rw-r--r--   0        0        0     1105 2023-07-30 14:44:33.851920 seagoat-0.7.3/seagoat/sources/ripgrep.py
+-rw-r--r--   0        0        0     2861 1970-01-01 00:00:00.000000 seagoat-0.7.3/PKG-INFO
```

### Comparing `seagoat-0.7.2/LICENSE` & `seagoat-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `seagoat-0.7.2/README.md` & `seagoat-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `seagoat-0.7.2/pyproject.toml` & `seagoat-0.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "seagoat"
-version = "0.7.2"
+version = "0.7.3"
 description = "A semantic-code search engine"
 authors = ["Daniel Kantor <git@daniel-kantor.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.scripts]
 gt = "seagoat.cli:seagoat"
 seagoat = "seagoat.cli:seagoat"
 seagoat-server = "seagoat.server:server"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-chromadb = "^0.3.26"
+chromadb = "^0.4.0"
 gitpython = "^3.1.31"
 tqdm = "^4.65.0"
 appdirs = "^1.4.4"
 click = "^8.1.3"
 prompt-toolkit = "^3.0.38"
 blessed = "^1.20.0"
 pygments = "^2.15.1"
```

### Comparing `seagoat-0.7.2/seagoat/cache.py` & `seagoat-0.7.3/seagoat/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Generic
 from typing import TypeVar
 
 import appdirs
 
 T = TypeVar("T")
 
-CACHE_FORMAT_VERSION = 15
+CACHE_FORMAT_VERSION = 16
 
 
 class Cache(Generic[T]):
     def __init__(self, cache_name: str, path: Path, initial_value: T):
         self._path = path
         self.data = initial_value
         self._cache_name = cache_name
```

### Comparing `seagoat-0.7.2/seagoat/cli.py` & `seagoat-0.7.3/seagoat/cli.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.7.2/seagoat/engine.py` & `seagoat-0.7.3/seagoat/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,17 +92,14 @@
                 continue
 
             self._add_to_collection(chunk)
             self._cache.data["chunks_already_analyzed"].add(chunk.chunk_id)
 
         self._cache.persist()
 
-        for source in chain(*self._fetchers.values()):
-            source["persist"]()
-
     def query(self, query: str):
         self.query_string = query
 
     async def fetch(self):
         self._results = []
         executor = ThreadPoolExecutor(max_workers=1)
         loop = asyncio.get_event_loop()
```

### Comparing `seagoat-0.7.2/seagoat/file.py` & `seagoat-0.7.3/seagoat/file.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.7.2/seagoat/repository.py` & `seagoat-0.7.3/seagoat/repository.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.7.2/seagoat/result.py` & `seagoat-0.7.3/seagoat/result.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.7.2/seagoat/server.py` & `seagoat-0.7.3/seagoat/server.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.7.2/seagoat/sources/chroma.py` & `seagoat-0.7.3/seagoat/sources/chroma.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,21 +6,15 @@
 from seagoat.cache import Cache
 from seagoat.repository import Repository
 from seagoat.result import Result
 
 
 def initialize(repository: Repository):
     cache = Cache("chroma", Path(repository.path), {})
-    chroma_client = chromadb.Client(
-        chromadb.Settings(
-            chroma_db_impl="duckdb+parquet",
-            persist_directory=str(cache.get_cache_folder()),
-            anonymized_telemetry=False,
-        )
-    )
+    chroma_client = chromadb.PersistentClient(path=str(cache.get_cache_folder()))
     chroma_collection = chroma_client.get_or_create_collection(name="code_data")
 
     def fetch(query_text: str):
         chromadb_results = [
             chroma_collection.query(query_texts=[query_text], n_results=50)
         ]
         metadata_with_distance = (
@@ -55,9 +49,8 @@
             )
         except IDAlreadyExistsError:
             pass
 
     return {
         "fetch": fetch,
         "cache_chunk": cache_chunk,
-        "persist": chroma_client.persist,
     }
```

### Comparing `seagoat-0.7.2/seagoat/sources/ripgrep.py` & `seagoat-0.7.3/seagoat/sources/ripgrep.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,16 +32,11 @@
     def fetch(query_text: str):
         return _fetch(query_text, path)
 
     def cache_chunk(_):
         # Ripgrep does not need a cache for chunks
         pass
 
-    def persist():
-        # Ripgrep does not need persistence
-        pass
-
     return {
         "fetch": fetch,
         "cache_chunk": cache_chunk,
-        "persist": persist,
     }
```

### Comparing `seagoat-0.7.2/PKG-INFO` & `seagoat-0.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: seagoat
-Version: 0.7.2
+Version: 0.7.3
 Summary: A semantic-code search engine
 License: MIT
 Author: Daniel Kantor
 Author-email: git@daniel-kantor.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: blessed (>=1.20.0,<2.0.0)
-Requires-Dist: chromadb (>=0.3.26,<0.4.0)
+Requires-Dist: chromadb (>=0.4.0,<0.5.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: flask (>=2.3.2,<3.0.0)
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
 Requires-Dist: nest-asyncio (>=1.5.6,<2.0.0)
 Requires-Dist: prompt-toolkit (>=3.0.38,<4.0.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: pygments (>=2.15.1,<3.0.0)
```

