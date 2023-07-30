# Comparing `tmp/aiolyric-1.0.9.tar.gz` & `tmp/aiolyric-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiolyric-1.0.9.tar", last modified: Tue Feb 22 09:51:26 2022, max compression
+gzip compressed data, was "aiolyric-1.1.0.tar", last modified: Sun Jul 30 18:49:06 2023, max compression
```

## Comparing `aiolyric-1.0.9.tar` & `aiolyric-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 09:51:26.746860 aiolyric-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-02-22 09:51:19.000000 aiolyric-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      809 2022-02-22 09:51:26.746860 aiolyric-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      500 2022-02-22 09:51:19.000000 aiolyric-1.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 09:51:26.746860 aiolyric-1.0.9/aiolyric/
--rw-r--r--   0 runner    (1001) docker     (121)     5013 2022-02-22 09:51:19.000000 aiolyric-1.0.9/aiolyric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 09:51:26.746860 aiolyric-1.0.9/aiolyric/client/
--rw-r--r--   0 runner    (1001) docker     (121)     2662 2022-02-22 09:51:19.000000 aiolyric-1.0.9/aiolyric/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-02-22 09:51:19.000000 aiolyric-1.0.9/aiolyric/const.py
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-02-22 09:51:19.000000 aiolyric-1.0.9/aiolyric/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 09:51:26.746860 aiolyric-1.0.9/aiolyric/objects/
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-02-22 09:51:19.000000 aiolyric-1.0.9/aiolyric/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-02-22 09:51:19.000000 aiolyric-1.0.9/aiolyric/objects/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     7279 2022-02-22 09:51:19.000000 aiolyric-1.0.9/aiolyric/objects/device.py
--rw-r--r--   0 runner    (1001) docker     (121)     4918 2022-02-22 09:51:19.000000 aiolyric-1.0.9/aiolyric/objects/location.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 09:51:26.746860 aiolyric-1.0.9/aiolyric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      809 2022-02-22 09:51:26.000000 aiolyric-1.0.9/aiolyric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-02-22 09:51:26.000000 aiolyric-1.0.9/aiolyric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-22 09:51:26.000000 aiolyric-1.0.9/aiolyric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-02-22 09:51:26.000000 aiolyric-1.0.9/aiolyric.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-02-22 09:51:26.000000 aiolyric-1.0.9/aiolyric.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-22 09:51:26.746860 aiolyric-1.0.9/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)      565 2022-02-22 09:51:19.000000 aiolyric-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:49:06.503139 aiolyric-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-30 18:48:57.000000 aiolyric-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-30 18:49:06.503139 aiolyric-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-30 18:48:57.000000 aiolyric-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:49:06.503139 aiolyric-1.1.0/aiolyric/
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-07-30 18:48:57.000000 aiolyric-1.1.0/aiolyric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:49:06.503139 aiolyric-1.1.0/aiolyric/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-30 18:48:57.000000 aiolyric-1.1.0/aiolyric/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-30 18:48:57.000000 aiolyric-1.1.0/aiolyric/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-30 18:48:57.000000 aiolyric-1.1.0/aiolyric/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:49:06.503139 aiolyric-1.1.0/aiolyric/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-30 18:48:57.000000 aiolyric-1.1.0/aiolyric/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-30 18:48:57.000000 aiolyric-1.1.0/aiolyric/objects/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-07-30 18:48:57.000000 aiolyric-1.1.0/aiolyric/objects/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-07-30 18:48:57.000000 aiolyric-1.1.0/aiolyric/objects/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-30 18:48:57.000000 aiolyric-1.1.0/aiolyric/objects/priority.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:49:06.503139 aiolyric-1.1.0/aiolyric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-30 18:49:06.000000 aiolyric-1.1.0/aiolyric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-30 18:49:06.000000 aiolyric-1.1.0/aiolyric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 18:49:06.000000 aiolyric-1.1.0/aiolyric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-30 18:49:06.000000 aiolyric-1.1.0/aiolyric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-30 18:49:06.000000 aiolyric-1.1.0/aiolyric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 18:49:06.503139 aiolyric-1.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      565 2023-07-30 18:48:57.000000 aiolyric-1.1.0/setup.py
```

### Comparing `aiolyric-1.0.9/LICENSE` & `aiolyric-1.1.0/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020 Aidan Timson
+Copyright (c) 2020-2023 Aidan Timson
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `aiolyric-1.0.9/PKG-INFO` & `aiolyric-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
 Name: aiolyric
-Version: 1.0.9
+Version: 1.1.0
 Summary: AIO package for the Honeywell Lyric Platform.
 Home-page: https://github.com/timmo001/aiolyric
 Author: Aidan Timson (Timmo)
 Author-email: contact@timmo.xyz
 License: MIT
 Keywords: honeywell lyric thermostat
-Platform: UNKNOWN
 License-File: LICENSE
 
 # AIOLyric
 
 Python package for the Honeywell Lyric Platform.
 
 ## Attributions / Contributions
 
 - [@bramkragten](https://github.com/bramkragten) for the original implementation. Referenced his [package](https://github.com/bramkragten/python-lyric) quite a bit whilst writing this one.
 - [@ludeeus](https://github.com/ludeeus) for his generator class. Made reading json into objects super simple. :tada:
 - [Everyone else](https://github.com/timmo001/aiolyric/graphs/contributors). Thanks for the help!
-
-
```

### Comparing `aiolyric-1.0.9/aiolyric/__init__.py` & `aiolyric-1.1.0/aiolyric/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 """Lyric: Init"""
-from aiohttp import ClientResponse
 from typing import List
 
+from aiohttp import ClientResponse
+
 from .const import BASE_URL
 from .objects.base import LyricBase
 from .objects.device import LyricDevice
 from .objects.location import LyricLocation
+from .objects.priority import LyricPriority, LyricRoom
 
 
 class Lyric(LyricBase):
     """Handles authentication refresh tokens."""
 
-    def __init__(self, client: "LyricClient", client_id: str) -> None:
+    def __init__(
+        self,
+        client: "LyricClient",
+        client_id: str,
+    ) -> None:
         """Initialize the token manager class."""
         self._client = client
         self._client_id = client_id
         self._devices: List[LyricDevice] = []
         self._devices_dict: dict = {}
         self._locations: List[LyricLocation] = []
         self._locations_dict: dict = {}
+        self._rooms_dict: dict = {}    
 
     @property
     def client_id(self) -> str:
         return self._client_id
 
     @property
     def devices(self) -> List[LyricDevice]:
@@ -36,15 +43,22 @@
     def locations(self) -> List[LyricLocation]:
         return self._locations
 
     @property
     def locations_dict(self) -> dict:
         return self._locations_dict
 
-    async def get_devices(self, location_id: int) -> None:
+    @property
+    def rooms_dict(self) -> dict[str, LyricRoom]:
+        return self._rooms_dict
+
+    async def get_devices(
+        self,
+        location_id: int,
+    ) -> None:
         """Get Devices."""
         response: ClientResponse = await self._client.get(
             f"{BASE_URL}/devices?apikey={self.client_id}&locationId={location_id}"
         )
         json = await response.json()
         self.logger.debug(json)
         self._devices = [LyricDevice(self._client, device) for device in json or []]
@@ -62,14 +76,35 @@
         self._locations = [
             LyricLocation(self._client, location) for location in json or []
         ]
         self._locations_dict: dict = {}
         for location in self._locations:
             self._locations_dict[location.locationID] = location
 
+    async def get_thermostat_rooms(
+            self,
+            location_id: int,
+            device_id: str
+        ) -> None:
+        """Get Priority, which contains accessory information."""
+        response: ClientResponse = await self._client.get(
+            f"{BASE_URL}/devices/thermostats/{device_id}/priority?apikey={self.client_id}&locationId={location_id}"
+        )
+        json = await response.json()
+        self.logger.debug(json)
+        
+        priority = LyricPriority(json)
+
+        macId = priority.deviceId   # device id in the priority payload refers to the mac address of the device
+        self._rooms_dict[macId]: dict = {}
+        
+        # add each room to the room dictionary. Rooms contain motion, temp, and humidity averages for all accessories in a room
+        for room in priority.currentPriority.rooms:
+            self._rooms_dict[macId][room.id] = room
+
     async def update_thermostat(
         self,
         location: LyricLocation,
         device: LyricDevice,
         mode=None,
         heatSetpoint=None,
         coolSetpoint=None,
@@ -125,22 +160,27 @@
 
         return await self._client.post(
             f"{BASE_URL}/devices/thermostats/{device.deviceID}?apikey={self._client_id}&locationId={location.locationID}",
             json=data,
         )
 
     async def update_fan(
-        self, location: LyricLocation, device: LyricDevice, mode: str
+        self,
+        location: LyricLocation,
+        device: LyricDevice,
+        mode: str,
     ) -> ClientResponse:
         """Update Fan."""
         self.logger.debug("Update Fan")
 
         data = {}
 
-        if mode is None:
+        if mode is not None:
+            data["mode"] = mode
+        else:
             data["mode"] = device.fanMode
 
         self.logger.debug(data)
 
         return await self._client.post(
             f"{BASE_URL}/devices/thermostats/{device.deviceID}/fan?apikey={self._client_id}&locationId={location.locationID}",
             json=data,
```

### Comparing `aiolyric-1.0.9/aiolyric/client/__init__.py` & `aiolyric-1.1.0/aiolyric/client/__init__.py`

 * *Files identical despite different names*

### Comparing `aiolyric-1.0.9/aiolyric/objects/device.py` & `aiolyric-1.1.0/aiolyric/objects/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,19 @@
 
 
 class SettingsSpecialmode(LyricBase):
     @property
     def _(self):
         return None
 
+class SettingsFan(LyricBase):
+    @property
+    def fan(self):
+        return self.atributes.get("fan", {})
+        
 
 class Settings(LyricBase):
     @property
     def hardwareSettings(self):
         return SettingsHardwaresettings(self.attributes.get("hardwareSettings", {}))
 
     @property
@@ -78,14 +83,26 @@
     def specialMode(self):
         return SettingsSpecialmode(self.attributes.get("specialMode", {}))
 
     @property
     def devicePairingEnabled(self):
         return self.attributes.get("devicePairingEnabled", True)
 
+    @property
+    def fanModes(self):
+        return SettingsFan(self.attributes.get("allowedModes", []))
+
+    @property
+    def fanChangeableValues(self):
+        return SettingsFan(self.attributes.get("changeableValues", {}))
+    
+    @property
+    def fanMode(self):
+        return fanChangeableValues(self.attributes.get("mode", None))
+
 
 class Devicesettings(LyricBase):
     @property
     def _(self):
         return None
```

### Comparing `aiolyric-1.0.9/aiolyric/objects/location.py` & `aiolyric-1.1.0/aiolyric/objects/location.py`

 * *Files identical despite different names*

### Comparing `aiolyric-1.0.9/aiolyric.egg-info/PKG-INFO` & `aiolyric-1.1.0/aiolyric.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
 Name: aiolyric
-Version: 1.0.9
+Version: 1.1.0
 Summary: AIO package for the Honeywell Lyric Platform.
 Home-page: https://github.com/timmo001/aiolyric
 Author: Aidan Timson (Timmo)
 Author-email: contact@timmo.xyz
 License: MIT
 Keywords: honeywell lyric thermostat
-Platform: UNKNOWN
 License-File: LICENSE
 
 # AIOLyric
 
 Python package for the Honeywell Lyric Platform.
 
 ## Attributions / Contributions
 
 - [@bramkragten](https://github.com/bramkragten) for the original implementation. Referenced his [package](https://github.com/bramkragten/python-lyric) quite a bit whilst writing this one.
 - [@ludeeus](https://github.com/ludeeus) for his generator class. Made reading json into objects super simple. :tada:
 - [Everyone else](https://github.com/timmo001/aiolyric/graphs/contributors). Thanks for the help!
-
-
```

### Comparing `aiolyric-1.0.9/setup.py` & `aiolyric-1.1.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 import io
 
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
-version = "1.0.9"
+version = "1.1.0"
 
 setup(
     name="aiolyric",
     version=version,
     description="AIO package for the Honeywell Lyric Platform.",
     long_description=io.open("README.md", encoding="UTF-8").read(),
     keywords="honeywell lyric thermostat",
```

