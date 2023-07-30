# Comparing `tmp/uniserde-0.3.3.tar.gz` & `tmp/uniserde-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniserde-0.3.3.tar", max compression
+gzip compressed data, was "uniserde-0.3.4.tar", max compression
```

## Comparing `uniserde-0.3.3.tar` & `uniserde-0.3.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1059 2023-07-21 17:40:19.302257 uniserde-0.3.3/LICENSE
--rw-r--r--   0        0        0     7783 2023-07-29 22:22:24.242305 uniserde-0.3.3/README.md
--rw-r--r--   0        0        0      695 2023-07-29 22:24:17.318955 uniserde-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      328 2023-07-04 19:27:50.392268 uniserde-0.3.3/uniserde/__init__.py
--rw-r--r--   0        0        0     2098 2023-07-28 13:46:04.514003 uniserde-0.3.3/uniserde/bson_deserialize.py
--rw-r--r--   0        0        0     8440 2023-07-28 13:42:15.590760 uniserde-0.3.3/uniserde/caching_serdeserializer.py
--rw-r--r--   0        0        0     1210 2023-07-04 19:24:43.375352 uniserde-0.3.3/uniserde/case_convert.py
--rw-r--r--   0        0        0     4051 2023-07-28 13:42:15.590760 uniserde-0.3.3/uniserde/common.py
--rw-r--r--   0        0        0     6022 2023-07-29 22:20:24.589016 uniserde-0.3.3/uniserde/json_deserialize.py
--rw-r--r--   0        0        0      600 2023-07-22 10:52:35.786683 uniserde-0.3.3/uniserde/lazy_wrapped.py
--rw-r--r--   0        0        0     1974 2023-07-04 19:24:43.382018 uniserde-0.3.3/uniserde/objectid_proxy.py
--rw-r--r--   0        0        0     8700 2023-07-29 22:20:20.432352 uniserde-0.3.3/uniserde/schema_mongodb.py
--rw-r--r--   0        0        0     2150 2023-07-29 22:24:28.305621 uniserde-0.3.3/uniserde/serde_bson.py
--rw-r--r--   0        0        0     2670 2023-07-28 13:42:15.594093 uniserde-0.3.3/uniserde/serde_class.py
--rw-r--r--   0        0        0     5488 2023-07-29 22:21:45.548983 uniserde-0.3.3/uniserde/serde_json.py
--rw-r--r--   0        0        0      487 2023-07-04 19:24:43.382018 uniserde-0.3.3/uniserde/typedefs.py
--rw-r--r--   0        0        0     8549 1970-01-01 00:00:00.000000 uniserde-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-07-21 17:40:19.302257 uniserde-0.3.4/LICENSE
+-rw-r--r--   0        0        0     8358 2023-07-30 06:09:10.148042 uniserde-0.3.4/README.md
+-rw-r--r--   0        0        0      695 2023-07-30 06:24:17.458574 uniserde-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      328 2023-07-04 19:27:50.392268 uniserde-0.3.4/uniserde/__init__.py
+-rw-r--r--   0        0        0     2098 2023-07-28 13:46:04.514003 uniserde-0.3.4/uniserde/bson_deserialize.py
+-rw-r--r--   0        0        0     9416 2023-07-30 06:21:16.785122 uniserde-0.3.4/uniserde/caching_serdeserializer.py
+-rw-r--r--   0        0        0     1210 2023-07-04 19:24:43.375352 uniserde-0.3.4/uniserde/case_convert.py
+-rw-r--r--   0        0        0     4051 2023-07-28 13:42:15.590760 uniserde-0.3.4/uniserde/common.py
+-rw-r--r--   0        0        0     6022 2023-07-30 06:12:14.778353 uniserde-0.3.4/uniserde/json_deserialize.py
+-rw-r--r--   0        0        0      600 2023-07-22 10:52:35.786683 uniserde-0.3.4/uniserde/lazy_wrapped.py
+-rw-r--r--   0        0        0     1974 2023-07-04 19:24:43.382018 uniserde-0.3.4/uniserde/objectid_proxy.py
+-rw-r--r--   0        0        0     9065 2023-07-30 06:23:39.365214 uniserde-0.3.4/uniserde/schema_mongodb.py
+-rw-r--r--   0        0        0     2150 2023-07-29 22:24:28.305621 uniserde-0.3.4/uniserde/serde_bson.py
+-rw-r--r--   0        0        0     2670 2023-07-28 13:42:15.594093 uniserde-0.3.4/uniserde/serde_class.py
+-rw-r--r--   0        0        0     5688 2023-07-30 06:23:39.368547 uniserde-0.3.4/uniserde/serde_json.py
+-rw-r--r--   0        0        0      487 2023-07-04 19:24:43.382018 uniserde-0.3.4/uniserde/typedefs.py
+-rw-r--r--   0        0        0     9124 1970-01-01 00:00:00.000000 uniserde-0.3.4/PKG-INFO
```

### Comparing `uniserde-0.3.3/LICENSE` & `uniserde-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.3/README.md` & `uniserde-0.3.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -81,42 +81,45 @@
   JavaScript
 - BSON uses the same conventions as JSON
 - Python class names are expected to be written in UpperCamelCase
 - Python enum values must be in ALL_UPPER_CASE
 
 ### JSON
 
-| Python         | JSON            | Notes                                                                                                                 |
-| -------------- | --------------- | --------------------------------------------------------------------------------------------------------------------  |
-| bool           | bool            |                                                                                                                       |
-| int            | float           |                                                                                                                       |
-| float          | float           |                                                                                                                       |
-| str            | str             |                                                                                                                       |
-| List           | list            |                                                                                                                       |
-| Optional       | value or `None` |                                                                                                                       |
-| Any            | as-is           |                                                                                                                       |
-| Literal[str]   | str             |                                                                                                                       |
-| enum.Enum      | str             | Enum values are mapped to their name (NOT value!)                                                                     |
-| custom class   | dict            | Each attribute is stored as key, in lowerCamelCase. If marked with `as_child`, an additional `type` field is added.   |
-| bytes          | str             | base64 encoded                                                                                                        |
-| datetime       | str             | as ISO 8601 - with timezone. Naïve datetimes are intentionally not supported. Do yourself a favor and don't use them. |
-| timedelta      | float           | duration, in seconds                                                                                                  |
-| Dict[str, ...] | dict            |                                                                                                                       |
-| bson.ObjectId  | str             |                                                                                                                       |
+| Python           | JSON              | Notes                                                                                                                 |
+| ---------------- | ----------------- | --------------------------------------------------------------------------------------------------------------------  |
+| `bool`           | `bool`            |                                                                                                                       |
+| `int`            | `float`           |                                                                                                                       |
+| `float`          | `float`           |                                                                                                                       |
+| `str`            | `str`             |                                                                                                                       |
+| `Tuple`          | `list`            |                                                                                                                       |
+| `List`           | `list`            |                                                                                                                       |
+| `Set`            | `list`            |                                                                                                                       |
+| `Optional`       | value or `None`   |                                                                                                                       |
+| `Any`            | as-is             |                                                                                                                       |
+| `Literal[str]`   | `str`             |                                                                                                                       |
+| `enum.Enum`      | `str`             | Enum values are mapped to their name (NOT value!)                                                                     |
+| `enum.Flag`      | `List[str]`       | Each flag is encoded the same way a single `Enum` would.                                                              |
+| custom class     | `dict`            | Each attribute is stored as key, in lowerCamelCase. If marked with `as_child`, an additional `type` field is added.   |
+| `bytes`          | `str`             | base64 encoded                                                                                                        |
+| `datetime`       | `str`             | as ISO 8601 - with timezone. Naïve datetimes are intentionally not supported. Do yourself a favor and don't use them. |
+| `timedelta`      | `float`           | duration, in seconds                                                                                                  |
+| `Dict[str, ...]` | `dict`            |                                                                                                                       |
+| `bson.ObjectId`  | `str`             |                                                                                                                       |
 
 ### BSON
 
 BSON uses the same conventions as JSON, with just a few changes
 
-| Python        | BSON          | Notes                                                                                                                                                 |
-| ------------- | ------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
-| custom class  | dict          | Same as JSON, but any fields named `id` are renamed to `_id` to match MongoDB. (Exception: if an `_id` field is already present, `id` is not renamed) |
-| bytes         | bytes         |                                                                                                                                                       |
-| datetime      | datetime      | Serialization requires a timezone be set. Deserialization imputes UTC, to match MongoDB convention.                                                   |
-| bson.ObjectId | bson.ObjectId |                                                                                                                                                       |
+| Python          | BSON            | Notes                                                                                                                                                 |
+| --------------- | --------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
+| custom class    | `dict`          | Same as JSON, but any fields named `id` are renamed to `_id` to match MongoDB. (Exception: if an `_id` field is already present, `id` is not renamed) |
+| `bytes`         | `bytes`         |                                                                                                                                                       |
+| `datetime`      | `datetime`      | Serialization requires a timezone be set. Deserialization imputes UTC, to match MongoDB convention.                                                   |
+| `bson.ObjectId` | `bson.ObjectId` |                                                                                                                                                       |
 
 ## Schema Generation
 
 If you are working with MongoDB you will come to appreciate the automatic schema
 generation. Calling `uniserde.as_mongodb_schema` on any supported class will return
 a MongoDB compatible JSON schema without hassle.
```

### Comparing `uniserde-0.3.3/pyproject.toml` & `uniserde-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uniserde"
-version = "0.3.3"
+version = "0.3.4"
 description = "Convention based, effortless serialization and deserialization"
 authors = ["Jakob Pinterits <jakob.pinterits@gmail.com>"]
 license = "MIT"
 repository = "https://gitlab.com/Vivern/uniserde"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `uniserde-0.3.3/uniserde/bson_deserialize.py` & `uniserde-0.3.4/uniserde/bson_deserialize.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.3/uniserde/caching_serdeserializer.py` & `uniserde-0.3.4/uniserde/caching_serdeserializer.py`

 * *Files 10% similar despite different names*

```diff
@@ -127,15 +127,42 @@
                 override_method_func = override_method.__func__
             except AttributeError:
                 override_method_func = override_method
 
             if override_method_func is not serde_class_method.__func__:
                 return lambda self, value, _type: override_method(value, {})
 
-        # Case: Enum
+        # Case enum.Flag
+        if issubclass(value_type, enum.Flag):
+
+            def handle_flag(self, value, _type):
+                if not isinstance(value, list):
+                    raise SerdeError(f"Expected a list, got `{value}`")
+
+                result = value_type(0)
+
+                for item in value:
+                    if not isinstance(item, str):
+                        raise SerdeError(f"Expected enumeration string, got `{item}`")
+
+                    try:
+                        py_name = case_convert.camel_case_to_all_upper(
+                            item
+                        )  # ValueError if not camel case
+                        result |= value_type[py_name]  # ValueError if not in enum
+                    except KeyError:
+                        raise SerdeError(
+                            f"Invalid enumeration value `{item}`"
+                        ) from None
+
+                return result
+
+            return handle_flag
+
+        # Case: enum.Enum
         if issubclass(value_type, enum.Enum):
 
             def handle_enum(self, value, _type):
                 if not isinstance(value, str):
                     raise SerdeError(f"Expected enumeration string, got `{value}`")
 
                 try:
```

### Comparing `uniserde-0.3.3/uniserde/case_convert.py` & `uniserde-0.3.4/uniserde/case_convert.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.3/uniserde/common.py` & `uniserde-0.3.4/uniserde/common.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.3/uniserde/json_deserialize.py` & `uniserde-0.3.4/uniserde/json_deserialize.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,27 +66,56 @@
         value_type: Type[timedelta],
     ) -> timedelta:
         if not isinstance(value, (int, float)):
             raise SerdeError(f"Expected number, got `{value}`")
 
         return timedelta(seconds=value)
 
+    def _deserialize_tuple_from_list(
+        self,
+        value: Any,
+        value_type: Type[Tuple],
+    ) -> Tuple[Any]:
+        if not isinstance(value, list):
+            raise SerdeError(f"Expected list, got `{value}`")
+
+        subtypes = get_args(value_type)
+
+        if len(value) != len(subtypes):
+            raise SerdeError(
+                f"Expected list of length {len(subtypes)}, but received one of length {len(value)}"
+            )
+
+        return tuple(self.process(v, subtype) for v, subtype in zip(value, subtypes))
+
     def _deserialize_list_from_list(
         self,
         value: Any,
         value_type: Type[List],
     ) -> List[Any]:
         if not isinstance(value, list):
             raise SerdeError(f"Expected list, got `{value}`")
 
         subtype = get_args(value_type)[0]
         child_deserializer = self._get_handler(subtype)
 
         return [child_deserializer(self, v, subtype) for v in value]
 
+    def _deserialize_set_from_list(
+        self,
+        value: Any,
+        value_type: Type[Set],
+    ) -> Set:
+        if not isinstance(value, list):
+            raise SerdeError(f"Expected list, got `{value}`")
+
+        subtype = get_args(value_type)[0]
+
+        return set(self.process(v, subtype) for v in value)
+
     def _deserialize_dict_from_dict(
         self,
         value: Any,
         value_type: Type[Dict],
     ) -> Dict[Any, Any]:
         if not isinstance(value, dict):
             raise SerdeError(f"Expected dict, got `{value}`")
@@ -143,62 +172,33 @@
     ) -> str:
         options = get_args(value_type)
         if value not in options:
             raise SerdeError(f"Expected `{value_type}`, got `{value}`")
 
         return value
 
-    def _deserialize_tuple_from_list(
-        self,
-        value: Any,
-        value_type: Type[Tuple],
-    ) -> Tuple[Any]:
-        if not isinstance(value, list):
-            raise SerdeError(f"Expected list, got `{value}`")
-
-        subtypes = get_args(value_type)
-
-        if len(value) != len(subtypes):
-            raise SerdeError(
-                f"Expected list of length {len(subtypes)}, but received one of length {len(value)}"
-            )
-
-        return tuple(self.process(v, subtype) for v, subtype in zip(value, subtypes))
-
-    def _deserialize_set_from_list(
-        self,
-        value: Any,
-        value_type: Type[Set],
-    ) -> Set:
-        if not isinstance(value, list):
-            raise SerdeError(f"Expected list, got `{value}`")
-
-        subtype = get_args(value_type)[0]
-
-        return set(self.process(v, subtype) for v in value)
-
     _passthrough_types = {
         bool,
         int,
         float,
         str,
     }  # type: ignore
 
     _handler_cache = {
         bytes: _deserialize_bytes_from_str,
         datetime: _deserialize_datetime_from_str,
         timedelta: _deserialize_timedelta_from_float,
+        tuple: _deserialize_tuple_from_list,
         list: _deserialize_list_from_list,
+        set: _deserialize_set_from_list,
         dict: _deserialize_dict_from_dict,
         Union: _deserialize_optional,
         Any: _deserialize_any,
         ObjectId: _deserialize_object_id_from_str,
         Literal: _deserialize_literal_as_is,
-        tuple: _deserialize_tuple_from_list,
-        set: _deserialize_set_from_list,
     }  # type: ignore
 
     _override_method_name = "from_json"
 
 
 def from_json(
     value: Any,
```

### Comparing `uniserde-0.3.3/uniserde/lazy_wrapped.py` & `uniserde-0.3.4/uniserde/lazy_wrapped.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.3/uniserde/objectid_proxy.py` & `uniserde-0.3.4/uniserde/objectid_proxy.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.3/uniserde/schema_mongodb.py` & `uniserde-0.3.4/uniserde/schema_mongodb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+import enum
 import inspect
 from datetime import datetime, timedelta
-from enum import Enum
 from typing import *  # type: ignore
 
 from . import case_convert, serde_class
 from .common import *
 from .objectid_proxy import ObjectId
 from .typedefs import Jsonable
 
@@ -200,16 +200,28 @@
                 override_method_func = override_method.__func__
             except AttributeError:
                 override_method_func = override_method
 
             if override_method_func is not serde_class_method.__func__:
                 return override_method()
 
-        # Case: Enum
-        if issubclass(value_type, Enum):
+        # Case: enum.Flag
+        if issubclass(value_type, enum.Flag):
+            return {
+                "type": "array",
+                "items": {
+                    "enum": [
+                        case_convert.all_upper_to_camel_case(variant.name)
+                        for variant in value_type
+                    ],
+                },
+            }
+
+        # Case: enum.Enum
+        if issubclass(value_type, enum.Enum):
             return {
                 "enum": [
                     case_convert.all_upper_to_camel_case(variant.name)
                     for variant in value_type
                 ],
             }
```

### Comparing `uniserde-0.3.3/uniserde/serde_bson.py` & `uniserde-0.3.4/uniserde/serde_bson.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.3/uniserde/serde_class.py` & `uniserde-0.3.4/uniserde/serde_class.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.3/uniserde/serde_json.py` & `uniserde-0.3.4/uniserde/serde_json.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import base64
+import enum
 import inspect
 import typing
 from datetime import datetime, timedelta
-from enum import Enum
 from typing import *  # type: ignore
 
 from . import case_convert, serde_class
 from .common import *
 from .objectid_proxy import ObjectId
 from .typedefs import Jsonable
 
@@ -77,23 +77,45 @@
     value_type: Type,
     recur: Recur,
 ) -> float:
     assert isinstance(value, timedelta), value
     return value.total_seconds()
 
 
+def serialize_tuple_as_list(
+    value: Any,
+    value_type: Type,
+    recur: Recur,
+) -> List[Any]:
+    assert isinstance(value, tuple), value
+    subtypes = typing.get_args(value_type)
+    assert len(subtypes) == len(value), (subtypes, value)
+
+    return [recur(v, subtype) for v, subtype in zip(value, subtypes)]
+
+
 def serialize_list_to_list(
     value: Any,
     value_type: Type,
     recur: Recur,
 ) -> List[Any]:
     assert isinstance(value, list), value
     return [recur(v, typing.get_args(value_type)[0]) for v in value]
 
 
+def serialize_set_as_list(
+    value: Any,
+    value_type: Type,
+    recur: Recur,
+) -> List[Any]:
+    assert isinstance(value, set), value
+    subtype = typing.get_args(value_type)[0]
+    return [recur(v, subtype) for v in value]
+
+
 def serialize_dict_to_dict(
     value: Any,
     value_type: Type,
     recur: Recur,
 ) -> Dict[Any, Any]:
     subtypes = typing.get_args(value_type)
     assert isinstance(value, dict), value
@@ -133,36 +155,14 @@
     value_type: Type,
     recur: Recur,
 ) -> Any:
     assert isinstance(value, str), value
     return value
 
 
-def serialize_tuple_as_list(
-    value: Any,
-    value_type: Type,
-    recur: Recur,
-) -> List[Any]:
-    assert isinstance(value, tuple), value
-    subtypes = typing.get_args(value_type)
-    assert len(subtypes) == len(value), (subtypes, value)
-
-    return [recur(v, subtype) for v, subtype in zip(value, subtypes)]
-
-
-def serialize_set_as_list(
-    value: Any,
-    value_type: Type,
-    recur: Recur,
-) -> List[Any]:
-    assert isinstance(value, set), value
-    subtype = typing.get_args(value_type)[0]
-    return [recur(v, subtype) for v in value]
-
-
 def serialize_class(
     value: Any,
     value_type: Type,
     recur: Recur,
 ) -> Any:
     assert inspect.isclass(value_type), value_type
 
@@ -171,16 +171,21 @@
         override_method = getattr(value, "as_json")
     except AttributeError:
         pass
     else:
         if override_method.__func__ is not serde_class.Serde.as_json:
             return override_method()
 
-    # Case: Enum
-    if issubclass(value_type, Enum):
+    # Case: enum.Flag
+    if issubclass(value_type, enum.Flag):
+        assert isinstance(value, value_type), value
+        return [case_convert.all_upper_to_camel_case(flag.name) for flag in value]
+
+    # Case: enum.Enum
+    if issubclass(value_type, enum.Enum):
         assert isinstance(value, value_type), value
         return case_convert.all_upper_to_camel_case(value.name)
 
     # Case: Anything else
     # Make sure to serialize as the correct class
     if should_serialize_as_child(value_type):
         assert issubclass(type(value), value_type), (type(value), value_type)
@@ -204,22 +209,22 @@
     bool: serialize_bool_to_bool,
     int: serialize_int_to_int,
     float: serialize_float_to_float,
     bytes: serialize_bytes_to_str,
     str: serialize_str_to_str,
     datetime: serialize_datetime_to_str,
     timedelta: serialize_timedelta_to_float,
+    tuple: serialize_tuple_as_list,
     list: serialize_list_to_list,
+    set: serialize_set_as_list,
     dict: serialize_dict_to_dict,
     Union: serialize_optional,
     Any: serialize_any,
     ObjectId: serialize_object_id_to_str,
     Literal: serialize_literal_as_is,
-    tuple: serialize_tuple_as_list,
-    set: serialize_set_as_list,
 }
 
 
 def as_json(
     value: Any,
     *,
     as_type: Optional[Type] = None,
```

### Comparing `uniserde-0.3.3/PKG-INFO` & `uniserde-0.3.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniserde
-Version: 0.3.3
+Version: 0.3.4
 Summary: Convention based, effortless serialization and deserialization
 Home-page: https://gitlab.com/Vivern/uniserde
 License: MIT
 Author: Jakob Pinterits
 Author-email: jakob.pinterits@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -101,42 +101,45 @@
   JavaScript
 - BSON uses the same conventions as JSON
 - Python class names are expected to be written in UpperCamelCase
 - Python enum values must be in ALL_UPPER_CASE
 
 ### JSON
 
-| Python         | JSON            | Notes                                                                                                                 |
-| -------------- | --------------- | --------------------------------------------------------------------------------------------------------------------  |
-| bool           | bool            |                                                                                                                       |
-| int            | float           |                                                                                                                       |
-| float          | float           |                                                                                                                       |
-| str            | str             |                                                                                                                       |
-| List           | list            |                                                                                                                       |
-| Optional       | value or `None` |                                                                                                                       |
-| Any            | as-is           |                                                                                                                       |
-| Literal[str]   | str             |                                                                                                                       |
-| enum.Enum      | str             | Enum values are mapped to their name (NOT value!)                                                                     |
-| custom class   | dict            | Each attribute is stored as key, in lowerCamelCase. If marked with `as_child`, an additional `type` field is added.   |
-| bytes          | str             | base64 encoded                                                                                                        |
-| datetime       | str             | as ISO 8601 - with timezone. Naïve datetimes are intentionally not supported. Do yourself a favor and don't use them. |
-| timedelta      | float           | duration, in seconds                                                                                                  |
-| Dict[str, ...] | dict            |                                                                                                                       |
-| bson.ObjectId  | str             |                                                                                                                       |
+| Python           | JSON              | Notes                                                                                                                 |
+| ---------------- | ----------------- | --------------------------------------------------------------------------------------------------------------------  |
+| `bool`           | `bool`            |                                                                                                                       |
+| `int`            | `float`           |                                                                                                                       |
+| `float`          | `float`           |                                                                                                                       |
+| `str`            | `str`             |                                                                                                                       |
+| `Tuple`          | `list`            |                                                                                                                       |
+| `List`           | `list`            |                                                                                                                       |
+| `Set`            | `list`            |                                                                                                                       |
+| `Optional`       | value or `None`   |                                                                                                                       |
+| `Any`            | as-is             |                                                                                                                       |
+| `Literal[str]`   | `str`             |                                                                                                                       |
+| `enum.Enum`      | `str`             | Enum values are mapped to their name (NOT value!)                                                                     |
+| `enum.Flag`      | `List[str]`       | Each flag is encoded the same way a single `Enum` would.                                                              |
+| custom class     | `dict`            | Each attribute is stored as key, in lowerCamelCase. If marked with `as_child`, an additional `type` field is added.   |
+| `bytes`          | `str`             | base64 encoded                                                                                                        |
+| `datetime`       | `str`             | as ISO 8601 - with timezone. Naïve datetimes are intentionally not supported. Do yourself a favor and don't use them. |
+| `timedelta`      | `float`           | duration, in seconds                                                                                                  |
+| `Dict[str, ...]` | `dict`            |                                                                                                                       |
+| `bson.ObjectId`  | `str`             |                                                                                                                       |
 
 ### BSON
 
 BSON uses the same conventions as JSON, with just a few changes
 
-| Python        | BSON          | Notes                                                                                                                                                 |
-| ------------- | ------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
-| custom class  | dict          | Same as JSON, but any fields named `id` are renamed to `_id` to match MongoDB. (Exception: if an `_id` field is already present, `id` is not renamed) |
-| bytes         | bytes         |                                                                                                                                                       |
-| datetime      | datetime      | Serialization requires a timezone be set. Deserialization imputes UTC, to match MongoDB convention.                                                   |
-| bson.ObjectId | bson.ObjectId |                                                                                                                                                       |
+| Python          | BSON            | Notes                                                                                                                                                 |
+| --------------- | --------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
+| custom class    | `dict`          | Same as JSON, but any fields named `id` are renamed to `_id` to match MongoDB. (Exception: if an `_id` field is already present, `id` is not renamed) |
+| `bytes`         | `bytes`         |                                                                                                                                                       |
+| `datetime`      | `datetime`      | Serialization requires a timezone be set. Deserialization imputes UTC, to match MongoDB convention.                                                   |
+| `bson.ObjectId` | `bson.ObjectId` |                                                                                                                                                       |
 
 ## Schema Generation
 
 If you are working with MongoDB you will come to appreciate the automatic schema
 generation. Calling `uniserde.as_mongodb_schema` on any supported class will return
 a MongoDB compatible JSON schema without hassle.
```

