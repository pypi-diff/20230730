# Comparing `tmp/litechain-0.1.5.tar.gz` & `tmp/litechain-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litechain-0.1.5.tar", last modified: Tue Jul 25 20:29:30 2023, max compression
+gzip compressed data, was "litechain-0.1.6.tar", last modified: Sun Jul 30 05:55:08 2023, max compression
```

## Comparing `litechain-0.1.5.tar` & `litechain-0.1.6.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:29:30.534257 litechain-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-25 20:29:19.000000 litechain-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-25 20:29:19.000000 litechain-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-07-25 20:29:30.534257 litechain-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-07-25 20:29:19.000000 litechain-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:29:30.534257 litechain-0.1.5/litechain/
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-07-25 20:29:19.000000 litechain-0.1.5/litechain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:29:30.534257 litechain-0.1.5/litechain/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-25 20:29:19.000000 litechain-0.1.5/litechain/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:29:30.534257 litechain-0.1.5/litechain/contrib/llms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 20:29:19.000000 litechain-0.1.5/litechain/contrib/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-07-25 20:29:19.000000 litechain-0.1.5/litechain/contrib/llms/gpt4all_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-07-25 20:29:19.000000 litechain-0.1.5/litechain/contrib/llms/open_ai.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:29:30.534257 litechain-0.1.5/litechain/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 20:29:19.000000 litechain-0.1.5/litechain/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23686 2023-07-25 20:29:19.000000 litechain-0.1.5/litechain/core/chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:29:30.534257 litechain-0.1.5/litechain/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 20:29:19.000000 litechain-0.1.5/litechain/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-25 20:29:19.000000 litechain-0.1.5/litechain/utils/async_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-07-25 20:29:19.000000 litechain-0.1.5/litechain/utils/chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:29:30.534257 litechain-0.1.5/litechain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-07-25 20:29:30.000000 litechain-0.1.5/litechain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-25 20:29:30.000000 litechain-0.1.5/litechain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 20:29:30.000000 litechain-0.1.5/litechain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-25 20:29:30.000000 litechain-0.1.5/litechain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-25 20:29:30.000000 litechain-0.1.5/litechain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-25 20:29:19.000000 litechain-0.1.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 20:29:30.534257 litechain-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-25 20:29:19.000000 litechain-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:29:30.534257 litechain-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 20:29:19.000000 litechain-0.1.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:55:08.751570 litechain-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-30 05:54:53.000000 litechain-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-30 05:54:53.000000 litechain-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-07-30 05:55:08.747570 litechain-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-07-30 05:54:53.000000 litechain-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:55:08.747570 litechain-0.1.6/litechain/
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-07-30 05:54:53.000000 litechain-0.1.6/litechain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:55:08.747570 litechain-0.1.6/litechain/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-30 05:54:53.000000 litechain-0.1.6/litechain/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:55:08.747570 litechain-0.1.6/litechain/contrib/llms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 05:54:53.000000 litechain-0.1.6/litechain/contrib/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-07-30 05:54:53.000000 litechain-0.1.6/litechain/contrib/llms/gpt4all_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-07-30 05:54:53.000000 litechain-0.1.6/litechain/contrib/llms/open_ai.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:55:08.747570 litechain-0.1.6/litechain/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 05:54:53.000000 litechain-0.1.6/litechain/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30343 2023-07-30 05:54:53.000000 litechain-0.1.6/litechain/core/chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:55:08.747570 litechain-0.1.6/litechain/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 05:54:53.000000 litechain-0.1.6/litechain/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-30 05:54:53.000000 litechain-0.1.6/litechain/utils/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-07-30 05:54:53.000000 litechain-0.1.6/litechain/utils/async_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-07-30 05:54:53.000000 litechain-0.1.6/litechain/utils/chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:55:08.747570 litechain-0.1.6/litechain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-07-30 05:55:08.000000 litechain-0.1.6/litechain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-30 05:55:08.000000 litechain-0.1.6/litechain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 05:55:08.000000 litechain-0.1.6/litechain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-30 05:55:08.000000 litechain-0.1.6/litechain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-30 05:55:08.000000 litechain-0.1.6/litechain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-30 05:54:53.000000 litechain-0.1.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 05:55:08.751570 litechain-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-30 05:54:53.000000 litechain-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:55:08.747570 litechain-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 05:54:53.000000 litechain-0.1.6/tests/__init__.py
```

### Comparing `litechain-0.1.5/LICENSE` & `litechain-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `litechain-0.1.5/PKG-INFO` & `litechain-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litechain
-Version: 0.1.5
+Version: 0.1.6
 Summary: Build robust LLM applications with true composability 🔗
 Home-page: https://github.com/rogeriochaves/litechain
 Author: Rogerio Chaves
 Author-email: rogeriocfj@gmail.com
 License: MIT
 Project-URL: Documentation, https://rogeriochaves.github.io/litechain/
 Project-URL: Source Code, https://github.com/rogeriochaves/litechain
```

### Comparing `litechain-0.1.5/README.md` & `litechain-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `litechain-0.1.5/litechain/__init__.py` & `litechain-0.1.6/litechain/__init__.py`

 * *Files identical despite different names*

### Comparing `litechain-0.1.5/litechain/contrib/__init__.py` & `litechain-0.1.6/litechain/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `litechain-0.1.5/litechain/contrib/llms/gpt4all_chain.py` & `litechain-0.1.6/litechain/contrib/llms/gpt4all_chain.py`

 * *Files identical despite different names*

### Comparing `litechain-0.1.5/litechain/contrib/llms/open_ai.py` & `litechain-0.1.6/litechain/contrib/llms/open_ai.py`

 * *Files identical despite different names*

### Comparing `litechain-0.1.5/litechain/core/chain.py` & `litechain-0.1.6/litechain/core/chain.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,18 @@
     Optional,
     Tuple,
     TypeVar,
     Union,
     cast,
 )
 
-from litechain.utils.async_generator import as_async_generator
+import asyncstdlib
+
+from litechain.utils.async_generator import as_async_generator, merge
+from litechain.utils._typing import unwrap
 
 T = TypeVar("T")
 U = TypeVar("U")
 V = TypeVar("V")
 W = TypeVar("W")
 X = TypeVar("X")
 
@@ -90,21 +93,22 @@
     def __call__(self, input: T) -> AsyncGenerator[ChainOutput[U], Any]:
         result = self._call(input)
         return self._wrap(result)
 
     def _wrap(
         self,
         value: Union[AsyncGenerator[ChainOutput[V], Any], AsyncGenerator[V, Any], V],
+        final: Optional[bool] = None,
         name: Optional[str] = None,
     ) -> AsyncGenerator[ChainOutput[V], Any]:
         async def _wrap(
             values: Union[AsyncGenerator[ChainOutput[V], Any], AsyncGenerator[V, Any]],
         ) -> AsyncGenerator[ChainOutput[V], Any]:
             async for value in values:
-                yield self._output_wrap(value, name=name)
+                yield self._output_wrap(value, final=final, name=name)
 
         if isinstance(value, AsyncGenerator):
             return _wrap(value)
         return _wrap(as_async_generator(value))
 
     def _output_wrap(
         self, value: Union[ChainOutput[V], V], final=None, name=None
@@ -173,14 +177,49 @@
                 yield cast(ChainOutput[V], to_reyield)
                 if len(values) > prev_len_values:  # as soon as there is a new value
                     prev_len_values = len(values)
                     yield self._output_wrap(fn(values[-1]), name=next_name)
 
         return Chain[T, V](next_name, lambda input: map(input))
 
+    def filter(self, fn: Callable[[U], bool]) -> "Chain[T, U]":
+        """
+        Filters the output of the current chain, keeping only the values that return True.
+
+        This method is non-blocking and expects a function that returns True for keeping the value,
+        or False for dropping it, as they arrive.
+
+        Example:
+
+        >>> from litechain import Chain, as_async_generator, collect_final_output
+        >>> import asyncio
+        ...
+        >>> async def example():
+        ...     numbers_chain = Chain[int, int]("NumbersChain", lambda input: as_async_generator(*range(0, input)))
+        ...     even_chain = numbers_chain.filter(lambda input: input % 2 == 0)
+        ...     return await collect_final_output(even_chain(9))
+        ...
+        >>> asyncio.run(example())
+        [0, 2, 4, 6, 8]
+        """
+
+        next_name = f"{self.name}@filter"
+
+        async def filter(input: T) -> AsyncGenerator[ChainOutput[U], Any]:
+            # Reyield previous chain so we never block the stream, and at the same time yield mapped values
+            prev_len_values = 0
+            async for values, to_reyield in self._reyield(self(input)):
+                yield to_reyield
+                if len(values) > prev_len_values:  # as soon as there is a new value
+                    prev_len_values = len(values)
+                    if fn(values[-1]):
+                        yield self._output_wrap(values[-1], name=next_name)
+
+        return Chain[T, U](next_name, lambda input: filter(input))
+
     def and_then(
         self,
         next: Callable[
             [Iterable[U]],
             Union[AsyncGenerator[ChainOutput[V], Any], AsyncGenerator[V, Any], V],
         ],
     ) -> "Chain[T, V]":
@@ -240,14 +279,89 @@
             # Then, call in the next chain
             iter_v = self._wrap(next(iter_u), name=next_name)
             async for v in iter_v:
                 yield v
 
         return Chain[T, V](next_name, and_then)
 
+    def pipe(
+        self,
+        fn: Callable[
+            [AsyncGenerator[U, Any]], AsyncGenerator[Union[ChainOutput[V], V], Any]
+        ],
+    ) -> "Chain[T, V]":
+        """
+        Lower level constructor to pipe a chain into another one, giving you the underlying AsyncGenerator.
+        Pipe takes a callback function which should always produce an AsyncGenerator in return, which means you
+        need to declare an async function and your function needs to use `yield` for generating values, the advantage
+        of that is that you have fine control on whether it will be blocking the stream or not.
+
+        In fact, with pipe you can reconstruct `map` and `and_then`, for example:
+
+        >>> from litechain import Chain, as_async_generator, collect_final_output
+        >>> from typing import List, AsyncGenerator
+        >>> import asyncio
+        ...
+        >>> async def example(items):
+        ...     async def mario_pipe(stream: AsyncGenerator[str, None]) -> AsyncGenerator[str, None]:
+        ...        waiting_for_mushroom = False
+        ...        async for item in stream:
+        ...            if item == "Mario":
+        ...                waiting_for_mushroom = True
+        ...            elif item == "Mushroom" and waiting_for_mushroom:
+        ...                yield "Super Mario!"
+        ...            else:
+        ...                yield item + "?"
+        ...
+        ...     piped_chain = Chain[List[str], str](
+        ...         "PipedChain", lambda items: as_async_generator(*items)
+        ...     ).pipe(mario_pipe)
+        ...
+        ...     return await collect_final_output(piped_chain(items))
+        ...
+        >>> asyncio.run(example(["Mario", "Mushroom"]))
+        ['Super Mario!']
+        >>> asyncio.run(example(["Luigi"]))
+        ['Luigi?']
+        >>> asyncio.run(example(["Mario", "Luigi", "Mushroom"]))
+        ['Luigi?', 'Super Mario!']
+
+        As you can see this pipe blocks kinda like `and_then` when it sees "Mario", until a mushroom arrives, but for other random items
+        such as "Luigi" it just re-yields it immediately, adding a question mark, non-blocking, like `map`.
+
+        You can also call another chain from `pipe` directly, just be sure to re-yield its outputs
+        """
+
+        next_name = f"{self.name}@pipe"
+
+        async def filter_final_output(
+            async_iterable: AsyncGenerator[ChainOutput[U], Any]
+        ) -> AsyncGenerator[U, Any]:
+            async for output in async_iterable:
+                if output.final:
+                    yield cast(U, output.data)
+
+        def pipe(input: T) -> AsyncGenerator[ChainOutput[V], Any]:
+            previous, final = asyncstdlib.tee(self(input), n=2, lock=asyncio.Lock())
+
+            previous = self._wrap(previous, name=next_name, final=False)
+            previous = cast(AsyncGenerator[ChainOutput[V], Any], previous)
+
+            final = filter_final_output(
+                cast(AsyncGenerator[ChainOutput[U], Any], final)
+            )
+            final = cast(
+                AsyncGenerator[ChainOutput[V], Any],
+                self._wrap(fn(final), name=next_name),
+            )
+
+            return merge(previous, final)
+
+        return Chain[T, V](next_name, pipe)
+
     def collect(self: "Chain[T, U]") -> "SingleOutputChain[T, List[U]]":
         """
         Collects all the outputs produced by the chain and returns them as a list.
 
         This method is blocking useful when the next chain or processing step needs to have access to the
         entire output all at once, rather than processing elements as they arrive.
 
@@ -317,15 +431,15 @@
 
         async def _join(
             input: T,
         ) -> AsyncGenerator[ChainOutput[str], Any]:
             # First, reyield previous chain so we never block the stream, and collect the results until they are done
             iter_u: Iterable[str] = []
             async for values, to_reyield in self._reyield(self(input)):
-                yield cast(ChainOutput[str], to_reyield)
+                yield to_reyield
                 iter_u = values
 
             # Then, return the joined result
             output: str = separator.join(iter_u)
             yield self._output_wrap(output, name=next_name)
 
         return SingleOutputChain[T, str](next_name, _join)
@@ -423,25 +537,20 @@
     """"""
 
     _call: Callable[
         [T], Union[AsyncGenerator[ChainOutput[U], Any], AsyncGenerator[U, Any], U]
     ]
 
     async def _reyield(
-        self, async_iterable: AsyncGenerator[ChainOutput[U], Any], at: str
+        self, async_iterable: AsyncGenerator[ChainOutput[U], Any]
     ) -> AsyncGenerator[Tuple[Optional[U], ChainOutput[U]], Any]:
         final_value: Optional[U] = None
         async for u in async_iterable:
             u_rewrapped = self._output_wrap(u, final=False)
             if u.final:
-                if final_value is not None:
-                    # TODO: try to make this happen with a bad use case, is it even breakable?
-                    raise Exception(
-                        f"Expected a single item at the end of SingleOutputChain, found multiple for {self.name}@{at}"
-                    )
                 final_value = u.data
             yield (final_value, u_rewrapped)
 
     def map(self, fn: Callable[[U], V]) -> "SingleOutputChain[T, V]":
         """
         Similar to `Chain.map`, this method applies a function to the final output of the chain, but returns a SingleOutputChain.
 
@@ -451,27 +560,59 @@
         """
 
         next_name = f"{self.name}@map"
 
         async def map(input: T) -> AsyncGenerator[ChainOutput[V], Any]:
             # Reyield previous chain so we never block the stream, and at the same time yield mapped values
             final_u: Optional[U] = None
-            async for value, to_reyield in self._reyield(self(input), "map"):
+            async for value, to_reyield in self._reyield(self(input)):
                 yield cast(ChainOutput[V], to_reyield)
                 final_u = value
 
-            if final_u is None:
-                # TODO: try to make this happen with a bad use case, is it even breakable?
-                raise Exception(
-                    f"Expected item at the end of the chain, found None for {self.name}@map"
-                )
-            yield self._output_wrap(fn(final_u), name=next_name)
+            yield self._output_wrap(fn(unwrap(final_u)), name=next_name)
 
         return SingleOutputChain[T, V](next_name, lambda input: map(input))
 
+    def filter(self, fn: Callable[[U], bool]) -> "SingleOutputChain[T, Union[U, None]]":
+        """
+        Similar to `Chain.filter`, however, singe SingleOutputChain must always produce a value, this method simply replaces
+        the value with a None if the filter function returns False
+
+        The `fn` parameter is a function that takes a value of type U and returns a bool.
+
+        Example:
+
+        >>> from litechain import Chain, as_async_generator, collect_final_output
+        >>> import asyncio
+        ...
+        >>> async def example():
+        ...     numbers_chain = Chain[int, int]("NumbersChain", lambda input: as_async_generator(*range(0, input)))
+        ...     even_chain = numbers_chain.collect().filter(lambda numbers: all([n % 2 == 0 for n in numbers]))
+        ...     return await collect_final_output(even_chain(9))
+        ...
+        >>> asyncio.run(example())
+        [None]
+        """
+        next_name = f"{self.name}@filter"
+
+        async def filter(input: T) -> AsyncGenerator[ChainOutput[Union[U, None]], Any]:
+            # Reyield previous chain so we never block the stream, and at the same time yield filtered values
+            final_u: Optional[U] = None
+            async for value, to_reyield in self._reyield(self(input)):
+                yield cast(ChainOutput[Union[U, None]], to_reyield)
+                final_u = value
+
+            yield self._output_wrap(
+                final_u if fn(unwrap(final_u)) else None, name=next_name
+            )
+
+        return SingleOutputChain[T, Union[U, None]](
+            next_name, lambda input: filter(input)
+        )
+
     def and_then(
         self,
         next: Callable[
             [U],
             Union[AsyncGenerator[ChainOutput[V], Any], AsyncGenerator[V, Any], V],
         ],
     ) -> "Chain[T, V]":
@@ -485,31 +626,57 @@
             next_name = next.name
 
         async def and_then(
             input: T,
         ) -> AsyncGenerator[ChainOutput[V], Any]:
             # First, reyield previous chain so we never block the stream, and collect the last result when it is done
             final_u: Optional[U] = None
-            async for value, to_reyield in self._reyield(self(input), "and_then"):
+            async for value, to_reyield in self._reyield(self(input)):
                 yield cast(ChainOutput[V], to_reyield)
                 final_u = value
 
-            if final_u is None:
-                # TODO: try to make this happen with a bad use case, is it even breakable?
-                raise Exception(
-                    f"Expected item at the end of the chain, found None for {self.name}@and_then"
-                )
-
             # Then, call in the next chain
-            iter_v = self._wrap(next(final_u), name=next_name)
+            iter_v = self._wrap(next(unwrap(final_u)), name=next_name)
             async for v in iter_v:
                 yield v
 
         return Chain[T, V](next_name, and_then)
 
+    def pipe(
+        self,
+        fn: Callable[
+            [AsyncGenerator[U, Any]], AsyncGenerator[Union[ChainOutput[V], V], Any]
+        ],
+    ) -> "Chain[T, V]":
+        """
+        Similar to `Chain.pipe`, except that it takes a stream that will only even produce a single value, so it effectively works basically the same as `and_then`, only with a different interface.
+
+        For detailed examples, refer to the documentation of `Chain.pipe`.
+        """
+        next_name = f"{self.name}@pipe"
+        if hasattr(next, "name"):
+            next_name = next.name
+
+        async def pipe(
+            input: T,
+        ) -> AsyncGenerator[ChainOutput[V], Any]:
+            # First, reyield previous chain so we never block the stream, and collect the last result when it is done
+            final_u: Optional[U] = None
+            async for value, to_reyield in self._reyield(self(input)):
+                yield cast(ChainOutput[V], to_reyield)
+                final_u = value
+
+            # Then, call in the piping function
+            single_item_stream = as_async_generator(unwrap(final_u))
+            iter_v = self._wrap(fn(single_item_stream), name=next_name)
+            async for v in iter_v:
+                yield cast(ChainOutput[V], v)
+
+        return Chain[T, V](next_name, pipe)
+
     def gather(
         self: "Union[SingleOutputChain[T, List[AsyncGenerator[ChainOutput[V], Any]]], SingleOutputChain[T, List[AsyncGenerator[V, Any]]]]",
     ) -> "SingleOutputChain[T, List[List[V]]]":
         """
         Similar to `Chain.gather`, this method waits for all the async generators in the list returned by the chain to finish and gathers their results in a list.
 
         For detailed examples, refer to the documentation of `Chain.gather`.
@@ -525,25 +692,20 @@
                 Union[
                     List[AsyncGenerator[ChainOutput[V], Any]],
                     List[AsyncGenerator[V, Any]],
                 ]
             ] = None
 
             # TODO: try to work out why the type signature of self(input) is not fitting in there, it should
-            async for value, to_reyield in self._reyield(
-                cast(Any, self(input)), "gather"
-            ):
+            async for value, to_reyield in self._reyield(cast(Any, self(input))):
                 yield cast(ChainOutput[List[List[V]]], to_reyield)
                 final_u = value
 
             if final_u is None:
-                # TODO: try to make this happen with a bad use case, is it even breakable?
-                raise Exception(
-                    f"Expected item at the end of the chain, found None for {self.name}@gather"
-                )
+                final_u = []
 
             async def consume_async_generator(
                 generator: AsyncGenerator[X, Any],
             ) -> Iterable[X]:
                 return [item async for item in generator]
 
             # TODO: should we really wait for everything to arrive before calling asyncio gather? Can we call it during the previous reyield?
```

### Comparing `litechain-0.1.5/litechain/utils/chain.py` & `litechain-0.1.6/litechain/utils/chain.py`

 * *Files identical despite different names*

### Comparing `litechain-0.1.5/litechain.egg-info/PKG-INFO` & `litechain-0.1.6/litechain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litechain
-Version: 0.1.5
+Version: 0.1.6
 Summary: Build robust LLM applications with true composability 🔗
 Home-page: https://github.com/rogeriochaves/litechain
 Author: Rogerio Chaves
 Author-email: rogeriocfj@gmail.com
 License: MIT
 Project-URL: Documentation, https://rogeriochaves.github.io/litechain/
 Project-URL: Source Code, https://github.com/rogeriochaves/litechain
```

### Comparing `litechain-0.1.5/litechain.egg-info/SOURCES.txt` & `litechain-0.1.6/litechain.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -12,10 +12,11 @@
 litechain/contrib/__init__.py
 litechain/contrib/llms/__init__.py
 litechain/contrib/llms/gpt4all_chain.py
 litechain/contrib/llms/open_ai.py
 litechain/core/__init__.py
 litechain/core/chain.py
 litechain/utils/__init__.py
+litechain/utils/_typing.py
 litechain/utils/async_generator.py
 litechain/utils/chain.py
 tests/__init__.py
```

### Comparing `litechain-0.1.5/setup.py` & `litechain-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="litechain",
-    version="0.1.5",
+    version="0.1.6",
     packages=find_packages(),
     install_requires=requirements,
     author="Rogerio Chaves",
     author_email="rogeriocfj@gmail.com",
     description="Build robust LLM applications with true composability 🔗",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

