# Comparing `tmp/pydantic_xml-2.0.0a2.tar.gz` & `tmp/pydantic_xml-2.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_xml-2.0.0a2.tar", max compression
+gzip compressed data, was "pydantic_xml-2.0.0b1.tar", max compression
```

## Comparing `pydantic_xml-2.0.0a2.tar` & `pydantic_xml-2.0.0b1.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1211 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/LICENSE
--rw-r--r--   0        0        0     3335 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/README.rst
--rw-r--r--   0        0        0      453 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/__init__.py
--rw-r--r--   0        0        0      489 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/config.py
--rw-r--r--   0        0        0       80 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/element/__init__.py
--rw-r--r--   0        0        0    13335 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/element/element.py
--rw-r--r--   0        0        0      374 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/element/native/__init__.py
--rw-r--r--   0        0        0     1671 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/element/native/lxml.py
--rw-r--r--   0        0        0     1173 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/element/native/std.py
--rw-r--r--   0        0        0      712 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/errors.py
--rw-r--r--   0        0        0    12352 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/model.py
--rw-r--r--   0        0        0        0 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/py.typed
--rw-r--r--   0        0        0       36 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/serializers/__init__.py
--rw-r--r--   0        0        0       99 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/serializers/factories/__init__.py
--rw-r--r--   0        0        0     3386 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/serializers/factories/heterogeneous.py
--rw-r--r--   0        0        0     3290 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/serializers/factories/homogeneous.py
--rw-r--r--   0        0        0     5492 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/serializers/factories/mapping.py
--rw-r--r--   0        0        0    11466 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/serializers/factories/model.py
--rw-r--r--   0        0        0     5561 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/serializers/factories/primitive.py
--rw-r--r--   0        0        0     1428 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/serializers/factories/typed_mapping.py
--rw-r--r--   0        0        0     5135 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/serializers/factories/union.py
--rw-r--r--   0        0        0     2659 2023-07-24 18:53:31.760739 pydantic_xml-2.0.0a2/pydantic_xml/serializers/factories/wrapper.py
--rw-r--r--   0        0        0     9774 2023-07-24 18:53:31.760739 pydantic_xml-2.0.0a2/pydantic_xml/serializers/serializer.py
--rw-r--r--   0        0        0      322 2023-07-24 18:53:31.760739 pydantic_xml-2.0.0a2/pydantic_xml/typedefs.py
--rw-r--r--   0        0        0     2131 2023-07-24 18:53:31.760739 pydantic_xml-2.0.0a2/pydantic_xml/utils.py
--rw-r--r--   0        0        0     1883 2023-07-24 18:53:31.760739 pydantic_xml-2.0.0a2/pyproject.toml
--rw-r--r--   0        0        0     4823 1970-01-01 00:00:00.000000 pydantic_xml-2.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-07-30 08:33:00.589908 pydantic_xml-2.0.0b1/LICENSE
+-rw-r--r--   0        0        0     3335 2023-07-30 08:33:00.589908 pydantic_xml-2.0.0b1/README.rst
+-rw-r--r--   0        0        0      453 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/__init__.py
+-rw-r--r--   0        0        0      489 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/config.py
+-rw-r--r--   0        0        0       80 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/element/__init__.py
+-rw-r--r--   0        0        0    14764 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/element/element.py
+-rw-r--r--   0        0        0      374 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/element/native/__init__.py
+-rw-r--r--   0        0        0     1671 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/element/native/lxml.py
+-rw-r--r--   0        0        0     1173 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/element/native/std.py
+-rw-r--r--   0        0        0      712 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/errors.py
+-rw-r--r--   0        0        0    12352 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/model.py
+-rw-r--r--   0        0        0        0 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/py.typed
+-rw-r--r--   0        0        0       36 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/serializers/__init__.py
+-rw-r--r--   0        0        0      113 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/__init__.py
+-rw-r--r--   0        0        0     3386 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/heterogeneous.py
+-rw-r--r--   0        0        0     3290 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/homogeneous.py
+-rw-r--r--   0        0        0     5492 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/mapping.py
+-rw-r--r--   0        0        0    11717 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/model.py
+-rw-r--r--   0        0        0     5639 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/primitive.py
+-rw-r--r--   0        0        0     5081 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/tagged_union.py
+-rw-r--r--   0        0        0     1428 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/typed_mapping.py
+-rw-r--r--   0        0        0     5135 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/union.py
+-rw-r--r--   0        0        0     2659 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/wrapper.py
+-rw-r--r--   0        0        0    10099 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/serializers/serializer.py
+-rw-r--r--   0        0        0      322 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/typedefs.py
+-rw-r--r--   0        0        0     2131 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pydantic_xml/utils.py
+-rw-r--r--   0        0        0     1946 2023-07-30 08:33:00.593908 pydantic_xml-2.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0     4896 1970-01-01 00:00:00.000000 pydantic_xml-2.0.0b1/PKG-INFO
```

### Comparing `pydantic_xml-2.0.0a2/LICENSE` & `pydantic_xml-2.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0a2/README.rst` & `pydantic_xml-2.0.0b1/README.rst`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0a2/pydantic_xml/element/element.py` & `pydantic_xml-2.0.0b1/pydantic_xml/element/element.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,40 @@
         """
         Checks if the element is empty (has not text, attributes or sub-elements).
 
         :return: `True` if the element is empty otherwise `False`.
         """
 
     @abc.abstractmethod
+    def get_attrib(self, name: str) -> Optional[str]:
+        """
+        Returns an attribute from the xml element matching `name`.
+
+        :return: element attribute
+        """
+
+    @abc.abstractmethod
+    def find_element(
+            self,
+            tag: str,
+            search_mode: 'SearchMode',
+            look_behind: bool = True,
+            step_forward: bool = True,
+    ) -> Optional['XmlElement[Any]']:
+        """
+        Searches for an element with the provided tag.
+
+        :param tag: element tag to be found or created
+        :param search_mode: element search mode
+        :param look_behind: look in the previous element
+        :param step_forward: increment next element index
+        :return: xml element
+        """
+
+    @abc.abstractmethod
     def pop_text(self) -> Optional[str]:
         """
         Extracts the text from the xml element.
         All subsequent calls return `None`.
 
         :return: element text
         """
@@ -255,14 +281,17 @@
     def set_attributes(self, attributes: Dict[str, str]) -> None:
         self._state.attrib = dict(attributes)
 
     def append_element(self, element: 'XmlElement[NativeElement]') -> None:
         self._state.elements.append(element)
         self._state.next_element_idx += 1
 
+    def get_attrib(self, name: str) -> Optional[str]:
+        return self._state.attrib.get(name, None) if self._state.attrib else None
+
     def pop_text(self) -> Optional[str]:
         result, self._state.text = self._state.text, None
 
         return result
 
     def pop_attrib(self, name: str) -> Optional[str]:
         return self._state.attrib.pop(name, None) if self._state.attrib else None
@@ -271,43 +300,49 @@
         result, self._state.attrib = self._state.attrib, None
 
         return result
 
     def pop_element(self, tag: str, search_mode: 'SearchMode') -> Optional['XmlElement[NativeElement]']:
         searcher: Searcher[NativeElement] = get_searcher(search_mode)
 
-        return searcher(self._state, tag, False)
+        return searcher(self._state, tag, False, True)
 
     def find_sub_element(self, path: Sequence[str], search_mode: 'SearchMode') -> Optional['XmlElement[NativeElement]']:
         assert len(path) > 0, "path can't be empty"
 
         root, path = path[0], path[1:]
-        element = self._find_element(root, search_mode)
+        element = self.find_element(root, search_mode)
         if element and path:
             return element.find_sub_element(path, search_mode)
 
         return element
 
     def find_element_or_create(
             self,
             tag: str,
             search_mode: 'SearchMode',
             nsmap: Optional[NsMap],
     ) -> 'XmlElement[NativeElement]':
-        if (sub_element := self._find_element(tag, search_mode)) is None:
+        if (sub_element := self.find_element(tag, search_mode)) is None:
             sub_element = self.make_element(tag=tag, nsmap=nsmap)
             self._state.elements.append(sub_element)
             self._state.next_element_idx += 1
 
         return sub_element
 
-    def _find_element(self, tag: str, search_mode: 'SearchMode') -> Optional['XmlElement[NativeElement]']:
+    def find_element(
+            self,
+            tag: str,
+            search_mode: 'SearchMode',
+            look_behind: bool = True,
+            step_forward: bool = True,
+    ) -> Optional['XmlElement[NativeElement]']:
         searcher: Searcher[NativeElement] = get_searcher(search_mode)
 
-        return searcher(self._state, tag, True)
+        return searcher(self._state, tag, look_behind, step_forward)
 
 
 class SearchMode(str, Enum):
     """
     Element search mode.
 
     strict: search for an element sequentially one by one.
@@ -316,15 +351,15 @@
     """
 
     STRICT = 'strict'
     ORDERED = 'ordered'
     UNORDERED = 'unordered'
 
 
-Searcher = Callable[[XmlElement.State[NativeElement], str, bool], Optional[XmlElement[NativeElement]]]
+Searcher = Callable[[XmlElement.State[NativeElement], str, bool, bool], Optional[XmlElement[NativeElement]]]
 
 
 def get_searcher(search_mode: SearchMode) -> Searcher[NativeElement]:
     if search_mode == SearchMode.STRICT:
         return strict_search
     elif search_mode == SearchMode.ORDERED:
         return ordered_search
@@ -334,93 +369,105 @@
         raise AssertionError("unreachable")
 
 
 def strict_search(
         state: XmlElement.State[NativeElement],
         tag: str,
         look_behind: bool = False,
+        step_forward: bool = True,
 ) -> Optional[XmlElement[NativeElement]]:
     """
     Searches for a sub-element sequentially one by one.
 
     :param state: element state
     :param tag: sub-element tag for be searched for
-    :param look_behind: look for a previous element
+    :param look_behind: look in the previous element
+    :param step_forward: increment next element index
     :return: found element or `None` if the element not found
     """
 
     result: Optional[XmlElement[NativeElement]] = None
 
     if look_behind and (result := _look_behind(state, tag)) is not None:
         return result
 
     if state.next_element_idx < len(state.elements) and state.elements[state.next_element_idx].tag == tag:
         result = state.elements[state.next_element_idx]
-        state.next_element_idx += 1
+        if step_forward:
+            state.next_element_idx += 1
 
     return result
 
 
 def ordered_search(
         state: XmlElement.State[NativeElement],
         tag: str,
         look_behind: bool = False,
+        step_forward: bool = True,
 ) -> Optional[XmlElement[NativeElement]]:
     """
     Searches for an element sequentially skipping unmatched ones.
 
     :param state: element state
     :param tag: sub-element tag for be searched for
-    :param look_behind: look for a previous element
+    :param look_behind: look in the previous element
+    :param step_forward: increment next element index
     :return: found element or `None` if the element not found
     """
 
     result: Optional[XmlElement[Any]] = None
 
     if look_behind and (result := _look_behind(state, tag)) is not None:
         return result
 
     next_element_idx = state.next_element_idx
     while next_element_idx < len(state.elements):
         element = state.elements[next_element_idx]
         next_element_idx += 1
 
         if element.tag == tag:
-            state.next_element_idx = next_element_idx
+            if step_forward:
+                state.next_element_idx = next_element_idx
+
             result = element
             break
 
     return result
 
 
 def unordered_search(
         state: XmlElement.State[NativeElement],
         tag: str,
         look_behind: bool = False,
+        step_forward: bool = True,
 ) -> Optional[XmlElement[NativeElement]]:
     """
     Searches search for an element ignoring elements order.
 
     :param state: element state
     :param tag: sub-element tag for be searched for
-    :param look_behind: look for a previous element
+    :param look_behind: look in the previous element
+    :param step_forward: increment next element index
     :return: found element or `None` if the requested element not found
     """
 
     result: Optional[XmlElement[NativeElement]] = None
 
     if look_behind and (result := _look_behind(state, tag)) is not None:
         return result
 
     for idx in range(state.next_element_idx, len(state.elements)):
         element = state.elements[idx]
         if element.tag == tag:
             state.elements[state.next_element_idx], state.elements[idx] = \
                 state.elements[idx], state.elements[state.next_element_idx]
-            state.next_element_idx += 1
+
+            if step_forward:
+                state.next_element_idx += 1
+
             result = element
             break
 
     return result
 
 
 def _look_behind(state: XmlElement.State[NativeElement], tag: str) -> Optional[XmlElement[NativeElement]]:
```

### Comparing `pydantic_xml-2.0.0a2/pydantic_xml/element/native/lxml.py` & `pydantic_xml-2.0.0b1/pydantic_xml/element/native/lxml.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0a2/pydantic_xml/element/native/std.py` & `pydantic_xml-2.0.0b1/pydantic_xml/element/native/std.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0a2/pydantic_xml/errors.py` & `pydantic_xml-2.0.0b1/pydantic_xml/errors.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0a2/pydantic_xml/model.py` & `pydantic_xml-2.0.0b1/pydantic_xml/model.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0a2/pydantic_xml/serializers/factories/heterogeneous.py` & `pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/heterogeneous.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0a2/pydantic_xml/serializers/factories/homogeneous.py` & `pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/homogeneous.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0a2/pydantic_xml/serializers/factories/mapping.py` & `pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/mapping.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0a2/pydantic_xml/serializers/factories/model.py` & `pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import abc
 import typing
-from typing import Any, Dict, Optional, Type
+from typing import Any, Dict, Mapping, Optional, Type
 
 from pydantic_core import core_schema as pcs
 
 import pydantic_xml as pxml
 from pydantic_xml import errors
 from pydantic_xml.element import XmlElementReader, XmlElementWriter
 from pydantic_xml.serializers.serializer import SearchMode, Serializer, XmlEntityInfoP
@@ -107,14 +107,18 @@
     def element_name(self) -> str:
         return self._element_name
 
     @property
     def nsmap(self) -> Optional[NsMap]:
         return self._nsmap
 
+    @property
+    def fields_serializers(self) -> Mapping[str, Serializer]:
+        return self._field_serializers
+
     def serialize(
             self,
             element: XmlElementWriter,
             value: 'pxml.BaseXmlModel',
             encoded: Dict[str, Any],
             *,
             skip_empty: bool = False,
@@ -257,14 +261,18 @@
         self._computed = computed
 
     @property
     def model(self) -> Type['pxml.BaseXmlModel']:
         return self._model
 
     @property
+    def model_serializer(self) -> Optional[BaseModelSerializer]:
+        return self._model.__xml_serializer__
+
+    @property
     def element_name(self) -> str:
         return self._element_name
 
     @property
     def nsmap(self) -> Optional[NsMap]:
         return self._nsmap
```

### Comparing `pydantic_xml-2.0.0a2/pydantic_xml/serializers/factories/primitive.py` & `pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/primitive.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,18 @@
 
         return cls(name, ns, nsmap, computed)
 
     def __init__(self, name: str, ns: Optional[str], nsmap: Optional[NsMap], computed: bool):
         self._attr_name = QName.from_alias(tag=name, ns=ns, nsmap=nsmap, is_attr=True).uri
         self._computed = computed
 
+    @property
+    def attr_name(self) -> str:
+        return self._attr_name
+
     def serialize(
             self, element: XmlElementWriter, value: Any, encoded: Any, *, skip_empty: bool = False,
     ) -> Optional[XmlElementWriter]:
         if value is None and skip_empty:
             return element
 
         element.set_attribute(self._attr_name, str(encoded))
```

### Comparing `pydantic_xml-2.0.0a2/pydantic_xml/serializers/factories/typed_mapping.py` & `pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/typed_mapping.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0a2/pydantic_xml/serializers/factories/union.py` & `pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/union.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0a2/pydantic_xml/serializers/factories/wrapper.py` & `pydantic_xml-2.0.0b1/pydantic_xml/serializers/factories/wrapper.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0a2/pydantic_xml/serializers/serializer.py` & `pydantic_xml-2.0.0b1/pydantic_xml/serializers/serializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,30 +20,32 @@
     PRIMITIVE = 1
     MODEL = 2
     HOMOGENEOUS_COLLECTION = 3
     HETEROGENEOUS_COLLECTION = 4
     MAPPING = 5
     TYPED_MAPPING = 6
     UNION = 7
-    DEFINITIONS = 8
-    DEFINITION_REF = 9
-    JSON_OR_PYTHON = 10
+    TAGGED_UNION = 8
+    DEFINITIONS = 9
+    DEFINITION_REF = 10
+    JSON_OR_PYTHON = 11
 
 
 TYPE_FAMILY = {
     'none':             SchemaTypeFamily.PRIMITIVE,
     'bool':             SchemaTypeFamily.PRIMITIVE,
     'int':              SchemaTypeFamily.PRIMITIVE,
     'float':            SchemaTypeFamily.PRIMITIVE,
     'str':              SchemaTypeFamily.PRIMITIVE,
     'bytes':            SchemaTypeFamily.PRIMITIVE,
     'date':             SchemaTypeFamily.PRIMITIVE,
     'time':             SchemaTypeFamily.PRIMITIVE,
     'datetime':         SchemaTypeFamily.PRIMITIVE,
     'timedelta':        SchemaTypeFamily.PRIMITIVE,
+    'uuid':             SchemaTypeFamily.PRIMITIVE,
     'url':              SchemaTypeFamily.PRIMITIVE,
     'multi-host-url':   SchemaTypeFamily.PRIMITIVE,
     'json':             SchemaTypeFamily.PRIMITIVE,
     'literal':          SchemaTypeFamily.PRIMITIVE,
     'lax-or-strict':    SchemaTypeFamily.PRIMITIVE,
     'is-instance':      SchemaTypeFamily.PRIMITIVE,
 
@@ -56,14 +58,15 @@
 
     'tuple-positional': SchemaTypeFamily.HETEROGENEOUS_COLLECTION,
 
     'dict':             SchemaTypeFamily.MAPPING,
     'typed-dict':       SchemaTypeFamily.TYPED_MAPPING,
 
     'union':            SchemaTypeFamily.UNION,
+    'tagged-union':     SchemaTypeFamily.TAGGED_UNION,
 
     'function-before':  SchemaTypeFamily.META,
     'function-after':   SchemaTypeFamily.META,
     'function-wrap':    SchemaTypeFamily.META,
     'function-plain':   SchemaTypeFamily.META,
     'default':          SchemaTypeFamily.META,
     'nullable':         SchemaTypeFamily.META,
@@ -232,14 +235,18 @@
             schema = typing.cast(pcs.TypedDictSchema, schema)
             return factories.typed_mapping.from_core_schema(schema, ctx)
 
         elif type_family is SchemaTypeFamily.UNION:
             schema = typing.cast(pcs.UnionSchema, schema)
             return factories.union.from_core_schema(schema, ctx)
 
+        elif type_family is SchemaTypeFamily.TAGGED_UNION:
+            schema = typing.cast(pcs.TaggedUnionSchema, schema)
+            return factories.tagged_union.from_core_schema(schema, ctx)
+
         else:
             raise AssertionError("unreachable")
 
     @abc.abstractmethod
     def serialize(
             self, element: XmlElementWriter, value: Any, encoded: Any, *, skip_empty: bool = False,
     ) -> Optional[XmlElementWriter]:
```

### Comparing `pydantic_xml-2.0.0a2/pydantic_xml/utils.py` & `pydantic_xml-2.0.0b1/pydantic_xml/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0a2/pyproject.toml` & `pydantic_xml-2.0.0b1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-xml"
-version = "2.0.0a2"
+version = "2.0.0b1"
 description = "pydantic xml extension"
 authors = ["Dmitry Pershin <dapper1291@gmail.com>"]
 license = "Unlicense"
 readme = "README.rst"
 homepage = "https://github.com/dapper91/pydantic-xml"
 repository = "https://github.com/dapper91/pydantic-xml"
 documentation = "https://github.com/dapper91/pydantic-xml"
@@ -13,14 +13,16 @@
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "License :: Public Domain",
     "Topic :: Software Development :: Libraries",
+    'Framework :: Pydantic',
+    'Framework :: Pydantic :: 2',
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
```

### Comparing `pydantic_xml-2.0.0a2/PKG-INFO` & `pydantic_xml-2.0.0b1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: pydantic-xml
-Version: 2.0.0a2
+Version: 2.0.0b1
 Summary: pydantic xml extension
 Home-page: https://github.com/dapper91/pydantic-xml
 License: Unlicense
 Keywords: pydantic,xml,serialization,deserialization,parsing,lxml
 Author: Dmitry Pershin
 Author-email: dapper1291@gmail.com
 Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: Pydantic
+Classifier: Framework :: Pydantic :: 2
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: License :: Public Domain
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

