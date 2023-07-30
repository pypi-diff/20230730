# Comparing `tmp/mmcb-avt-0.0.96.tar.gz` & `tmp/mmcb-avt-0.0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmcb-avt-0.0.96.tar", last modified: Sun Jul 30 14:41:00 2023, max compression
+gzip compressed data, was "mmcb-avt-0.0.97.tar", last modified: Sun Jul 30 15:36:49 2023, max compression
```

## Comparing `mmcb-avt-0.0.96.tar` & `mmcb-avt-0.0.97.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-30 14:41:00.107931 mmcb-avt-0.0.96/
--rw-r--r--   0 avt        (501) staff       (20)    13827 2023-02-01 15:48:35.000000 mmcb-avt-0.0.96/LICENSE
--rw-r--r--   0 avt        (501) staff       (20)     9020 2023-07-30 14:41:00.107062 mmcb-avt-0.0.96/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)     7797 2023-05-12 10:49:39.000000 mmcb-avt-0.0.96/README.md
--rw-r--r--   0 avt        (501) staff       (20)      104 2023-05-17 14:30:45.000000 mmcb-avt-0.0.96/pyproject.toml
--rw-r--r--   0 avt        (501) staff       (20)       38 2023-07-30 14:41:00.108794 mmcb-avt-0.0.96/setup.cfg
--rw-r--r--   0 avt        (501) staff       (20)     2593 2023-07-30 14:40:41.000000 mmcb-avt-0.0.96/setup.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-30 14:41:00.079760 mmcb-avt-0.0.96/src/
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-30 14:41:00.100664 mmcb-avt-0.0.96/src/mmcb/
--rw-r--r--   0 avt        (501) staff       (20)        0 2022-05-29 13:37:50.000000 mmcb-avt-0.0.96/src/mmcb/__init__.py
--rw-r--r--   0 avt        (501) staff       (20)    93158 2023-07-28 13:44:08.000000 mmcb-avt-0.0.96/src/mmcb/common.py
--rw-r--r--   0 avt        (501) staff       (20)    33065 2023-07-30 14:39:18.000000 mmcb-avt-0.0.96/src/mmcb/configure_environment.py
--rwxr-xr-x   0 avt        (501) staff       (20)    14299 2023-07-28 13:44:08.000000 mmcb-avt-0.0.96/src/mmcb/dat2plot.py
--rwxr-xr-x   0 avt        (501) staff       (20)     9078 2023-03-06 10:10:59.000000 mmcb-avt-0.0.96/src/mmcb/dat2root.py
--rwxr-xr-x   0 avt        (501) staff       (20)    33782 2023-05-27 08:13:36.000000 mmcb-avt-0.0.96/src/mmcb/detect.py
--rwx------   0 avt        (501) staff       (20)     3235 2023-05-17 14:42:59.000000 mmcb-avt-0.0.96/src/mmcb/dmm.py
--rw-r--r--   0 avt        (501) staff       (20)     4688 2023-05-17 14:29:45.000000 mmcb-avt-0.0.96/src/mmcb/dmm_interface.py
--rwxr-xr-x   0 avt        (501) staff       (20)   112129 2023-03-06 09:12:53.000000 mmcb-avt-0.0.96/src/mmcb/iv.py
--rw-r--r--   0 avt        (501) staff       (20)    24909 2023-05-11 15:25:26.000000 mmcb-avt-0.0.96/src/mmcb/lexicon.py
--rwxr-xr-x   0 avt        (501) staff       (20)    12231 2023-03-08 10:55:33.000000 mmcb-avt-0.0.96/src/mmcb/liveplot.py
--rwxr-xr-x   0 avt        (501) staff       (20)     7040 2023-03-08 10:54:40.000000 mmcb-avt-0.0.96/src/mmcb/log2dat.py
--rwxr-xr-x   0 avt        (501) staff       (20)     7889 2023-02-01 16:03:37.000000 mmcb-avt-0.0.96/src/mmcb/peltier.py
--rwxr-xr-x   0 avt        (501) staff       (20)    33621 2023-03-06 10:22:31.000000 mmcb-avt-0.0.96/src/mmcb/psuset.py
--rwxr-xr-x   0 avt        (501) staff       (20)    21883 2023-03-06 09:13:15.000000 mmcb-avt-0.0.96/src/mmcb/psustat.py
--rwxr-xr-x   0 avt        (501) staff       (20)    13517 2023-05-27 08:13:52.000000 mmcb-avt-0.0.96/src/mmcb/sense.py
--rw-r--r--   0 avt        (501) staff       (20)    40226 2023-03-21 22:25:32.000000 mmcb-avt-0.0.96/src/mmcb/sensors.py
--rw-r--r--   0 avt        (501) staff       (20)    40258 2023-03-16 14:01:16.000000 mmcb-avt-0.0.96/src/mmcb/sensors_mod.py
--rw-r--r--   0 avt        (501) staff       (20)    17705 2023-03-08 09:27:13.000000 mmcb-avt-0.0.96/src/mmcb/sequence.py
--rwxr-xr-x   0 avt        (501) staff       (20)    17659 2023-03-06 09:10:49.000000 mmcb-avt-0.0.96/src/mmcb/ult80.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-30 14:41:00.105083 mmcb-avt-0.0.96/src/mmcb_avt.egg-info/
--rw-r--r--   0 avt        (501) staff       (20)     9020 2023-07-30 14:41:00.000000 mmcb-avt-0.0.96/src/mmcb_avt.egg-info/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)      694 2023-07-30 14:41:00.000000 mmcb-avt-0.0.96/src/mmcb_avt.egg-info/SOURCES.txt
--rw-r--r--   0 avt        (501) staff       (20)        1 2023-07-30 14:41:00.000000 mmcb-avt-0.0.96/src/mmcb_avt.egg-info/dependency_links.txt
--rw-r--r--   0 avt        (501) staff       (20)      330 2023-07-30 14:41:00.000000 mmcb-avt-0.0.96/src/mmcb_avt.egg-info/entry_points.txt
--rw-r--r--   0 avt        (501) staff       (20)      228 2023-07-30 14:41:00.000000 mmcb-avt-0.0.96/src/mmcb_avt.egg-info/requires.txt
--rw-r--r--   0 avt        (501) staff       (20)        5 2023-07-30 14:41:00.000000 mmcb-avt-0.0.96/src/mmcb_avt.egg-info/top_level.txt
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-30 14:41:00.105676 mmcb-avt-0.0.96/tests/
--rw-r--r--   0 avt        (501) staff       (20)      137 2023-05-14 12:24:42.000000 mmcb-avt-0.0.96/tests/test_lexicon.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-30 15:36:49.696299 mmcb-avt-0.0.97/
+-rw-r--r--   0 avt        (501) staff       (20)    13827 2023-02-01 15:48:35.000000 mmcb-avt-0.0.97/LICENSE
+-rw-r--r--   0 avt        (501) staff       (20)     9020 2023-07-30 15:36:49.695644 mmcb-avt-0.0.97/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)     7797 2023-05-12 10:49:39.000000 mmcb-avt-0.0.97/README.md
+-rw-r--r--   0 avt        (501) staff       (20)      104 2023-05-17 14:30:45.000000 mmcb-avt-0.0.97/pyproject.toml
+-rw-r--r--   0 avt        (501) staff       (20)       38 2023-07-30 15:36:49.696508 mmcb-avt-0.0.97/setup.cfg
+-rw-r--r--   0 avt        (501) staff       (20)     2593 2023-07-30 15:36:22.000000 mmcb-avt-0.0.97/setup.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-30 15:36:49.649848 mmcb-avt-0.0.97/src/
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-30 15:36:49.687917 mmcb-avt-0.0.97/src/mmcb/
+-rw-r--r--   0 avt        (501) staff       (20)        0 2022-05-29 13:37:50.000000 mmcb-avt-0.0.97/src/mmcb/__init__.py
+-rw-r--r--   0 avt        (501) staff       (20)    93158 2023-07-28 13:44:08.000000 mmcb-avt-0.0.97/src/mmcb/common.py
+-rw-r--r--   0 avt        (501) staff       (20)    33171 2023-07-30 15:36:07.000000 mmcb-avt-0.0.97/src/mmcb/configure_environment.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    14299 2023-07-28 13:44:08.000000 mmcb-avt-0.0.97/src/mmcb/dat2plot.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     9078 2023-03-06 10:10:59.000000 mmcb-avt-0.0.97/src/mmcb/dat2root.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    33782 2023-05-27 08:13:36.000000 mmcb-avt-0.0.97/src/mmcb/detect.py
+-rwx------   0 avt        (501) staff       (20)     3235 2023-05-17 14:42:59.000000 mmcb-avt-0.0.97/src/mmcb/dmm.py
+-rw-r--r--   0 avt        (501) staff       (20)     4688 2023-05-17 14:29:45.000000 mmcb-avt-0.0.97/src/mmcb/dmm_interface.py
+-rwxr-xr-x   0 avt        (501) staff       (20)   112129 2023-03-06 09:12:53.000000 mmcb-avt-0.0.97/src/mmcb/iv.py
+-rw-r--r--   0 avt        (501) staff       (20)    24909 2023-05-11 15:25:26.000000 mmcb-avt-0.0.97/src/mmcb/lexicon.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    12231 2023-03-08 10:55:33.000000 mmcb-avt-0.0.97/src/mmcb/liveplot.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     7040 2023-03-08 10:54:40.000000 mmcb-avt-0.0.97/src/mmcb/log2dat.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     7889 2023-02-01 16:03:37.000000 mmcb-avt-0.0.97/src/mmcb/peltier.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    33621 2023-03-06 10:22:31.000000 mmcb-avt-0.0.97/src/mmcb/psuset.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    21883 2023-03-06 09:13:15.000000 mmcb-avt-0.0.97/src/mmcb/psustat.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    13517 2023-05-27 08:13:52.000000 mmcb-avt-0.0.97/src/mmcb/sense.py
+-rw-r--r--   0 avt        (501) staff       (20)    40226 2023-03-21 22:25:32.000000 mmcb-avt-0.0.97/src/mmcb/sensors.py
+-rw-r--r--   0 avt        (501) staff       (20)    40258 2023-03-16 14:01:16.000000 mmcb-avt-0.0.97/src/mmcb/sensors_mod.py
+-rw-r--r--   0 avt        (501) staff       (20)    17705 2023-03-08 09:27:13.000000 mmcb-avt-0.0.97/src/mmcb/sequence.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    17659 2023-03-06 09:10:49.000000 mmcb-avt-0.0.97/src/mmcb/ult80.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-30 15:36:49.693724 mmcb-avt-0.0.97/src/mmcb_avt.egg-info/
+-rw-r--r--   0 avt        (501) staff       (20)     9020 2023-07-30 15:36:49.000000 mmcb-avt-0.0.97/src/mmcb_avt.egg-info/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)      694 2023-07-30 15:36:49.000000 mmcb-avt-0.0.97/src/mmcb_avt.egg-info/SOURCES.txt
+-rw-r--r--   0 avt        (501) staff       (20)        1 2023-07-30 15:36:49.000000 mmcb-avt-0.0.97/src/mmcb_avt.egg-info/dependency_links.txt
+-rw-r--r--   0 avt        (501) staff       (20)      330 2023-07-30 15:36:49.000000 mmcb-avt-0.0.97/src/mmcb_avt.egg-info/entry_points.txt
+-rw-r--r--   0 avt        (501) staff       (20)      228 2023-07-30 15:36:49.000000 mmcb-avt-0.0.97/src/mmcb_avt.egg-info/requires.txt
+-rw-r--r--   0 avt        (501) staff       (20)        5 2023-07-30 15:36:49.000000 mmcb-avt-0.0.97/src/mmcb_avt.egg-info/top_level.txt
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-07-30 15:36:49.694457 mmcb-avt-0.0.97/tests/
+-rw-r--r--   0 avt        (501) staff       (20)      137 2023-05-14 12:24:42.000000 mmcb-avt-0.0.97/tests/test_lexicon.py
```

### Comparing `mmcb-avt-0.0.96/LICENSE` & `mmcb-avt-0.0.97/LICENSE`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.96/PKG-INFO` & `mmcb-avt-0.0.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcb-avt
-Version: 0.0.96
+Version: 0.0.97
 Summary: ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.
 Home-page: https://gitlab.ph.liv.ac.uk/avt/atlas-itk-pmmcb
 Author: Alan Taylor, Manex Ormazabal
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mmcb-avt-0.0.96/README.md` & `mmcb-avt-0.0.97/README.md`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.96/setup.py` & `mmcb-avt-0.0.97/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="mmcb-avt",
-    version="0.0.96",
+    version="0.0.97",
     author="Alan Taylor, Manex Ormazabal",
     author_email="avt@hep.ph.liv.ac.uk",
     maintainer="Alan Taylor",
     maintainer_email="avt@hep.ph.liv.ac.uk",
     description="ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `mmcb-avt-0.0.96/src/mmcb/common.py` & `mmcb-avt-0.0.97/src/mmcb/common.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.96/src/mmcb/configure_environment.py` & `mmcb-avt-0.0.97/src/mmcb/configure_environment.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,29 +422,32 @@
                 f'multiplexer channel attached sensors: {", ".join(hex(x) for x in duplicates)}'
             )
 
         return retval
 
     def _report_analogue_mux_channels_out_of_range(self):
         """
-        Report analogue multiplexer channels out of range, and that the NTC
+        Report analogue multiplexer channels out of range, and that the sensor
         needs to have an analogue channel specified.
         """
 
         retval = True
         sensors_with_multiple_inputs = [sensors.Ads1015, sensors.Pcf8591]
 
         for sensor in self._sensors:
             check = functools.partial(isinstance, sensor)
             if any(map(check, sensors_with_multiple_inputs)):
                 if sensor.analogue_input not in sensor.supported_analogue_inputs:
                     retval = False
+                    inputs = ', '.join(
+                        map(str, sensor.supported_analogue_inputs)
+                    )
                     print(
                         f'{sensor.description}: analogue input not in '
-                        f'{sensor.supported_analogue_inputs}: {sensor.analogue_input}'
+                        f'{inputs}: {sensor.analogue_input}'
                     )
 
         return retval
 
     def _report_sensor_i2c_addresses_out_of_range(self):
         """Report sensor I2C addresses out of range."""
```

### Comparing `mmcb-avt-0.0.96/src/mmcb/dat2plot.py` & `mmcb-avt-0.0.97/src/mmcb/dat2plot.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.96/src/mmcb/dat2root.py` & `mmcb-avt-0.0.97/src/mmcb/dat2root.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.96/src/mmcb/detect.py` & `mmcb-avt-0.0.97/src/mmcb/detect.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.96/src/mmcb/dmm.py` & `mmcb-avt-0.0.97/src/mmcb/dmm.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.96/src/mmcb/dmm_interface.py` & `mmcb-avt-0.0.97/src/mmcb/dmm_interface.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.96/src/mmcb/iv.py` & `mmcb-avt-0.0.97/src/mmcb/iv.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.96/src/mmcb/lexicon.py` & `mmcb-avt-0.0.97/src/mmcb/lexicon.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.96/src/mmcb/liveplot.py` & `mmcb-avt-0.0.97/src/mmcb/liveplot.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.96/src/mmcb/log2dat.py` & `mmcb-avt-0.0.97/src/mmcb/log2dat.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.96/src/mmcb/peltier.py` & `mmcb-avt-0.0.97/src/mmcb/peltier.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.96/src/mmcb/psuset.py` & `mmcb-avt-0.0.97/src/mmcb/psuset.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.96/src/mmcb/psustat.py` & `mmcb-avt-0.0.97/src/mmcb/psustat.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.96/src/mmcb/sense.py` & `mmcb-avt-0.0.97/src/mmcb/sense.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.96/src/mmcb/sensors.py` & `mmcb-avt-0.0.97/src/mmcb/sensors.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.96/src/mmcb/sensors_mod.py` & `mmcb-avt-0.0.97/src/mmcb/sensors_mod.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.96/src/mmcb/sequence.py` & `mmcb-avt-0.0.97/src/mmcb/sequence.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.96/src/mmcb/ult80.py` & `mmcb-avt-0.0.97/src/mmcb/ult80.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.96/src/mmcb_avt.egg-info/PKG-INFO` & `mmcb-avt-0.0.97/src/mmcb_avt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcb-avt
-Version: 0.0.96
+Version: 0.0.97
 Summary: ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.
 Home-page: https://gitlab.ph.liv.ac.uk/avt/atlas-itk-pmmcb
 Author: Alan Taylor, Manex Ormazabal
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mmcb-avt-0.0.96/src/mmcb_avt.egg-info/SOURCES.txt` & `mmcb-avt-0.0.97/src/mmcb_avt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

