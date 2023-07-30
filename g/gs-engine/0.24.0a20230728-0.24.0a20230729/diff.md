# Comparing `tmp/gs_engine-0.24.0a20230728-py2.py3-none-macosx_11_0_x86_64.whl.zip` & `tmp/gs_engine-0.24.0a20230729-py2.py3-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 12192 bytes, number of entries: 9
--rw-rw-r--  2.0 unx      840 b- defN 23-Jul-28 21:19 gs_engine-0.24.0a20230728.dist-info/RECORD
--rw-r--r--  2.0 unx      140 b- defN 23-Jul-28 21:08 gs_engine-0.24.0a20230728.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-Jul-28 21:08 gs_engine-0.24.0a20230728.dist-info/top_level.txt
--rw-r--r--  2.0 unx    22193 b- defN 23-Jul-28 21:08 gs_engine-0.24.0a20230728.dist-info/METADATA
--rw-r--r--  2.0 unx      694 b- defN 23-Jul-28 19:14 graphscope_runtime/__init__.py
--rw-r--r--  2.0 unx     1573 b- defN 23-Jul-28 19:14 graphscope.runtime/conf/log4j2.xml
--rw-r--r--  2.0 unx      398 b- defN 23-Jul-28 19:14 graphscope.runtime/conf/executor.vineyard.properties
--rw-r--r--  2.0 unx      549 b- defN 23-Jul-28 19:14 graphscope.runtime/conf/frontend.vineyard.properties
--rw-r--r--  2.0 unx      204 b- defN 23-Jul-28 19:14 graphscope.runtime/conf/log4rs.yml
-9 files, 26610 bytes uncompressed, 10730 bytes compressed:  59.7%
+Zip file size: 12194 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      694 b- defN 23-Jul-29 19:04 graphscope_runtime/__init__.py
+-rw-rw-r--  2.0 unx      840 b- defN 23-Jul-29 20:58 gs_engine-0.24.0a20230729.dist-info/RECORD
+-rw-r--r--  2.0 unx      140 b- defN 23-Jul-29 20:48 gs_engine-0.24.0a20230729.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-Jul-29 20:48 gs_engine-0.24.0a20230729.dist-info/top_level.txt
+-rw-r--r--  2.0 unx    22193 b- defN 23-Jul-29 20:48 gs_engine-0.24.0a20230729.dist-info/METADATA
+-rw-r--r--  2.0 unx     1573 b- defN 23-Jul-29 19:04 graphscope.runtime/conf/log4j2.xml
+-rw-r--r--  2.0 unx      398 b- defN 23-Jul-29 19:04 graphscope.runtime/conf/executor.vineyard.properties
+-rw-r--r--  2.0 unx      549 b- defN 23-Jul-29 19:04 graphscope.runtime/conf/frontend.vineyard.properties
+-rw-r--r--  2.0 unx      204 b- defN 23-Jul-29 19:04 graphscope.runtime/conf/log4rs.yml
+9 files, 26610 bytes uncompressed, 10732 bytes compressed:  59.7%
```

## zipnote {}

```diff
@@ -1,20 +1,20 @@
-Filename: gs_engine-0.24.0a20230728.dist-info/RECORD
+Filename: graphscope_runtime/__init__.py
 Comment: 
 
-Filename: gs_engine-0.24.0a20230728.dist-info/WHEEL
+Filename: gs_engine-0.24.0a20230729.dist-info/RECORD
 Comment: 
 
-Filename: gs_engine-0.24.0a20230728.dist-info/top_level.txt
+Filename: gs_engine-0.24.0a20230729.dist-info/WHEEL
 Comment: 
 
-Filename: gs_engine-0.24.0a20230728.dist-info/METADATA
+Filename: gs_engine-0.24.0a20230729.dist-info/top_level.txt
 Comment: 
 
-Filename: graphscope_runtime/__init__.py
+Filename: gs_engine-0.24.0a20230729.dist-info/METADATA
 Comment: 
 
 Filename: graphscope.runtime/conf/log4j2.xml
 Comment: 
 
 Filename: graphscope.runtime/conf/executor.vineyard.properties
 Comment:
```

## Comparing `gs_engine-0.24.0a20230728.dist-info/RECORD` & `gs_engine-0.24.0a20230729.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-gs_engine-0.24.0a20230728.dist-info/RECORD,,
-gs_engine-0.24.0a20230728.dist-info/WHEEL,sha256=JeJsisTYcAevTYzb1wnrct0jVz24aCikiWmejptvi8w,140
-gs_engine-0.24.0a20230728.dist-info/top_level.txt,sha256=8OYX8275H-myeSCvZ0ZHMFaQrPlxRlQfm6Z2pK0SbFw,19
-gs_engine-0.24.0a20230728.dist-info/METADATA,sha256=8N_BgIaeR-RO1Q_JpCtUOv0qI5bdjgpHKewYld7NlP4,22193
 graphscope_runtime/__init__.py,sha256=w_Me0NHI5zy8GitMCD7mzOi0Qz7ZfeE2zUI5wGfZIyM,694
+gs_engine-0.24.0a20230729.dist-info/RECORD,,
+gs_engine-0.24.0a20230729.dist-info/WHEEL,sha256=JeJsisTYcAevTYzb1wnrct0jVz24aCikiWmejptvi8w,140
+gs_engine-0.24.0a20230729.dist-info/top_level.txt,sha256=8OYX8275H-myeSCvZ0ZHMFaQrPlxRlQfm6Z2pK0SbFw,19
+gs_engine-0.24.0a20230729.dist-info/METADATA,sha256=0ZtrNShEqFKiBa5EFdRa4WDcmuLWfjtGgYh3u3xdEsM,22193
 graphscope.runtime/conf/log4j2.xml,sha256=JiMUDFQ779aE33kOkah4-VlGQqMVW1_xlzWVZsvhHWQ,1573
 graphscope.runtime/conf/executor.vineyard.properties,sha256=FX6Og8G2x4VrMvdtT-XGjTsDGkY0iTWrLlNUg2aFX6o,398
 graphscope.runtime/conf/frontend.vineyard.properties,sha256=EaH9P5c8ZDA0YrjcVX_4OeASQXI7rF1yIxGO6lblr-c,549
 graphscope.runtime/conf/log4rs.yml,sha256=jFXF2AwsTarQhUr2vH4qD9-TJGdY2vVbvBtGYm-fotM,204
```

## Comparing `gs_engine-0.24.0a20230728.dist-info/METADATA` & `gs_engine-0.24.0a20230729.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gs-engine
-Version: 0.24.0a20230728
+Version: 0.24.0a20230729
 Home-page: https://github.com/alibaba/GraphScope
 Author: GraphScope Team, Damo Academy
 Author-email: graphscope@alibaba-inc.com
 License: Apache License 2.0
 Keywords: GraphScope,Graph Computations
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

