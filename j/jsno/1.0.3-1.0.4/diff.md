# Comparing `tmp/jsno-1.0.3.tar.gz` & `tmp/jsno-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsno-1.0.3.tar", last modified: Sat Jul 29 14:43:03 2023, max compression
+gzip compressed data, was "jsno-1.0.4.tar", last modified: Sun Jul 30 15:35:23 2023, max compression
```

## Comparing `jsno-1.0.3.tar` & `jsno-1.0.4.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-29 14:43:03.088676 jsno-1.0.3/
--rw-r--r--   0 pekka      (501) staff       (20)     1060 2023-07-11 17:26:17.000000 jsno-1.0.3/LICENSE
--rw-r--r--   0 pekka      (501) staff       (20)     4007 2023-07-29 14:43:03.088272 jsno-1.0.3/PKG-INFO
--rw-r--r--   0 pekka      (501) staff       (20)     2281 2023-07-29 10:12:41.000000 jsno-1.0.3/README.md
-drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-29 14:43:03.080115 jsno-1.0.3/jsno/
--rw-r--r--   0 pekka      (501) staff       (20)     1405 2023-07-29 14:38:38.000000 jsno-1.0.3/jsno/__init__.py
--rw-r--r--   0 pekka      (501) staff       (20)     2398 2023-07-29 14:33:44.000000 jsno-1.0.3/jsno/abc.py
--rw-r--r--   0 pekka      (501) staff       (20)     4438 2023-07-29 09:40:36.000000 jsno-1.0.3/jsno/jsonify.py
--rw-r--r--   0 pekka      (501) staff       (20)      425 2023-07-23 10:01:17.000000 jsno-1.0.3/jsno/jsonize.py
--rw-r--r--   0 pekka      (501) staff       (20)      494 2023-07-23 10:02:00.000000 jsno-1.0.3/jsno/method.py
--rw-r--r--   0 pekka      (501) staff       (20)     5243 2023-07-29 14:17:17.000000 jsno-1.0.3/jsno/standard.py
--rw-r--r--   0 pekka      (501) staff       (20)     4079 2023-07-29 14:35:11.000000 jsno-1.0.3/jsno/unjsonify.py
--rw-r--r--   0 pekka      (501) staff       (20)      869 2023-07-29 09:00:26.000000 jsno-1.0.3/jsno/utils.py
--rw-r--r--   0 pekka      (501) staff       (20)     3387 2023-07-29 08:59:40.000000 jsno-1.0.3/jsno/variant.py
-drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-29 14:43:03.082078 jsno-1.0.3/jsno.egg-info/
--rw-r--r--   0 pekka      (501) staff       (20)     4007 2023-07-29 14:43:03.000000 jsno-1.0.3/jsno.egg-info/PKG-INFO
--rw-r--r--   0 pekka      (501) staff       (20)      512 2023-07-29 14:43:03.000000 jsno-1.0.3/jsno.egg-info/SOURCES.txt
--rw-r--r--   0 pekka      (501) staff       (20)        1 2023-07-29 14:43:03.000000 jsno-1.0.3/jsno.egg-info/dependency_links.txt
--rw-r--r--   0 pekka      (501) staff       (20)       23 2023-07-29 14:43:03.000000 jsno-1.0.3/jsno.egg-info/requires.txt
--rw-r--r--   0 pekka      (501) staff       (20)        5 2023-07-29 14:43:03.000000 jsno-1.0.3/jsno.egg-info/top_level.txt
--rw-r--r--   0 pekka      (501) staff       (20)      711 2023-07-29 14:38:45.000000 jsno-1.0.3/pyproject.toml
--rw-r--r--   0 pekka      (501) staff       (20)       38 2023-07-29 14:43:03.088805 jsno-1.0.3/setup.cfg
-drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-29 14:43:03.087494 jsno-1.0.3/tests/
--rw-r--r--   0 pekka      (501) staff       (20)     1129 2023-07-29 09:57:25.000000 jsno-1.0.3/tests/test_abc.py
--rw-r--r--   0 pekka      (501) staff       (20)     4207 2023-07-29 14:40:19.000000 jsno-1.0.3/tests/test_dataclasses.py
--rw-r--r--   0 pekka      (501) staff       (20)     2905 2023-07-29 13:51:44.000000 jsno-1.0.3/tests/test_dates.py
--rw-r--r--   0 pekka      (501) staff       (20)     1087 2023-07-15 09:44:23.000000 jsno-1.0.3/tests/test_examples.py
--rw-r--r--   0 pekka      (501) staff       (20)     2437 2023-07-29 13:40:19.000000 jsno-1.0.3/tests/test_jsonify.py
--rw-r--r--   0 pekka      (501) staff       (20)     2734 2023-07-16 16:57:33.000000 jsno-1.0.3/tests/test_methods.py
--rw-r--r--   0 pekka      (501) staff       (20)     1713 2023-07-29 13:38:35.000000 jsno-1.0.3/tests/test_standard.py
--rw-r--r--   0 pekka      (501) staff       (20)     4436 2023-07-29 14:16:23.000000 jsno-1.0.3/tests/test_unjsonify.py
--rw-r--r--   0 pekka      (501) staff       (20)     2885 2023-07-29 07:58:13.000000 jsno-1.0.3/tests/test_variant.py
+drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-30 15:35:23.490697 jsno-1.0.4/
+-rw-r--r--   0 pekka      (501) staff       (20)     1060 2023-07-11 17:26:17.000000 jsno-1.0.4/LICENSE
+-rw-r--r--   0 pekka      (501) staff       (20)    10330 2023-07-30 15:35:23.490381 jsno-1.0.4/PKG-INFO
+-rw-r--r--   0 pekka      (501) staff       (20)     8604 2023-07-30 15:31:42.000000 jsno-1.0.4/README.md
+drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-30 15:35:23.482623 jsno-1.0.4/jsno/
+-rw-r--r--   0 pekka      (501) staff       (20)     1748 2023-07-30 15:33:51.000000 jsno-1.0.4/jsno/__init__.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2316 2023-07-29 19:39:45.000000 jsno-1.0.4/jsno/abc.py
+-rw-r--r--   0 pekka      (501) staff       (20)     4542 2023-07-29 19:39:45.000000 jsno-1.0.4/jsno/jsonify.py
+-rw-r--r--   0 pekka      (501) staff       (20)      710 2023-07-30 15:32:48.000000 jsno-1.0.4/jsno/jsonize.py
+-rw-r--r--   0 pekka      (501) staff       (20)      630 2023-07-29 19:08:24.000000 jsno-1.0.4/jsno/method.py
+-rw-r--r--   0 pekka      (501) staff       (20)     5243 2023-07-29 19:40:07.000000 jsno-1.0.4/jsno/standard.py
+-rw-r--r--   0 pekka      (501) staff       (20)     3976 2023-07-29 19:39:45.000000 jsno-1.0.4/jsno/unjsonify.py
+-rw-r--r--   0 pekka      (501) staff       (20)      882 2023-07-29 19:39:45.000000 jsno-1.0.4/jsno/utils.py
+-rw-r--r--   0 pekka      (501) staff       (20)     3437 2023-07-29 19:39:45.000000 jsno-1.0.4/jsno/variant.py
+drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-30 15:35:23.484047 jsno-1.0.4/jsno.egg-info/
+-rw-r--r--   0 pekka      (501) staff       (20)    10330 2023-07-30 15:35:23.000000 jsno-1.0.4/jsno.egg-info/PKG-INFO
+-rw-r--r--   0 pekka      (501) staff       (20)      568 2023-07-30 15:35:23.000000 jsno-1.0.4/jsno.egg-info/SOURCES.txt
+-rw-r--r--   0 pekka      (501) staff       (20)        1 2023-07-30 15:35:23.000000 jsno-1.0.4/jsno.egg-info/dependency_links.txt
+-rw-r--r--   0 pekka      (501) staff       (20)       23 2023-07-30 15:35:23.000000 jsno-1.0.4/jsno.egg-info/requires.txt
+-rw-r--r--   0 pekka      (501) staff       (20)        5 2023-07-30 15:35:23.000000 jsno-1.0.4/jsno.egg-info/top_level.txt
+-rw-r--r--   0 pekka      (501) staff       (20)      711 2023-07-30 15:33:55.000000 jsno-1.0.4/pyproject.toml
+-rw-r--r--   0 pekka      (501) staff       (20)       38 2023-07-30 15:35:23.490768 jsno-1.0.4/setup.cfg
+drwxr-xr-x   0 pekka      (501) staff       (20)        0 2023-07-30 15:35:23.489733 jsno-1.0.4/tests/
+-rw-r--r--   0 pekka      (501) staff       (20)     1223 2023-07-29 19:21:09.000000 jsno-1.0.4/tests/test_abc.py
+-rw-r--r--   0 pekka      (501) staff       (20)      936 2023-07-30 15:34:37.000000 jsno-1.0.4/tests/test_ast_example.py
+-rw-r--r--   0 pekka      (501) staff       (20)     4205 2023-07-29 18:53:29.000000 jsno-1.0.4/tests/test_dataclasses.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2905 2023-07-29 18:50:18.000000 jsno-1.0.4/tests/test_dates.py
+-rw-r--r--   0 pekka      (501) staff       (20)      165 2023-07-30 07:55:38.000000 jsno-1.0.4/tests/test_dumps_and_loads.py
+-rw-r--r--   0 pekka      (501) staff       (20)     1794 2023-07-30 15:34:48.000000 jsno-1.0.4/tests/test_examples.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2437 2023-07-29 18:53:15.000000 jsno-1.0.4/tests/test_jsonify.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2735 2023-07-29 18:46:29.000000 jsno-1.0.4/tests/test_methods.py
+-rw-r--r--   0 pekka      (501) staff       (20)     1713 2023-07-29 18:45:56.000000 jsno-1.0.4/tests/test_standard.py
+-rw-r--r--   0 pekka      (501) staff       (20)     4437 2023-07-29 18:50:19.000000 jsno-1.0.4/tests/test_unjsonify.py
+-rw-r--r--   0 pekka      (501) staff       (20)     2886 2023-07-29 18:52:46.000000 jsno-1.0.4/tests/test_variant.py
```

### Comparing `jsno-1.0.3/LICENSE` & `jsno-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jsno-1.0.3/jsno/abc.py` & `jsno-1.0.4/jsno/abc.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import base64
 
 from collections.abc import ByteString, Mapping, Sequence, Set
 
 from jsno.jsonify import jsonify
 from jsno.unjsonify import unjsonify, typecheck, raise_error, cast
-from jsno.utils import get_args, get_origin
+from jsno.utils import get_args
 
 
 # Mapping
 
 
 @jsonify.register(Mapping)
 def _(value):
@@ -26,27 +26,25 @@
     a JSON object (dict).
     """
 
     typecheck(value, dict, as_type)
 
     arg_types = get_args(as_type)
 
-    # need to take origin for this to work for Dict and List
-    origin = get_origin(as_type) or as_type
-
     if not arg_types:
-        return cast(value, origin)
+        return cast(value, as_type)
     else:
         unjsonify_key = unjsonify[arg_types[0]]
         unjsonify_val = unjsonify[arg_types[1]]
 
-        return origin({
+        as_dict = {
             unjsonify_key(key): unjsonify_val(val)
             for (key, val) in value.items()
-        })
+        }
+        return cast(as_dict, as_type)
 
 
 # Sequence
 
 
 @jsonify.register(Sequence)
 def jsonify_sequence(value):
@@ -64,46 +62,46 @@
     else:
         unjsonify_item = unjsonify[arg_types[0]]
         return cast([unjsonify_item(item) for item in value], as_type)
 
 
 # Set
 
+
 @jsonify.register(Set)
 def _(value):
     """
     Set is not a sequence, so it needs it's own jsonifier.
     Because the order of iterating over a set is not defined, the jsonification
     tries to sort the set first, to make the results more predictable.
     """
 
     # if possible, sort the values first.
     try:
         value = sorted(value, key=lambda v: (type(v).__name__, v))
-    except:
+    except Exception:
         pass
 
-    return [jsonify(val) for val in value]
+    return jsonify_sequence(value)
 
 
 unjsonify.register(Set)(unjsonify_sequence)
 
 
 # ByteString abstract base class
 
 
 @jsonify.register(ByteString)
 def _(value):
-    return base64.b64encode(value).decode('ascii')
+    return base64.b64encode(value).decode("ascii")
 
 
 @unjsonify.register(ByteString)
 def _(value, as_type):
     typecheck(value, str, as_type)
 
     try:
-        return base64.b64decode(value.encode('ascii'))
+        return base64.b64decode(value.encode("ascii"))
     except ValueError as exc:
         detail = exc.args[0]
 
     raise_error(value, as_type, detail)
-
```

### Comparing `jsno-1.0.3/jsno/jsonify.py` & `jsno-1.0.4/jsno/jsonify.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,28 +7,27 @@
 
 """
 valid JSON types.
 """
 JSON = bool | int | float | str | list["JSON"] | dict[str, "JSON"] | None
 
 
-
 def jsonify_dataclass(value) -> dict[str, JSON]:
     """
     Jsonify a value whose type is a dataclass.
     """
-    result = {}
-
+    result: dict[str, JSON] = {}
+    value_type: type = type(value)
 
-    if (family := get_variantfamily(type(value))):
+    if family := get_variantfamily(value_type):
         # if the value's class is a member of a variant family,
         # first add the variant label to the jsonified result
-        result[family.label_name] = family.get_label(type(value))
+        result[family.label_name] = family.get_label(value_type)
 
-    for field in get_dataclass_fields(type(value)):
+    for field in get_dataclass_fields(value_type):
         val = getattr(value, field.name)
 
         # skip optional values that are None
         if val is not None or not is_optional(field.type):
             result[field.name] = jsonify(val)
 
     return result
@@ -62,15 +61,14 @@
                 # found the first transformed value
                 result = value[:ix]
                 result.append(val_json)
                 ix += 1
                 break
             ix += 1
 
-
     while ix < count:
         val_json = call_jsonify(value[ix])
         result.append(value[ix] if val_json is value[ix] else val_json)
         ix += 1
 
     return result
 
@@ -152,14 +150,17 @@
     elif as_type is dict:
         return jsonify_dict(value)
     else:
         return generic_jsonify.dispatch(as_type)(value)
 
 
 class Jsonify:
+    """
+    Singleton type for the jsonify function
+    """
 
     def __call__(self, value) -> JSON:
         """
         Jsonify any value that supports jsonification.
         """
         return call_jsonify(value)
```

### Comparing `jsno-1.0.3/jsno/standard.py` & `jsno-1.0.4/jsno/standard.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from jsno.jsonify import jsonify
 from jsno.unjsonify import unjsonify, typecheck, raise_error, cast
 from jsno.utils import get_args
 
 
 # marking types to be jsonified as strings
 
+
 def jsonify_to_string(value):
     return str(value)
 
 
 def unjsonify_from_string(value, as_type):
     typecheck(value, str, as_type)
     return cast(value, as_type)
@@ -146,14 +147,15 @@
 
 # enums
 
 @jsonify.register(enum.Enum)
 def _(enum):
     return enum.name
 
+
 @unjsonify.register(enum.Enum)
 def _(value, as_type):
     typecheck(value, str, as_type)
     try:
         return getattr(as_type, value)
     except AttributeError:
         pass
@@ -162,22 +164,22 @@
 
 
 # datetime.date
 
 
 @jsonify.register(datetime.date)
 def _(date):
-    return f'{date.year}-{date.month:02}-{date.day:02}'
+    return f"{date.year}-{date.month:02}-{date.day:02}"
 
 
 @unjsonify.register(datetime.date)
 def _(value, as_type):
     typecheck(value, str, as_type)
     try:
-        (ys, ms, ds) = value.split('-')
+        (ys, ms, ds) = value.split("-")
         return as_type(int(ys), int(ms), int(ds))
     except ValueError as exc:
         detail = exc.args[0]
 
     raise_error(value, as_type, detail)
 
 
@@ -246,15 +248,14 @@
 jsonify_as_string(pathlib.Path)
 
 # complex numbers
 
 jsonify_as_string(complex)
 
 
-
 @jsonify.register(range)
 def _(value):
     result = {"start": value.start, "stop": value.stop}
     if value.step != 1:
         result["step"] = value.step
     return result
 
@@ -269,8 +270,7 @@
 @unjsonify.register(range)
 def _(value, as_type):
     it = unjsonify[Range](value)
     if it.step == 0:
         raise_error(value, as_type, "Range step must not be zero")
 
     return as_type(it.start, it.stop, it.step or 1)
-
```

### Comparing `jsno-1.0.3/jsno/unjsonify.py` & `jsno-1.0.4/jsno/unjsonify.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,12 @@
-import base64
 import dataclasses
-import datetime
-import enum
 import functools
 import types
 
 
-from collections.abc import ByteString, Mapping, Sequence, Set
 from typing import Any, Union, Literal
 
 
 from jsno.utils import get_origin, get_args, get_dataclass_fields
 from jsno.variant import get_variantfamily
 
 
@@ -47,20 +43,19 @@
         return value
 
     try:
         return origin_type(value)
     except ValueError as exc:
         detail = exc.args[0]
 
-    raise_error(value, as_type)
+    raise_error(value, as_type, detail)
 
 
 @functools.singledispatch
 def unjsonify_type(value, as_type):
-
     if dataclasses.is_dataclass(as_type):
         return unjsonify_dataclass(value, as_type)
 
     raise TypeError(f"Unjsonify not defined for {as_type}")
 
 
 def unjsonify_dataclass(value, as_type):
@@ -101,16 +96,16 @@
     options = get_args(as_type)
 
     if value in options:
         return value
 
     raise_error(value, as_type)
 
-class Unjsonify:
 
+class Unjsonify:
     def _dispatch(self, type_):
 
         origin = get_origin(type_) or type_
 
         # special cases needed for constructs in typing module, as
         # singledispatch fails cannot handle Union and Literal
         if origin is Union:
@@ -122,16 +117,15 @@
             # covers list[X], dict[K,V], etc.
             func = unjsonify_type.dispatch(origin)
 
         # return a specialized version of the unjsonify function
         return lambda value: func(value, type_)
 
     def __getitem__(self, type_):
-
-        if (isinstance(type_, type) and (family := get_variantfamily(type_))):
+        if isinstance(type_, type) and (family := get_variantfamily(type_)):
             return lambda value: unjsonify_variant(value, type_, family)
 
         return self._dispatch(type_)
 
     def register(self, type_):
         return unjsonify_type.register(type_)
 
@@ -153,9 +147,9 @@
             continue
 
     raise UnjsonifyError(f"Cannot unjsonify as {as_type}", value)
 
 
 @unjsonify.register(Any)
 def _(value, as_type):
-    """ Unjsonify Any type: just return the value """
+    """Unjsonify Any type: just return the value"""
     return value
```

### Comparing `jsno-1.0.3/jsno/utils.py` & `jsno-1.0.4/jsno/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import dataclasses
 import functools
 import types
 import typing
 
 
 union_types = (
-    typing.Union ,   # Union[X] or Optional[X]
-    types.UnionType  # X | Y or X | None
+    typing.Union,  # Union[X] or Optional[X]
+    types.UnionType,  # X | Y or X | None
 )
 
 
 @functools.cache
 def get_origin(type):
     """
     Cached version typing.get_origin() to make sure it's quick to check.
@@ -23,16 +23,18 @@
     """
     Cached version typing.get_args() to make sure it's quick to check.
     """
     return typing.get_args(type)
 
 
 @functools.cache
-def get_dataclass_fields(cls):
-    """ Cache dataclass fields for speed """
+def get_dataclass_fields(cls: type):
+    """
+    Cache dataclass fields for speed
+    """
     return dataclasses.fields(cls)
 
 
 def is_optional(type_) -> bool:
     """
     Check if a type object is instance of optional type
     (something that could be None)
```

### Comparing `jsno-1.0.3/jsno/variant.py` & `jsno-1.0.4/jsno/variant.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 
 class VariantFamily:
     """
     VariantFamily represents a variant class hierarchy.
     """
 
-    def __init__(self, root_class, label_name: str):
+    def __init__(self, root_class: type, label_name: str):
         self.root_class = root_class
         self.label_name = label_name
 
-        self._label_for_class = {}
-        self._class_for_label = {}
+        self._label_for_class: dict[type, str] = {}
+        self._class_for_label: dict[str, type | None] = {}
 
     def get_variant(self, label: str) -> type | None:
         """
         Get the variant class corresponding to the given label,
         or None if there is no class registerd for that label.
         """
 
@@ -34,15 +34,15 @@
 
     def _search_variant(self, label: str, cls: type) -> type | None:
 
         if label == self.get_label(cls):
             return cls
 
         for sub in cls.__subclasses__():
-            if (it := self._search_variant(label, sub)):
+            if it := self._search_variant(label, sub):
                 return it
 
         return None
 
     def get_label(self, cls: type) -> str:
         """
         Get the label for a class. If not expiclitly, set, using the
@@ -69,23 +69,23 @@
     """
     Get the VariantFamily instance corresponding to a class,
     or None, if it is not part of a variant hierarchy
     """
     return None
 
 
-def get_variantfamily(cls : type) -> VariantFamily:
+def get_variantfamily(cls: type) -> VariantFamily | None:
     """
     Get the variant family that the argument type is part of, or
     None if it is not part of any.
     """
     return _get_variantfamily.dispatch(cls)(None)
 
 
-def variantfamily(label: str = 'label') -> Callable[[type], type]:
+def variantfamily(label: str = "label") -> Callable[[type], type]:
     """
     Decorator for marking the root of a variant family.
     """
 
     def decorator(cls: type) -> type:
 
         # make sure that the class is not already part of a variant
@@ -116,9 +116,8 @@
         family = get_variantfamily(cls)
         if not family:
             raise TypeError(f"Not member of a variant family: {cls}")
 
         family.register_variant(cls, label)
         return cls
 
-
     return decorator
```

### Comparing `jsno-1.0.3/jsno.egg-info/SOURCES.txt` & `jsno-1.0.4/jsno.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 jsno/variant.py
 jsno.egg-info/PKG-INFO
 jsno.egg-info/SOURCES.txt
 jsno.egg-info/dependency_links.txt
 jsno.egg-info/requires.txt
 jsno.egg-info/top_level.txt
 tests/test_abc.py
+tests/test_ast_example.py
 tests/test_dataclasses.py
 tests/test_dates.py
+tests/test_dumps_and_loads.py
 tests/test_examples.py
 tests/test_jsonify.py
 tests/test_methods.py
 tests/test_standard.py
 tests/test_unjsonify.py
 tests/test_variant.py
```

### Comparing `jsno-1.0.3/pyproject.toml` & `jsno-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jsno"
-version = "1.0.3"
+version = "1.0.4"
 description = "Convert Python data to and from json-compatible data structures"
 readme = "README.md"
 authors = [{ name = "Pekka Uronen", email = "pekka.uronen@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `jsno-1.0.3/tests/test_abc.py` & `jsno-1.0.4/tests/test_abc.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,14 +23,18 @@
     dc = jsonify(os.environ)
 
     userdict = unjsonify[collections.UserDict](dc)
     assert type(userdict) is collections.UserDict
     assert userdict == dc
 
 
+def test_unjsonify_untyped_dict():
+    assert unjsonify[dict]({"foo": 123}) == {"foo": 123}
+
+
 def test_unjsonify_bytestring_failure():
     with pytest.raises(UnjsonifyError):
         unjsonify[bytes]("foo")
 
 
 def test_jsonify_mixed_set():
     assert jsonify(set((1, 2, 3, "abc", None))) == [None, 1, 2, 3, "abc"]
```

### Comparing `jsno-1.0.3/tests/test_dataclasses.py` & `jsno-1.0.4/tests/test_dataclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,11 +177,10 @@
 
 def test_unjsonifty_dataclass_with_default_value():
     user = unjsonify[User]({"username": "usr"})
 
     assert user == User(username="usr")
     assert user.password == "pAssW0rd"
 
-    user = unjsonify[User]({"username": "usr", "password": "", "metadata":  [{"key": 100}]})
+    user = unjsonify[User]({"username": "usr", "password": "", "metadata": [{"key": 100}]})
 
     assert user == User(username="usr", password="", metadata=[{"key": 100}])
-
```

### Comparing `jsno-1.0.3/tests/test_dates.py` & `jsno-1.0.4/tests/test_dates.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -35,14 +35,15 @@
             "2023-07-15T08:40:10.000120Z",
             "2023-07-15T08:40:10.000001Z",
             "5012-07-15T08:41:20.123400",
             "2023-07-29T13:23:11Z",
         ]
     )
 
+
 def test_jsonify_old_dates():
     assert (
         jsonify(
             [
                 datetime.datetime(1940, 7, 15, 8, 39, 0, tzinfo=helsinki),
                 datetime.datetime(1960, 7, 15, 8, 39, 0, tzinfo=helsinki),
                 datetime.datetime(1980, 7, 15, 8, 39, 0, tzinfo=helsinki),
@@ -82,8 +83,7 @@
         )
     )
 
 
 def test_unjsonify_datetime_failure():
     with pytest.raises(UnjsonifyError):
         unjsonify[datetime.datetime]('2023-13-13T12:34:56')
-
```

### Comparing `jsno-1.0.3/tests/test_jsonify.py` & `jsno-1.0.4/tests/test_jsonify.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 import datetime
 
 import pytest
 
 from jsno.jsonify import jsonify
 
 
-
 def test_jsonify_none():
-    assert jsonify(None) == None
+    assert jsonify(None) is None
 
 
 def test_jsonify_string():
     assert jsonify("foo") == "foo"
 
 
 def test_jsonify_int():
     assert jsonify(123) == 123
 
 
 def test_jsonify_tuple():
     assert jsonify(("x", 1, datetime.date(2023, 7, 15))) == ["x", 1, "2023-07-15"]
 
+
 def test_jsonify_set():
     assert jsonify(set("abababa")) == ["a", "b"]
 
 
 def test_jsonify_fonzenset():
     assert jsonify(frozenset("abababa")) == ["a", "b"]
```

### Comparing `jsno-1.0.3/tests/test_methods.py` & `jsno-1.0.4/tests/test_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     """
     assert (
         unjsonify[NamedList]({'name': 'List', 'items': [1, 2, 3]})
         ==
         NamedList([1, 2, 3], name="List")
     )
 
+
 class RenamedList(NamedList):
     """
     Subclass of NmedList, to be registered with custom jsonification
     methods.
     """
     pass
```

### Comparing `jsno-1.0.3/tests/test_standard.py` & `jsno-1.0.4/tests/test_standard.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 
 def test_jsonify_path():
     assert jsonify(pathlib.Path("/dev/null")) == "/dev/null"
 
 
 def test_unjsonify_path():
-    assert unjsonify[pathlib.Path]("/dev/null")  == pathlib.Path("/dev/null")
+    assert unjsonify[pathlib.Path]("/dev/null") == pathlib.Path("/dev/null")
 
 
 def test_jsonify_zoneinfo():
     assert (
         jsonify(zoneinfo.ZoneInfo("Europe/Helsinki")) ==
         "Europe/Helsinki"
     )
@@ -60,13 +60,13 @@
 
     with pytest.raises(zoneinfo.ZoneInfoNotFoundError):
         unjsonify[ZoneInfoSub]("Europe/Vantaa")
 
 
 def test_jsonify_range():
     run_tests(range(100), {"start": 0, "stop": 100})
-    run_tests(range(10, 0,-1), {"start": 10, "stop": 0, "step": -1})
+    run_tests(range(10, 0, -1), {"start": 10, "stop": 0, "step": -1})
 
 
 def test_jsonify_range_failure():
     with pytest.raises(UnjsonifyError):
         unjsonify[range]({"start": 1, "stop": 6, "step": 0})
```

### Comparing `jsno-1.0.3/tests/test_unjsonify.py` & `jsno-1.0.4/tests/test_unjsonify.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 
 
 helsinki = zoneinfo.ZoneInfo("Europe/Helsinki")
 utc = zoneinfo.ZoneInfo("UTC")
 
 
 def test_unjsonify_none():
-    assert unjsonify[type(None)](None) == None
+    assert unjsonify[type(None)](None) is None
 
 
 def test_unjsonify_any():
-    assert unjsonify[Any](None) == None
+    assert unjsonify[Any](None) is None
 
 
 def test_unjsonify_none_from_string_fails():
     with pytest.raises(UnjsonifyError):
-        assert unjsonify[type(None)]("foo") == None
+        assert unjsonify[type(None)]("foo") is None
 
 
 def test_unjsonify_string():
     assert unjsonify[str]("foo") == "foo"
 
 
 def test_unjsonify_float():
@@ -97,14 +97,15 @@
 def test_unjsonify_list_of_union_types():
     assert unjsonify[List[str | int]](["Yes", 51, "No"]) == ["Yes", 51, "No"]
 
 
 def test_unjsonify_list_of_union_types2():
     assert unjsonify[List[int | str]](["Yes", 51, "No"]) == ["Yes", 51, "No"]
 
+
 def test_unjsonify_list_of_union_types3():
     assert unjsonify[List[list[bool] | int | str]](["Yes", 51, [True]]) == ["Yes", 51, [True]]
 
 
 def test_unjsonify_list_of_typing_optionals():
     assert unjsonify[List[Optional[str]]](["Yes", None, "No"]) == ["Yes", None, "No"]
```

### Comparing `jsno-1.0.3/tests/test_variant.py` & `jsno-1.0.4/tests/test_variant.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from dataclasses import dataclass
 
 import pytest
 
 from jsno import jsonify, unjsonify, variantfamily, variantlabel, UnjsonifyError
 
 
-
 @variantfamily(label='type')
 class Expression:
     pass
 
 
 @dataclass
 class Literal(Expression):
@@ -54,20 +53,20 @@
         return self.left.evaluate(context) or self.right.evaluate(context)
 
 
 expr = And(Not(Variable("x")), Or(Variable("y"), Literal(False)))
 
 
 def test_expression_evaluation():
-   assert expr.evaluate({"x": False, "y": True}) is True
-   assert expr.evaluate({"x": False, "y": False}) is False
+    assert expr.evaluate({"x": False, "y": True}) is True
+    assert expr.evaluate({"x": False, "y": False}) is False
 
 
 def test_jsonify_variant():
-    jsonified =  jsonify(expr)
+    jsonified = jsonify(expr)
 
     assert jsonified == {
         "type": "And",
         "left": {
             "type": "NOT",
             "expr": {
                 "type": "Variable",
@@ -102,14 +101,15 @@
         unjsonify[Expression]({"type": "Whatever", "value": False})
 
 
 def test_jsonify_variant_no_label_error():
     with pytest.raises(UnjsonifyError):
         unjsonify[Expression]({"x-type": "Literal", "value": False})
 
+
 def test_jsonify_variant_not_dict_error():
     with pytest.raises(UnjsonifyError):
         unjsonify[Expression]("Something else")
 
 
 def test_variantlabel_error():
```

