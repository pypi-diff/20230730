# Comparing `tmp/cmdcomp-1.2.0.tar.gz` & `tmp/cmdcomp-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdcomp-1.2.0.tar", max compression
+gzip compressed data, was "cmdcomp-2.0.0.tar", max compression
```

## Comparing `cmdcomp-1.2.0.tar` & `cmdcomp-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,35 @@
--rw-r--r--   0        0        0     1512 2023-07-15 01:20:00.699026 cmdcomp-1.2.0/README.md
--rw-r--r--   0        0        0       79 2023-07-15 01:20:00.699026 cmdcomp-1.2.0/cmdcomp/__init__.py
--rw-r--r--   0        0        0     2446 2023-07-15 01:20:00.699026 cmdcomp-1.2.0/cmdcomp/app.py
--rw-r--r--   0        0        0     2070 2023-07-15 01:20:00.699026 cmdcomp-1.2.0/cmdcomp/completion.py
--rw-r--r--   0        0        0        0 2023-07-15 01:20:00.699026 cmdcomp-1.2.0/cmdcomp/config/__init__.py
--rw-r--r--   0        0        0      540 2023-07-15 01:20:00.699026 cmdcomp-1.2.0/cmdcomp/config/app_info.py
--rw-r--r--   0        0        0      266 2023-07-15 01:20:00.699026 cmdcomp-1.2.0/cmdcomp/config/cmdcomp_info.py
--rw-r--r--   0        0        0        0 2023-07-15 01:20:00.699026 cmdcomp-1.2.0/cmdcomp/config/command/__init__.py
--rw-r--r--   0        0        0     3319 2023-07-15 01:20:00.699026 cmdcomp-1.2.0/cmdcomp/config/command/command.py
--rw-r--r--   0        0        0      348 2023-07-15 01:20:00.699026 cmdcomp-1.2.0/cmdcomp/config/command/option/__init__.py
--rw-r--r--   0        0        0      336 2023-07-15 01:20:00.703026 cmdcomp-1.2.0/cmdcomp/config/command/option/command_option.py
--rw-r--r--   0        0        0      378 2023-07-15 01:20:00.703026 cmdcomp-1.2.0/cmdcomp/config/command/option/file_option.py
--rw-r--r--   0        0        0      910 2023-07-15 01:20:00.703026 cmdcomp-1.2.0/cmdcomp/config/config.py
--rw-r--r--   0        0        0      115 2023-07-15 01:20:00.703026 cmdcomp-1.2.0/cmdcomp/config/model.py
--rw-r--r--   0        0        0      206 2023-07-15 01:20:00.703026 cmdcomp-1.2.0/cmdcomp/exception.py
--rw-r--r--   0        0        0       85 2023-07-15 01:20:00.703026 cmdcomp-1.2.0/cmdcomp/main.py
--rw-r--r--   0        0        0      131 2023-07-15 01:20:00.703026 cmdcomp-1.2.0/cmdcomp/shell.py
--rw-r--r--   0        0        0     1732 2023-07-15 01:20:00.703026 cmdcomp-1.2.0/cmdcomp/templates/bash.sh.jinja
--rw-r--r--   0        0        0     1277 2023-07-15 01:20:00.703026 cmdcomp-1.2.0/cmdcomp/templates/zsh.sh.jinja
--rw-r--r--   0        0        0     1696 2023-07-15 01:20:00.703026 cmdcomp-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2455 1970-01-01 00:00:00.000000 cmdcomp-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1517 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/README.md
+-rw-r--r--   0        0        0       79 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/cmdcomp/__init__.py
+-rw-r--r--   0        0        0     2358 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/cmdcomp/app.py
+-rw-r--r--   0        0        0      573 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/cmdcomp/completion.py
+-rw-r--r--   0        0        0      757 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/cmdcomp/config.py
+-rw-r--r--   0        0        0      206 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/cmdcomp/exception.py
+-rw-r--r--   0        0        0      115 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/cmdcomp/main.py
+-rw-r--r--   0        0        0      115 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/cmdcomp/model.py
+-rw-r--r--   0        0        0      131 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/cmdcomp/shell.py
+-rw-r--r--   0        0        0        0 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/cmdcomp/v1/__init__.py
+-rw-r--r--   0        0        0      535 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/cmdcomp/v1/app_info.py
+-rw-r--r--   0        0        0      261 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/cmdcomp/v1/cmdcomp_info.py
+-rw-r--r--   0        0        0     3358 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/cmdcomp/v1/command/__init__.py
+-rw-r--r--   0        0        0      338 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/cmdcomp/v1/command/option/__init__.py
+-rw-r--r--   0        0        0      331 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/cmdcomp/v1/command/option/command_option.py
+-rw-r--r--   0        0        0      373 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/cmdcomp/v1/command/option/file_option.py
+-rw-r--r--   0        0        0     2087 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/cmdcomp/v1/completion.py
+-rw-r--r--   0        0        0      377 2023-07-30 16:14:40.093257 cmdcomp-2.0.0/cmdcomp/v1/config.py
+-rw-r--r--   0        0        0     1732 2023-07-30 16:14:40.097257 cmdcomp-2.0.0/cmdcomp/v1/templates/bash.sh.jinja
+-rw-r--r--   0        0        0     1277 2023-07-30 16:14:40.097257 cmdcomp-2.0.0/cmdcomp/v1/templates/zsh.sh.jinja
+-rw-r--r--   0        0        0        0 2023-07-30 16:14:40.097257 cmdcomp-2.0.0/cmdcomp/v2/__init__.py
+-rw-r--r--   0        0        0      535 2023-07-30 16:14:40.097257 cmdcomp-2.0.0/cmdcomp/v2/app_info.py
+-rw-r--r--   0        0        0      261 2023-07-30 16:14:40.097257 cmdcomp-2.0.0/cmdcomp/v2/cmdcomp_info.py
+-rw-r--r--   0        0        0     6820 2023-07-30 16:14:40.097257 cmdcomp-2.0.0/cmdcomp/v2/command/__init__.py
+-rw-r--r--   0        0        0      371 2023-07-30 16:14:40.097257 cmdcomp-2.0.0/cmdcomp/v2/command/argument/__init__.py
+-rw-r--r--   0        0        0      789 2023-07-30 16:14:40.097257 cmdcomp-2.0.0/cmdcomp/v2/command/argument/command_argument.py
+-rw-r--r--   0        0        0      744 2023-07-30 16:14:40.097257 cmdcomp-2.0.0/cmdcomp/v2/command/argument/file_argument.py
+-rw-r--r--   0        0        0      601 2023-07-30 16:14:40.097257 cmdcomp-2.0.0/cmdcomp/v2/command/argument/flag_argument.py
+-rw-r--r--   0        0        0     1668 2023-07-30 16:14:40.097257 cmdcomp-2.0.0/cmdcomp/v2/command/argument/values_argument.py
+-rw-r--r--   0        0        0      747 2023-07-30 16:14:40.097257 cmdcomp-2.0.0/cmdcomp/v2/completion.py
+-rw-r--r--   0        0        0      380 2023-07-30 16:14:40.097257 cmdcomp-2.0.0/cmdcomp/v2/config.py
+-rw-r--r--   0        0        0     4215 2023-07-30 16:14:40.097257 cmdcomp-2.0.0/cmdcomp/v2/templates/bash.sh.jinja
+-rw-r--r--   0        0        0     2575 2023-07-30 16:14:40.097257 cmdcomp-2.0.0/cmdcomp/v2/templates/zsh.sh.jinja
+-rw-r--r--   0        0        0     1779 2023-07-30 16:14:40.097257 cmdcomp-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2504 1970-01-01 00:00:00.000000 cmdcomp-2.0.0/PKG-INFO
```

### Comparing `cmdcomp-1.2.0/README.md` & `cmdcomp-2.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         <img src="https://badge.fury.io/py/cmdcomp.svg" alt="PIP Version">
     </a>
     <a href="https://hub.docker.com/r/yassun4dev/cmdcomp">
         <img src="https://img.shields.io/docker/v/yassun4dev/cmdcomp/latest?label=docker%20version" alt="Docker Version">
     </a>
 </p>
 
-`cmdcomp` generate shell completion file (bash or zsh) from config toml file.
+`cmdcomp` generate shell completion file (bash or zsh) from config yaml/toml file.
 
 ## Install
 
 ```shell
 pip install cmdcomp
 ```
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 # Command Completion Generator Tool
                   [Test_Suite] [PIP_Version] [Docker_Version]
-`cmdcomp` generate shell completion file (bash or zsh) from config toml file.
-## Install ```shell pip install cmdcomp ``` ## Usage ### Local ```shell cmdcomp
---file ${YOUR_CONFIG_FILE} --shell-type bash ``` ### Docker ```shell docker run
---rm -itv $(pwd):/app/cmdcomp yassun4dev/cmdcomp --file ${YOUR_CONFIG_FILE} --
-shell-type bash ``` ## Config Configuration can be written in JSON, YAML, and
-TOML file formats. ### Sample ```toml [cmdcomp] version = "1" [app] name =
-"mycli" alias = "my-cli" [root] options = ["-h", "--help", "--version"]
-[root.subcommands.list] options = ["-a"] alias = "ls"
+`cmdcomp` generate shell completion file (bash or zsh) from config yaml/toml
+file. ## Install ```shell pip install cmdcomp ``` ## Usage ### Local ```shell
+cmdcomp --file ${YOUR_CONFIG_FILE} --shell-type bash ``` ### Docker ```shell
+docker run --rm -itv $(pwd):/app/cmdcomp yassun4dev/cmdcomp --file $
+{YOUR_CONFIG_FILE} --shell-type bash ``` ## Config Configuration can be written
+in JSON, YAML, and TOML file formats. ### Sample ```toml [cmdcomp] version =
+"1" [app] name = "mycli" alias = "my-cli" [root] options = ["-h", "--help", "--
+version"] [root.subcommands.list] options = ["-a"] alias = "ls"
 [root.subcommands.execute] options = { type = "command", execute =
 "your_app_name ps -s" } alias = ["restart", "shell", "log"]
 [root.subcommands.cd] options = { type = "file", base_path = "$(cd $(dirname
 $0); pwd)/../apps" } ``` ### JSON Schema https://raw.githubusercontent.com/
 yassun4dev/cmdcomp/main/docs/config.schema.json
```

### Comparing `cmdcomp-1.2.0/cmdcomp/app.py` & `cmdcomp-2.0.0/cmdcomp/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 class App:
     @classmethod
-    def run(
-        cls,
-        args: list[str] | None = None,
-        *,
-        throw_exception: bool = True,
-    ) -> None:
+    def run(cls, args: list[str] | None = None) -> None:
         import logging
         from argparse import ArgumentParser, BooleanOptionalAction, FileType
         from logging import getLogger
 
+        import argcomplete
         from rich.console import Console
         from rich.logging import RichHandler
 
         from cmdcomp import __version__
         from cmdcomp.completion import generate
-        from cmdcomp.config.config import load
+        from cmdcomp.config import load
         from cmdcomp.shell import ShellType
 
         parser = ArgumentParser(
             prog="cmdcomp",
             description="A command-line tool for comparing commands.",
         )
 
@@ -54,14 +50,16 @@
 
         parser.add_argument(
             "--verbose",
             action=BooleanOptionalAction,
             help="output verbose log.",
         )
 
+        argcomplete.autocomplete(parser)
+
         space = parser.parse_args(args)
 
         logging.basicConfig(
             format="%(message)s",
             handlers=[
                 RichHandler(
                     level=logging.DEBUG if space.verbose else logging.INFO,
@@ -82,11 +80,8 @@
 
         except Exception as e:
             if space.verbose:
                 logger.exception(e)
             else:
                 logger.error(e)
 
-            if throw_exception:
-                raise e
-            else:
-                exit(1)
+            raise e
```

### Comparing `cmdcomp-1.2.0/cmdcomp/completion.py` & `cmdcomp-2.0.0/cmdcomp/v1/completion.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,69 +1,69 @@
 from functools import reduce
 from pathlib import Path
 
 from mergedeep import merge
 
-from cmdcomp.config.command.command import (
-    Candidates,
-    Command,
-    Completions,
-    SubCommandsCommand,
+from cmdcomp.shell import ShellType
+from cmdcomp.v1.command import (
+    V1Candidates,
+    V1Command,
+    V1Completions,
+    V1SubCommandsCommand,
     get_candidates,
     get_targets,
 )
-from cmdcomp.config.config import Config
-from cmdcomp.shell import ShellType
+from cmdcomp.v1.config import V1Config
 
 
-def generate(shell: ShellType, config: Config):
+def generate_v1(shell: ShellType, config: V1Config):
     from jinja2 import Environment, FileSystemLoader
 
     env = Environment(
         loader=FileSystemLoader(Path(__file__).parent / "templates"),
     )
     template = env.get_template(f"{shell.value}.sh.jinja")
 
     return template.render(
         app_name=config.app.name,
         app_aliases=config.app.aliases + config.root.aliases,
-        completions_list=generate_completions_list(config),
+        completions_list=_generate_completions_list(config),
     )
 
 
-def generate_completions_list(config: Config):
+def _generate_completions_list(config: V1Config):
     completions_list = [get_candidates(config.root)]
 
     _update_completions_list(
         completions_list,
         config.root,
     )
 
     return completions_list
 
 
 def _update_completions_list(
-    completions_list: list[Completions],
-    command: Command,
+    completions_list: list[V1Completions],
+    command: V1Command,
     keys: list[str] | None = None,
 ):
     if keys is None:
         keys = []
 
-    if not isinstance(command, SubCommandsCommand):
+    if not isinstance(command, V1SubCommandsCommand):
         return
 
     for name, optional_subcommand in command.subcommands.items():
-        subcommand = optional_subcommand or SubCommandsCommand.model_validate({})
+        subcommand = optional_subcommand or V1SubCommandsCommand.model_validate({})
 
         new_keys = keys + ["|".join(get_targets(name, subcommand))]
 
         _update_completions_list(completions_list, subcommand, new_keys)
 
-        candidates: Candidates = get_candidates(subcommand)
+        candidates: V1Candidates = get_candidates(subcommand)
 
         if len(candidates) == 0:
             continue
 
         while len(completions_list) < len(new_keys) + 1:
             completions_list.append({})
 
@@ -73,9 +73,9 @@
                 _swap_key_value,  # type: ignore
                 reversed(new_keys),
                 candidates,  # type: ignore
             ),
         )
 
 
-def _swap_key_value(prev: Completions, key: str) -> Completions:
+def _swap_key_value(prev: V1Completions, key: str) -> V1Completions:
     return {key: prev}
```

### Comparing `cmdcomp-1.2.0/cmdcomp/config/app_info.py` & `cmdcomp-2.0.0/cmdcomp/v1/app_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Annotated
 
 from pydantic import Field
 
-from cmdcomp.config.model import Model
+from cmdcomp.model import Model
 
 
-class AppInfo(Model):
+class V1AppInfo(Model):
     """your cli app info."""
 
     name: Annotated[str, Field(title="your cli app name.")]
 
     alias: Annotated[
         str | list[str],
         Field(
```

### Comparing `cmdcomp-1.2.0/cmdcomp/config/command/command.py` & `cmdcomp-2.0.0/cmdcomp/v1/command/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,124 +1,119 @@
 from functools import reduce
 from operator import add
 from typing import Annotated, NewType, OrderedDict
 
 from pydantic import ConfigDict, Field
 
-from cmdcomp.config.command.option import (
-    OptionType,
-    SpecificOptions,
-    StrOption,
-    StrOptions,
-)
-from cmdcomp.config.command.option.command_option import CommandOption
-from cmdcomp.config.command.option.file_option import FileOption
-from cmdcomp.config.model import Model
 from cmdcomp.exception import NeverReach
+from cmdcomp.model import Model
+from cmdcomp.v1.command.option import V1OptionType, V1SpecificOptions, V1StrOption
+from cmdcomp.v1.command.option.command_option import V1CommandOption
+from cmdcomp.v1.command.option.file_option import V1FileOption
 
-SubcommandName = NewType("SubcommandName", str)
+V1SubcommandName = NewType("V1SubcommandName", str)
 
-Candidate = SubcommandName | StrOption
-Candidates = list[Candidate] | list[dict[OptionType, str]]
+V1Candidate = V1SubcommandName | V1StrOption
+V1Candidates = list[V1Candidate] | list[dict[V1OptionType, str]]
 
-Completions = Candidates | dict[str, "Completions"]  # type: ignore
+V1Completions = V1Candidates | dict[str, "V1Completions"]  # type: ignore
 
 
-class SubCommandsCommand(Model):
+class V1SubCommandsCommand(Model):
     """A command that can specify a subcommand."""
 
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
     alias: Annotated[
         str | list[str],
         Field(
             title="alias of the command.",
             default_factory=list,
         ),
     ]
 
     options: Annotated[
-        StrOptions,
+        V1StrOption | list[V1StrOption],
         Field(
             title="options of the command.",
             default_factory=list,
         ),
     ]
 
-    subcommands: OrderedDict[SubcommandName, "Command | None"] = Field(
+    subcommands: OrderedDict[V1SubcommandName, "V1Command | None"] = Field(
         title="subcommands of the command.",
         default_factory=OrderedDict,
     )
 
     @property
     def aliases(self) -> list[str]:
         if isinstance(self.alias, str):
             return [self.alias]
         else:
             return self.alias
 
 
-class SpecificOptionsCommand(Model):
+class V1SpecificOptionsCommand(Model):
     """A command that can specify options."""
 
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
     alias: Annotated[
         str | list[str],
         Field(
             title="alias of the command.",
             default_factory=list,
         ),
     ]
 
     options: Annotated[
-        SpecificOptions,
+        V1SpecificOptions,
         Field(
             title="options of the command.",
         ),
     ]
 
     @property
     def aliases(self) -> list[str]:
         if isinstance(self.alias, str):
             return [self.alias]
         else:
             return self.alias
 
 
-Command = SubCommandsCommand | SpecificOptionsCommand
+V1Command = V1SubCommandsCommand | V1SpecificOptionsCommand
 
-Subcommands = OrderedDict[SubcommandName, Command | None]
+Subcommands = OrderedDict[V1SubcommandName, V1Command | None]
 
 
-def get_targets(name: SubcommandName, subcommand: Command) -> list[str]:
+def get_targets(name: V1SubcommandName, subcommand: V1Command) -> list[str]:
     return [name] + subcommand.aliases
 
 
-def get_candidates(command: Command) -> Candidates:
+def get_candidates(command: V1Command) -> V1Candidates:
     match command:
-        case SubCommandsCommand():
+        case V1SubCommandsCommand():
             return (
                 [command.options]
                 if isinstance(command.options, str)
                 else command.options
             ) + reduce(
                 add,
                 [
                     get_targets(
                         name,
-                        subcommand or SubCommandsCommand.model_validate({}),
+                        subcommand or V1SubCommandsCommand.model_validate({}),
                     )
                     for name, subcommand in command.subcommands.items()
                 ],
                 [],
             )
-        case SpecificOptionsCommand():
-            if isinstance(command.options, CommandOption):
+        case V1SpecificOptionsCommand():
+            if isinstance(command.options, V1CommandOption):
                 return [{"command": f"$({command.options.execute})"}]
 
-            elif isinstance(command.options, FileOption):
+            elif isinstance(command.options, V1FileOption):
                 return [{"file": command.options.base_path}]
             else:
                 raise NeverReach(command.options)
         case _:
             raise NeverReach(command)
```

### Comparing `cmdcomp-1.2.0/cmdcomp/config/config.py` & `cmdcomp-2.0.0/cmdcomp/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 import json
 import os
 import tomllib
 from typing import BinaryIO
 
 import yaml
-from pydantic import ConfigDict
+from pydantic import RootModel
 
-from cmdcomp.config.app_info import AppInfo
-from cmdcomp.config.cmdcomp_info import CmdCompInfo
-from cmdcomp.config.command.command import Command
-from cmdcomp.config.model import Model
+from cmdcomp.v1.config import V1Config
+from cmdcomp.v2.config import V2Config
 
 
-class Config(Model):
+class Config(RootModel):
     """cmdcomp config."""
 
-    model_config = ConfigDict(arbitrary_types_allowed=True, extra="forbid")
-
-    cmdcomp: CmdCompInfo
-    app: AppInfo
-    root: Command
+    root: V1Config | V2Config
 
 
 def load(file: BinaryIO) -> Config:
     _, extention = os.path.splitext(file.name)
     match extention:
+        # TODO: In v2, we will remove support for json.
         case ".json":
             data = json.load(file)
+
         case ".yaml" | ".yml":
             data = yaml.full_load(file)
+
         case ".toml":
             data = tomllib.load(file)
+
         case _:
             raise Exception(f"Unsupported config file type `{extention}`.")
 
     return Config.model_validate(data)
```

### Comparing `cmdcomp-1.2.0/cmdcomp/templates/bash.sh.jinja` & `cmdcomp-2.0.0/cmdcomp/v1/templates/bash.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.2.0/cmdcomp/templates/zsh.sh.jinja` & `cmdcomp-2.0.0/cmdcomp/v1/templates/zsh.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.2.0/pyproject.toml` & `cmdcomp-2.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmdcomp"
-version = "1.2.0"
+version = "2.0.0"
 description = "cmdcomp is a cli tool completion generator for shell."
 authors = ["Yasutanium <yassun4dev@outlook.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 repository = "https://github.com/yassun4dev/cmdcomp"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -18,25 +18,27 @@
 ]
 
 [tool.poetry.scripts]
 cmdcomp = "cmdcomp.main:main"
 
 [tool.taskipy.tasks]
 generate-json-schema = "python tasks/generate_json_schema.py > docs/config.schema.json"
+generate-completion = "register-python-argcomplete cmdcomp"
 test = "pytest"
 format = "black --target-version py310 ."
 lint = "pyright cmdcomp/** tests/**"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pydantic = "^2.0"
 jinja2 = "^3.1.2"
 mergedeep = "^1.3.4"
 pyyaml = "^6.0"
 rich = "^13.4.2"
+argcomplete = "^3.1.1"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
 black = "^23.1.0"
 isort = "^5.12.0"
 pytest = "^7.2.2"
 pyright = "^1.1.300"
```

### Comparing `cmdcomp-1.2.0/PKG-INFO` & `cmdcomp-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: cmdcomp
-Version: 1.2.0
+Version: 2.0.0
 Summary: cmdcomp is a cli tool completion generator for shell.
 Home-page: https://github.com/yassun4dev/cmdcomp
 License: BSD-3-Clause
 Author: Yasutanium
 Author-email: yassun4dev@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
+Requires-Dist: argcomplete (>=3.1.1,<4.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: mergedeep (>=1.3.4,<2.0.0)
 Requires-Dist: pydantic (>=2.0,<3.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Project-URL: Repository, https://github.com/yassun4dev/cmdcomp
 Description-Content-Type: text/markdown
@@ -33,15 +34,15 @@
         <img src="https://badge.fury.io/py/cmdcomp.svg" alt="PIP Version">
     </a>
     <a href="https://hub.docker.com/r/yassun4dev/cmdcomp">
         <img src="https://img.shields.io/docker/v/yassun4dev/cmdcomp/latest?label=docker%20version" alt="Docker Version">
     </a>
 </p>
 
-`cmdcomp` generate shell completion file (bash or zsh) from config toml file.
+`cmdcomp` generate shell completion file (bash or zsh) from config yaml/toml file.
 
 ## Install
 
 ```shell
 pip install cmdcomp
 ```
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1 Name: cmdcomp Version: 1.2.0 Summary: cmdcomp is a cli
+Metadata-Version: 2.1 Name: cmdcomp Version: 2.0.0 Summary: cmdcomp is a cli
 tool completion generator for shell. Home-page: https://github.com/yassun4dev/
 cmdcomp License: BSD-3-Clause Author: Yasutanium Author-email:
 yassun4dev@outlook.com Requires-Python: >=3.11,<4.0 Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
-Software Development Classifier: Typing :: Typed Requires-Dist: jinja2
-(>=3.1.2,<4.0.0) Requires-Dist: mergedeep (>=1.3.4,<2.0.0) Requires-Dist:
-pydantic (>=2.0,<3.0) Requires-Dist: pyyaml (>=6.0,<7.0) Requires-Dist: rich
-(>=13.4.2,<14.0.0) Project-URL: Repository, https://github.com/yassun4dev/
-cmdcomp Description-Content-Type: text/markdown # Command Completion Generator
-Tool
+Software Development Classifier: Typing :: Typed Requires-Dist: argcomplete
+(>=3.1.1,<4.0.0) Requires-Dist: jinja2 (>=3.1.2,<4.0.0) Requires-Dist:
+mergedeep (>=1.3.4,<2.0.0) Requires-Dist: pydantic (>=2.0,<3.0) Requires-Dist:
+pyyaml (>=6.0,<7.0) Requires-Dist: rich (>=13.4.2,<14.0.0) Project-URL:
+Repository, https://github.com/yassun4dev/cmdcomp Description-Content-Type:
+text/markdown # Command Completion Generator Tool
                   [Test_Suite] [PIP_Version] [Docker_Version]
-`cmdcomp` generate shell completion file (bash or zsh) from config toml file.
-## Install ```shell pip install cmdcomp ``` ## Usage ### Local ```shell cmdcomp
---file ${YOUR_CONFIG_FILE} --shell-type bash ``` ### Docker ```shell docker run
---rm -itv $(pwd):/app/cmdcomp yassun4dev/cmdcomp --file ${YOUR_CONFIG_FILE} --
-shell-type bash ``` ## Config Configuration can be written in JSON, YAML, and
-TOML file formats. ### Sample ```toml [cmdcomp] version = "1" [app] name =
-"mycli" alias = "my-cli" [root] options = ["-h", "--help", "--version"]
-[root.subcommands.list] options = ["-a"] alias = "ls"
+`cmdcomp` generate shell completion file (bash or zsh) from config yaml/toml
+file. ## Install ```shell pip install cmdcomp ``` ## Usage ### Local ```shell
+cmdcomp --file ${YOUR_CONFIG_FILE} --shell-type bash ``` ### Docker ```shell
+docker run --rm -itv $(pwd):/app/cmdcomp yassun4dev/cmdcomp --file $
+{YOUR_CONFIG_FILE} --shell-type bash ``` ## Config Configuration can be written
+in JSON, YAML, and TOML file formats. ### Sample ```toml [cmdcomp] version =
+"1" [app] name = "mycli" alias = "my-cli" [root] options = ["-h", "--help", "--
+version"] [root.subcommands.list] options = ["-a"] alias = "ls"
 [root.subcommands.execute] options = { type = "command", execute =
 "your_app_name ps -s" } alias = ["restart", "shell", "log"]
 [root.subcommands.cd] options = { type = "file", base_path = "$(cd $(dirname
 $0); pwd)/../apps" } ``` ### JSON Schema https://raw.githubusercontent.com/
 yassun4dev/cmdcomp/main/docs/config.schema.json
```

