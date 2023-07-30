# Comparing `tmp/hishel-0.0.5.tar.gz` & `tmp/hishel-0.0.6.tar.gz`

## Comparing `hishel-0.0.5.tar` & `hishel-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 hishel-0.0.5/CHANGELOG.md
--rw-r--r--   0        0        0     3813 2020-02-02 00:00:00.000000 hishel-0.0.5/README.md
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/__about__.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/__init__.py
--rw-r--r--   0        0        0    11263 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_controller.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_exceptions.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_files.py
--rw-r--r--   0        0        0     7921 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_headers.py
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_serializers.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_synchronization.py
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/py.typed
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_async/__init__.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_async/_client.py
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_async/_mock.py
--rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_async/_pool.py
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_async/_storages.py
--rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_async/_transports.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_sync/__init__.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_sync/_client.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_sync/_mock.py
--rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_sync/_pool.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_sync/_storages.py
--rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 hishel-0.0.5/hishel/_sync/_transports.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 hishel-0.0.5/.gitignore
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 hishel-0.0.5/LICENSE
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 hishel-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 hishel-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 hishel-0.0.6/CHANGELOG.md
+-rw-r--r--   0        0        0     3813 2020-02-02 00:00:00.000000 hishel-0.0.6/README.md
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 hishel-0.0.6/hishel/__about__.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 hishel-0.0.6/hishel/__init__.py
+-rw-r--r--   0        0        0    11396 2020-02-02 00:00:00.000000 hishel-0.0.6/hishel/_controller.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 hishel-0.0.6/hishel/_exceptions.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 hishel-0.0.6/hishel/_files.py
+-rw-r--r--   0        0        0     7921 2020-02-02 00:00:00.000000 hishel-0.0.6/hishel/_headers.py
+-rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 hishel-0.0.6/hishel/_serializers.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 hishel-0.0.6/hishel/_synchronization.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 hishel-0.0.6/hishel/_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hishel-0.0.6/hishel/py.typed
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hishel-0.0.6/hishel/_async/__init__.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 hishel-0.0.6/hishel/_async/_client.py
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 hishel-0.0.6/hishel/_async/_mock.py
+-rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 hishel-0.0.6/hishel/_async/_pool.py
+-rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 hishel-0.0.6/hishel/_async/_storages.py
+-rw-r--r--   0        0        0     5811 2020-02-02 00:00:00.000000 hishel-0.0.6/hishel/_async/_transports.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hishel-0.0.6/hishel/_sync/__init__.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 hishel-0.0.6/hishel/_sync/_client.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 hishel-0.0.6/hishel/_sync/_mock.py
+-rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 hishel-0.0.6/hishel/_sync/_pool.py
+-rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 hishel-0.0.6/hishel/_sync/_storages.py
+-rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 hishel-0.0.6/hishel/_sync/_transports.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 hishel-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 hishel-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 hishel-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 hishel-0.0.6/PKG-INFO
```

### Comparing `hishel-0.0.5/README.md` & `hishel-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `hishel-0.0.5/hishel/_controller.py` & `hishel-0.0.6/hishel/_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,36 +192,38 @@
         if last_modified:
             precondition_headers.append((b"If-Unmodified-Since", last_modified))
         if etag:
             precondition_headers.append((b"If-None-Match", etag))
 
         request.headers.extend(precondition_headers)
 
-    def _validate_vary(self, request: Request, response: Response) -> bool:
+    def _validate_vary(
+        self, request: Request, response: Response, original_request: Request
+    ) -> bool:
         """
         Determines whether the "vary" headers in the request and response headers are identical.
 
         See also (https://www.rfc-editor.org/rfc/rfc9111.html#name-calculating-cache-keys-with).
         """
 
         vary_headers = extract_header_values_decoded(response.headers, b"vary")
         vary = Vary.from_value(vary_values=vary_headers)
         for vary_header in vary._values:
             if vary_header == "*":
                 return False  # pragma: no cover
 
             if extract_header_values(
                 request.headers, vary_header
-            ) != extract_header_values(response.headers, vary_header):
+            ) != extract_header_values(original_request.headers, vary_header):
                 return False
 
         return True
 
     def construct_response_from_cache(
-        self, request: Request, response: Response
+        self, request: Request, response: Response, original_request: Request
     ) -> tp.Union[Response, Request, None]:
         """
         Specifies whether the response should be used, skipped, or validated by the cache.
 
         This method makes a decision regarding what to do with
         the stored response when it is retrieved from storage.
         It might be ready for use or it might need to be revalidated.
@@ -241,15 +243,17 @@
 
         response_cache_control = parse_cache_control(
             extract_header_values_decoded(response.headers, b"Cache-Control")
         )
 
         # request header fields nominated by the stored
         # response (if any) match those presented (see Section 4.1)
-        if not self._validate_vary(request=request, response=response):
+        if not self._validate_vary(
+            request=request, response=response, original_request=original_request
+        ):
             # If the vary headers does not match, then do not use the response
             return None  # pragma: no cover
 
         # the stored response does not contain the
         # no-cache directive (Section 5.2.2.4), unless
         # it is successfully validated (Section 4.3)
         if (
```

### Comparing `hishel-0.0.5/hishel/_files.py` & `hishel-0.0.6/hishel/_files.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.5/hishel/_headers.py` & `hishel-0.0.6/hishel/_headers.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.5/hishel/_synchronization.py` & `hishel-0.0.6/hishel/_synchronization.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.5/hishel/_utils.py` & `hishel-0.0.6/hishel/_utils.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.5/hishel/_async/_client.py` & `hishel-0.0.6/hishel/_async/_client.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.5/hishel/_async/_mock.py` & `hishel-0.0.6/hishel/_async/_mock.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.5/hishel/_async/_pool.py` & `hishel-0.0.6/hishel/_async/_pool.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,21 +27,25 @@
             if storage is not None
             else AsyncFileStorage(serializer=JSONSerializer())
         )
         self._controller = controller if controller is not None else Controller()
 
     async def handle_async_request(self, request: Request) -> Response:
         key = generate_key(request)
-        stored_resposne = await self._storage.retreive(key)
+        stored_data = await self._storage.retreive(key)
 
-        if stored_resposne:
+        if stored_data:
             # Try using the stored response if it was discovered.
 
+            stored_resposne, stored_request = stored_data
+
             res = self._controller.construct_response_from_cache(
-                request=request, response=stored_resposne
+                request=request,
+                response=stored_resposne,
+                original_request=stored_request,
             )
 
             if isinstance(res, Response):
                 # Simply use the response if the controller determines it is ready for use.
                 res.extensions["from_cache"] = True  # type: ignore[index]
                 return res
 
@@ -52,23 +56,23 @@
 
                 # Merge headers with the stale response.
                 full_response = self._controller.handle_validation_response(
                     old_response=stored_resposne, new_response=response
                 )
 
                 await full_response.aread()
-                await self._storage.store(key, full_response)
+                await self._storage.store(key, response=full_response, request=request)
                 full_response.extensions["from_cache"] = response.status == 304  # type: ignore[index]
                 return full_response
 
         response = await self._pool.handle_async_request(request)
 
         if self._controller.is_cachable(request=request, response=response):
             await response.aread()
-            await self._storage.store(key, response)
+            await self._storage.store(key, response=response, request=request)
 
         response.extensions["from_cache"] = False  # type: ignore[index]
         return response
 
     async def aclose(self) -> None:
         await self._storage.aclose()
```

### Comparing `hishel-0.0.5/hishel/_async/_storages.py` & `hishel-0.0.6/hishel/_async/_storages.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import time
 import typing as tp
 from pathlib import Path
 
 import redis.asyncio as redis
-from httpcore import Response
+from httpcore import Request, Response
 
 from hishel._serializers import BaseSerializer
 
 from .._files import AsyncFileManager
 from .._serializers import JSONSerializer
 from .._synchronization import AsyncLock
 
@@ -20,18 +20,18 @@
 class AsyncBaseStorage:
     def __init__(self, serializer: tp.Optional[BaseSerializer] = None) -> None:
         if serializer:  # pragma: no cover
             self._serializer = serializer
         else:
             self._serializer = JSONSerializer()
 
-    async def store(self, key: str, response: Response) -> None:
+    async def store(self, key: str, response: Response, request: Request) -> None:
         raise NotImplementedError()
 
-    async def retreive(self, key: str) -> tp.Optional[Response]:
+    async def retreive(self, key: str) -> tp.Optional[tp.Tuple[Response, Request]]:
         raise NotImplementedError()
 
     async def aclose(self) -> None:
         raise NotImplementedError()
 
 
 class AsyncFileStorage(AsyncBaseStorage):
@@ -50,24 +50,25 @@
         if not self._base_path.is_dir():
             self._base_path.mkdir(parents=True)
 
         self._file_manager = AsyncFileManager(is_binary=self._serializer.is_binary)
         self._ttl = ttl
         self._lock = AsyncLock()
 
-    async def store(self, key: str, response: Response) -> None:
+    async def store(self, key: str, response: Response, request: Request) -> None:
         response_path = self._base_path / key
 
         async with self._lock:
             await self._file_manager.write_to(
-                str(response_path), self._serializer.dumps(response)
+                str(response_path),
+                self._serializer.dumps(response=response, request=request),
             )
         await self._remove_expired_caches()
 
-    async def retreive(self, key: str) -> tp.Optional[Response]:
+    async def retreive(self, key: str) -> tp.Optional[tp.Tuple[Response, Request]]:
         response_path = self._base_path / key
 
         async with self._lock:
             if response_path.exists():
                 return self._serializer.loads(
                     await self._file_manager.read_from(str(response_path))
                 )
@@ -100,18 +101,22 @@
 
         if client is None:
             self._client = redis.Redis()  # type: ignore
         else:  # pragma: no cover
             self._client = client
         self._ttl = ttl
 
-    async def store(self, key: str, response: Response) -> None:
-        await self._client.set(key, self._serializer.dumps(response), ex=self._ttl)
+    async def store(self, key: str, response: Response, request: Request) -> None:
+        await self._client.set(
+            key,
+            self._serializer.dumps(response=response, request=request),
+            ex=self._ttl,
+        )
 
-    async def retreive(self, key: str) -> tp.Optional[Response]:
+    async def retreive(self, key: str) -> tp.Optional[tp.Tuple[Response, Request]]:
         cached_response = await self._client.get(key)
         if cached_response is None:
             return None
 
         return self._serializer.loads(cached_response)
 
     async def aclose(self) -> None:  # pragma: no cover
```

### Comparing `hishel-0.0.5/hishel/_async/_transports.py` & `hishel-0.0.6/hishel/_async/_transports.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,21 +47,25 @@
                 target=request.url.raw_path,
             ),
             headers=request.headers.raw,
             content=request.stream,
             extensions=request.extensions,
         )
         key = generate_key(httpcore_request)
-        stored_resposne = await self._storage.retreive(key)
+        stored_data = await self._storage.retreive(key)
 
-        if stored_resposne:
+        if stored_data:
             # Try using the stored response if it was discovered.
 
+            stored_resposne, stored_request = stored_data
+
             res = self._controller.construct_response_from_cache(
-                request=httpcore_request, response=stored_resposne
+                request=httpcore_request,
+                response=stored_resposne,
+                original_request=stored_request,
             )
 
             if isinstance(res, httpcore.Response):
                 # Simply use the response if the controller determines it is ready for use.
                 assert isinstance(res.stream, tp.AsyncIterable)
                 res.extensions["from_cache"] = True  # type: ignore[index]
                 return Response(
@@ -93,15 +97,17 @@
 
                 # Merge headers with the stale response.
                 full_response = self._controller.handle_validation_response(
                     old_response=stored_resposne, new_response=httpcore_response
                 )
 
                 await full_response.aread()
-                await self._storage.store(key, full_response)
+                await self._storage.store(
+                    key, response=full_response, request=httpcore_request
+                )
 
                 assert isinstance(full_response.stream, tp.AsyncIterable)
                 full_response.extensions["from_cache"] = (  # type: ignore[index]
                     httpcore_response.status == 304
                 )
                 return Response(
                     status_code=full_response.status,
@@ -119,15 +125,17 @@
             extensions=response.extensions,
         )
         await httpcore_response.aread()
 
         if self._controller.is_cachable(
             request=httpcore_request, response=httpcore_response
         ):
-            await self._storage.store(key, httpcore_response)
+            await self._storage.store(
+                key, response=httpcore_response, request=httpcore_request
+            )
 
         response.extensions["from_cache"] = False  # type: ignore[index]
         return Response(
             status_code=httpcore_response.status,
             headers=httpcore_response.headers,
             stream=AsyncResponseStream(fake_stream(httpcore_response.content)),
             extensions=httpcore_response.extensions,
```

### Comparing `hishel-0.0.5/hishel/_sync/_client.py` & `hishel-0.0.6/hishel/_sync/_client.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.5/hishel/_sync/_mock.py` & `hishel-0.0.6/hishel/_sync/_mock.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.5/hishel/_sync/_pool.py` & `hishel-0.0.6/hishel/_sync/_pool.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,21 +27,25 @@
             if storage is not None
             else FileStorage(serializer=JSONSerializer())
         )
         self._controller = controller if controller is not None else Controller()
 
     def handle_request(self, request: Request) -> Response:
         key = generate_key(request)
-        stored_resposne = self._storage.retreive(key)
+        stored_data = self._storage.retreive(key)
 
-        if stored_resposne:
+        if stored_data:
             # Try using the stored response if it was discovered.
 
+            stored_resposne, stored_request = stored_data
+
             res = self._controller.construct_response_from_cache(
-                request=request, response=stored_resposne
+                request=request,
+                response=stored_resposne,
+                original_request=stored_request,
             )
 
             if isinstance(res, Response):
                 # Simply use the response if the controller determines it is ready for use.
                 res.extensions["from_cache"] = True  # type: ignore[index]
                 return res
 
@@ -52,23 +56,23 @@
 
                 # Merge headers with the stale response.
                 full_response = self._controller.handle_validation_response(
                     old_response=stored_resposne, new_response=response
                 )
 
                 full_response.read()
-                self._storage.store(key, full_response)
+                self._storage.store(key, response=full_response, request=request)
                 full_response.extensions["from_cache"] = response.status == 304  # type: ignore[index]
                 return full_response
 
         response = self._pool.handle_request(request)
 
         if self._controller.is_cachable(request=request, response=response):
             response.read()
-            self._storage.store(key, response)
+            self._storage.store(key, response=response, request=request)
 
         response.extensions["from_cache"] = False  # type: ignore[index]
         return response
 
     def close(self) -> None:
         self._storage.close()
```

### Comparing `hishel-0.0.5/hishel/_sync/_storages.py` & `hishel-0.0.6/hishel/_sync/_storages.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import time
 import typing as tp
 from pathlib import Path
 
 import redis
-from httpcore import Response
+from httpcore import Request, Response
 
 from hishel._serializers import BaseSerializer
 
 from .._files import FileManager
 from .._serializers import JSONSerializer
 from .._synchronization import Lock
 
@@ -20,18 +20,18 @@
 class BaseStorage:
     def __init__(self, serializer: tp.Optional[BaseSerializer] = None) -> None:
         if serializer:  # pragma: no cover
             self._serializer = serializer
         else:
             self._serializer = JSONSerializer()
 
-    def store(self, key: str, response: Response) -> None:
+    def store(self, key: str, response: Response, request: Request) -> None:
         raise NotImplementedError()
 
-    def retreive(self, key: str) -> tp.Optional[Response]:
+    def retreive(self, key: str) -> tp.Optional[tp.Tuple[Response, Request]]:
         raise NotImplementedError()
 
     def close(self) -> None:
         raise NotImplementedError()
 
 
 class FileStorage(BaseStorage):
@@ -50,24 +50,25 @@
         if not self._base_path.is_dir():
             self._base_path.mkdir(parents=True)
 
         self._file_manager = FileManager(is_binary=self._serializer.is_binary)
         self._ttl = ttl
         self._lock = Lock()
 
-    def store(self, key: str, response: Response) -> None:
+    def store(self, key: str, response: Response, request: Request) -> None:
         response_path = self._base_path / key
 
         with self._lock:
             self._file_manager.write_to(
-                str(response_path), self._serializer.dumps(response)
+                str(response_path),
+                self._serializer.dumps(response=response, request=request),
             )
         self._remove_expired_caches()
 
-    def retreive(self, key: str) -> tp.Optional[Response]:
+    def retreive(self, key: str) -> tp.Optional[tp.Tuple[Response, Request]]:
         response_path = self._base_path / key
 
         with self._lock:
             if response_path.exists():
                 return self._serializer.loads(
                     self._file_manager.read_from(str(response_path))
                 )
@@ -100,18 +101,22 @@
 
         if client is None:
             self._client = redis.Redis()  # type: ignore
         else:  # pragma: no cover
             self._client = client
         self._ttl = ttl
 
-    def store(self, key: str, response: Response) -> None:
-        self._client.set(key, self._serializer.dumps(response), ex=self._ttl)
+    def store(self, key: str, response: Response, request: Request) -> None:
+        self._client.set(
+            key,
+            self._serializer.dumps(response=response, request=request),
+            ex=self._ttl,
+        )
 
-    def retreive(self, key: str) -> tp.Optional[Response]:
+    def retreive(self, key: str) -> tp.Optional[tp.Tuple[Response, Request]]:
         cached_response = self._client.get(key)
         if cached_response is None:
             return None
 
         return self._serializer.loads(cached_response)
 
     def close(self) -> None:  # pragma: no cover
```

### Comparing `hishel-0.0.5/hishel/_sync/_transports.py` & `hishel-0.0.6/hishel/_sync/_transports.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,21 +47,25 @@
                 target=request.url.raw_path,
             ),
             headers=request.headers.raw,
             content=request.stream,
             extensions=request.extensions,
         )
         key = generate_key(httpcore_request)
-        stored_resposne = self._storage.retreive(key)
+        stored_data = self._storage.retreive(key)
 
-        if stored_resposne:
+        if stored_data:
             # Try using the stored response if it was discovered.
 
+            stored_resposne, stored_request = stored_data
+
             res = self._controller.construct_response_from_cache(
-                request=httpcore_request, response=stored_resposne
+                request=httpcore_request,
+                response=stored_resposne,
+                original_request=stored_request,
             )
 
             if isinstance(res, httpcore.Response):
                 # Simply use the response if the controller determines it is ready for use.
                 assert isinstance(res.stream, tp.Iterable)
                 res.extensions["from_cache"] = True  # type: ignore[index]
                 return Response(
@@ -93,15 +97,17 @@
 
                 # Merge headers with the stale response.
                 full_response = self._controller.handle_validation_response(
                     old_response=stored_resposne, new_response=httpcore_response
                 )
 
                 full_response.read()
-                self._storage.store(key, full_response)
+                self._storage.store(
+                    key, response=full_response, request=httpcore_request
+                )
 
                 assert isinstance(full_response.stream, tp.Iterable)
                 full_response.extensions["from_cache"] = (  # type: ignore[index]
                     httpcore_response.status == 304
                 )
                 return Response(
                     status_code=full_response.status,
@@ -119,15 +125,17 @@
             extensions=response.extensions,
         )
         httpcore_response.read()
 
         if self._controller.is_cachable(
             request=httpcore_request, response=httpcore_response
         ):
-            self._storage.store(key, httpcore_response)
+            self._storage.store(
+                key, response=httpcore_response, request=httpcore_request
+            )
 
         response.extensions["from_cache"] = False  # type: ignore[index]
         return Response(
             status_code=httpcore_response.status,
             headers=httpcore_response.headers,
             stream=ResponseStream(fake_stream(httpcore_response.content)),
             extensions=httpcore_response.extensions,
```

### Comparing `hishel-0.0.5/LICENSE` & `hishel-0.0.6/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright © 2020, Karen Petrosyan.
+Copyright © 2023, Karen Petrosyan.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `hishel-0.0.5/pyproject.toml` & `hishel-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hishel-0.0.5/PKG-INFO` & `hishel-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hishel
-Version: 0.0.5
+Version: 0.0.6
 Summary: Persistant cache implementation for httpx and httpcore
 Project-URL: Homepage, https://github.com/karosis88/hishel
 Project-URL: Source, https://github.com/karosis88/hishel
 Author-email: Kar Petrosyan <kar.petrosyanpy@gmail.com>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
@@ -135,14 +135,19 @@
 
 - Fork the project.
 - Make change.
 - Open the pull request.
 
 # Changelog
 
+## 0.0.6 (7/29/2023)
+
+- Fix `Vary` header validation. (#8)
+- Dump original requests with the responses (#7) 
+
 ## 0.0.5 (7/29/2023)
 
 - Fix httpx response streaming.
 
 ## 0.0.4 (7/29/2023)
 
 - Change `YamlSerializer` name to `YAMLSerializer`.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hishel Version: 0.0.5 Summary: Persistant cache
+Metadata-Version: 2.1 Name: hishel Version: 0.0.6 Summary: Persistant cache
 implementation for httpx and httpcore Project-URL: Homepage, https://
 github.com/karosis88/hishel Project-URL: Source, https://github.com/karosis88/
 hishel Author-email: Kar Petrosyan
 petrosyanpy@gmail.com> License-Expression: BSD-3-Clause License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Web
 Environment Classifier: Framework :: AsyncIO Classifier: Framework :: Trio
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
@@ -59,13 +59,14 @@
 from the cache ``` ## How and where are the responses saved? The responses are
 stored by `Hishel` in [storages](https://karosis88.github.io/hishel/userguide/
 #storages). You have complete control over them; you can change storage or even
 write your own if necessary. ## Contributing `Hishel` is a powerful tool, but
 it is also a new project with potential flaws, so we welcome contributions! You
 can open the pull request by following these instructions if you want to
 improve `Hishel`. ð - Fork the project. - Make change. - Open the pull
-request. # Changelog ## 0.0.5 (7/29/2023) - Fix httpx response streaming. ##
-0.0.4 (7/29/2023) - Change `YamlSerializer` name to `YAMLSerializer`. ## 0.0.3
-(7/28/2023) - Add `from_cache` response extension. - Add `typing_extensions`
-into the requirements. ## 0.0.2 (7/25/2023) - Add [redis](https://redis.io/
-) support. - Make backends thread and task safe. - Add black as a new linter. -
-Add an expire time for cached responses.
+request. # Changelog ## 0.0.6 (7/29/2023) - Fix `Vary` header validation. (#8)
+- Dump original requests with the responses (#7) ## 0.0.5 (7/29/2023) - Fix
+httpx response streaming. ## 0.0.4 (7/29/2023) - Change `YamlSerializer` name
+to `YAMLSerializer`. ## 0.0.3 (7/28/2023) - Add `from_cache` response
+extension. - Add `typing_extensions` into the requirements. ## 0.0.2 (7/25/
+2023) - Add [redis](https://redis.io/) support. - Make backends thread and task
+safe. - Add black as a new linter. - Add an expire time for cached responses.
```

