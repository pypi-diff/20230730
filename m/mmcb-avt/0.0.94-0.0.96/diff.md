# Comparing `tmp/mmcb-avt-0.0.94.tar.gz` & `tmp/mmcb-avt-0.0.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmcb-avt-0.0.94.tar", last modified: Sun Jul 30 12:45:44 2023, max compression
+gzip compressed data, was "mmcb-avt-0.0.96.tar", last modified: Sun Jul 30 14:41:00 2023, max compression
```

## Comparing `mmcb-avt-0.0.94.tar` & `mmcb-avt-0.0.96.tar`

### file list

```diff
@@ -1,39 +1,38 @@
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-30 12:45:44.213572 mmcb-avt-0.0.94/
--rw-r--r--   0 avt        (501) staff       (20)    13827 2023-02-01 15:48:35.000000 mmcb-avt-0.0.94/LICENSE
--rw-r--r--   0 avt        (501) staff       (20)     9020 2023-07-30 12:45:44.212853 mmcb-avt-0.0.94/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)     7797 2023-05-12 10:49:39.000000 mmcb-avt-0.0.94/README.md
--rw-r--r--   0 avt        (501) staff       (20)      104 2023-05-17 14:30:45.000000 mmcb-avt-0.0.94/pyproject.toml
--rw-r--r--   0 avt        (501) staff       (20)       38 2023-07-30 12:45:44.213783 mmcb-avt-0.0.94/setup.cfg
--rw-r--r--   0 avt        (501) staff       (20)     2593 2023-07-30 12:44:08.000000 mmcb-avt-0.0.94/setup.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-30 12:45:44.169249 mmcb-avt-0.0.94/src/
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-30 12:45:44.203113 mmcb-avt-0.0.94/src/mmcb/
--rw-r--r--   0 avt        (501) staff       (20)        0 2022-05-29 13:37:50.000000 mmcb-avt-0.0.94/src/mmcb/__init__.py
--rw-r--r--   0 avt        (501) staff       (20)    93158 2023-07-28 13:44:08.000000 mmcb-avt-0.0.94/src/mmcb/common.py
--rw-r--r--   0 avt        (501) staff       (20)    33316 2023-07-30 12:44:34.000000 mmcb-avt-0.0.94/src/mmcb/configure_environment.py
--rw-r--r--   0 avt        (501) staff       (20)    33333 2023-07-30 10:51:05.000000 mmcb-avt-0.0.94/src/mmcb/configure_environment_2.py
--rwxr-xr-x   0 avt        (501) staff       (20)    14299 2023-07-28 13:44:08.000000 mmcb-avt-0.0.94/src/mmcb/dat2plot.py
--rwxr-xr-x   0 avt        (501) staff       (20)     9078 2023-03-06 10:10:59.000000 mmcb-avt-0.0.94/src/mmcb/dat2root.py
--rwxr-xr-x   0 avt        (501) staff       (20)    33782 2023-05-27 08:13:36.000000 mmcb-avt-0.0.94/src/mmcb/detect.py
--rwx------   0 avt        (501) staff       (20)     3235 2023-05-17 14:42:59.000000 mmcb-avt-0.0.94/src/mmcb/dmm.py
--rw-r--r--   0 avt        (501) staff       (20)     4688 2023-05-17 14:29:45.000000 mmcb-avt-0.0.94/src/mmcb/dmm_interface.py
--rwxr-xr-x   0 avt        (501) staff       (20)   112129 2023-03-06 09:12:53.000000 mmcb-avt-0.0.94/src/mmcb/iv.py
--rw-r--r--   0 avt        (501) staff       (20)    24909 2023-05-11 15:25:26.000000 mmcb-avt-0.0.94/src/mmcb/lexicon.py
--rwxr-xr-x   0 avt        (501) staff       (20)    12231 2023-03-08 10:55:33.000000 mmcb-avt-0.0.94/src/mmcb/liveplot.py
--rwxr-xr-x   0 avt        (501) staff       (20)     7040 2023-03-08 10:54:40.000000 mmcb-avt-0.0.94/src/mmcb/log2dat.py
--rwxr-xr-x   0 avt        (501) staff       (20)     7889 2023-02-01 16:03:37.000000 mmcb-avt-0.0.94/src/mmcb/peltier.py
--rwxr-xr-x   0 avt        (501) staff       (20)    33621 2023-03-06 10:22:31.000000 mmcb-avt-0.0.94/src/mmcb/psuset.py
--rwxr-xr-x   0 avt        (501) staff       (20)    21883 2023-03-06 09:13:15.000000 mmcb-avt-0.0.94/src/mmcb/psustat.py
--rwxr-xr-x   0 avt        (501) staff       (20)    13517 2023-05-27 08:13:52.000000 mmcb-avt-0.0.94/src/mmcb/sense.py
--rw-r--r--   0 avt        (501) staff       (20)    40226 2023-03-21 22:25:32.000000 mmcb-avt-0.0.94/src/mmcb/sensors.py
--rw-r--r--   0 avt        (501) staff       (20)    40258 2023-03-16 14:01:16.000000 mmcb-avt-0.0.94/src/mmcb/sensors_mod.py
--rw-r--r--   0 avt        (501) staff       (20)    17705 2023-03-08 09:27:13.000000 mmcb-avt-0.0.94/src/mmcb/sequence.py
--rwxr-xr-x   0 avt        (501) staff       (20)    17659 2023-03-06 09:10:49.000000 mmcb-avt-0.0.94/src/mmcb/ult80.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-30 12:45:44.210316 mmcb-avt-0.0.94/src/mmcb_avt.egg-info/
--rw-r--r--   0 avt        (501) staff       (20)     9020 2023-07-30 12:45:44.000000 mmcb-avt-0.0.94/src/mmcb_avt.egg-info/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)      730 2023-07-30 12:45:44.000000 mmcb-avt-0.0.94/src/mmcb_avt.egg-info/SOURCES.txt
--rw-r--r--   0 avt        (501) staff       (20)        1 2023-07-30 12:45:44.000000 mmcb-avt-0.0.94/src/mmcb_avt.egg-info/dependency_links.txt
--rw-r--r--   0 avt        (501) staff       (20)      330 2023-07-30 12:45:44.000000 mmcb-avt-0.0.94/src/mmcb_avt.egg-info/entry_points.txt
--rw-r--r--   0 avt        (501) staff       (20)      228 2023-07-30 12:45:44.000000 mmcb-avt-0.0.94/src/mmcb_avt.egg-info/requires.txt
--rw-r--r--   0 avt        (501) staff       (20)        5 2023-07-30 12:45:44.000000 mmcb-avt-0.0.94/src/mmcb_avt.egg-info/top_level.txt
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-30 12:45:44.211032 mmcb-avt-0.0.94/tests/
--rw-r--r--   0 avt        (501) staff       (20)      137 2023-05-14 12:24:42.000000 mmcb-avt-0.0.94/tests/test_lexicon.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-30 14:41:00.107931 mmcb-avt-0.0.96/
+-rw-r--r--   0 avt        (501) staff       (20)    13827 2023-02-01 15:48:35.000000 mmcb-avt-0.0.96/LICENSE
+-rw-r--r--   0 avt        (501) staff       (20)     9020 2023-07-30 14:41:00.107062 mmcb-avt-0.0.96/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)     7797 2023-05-12 10:49:39.000000 mmcb-avt-0.0.96/README.md
+-rw-r--r--   0 avt        (501) staff       (20)      104 2023-05-17 14:30:45.000000 mmcb-avt-0.0.96/pyproject.toml
+-rw-r--r--   0 avt        (501) staff       (20)       38 2023-07-30 14:41:00.108794 mmcb-avt-0.0.96/setup.cfg
+-rw-r--r--   0 avt        (501) staff       (20)     2593 2023-07-30 14:40:41.000000 mmcb-avt-0.0.96/setup.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-30 14:41:00.079760 mmcb-avt-0.0.96/src/
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-30 14:41:00.100664 mmcb-avt-0.0.96/src/mmcb/
+-rw-r--r--   0 avt        (501) staff       (20)        0 2022-05-29 13:37:50.000000 mmcb-avt-0.0.96/src/mmcb/__init__.py
+-rw-r--r--   0 avt        (501) staff       (20)    93158 2023-07-28 13:44:08.000000 mmcb-avt-0.0.96/src/mmcb/common.py
+-rw-r--r--   0 avt        (501) staff       (20)    33065 2023-07-30 14:39:18.000000 mmcb-avt-0.0.96/src/mmcb/configure_environment.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    14299 2023-07-28 13:44:08.000000 mmcb-avt-0.0.96/src/mmcb/dat2plot.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     9078 2023-03-06 10:10:59.000000 mmcb-avt-0.0.96/src/mmcb/dat2root.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    33782 2023-05-27 08:13:36.000000 mmcb-avt-0.0.96/src/mmcb/detect.py
+-rwx------   0 avt        (501) staff       (20)     3235 2023-05-17 14:42:59.000000 mmcb-avt-0.0.96/src/mmcb/dmm.py
+-rw-r--r--   0 avt        (501) staff       (20)     4688 2023-05-17 14:29:45.000000 mmcb-avt-0.0.96/src/mmcb/dmm_interface.py
+-rwxr-xr-x   0 avt        (501) staff       (20)   112129 2023-03-06 09:12:53.000000 mmcb-avt-0.0.96/src/mmcb/iv.py
+-rw-r--r--   0 avt        (501) staff       (20)    24909 2023-05-11 15:25:26.000000 mmcb-avt-0.0.96/src/mmcb/lexicon.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    12231 2023-03-08 10:55:33.000000 mmcb-avt-0.0.96/src/mmcb/liveplot.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     7040 2023-03-08 10:54:40.000000 mmcb-avt-0.0.96/src/mmcb/log2dat.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     7889 2023-02-01 16:03:37.000000 mmcb-avt-0.0.96/src/mmcb/peltier.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    33621 2023-03-06 10:22:31.000000 mmcb-avt-0.0.96/src/mmcb/psuset.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    21883 2023-03-06 09:13:15.000000 mmcb-avt-0.0.96/src/mmcb/psustat.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    13517 2023-05-27 08:13:52.000000 mmcb-avt-0.0.96/src/mmcb/sense.py
+-rw-r--r--   0 avt        (501) staff       (20)    40226 2023-03-21 22:25:32.000000 mmcb-avt-0.0.96/src/mmcb/sensors.py
+-rw-r--r--   0 avt        (501) staff       (20)    40258 2023-03-16 14:01:16.000000 mmcb-avt-0.0.96/src/mmcb/sensors_mod.py
+-rw-r--r--   0 avt        (501) staff       (20)    17705 2023-03-08 09:27:13.000000 mmcb-avt-0.0.96/src/mmcb/sequence.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    17659 2023-03-06 09:10:49.000000 mmcb-avt-0.0.96/src/mmcb/ult80.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-30 14:41:00.105083 mmcb-avt-0.0.96/src/mmcb_avt.egg-info/
+-rw-r--r--   0 avt        (501) staff       (20)     9020 2023-07-30 14:41:00.000000 mmcb-avt-0.0.96/src/mmcb_avt.egg-info/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)      694 2023-07-30 14:41:00.000000 mmcb-avt-0.0.96/src/mmcb_avt.egg-info/SOURCES.txt
+-rw-r--r--   0 avt        (501) staff       (20)        1 2023-07-30 14:41:00.000000 mmcb-avt-0.0.96/src/mmcb_avt.egg-info/dependency_links.txt
+-rw-r--r--   0 avt        (501) staff       (20)      330 2023-07-30 14:41:00.000000 mmcb-avt-0.0.96/src/mmcb_avt.egg-info/entry_points.txt
+-rw-r--r--   0 avt        (501) staff       (20)      228 2023-07-30 14:41:00.000000 mmcb-avt-0.0.96/src/mmcb_avt.egg-info/requires.txt
+-rw-r--r--   0 avt        (501) staff       (20)        5 2023-07-30 14:41:00.000000 mmcb-avt-0.0.96/src/mmcb_avt.egg-info/top_level.txt
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-30 14:41:00.105676 mmcb-avt-0.0.96/tests/
+-rw-r--r--   0 avt        (501) staff       (20)      137 2023-05-14 12:24:42.000000 mmcb-avt-0.0.96/tests/test_lexicon.py
```

### Comparing `mmcb-avt-0.0.94/LICENSE` & `mmcb-avt-0.0.96/LICENSE`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.94/PKG-INFO` & `mmcb-avt-0.0.96/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcb-avt
-Version: 0.0.94
+Version: 0.0.96
 Summary: ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.
 Home-page: https://gitlab.ph.liv.ac.uk/avt/atlas-itk-pmmcb
 Author: Alan Taylor, Manex Ormazabal
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mmcb-avt-0.0.94/README.md` & `mmcb-avt-0.0.96/README.md`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.94/setup.py` & `mmcb-avt-0.0.96/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="mmcb-avt",
-    version="0.0.94",
+    version="0.0.96",
     author="Alan Taylor, Manex Ormazabal",
     author_email="avt@hep.ph.liv.ac.uk",
     maintainer="Alan Taylor",
     maintainer_email="avt@hep.ph.liv.ac.uk",
     description="ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `mmcb-avt-0.0.94/src/mmcb/common.py` & `mmcb-avt-0.0.96/src/mmcb/common.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.94/src/mmcb/configure_environment.py` & `mmcb-avt-0.0.96/src/mmcb/configure_environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 tracker(ITK) pixels multi-module cycling box.
 
 This script is expected to run on a Raspberry Pi.
 """
 
 import collections
 import contextlib
+import functools
 import itertools
 import math
 import time
 
 import qwiic_tca9548a
 
 from mmcb import sensors
@@ -308,22 +309,14 @@
                     sensor1.sensor_i2c_address
                     for sensor1, sensor2 in itertools.combinations(
                         sensors_on_this_mux_channel, 2
                     )
                     if sensor1 == sensor2
                 }
 
-                # i2c_addresses_on_this_mux_channel = [
-                #     sensor.sensor_i2c_address
-                #     for sensor in sensors_on_this_mux
-                #     if sensor.multiplexer_channel == mux_channel
-                # ]
-                # counts = collections.Counter(i2c_addresses_on_this_mux_channel)
-                # duplicates = [k for k, v in counts.items() if v > 1]
-
                 if duplicates:
                     retval = False
                     print(
                         f'conflicting I2C addresses found on mux {hex(mux_address)} '
                         f'channel {mux_channel}: {", ".join(hex(x) for x in duplicates)}'
                     )
         return retval
@@ -427,24 +420,26 @@
             print(
                 'I2C address conflict between directly attached and '
                 f'multiplexer channel attached sensors: {", ".join(hex(x) for x in duplicates)}'
             )
 
         return retval
 
-    def _report_ntc_analogue_mux_channels_out_of_range(self):
+    def _report_analogue_mux_channels_out_of_range(self):
         """
         Report analogue multiplexer channels out of range, and that the NTC
         needs to have an analogue channel specified.
         """
 
         retval = True
+        sensors_with_multiple_inputs = [sensors.Ads1015, sensors.Pcf8591]
 
         for sensor in self._sensors:
-            if isinstance(sensor, sensors.AtlasNtc):
+            check = functools.partial(isinstance, sensor)
+            if any(map(check, sensors_with_multiple_inputs)):
                 if sensor.analogue_input not in sensor.supported_analogue_inputs:
                     retval = False
                     print(
                         f'{sensor.description}: analogue input not in '
                         f'{sensor.supported_analogue_inputs}: {sensor.analogue_input}'
                     )
 
@@ -514,15 +509,15 @@
             self._report_mux_i2c_not_in_range,
             self._report_mux_channel_not_in_range,
             self._report_mux_missing_address_or_channel,
             self._report_mux_conflicting_i2c_addresses_within_channels,
             self._report_mux_conflict_with_directly_connected_sensors,
             self._report_i2c_bus_directly_connected_conflicting_addresses,
             self._report_conflicting_i2c_addresses_between_channels_and_directly_connected,
-            self._report_ntc_analogue_mux_channels_out_of_range,
+            self._report_analogue_mux_channels_out_of_range,
             self._report_sensor_i2c_addresses_out_of_range,
             self._report_sensor_unsupported_thermocouple_type,
         )
         results = [report() for report in reports]
         configuration_ok = all(results)
         if not configuration_ok:
             self._sensors.clear()
```

### Comparing `mmcb-avt-0.0.94/src/mmcb/dat2plot.py` & `mmcb-avt-0.0.96/src/mmcb/dat2plot.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.94/src/mmcb/dat2root.py` & `mmcb-avt-0.0.96/src/mmcb/dat2root.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.94/src/mmcb/detect.py` & `mmcb-avt-0.0.96/src/mmcb/detect.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.94/src/mmcb/dmm.py` & `mmcb-avt-0.0.96/src/mmcb/dmm.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.94/src/mmcb/dmm_interface.py` & `mmcb-avt-0.0.96/src/mmcb/dmm_interface.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.94/src/mmcb/iv.py` & `mmcb-avt-0.0.96/src/mmcb/iv.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.94/src/mmcb/lexicon.py` & `mmcb-avt-0.0.96/src/mmcb/lexicon.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.94/src/mmcb/liveplot.py` & `mmcb-avt-0.0.96/src/mmcb/liveplot.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.94/src/mmcb/log2dat.py` & `mmcb-avt-0.0.96/src/mmcb/log2dat.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.94/src/mmcb/peltier.py` & `mmcb-avt-0.0.96/src/mmcb/peltier.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.94/src/mmcb/psuset.py` & `mmcb-avt-0.0.96/src/mmcb/psuset.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.94/src/mmcb/psustat.py` & `mmcb-avt-0.0.96/src/mmcb/psustat.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.94/src/mmcb/sense.py` & `mmcb-avt-0.0.96/src/mmcb/sense.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.94/src/mmcb/sensors.py` & `mmcb-avt-0.0.96/src/mmcb/sensors.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.94/src/mmcb/sensors_mod.py` & `mmcb-avt-0.0.96/src/mmcb/sensors_mod.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.94/src/mmcb/sequence.py` & `mmcb-avt-0.0.96/src/mmcb/sequence.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.94/src/mmcb/ult80.py` & `mmcb-avt-0.0.96/src/mmcb/ult80.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.94/src/mmcb_avt.egg-info/PKG-INFO` & `mmcb-avt-0.0.96/src/mmcb_avt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcb-avt
-Version: 0.0.94
+Version: 0.0.96
 Summary: ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.
 Home-page: https://gitlab.ph.liv.ac.uk/avt/atlas-itk-pmmcb
 Author: Alan Taylor, Manex Ormazabal
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mmcb-avt-0.0.94/src/mmcb_avt.egg-info/SOURCES.txt` & `mmcb-avt-0.0.96/src/mmcb_avt.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 src/mmcb/__init__.py
 src/mmcb/common.py
 src/mmcb/configure_environment.py
-src/mmcb/configure_environment_2.py
 src/mmcb/dat2plot.py
 src/mmcb/dat2root.py
 src/mmcb/detect.py
 src/mmcb/dmm.py
 src/mmcb/dmm_interface.py
 src/mmcb/iv.py
 src/mmcb/lexicon.py
```

