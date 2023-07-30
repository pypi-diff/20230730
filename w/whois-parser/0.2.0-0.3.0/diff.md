# Comparing `tmp/whois_parser-0.2.0.tar.gz` & `tmp/whois_parser-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whois_parser-0.2.0.tar", max compression
+gzip compressed data, was "whois_parser-0.3.0.tar", max compression
```

## Comparing `whois_parser-0.2.0.tar` & `whois_parser-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1070 2023-07-09 01:02:06.011940 whois_parser-0.2.0/LICENSE
--rw-r--r--   0        0        0     1952 2023-07-09 01:02:06.011940 whois_parser-0.2.0/README.md
--rw-r--r--   0        0        0      834 2023-07-09 01:02:25.140238 whois_parser-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      153 2023-07-09 01:02:06.011940 whois_parser-0.2.0/whois_parser/__init__.py
--rw-r--r--   0        0        0      978 2023-07-09 01:02:06.011940 whois_parser-0.2.0/whois_parser/dataclasses.py
--rw-r--r--   0        0        0     1302 2023-07-09 01:02:06.011940 whois_parser-0.2.0/whois_parser/parser.py
--rw-r--r--   0        0        0      136 2023-07-09 01:02:06.011940 whois_parser-0.2.0/whois_parser/parsers/__init__.py
--rw-r--r--   0        0        0    10889 2023-07-09 01:02:06.011940 whois_parser-0.2.0/whois_parser/parsers/abstract.py
--rw-r--r--   0        0        0     6385 2023-07-09 01:02:06.011940 whois_parser-0.2.0/whois_parser/parsers/base.py
--rw-r--r--   0        0        0      406 2023-07-09 01:02:06.011940 whois_parser-0.2.0/whois_parser/parsers/be.py
--rw-r--r--   0        0        0      117 2023-07-09 01:02:06.011940 whois_parser-0.2.0/whois_parser/parsers/constants.py
--rw-r--r--   0        0        0     1867 2023-07-09 01:02:06.011940 whois_parser-0.2.0/whois_parser/parsers/jp.py
--rw-r--r--   0        0        0      399 2023-07-09 01:02:06.011940 whois_parser-0.2.0/whois_parser/parsers/uk.py
--rw-r--r--   0        0        0     1536 2023-07-09 01:02:06.011940 whois_parser-0.2.0/whois_parser/parsers/utils.py
--rw-r--r--   0        0        0     2578 1970-01-01 00:00:00.000000 whois_parser-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-30 07:47:26.460525 whois_parser-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1952 2023-07-30 07:47:26.460525 whois_parser-0.3.0/README.md
+-rw-r--r--   0        0        0      836 2023-07-30 07:47:44.112374 whois_parser-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      153 2023-07-30 07:47:26.464525 whois_parser-0.3.0/whois_parser/__init__.py
+-rw-r--r--   0        0        0     1013 2023-07-30 07:47:26.464525 whois_parser-0.3.0/whois_parser/dataclasses.py
+-rw-r--r--   0        0        0     1302 2023-07-30 07:47:26.464525 whois_parser-0.3.0/whois_parser/parser.py
+-rw-r--r--   0        0        0      136 2023-07-30 07:47:26.464525 whois_parser-0.3.0/whois_parser/parsers/__init__.py
+-rw-r--r--   0        0        0    11214 2023-07-30 07:47:26.464525 whois_parser-0.3.0/whois_parser/parsers/abstract.py
+-rw-r--r--   0        0        0     6385 2023-07-30 07:47:26.464525 whois_parser-0.3.0/whois_parser/parsers/base.py
+-rw-r--r--   0        0        0      406 2023-07-30 07:47:26.464525 whois_parser-0.3.0/whois_parser/parsers/be.py
+-rw-r--r--   0        0        0      117 2023-07-30 07:47:26.464525 whois_parser-0.3.0/whois_parser/parsers/constants.py
+-rw-r--r--   0        0        0     1867 2023-07-30 07:47:26.464525 whois_parser-0.3.0/whois_parser/parsers/jp.py
+-rw-r--r--   0        0        0      399 2023-07-30 07:47:26.464525 whois_parser-0.3.0/whois_parser/parsers/uk.py
+-rw-r--r--   0        0        0     1536 2023-07-30 07:47:26.464525 whois_parser-0.3.0/whois_parser/parsers/utils.py
+-rw-r--r--   0        0        0      733 2023-07-30 07:47:26.464525 whois_parser-0.3.0/whois_parser/settings.py
+-rw-r--r--   0        0        0     2578 1970-01-01 00:00:00.000000 whois_parser-0.3.0/PKG-INFO
```

### Comparing `whois_parser-0.2.0/LICENSE` & `whois_parser-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `whois_parser-0.2.0/README.md` & `whois_parser-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `whois_parser-0.2.0/pyproject.toml` & `whois_parser-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "whois-parser"
-version = "0.2.0"
+version = "0.3.0"
 description = "Yet another whois parser for Python"
 authors = ["Manabu Niseki <manabu.niseki@gmail.com>"]
 homepage = "https://github.com/ninoseki/whois-parser"
 repository = "https://github.com/ninoseki/whois-parser"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 dateparser = ">=1.1,<2.0"
-pyparsing = ">=3.0,<4.0"
+pyparsing = ">=3.1,<4.0"
 
 [tool.poetry.dev-dependencies]
-black = "^23.3"
+black = "^23.7"
 coveralls = "^3.3.1"
 isort = "^5.12"
 mypy = "^1.4"
 pre-commit = "^3.3"
 pytest = "^7.4"
 pytest-asyncio = "^0.21"
 pytest-cov = "^4.1"
 pytest-mock = "^3.11"
-pytest-randomly = "^3.12"
-pytest-sugar = "^0.9"
+pytest-randomly = "^3.13"
 pyupgrade = "^3.9"
+urllib3 = ">=1.26,<2.0"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 
 [build-system]
 requires = ["poetry-core", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `whois_parser-0.2.0/whois_parser/dataclasses.py` & `whois_parser-0.3.0/whois_parser/dataclasses.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,7 +46,9 @@
 
     domain: Optional[str] = None
     registrar: Optional[str] = None
 
     expires_at: Optional[Union[datetime, str]] = None
     registered_at: Optional[Union[datetime, str]] = None
     updated_at: Optional[Union[datetime, str]] = None
+
+    is_rate_limited: bool = False
```

### Comparing `whois_parser-0.2.0/whois_parser/parser.py` & `whois_parser-0.3.0/whois_parser/parser.py`

 * *Files identical despite different names*

### Comparing `whois_parser-0.2.0/whois_parser/parsers/abstract.py` & `whois_parser-0.3.0/whois_parser/parsers/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABC, abstractmethod
 from datetime import datetime
 from typing import Optional, Union
 
 from pyparsing import ParserElement
 
-from .. import dataclasses
+from .. import dataclasses, settings
 from .constants import ANY_CHARACTERS, DEILIMITER, SPACE_OR_TAB
 from .utils import build_common_prefix_pattern, find, find_all, parse_datetime
 
 
 def normalize_raw_text(raw_text: str) -> str:
     """Normalize raw text
 
@@ -75,14 +75,15 @@
             name_servers=self._find_name_servers(),
             registered_at=self._find_registered_at(),
             registrant=self._find_registrant(),
             registrar=self._find_registrar(),
             statuses=self._find_statuses(),
             tech=self._find_tech(),
             updated_at=self._find_updated_at(),
+            is_rate_limited=self._is_rate_limited(),
         )
 
     @abstractmethod
     def _find_tech(self) -> dataclasses.Tech:
         """Find tech fields
 
         Returns:
@@ -332,7 +333,15 @@
                     delimiter=delimiter,
                 )
             )
             if len(values) > 0:
                 return values
 
         return []
+
+    def _is_rate_limited(self) -> bool:
+        """Check whether rate limited or not.
+
+        Returns:
+            bool: Returns True if it's rate limited. Otherwise False.
+        """
+        return self.raw_text.strip() in settings.WHOIS_RATE_LIMIT_MESSAGES
```

### Comparing `whois_parser-0.2.0/whois_parser/parsers/base.py` & `whois_parser-0.3.0/whois_parser/parsers/base.py`

 * *Files identical despite different names*

### Comparing `whois_parser-0.2.0/whois_parser/parsers/jp.py` & `whois_parser-0.3.0/whois_parser/parsers/jp.py`

 * *Files identical despite different names*

### Comparing `whois_parser-0.2.0/whois_parser/parsers/utils.py` & `whois_parser-0.3.0/whois_parser/parsers/utils.py`

 * *Files identical despite different names*

### Comparing `whois_parser-0.2.0/PKG-INFO` & `whois_parser-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: whois-parser
-Version: 0.2.0
+Version: 0.3.0
 Summary: Yet another whois parser for Python
 Home-page: https://github.com/ninoseki/whois-parser
 Author: Manabu Niseki
 Author-email: manabu.niseki@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dateparser (>=1.1,<2.0)
-Requires-Dist: pyparsing (>=3.0,<4.0)
+Requires-Dist: pyparsing (>=3.1,<4.0)
 Project-URL: Repository, https://github.com/ninoseki/whois-parser
 Description-Content-Type: text/markdown
 
 # whois-parser
 
 [![PyPI version](https://badge.fury.io/py/whois-parser.svg)](https://badge.fury.io/py/whois-parser)
 [![Python CI](https://github.com/ninoseki/whois-parser/actions/workflows/test.yml/badge.svg)](https://github.com/ninoseki/whois-parser/actions/workflows/test.yml)
```

