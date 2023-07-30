# Comparing `tmp/dictionary-search-1.1.0.tar.gz` & `tmp/dictionary-search-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dictionary-search-1.1.0.tar", last modified: Wed Jul 26 17:08:45 2023, max compression
+gzip compressed data, was "dictionary-search-1.1.1.tar", last modified: Sun Jul 30 18:00:58 2023, max compression
```

## Comparing `dictionary-search-1.1.0.tar` & `dictionary-search-1.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:08:45.321568 dictionary-search-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-26 17:08:43.000000 dictionary-search-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-26 17:08:43.000000 dictionary-search-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-07-26 17:08:45.321568 dictionary-search-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-26 17:08:43.000000 dictionary-search-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 17:08:43.000000 dictionary-search-1.1.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:08:45.321568 dictionary-search-1.1.0/dictionary_search/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-26 17:08:43.000000 dictionary-search-1.1.0/dictionary_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-26 17:08:43.000000 dictionary-search-1.1.0/dictionary_search/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-26 17:08:43.000000 dictionary-search-1.1.0/dictionary_search/structural.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:08:45.321568 dictionary-search-1.1.0/dictionary_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-07-26 17:08:45.000000 dictionary-search-1.1.0/dictionary_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-26 17:08:45.000000 dictionary-search-1.1.0/dictionary_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 17:08:45.000000 dictionary-search-1.1.0/dictionary_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-26 17:08:45.000000 dictionary-search-1.1.0/dictionary_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 17:08:45.000000 dictionary-search-1.1.0/dictionary_search.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-26 17:08:45.321568 dictionary-search-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 17:08:43.000000 dictionary-search-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:08:45.321568 dictionary-search-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:08:43.000000 dictionary-search-1.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:08:45.321568 dictionary-search-1.1.0/tests/structural/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:08:43.000000 dictionary-search-1.1.0/tests/structural/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-26 17:08:43.000000 dictionary-search-1.1.0/tests/structural/test_flat.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-26 17:08:43.000000 dictionary-search-1.1.0/tests/structural/test_nest.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-26 17:08:43.000000 dictionary-search-1.1.0/tests/test_search_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-26 17:08:43.000000 dictionary-search-1.1.0/tests/test_search_one.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:00:58.593665 dictionary-search-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-30 18:00:57.000000 dictionary-search-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-30 18:00:57.000000 dictionary-search-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-07-30 18:00:58.593665 dictionary-search-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-30 18:00:57.000000 dictionary-search-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-30 18:00:57.000000 dictionary-search-1.1.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:00:58.593665 dictionary-search-1.1.1/dictionary_search/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-30 18:00:57.000000 dictionary-search-1.1.1/dictionary_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-30 18:00:57.000000 dictionary-search-1.1.1/dictionary_search/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-30 18:00:57.000000 dictionary-search-1.1.1/dictionary_search/structural.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:00:58.593665 dictionary-search-1.1.1/dictionary_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-07-30 18:00:58.000000 dictionary-search-1.1.1/dictionary_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-30 18:00:58.000000 dictionary-search-1.1.1/dictionary_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 18:00:58.000000 dictionary-search-1.1.1/dictionary_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-30 18:00:58.000000 dictionary-search-1.1.1/dictionary_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 18:00:58.000000 dictionary-search-1.1.1/dictionary_search.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-30 18:00:58.593665 dictionary-search-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 18:00:57.000000 dictionary-search-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:00:58.593665 dictionary-search-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 18:00:57.000000 dictionary-search-1.1.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:00:58.593665 dictionary-search-1.1.1/tests/structural/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 18:00:57.000000 dictionary-search-1.1.1/tests/structural/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-30 18:00:57.000000 dictionary-search-1.1.1/tests/structural/test_flat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-30 18:00:57.000000 dictionary-search-1.1.1/tests/structural/test_nest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-30 18:00:57.000000 dictionary-search-1.1.1/tests/test_search_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-30 18:00:57.000000 dictionary-search-1.1.1/tests/test_search_one.py
```

### Comparing `dictionary-search-1.1.0/LICENSE` & `dictionary-search-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dictionary-search-1.1.0/PKG-INFO` & `dictionary-search-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dictionary-search
-Version: 1.1.0
+Version: 1.1.1
 Summary: Small dictionary search utils
 Home-page: https://github.com/cr0hn/python-dictionary-search
 Author: Daniel Garcia / Cesar Gallego
 Maintainer: Daniel Garcia (cr0hn)
 Maintainer-email: cr0hn@cr0hn.com
 License: License :: OSI Approved :: MIT License
 Description: # Dictionary Search tools
```

### Comparing `dictionary-search-1.1.0/README.md` & `dictionary-search-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dictionary-search-1.1.0/dictionary_search/search.py` & `dictionary-search-1.1.1/dictionary_search/search.py`

 * *Files identical despite different names*

### Comparing `dictionary-search-1.1.0/dictionary_search/structural.py` & `dictionary-search-1.1.1/dictionary_search/structural.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import Iterable, List, Any, Tuple
 from functools import singledispatch, reduce
-from itertools import groupby
 
 
 def __next_current(current: str, n: str):
     if current != "":
         return f"{current}.{n}"
     return n
 
@@ -19,36 +18,45 @@
     for k, v in d.items():
         nc = __next_current(current, k)
         yield from flat(v, nc)
 
 
 @flat.register(list)
 def _(l: list, current: str = "") -> Iterable[tuple]:
+    if len(l) == 0:
+        yield current, l
+        return  
     for i, v in enumerate(l):
         nc = __next_current(current, f"[{i}]")
         yield from flat(v, nc)
 
 
 def __part_type(part: str) -> str | int:
     if part.startswith("[") and part.endswith("]"):
         return int(part[1:-1])
     return part
 
 
+# TODO: please structural pattern matching this
 def __nest_recursion(data, part_value):
     parts, value = part_value
     if isinstance(parts, list) and len(parts) == 1:
-        if isinstance(parts[0], int) and len(data) <= parts[0]:
-            data.extend([None] * (parts[0] - len(data) + 1))
+        if isinstance(parts[0], int):
+            if len(data) == 0:
+                data = []
+            if len(data) <= parts[0]:
+                data.extend([None] * (parts[0] - len(data) + 1))
         data[parts[0]] = value
     elif isinstance(parts, list) and isinstance(parts[0], str):
         if parts[0] not in data:
             data[parts[0]] = {}
         data[parts[0]] = __nest_recursion(data[parts[0]], (parts[1:], value))
     elif isinstance(parts[0], int):
+        if len(data) == 0:
+            data = []
         if len(data) <= parts[0]:
             data.extend([None] * (parts[0] - len(data) + 1))
         data[parts[0]] = __nest_recursion(data[parts[0]], (parts[1:], value))
     else:
         raise NotImplementedError
     return data
```

### Comparing `dictionary-search-1.1.0/dictionary_search.egg-info/PKG-INFO` & `dictionary-search-1.1.1/dictionary_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dictionary-search
-Version: 1.1.0
+Version: 1.1.1
 Summary: Small dictionary search utils
 Home-page: https://github.com/cr0hn/python-dictionary-search
 Author: Daniel Garcia / Cesar Gallego
 Maintainer: Daniel Garcia (cr0hn)
 Maintainer-email: cr0hn@cr0hn.com
 License: License :: OSI Approved :: MIT License
 Description: # Dictionary Search tools
```

### Comparing `dictionary-search-1.1.0/setup.cfg` & `dictionary-search-1.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `dictionary-search-1.1.0/tests/structural/test_flat.py` & `dictionary-search-1.1.1/tests/structural/test_flat.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,21 @@
     l = [1, 2, 3]
 
     res = list(flat(l))
 
     assert res == [("[0]", 1), ("[1]", 2), ("[2]", 3)]
 
 
+def test_nested_empty_list():
+    l = {"a": {"b": []}}
+
+    res = list(flat(l))
+
+    assert res == [("a.b", [])]
+
 def test_nested_list():
     l = [1, [2, 3]]
 
     res = list(flat(l))
 
     assert res == [("[0]", 1), ("[1].[0]", 2), ("[1].[1]", 3)]
```

### Comparing `dictionary-search-1.1.0/tests/structural/test_nest.py` & `dictionary-search-1.1.1/tests/structural/test_nest.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,7 +29,13 @@
     d = [("a.b", 1), ("a.c", 2), ("d", 3)]
     assert nest(d) == {"a": {"b": 1, "c": 2}, "d": 3}
 
 
 def test_index_nesting():
     d = [("[0]", 1), ("[1]", 2), ("[2]", 3)]
     assert nest(d) == [1, 2, 3]
+
+
+def test_empty_list_nested():
+    d = [('_meta.operators', [])]
+
+    assert nest(d) == {'_meta': {'operators': []}}
```

