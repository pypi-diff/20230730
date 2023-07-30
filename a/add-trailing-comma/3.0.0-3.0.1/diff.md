# Comparing `tmp/add_trailing_comma-3.0.0.tar.gz` & `tmp/add_trailing_comma-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "add_trailing_comma-3.0.0.tar", last modified: Sat Jul  1 17:57:01 2023, max compression
+gzip compressed data, was "add_trailing_comma-3.0.1.tar", last modified: Sun Jul 30 21:11:29 2023, max compression
```

## Comparing `add_trailing_comma-3.0.0.tar` & `add_trailing_comma-3.0.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-01 17:57:01.880476 add_trailing_comma-3.0.0/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-07-01 17:56:56.000000 add_trailing_comma-3.0.0/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4669 2023-07-01 17:57:01.880476 add_trailing_comma-3.0.0/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4032 2023-07-01 17:57:01.000000 add_trailing_comma-3.0.0/README.md
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-01 17:57:01.880476 add_trailing_comma-3.0.0/add_trailing_comma/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-07-01 17:56:56.000000 add_trailing_comma-3.0.0/add_trailing_comma/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      135 2023-07-01 17:56:56.000000 add_trailing_comma-3.0.0/add_trailing_comma/__main__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      733 2023-07-01 17:56:56.000000 add_trailing_comma-3.0.0/add_trailing_comma/_ast_helpers.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2126 2023-07-01 17:56:56.000000 add_trailing_comma-3.0.0/add_trailing_comma/_data.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2991 2023-07-01 17:56:56.000000 add_trailing_comma-3.0.0/add_trailing_comma/_main.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-01 17:57:01.880476 add_trailing_comma-3.0.0/add_trailing_comma/_plugins/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-07-01 17:56:56.000000 add_trailing_comma-3.0.0/add_trailing_comma/_plugins/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1129 2023-07-01 17:56:56.000000 add_trailing_comma-3.0.0/add_trailing_comma/_plugins/_with.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1582 2023-07-01 17:56:56.000000 add_trailing_comma-3.0.0/add_trailing_comma/_plugins/calls.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1254 2023-07-01 17:56:56.000000 add_trailing_comma-3.0.0/add_trailing_comma/_plugins/classes.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1384 2023-07-01 17:56:56.000000 add_trailing_comma-3.0.0/add_trailing_comma/_plugins/functions.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1256 2023-07-01 17:56:56.000000 add_trailing_comma-3.0.0/add_trailing_comma/_plugins/imports.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3058 2023-07-01 17:56:56.000000 add_trailing_comma-3.0.0/add_trailing_comma/_plugins/literals.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2451 2023-07-01 17:56:56.000000 add_trailing_comma-3.0.0/add_trailing_comma/_plugins/match.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6613 2023-07-01 17:56:56.000000 add_trailing_comma-3.0.0/add_trailing_comma/_token_helpers.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-01 17:57:01.880476 add_trailing_comma-3.0.0/add_trailing_comma.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4669 2023-07-01 17:57:01.000000 add_trailing_comma-3.0.0/add_trailing_comma.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      790 2023-07-01 17:57:01.000000 add_trailing_comma-3.0.0/add_trailing_comma.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-07-01 17:57:01.000000 add_trailing_comma-3.0.0/add_trailing_comma.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       69 2023-07-01 17:57:01.000000 add_trailing_comma-3.0.0/add_trailing_comma.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       19 2023-07-01 17:57:01.000000 add_trailing_comma-3.0.0/add_trailing_comma.egg-info/requires.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       19 2023-07-01 17:57:01.000000 add_trailing_comma-3.0.0/add_trailing_comma.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1233 2023-07-01 17:57:01.880476 add_trailing_comma-3.0.0/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-07-01 17:56:56.000000 add_trailing_comma-3.0.0/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-30 21:11:29.909244 add_trailing_comma-3.0.1/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-07-30 20:36:19.000000 add_trailing_comma-3.0.1/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3984 2023-07-30 21:11:29.909244 add_trailing_comma-3.0.1/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3347 2023-07-30 21:11:29.000000 add_trailing_comma-3.0.1/README.md
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-30 21:11:29.909244 add_trailing_comma-3.0.1/add_trailing_comma/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-07-30 20:36:19.000000 add_trailing_comma-3.0.1/add_trailing_comma/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      135 2023-07-30 20:36:19.000000 add_trailing_comma-3.0.1/add_trailing_comma/__main__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      733 2023-07-30 20:36:19.000000 add_trailing_comma-3.0.1/add_trailing_comma/_ast_helpers.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2126 2023-07-30 20:36:19.000000 add_trailing_comma-3.0.1/add_trailing_comma/_data.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3014 2023-07-30 21:11:29.000000 add_trailing_comma-3.0.1/add_trailing_comma/_main.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-30 21:11:29.909244 add_trailing_comma-3.0.1/add_trailing_comma/_plugins/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-07-30 20:36:19.000000 add_trailing_comma-3.0.1/add_trailing_comma/_plugins/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1129 2023-07-30 20:36:19.000000 add_trailing_comma-3.0.1/add_trailing_comma/_plugins/_with.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1582 2023-07-30 20:36:19.000000 add_trailing_comma-3.0.1/add_trailing_comma/_plugins/calls.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1254 2023-07-30 20:36:19.000000 add_trailing_comma-3.0.1/add_trailing_comma/_plugins/classes.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1384 2023-07-30 20:36:19.000000 add_trailing_comma-3.0.1/add_trailing_comma/_plugins/functions.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1256 2023-07-30 20:36:19.000000 add_trailing_comma-3.0.1/add_trailing_comma/_plugins/imports.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3058 2023-07-30 20:36:19.000000 add_trailing_comma-3.0.1/add_trailing_comma/_plugins/literals.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2451 2023-07-30 20:36:19.000000 add_trailing_comma-3.0.1/add_trailing_comma/_plugins/match.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     6865 2023-07-30 21:11:29.000000 add_trailing_comma-3.0.1/add_trailing_comma/_token_helpers.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-30 21:11:29.909244 add_trailing_comma-3.0.1/add_trailing_comma.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3984 2023-07-30 21:11:29.000000 add_trailing_comma-3.0.1/add_trailing_comma.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      790 2023-07-30 21:11:29.000000 add_trailing_comma-3.0.1/add_trailing_comma.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-07-30 21:11:29.000000 add_trailing_comma-3.0.1/add_trailing_comma.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       69 2023-07-30 21:11:29.000000 add_trailing_comma-3.0.1/add_trailing_comma.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       19 2023-07-30 21:11:29.000000 add_trailing_comma-3.0.1/add_trailing_comma.egg-info/requires.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       19 2023-07-30 21:11:29.000000 add_trailing_comma-3.0.1/add_trailing_comma.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1233 2023-07-30 21:11:29.909244 add_trailing_comma-3.0.1/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-07-30 20:36:19.000000 add_trailing_comma-3.0.1/setup.py
```

### Comparing `add_trailing_comma-3.0.0/LICENSE` & `add_trailing_comma-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-3.0.0/PKG-INFO` & `add_trailing_comma-3.0.1/add_trailing_comma.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: add_trailing_comma
-Version: 3.0.0
+Name: add-trailing-comma
+Version: 3.0.1
 Summary: Automatically add trailing commas to calls and literals
 Home-page: https://github.com/asottile/add-trailing-comma
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -34,15 +34,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/add-trailing-comma
-    rev: v3.0.0
+    rev: v3.0.1
     hooks:
     -   id: add-trailing-comma
 ```
 
 ## multi-line method invocation style -- why?
 
 ```python
@@ -98,32 +98,14 @@
  x(
      arg,
 -    arg
 +    arg,
  )
 ```
 
-### trailing commas for function calls with unpackings
-
-If `--py35-plus` is passed, `add-trailing-comma` will also perform the
-following change:
-
-```diff
- x(
--    *args
-+    *args,
- )
- y(
--    **kwargs
-+    **kwargs,
- )
-```
-
-Note that this would cause a **`SyntaxError`** in earlier python versions.
-
 ### trailing commas for tuple / list / dict / set literals
 
 ```diff
  x = [
 -    1, 2, 3
 +    1, 2, 3,
  ]
@@ -143,40 +125,14 @@
  async def func(
          arg1,
 -        arg2
 +        arg2,
  ):
 ```
 
-### trailing commas for function definitions with unpacking arguments
-
-If `--py36-plus` is passed, `add-trailing-comma` will also perform the
-following change:
-
-```diff
- def f(
--    *args
-+    *args,
- ): pass
-
-
- def g(
--    **kwargs
-+    **kwargs,
- ): pass
-
-
- def h(
--    *, kw=1
-+    *, kw=1,
- ): pass
-```
-
-Note that this would cause a **`SyntaxError`** in earlier python versions.
-
 ### trailing commas for `from` imports
 
 ```diff
  from os import (
      path,
 -    makedirs
 +    makedirs,
```

### Comparing `add_trailing_comma-3.0.0/README.md` & `add_trailing_comma-3.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: add_trailing_comma
+Version: 3.0.1
+Summary: Automatically add trailing commas to calls and literals
+Home-page: https://github.com/asottile/add-trailing-comma
+Author: Anthony Sottile
+Author-email: asottile@umich.edu
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![build status](https://github.com/asottile/add-trailing-comma/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/add-trailing-comma/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/add-trailing-comma/main.svg)](https://results.pre-commit.ci/latest/github/asottile/add-trailing-comma/main)
 
 add-trailing-comma
 ==================
 
 A tool (and pre-commit hook) to automatically add trailing commas to calls and
@@ -17,15 +34,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/add-trailing-comma
-    rev: v3.0.0
+    rev: v3.0.1
     hooks:
     -   id: add-trailing-comma
 ```
 
 ## multi-line method invocation style -- why?
 
 ```python
@@ -81,32 +98,14 @@
  x(
      arg,
 -    arg
 +    arg,
  )
 ```
 
-### trailing commas for function calls with unpackings
-
-If `--py35-plus` is passed, `add-trailing-comma` will also perform the
-following change:
-
-```diff
- x(
--    *args
-+    *args,
- )
- y(
--    **kwargs
-+    **kwargs,
- )
-```
-
-Note that this would cause a **`SyntaxError`** in earlier python versions.
-
 ### trailing commas for tuple / list / dict / set literals
 
 ```diff
  x = [
 -    1, 2, 3
 +    1, 2, 3,
  ]
@@ -126,40 +125,14 @@
  async def func(
          arg1,
 -        arg2
 +        arg2,
  ):
 ```
 
-### trailing commas for function definitions with unpacking arguments
-
-If `--py36-plus` is passed, `add-trailing-comma` will also perform the
-following change:
-
-```diff
- def f(
--    *args
-+    *args,
- ): pass
-
-
- def g(
--    **kwargs
-+    **kwargs,
- ): pass
-
-
- def h(
--    *, kw=1
-+    *, kw=1,
- ): pass
-```
-
-Note that this would cause a **`SyntaxError`** in earlier python versions.
-
 ### trailing commas for `from` imports
 
 ```diff
  from os import (
      path,
 -    makedirs
 +    makedirs,
```

### Comparing `add_trailing_comma-3.0.0/add_trailing_comma/_ast_helpers.py` & `add_trailing_comma-3.0.1/add_trailing_comma/_ast_helpers.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-3.0.0/add_trailing_comma/_data.py` & `add_trailing_comma-3.0.1/add_trailing_comma/_data.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-3.0.0/add_trailing_comma/_main.py` & `add_trailing_comma-3.0.1/add_trailing_comma/_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             continue
 
         # though this is a defaultdict, by using `.get()` this function's
         # self time is almost 50% faster
         for callback in callbacks.get(token.offset, ()):
             callback(i, tokens)
 
-        if token.src in START_BRACES:
+        if token.name == 'OP' and token.src in START_BRACES:
             fix_brace(
                 tokens, find_simple(i, tokens),
                 add_comma=False,
                 remove_comma=False,
             )
 
     return tokens_to_src(tokens)
```

### Comparing `add_trailing_comma-3.0.0/add_trailing_comma/_plugins/_with.py` & `add_trailing_comma-3.0.1/add_trailing_comma/_plugins/_with.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-3.0.0/add_trailing_comma/_plugins/calls.py` & `add_trailing_comma-3.0.1/add_trailing_comma/_plugins/calls.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-3.0.0/add_trailing_comma/_plugins/classes.py` & `add_trailing_comma-3.0.1/add_trailing_comma/_plugins/classes.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-3.0.0/add_trailing_comma/_plugins/functions.py` & `add_trailing_comma-3.0.1/add_trailing_comma/_plugins/functions.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-3.0.0/add_trailing_comma/_plugins/imports.py` & `add_trailing_comma-3.0.1/add_trailing_comma/_plugins/imports.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-3.0.0/add_trailing_comma/_plugins/literals.py` & `add_trailing_comma-3.0.1/add_trailing_comma/_plugins/literals.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-3.0.0/add_trailing_comma/_plugins/match.py` & `add_trailing_comma-3.0.1/add_trailing_comma/_plugins/match.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-3.0.0/add_trailing_comma/_token_helpers.py` & `add_trailing_comma-3.0.1/add_trailing_comma/_token_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 
 def find_simple(first_brace: int, tokens: list[Token]) -> Fix | None:
     brace_stack = [first_brace]
     multi_arg = False
 
     for i in range(first_brace + 1, len(tokens)):
         token = tokens[i]
-        if token.src in START_BRACES:
+        if token.name == 'OP' and token.src in START_BRACES:
             brace_stack.append(i)
-        elif token.src in END_BRACES:
+        elif token.name == 'OP' and token.src in END_BRACES:
             brace_stack.pop()
 
         if len(brace_stack) == 1 and token.src == ',':
             multi_arg = True
 
         if not brace_stack:
             break
@@ -90,19 +90,19 @@
     #
     #     func_name(arg, arg, arg)
     #              ^ outer paren
     first_brace = None
     paren_stack = []
     for i in range(i, len(tokens)):
         token = tokens[i]
-        if token.src == '(':
+        if token.name == 'OP' and token.src == '(':
             paren_stack.append(i)
         # the ast lies to us about the beginning of parenthesized functions.
         # See #3. (why we make sure there's something to pop here)
-        elif token.src == ')' and paren_stack:
+        elif token.name == 'OP' and token.src == ')' and paren_stack:
             paren_stack.pop()
 
         if (token.line, token.utf8_byte_offset) in arg_offsets:
             first_brace = paren_stack[0]
             break
     else:
         raise AssertionError('Past end?')
@@ -128,14 +128,18 @@
             # inside.
             not fix_data.multi_arg and
             tokens[first_brace + 1].src in START_BRACES and
             tokens[last_brace - 1].src in END_BRACES or
             # Don't unhug when containing a single token (such as a triple
             # quoted string).
             first_brace + 2 == last_brace or
+            (
+                tokens[first_brace + 1].name == 'FSTRING_START' and
+                tokens[last_brace - 1].name == 'FSTRING_END'
+            ) or
             # don't unhug if it is a single line
             fix_data.remove_comma
     ):
         hug_open = hug_close = False
 
     # fix open hugging
     if hug_open:
```

### Comparing `add_trailing_comma-3.0.0/add_trailing_comma.egg-info/PKG-INFO` & `add_trailing_comma-3.0.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: add-trailing-comma
-Version: 3.0.0
-Summary: Automatically add trailing commas to calls and literals
-Home-page: https://github.com/asottile/add-trailing-comma
-Author: Anthony Sottile
-Author-email: asottile@umich.edu
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![build status](https://github.com/asottile/add-trailing-comma/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/add-trailing-comma/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/add-trailing-comma/main.svg)](https://results.pre-commit.ci/latest/github/asottile/add-trailing-comma/main)
 
 add-trailing-comma
 ==================
 
 A tool (and pre-commit hook) to automatically add trailing commas to calls and
@@ -34,15 +17,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/add-trailing-comma
-    rev: v3.0.0
+    rev: v3.0.1
     hooks:
     -   id: add-trailing-comma
 ```
 
 ## multi-line method invocation style -- why?
 
 ```python
@@ -98,32 +81,14 @@
  x(
      arg,
 -    arg
 +    arg,
  )
 ```
 
-### trailing commas for function calls with unpackings
-
-If `--py35-plus` is passed, `add-trailing-comma` will also perform the
-following change:
-
-```diff
- x(
--    *args
-+    *args,
- )
- y(
--    **kwargs
-+    **kwargs,
- )
-```
-
-Note that this would cause a **`SyntaxError`** in earlier python versions.
-
 ### trailing commas for tuple / list / dict / set literals
 
 ```diff
  x = [
 -    1, 2, 3
 +    1, 2, 3,
  ]
@@ -143,40 +108,14 @@
  async def func(
          arg1,
 -        arg2
 +        arg2,
  ):
 ```
 
-### trailing commas for function definitions with unpacking arguments
-
-If `--py36-plus` is passed, `add-trailing-comma` will also perform the
-following change:
-
-```diff
- def f(
--    *args
-+    *args,
- ): pass
-
-
- def g(
--    **kwargs
-+    **kwargs,
- ): pass
-
-
- def h(
--    *, kw=1
-+    *, kw=1,
- ): pass
-```
-
-Note that this would cause a **`SyntaxError`** in earlier python versions.
-
 ### trailing commas for `from` imports
 
 ```diff
  from os import (
      path,
 -    makedirs
 +    makedirs,
```

### Comparing `add_trailing_comma-3.0.0/add_trailing_comma.egg-info/SOURCES.txt` & `add_trailing_comma-3.0.1/add_trailing_comma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-3.0.0/setup.cfg` & `add_trailing_comma-3.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = add_trailing_comma
-version = 3.0.0
+version = 3.0.1
 description = Automatically add trailing commas to calls and literals
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/asottile/add-trailing-comma
 author = Anthony Sottile
 author_email = asottile@umich.edu
 license = MIT
```

