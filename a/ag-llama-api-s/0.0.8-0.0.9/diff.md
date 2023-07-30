# Comparing `tmp/ag_llama_api_s-0.0.8.tar.gz` & `tmp/ag_llama_api_s-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ag_llama_api_s-0.0.8.tar", last modified: Thu Jul 27 11:43:12 2023, max compression
+gzip compressed data, was "dist\ag_llama_api_s-0.0.9.tar", last modified: Thu Jul 27 11:50:26 2023, max compression
```

## Comparing `ag_llama_api_s-0.0.8.tar` & `ag_llama_api_s-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 11:43:12.913389 ag_llama_api_s-0.0.8/
--rw-rw-rw-   0        0        0      768 2023-07-27 11:43:12.912392 ag_llama_api_s-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-27 11:43:12.891454 ag_llama_api_s-0.0.8/ag_llama_api_s/
--rw-rw-rw-   0        0        0     2187 2023-07-24 22:23:15.000000 ag_llama_api_s-0.0.8/ag_llama_api_s/__init__.py
--rw-rw-rw-   0        0        0     8785 2023-07-27 11:11:47.000000 ag_llama_api_s-0.0.8/ag_llama_api_s/__main__.py
--rw-rw-rw-   0        0        0     2011 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.8/ag_llama_api_s/choice.py
--rw-rw-rw-   0        0        0     5270 2023-07-27 11:42:39.000000 ag_llama_api_s-0.0.8/ag_llama_api_s/model.py
--rw-rw-rw-   0        0        0     1850 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.8/ag_llama_api_s/tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:43:12.901427 ag_llama_api_s-0.0.8/ag_llama_api_s.egg-info/
--rw-rw-rw-   0        0        0      768 2023-07-27 11:43:12.000000 ag_llama_api_s-0.0.8/ag_llama_api_s.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      427 2023-07-27 11:43:12.000000 ag_llama_api_s-0.0.8/ag_llama_api_s.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 11:43:12.000000 ag_llama_api_s-0.0.8/ag_llama_api_s.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      297 2023-07-27 11:43:12.000000 ag_llama_api_s-0.0.8/ag_llama_api_s.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-27 11:43:12.000000 ag_llama_api_s-0.0.8/ag_llama_api_s.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 11:43:12.914386 ag_llama_api_s-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2571 2023-07-27 10:19:00.000000 ag_llama_api_s-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:43:12.906407 ag_llama_api_s-0.0.8/tests/
--rw-rw-rw-   0        0        0     1121 2023-06-28 17:09:17.000000 ag_llama_api_s-0.0.8/tests/test_choice.py
--rw-rw-rw-   0        0        0     2982 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.8/tests/test_model.py
--rw-rw-rw-   0        0        0     1945 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.8/tests/test_tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:43:12.910396 ag_llama_api_s-0.0.8/utils/
--rw-rw-rw-   0        0        0     1238 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.8/utils/download.py
--rw-rw-rw-   0        0        0      595 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.8/utils/render.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:50:26.359736 ag_llama_api_s-0.0.9/
+-rw-rw-rw-   0        0        0      768 2023-07-27 11:50:26.357742 ag_llama_api_s-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-27 11:50:26.336797 ag_llama_api_s-0.0.9/ag_llama_api_s/
+-rw-rw-rw-   0        0        0     2187 2023-07-24 22:23:15.000000 ag_llama_api_s-0.0.9/ag_llama_api_s/__init__.py
+-rw-rw-rw-   0        0        0     8785 2023-07-27 11:11:47.000000 ag_llama_api_s-0.0.9/ag_llama_api_s/__main__.py
+-rw-rw-rw-   0        0        0     2011 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.9/ag_llama_api_s/choice.py
+-rw-rw-rw-   0        0        0     5753 2023-07-27 11:50:22.000000 ag_llama_api_s-0.0.9/ag_llama_api_s/model.py
+-rw-rw-rw-   0        0        0     1850 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.9/ag_llama_api_s/tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:50:26.346773 ag_llama_api_s-0.0.9/ag_llama_api_s.egg-info/
+-rw-rw-rw-   0        0        0      768 2023-07-27 11:50:26.000000 ag_llama_api_s-0.0.9/ag_llama_api_s.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      427 2023-07-27 11:50:26.000000 ag_llama_api_s-0.0.9/ag_llama_api_s.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 11:50:26.000000 ag_llama_api_s-0.0.9/ag_llama_api_s.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      297 2023-07-27 11:50:26.000000 ag_llama_api_s-0.0.9/ag_llama_api_s.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-27 11:50:26.000000 ag_llama_api_s-0.0.9/ag_llama_api_s.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 11:50:26.359736 ag_llama_api_s-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2571 2023-07-27 10:19:00.000000 ag_llama_api_s-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:50:26.351756 ag_llama_api_s-0.0.9/tests/
+-rw-rw-rw-   0        0        0     1121 2023-06-28 17:09:17.000000 ag_llama_api_s-0.0.9/tests/test_choice.py
+-rw-rw-rw-   0        0        0     2982 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.9/tests/test_model.py
+-rw-rw-rw-   0        0        0     1945 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.9/tests/test_tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:50:26.355748 ag_llama_api_s-0.0.9/utils/
+-rw-rw-rw-   0        0        0     1238 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.9/utils/download.py
+-rw-rw-rw-   0        0        0      595 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.9/utils/render.py
```

### Comparing `ag_llama_api_s-0.0.8/PKG-INFO` & `ag_llama_api_s-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ag_llama_api_s
-Version: 0.0.8
+Version: 0.0.9
 Summary: ag_llama_api_s Test Package for Somthing
 Author: AA
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ag_llama_api_s-0.0.8/ag_llama_api_s/__init__.py` & `ag_llama_api_s-0.0.9/ag_llama_api_s/__init__.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.8/ag_llama_api_s/__main__.py` & `ag_llama_api_s-0.0.9/ag_llama_api_s/__main__.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.8/ag_llama_api_s/choice.py` & `ag_llama_api_s-0.0.9/ag_llama_api_s/choice.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.8/ag_llama_api_s/model.py` & `ag_llama_api_s-0.0.9/ag_llama_api_s/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         self,
         prompt,
         max_tokens=16,
         temperature=1.0,
         top_p=1.0,
     ):
         self.wait_and_clear_gpu()
-        logger.info(f"Got number of tokens: {self.get_tokens_count(prompt)}")
+        logger.info(f"Got number of tokens: {self.get_tokens_count_v2(prompt)}")
         """Create a completion stream for the provided prompt."""
         logger.info(f"Generating pipeline for {self.path}")
         pipe = pipeline(
                 "text-generation",
                 model=self.model,
                 tokenizer=self.tokenizer,
                 max_length=max_tokens,
@@ -76,14 +76,25 @@
             if self.s_tokenizer:
                 return len(self.s_tokenizer.EncodeAsIds(prompt))+1#+1 for eos
             batch = self.tokenizer.encode(prompt, return_tensors="pt")
             return batch.shape[-1]
         elif isinstance(prompt, torch.Tensor) and prompt.dim() == 1:
             return prompt.shape[-1]
         raise TypeError("prompt must be a string or a 1-d tensor")
+    
+    def get_tokens_count_v2(self, prompt):
+        """Tokenize a string into a tensor of token IDs."""
+        if isinstance(prompt, str):
+            if len(prompt) == 0:
+                return 0
+            batch = self.tokenizer.encode(prompt, return_tensors="pt")
+            return batch.shape[-1]
+        elif isinstance(prompt, torch.Tensor) and prompt.dim() == 1:
+            return prompt.shape[-1]
+        raise TypeError("prompt must be a string or a 1-d tensor")
 
     def wait_and_clear_gpu(self):
         """Wait for GPU memory to be released and clear the cache."""
         # torch.cuda.empty_cache()
         logger.debug("Waiting for GPU memory to be released")
         
         pynvml.nvmlInit()
```

### Comparing `ag_llama_api_s-0.0.8/ag_llama_api_s/tokenizer.py` & `ag_llama_api_s-0.0.9/ag_llama_api_s/tokenizer.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.8/ag_llama_api_s.egg-info/PKG-INFO` & `ag_llama_api_s-0.0.9/ag_llama_api_s.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ag-llama-api-s
-Version: 0.0.8
+Version: 0.0.9
 Summary: ag_llama_api_s Test Package for Somthing
 Author: AA
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ag_llama_api_s-0.0.8/setup.py` & `ag_llama_api_s-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.8/tests/test_choice.py` & `ag_llama_api_s-0.0.9/tests/test_choice.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.8/tests/test_model.py` & `ag_llama_api_s-0.0.9/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.8/tests/test_tokenizer.py` & `ag_llama_api_s-0.0.9/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.8/utils/download.py` & `ag_llama_api_s-0.0.9/utils/download.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.8/utils/render.py` & `ag_llama_api_s-0.0.9/utils/render.py`

 * *Files identical despite different names*

