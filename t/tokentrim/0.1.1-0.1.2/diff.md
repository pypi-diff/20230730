# Comparing `tmp/tokentrim-0.1.1.tar.gz` & `tmp/tokentrim-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokentrim-0.1.1.tar", max compression
+gzip compressed data, was "tokentrim-0.1.2.tar", max compression
```

## Comparing `tokentrim-0.1.1.tar` & `tokentrim-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1064 2023-07-29 23:24:50.484214 tokentrim-0.1.1/LICENSE
--rw-r--r--   0        0        0      355 2023-07-30 00:07:03.345546 tokentrim-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       27 2023-07-30 00:06:48.037573 tokentrim-0.1.1/tokentrim/__init__.py
--rw-r--r--   0        0        0     5428 2023-07-29 23:50:44.552404 tokentrim-0.1.1/tokentrim/tokentrim.py
--rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 tokentrim-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-29 23:24:50.484214 tokentrim-0.1.2/LICENSE
+-rw-r--r--   0        0        0      355 2023-07-30 00:38:04.714219 tokentrim-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-07-30 00:06:48.037573 tokentrim-0.1.2/tokentrim/__init__.py
+-rw-r--r--   0        0        0     5490 2023-07-30 00:37:12.542314 tokentrim-0.1.2/tokentrim/tokentrim.py
+-rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 tokentrim-0.1.2/PKG-INFO
```

### Comparing `tokentrim-0.1.1/LICENSE` & `tokentrim-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tokentrim-0.1.1/tokentrim/tokentrim.py` & `tokentrim-0.1.2/tokentrim/tokentrim.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import tiktoken
-from typing import List, Dict, Any, Tuple, Optional
+from typing import List, Dict, Any, Tuple, Optional, Union
 
 MODEL_MAX_TOKENS = {
   'gpt-4': 8192,
   'gpt-4-0613': 8192,
   'gpt-4-32k': 32768,
   'gpt-4-32k-0613': 32768,
   'gpt-3.5-turbo': 4096,
@@ -64,29 +64,32 @@
 def shorten_message_to_fit_limit(message: Dict[str, Any], tokens_needed: int,
                                  model: str) -> None:
   """
   Shorten a message to fit within a token limit by removing characters from the middle.
   """
 
   content = message["content"]
-  left_half = content[:len(content) // 2]
-  right_half = content[len(content) // 2:]
 
   while True:
+    total_tokens = num_tokens_from_messages([message], model)
+
+    if total_tokens <= tokens_needed:
+      break
+
+    ratio = tokens_needed / total_tokens
+
+    new_length = int(len(content) * ratio)
+
+    half_length = new_length // 2
+    left_half = content[:half_length]
+    right_half = content[-half_length:]
+
     trimmed_content = left_half + '...' + right_half
     message["content"] = trimmed_content
-    if num_tokens_from_messages([message], model) > tokens_needed:
-      if len(left_half) > len(right_half):
-        # Cut from the left half if it's longer or equal
-        left_half = left_half[:-1]
-      else:
-        # Otherwise cut from the right half
-        right_half = right_half[1:]
-    else:
-      break
+    content = trimmed_content
 
 
 def trim(
   messages: List[Dict[str, Any]],
   model: str,
   system_message: Optional[str] = None,
   trim_ratio: float = 0.75,
@@ -102,14 +105,18 @@
         trim_ratio: Target ratio of tokens to use after trimming. Default is 0.75, meaning it will trim messages so they use about 75% of the model's token limit.
         return_response_tokens: If True, also return the number of tokens left available for the response after trimming.
 
     Returns:
         Trimmed messages and optionally the number of tokens available for response.
     """
 
+  # Check if model is valid
+  if model not in MODEL_MAX_TOKENS:
+    raise ValueError(f"Invalid model: {model}")
+
   # Initialize max_tokens
   max_tokens = int(MODEL_MAX_TOKENS[model] * trim_ratio)
 
   # Deduct the system message tokens from the max_tokens if system message exists
   if system_message:
     system_message_event = {"role": "system", "content": system_message}
     system_message_tokens = num_tokens_from_messages([system_message_event],
```

### Comparing `tokentrim-0.1.1/PKG-INFO` & `tokentrim-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokentrim
-Version: 0.1.1
+Version: 0.1.2
 Summary: Easily trim 'messages' arrays for use with GPTs.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

