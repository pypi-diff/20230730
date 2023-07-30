# Comparing `tmp/async_wrapper-0.2.2.tar.gz` & `tmp/async_wrapper-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_wrapper-0.2.2.tar", max compression
+gzip compressed data, was "async_wrapper-0.3.1.tar", max compression
```

## Comparing `async_wrapper-0.2.2.tar` & `async_wrapper-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     1070 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/LICENSE
--rw-r--r--   0        0        0     1823 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/README.md
--rw-r--r--   0        0        0     3565 2023-07-29 21:39:45.196393 async_wrapper-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      419 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/__init__.py
--rw-r--r--   0        0        0       63 2023-07-29 21:39:45.244394 async_wrapper-0.2.2/src/async_wrapper/_version.py
--rw-r--r--   0        0        0      157 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/convert/__init__.py
--rw-r--r--   0        0        0      109 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/convert/asynclib/__init__.py
--rw-r--r--   0        0        0     1007 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/convert/asynclib/_loky.py
--rw-r--r--   0        0        0      564 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/convert/asynclib/_thread.py
--rw-r--r--   0        0        0      409 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/convert/asynclib/base.py
--rw-r--r--   0        0        0      654 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/convert/asynclib/main.py
--rw-r--r--   0        0        0     1721 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/convert/main.py
--rw-r--r--   0        0        0      107 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/convert/synclib/__init__.py
--rw-r--r--   0        0        0      983 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/convert/synclib/_loky.py
--rw-r--r--   0        0        0     1140 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/convert/synclib/_thread.py
--rw-r--r--   0        0        0     1136 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/convert/synclib/base.py
--rw-r--r--   0        0        0      656 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/convert/synclib/main.py
--rw-r--r--   0        0        0        0 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/py.typed
--rw-r--r--   0        0        0      209 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/task_group/__init__.py
--rw-r--r--   0        0        0     3707 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/task_group/_anyio.py
--rw-r--r--   0        0        0     9566 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/task_group/base.py
--rw-r--r--   0        0        0     1735 2023-07-29 21:39:26.648053 async_wrapper-0.2.2/src/async_wrapper/task_group/main.py
--rw-r--r--   0        0        0     2810 1970-01-01 00:00:00.000000 async_wrapper-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-30 15:57:49.562929 async_wrapper-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1776 2023-07-30 15:57:49.562929 async_wrapper-0.3.1/README.md
+-rw-r--r--   0        0        0     3535 2023-07-30 15:58:01.571217 async_wrapper-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      288 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/__init__.py
+-rw-r--r--   0        0        0       63 2023-07-30 15:58:01.607218 async_wrapper-0.3.1/src/async_wrapper/_version.py
+-rw-r--r--   0        0        0      157 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/convert/__init__.py
+-rw-r--r--   0        0        0      109 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/convert/asynclib/__init__.py
+-rw-r--r--   0        0        0     1007 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/convert/asynclib/_loky.py
+-rw-r--r--   0        0        0      564 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/convert/asynclib/_thread.py
+-rw-r--r--   0        0        0      409 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/convert/asynclib/base.py
+-rw-r--r--   0        0        0      654 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/convert/asynclib/main.py
+-rw-r--r--   0        0        0     1721 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/convert/main.py
+-rw-r--r--   0        0        0      107 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/convert/synclib/__init__.py
+-rw-r--r--   0        0        0      983 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/convert/synclib/_loky.py
+-rw-r--r--   0        0        0     1140 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/convert/synclib/_thread.py
+-rw-r--r--   0        0        0     1136 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/convert/synclib/base.py
+-rw-r--r--   0        0        0      656 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/convert/synclib/main.py
+-rw-r--r--   0        0        0        0 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/py.typed
+-rw-r--r--   0        0        0      188 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/task_group/__init__.py
+-rw-r--r--   0        0        0      104 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/task_group/exception.py
+-rw-r--r--   0        0        0     8414 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/task_group/future.py
+-rw-r--r--   0        0        0     5004 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/task_group/task_group.py
+-rw-r--r--   0        0        0     2505 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/task_group/value.py
+-rw-r--r--   0        0        0     2763 1970-01-01 00:00:00.000000 async_wrapper-0.3.1/PKG-INFO
```

### Comparing `async_wrapper-0.2.2/LICENSE` & `async_wrapper-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.2.2/pyproject.toml` & `async_wrapper-0.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async-wrapper"
-version = "0.2.2"
+version = "0.3.1"
 description = "async wrapper"
 authors = ["phi <phi.friday@gmail.com>"]
 readme = "README.md"
 license = "MIT License"
 homepage = "https://github.com/phi-friday/async-wrapper"
 repository = "https://github.com/phi-friday/async-wrapper"
 packages = [{ include = "async_wrapper", from = 'src' }]
@@ -112,12 +112,10 @@
 ]
 
 [tool.ruff.isort]
 known-local-folder = ["async_wrapper"]
 required-imports = ["from __future__ import annotations"]
 
 [tool.pyright]
-venvPath = "."
-venv = '.venv'
 pythonVersion = '3.8'
 pythonPlatform = 'Linux'
 diagnostic = 'basic'
```

### Comparing `async_wrapper-0.2.2/src/async_wrapper/convert/asynclib/_loky.py` & `async_wrapper-0.3.1/src/async_wrapper/convert/asynclib/_loky.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.2.2/src/async_wrapper/convert/asynclib/_thread.py` & `async_wrapper-0.3.1/src/async_wrapper/convert/asynclib/_thread.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.2.2/src/async_wrapper/convert/asynclib/main.py` & `async_wrapper-0.3.1/src/async_wrapper/convert/asynclib/main.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.2.2/src/async_wrapper/convert/main.py` & `async_wrapper-0.3.1/src/async_wrapper/convert/main.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.2.2/src/async_wrapper/convert/synclib/_loky.py` & `async_wrapper-0.3.1/src/async_wrapper/convert/synclib/_loky.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.2.2/src/async_wrapper/convert/synclib/_thread.py` & `async_wrapper-0.3.1/src/async_wrapper/convert/synclib/_thread.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.2.2/src/async_wrapper/convert/synclib/base.py` & `async_wrapper-0.3.1/src/async_wrapper/convert/synclib/base.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.2.2/src/async_wrapper/convert/synclib/main.py` & `async_wrapper-0.3.1/src/async_wrapper/convert/synclib/main.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.2.2/src/async_wrapper/task_group/_anyio.py` & `async_wrapper-0.3.1/src/async_wrapper/task_group/task_group.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,145 +1,178 @@
 from __future__ import annotations
 
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Awaitable,
-    Callable,
-    Coroutine,
-    Generic,
-    TypeVar,
-    final,
-)
+from functools import partial, wraps
+from typing import TYPE_CHECKING, Any, Awaitable, Callable, Coroutine, Generic, TypeVar
 from weakref import WeakSet
 
-from anyio import Semaphore as _Semaphore
-from anyio import create_task_group
+from anyio.abc import TaskGroup as _TaskGroup
 from typing_extensions import ParamSpec, Self, override
 
-from async_wrapper.task_group.base import (
-    BaseSoonWrapper,
-    BaseTaskGroup,
-    Future,
-    Semaphore,
-    SoonValue,
-)
+from async_wrapper.task_group.future import Future
+from async_wrapper.task_group.value import SoonValue
 
 if TYPE_CHECKING:
     from types import TracebackType
 
-    from anyio.abc import Semaphore as AnyioSemaphore  # type: ignore
-    from anyio.abc import TaskGroup as _TaskGroup
+    from anyio.abc import CancelScope, Semaphore
 
 
-ValueT = TypeVar("ValueT")
 ValueT_co = TypeVar("ValueT_co", covariant=True)
 OtherValueT_co = TypeVar("OtherValueT_co", covariant=True)
 ParamT = ParamSpec("ParamT")
 OtherParamT = ParamSpec("OtherParamT")
 
-__all__ = ["SoonWrapper", "wrap_soon", "get_task_group", "get_semaphore_class"]
 
-
-class CancelError(Exception):
-    ...
-
-
-class TaskGroup(BaseTaskGroup):
-    def __init__(self) -> None:
-        self._task_group: _TaskGroup = create_task_group()
+class TaskGroupWrapper(_TaskGroup):
+    def __init__(self, task_group: _TaskGroup) -> None:
+        self._task_group = task_group
         self._futures: WeakSet[Future[Any]] = WeakSet()
 
+    @property
+    def futures(self) -> WeakSet[Future[Any]]:
+        """futures using wrapper"""
+        return self._futures.copy()
+
+    @property
     @override
-    def start_soon(
-        self,
-        func: Callable[ParamT, Coroutine[Any, Any, ValueT_co]],
-        *args: ParamT.args,
-        **kwargs: ParamT.kwargs,
-    ) -> SoonValue[ValueT_co]:
-        value = SoonValue()
-        future = self._as_future(func, *args, **kwargs)
-        value._set_future(future)  # noqa: SLF001
-        self._task_group.start_soon(_as_coro, future)
-        return value
+    def cancel_scope(self) -> CancelScope:
+        return self._task_group.cancel_scope
 
-    def _as_future(
+    @override
+    async def spawn(
         self,
-        func: Callable[ParamT, Coroutine[Any, Any, ValueT_co]],
-        *args: ParamT.args,
-        **kwargs: ParamT.kwargs,
-    ) -> Future[ValueT_co]:
-        coro = func(*args, **kwargs)
-        future = Future(coro)
-        self._futures.add(future)
-        return future
+        func: Callable[..., Awaitable[Any]],
+        *args: Any,
+        name: Any = None,
+    ) -> None:
+        raise NotImplementedError
 
-    @property
     @override
-    def is_active(self) -> bool:
-        return self._task_group._active  # type: ignore # noqa: SLF001
+    def start_soon(
+        self,
+        func: Callable[..., Awaitable[Any]],
+        *args: Any,
+        name: Any = None,
+    ) -> None:
+        future = self._as_future(func, *args)
+        return self._task_group.start_soon(future, name=name)
 
-    @property
     @override
-    def tasks(self) -> WeakSet[Future[Any]]:
-        return self._futures
+    async def start(
+        self,
+        func: Callable[..., Awaitable[Any]],
+        *args: Any,
+        name: Any = None,
+    ) -> Any:
+        raise NotImplementedError
 
     @override
     async def __aenter__(self) -> Self:
         await self._task_group.__aenter__()
         return self
 
     @override
     async def __aexit__(
         self,
         exc_type: type[BaseException] | None,
-        exc: BaseException | None,
-        traceback: TracebackType | None,
-    ) -> Any:
-        tasks = tuple(self.tasks)
-        if tasks:
-            await self.wait(tasks)
-        return await self._task_group.__aexit__(exc_type, exc, traceback)
-
-
-@final
-class SoonWrapper(
-    BaseSoonWrapper[TaskGroup, ParamT, ValueT_co],
-    Generic[ParamT, ValueT_co],
-):
-    if TYPE_CHECKING:
-
-        @override
-        def __new__(
-            cls,
-            func: Callable[OtherParamT, Awaitable[OtherValueT_co]],
-            task_group: TaskGroup,
-            semaphore: Semaphore | None = None,
-        ) -> SoonWrapper[OtherParamT, OtherValueT_co]:
-            ...
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> bool | None:
+        return await self._task_group.__aexit__(exc_type, exc_val, exc_tb)
 
-    @override
-    def __call__(
+    def wrap(
+        self,
+        func: Callable[ParamT, Awaitable[ValueT_co]],
+        semaphore: Semaphore | None = None,
+    ) -> SoonWrapper[ParamT, ValueT_co]:
+        """wrap function to use in wrapper.
+
+        func will return soon value.
+
+        Args:
+            func: target func
+            semaphore: anyio semaphore. Defaults to None.
+
+        Returns:
+            wrapped func
+        """
+        return SoonWrapper(func, self, semaphore)
+
+    def _as_future(
+        self,
+        func: Callable[ParamT, Awaitable[ValueT_co]],
+        *args: ParamT.args,
+        **kwargs: ParamT.kwargs,
+    ) -> Future[ValueT_co]:
+        coro = _as_coro(func, *args, **kwargs)
+        future = Future(coro)
+        self._futures.add(future)
+        future.add_done_callback(partial(_remove_future, task_group=self))
+        return future
+
+
+class SoonWrapper(Generic[ParamT, ValueT_co]):
+    def __init__(
+        self,
+        func: Callable[ParamT, Awaitable[ValueT_co]],
+        task_group: _TaskGroup,
+        semaphore: Semaphore | None = None,
+    ) -> None:
+        self.func = func
+        self.task_group = task_group
+        self.semaphore = semaphore
+        self._wrapped = None
+
+    def __call__(  # noqa: D102
         self,
         *args: ParamT.args,
         **kwargs: ParamT.kwargs,
     ) -> SoonValue[ValueT_co]:
-        wrapped = self.task_group._wrap(self.func, self.semaphore)  # noqa: SLF001
-        return self.task_group.start_soon(wrapped, *args, **kwargs)
+        value: SoonValue[ValueT_co] = SoonValue()
+        coro = self.wrapped(*args, **kwargs)
+        future = Future(coro)
+        value._set_future(future)  # noqa: SLF001
+        self.task_group.start_soon(future)
+        return value
+
+    @property
+    def wrapped(self) -> Callable[ParamT, Coroutine[Any, Any, ValueT_co]]:
+        """wrapped func using semaphore"""
+        if self._wrapped is not None:
+            return self._wrapped
+
+        @wraps(self.func)
+        async def wrapped(*args: ParamT.args, **kwargs: ParamT.kwargs) -> ValueT_co:
+            if self.semaphore is None:
+                return await self.func(*args, **kwargs)
+            async with self.semaphore:
+                return await self.func(*args, **kwargs)
+
+        self._wrapped = wrapped
+        return wrapped
 
-    @override
     def copy(self, semaphore: Semaphore | None = None) -> Self:
+        """copy self.
+
+        Args:
+            semaphore: anyio semaphore.
+                Defaults to None.
+                if not None, overwrite.
+
+        Returns:
+            self
+        """
         if semaphore is None:
             semaphore = self.semaphore
         return SoonWrapper(self.func, self.task_group, semaphore)
 
 
-def get_semaphore_class() -> type[AnyioSemaphore]:
-    return _Semaphore
-
-
-async def _as_coro(future: Future[ValueT_co]) -> ValueT_co:
-    return await future
+async def _as_coro(
+    func: Callable[ParamT, Awaitable[ValueT_co]],
+    *args: ParamT.args,
+    **kwargs: ParamT.kwargs,
+) -> ValueT_co:
+    return await func(*args, **kwargs)
 
 
-wrap_soon = SoonWrapper
-get_task_group = TaskGroup
+def _remove_future(future: Future[Any], task_group: TaskGroupWrapper) -> None:
+    task_group._futures.remove(future)  # noqa: SLF001
```

### Comparing `async_wrapper-0.2.2/PKG-INFO` & `async_wrapper-0.3.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-wrapper
-Version: 0.2.2
+Version: 0.3.1
 Summary: async wrapper
 Home-page: https://github.com/phi-friday/async-wrapper
 License: MIT
 Author: phi
 Author-email: phi.friday@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -39,61 +39,61 @@
 $ pip install "async_wrapper[loky]"
 ```
 
 ## how to use
 ```python
 from __future__ import annotations
 
-import asyncio
 import time
 
-from async_wrapper import (
-    async_to_sync,
-    get_semaphore_class,
-    get_task_group_factory,
-    get_task_group_wrapper,
-)
+import anyio
+
+from async_wrapper import TaskGroupWrapper, async_to_sync
 
 
 @async_to_sync("thread")
 async def sample_func() -> int:
-    await asyncio.sleep(1)
+    await anyio.sleep(1)
     return 1
 
 
-result = sample_func()
-assert isinstance(result, int)
-assert result == 1
-
-
 async def sample_func_2(x: int) -> int:
-    await asyncio.sleep(1)
+    await anyio.sleep(1)
     return x
 
 
-async def main():
-    wrapper = get_task_group_wrapper()
-    factory = get_task_group_factory()
-    Semaphore = get_semaphore_class()
-    semaphore = Semaphore(2)
+def main():
+    result = sample_func()
+    assert isinstance(result, int)
+    assert result == 1
+
+
+async def async_main():
+    semaphore = anyio.Semaphore(2)
 
     start = time.perf_counter()
-    async with factory() as task_group:
-        wrapped = wrapper(sample_func_2, task_group, semaphore)
-        value_1 = wrapped(1)
-        value_2 = wrapped(2)
-        value_3 = wrapped(3)
+    async with anyio.create_task_group() as task_group:
+        wrapper = TaskGroupWrapper(task_group)
+        func = wrapper.wrap(sample_func_2, semaphore)
+        value_1 = func(1)
+        value_2 = func(2)
+        value_3 = func(3)
     end = time.perf_counter()
 
     assert isinstance(value_1.value, int)
     assert isinstance(value_2.value, int)
     assert isinstance(value_3.value, int)
     assert value_1.value == 1
     assert value_2.value == 2
     assert value_3.value == 3
     assert 1.5 < end - start < 2.5
+
+
+if __name__ == "__main__":
+    main()
+    anyio.run(async_main)
 ```
 
 ## License
 
 MIT, see [LICENSE](https://github.com/phi-friday/async-wrapper/blob/main/LICENSE).
```

