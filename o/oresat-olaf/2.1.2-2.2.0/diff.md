# Comparing `tmp/oresat-olaf-2.1.2.tar.gz` & `tmp/oresat-olaf-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oresat-olaf-2.1.2.tar", last modified: Thu May 18 23:30:42 2023, max compression
+gzip compressed data, was "oresat-olaf-2.2.0.tar", last modified: Sun Jul 30 18:49:23 2023, max compression
```

## Comparing `oresat-olaf-2.1.2.tar` & `oresat-olaf-2.2.0.tar`

### file list

```diff
@@ -1,89 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:30:42.056764 oresat-olaf-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-18 23:30:42.056764 oresat-olaf-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:30:42.040764 oresat-olaf-2.1.2/olaf/
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:30:42.040764 oresat-olaf-2.1.2/olaf/_internals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/_internals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/_internals/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:30:42.040764 oresat-olaf-2.1.2/olaf/_internals/data/
--rw-r--r--   0 runner    (1001) docker     (123)    82085 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/_internals/data/oresat_app.eds
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/_internals/master_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    17209 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/_internals/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:30:42.044764 oresat-olaf-2.1.2/olaf/_internals/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/_internals/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/_internals/resources/ecss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/_internals/resources/file_caches.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/_internals/resources/fread.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/_internals/resources/fwrite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/_internals/resources/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/_internals/resources/os_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/_internals/resources/power_control.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/_internals/resources/store_eds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/_internals/resources/system_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/_internals/resources/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:30:42.044764 oresat-olaf-2.1.2/olaf/_internals/rest_api/
--rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/_internals/rest_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:30:42.048764 oresat-olaf-2.1.2/olaf/_internals/rest_api/static/
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/_internals/rest_api/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:30:42.052764 oresat-olaf-2.1.2/olaf/_internals/rest_api/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/_internals/rest_api/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/_internals/rest_api/templates/fread.html
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/_internals/rest_api/templates/fwrite.html
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/_internals/rest_api/templates/logs.html
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/_internals/rest_api/templates/od.html
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/_internals/rest_api/templates/os_command.html
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/_internals/rest_api/templates/power_control.html
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/_internals/rest_api/templates/root.html
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/_internals/rest_api/templates/system_info.html
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/_internals/rest_api/templates/updater.html
--rw-r--r--   0 runner    (1001) docker     (123)    15341 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/_internals/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:30:42.052764 oresat-olaf-2.1.2/olaf/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/common/cpufreq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/common/ecss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/common/gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/common/oresat_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/common/oresat_file_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/common/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/common/timer_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:30:42.052764 oresat-olaf-2.1.2/olaf/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2478 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/scripts/file_transfer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1832 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/scripts/new_eds.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1208 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/scripts/os_command.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5444 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/scripts/sdo_transfer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      456 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/scripts/sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3537 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/olaf/scripts/system_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:30:42.056764 oresat-olaf-2.1.2/oresat_olaf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-18 23:30:42.000000 oresat-olaf-2.1.2/oresat_olaf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-18 23:30:42.000000 oresat-olaf-2.1.2/oresat_olaf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 23:30:42.000000 oresat-olaf-2.1.2/oresat_olaf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-18 23:30:42.000000 oresat-olaf-2.1.2/oresat_olaf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-18 23:30:42.000000 oresat-olaf-2.1.2/oresat_olaf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-18 23:30:42.000000 oresat-olaf-2.1.2/oresat_olaf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-18 23:30:42.060764 oresat-olaf-2.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:30:42.056764 oresat-olaf-2.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:30:42.056764 oresat-olaf-2.1.2/tests/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/tests/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/tests/common/test_ecss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/tests/common/test_oresat_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/tests/common/test_oresat_file_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/tests/common/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:30:42.056764 oresat-olaf-2.1.2/tests/internals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/tests/internals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:30:42.056764 oresat-olaf-2.1.2/tests/internals/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/tests/internals/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/tests/internals/resources/test_ecss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/tests/internals/resources/test_file_caches.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/tests/internals/resources/test_fread.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/tests/internals/resources/test_fwrite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/tests/internals/resources/test_os_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/tests/internals/resources/test_system_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/tests/internals/test_rest_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 23:30:42.056764 oresat-olaf-2.1.2/tests/internals/updater/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/tests/internals/updater/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-05-18 23:30:30.000000 oresat-olaf-2.1.2/tests/internals/updater/test_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:49:23.680693 oresat-olaf-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-30 18:49:23.680693 oresat-olaf-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:49:23.672693 oresat-olaf-2.2.0/olaf/
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:49:23.672693 oresat-olaf-2.2.0/olaf/_internals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/_internals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/_internals/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:49:23.672693 oresat-olaf-2.2.0/olaf/_internals/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    83322 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/_internals/data/oresat_app.eds
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/_internals/master_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17502 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/_internals/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:49:23.672693 oresat-olaf-2.2.0/olaf/_internals/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/_internals/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/_internals/resources/daemons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/_internals/resources/ecss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/_internals/resources/file_caches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/_internals/resources/fread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/_internals/resources/fwrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/_internals/resources/power_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/_internals/resources/store_eds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/_internals/resources/system_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:49:23.672693 oresat-olaf-2.2.0/olaf/_internals/rest_api/
+-rw-r--r--   0 runner    (1001) docker     (123)    10013 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/_internals/rest_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:49:23.672693 oresat-olaf-2.2.0/olaf/_internals/rest_api/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/_internals/rest_api/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:49:23.676693 oresat-olaf-2.2.0/olaf/_internals/rest_api/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/_internals/rest_api/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/_internals/rest_api/templates/daemons.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/_internals/rest_api/templates/fread.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/_internals/rest_api/templates/fwrite.html
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/_internals/rest_api/templates/logs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/_internals/rest_api/templates/od.html
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/_internals/rest_api/templates/oresat_configs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/_internals/rest_api/templates/os_command.html
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/_internals/rest_api/templates/power_control.html
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/_internals/rest_api/templates/root.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/_internals/rest_api/templates/system_info.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/_internals/rest_api/templates/updater.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:49:23.676693 oresat-olaf-2.2.0/olaf/_internals/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/_internals/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/_internals/services/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/_internals/services/os_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/_internals/services/updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15336 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/_internals/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:49:23.676693 oresat-olaf-2.2.0/olaf/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/common/adc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/common/cpufreq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/common/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/common/ecss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/common/gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/common/oresat_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/common/oresat_file_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/common/pru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/common/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/common/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/common/timer_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:49:23.680693 oresat-olaf-2.2.0/olaf/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2478 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/scripts/file_transfer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1832 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/scripts/new_eds.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1208 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/scripts/os_command.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5444 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/scripts/sdo_transfer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      456 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/scripts/sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3537 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/olaf/scripts/system_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:49:23.680693 oresat-olaf-2.2.0/oresat_olaf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-30 18:49:23.000000 oresat-olaf-2.2.0/oresat_olaf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-30 18:49:23.000000 oresat-olaf-2.2.0/oresat_olaf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 18:49:23.000000 oresat-olaf-2.2.0/oresat_olaf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-30 18:49:23.000000 oresat-olaf-2.2.0/oresat_olaf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-30 18:49:23.000000 oresat-olaf-2.2.0/oresat_olaf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-30 18:49:23.000000 oresat-olaf-2.2.0/oresat_olaf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 18:49:23.680693 oresat-olaf-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:49:23.680693 oresat-olaf-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:49:23.680693 oresat-olaf-2.2.0/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/tests/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/tests/common/test_ecss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/tests/common/test_oresat_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/tests/common/test_oresat_file_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/tests/common/test_pru.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/tests/common/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:49:23.680693 oresat-olaf-2.2.0/tests/internals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/tests/internals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:49:23.680693 oresat-olaf-2.2.0/tests/internals/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/tests/internals/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/tests/internals/resources/test_ecss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/tests/internals/resources/test_file_caches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/tests/internals/resources/test_fread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/tests/internals/resources/test_fwrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/tests/internals/resources/test_system_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:49:23.680693 oresat-olaf-2.2.0/tests/internals/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/tests/internals/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/tests/internals/services/test_os_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/tests/internals/test_rest_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:49:23.680693 oresat-olaf-2.2.0/tests/internals/updater/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/tests/internals/updater/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-30 18:49:13.000000 oresat-olaf-2.2.0/tests/internals/updater/test_updater.py
```

### Comparing `oresat-olaf-2.1.2/LICENSE` & `oresat-olaf-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.2/PKG-INFO` & `oresat-olaf-2.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 Metadata-Version: 2.1
 Name: oresat-olaf
-Version: 2.1.2
+Version: 2.2.0
 Summary: Application framework for all OreSat Linux boards
-Home-page: https://github.com/oresat/oresat-olaf
-Author: PSAS
-Author-email: oresat@pdx.edu
-Maintainer: PSAS
-Maintainer-email: oresat@pdx.edu
 License: GPL-3.0
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 OLAF (OreSat Linux App Framework)
```

### Comparing `oresat-olaf-2.1.2/README.rst` & `oresat-olaf-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.2/olaf/_internals/app.py` & `oresat-olaf-2.2.0/olaf/_internals/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 import subprocess
 from os.path import abspath, dirname
 
 import canopen
 from loguru import logger
 
 from ..common.resource import Resource
+from ..common.service import Service
 from .node import Node, NodeStop
 from .master_node import MasterNode
 from .updater import Updater
-from .resources.os_command import OSCommandResource
 from .resources.system_info import SystemInfoResource
 from .resources.file_caches import FileCachesResource
 from .resources.fread import FreadResource
 from .resources.fwrite import FwriteResource
 from .resources.ecss import ECSSResource
-from .resources.updater import UpdaterResource
-from .resources.logs import LogsResource
 from .resources.store_eds import StoreEdsResource
 from .resources.power_control import PowerControlResource
+from .resources.daemons import DaemonsResource
+from .services.os_command import OSCommandService
+from .services.updater import UpdaterService
+from .services.logs import LogsService
 
 
 class App:
     '''
     The application class that manages the CAN bus and resources.
 
     Use the global ``olaf.app`` obect.
@@ -33,14 +35,15 @@
     '''Internal eds file incase app's is misformatted or missing.'''
 
     def __init__(self):
 
         self._od = None
         self._bus = None
         self._resources = []
+        self._services = []
         self._node = None
         self._updater = None
         self._factory_reset_cb = None
 
         # setup event
         for sig in ['SIGTERM', 'SIGHUP', 'SIGINT']:
             signal.signal(getattr(signal, sig), self._quit)
@@ -67,15 +70,15 @@
         else:
             self._node_id = 0x7C
 
         # make sure these are set
         self._od.node_id = self._node_id
         self._od.bitrate = 1_000_000  # oresat node will always have 1 Mbps
 
-    def setup(self, eds: str, bus: str, node_id: [int, str] = 0, master_node: bool = False):
+    def setup(self, eds: str, bus: str, node_id: int or str = 0, master_node: bool = False):
         '''
         Setup the app. Will be called by ``olaf_setup`` automatically.
 
         Parameters
         ----------
         eds: str
             File path to EDS or DCF file.
@@ -121,51 +124,72 @@
         else:
             self._node = Node(self._od, bus)
 
         # setup updater
         self._updater = Updater(f'{self._node.work_base_dir}/updater',
                                 f'{self._node.cache_base_dir}/updates')
 
-        # default resources
-        self.add_resource(OSCommandResource())
+        # default core services
+        self.add_service(UpdaterService(self._updater))
+        self.add_service(LogsService())
+        self.add_service(OSCommandService())
+
+        # default core resources
         self.add_resource(ECSSResource())
         self.add_resource(SystemInfoResource())
         self.add_resource(FileCachesResource())
         self.add_resource(FreadResource())
         self.add_resource(FwriteResource())
-        self.add_resource(UpdaterResource(self._updater))
-        self.add_resource(LogsResource())
         self.add_resource(StoreEdsResource(eds))
         self.add_resource(PowerControlResource())
+        self.add_resource(DaemonsResource())
 
     def add_resource(self, resource: Resource):
         '''
         Add a resource for the app
 
         Parameters
         ----------
         resource: Resource
             The resource to add.
         '''
 
         self._resources.append(resource)
 
+    def add_service(self, service: Service):
+        '''
+        Add a resource for the app
+
+        Parameters
+        ----------
+        service: Service
+            The service to add.
+        '''
+
+        self._services.append(service)
+
     def run(self):
         logger.info(f'{self._node.name} app is starting')
 
+        for service in self._services:
+            service.start(self._node)
+
         for resource in self._resources:
             resource.start(self._node)
 
         if self._node:
             try:
                 reset = self._node.run()
             except Exception as e:
                 logger.exception(f'unexpected error was raised by app node: {e}')
                 reset = NodeStop.SOFT_RESET
 
+        for service in self._services:
+            service.stop()
+
         for resource in self._resources:
             resource.end()
 
         logger.info(f'{self._node.name} app has ended')
 
         if reset == NodeStop.HARD_RESET:
             logger.info('hard reseting the system')
@@ -212,10 +236,14 @@
         return self._node
 
     def set_factory_reset_callback(self, cb_func):
         '''Set a custom factory reset callback function.'''
 
         self._factory_reset_cb = cb_func
 
+    @property
+    def od(self) -> canopen.ObjectDictionary:
+        return self._od
+
 
 app = App()
 '''The global instance of the OLAF app.'''
```

### Comparing `oresat-olaf-2.1.2/olaf/_internals/data/oresat_app.eds` & `oresat-olaf-2.2.0/olaf/_internals/data/oresat_app.eds`

 * *Files 1% similar despite different names*

```diff
@@ -4173,27 +4173,28 @@
 ParameterName=NMTStartup
 ObjectType=0x07
 DataType=0x0007
 AccessType=rw
 DefaultValue=0x00000008
 
 [ManufacturerObjects]
-SupportedObjects=12
+SupportedObjects=13
 1=0x2000
 2=0x2010
 3=0x2011
 4=0x2100
 5=0x3000
 6=0x3001
 7=0x3002
 8=0x3003
 9=0x3004
 10=0x3005
 11=0x3006
-12=0x3100
+12=0x3007
+13=0x3100
 
 ;CAN Bus redundancy management as defined in ECSS-E-ST-50-15C
 [2000]
 ParameterName=BUS management
 ObjectType=0x09
 SubNumber=5
 
@@ -4691,39 +4692,39 @@
 DataType=0x0001
 AccessType=wo
 DefaultValue=0
 
 [3003]
 ParameterName=Fread
 ObjectType=0x09
-SubNumber=5
+SubNumber=7
 
 [3003sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x04
+DefaultValue=0x06
 
-;Name of the file to read. Uses Index 3002 to find file names.
+;Name of the file to be read. Must be set before index 2.
 [3003sub1]
 ParameterName=File name
 ObjectType=0x07
 DataType=0x0009
 AccessType=rw
 
 ;Data of the file selected in subindex 1
 [3003sub2]
 ParameterName=File data
 ObjectType=0x07
 DataType=0x000F
 AccessType=ro
 DefaultValue=0
 
-;Gets the CRC32 of the file
+;Gets the CRC32 of the file selected in subindex 1
 [3003sub3]
 ParameterName=CRC32
 ObjectType=0x07
 DataType=0x0007
 AccessType=ro
 DefaultValue=0
 
@@ -4731,25 +4732,40 @@
 [3003sub4]
 ParameterName=Delete file
 ObjectType=0x07
 DataType=0x0001
 AccessType=wo
 DefaultValue=0
 
+;Number of files in the cache
+[3003sub5]
+ParameterName=Total files
+ObjectType=0x07
+DataType=0x0006
+AccessType=ro
+DefaultValue=0
+
+;File names in cache as a JSON list
+[3003sub6]
+ParameterName=File names
+ObjectType=0x07
+DataType=0x0009
+AccessType=ro
+
 [3004]
 ParameterName=Fwrite
 ObjectType=0x09
-SubNumber=3
+SubNumber=7
 
 [3004sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
-DefaultValue=0x02
+DefaultValue=0x06
 
 ;Name of the file to be written. Must be set before index 2.
 [3004sub1]
 ParameterName=File name
 ObjectType=0x07
 DataType=0x0009
 AccessType=rw
@@ -4758,72 +4774,101 @@
 [3004sub2]
 ParameterName=File data
 ObjectType=0x07
 DataType=0x000F
 AccessType=wo
 DefaultValue=0
 
+;Gets the CRC32 of the file selected in subindex 1
+[3004sub3]
+ParameterName=CRC32
+ObjectType=0x07
+DataType=0x0007
+AccessType=ro
+DefaultValue=0
+
+[3004sub4]
+ParameterName=Delete file
+ObjectType=0x07
+DataType=0x0001
+AccessType=wo
+DefaultValue=0
+
+[3004sub5]
+ParameterName=Total files
+ObjectType=0x07
+DataType=0x0006
+AccessType=ro
+DefaultValue=0
+
+;File names in cache as a JSON list
+[3004sub6]
+ParameterName=File names
+ObjectType=0x07
+DataType=0x0009
+AccessType=ro
+
 [3005]
-ParameterName=App manager
+ParameterName=Daemon manager
 ObjectType=0x09
 SubNumber=7
 
 [3005sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
 AccessType=const
 DefaultValue=0x06
 
 [3005sub1]
-ParameterName=Total apps
+ParameterName=Total daemons
 ObjectType=0x07
 DataType=0x0005
 AccessType=ro
 DefaultValue=0
 PDOMapping=1
 
 [3005sub2]
-ParameterName=Active apps
+ParameterName=Active daemons
 ObjectType=0x07
 DataType=0x0005
 AccessType=ro
 DefaultValue=0
 PDOMapping=1
 
 [3005sub3]
-ParameterName=Failed apps
+ParameterName=Failed daemons
 ObjectType=0x07
 DataType=0x0005
 AccessType=ro
 DefaultValue=0
 PDOMapping=1
 
 [3005sub4]
-ParameterName=Select app
+ParameterName=Select daemon
 ObjectType=0x07
 DataType=0x0005
 AccessType=rw
 DefaultValue=0
 
 [3005sub5]
-ParameterName=App name
+ParameterName=Daemon name
 ObjectType=0x07
 DataType=0x0009
 AccessType=ro
 
 [3005sub6]
 ParameterName=Daemon state
 ObjectType=0x07
 DataType=0x0005
-AccessType=rw
+AccessType=ro
 DefaultValue=0
 
 [3006]
-ParameterName=New Record
+ParameterName=Logs
 ObjectType=0x09
 SubNumber=3
 
 [3006sub0]
 ParameterName=Highest sub-index supported
 ObjectType=0x07
 DataType=0x0005
@@ -4841,14 +4886,46 @@
 ;Get the logs since boot as a string.
 [3006sub2]
 ParameterName=Get logs
 ObjectType=0x07
 DataType=0x0009
 AccessType=ro
 
+[3007]
+ParameterName=OreSat config
+ObjectType=0x09
+SubNumber=3
+
+[3007sub0]
+ParameterName=Highest sub-index supported
+ObjectType=0x07
+DataType=0x0005
+AccessType=const
+DefaultValue=0x02
+
+;OreSat the card is for:
+;
+;- 0: ORESAT0
+;- 1: ORESAT0.5
+;- 2: ORESAT
+[3007sub1]
+ParameterName=OreSat
+ObjectType=0x07
+DataType=0x0005
+AccessType=rw
+DefaultValue=1
+
+;Toggle flight mode flight. Default on.
+[3007sub2]
+ParameterName=Flight mode
+ObjectType=0x07
+DataType=0x0001
+AccessType=rw
+DefaultValue=1
+
 [3100]
 ParameterName=Updater
 ObjectType=0x09
 SubNumber=6
 
 [3100sub0]
 ParameterName=Highest sub-index supported
```

### Comparing `oresat-olaf-2.1.2/olaf/_internals/master_node.py` & `oresat-olaf-2.2.0/olaf/_internals/master_node.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.2/olaf/_internals/node.py` & `oresat-olaf-2.2.0/olaf/_internals/node.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pathlib import Path
 from threading import Event
 
 import canopen
 import psutil
 from loguru import logger
 
+from ..common.daemon import Daemon
 from ..common.timer_loop import TimerLoop
 from ..common.oresat_file_cache import OreSatFileCache
 
 
 class NodeStop(IntEnum):
 
     SOFT_RESET = 1
@@ -48,14 +49,15 @@
         self._network = None
         self._event = Event()
         self._read_cbs = {}
         self._write_cbs = {}
         self._syncs = 0
         self._reset = NodeStop.SOFT_RESET
         self._tpdo_timers = []
+        self._daemons = {}
 
         if geteuid() == 0:  # running as root
             self.work_base_dir = '/var/lib/oresat'
             self.cache_base_dir = '/var/cache/oresat'
         else:
             self.work_base_dir = str(Path.home()) + '/.oresat'
             self.cache_base_dir = str(Path.home()) + '/.cache/oresat'
@@ -300,15 +302,14 @@
             self._node = None
 
     def _monitor_can(self):
         '''Monitor the CAN bus and CAN network'''
 
         first_bus_down = True  # flag to only log error message on first error
         self.first_bus_reset = True  # flag to only log error message on first error
-        logger.info(f'{self.name} app is running')
         while not self._event.is_set():
             bus = psutil.net_if_stats().get(self._bus)
             if not bus:  # bus does not exist
                 self._disable_network()
                 if first_bus_down:
                     logger.critical(f'{self._bus} does not exists, nothing OLAF can do')
                     first_bus_down = False
@@ -332,36 +333,41 @@
 
         Returns
         -------
         NodeStop
             Reset / power off condition.
         '''
 
-        logger.info(f'{self.name} app is starting')
+        logger.info(f'{self.name} node is starting')
         if geteuid() != 0:  # running as root
             logger.warning('not running as root, cannot restart CAN bus if it goes down')
 
         try:
             self._monitor_can()
         except Exception as e:
             logger.exception(e)
 
         # stop the node and TPDO timers
         self._destroy_node()
 
-        logger.info(f'{self.name} app has ended')
+        logger.info(f'{self.name} node has ended')
         return self._reset
 
     def stop(self, reset: NodeStop = None):
         '''End the run loop'''
 
         if reset is not None:
             self._reset = reset
         self._event.set()
 
+    def add_daemon(self, name: str):
+        '''Add a daemon for the node to monitor and/or control'''
+
+        self._daemons[name] = Daemon(name)
+
     def add_sdo_read_callback(self, index: int, sdo_cb):
         '''
         Add an SDO read callback
 
         Parameters
         ----------
         index: int
@@ -453,15 +459,16 @@
         if ret is None:
             ret = od.value
 
         return ret
 
     def _on_sdo_write(self, index: int, subindex: int, od: canopen.objectdictionary.Variable,
                       data: bytes):
-        '''SDO write callback function. Gives access to the data being received on a SDO write.
+        '''
+        SDO write callback function. Gives access to the data being received on a SDO write.
 
         *Note:* data is still written to object dictionary before call.
 
         Parameters
         ----------
         index: int
             The index the SDO being written to.
@@ -485,16 +492,15 @@
                     logger.exception(f'sdo write cb for 0x{index:04X} 0x{subindex:02X} raised: '
                                      f'{e}')
 
     @property
     def name(self) -> str:
         '''str: The nodes name.'''
 
-        if self._node:
-            return self._node.object_dictionary.device_information.product_name
+        return self._od.device_information.product_name
 
     @property
     def od(self) -> canopen.ObjectDictionary:
         '''canopen.ObjectDictionary: Access to the object dictionary.'''
 
         return self._od
 
@@ -508,10 +514,16 @@
     def fwrite_cache(self) -> OreSatFileCache:
         '''OreSatFile: Cache the CANopen master node can write to.'''
 
         return self._fwrite_cache
 
     @property
     def is_running(self) -> bool:
-        '''bool: is the node loop running'''
+        '''bool: Is the node loop running'''
 
         return not self._event.is_set()
+
+    @property
+    def daemons(self) -> dict:
+        '''dict: The dictionary of external daemons that are monitored and/or controllable'''
+
+        return self._daemons
```

### Comparing `oresat-olaf-2.1.2/olaf/_internals/resources/ecss.py` & `oresat-olaf-2.2.0/olaf/_internals/resources/ecss.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.2/olaf/_internals/resources/file_caches.py` & `oresat-olaf-2.2.0/olaf/_internals/resources/file_caches.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,36 +38,40 @@
     def on_read(self, index: int, subindex: int):
 
         ret = None
 
         if index != self.index:
             return ret
 
-        try:
-            if subindex == Subindex.FREAD_LEN:
-                ret = len(self.node.fread_cache)
-            elif subindex == Subindex.FWRITE_LEN:
-                ret = len(self.node.fwrite_cache)
-            elif subindex == Subindex.CACHE_SELECTOR:
-                ret = self.selector
-            elif subindex == Subindex.FILTER:
-                ret = self.filter
-            elif subindex == Subindex.CACHE_LENGTH:
-                ret = len(self.file_caches[self.selector].files(self.filter))
-            elif subindex == Subindex.ITER:
-                ret = self.iter
-            elif subindex == Subindex.FILE_NAME:
-                ret = self.file_caches[self.selector].files(self.filter)[self.iter].name
-            elif subindex == Subindex.FILE_SIZE:
-                dir_name = self.file_caches[self.selector].dir
-                file_name = self.file_caches[self.selector].files(self.filter)[self.iter].name
-                file_path = f'{dir_name}/{file_name}'
+        if subindex == Subindex.FREAD_LEN:
+            cache_len = len(self.node.fread_cache)
+            ret = cache_len if cache_len < 255 else 255
+        elif subindex == Subindex.FWRITE_LEN:
+            cache_len = len(self.node.fwrite_cache)
+            ret = cache_len if cache_len < 255 else 255
+        elif subindex == Subindex.CACHE_SELECTOR:
+            ret = self.selector
+        elif subindex == Subindex.FILTER:
+            ret = self.filter
+        elif subindex == Subindex.CACHE_LENGTH:
+            cache_len = len(self.file_caches[self.selector].files(self.filter))
+            ret = cache_len if cache_len < 255 else 255
+        elif subindex == Subindex.ITER:
+            ret = self.iter
+        elif subindex == Subindex.FILE_NAME:
+            files = self.file_caches[self.selector].files(self.filter)
+            ret = files[self.iter].name if self.iter < len(files) else ''
+        elif subindex == Subindex.FILE_SIZE:
+            dir_name = self.file_caches[self.selector].dir
+            files = self.file_caches[self.selector].files(self.filter)
+            if self.iter < len(files):
+                file_path = f'{dir_name}/{files[self.iter].name}'
                 ret = getsize(file_path)
-        except Exception as e:
-            logger.error(e)
+            else:
+                ret = 0
 
         return ret
 
     def on_write(self, index: int, subindex: int, value):
 
         if index != self.index:
             return
```

### Comparing `oresat-olaf-2.1.2/olaf/_internals/resources/fread.py` & `oresat-olaf-2.2.0/olaf/_internals/resources/fwrite.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,86 +1,101 @@
+import json
 import zlib
 from os import remove, listdir
-from os.path import basename
+from os.path import basename, isfile
 from pathlib import Path
 from enum import IntEnum, auto
 
 from loguru import logger
 
+from ...common.oresat_file import OreSatFile
 from ...common.resource import Resource
 
 
 class Subindex(IntEnum):
     FILE_NAME = auto()
     FILE_DATA = auto()
     CRC32 = auto()
     DELETE_FILE = auto()
+    TOTAL_FILES = auto()
+    FILE_NAMES = auto()
 
 
-class FreadResource(Resource):
-    '''Resource for readings file over the CAN bus'''
+class FwriteResource(Resource):
+    '''Resource for writing files over the CAN bus'''
 
     def __init__(self):
         super().__init__()
 
-        self.index = 0x3003
+        self.index = 0x3004
         self.file_path = ''
 
-        self.tmp_dir = '/tmp/oresat/fread'
+        self.tmp_dir = '/tmp/oresat/fwrite'
         Path(self.tmp_dir).mkdir(parents=True, exist_ok=True)
-        logger.debug(f'fread tmp dir is {self.tmp_dir}')
+        logger.debug(f'fwrite tmp dir is {self.tmp_dir}')
         for i in listdir(self.tmp_dir):
             remove(f'{self.tmp_dir}/{i}')
 
     def on_start(self):
 
         self.node.add_sdo_read_callback(self.index, self.on_read)
         self.node.add_sdo_write_callback(self.index, self.on_write)
 
     def on_read(self, index: int, subindex: int):
 
         ret = None
 
         if index != self.index:
-            return ret
+            return
 
         if subindex == Subindex.FILE_NAME:
             ret = basename(self.file_path)
         elif subindex == Subindex.CRC32:
-            try:
+            if isfile(self.file_path):
                 with open(self.file_path, 'rb') as f:
                     ret = zlib.crc32(f.read())
-            except FileNotFoundError as e:
-                logger.exception(e)
-        elif subindex == Subindex.FILE_DATA:
-            if not self.file_path:
-                logger.error('fread file path was not set before trying to read file data')
-                return b''
-
-            try:
-                with open(self.file_path, 'rb') as f:
-                    ret = f.read()
-            except FileNotFoundError as e:
-                logger.exception(e)
+            else:
+                logger.debug(f'cannot get CRC32, file "{self.file_path}" does not exist')
+                ret = 0
+        elif subindex == Subindex.TOTAL_FILES:
+            ret = len(self.node.fwrite_cache)
+        elif subindex == Subindex.FILE_NAMES:
+            ret = json.dumps([i.name for i in self.node.fwrite_cache.files()])
 
         return ret
 
     def on_write(self, index: int, subindex: int, value):
 
         if index != self.index:
             return
 
         if subindex == Subindex.FILE_NAME:
             try:
-                self.file_path = self.node.fread_cache.get(value, self.tmp_dir, True)
-            except FileNotFoundError:
-                logger.error(f'file {value} not in fread cache')
+                OreSatFile(value)  # valiate file name format
+                self.file_path = self.tmp_dir + '/' + value
+            except ValueError:
+                logger.error(f'{value} is not a valid file name format')
                 self.file_path = ''
+        elif subindex == Subindex.FILE_DATA:
+            if not self.file_path:
+                logger.error('fwrite file path was not set before file data was sent')
+                return
+
+            try:
+                with open(self.file_path, 'wb') as f:
+                    f.write(value)
+                logger.info(f'receive new file: {basename(self.file_path)}')
+                self.node.fwrite_cache.add(self.file_path, consume=True)
+            except Exception as e:
+                logger.exception(e)
+
+            # clear file data OD obj value to not waste memory
+            self.node.od[index][subindex].value = ''
         elif subindex == Subindex.DELETE_FILE:
             if self.file_path:
                 # delete file from cache and tmp dir
-                self.node.fread_cache.remove(basename(self.file_path))
+                self.node.fwrite_cache.remove(basename(self.file_path))
                 remove(self.file_path)
                 self.file_path = ''
-                logger.info(f'{basename(self.file_path)} was deleted from fread cache')
+                logger.info(f'{basename(self.file_path)} was deleted from fwrite cache')
             else:
-                logger.error('fread file path was not set before trying to delete file')
+                logger.error('fwrite file path was not set before trying to delete file')
```

### Comparing `oresat-olaf-2.1.2/olaf/_internals/resources/logs.py` & `oresat-olaf-2.2.0/olaf/_internals/services/logs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,47 @@
 import tarfile
 from os import listdir
 
 from loguru import logger
 
-from ...common.resource import Resource
+from ...common.service import Service
 from ...common.oresat_file import new_oresat_file
-from ...common.timer_loop import TimerLoop
 
 
-class LogsResource(Resource):
-    '''Resource for getting logs'''
+class LogsService(Service):
+    '''Service for getting logs'''
 
     def __init__(self):
         super().__init__()
 
         self.index = 0x3006
         self.logs_dir_path = '/var/log/journal/'
 
-        self.timer_loop = TimerLoop('logs resource', self._loop, 500)
-        self.failed = True
-
     def on_start(self):
 
         self.make_logs_obj = self.node.od[self.index][1]
         self.make_logs_obj.value = False  # make sure this is False by default
 
         self.node.add_sdo_read_callback(self.index, self.on_read)
 
-        self.timer_loop.start()
-
-    def on_end(self):
-
-        self.timer_loop.stop()
-
-    def _loop(self):
+    def on_loop(self):
 
         if self.make_logs_obj.value:
             logger.info('Making a copy of logs')
 
             tar_file_path = '/tmp/' + new_oresat_file('logs', ext='.tar.xz')
 
             with tarfile.open(tar_file_path, 'w:xz') as t:
                 for i in listdir(self.logs_dir_path):
                     t.add(self.logs_dir_path + '/' + i, arcname=i)
 
             self.node.fread_cache.add(tar_file_path, consume=True)
             self.make_logs_obj.value = False
 
-        return True
+        self.sleep(0.5)
 
     def on_read(self, index: int, subindex: int):
 
         if index != self.index and subindex != 2:
             return
 
         with open('/tmp/olaf.log', 'r') as f:
```

### Comparing `oresat-olaf-2.1.2/olaf/_internals/resources/power_control.py` & `oresat-olaf-2.2.0/olaf/_internals/resources/power_control.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.2/olaf/_internals/resources/store_eds.py` & `oresat-olaf-2.2.0/olaf/_internals/resources/store_eds.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.2/olaf/_internals/resources/system_info.py` & `oresat-olaf-2.2.0/olaf/_internals/resources/system_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,25 +112,25 @@
         elif subindex == Subindex.RAM_FREE:
             ret = psutil.virtual_memory().free // _B_TO_MB
         elif subindex == Subindex.RAM_SHARED:
             ret = psutil.virtual_memory().shared // _B_TO_MB
         elif subindex == Subindex.RAM_BUFFERED:
             ret = psutil.virtual_memory().buffers // _B_TO_MB
         elif subindex == Subindex.RAM_PERCENT:
-            ret = psutil.virtual_memory().percent
+            ret = int(psutil.virtual_memory().percent)
         elif subindex == Subindex.SWAP_FREE:
             ret = psutil.swap_memory().free // _B_TO_MB
         elif subindex == Subindex.SWAP_PERCENT:
-            ret = psutil.swap_memory().percent
+            ret = int(psutil.swap_memory().percent)
         elif subindex == Subindex.PROCS:
             ret = len(psutil.pids())
         elif subindex == Subindex.ROOT_PART_FREE:
             ret = psutil.disk_usage('/').free // _B_TO_MB
         elif subindex == Subindex.ROOT_PART_PERCENT:
-            ret = psutil.disk_usage('/').percent
+            ret = int(psutil.disk_usage('/').percent)
 
         return ret
 
     def on_write(self, index: int, subindex: int, value):
 
         if index != self.index or subindex != Subindex.RPROC_ITER:
             return
```

### Comparing `oresat-olaf-2.1.2/olaf/_internals/resources/updater.py` & `oresat-olaf-2.2.0/olaf/_internals/services/updater.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,45 @@
 from enum import IntEnum, auto
 
 from loguru import logger
 
-from ...common.resource import Resource
-from ...common.timer_loop import TimerLoop
+from ...common.service import Service
 from ..updater import Updater, UpdaterError
 
 
 class Subindex(IntEnum):
     STATUS = auto()
     UPDATES_CACHED = auto()
     LIST_AVAILABLE = auto()
     UPDATE = auto()
     MAKE_STATUS_FILE = auto()
 
 
-class UpdaterResource(Resource):
-    '''Resource for interacting with the updater'''
+class UpdaterService(Service):
+    '''Service for interacting with the updater'''
 
     def __init__(self, updater: Updater):
         super().__init__()
 
         self._updater = updater
         self.index = 0x3100
-        self.timer_loop = TimerLoop('updater resource', self._loop, 500)
 
     def on_start(self):
 
         record = self.node.od[self.index]
         self.update_obj = record[Subindex.UPDATE.value]
         self.make_status_obj = record[Subindex.MAKE_STATUS_FILE.value]
-        self.timer_loop.start()
 
         # make sure defaults are set correctly (override the values from eds/dcf)
         self.update_obj.value = False
         self.make_status_obj.value = False
 
         self.node.add_sdo_read_callback(self.index, self.on_read)
 
-    def on_end(self):
-
-        self.timer_loop.stop()
-
-    def _loop(self):
+    def on_loop(self):
 
         # check for update files in fwrite cache
         for i in self.node.fwrite_cache.files('update'):
             self._updater.add_update(self.node.fwrite_cache.dir + '/' + i)
 
         # check for flag to start a update
         if self.update_obj.value:
@@ -58,22 +51,22 @@
 
         # check for flag to make a status archive
         if self.make_status_obj.value:
             status_archive_file_path = self._updater.make_status_archive()
             self.node.fread_cache.add(status_archive_file_path, consume=True)
             self.make_status_obj.value = False
 
-        return True
+        self.sleep(0.5)
 
     def on_read(self, index: int, subindex: int):
 
         ret = None
 
         if index == self.index:
             if subindex == Subindex.STATUS:
                 ret = self._updater.status.value
             elif subindex == Subindex.UPDATES_CACHED:
-                ret = self._updater.updates_cached
+                ret = len(self._updater.updates_cached)
             elif subindex == Subindex.LIST_AVAILABLE:
-                ret = ' '.join(self._cache.files())
+                ret = ' '.join(self._updater.updates_cached)
 
         return ret
```

### Comparing `oresat-olaf-2.1.2/olaf/_internals/rest_api/__init__.py` & `oresat-olaf-2.2.0/olaf/_internals/rest_api/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     DataType.INTEGER8,
     DataType.INTEGER16,
     DataType.INTEGER32,
     DataType.INTEGER64,
     DataType.UNSIGNED8,
     DataType.UNSIGNED16,
     DataType.UNSIGNED32,
-    DataType.UNSIGNED64
+    DataType.UNSIGNED64,
 ]
 
 
 class RestAPI:
     '''
     An optional Flask app for reading and writing values into the OD.
 
@@ -118,134 +118,174 @@
         Template file name.
     name: str
         Nice name for the template.
     '''
     return render_template(template, title=_TITLE, name=name)
 
 
+def make_error_json(error: str) -> str:
+    '''
+    Make the stand error json message for the REST API
+
+    Parameters
+    ----------
+    error: str
+        The error message
+
+    Returns
+    -------
+    str
+        The JSON error message
+    '''
+
+    return jsonify({'error': error})
+
+
 rest_api = RestAPI()
 '''The global instance of the REST API.'''
 
 
 @rest_api.app.route('/')
 def root():
 
     routes = []
     for p in rest_api.app.url_map.iter_rules():
         route = str(p)
         if not route.startswith('/static/') and not route.startswith('/od/') \
-                and route not in ['/', '/favicon.ico']:
+                and route not in ['/', '/favicon.ico', '/od-all']:
             routes.append(str(p))
 
     routes = natsorted(routes)
 
     return render_template('root.html', title=os.uname()[1], routes=routes)
 
 
 @rest_api.app.route('/favicon.ico')
 def favicon():
     path = os.path.dirname(os.path.abspath(__file__))
     return send_from_directory(f'{path}/static', 'favicon.ico')
 
 
+def _json_value_to_value(data_type: DataType, json_value):
+    '''Convert JSON value to real OD value to bytes for SDO callback'''
+
+    if data_type == DataType.BOOLEAN and not isinstance(json_value, bool):
+        value = True if json_value.lower() == 'true' else False
+    elif data_type in INT_TYPES and not isinstance(json_value, int):
+        value = int(json_value, 16) if json_value.startswith('0x') else int(json_value)
+    elif data_type in [DataType.REAL32, DataType.REAL64]:
+        value = float(json_value)
+    elif data_type == DataType.DOMAIN:
+        value = base64.decodebytes(json_value.encode('utf-8'))
+    else:  # str
+        value = json_value
+
+    return value
+
+
 @rest_api.app.route('/od/<index>/', methods=['GET', 'PUT'])
 def od_index(index: str):
 
     try:
         index = int(index, 16) if index.startswith('0x') else int(index)
     except ValueError:
-        return jsonify({'error': f'invalid index {index}'})
+        return make_error_json(f'invalid index {index}')
 
     try:
-        obj = app.node.od[index]
+        obj = app.od[index]
     except Exception:
         msg = f'no object at index {index:02X}'
-        logger.error(f'RestApiError: {msg}')
-        return jsonify({'error': msg})
+        logger.error(f'REST API error: {msg}')
+        return make_error_json(msg)
 
     if request.method == 'PUT':
-        raw = request.json['value']
-        data_type = obj.data_type
+        try:
+            json_value = request.json['value']
 
-        if data_type == DataType.DOMAIN:
-            app.node._node.sdo[index].raw = base64.decodebytes(raw.encode('utf-8'))
-        else:
-            app.node._node.sdo[index].phys = raw_to_value(data_type, raw)
+            # convert value from JSON to bytes for SDO callback
+            value = _json_value_to_value(obj.data_type, json_value)
+            raw = obj.encode_raw(value)
+
+            app.node._on_sdo_write(index, 0, obj, raw)
+        except Exception as e:
+            logger.error(f'REST API error: {e}')
+            return make_error_json(str(e))
 
-    return jsonify(object_to_json(index))
+    return jsonify(_object_to_dict(index))
 
 
 @rest_api.app.route('/od/<index>/<subindex>/', methods=['GET', 'PUT'])
 def od_subindex(index: str, subindex: str):
 
     try:
         index = int(index, 16) if index.startswith('0x') else int(index)
         subindex = int(subindex, 16) if subindex.startswith('0x') else int(subindex)
     except ValueError:
-        return jsonify({'error': f'invalid index {index} or subindex {subindex}'})
+        return make_error_json(f'invalid index {index} or subindex {subindex}')
 
     try:
-        obj = app.node.od[index][subindex]
+        obj = app.od[index][subindex]
     except Exception:
         msg = f'no object at index {index:04X} subindex {subindex:02X}'
-        logger.error(f'RestApiError: {msg}')
-        return jsonify({'error': msg})
+        logger.error(f'REST API error: {msg}')
+        return make_error_json(msg)
 
     if request.method == 'PUT':
-        raw = request.json['value']
-        data_type = obj.data_type
-
-        if data_type == DataType.DOMAIN:
-            app.node._node.sdo[index][subindex].raw = base64.decodebytes(raw.encode('utf-8'))
-        else:
-            app.node._node.sdo[index][subindex].phys = raw_to_value(data_type, raw)
-
-    return jsonify(object_to_json(index, subindex))
+        try:
+            json_value = request.json['value']
 
+            # convert value from JSON to bytes for SDO callback
+            value = _json_value_to_value(obj.data_type, json_value)
+            raw = obj.encode_raw(value)
 
-def raw_to_value(data_type: DataType, raw):
-    value = None
+            app.node._on_sdo_write(index, subindex, obj, raw)
+        except Exception as e:
+            logger.error(f'REST API error: {e}')
+            return make_error_json(str(e))
 
-    if data_type == DataType.BOOLEAN and not isinstance(raw, bool):
-        value = True if raw.lower() == 'true' else False
-    elif data_type in INT_TYPES and not isinstance(raw, int):
-        value = int(raw, 16) if raw.startswith('0x') else int(raw)
-    elif data_type in [DataType.REAL32, DataType.REAL64]:
-        value = float(raw)
-    else:
-        value = raw
+    return jsonify(_object_to_dict(index, subindex))
 
-    return value
 
+def _object_to_dict(index: int, subindex: int = None) -> dict:
+    '''
+    Convert a OD object to a dictionary.
 
-def object_to_json(index: int, subindex: int = None) -> dict:
+    Parameters
+    ----------
+    index: int
+        The index of the object to convert.
+    subindex: int
+        Optional subindex of the object to convert.
+
+    Returns
+    -------
+    dict
+        The object as a dictionary.
+    '''
 
     if subindex is None:
         try:
             obj = app.node.od[index]
-            if isinstance(obj, canopen.objectdictionary.Variable):
-                if obj.data_type == DataType.DOMAIN:
-                    raw = app.node._node.sdo[index].raw
-                    value = base64.encodebytes(raw).decode('utf-8')
-                else:
-                    value = app.node._node.sdo[index].phys
-        except Exception as e:
-            logger.debug(e)
-            return {'error': f'0x{index:04X} is not a valid index'}
+        except Exception:
+            msg = f'0x{index:04X} is not a valid index'
+            logger.debug('REST API error: ' + msg)
+            return make_error_json(msg)
     else:
         try:
             obj = app.node.od[index][subindex]
-            if obj.data_type == DataType.DOMAIN:
-                raw = app.node._node.sdo[index][subindex].raw
-                value = base64.encodebytes(raw).decode('utf-8')
-            else:
-                value = app.node._node.sdo[index][subindex].phys
-        except Exception as e:
-            logger.debug(e)
-            return {'error': f'0x{subindex:02X} not a valid subindex for index 0x{index:04X}'}
+        except Exception:
+            msg = f'0x{subindex:02X} not a valid subindex for index 0x{index:04X}'
+            logger.debug('REST API error: ' + msg)
+            return make_error_json(msg)
+
+    if isinstance(obj, canopen.objectdictionary.Variable):
+        value = app.node._on_sdo_read(index, subindex, obj)
+        if obj.data_type in [DataType.DOMAIN, DataType.OCTET_STRING] and value is not None:
+            # encode bytes data types for JSON
+            value = base64.encodebytes(value).decode('utf-8')
 
     data = {
         'name': obj.name,
     }
 
     if isinstance(obj, canopen.objectdictionary.Variable):
         data['object_type'] = 'VARIABLE'
@@ -253,19 +293,29 @@
         data['data_type'] = DataType(obj.data_type).name
         if obj.access_type == 'wo':
             data['value'] = ''
         else:
             data['value'] = value
     elif isinstance(obj, canopen.objectdictionary.Array):
         data['object_type'] = 'ARRAY'
-        data['subindexes'] = {subindex: object_to_json(index, subindex) for subindex in obj}
+        data['subindexes'] = {subindex: _object_to_dict(index, subindex) for subindex in obj}
     else:
         data['object_type'] = 'RECORD'
-        data['subindexes'] = {subindex: object_to_json(index, subindex) for subindex in obj}
+        data['subindexes'] = {subindex: _object_to_dict(index, subindex) for subindex in obj}
+
+    return data
 
+
+@rest_api.app.route('/od-all', methods=['GET'])
+def get_all_object():
+    data = {}
+    for index in app.od:
+        if index < 0x1000:
+            continue
+        data[index] = _object_to_dict(index)
     return data
 
 
 @rest_api.app.route('/od')
 def od_template():
     return render_olaf_template('od.html', name='Object Dictionary')
 
@@ -299,7 +349,17 @@
 def logs_template():
     return render_olaf_template('logs.html', name='Logs')
 
 
 @rest_api.app.route('/power-control')
 def power_control_template():
     return render_olaf_template('power_control.html', name='Power Control')
+
+
+@rest_api.app.route('/daemons')
+def daemons_template():
+    return render_olaf_template('daemons.html', name='External Daemons')
+
+
+@rest_api.app.route('/oresat-configs')
+def oresat_configs_template():
+    return render_olaf_template('oresat_configs.html', name='OreSat Configs')
```

### Comparing `oresat-olaf-2.1.2/olaf/_internals/rest_api/static/favicon.ico` & `oresat-olaf-2.2.0/olaf/_internals/rest_api/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.2/olaf/_internals/rest_api/templates/base.html` & `oresat-olaf-2.2.0/olaf/_internals/rest_api/templates/base.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 <!DOCTYPE html>
-<html lang='en'>
+<html lang="en">
 <head>
   <title>{{title}}</title>
   <style>
     #headerGrid {
       display: grid;
       grid-template-columns: 25% 50% 25%;
     }
     #headerCenter {
       text-align: center;
     }
   </style>
-  <div id='headerGrid'>
-    <div id='headerLeft'>
-       <a href='/'>home</a>
+  <div id="headerGrid">
+    <div id="headerLeft">
+       <a href="/">home</a>
     </div>
-    <div id='headerCenter'>
+    <div id="headerCenter">
       <h2>{{name}}</h2>
     </div>
-    <div id='headerRight'>
+    <div id="headerRight">
     </div>
   </div>
 </head>
 <body>
   <style>
     #content {
       text-align: center;
@@ -36,77 +36,87 @@
      * @param {String} subindex The eubndex of the object to write to. Set to
      * null if subindex is not needed. 
      *
      * @return {Object} The object from the OD.
      */
     async function readValue(index, subindex) {
       let url = `http://${window.location.host}/od/${index}`;
-      if (subindex !== null && subindex !== '') {
+      if (subindex !== null && subindex !== "") {
         url = `http://${window.location.host}/od/${index}/${subindex}`;
       }
 
       return await fetch(url)
         .then(response => response.json())
-        .then(data => { return data; });
+        .then(data => {
+          if (data.error !== undefined) {
+            console.log(data);
+          }
+          return data;
+        });
     }
 
     /**
      * Write a value to OD.
      *
      * @param {String} index The index of the object to write to.
      * @param {String} subindex The eubndex of the object to write to. Set to
      * an emoty sring or null if subindex is not needed. 
      * @param {Any} value The value to write to OD.
      *
      * @return {Object} The object after the new value was written to it.
      */
     async function writeValue(index, subindex, value) {
       let options = {
-        'method': 'PUT',
+        "method": "PUT",
         headers: {
-          'Content-Type': 'application/json',
+          "Content-Type": "application/json",
         },
-        'body': JSON.stringify({
-          'value': value,
+        "body": JSON.stringify({
+          "value": value,
         }),
       };
       
       let url = `http://${window.location.host}/od/${index}`;
-      if (subindex !== null && subindex !== '') {
+      if (subindex !== null && subindex !== "") {
         url = `http://${window.location.host}/od/${index}/${subindex}`;
       }
 
       return await fetch(url, options)
         .then(response => response.json())
-        .then(data => { return data; });
+        .then(data => {
+          if (data.error !== undefined) {
+            console.log(data);
+          }
+          return data;
+        });
     }
 
     /**
      * Convert a SCET value to a data object.
      *
      * @param {Number} scet The SCET value.
      *
      * @return {Date} The date object.
      */
     function scetToDate(scet) {
       // convert to binary
       let base2 = scet.toString(2);
-      const leadingZeros = '0'.repeat(64 - base2.length);
+      const leadingZeros = "0".repeat(64 - base2.length);
       base2 = leadingZeros + base2;
 
       const coarseStr = base2.substring(32);
       const fineStr = base2.substring(8, 32);
 
       const coarse = parseInt(coarseStr, 2);
       const fine = parseInt(fineStr, 2);
 
       // make unix time in ms
       const time = coarse * 1000 + fine / 1000;
 
       return new Date(time);
     }
   </script>
-  <div id='content'>
+  <div id="content">
     {% block content %}{% endblock %}
   </div>
 </body>
 </html>
```

### Comparing `oresat-olaf-2.1.2/olaf/_internals/rest_api/templates/fread.html` & `oresat-olaf-2.2.0/olaf/_internals/rest_api/templates/fread.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-{% extends 'base.html' %}
+{% extends "base.html" %}
 
 {% block content %}
   <label for="files">Select a File</label>  
-  <select id='files'>
-    <option value='1'>NONE</option>  
+  <select id="files">
+    <option value="1">NONE</option>  
   </select>
   <br/>
   <br/>
-  <button id='downloadFileButton' onclick='downloadFile()' disabled>Download</button>
-  <button id='deleteFileButton' onclick='deleteFile()' disabled>Delete</button>
+  <button id="downloadFileButton" onclick="downloadFile()" disabled>Download</button>
+  <button id="deleteFileButton" onclick="deleteFile()" disabled>Delete</button>
   <script>
     async function getFileList() {
-      const fileName = document.getElementById('files').value;
-      const files = await readValue('0x3002','0x01');
-      const select = document.getElementById('files');
+      const fileName = document.getElementById("files").value;
+      const files = await readValue("0x3002","0x01");
+      const select = document.getElementById("files");
 
       if (files.value === 0) {
-          document.getElementById('downloadFileButton').disabled = true;
-          document.getElementById('deleteFileButton').disabled = true;
+          document.getElementById("downloadFileButton").disabled = true;
+          document.getElementById("deleteFileButton").disabled = true;
       } else {
-          document.getElementById('downloadFileButton').disabled = false;
-          document.getElementById('deleteFileButton').disabled = false;
+          document.getElementById("downloadFileButton").disabled = false;
+          document.getElementById("deleteFileButton").disabled = false;
       }
 
       // remove all current options
-      let options = select.getElementsByTagName('option');
+      let options = select.getElementsByTagName("option");
       for (let i = options.length - 1; i >= 0; i--) {
         select.removeChild(options[i]);
       }
 
       // add all files
       for (let i = 0; i < files.value; i++) {
-        let opt = document.createElement('option');
-        const iterObj = await writeValue('0x3002', '0x06', i)
-        const nameObj = await readValue('0x3002', '0x07')
+        let opt = document.createElement("option");
+        const iterObj = await writeValue("0x3002", "0x06", i)
+        const nameObj = await readValue("0x3002", "0x07")
         opt.value = nameObj.value;
         opt.innerHTML = nameObj.value;
         select.appendChild(opt);
       }
 
       // reselect previous option
-      if (fileName !== '') {
+      if (fileName !== "") {
         select.value = fileName;
       }
     }
 
     async function downloadFile() {
-      const fileName = document.getElementById('files').value;
-      const fileNameObj = await writeValue('0x3003', '0x01', fileName);
-      const fileDataObj = await readValue('0x3003', '0x02');
+      const fileName = document.getElementById("files").value;
+      const fileNameObj = await writeValue("0x3003", "0x01", fileName);
+      const fileDataObj = await readValue("0x3003", "0x02");
 
       const byteCharacters = atob(fileDataObj.value);
       const byteArrays = [];
       const sliceSize = 512;
 
       for (let offset = 0; offset < byteCharacters.length; offset += sliceSize) {
         const slice = byteCharacters.slice(offset, offset + sliceSize);
@@ -63,27 +63,27 @@
         }
 
         const byteArray = new Uint8Array(byteNumbers);
         byteArrays.push(byteArray);
       }
 
       const blob = new Blob(byteArrays, {
-        type: 'application/octet-stream'
+        type: "application/octet-stream"
       });
 
-      const a = document.createElement('a');
+      const a = document.createElement("a");
       a.download = fileNameObj.value;
       a.href = window.URL.createObjectURL(blob);
       a.click();
     }
 
     async function deleteFile() {
-      const fileName = document.getElementById('files').value;
-      const fileNameObj = await writeValue('0x3003', '0x01', fileName);
-      const fileDeleteObj = await writeValue('0x3003', '0x04', true);
+      const fileName = document.getElementById("files").value;
+      const fileNameObj = await writeValue("0x3003", "0x01", fileName);
+      const fileDeleteObj = await writeValue("0x3003", "0x04", true);
     }
 
 
     getFileList();
     const interval = setInterval(function() {
       getFileList();
     }, 60000);
```

### Comparing `oresat-olaf-2.1.2/olaf/_internals/rest_api/templates/fwrite.html` & `oresat-olaf-2.2.0/olaf/_internals/rest_api/templates/fwrite.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,46 @@
-{% extends 'base.html' %}
+{% extends "base.html" %}
 
 {% block content %}
-  <label for='filename'>File:</label>
-  <input type='file' id='filename' name='filename'/>
-  <button onclick='uploadFile()'>Upload</button>
+  <label for="filename">File:</label>
+  <input type="file" id="filename" name="filename"/>
+  <button onclick="uploadFile()">Upload</button>
+  <p><b>NOTE:</b> All file must be in <i>card_keyword_unixtime.extension</i> format</p>
   <script>
     /** Callback when the upload button is clicked. */
     function uploadFile() {
-      const file = document.getElementById('filename').files[0];
+      const file = document.getElementById("filename").files[0];
 
       const fileReader = new FileReader();
       fileReader.readAsBinaryString(file);
       fileReader.onload = function() {
         fwrite(file.name, fileReader.result);
       }
       fileReader.onerror = function() {
-        alert(fileReader.error);
+        alert("error: " + fileReader.error);
       }
     }
 
     /**
      * Write file to OLAF app.
      *
      * @param fileName {String} The file name to write.
      * @param fileData {String} The file data as a binary string to write.
      */
     async function fwrite(fileName, fileData) {
      // Write the file name to OD.
-      const obj = await writeValue('0x3004','0x01', fileName);
+      const obj = await writeValue("0x3004","0x01", fileName);
 
-      // Validate the file name was set to new value in OD, if it wasn't it was not a
+      // Validate the file name was set to new value in OD, if it wasn"t it was not a
       // valid file name.
       if (obj.value !== fileName) {
-        alert('fwrite failed due to an invalid file name format');
+        alert("error: fwrite failed due to an invalid file name format");
         return;
       }
 
      // Write the file data to OD.
-      await writeValue('0x3004','0x02', btoa(fileData));
+      await writeValue("0x3004","0x02", btoa(fileData));
       
-      alert('fwrite was successful');
+      alert("fwrite was successful");
     }
   </script>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,2 +1,3 @@
-{% extends 'base.html' %} {% block content %} File: [File] Upload
+{% extends "base.html" %} {% block content %} File: [File] Upload
+NOTE: All file must be in card_keyword_unixtime.extension format
  {% endblock %}
```

### Comparing `oresat-olaf-2.1.2/olaf/_internals/rest_api/templates/logs.html` & `oresat-olaf-2.2.0/olaf/_internals/rest_api/templates/logs.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-{% extends 'base.html' %}
+{% extends "base.html" %}
 
 {% block content %}
   <style>
     #page {
       justify-content: center;
       display: flex;
     }
     textarea {
       resize: none;
       width: 100%;
     }
   </style>
-  <div id='page'>
+  <div id="page">
     <br/>
-    <textarea id='logs' rows=40 disabled></textarea>
+    <textarea id="logs" rows=40 disabled></textarea>
   </div>
   <script>
     async function updateLogs() {
-      const logsObj = await readValue('0x3006', '0x02');
-      document.getElementById('logs').value = logsObj.value;
+      const logsObj = await readValue("0x3006", "0x02");
+      document.getElementById("logs").value = logsObj.value;
     }
 
     updateLogs();
     const interval = setInterval(function() {
       updateLogs()
     }, 60000);
   </script>
```

### Comparing `oresat-olaf-2.1.2/olaf/_internals/rest_api/templates/os_command.html` & `oresat-olaf-2.2.0/olaf/_internals/rest_api/templates/os_command.html`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends 'base.html' %}
+{% extends "base.html" %}
 
 {% block content %}
   <style>
     #page {
       justify-content: center;
       display: flex;
     }
@@ -17,62 +17,62 @@
       width: 94%;
     }
     textarea {
       resize: none;
       width: 100%;
     }
   </style>
-  <div id='page'>
-    <div id='abc'>
-      <a class='boldText'>Status: </a><span id='status'></span>
+  <div id="page">
+    <div id="abc">
+      <a class="boldText">Status: </a><span id="status"></span>
       <br/>
       <br/>
-      <label for='command'>Bash Command:</label>
+      <label for="command">Bash Command:</label>
       <br/>
-      <input type='text' id='command' name='command'/>
-      <button onclick='runCommand()'>Run</button>
+      <input type="text" id="command" name="command"/>
+      <button onclick="runCommand()">Run</button>
       <br/>
       <br/>
-      <a class='boldText'>Reply:</a>
+      <a class="boldText">Reply:</a>
       <br/>
-      <textarea id='reply' rows=30 disabled></textarea>
+      <textarea id="reply" rows=30 disabled></textarea>
     </div>
   </div>
   <script>
     const states = {
-        0: 'NO_ERROR_NO_REPLY',
-        1: 'NO_ERROR_REPLY',
-        2: 'ERROR_NO_REPLY',
-        3: 'ERROR_REPLY',
-        255: 'EXECUTING',
+        0: "NO_ERROR_NO_REPLY",
+        1: "NO_ERROR_REPLY",
+        2: "ERROR_NO_REPLY",
+        3: "ERROR_REPLY",
+        255: "EXECUTING",
     };
 
     async function runCommand() {
       // clear last reply
-      document.getElementById('reply').value = '';
+      document.getElementById("reply").value = "";
 
       // reset field incase of very quick commands
-      document.getElementById('status').textContent = 'EXECUTING';
+      document.getElementById("status").textContent = "EXECUTING";
 
-      const value = document.getElementById('command').value;
+      const value = document.getElementById("command").value;
 
-      writeValue('0x1023', '0x01', btoa(value));
+      writeValue("0x1023", "0x01", btoa(value));
     }
 
     async function updateStatus() {
-      const reply_states = ['NO_ERROR_REPLY', 'ERROR_REPLY'];
+      const reply_states = ["NO_ERROR_REPLY", "ERROR_REPLY"];
 
-      const statusObj = await readValue('0x1023', '0x02');
-      const status = document.getElementById('status');
-      const newStatus = states[statusObj['value']];
+      const statusObj = await readValue("0x1023", "0x02");
+      const status = document.getElementById("status");
+      const newStatus = states[statusObj["value"]];
 
       // state has change to a new state with a reply, display reply
-      if (status.textContent === 'EXECUTING' && reply_states.includes(newStatus)) {
-        const replyObj = await readValue('0x1023', '0x03');
-        document.getElementById('reply').value = atob(replyObj.value);
+      if (status.textContent === "EXECUTING" && reply_states.includes(newStatus)) {
+        const replyObj = await readValue("0x1023", "0x03");
+        document.getElementById("reply").value = atob(replyObj.value);
       }
 
       status.textContent = newStatus;
     }
 
     runCommand();
     updateStatus();
```

### Comparing `oresat-olaf-2.1.2/olaf/_internals/rest_api/templates/system_info.html` & `oresat-olaf-2.2.0/olaf/_internals/rest_api/templates/system_info.html`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends 'base.html' %}
+{% extends "base.html" %}
 
 {% block content %}
   <style>
     table {
       font-family: arial, sans-serif;
       border-collapse: collapse;
       margin-left: auto;
@@ -13,145 +13,145 @@
       text-align: left;
       padding: 8px;
     }
   </style>
   <table>
     <tr>
       <td>OS Name</td>
-      <td><span id='osName'></span></td>
+      <td><span id="osName"></span></td>
     </tr>
     <tr>
       <td>OS Distro</td>
-      <td><span id='osDistro'></span></td>
+      <td><span id="osDistro"></span></td>
     </tr>
     <tr>
       <td>OS Kernel Version</td>
-      <td><span id='osKernelVersion'></span></td>
+      <td><span id="osKernelVersion"></span></td>
     </tr>
     <tr>
       <td>Hostname</td>
-      <td><span id='hostname'></span></td>
+      <td><span id="hostname"></span></td>
     </tr>
     <tr>
       <td>Uptime</td>
-      <td><span id='uptime'></span> s</td>
+      <td><span id="uptime"></span> s</td>
     </tr>
     <tr>
       <td>Number of CPUs</td>
-      <td><span id='cpuNum'></span></td>
+      <td><span id="cpuNum"></span></td>
     </tr>
     <tr>
       <td>CPU Architecture</td>
-      <td><span id='cpuArch'></span></td>
+      <td><span id="cpuArch"></span></td>
     </tr>
     <tr>
       <td>CPU Governor</td>
-      <td><span id='cpuGov'></span></td>
+      <td><span id="cpuGov"></span></td>
     </tr>
     <tr>
       <td>CPU Frequency</td>
-      <td><span id='cpuFreq'></span> MHz</td>
+      <td><span id="cpuFreq"></span> MHz</td>
     </tr>
     <tr>
       <td>Number of Remote Processors</td>
-      <td><span id='remoteProcNum'></span></td>
+      <td><span id="remoteProcNum"></span></td>
     </tr>
     <tr>
       <td>Load 1 minute</td>
-      <td><span id='load1Min'></span></td>
+      <td><span id="load1Min"></span></td>
     </tr>
     <tr>
       <td>Load 5 minute</td>
-      <td><span id='load5Min'></span></td>
+      <td><span id="load5Min"></span></td>
     </tr>
     <tr>
       <td>Load 15 minute</td>
-      <td><span id='load15Min'></span></td>
+      <td><span id="load15Min"></span></td>
     </tr>
     <tr>
       <td>RAM Total</td>
-      <td><span id='ramTotal'></span> MB</td>
+      <td><span id="ramTotal"></span> MB</td>
     </tr>
     <tr>
       <td>RAM Free</td>
-      <td><span id='ramFree'></span> MB</td>
+      <td><span id="ramFree"></span> MB</td>
     </tr>
     <tr>
       <td>RAM Shared</td>
-      <td><span id='ramShared'></span> MB</td>
+      <td><span id="ramShared"></span> MB</td>
     </tr>
     <tr>
       <td>RAM Buffered</td>
-      <td><span id='ramBuffered'></span> MB</td>
+      <td><span id="ramBuffered"></span> MB</td>
     </tr>
     <tr>
       <td>RAM Percent</td>
-      <td><span id='ramPercent'></span> %</td>
+      <td><span id="ramPercent"></span> %</td>
     </tr>
     <tr>
       <td>Swap Total</td>
-      <td><span id='swapTotal'></span> MB</td>
+      <td><span id="swapTotal"></span> MB</td>
     </tr>
     <tr>
       <td>Swap Free</td>
-      <td><span id='swapFree'></span> MB</td>
+      <td><span id="swapFree"></span> MB</td>
     </tr>
     <tr>
       <td>Swap Percent</td>
-      <td><span id='swapPercent'></span> %</td>
+      <td><span id="swapPercent"></span> %</td>
     </tr>
     <tr>
       <td>Number of Current Processes</td>
-      <td><span id='procs'></span></td>
+      <td><span id="procs"></span></td>
     </tr>
     <tr>
       <td>Root Partition Total</td>
-      <td><span id='rootPartTotal'></span> MB</td>
+      <td><span id="rootPartTotal"></span> MB</td>
     </tr>
     <tr>
       <td>Root Partition Free</td>
-      <td><span id='rootPartFree'></span> MB</td>
+      <td><span id="rootPartFree"></span> MB</td>
     </tr>
     <tr>
       <td>Root Partition Percent</td>
-      <td><span id='rootPartPercent'></span> %</td>
+      <td><span id="rootPartPercent"></span> %</td>
     </tr>
   </table>
   <script>
     const subindexNames = {
-      0x01: 'osName',
-      0x02: 'osDistro',
-      0x03: 'osKernelVersion',
-      0x04: 'hostname',
-      0x05: 'uptime',
-      0x06: 'cpuNum',
-      0x07: 'cpuArch',
-      0x08: 'cpuGov',
-      0x09: 'cpuFreq',
-      0x0A: 'remoteProcNum',
-      0x0E: 'load1Min',
-      0x0F: 'load5Min',
-      0x10: 'load15Min',
-      0x11: 'ramTotal',
-      0x12: 'ramFree',
-      0x13: 'ramShared',
-      0x14: 'ramBuffered',
-      0x15: 'ramPercent',
-      0x16: 'swapTotal',
-      0x17: 'swapFree',
-      0x18: 'swapPercent',
-      0x19: 'procs',
-      0x1A: 'rootPartTotal',
-      0x1B: 'rootPartFree',
-      0x1C: 'rootPartPercent',
+      0x01: "osName",
+      0x02: "osDistro",
+      0x03: "osKernelVersion",
+      0x04: "hostname",
+      0x05: "uptime",
+      0x06: "cpuNum",
+      0x07: "cpuArch",
+      0x08: "cpuGov",
+      0x09: "cpuFreq",
+      0x0A: "remoteProcNum",
+      0x0E: "load1Min",
+      0x0F: "load5Min",
+      0x10: "load15Min",
+      0x11: "ramTotal",
+      0x12: "ramFree",
+      0x13: "ramShared",
+      0x14: "ramBuffered",
+      0x15: "ramPercent",
+      0x16: "swapTotal",
+      0x17: "swapFree",
+      0x18: "swapPercent",
+      0x19: "procs",
+      0x1A: "rootPartTotal",
+      0x1B: "rootPartFree",
+      0x1C: "rootPartPercent",
     };
 
     async  function updateAll() {
       let tmp;
-      const obj = await readValue('0x3001', null);
+      const obj = await readValue("0x3001", null);
       for (const subindex in subindexNames) {
         tmp = document.getElementById(subindexNames[subindex]);
         tmp.textContent = obj.subindexes[subindex].value;
       }
     }
 
     updateAll();
```

### Comparing `oresat-olaf-2.1.2/olaf/_internals/rest_api/templates/updater.html` & `oresat-olaf-2.2.0/olaf/_internals/rest_api/templates/updater.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends 'base.html' %}
+{% extends "base.html" %}
 
 {% block content %}
   <style>
     table {
       font-family: arial, sans-serif;
       border-collapse: collapse;
       margin-left: auto;
@@ -13,64 +13,64 @@
       text-align: left;
       padding: 8px;
     }
   </style>
   <table>
     <tr>
       <td>Status</td>
-      <td><span id='status'></span></td>
+      <td><span id="status"></span></td>
     </tr>
     <tr>
       <td>Updates Available</td>
-      <td><span id='updatesAvailable'></span></td>
+      <td><span id="updatesAvailable"></span></td>
     </tr>
   </table>
   <br/>
-  <button id='startUpdateButton' onclick='startUpdate()' disabled>Start Update</button>
-  <button id='makeStatusFileButton' onclick='makeStatusFile()'>Generate Status File</button>
+  <button id="startUpdateButton" onclick="startUpdate()" disabled>Start Update</button>
+  <button id="makeStatusFileButton" onclick="makeStatusFile()">Generate Status File</button>
   <script>
     const STATES = {
-      0: 'UPDATE_SUCCESSFUL',
-      1: 'PRE_UPDATE_FAILED',
-      2: 'UPDATE_FAILED',
-      255: 'UPDATING',
+      0: "UPDATE_SUCCESSFUL",
+      1: "PRE_UPDATE_FAILED",
+      2: "UPDATE_FAILED",
+      255: "UPDATING",
     }
 
     async function updaterInfo() {
-      const statusObj = await readValue('0x3100', '0x01');
+      const statusObj = await readValue("0x3100", "0x01");
       const newState = STATES[statusObj.value];
-      document.getElementById('status').textContent = newState;
+      document.getElementById("status").textContent = newState;
 
-      const updatesObj = await readValue('0x3100', '0x02');
-      document.getElementById('updatesAvailable').textContent = updatesObj.value;
+      const updatesObj = await readValue("0x3100", "0x02");
+      document.getElementById("updatesAvailable").textContent = updatesObj.value;
 
-      if (newState === 'UPDATING') {
-        document.getElementById('startUpdateButton').disabled = true;
-        document.getElementById('makeStatusFileButton').disabled = true;
+      if (newState === "UPDATING") {
+        document.getElementById("startUpdateButton").disabled = true;
+        document.getElementById("makeStatusFileButton").disabled = true;
       } else {
         if (updatesObj.value === 0) {
-          document.getElementById('startUpdateButton').disabled = true;
-          document.getElementById('makeStatusFileButton').disabled = false;
+          document.getElementById("startUpdateButton").disabled = true;
+          document.getElementById("makeStatusFileButton").disabled = false;
         } else {
-          document.getElementById('startUpdateButton').disabled = false;
-          document.getElementById('makeStatusFileButton').disabled = false;
+          document.getElementById("startUpdateButton").disabled = false;
+          document.getElementById("makeStatusFileButton").disabled = false;
         }
       }
     }
 
     async function startUpdate() {
-      document.getElementById('startUpdateButton').disabled = false;
-      document.getElementById('makeStatusFileButton').disabled = true;
-      writeValue('0x3100', '0x04', true);
+      document.getElementById("startUpdateButton").disabled = false;
+      document.getElementById("makeStatusFileButton").disabled = true;
+      writeValue("0x3100", "0x04", true);
     }
 
     async function makeStatusFile() {
-      document.getElementById('startUpdateButton').disabled = true;
-      document.getElementById('makeStatusFileButton').disabled = false;
-      writeValue('0x3100', '0x05', true);
+      document.getElementById("startUpdateButton").disabled = true;
+      document.getElementById("makeStatusFileButton").disabled = false;
+      writeValue("0x3100", "0x05", true);
     }
 
     updaterInfo();
     const interval = setInterval(function() {
       updaterInfo();
     }, 10000);
   </script>
```

### Comparing `oresat-olaf-2.1.2/olaf/_internals/updater.py` & `oresat-olaf-2.2.0/olaf/_internals/updater.py`

 * *Files 2% similar despite different names*

```diff
@@ -415,18 +415,18 @@
     @property
     def status(self) -> UpdaterState:
         '''UpdaterState: The current state.'''
 
         return self._state
 
     @property
-    def updates_cached(self) -> int:
-        '''int: The number of update archives in cache.'''
+    def updates_cached(self) -> list:
+        '''list: The list of update archives in cache.'''
 
-        return len(self._cache.files())
+        return self._cache.files()
 
     @property
     def list_updates(self) -> str:
         '''str: Get a JSON list of file_name in cache.'''
 
         return json.dumps([i.name for i in self._cache.files()])
```

### Comparing `oresat-olaf-2.1.2/olaf/common/ecss.py` & `oresat-olaf-2.2.0/olaf/common/ecss.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.2/olaf/common/oresat_file.py` & `oresat-olaf-2.2.0/olaf/common/oresat_file.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 '''File name format for OreSat files'''
 
 from os import uname
 from os.path import basename
 from time import time
 
 
-def new_oresat_file(keyword: str, board: str = '', date: float = -1.0, ext: str = '') -> str:
-    '''Convience function for making valid oresat file_names
+def new_oresat_file(keyword: str, card: str = '', date: float = -1.0, ext: str = '') -> str:
+    '''
+    Convience function for making valid oresat file_names
 
     Parameters
     ----------
     keyword: str
         The keyword for the new file_name
-    board: str
-        The board name for the file_name. If not set, the hostname will be
+    card: str
+        The card name for the file_name. If not set, the hostname will be
         used.
-    date: Union(None, float)
+    date: float
         Unix timestamp the file was made. Set to a :py:func:`time.time` value or set to a negative
         number to use current time.
     ext: str
         The file extension. Optional.
 
     Returns
     -------
     str
         The new oresat file name.
     '''
 
-    if not board:
-        board = uname()[1]
+    if not card:
+        card = uname()[1]
+
+    if card.startswith('oresat-'):
+        card = card[7:]  # remove 'oresat-'
 
     if date < 0:
-        date_str = str(int(time()))
+        date_str = str(int(time() * 1000))
     else:
-        date_str = str(int(date))
+        date_str = str(int(date * 1000))
 
     # make sure the extension starts with a '.'
     if len(ext) > 0 and ext[0] != '.':
         ext = '.' + ext
 
-    name = board + '_' + keyword + '_' + date_str + ext
+    name = card + '_' + keyword + '_' + date_str + ext
 
     return name.lower()
 
 
 class OreSatFile:
     '''A class that follows the OreSat file format.'''
 
@@ -62,26 +66,26 @@
 
         self._name = basename(file)
 
         split = self._name.split('_')
         if len(split) != 3:
             raise ValueError('invalid OreSat file name')
 
-        self._board = split[0]
+        self._card = split[0]
         self._keyword = split[1]
         temp = split[2]
 
-        if not self._board or not self._keyword or not temp:
+        if not self._card or not self._keyword or not temp:
             raise ValueError('invalid OreSat file name')
 
         if '.' in temp:
-            self._date = float(temp.split('.')[0])
+            self._date = float(temp.split('.')[0]) / 1000
             self._extension = temp[temp.find('.'):]
         else:
-            self._date = float(temp)
+            self._date = float(temp) / 1000
             self._extension = ''
 
     def __repr__(self):
 
         return '{} {}'.format(self.__class__.__name__, self._name)
 
     def __str__(self):
@@ -99,29 +103,29 @@
     @property
     def name(self) -> str:
         '''str: The name of the file. Read only.'''
 
         return self._name
 
     @property
-    def board(self) -> str:
-        '''str: The board the file is for or the board the file was made on. Read only.'''
+    def card(self) -> str:
+        '''str: The card the file is for or the card the file was made on. Read only.'''
 
-        return self._board
+        return self._card
 
     @property
     def keyword(self) -> str:
         '''str: The keyword for the file, this can be used to figure out what todo with the
         file. Read only.'''
 
         return self._keyword
 
     @property
     def date(self) -> float:
-        '''float: The Unix time the file was made. Read only.'''
+        '''float: The Unix time the file was made in milliseconds. Read only.'''
 
         return self._date
 
     @property
     def extension(self) -> str:
         '''str: The file extension. Can be an empty string. Read only.'''
```

### Comparing `oresat-olaf-2.1.2/olaf/common/oresat_file_cache.py` & `oresat-olaf-2.2.0/olaf/common/oresat_file_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+'''File cache class for OreSat files.'''
+
 import shutil
 from os import listdir, remove
 from os.path import basename, abspath, isfile
 from pathlib import Path
 from threading import Lock
 from copy import deepcopy
```

### Comparing `oresat-olaf-2.1.2/olaf/common/resource.py` & `oresat-olaf-2.2.0/olaf/common/resource.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-'''The OreSat Linux base app resource'''
+'''The OreSat Linux base app resource. It is a nice way to organize OD callbacks.'''
 
 from loguru import logger
 
 from .._internals.node import Node
 
 
 class Resource:
-    '''OreSat Linux app resource.
+    '''
+    OreSat Linux app resource. Used to setup OD callbacks in a common, isolated environment.
 
     All the ``on_*`` members can be overridden as needed.
     '''
 
     def __init__(self):
 
         self.node = None
```

### Comparing `oresat-olaf-2.1.2/olaf/common/timer_loop.py` & `oresat-olaf-2.2.0/olaf/common/timer_loop.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+'''A quick timer-based class that calls a function in a loop'''
+
 from threading import Thread, Event
 
 from canopen.objectdictionary import Variable
 
 from .. import logger
```

### Comparing `oresat-olaf-2.1.2/olaf/scripts/file_transfer.py` & `oresat-olaf-2.2.0/olaf/scripts/file_transfer.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.2/olaf/scripts/new_eds.py` & `oresat-olaf-2.2.0/olaf/scripts/new_eds.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.2/olaf/scripts/os_command.py` & `oresat-olaf-2.2.0/olaf/scripts/os_command.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.2/olaf/scripts/sdo_transfer.py` & `oresat-olaf-2.2.0/olaf/scripts/sdo_transfer.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.2/olaf/scripts/system_info.py` & `oresat-olaf-2.2.0/olaf/scripts/system_info.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.2/oresat_olaf.egg-info/PKG-INFO` & `oresat-olaf-2.2.0/oresat_olaf.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 Metadata-Version: 2.1
 Name: oresat-olaf
-Version: 2.1.2
+Version: 2.2.0
 Summary: Application framework for all OreSat Linux boards
-Home-page: https://github.com/oresat/oresat-olaf
-Author: PSAS
-Author-email: oresat@pdx.edu
-Maintainer: PSAS
-Maintainer-email: oresat@pdx.edu
 License: GPL-3.0
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 OLAF (OreSat Linux App Framework)
```

### Comparing `oresat-olaf-2.1.2/oresat_olaf.egg-info/SOURCES.txt` & `oresat-olaf-2.2.0/oresat_olaf.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,55 @@
 LICENSE
 README.rst
 pyproject.toml
-setup.cfg
 olaf/__init__.py
 olaf/_internals/__init__.py
 olaf/_internals/app.py
 olaf/_internals/master_node.py
 olaf/_internals/node.py
 olaf/_internals/updater.py
 olaf/_internals/data/oresat_app.eds
 olaf/_internals/resources/__init__.py
+olaf/_internals/resources/daemons.py
 olaf/_internals/resources/ecss.py
 olaf/_internals/resources/file_caches.py
 olaf/_internals/resources/fread.py
 olaf/_internals/resources/fwrite.py
-olaf/_internals/resources/logs.py
-olaf/_internals/resources/os_command.py
 olaf/_internals/resources/power_control.py
 olaf/_internals/resources/store_eds.py
 olaf/_internals/resources/system_info.py
-olaf/_internals/resources/updater.py
 olaf/_internals/rest_api/__init__.py
 olaf/_internals/rest_api/static/favicon.ico
 olaf/_internals/rest_api/templates/base.html
+olaf/_internals/rest_api/templates/daemons.html
 olaf/_internals/rest_api/templates/fread.html
 olaf/_internals/rest_api/templates/fwrite.html
 olaf/_internals/rest_api/templates/logs.html
 olaf/_internals/rest_api/templates/od.html
+olaf/_internals/rest_api/templates/oresat_configs.html
 olaf/_internals/rest_api/templates/os_command.html
 olaf/_internals/rest_api/templates/power_control.html
 olaf/_internals/rest_api/templates/root.html
 olaf/_internals/rest_api/templates/system_info.html
 olaf/_internals/rest_api/templates/updater.html
+olaf/_internals/services/__init__.py
+olaf/_internals/services/logs.py
+olaf/_internals/services/os_command.py
+olaf/_internals/services/updater.py
 olaf/common/__init__.py
+olaf/common/adc.py
 olaf/common/cpufreq.py
+olaf/common/daemon.py
 olaf/common/ecss.py
 olaf/common/gpio.py
 olaf/common/oresat_file.py
 olaf/common/oresat_file_cache.py
+olaf/common/pru.py
 olaf/common/resource.py
+olaf/common/service.py
 olaf/common/timer_loop.py
 olaf/scripts/__init__.py
 olaf/scripts/file_transfer.py
 olaf/scripts/new_eds.py
 olaf/scripts/os_command.py
 olaf/scripts/sdo_transfer.py
 olaf/scripts/sync.py
@@ -54,19 +61,21 @@
 oresat_olaf.egg-info/requires.txt
 oresat_olaf.egg-info/top_level.txt
 tests/__init__.py
 tests/common/__init__.py
 tests/common/test_ecss.py
 tests/common/test_oresat_file.py
 tests/common/test_oresat_file_cache.py
+tests/common/test_pru.py
 tests/common/test_resources.py
 tests/internals/__init__.py
 tests/internals/test_rest_api.py
 tests/internals/resources/__init__.py
 tests/internals/resources/test_ecss.py
 tests/internals/resources/test_file_caches.py
 tests/internals/resources/test_fread.py
 tests/internals/resources/test_fwrite.py
-tests/internals/resources/test_os_command.py
 tests/internals/resources/test_system_info.py
+tests/internals/services/__init__.py
+tests/internals/services/test_os_command.py
 tests/internals/updater/__init__.py
 tests/internals/updater/test_updater.py
```

### Comparing `oresat-olaf-2.1.2/tests/common/test_ecss.py` & `oresat-olaf-2.2.0/tests/common/test_ecss.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.2/tests/common/test_oresat_file.py` & `oresat-olaf-2.2.0/tests/common/test_oresat_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,44 +4,44 @@
 from olaf.common.oresat_file import new_oresat_file, OreSatFile
 
 
 class TestOreSatFile(unittest.TestCase):
     def test_new_oresat_file(self):
 
         file = new_oresat_file('keyword', 'test', 100)
-        self.assertEqual(file, 'test_keyword_100')
+        self.assertEqual(file, 'test_keyword_100000')
 
         file = new_oresat_file('keyword', 'test', 100, 'txt')
-        self.assertEqual(file, 'test_keyword_100.txt')
+        self.assertEqual(file, 'test_keyword_100000.txt')
 
         file = new_oresat_file('keyword', 'test', 100, '.txt')
-        self.assertEqual(file, 'test_keyword_100.txt')
+        self.assertEqual(file, 'test_keyword_100000.txt')
 
         self.assertIsNotNone(new_oresat_file('test'))
 
     def test_oresat_file(self):
 
         name = 'name_test_12345.txt'
         file = OreSatFile(name)
-        self.assertEqual(file.board, 'name')
+        self.assertEqual(file.card, 'name')
         self.assertEqual(file.keyword, 'test')
-        self.assertEqual(file.date, 12345.0)
+        self.assertEqual(file.date, 12.345)
         self.assertEqual(file.extension, '.txt')
         self.assertEqual(file.name, name)
 
         name = 'name_test_12345.tar.xz'
         file = OreSatFile(name)
-        self.assertEqual(file.date, 12345.0)
+        self.assertEqual(file.date, 12.345)
         self.assertEqual(file.extension, '.tar.xz')
 
         name = '/this/is/test/name_test_123'
         file = OreSatFile(name)
-        self.assertEqual(file.board, 'name')
+        self.assertEqual(file.card, 'name')
         self.assertEqual(file.keyword, 'test')
-        self.assertEqual(file.date, 123.0)
+        self.assertEqual(file.date, 0.123)
         self.assertEqual(file.extension, '')
         self.assertEqual(file.name, os.path.basename(name))
 
         with self.assertRaises(ValueError):
             OreSatFile('nametest12345')
 
         with self.assertRaises(ValueError):
```

### Comparing `oresat-olaf-2.1.2/tests/common/test_oresat_file_cache.py` & `oresat-olaf-2.2.0/tests/common/test_oresat_file_cache.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.2/tests/common/test_resources.py` & `oresat-olaf-2.2.0/tests/common/test_resources.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.2/tests/internals/resources/__init__.py` & `oresat-olaf-2.2.0/tests/internals/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.2/tests/internals/resources/test_file_caches.py` & `oresat-olaf-2.2.0/tests/internals/resources/test_file_caches.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.2/tests/internals/resources/test_fread.py` & `oresat-olaf-2.2.0/tests/internals/resources/test_fwrite.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,77 @@
+import json
 import random
 import string
 import unittest
+from os import remove
 from os.path import basename
 
 from olaf import new_oresat_file
-from olaf._internals.resources.fread import FreadResource, Subindex
+from olaf._internals.resources.fwrite import FwriteResource, Subindex
 
 from . import MockApp
 
 
-class TestFreadResource(unittest.TestCase):
+class TestFwriteResource(unittest.TestCase):
 
     def setUp(self):
 
         self.app = MockApp()
-        self.app.add_resource(FreadResource())
+        self.app.add_resource(FwriteResource())
         self.app.start()
 
     def tearDown(self):
 
         self.app.stop()
 
-    def test_read(self):
+    def test_write(self):
 
         index = self.app.resource.index
 
-        self.assertEqual(len(self.app.node.fread_cache), 0)
-
-        # empty cache
-        self.assertIn(self.app.sdo_read(index, Subindex.FILE_NAME.value), ['', 'x'])
-        self.assertEqual(self.app.sdo_read(index, Subindex.FILE_DATA.value), b'')
-        self.app.sdo_write(index, Subindex.DELETE_FILE.value, True)
-
-        # test sdo trasfer of a file that does not exist
-        file_name = new_oresat_file('test')
-        self.app.sdo_write(index, Subindex.FILE_NAME.value, file_name)
-        self.app.sdo_write(index, Subindex.FILE_NAME.value, new_oresat_file('abc'))
-        self.assertEqual(self.app.sdo_read(index, Subindex.FILE_NAME.value), '')
-        self.assertEqual(self.app.sdo_read(index, Subindex.FILE_DATA.value), b'')
+        self.assertEqual(len(self.app.node.fwrite_cache), 0)
 
         # add a file to the cache
         file_name = new_oresat_file('test')
         file_path = '/tmp/' + file_name
         file_data = ''.join(random.choice(string.ascii_letters) for i in range(100))
         with open(file_path, 'w') as f:
             f.write(file_data)
-        self.app.node.fread_cache.add(file_path, True)
-        self.assertEqual(len(self.app.node.fread_cache), 1)
 
         # test sdo trasfer of a file
         self.app.sdo_write(index, Subindex.FILE_NAME.value, basename(file_name))
         self.assertEqual(self.app.sdo_read(index, Subindex.FILE_NAME.value), file_name)
-        self.assertEqual(self.app.sdo_read(index, Subindex.FILE_DATA.value).decode(), file_data)
-        self.app.sdo_write(index, Subindex.DELETE_FILE.value, True)
-        self.assertEqual(len(self.app.node.fread_cache), 0)
+        self.app.sdo_write(index, Subindex.FILE_DATA.value, file_data.encode())
+        self.assertEqual(len(self.app.node.fwrite_cache), 1)
+        self.assertEqual(self.app.sdo_read(index, Subindex.TOTAL_FILES.value), 1)
+        file_names = json.loads(self.app.sdo_read(index, Subindex.FILE_NAMES.value))
+        self.assertListEqual(file_names, [file_name])
+
+        # test sdo trasfer of a file to over write
+        self.app.sdo_write(index, Subindex.FILE_NAME.value, basename(file_name))
+        self.assertEqual(self.app.sdo_read(index, Subindex.FILE_NAME.value), file_name)
+        self.app.sdo_write(index, Subindex.FILE_DATA.value, file_data.encode())
+        self.assertEqual(len(self.app.node.fwrite_cache), 1)
+        self.assertEqual(self.app.sdo_read(index, Subindex.TOTAL_FILES.value), 1)
+        file_names = json.loads(self.app.sdo_read(index, Subindex.FILE_NAMES.value))
+        self.assertListEqual(file_names, [file_name])
+
+        # remove test file
+        remove(file_path)
+
+        # add another file to the cache
+        file_name2 = new_oresat_file('test2')
+        file_path2 = '/tmp/' + file_name2
+        file_data2 = ''.join(random.choice(string.ascii_letters) for i in range(100))
+        with open(file_path2, 'w') as f:
+            f.write(file_data2)
+
+        # test sdo trasfer of a file
+        self.app.sdo_write(index, Subindex.FILE_NAME.value, basename(file_name2))
+        self.assertEqual(self.app.sdo_read(index, Subindex.FILE_NAME.value), file_name2)
+        self.app.sdo_write(index, Subindex.FILE_DATA.value, file_data2.encode())
+        self.assertEqual(len(self.app.node.fwrite_cache), 2)
+        self.assertEqual(self.app.sdo_read(index, Subindex.TOTAL_FILES.value), 2)
+        file_names = json.loads(self.app.sdo_read(index, Subindex.FILE_NAMES.value))
+        self.assertListEqual(file_names, [file_name, file_name2])
+
+        # remove test file
+        remove(file_path2)
```

### Comparing `oresat-olaf-2.1.2/tests/internals/resources/test_os_command.py` & `oresat-olaf-2.2.0/tests/internals/services/test_os_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import unittest
 from time import sleep
 
-from olaf._internals.resources.os_command import OSCommandState, OSCommandResource
+from olaf._internals.services.os_command import OSCommandState, OSCommandService
 
 from . import MockApp
 
 
 class TestOSCommand(unittest.TestCase):
 
     def setUp(self):
 
         self.app = MockApp()
-        self.app.add_resource(OSCommandResource())
+        self.app.add_service(OSCommandService())
         self.app.start()
-        self.index = self.app.resource.index
+        self.index = self.app.service.index
 
     def tearDown(self):
 
         self.app.stop()
 
     def run_os_command(self, command: str):
         '''send os command add give some time to run it'''
```

### Comparing `oresat-olaf-2.1.2/tests/internals/resources/test_system_info.py` & `oresat-olaf-2.2.0/tests/internals/resources/test_system_info.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.2/tests/internals/test_rest_api.py` & `oresat-olaf-2.2.0/tests/internals/test_rest_api.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.1.2/tests/internals/updater/test_updater.py` & `oresat-olaf-2.2.0/tests/internals/updater/test_updater.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,40 +36,40 @@
         self.assertFalse(is_update_archive('star-tracker_capture_12346789.tar.xz'))
 
     def test_updater_default(self):
         updater = Updater(self._work_dir, self._cache_dir)
 
         # properties defaults
         self.assertEqual(updater.status, UpdaterState.UPDATE_SUCCESSFUL)
-        self.assertEqual(updater.updates_cached, 0)
+        self.assertEqual(updater.updates_cached, [])
         self.assertEqual(updater.list_updates, '[]')
         self.assertEqual(updater.update_archive, '')
         self.assertEqual(updater.total_instructions, 0)
         self.assertEqual(updater.instruction_index, 0)
         self.assertEqual(updater.instruction_percent, 0)
         self.assertEqual(updater.instruction_command, '')
 
     def test_add_update_archive(self):
         updater = Updater(self._work_dir, self._cache_dir)
-        updates_cached = updater.updates_cached
+        updates_cached = len(updater.updates_cached)
 
         self.assertFalse(updater.add_update_archive('invalid-file-path'))
-        self.assertEqual(updater.updates_cached, updates_cached)
+        self.assertEqual(len(updater.updates_cached), updates_cached)
 
         self.assertTrue(updater.add_update_archive(PATH + '/test_update_1611940000.tar.xz'))
-        self.assertEqual(updater.updates_cached, updates_cached + 1)
+        self.assertEqual(len(updater.updates_cached), updates_cached + 1)
 
         self.assertTrue(updater.add_update_archive(PATH + '/test_update_1611941111.tar.xz'))
-        self.assertEqual(updater.updates_cached, updates_cached + 2)
+        self.assertEqual(len(updater.updates_cached), updates_cached + 2)
 
         # add the same file (should override)
         self.assertTrue(updater.add_update_archive(PATH + '/test_update_1611942222.tar.xz'))
         self.assertTrue(updater.add_update_archive(PATH + '/test_update_1611942222.tar.xz'))
         self.assertTrue(updater.add_update_archive(PATH + '/test_update_1611942222.tar.xz'))
-        self.assertEqual(updater.updates_cached, updates_cached + 3)
+        self.assertEqual(len(updater.updates_cached), updates_cached + 3)
 
     @unittest.skipUnless(isfile('/usr/bin/dpkg'), 'requires dpkg')
     def test_make_status_file(self):
         updater = Updater(self._work_dir, self._cache_dir)
 
         status_archive = updater.make_status_archive()
         self.assertTrue(isfile(status_archive))
```

