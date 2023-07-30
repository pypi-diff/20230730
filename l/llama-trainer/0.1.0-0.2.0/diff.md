# Comparing `tmp/llama-trainer-0.1.0.tar.gz` & `tmp/llama-trainer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama-trainer-0.1.0.tar", last modified: Fri Jul 28 10:36:32 2023, max compression
+gzip compressed data, was "llama-trainer-0.2.0.tar", last modified: Sun Jul 30 17:23:46 2023, max compression
```

## Comparing `llama-trainer-0.1.0.tar` & `llama-trainer-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:36:32.938819 llama-trainer-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 10:36:20.000000 llama-trainer-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-28 10:36:32.938819 llama-trainer-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-28 10:36:20.000000 llama-trainer-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:36:32.934819 llama-trainer-0.1.0/llama_trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-28 10:36:20.000000 llama-trainer-0.1.0/llama_trainer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:36:32.938819 llama-trainer-0.1.0/llama_trainer/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 10:36:20.000000 llama-trainer-0.1.0/llama_trainer/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-07-28 10:36:20.000000 llama-trainer-0.1.0/llama_trainer/cli/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-28 10:36:20.000000 llama-trainer-0.1.0/llama_trainer/infer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9226 2023-07-28 10:36:20.000000 llama-trainer-0.1.0/llama_trainer/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:36:32.938819 llama-trainer-0.1.0/llama_trainer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-28 10:36:20.000000 llama-trainer-0.1.0/llama_trainer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-07-28 10:36:20.000000 llama-trainer-0.1.0/llama_trainer/utils/llama_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-28 10:36:20.000000 llama-trainer-0.1.0/llama_trainer/utils/stopping_criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-28 10:36:20.000000 llama-trainer-0.1.0/llama_trainer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:36:32.934819 llama-trainer-0.1.0/llama_trainer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-28 10:36:32.000000 llama-trainer-0.1.0/llama_trainer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-28 10:36:32.000000 llama-trainer-0.1.0/llama_trainer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:36:32.000000 llama-trainer-0.1.0/llama_trainer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-28 10:36:32.000000 llama-trainer-0.1.0/llama_trainer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-28 10:36:32.000000 llama-trainer-0.1.0/llama_trainer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-28 10:36:20.000000 llama-trainer-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 10:36:32.938819 llama-trainer-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-07-28 10:36:20.000000 llama-trainer-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:23:46.640860 llama-trainer-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-30 17:23:32.000000 llama-trainer-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-30 17:23:46.640860 llama-trainer-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-30 17:23:32.000000 llama-trainer-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:23:46.636860 llama-trainer-0.2.0/llama_trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-30 17:23:32.000000 llama-trainer-0.2.0/llama_trainer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:23:46.640860 llama-trainer-0.2.0/llama_trainer/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 17:23:32.000000 llama-trainer-0.2.0/llama_trainer/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-07-30 17:23:32.000000 llama-trainer-0.2.0/llama_trainer/cli/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-30 17:23:32.000000 llama-trainer-0.2.0/llama_trainer/infer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9305 2023-07-30 17:23:32.000000 llama-trainer-0.2.0/llama_trainer/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:23:46.640860 llama-trainer-0.2.0/llama_trainer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-30 17:23:32.000000 llama-trainer-0.2.0/llama_trainer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-07-30 17:23:32.000000 llama-trainer-0.2.0/llama_trainer/utils/llama_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-30 17:23:32.000000 llama-trainer-0.2.0/llama_trainer/utils/stopping_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-30 17:23:32.000000 llama-trainer-0.2.0/llama_trainer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:23:46.640860 llama-trainer-0.2.0/llama_trainer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-30 17:23:46.000000 llama-trainer-0.2.0/llama_trainer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-30 17:23:46.000000 llama-trainer-0.2.0/llama_trainer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 17:23:46.000000 llama-trainer-0.2.0/llama_trainer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-30 17:23:46.000000 llama-trainer-0.2.0/llama_trainer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-30 17:23:46.000000 llama-trainer-0.2.0/llama_trainer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-30 17:23:32.000000 llama-trainer-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 17:23:46.640860 llama-trainer-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-07-30 17:23:32.000000 llama-trainer-0.2.0/setup.py
```

### Comparing `llama-trainer-0.1.0/PKG-INFO` & `llama-trainer-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-trainer
-Version: 0.1.0
+Version: 0.2.0
 Summary: Llama trainer utility
 Home-page: https://github.com/Riccorl/llama-trainer
 Author: Riccardo Orlando
 Author-email: orlandorcc@gmail.com
 License: Apache
 Keywords: NLP deep learning transformer pytorch llama llms hf huggingface
 Classifier: Intended Audience :: Science/Research
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # 🦙 Llama Trainer Utility
 
-[![Upload to PyPi](https://github.com/Riccorl/llama-trainer/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Riccorl/llama-trainer/actions/workflows/python-publish.yml)
+[![Upload to PyPi](https://github.com/Riccorl/llama-trainer/actions/workflows/python-publish-pypi.yml/badge.svg)](https://github.com/Riccorl/llama-trainer/actions/workflows/python-publish-pypi.yml)
 
 A "just few lines of code" utility for fine-tuning (not only) Llama models.
 
 To install:
 
 ```bash
 pip install llama-trainer
```

### Comparing `llama-trainer-0.1.0/README.md` & `llama-trainer-0.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # 🦙 Llama Trainer Utility
 
-[![Upload to PyPi](https://github.com/Riccorl/llama-trainer/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Riccorl/llama-trainer/actions/workflows/python-publish.yml)
+[![Upload to PyPi](https://github.com/Riccorl/llama-trainer/actions/workflows/python-publish-pypi.yml/badge.svg)](https://github.com/Riccorl/llama-trainer/actions/workflows/python-publish-pypi.yml)
 
 A "just few lines of code" utility for fine-tuning (not only) Llama models.
 
 To install:
 
 ```bash
 pip install llama-trainer
```

### Comparing `llama-trainer-0.1.0/llama_trainer/cli/train.py` & `llama-trainer-0.2.0/llama_trainer/cli/train.py`

 * *Files identical despite different names*

### Comparing `llama-trainer-0.1.0/llama_trainer/infer.py` & `llama-trainer-0.2.0/llama_trainer/infer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 import torch
 from peft import AutoPeftModelForCausalLM
 from transformers import AutoTokenizer, PreTrainedModel, StoppingCriteriaList
 from llama_trainer.utils import is_package_available
 from llama_trainer.utils.stopping_criteria import SentinelTokenStoppingCriteria
 
 
@@ -33,22 +33,22 @@
         self.model = model
         self.tokenizer = AutoTokenizer.from_pretrained(model.config.name_or_path)
 
         self.device = self.model.device
 
     def __call__(
         self,
-        prompt: str,
+        prompt: Union[str, List[str]],
         do_sample: bool = True,
         max_new_tokens: int = 100,
         top_p: float = 0.9,
         temperature: float = 0.9,
         stop_token: Optional[Union[str, int]] = None,
         generation_kwargs: Dict[str, Any] = None,
-    ) -> Any:
+    ) -> List[str]:
         input_ids = self.tokenizer(
             prompt, return_tensors="pt", truncation=True
         ).input_ids
 
         # check if device of the model is cuda
         input_ids = input_ids.to(self.model.device)
 
@@ -77,11 +77,9 @@
             "top_p": top_p,
             "temperature": temperature,
             "stopping_criteria": stopping_criteria_list,
             **generation_kwargs,
         }
         outputs = self.model.generate(**generation_kwargs)
         outputs = outputs.detach().cpu().numpy()
-        decoded = self.tokenizer.batch_decode(outputs, skip_special_tokens=True)[0][
-            len(prompt) :
-        ]
+        decoded = self.tokenizer.batch_decode(outputs, skip_special_tokens=True)
         return decoded
```

### Comparing `llama-trainer-0.1.0/llama_trainer/trainer.py` & `llama-trainer-0.2.0/llama_trainer/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         bnb_4bit_compute_dtype: str = "bfloat16",
         bnb_4bit_quant_type: str = "nf4",
         num_train_epochs: int = 3,
         fp16: bool = False,
         bf16: bool = True,
         tf32: bool = True,
         use_flash_attn: bool = False,
-        packing: bool = True,
+        packing: bool = False,
         gradient_checkpointing: bool = True,
         optim: str = "paged_adamw_32bit",
         lr_scheduler_type: str = "constant",
         max_steps: int = -1,
         warmup_ratio: float = 0.03,
         group_by_length: bool = False,
         save_steps: int = 100,
@@ -100,27 +100,30 @@
         self.merge_and_push = merge_and_push
         self.device_map = device_map
 
         if output_dir is None:
             output_dir = Path("output") / f"{self.model_name}"
         self.output_dir = Path(output_dir)
 
+        self.kwargs = kwargs
+
     def train(self):
         self.training_arguments = TrainingArguments(
             output_dir=self.output_dir,
             per_device_train_batch_size=self.per_device_train_batch_size,
             gradient_accumulation_steps=self.gradient_accumulation_steps,
             optim=self.optim,
             save_steps=self.save_steps,
             logging_steps=self.logging_steps,
             learning_rate=self.learning_rate,
             fp16=self.fp16,
             bf16=self.bf16,
             tf32=self.tf32,
             max_grad_norm=self.max_grad_norm,
+            num_train_epochs=self.num_train_epochs,
             max_steps=self.max_steps,
             warmup_ratio=self.warmup_ratio,
             group_by_length=self.group_by_length,
             lr_scheduler_type=self.lr_scheduler_type,
         )
 
         self.model, self.peft_config, self.tokenizer = self.create_and_prepare_model(
@@ -149,14 +152,15 @@
             peft_config=self.peft_config,
             max_seq_length=self.max_seq_length,
             tokenizer=self.tokenizer,
             args=self.training_arguments,
             dataset_text_field=self.dataset_text_field,
             formatting_func=self.formatting_func,
             packing=self.packing,
+            **self.kwargs,
         )
 
         self.trainer.train()
 
         if self.merge_and_push:
             self.merge_and_save()
 
@@ -196,15 +200,14 @@
                 print(
                     "Your GPU supports bfloat16, you can accelerate training with the argument --bf16"
                 )
                 print("=" * 80)
 
         # Load the entire model on the GPU 0
         # switch to `device_map = "auto"` for multi-GPU
-        # device_map = {"": 0}
         device_map = device_map
 
         model = AutoModelForCausalLM.from_pretrained(
             model_name,
             quantization_config=bnb_config,
             device_map=device_map,
             use_auth_token=True,
```

### Comparing `llama-trainer-0.1.0/llama_trainer/utils/llama_patch.py` & `llama-trainer-0.2.0/llama_trainer/utils/llama_patch.py`

 * *Files identical despite different names*

### Comparing `llama-trainer-0.1.0/llama_trainer/utils/stopping_criteria.py` & `llama-trainer-0.2.0/llama_trainer/utils/stopping_criteria.py`

 * *Files identical despite different names*

### Comparing `llama-trainer-0.1.0/llama_trainer.egg-info/PKG-INFO` & `llama-trainer-0.2.0/llama_trainer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-trainer
-Version: 0.1.0
+Version: 0.2.0
 Summary: Llama trainer utility
 Home-page: https://github.com/Riccorl/llama-trainer
 Author: Riccardo Orlando
 Author-email: orlandorcc@gmail.com
 License: Apache
 Keywords: NLP deep learning transformer pytorch llama llms hf huggingface
 Classifier: Intended Audience :: Science/Research
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # 🦙 Llama Trainer Utility
 
-[![Upload to PyPi](https://github.com/Riccorl/llama-trainer/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Riccorl/llama-trainer/actions/workflows/python-publish.yml)
+[![Upload to PyPi](https://github.com/Riccorl/llama-trainer/actions/workflows/python-publish-pypi.yml/badge.svg)](https://github.com/Riccorl/llama-trainer/actions/workflows/python-publish-pypi.yml)
 
 A "just few lines of code" utility for fine-tuning (not only) Llama models.
 
 To install:
 
 ```bash
 pip install llama-trainer
```

### Comparing `llama-trainer-0.1.0/setup.py` & `llama-trainer-0.2.0/setup.py`

 * *Files identical despite different names*

