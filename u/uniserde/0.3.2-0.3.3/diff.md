# Comparing `tmp/uniserde-0.3.2.tar.gz` & `tmp/uniserde-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniserde-0.3.2.tar", max compression
+gzip compressed data, was "uniserde-0.3.3.tar", max compression
```

## Comparing `uniserde-0.3.2.tar` & `uniserde-0.3.3.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0     7626 2023-07-04 14:25:24.085255 uniserde-0.3.2/README.md
--rw-r--r--   0        0        0      645 2023-07-04 19:38:03.976274 uniserde-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      328 2023-07-04 19:27:50.392268 uniserde-0.3.2/uniserde/__init__.py
--rw-r--r--   0        0        0     2075 2023-07-04 19:37:44.222921 uniserde-0.3.2/uniserde/bson_deserialize.py
--rw-r--r--   0        0        0     7941 2023-07-04 19:33:02.725963 uniserde-0.3.2/uniserde/caching_deserializer.py
--rw-r--r--   0        0        0     1210 2023-07-04 19:24:43.375352 uniserde-0.3.2/uniserde/case_convert.py
--rw-r--r--   0        0        0     4091 2023-07-04 18:37:13.467910 uniserde-0.3.2/uniserde/common.py
--rw-r--r--   0        0        0     5686 2023-07-04 19:32:32.782597 uniserde-0.3.2/uniserde/json_deserialize.py
--rw-r--r--   0        0        0     1974 2023-07-04 19:24:43.382018 uniserde-0.3.2/uniserde/objectid_proxy.py
--rw-r--r--   0        0        0     7094 2023-07-04 19:24:43.378685 uniserde-0.3.2/uniserde/schema_mongodb.py
--rw-r--r--   0        0        0     2152 2023-07-04 19:24:43.382018 uniserde-0.3.2/uniserde/serde_bson.py
--rw-r--r--   0        0        0     2697 2023-07-04 19:28:59.365686 uniserde-0.3.2/uniserde/serde_class.py
--rw-r--r--   0        0        0     5275 2023-07-04 19:24:43.378685 uniserde-0.3.2/uniserde/serde_json.py
--rw-r--r--   0        0        0      487 2023-07-04 19:24:43.382018 uniserde-0.3.2/uniserde/typedefs.py
--rw-r--r--   0        0        0     8352 1970-01-01 00:00:00.000000 uniserde-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-07-21 17:40:19.302257 uniserde-0.3.3/LICENSE
+-rw-r--r--   0        0        0     7783 2023-07-29 22:22:24.242305 uniserde-0.3.3/README.md
+-rw-r--r--   0        0        0      695 2023-07-29 22:24:17.318955 uniserde-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      328 2023-07-04 19:27:50.392268 uniserde-0.3.3/uniserde/__init__.py
+-rw-r--r--   0        0        0     2098 2023-07-28 13:46:04.514003 uniserde-0.3.3/uniserde/bson_deserialize.py
+-rw-r--r--   0        0        0     8440 2023-07-28 13:42:15.590760 uniserde-0.3.3/uniserde/caching_serdeserializer.py
+-rw-r--r--   0        0        0     1210 2023-07-04 19:24:43.375352 uniserde-0.3.3/uniserde/case_convert.py
+-rw-r--r--   0        0        0     4051 2023-07-28 13:42:15.590760 uniserde-0.3.3/uniserde/common.py
+-rw-r--r--   0        0        0     6022 2023-07-29 22:20:24.589016 uniserde-0.3.3/uniserde/json_deserialize.py
+-rw-r--r--   0        0        0      600 2023-07-22 10:52:35.786683 uniserde-0.3.3/uniserde/lazy_wrapped.py
+-rw-r--r--   0        0        0     1974 2023-07-04 19:24:43.382018 uniserde-0.3.3/uniserde/objectid_proxy.py
+-rw-r--r--   0        0        0     8700 2023-07-29 22:20:20.432352 uniserde-0.3.3/uniserde/schema_mongodb.py
+-rw-r--r--   0        0        0     2150 2023-07-29 22:24:28.305621 uniserde-0.3.3/uniserde/serde_bson.py
+-rw-r--r--   0        0        0     2670 2023-07-28 13:42:15.594093 uniserde-0.3.3/uniserde/serde_class.py
+-rw-r--r--   0        0        0     5488 2023-07-29 22:21:45.548983 uniserde-0.3.3/uniserde/serde_json.py
+-rw-r--r--   0        0        0      487 2023-07-04 19:24:43.382018 uniserde-0.3.3/uniserde/typedefs.py
+-rw-r--r--   0        0        0     8549 1970-01-01 00:00:00.000000 uniserde-0.3.3/PKG-INFO
```

### Comparing `uniserde-0.3.2/README.md` & `uniserde-0.3.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -95,14 +95,15 @@
 | Optional       | value or `None` |                                                                                                                       |
 | Any            | as-is           |                                                                                                                       |
 | Literal[str]   | str             |                                                                                                                       |
 | enum.Enum      | str             | Enum values are mapped to their name (NOT value!)                                                                     |
 | custom class   | dict            | Each attribute is stored as key, in lowerCamelCase. If marked with `as_child`, an additional `type` field is added.   |
 | bytes          | str             | base64 encoded                                                                                                        |
 | datetime       | str             | as ISO 8601 - with timezone. Naïve datetimes are intentionally not supported. Do yourself a favor and don't use them. |
+| timedelta      | float           | duration, in seconds                                                                                                  |
 | Dict[str, ...] | dict            |                                                                                                                       |
 | bson.ObjectId  | str             |                                                                                                                       |
 
 ### BSON
 
 BSON uses the same conventions as JSON, with just a few changes
```

### Comparing `uniserde-0.3.2/pyproject.toml` & `uniserde-0.3.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "uniserde"
-version = "0.3.2"
+version = "0.3.3"
 description = "Convention based, effortless serialization and deserialization"
 authors = ["Jakob Pinterits <jakob.pinterits@gmail.com>"]
 license = "MIT"
 repository = "https://gitlab.com/Vivern/uniserde"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-dateutil = "^2.8.2"
 typing-extensions = "^4.7.1"
+pymongo = { version = "^4.4.0", optional = true }
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 black = "^22.3.0"
 isort = "^5.10.1"
 pre-commit = "^2.19.0"
 mongo-schema = "^1.0.0"
```

### Comparing `uniserde-0.3.2/uniserde/bson_deserialize.py` & `uniserde-0.3.3/uniserde/bson_deserialize.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from datetime import datetime, timezone
 from typing import *  # type: ignore
 
 from uniserde.objectid_proxy import ObjectId
 
-from . import caching_deserializer, case_convert, json_deserialize
+from . import caching_serdeserializer, case_convert, json_deserialize
 from .common import SerdeError
 from .typedefs import Bsonable
 
 __all__ = [
     "from_bson",
 ]
 
 
 T = TypeVar("T")
 
 
-class BsonDeserializer(caching_deserializer.CachingDeserializer[Bsonable]):
-    def _get_class_fields_and_deserializers(
+class BsonDeserializer(caching_serdeserializer.CachingSerDeserializer[Bsonable, Any]):
+    def _get_class_fields_and_handlers(
         self, value_type: Type
     ) -> Iterable[Tuple[str, str, Callable[[Bsonable, Type], Any]]]:
         for field_name_py, field_type in get_type_hints(value_type).items():
             if field_name_py == "id":
                 field_name_doc = "_id"
             else:
                 field_name_doc = case_convert.all_lower_to_camel_case(field_name_py)
@@ -49,17 +49,18 @@
     _passthrough_types = {
         bool,
         int,
         float,
         bytes,
         str,
         ObjectId,
-    }
-    _deserializer_cache = json_deserialize.JsonDeserializer._deserializer_cache.copy()  # type: ignore
-    _deserializer_cache[datetime] = _deserialize_datetime_from_datetime
+    }  # type: ignore
+
+    _handler_cache = json_deserialize.JsonDeserializer._handler_cache.copy()  # type: ignore
+    _handler_cache[datetime] = _deserialize_datetime_from_datetime  # type: ignore
     _override_method_name = "from_bson"
 
 
 def from_bson(
     value: Any,
     as_type: Type[T],
     *,
@@ -67,8 +68,8 @@
 ) -> T:
     deserializer = BsonDeserializer(
         custom_deserializers={
             t: lambda v, _: cb(v) for t, cb in custom_deserializers.items()
         }
     )
 
-    return deserializer.deserialize(value, as_type)
+    return deserializer.process(value, as_type)
```

### Comparing `uniserde-0.3.2/uniserde/case_convert.py` & `uniserde-0.3.3/uniserde/case_convert.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.2/uniserde/common.py` & `uniserde-0.3.3/uniserde/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import inspect
 import re
 from datetime import datetime
-from typing import Any, Callable, Dict, Iterable, Optional, Type, get_origin
+from typing import *  # type: ignore
 
 from .objectid_proxy import ObjectId
 
 Recur = Callable[[Any, Type], Any]
 Serializer = Callable[[Any, Type, Recur], Any]
 Deserializer = Callable[[Any, Type, Recur], Any]
```

### Comparing `uniserde-0.3.2/uniserde/json_deserialize.py` & `uniserde-0.3.3/uniserde/json_deserialize.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import base64
-from datetime import datetime
+from datetime import datetime, timedelta
 from typing import *  # type: ignore
 
 import dateutil.parser
 
-from . import caching_deserializer, case_convert
+from . import caching_serdeserializer, case_convert
 from .common import SerdeError
 from .objectid_proxy import ObjectId
 from .serde_json import Jsonable
 from .typedefs import Jsonable
 
 __all__ = [
     "from_json",
 ]
 
 
 T = TypeVar("T")
 
 
-class JsonDeserializer(caching_deserializer.CachingDeserializer[Jsonable]):
-    def _get_class_fields_and_deserializers(
+class JsonDeserializer(caching_serdeserializer.CachingSerDeserializer[Jsonable, Any]):
+    def _get_class_fields_and_handlers(
         self, value_type: Type
     ) -> Iterable[Tuple[str, str, Callable[[Jsonable, Type], Any]]]:
         for field_name_py, field_type in get_type_hints(value_type).items():
             yield (
                 field_name_py,
                 case_convert.all_lower_to_camel_case(field_name_py),
                 field_type,
@@ -56,42 +56,52 @@
             raise SerdeError(f"Expected date/time, got `{value}`") from None
 
         if result.tzinfo is None:
             raise SerdeError(f"The date/time value `{value}` is missing a timezone.")
 
         return result
 
+    def _deserialize_timedelta_from_float(
+        self,
+        value: Any,
+        value_type: Type[timedelta],
+    ) -> timedelta:
+        if not isinstance(value, (int, float)):
+            raise SerdeError(f"Expected number, got `{value}`")
+
+        return timedelta(seconds=value)
+
     def _deserialize_list_from_list(
         self,
         value: Any,
         value_type: Type[List],
     ) -> List[Any]:
         if not isinstance(value, list):
             raise SerdeError(f"Expected list, got `{value}`")
 
         subtype = get_args(value_type)[0]
-        child_deserializer = self._get_deserializer(subtype)
+        child_deserializer = self._get_handler(subtype)
 
         return [child_deserializer(self, v, subtype) for v in value]
 
     def _deserialize_dict_from_dict(
         self,
         value: Any,
         value_type: Type[Dict],
     ) -> Dict[Any, Any]:
         if not isinstance(value, dict):
             raise SerdeError(f"Expected dict, got `{value}`")
 
         subtypes = get_args(value_type)
 
         key_type = subtypes[0]
-        key_deserializer = self._get_deserializer(key_type)
+        key_deserializer = self._get_handler(key_type)
 
         value_type = subtypes[1]
-        value_deserializer = self._get_deserializer(value_type)
+        value_deserializer = self._get_handler(value_type)
 
         return {
             key_deserializer(self, k, key_type): value_deserializer(self, v, value_type)
             for k, v in value.items()
         }
 
     def _deserialize_object_id_from_str(
@@ -113,15 +123,15 @@
         self,
         value: Any,
         value_type: Type,
     ) -> Any:
         if value is None:
             return None
 
-        return self.deserialize(value, get_args(value_type)[0])
+        return self.process(value, get_args(value_type)[0])
 
     def _deserialize_any(
         self,
         value: Any,
         value_type: Type[Any],
     ) -> Any:
         return value
@@ -148,49 +158,48 @@
         subtypes = get_args(value_type)
 
         if len(value) != len(subtypes):
             raise SerdeError(
                 f"Expected list of length {len(subtypes)}, but received one of length {len(value)}"
             )
 
-        return tuple(
-            self.deserialize(v, subtype) for v, subtype in zip(value, subtypes)
-        )
+        return tuple(self.process(v, subtype) for v, subtype in zip(value, subtypes))
 
     def _deserialize_set_from_list(
         self,
         value: Any,
         value_type: Type[Set],
     ) -> Set:
         if not isinstance(value, list):
             raise SerdeError(f"Expected list, got `{value}`")
 
         subtype = get_args(value_type)[0]
 
-        return set(self.deserialize(v, subtype) for v in value)
+        return set(self.process(v, subtype) for v in value)
 
     _passthrough_types = {
         bool,
         int,
         float,
         str,
-    }
+    }  # type: ignore
 
-    _deserializer_cache = {
+    _handler_cache = {
         bytes: _deserialize_bytes_from_str,
         datetime: _deserialize_datetime_from_str,
+        timedelta: _deserialize_timedelta_from_float,
         list: _deserialize_list_from_list,
         dict: _deserialize_dict_from_dict,
         Union: _deserialize_optional,
         Any: _deserialize_any,
         ObjectId: _deserialize_object_id_from_str,
         Literal: _deserialize_literal_as_is,
         tuple: _deserialize_tuple_from_list,
         set: _deserialize_set_from_list,
-    }
+    }  # type: ignore
 
     _override_method_name = "from_json"
 
 
 def from_json(
     value: Any,
     as_type: Type[T],
@@ -199,8 +208,8 @@
 ) -> T:
     deserializer = JsonDeserializer(
         custom_deserializers={
             t: lambda v, _: cb(v) for t, cb in custom_deserializers.items()
         }
     )
 
-    return deserializer.deserialize(value, as_type)
+    return deserializer.process(value, as_type)
```

### Comparing `uniserde-0.3.2/uniserde/objectid_proxy.py` & `uniserde-0.3.3/uniserde/objectid_proxy.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.2/uniserde/serde_bson.py` & `uniserde-0.3.3/uniserde/serde_bson.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from typing import Any, Dict, Optional
+from typing import *  # type: ignore
 
 from . import serde_class, serde_json
 from .common import *
 from .objectid_proxy import ObjectId
 from .typedefs import Bsonable
 
 __all__ = [
```

### Comparing `uniserde-0.3.2/uniserde/serde_class.py` & `uniserde-0.3.3/uniserde/serde_class.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Any, Callable, Dict, Optional, Type, TypeVar
+from typing import *  # type: ignore
 
 import uniserde
 
 T = TypeVar("T", bound="Serde")
 
 
 class Serde:
```

### Comparing `uniserde-0.3.2/uniserde/serde_json.py` & `uniserde-0.3.3/uniserde/serde_json.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import base64
 import inspect
 import typing
-from datetime import datetime
+from datetime import datetime, timedelta
 from enum import Enum
-from typing import Any, Dict, List, Literal, Tuple, Type, Union
+from typing import *  # type: ignore
 
 from . import case_convert, serde_class
 from .common import *
 from .objectid_proxy import ObjectId
 from .typedefs import Jsonable
 
 __all__ = [
@@ -68,14 +68,23 @@
     assert isinstance(value, datetime), value
     assert (
         value.tzinfo is not None
     ), f"Encountered datetime without a timezone. Please always set timezones, or expect hard to find bugs."
     return value.isoformat()
 
 
+def serialize_timedelta_to_float(
+    value: Any,
+    value_type: Type,
+    recur: Recur,
+) -> float:
+    assert isinstance(value, timedelta), value
+    return value.total_seconds()
+
+
 def serialize_list_to_list(
     value: Any,
     value_type: Type,
     recur: Recur,
 ) -> List[Any]:
     assert isinstance(value, list), value
     return [recur(v, typing.get_args(value_type)[0]) for v in value]
@@ -194,14 +203,15 @@
 JSON_SERIALIZERS: Dict[Type, Serializer] = {
     bool: serialize_bool_to_bool,
     int: serialize_int_to_int,
     float: serialize_float_to_float,
     bytes: serialize_bytes_to_str,
     str: serialize_str_to_str,
     datetime: serialize_datetime_to_str,
+    timedelta: serialize_timedelta_to_float,
     list: serialize_list_to_list,
     dict: serialize_dict_to_dict,
     Union: serialize_optional,
     Any: serialize_any,
     ObjectId: serialize_object_id_to_str,
     Literal: serialize_literal_as_is,
     tuple: serialize_tuple_as_list,
```

### Comparing `uniserde-0.3.2/PKG-INFO` & `uniserde-0.3.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: uniserde
-Version: 0.3.2
+Version: 0.3.3
 Summary: Convention based, effortless serialization and deserialization
 Home-page: https://gitlab.com/Vivern/uniserde
 License: MIT
 Author: Jakob Pinterits
 Author-email: jakob.pinterits@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pymongo (>=4.4.0,<5.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: typing-extensions (>=4.7.1,<5.0.0)
 Project-URL: Repository, https://gitlab.com/Vivern/uniserde
 Description-Content-Type: text/markdown
 
 # Convention based, effortless serialization and deserialization
 
@@ -114,14 +115,15 @@
 | Optional       | value or `None` |                                                                                                                       |
 | Any            | as-is           |                                                                                                                       |
 | Literal[str]   | str             |                                                                                                                       |
 | enum.Enum      | str             | Enum values are mapped to their name (NOT value!)                                                                     |
 | custom class   | dict            | Each attribute is stored as key, in lowerCamelCase. If marked with `as_child`, an additional `type` field is added.   |
 | bytes          | str             | base64 encoded                                                                                                        |
 | datetime       | str             | as ISO 8601 - with timezone. Naïve datetimes are intentionally not supported. Do yourself a favor and don't use them. |
+| timedelta      | float           | duration, in seconds                                                                                                  |
 | Dict[str, ...] | dict            |                                                                                                                       |
 | bson.ObjectId  | str             |                                                                                                                       |
 
 ### BSON
 
 BSON uses the same conventions as JSON, with just a few changes
```

