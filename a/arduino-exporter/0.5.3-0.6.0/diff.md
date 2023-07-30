# Comparing `tmp/arduino_exporter-0.5.3.tar.gz` & `tmp/arduino_exporter-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arduino_exporter-0.5.3.tar", last modified: Wed Oct  5 13:11:20 2022, max compression
+gzip compressed data, was "arduino_exporter-0.6.0.tar", last modified: Sun Jul 30 21:37:27 2023, max compression
```

## Comparing `arduino_exporter-0.5.3.tar` & `arduino_exporter-0.6.0.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 13:11:20.582407 arduino_exporter-0.5.3/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 13:11:20.574407 arduino_exporter-0.5.3/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-10-05 13:10:45.000000 arduino_exporter-0.5.3/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-10-05 13:10:45.000000 arduino_exporter-0.5.3/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 13:11:20.574407 arduino_exporter-0.5.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      329 2022-10-05 13:10:45.000000 arduino_exporter-0.5.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-10-05 13:10:45.000000 arduino_exporter-0.5.3/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 13:11:20.578407 arduino_exporter-0.5.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      477 2022-10-05 13:10:45.000000 arduino_exporter-0.5.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      570 2022-10-05 13:10:45.000000 arduino_exporter-0.5.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      564 2022-10-05 13:10:45.000000 arduino_exporter-0.5.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-05 13:10:45.000000 arduino_exporter-0.5.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)      469 2022-10-05 13:10:45.000000 arduino_exporter-0.5.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5219 2022-10-05 13:10:45.000000 arduino_exporter-0.5.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-10-05 13:10:45.000000 arduino_exporter-0.5.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-10-05 13:10:45.000000 arduino_exporter-0.5.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      940 2022-10-05 13:10:45.000000 arduino_exporter-0.5.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     2729 2022-10-05 13:11:20.582407 arduino_exporter-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1894 2022-10-05 13:10:45.000000 arduino_exporter-0.5.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 13:11:20.578407 arduino_exporter-0.5.3/cache/
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-10-05 13:10:45.000000 arduino_exporter-0.5.3/cache/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 13:11:20.578407 arduino_exporter-0.5.3/deploy/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 13:10:45.000000 arduino_exporter-0.5.3/deploy/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-10-05 13:10:45.000000 arduino_exporter-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-10-05 13:10:45.000000 arduino_exporter-0.5.3/renovate.json
--rw-r--r--   0 runner    (1001) docker     (121)     1468 2022-10-05 13:11:20.586407 arduino_exporter-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1553 2022-10-05 13:10:45.000000 arduino_exporter-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 13:11:20.566407 arduino_exporter-0.5.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 13:11:20.578407 arduino_exporter-0.5.3/src/arduino_exporter/
--rw-r--r--   0 runner    (1001) docker     (121)     1681 2022-10-05 13:10:45.000000 arduino_exporter-0.5.3/src/arduino_exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3895 2022-10-05 13:10:45.000000 arduino_exporter-0.5.3/src/arduino_exporter/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 13:11:20.582407 arduino_exporter-0.5.3/src/arduino_exporter/exception/
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-10-05 13:10:45.000000 arduino_exporter-0.5.3/src/arduino_exporter/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7714 2022-10-05 13:10:45.000000 arduino_exporter-0.5.3/src/arduino_exporter/prometheus.py
--rw-r--r--   0 runner    (1001) docker     (121)     1830 2022-10-05 13:10:45.000000 arduino_exporter-0.5.3/src/arduino_exporter/serial.py
--rw-r--r--   0 runner    (1001) docker     (121)     1786 2022-10-05 13:10:45.000000 arduino_exporter-0.5.3/src/arduino_exporter/server.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 13:11:20.582407 arduino_exporter-0.5.3/src/arduino_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2729 2022-10-05 13:11:20.000000 arduino_exporter-0.5.3/src/arduino_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      868 2022-10-05 13:11:20.000000 arduino_exporter-0.5.3/src/arduino_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-05 13:11:20.000000 arduino_exporter-0.5.3/src/arduino_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-05 13:11:19.000000 arduino_exporter-0.5.3/src/arduino_exporter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-10-05 13:11:20.000000 arduino_exporter-0.5.3/src/arduino_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-05 13:11:20.000000 arduino_exporter-0.5.3/src/arduino_exporter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 13:11:20.582407 arduino_exporter-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-10-05 13:10:45.000000 arduino_exporter-0.5.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1185 2022-10-05 13:10:45.000000 arduino_exporter-0.5.3/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)      719 2022-10-05 13:10:45.000000 arduino_exporter-0.5.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:37:27.738630 arduino_exporter-0.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:37:27.734630 arduino_exporter-0.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:37:27.734630 arduino_exporter-0.6.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:37:27.734630 arduino_exporter-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-30 21:37:27.738630 arduino_exporter-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:37:27.734630 arduino_exporter-0.6.0/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/cache/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:37:27.734630 arduino_exporter-0.6.0/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/deploy/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-30 21:37:27.738630 arduino_exporter-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:37:27.730630 arduino_exporter-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:37:27.734630 arduino_exporter-0.6.0/src/arduino_exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/src/arduino_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/src/arduino_exporter/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:37:27.738630 arduino_exporter-0.6.0/src/arduino_exporter/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/src/arduino_exporter/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7711 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/src/arduino_exporter/prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/src/arduino_exporter/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/src/arduino_exporter/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:37:27.738630 arduino_exporter-0.6.0/src/arduino_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-30 21:37:27.000000 arduino_exporter-0.6.0/src/arduino_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-30 21:37:27.000000 arduino_exporter-0.6.0/src/arduino_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 21:37:27.000000 arduino_exporter-0.6.0/src/arduino_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-30 21:37:27.000000 arduino_exporter-0.6.0/src/arduino_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 21:37:27.000000 arduino_exporter-0.6.0/src/arduino_exporter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-30 21:37:27.000000 arduino_exporter-0.6.0/src/arduino_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-30 21:37:27.000000 arduino_exporter-0.6.0/src/arduino_exporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:37:27.738630 arduino_exporter-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-30 21:37:01.000000 arduino_exporter-0.6.0/tox.ini
```

### Comparing `arduino_exporter-0.5.3/.github/workflows/release.yml` & `arduino_exporter-0.6.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `arduino_exporter-0.5.3/.gitignore` & `arduino_exporter-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `arduino_exporter-0.5.3/CODE_OF_CONDUCT.md` & `arduino_exporter-0.6.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `arduino_exporter-0.5.3/CONTRIBUTING.rst` & `arduino_exporter-0.6.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `arduino_exporter-0.5.3/LICENSE.txt` & `arduino_exporter-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arduino_exporter-0.5.3/Makefile` & `arduino_exporter-0.6.0/Makefile`

 * *Files 11% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 .PHONY: version
 version:
 	$(PYTHON) setup.py --version
 
 
 ## release: Release to PyPi
 release:
-	$(PYTHON) -m twine upload --repository-url https://upload.pypi.org/legacy/ dist/*
+	$(PYTHON) -m twine upload --repository-url https://upload.pypi.org/legacy/ dist/*  --verbose
 
 
 ## install: Install the package locally
 .PHONY: install
 install:
 	$(PYTHON) setup.py install
```

### Comparing `arduino_exporter-0.5.3/PKG-INFO` & `arduino_exporter-0.6.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arduino_exporter
-Version: 0.5.3
+Version: 0.6.0
 Summary: Arduino Prometheus Exporter.
 Home-page: https://github.com/clivern/arduino_exporter/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
 Project-URL: Documentation, https://github.com/clivern/arduino_exporter/
 Project-URL: Source, https://github.com/clivern/arduino_exporter/
@@ -28,15 +28,15 @@
 |
 
 ===========================
 Arduino Prometheus Exporter
 ===========================
 
 You can run this exporter on a device (PC or Raspberry PI) connected to an arduino. The exporter will listen to messages sent over the serial port and update the metrics exposed to prometheus.
-I used this project to visualize and trigger alerts for a lot of sensors values like sound, temperature and water level.
+I used this project to visualize and trigger alerts for a lot of sensors values like sound, temperature and water level ... etc
 
 To use the exporter, follow the following steps:
 
 1. Create a python virtual environment.
 
 .. code-block::
 
@@ -51,16 +51,16 @@
     $ pip install arduino-exporter
 
 
 3. To run the arduino exporter process. You can use systemd to run the process on PC or Raspberry PI. The serial port value can be retrieved from arduino IDE.
 
 .. code-block::
 
-    $ python -m arduino_exporter.cli run $serial_port --p $http_port -vv >> /var/log/arduino_exporter.log
-    $ python -m arduino_exporter.cli run /dev/cu.usbmodem14101 --p 8000 -vv >> /var/log/arduino_exporter.log
+    $ arduino_exporter server run -s $serial_port --p $http_port
+    $ arduino_exporter server run -s /dev/cu.usbmodem14101 --p 8000
 
 
 4. Upload a sketch to the arduino to send the metrics to the serial port.
 
 .. code-block::
 
     #define LED 13
```

### Comparing `arduino_exporter-0.5.3/README.rst` & `arduino_exporter-0.6.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 |
 
 ===========================
 Arduino Prometheus Exporter
 ===========================
 
 You can run this exporter on a device (PC or Raspberry PI) connected to an arduino. The exporter will listen to messages sent over the serial port and update the metrics exposed to prometheus.
-I used this project to visualize and trigger alerts for a lot of sensors values like sound, temperature and water level.
+I used this project to visualize and trigger alerts for a lot of sensors values like sound, temperature and water level ... etc
 
 To use the exporter, follow the following steps:
 
 1. Create a python virtual environment.
 
 .. code-block::
 
@@ -31,16 +31,16 @@
     $ pip install arduino-exporter
 
 
 3. To run the arduino exporter process. You can use systemd to run the process on PC or Raspberry PI. The serial port value can be retrieved from arduino IDE.
 
 .. code-block::
 
-    $ python -m arduino_exporter.cli run $serial_port --p $http_port -vv >> /var/log/arduino_exporter.log
-    $ python -m arduino_exporter.cli run /dev/cu.usbmodem14101 --p 8000 -vv >> /var/log/arduino_exporter.log
+    $ arduino_exporter server run -s $serial_port --p $http_port
+    $ arduino_exporter server run -s /dev/cu.usbmodem14101 --p 8000
 
 
 4. Upload a sketch to the arduino to send the metrics to the serial port.
 
 .. code-block::
 
     #define LED 13
@@ -52,8 +52,8 @@
 
     void loop() {
       digitalWrite(LED, HIGH);
       delay(1000);
       digitalWrite(LED, LOW);
       delay(1000);
       Serial.write("{\"type\": \"gauge\", \"name\": \"room_temp\", \"help\": \"the room temperature.\", \"method\": \"set\", \"value\": 14.3, \"labels\": {\"place\": \"us\"}}");
-    }
+    }
```

### Comparing `arduino_exporter-0.5.3/setup.cfg` & `arduino_exporter-0.6.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -23,31 +23,37 @@
 [options]
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 install_requires = 
-	pyserial
-	prometheus-client
-	importlib-metadata; python_version<"3.8"
+	click<=8.1.6
+	pyserial<=3.5
+	prometheus-client<=0.17.1
+	importlib-metadata<=6.8.0; python_version<"3.8"
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 	cache
 	deploy
 testing = 
+	click
 	pyserial
 	prometheus-client
 	setuptools
 	pytest
 	pytest-cov
 
+[options.entry_points]
+console_scripts = 
+	arduino_exporter = arduino_exporter.cli:main
+
 [tool:pytest]
 addopts = 
 	--verbose
 norecursedirs = 
 	dist
 	build
 	.tox
```

### Comparing `arduino_exporter-0.5.3/setup.py` & `arduino_exporter-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `arduino_exporter-0.5.3/src/arduino_exporter/__init__.py` & `arduino_exporter-0.6.0/src/arduino_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `arduino_exporter-0.5.3/src/arduino_exporter/exception/__init__.py` & `arduino_exporter-0.6.0/src/arduino_exporter/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `arduino_exporter-0.5.3/src/arduino_exporter/prometheus.py` & `arduino_exporter-0.6.0/src/arduino_exporter/prometheus.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from prometheus_client import Gauge
 from prometheus_client import Summary
 from prometheus_client import Histogram
 from prometheus_client import Info
 from prometheus_client import Enum
 
 
-class Prometheus():
+class Prometheus:
     """Prometheus Class"""
 
     def __init__(self):
         self.metrics = {}
 
     def store(self, data):
         """
@@ -59,31 +59,31 @@
 
         # Avoid any bad input
         try:
             item = json.loads(data.strip())
         except Exception:
             return
 
-        if 'help' not in item.keys():
-            item['help'] = ''
+        if "help" not in item.keys():
+            item["help"] = ""
 
-        if 'labels' not in item.keys():
-            item['labels'] = {}
+        if "labels" not in item.keys():
+            item["labels"] = {}
 
-        if item['type'] == 'counter' or item['type'] == 'c':
+        if item["type"] == "counter" or item["type"] == "c":
             self.counter(item)
-        elif item['type'] == 'gauge' or item['type'] == 'g':
+        elif item["type"] == "gauge" or item["type"] == "g":
             self.gauge(item)
-        elif item['type'] == 'summary' or item['type'] == 's':
+        elif item["type"] == "summary" or item["type"] == "s":
             self.summary(item)
-        elif item['type'] == 'histogram' or item['type'] == 'h':
+        elif item["type"] == "histogram" or item["type"] == "h":
             self.histogram(item)
-        elif item['type'] == 'info' or item['type'] == 'i':
+        elif item["type"] == "info" or item["type"] == "i":
             self.info(item)
-        elif item['type'] == 'enum' or item['type'] == 'e':
+        elif item["type"] == "enum" or item["type"] == "e":
             self.enum(item)
 
     def counter(self, item):
         """
         Prometheus Counter
 
         Args:
@@ -98,23 +98,23 @@
                         "type": "trousers"
                     }
                 }
         """
         c = None
 
         for name, metric in self.metrics.items():
-            if name == item['name']:
+            if name == item["name"]:
                 c = metric
 
         if c is None:
-            c = Counter(item['name'], item['help'], item['labels'].keys())
-            c = c.labels(*item['labels'].values())
+            c = Counter(item["name"], item["help"], item["labels"].keys())
+            c = c.labels(*item["labels"].values())
 
-        c.inc(item['value'])
-        self.metrics[item['name']] = c
+        c.inc(item["value"])
+        self.metrics[item["name"]] = c
         return c
 
     def gauge(self, item):
         """
         Prometheus Gauge
 
         Args:
@@ -129,29 +129,29 @@
                         "type": "trousers"
                     }
                 }
         """
         g = None
 
         for name, metric in self.metrics.items():
-            if name == item['name']:
+            if name == item["name"]:
                 g = metric
 
         if g is None:
-            g = Gauge(item['name'], item['help'], item['labels'].keys())
-            g = g.labels(*item['labels'].values())
+            g = Gauge(item["name"], item["help"], item["labels"].keys())
+            g = g.labels(*item["labels"].values())
 
-        if item['method'] == 'inc':
-            g.inc(item['value'])
-        elif item['method'] == 'dec':
-            g.dec(item['value'])
-        elif item['method'] == 'set':
-            g.set(item['value'])
+        if item["method"] == "inc":
+            g.inc(item["value"])
+        elif item["method"] == "dec":
+            g.dec(item["value"])
+        elif item["method"] == "set":
+            g.set(item["value"])
 
-        self.metrics[item['name']] = g
+        self.metrics[item["name"]] = g
 
         return g
 
     def summary(self, item):
         """
         Prometheus Summary
 
@@ -167,24 +167,23 @@
                         "type": "trousers"
                     }
                 }
         """
         s = None
 
         for name, metric in self.metrics.items():
-            if name == item['name']:
+            if name == item["name"]:
                 s = metric
 
-
         if s is None:
-            s = Summary(item['name'], item['help'], item['labels'].keys())
-            s = s.labels(*item['labels'].values())
+            s = Summary(item["name"], item["help"], item["labels"].keys())
+            s = s.labels(*item["labels"].values())
 
-        s.observe(item['value'])
-        self.metrics[item['name']] = s
+        s.observe(item["value"])
+        self.metrics[item["name"]] = s
         return s
 
     def histogram(self, item):
         """
         Prometheus Histogram
 
         Args:
@@ -199,23 +198,23 @@
                         "type": "trousers"
                     }
                 }
         """
         h = None
 
         for name, metric in self.metrics.items():
-            if name == item['name']:
+            if name == item["name"]:
                 h = metric
 
         if h is None:
-            h = Histogram(item['name'], item['help'], item['labels'].keys())
-            h = h.labels(*item['labels'].values())
+            h = Histogram(item["name"], item["help"], item["labels"].keys())
+            h = h.labels(*item["labels"].values())
 
-        h.observe(item['value'])
-        self.metrics[item['name']] = h
+        h.observe(item["value"])
+        self.metrics[item["name"]] = h
         return h
 
     def info(self, item):
         """
         Prometheus Info
 
         Args:
@@ -226,22 +225,22 @@
                     "help": "the amount of orders.",
                     "value": {'version': '1.2.3', 'buildhost': 'foo@bar'}
                 }
         """
         i = None
 
         for name, metric in self.metrics.items():
-            if name == item['name']:
+            if name == item["name"]:
                 i = metric
 
         if i is None:
-            i = Info(item['name'], item['help'])
+            i = Info(item["name"], item["help"])
 
-        i.info(item['value'])
-        self.metrics[item['name']] = i
+        i.info(item["value"])
+        self.metrics[item["name"]] = i
         return i
 
     def enum(self, item):
         """
         Prometheus Enum
 
         Args:
@@ -253,16 +252,16 @@
                     "states": ['starting', 'running', 'stopped'],
                     "state": 'starting'
                 }
         """
         e = None
 
         for name, metric in self.metrics.items():
-            if name == item['name']:
+            if name == item["name"]:
                 e = metric
 
         if e is None:
-            e = Enum(item['name'], item['help'], states=item['states'])
+            e = Enum(item["name"], item["help"], states=item["states"])
 
-        e.state(item['state'])
-        self.metrics[item['name']] = e
+        e.state(item["state"])
+        self.metrics[item["name"]] = e
         return e
```

### Comparing `arduino_exporter-0.5.3/src/arduino_exporter/serial.py` & `arduino_exporter-0.6.0/src/arduino_exporter/serial.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import serial
 
 
-class Serial():
+class Serial:
     """Serial Class"""
 
     def __init__(self, serial_port):
         self._serial_port = serial_port
         self._serial = serial.Serial(self._serial_port, 9800, timeout=1)
 
     def read(self):
@@ -46,14 +46,14 @@
     def write(self, message):
         """
         Write into serial port
 
         Args:
             message: The message to send
         """
-        self._serial.write(bytes(message, 'utf-8'))
+        self._serial.write(bytes(message, "utf-8"))
 
     def close(self):
         """
         Close the serial port
         """
         self._serial.close()
```

### Comparing `arduino_exporter-0.5.3/src/arduino_exporter/server.py` & `arduino_exporter-0.6.0/src/arduino_exporter/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from prometheus_client import start_http_server
 
 
-class Server():
+class Server:
     """Server Class"""
 
     def __init__(self, http_port):
         """
         Class Constructor
 
         Args:
```

### Comparing `arduino_exporter-0.5.3/src/arduino_exporter.egg-info/PKG-INFO` & `arduino_exporter-0.6.0/src/arduino_exporter.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arduino-exporter
-Version: 0.5.3
+Version: 0.6.0
 Summary: Arduino Prometheus Exporter.
 Home-page: https://github.com/clivern/arduino_exporter/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
 Project-URL: Documentation, https://github.com/clivern/arduino_exporter/
 Project-URL: Source, https://github.com/clivern/arduino_exporter/
@@ -28,15 +28,15 @@
 |
 
 ===========================
 Arduino Prometheus Exporter
 ===========================
 
 You can run this exporter on a device (PC or Raspberry PI) connected to an arduino. The exporter will listen to messages sent over the serial port and update the metrics exposed to prometheus.
-I used this project to visualize and trigger alerts for a lot of sensors values like sound, temperature and water level.
+I used this project to visualize and trigger alerts for a lot of sensors values like sound, temperature and water level ... etc
 
 To use the exporter, follow the following steps:
 
 1. Create a python virtual environment.
 
 .. code-block::
 
@@ -51,16 +51,16 @@
     $ pip install arduino-exporter
 
 
 3. To run the arduino exporter process. You can use systemd to run the process on PC or Raspberry PI. The serial port value can be retrieved from arduino IDE.
 
 .. code-block::
 
-    $ python -m arduino_exporter.cli run $serial_port --p $http_port -vv >> /var/log/arduino_exporter.log
-    $ python -m arduino_exporter.cli run /dev/cu.usbmodem14101 --p 8000 -vv >> /var/log/arduino_exporter.log
+    $ arduino_exporter server run -s $serial_port --p $http_port
+    $ arduino_exporter server run -s /dev/cu.usbmodem14101 --p 8000
 
 
 4. Upload a sketch to the arduino to send the metrics to the serial port.
 
 .. code-block::
 
     #define LED 13
```

### Comparing `arduino_exporter-0.5.3/src/arduino_exporter.egg-info/SOURCES.txt` & `arduino_exporter-0.6.0/src/arduino_exporter.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -23,13 +23,14 @@
 src/arduino_exporter/cli.py
 src/arduino_exporter/prometheus.py
 src/arduino_exporter/serial.py
 src/arduino_exporter/server.py
 src/arduino_exporter.egg-info/PKG-INFO
 src/arduino_exporter.egg-info/SOURCES.txt
 src/arduino_exporter.egg-info/dependency_links.txt
+src/arduino_exporter.egg-info/entry_points.txt
 src/arduino_exporter.egg-info/not-zip-safe
 src/arduino_exporter.egg-info/requires.txt
 src/arduino_exporter.egg-info/top_level.txt
 src/arduino_exporter/exception/__init__.py
 tests/__init__.py
 tests/test_client.py
```

### Comparing `arduino_exporter-0.5.3/tests/__init__.py` & `arduino_exporter-0.6.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `arduino_exporter-0.5.3/tests/test_client.py` & `arduino_exporter-0.6.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `arduino_exporter-0.5.3/tox.ini` & `arduino_exporter-0.6.0/tox.ini`

 * *Files identical despite different names*

