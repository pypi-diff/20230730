# Comparing `tmp/atro_args-0.2.4.tar.gz` & `tmp/atro_args-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atro_args-0.2.4.tar", max compression
+gzip compressed data, was "atro_args-0.2.5.tar", max compression
```

## Comparing `atro_args-0.2.4.tar` & `atro_args-0.2.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      963 2023-07-28 19:02:59.510131 atro_args-0.2.4/README.md
--rw-r--r--   0        0        0       89 2023-07-28 15:55:58.438531 atro_args-0.2.4/atro_args/__init__.py
--rw-r--r--   0        0        0     1699 2023-07-28 19:48:36.731517 atro_args-0.2.4/atro_args/arg.py
--rw-r--r--   0        0        0      333 2023-07-28 15:55:58.438531 atro_args-0.2.4/atro_args/arg_source.py
--rw-r--r--   0        0        0     1328 2023-07-28 19:57:23.861331 atro_args-0.2.4/atro_args/helpers.py
--rw-r--r--   0        0        0     8364 2023-07-30 13:49:26.590872 atro_args-0.2.4/atro_args/input_args.py
--rw-r--r--   0        0        0      407 2023-07-30 13:49:59.710588 atro_args-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1363 1970-01-01 00:00:00.000000 atro_args-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      963 2023-07-28 19:02:59.510131 atro_args-0.2.5/README.md
+-rw-r--r--   0        0        0       89 2023-07-28 15:55:58.438531 atro_args-0.2.5/atro_args/__init__.py
+-rw-r--r--   0        0        0     1699 2023-07-28 19:48:36.731517 atro_args-0.2.5/atro_args/arg.py
+-rw-r--r--   0        0        0      333 2023-07-28 15:55:58.438531 atro_args-0.2.5/atro_args/arg_source.py
+-rw-r--r--   0        0        0     1328 2023-07-28 19:57:23.861331 atro_args-0.2.5/atro_args/helpers.py
+-rw-r--r--   0        0        0     8737 2023-07-30 14:37:53.380669 atro_args-0.2.5/atro_args/input_args.py
+-rw-r--r--   0        0        0      407 2023-07-30 14:38:17.873946 atro_args-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1363 1970-01-01 00:00:00.000000 atro_args-0.2.5/PKG-INFO
```

### Comparing `atro_args-0.2.4/README.md` & `atro_args-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `atro_args-0.2.4/atro_args/arg.py` & `atro_args-0.2.5/atro_args/arg.py`

 * *Files identical despite different names*

### Comparing `atro_args-0.2.4/atro_args/helpers.py` & `atro_args-0.2.5/atro_args/helpers.py`

 * *Files identical despite different names*

### Comparing `atro_args-0.2.4/atro_args/input_args.py` & `atro_args-0.2.5/atro_args/input_args.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from argparse import ArgumentParser
 from collections.abc import Mapping, Sequence
 from os import environ
 from pathlib import Path
 from typing import Any
-
+import sys
 import yaml
 from annotated_types import UpperCase
 from dotenv import load_dotenv
 from pydantic import BaseModel, field_validator
 
 from atro_args.arg import Arg
 from atro_args.arg_source import ArgSource
@@ -37,31 +37,36 @@
         if len(set(v)) != len(v):
             raise ValueError("arg_priority must be unique")
         return v
 
     def add_arg(self, arg: Arg):
         self.args.append(arg)
 
-    def get_cli_args(self, cli_input_args: Sequence[str] | None) -> dict[str, str]:
+    def get_cli_args(self, cli_input_args: Sequence[str] | None = None) -> dict[str, str]:
         parser = ArgumentParser()
         for arg in self.args:
             if arg.accept_via_cli:
                 # Making some adjustments
                 other_names = ["-" + name for name in arg.other_names]
                 arg_type = arg.arg_type
                 if arg_type in [Sequence, Mapping, list, dict]:
                     # loading a json as dict or list will fail in argparse, as it will load each element char by char, bypassing that issue by loading it as a string and then converting it to the desired type
                     arg_type = str
 
-                parser.add_argument(f"--{arg.name}", *other_names, type=arg_type, help=arg.help, required=False)
-                
-        if cli_input_args is None or len(cli_input_args) == 0:
-            return vars(parser.parse_args())
-        else:
-            return vars(parser.parse_args(cli_input_args))
+                parser.add_argument(f"--{arg.name}"
+                                    , *other_names, type=arg_type, help=arg.help, required=False)
+        # Using parse_known_args instead of parse_args as parse_args throws on empty input.
+        output = vars(parser.parse_known_args(cli_input_args)[0]) or {}
+
+        for name in [arg.name for arg in self.args]:
+            # Edge case where argument has "-" in the name argparse would return this as _ instead.
+            if "-" in name and name.replace("-", "_") in output.keys() and name not in output.keys():
+                output[name] = output.pop(name.replace("-", "_"))
+        
+        return output
 
     def get_env_args(self) -> dict[str, str]:
         envs: dict[str, str] = {}
         for arg in self.args:
             env = environ.get(f"{self.prefix}_{arg.name}".upper())
             if env is not None:
                 envs[arg.name] = env
```

### Comparing `atro_args-0.2.4/PKG-INFO` & `atro_args-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atro-args
-Version: 0.2.4
+Version: 0.2.5
 Summary: 
 Author: atropos
 Author-email: sv7n@pm.me
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

