# Comparing `tmp/pyhyypapihawkmod-1.2.0b8.tar.gz` & `tmp/pyhyypapihawkmod-1.3.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhyypapihawkmod-1.2.0b8.tar", last modified: Sat Jul 29 11:10:06 2023, max compression
+gzip compressed data, was "pyhyypapihawkmod-1.3.0b3.tar", last modified: Sun Jul 30 16:44:24 2023, max compression
```

## Comparing `pyhyypapihawkmod-1.2.0b8.tar` & `pyhyypapihawkmod-1.3.0b3.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 11:10:06.896834 pyhyypapihawkmod-1.2.0b8/
--rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b8/LICENSE.md
--rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b8/MANIFEST.in
--rw-rw-rw-   0        0        0      519 2023-07-29 11:10:06.896330 pyhyypapihawkmod-1.2.0b8/PKG-INFO
--rw-rw-rw-   0        0        0     2459 2023-07-29 11:05:28.000000 pyhyypapihawkmod-1.2.0b8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 11:10:06.882316 pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/
--rw-rw-rw-   0        0        0      429 2023-06-19 07:52:00.000000 pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/__init__.py
--rw-rw-rw-   0        0        0      151 2023-07-28 18:18:42.000000 pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/__main__.py
--rw-rw-rw-   0        0        0    12205 2023-07-29 11:08:57.000000 pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/alarm_info.py
--rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/android_checkin_pb2.py
--rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/checkin_pb2.py
--rw-rw-rw-   0        0        0    29649 2023-07-29 11:05:40.000000 pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/client.py
--rw-rw-rw-   0        0        0     4084 2023-07-29 09:36:17.000000 pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/constants.py
--rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/exceptions.py
--rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/mcs_pb2.py
--rw-rw-rw-   0        0        0    16227 2023-07-28 18:18:42.000000 pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/push_receiver.py
-drwxrwxrwx   0        0        0        0 2023-07-29 11:10:06.893824 pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod.egg-info/
--rw-rw-rw-   0        0        0      519 2023-07-29 11:10:06.000000 pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2023-07-29 11:10:06.000000 pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 11:10:06.000000 pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-29 11:10:06.000000 pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-29 11:10:06.000000 pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 11:10:06.897337 pyhyypapihawkmod-1.2.0b8/setup.cfg
--rw-rw-rw-   0        0        0      923 2023-07-29 11:05:05.000000 pyhyypapihawkmod-1.2.0b8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 16:44:24.863539 pyhyypapihawkmod-1.3.0b3/
+-rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b3/LICENSE.md
+-rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b3/MANIFEST.in
+-rw-rw-rw-   0        0        0      519 2023-07-30 16:44:24.862034 pyhyypapihawkmod-1.3.0b3/PKG-INFO
+-rw-rw-rw-   0        0        0     3094 2023-07-30 16:43:15.000000 pyhyypapihawkmod-1.3.0b3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 16:44:24.841998 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/
+-rw-rw-rw-   0        0        0      410 2023-07-30 15:49:06.000000 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/__init__.py
+-rw-rw-rw-   0        0        0      162 2023-07-30 07:50:36.000000 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/__main__.py
+-rw-rw-rw-   0        0        0    12324 2023-07-30 07:42:04.000000 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/alarm_info.py
+-rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/android_checkin_pb2.py
+-rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/checkin_pb2.py
+-rw-rw-rw-   0        0        0    32745 2023-07-30 16:39:10.000000 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/client.py
+-rw-rw-rw-   0        0        0     4114 2023-07-30 16:00:32.000000 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/constants.py
+-rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/exceptions.py
+-rw-rw-rw-   0        0        0     1999 2023-07-30 15:55:41.000000 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/imei.py
+-rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/mcs_pb2.py
+-rw-rw-rw-   0        0        0    17749 2023-07-30 16:15:07.000000 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/push_receiver.py
+drwxrwxrwx   0        0        0        0 2023-07-30 16:44:24.860040 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod.egg-info/
+-rw-rw-rw-   0        0        0      519 2023-07-30 16:44:24.000000 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      576 2023-07-30 16:44:24.000000 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 16:44:24.000000 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-30 16:44:24.000000 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-30 16:44:24.000000 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 16:44:24.864035 pyhyypapihawkmod-1.3.0b3/setup.cfg
+-rw-rw-rw-   0        0        0      923 2023-07-30 15:18:53.000000 pyhyypapihawkmod-1.3.0b3/setup.py
```

### Comparing `pyhyypapihawkmod-1.2.0b8/LICENSE.md` & `pyhyypapihawkmod-1.3.0b3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b8/PKG-INFO` & `pyhyypapihawkmod-1.3.0b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.2.0b8
+Version: 1.3.0b3
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.2.0b8/README.md` & `pyhyypapihawkmod-1.3.0b3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -37,14 +37,28 @@
 
 ```
 print(json.dumps(client.get_sync_info(),indent=2))
 
 ```
 
 Changelog 
+1.3.0b3
+- Hotfix, notifications appear to go to random people. Implemented random IMEI
+
+1.3.0b2
+- Implementation of push receiver.
+
+1.3.0b1
+- API supports both push and poll mode.
+- API will can now send to Home Assistant when data is ready instead of Home assistant Polling
+- Relevant new methods:
+  - `request_alarm_info_push_to_hass()` - Hass can call this to request an earlier push instead of the 30 seconds
+  - `initialize_alarm_info_push_timer()` - Hass must call this when ready as it initializes the timer in the API
+  - `register_alarm_info_callback()` - Hass muss register a callback method using this method
+
 
 1.2.0b8
 - Added additional debug checks
 
 1.2.0b2
 - Added additional checks for openviolated and tampered information when not received
```

### Comparing `pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/alarm_info.py` & `pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/alarm_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,40 +10,45 @@
 
 _LOGGER = logging.getLogger(__name__)
 
 
 if TYPE_CHECKING:
     from .client import HyypClient
 
-SLEEP_DELAY = 0.6
+SLEEP_DELAY = 0.5
 
 class HyypAlarmInfos:
     """Initialize Hyyp alarm objects."""
 
     def __init__(self, client: HyypClient) -> None:
         """init."""
         self._client = client
         self._sync_info: dict = {}
         self._state_info: dict = {}
         self._notifications: dict = {}
         self._zone_state_info = []
         self._last_notification_check_timestamp = 0
 
-    def _fetch_data(self) -> None:
+    def _fetch_data(self, forced=False) -> None:
         """Fetch data via client api."""
-        time.sleep(SLEEP_DELAY)
+        #forced = False
+        if not forced:
+            time.sleep(SLEEP_DELAY)
         self._sync_info = self._client.get_sync_info()
-        time.sleep(SLEEP_DELAY)
-        self._state_info = self._client.get_state_info()
-        self._zone_state_info.clear()
-        for site in self._sync_info["sites"]:
-            siteid = site["id"]
+        if not forced:
             time.sleep(SLEEP_DELAY)
-            entry = {siteid : self._client.get_zone_state_info(site_id=siteid)}
-            self._zone_state_info.append(entry)
+        self._state_info = self._client.get_state_info()
+        if not forced:
+            self._zone_state_info.clear()
+            for site in self._sync_info["sites"]:
+                siteid = site["id"]
+                time.sleep(SLEEP_DELAY)
+                site_zone_info = self._client.get_zone_state_info(site_id=siteid)
+                entry = {siteid : site_zone_info}
+                self._zone_state_info.append(entry)
 
             
         
     def get_zone_state_info_for_site(self, site):
         current_siteinfo = None
         for siteinfo in self._zone_state_info:
             if site in siteinfo:
@@ -51,18 +56,14 @@
                 if current_siteinfo is None:
                     return None
                 if "status" not in current_siteinfo:
                     return None
                 if current_siteinfo["status"] != "SUCCESS":
                     return None
         return current_siteinfo
-    
-            
-
-
         
     def _fetch_notifications(self, site_id: int) -> dict[Any,Any]:
         """Fetch and cache site notifications."""
         self._notifications = self._client.site_notifications(site_id=site_id)
 
 
     def _last_notice(self) -> dict[Any, Any]:
@@ -113,20 +114,18 @@
         return _response
 
 
     def _triggered_zones(self) -> Any:
            
         triggeredZoneIds = []
         _new_notifications = self._new_notifications()
-        
         for _notification in _new_notifications:
             if _notification['eventNumber'] != 5:
                 continue
-            triggeredZoneIds.append(_notification['zoneId'])  
-                 
+            triggeredZoneIds.append(_notification['zoneId'])         
         _response = triggeredZoneIds
         
         return _response
      
 
      
     def _format_data(self) -> dict[Any, Any]:
@@ -162,58 +161,54 @@
             site_ids[site]["lastNoticeName"] = _last_notice["lastNoticeName"]
 
             # Add triggers (PGM / Automations in APP)
             site_ids[site]["triggers"] = {}
             for trigger_id in trigger_ids:
                 if trigger_id not in site_ids[site]["triggerIds"]:
                     continue
-                else:
-                    site_ids[site]["triggers"] = {
-                        key: value
-                        for (key, value) in trigger_ids.items()            
-                    }
-                
-            
+                site_ids[site]["triggers"] = {
+                    key: value
+                    for (key, value) in trigger_ids.items()            
+                }
+                    
             # Add partition info.
             site_ids[site]["partitions"] = {
                 partition_id: partition_ids[partition_id]
                 for partition_id in site_ids[site]["partitionIds"]
             }
 
             for partition in partition_ids:
                 # Add zone info to partition.
                 if partition not in site_ids[site]["partitions"]:
                     continue
-                else:  
-                    site_ids[site]["partitions"][partition]["zones"] = {
-                        key: value
-                        for (key, value) in zone_ids.items()
-                        if key in site_ids[site]["partitions"][partition]["zoneIds"]
-                    }
+                site_ids[site]["partitions"][partition]["zones"] = {
+                    key: value
+                    for (key, value) in zone_ids.items()
+                    if key in site_ids[site]["partitions"][partition]["zoneIds"]
+                }
 
                 # Add zone bypass info to zone.
                 for zone in site_ids[site]["partitions"][partition]["zones"]:
                     site_ids[site]["partitions"][partition]["zones"][zone][
                         "bypassed"
                     ] = bool(zone in self._state_info["bypassedZoneIds"])
 
-
-
-                # New zone information from IDS servers
+                # New zone information from IDS servers               
                 for zone in site_ids[site]["partitions"][partition]["zones"]:
                     if zone_states is None:
                         continue
                     if "zones" not in zone_states:
                         continue
                     for zone_state in zone_states["zones"]:
                         if site_ids[site]["partitions"][partition]["zones"][zone][
                             "number"] != zone_state["number"]:
                             continue
-                        site_ids[site]["partitions"][partition]["zones"][zone][
-                            "bypassed"] = bool(zone_state["bypassed"])
+                     #   site_ids[site]["partitions"][partition]["zones"][zone][
+                     #       "bypassed"] = bool(zone_state["bypassed"] or 
+                     #                          zone in self._state_info["bypassedZoneIds"])
                         site_ids[site]["partitions"][partition]["zones"][zone][
                             "openviolated"] = bool(zone_state["openViolated"])
                         site_ids[site]["partitions"][partition]["zones"][zone][
                             "tampered"] = bool(zone_state["tampered"])
                         site_ids[site]["partitions"][partition]["zones"][zone][
                             "stay_bypassed"] = False
 
@@ -238,39 +233,34 @@
 
                 # Add partition stay_armed status.
                 site_ids[site]["partitions"][partition]["stayArmed"] = False
                 
                 for stay_profile in site_ids[site]["partitions"][partition]["stayProfiles"]:
                     if stay_profile not in self._state_info["armedStayProfileIds"]:
                         continue
-                    
                     site_ids[site]["partitions"][partition]["stayArmed"] = bool(
                         stay_profile in self._state_info["armedStayProfileIds"]
                     )
-                    
                     site_ids[site]["partitions"][partition]["stayArmedProfileName"] = (
                         site_ids[site]["partitions"][partition]["stayProfiles"][
                             stay_profile]["name"]
                     )
-                    
                     # Show zone as bypassed if stay partition has it bypassed                 
                     for zone in site_ids[site]["partitions"][partition]["zones"]:
                         bypassed_due_to_stay = zone in site_ids[site]["partitions"][partition]["stayProfiles"][stay_profile]['zoneIds']
                         site_ids[site]["partitions"][partition]["zones"][zone]["stay_bypassed"] = bypassed_due_to_stay
                         site_ids[site]["partitions"][partition]["zones"][zone][
                         "bypassed"
                         ] = bool(site_ids[site]["partitions"][partition]["zones"][zone]["bypassed"] or bypassed_due_to_stay)
                         
-
         return site_ids
 
-    def status(self) -> dict[Any, Any]:
+    def status(self, forced=False) -> dict[Any, Any]:
         """Return the status of Hyyp connected alarms."""
-
-        self._fetch_data()
+        self._fetch_data(forced=forced)
         formatted_data: dict[Any, Any] = self._format_data()
 
         return formatted_data
 
 
 
     def debug_thread(self):
```

### Comparing `pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/android_checkin_pb2.py` & `pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/android_checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/checkin_pb2.py` & `pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/client.py` & `pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """Hyyp Client API."""
 from __future__ import annotations
 
 import logging
 from typing import Any
 
 import requests
+import threading as thread
+import time
 
 from .alarm_info import HyypAlarmInfos
-from .constants import DEFAULT_TIMEOUT, REQUEST_HEADER, STD_PARAMS, DEBUG_CLIENT_STRING, HyypPkg
+from .push_receiver import FCMListener, FCMRegistration
+from .constants import DEFAULT_TIMEOUT, REQUEST_HEADER, STD_PARAMS, DEBUG_CLIENT_STRING, PUSH_DELAY, GCF_SENDER_ID, IMEI_SEED, HyypPkg
 from .exceptions import HTTPError, HyypApiError, InvalidURL
+from .imei import ImeiGenerator
 
 _LOGGER = logging.getLogger(__name__)
 
 BASE_URL = "ids.trintel.co.za/Inhep-Impl-1.0-SNAPSHOT/"
 API_ENDPOINT_LOGIN = "/auth/login"
 API_ENDPOINT_CHECK_APP_VERSION = "/auth/checkAppVersion"
 API_ENDPOINT_GET_SITE_NOTIFICATIONS = "/device/getSiteNotifications"
@@ -28,44 +32,56 @@
 API_ENDPOINT_SET_ZONE_BYPASS = "/device/bypass"
 API_ENDPOINT_GET_CAMERA_BY_PARTITION = "/device/getCameraByPartition"
 API_ENDPOINT_UPDATE_SUB_USER = "/user/updateSubUser"
 API_ENDPOINT_SET_NOTIFICATION_SUBSCRIPTIONS = "/user/setNotificationSubscriptionsNew"
 API_ENDPOINT_TRIGGER_AUTOMATION = "/device/trigger"
 API_ENDPOINT_GET_ZONE_STATE_INFO = "/device/getZoneStateInfo"
 
-
+REQUEST_PUSH_TIMEOUT = 1.5
 class HyypClient:
     """Initialize api client object."""
 
     def __init__(
         self,
         email: str | None = None,
         password: str | None = None,
         pkg: str = HyypPkg.ADT_SECURE_HOME.value,
         timeout: int = DEFAULT_TIMEOUT,
         token: str | None = None,
         userid: int | None = None,
+        fcm_credentials: None = None,
+        imei: str | None = None
     ) -> None:
         """Initialize the client object."""
         self._email = email
         self._password = password
         self._session = requests.session()
         self._session.headers.update(REQUEST_HEADER)
         STD_PARAMS["pkg"] = pkg
         STD_PARAMS["token"] = token
         STD_PARAMS["userId"] = userid
+        STD_PARAMS["imei"] = imei
         self._timeout = timeout
-
+        self.callback_function_alarm_info = None
+        self.callback_function_fcm_info = None
+        self.time_to_push = PUSH_DELAY
+        self.forced_refresh = False
+        self.alarminfos = HyypAlarmInfos(self)
+        self.fcm_listener = FCMListener()
+        self.fcm_register = FCMRegistration()
+        self.fcm_credentials = fcm_credentials
+        
     def login(self) -> Any:
         """Login to ADT Secure Home API."""
 
+
+
         _params = STD_PARAMS.copy()
         _params["email"] = self._email
         _params["password"] = self._password
-
         try:
             req = self._session.get(
                 "https://" + BASE_URL + API_ENDPOINT_LOGIN,
                 allow_redirects=False,
                 params=_params,
                 timeout=self._timeout,
             )
@@ -94,14 +110,18 @@
 
         STD_PARAMS["token"] = _json_result["token"]
         STD_PARAMS["userId"] = _json_result["user"]["id"]
 
         DEBUG_CLIENT_STRING["client_string"] = _json_result
         return _json_result
 
+    def generate_imei(self):
+        imei = ImeiGenerator().generate_imei(IMEI_SEED)
+        return imei
+
     def check_app_version(self) -> Any:
         """Check App version via API."""
 
         _params = STD_PARAMS.copy()
         _params["clientImei"] = STD_PARAMS["imei"]
 
         try:
@@ -134,18 +154,72 @@
         if _json_result["status"] != "SUCCESS" and _json_result["error"] is not None:
             raise HyypApiError(
                 f"Error checking app version from api: {_json_result['error']}"
             )
 
         return _json_result
 
+    def alarm_info_push_timer(self):
+        SLEEP_DELAY = 0.1
+        while 1:
+            if self.forced_refresh and self.time_to_push > REQUEST_PUSH_TIMEOUT:
+                self.time_to_push = REQUEST_PUSH_TIMEOUT
+            while self.time_to_push > 0:
+                time.sleep(SLEEP_DELAY)
+                self.time_to_push -= SLEEP_DELAY
+            alarminfo = self.load_alarm_infos()
+            self.callback_function_alarm_info(alarminfo)
+            self.forced_refresh = False
+            self.time_to_push = PUSH_DELAY
+
+    def request_alarm_info_push_to_hass(self):
+        self.forced_refresh = True
+        self.time_to_push = REQUEST_PUSH_TIMEOUT
+        
+    def initialize_alarm_info_push_timer(self):
+        thread.Thread(target=self.alarm_info_push_timer).start()
+
+    def register_alarm_info_callback(self, callback_function):
+        self.callback_function_alarm_info = callback_function
+
     def load_alarm_infos(self) -> dict[Any, Any]:
         """Get alarm infos formatted for hass infos."""
+        forced = self.forced_refresh
+        #return HyypAlarmInfos(self).status()
+        return self.alarminfos.status(forced=forced)
+
+    def initialize_fcm_notification_listener(self, persistent_pids = None):
+        
+        if self.fcm_credentials is None:
+            _LOGGER.warning("No FCM credentials available, disabling notifications")
+            return
+        if "fcm" not in self.fcm_credentials:
+            _LOGGER.warning("No FCM credentials available, disabling notifications")
+            return
+        thread.Thread(target=self.fcm_notification_thread,
+                      kwargs={'persistent_ids': persistent_pids}).start()
+        #thread.Thread(target=self.alarm_info_push_timer).start()
+
+
+    def fcm_notification_thread(self, persistent_ids = None):
+        gcm_address = self.fcm_credentials["fcm"]["token"]
+        self.store_gcm_registrationid(gcm_id=gcm_address)  
+        self.fcm_listener.runner(callback=self.callback_function_fcm_info,
+                                 credentials=self.fcm_credentials,
+                                 persistent_ids=persistent_ids)
+
+
+    def register_fcm_info_callback(self, callback_function):
+        self.callback_function_fcm_info = callback_function
+        
+
+    def get_intial_fcm_credentials(self):
+        return self.fcm_register.register(sender_id=GCF_SENDER_ID)
+        # error checker??
 
-        return HyypAlarmInfos(self).status()
 
     def get_debug_infos(self) -> dict[Any, Any]:
         """Get alarm infos formatted for hass infos."""
         return HyypAlarmInfos(self).get_debug_info()
 
     def site_notifications(
         self, site_id: int, timestamp: int | None = None, json_key: int | None = None
@@ -544,32 +618,30 @@
             )
 
         if json_key is None:
             return _json_result
 
         return _json_result[json_key]
 
-    def store_gcm_registrationid(self, gcm_id: str | None = None) -> Any:
+    def store_gcm_registrationid(self, gcm_id = None) -> Any:
         """Store gcmid."""
-
         _params = STD_PARAMS.copy()
         _params["gcmId"] = gcm_id
         del _params["imei"]
         _params["clientImei"] = STD_PARAMS["imei"]
-
         try:
             req = self._session.post(
                 "https://" + BASE_URL + API_ENDPOINT_STORE_GCM_REGISTRATION_ID,
                 allow_redirects=False,
                 params=_params,
                 timeout=self._timeout,
             )
-
+        
             req.raise_for_status()
-
+        
         except requests.ConnectionError as err:
             raise InvalidURL("A Invalid URL or Proxy error occured") from err
 
         except requests.HTTPError as err:
             raise HTTPError from err
 
         try:
@@ -581,15 +653,14 @@
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         if _json_result["status"] != "SUCCESS" and _json_result["error"] is not None:
             raise HyypApiError(f"Storing gcm id failed with: {_json_result['error']}")
-
         return _json_result
 
     def set_user_preference(
         self,
         store_for: str,
         new_code: int,
         site_id: str,
@@ -728,15 +799,15 @@
             req.raise_for_status()
 
         except requests.ConnectionError as err:
             raise InvalidURL("A Invalid URL or Proxy error occured") from err
 
         except requests.HTTPError as err:
             raise HTTPError from err
-
+        
         try:
             _json_result: dict[Any, Any] = req.json()
 
         except ValueError as err:
             raise HyypApiError(
                 "Impossible to decode response: "
                 + str(err)
@@ -860,15 +931,15 @@
         _params: dict[str, Any] = STD_PARAMS.copy()
         _params["partitionId"] = partition_id
         _params["zones"] = zones
         _params["stayProfileId"] = stay_profile_id
         _params["pin"] = pin
         del _params["imei"]
         _params["clientImei"] = STD_PARAMS["imei"]
-
+        
         try:
             req = self._session.get(
                 "https://" + BASE_URL + API_ENDPOINT_SET_ZONE_BYPASS,
                 allow_redirects=False,
                 params=_params,
                 timeout=self._timeout,
             )
```

### Comparing `pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/constants.py` & `pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """Hyyp API constants."""
 from enum import Enum
 
+PUSH_DELAY = 30
 DEFAULT_TIMEOUT = 25
 MAX_RETRIES = 3
 GCF_SENDER_ID = 87969245803
 REQUEST_HEADER = {
     "User-Agent": "okhttp/3.12.1",
 }  # Standard android header.
+
+IMEI_SEED = "15241971"
 STD_PARAMS = {
-    "imei": "152419714130158",  # Alphabet soup starts at 0
+    "imei": None,  # Alphabet soup starts at 0
     "appVersionCode": "401",
     "_appVersionCode": "401",
     "deviceOS": "12.0",
     "deviceName": "Python API",
     "pkg": "za.co.adt.securehome.android",
     "_appVersionName": "3.5.19",
     "token": None,
```

### Comparing `pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/mcs_pb2.py` & `pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/mcs_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/push_receiver.py` & `pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/push_receiver.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,174 +49,15 @@
 CHECKIN_URL = "https://android.clients.google.com/checkin"
 FCM_SUBSCRIBE = "https://fcm.googleapis.com/fcm/connect/subscribe"
 FCM_ENDPOINT = "https://fcm.googleapis.com/fcm/send"
 GOOGLE_MTALK_ENDPOINT = "mtalk.google.com"
 READ_TIMEOUT_SECS = 60 * 60
 MIN_RESET_INTERVAL_SECS = 60 * 5
 
-
-def __do_request(req, retries=5):
-    for _ in range(retries):
-        try:
-            resp = urlopen(req)
-            resp_data = resp.read()
-            resp.close()
-            _LOGGER.debug(resp_data)
-            return resp_data
-        except Exception as err:
-            _LOGGER.debug("error during request", exc_info=err)
-            time.sleep(1)
-    return None
-
-
-def gcm_check_in(androidId=None, securityToken=None, **kwargs):
-    """
-    perform check-in request
-
-    androidId, securityToken can be provided if we already did the initial
-    check-in
-
-    returns dict with androidId, securityToken and more
-    """
-    chrome = ChromeBuildProto()
-    chrome.platform = 3
-    chrome.chrome_version = "63.0.3234.0"
-    chrome.channel = 1
-
-    checkin = AndroidCheckinProto()
-    checkin.type = 3
-    checkin.chrome_build.CopyFrom(chrome)  # pylint: disable=maybe-no-member
-
-    payload = AndroidCheckinRequest()
-    payload.user_serial_number = 0
-    payload.checkin.CopyFrom(checkin)  # pylint: disable=maybe-no-member
-    payload.version = 3
-    if androidId:
-        payload.id = int(androidId)
-    if securityToken:
-        payload.security_token = int(securityToken)
-
-    _LOGGER.debug(payload)
-    req = Request(
-        url=CHECKIN_URL,
-        headers={"Content-Type": "application/x-protobuf"},
-        data=payload.SerializeToString(),
-    )
-    resp_data = __do_request(req)
-    resp = AndroidCheckinResponse()
-    resp.ParseFromString(resp_data)
-    _LOGGER.debug(resp)
-    return MessageToDict(resp)
-
-
-def urlsafe_base64(data):
-    """
-    base64-encodes data with -_ instead of +/ and removes all = padding.
-    also strips newlines
-
-    returns a string
-    """
-    res = urlsafe_b64encode(data).replace(b"=", b"")
-    return res.replace(b"\n", b"").decode("ascii")
-
-
-def gcm_register(appId, retries=5, **kwargs):
-    """
-    obtains a gcm token
-
-    appId: app id as an integer
-    retries: number of failed requests before giving up
-
-    returns {"token": "...", "appId": 123123, "androidId":123123,
-             "securityToken": 123123}
-    """
-    # contains androidId, securityToken and more
-    chk = gcm_check_in()
-    _LOGGER.debug(chk)
-    body = {
-        "app": "org.chromium.linux",
-        "X-subtype": appId,
-        "device": chk["androidId"],
-        "sender": urlsafe_base64(SERVER_KEY),
-    }
-    data = urlencode(body)
-    _LOGGER.debug(data)
-    auth = "AidLogin {}:{}".format(chk["androidId"], chk["securityToken"])
-    req = Request(
-        url=REGISTER_URL, headers={"Authorization": auth}, data=data.encode("utf-8")
-    )
-    for _ in range(retries):
-        resp_data = __do_request(req, retries)
-        if b"Error" in resp_data:
-            err = resp_data.decode("utf-8")
-            _LOGGER.error("Register request has failed with %d", err)
-            continue
-        token = resp_data.decode("utf-8").split("=")[1]
-        chkfields = {k: chk[k] for k in ["androidId", "securityToken"]}
-        res = {"token": token, "appId": appId}
-        res.update(chkfields)
-        return res
-    return None
-
-
-def fcm_register(sender_id, token, retries=5):
-    """
-    generates key pair and obtains a fcm token
-
-    sender_id: sender id as an integer
-    token: the subscription token in the dict returned by gcm_register
-
-    returns {"keys": keys, "fcm": {...}}
-    """
-    # I used this analyzer to figure out how to slice the asn1 structs
-    # https://lapo.it/asn1js
-    # first byte of public key is skipped for some reason
-    # maybe it's always zero
-    public, private = generate_pair("ec", curve=str("secp256r1"))
-
-    _LOGGER.debug("# public")
-    _LOGGER.debug(b64encode(public.asn1.dump()))
-    _LOGGER.debug("# private")
-    _LOGGER.debug(b64encode(private.asn1.dump()))
-    keys = {
-        "public": urlsafe_base64(public.asn1.dump()[26:]),
-        "private": urlsafe_base64(private.asn1.dump()),
-        "secret": urlsafe_base64(os.urandom(16)),
-    }
-    data = urlencode(
-        {
-            "authorized_entity": sender_id,
-            "endpoint": "{}/{}".format(FCM_ENDPOINT, token),
-            "encryption_key": keys["public"],
-            "encryption_auth": keys["secret"],
-        }
-    )
-    _LOGGER.debug(data)
-    req = Request(url=FCM_SUBSCRIBE, data=data.encode("utf-8"))
-    resp_data = __do_request(req, retries)
-    return {"keys": keys, "fcm": json.loads(resp_data.decode("utf-8"))}
-
-
-def register(sender_id):
-    """register gcm and fcm tokens for sender_id"""
-    app_id = "wp:receiver.push.com#{}".format(uuid.uuid4())
-    subscription = gcm_register(appId=app_id)
-    _LOGGER.debug(subscription)
-    fcm = fcm_register(sender_id=sender_id, token=subscription["token"])
-    _LOGGER.debug(fcm)
-    res = {"gcm": subscription}
-    res.update(fcm)
-    return res
-
-
-# -------------------------------------------------------------------------
-
-
 MCS_VERSION = 41
-
 PACKET_BY_TAG = [
     HeartbeatPing,
     HeartbeatAck,
     LoginRequest,
     LoginResponse,
     Close,
     "MessageStanza",
@@ -229,279 +70,441 @@
     "HttpResponse",
     "BindAccountRequest",
     "BindAccountResponse",
     "TalkMetadata",
 ]
 
 
-def __read(sock, size):
-    buf = b""
-    while len(buf) < size:
-        buf += sock.recv(size - len(buf))
-    return buf
-
-
-# protobuf variable length integers are encoded in base 128
-# each byte contains 7 bits of the integer and the msb is set if there's
-# more. pretty simple to implement
-
-
-def __read_varint32(value):
-    res = 0
-    shift = 0
-    while True:
-        (b,) = struct.unpack("B", __read(value, 1))
-        res |= (b & 0x7F) << shift
-        if (b & 0x80) == 0:
-            break
-        shift += 7
-    return res
-
-
-def __encode_varint32(value):
-    res = bytearray([])
-    while value != 0:
-        b = value & 0x7F
-        value >>= 7
-        if value != 0:
-            b |= 0x80
-        res.append(b)
-    return bytes(res)
-
-
-def __send(google_socket, data):
-    header = bytearray([MCS_VERSION, PACKET_BY_TAG.index(type(data))])
-    _LOGGER.debug(data)
-    payload = data.SerializeToString()
-    buf = bytes(header) + __encode_varint32(len(payload)) + payload
-    _LOGGER.debug(hexlify(buf))
-    total = 0
-    while total < len(buf):
-        sent = google_socket.send(buf[total:])
-        if sent == 0:
-            raise RuntimeError("socket connection broken")
-        total += sent
-
-
-def __recv(data, first=False):
-
-    try:
-        readable, _, _ = select.select(
-            [
-                data,
-            ],
-            [],
-            [],
-            READ_TIMEOUT_SECS,
-        )
-        if len(readable) == 0:
-            _LOGGER.debug("Select read timeout")
-            return None
 
-    except select.error:
-        _LOGGER.debug("Select error")
+
+class FCMRegistration:
+    
+    
+    def __init__(
+        self,
+    ) -> None:
+
+        self.blank = '123'
+
+    def __do_request(self, req, retries=5):
+        for _ in range(retries):
+            try:
+                resp = urlopen(req)
+                resp_data = resp.read()
+                resp.close()
+                _LOGGER.debug(resp_data)
+                return resp_data
+            except Exception as err:
+                _LOGGER.debug("error during request", exc_info=err)
+                time.sleep(1)
         return None
 
-    _LOGGER.debug("Data available to read")
 
-    if first:
-        version, tag = struct.unpack("BB", __read(data, 2))
-        _LOGGER.debug("version %s", version)
-        if version < MCS_VERSION and version != 38:
-            raise RuntimeError("protocol version {} unsupported".format(version))
-    else:
-        (tag,) = struct.unpack("B", __read(data, 1))
-    _LOGGER.debug("tag %s (%s)", tag, PACKET_BY_TAG[tag])
-    size = __read_varint32(data)
-    _LOGGER.debug("size %s", size)
-    if size >= 0:
-        buf = __read(data, size)
-        _LOGGER.debug(hexlify(buf))
-        packet = PACKET_BY_TAG[tag]
-        payload = packet()
-        payload.ParseFromString(buf)
+    def gcm_check_in(self, androidId=None, securityToken=None, **kwargs):
+        """
+        perform check-in request
+
+        androidId, securityToken can be provided if we already did the initial
+        check-in
+
+        returns dict with androidId, securityToken and more
+        """
+        chrome = ChromeBuildProto()
+        chrome.platform = 3
+        chrome.chrome_version = "63.0.3234.0"
+        chrome.channel = 1
+
+        checkin = AndroidCheckinProto()
+        checkin.type = 3
+        checkin.chrome_build.CopyFrom(chrome)  # pylint: disable=maybe-no-member
+
+        payload = AndroidCheckinRequest()
+        payload.user_serial_number = 0
+        payload.checkin.CopyFrom(checkin)  # pylint: disable=maybe-no-member
+        payload.version = 3
+        if androidId:
+            payload.id = int(androidId)
+        if securityToken:
+            payload.security_token = int(securityToken)
+
         _LOGGER.debug(payload)
-        return payload
-    return None
+        req = Request(
+            url=CHECKIN_URL,
+            headers={"Content-Type": "application/x-protobuf"},
+            data=payload.SerializeToString(),
+        )
+        resp_data = self.__do_request(req)
+        resp = AndroidCheckinResponse()
+        resp.ParseFromString(resp_data)
+        _LOGGER.debug(resp)
+        return MessageToDict(resp)
+
+
+    def urlsafe_base64(self, data):
+        """
+        base64-encodes data with -_ instead of +/ and removes all = padding.
+        also strips newlines
+
+        returns a string
+        """
+        res = urlsafe_b64encode(data).replace(b"=", b"")
+        return res.replace(b"\n", b"").decode("ascii")
+
+
+    def gcm_register(self, appId, retries=5, **kwargs):
+        """
+        obtains a gcm token
+
+        appId: app id as an integer
+        retries: number of failed requests before giving up
+
+        returns {"token": "...", "appId": 123123, "androidId":123123,
+                "securityToken": 123123}
+        """
+        # contains androidId, securityToken and more
+        chk = self.gcm_check_in()
+        _LOGGER.debug(chk)
+        body = {
+            "app": "org.chromium.linux",
+            "X-subtype": appId,
+            "device": chk["androidId"],
+            "sender": self.urlsafe_base64(SERVER_KEY),
+        }
+        data = urlencode(body)
+        _LOGGER.debug(data)
+        auth = "AidLogin {}:{}".format(chk["androidId"], chk["securityToken"])
+        req = Request(
+            url=REGISTER_URL, headers={"Authorization": auth}, data=data.encode("utf-8")
+        )
+        for _ in range(retries):
+            resp_data = self.__do_request(req, retries)
+            if b"Error" in resp_data:
+                err = resp_data.decode("utf-8")
+                _LOGGER.error("Register request has failed with %d", err)
+                continue
+            token = resp_data.decode("utf-8").split("=")[1]
+            chkfields = {k: chk[k] for k in ["androidId", "securityToken"]}
+            res = {"token": token, "appId": appId}
+            res.update(chkfields)
+            return res
+        return None
 
 
-def __app_data_by_key(data, key, blow_shit_up=True):
-    for item in data.app_data:
-        if item.key == key:
-            return item.value
-    if blow_shit_up:
-        raise RuntimeError("couldn't find in app_data {}".format(key))
-    return None
-
-
-def __open():
-
-    context = ssl.create_default_context()
-    google_socket = socket.create_connection((GOOGLE_MTALK_ENDPOINT, 5228))
-    google_socket = context.wrap_socket(
-        google_socket, server_hostname=GOOGLE_MTALK_ENDPOINT
-    )
-    _LOGGER.debug("connected to ssl socket")
-    return google_socket
-
-
-def __login(credentials, persistent_ids):
-    google_socket = __open()
-
-    gcm_check_in(**credentials["gcm"])
-    req = LoginRequest()
-    req.adaptive_heartbeat = False
-    req.auth_service = 2
-    req.auth_token = credentials["gcm"]["securityToken"]
-    req.id = "chrome-63.0.3234.0"
-    req.domain = "mcs.android.com"
-    req.device_id = "android-%x" % int(credentials["gcm"]["androidId"])
-    req.network_type = 1
-    req.resource = credentials["gcm"]["androidId"]
-    req.user = credentials["gcm"]["androidId"]
-    req.use_rmq2 = True
-    req.setting.add(name="new_vc", value="1")  # pylint: disable=maybe-no-member
-    req.received_persistent_id.extend(persistent_ids)  # pylint: disable=maybe-no-member
-    __send(google_socket, req)
-    login_response = __recv(google_socket, first=True)
-    _LOGGER.debug("Received login response: %s", login_response)
-    return google_socket
-
-
-def __reset(google_socket, credentials, persistent_ids):
-    last_reset = 0
-    now = time.time()
-    if now - last_reset < MIN_RESET_INTERVAL_SECS:
-        raise Exception("Too many connection reset attempts.")
-    last_reset = now
-    _LOGGER.debug("Reestablishing connection")
-    try:
-        google_socket.shutdown(2)
-        google_socket.close()
-    except OSError as err:
-        _LOGGER.debug("Unable to close connection %f", err)
-    return __login(credentials, persistent_ids)
+    def fcm_register(self, sender_id, token, retries=5):
+        """
+        generates key pair and obtains a fcm token
+
+        sender_id: sender id as an integer
+        token: the subscription token in the dict returned by gcm_register
+
+        returns {"keys": keys, "fcm": {...}}
+        """
+        # I used this analyzer to figure out how to slice the asn1 structs
+        # https://lapo.it/asn1js
+        # first byte of public key is skipped for some reason
+        # maybe it's always zero
+        public, private = generate_pair("ec", curve=str("secp256r1"))
+
+        _LOGGER.debug("# public")
+        _LOGGER.debug(b64encode(public.asn1.dump()))
+        _LOGGER.debug("# private")
+        _LOGGER.debug(b64encode(private.asn1.dump()))
+        keys = {
+            "public": self.urlsafe_base64(public.asn1.dump()[26:]),
+            "private": self.urlsafe_base64(private.asn1.dump()),
+            "secret": self.urlsafe_base64(os.urandom(16)),
+        }
+        data = urlencode(
+            {
+                "authorized_entity": sender_id,
+                "endpoint": "{}/{}".format(FCM_ENDPOINT, token),
+                "encryption_key": keys["public"],
+                "encryption_auth": keys["secret"],
+            }
+        )
+        _LOGGER.debug(data)
+        req = Request(url=FCM_SUBSCRIBE, data=data.encode("utf-8"))
+        resp_data = self.__do_request(req, retries)
+        return {"keys": keys, "fcm": json.loads(resp_data.decode("utf-8"))}
 
 
-def __listen(credentials, callback, persistent_ids, obj):
-    google_socket = __login(credentials, persistent_ids)
+    def register(self, sender_id):
+        """register gcm and fcm tokens for sender_id"""
+        app_id = "wp:receiver.push.com#{}".format(uuid.uuid4())
+        subscription = self.gcm_register(appId=app_id)
+        _LOGGER.debug(subscription)
+        fcm = self.fcm_register(sender_id=sender_id, token=subscription["token"])
+        _LOGGER.debug(fcm)
+        res = {"gcm": subscription}
+        res.update(fcm)
+        return res
+
+
+# -------------------------------------------------------------------------
+
+
+class FCMListener:
+
+    
+    def __init__(
+        self,
+    ) -> None:
+        self.fcm_registration = FCMRegistration()
+        self.received_persistent_ids = []
+
+
+    def __read(self, sock, size):
+        buf = b""
+        while len(buf) < size:
+            buf += sock.recv(size - len(buf))
+        return buf
+
+
+    # protobuf variable length integers are encoded in base 128
+    # each byte contains 7 bits of the integer and the msb is set if there's
+    # more. pretty simple to implement
+
+
+    def __read_varint32(self, value):
+        res = 0
+        shift = 0
+        while True:
+            (b,) = struct.unpack("B", self.__read(value, 1))
+            res |= (b & 0x7F) << shift
+            if (b & 0x80) == 0:
+                break
+            shift += 7
+        return res
+
+
+    def __encode_varint32(self, value):
+        res = bytearray([])
+        while value != 0:
+            b = value & 0x7F
+            value >>= 7
+            if value != 0:
+                b |= 0x80
+            res.append(b)
+        return bytes(res)
+
+
+    def __send(self, google_socket, data):
+        header = bytearray([MCS_VERSION, PACKET_BY_TAG.index(type(data))])
+        _LOGGER.debug(data)
+        payload = data.SerializeToString()
+        buf = bytes(header) + self.__encode_varint32(len(payload)) + payload
+        _LOGGER.debug(hexlify(buf))
+        total = 0
+        while total < len(buf):
+            sent = google_socket.send(buf[total:])
+            if sent == 0:
+                raise RuntimeError("socket connection broken")
+            total += sent
+
+
+    def __recv(self, data, first=False):
 
-    while True:
         try:
-            data = __recv(google_socket)
-            if isinstance(data, DataMessageStanza):
-                msg_id = __handle_data_message(data, credentials, callback, obj)
-                persistent_ids.append(msg_id)
-            elif isinstance(data, HeartbeatPing):
-                __handle_ping(google_socket, data)
-            elif data is None or isinstance(data, Close):
-                google_socket = __reset(google_socket, credentials, persistent_ids)
-            else:
-                _LOGGER.debug("Unexpected message type %s", type(data))
-        except ConnectionResetError:
-            _LOGGER.debug("Connection Reset: Reconnecting")
-            google_socket = __login(credentials, persistent_ids)
-
-
-def __handle_data_message(data, credentials, callback, obj):
-    load_der_private_key = serialization.load_der_private_key
-
-    crypto_key = __app_data_by_key(
-        data, "crypto-key", blow_shit_up=False
-    )  # Can be None
-    if crypto_key:
-        crypto_key = crypto_key[3:]  # strip dh=
-
-    salt = __app_data_by_key(data, "encryption", blow_shit_up=False)  # Can be None
-    if salt:
-        salt = salt[5:]  # strip salt=
-
-    crypto_key = urlsafe_b64decode(crypto_key.encode("ascii"))
-    salt = urlsafe_b64decode(salt.encode("ascii"))
-    der_data = credentials["keys"]["private"]
-    der_data = urlsafe_b64decode(der_data.encode("ascii") + b"========")
-    secret = credentials["keys"]["secret"]
-    secret = urlsafe_b64decode(secret.encode("ascii") + b"========")
-    privkey = load_der_private_key(der_data, password=None, backend=default_backend())
-    decrypted = http_ece.decrypt(
-        data.raw_data,
-        salt=salt,
-        private_key=privkey,
-        dh=crypto_key,
-        version="aesgcm",
-        auth_secret=secret,
-    )
-    _LOGGER.debug("Received data message %s: %s", data.persistent_id, decrypted)
-    callback(obj, json.loads(decrypted.decode("utf-8")), data)
-    return data.persistent_id
-
-
-def __handle_ping(google_socket, data):
-    _LOGGER.debug(
-        "Responding to ping: Stream ID: %s, Last: %s, Status: %s",
-        data.stream_id,
-        data.last_stream_id_received,
-        data.status,
-    )
-    req = HeartbeatAck()
-    req.stream_id = data.stream_id + 1
-    req.last_stream_id_received = data.stream_id
-    req.status = data.status
-    __send(google_socket, req)
-
-
-def listen(credentials, callback, received_persistent_ids=None, obj=None):
-    """
-    listens for push notifications
-
-    credentials: credentials object returned by register()
-    callback(obj, notification, data_message): called on notifications
-    received_persistent_ids: any persistent id's you already received.
-                             array of strings
-    obj: optional arbitrary value passed to callback
-    """
+            readable, _, _ = select.select(
+                [
+                    data,
+                ],
+                [],
+                [],
+                READ_TIMEOUT_SECS,
+            )
+            if len(readable) == 0:
+                _LOGGER.debug("Select read timeout")
+                return None
 
-    if received_persistent_ids is None:
-        received_persistent_ids = []
+        except select.error:
+            _LOGGER.debug("Select error")
+            return None
 
-    __listen(credentials, callback, received_persistent_ids, obj)
+        _LOGGER.debug("Data available to read")
 
+        if first:
+            version, tag = struct.unpack("BB", self.__read(data, 2))
+            _LOGGER.debug("version %s", version)
+            if version < MCS_VERSION and version != 38:
+                raise RuntimeError("protocol version {} unsupported".format(version))
+        else:
+            (tag,) = struct.unpack("B", self.__read(data, 1))
+        _LOGGER.debug("tag %s (%s)", tag, PACKET_BY_TAG[tag])
+        size = self.__read_varint32(data)
+        _LOGGER.debug("size %s", size)
+        if size >= 0:
+            buf = self.__read(data, size)
+            _LOGGER.debug(hexlify(buf))
+            packet = PACKET_BY_TAG[tag]
+            payload = packet()
+            payload.ParseFromString(buf)
+            _LOGGER.debug(payload)
+            return payload
+        return None
 
-def run_example():
-    """sample that registers a token and waits for notifications"""
 
-    logging.basicConfig(level=logging.INFO)
+    def __app_data_by_key(self, data, key, blow_shit_up=True):
+        for item in data.app_data:
+            if item.key == key:
+                return item.value
+        if blow_shit_up:
+            raise RuntimeError("couldn't find in app_data {}".format(key))
+        return None
 
-    data_path = appdirs.user_data_dir(appname="push_receiver", appauthor=False)
-    try:
-        os.makedirs(data_path)
-    except FileExistsError:
-        pass
-    credentials_path = os.path.join(data_path, "credentials.json")
-    persistent_ids_path = os.path.join(data_path, "persistent_ids")
-
-    try:
-        with open(credentials_path, "r", encoding="UTF-8") as cred_file:
-            credentials = json.load(cred_file)
-
-    except FileNotFoundError:
-        credentials = register(sender_id=int(GCF_SENDER_ID))
-        with open(credentials_path, "w", encoding="UTF-8") as cred_file:
-            json.dump(credentials, cred_file)
-
-    _LOGGER.debug(credentials)
-    print("send notifications to {}".format(credentials["fcm"]["token"]))
-
-    def on_notification(obj, notification, data_message):
-        idstr = data_message.persistent_id + "\n"
-        with open(persistent_ids_path, "r", encoding="UTF-8") as cred_file:
-            if idstr in cred_file:
-                return
-        with open(persistent_ids_path, "a", encoding="UTF-8") as cred_file:
-            cred_file.write(idstr)
-        print("Notification: \n")
-        print(json.dumps(notification, indent=2))
 
-    with open(persistent_ids_path, "a+", encoding="UTF-8") as cred_file:
-        received_persistent_ids = [x.strip() for x in cred_file]
+    def __open(self):
 
-    listen(credentials, on_notification, received_persistent_ids)
+        context = ssl.create_default_context()
+        google_socket = socket.create_connection((GOOGLE_MTALK_ENDPOINT, 5228))
+        google_socket = context.wrap_socket(
+            google_socket, server_hostname=GOOGLE_MTALK_ENDPOINT
+        )
+        _LOGGER.debug("connected to ssl socket")
+        return google_socket
+
+
+    def __login(self, credentials, persistent_ids):
+        google_socket = self.__open()
+
+        self.fcm_registration.gcm_check_in(**credentials["gcm"])
+        req = LoginRequest()
+        req.adaptive_heartbeat = False
+        req.auth_service = 2
+        req.auth_token = credentials["gcm"]["securityToken"]
+        req.id = "chrome-63.0.3234.0"
+        req.domain = "mcs.android.com"
+        req.device_id = "android-%x" % int(credentials["gcm"]["androidId"])
+        req.network_type = 1
+        req.resource = credentials["gcm"]["androidId"]
+        req.user = credentials["gcm"]["androidId"]
+        req.use_rmq2 = True
+        req.setting.add(name="new_vc", value="1")  # pylint: disable=maybe-no-member
+        req.received_persistent_id.extend(persistent_ids)  # pylint: disable=maybe-no-member
+        self.__send(google_socket, req)
+        login_response = self.__recv(google_socket, first=True)
+        _LOGGER.debug("Received login response: %s", login_response)
+        return google_socket
+
+
+    def __reset(self, google_socket, credentials, persistent_ids):
+        last_reset = 0
+        now = time.time()
+        if now - last_reset < MIN_RESET_INTERVAL_SECS:
+            raise Exception("Too many connection reset attempts.")
+        last_reset = now
+        _LOGGER.debug("Reestablishing connection")
+        try:
+            google_socket.shutdown(2)
+            google_socket.close()
+        except OSError as err:
+            _LOGGER.debug("Unable to close connection %f", err)
+        return self.__login(credentials, persistent_ids)
+
+
+    def __listen(self, credentials, callback, persistent_ids, obj):
+        google_socket = self.__login(credentials, persistent_ids)
+
+        while True:
+            try:
+                data = self.__recv(google_socket)
+                if isinstance(data, DataMessageStanza):
+                    msg_id = self.__handle_data_message(data, credentials, callback, obj)
+                    persistent_ids.append(msg_id)
+                elif isinstance(data, HeartbeatPing):
+                    self.__handle_ping(google_socket, data)
+                elif data is None or isinstance(data, Close):
+                    google_socket = self.__reset(google_socket, credentials, persistent_ids)
+                else:
+                    _LOGGER.debug("Unexpected message type %s", type(data))
+            except ConnectionResetError:
+                _LOGGER.debug("Connection Reset: Reconnecting")
+                google_socket = self.__login(credentials, persistent_ids)
+
+
+    def __handle_data_message(self, data, credentials, callback, obj):
+        load_der_private_key = serialization.load_der_private_key
+
+        crypto_key = self.__app_data_by_key(
+            data, "crypto-key", blow_shit_up=False
+        )  # Can be None
+        if crypto_key:
+            crypto_key = crypto_key[3:]  # strip dh=
+
+        salt = self.__app_data_by_key(data, "encryption", blow_shit_up=False)  # Can be None
+        if salt:
+            salt = salt[5:]  # strip salt=
+
+        crypto_key = urlsafe_b64decode(crypto_key.encode("ascii"))
+        salt = urlsafe_b64decode(salt.encode("ascii"))
+        der_data = credentials["keys"]["private"]
+        der_data = urlsafe_b64decode(der_data.encode("ascii") + b"========")
+        secret = credentials["keys"]["secret"]
+        secret = urlsafe_b64decode(secret.encode("ascii") + b"========")
+        privkey = load_der_private_key(der_data, password=None, backend=default_backend())
+        decrypted = http_ece.decrypt(
+            data.raw_data,
+            salt=salt,
+            private_key=privkey,
+            dh=crypto_key,
+            version="aesgcm",
+            auth_secret=secret,
+        )
+        _LOGGER.debug("Received data message %s: %s", data.persistent_id, decrypted)
+        callback(obj, json.loads(decrypted.decode("utf-8")), data)
+        return data.persistent_id
+
+
+    def __handle_ping(self, google_socket, data):
+        _LOGGER.debug(
+            "Responding to ping: Stream ID: %s, Last: %s, Status: %s",
+            data.stream_id,
+            data.last_stream_id_received,
+            data.status,
+        )
+        req = HeartbeatAck()
+        req.stream_id = data.stream_id + 1
+        req.last_stream_id_received = data.stream_id
+        req.status = data.status
+        self.__send(google_socket, req)
+
+
+    def listen(self, credentials, callback, received_persistent_ids=None, obj=None):
+        """
+        listens for push notifications
+
+        credentials: credentials object returned by register()
+        callback(obj, notification, data_message): called on notifications
+        received_persistent_ids: any persistent id's you already received.
+                                array of strings
+        obj: optional arbitrary value passed to callback
+        """
+        received_persistent_ids = []
+        if received_persistent_ids is None:
+            received_persistent_ids = []
+
+        self.__listen(credentials, callback, received_persistent_ids, obj)
+
+
+    def runner(self, callback, credentials = None, persistent_ids = None):
+        """sample that registers a token and waits for notifications"""
+        logging.basicConfig(level=logging.INFO)
+        if persistent_ids is None:
+            persistent_ids = []
+            
+        if credentials is None:
+            credentials = self.fcm_registration.register(sender_id=int(GCF_SENDER_ID))
+            _credentials = {"credentials" : credentials}
+            callback(_credentials) #doesn't do anything for now. Using a different method currently
+
+        def on_notification(obj, notification, data_message):
+            idstr = data_message.persistent_id
+            if idstr in persistent_ids:
+                return
+            persistent_ids.append(idstr)
+            self.received_persistent_ids = persistent_ids
+            _new_persistend_ids = {"new_persistent_id" : idstr}
+            callback(_new_persistend_ids)
+            _notification = {"notification" : notification}
+            callback(_notification)
+            _LOGGER.debug(_notification)        
+        self.listen(credentials, on_notification, self.received_persistent_ids)
```

### Comparing `pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod.egg-info/PKG-INFO` & `pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.2.0b8
+Version: 1.3.0b3
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod.egg-info/SOURCES.txt` & `pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 pyhyypapihawkmod/__main__.py
 pyhyypapihawkmod/alarm_info.py
 pyhyypapihawkmod/android_checkin_pb2.py
 pyhyypapihawkmod/checkin_pb2.py
 pyhyypapihawkmod/client.py
 pyhyypapihawkmod/constants.py
 pyhyypapihawkmod/exceptions.py
+pyhyypapihawkmod/imei.py
 pyhyypapihawkmod/mcs_pb2.py
 pyhyypapihawkmod/push_receiver.py
 pyhyypapihawkmod.egg-info/PKG-INFO
 pyhyypapihawkmod.egg-info/SOURCES.txt
 pyhyypapihawkmod.egg-info/dependency_links.txt
 pyhyypapihawkmod.egg-info/requires.txt
 pyhyypapihawkmod.egg-info/top_level.txt
```

### Comparing `pyhyypapihawkmod-1.2.0b8/setup.py` & `pyhyypapihawkmod-1.3.0b3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhyypapihawkmod',
-    version="1.2.0b8",
+    version="1.3.0b3",
     license='Apache Software License 2.0',
     author='hawky358 (Original code by Renier Moorcroft)',
     author_email='hawky358@users.github.com',
     description='IDS Hyyp/ADT Secure Home API',
     long_description="API for accessing IDS Hyyp. This is used by ADT Home Connect and possibly others. Please view readme on github (Based on 0.0.0.8 by Renier Moorcroft with updated protobuf files) ",
     url='https://github.com/hawky358/pyHyypApi',
     packages=setuptools.find_packages(),
```

