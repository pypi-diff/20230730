# Comparing `tmp/atro_args-0.2.3.tar.gz` & `tmp/atro_args-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atro_args-0.2.3.tar", max compression
+gzip compressed data, was "atro_args-0.2.4.tar", max compression
```

## Comparing `atro_args-0.2.3.tar` & `atro_args-0.2.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      963 2023-07-28 19:02:59.510131 atro_args-0.2.3/README.md
--rw-r--r--   0        0        0       89 2023-07-28 15:55:58.438531 atro_args-0.2.3/atro_args/__init__.py
--rw-r--r--   0        0        0     1699 2023-07-28 19:48:36.731517 atro_args-0.2.3/atro_args/arg.py
--rw-r--r--   0        0        0      333 2023-07-28 15:55:58.438531 atro_args-0.2.3/atro_args/arg_source.py
--rw-r--r--   0        0        0     1327 2023-07-28 19:46:54.751810 atro_args-0.2.3/atro_args/helpers.py
--rw-r--r--   0        0        0     8472 2023-07-28 19:56:18.655100 atro_args-0.2.3/atro_args/input_args.py
--rw-r--r--   0        0        0      411 2023-07-28 19:56:26.498381 atro_args-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1363 1970-01-01 00:00:00.000000 atro_args-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      963 2023-07-28 19:02:59.510131 atro_args-0.2.4/README.md
+-rw-r--r--   0        0        0       89 2023-07-28 15:55:58.438531 atro_args-0.2.4/atro_args/__init__.py
+-rw-r--r--   0        0        0     1699 2023-07-28 19:48:36.731517 atro_args-0.2.4/atro_args/arg.py
+-rw-r--r--   0        0        0      333 2023-07-28 15:55:58.438531 atro_args-0.2.4/atro_args/arg_source.py
+-rw-r--r--   0        0        0     1328 2023-07-28 19:57:23.861331 atro_args-0.2.4/atro_args/helpers.py
+-rw-r--r--   0        0        0     8364 2023-07-30 13:49:26.590872 atro_args-0.2.4/atro_args/input_args.py
+-rw-r--r--   0        0        0      407 2023-07-30 13:49:59.710588 atro_args-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1363 1970-01-01 00:00:00.000000 atro_args-0.2.4/PKG-INFO
```

### Comparing `atro_args-0.2.3/README.md` & `atro_args-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `atro_args-0.2.3/atro_args/arg.py` & `atro_args-0.2.4/atro_args/arg.py`

 * *Files identical despite different names*

### Comparing `atro_args-0.2.3/atro_args/helpers.py` & `atro_args-0.2.4/atro_args/helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import ast
 import json
 import logging
-from typing import Mapping, Sequence
+from collections.abc import Mapping, Sequence
 
 
 def load_to_py_type(s, arg_type):
     # If type is correct return as is
     if type(s) == arg_type:
         logging.debug(f"{s} is already of type {arg_type} no need to parse.")
         return s
 
-
     if arg_type in [Mapping, Sequence, list, dict]:
         if not isinstance(s, str):
             raise ValueError(f"Could not load {s} as {arg_type} because it is not clear how to load type {type(s)} into {arg_type}.")
-        
+
         try:
             logging.debug(f"Trying to load {s} as json.")
             json_loaded = json.loads(s)
             if isinstance(json_loaded, arg_type):
                 logging.debug(f"Loaded {s} as json, checking if type is {arg_type} if so returning.")
                 return json_loaded
         except json.JSONDecodeError:
@@ -27,8 +26,8 @@
                 ast_loaded = ast.literal_eval(s)
                 if isinstance(ast_loaded, arg_type):
                     logging.debug(f"Loaded {s} using ast, checking if type is {arg_type} if so returning.")
                     return ast_loaded
             except (ValueError, SyntaxError):
                 raise ValueError(f"Could not load {s} as {arg_type}.")
 
-    return arg_type(s)
+    return arg_type(s)
```

### Comparing `atro_args-0.2.3/atro_args/input_args.py` & `atro_args-0.2.4/atro_args/input_args.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from argparse import ArgumentParser
-from collections.abc import Sequence
+from collections.abc import Mapping, Sequence
 from os import environ
 from pathlib import Path
-from typing import Any, Mapping
+from typing import Any
 
 import yaml
 from annotated_types import UpperCase
 from dotenv import load_dotenv
 from pydantic import BaseModel, field_validator
 
 from atro_args.arg import Arg
@@ -19,15 +19,15 @@
     """InputArgs is a model that represents the input arguments of an application. After it is initialized the parse_args method can be called to parse the arguments and return them as a dictionary.
 
     Attributes:
         prefix (UpperCase): The prefix to use for environment variables. Defaults to "ATRO_ARGS". This means that the environment variable for the argument "name" will be "ATRO_ARGS_NAME" and the environment variable for the argument "other_names" will be "ATRO_ARGS_OTHER_NAMES".
         args (list[Arg], optional): A list of arguments to parse. Defaults to [].
         env_files (list[Path], optional): A list of paths to environment files. Defaults to [Path(".env")] which is the .env file in the directory where the application is ran from.
         yaml_files (list[Path], optional): A list of paths to yaml files. Defaults to [].
-        arg_priority: (list[ArgSource], optional): A list of ArgSource enums that represent the priority of the arguments. Defaults to [ArgSource.cli_args, ArgSource.yaml_files, ArgSource.envs, ArgSource.env_files]. This means that if an argument is passed via CLI it will take priority over the same argument passed via a yaml file, which will take priority over the same argument passed via ENV, which will take priority over the same argument passed via an ENV file.
+        arg_priority: (list[ArgSource], optional): A list of ArgSource enums that represent the priority of the arguments. This means that if an argument is passed via CLI it will take priority over the same argument passed via a yaml file and so on.
     """
 
     prefix: UpperCase = "ATRO_ARGS"
     args: list[Arg] = []
     env_files: list[Path] = [Path(".env")]
     yaml_files: list[Path] = []
     arg_priority: list[ArgSource] = [ArgSource.cli_args, ArgSource.yaml_files, ArgSource.envs, ArgSource.env_files]
@@ -42,23 +42,26 @@
         self.args.append(arg)
 
     def get_cli_args(self, cli_input_args: Sequence[str] | None) -> dict[str, str]:
         parser = ArgumentParser()
         for arg in self.args:
             if arg.accept_via_cli:
                 # Making some adjustments
-                other_names = [f"-" + name for name in arg.other_names]
+                other_names = ["-" + name for name in arg.other_names]
                 arg_type = arg.arg_type
                 if arg_type in [Sequence, Mapping, list, dict]:
                     # loading a json as dict or list will fail in argparse, as it will load each element char by char, bypassing that issue by loading it as a string and then converting it to the desired type
                     arg_type = str
-                
-                parser.add_argument(f"--{arg.name}", *other_names, type=arg_type, help=arg.help, required=False)
 
-        return vars(parser.parse_args(cli_input_args or []))
+                parser.add_argument(f"--{arg.name}", *other_names, type=arg_type, help=arg.help, required=False)
+                
+        if cli_input_args is None or len(cli_input_args) == 0:
+            return vars(parser.parse_args())
+        else:
+            return vars(parser.parse_args(cli_input_args))
 
     def get_env_args(self) -> dict[str, str]:
         envs: dict[str, str] = {}
         for arg in self.args:
             env = environ.get(f"{self.prefix}_{arg.name}".upper())
             if env is not None:
                 envs[arg.name] = env
@@ -175,15 +178,15 @@
 
         Args:
             cli_input_args (Sequence[str]): A list of strings representing the CLI arguments. Defaults to None which means the arguments will be read from sys.argv.
 
         Returns:
             A dictionary with keys being the argument names and values being the argument values. Argument values will be of the type specified in the Arg model.
         """
-        
+
         model: dict[str, Any] = {arg.name: arg.default for arg in self.args}
 
         cli_args = self.get_cli_args(cli_input_args)
         env_args = self.get_env_args()
         env_file_args = self.get_env_file_args()
         yaml_file_args = self.get_yaml_file_args()
```

### Comparing `atro_args-0.2.3/PKG-INFO` & `atro_args-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atro-args
-Version: 0.2.3
+Version: 0.2.4
 Summary: 
 Author: atropos
 Author-email: sv7n@pm.me
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

