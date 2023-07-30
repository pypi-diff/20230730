# Comparing `tmp/pydiscovergy-2.0.2.tar.gz` & `tmp/pydiscovergy-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydiscovergy-2.0.2.tar", max compression
+gzip compressed data, was "pydiscovergy-2.0.3.tar", max compression
```

## Comparing `pydiscovergy-2.0.2.tar` & `pydiscovergy-2.0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1081 2023-07-25 16:50:27.914903 pydiscovergy-2.0.2/LICENSE
--rw-r--r--   0        0        0      575 2023-07-25 16:50:27.914903 pydiscovergy-2.0.2/README.md
--rw-r--r--   0        0        0      102 2023-07-25 16:50:27.914903 pydiscovergy-2.0.2/pydiscovergy/__init__.py
--rw-r--r--   0        0        0      330 2023-07-25 16:50:27.914903 pydiscovergy-2.0.2/pydiscovergy/authentication/__init__.py
--rw-r--r--   0        0        0      444 2023-07-25 16:50:27.914903 pydiscovergy-2.0.2/pydiscovergy/authentication/base.py
--rw-r--r--   0        0        0      658 2023-07-25 16:50:27.914903 pydiscovergy-2.0.2/pydiscovergy/authentication/basicauth.py
--rw-r--r--   0        0        0     7022 2023-07-25 16:50:27.914903 pydiscovergy-2.0.2/pydiscovergy/authentication/token.py
--rw-r--r--   0        0        0      646 2023-07-25 16:50:27.914903 pydiscovergy-2.0.2/pydiscovergy/const.py
--rw-r--r--   0        0        0     6278 2023-07-25 16:50:27.914903 pydiscovergy-2.0.2/pydiscovergy/discovergy.py
--rw-r--r--   0        0        0      547 2023-07-25 16:50:27.914903 pydiscovergy-2.0.2/pydiscovergy/error.py
--rw-r--r--   0        0        0     1041 2023-07-25 16:50:27.914903 pydiscovergy-2.0.2/pydiscovergy/marshmallow.py
--rw-r--r--   0        0        0     1447 2023-07-25 16:50:27.914903 pydiscovergy-2.0.2/pydiscovergy/models.py
--rw-r--r--   0        0        0     1095 2023-07-25 16:50:27.914903 pydiscovergy-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     1473 1970-01-01 00:00:00.000000 pydiscovergy-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-07-30 19:07:13.912165 pydiscovergy-2.0.3/LICENSE
+-rw-r--r--   0        0        0      575 2023-07-30 19:07:13.912165 pydiscovergy-2.0.3/README.md
+-rw-r--r--   0        0        0      102 2023-07-30 19:07:13.912165 pydiscovergy-2.0.3/pydiscovergy/__init__.py
+-rw-r--r--   0        0        0      330 2023-07-30 19:07:13.912165 pydiscovergy-2.0.3/pydiscovergy/authentication/__init__.py
+-rw-r--r--   0        0        0      484 2023-07-30 19:07:13.912165 pydiscovergy-2.0.3/pydiscovergy/authentication/base.py
+-rw-r--r--   0        0        0      698 2023-07-30 19:07:13.912165 pydiscovergy-2.0.3/pydiscovergy/authentication/basicauth.py
+-rw-r--r--   0        0        0     7090 2023-07-30 19:07:13.912165 pydiscovergy-2.0.3/pydiscovergy/authentication/token.py
+-rw-r--r--   0        0        0      646 2023-07-30 19:07:13.912165 pydiscovergy-2.0.3/pydiscovergy/const.py
+-rw-r--r--   0        0        0     6297 2023-07-30 19:07:13.912165 pydiscovergy-2.0.3/pydiscovergy/discovergy.py
+-rw-r--r--   0        0        0      547 2023-07-30 19:07:13.912165 pydiscovergy-2.0.3/pydiscovergy/error.py
+-rw-r--r--   0        0        0     1117 2023-07-30 19:07:13.912165 pydiscovergy-2.0.3/pydiscovergy/marshmallow.py
+-rw-r--r--   0        0        0     1495 2023-07-30 19:07:13.912165 pydiscovergy-2.0.3/pydiscovergy/models.py
+-rw-r--r--   0        0        0        0 2023-07-30 19:07:13.912165 pydiscovergy-2.0.3/pydiscovergy/py.typed
+-rw-r--r--   0        0        0     1158 2023-07-30 19:07:13.912165 pydiscovergy-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1473 1970-01-01 00:00:00.000000 pydiscovergy-2.0.3/PKG-INFO
```

### Comparing `pydiscovergy-2.0.2/LICENSE` & `pydiscovergy-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydiscovergy-2.0.2/README.md` & `pydiscovergy-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pydiscovergy-2.0.2/pydiscovergy/authentication/token.py` & `pydiscovergy-2.0.3/pydiscovergy/authentication/token.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Authentication module for token auth."""
 from __future__ import annotations
 
 import json
 from dataclasses import dataclass
 from urllib.parse import parse_qs
 
-from authlib.integrations.httpx_client import AsyncOAuth1Client
+from authlib.integrations.httpx_client import AsyncOAuth1Client  # type: ignore[import]
 from httpx import AsyncClient, HTTPStatusError, RequestError
 
 from ..const import (
     API_ACCESS_TOKEN,
     API_AUTHORIZATION,
     API_CONSUMER_TOKEN,
     API_REQUEST_TOKEN,
@@ -51,15 +51,19 @@
     """Authentication class for token auth."""
 
     consumer_token: ConsumerToken
     access_token: AccessToken
     app_name: str = DEFAULT_APP_NAME
 
     async def get_client(
-        self, email: str, password: str, timeout: int, httpx_client: AsyncClient = None
+        self,
+        email: str,
+        password: str,
+        timeout: int,
+        httpx_client: AsyncClient | None = None,
     ) -> AsyncOAuth1Client:
         """Returns a AsyncOAuth1Client."""
 
         await self._do_exchange(email, password)
         return AsyncOAuth1Client(**self._get_oauth_client_params(), timeout=timeout)
 
     async def _do_exchange(
@@ -122,15 +126,15 @@
                     consumer_tokens["key"], consumer_tokens["secret"]
                 )
                 return self.consumer_token
             except RequestError as exc:
                 raise DiscovergyClientError from exc
             except HTTPStatusError as exc:
                 raise HTTPError(
-                    f"Status {exc.response.status_code}: {exc.response.content}"
+                    f"Status {exc.response.status_code}: {exc.response.content!r}"
                 ) from exc
             except json.JSONDecodeError as exc:
                 raise DiscovergyError(f"Failed to decode json: {exc}") from exc
 
     async def _fetch_request_token(self) -> RequestToken:
         """Fetch request token."""
         async with AsyncOAuth1Client(
@@ -169,15 +173,15 @@
                 raise DiscovergyClientError from exc
             except HTTPStatusError as exc:
                 if exc.response.status_code == 403:
                     # the credentials are invaild so raise the correct error
                     raise InvalidLogin from exc
                 raise HTTPError(
                     f"Request failed with {exc.response.status_code}: "
-                    f"{exc.response.content}"
+                    f"{exc.response.content!r}"
                 ) from exc
 
     async def _fetch_access_token(
         self, request_token, request_token_secret, verifier
     ) -> AccessToken:
         """Fetch access token."""
         async with AsyncOAuth1Client(
```

### Comparing `pydiscovergy-2.0.2/pydiscovergy/const.py` & `pydiscovergy-2.0.3/pydiscovergy/const.py`

 * *Files identical despite different names*

### Comparing `pydiscovergy-2.0.2/pydiscovergy/discovergy.py` & `pydiscovergy-2.0.3/pydiscovergy/discovergy.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 @dataclass
 class Discovergy:
     """Async client for Discovergy API."""
 
     email: str
     password: str
     timeout: int = DEFAULT_TIMEOUT
-    httpx_client: httpx.AsyncClient = None
+    httpx_client: httpx.AsyncClient | None = None
     authentication: BaseAuthentication = BasicAuth()
 
-    async def _get(self, path: str, params: dict[str, Any] = None) -> Any:
+    async def _get(self, path: str, params: dict[str, Any] | None = None) -> Any:
         """Execute a GET request against the API."""
 
         # remove keys with empty values
         if params is not None:
             params = {key: value for (key, value) in params.items() if value != ""}
 
         # get ready to use client from authentication module
@@ -69,28 +69,28 @@
             if exception.response.status_code == 401 and isinstance(
                 self.authentication, BasicAuth
             ):
                 raise InvalidLogin from exception
 
             raise HTTPError(
                 f"Request failed with HTTP status {exception.response.status_code}: "
-                f"{exception.response.content}"
+                f"{exception.response.content!r}"
             ) from exception
         except json.JSONDecodeError as exception:
             raise DiscovergyError(f"JSON decoding failed: {exception}") from exception
 
     async def meters(self) -> list[Meter]:
         """Get list of smart meters."""
         response = await self._get("/meters")
-        return Meter.schema().load(response, many=True)  # pylint: disable=no-member
+        return Meter.schema().load(response, many=True)  # type: ignore[attr-defined]
 
     async def meter_last_reading(self, meter_id: str) -> Reading:
         """Get last reading for meter"""
         response = await self._get("/last_reading", params={"meterId": meter_id})
-        return Reading.schema().load(response)  # pylint: disable=no-member
+        return Reading.schema().load(response)  # type: ignore[attr-defined]
 
     async def meter_readings(
         self,
         meter_id: str,
         start_time: datetime,
         end_time: datetime | None = None,
         resolution: Resolution | None = None,
@@ -122,15 +122,15 @@
             "fields": ("" if field_names is None else ",".join(field_names)),
             "resolution": ("" if resolution is None else str(resolution)),
             "disaggregation": str(disaggregation).lower(),
             "each": str(each).lower(),
         }
 
         response = await self._get("/readings", params)
-        return Reading.schema().load(response, many=True)  # pylint: disable=no-member
+        return Reading.schema().load(response, many=True)  # type: ignore[attr-defined]
 
     async def meter_field_names(self, meter_id: str) -> list[str]:
         """Return all available measurement field names for the specified meter."""
         field_names = await self._get("/field_names", params={"meterId": meter_id})
         return FieldNameList.schema().load({"field_names": field_names}).field_names
 
     async def meter_devices(self, meter_id: str) -> list[str]:
```

### Comparing `pydiscovergy-2.0.2/pydiscovergy/error.py` & `pydiscovergy-2.0.3/pydiscovergy/error.py`

 * *Files identical despite different names*

### Comparing `pydiscovergy-2.0.2/pydiscovergy/marshmallow.py` & `pydiscovergy-2.0.3/pydiscovergy/marshmallow.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,35 +3,35 @@
 
 from dataclasses_json import DataClassJsonMixin, config
 from marshmallow import fields
 
 from pydiscovergy.models import Statistic
 
 
-@dataclass
+@dataclass(frozen=True, slots=True)
 class DeviceList(DataClassJsonMixin):
     """Helper class to deserialize device data from API."""
 
     devices: list[str] = field(metadata=config(mm_field=fields.List(fields.String())))
 
 
-@dataclass
+@dataclass(frozen=True, slots=True)
 class FieldNameList(DataClassJsonMixin):
     """Helper class to deserialize field name data from API."""
 
     field_names: list[str] = field(
         metadata=config(mm_field=fields.List(fields.String()))
     )
 
 
-@dataclass
+@dataclass(frozen=True, slots=True)
 class Statistics(DataClassJsonMixin):
     """Helper class to deserialize statistics data from API."""
 
     statistics: dict[str, Statistic] = field(
         metadata=config(
             mm_field=fields.Dict(
                 keys=fields.String(),
-                values=fields.Nested(Statistic.schema()),  # pylint: disable=no-member
+                values=fields.Nested(Statistic.schema()),  # type: ignore[attr-defined]
             )
         )
     )
```

### Comparing `pydiscovergy-2.0.2/pydiscovergy/models.py` & `pydiscovergy-2.0.3/pydiscovergy/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
 import pytz
 from dataclasses_json import CatchAll, LetterCase, Undefined, config, dataclass_json
 from marshmallow import fields
 
 
 @dataclass_json(letter_case=LetterCase.CAMEL)
-@dataclass(frozen=True)
+@dataclass(frozen=True, slots=True)
 class Location:
     """Represents a smart meter location."""
 
     street: str
     street_number: str
     city: str
     zip: int
     country: str
 
 
 @dataclass_json
-@dataclass(frozen=True)
+@dataclass(frozen=True, slots=True)
 class Reading:
     """Represents a reading of a smart meter."""
 
     time: datetime = field(metadata=config(mm_field=fields.DateTime("timestamp_ms")))
     values: dict[str, float] = field(
         metadata=config(
             mm_field=fields.Dict(keys=fields.String(), values=fields.Float())
@@ -33,27 +33,27 @@
 
     @property
     def time_with_timezone(self) -> datetime:
         return pytz.timezone("UTC").localize(self.time)
 
 
 @dataclass_json
-@dataclass(frozen=True)
+@dataclass(frozen=True, slots=True)
 class Statistic:
     """Represents a meter statistic entry."""
 
     count: int
     minimum: float
     maximum: float
     mean: float
     variance: float
 
 
 @dataclass_json(undefined=Undefined.INCLUDE, letter_case=LetterCase.CAMEL)
-@dataclass(frozen=True)
+@dataclass(frozen=True, slots=True)
 class Meter:
     """Represents a smart meter."""
 
     meter_id: str
     serial_number: str
     full_serial_number: str
     type: str
```

### Comparing `pydiscovergy-2.0.2/pyproject.toml` & `pydiscovergy-2.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pydiscovergy"
-version = "2.0.2"
+version = "2.0.3"
 description = "Async Python 3 library for interacting with Discovergy smart meters API"
 authors = ["Jan-Philipp Benecke <jan-philipp@bnck.me>"]
 repository = "https://github.com/jpbede/pydiscovergy"
 license = "MIT"
 readme = "README.md"
 packages = [
   { include = "pydiscovergy" }
 ]
 keywords = ["discovergy", "smart meter", "smart home"]
 
 [tool.poetry.dependencies]
-python = ">=3.9, <3.12"
-authlib = "<1.0.0"
+python = ">=3.9, <3.13" # needed by dataclasses-json
+authlib = ">=0.15"
 httpx = "^0.24.0"
-dataclasses-json = "^0.5.13"
+dataclasses-json = "^0.5.14"
 marshmallow = "^3.19.0"
 pytz = "^2023.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-asyncio = ">=0.20.3,<0.22.0"
 pytest-cov = "^4.0.0"
 respx = "^0.20.1"
 black = "^23.1.0"
 pre-commit = ">=2.21,<4.0"
 pytest-httpx = "^0.22.0"
+mypy = "^1.4.1"
+ruff = "^0.0.280"
 
 [tool.black]
 target-version = ["py311"]
 
 [tool.ruff]
 target-version = "py311"
```

### Comparing `pydiscovergy-2.0.2/PKG-INFO` & `pydiscovergy-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pydiscovergy
-Version: 2.0.2
+Version: 2.0.3
 Summary: Async Python 3 library for interacting with Discovergy smart meters API
 Home-page: https://github.com/jpbede/pydiscovergy
 License: MIT
 Keywords: discovergy,smart meter,smart home
 Author: Jan-Philipp Benecke
 Author-email: jan-philipp@bnck.me
-Requires-Python: >=3.9,<3.12
+Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: authlib (<1.0.0)
-Requires-Dist: dataclasses-json (>=0.5.13,<0.6.0)
+Requires-Dist: authlib (>=0.15)
+Requires-Dist: dataclasses-json (>=0.5.14,<0.6.0)
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: marshmallow (>=3.19.0,<4.0.0)
 Requires-Dist: pytz (>=2023.3,<2024.0)
 Project-URL: Repository, https://github.com/jpbede/pydiscovergy
 Description-Content-Type: text/markdown
 
 # pydiscovergy
```

