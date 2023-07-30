# Comparing `tmp/cmdcomp-2.0.0.tar.gz` & `tmp/cmdcomp-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdcomp-2.0.0.tar", max compression
+gzip compressed data, was "cmdcomp-2.0.1.tar", max compression
```

## Comparing `cmdcomp-2.0.0.tar` & `cmdcomp-2.0.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1517 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/README.md
--rw-r--r--   0        0        0       79 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/cmdcomp/__init__.py
--rw-r--r--   0        0        0     2358 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/cmdcomp/app.py
--rw-r--r--   0        0        0      573 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/cmdcomp/completion.py
--rw-r--r--   0        0        0      757 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/cmdcomp/config.py
--rw-r--r--   0        0        0      206 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/cmdcomp/exception.py
--rw-r--r--   0        0        0      115 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/cmdcomp/main.py
--rw-r--r--   0        0        0      115 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/cmdcomp/model.py
--rw-r--r--   0        0        0      131 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/cmdcomp/shell.py
--rw-r--r--   0        0        0        0 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/cmdcomp/v1/__init__.py
--rw-r--r--   0        0        0      535 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/cmdcomp/v1/app_info.py
--rw-r--r--   0        0        0      261 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/cmdcomp/v1/cmdcomp_info.py
--rw-r--r--   0        0        0     3358 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/cmdcomp/v1/command/__init__.py
--rw-r--r--   0        0        0      338 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/cmdcomp/v1/command/option/__init__.py
--rw-r--r--   0        0        0      331 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/cmdcomp/v1/command/option/command_option.py
--rw-r--r--   0        0        0      373 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/cmdcomp/v1/command/option/file_option.py
--rw-r--r--   0        0        0     2087 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/cmdcomp/v1/completion.py
--rw-r--r--   0        0        0      377 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/cmdcomp/v1/config.py
--rw-r--r--   0        0        0     1732 2023-07-30 16:14:40.097257 cmdcomp-2.0.0/cmdcomp/v1/templates/bash.sh.jinja
--rw-r--r--   0        0        0     1277 2023-07-30 16:14:40.097257 cmdcomp-2.0.0/cmdcomp/v1/templates/zsh.sh.jinja
--rw-r--r--   0        0        0        0 2023-07-30 16:14:40.097257 cmdcomp-2.0.0/cmdcomp/v2/__init__.py
--rw-r--r--   0        0        0      535 2023-07-30 16:14:40.097257 cmdcomp-2.0.0/cmdcomp/v2/app_info.py
--rw-r--r--   0        0        0      261 2023-07-30 16:14:40.097257 cmdcomp-2.0.0/cmdcomp/v2/cmdcomp_info.py
--rw-r--r--   0        0        0     6820 2023-07-30 16:14:40.097257 cmdcomp-2.0.0/cmdcomp/v2/command/__init__.py
--rw-r--r--   0        0        0      371 2023-07-30 16:14:40.097257 cmdcomp-2.0.0/cmdcomp/v2/command/argument/__init__.py
--rw-r--r--   0        0        0      789 2023-07-30 16:14:40.097257 cmdcomp-2.0.0/cmdcomp/v2/command/argument/command_argument.py
--rw-r--r--   0        0        0      744 2023-07-30 16:14:40.097257 cmdcomp-2.0.0/cmdcomp/v2/command/argument/file_argument.py
--rw-r--r--   0        0        0      601 2023-07-30 16:14:40.097257 cmdcomp-2.0.0/cmdcomp/v2/command/argument/flag_argument.py
--rw-r--r--   0        0        0     1668 2023-07-30 16:14:40.097257 cmdcomp-2.0.0/cmdcomp/v2/command/argument/values_argument.py
--rw-r--r--   0        0        0      747 2023-07-30 16:14:40.097257 cmdcomp-2.0.0/cmdcomp/v2/completion.py
--rw-r--r--   0        0        0      380 2023-07-30 16:14:40.097257 cmdcomp-2.0.0/cmdcomp/v2/config.py
--rw-r--r--   0        0        0     4215 2023-07-30 16:14:40.097257 cmdcomp-2.0.0/cmdcomp/v2/templates/bash.sh.jinja
--rw-r--r--   0        0        0     2575 2023-07-30 16:14:40.097257 cmdcomp-2.0.0/cmdcomp/v2/templates/zsh.sh.jinja
--rw-r--r--   0        0        0     1779 2023-07-30 16:14:40.097257 cmdcomp-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     2504 1970-01-01 00:00:00.000000 cmdcomp-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2425 2023-07-30 16:51:34.110601 cmdcomp-2.0.1/README.md
+-rw-r--r--   0        0        0       79 2023-07-30 16:51:34.110601 cmdcomp-2.0.1/cmdcomp/__init__.py
+-rw-r--r--   0        0        0     2358 2023-07-30 16:51:34.110601 cmdcomp-2.0.1/cmdcomp/app.py
+-rw-r--r--   0        0        0      573 2023-07-30 16:51:34.110601 cmdcomp-2.0.1/cmdcomp/completion.py
+-rw-r--r--   0        0        0      734 2023-07-30 16:51:34.110601 cmdcomp-2.0.1/cmdcomp/config.py
+-rw-r--r--   0        0        0      444 2023-07-30 16:51:34.110601 cmdcomp-2.0.1/cmdcomp/exception.py
+-rw-r--r--   0        0        0      115 2023-07-30 16:51:34.110601 cmdcomp-2.0.1/cmdcomp/main.py
+-rw-r--r--   0        0        0      115 2023-07-30 16:51:34.110601 cmdcomp-2.0.1/cmdcomp/model.py
+-rw-r--r--   0        0        0      131 2023-07-30 16:51:34.110601 cmdcomp-2.0.1/cmdcomp/shell.py
+-rw-r--r--   0        0        0        0 2023-07-30 16:51:34.110601 cmdcomp-2.0.1/cmdcomp/v1/__init__.py
+-rw-r--r--   0        0        0      535 2023-07-30 16:51:34.110601 cmdcomp-2.0.1/cmdcomp/v1/app_info.py
+-rw-r--r--   0        0        0      261 2023-07-30 16:51:34.110601 cmdcomp-2.0.1/cmdcomp/v1/cmdcomp_info.py
+-rw-r--r--   0        0        0     3358 2023-07-30 16:51:34.110601 cmdcomp-2.0.1/cmdcomp/v1/command/__init__.py
+-rw-r--r--   0        0        0      338 2023-07-30 16:51:34.110601 cmdcomp-2.0.1/cmdcomp/v1/command/option/__init__.py
+-rw-r--r--   0        0        0      331 2023-07-30 16:51:34.110601 cmdcomp-2.0.1/cmdcomp/v1/command/option/command_option.py
+-rw-r--r--   0        0        0      373 2023-07-30 16:51:34.110601 cmdcomp-2.0.1/cmdcomp/v1/command/option/file_option.py
+-rw-r--r--   0        0        0     2103 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/cmdcomp/v1/completion.py
+-rw-r--r--   0        0        0      377 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/cmdcomp/v1/config.py
+-rw-r--r--   0        0        0     1732 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/cmdcomp/v1/templates/bash.sh.jinja
+-rw-r--r--   0        0        0     1277 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/cmdcomp/v1/templates/zsh.sh.jinja
+-rw-r--r--   0        0        0        0 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/cmdcomp/v2/__init__.py
+-rw-r--r--   0        0        0      535 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/cmdcomp/v2/app_info.py
+-rw-r--r--   0        0        0      261 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/cmdcomp/v2/cmdcomp_info.py
+-rw-r--r--   0        0        0     6844 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/cmdcomp/v2/command/__init__.py
+-rw-r--r--   0        0        0      371 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/cmdcomp/v2/command/argument/__init__.py
+-rw-r--r--   0        0        0      789 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/cmdcomp/v2/command/argument/command_argument.py
+-rw-r--r--   0        0        0      744 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/cmdcomp/v2/command/argument/file_argument.py
+-rw-r--r--   0        0        0      601 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/cmdcomp/v2/command/argument/flag_argument.py
+-rw-r--r--   0        0        0     1668 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/cmdcomp/v2/command/argument/values_argument.py
+-rw-r--r--   0        0        0      747 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/cmdcomp/v2/completion.py
+-rw-r--r--   0        0        0      380 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/cmdcomp/v2/config.py
+-rw-r--r--   0        0        0     4215 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/cmdcomp/v2/templates/bash.sh.jinja
+-rw-r--r--   0        0        0     2575 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/cmdcomp/v2/templates/zsh.sh.jinja
+-rw-r--r--   0        0        0     1779 2023-07-30 16:51:34.114601 cmdcomp-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3412 1970-01-01 00:00:00.000000 cmdcomp-2.0.1/PKG-INFO
```

### Comparing `cmdcomp-2.0.0/cmdcomp/app.py` & `cmdcomp-2.0.1/cmdcomp/app.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.0/cmdcomp/completion.py` & `cmdcomp-2.0.1/cmdcomp/completion.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.0/cmdcomp/v1/app_info.py` & `cmdcomp-2.0.1/cmdcomp/v1/app_info.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.0/cmdcomp/v1/command/__init__.py` & `cmdcomp-2.0.1/cmdcomp/v1/command/__init__.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.0/cmdcomp/v1/completion.py` & `cmdcomp-2.0.1/cmdcomp/v1/completion.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     )
 
 
 def _generate_completions_list(config: V1Config):
     completions_list = [get_candidates(config.root)]
 
     _update_completions_list(
-        completions_list,
+        completions_list,  # type: ignore
         config.root,
     )
 
     return completions_list
 
 
 def _update_completions_list(
```

### Comparing `cmdcomp-2.0.0/cmdcomp/v1/templates/bash.sh.jinja` & `cmdcomp-2.0.1/cmdcomp/v1/templates/bash.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.0/cmdcomp/v1/templates/zsh.sh.jinja` & `cmdcomp-2.0.1/cmdcomp/v1/templates/zsh.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.0/cmdcomp/v2/app_info.py` & `cmdcomp-2.0.1/cmdcomp/v2/app_info.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.0/cmdcomp/v2/command/__init__.py` & `cmdcomp-2.0.1/cmdcomp/v2/command/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from cmdcomp.v2.command.argument.values_argument import (
     V2ValueArgument,
     V2ValuesArgument,
 )
 
 from .argument import V2Argument
 
-Position: TypeAlias = int
+Position: TypeAlias = Annotated[int, Field(ge=1)]
 Keyword = Annotated[str, Field(pattern=r"^--?[a-zA-Z0-9_-]+$")]
 SubcommandName: TypeAlias = str
 
 
 class V2PoristionalArgumentsCommand(Model):
     model_config = ConfigDict(arbitrary_types_allowed=True)
```

### Comparing `cmdcomp-2.0.0/cmdcomp/v2/command/argument/command_argument.py` & `cmdcomp-2.0.1/cmdcomp/v2/command/argument/command_argument.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.0/cmdcomp/v2/command/argument/file_argument.py` & `cmdcomp-2.0.1/cmdcomp/v2/command/argument/file_argument.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.0/cmdcomp/v2/command/argument/flag_argument.py` & `cmdcomp-2.0.1/cmdcomp/v2/command/argument/flag_argument.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.0/cmdcomp/v2/command/argument/values_argument.py` & `cmdcomp-2.0.1/cmdcomp/v2/command/argument/values_argument.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.0/cmdcomp/v2/completion.py` & `cmdcomp-2.0.1/cmdcomp/v2/completion.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.0/cmdcomp/v2/templates/bash.sh.jinja` & `cmdcomp-2.0.1/cmdcomp/v2/templates/bash.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.0/cmdcomp/v2/templates/zsh.sh.jinja` & `cmdcomp-2.0.1/cmdcomp/v2/templates/zsh.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-2.0.0/pyproject.toml` & `cmdcomp-2.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmdcomp"
-version = "2.0.0"
+version = "2.0.1"
 description = "cmdcomp is a cli tool completion generator for shell."
 authors = ["Yasutanium <yassun4dev@outlook.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 repository = "https://github.com/yassun4dev/cmdcomp"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

