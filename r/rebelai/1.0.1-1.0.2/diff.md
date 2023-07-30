# Comparing `tmp/rebelai-1.0.1-py2.py3-none-any.whl.zip` & `tmp/rebelai-1.0.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 17907 bytes, number of entries: 11
--rw-r--r--  2.0 unx      129 b- defN 23-Jul-30 19:50 rebelai/__init__.py
+Zip file size: 17943 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      129 b- defN 23-Jul-30 20:14 rebelai/__init__.py
 -rw-r--r--  2.0 unx     2002 b- defN 23-Jul-30 19:36 rebelai/const.py
 -rw-r--r--  2.0 unx     3555 b- defN 23-Jul-30 19:35 rebelai/enums.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 19:33 rebelai/py.typed
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 19:33 rebelai/ai/py.typed
--rw-------  2.0 unx    35115 b- defN 23-Jul-30 19:51 rebelai-1.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2903 b- defN 23-Jul-30 19:51 rebelai-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jul-30 19:51 rebelai-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-30 19:51 rebelai-1.0.1.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-30 15:48 rebelai-1.0.1.dist-info/zip-safe
--rw-rw-r--  2.0 unx      837 b- defN 23-Jul-30 19:51 rebelai-1.0.1.dist-info/RECORD
-11 files, 44660 bytes uncompressed, 16495 bytes compressed:  63.1%
+-rw-------  2.0 unx    35115 b- defN 23-Jul-30 20:15 rebelai-1.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3091 b- defN 23-Jul-30 20:15 rebelai-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-30 20:15 rebelai-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-30 20:15 rebelai-1.0.2.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-30 15:48 rebelai-1.0.2.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      837 b- defN 23-Jul-30 20:15 rebelai-1.0.2.dist-info/RECORD
+11 files, 44848 bytes uncompressed, 16531 bytes compressed:  63.1%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: rebelai/py.typed
 Comment: 
 
 Filename: rebelai/ai/py.typed
 Comment: 
 
-Filename: rebelai-1.0.1.dist-info/LICENSE
+Filename: rebelai-1.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: rebelai-1.0.1.dist-info/METADATA
+Filename: rebelai-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: rebelai-1.0.1.dist-info/WHEEL
+Filename: rebelai-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: rebelai-1.0.1.dist-info/top_level.txt
+Filename: rebelai-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: rebelai-1.0.1.dist-info/zip-safe
+Filename: rebelai-1.0.2.dist-info/zip-safe
 Comment: 
 
-Filename: rebelai-1.0.1.dist-info/RECORD
+Filename: rebelai-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rebelai/__init__.py

```diff
@@ -1,5 +1,5 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """rebelai -- providing free ai access to everyone"""
 
-__version__: str = "1.0.1"
+__version__: str = "1.0.2"
```

## Comparing `rebelai-1.0.1.dist-info/LICENSE` & `rebelai-1.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rebelai-1.0.1.dist-info/METADATA` & `rebelai-1.0.2.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rebelai
-Version: 1.0.1
+Version: 1.0.2
 Summary: providing free access to proprietary ai models in python
 Home-page: https://ari-web.xyz/gh/rebelai
 Author: Ari Archer
 Author-email: ari.web.xyz@gmail.com
 License: GPLv3+
 Keywords: http,http-client,api,https,ai,machine learning,openai
 Classifier: Development Status :: 5 - Production/Stable
@@ -59,14 +59,16 @@
             -   `alpaca_7b` -- the 7 billion neuron alpaca model
         -   `deepai` -- access to all deepai models
             -   `deepai` -- generic function for deepai access for free, takes DeepAIModel, see doc string for more info
         -   `gpt` -- access to "open"ai models ( kinda )
             -   `gpt3` -- access to gpt3 model
             -   `gpt4` -- access to gpt3 model ( youchat )
         -   `pollinations` -- access to pollinations image generation api
+            -   `pollinations` -- access to the generation model
         -   `prodia` -- access to prodia image generation api ( limited access and proxies dont seem to work :( )
+            -   `prodia` -- generic function to access prodia api, takes `ProdiaModel` and `ProdiaSampler`, see doc string
 
 # tips
 
 -   use proxies ( for example gimmeproxy api,, https://gimmeproxy.com/api/getProxy?post=true&get=true&user-agent=true&supportsHttps=true&protocol=http&minSpeed=20&curl=true )
     -   dont forget to test if theyre responsive by making a proxies request to for example https://example.com/
 -   check docstrings, they have info about arguments and proxies
```

## Comparing `rebelai-1.0.1.dist-info/RECORD` & `rebelai-1.0.2.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-rebelai/__init__.py,sha256=11x-sah7ERsOcUA1TIUw4_NB-VmyuX4-VKa1VV_mQX0,129
+rebelai/__init__.py,sha256=8pgHZphmxRyNxDmIsIe8YzgodyOMzTbykJ-eySP0bB0,129
 rebelai/const.py,sha256=Hb06cmLY_zdHrSI-yQOZPSXvZuYvBZZpAegDLqbWVYc,2002
 rebelai/enums.py,sha256=ehaDobrl6JrhUrX4hd6RPl17UphiMMpBy8WFIeaG72w,3555
 rebelai/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 rebelai/ai/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-rebelai-1.0.1.dist-info/LICENSE,sha256=Rgc3Ns1SKdwsPGFZc5xrgE6-VV8DXkUUgP5FRclaUvk,35115
-rebelai-1.0.1.dist-info/METADATA,sha256=BE_z_d6lcOjdn8MWuiH7CjR7Hkzp2dpDWZn-WEHk72k,2903
-rebelai-1.0.1.dist-info/WHEEL,sha256=k3vXr0c0OitO0k9eCWBlI2yTYnpb_n_I2SGzrrfY7HY,110
-rebelai-1.0.1.dist-info/top_level.txt,sha256=rgLyT5avUbh1GgLMKFze_THimdNRD3ht3aiMAF8ysA0,8
-rebelai-1.0.1.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-rebelai-1.0.1.dist-info/RECORD,,
+rebelai-1.0.2.dist-info/LICENSE,sha256=Rgc3Ns1SKdwsPGFZc5xrgE6-VV8DXkUUgP5FRclaUvk,35115
+rebelai-1.0.2.dist-info/METADATA,sha256=L9nV3XHzZXIE72o3o95Ss5V6EWOXXTMA5KutWxxYiME,3091
+rebelai-1.0.2.dist-info/WHEEL,sha256=k3vXr0c0OitO0k9eCWBlI2yTYnpb_n_I2SGzrrfY7HY,110
+rebelai-1.0.2.dist-info/top_level.txt,sha256=rgLyT5avUbh1GgLMKFze_THimdNRD3ht3aiMAF8ysA0,8
+rebelai-1.0.2.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+rebelai-1.0.2.dist-info/RECORD,,
```

