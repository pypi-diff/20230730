# Comparing `tmp/pymeterreader-0.2.3.tar.gz` & `tmp/pymeterreader-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymeterreader-0.2.3.tar", last modified: Mon Jun 12 08:26:49 2023, max compression
+gzip compressed data, was "pymeterreader-0.3.0.tar", last modified: Sun Jul 30 11:44:01 2023, max compression
```

## Comparing `pymeterreader-0.2.3.tar` & `pymeterreader-0.3.0.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:26:49.194735 pymeterreader-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-12 08:26:49.194735 pymeterreader-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/example_configuration.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:26:49.190734 pymeterreader-0.2.3/pymeterreader/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:26:49.190734 pymeterreader-0.2.3/pymeterreader/core/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/core/channel_description.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/core/channel_upload_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/core/meter_reader_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/core/meter_reader_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:26:49.194735 pymeterreader-0.2.3/pymeterreader/device_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/device_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/device_lib/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/device_lib/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/device_lib/meter_plain.py
--rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/device_lib/meter_sml.py
--rw-r--r--   0 runner    (1001) docker     (123)    28538 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/device_lib/sensor_bme280.py
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/device_lib/serial_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/device_lib/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/device_lib/test_meter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/device_lib/test_meter_plain.py
--rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/device_lib/test_meter_sml.py
--rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/device_lib/test_sensor_bme280.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:26:49.194735 pymeterreader-0.2.3/pymeterreader/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/gateway/basegateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/gateway/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/gateway/volkszaehler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/meter_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:26:49.194735 pymeterreader-0.2.3/pymeterreader/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/metrics/metrics_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/metrics/prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/test_meter_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:26:49.194735 pymeterreader-0.2.3/pymeterreader/wizard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/wizard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/wizard/detector.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/wizard/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/wizard/ncui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:26:49.190734 pymeterreader-0.2.3/pymeterreader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-12 08:26:49.000000 pymeterreader-0.2.3/pymeterreader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-12 08:26:49.000000 pymeterreader-0.2.3/pymeterreader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 08:26:49.000000 pymeterreader-0.2.3/pymeterreader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-12 08:26:49.000000 pymeterreader-0.2.3/pymeterreader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-12 08:26:49.000000 pymeterreader-0.2.3/pymeterreader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-12 08:26:49.000000 pymeterreader-0.2.3/pymeterreader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 08:26:49.194735 pymeterreader-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:44:01.145449 pymeterreader-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-30 11:44:01.145449 pymeterreader-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/example_configuration.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:44:01.141448 pymeterreader-0.3.0/pymeterreader/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/pymeterreader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:44:01.141448 pymeterreader-0.3.0/pymeterreader/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/pymeterreader/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/pymeterreader/core/channel_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/pymeterreader/core/channel_upload_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/pymeterreader/core/meter_reader_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/pymeterreader/core/meter_reader_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:44:01.145449 pymeterreader-0.3.0/pymeterreader/device_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/pymeterreader/device_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/pymeterreader/device_lib/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/pymeterreader/device_lib/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/pymeterreader/device_lib/meter_plain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/pymeterreader/device_lib/meter_sml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28538 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/pymeterreader/device_lib/sensor_bme280.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/pymeterreader/device_lib/serial_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/pymeterreader/device_lib/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/pymeterreader/device_lib/test_meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/pymeterreader/device_lib/test_meter_plain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/pymeterreader/device_lib/test_meter_sml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/pymeterreader/device_lib/test_sensor_bme280.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:44:01.145449 pymeterreader-0.3.0/pymeterreader/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/pymeterreader/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/pymeterreader/gateway/basegateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/pymeterreader/gateway/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/pymeterreader/gateway/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/pymeterreader/gateway/volkszaehler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/pymeterreader/meter_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:44:01.145449 pymeterreader-0.3.0/pymeterreader/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/pymeterreader/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/pymeterreader/metrics/metrics_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/pymeterreader/metrics/prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/pymeterreader/test_meter_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:44:01.145449 pymeterreader-0.3.0/pymeterreader/wizard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/pymeterreader/wizard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/pymeterreader/wizard/detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/pymeterreader/wizard/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/pymeterreader/wizard/ncui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:44:01.141448 pymeterreader-0.3.0/pymeterreader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-30 11:44:01.000000 pymeterreader-0.3.0/pymeterreader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-30 11:44:01.000000 pymeterreader-0.3.0/pymeterreader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 11:44:01.000000 pymeterreader-0.3.0/pymeterreader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-30 11:44:01.000000 pymeterreader-0.3.0/pymeterreader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-30 11:44:01.000000 pymeterreader-0.3.0/pymeterreader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-30 11:44:01.000000 pymeterreader-0.3.0/pymeterreader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 11:44:01.145449 pymeterreader-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-30 11:43:50.000000 pymeterreader-0.3.0/setup.py
```

### Comparing `pymeterreader-0.2.3/LICENSE` & `pymeterreader-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.3/PKG-INFO` & `pymeterreader-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeterreader
-Version: 0.2.3
+Version: 0.3.0
 Summary: pymeterreader is a service to poll smart meters and sensors.It supports uploading to volkszaehler middleware via its REST API.
 Home-page: https://github.com/Schwaneberg/pymeterreader
 Author: Oliver Schwaneberg
 Author-email: Oliver.Schwaneberg@gmail.com
 License: BSD-2-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `pymeterreader-0.2.3/README.md` & `pymeterreader-0.3.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # pymeterreader
 ## Summary
 A flexible and easy to configure service to collect and forward readings from smart meters and other sensors.
 It supports the Volkszaehler middleware and can be used as a replacement of vzlogger.
 Alternatively it supports exposing measurements in the OpenMetrics format for usage with monitoring tools like Prometheus.
+Since version 0.3.0, it also supports MQTT, allowing many applications such as Home Assistant.
 
 ## Supported Devices
 - Meters with SML protocol, tested with EMH electricity meters
 - Meters with plain serial protocols such as Landis+Gyr ULTRAHEAT T550 (UH50…)
 - Bosch BME280 sensor for air humidity, temperature and pressure
 
 ## Installation
@@ -53,7 +54,63 @@
     static_configs:
       - targets: ['localhost:8080']
     relabel_configs:
       - source_labels: [ __name__ ]
         regex: pymeterreader_power_consumption_watts
         action: drop
 ```
+
+## MQTT
+The uuid field will be used to define a topic, when the gateway type is MQTT.
+Channels can be extended by defining "device_class" and "unit_of_measurement".
+Note that the wizard does not yet support MQTT configuration.
+
+Example configuration:
+```
+devices:
+  '12345678':
+    channels:
+      '6.8':
+        interval: 12h
+        uuid: meter/heat/total_absorbed
+        unit_of_measurement: kWh
+    meter_address: hwgrep://0403:6015
+    meter_id: '12345678'
+    protocol: PLAIN
+  1 HLYxx:
+    channels:
+      1-0:1.8.0*255:
+        interval: 5m
+        uuid: meter/electric/total_absorbed
+      1-0:2.8.0*255:
+        interval: 5m
+        uuid: meter/electric/total_yield
+    meter_address: hwgrep://10c4:ea60
+    protocol: SML
+  BME280-078fc53ee157b535d787a94e8ac2f05ed6083c8d21ef77389021ae97961d7d0a:
+    channels:
+      HUMIDITY:
+        interval: 1h
+        uuid: basement/sensor/humidity
+        unit_of_measurement: "%"
+        device_class: humidity
+      PRESSURE:
+        factor: 0.01
+        interval: 1h
+        uuid: basement/sensor/pressure
+        unit_of_measurement: hPa
+        device_class: atmospheric_pressure
+      TEMPERATURE:
+        interval: 1h
+        uuid: basement/sensor/temperature
+        device_class: temperature
+        unit_of_measurement: °C
+    meter_address: 0x76@I2C(1)
+    meter_id: BME280-078fc53ee157b535d787a94e8ac2f05ed6083c8d21ef77389021ae97961d7d0a
+    protocol: BME280
+middleware:
+  type: mqtt
+  middleware_url: localhost
+  user: username
+  password: password
+  port: 1883
+```
```

### Comparing `pymeterreader-0.2.3/example_configuration.yaml` & `pymeterreader-0.3.0/example_configuration.yaml`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.3/pymeterreader/core/channel_upload_info.py` & `pymeterreader-0.3.0/pymeterreader/core/channel_upload_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,13 +8,17 @@
     """
     Channel Upload info structure
     :param uuid: uuid of db entry to feed
     :param interval: interval between readings in seconds
     :param factor: multiply to original values, e.g. to conver kWh to Wh
     :param last_upload: time of last upload to middleware
     :param last_value: last value in middleware
+    :param device_class: device class hint (default: energy)
+    :param unit_of_measurement: Unit of measurement (default: "W")
     """
     uuid: str
     interval: timedelta
     factor: float
     last_upload: datetime
     last_value: tp.Union[int, float]
+    device_class: str
+    unit_of_measurement: str
```

### Comparing `pymeterreader-0.2.3/pymeterreader/core/meter_reader_node.py` & `pymeterreader-0.3.0/pymeterreader/core/meter_reader_node.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.3/pymeterreader/core/meter_reader_task.py` & `pymeterreader-0.3.0/pymeterreader/core/meter_reader_task.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.3/pymeterreader/device_lib/base.py` & `pymeterreader-0.3.0/pymeterreader/device_lib/base.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.3/pymeterreader/device_lib/common.py` & `pymeterreader-0.3.0/pymeterreader/device_lib/common.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.3/pymeterreader/device_lib/meter_plain.py` & `pymeterreader-0.3.0/pymeterreader/device_lib/meter_plain.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.3/pymeterreader/device_lib/meter_sml.py` & `pymeterreader-0.3.0/pymeterreader/device_lib/meter_sml.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.3/pymeterreader/device_lib/sensor_bme280.py` & `pymeterreader-0.3.0/pymeterreader/device_lib/sensor_bme280.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.3/pymeterreader/device_lib/serial_reader.py` & `pymeterreader-0.3.0/pymeterreader/device_lib/serial_reader.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.3/pymeterreader/device_lib/test_base.py` & `pymeterreader-0.3.0/pymeterreader/device_lib/test_base.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.3/pymeterreader/device_lib/test_meter.py` & `pymeterreader-0.3.0/pymeterreader/device_lib/test_meter.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.3/pymeterreader/device_lib/test_meter_plain.py` & `pymeterreader-0.3.0/pymeterreader/device_lib/test_meter_plain.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.3/pymeterreader/device_lib/test_meter_sml.py` & `pymeterreader-0.3.0/pymeterreader/device_lib/test_meter_sml.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.3/pymeterreader/device_lib/test_sensor_bme280.py` & `pymeterreader-0.3.0/pymeterreader/device_lib/test_sensor_bme280.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.3/pymeterreader/gateway/basegateway.py` & `pymeterreader-0.3.0/pymeterreader/gateway/basegateway.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.3/pymeterreader/gateway/debug.py` & `pymeterreader-0.3.0/pymeterreader/gateway/debug.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.3/pymeterreader/gateway/volkszaehler.py` & `pymeterreader-0.3.0/pymeterreader/gateway/volkszaehler.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.3/pymeterreader/meter_reader.py` & `pymeterreader-0.3.0/pymeterreader/meter_reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from datetime import datetime, timezone
 
 from yaml import load, FullLoader
 
 from pymeterreader.core import MeterReaderTask, MeterReaderNode, ChannelUploadInfo
 from pymeterreader.device_lib import strip, SmlReader, PlainReader, Bme280Reader, BaseReader
 from pymeterreader.device_lib.common import humanfriendly_time_parser, ConfigurationError
-from pymeterreader.gateway import BaseGateway, VolkszaehlerGateway, DebugGateway
+from pymeterreader.gateway import BaseGateway, VolkszaehlerGateway, DebugGateway, MQTTGateway
 from pymeterreader.metrics.metrics_collector import MetricsJiTCollector
 
 PARSER = argparse.ArgumentParser(description='MeterReader reads out supported devices '
                                              'and forwards the data to a middleware '
                                              '(e.g. see https://volkszaehler.org/).')
 
 PARSER.add_argument('-d', '--debug', help='Make process chatty.', action='store_true')
@@ -42,14 +42,16 @@
             # Configure Middleware uploads
             middleware_type = config.get('middleware').pop('type')
             middleware_configuration: dict = config.get('middleware')
             if middleware_type == 'volkszaehler':
                 gateway: tp.Optional[BaseGateway] = VolkszaehlerGateway(**middleware_configuration)
             elif middleware_type == 'debug':
                 gateway = DebugGateway(**middleware_configuration)
+            elif middleware_type == "mqtt":
+                gateway = MQTTGateway(**middleware_configuration)
             else:
                 logging.error(f'Middleware "{middleware_type}" not supported!')
                 gateway = None
             if gateway is not None:
                 for meter_name, device in config.get('devices').items():
                     protocol = strip(device.pop('protocol'))
                     configuration_channels = device.pop('channels', {})
@@ -70,17 +72,20 @@
                         if sample is not None:
                             available_channels = {}
                             for sample_channel in sample.channels:
                                 for configuration_channel_name, configuration_channel in configuration_channels.items():
                                     interval = humanfriendly_time_parser(configuration_channel.get('interval', '1h'))
                                     uuid = configuration_channel.get('uuid')
                                     factor = configuration_channel.get('factor', 1.0)
+                                    device_class = configuration_channel.get('device_class', 'energy')
+                                    unit_of_measurement = configuration_channel.get('unit_of_measurement', 'Wh')
                                     if strip(str(configuration_channel_name)) in strip(sample_channel.channel_name):
                                         zero_datetime = datetime.fromtimestamp(0, timezone.utc)
-                                        upload_info = ChannelUploadInfo(uuid, interval, factor, zero_datetime, - 1)
+                                        upload_info = ChannelUploadInfo(uuid, interval, factor, zero_datetime, - 1,
+                                                                        device_class, unit_of_measurement)
                                         # Replacing config string with exact match
                                         available_channels[sample_channel.channel_name] = upload_info
                             # Do not require configuring channels if Prometheus Server is active
                             if len(available_channels) > 0 or metrics_config is not None:
                                 meter_reader_node = MeterReaderNode(available_channels,
                                                                     reader,
                                                                     gateway)
```

### Comparing `pymeterreader-0.2.3/pymeterreader/metrics/metrics_collector.py` & `pymeterreader-0.3.0/pymeterreader/metrics/metrics_collector.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.3/pymeterreader/test_meter_reader.py` & `pymeterreader-0.3.0/pymeterreader/test_meter_reader.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.3/pymeterreader/wizard/generator.py` & `pymeterreader-0.3.0/pymeterreader/wizard/generator.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.3/pymeterreader/wizard/ncui.py` & `pymeterreader-0.3.0/pymeterreader/wizard/ncui.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.3/pymeterreader.egg-info/PKG-INFO` & `pymeterreader-0.3.0/pymeterreader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeterreader
-Version: 0.2.3
+Version: 0.3.0
 Summary: pymeterreader is a service to poll smart meters and sensors.It supports uploading to volkszaehler middleware via its REST API.
 Home-page: https://github.com/Schwaneberg/pymeterreader
 Author: Oliver Schwaneberg
 Author-email: Oliver.Schwaneberg@gmail.com
 License: BSD-2-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `pymeterreader-0.2.3/pymeterreader.egg-info/SOURCES.txt` & `pymeterreader-0.3.0/pymeterreader.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 pymeterreader/device_lib/test_meter.py
 pymeterreader/device_lib/test_meter_plain.py
 pymeterreader/device_lib/test_meter_sml.py
 pymeterreader/device_lib/test_sensor_bme280.py
 pymeterreader/gateway/__init__.py
 pymeterreader/gateway/basegateway.py
 pymeterreader/gateway/debug.py
+pymeterreader/gateway/mqtt.py
 pymeterreader/gateway/volkszaehler.py
 pymeterreader/metrics/__init__.py
 pymeterreader/metrics/metrics_collector.py
 pymeterreader/metrics/prefix.py
 pymeterreader/wizard/__init__.py
 pymeterreader/wizard/detector.py
 pymeterreader/wizard/generator.py
```

### Comparing `pymeterreader-0.2.3/setup.py` & `pymeterreader-0.3.0/setup.py`

 * *Files identical despite different names*

