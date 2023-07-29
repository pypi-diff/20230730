# Comparing `tmp/ez_cqrs-2.2.0.tar.gz` & `tmp/ez_cqrs-2.3.0.tar.gz`

## Comparing `ez_cqrs-2.2.0.tar` & `ez_cqrs-2.3.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/.tool-versions
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/mkdocs.yml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/.vscode/settings.json
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/ez_cqrs/__init__.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/ez_cqrs/acid_exec.py
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/ez_cqrs/components.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/ez_cqrs/error.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/ez_cqrs/handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/ez_cqrs/py.typed
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/ez_cqrs/framework/__init__.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/ez_cqrs/framework/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/ez_cqrs/utilities/__init__.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/ez_cqrs/utilities/cli.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/requirements/core.txt
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/requirements/dev.txt
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/scripts/new_release.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/tests/__init__.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/tests/conftest.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/tests/test_acid_exec.py
--rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/tests/test_framework.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/LICENSE
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/README.md
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/pyproject.toml
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 ez_cqrs-2.3.0/.tool-versions
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ez_cqrs-2.3.0/mkdocs.yml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-2.3.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-2.3.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 ez_cqrs-2.3.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 ez_cqrs-2.3.0/.vscode/settings.json
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ez_cqrs-2.3.0/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.3.0/ez_cqrs/__init__.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 ez_cqrs-2.3.0/ez_cqrs/acid_exec.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 ez_cqrs-2.3.0/ez_cqrs/components.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 ez_cqrs-2.3.0/ez_cqrs/error.py
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 ez_cqrs-2.3.0/ez_cqrs/handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.3.0/ez_cqrs/py.typed
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 ez_cqrs-2.3.0/ez_cqrs/framework/__init__.py
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 ez_cqrs-2.3.0/ez_cqrs/framework/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.3.0/ez_cqrs/utilities/__init__.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ez_cqrs-2.3.0/ez_cqrs/utilities/cli.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 ez_cqrs-2.3.0/requirements/core.txt
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 ez_cqrs-2.3.0/requirements/dev.txt
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-2.3.0/scripts/new_release.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-2.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-2.3.0/tests/test_acid_exec.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 ez_cqrs-2.3.0/tests/test_framework.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ez_cqrs-2.3.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-2.3.0/LICENSE
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ez_cqrs-2.3.0/README.md
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 ez_cqrs-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 ez_cqrs-2.3.0/PKG-INFO
```

### Comparing `ez_cqrs-2.2.0/.github/workflows/release.yml` & `ez_cqrs-2.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.2.0/.github/workflows/test.yml` & `ez_cqrs-2.3.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.2.0/.vscode/settings.json` & `ez_cqrs-2.3.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.2.0/ez_cqrs/acid_exec.py` & `ez_cqrs-2.3.0/ez_cqrs/acid_exec.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.2.0/ez_cqrs/components.py` & `ez_cqrs-2.3.0/ez_cqrs/components.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,7 +41,8 @@
     To simplify serialization, an event should be an enum, and each variant should carry
     any important information.
     """
 
 
 C = TypeVar("C", bound=Command)
 E = TypeVar("E", bound=DomainEvent)
+OUT = TypeVar("OUT", bound=UseCaseOutput)
```

### Comparing `ez_cqrs-2.2.0/ez_cqrs/error.py` & `ez_cqrs-2.3.0/ez_cqrs/error.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.2.0/ez_cqrs/handler.py` & `ez_cqrs-2.3.0/ez_cqrs/handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """Command handler definition."""
 from __future__ import annotations
 
 import abc
 from typing import TYPE_CHECKING, Any, Generic
 
-from ez_cqrs.components import C, E
+from ez_cqrs.components import OUT, C, E
 
 if TYPE_CHECKING:
     import pydantic
     from result import Result
 
     from ez_cqrs.acid_exec import OpsRegistry
-    from ez_cqrs.components import UseCaseOutput
     from ez_cqrs.error import ExecutionError
 
 
-class CommandHandler(abc.ABC, Generic[C, E]):
+class CommandHandler(abc.ABC, Generic[C, E, OUT]):
     """Command handler handles every command to complete one user intent."""
 
     @abc.abstractmethod
     def validate(
         self,
         command: C,
     ) -> Result[None, pydantic.ValidationError]:
@@ -27,15 +26,15 @@
 
     @abc.abstractmethod
     async def handle(
         self,
         command: C,
         ops_registry: OpsRegistry[Any],
         event_registry: list[E],
-    ) -> Result[UseCaseOutput, ExecutionError]:
+    ) -> Result[OUT, ExecutionError]:
         """
         Consume and process commands.
 
         The result should be either a vector of events if the command is successful,
         or an error is the command is rejected.
 
         _All business logic belongs in this method_.
```

### Comparing `ez_cqrs-2.2.0/ez_cqrs/framework/__init__.py` & `ez_cqrs-2.3.0/ez_cqrs/framework/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,43 +4,42 @@
 import asyncio
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Any, Generic, TypeVar, final
 
 from result import Ok
 
 from ez_cqrs.acid_exec import OpsRegistry
-from ez_cqrs.components import C, E
+from ez_cqrs.components import OUT, C, E
 
 if TYPE_CHECKING:
     import pydantic
     from result import Result
 
     from ez_cqrs.acid_exec import ACID
-    from ez_cqrs.components import UseCaseOutput
     from ez_cqrs.error import ExecutionError
     from ez_cqrs.handler import CommandHandler, EventDispatcher
 
 T = TypeVar("T")
 
 
 @final
 @dataclass(repr=True, frozen=True, eq=False)
-class EzCqrs(Generic[C, E]):
+class EzCqrs(Generic[C, E, OUT]):
     """EzCqrs framework."""
 
-    cmd_handler: CommandHandler[C, E]
+    cmd_handler: CommandHandler[C, E, OUT]
     event_dispatcher: EventDispatcher[E]
 
     async def run(
         self,
         cmd: C,
         max_transactions: int,
         app_database: ACID | None,
         event_registry: list[E],
-    ) -> Result[UseCaseOutput, ExecutionError | pydantic.ValidationError]:
+    ) -> Result[OUT, ExecutionError | pydantic.ValidationError]:
         """
         Validate and execute command, then dispatch command events.
 
         Dispatched events are returned to the caller for client specific usage.
         """
         if max_transactions > 0 and not app_database:
             msg = "You are not setting a database to commit transactions"
```

### Comparing `ez_cqrs-2.2.0/ez_cqrs/framework/testing.py` & `ez_cqrs-2.3.0/ez_cqrs/framework/testing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Testing framework for EzCQRS framework."""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Generic, final
 
 from result import Ok
 
-from ez_cqrs.components import C, E
+from ez_cqrs.components import OUT, C, E
 from ez_cqrs.error import DomainError
 
 if TYPE_CHECKING:
     from result import Result
 
     from ez_cqrs.acid_exec import ACID
     from ez_cqrs.components import UseCaseOutput
@@ -18,18 +18,18 @@
 
 NO_COMMAND_ERROR = "There's not command setted."
 CLEAR_ERROR = "Command already set. run `clear()`"
 NO_EXECUTION_ERROR = "Run execute before checking results."
 
 
 @final
-class EzCQRSTester(Generic[C, E]):
+class EzCQRSTester(Generic[C, E, OUT]):
     """Testing framework for EzCRQS."""
 
-    def __init__(self, framework: EzCqrs[C, E], app_database: ACID | None) -> None:
+    def __init__(self, framework: EzCqrs[C, E, OUT], app_database: ACID | None) -> None:
         """Test framework for EzCRQS."""
         self.framework = framework
         self.app_database = app_database
 
         self.command: C | None = None
 
     def with_command(self, command: C) -> None:
```

### Comparing `ez_cqrs-2.2.0/ez_cqrs/utilities/cli.py` & `ez_cqrs-2.3.0/ez_cqrs/utilities/cli.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.2.0/requirements/dev.txt` & `ez_cqrs-2.3.0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.2.0/scripts/new_release.py` & `ez_cqrs-2.3.0/scripts/new_release.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.2.0/tests/conftest.py` & `ez_cqrs-2.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.2.0/tests/test_acid_exec.py` & `ez_cqrs-2.3.0/tests/test_acid_exec.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.2.0/tests/test_framework.py` & `ez_cqrs-2.3.0/tests/test_framework.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,16 +58,19 @@
 
 @dataclass(frozen=True)
 class DepositMoneyOutput(UseCaseOutput):
     account_id: str
     amount: int
 
 
+BankAccountOutput: TypeAlias = Union[OpenAccountOutput, DepositMoneyOutput]
+
+
 class BankAccountCommandHandler(
-    CommandHandler[BankAccountCommand, BankAccountEvent],
+    CommandHandler[BankAccountCommand, BankAccountEvent, BankAccountOutput],
 ):
     def validate(
         self,
         command: BankAccountCommand,
     ) -> Result[None, ValidationError]:
         if isinstance(command, OpenAccount):
 
@@ -93,15 +96,15 @@
         assert_never(command)
 
     async def handle(
         self,
         command: BankAccountCommand,
         ops_registry: OpsRegistry[Any],
         event_registry: list[BankAccountEvent],
-    ) -> Result[UseCaseOutput, ExecutionError]:
+    ) -> Result[BankAccountOutput, ExecutionError]:
         _ = ops_registry
 
         if isinstance(command, OpenAccount):
             event_registry.append(
                 AccountOpened(
                     account_id=command.account_id,
                     amount=command.amount,
@@ -128,16 +131,20 @@
 class BankAccountEventDispatcher(EventDispatcher[BankAccountEvent]):
     async def dispatch(self, event: BankAccountEvent) -> None:
         _ = event
 
 
 async def test_execution_both_commands() -> None:
     """Test both commands execution."""
-    framework_tester = EzCQRSTester[BankAccountCommand, BankAccountEvent](
-        framework=EzCqrs[BankAccountCommand, BankAccountEvent](
+    framework_tester = EzCQRSTester[
+        BankAccountCommand,
+        BankAccountEvent,
+        BankAccountOutput,
+    ](
+        framework=EzCqrs[BankAccountCommand, BankAccountEvent, BankAccountOutput](
             cmd_handler=BankAccountCommandHandler(),
             event_dispatcher=BankAccountEventDispatcher(),
         ),
         app_database=None,
     )
     framework_tester.with_command(command=OpenAccount(account_id="123", amount=12))
     assert await framework_tester.expect(
```

### Comparing `ez_cqrs-2.2.0/.gitignore` & `ez_cqrs-2.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.2.0/LICENSE` & `ez_cqrs-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.2.0/pyproject.toml` & `ez_cqrs-2.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ez_cqrs"
-version = "2.2.0"
+version = "2.3.0"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 authors = [
```

### Comparing `ez_cqrs-2.2.0/PKG-INFO` & `ez_cqrs-2.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez_cqrs
-Version: 2.2.0
+Version: 2.3.0
 Project-URL: Documentation, https://github.com/Tomperez98/ez-cqrs#readme
 Project-URL: Issues, https://github.com/Tomperez98/ez-cqrs/issues
 Project-URL: Source, https://github.com/Tomperez98/ez-cqrs
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

