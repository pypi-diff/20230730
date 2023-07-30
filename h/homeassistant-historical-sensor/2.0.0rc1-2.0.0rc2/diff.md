# Comparing `tmp/homeassistant-historical-sensor-2.0.0rc1.tar.gz` & `tmp/homeassistant-historical-sensor-2.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homeassistant-historical-sensor-2.0.0rc1.tar", last modified: Mon Jul 17 15:31:58 2023, max compression
+gzip compressed data, was "homeassistant-historical-sensor-2.0.0rc2.tar", last modified: Sun Jul 30 15:37:39 2023, max compression
```

## Comparing `homeassistant-historical-sensor-2.0.0rc1.tar` & `homeassistant-historical-sensor-2.0.0rc2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:31:58.910909 homeassistant-historical-sensor-2.0.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-17 15:31:58.910909 homeassistant-historical-sensor-2.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-17 15:31:47.000000 homeassistant-historical-sensor-2.0.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:31:58.906909 homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor/
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-17 15:31:47.000000 homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-17 15:31:47.000000 homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-07-17 15:31:47.000000 homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-17 15:31:47.000000 homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor/recorderutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    14581 2023-07-17 15:31:47.000000 homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-17 15:31:47.000000 homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:31:58.910909 homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-17 15:31:58.000000 homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-17 15:31:58.000000 homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:31:58.000000 homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 15:31:58.000000 homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-17 15:31:47.000000 homeassistant-historical-sensor-2.0.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-17 15:31:58.910909 homeassistant-historical-sensor-2.0.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:37:39.756650 homeassistant-historical-sensor-2.0.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-30 15:37:39.756650 homeassistant-historical-sensor-2.0.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-30 15:37:30.000000 homeassistant-historical-sensor-2.0.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:37:39.756650 homeassistant-historical-sensor-2.0.0rc2/homeassistant_historical_sensor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-30 15:37:30.000000 homeassistant-historical-sensor-2.0.0rc2/homeassistant_historical_sensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-30 15:37:30.000000 homeassistant-historical-sensor-2.0.0rc2/homeassistant_historical_sensor/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-07-30 15:37:30.000000 homeassistant-historical-sensor-2.0.0rc2/homeassistant_historical_sensor/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-30 15:37:30.000000 homeassistant-historical-sensor-2.0.0rc2/homeassistant_historical_sensor/recorderutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14592 2023-07-30 15:37:30.000000 homeassistant-historical-sensor-2.0.0rc2/homeassistant_historical_sensor/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-30 15:37:30.000000 homeassistant-historical-sensor-2.0.0rc2/homeassistant_historical_sensor/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:37:39.756650 homeassistant-historical-sensor-2.0.0rc2/homeassistant_historical_sensor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-30 15:37:39.000000 homeassistant-historical-sensor-2.0.0rc2/homeassistant_historical_sensor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-30 15:37:39.000000 homeassistant-historical-sensor-2.0.0rc2/homeassistant_historical_sensor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 15:37:39.000000 homeassistant-historical-sensor-2.0.0rc2/homeassistant_historical_sensor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-30 15:37:39.000000 homeassistant-historical-sensor-2.0.0rc2/homeassistant_historical_sensor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-30 15:37:30.000000 homeassistant-historical-sensor-2.0.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-30 15:37:39.756650 homeassistant-historical-sensor-2.0.0rc2/setup.cfg
```

### Comparing `homeassistant-historical-sensor-2.0.0rc1/PKG-INFO` & `homeassistant-historical-sensor-2.0.0rc2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeassistant-historical-sensor
-Version: 2.0.0rc1
+Version: 2.0.0rc2
 Summary: Historical sensors for HomeAssistant
 Home-page: https://github.com/ldotlopez/ha-historical-sensor
 Author: Luis López
 Author-email: luis@cuarentaydos.com
 Project-URL: Repository, https://github.com/ldotlopez/ha-historical-sensor/
 Project-URL: Bug Tracker, https://github.com/ldotlopez/ha-historical-sensor/issues
 Requires-Python: >=3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 2.0.0rc1
+Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 2.0.0rc2
 Summary: Historical sensors for HomeAssistant Home-page: https://github.com/
 ldotlopez/ha-historical-sensor Author: Luis LÃ³pez Author-email:
 luis@cuarentaydos.com Project-URL: Repository, https://github.com/ldotlopez/ha-
 historical-sensor/ Project-URL: Bug Tracker, https://github.com/ldotlopez/ha-
 historical-sensor/issues Requires-Python: >=3.10 Description-Content-Type:
 text/markdown # Historical sensors for Home Assistant ![](icon-64.png)  !
 [GitHub Release (latest SemVer including pre-releases)](https://img.shields.io/
```

### Comparing `homeassistant-historical-sensor-2.0.0rc1/README.md` & `homeassistant-historical-sensor-2.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor/__init__.py` & `homeassistant-historical-sensor-2.0.0rc2/homeassistant_historical_sensor/__init__.py`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor/consts.py` & `homeassistant-historical-sensor-2.0.0rc2/homeassistant_historical_sensor/consts.py`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor/patches.py` & `homeassistant-historical-sensor-2.0.0rc2/homeassistant_historical_sensor/patches.py`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor/recorderutil.py` & `homeassistant-historical-sensor-2.0.0rc2/homeassistant_historical_sensor/recorderutil.py`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor/sensor.py` & `homeassistant-historical-sensor-2.0.0rc2/homeassistant_historical_sensor/sensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301,
 # USA.
 
 
 import logging
 from abc import abstractmethod
-from datetime import timedelta
+from datetime import datetime, timedelta
 
 import sqlalchemy.exc
 import sqlalchemy.orm
 from homeassistant.components import recorder
 from homeassistant.components.recorder import db_schema
 from homeassistant.components.recorder.models import StatisticData, StatisticMetaData
 from homeassistant.components.recorder.statistics import (
@@ -392,23 +392,23 @@
 
         await super().async_added_to_hass()
 
         _LOGGER.debug(f"{self.entity_id}: added to hass, do initial update")
         await self._async_historical_handle_update()
         self._remove_time_tracker_fn = async_track_time_interval(
             self.hass,
-            self._async_historical_handle_update,  # type: ignore[call-arg]
+            self._async_historical_handle_update,
             self.UPDATE_INTERVAL,
         )
 
         _LOGGER.debug(
             f"{self.entity_id}: "
             + f"updating each {self.UPDATE_INTERVAL.total_seconds()} seconds "
         )
 
     async def async_will_remove_from_hass(self) -> None:
         if self._remove_time_tracker_fn:
             self._remove_time_tracker_fn()
 
-    async def _async_historical_handle_update(self) -> None:
+    async def _async_historical_handle_update(self, _: datetime | None = None) -> None:
         await self.async_update_historical()
         await self.async_write_ha_historical_states()
```

### Comparing `homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor/state.py` & `homeassistant-historical-sensor-2.0.0rc2/homeassistant_historical_sensor/state.py`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor.egg-info/PKG-INFO` & `homeassistant-historical-sensor-2.0.0rc2/homeassistant_historical_sensor.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeassistant-historical-sensor
-Version: 2.0.0rc1
+Version: 2.0.0rc2
 Summary: Historical sensors for HomeAssistant
 Home-page: https://github.com/ldotlopez/ha-historical-sensor
 Author: Luis López
 Author-email: luis@cuarentaydos.com
 Project-URL: Repository, https://github.com/ldotlopez/ha-historical-sensor/
 Project-URL: Bug Tracker, https://github.com/ldotlopez/ha-historical-sensor/issues
 Requires-Python: >=3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 2.0.0rc1
+Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 2.0.0rc2
 Summary: Historical sensors for HomeAssistant Home-page: https://github.com/
 ldotlopez/ha-historical-sensor Author: Luis LÃ³pez Author-email:
 luis@cuarentaydos.com Project-URL: Repository, https://github.com/ldotlopez/ha-
 historical-sensor/ Project-URL: Bug Tracker, https://github.com/ldotlopez/ha-
 historical-sensor/issues Requires-Python: >=3.10 Description-Content-Type:
 text/markdown # Historical sensors for Home Assistant ![](icon-64.png)  !
 [GitHub Release (latest SemVer including pre-releases)](https://img.shields.io/
```

### Comparing `homeassistant-historical-sensor-2.0.0rc1/homeassistant_historical_sensor.egg-info/SOURCES.txt` & `homeassistant-historical-sensor-2.0.0rc2/homeassistant_historical_sensor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-2.0.0rc1/setup.cfg` & `homeassistant-historical-sensor-2.0.0rc2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = homeassistant-historical-sensor
-version = 2.0.0rc1
+version = 2.0.0rc2
 author = Luis López
 author_email = luis@cuarentaydos.com
 description = Historical sensors for HomeAssistant
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ldotlopez/ha-historical-sensor
 project_urls =
```

