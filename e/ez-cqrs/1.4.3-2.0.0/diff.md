# Comparing `tmp/ez_cqrs-1.4.3.tar.gz` & `tmp/ez_cqrs-2.0.0.tar.gz`

## Comparing `ez_cqrs-1.4.3.tar` & `ez_cqrs-2.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/.tool-versions
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/mkdocs.yml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/.github/CODEOWNERS
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/.github/workflows/release.yml
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/.github/workflows/test.yml
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/.vscode/settings.json
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/ez_cqrs/__init__.py
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/ez_cqrs/acid_exec.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/ez_cqrs/components.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/ez_cqrs/error.py
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/ez_cqrs/framework.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/ez_cqrs/handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/ez_cqrs/py.typed
--rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/ez_cqrs/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/ez_cqrs/utilities/__init__.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/ez_cqrs/utilities/cli.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/requirements/core.txt
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/requirements/dev.txt
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/scripts/new_release.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/tests/__init__.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/tests/integration/conftest.py
--rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/tests/integration/test_execution.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/tests/unit/test_acid_exec.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/LICENSE
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/README.md
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/pyproject.toml
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/.tool-versions
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/mkdocs.yml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/.vscode/settings.json
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/ez_cqrs/__init__.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/ez_cqrs/acid_exec.py
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/ez_cqrs/components.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/ez_cqrs/error.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/ez_cqrs/handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/ez_cqrs/py.typed
+-rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/ez_cqrs/framework/__init__.py
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/ez_cqrs/framework/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/ez_cqrs/utilities/__init__.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/ez_cqrs/utilities/cli.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/requirements/core.txt
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/requirements/dev.txt
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/scripts/new_release.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/tests/conftest.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/tests/test_acid_exec.py
+-rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/tests/test_framework.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/LICENSE
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/README.md
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/PKG-INFO
```

### Comparing `ez_cqrs-1.4.3/.github/workflows/release.yml` & `ez_cqrs-2.0.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.4.3/.github/workflows/test.yml` & `ez_cqrs-2.0.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.4.3/.vscode/settings.json` & `ez_cqrs-2.0.0/.vscode/settings.json`

 * *Files 17% similar despite different names*

```diff
@@ -6,18 +6,26 @@
         100
     ],
     "python.testing.pytestArgs": [
         "tests",
         // https://github.com/microsoft/vscode-python/issues/693#issuecomment-367856613
         "--no-cov"
     ],
-    "python.testing.pytestEnabled": true,
+    "[python]": {
+        "diffEditor.ignoreTrimWhitespace": false,
+        "editor.formatOnType": false,
+        "editor.wordBasedSuggestions": false
+    },
     "python.analysis.autoImportCompletions": true,
-    "python.analysis.completeFunctionParens": true,
-    "python.analysis.inlayHints.callArgumentNames": true,
-    "python.analysis.inlayHints.variableTypes": true,
+    "python.analysis.extraCommitChars": false,
+    "python.analysis.inlayHints.callArgumentNames": false,
+    "python.analysis.inlayHints.pytestParameters": false,
+    "python.analysis.inlayHints.functionReturnTypes": false,
+    "python.analysis.inlayHints.variableTypes": false,
     "python.analysis.typeCheckingMode": "basic",
     "python.analysis.userFileIndexingLimit": -1,
-    "[python]": {
-        "editor.defaultFormatter": "ms-python.black-formatter"
-    }
+    "python.testing.unittestEnabled": false,
+    "python.testing.pytestEnabled": true,
+    "python.analysis.diagnosticMode": "workspace",
+
+
 }
```

### Comparing `ez_cqrs-1.4.3/ez_cqrs/acid_exec.py` & `ez_cqrs-2.0.0/ez_cqrs/acid_exec.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         return self._storage.copy()
 
     def storage_length(self) -> int:
         """Get storage length."""
         return len(self._storage)
 
 
-class IRepository(abc.ABC):
+class ACID(abc.ABC):
     """
     Repository gives acces to the system database layer.
 
     A database must support transaction operations.
 
     Besides being the client between the core layer and the persistence layer,
     a system repository is intended to be used right before a command handling
```

### Comparing `ez_cqrs-1.4.3/ez_cqrs/components.py` & `ez_cqrs-2.0.0/ez_cqrs/components.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 """CQRS core components."""
 from __future__ import annotations
 
-import abc
 from dataclasses import dataclass
 from typing import TypeVar
 
 from mashumaro import DataClassDictMixin
 from mashumaro.mixins.orjson import DataClassORJSONMixin
 
 
 @dataclass(frozen=True)
-class Command(abc.ABC, DataClassDictMixin):
+class UseCaseOutput(DataClassDictMixin):
+    """UseCase Output container."""
+
+
+@dataclass(frozen=True)
+class Command(DataClassDictMixin):
     """
     Command baseclass.
 
     In order to make changes to our system we'll need commands. These
     are the simplest components of any CQRS system and consist of little more than
     packaged data.
     """
 
 
 @dataclass(frozen=True)
-class DomainEvent(abc.ABC, DataClassORJSONMixin):
+class DomainEvent(DataClassORJSONMixin):
     """
     Domain Event base class.
 
     A `DomainEvent` represents any business change in the state of an `Aggregate`.
     `DomainEvents` are inmutable, and when [event sourcing](https://martinfowler.com/eaaDev/EventSourcing.html)
     is used they are the single source of truth.
```

### Comparing `ez_cqrs-1.4.3/ez_cqrs/error.py` & `ez_cqrs-2.0.0/ez_cqrs/error.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.4.3/ez_cqrs/framework.py` & `ez_cqrs-2.0.0/ez_cqrs/framework/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """Ez-Cqrs Framwork."""
 from __future__ import annotations
 
 import asyncio
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Any, Generic, TypeVar, final
 
-from result import Ok, Result
+from result import Ok
 
-from ez_cqrs.acid_exec import IRepository, OpsRegistry
+from ez_cqrs.acid_exec import OpsRegistry
 from ez_cqrs.components import C, E
 
 if TYPE_CHECKING:
     import pydantic
+    from result import Result
 
+    from ez_cqrs.acid_exec import ACID
+    from ez_cqrs.components import UseCaseOutput
     from ez_cqrs.error import ExecutionError
     from ez_cqrs.handler import CommandHandler, EventDispatcher
 
 T = TypeVar("T")
 
 
 @final
@@ -27,16 +30,19 @@
     cmd_handler: CommandHandler[C, E]
     event_dispatcher: EventDispatcher[E]
 
     async def run(
         self,
         cmd: C,
         max_transactions: int,
-        app_database: IRepository | None,
-    ) -> Result[Any, ExecutionError | pydantic.ValidationError]:
+        app_database: ACID | None,
+    ) -> Result[
+        tuple[UseCaseOutput, list[E]],
+        ExecutionError | pydantic.ValidationError,
+    ]:
         """
         Validate and execute command, then dispatch command events.
 
         Dispatched events are returned to the caller for client specific usage.
         """
         if max_transactions > 0 and not app_database:
             msg = "You are not setting a database to commit transactions"
@@ -78,8 +84,8 @@
 
         event_dispatch_tasks = (
             self.event_dispatcher.dispatch(x) for x in event_registry
         )
 
         asyncio.gather(*event_dispatch_tasks, return_exceptions=False)
 
-        return Ok(execution_result_or_err.unwrap())
+        return Ok((execution_result_or_err.unwrap(), event_registry))
```

### Comparing `ez_cqrs-1.4.3/ez_cqrs/handler.py` & `ez_cqrs-2.0.0/ez_cqrs/handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from ez_cqrs.components import C, E
 
 if TYPE_CHECKING:
     import pydantic
     from result import Result
 
     from ez_cqrs.acid_exec import OpsRegistry
+    from ez_cqrs.components import UseCaseOutput
     from ez_cqrs.error import ExecutionError
 
 
 class CommandHandler(abc.ABC, Generic[C, E]):
     """Command handler handles every command to complete one user intent."""
 
     @abc.abstractmethod
@@ -26,15 +27,15 @@
 
     @abc.abstractmethod
     async def handle(
         self,
         command: C,
         ops_registry: OpsRegistry[Any],
         event_registry: list[E],
-    ) -> Result[Any, ExecutionError]:
+    ) -> Result[UseCaseOutput, ExecutionError]:
         """
         Consume and process commands.
 
         The result should be either a vector of events if the command is successful,
         or an error is the command is rejected.
 
         _All business logic belongs in this method_.
```

### Comparing `ez_cqrs-1.4.3/ez_cqrs/utilities/cli.py` & `ez_cqrs-2.0.0/ez_cqrs/utilities/cli.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.4.3/requirements/dev.txt` & `ez_cqrs-2.0.0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.4.3/scripts/new_release.py` & `ez_cqrs-2.0.0/scripts/new_release.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.4.3/tests/integration/conftest.py` & `ez_cqrs-2.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.4.3/tests/unit/test_acid_exec.py` & `ez_cqrs-2.0.0/tests/test_acid_exec.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.4.3/.gitignore` & `ez_cqrs-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.4.3/LICENSE` & `ez_cqrs-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.4.3/pyproject.toml` & `ez_cqrs-2.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ez_cqrs"
-version = "1.4.3"
+version = "2.0.0"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 authors = [
@@ -50,15 +50,22 @@
     "node_modules",
     "venv",
 ]
 
 [tool.ruff.per-file-ignores]
 "scripts/*.py" = ["INP001"]
 "__init__.py" = ["D104"]
-"tests/*.py" = ["INP001", "S101"]
+"tests/*.py" = ["INP001", "S101", "D101", "D102"]
+
+[tool.ruff.flake8-type-checking]
+runtime-evaluated-base-classes = [
+    "pydantic.BaseModel",
+    "mashumaro.mixins.orjson.DataClassORJSONMixin",
+]
+strict = true
 
 [tool.ruff.isort]
 known-first-party = ["ez_cqrs"]
 force-wrap-aliases = true
 combine-as-imports = true
 required-imports = ["from __future__ import annotations"]
```

### Comparing `ez_cqrs-1.4.3/PKG-INFO` & `ez_cqrs-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez_cqrs
-Version: 1.4.3
+Version: 2.0.0
 Project-URL: Documentation, https://github.com/Tomperez98/ez-cqrs#readme
 Project-URL: Issues, https://github.com/Tomperez98/ez-cqrs/issues
 Project-URL: Source, https://github.com/Tomperez98/ez-cqrs
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

