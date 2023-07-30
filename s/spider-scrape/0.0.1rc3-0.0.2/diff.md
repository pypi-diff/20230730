# Comparing `tmp/spider_scrape-0.0.1rc3.tar.gz` & `tmp/spider_scrape-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spider_scrape-0.0.1rc3.tar", max compression
+gzip compressed data, was "spider_scrape-0.0.2.tar", max compression
```

## Comparing `spider_scrape-0.0.1rc3.tar` & `spider_scrape-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1118 2023-07-15 10:16:29.599632 spider_scrape-0.0.1rc3/LICENSE
--rw-r--r--   0        0        0      379 2023-07-15 10:16:29.599729 spider_scrape-0.0.1rc3/README.md
--rw-r--r--   0        0        0      841 2023-07-18 19:56:25.269492 spider_scrape-0.0.1rc3/pyproject.toml
--rw-r--r--   0        0        0      190 2023-07-15 10:16:29.600047 spider_scrape-0.0.1rc3/spider_scrape/__init__.py
--rw-r--r--   0        0        0     1747 2023-07-16 11:47:32.921523 spider_scrape-0.0.1rc3/spider_scrape/arango_db.py
--rw-r--r--   0        0        0     1712 2023-07-18 19:53:25.133023 spider_scrape-0.0.1rc3/spider_scrape/bs.py
--rw-r--r--   0        0        0      455 2023-07-16 11:47:32.914044 spider_scrape-0.0.1rc3/spider_scrape/db.py
--rw-r--r--   0        0        0      746 2023-07-16 11:47:09.633283 spider_scrape-0.0.1rc3/spider_scrape/scraper.py
--rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 spider_scrape-0.0.1rc3/PKG-INFO
+-rw-r--r--   0        0        0     1118 2023-07-30 11:02:59.116864 spider_scrape-0.0.2/LICENSE
+-rw-r--r--   0        0        0      379 2023-07-30 11:02:59.116864 spider_scrape-0.0.2/README.md
+-rw-r--r--   0        0        0      802 2023-07-30 11:02:59.116864 spider_scrape-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      190 2023-07-30 11:02:59.116864 spider_scrape-0.0.2/spider_scrape/__init__.py
+-rw-r--r--   0        0        0     1853 2023-07-30 11:02:59.116864 spider_scrape-0.0.2/spider_scrape/arango_db.py
+-rw-r--r--   0        0        0     1735 2023-07-30 11:02:59.116864 spider_scrape-0.0.2/spider_scrape/bs.py
+-rw-r--r--   0        0        0      455 2023-07-30 11:02:59.116864 spider_scrape-0.0.2/spider_scrape/db.py
+-rw-r--r--   0        0        0      746 2023-07-30 11:02:59.116864 spider_scrape-0.0.2/spider_scrape/scraper.py
+-rw-r--r--   0        0        0     1070 1970-01-01 00:00:00.000000 spider_scrape-0.0.2/PKG-INFO
```

### Comparing `spider_scrape-0.0.1rc3/LICENSE` & `spider_scrape-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spider_scrape-0.0.1rc3/pyproject.toml` & `spider_scrape-0.0.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "spider-scrape"
-version = "0.0.1rc3"
-description = ""
+version = "0.0.2"
+description = "Website Scrape Tool"
 authors = ["Philip May <philip@may.la>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "spider_scrape"}]
 
 [build-system]
 requires = ["poetry-core"]
@@ -15,20 +15,18 @@
 python = "^3.8"
 beautifulsoup4 = "*"
 python-arango = {version = "*", optional = true}
 attrs = "*"
 markdownify = "*"
 mdformat = "*"
 
-[tool.poetry.group.lint]
-optional = true
-
 [tool.poetry.group.lint.dependencies]
-black = {version = "*"}
-ruff = {version = "*"}
+black = "*"
+ruff = "*"
+mypy = "*"
 
 [tool.poetry.extras]
 arango = ["python-arango"]
 
 [tool.black]
 line-length = 119
 target-versions = ["py38", "py39", "py310", "py311"]
```

### Comparing `spider_scrape-0.0.1rc3/spider_scrape/arango_db.py` & `spider_scrape-0.0.2/spider_scrape/arango_db.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,33 +18,37 @@
     db_name: str
     username: str
     password: str
     collection_name: str
     attribute_name: str
     batch_size: int = field(default=20)
 
-    def _get_arango_client(self):
+    def get_arango_client(self):
         arango_client = ArangoClient(hosts=self.hosts)
         return arango_client
 
-    def _get_connection(self, arango_client):
+    def get_connection(self, arango_client):
         connection = arango_client.db(self.db_name, username=self.username, password=self.password)
         return connection
 
     def load_batch(self) -> Sequence:
-        with closing(self._get_arango_client()) as arango_client:
-            connection = self._get_connection(arango_client)
-            bind_vars = {"@coll": self.collection_name, "attribute": self.attribute_name}
+        with closing(self.get_arango_client()) as arango_client:
+            connection = self.get_connection(arango_client)
+            bind_vars = {
+                "@coll": self.collection_name,
+                "attribute": self.attribute_name,
+                "batch_size": self.batch_size,
+            }
             cursor = connection.aql.execute(
-                "FOR doc IN @@coll FILTER !HAS(doc, @attribute) RETURN doc",
+                "FOR doc IN @@coll FILTER !HAS(doc, @attribute) LIMIT @batch_size RETURN doc",
                 bind_vars=bind_vars,
                 batch_size=self.batch_size,
             )
             with closing(cursor) as closing_cursor:
                 batch = closing_cursor.batch()
         return batch
 
     def save_batch(self, batch: Sequence):
-        with closing(self._get_arango_client()) as arango_client:
-            connection = self._get_connection(arango_client)
+        with closing(self.get_arango_client()) as arango_client:
+            connection = self.get_connection(arango_client)
             collection = connection.collection(self.collection_name)
             collection.import_bulk(batch, on_duplicate="update")
```

### Comparing `spider_scrape-0.0.1rc3/spider_scrape/bs.py` & `spider_scrape-0.0.2/spider_scrape/bs.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 
 """Beautiful Soup specific tools."""
 
 import re
 from typing import Optional
 
 import mdformat
-from markdownify import MarkdownConverter, markdownify
+from markdownify import MarkdownConverter, markdownify  # type: ignore
 
 
 def extract_text(soup, join_str=None) -> str:
     if join_str is None:
         join_str = " "
     texts = [text for text in soup.stripped_strings]
-    texts = join_str.join(texts)
-    return texts
+    result: str = join_str.join(texts)
+    return result
 
 
 def normalize_text(text) -> str:
     text = text.replace("\xa0", " ")
     text = text.replace("\u200b", " ")
     text = re.sub("  +", " ", text)
     text = text.strip()
```

### Comparing `spider_scrape-0.0.1rc3/spider_scrape/scraper.py` & `spider_scrape-0.0.2/spider_scrape/scraper.py`

 * *Files identical despite different names*

### Comparing `spider_scrape-0.0.1rc3/PKG-INFO` & `spider_scrape-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: spider-scrape
-Version: 0.0.1rc3
-Summary: 
+Version: 0.0.2
+Summary: Website Scrape Tool
 License: MIT
 Author: Philip May
 Author-email: philip@may.la
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

