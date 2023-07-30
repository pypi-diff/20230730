# Comparing `tmp/potnanny-0.1.1.tar.gz` & `tmp/potnanny-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "potnanny-0.1.1.tar", last modified: Fri Jul 28 04:15:14 2023, max compression
+gzip compressed data, was "potnanny-0.1.2.tar", last modified: Sun Jul 30 08:14:31 2023, max compression
```

## Comparing `potnanny-0.1.1.tar` & `potnanny-0.1.2.tar`

### file list

```diff
@@ -1,122 +1,136 @@
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-28 04:15:14.364264 potnanny-0.1.1/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)    35113 2023-07-27 13:31:05.000000 potnanny-0.1.1/LICENSE
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3215 2023-07-28 04:15:14.364264 potnanny-0.1.1/PKG-INFO
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2926 2023-07-27 13:31:05.000000 potnanny-0.1.1/README.md
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-28 04:15:14.344264 potnanny-0.1.1/potnanny/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/__init__.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-28 04:15:14.348264 potnanny-0.1.1/potnanny/api/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2675 2023-07-28 04:13:01.000000 potnanny-0.1.1/potnanny/api/__init__.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2565 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/api/actions.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2947 2023-07-28 04:14:36.000000 potnanny-0.1.1/potnanny/api/auth.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2576 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/api/controls.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      488 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/api/decorators.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     5969 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/api/devices.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      954 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/api/environments.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      173 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/api/index.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2712 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/api/keychains.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1449 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/api/plugins.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2852 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/api/rooms.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3113 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/api/schedules.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1874 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/api/settings.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      695 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/api/tests.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2423 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/api/users.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1449 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/api/utils.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1095 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/api/wifi.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1879 2023-07-28 04:12:22.000000 potnanny-0.1.1/potnanny/app.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3014 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/cli.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3239 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/config.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-28 04:15:14.352264 potnanny-0.1.1/potnanny/controllers/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/controllers/__init__.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      724 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/controllers/cleanup.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      574 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/controllers/device.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     4240 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/controllers/discover.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3401 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/controllers/environment.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3401 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/controllers/environment_orig.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3468 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/controllers/graph.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     4693 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/controllers/outlet.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      843 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/controllers/pipeline.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-28 04:15:14.352264 potnanny-0.1.1/potnanny/controllers/poll/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)       45 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/controllers/poll/__init__.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     5135 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/controllers/poll/ble.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1532 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/controllers/poll/gpio.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2479 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/controllers/poll/parse.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1904 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/controllers/poll/poll.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      706 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/controllers/schedule.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      849 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/controllers/trigger.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3342 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/controllers/worker.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3043 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/database.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)       73 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/events.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)       83 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/exc.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      662 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/locks.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-28 04:15:14.356264 potnanny-0.1.1/potnanny/models/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/models/__init__.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3722 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/models/action.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     4055 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/models/control.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     5689 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/models/device.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1242 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/models/error.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1309 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/models/ext.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3362 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/models/interface.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1372 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/models/keychain.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1253 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/models/measurement.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1354 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/models/mixins.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1693 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/models/room.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3838 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/models/schedule.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      942 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/models/trigger.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1830 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/models/user.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1157 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/models/weekday.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-28 04:15:14.356264 potnanny-0.1.1/potnanny/plugins/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      320 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/plugins/__init__.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      906 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/plugins/base.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      267 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/plugins/category.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     4290 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/plugins/mixins.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-28 04:15:14.360264 potnanny-0.1.1/potnanny/utils/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      940 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/utils/__init__.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      887 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/utils/eval.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      332 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/utils/lists.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      798 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/utils/network.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      371 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/utils/numbers.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      227 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/utils/paths.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1263 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/utils/pids.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1285 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/utils/plugins.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      363 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/utils/pw.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2206 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/utils/scanner.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      343 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/utils/serial.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      409 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/utils/shell.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      299 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/utils/temperature.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2094 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/utils/times.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      822 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/utils/vpd.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     5323 2023-07-27 13:31:05.000000 potnanny-0.1.1/potnanny/utils/wifi.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-28 04:15:14.344264 potnanny-0.1.1/potnanny.egg-info/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3215 2023-07-28 04:15:14.000000 potnanny-0.1.1/potnanny.egg-info/PKG-INFO
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2873 2023-07-28 04:15:14.000000 potnanny-0.1.1/potnanny.egg-info/SOURCES.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        1 2023-07-28 04:15:14.000000 potnanny-0.1.1/potnanny.egg-info/dependency_links.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)       47 2023-07-28 04:15:14.000000 potnanny-0.1.1/potnanny.egg-info/entry_points.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      305 2023-07-28 04:15:14.000000 potnanny-0.1.1/potnanny.egg-info/requires.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        9 2023-07-28 04:15:14.000000 potnanny-0.1.1/potnanny.egg-info/top_level.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)       38 2023-07-28 04:15:14.364264 potnanny-0.1.1/setup.cfg
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1243 2023-07-28 04:11:39.000000 potnanny-0.1.1/setup.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-28 04:15:14.364264 potnanny-0.1.1/tests/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2721 2023-07-27 13:31:05.000000 potnanny-0.1.1/tests/test_ctrl_environments.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1431 2023-07-27 13:31:05.000000 potnanny-0.1.1/tests/test_ctrl_outlet.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      690 2023-07-27 13:31:05.000000 potnanny-0.1.1/tests/test_locks.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3649 2023-07-27 13:31:05.000000 potnanny-0.1.1/tests/test_model_action.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1197 2023-07-27 13:31:05.000000 potnanny-0.1.1/tests/test_model_control.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1181 2023-07-27 13:31:05.000000 potnanny-0.1.1/tests/test_model_device.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1813 2023-07-27 13:31:05.000000 potnanny-0.1.1/tests/test_model_interface.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     2190 2023-07-27 13:31:05.000000 potnanny-0.1.1/tests/test_model_keychain.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      792 2023-07-27 13:31:05.000000 potnanny-0.1.1/tests/test_model_measurement.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      720 2023-07-27 13:31:05.000000 potnanny-0.1.1/tests/test_model_mixins.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1632 2023-07-27 13:31:05.000000 potnanny-0.1.1/tests/test_model_room.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1736 2023-07-27 13:31:05.000000 potnanny-0.1.1/tests/test_model_user.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      947 2023-07-27 13:31:05.000000 potnanny-0.1.1/tests/test_model_utils.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      767 2023-07-27 13:31:05.000000 potnanny-0.1.1/tests/test_pids.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3138 2023-07-27 13:31:05.000000 potnanny-0.1.1/tests/test_queries.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      544 2023-07-27 13:31:05.000000 potnanny-0.1.1/tests/test_scanner.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      808 2023-07-27 13:31:05.000000 potnanny-0.1.1/tests/test_utils_eval.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      369 2023-07-27 13:31:05.000000 potnanny-0.1.1/tests/test_utils_lists.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      455 2023-07-27 13:31:05.000000 potnanny-0.1.1/tests/test_utils_numbers.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      333 2023-07-27 13:31:05.000000 potnanny-0.1.1/tests/test_utils_paths.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      428 2023-07-27 13:31:05.000000 potnanny-0.1.1/tests/test_utils_pw.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      450 2023-07-27 13:31:05.000000 potnanny-0.1.1/tests/test_utils_temperature.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      816 2023-07-27 13:31:05.000000 potnanny-0.1.1/tests/test_utils_times.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      326 2023-07-27 13:31:05.000000 potnanny-0.1.1/tests/test_utils_vpd.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-30 08:14:31.336602 potnanny-0.1.2/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)    35113 2023-07-28 04:26:10.000000 potnanny-0.1.2/LICENSE
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       83 2023-07-30 08:13:55.000000 potnanny-0.1.2/MANIFEST.in
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3215 2023-07-30 08:14:31.332602 potnanny-0.1.2/PKG-INFO
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2926 2023-07-28 04:26:10.000000 potnanny-0.1.2/README.md
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-30 08:14:31.308602 potnanny-0.1.2/potnanny/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/__init__.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-30 08:14:31.312602 potnanny-0.1.2/potnanny/api/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2675 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/api/__init__.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2565 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/api/actions.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2947 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/api/auth.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2576 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/api/controls.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      488 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/api/decorators.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     5969 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/api/devices.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      954 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/api/environments.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      173 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/api/index.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2712 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/api/keychains.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1449 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/api/plugins.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2852 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/api/rooms.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3113 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/api/schedules.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1874 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/api/settings.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-30 08:14:31.304602 potnanny-0.1.2/potnanny/api/static/
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-30 08:14:31.312602 potnanny-0.1.2/potnanny/api/static/css/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)    95609 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/api/static/css/bootstrap-icons.css
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)   155845 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/api/static/css/bootstrap.min.css
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-30 08:14:31.312602 potnanny-0.1.2/potnanny/api/static/css/fonts/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)   121296 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/api/static/css/fonts/bootstrap-icons.woff2
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-30 08:14:31.312602 potnanny-0.1.2/potnanny/api/static/htdocs/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2948 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/api/static/htdocs/index.html
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-30 08:14:31.316602 potnanny-0.1.2/potnanny/api/static/js/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)   456323 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/api/static/js/app.js
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)    78743 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/api/static/js/bootstrap.bundle.min.js
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-30 08:14:31.316602 potnanny-0.1.2/potnanny/api/templates/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3002 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/api/templates/index.html
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      695 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/api/tests.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2423 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/api/users.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1449 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/api/utils.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1095 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/api/wifi.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1879 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/app.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3014 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/cli.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3239 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/config.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-30 08:14:31.320602 potnanny-0.1.2/potnanny/controllers/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/controllers/__init__.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      724 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/controllers/cleanup.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      574 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/controllers/device.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     4240 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/controllers/discover.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3401 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/controllers/environment.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3401 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/controllers/environment_orig.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3468 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/controllers/graph.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     4693 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/controllers/outlet.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      843 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/controllers/pipeline.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-30 08:14:31.320602 potnanny-0.1.2/potnanny/controllers/poll/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       45 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/controllers/poll/__init__.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     5135 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/controllers/poll/ble.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1532 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/controllers/poll/gpio.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2479 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/controllers/poll/parse.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1904 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/controllers/poll/poll.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      706 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/controllers/schedule.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      849 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/controllers/trigger.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3342 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/controllers/worker.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3043 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/database.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       73 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/events.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       83 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/exc.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      662 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/locks.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-30 08:14:31.324602 potnanny-0.1.2/potnanny/models/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/models/__init__.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3722 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/models/action.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     4055 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/models/control.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     5689 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/models/device.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1242 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/models/error.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1309 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/models/ext.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3362 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/models/interface.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1372 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/models/keychain.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1253 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/models/measurement.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1354 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/models/mixins.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1693 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/models/room.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3838 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/models/schedule.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      942 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/models/trigger.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1830 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/models/user.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1157 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/models/weekday.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-30 08:14:31.324602 potnanny-0.1.2/potnanny/plugins/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      320 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/plugins/__init__.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      906 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/plugins/base.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      267 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/plugins/category.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     4290 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/plugins/mixins.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-30 08:14:31.328602 potnanny-0.1.2/potnanny/utils/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      940 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/utils/__init__.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      887 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/utils/eval.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      332 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/utils/lists.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      798 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/utils/network.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      371 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/utils/numbers.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      227 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/utils/paths.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1263 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/utils/pids.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1285 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/utils/plugins.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      363 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/utils/pw.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2206 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/utils/scanner.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      343 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/utils/serial.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      409 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/utils/shell.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      299 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/utils/temperature.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2094 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/utils/times.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      822 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/utils/vpd.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     5323 2023-07-28 04:26:10.000000 potnanny-0.1.2/potnanny/utils/wifi.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-30 08:14:31.308602 potnanny-0.1.2/potnanny.egg-info/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3215 2023-07-30 08:14:31.000000 potnanny-0.1.2/potnanny.egg-info/PKG-INFO
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3172 2023-07-30 08:14:31.000000 potnanny-0.1.2/potnanny.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        1 2023-07-30 08:14:31.000000 potnanny-0.1.2/potnanny.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       47 2023-07-30 08:14:31.000000 potnanny-0.1.2/potnanny.egg-info/entry_points.txt
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      305 2023-07-30 08:14:31.000000 potnanny-0.1.2/potnanny.egg-info/requires.txt
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        9 2023-07-30 08:14:31.000000 potnanny-0.1.2/potnanny.egg-info/top_level.txt
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       38 2023-07-30 08:14:31.336602 potnanny-0.1.2/setup.cfg
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1243 2023-07-30 08:08:26.000000 potnanny-0.1.2/setup.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-07-30 08:14:31.332602 potnanny-0.1.2/tests/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2721 2023-07-28 04:26:10.000000 potnanny-0.1.2/tests/test_ctrl_environments.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1431 2023-07-28 04:26:10.000000 potnanny-0.1.2/tests/test_ctrl_outlet.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      690 2023-07-28 04:26:10.000000 potnanny-0.1.2/tests/test_locks.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3649 2023-07-28 04:26:10.000000 potnanny-0.1.2/tests/test_model_action.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1197 2023-07-28 04:26:10.000000 potnanny-0.1.2/tests/test_model_control.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1181 2023-07-28 04:26:10.000000 potnanny-0.1.2/tests/test_model_device.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1813 2023-07-28 04:26:10.000000 potnanny-0.1.2/tests/test_model_interface.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     2190 2023-07-28 04:26:10.000000 potnanny-0.1.2/tests/test_model_keychain.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      792 2023-07-28 04:26:10.000000 potnanny-0.1.2/tests/test_model_measurement.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      720 2023-07-28 04:26:10.000000 potnanny-0.1.2/tests/test_model_mixins.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1632 2023-07-28 04:26:10.000000 potnanny-0.1.2/tests/test_model_room.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1736 2023-07-28 04:26:10.000000 potnanny-0.1.2/tests/test_model_user.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      947 2023-07-28 04:26:10.000000 potnanny-0.1.2/tests/test_model_utils.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      767 2023-07-28 04:26:10.000000 potnanny-0.1.2/tests/test_pids.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3138 2023-07-28 04:26:10.000000 potnanny-0.1.2/tests/test_queries.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      544 2023-07-28 04:26:10.000000 potnanny-0.1.2/tests/test_scanner.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      808 2023-07-28 04:26:10.000000 potnanny-0.1.2/tests/test_utils_eval.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      369 2023-07-28 04:26:10.000000 potnanny-0.1.2/tests/test_utils_lists.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      455 2023-07-28 04:26:10.000000 potnanny-0.1.2/tests/test_utils_numbers.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      333 2023-07-28 04:26:10.000000 potnanny-0.1.2/tests/test_utils_paths.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      428 2023-07-28 04:26:10.000000 potnanny-0.1.2/tests/test_utils_pw.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      450 2023-07-28 04:26:10.000000 potnanny-0.1.2/tests/test_utils_temperature.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      816 2023-07-28 04:26:10.000000 potnanny-0.1.2/tests/test_utils_times.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      326 2023-07-28 04:26:10.000000 potnanny-0.1.2/tests/test_utils_vpd.py
```

### Comparing `potnanny-0.1.1/LICENSE` & `potnanny-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/PKG-INFO` & `potnanny-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: potnanny
-Version: 0.1.1
+Version: 0.1.2
 Summary: Potnanny grow room automation controller.
 Home-page: https://github.com/potnanny/application
 Author: J Leary
 Author-email: potnanny@gmail.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `potnanny-0.1.1/README.md` & `potnanny-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/api/__init__.py` & `potnanny-0.1.2/potnanny/api/__init__.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/api/actions.py` & `potnanny-0.1.2/potnanny/api/actions.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/api/auth.py` & `potnanny-0.1.2/potnanny/api/auth.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/api/controls.py` & `potnanny-0.1.2/potnanny/api/controls.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/api/devices.py` & `potnanny-0.1.2/potnanny/api/devices.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/api/environments.py` & `potnanny-0.1.2/potnanny/api/environments.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/api/keychains.py` & `potnanny-0.1.2/potnanny/api/keychains.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/api/plugins.py` & `potnanny-0.1.2/potnanny/api/plugins.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/api/rooms.py` & `potnanny-0.1.2/potnanny/api/rooms.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/api/schedules.py` & `potnanny-0.1.2/potnanny/api/schedules.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/api/settings.py` & `potnanny-0.1.2/potnanny/api/settings.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/api/tests.py` & `potnanny-0.1.2/potnanny/api/tests.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/api/users.py` & `potnanny-0.1.2/potnanny/api/users.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/api/utils.py` & `potnanny-0.1.2/potnanny/api/utils.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/api/wifi.py` & `potnanny-0.1.2/potnanny/api/wifi.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/app.py` & `potnanny-0.1.2/potnanny/app.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/cli.py` & `potnanny-0.1.2/potnanny/cli.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/config.py` & `potnanny-0.1.2/potnanny/config.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/controllers/cleanup.py` & `potnanny-0.1.2/potnanny/controllers/cleanup.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/controllers/device.py` & `potnanny-0.1.2/potnanny/controllers/device.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/controllers/discover.py` & `potnanny-0.1.2/potnanny/controllers/discover.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/controllers/environment.py` & `potnanny-0.1.2/potnanny/controllers/environment.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/controllers/environment_orig.py` & `potnanny-0.1.2/potnanny/controllers/environment_orig.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/controllers/graph.py` & `potnanny-0.1.2/potnanny/controllers/graph.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/controllers/outlet.py` & `potnanny-0.1.2/potnanny/controllers/outlet.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/controllers/pipeline.py` & `potnanny-0.1.2/potnanny/controllers/pipeline.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/controllers/poll/ble.py` & `potnanny-0.1.2/potnanny/controllers/poll/ble.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/controllers/poll/gpio.py` & `potnanny-0.1.2/potnanny/controllers/poll/gpio.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/controllers/poll/parse.py` & `potnanny-0.1.2/potnanny/controllers/poll/parse.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/controllers/poll/poll.py` & `potnanny-0.1.2/potnanny/controllers/poll/poll.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/controllers/schedule.py` & `potnanny-0.1.2/potnanny/controllers/schedule.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/controllers/trigger.py` & `potnanny-0.1.2/potnanny/controllers/trigger.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/controllers/worker.py` & `potnanny-0.1.2/potnanny/controllers/worker.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/database.py` & `potnanny-0.1.2/potnanny/database.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/locks.py` & `potnanny-0.1.2/potnanny/locks.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/models/action.py` & `potnanny-0.1.2/potnanny/models/action.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/models/control.py` & `potnanny-0.1.2/potnanny/models/control.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/models/device.py` & `potnanny-0.1.2/potnanny/models/device.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/models/error.py` & `potnanny-0.1.2/potnanny/models/error.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/models/ext.py` & `potnanny-0.1.2/potnanny/models/ext.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/models/interface.py` & `potnanny-0.1.2/potnanny/models/interface.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/models/keychain.py` & `potnanny-0.1.2/potnanny/models/keychain.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/models/measurement.py` & `potnanny-0.1.2/potnanny/models/measurement.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/models/mixins.py` & `potnanny-0.1.2/potnanny/models/mixins.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/models/room.py` & `potnanny-0.1.2/potnanny/models/room.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/models/schedule.py` & `potnanny-0.1.2/potnanny/models/schedule.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/models/trigger.py` & `potnanny-0.1.2/potnanny/models/trigger.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/models/user.py` & `potnanny-0.1.2/potnanny/models/user.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/models/weekday.py` & `potnanny-0.1.2/potnanny/models/weekday.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/plugins/base.py` & `potnanny-0.1.2/potnanny/plugins/base.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/plugins/mixins.py` & `potnanny-0.1.2/potnanny/plugins/mixins.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/utils/__init__.py` & `potnanny-0.1.2/potnanny/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/utils/eval.py` & `potnanny-0.1.2/potnanny/utils/eval.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/utils/network.py` & `potnanny-0.1.2/potnanny/utils/network.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/utils/pids.py` & `potnanny-0.1.2/potnanny/utils/pids.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/utils/plugins.py` & `potnanny-0.1.2/potnanny/utils/plugins.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/utils/scanner.py` & `potnanny-0.1.2/potnanny/utils/scanner.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/utils/times.py` & `potnanny-0.1.2/potnanny/utils/times.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/utils/vpd.py` & `potnanny-0.1.2/potnanny/utils/vpd.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny/utils/wifi.py` & `potnanny-0.1.2/potnanny/utils/wifi.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/potnanny.egg-info/PKG-INFO` & `potnanny-0.1.2/potnanny.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: potnanny
-Version: 0.1.1
+Version: 0.1.2
 Summary: Potnanny grow room automation controller.
 Home-page: https://github.com/potnanny/application
 Author: J Leary
 Author-email: potnanny@gmail.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `potnanny-0.1.1/potnanny.egg-info/SOURCES.txt` & `potnanny-0.1.2/potnanny.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+MANIFEST.in
 README.md
 setup.py
 potnanny/__init__.py
 potnanny/app.py
 potnanny/cli.py
 potnanny/config.py
 potnanny/database.py
@@ -28,14 +29,21 @@
 potnanny/api/rooms.py
 potnanny/api/schedules.py
 potnanny/api/settings.py
 potnanny/api/tests.py
 potnanny/api/users.py
 potnanny/api/utils.py
 potnanny/api/wifi.py
+potnanny/api/static/css/bootstrap-icons.css
+potnanny/api/static/css/bootstrap.min.css
+potnanny/api/static/css/fonts/bootstrap-icons.woff2
+potnanny/api/static/htdocs/index.html
+potnanny/api/static/js/app.js
+potnanny/api/static/js/bootstrap.bundle.min.js
+potnanny/api/templates/index.html
 potnanny/controllers/__init__.py
 potnanny/controllers/cleanup.py
 potnanny/controllers/device.py
 potnanny/controllers/discover.py
 potnanny/controllers/environment.py
 potnanny/controllers/environment_orig.py
 potnanny/controllers/graph.py
```

### Comparing `potnanny-0.1.1/setup.py` & `potnanny-0.1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='potnanny',
-    version='0.1.1',
+    version='0.1.2',
     python_requires=">=3.9",
     packages=setuptools.find_packages(),
     include_package_data=True,
     description='Potnanny grow room automation controller.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='J Leary',
```

### Comparing `potnanny-0.1.1/tests/test_ctrl_environments.py` & `potnanny-0.1.2/tests/test_ctrl_environments.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/tests/test_ctrl_outlet.py` & `potnanny-0.1.2/tests/test_ctrl_outlet.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/tests/test_locks.py` & `potnanny-0.1.2/tests/test_locks.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/tests/test_model_action.py` & `potnanny-0.1.2/tests/test_model_action.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/tests/test_model_control.py` & `potnanny-0.1.2/tests/test_model_control.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/tests/test_model_device.py` & `potnanny-0.1.2/tests/test_model_device.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/tests/test_model_interface.py` & `potnanny-0.1.2/tests/test_model_interface.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/tests/test_model_keychain.py` & `potnanny-0.1.2/tests/test_model_keychain.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/tests/test_model_measurement.py` & `potnanny-0.1.2/tests/test_model_measurement.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/tests/test_model_mixins.py` & `potnanny-0.1.2/tests/test_model_mixins.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/tests/test_model_room.py` & `potnanny-0.1.2/tests/test_model_room.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/tests/test_model_user.py` & `potnanny-0.1.2/tests/test_model_user.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/tests/test_model_utils.py` & `potnanny-0.1.2/tests/test_model_utils.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/tests/test_pids.py` & `potnanny-0.1.2/tests/test_pids.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/tests/test_queries.py` & `potnanny-0.1.2/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/tests/test_scanner.py` & `potnanny-0.1.2/tests/test_scanner.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/tests/test_utils_eval.py` & `potnanny-0.1.2/tests/test_utils_eval.py`

 * *Files identical despite different names*

### Comparing `potnanny-0.1.1/tests/test_utils_times.py` & `potnanny-0.1.2/tests/test_utils_times.py`

 * *Files identical despite different names*

