# Comparing `tmp/compel-2.0.1rc1.tar.gz` & `tmp/compel-2.0.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/damian/2.current/stablediffusion/compel/dist/.tmp-f99dy6mm/compel-2.0.1rc1.tar", last modified: Thu Jul 20 18:55:38 2023, max compression
+gzip compressed data, was "compel-2.0.2.dev1.tar", last modified: Sun Jul 30 11:59:08 2023, max compression
```

## Comparing `compel-2.0.1rc1.tar` & `compel-2.0.2.dev1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-20 18:55:38.000000 compel-2.0.1rc1/
--rw-r--r--   0 damian     (501) staff       (20)     1064 2023-03-07 13:01:09.000000 compel-2.0.1rc1/LICENSE
--rw-r--r--   0 damian     (501) staff       (20)    12250 2023-07-20 18:55:38.000000 compel-2.0.1rc1/PKG-INFO
--rw-r--r--   0 damian     (501) staff       (20)    11669 2023-07-18 14:01:58.000000 compel-2.0.1rc1/README.md
--rw-r--r--   0 damian     (501) staff       (20)      766 2023-07-20 18:55:28.000000 compel-2.0.1rc1/pyproject.toml
--rw-r--r--   0 damian     (501) staff       (20)       38 2023-07-20 18:55:38.000000 compel-2.0.1rc1/setup.cfg
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-20 18:55:38.000000 compel-2.0.1rc1/src/
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-20 18:55:38.000000 compel-2.0.1rc1/src/compel/
--rw-r--r--   0 damian     (501) staff       (20)      175 2023-06-03 06:15:19.000000 compel-2.0.1rc1/src/compel/__init__.py
--rw-r--r--   0 damian     (501) staff       (20)    20730 2023-07-20 18:51:59.000000 compel-2.0.1rc1/src/compel/compel.py
--rw-r--r--   0 damian     (501) staff       (20)     1833 2023-03-15 21:38:57.000000 compel-2.0.1rc1/src/compel/conditioning_scheduler.py
--rw-r--r--   0 damian     (501) staff       (20)     1581 2023-03-07 13:01:09.000000 compel-2.0.1rc1/src/compel/cross_attention_control.py
--rw-r--r--   0 damian     (501) staff       (20)      653 2023-06-03 06:15:19.000000 compel-2.0.1rc1/src/compel/diffusers_textual_inversion_manager.py
--rw-r--r--   0 damian     (501) staff       (20)    30822 2023-07-20 18:51:59.000000 compel-2.0.1rc1/src/compel/embeddings_provider.py
--rw-r--r--   0 damian     (501) staff       (20)    30771 2023-07-04 21:57:36.000000 compel-2.0.1rc1/src/compel/prompt_parser.py
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-20 18:55:38.000000 compel-2.0.1rc1/src/compel.egg-info/
--rw-r--r--   0 damian     (501) staff       (20)    12250 2023-07-20 18:55:38.000000 compel-2.0.1rc1/src/compel.egg-info/PKG-INFO
--rw-r--r--   0 damian     (501) staff       (20)      512 2023-07-20 18:55:38.000000 compel-2.0.1rc1/src/compel.egg-info/SOURCES.txt
--rw-r--r--   0 damian     (501) staff       (20)        1 2023-07-20 18:55:38.000000 compel-2.0.1rc1/src/compel.egg-info/dependency_links.txt
--rw-r--r--   0 damian     (501) staff       (20)       56 2023-07-20 18:55:38.000000 compel-2.0.1rc1/src/compel.egg-info/requires.txt
--rw-r--r--   0 damian     (501) staff       (20)        7 2023-07-20 18:55:38.000000 compel-2.0.1rc1/src/compel.egg-info/top_level.txt
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-20 18:55:38.000000 compel-2.0.1rc1/test/
--rw-r--r--   0 damian     (501) staff       (20)    16457 2023-07-18 10:18:45.000000 compel-2.0.1rc1/test/test_compel.py
--rw-r--r--   0 damian     (501) staff       (20)    21072 2023-06-03 06:15:11.000000 compel-2.0.1rc1/test/test_embeddings_provider.py
--rw-r--r--   0 damian     (501) staff       (20)    47562 2023-06-03 06:55:54.000000 compel-2.0.1rc1/test/test_prompt_parser.py
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-30 11:59:08.570886 compel-2.0.2.dev1/
+-rw-r--r--   0 damian     (501) staff       (20)     1064 2023-03-07 13:01:09.000000 compel-2.0.2.dev1/LICENSE
+-rw-r--r--   0 damian     (501) staff       (20)    12388 2023-07-30 11:59:08.570483 compel-2.0.2.dev1/PKG-INFO
+-rw-r--r--   0 damian     (501) staff       (20)    11805 2023-07-30 11:40:17.000000 compel-2.0.2.dev1/README.md
+-rw-r--r--   0 damian     (501) staff       (20)      765 2023-07-30 11:40:34.000000 compel-2.0.2.dev1/pyproject.toml
+-rw-r--r--   0 damian     (501) staff       (20)       38 2023-07-30 11:59:08.570981 compel-2.0.2.dev1/setup.cfg
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-30 11:59:08.557958 compel-2.0.2.dev1/src/
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-30 11:59:08.564628 compel-2.0.2.dev1/src/compel/
+-rw-r--r--   0 damian     (501) staff       (20)      175 2023-06-03 06:15:19.000000 compel-2.0.2.dev1/src/compel/__init__.py
+-rw-r--r--   0 damian     (501) staff       (20)    21417 2023-07-30 11:40:17.000000 compel-2.0.2.dev1/src/compel/compel.py
+-rw-r--r--   0 damian     (501) staff       (20)     1833 2023-03-15 21:38:57.000000 compel-2.0.2.dev1/src/compel/conditioning_scheduler.py
+-rw-r--r--   0 damian     (501) staff       (20)     1581 2023-03-07 13:01:09.000000 compel-2.0.2.dev1/src/compel/cross_attention_control.py
+-rw-r--r--   0 damian     (501) staff       (20)      653 2023-06-03 06:15:19.000000 compel-2.0.2.dev1/src/compel/diffusers_textual_inversion_manager.py
+-rw-r--r--   0 damian     (501) staff       (20)    30956 2023-07-30 11:40:17.000000 compel-2.0.2.dev1/src/compel/embeddings_provider.py
+-rw-r--r--   0 damian     (501) staff       (20)    30771 2023-07-04 21:57:36.000000 compel-2.0.2.dev1/src/compel/prompt_parser.py
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-30 11:59:08.567330 compel-2.0.2.dev1/src/compel.egg-info/
+-rw-r--r--   0 damian     (501) staff       (20)    12388 2023-07-30 11:59:08.000000 compel-2.0.2.dev1/src/compel.egg-info/PKG-INFO
+-rw-r--r--   0 damian     (501) staff       (20)      512 2023-07-30 11:59:08.000000 compel-2.0.2.dev1/src/compel.egg-info/SOURCES.txt
+-rw-r--r--   0 damian     (501) staff       (20)        1 2023-07-30 11:59:08.000000 compel-2.0.2.dev1/src/compel.egg-info/dependency_links.txt
+-rw-r--r--   0 damian     (501) staff       (20)       56 2023-07-30 11:59:08.000000 compel-2.0.2.dev1/src/compel.egg-info/requires.txt
+-rw-r--r--   0 damian     (501) staff       (20)        7 2023-07-30 11:59:08.000000 compel-2.0.2.dev1/src/compel.egg-info/top_level.txt
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-30 11:59:08.569345 compel-2.0.2.dev1/test/
+-rw-r--r--   0 damian     (501) staff       (20)    16457 2023-07-18 10:18:45.000000 compel-2.0.2.dev1/test/test_compel.py
+-rw-r--r--   0 damian     (501) staff       (20)    21072 2023-06-03 06:15:11.000000 compel-2.0.2.dev1/test/test_embeddings_provider.py
+-rw-r--r--   0 damian     (501) staff       (20)    47562 2023-06-03 06:55:54.000000 compel-2.0.2.dev1/test/test_prompt_parser.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `compel-2.0.1rc1/LICENSE` & `compel-2.0.2.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `compel-2.0.1rc1/PKG-INFO` & `compel-2.0.2.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compel
-Version: 2.0.1rc1
+Version: 2.0.2.dev1
 Summary: A prompting enhancement library for transformers-type text embedding systems.
 Author-email: Damian Stewart <null@damianstewart.com>
 Project-URL: Homepage, https://github.com/damian0815/compel
 Project-URL: Bug Tracker, https://github.com/damian0815/compel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -95,14 +95,16 @@
 If this doesn't help, you could try this advice offered by @kshieh1: 
 > After image generation, you should explictly de-reference the tensor object (i.e., prompt_embeds = None) and call gc.collect()
 
 See https://github.com/damian0815/compel/issues/24 for more details. Thanks @kshieh1 !
 
 ## Changelog
 
+#### 2.0.1 - fix for [#45](https://github.com/damian0815/compel/issues/45) padding issue with SDXL non-truncated prompts and `.and()` 
+
 ### 2.0.0 - SDXL Support
 
 With big thanks to Patrick von Platen from Hugging Face for [the pull request](https://github.com/damian0815/compel/pull/41), Compel now supports SDXL. Use it like this: 
 
 ```
 from compel import Compel, ReturnedEmbeddingsType
 from diffusers import DiffusionPipeline
```

### Comparing `compel-2.0.1rc1/README.md` & `compel-2.0.2.dev1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,16 @@
 If this doesn't help, you could try this advice offered by @kshieh1: 
 > After image generation, you should explictly de-reference the tensor object (i.e., prompt_embeds = None) and call gc.collect()
 
 See https://github.com/damian0815/compel/issues/24 for more details. Thanks @kshieh1 !
 
 ## Changelog
 
+#### 2.0.1 - fix for [#45](https://github.com/damian0815/compel/issues/45) padding issue with SDXL non-truncated prompts and `.and()` 
+
 ### 2.0.0 - SDXL Support
 
 With big thanks to Patrick von Platen from Hugging Face for [the pull request](https://github.com/damian0815/compel/pull/41), Compel now supports SDXL. Use it like this: 
 
 ```
 from compel import Compel, ReturnedEmbeddingsType
 from diffusers import DiffusionPipeline
```

### Comparing `compel-2.0.1rc1/pyproject.toml` & `compel-2.0.2.dev1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "compel"
-version = "2.0.1-pre1"
+version = "2.0.2dev1"
 authors = [
   { name="Damian Stewart", email="null@damianstewart.com" },
 ]
 description = "A prompting enhancement library for transformers-type text embedding systems."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `compel-2.0.1rc1/src/compel/compel.py` & `compel-2.0.2.dev1/src/compel/compel.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         Build a conditioning tensor by parsing the text for Compel syntax, constructing a Conjunction, and then
         building a conditioning tensor from that Conjunction.
         """
         conjunction = self.parse_prompt_string(text)
         conditioning, _ = self.build_conditioning_tensor_for_conjunction(conjunction)
 
         if self.requires_pooled:
-            pooled = self.conditioning_provider.get_pooled_embeddings([text] )
+            pooled = self.conditioning_provider.get_pooled_embeddings([text], device=self.device)
             return conditioning, pooled
         else:
             return conditioning
 
     @torch.no_grad()
     def __call__(self, text: Union[str, List[str]]) -> torch.FloatTensor:
         """
@@ -186,15 +186,23 @@
             weight = conjunction.weights[i]
             if weight != 1:
                 # apply weight if we need to
                 empty_conditioning = self.build_conditioning_tensor('') if empty_conditioning is None else empty_conditioning
                 [padded_empty_conditioning, _] = self.pad_conditioning_tensors_to_same_length([empty_conditioning, this_conditioning])
                 this_conditioning = padded_empty_conditioning + (this_conditioning - padded_empty_conditioning) * weight
             to_concat.append(this_conditioning)
-        return torch.concat(to_concat, dim=1), options
+        assert all(c.shape == to_concat[0].shape for c in to_concat)
+        if len(to_concat[0].shape) == 2:
+            token_dim = 0
+        elif len(to_concat[0].shape) == 3:
+            print("huh. weird. please file a bug on the Compel github repo stating that \"build_conditioning_tensor_for_conjunction shape has length 3\". include your prompts and the code you use to invoke Compel.")
+            token_dim = 1
+        else:
+            assert False, f"unhandled conditioning shape length: {to_concat[0].shape}"
+        return torch.concat(to_concat, dim=token_dim), options
 
 
     def build_conditioning_tensor_for_prompt_object(self, prompt: Union[Blend, FlattenedPrompt],
                                                     ) -> Tuple[torch.Tensor, dict]:
         """
         Build a conditioning tensor for the given prompt object (either a Blend or a FlattenedPrompt).
         """
@@ -221,15 +229,17 @@
             conditionings = [c.unsqueeze(0) for c in conditionings]
             c0_shape = conditionings[0].shape
         if len(c0_shape) != 3:
             raise ValueError(f"All conditioning tensors must have the same number of dimensions (2 or 3)")
 
         if not all([c.shape[0] == c0_shape[0] and c.shape[2] == c0_shape[2] for c in conditionings]):
             raise ValueError(f"All conditioning tensors must have the same batch size ({c0_shape[0]}) and number of embeddings per token ({c0_shape[1]}")
-
+        
+        if len(emptystring_conditioning.shape) == 2:
+            emptystring_conditioning = emptystring_conditioning.unsqueeze(0)
         empty_z = torch.cat([emptystring_conditioning] * c0_shape[0])
         max_token_count = max([c.shape[1] for c in conditionings])
         # if necessary, pad shorter tensors out with an emptystring tensor
         for i, c in enumerate(conditionings):
             while c.shape[1] < max_token_count:
                 c = torch.cat([c, empty_z], dim=1)
                 conditionings[i] = c
```

### Comparing `compel-2.0.1rc1/src/compel/conditioning_scheduler.py` & `compel-2.0.2.dev1/src/compel/conditioning_scheduler.py`

 * *Files identical despite different names*

### Comparing `compel-2.0.1rc1/src/compel/cross_attention_control.py` & `compel-2.0.2.dev1/src/compel/cross_attention_control.py`

 * *Files identical despite different names*

### Comparing `compel-2.0.1rc1/src/compel/diffusers_textual_inversion_manager.py` & `compel-2.0.2.dev1/src/compel/diffusers_textual_inversion_manager.py`

 * *Files identical despite different names*

### Comparing `compel-2.0.1rc1/src/compel/embeddings_provider.py` & `compel-2.0.2.dev1/src/compel/embeddings_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,17 +227,20 @@
             if include_start_and_end_markers:
                 token_ids = [self.tokenizer.bos_token_id] + token_ids + [self.tokenizer.eos_token_id]
 
             result.append(token_ids)
 
         return result
 
-    def get_pooled_embeddings(self, texts: List[str], attention_mask: Optional[torch.Tensor]=None) -> Optional[torch.Tensor]:
+    def get_pooled_embeddings(self, texts: List[str], attention_mask: Optional[torch.Tensor]=None, device: Optional[str]=None) -> Optional[torch.Tensor]:
+        
+        device = device or self.text_encoder.device
+
         token_ids = self.get_token_ids(texts, padding="max_length", truncation_override=True)
-        token_ids = torch.tensor(token_ids, dtype=torch.long).to(self.text_encoder.device)
+        token_ids = torch.tensor(token_ids, dtype=torch.long).to(device)
 
         text_encoder_output = self.text_encoder(token_ids, attention_mask, return_dict=True)
         pooled = text_encoder_output.text_embeds
 
         return pooled
 
 
@@ -493,16 +496,19 @@
         return self.embedding_providers[0].tokenizer
 
     def get_token_ids(self, *args, **kwargs):
         # get token ids does not use padding. The padding ID is the only ID that can differ between tokenizers
         # so for simplicity, we just return `get_token_ids` of the first tokenizer
         return self.embedding_providers[0].get_token_ids(self, *args, **kwargs)
 
-    def get_pooled_embeddings(self, texts: List[str], attention_mask: Optional[torch.Tensor]=None) -> Optional[torch.Tensor]:
-        pooled = [self.embedding_providers[provider_index].get_pooled_embeddings(texts, attention_mask)
+    def get_pooled_embeddings(
+        self, texts: List[str], attention_mask: Optional[torch.Tensor] = None, device: Optional[str] = None
+    ) -> Optional[torch.Tensor]:
+
+        pooled = [self.embedding_providers[provider_index].get_pooled_embeddings(texts, attention_mask, device=device)
                   for provider_index, requires_pooled in enumerate(self.requires_pooled_mask) if requires_pooled]
 
         if len(pooled) == 0:
             return None
 
         return torch.cat(pooled, dim=-1)
```

### Comparing `compel-2.0.1rc1/src/compel/prompt_parser.py` & `compel-2.0.2.dev1/src/compel/prompt_parser.py`

 * *Files identical despite different names*

### Comparing `compel-2.0.1rc1/src/compel.egg-info/PKG-INFO` & `compel-2.0.2.dev1/src/compel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compel
-Version: 2.0.1rc1
+Version: 2.0.2.dev1
 Summary: A prompting enhancement library for transformers-type text embedding systems.
 Author-email: Damian Stewart <null@damianstewart.com>
 Project-URL: Homepage, https://github.com/damian0815/compel
 Project-URL: Bug Tracker, https://github.com/damian0815/compel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -95,14 +95,16 @@
 If this doesn't help, you could try this advice offered by @kshieh1: 
 > After image generation, you should explictly de-reference the tensor object (i.e., prompt_embeds = None) and call gc.collect()
 
 See https://github.com/damian0815/compel/issues/24 for more details. Thanks @kshieh1 !
 
 ## Changelog
 
+#### 2.0.1 - fix for [#45](https://github.com/damian0815/compel/issues/45) padding issue with SDXL non-truncated prompts and `.and()` 
+
 ### 2.0.0 - SDXL Support
 
 With big thanks to Patrick von Platen from Hugging Face for [the pull request](https://github.com/damian0815/compel/pull/41), Compel now supports SDXL. Use it like this: 
 
 ```
 from compel import Compel, ReturnedEmbeddingsType
 from diffusers import DiffusionPipeline
```

### Comparing `compel-2.0.1rc1/src/compel.egg-info/SOURCES.txt` & `compel-2.0.2.dev1/src/compel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `compel-2.0.1rc1/test/test_compel.py` & `compel-2.0.2.dev1/test/test_compel.py`

 * *Files identical despite different names*

### Comparing `compel-2.0.1rc1/test/test_embeddings_provider.py` & `compel-2.0.2.dev1/test/test_embeddings_provider.py`

 * *Files identical despite different names*

### Comparing `compel-2.0.1rc1/test/test_prompt_parser.py` & `compel-2.0.2.dev1/test/test_prompt_parser.py`

 * *Files identical despite different names*

