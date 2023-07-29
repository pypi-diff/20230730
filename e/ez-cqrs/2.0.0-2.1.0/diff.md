# Comparing `tmp/ez_cqrs-2.0.0.tar.gz` & `tmp/ez_cqrs-2.1.0.tar.gz`

## Comparing `ez_cqrs-2.0.0.tar` & `ez_cqrs-2.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/.tool-versions
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/mkdocs.yml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/.vscode/settings.json
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/ez_cqrs/__init__.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/ez_cqrs/acid_exec.py
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/ez_cqrs/components.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/ez_cqrs/error.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/ez_cqrs/handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/ez_cqrs/py.typed
--rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/ez_cqrs/framework/__init__.py
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/ez_cqrs/framework/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/ez_cqrs/utilities/__init__.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/ez_cqrs/utilities/cli.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/requirements/core.txt
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/requirements/dev.txt
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/scripts/new_release.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/tests/__init__.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/tests/conftest.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/tests/test_acid_exec.py
--rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/tests/test_framework.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/LICENSE
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/README.md
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 ez_cqrs-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/.tool-versions
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/mkdocs.yml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/.vscode/settings.json
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/ez_cqrs/__init__.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/ez_cqrs/acid_exec.py
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/ez_cqrs/components.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/ez_cqrs/error.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/ez_cqrs/handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/ez_cqrs/py.typed
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/ez_cqrs/framework/__init__.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/ez_cqrs/framework/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/ez_cqrs/utilities/__init__.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/ez_cqrs/utilities/cli.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/requirements/core.txt
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/requirements/dev.txt
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/scripts/new_release.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/tests/conftest.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/tests/test_acid_exec.py
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/tests/test_framework.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/LICENSE
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/README.md
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/PKG-INFO
```

### Comparing `ez_cqrs-2.0.0/.github/workflows/release.yml` & `ez_cqrs-2.1.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.0.0/.github/workflows/test.yml` & `ez_cqrs-2.1.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.0.0/.vscode/settings.json` & `ez_cqrs-2.1.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.0.0/ez_cqrs/acid_exec.py` & `ez_cqrs-2.1.0/ez_cqrs/acid_exec.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.0.0/ez_cqrs/components.py` & `ez_cqrs-2.1.0/ez_cqrs/components.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.0.0/ez_cqrs/error.py` & `ez_cqrs-2.1.0/ez_cqrs/error.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.0.0/ez_cqrs/handler.py` & `ez_cqrs-2.1.0/ez_cqrs/handler.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.0.0/ez_cqrs/framework/__init__.py` & `ez_cqrs-2.1.0/ez_cqrs/framework/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,29 +31,26 @@
     event_dispatcher: EventDispatcher[E]
 
     async def run(
         self,
         cmd: C,
         max_transactions: int,
         app_database: ACID | None,
-    ) -> Result[
-        tuple[UseCaseOutput, list[E]],
-        ExecutionError | pydantic.ValidationError,
-    ]:
+        event_registry: list[E],
+    ) -> Result[UseCaseOutput, ExecutionError | pydantic.ValidationError]:
         """
         Validate and execute command, then dispatch command events.
 
         Dispatched events are returned to the caller for client specific usage.
         """
         if max_transactions > 0 and not app_database:
             msg = "You are not setting a database to commit transactions"
             raise RuntimeError(msg)
 
         ops_registry = OpsRegistry[Any](max_lenght=max_transactions)
-        event_registry: list[E] = []
 
         validated_or_err = self.cmd_handler.validate(
             command=cmd,
         )
         if not isinstance(validated_or_err, Ok):
             return validated_or_err
 
@@ -84,8 +81,8 @@
 
         event_dispatch_tasks = (
             self.event_dispatcher.dispatch(x) for x in event_registry
         )
 
         asyncio.gather(*event_dispatch_tasks, return_exceptions=False)
 
-        return Ok((execution_result_or_err.unwrap(), event_registry))
+        return Ok(execution_result_or_err.unwrap())
```

### Comparing `ez_cqrs-2.0.0/ez_cqrs/framework/testing.py` & `ez_cqrs-2.1.0/ez_cqrs/framework/testing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """Testing framework for EzCQRS framework."""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Generic, final
 
+from result import Ok
+
 from ez_cqrs.components import C, E
+from ez_cqrs.error import DomainError
 
 if TYPE_CHECKING:
     from result import Result
 
     from ez_cqrs.acid_exec import ACID
     from ez_cqrs.components import UseCaseOutput
-    from ez_cqrs.error import DomainError
     from ez_cqrs.framework import EzCqrs
 
 
 NO_COMMAND_ERROR = "There's not command setted."
 CLEAR_ERROR = "Command already set. run `clear()`"
 NO_EXECUTION_ERROR = "Run execute before checking results."
 
@@ -41,19 +43,30 @@
         if self.command is None:
             raise RuntimeError(NO_COMMAND_ERROR)
         self.command = None
 
     async def expect(
         self,
         max_transactions: int,
-        expected: Result[tuple[UseCaseOutput, list[E]], DomainError],
+        expected_result: Result[UseCaseOutput, DomainError],
+        expected_events: list[E],
     ) -> bool:
         """Execute use case and expect a domain error."""
         if self.command is None:
             raise RuntimeError(NO_COMMAND_ERROR)
 
+        event_registry: list[E] = []
         use_case_result = await self.framework.run(
             cmd=self.command,
             max_transactions=max_transactions,
             app_database=self.app_database,
+            event_registry=event_registry,
+        )
+        if not isinstance(use_case_result, Ok):
+            error = use_case_result.err()
+            if not isinstance(error, DomainError):
+                msg = f"Encounter error is {error}"
+                raise RuntimeError(msg)
+
+        return all(
+            [use_case_result == expected_result, event_registry == expected_events],
         )
-        return use_case_result == expected
```

### Comparing `ez_cqrs-2.0.0/ez_cqrs/utilities/cli.py` & `ez_cqrs-2.1.0/ez_cqrs/utilities/cli.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.0.0/requirements/dev.txt` & `ez_cqrs-2.1.0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.0.0/scripts/new_release.py` & `ez_cqrs-2.1.0/scripts/new_release.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.0.0/tests/conftest.py` & `ez_cqrs-2.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.0.0/tests/test_acid_exec.py` & `ez_cqrs-2.1.0/tests/test_acid_exec.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.0.0/tests/test_framework.py` & `ez_cqrs-2.1.0/tests/test_framework.py`

 * *Files 3% similar despite different names*

```diff
@@ -138,25 +138,21 @@
             event_dispatcher=BankAccountEventDispatcher(),
         ),
         app_database=None,
     )
     framework_tester.with_command(command=OpenAccount(account_id="123", amount=12))
     assert await framework_tester.expect(
         max_transactions=0,
-        expected=Ok(
-            (
-                OpenAccountOutput(account_id="123"),
-                [AccountOpened(account_id="123", amount=12)],
-            ),
+        expected_result=Ok(
+            OpenAccountOutput(account_id="123"),
         ),
+        expected_events=[AccountOpened(account_id="123", amount=12)],
     )
     framework_tester.clear()
     framework_tester.with_command(command=DepositMoney(account_id="123", amount=20))
     assert await framework_tester.expect(
         max_transactions=0,
-        expected=Ok(
-            (
-                DepositMoneyOutput(account_id="123", amount=20),
-                [MoneyDeposited(account_id="123", amount=20)],
-            ),
+        expected_result=Ok(
+            DepositMoneyOutput(account_id="123", amount=20),
         ),
+        expected_events=[MoneyDeposited(account_id="123", amount=20)],
     )
```

### Comparing `ez_cqrs-2.0.0/.gitignore` & `ez_cqrs-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.0.0/LICENSE` & `ez_cqrs-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.0.0/pyproject.toml` & `ez_cqrs-2.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ez_cqrs"
-version = "2.0.0"
+version = "2.1.0"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 authors = [
```

### Comparing `ez_cqrs-2.0.0/PKG-INFO` & `ez_cqrs-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez_cqrs
-Version: 2.0.0
+Version: 2.1.0
 Project-URL: Documentation, https://github.com/Tomperez98/ez-cqrs#readme
 Project-URL: Issues, https://github.com/Tomperez98/ez-cqrs/issues
 Project-URL: Source, https://github.com/Tomperez98/ez-cqrs
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

