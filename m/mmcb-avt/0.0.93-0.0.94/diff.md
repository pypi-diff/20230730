# Comparing `tmp/mmcb-avt-0.0.93.tar.gz` & `tmp/mmcb-avt-0.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmcb-avt-0.0.93.tar", last modified: Fri Jul 28 13:45:42 2023, max compression
+gzip compressed data, was "mmcb-avt-0.0.94.tar", last modified: Sun Jul 30 12:45:44 2023, max compression
```

## Comparing `mmcb-avt-0.0.93.tar` & `mmcb-avt-0.0.94.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-28 13:45:42.291082 mmcb-avt-0.0.93/
--rw-r--r--   0 avt        (501) staff       (20)    13827 2023-02-01 15:48:35.000000 mmcb-avt-0.0.93/LICENSE
--rw-r--r--   0 avt        (501) staff       (20)     9020 2023-07-28 13:45:42.290212 mmcb-avt-0.0.93/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)     7797 2023-05-12 10:49:39.000000 mmcb-avt-0.0.93/README.md
--rw-r--r--   0 avt        (501) staff       (20)      104 2023-05-17 14:30:45.000000 mmcb-avt-0.0.93/pyproject.toml
--rw-r--r--   0 avt        (501) staff       (20)       38 2023-07-28 13:45:42.291291 mmcb-avt-0.0.93/setup.cfg
--rw-r--r--   0 avt        (501) staff       (20)     2593 2023-07-28 13:44:24.000000 mmcb-avt-0.0.93/setup.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-28 13:45:42.244313 mmcb-avt-0.0.93/src/
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-28 13:45:42.278929 mmcb-avt-0.0.93/src/mmcb/
--rw-r--r--   0 avt        (501) staff       (20)        0 2022-05-29 13:37:50.000000 mmcb-avt-0.0.93/src/mmcb/__init__.py
--rw-r--r--   0 avt        (501) staff       (20)    93158 2023-07-28 13:44:08.000000 mmcb-avt-0.0.93/src/mmcb/common.py
--rw-r--r--   0 avt        (501) staff       (20)    32436 2023-05-27 08:13:04.000000 mmcb-avt-0.0.93/src/mmcb/configure_environment.py
--rwxr-xr-x   0 avt        (501) staff       (20)    14299 2023-07-28 13:44:08.000000 mmcb-avt-0.0.93/src/mmcb/dat2plot.py
--rwxr-xr-x   0 avt        (501) staff       (20)     9078 2023-03-06 10:10:59.000000 mmcb-avt-0.0.93/src/mmcb/dat2root.py
--rwxr-xr-x   0 avt        (501) staff       (20)    33782 2023-05-27 08:13:36.000000 mmcb-avt-0.0.93/src/mmcb/detect.py
--rwx------   0 avt        (501) staff       (20)     3235 2023-05-17 14:42:59.000000 mmcb-avt-0.0.93/src/mmcb/dmm.py
--rw-r--r--   0 avt        (501) staff       (20)     4688 2023-05-17 14:29:45.000000 mmcb-avt-0.0.93/src/mmcb/dmm_interface.py
--rwxr-xr-x   0 avt        (501) staff       (20)   112129 2023-03-06 09:12:53.000000 mmcb-avt-0.0.93/src/mmcb/iv.py
--rw-r--r--   0 avt        (501) staff       (20)    24909 2023-05-11 15:25:26.000000 mmcb-avt-0.0.93/src/mmcb/lexicon.py
--rwxr-xr-x   0 avt        (501) staff       (20)    12231 2023-03-08 10:55:33.000000 mmcb-avt-0.0.93/src/mmcb/liveplot.py
--rwxr-xr-x   0 avt        (501) staff       (20)     7040 2023-03-08 10:54:40.000000 mmcb-avt-0.0.93/src/mmcb/log2dat.py
--rwxr-xr-x   0 avt        (501) staff       (20)     7889 2023-02-01 16:03:37.000000 mmcb-avt-0.0.93/src/mmcb/peltier.py
--rwxr-xr-x   0 avt        (501) staff       (20)    33621 2023-03-06 10:22:31.000000 mmcb-avt-0.0.93/src/mmcb/psuset.py
--rwxr-xr-x   0 avt        (501) staff       (20)    21883 2023-03-06 09:13:15.000000 mmcb-avt-0.0.93/src/mmcb/psustat.py
--rwxr-xr-x   0 avt        (501) staff       (20)    13517 2023-05-27 08:13:52.000000 mmcb-avt-0.0.93/src/mmcb/sense.py
--rw-r--r--   0 avt        (501) staff       (20)    40226 2023-03-21 22:25:32.000000 mmcb-avt-0.0.93/src/mmcb/sensors.py
--rw-r--r--   0 avt        (501) staff       (20)    40258 2023-03-16 14:01:16.000000 mmcb-avt-0.0.93/src/mmcb/sensors_mod.py
--rw-r--r--   0 avt        (501) staff       (20)    17705 2023-03-08 09:27:13.000000 mmcb-avt-0.0.93/src/mmcb/sequence.py
--rwxr-xr-x   0 avt        (501) staff       (20)    17659 2023-03-06 09:10:49.000000 mmcb-avt-0.0.93/src/mmcb/ult80.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-28 13:45:42.288231 mmcb-avt-0.0.93/src/mmcb_avt.egg-info/
--rw-r--r--   0 avt        (501) staff       (20)     9020 2023-07-28 13:45:42.000000 mmcb-avt-0.0.93/src/mmcb_avt.egg-info/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)      694 2023-07-28 13:45:42.000000 mmcb-avt-0.0.93/src/mmcb_avt.egg-info/SOURCES.txt
--rw-r--r--   0 avt        (501) staff       (20)        1 2023-07-28 13:45:42.000000 mmcb-avt-0.0.93/src/mmcb_avt.egg-info/dependency_links.txt
--rw-r--r--   0 avt        (501) staff       (20)      330 2023-07-28 13:45:42.000000 mmcb-avt-0.0.93/src/mmcb_avt.egg-info/entry_points.txt
--rw-r--r--   0 avt        (501) staff       (20)      228 2023-07-28 13:45:42.000000 mmcb-avt-0.0.93/src/mmcb_avt.egg-info/requires.txt
--rw-r--r--   0 avt        (501) staff       (20)        5 2023-07-28 13:45:42.000000 mmcb-avt-0.0.93/src/mmcb_avt.egg-info/top_level.txt
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-28 13:45:42.288992 mmcb-avt-0.0.93/tests/
--rw-r--r--   0 avt        (501) staff       (20)      137 2023-05-14 12:24:42.000000 mmcb-avt-0.0.93/tests/test_lexicon.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-30 12:45:44.213572 mmcb-avt-0.0.94/
+-rw-r--r--   0 avt        (501) staff       (20)    13827 2023-02-01 15:48:35.000000 mmcb-avt-0.0.94/LICENSE
+-rw-r--r--   0 avt        (501) staff       (20)     9020 2023-07-30 12:45:44.212853 mmcb-avt-0.0.94/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)     7797 2023-05-12 10:49:39.000000 mmcb-avt-0.0.94/README.md
+-rw-r--r--   0 avt        (501) staff       (20)      104 2023-05-17 14:30:45.000000 mmcb-avt-0.0.94/pyproject.toml
+-rw-r--r--   0 avt        (501) staff       (20)       38 2023-07-30 12:45:44.213783 mmcb-avt-0.0.94/setup.cfg
+-rw-r--r--   0 avt        (501) staff       (20)     2593 2023-07-30 12:44:08.000000 mmcb-avt-0.0.94/setup.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-30 12:45:44.169249 mmcb-avt-0.0.94/src/
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-30 12:45:44.203113 mmcb-avt-0.0.94/src/mmcb/
+-rw-r--r--   0 avt        (501) staff       (20)        0 2022-05-29 13:37:50.000000 mmcb-avt-0.0.94/src/mmcb/__init__.py
+-rw-r--r--   0 avt        (501) staff       (20)    93158 2023-07-28 13:44:08.000000 mmcb-avt-0.0.94/src/mmcb/common.py
+-rw-r--r--   0 avt        (501) staff       (20)    33316 2023-07-30 12:44:34.000000 mmcb-avt-0.0.94/src/mmcb/configure_environment.py
+-rw-r--r--   0 avt        (501) staff       (20)    33333 2023-07-30 10:51:05.000000 mmcb-avt-0.0.94/src/mmcb/configure_environment_2.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    14299 2023-07-28 13:44:08.000000 mmcb-avt-0.0.94/src/mmcb/dat2plot.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     9078 2023-03-06 10:10:59.000000 mmcb-avt-0.0.94/src/mmcb/dat2root.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    33782 2023-05-27 08:13:36.000000 mmcb-avt-0.0.94/src/mmcb/detect.py
+-rwx------   0 avt        (501) staff       (20)     3235 2023-05-17 14:42:59.000000 mmcb-avt-0.0.94/src/mmcb/dmm.py
+-rw-r--r--   0 avt        (501) staff       (20)     4688 2023-05-17 14:29:45.000000 mmcb-avt-0.0.94/src/mmcb/dmm_interface.py
+-rwxr-xr-x   0 avt        (501) staff       (20)   112129 2023-03-06 09:12:53.000000 mmcb-avt-0.0.94/src/mmcb/iv.py
+-rw-r--r--   0 avt        (501) staff       (20)    24909 2023-05-11 15:25:26.000000 mmcb-avt-0.0.94/src/mmcb/lexicon.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    12231 2023-03-08 10:55:33.000000 mmcb-avt-0.0.94/src/mmcb/liveplot.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     7040 2023-03-08 10:54:40.000000 mmcb-avt-0.0.94/src/mmcb/log2dat.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     7889 2023-02-01 16:03:37.000000 mmcb-avt-0.0.94/src/mmcb/peltier.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    33621 2023-03-06 10:22:31.000000 mmcb-avt-0.0.94/src/mmcb/psuset.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    21883 2023-03-06 09:13:15.000000 mmcb-avt-0.0.94/src/mmcb/psustat.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    13517 2023-05-27 08:13:52.000000 mmcb-avt-0.0.94/src/mmcb/sense.py
+-rw-r--r--   0 avt        (501) staff       (20)    40226 2023-03-21 22:25:32.000000 mmcb-avt-0.0.94/src/mmcb/sensors.py
+-rw-r--r--   0 avt        (501) staff       (20)    40258 2023-03-16 14:01:16.000000 mmcb-avt-0.0.94/src/mmcb/sensors_mod.py
+-rw-r--r--   0 avt        (501) staff       (20)    17705 2023-03-08 09:27:13.000000 mmcb-avt-0.0.94/src/mmcb/sequence.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    17659 2023-03-06 09:10:49.000000 mmcb-avt-0.0.94/src/mmcb/ult80.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-30 12:45:44.210316 mmcb-avt-0.0.94/src/mmcb_avt.egg-info/
+-rw-r--r--   0 avt        (501) staff       (20)     9020 2023-07-30 12:45:44.000000 mmcb-avt-0.0.94/src/mmcb_avt.egg-info/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)      730 2023-07-30 12:45:44.000000 mmcb-avt-0.0.94/src/mmcb_avt.egg-info/SOURCES.txt
+-rw-r--r--   0 avt        (501) staff       (20)        1 2023-07-30 12:45:44.000000 mmcb-avt-0.0.94/src/mmcb_avt.egg-info/dependency_links.txt
+-rw-r--r--   0 avt        (501) staff       (20)      330 2023-07-30 12:45:44.000000 mmcb-avt-0.0.94/src/mmcb_avt.egg-info/entry_points.txt
+-rw-r--r--   0 avt        (501) staff       (20)      228 2023-07-30 12:45:44.000000 mmcb-avt-0.0.94/src/mmcb_avt.egg-info/requires.txt
+-rw-r--r--   0 avt        (501) staff       (20)        5 2023-07-30 12:45:44.000000 mmcb-avt-0.0.94/src/mmcb_avt.egg-info/top_level.txt
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-30 12:45:44.211032 mmcb-avt-0.0.94/tests/
+-rw-r--r--   0 avt        (501) staff       (20)      137 2023-05-14 12:24:42.000000 mmcb-avt-0.0.94/tests/test_lexicon.py
```

### Comparing `mmcb-avt-0.0.93/LICENSE` & `mmcb-avt-0.0.94/LICENSE`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.93/PKG-INFO` & `mmcb-avt-0.0.94/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcb-avt
-Version: 0.0.93
+Version: 0.0.94
 Summary: ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.
 Home-page: https://gitlab.ph.liv.ac.uk/avt/atlas-itk-pmmcb
 Author: Alan Taylor, Manex Ormazabal
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mmcb-avt-0.0.93/README.md` & `mmcb-avt-0.0.94/README.md`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.93/setup.py` & `mmcb-avt-0.0.94/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="mmcb-avt",
-    version="0.0.93",
+    version="0.0.94",
     author="Alan Taylor, Manex Ormazabal",
     author_email="avt@hep.ph.liv.ac.uk",
     maintainer="Alan Taylor",
     maintainer_email="avt@hep.ph.liv.ac.uk",
     description="ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `mmcb-avt-0.0.93/src/mmcb/common.py` & `mmcb-avt-0.0.94/src/mmcb/common.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.93/src/mmcb/configure_environment.py` & `mmcb-avt-0.0.94/src/mmcb/configure_environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,35 +271,58 @@
                     f'{sensor.description}: '
                     'mux address and channel are both required'
                 )
 
         return retval
 
     def _report_mux_conflicting_i2c_addresses_within_channels(self):
-        """Report I2C address conflicts within multiplexer channels."""
+        """
+        Report I2C address conflicts within multiplexer channels.
+
+        Note that sensors on a mux channel with identical i2c addresses
+        are not regarded as duplicates if their analogue input channels are
+        different.
+        """
         retval = True
 
         for mux_address in self._unique_mux_addresses:
             sensors_on_this_mux = [
                 sensor
                 for sensor in self._sensors
                 if sensor.multiplexer_i2c_address == mux_address
             ]
             unique_channels_on_this_mux = {
                 sensor.multiplexer_channel for sensor in sensors_on_this_mux
             }
 
             for mux_channel in unique_channels_on_this_mux:
-                i2c_addresses_on_this_mux_channel = [
-                    sensor.sensor_i2c_address
+                sensors_on_this_mux_channel = (
+                    sensor
                     for sensor in sensors_on_this_mux
                     if sensor.multiplexer_channel == mux_channel
-                ]
-                counts = collections.Counter(i2c_addresses_on_this_mux_channel)
-                duplicates = [k for k, v in counts.items() if v > 1]
+                )
+
+                # worst case (1 mux, fully populated channel):
+                #     math.comb(255, 2) (n=32385)
+                # typical: less than 8 devices per mux channel (n=28)
+                duplicates = {
+                    sensor1.sensor_i2c_address
+                    for sensor1, sensor2 in itertools.combinations(
+                        sensors_on_this_mux_channel, 2
+                    )
+                    if sensor1 == sensor2
+                }
+
+                # i2c_addresses_on_this_mux_channel = [
+                #     sensor.sensor_i2c_address
+                #     for sensor in sensors_on_this_mux
+                #     if sensor.multiplexer_channel == mux_channel
+                # ]
+                # counts = collections.Counter(i2c_addresses_on_this_mux_channel)
+                # duplicates = [k for k, v in counts.items() if v > 1]
 
                 if duplicates:
                     retval = False
                     print(
                         f'conflicting I2C addresses found on mux {hex(mux_address)} '
                         f'channel {mux_channel}: {", ".join(hex(x) for x in duplicates)}'
                     )
```

### Comparing `mmcb-avt-0.0.93/src/mmcb/dat2plot.py` & `mmcb-avt-0.0.94/src/mmcb/dat2plot.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.93/src/mmcb/dat2root.py` & `mmcb-avt-0.0.94/src/mmcb/dat2root.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.93/src/mmcb/detect.py` & `mmcb-avt-0.0.94/src/mmcb/detect.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.93/src/mmcb/dmm.py` & `mmcb-avt-0.0.94/src/mmcb/dmm.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.93/src/mmcb/dmm_interface.py` & `mmcb-avt-0.0.94/src/mmcb/dmm_interface.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.93/src/mmcb/iv.py` & `mmcb-avt-0.0.94/src/mmcb/iv.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.93/src/mmcb/lexicon.py` & `mmcb-avt-0.0.94/src/mmcb/lexicon.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.93/src/mmcb/liveplot.py` & `mmcb-avt-0.0.94/src/mmcb/liveplot.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.93/src/mmcb/log2dat.py` & `mmcb-avt-0.0.94/src/mmcb/log2dat.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.93/src/mmcb/peltier.py` & `mmcb-avt-0.0.94/src/mmcb/peltier.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.93/src/mmcb/psuset.py` & `mmcb-avt-0.0.94/src/mmcb/psuset.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.93/src/mmcb/psustat.py` & `mmcb-avt-0.0.94/src/mmcb/psustat.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.93/src/mmcb/sense.py` & `mmcb-avt-0.0.94/src/mmcb/sense.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.93/src/mmcb/sensors.py` & `mmcb-avt-0.0.94/src/mmcb/sensors.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.93/src/mmcb/sensors_mod.py` & `mmcb-avt-0.0.94/src/mmcb/sensors_mod.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.93/src/mmcb/sequence.py` & `mmcb-avt-0.0.94/src/mmcb/sequence.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.93/src/mmcb/ult80.py` & `mmcb-avt-0.0.94/src/mmcb/ult80.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.93/src/mmcb_avt.egg-info/PKG-INFO` & `mmcb-avt-0.0.94/src/mmcb_avt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcb-avt
-Version: 0.0.93
+Version: 0.0.94
 Summary: ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.
 Home-page: https://gitlab.ph.liv.ac.uk/avt/atlas-itk-pmmcb
 Author: Alan Taylor, Manex Ormazabal
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mmcb-avt-0.0.93/src/mmcb_avt.egg-info/SOURCES.txt` & `mmcb-avt-0.0.94/src/mmcb_avt.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 src/mmcb/__init__.py
 src/mmcb/common.py
 src/mmcb/configure_environment.py
+src/mmcb/configure_environment_2.py
 src/mmcb/dat2plot.py
 src/mmcb/dat2root.py
 src/mmcb/detect.py
 src/mmcb/dmm.py
 src/mmcb/dmm_interface.py
 src/mmcb/iv.py
 src/mmcb/lexicon.py
```

