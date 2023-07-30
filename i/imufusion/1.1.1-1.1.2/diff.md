# Comparing `tmp/imufusion-1.1.1.tar.gz` & `tmp/imufusion-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imufusion-1.1.1.tar", last modified: Fri Jun 30 09:40:33 2023, max compression
+gzip compressed data, was "imufusion-1.1.2.tar", last modified: Sun Jul 30 16:25:01 2023, max compression
```

## Comparing `imufusion-1.1.1.tar` & `imufusion-1.1.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:40:33.552789 imufusion-1.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:40:33.548789 imufusion-1.1.1/Fusion/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-30 09:40:18.000000 imufusion-1.1.1/Fusion/Fusion.h
--rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-06-30 09:40:18.000000 imufusion-1.1.1/Fusion/FusionAhrs.c
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-06-30 09:40:18.000000 imufusion-1.1.1/Fusion/FusionAhrs.h
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-06-30 09:40:18.000000 imufusion-1.1.1/Fusion/FusionAxes.h
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-30 09:40:18.000000 imufusion-1.1.1/Fusion/FusionCalibration.h
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-30 09:40:18.000000 imufusion-1.1.1/Fusion/FusionCompass.c
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-30 09:40:18.000000 imufusion-1.1.1/Fusion/FusionCompass.h
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-30 09:40:18.000000 imufusion-1.1.1/Fusion/FusionConvention.h
--rw-r--r--   0 runner    (1001) docker     (123)    14137 2023-06-30 09:40:18.000000 imufusion-1.1.1/Fusion/FusionMath.h
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-30 09:40:18.000000 imufusion-1.1.1/Fusion/FusionOffset.c
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-30 09:40:18.000000 imufusion-1.1.1/Fusion/FusionOffset.h
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-30 09:40:18.000000 imufusion-1.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-30 09:40:18.000000 imufusion-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-30 09:40:33.552789 imufusion-1.1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:40:33.544789 imufusion-1.1.1/Python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:40:33.552789 imufusion-1.1.1/Python/Python-C-API/
--rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-06-30 09:40:18.000000 imufusion-1.1.1/Python/Python-C-API/Ahrs.h
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-30 09:40:18.000000 imufusion-1.1.1/Python/Python-C-API/Axes.h
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-30 09:40:18.000000 imufusion-1.1.1/Python/Python-C-API/Compass.h
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-30 09:40:18.000000 imufusion-1.1.1/Python/Python-C-API/Flags.h
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-30 09:40:18.000000 imufusion-1.1.1/Python/Python-C-API/Helpers.h
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-30 09:40:18.000000 imufusion-1.1.1/Python/Python-C-API/InternalStates.h
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-30 09:40:18.000000 imufusion-1.1.1/Python/Python-C-API/Offset.h
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-06-30 09:40:18.000000 imufusion-1.1.1/Python/Python-C-API/Quaternion.h
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-06-30 09:40:18.000000 imufusion-1.1.1/Python/Python-C-API/Settings.h
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-06-30 09:40:18.000000 imufusion-1.1.1/Python/Python-C-API/imufusion.c
--rw-r--r--   0 runner    (1001) docker     (123)    13876 2023-06-30 09:40:18.000000 imufusion-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:40:33.552789 imufusion-1.1.1/imufusion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-30 09:40:33.000000 imufusion-1.1.1/imufusion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-30 09:40:33.000000 imufusion-1.1.1/imufusion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 09:40:33.000000 imufusion-1.1.1/imufusion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-30 09:40:33.000000 imufusion-1.1.1/imufusion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 09:40:33.552789 imufusion-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-30 09:40:18.000000 imufusion-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:25:01.026789 imufusion-1.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:25:01.022789 imufusion-1.1.2/Fusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-30 16:24:44.000000 imufusion-1.1.2/Fusion/Fusion.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19090 2023-07-30 16:24:44.000000 imufusion-1.1.2/Fusion/FusionAhrs.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-07-30 16:24:44.000000 imufusion-1.1.2/Fusion/FusionAhrs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-07-30 16:24:44.000000 imufusion-1.1.2/Fusion/FusionAxes.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-30 16:24:44.000000 imufusion-1.1.2/Fusion/FusionCalibration.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-30 16:24:44.000000 imufusion-1.1.2/Fusion/FusionCompass.c
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-30 16:24:44.000000 imufusion-1.1.2/Fusion/FusionCompass.h
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-30 16:24:44.000000 imufusion-1.1.2/Fusion/FusionConvention.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14137 2023-07-30 16:24:44.000000 imufusion-1.1.2/Fusion/FusionMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-07-30 16:24:44.000000 imufusion-1.1.2/Fusion/FusionOffset.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-30 16:24:44.000000 imufusion-1.1.2/Fusion/FusionOffset.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-30 16:24:44.000000 imufusion-1.1.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-30 16:24:44.000000 imufusion-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-30 16:25:01.026789 imufusion-1.1.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:25:01.022789 imufusion-1.1.2/Python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:25:01.026789 imufusion-1.1.2/Python/Python-C-API/
+-rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-07-30 16:24:44.000000 imufusion-1.1.2/Python/Python-C-API/Ahrs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-30 16:24:44.000000 imufusion-1.1.2/Python/Python-C-API/Axes.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-30 16:24:44.000000 imufusion-1.1.2/Python/Python-C-API/Compass.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-30 16:24:44.000000 imufusion-1.1.2/Python/Python-C-API/Flags.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-30 16:24:44.000000 imufusion-1.1.2/Python/Python-C-API/Helpers.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-30 16:24:44.000000 imufusion-1.1.2/Python/Python-C-API/InternalStates.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-30 16:24:44.000000 imufusion-1.1.2/Python/Python-C-API/Offset.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-30 16:24:44.000000 imufusion-1.1.2/Python/Python-C-API/Quaternion.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-30 16:24:44.000000 imufusion-1.1.2/Python/Python-C-API/Settings.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-07-30 16:24:44.000000 imufusion-1.1.2/Python/Python-C-API/imufusion.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13988 2023-07-30 16:24:44.000000 imufusion-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:25:01.026789 imufusion-1.1.2/imufusion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-30 16:25:00.000000 imufusion-1.1.2/imufusion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-30 16:25:00.000000 imufusion-1.1.2/imufusion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 16:25:00.000000 imufusion-1.1.2/imufusion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-30 16:25:00.000000 imufusion-1.1.2/imufusion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 16:25:01.026789 imufusion-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-30 16:24:44.000000 imufusion-1.1.2/setup.py
```

### Comparing `imufusion-1.1.1/Fusion/Fusion.h` & `imufusion-1.1.2/Fusion/Fusion.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.1/Fusion/FusionAhrs.c` & `imufusion-1.1.2/Fusion/FusionAhrs.c`

 * *Files 0% similar despite different names*

```diff
@@ -78,25 +78,21 @@
  * @brief Sets the AHRS algorithm settings.
  * @param ahrs AHRS algorithm structure.
  * @param settings Settings.
  */
 void FusionAhrsSetSettings(FusionAhrs *const ahrs, const FusionAhrsSettings *const settings) {
     ahrs->settings.convention = settings->convention;
     ahrs->settings.gain = settings->gain;
-    if ((settings->accelerationRejection == 0.0f) || (settings->rejectionTimeout == 0)) {
+    ahrs->settings.accelerationRejection = settings->accelerationRejection == 0.0f ? FLT_MAX : powf(0.5f * sinf(FusionDegreesToRadians(settings->accelerationRejection)), 2);
+    ahrs->settings.magneticRejection = settings->magneticRejection == 0.0f ? FLT_MAX : powf(0.5f * sinf(FusionDegreesToRadians(settings->magneticRejection)), 2);
+    ahrs->settings.rejectionTimeout = settings->rejectionTimeout;
+    if ((settings->gain == 0.0f) || (settings->rejectionTimeout == 0)) {
         ahrs->settings.accelerationRejection = FLT_MAX;
-    } else {
-        ahrs->settings.accelerationRejection = powf(0.5f * sinf(FusionDegreesToRadians(settings->accelerationRejection)), 2);
-    }
-    if ((settings->magneticRejection == 0.0f) || (settings->rejectionTimeout == 0)) {
         ahrs->settings.magneticRejection = FLT_MAX;
-    } else {
-        ahrs->settings.magneticRejection = powf(0.5f * sinf(FusionDegreesToRadians(settings->magneticRejection)), 2);
     }
-    ahrs->settings.rejectionTimeout = settings->rejectionTimeout;
     if (ahrs->initialising == false) {
         ahrs->rampedGain = ahrs->settings.gain;
     }
     ahrs->rampedGainStep = (INITIAL_GAIN - ahrs->settings.gain) / INITIALISATION_PERIOD;
 }
 
 /**
@@ -113,15 +109,15 @@
 
     // Store accelerometer
     ahrs->accelerometer = accelerometer;
 
     // Ramp down gain during initialisation
     if (ahrs->initialising == true) {
         ahrs->rampedGain -= ahrs->rampedGainStep * deltaTime;
-        if (ahrs->rampedGain < ahrs->settings.gain) {
+        if ((ahrs->rampedGain < ahrs->settings.gain) || (ahrs->settings.gain == 0.0f)) {
             ahrs->rampedGain = ahrs->settings.gain;
             ahrs->initialising = false;
             ahrs->accelerationRejectionTimeout = false;
         }
     }
 
     // Calculate direction of gravity indicated by algorithm
```

### Comparing `imufusion-1.1.1/Fusion/FusionAhrs.h` & `imufusion-1.1.2/Fusion/FusionAhrs.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.1/Fusion/FusionAxes.h` & `imufusion-1.1.2/Fusion/FusionAxes.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.1/Fusion/FusionCalibration.h` & `imufusion-1.1.2/Fusion/FusionCalibration.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.1/Fusion/FusionCompass.c` & `imufusion-1.1.2/Fusion/FusionCompass.c`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.1/Fusion/FusionCompass.h` & `imufusion-1.1.2/Fusion/FusionCompass.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.1/Fusion/FusionConvention.h` & `imufusion-1.1.2/Fusion/FusionConvention.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.1/Fusion/FusionMath.h` & `imufusion-1.1.2/Fusion/FusionMath.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.1/Fusion/FusionOffset.c` & `imufusion-1.1.2/Fusion/FusionOffset.c`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.1/Fusion/FusionOffset.h` & `imufusion-1.1.2/Fusion/FusionOffset.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.1/LICENSE.md` & `imufusion-1.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.1/PKG-INFO` & `imufusion-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imufusion
-Version: 1.1.1
+Version: 1.1.2
 Summary: Fusion Python package
 Home-page: https://github.com/xioTechnologies/Fusion
 Author: x-io Technologies Limited
 Author-email: info@x-io.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `imufusion-1.1.1/Python/Python-C-API/Ahrs.h` & `imufusion-1.1.2/Python/Python-C-API/Ahrs.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.1/Python/Python-C-API/Axes.h` & `imufusion-1.1.2/Python/Python-C-API/Axes.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.1/Python/Python-C-API/Compass.h` & `imufusion-1.1.2/Python/Python-C-API/Compass.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.1/Python/Python-C-API/Flags.h` & `imufusion-1.1.2/Python/Python-C-API/Flags.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.1/Python/Python-C-API/Helpers.h` & `imufusion-1.1.2/Python/Python-C-API/Helpers.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.1/Python/Python-C-API/InternalStates.h` & `imufusion-1.1.2/Python/Python-C-API/InternalStates.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.1/Python/Python-C-API/Offset.h` & `imufusion-1.1.2/Python/Python-C-API/Offset.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.1/Python/Python-C-API/Quaternion.h` & `imufusion-1.1.2/Python/Python-C-API/Quaternion.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.1/Python/Python-C-API/Settings.h` & `imufusion-1.1.2/Python/Python-C-API/Settings.h`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.1/Python/Python-C-API/imufusion.c` & `imufusion-1.1.2/Python/Python-C-API/imufusion.c`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.1/README.md` & `imufusion-1.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -34,21 +34,21 @@
 
 The algorithm provides three outputs: quaternion, linear acceleration, and Earth acceleration.  The quaternion describes the orientation of the sensor relative to the Earth.  This can be converted to a rotation matrix using the `FusionQuaternionToMatrix` function or to Euler angles using the `FusionQuaternionToEuler` function.  The linear acceleration is the accelerometer measurement with the 1 g of gravity removed.  The Earth acceleration is the accelerometer measurement in the Earth coordinate frame with the 1 g of gravity removed.  The algorithm supports North-West-Up (NWU), East-North-Up (ENU), and North-East-Down (NED) axes conventions.
 
 ### Algorithm settings
 
 The AHRS algorithm settings are defined by the `FusionAhrsSettings` structure and set using the `FusionAhrsSetSettings` function.
 
-| Setting                 | Description                                                                                                                                                                                                   |
-|-------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `convention`            | Earth axes convention (NWD, ENU, or NED).                                                                                                                                                                     |
-| `gain`                  | Determines the influence of the gyroscope relative to other sensors.  A value of 0.5 is appropriate for most applications.                                                                                    |
-| `accelerationRejection` | Threshold (in degrees) used by the acceleration rejection feature.  A value of zero will disable this feature.  A value of 10 degrees is appropriate for most applications.                                   |
-| `magneticRejection`     | Threshold (in degrees) used by the magnetic rejection feature.  A value of zero will disable the feature. A value of 20 degrees is appropriate for most applications.                                         |
-| `rejectionTimeout`      | Acceleration and magnetic rejection timeout period (in samples).  A value of zero will disable the acceleration and magnetic rejection features.  A period of 5 seconds is appropriate for most applications. |
+| Setting                 | Description                                                                                                                                                                                                                   |
+|-------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `convention`            | Earth axes convention (NWD, ENU, or NED).                                                                                                                                                                                     |
+| `gain`                  | Determines the influence of the gyroscope relative to other sensors.  A value of zero will disable initialisation and the acceleration and magnetic rejection features.  A value of 0.5 is appropriate for most applications. |
+| `accelerationRejection` | Threshold (in degrees) used by the acceleration rejection feature.  A value of zero will disable this feature.  A value of 10 degrees is appropriate for most applications.                                                   |
+| `magneticRejection`     | Threshold (in degrees) used by the magnetic rejection feature.  A value of zero will disable the feature. A value of 20 degrees is appropriate for most applications.                                                         |
+| `rejectionTimeout`      | Acceleration and magnetic rejection timeout period (in samples).  A value of zero will disable the acceleration and magnetic rejection features.  A period of 5 seconds is appropriate for most applications.                 |
 
 ### Algorithm internal states
 
 The AHRS algorithm internal states are defined by the `FusionAhrsInternalStates` structure and obtained using the `FusionAhrsGetInternalStates` function.
 
 | State                        | Description                                                                                                                                                                                                                                                            |
 |------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
```

### Comparing `imufusion-1.1.1/imufusion.egg-info/PKG-INFO` & `imufusion-1.1.2/imufusion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imufusion
-Version: 1.1.1
+Version: 1.1.2
 Summary: Fusion Python package
 Home-page: https://github.com/xioTechnologies/Fusion
 Author: x-io Technologies Limited
 Author-email: info@x-io.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `imufusion-1.1.1/imufusion.egg-info/SOURCES.txt` & `imufusion-1.1.2/imufusion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imufusion-1.1.1/setup.py` & `imufusion-1.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
                                       "Fusion/FusionCompass.c",
                                       "Fusion/FusionOffset.c"],
                         include_dirs=[numpy.get_include()],
                         define_macros=[("FUSION_USE_NORMAL_SQRT", None)],
                         libraries=(["m"] if "linux" in sys.platform else []))  # link math library for Linux
 
 setup(name="imufusion",
-      version="1.1.1",
+      version="1.1.2",
       description="Fusion Python package",
       long_description="See [github](" + github_url + ") for documentation and examples.",
       long_description_content_type='text/markdown',
       url=github_url,
       author="x-io Technologies Limited",
       author_email="info@x-io.co.uk",
       license="MIT",
```

