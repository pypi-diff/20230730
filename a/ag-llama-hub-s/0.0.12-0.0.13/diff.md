# Comparing `tmp/ag_llama_hub_s-0.0.12.tar.gz` & `tmp/ag_llama_hub_s-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ag_llama_hub_s-0.0.12.tar", last modified: Sun Jul 30 10:10:51 2023, max compression
+gzip compressed data, was "dist\ag_llama_hub_s-0.0.13.tar", last modified: Sun Jul 30 10:31:36 2023, max compression
```

## Comparing `ag_llama_hub_s-0.0.12.tar` & `ag_llama_hub_s-0.0.13.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 10:10:51.923236 ag_llama_hub_s-0.0.12/
--rw-rw-rw-   0        0        0      835 2023-07-30 10:10:51.922268 ag_llama_hub_s-0.0.12/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-30 10:10:51.908188 ag_llama_hub_s-0.0.12/ag_llama_hub_s/
--rw-rw-rw-   0        0        0     2102 2023-07-25 14:37:05.000000 ag_llama_hub_s-0.0.12/ag_llama_hub_s/__init__.py
--rw-rw-rw-   0        0        0     3643 2023-07-30 09:17:59.000000 ag_llama_hub_s-0.0.12/ag_llama_hub_s/__main__.py
--rw-rw-rw-   0        0        0     5370 2023-07-30 10:10:40.000000 ag_llama_hub_s-0.0.12/ag_llama_hub_s/model.py
-drwxrwxrwx   0        0        0        0 2023-07-30 10:10:51.917250 ag_llama_hub_s-0.0.12/ag_llama_hub_s.egg-info/
--rw-rw-rw-   0        0        0      835 2023-07-30 10:10:51.000000 ag_llama_hub_s-0.0.12/ag_llama_hub_s.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2023-07-30 10:10:51.000000 ag_llama_hub_s-0.0.12/ag_llama_hub_s.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 10:10:51.000000 ag_llama_hub_s-0.0.12/ag_llama_hub_s.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      235 2023-07-30 10:10:51.000000 ag_llama_hub_s-0.0.12/ag_llama_hub_s.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-30 10:10:51.000000 ag_llama_hub_s-0.0.12/ag_llama_hub_s.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-30 10:10:51.924232 ag_llama_hub_s-0.0.12/setup.cfg
--rw-rw-rw-   0        0        0     2569 2023-07-30 09:10:29.000000 ag_llama_hub_s-0.0.12/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-30 10:10:51.920241 ag_llama_hub_s-0.0.12/utils/
--rw-rw-rw-   0        0        0     1238 2023-06-10 04:41:23.000000 ag_llama_hub_s-0.0.12/utils/download.py
--rw-rw-rw-   0        0        0      595 2023-06-10 04:41:23.000000 ag_llama_hub_s-0.0.12/utils/render.py
+drwxrwxrwx   0        0        0        0 2023-07-30 10:31:36.414731 ag_llama_hub_s-0.0.13/
+-rw-rw-rw-   0        0        0      835 2023-07-30 10:31:36.412736 ag_llama_hub_s-0.0.13/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-30 10:31:36.399388 ag_llama_hub_s-0.0.13/ag_llama_hub_s/
+-rw-rw-rw-   0        0        0     2102 2023-07-25 14:37:05.000000 ag_llama_hub_s-0.0.13/ag_llama_hub_s/__init__.py
+-rw-rw-rw-   0        0        0     3643 2023-07-30 09:17:59.000000 ag_llama_hub_s-0.0.13/ag_llama_hub_s/__main__.py
+-rw-rw-rw-   0        0        0     5462 2023-07-30 10:31:32.000000 ag_llama_hub_s-0.0.13/ag_llama_hub_s/model.py
+drwxrwxrwx   0        0        0        0 2023-07-30 10:31:36.408467 ag_llama_hub_s-0.0.13/ag_llama_hub_s.egg-info/
+-rw-rw-rw-   0        0        0      835 2023-07-30 10:31:36.000000 ag_llama_hub_s-0.0.13/ag_llama_hub_s.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2023-07-30 10:31:36.000000 ag_llama_hub_s-0.0.13/ag_llama_hub_s.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 10:31:36.000000 ag_llama_hub_s-0.0.13/ag_llama_hub_s.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      235 2023-07-30 10:31:36.000000 ag_llama_hub_s-0.0.13/ag_llama_hub_s.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-30 10:31:36.000000 ag_llama_hub_s-0.0.13/ag_llama_hub_s.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 10:31:36.414731 ag_llama_hub_s-0.0.13/setup.cfg
+-rw-rw-rw-   0        0        0     2569 2023-07-30 09:10:29.000000 ag_llama_hub_s-0.0.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 10:31:36.411738 ag_llama_hub_s-0.0.13/utils/
+-rw-rw-rw-   0        0        0     1238 2023-06-10 04:41:23.000000 ag_llama_hub_s-0.0.13/utils/download.py
+-rw-rw-rw-   0        0        0      595 2023-06-10 04:41:23.000000 ag_llama_hub_s-0.0.13/utils/render.py
```

### Comparing `ag_llama_hub_s-0.0.12/PKG-INFO` & `ag_llama_hub_s-0.0.13/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ag_llama_hub_s
-Version: 0.0.12
+Version: 0.0.13
 Summary: ag_llama_hub Test Package for Somthing
 Home-page: UNKNOWN
 Author: AA
 License: UNKNOWN
 Description: long_description
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ag_llama_hub_s-0.0.12/ag_llama_hub_s/__init__.py` & `ag_llama_hub_s-0.0.13/ag_llama_hub_s/__init__.py`

 * *Files identical despite different names*

### Comparing `ag_llama_hub_s-0.0.12/ag_llama_hub_s/__main__.py` & `ag_llama_hub_s-0.0.13/ag_llama_hub_s/__main__.py`

 * *Files identical despite different names*

### Comparing `ag_llama_hub_s-0.0.12/ag_llama_hub_s/model.py` & `ag_llama_hub_s-0.0.13/ag_llama_hub_s/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -123,14 +123,17 @@
     """Load a text generation model and make it stream-able."""
     logger.info(f"Loading tokenizer from {name_or_path}")
     tokenizer = LlamaTokenizer.from_pretrained(name_or_path)
     logger.info(f"Tokenizer loaded")
     logger.info(f"Loading model from {name_or_path}")
     model = LlamaForCausalLM.from_pretrained(name_or_path, device_map="auto", load_in_8bit=load_in_8bit)
     logger.info(f"Model loaded")
+    logger.info(f"Tieing weights")
+    model.tie_weights()
+    logger.info(f"Weights tied")
     # Check if the model has text generation capabilities.
     if not model.can_generate():
         logger.error(f"{name_or_path} is not a text generation model")
         raise TypeError(f"{name_or_path} is not a text generation model")
 
     return StreamModel(model, tokenizer,path=name_or_path)
```

### Comparing `ag_llama_hub_s-0.0.12/ag_llama_hub_s.egg-info/PKG-INFO` & `ag_llama_hub_s-0.0.13/ag_llama_hub_s.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ag-llama-hub-s
-Version: 0.0.12
+Version: 0.0.13
 Summary: ag_llama_hub Test Package for Somthing
 Home-page: UNKNOWN
 Author: AA
 License: UNKNOWN
 Description: long_description
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ag_llama_hub_s-0.0.12/setup.py` & `ag_llama_hub_s-0.0.13/setup.py`

 * *Files identical despite different names*

### Comparing `ag_llama_hub_s-0.0.12/utils/download.py` & `ag_llama_hub_s-0.0.13/utils/download.py`

 * *Files identical despite different names*

### Comparing `ag_llama_hub_s-0.0.12/utils/render.py` & `ag_llama_hub_s-0.0.13/utils/render.py`

 * *Files identical despite different names*

