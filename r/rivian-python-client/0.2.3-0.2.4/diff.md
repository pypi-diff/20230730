# Comparing `tmp/rivian_python_client-0.2.3.tar.gz` & `tmp/rivian_python_client-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rivian_python_client-0.2.3.tar", max compression
+gzip compressed data, was "rivian_python_client-0.2.4.tar", max compression
```

## Comparing `rivian_python_client-0.2.3.tar` & `rivian_python_client-0.2.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      325 2023-05-25 23:07:28.617647 rivian_python_client-0.2.3/README.md
--rw-r--r--   0        0        0      555 2023-05-25 23:07:28.617647 rivian_python_client-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      102 2023-05-25 23:07:28.617647 rivian_python_client-0.2.3/src/rivian/__init__.py
--rw-r--r--   0        0        0     2888 2023-05-25 23:07:28.617647 rivian_python_client-0.2.3/src/rivian/const.py
--rw-r--r--   0        0        0      779 2023-05-25 23:07:28.617647 rivian_python_client-0.2.3/src/rivian/exceptions.py
--rw-r--r--   0        0        0    23660 2023-05-25 23:07:28.617647 rivian_python_client-0.2.3/src/rivian/rivian.py
--rw-r--r--   0        0        0     7356 2023-05-25 23:07:28.617647 rivian_python_client-0.2.3/src/rivian/ws_monitor.py
--rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 rivian_python_client-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      325 2023-07-30 01:43:46.885077 rivian_python_client-0.2.4/README.md
+-rw-r--r--   0        0        0      555 2023-07-30 01:43:46.885077 rivian_python_client-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      102 2023-07-30 01:43:46.885077 rivian_python_client-0.2.4/src/rivian/__init__.py
+-rw-r--r--   0        0        0     3242 2023-07-30 01:43:46.885077 rivian_python_client-0.2.4/src/rivian/const.py
+-rw-r--r--   0        0        0      779 2023-07-30 01:43:46.885077 rivian_python_client-0.2.4/src/rivian/exceptions.py
+-rw-r--r--   0        0        0    23190 2023-07-30 01:43:46.885077 rivian_python_client-0.2.4/src/rivian/rivian.py
+-rw-r--r--   0        0        0     7383 2023-07-30 01:43:46.885077 rivian_python_client-0.2.4/src/rivian/ws_monitor.py
+-rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 rivian_python_client-0.2.4/PKG-INFO
```

### Comparing `rivian_python_client-0.2.3/pyproject.toml` & `rivian_python_client-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rivian-python-client"
-version = "0.2.3"
+version = "0.2.4"
 description = "Rivian API Client (Unofficial)"
 readme = "README.md"
 authors = ["Brian Retterer <bretterer@gmail.com>"]
 license = "MIT"
 packages = [
     { include = "rivian", from = "src" },
 ]
```

### Comparing `rivian_python_client-0.2.3/src/rivian/const.py` & `rivian_python_client-0.2.4/src/rivian/const.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,29 @@
 """Rivian constants."""
 from __future__ import annotations
 
 from typing import Final
 
+LIVE_SESSION_PROPERTIES: Final[set[str]] = {
+    "chargerId",
+    "currentCurrency",
+    "currentPrice",
+    "isFreeSession",
+    "isRivianCharger",
+    "kilometersChargedPerHour",
+    "locationId",
+    "power",
+    "rangeAddedThisSession",
+    "startTime",
+    "timeElapsed",
+    "timeRemaining",
+    "totalChargedEnergy",
+    "vehicleChargerState",
+}
+
 VEHICLE_STATE_PROPERTIES: Final[set[str]] = {
     # VehicleLocation
     "gnssLocation",
     # TimeStamped(String|Float|Int)
     "alarmSoundStatus",
     "batteryHvThermalEvent",
     "batteryHvThermalEventPropagation",
```

### Comparing `rivian_python_client-0.2.3/src/rivian/exceptions.py` & `rivian_python_client-0.2.4/src/rivian/exceptions.py`

 * *Files identical despite different names*

### Comparing `rivian_python_client-0.2.3/src/rivian/rivian.py` & `rivian_python_client-0.2.4/src/rivian/rivian.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 
 import asyncio
 import json
 import logging
 import socket
 import uuid
 from collections.abc import Callable
-from typing import Any
+from typing import Any, Type
 
 import aiohttp
 import async_timeout
 from aiohttp import ClientRequest, ClientResponse, ClientWebSocketResponse
 
-from .const import VEHICLE_STATE_PROPERTIES
+from .const import LIVE_SESSION_PROPERTIES, VEHICLE_STATE_PROPERTIES
 from .exceptions import (
     RivianApiException,
     RivianApiRateLimitError,
     RivianDataError,
     RivianExpiredTokenError,
     RivianInvalidCredentials,
     RivianInvalidOTP,
@@ -44,14 +44,33 @@
     "Apollographql-Client-Name": APOLLO_CLIENT_NAME,
 }
 
 LOCATION_TEMPLATE = "{ latitude longitude timeStamp }"
 VALUE_TEMPLATE = "{ timeStamp value }"
 TEMPLATE_MAP = {"gnssLocation": LOCATION_TEMPLATE}
 
+LIVE_SESSION_VALUE_RECORD_KEYS = {
+    "kilometersChargedPerHour",
+    "power",
+    "rangeAddedThisSession",
+    "timeRemaining",
+    "totalChargedEnergy",
+    "vehicleChargerState",
+}
+VALUE_RECORD_TEMPLATE = "{ __typename value updatedAt }"
+
+ERROR_CODE_CLASS_MAP: dict[str, Type[RivianApiException]] = {
+    "BAD_CURRENT_PASSWORD": RivianInvalidCredentials,
+    "DATA_ERROR": RivianDataError,
+    "INTERNAL_SERVER_ERROR": RivianApiException,
+    "RATE_LIMIT": RivianApiRateLimitError,
+    "SESSION_MANAGER_ERROR": RivianTemporarilyLockedError,
+    "UNAUTHENTICATED": RivianUnauthenticated,
+}
+
 
 class Rivian:
     """Main class for the Rivian API Client"""
 
     def __init__(
         self,
         client_id: str,
@@ -457,71 +476,64 @@
             "query": graphql_query,
             "variables": {"vehicleID": vin},
         }
 
         return await self.__graphql_query(headers, url, graphql_json)
 
     async def get_live_charging_session(
-        self, user_id: str, vin: str, properties: dict[str]
+        self, vin: str, properties: set[str] | None = None
     ) -> ClientResponse:
-        """get live charging session data (graphql)"""
-        url = GRAPHQL_CHARGING
+        """Get live charging session data."""
+        if not properties:
+            properties = LIVE_SESSION_PROPERTIES
 
+        url = GRAPHQL_CHARGING
         headers = BASE_HEADERS | {"U-Sess": self._user_session_token}
 
-        graphql_query = "query getLiveSessionData($vehicleId: ID!) {\n  getLiveSessionData(vehicleId: $vehicleId) {\n    __typename\n   "
-        detail_sensors = [
-            "vehicleChargerState",
-            "timeRemaining",
-            "kilometersChargedPerHour",
-            "power",
-            "rangeAddedThisSession",
-            "totalChargedEnergy",
-        ]
-        detail_sensor_template = (
-            "{\n      __typename\n      value\n      updatedAt\n    }\n"
+        fragment = " ".join(
+            f"{p} {VALUE_RECORD_TEMPLATE if p in LIVE_SESSION_VALUE_RECORD_KEYS else ''}"
+            for p in properties
         )
-
-        for key in properties:
-            template = ""
-            if key in detail_sensors:
-                template = detail_sensor_template
-            graphql_query += f"{key} {template}"
-        graphql_query += "}"
-        graphql_query += "}"
+        graphql_query = f"""
+            query getLiveSessionData($vehicleId: ID!) {{
+                getLiveSessionData(vehicleId: $vehicleId) {{
+                    __typename
+                    {fragment}
+                }}
+            }}"""
 
         graphql_json = {
             "operationName": "getLiveSessionData",
             "query": graphql_query,
-            "variables": {"userId": user_id, "vehicleId": vin},
+            "variables": {"vehicleId": vin},
         }
 
         return await self.__graphql_query(headers, url, graphql_json)
 
     async def subscribe_for_vehicle_updates(
         self,
-        vin: str,
+        vehicle_id: str,
         properties: set[str] | None = None,
         callback: Callable = None,
     ) -> Callable | None:
         """Open a web socket connection to receive updates."""
         if not properties:
             properties = VEHICLE_STATE_PROPERTIES
 
         try:
             await self._ws_connect()
             async with async_timeout.timeout(self.request_timeout):
                 await self._ws_monitor.connection_ack.wait()
             payload = {
                 "operationName": "VehicleState",
                 "query": f"subscription VehicleState($vehicleID: String!) {{ vehicleState(id: $vehicleID) {self._build_vehicle_state_fragment(properties)} }}",
-                "variables": {"vehicleID": vin},
+                "variables": {"vehicleID": vehicle_id},
             }
             unsubscribe = await self._ws_monitor.start_subscription(payload, callback)
-            _LOGGER.debug("%s subscribed to updates", vin)
+            _LOGGER.debug("%s subscribed to updates", vehicle_id)
             return unsubscribe
         except Exception as ex:  # pylint: disable=broad-except
             _LOGGER.error(ex)
 
     async def _ws_connect(self) -> ClientWebSocketResponse:
         """Initiate a websocket connection."""
 
@@ -572,42 +584,24 @@
                 "Error occurred while communicating with Rivian."
             ) from exception
 
         try:
             response_json = await response.json()
             if errors := response_json.get("errors"):
                 for error in errors:
-                    extensions = error["extensions"]
-                    if (code := extensions["code"]) == "UNAUTHENTICATED":
-                        raise RivianUnauthenticated(
-                            response.status, response_json, headers, body
-                        )
-                    if code == "DATA_ERROR":
-                        raise RivianDataError(
-                            response.status, response_json, headers, body
-                        )
-                    if code == "BAD_CURRENT_PASSWORD":
-                        raise RivianInvalidCredentials(
-                            response.status, response_json, headers, body
-                        )
-                    if (
-                        code == "BAD_USER_INPUT"
-                        and extensions["reason"] == "INVALID_OTP"
-                    ):
-                        raise RivianInvalidOTP(
-                            response.status, response_json, headers, body
-                        )
-                    if code == "SESSION_MANAGER_ERROR":
-                        raise RivianTemporarilyLockedError(
-                            response.status, response_json, headers, body
-                        )
-                    if code == "RATE_LIMIT":
-                        raise RivianApiRateLimitError(
-                            response.status, response_json, headers, body
-                        )
+                    if extensions := error.get("extensions"):
+                        code = extensions["code"]
+                        if err_cls := ERROR_CODE_CLASS_MAP.get(code):
+                            raise err_cls(response.status, response_json, headers, body)
+                        if code == "BAD_USER_INPUT" and (
+                            extensions["reason"] == "INVALID_OTP"
+                        ):
+                            raise RivianInvalidOTP(
+                                response.status, response_json, headers, body
+                            )
                 raise RivianApiException(
                     "Error occurred while reading the graphql response from Rivian.",
                     response.status,
                     response_json,
                     headers,
                     body,
                 )
```

### Comparing `rivian_python_client-0.2.3/src/rivian/ws_monitor.py` & `rivian_python_client-0.2.4/src/rivian/ws_monitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     async def _subscribe(self, _id: str, payload: dict[str, Any]) -> None:
         """Send a subscribe request."""
         await self._ws.send_json({"id": _id, "payload": payload, "type": "subscribe"})
 
     async def _resubscribe_all(self) -> None:
         """Resubscribe all subscriptions."""
         try:
-            async with async_timeout.timeout(10):
+            async with async_timeout.timeout(self._account.request_timeout):
                 await self.connection_ack.wait()
         except asyncio.TimeoutError:
             _LOGGER.error("A timeout occurred while attempting to resubscribe")
             return
         for _id, (_, payload) in self._subscriptions.items():
             await self._subscribe(_id, payload)
```

### Comparing `rivian_python_client-0.2.3/PKG-INFO` & `rivian_python_client-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rivian-python-client
-Version: 0.2.3
+Version: 0.2.4
 Summary: Rivian API Client (Unofficial)
 License: MIT
 Author: Brian Retterer
 Author-email: bretterer@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

