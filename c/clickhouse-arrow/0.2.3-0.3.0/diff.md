# Comparing `tmp/clickhouse_arrow-0.2.3.tar.gz` & `tmp/clickhouse_arrow-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickhouse_arrow-0.2.3.tar", max compression
+gzip compressed data, was "clickhouse_arrow-0.3.0.tar", max compression
```

## Comparing `clickhouse_arrow-0.2.3.tar` & `clickhouse_arrow-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11361 2023-03-25 13:20:32.938480 clickhouse_arrow-0.2.3/LICENSE
--rw-r--r--   0        0        0     1275 2023-03-25 13:18:15.085427 clickhouse_arrow-0.2.3/README.md
--rw-r--r--   0        0        0     7489 2023-04-06 05:55:41.050547 clickhouse_arrow-0.2.3/clickhouse_arrow/__init__.py
--rw-r--r--   0        0        0      691 2023-07-03 18:56:36.388150 clickhouse_arrow-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1925 1970-01-01 00:00:00.000000 clickhouse_arrow-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    11361 2023-03-25 13:20:32.938480 clickhouse_arrow-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1275 2023-03-25 13:18:15.085427 clickhouse_arrow-0.3.0/README.md
+-rw-r--r--   0        0        0     7477 2023-07-30 06:14:44.522060 clickhouse_arrow-0.3.0/clickhouse_arrow/__init__.py
+-rw-r--r--   0        0        0      691 2023-07-30 06:14:44.522240 clickhouse_arrow-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1925 1970-01-01 00:00:00.000000 clickhouse_arrow-0.3.0/PKG-INFO
```

### Comparing `clickhouse_arrow-0.2.3/LICENSE` & `clickhouse_arrow-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clickhouse_arrow-0.2.3/README.md` & `clickhouse_arrow-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `clickhouse_arrow-0.2.3/clickhouse_arrow/__init__.py` & `clickhouse_arrow-0.3.0/clickhouse_arrow/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,32 +23,32 @@
 
 
 class Client:
     """
     A minimal client that uses the ClickHouse HTTP API and Apache Arrow.
 
     Args:
-       url: (str) The host name of the server to connect to.
-       user: (str) The optional username to authenticate with.
-       password: (str) The optional password to authenticate with.
+       url: (str) The host name of the server to connect to, defaults to `http://localhost:8123/`.
+       user: (str) The optional username to authenticate with, defaults to `default`.
+       password: (str) The optional password to authenticate with, defaults to empty.
        pool: (PoolManager) The optional HTTP connection pool to use.
     """
 
     def __init__(
         self,
         url: str = "http://localhost:8123/",
         user: str = "default",
         password: str = "",
         pool: urllib3.PoolManager = None,
     ):
-        self._url = build_url(
-            url,
-            user=user,
-            password=password,
-        )
+        self._url = url
+        self._headers = {
+            "X-ClickHouse-User": user,
+            "X-ClickHouse-Key": password,
+        }
         self._pool = pool or urllib3.PoolManager()
 
     def execute(
         self,
         query: str,
         params: dict[str, Any] = None,
         settings: dict[str, Any] = None,
@@ -156,17 +156,16 @@
             data: (pyarrow.Table) The table of the data.
 
         Raises:
             ClickhouseException: When a non-success response status was received.
         """
         columns = ", ".join(f"`{c}`" for c in data.column_names)
         query = f"INSERT INTO {table} ({columns}) FORMAT Arrow"
-        params = urlencode({"query": query})
-        url = f"{self._url}&{params}"
-        headers = {"Content-Type": "application/octet-stream"}
+        url = append_url(self._url, query=query)
+        headers = self._headers | {"Content-Type": "application/octet-stream"}
         body = serialize_ipc(data)
         response = self._pool.urlopen(
             "POST",
             url,
             headers=headers,
             body=body,
         )
@@ -179,15 +178,15 @@
         settings: dict = None,
         format_: str = None,
     ):
         if format_:
             query += f" FORMAT {format_}"
         fields = create_post_body(query, params)
         body, content_type = urllib3.encode_multipart_formdata(fields)
-        headers = {"Content-Type": content_type}
+        headers = self._headers | {"Content-Type": content_type}
         url = append_url(self._url, **settings) if settings else self._url
         response = self._pool.urlopen(
             "POST",
             url,
             body=body,
             headers=headers,
             preload_content=False,
@@ -207,20 +206,16 @@
 
     def __init__(self, status, body):
         super().__init__(f"Unexpected HTTP response status code: {status}.")
         self.status = status
         self.body = body
 
 
-def build_url(url: str, **query) -> str:
-    return f"{url}{'?' if not url.endswith('?') else ''}{urlencode(query)}"
-
-
 def append_url(url: str, **query) -> str:
-    return f"{url}&{urlencode(query)}"
+    return f"{url}?{urlencode(query)}"
 
 
 def create_post_body(query: str, params: dict[str, Any]):
     body = {"query": query}
     if params:
         body.update({f"param_{k}": v for k, v in params.items()})
     return body
```

### Comparing `clickhouse_arrow-0.2.3/PKG-INFO` & `clickhouse_arrow-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clickhouse-arrow
-Version: 0.2.3
+Version: 0.3.0
 Summary: A minimal client that uses the ClickHouse HTTP API and Apache Arrow.
 Home-page: https://github.com/galpin/clickhouse-arrow
 Author: Martin Galpin
 Author-email: galpin@galpin.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

