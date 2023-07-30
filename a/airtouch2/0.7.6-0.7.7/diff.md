# Comparing `tmp/airtouch2-0.7.6.tar.gz` & `tmp/airtouch2-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airtouch2-0.7.6.tar", last modified: Sat Jul 15 03:49:24 2023, max compression
+gzip compressed data, was "airtouch2-0.7.7.tar", last modified: Sun Jul 30 09:24:42 2023, max compression
```

## Comparing `airtouch2-0.7.6.tar` & `airtouch2-0.7.7.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-15 03:49:24.555294 airtouch2-0.7.6/
--rw-r--r--   0 nathan    (1000) nathan    (1000)     1076 2023-01-10 07:31:33.000000 airtouch2-0.7.6/LICENSE
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2281 2023-07-15 03:49:24.555294 airtouch2-0.7.6/PKG-INFO
--rw-r--r--   0 nathan    (1000) nathan    (1000)      271 2023-01-10 07:31:33.000000 airtouch2-0.7.6/README.md
--rw-r--r--   0 nathan    (1000) nathan    (1000)      852 2023-07-15 03:47:27.000000 airtouch2-0.7.6/pyproject.toml
--rw-r--r--   0 nathan    (1000) nathan    (1000)       38 2023-07-15 03:49:24.555294 airtouch2-0.7.6/setup.cfg
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-15 03:49:24.551294 airtouch2-0.7.6/src/
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-15 03:49:24.551294 airtouch2-0.7.6/src/airtouch2/
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-15 03:49:24.551294 airtouch2-0.7.6/src/airtouch2/at2/
--rw-r--r--   0 nathan    (1000) nathan    (1000)     5511 2023-06-28 10:35:59.000000 airtouch2-0.7.6/src/airtouch2/at2/At2Aircon.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     3515 2023-07-15 03:40:22.000000 airtouch2-0.7.6/src/airtouch2/at2/At2Client.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     3301 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/at2/At2Group.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      204 2023-07-10 10:42:42.000000 airtouch2-0.7.6/src/airtouch2/at2/__init__.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-15 03:49:24.551294 airtouch2-0.7.6/src/airtouch2/at2plus/
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2789 2023-07-15 03:31:26.000000 airtouch2-0.7.6/src/airtouch2/at2plus/At2PlusAircon.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     8423 2023-07-15 03:40:27.000000 airtouch2-0.7.6/src/airtouch2/at2plus/At2PlusClient.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      190 2023-07-10 11:17:26.000000 airtouch2-0.7.6/src/airtouch2/at2plus/__init__.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-15 03:49:24.551294 airtouch2-0.7.6/src/airtouch2/common/
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2457 2023-07-11 11:20:25.000000 airtouch2-0.7.6/src/airtouch2/common/Buffer.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     4810 2023-07-15 03:40:27.000000 airtouch2-0.7.6/src/airtouch2/common/NetClient.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/common/__init__.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      428 2023-07-09 02:16:01.000000 airtouch2-0.7.6/src/airtouch2/common/interfaces.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-15 03:49:24.551294 airtouch2-0.7.6/src/airtouch2/helpers/
--rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/helpers/__init__.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      541 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/helpers/diff_bytes.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-15 03:49:24.551294 airtouch2-0.7.6/src/airtouch2/protocol/
--rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-03-19 07:06:23.000000 airtouch2-0.7.6/src/airtouch2/protocol/__init__.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-15 03:49:24.551294 airtouch2-0.7.6/src/airtouch2/protocol/at2/
--rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2/__init__.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2584 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2/constants.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2773 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2/conversions.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      647 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2/enums.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      865 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2/lookups.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      308 2023-07-11 11:17:00.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2/message_common.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-15 03:49:24.551294 airtouch2-0.7.6/src/airtouch2/protocol/at2/messages/
--rw-r--r--   0 nathan    (1000) nathan    (1000)      849 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2/messages/RequestState.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     5046 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2/messages/ResponseMessage.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      339 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2/messages/__init__.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2861 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2/messages/ac_commands.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     1867 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2/messages/group_commands.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-15 03:49:24.555294 airtouch2-0.7.6/src/airtouch2/protocol/at2plus/
--rw-r--r--   0 nathan    (1000) nathan    (1000)      148 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2plus/constants.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2768 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2plus/control_status_common.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     1128 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2plus/conversions.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2359 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2plus/crc16_modbus.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     1560 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2plus/enums.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     1113 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2plus/extended_common.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     3942 2023-07-11 11:17:00.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2plus/message_common.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-15 03:49:24.555294 airtouch2-0.7.6/src/airtouch2/protocol/at2plus/messages/
--rw-r--r--   0 nathan    (1000) nathan    (1000)     6156 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2plus/messages/AcAbilityMessage.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     3167 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2plus/messages/AcControl.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     4119 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2plus/messages/AcStatus.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-15 03:49:24.551294 airtouch2-0.7.6/src/airtouch2.egg-info/
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2281 2023-07-15 03:49:24.000000 airtouch2-0.7.6/src/airtouch2.egg-info/PKG-INFO
--rw-r--r--   0 nathan    (1000) nathan    (1000)     1649 2023-07-15 03:49:24.000000 airtouch2-0.7.6/src/airtouch2.egg-info/SOURCES.txt
--rw-r--r--   0 nathan    (1000) nathan    (1000)        1 2023-07-15 03:49:24.000000 airtouch2-0.7.6/src/airtouch2.egg-info/dependency_links.txt
--rw-r--r--   0 nathan    (1000) nathan    (1000)       10 2023-07-15 03:49:24.000000 airtouch2-0.7.6/src/airtouch2.egg-info/top_level.txt
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 09:24:42.943027 airtouch2-0.7.7/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1076 2023-01-10 07:31:33.000000 airtouch2-0.7.7/LICENSE
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2290 2023-07-30 09:24:42.943027 airtouch2-0.7.7/PKG-INFO
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      280 2023-07-20 10:35:40.000000 airtouch2-0.7.7/README.md
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      852 2023-07-30 09:06:41.000000 airtouch2-0.7.7/pyproject.toml
+-rw-r--r--   0 nathan    (1000) nathan    (1000)       38 2023-07-30 09:24:42.943027 airtouch2-0.7.7/setup.cfg
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 09:24:42.939027 airtouch2-0.7.7/src/
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 09:24:42.939027 airtouch2-0.7.7/src/airtouch2/
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 09:24:42.939027 airtouch2-0.7.7/src/airtouch2/at2/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2212 2023-07-30 08:39:21.000000 airtouch2-0.7.7/src/airtouch2/at2/At2Aircon.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     3741 2023-07-30 09:04:08.000000 airtouch2-0.7.7/src/airtouch2/at2/At2Client.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1735 2023-07-30 08:39:18.000000 airtouch2-0.7.7/src/airtouch2/at2/At2Group.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      196 2023-07-30 08:38:43.000000 airtouch2-0.7.7/src/airtouch2/at2/__init__.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 09:24:42.943027 airtouch2-0.7.7/src/airtouch2/at2plus/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2789 2023-07-25 09:38:07.000000 airtouch2-0.7.7/src/airtouch2/at2plus/At2PlusAircon.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     8423 2023-07-15 03:40:27.000000 airtouch2-0.7.7/src/airtouch2/at2plus/At2PlusClient.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      190 2023-07-10 11:17:26.000000 airtouch2-0.7.7/src/airtouch2/at2plus/__init__.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 09:24:42.943027 airtouch2-0.7.7/src/airtouch2/common/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2457 2023-07-11 11:20:25.000000 airtouch2-0.7.7/src/airtouch2/common/Buffer.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     4810 2023-07-15 03:40:27.000000 airtouch2-0.7.7/src/airtouch2/common/NetClient.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7.7/src/airtouch2/common/__init__.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1087 2023-07-30 08:40:29.000000 airtouch2-0.7.7/src/airtouch2/common/interfaces.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 09:24:42.943027 airtouch2-0.7.7/src/airtouch2/helpers/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7.7/src/airtouch2/helpers/__init__.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      541 2023-06-25 08:46:07.000000 airtouch2-0.7.7/src/airtouch2/helpers/diff_bytes.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 09:24:42.943027 airtouch2-0.7.7/src/airtouch2/protocol/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-03-19 07:06:23.000000 airtouch2-0.7.7/src/airtouch2/protocol/__init__.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 09:24:42.943027 airtouch2-0.7.7/src/airtouch2/protocol/at2/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2/__init__.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2401 2023-07-30 08:43:50.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2/constants.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1255 2023-07-30 08:43:56.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2/conversions.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      642 2023-07-30 08:44:00.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2/enums.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      865 2023-06-25 08:46:07.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2/lookups.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      308 2023-07-11 11:17:00.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2/message_common.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 09:24:42.943027 airtouch2-0.7.7/src/airtouch2/protocol/at2/messages/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      849 2023-06-25 08:46:07.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2/messages/RequestState.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)    10690 2023-07-30 09:01:26.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2/messages/SystemInfo.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      330 2023-07-30 08:44:10.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2/messages/__init__.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2976 2023-07-30 08:44:31.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2/messages/ac_commands.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1867 2023-07-30 08:33:55.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2/messages/group_commands.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 09:24:42.943027 airtouch2-0.7.7/src/airtouch2/protocol/at2plus/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      148 2023-06-25 08:46:07.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2plus/constants.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2768 2023-06-25 08:46:07.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2plus/control_status_common.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1128 2023-06-25 08:46:07.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2plus/conversions.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2359 2023-06-25 08:46:07.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2plus/crc16_modbus.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1560 2023-06-25 08:46:07.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2plus/enums.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1113 2023-06-25 08:46:07.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2plus/extended_common.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     3942 2023-07-11 11:17:00.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2plus/message_common.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 09:24:42.943027 airtouch2-0.7.7/src/airtouch2/protocol/at2plus/messages/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     6156 2023-06-25 08:46:07.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2plus/messages/AcAbilityMessage.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     3167 2023-06-25 08:46:07.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2plus/messages/AcControl.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     4119 2023-06-25 08:46:07.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2plus/messages/AcStatus.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 09:24:42.939027 airtouch2-0.7.7/src/airtouch2.egg-info/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2290 2023-07-30 09:24:42.000000 airtouch2-0.7.7/src/airtouch2.egg-info/PKG-INFO
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1644 2023-07-30 09:24:42.000000 airtouch2-0.7.7/src/airtouch2.egg-info/SOURCES.txt
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        1 2023-07-30 09:24:42.000000 airtouch2-0.7.7/src/airtouch2.egg-info/dependency_links.txt
+-rw-r--r--   0 nathan    (1000) nathan    (1000)       10 2023-07-30 09:24:42.000000 airtouch2-0.7.7/src/airtouch2.egg-info/top_level.txt
```

### Comparing `airtouch2-0.7.6/LICENSE` & `airtouch2-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.6/PKG-INFO` & `airtouch2-0.7.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airtouch2
-Version: 0.7.6
+Version: 0.7.7
 Summary: API for the monitoring and control of a Polyaire Airtouch 2 system over the local network
 Author-email: Nathan Van der Hoek <nathan.vanderhoek@student.adelaide.edu.au>
 License: MIT License
         
         Copyright (c) 2022 Nathan Van der Hoek
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,15 +35,15 @@
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Software Development :: Embedded Systems
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # airtouch2_python
-In-development Python client for the Polyaire AirTouch 2 airconditioning system
+In-development Python client for the Polyaire AirTouch 2 and 2+ airconditioning systems.
 
 ## Thanks to
 https://github.com/tonymyatt/airtouch3api
 
 https://github.com/ozczecho/vzduch-dotek
 
 https://community.home-assistant.io/t/polyaire-air-touch-2-or-3/19650/44
```

### Comparing `airtouch2-0.7.6/pyproject.toml` & `airtouch2-0.7.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=64"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "airtouch2"
 description = "API for the monitoring and control of a Polyaire Airtouch 2 system over the local network"
-version = "0.7.6"
+version = "0.7.7"
 authors = [{ name = "Nathan Van der Hoek", email = "nathan.vanderhoek@student.adelaide.edu.au" }]
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `airtouch2-0.7.6/src/airtouch2/at2/At2Client.py` & `airtouch2-0.7.7/src/airtouch2/at2/At2Client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 import asyncio
 from datetime import datetime
 import logging
 
 from airtouch2.common.NetClient import NetClient
 from airtouch2.protocol.at2.constants import MessageLength
-from airtouch2.protocol.at2.messages import RequestState, ResponseMessage
+from airtouch2.protocol.at2.messages import RequestState, SystemInfo
 from airtouch2.at2.At2Aircon import At2Aircon
 from airtouch2.at2.At2Group import At2Group
-from airtouch2.common.interfaces import Callback, Serializable, TaskCreator
+from airtouch2.common.interfaces import add_callback, Callback, Serializable, TaskCreator
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class At2Client:
+    aircons_by_id: dict[int, At2Aircon]
+    groups_by_id: dict[int, At2Group]
+    system_name: str
+
     def __init__(self, host: str, dump_responses: bool = False, task_creator: TaskCreator = asyncio.create_task):
-        # public
-        self.aircons: list[At2Aircon] = []
-        self.groups: list[At2Group] = []
+        self.aircons_by_id = {}
+        self.groups_by_id = {}
         self.system_name: str = "UNKNOWN"
 
-        # private
         self._client = NetClient(host, 8899, self._on_connect, self._handle_one_message, task_creator)
         self._dump_responses: bool = dump_responses
         self._new_ac_callbacks: list[Callback] = []
+        self._new_group_callbacks: list[Callback] = []
         self._found_ac = asyncio.Event()
 
         self.add_new_ac_callback(lambda: self._found_ac.set())
 
     async def connect(self) -> bool:
         return await self._client.connect()
 
@@ -38,65 +41,66 @@
             await asyncio.wait_for(self._found_ac.wait(), timeout)
         except TimeoutError:
             pass
 
     async def stop(self) -> None:
         await self._client.stop()
 
-    def add_new_ac_callback(self, callback: Callback):
-        self._new_ac_callbacks.append(callback)
-
-        def remove_callback() -> None:
-            if callback in self._new_ac_callbacks:
-                self._new_ac_callbacks.remove(callback)
-
-        return remove_callback
+    def add_new_ac_callback(self, callback: Callback) -> Callback:
+        """
+        Subscribe 'callback' to new AC discoveries.
+        Return a callback to unsubscribe.
+        """
+        return add_callback(callback, self._new_ac_callbacks)
+
+    def add_new_group_callback(self, callback: Callback):
+        """
+        Subscribe 'callback' to new group discoveries.
+        Return a callback to unsubscribe.
+        """
+        return add_callback(callback, self._new_group_callbacks)
 
     async def send(self, msg: Serializable):
         await self._client.send(msg)
 
     async def _on_connect(self):
         await self._client.send(RequestState())
 
-    async def _read_response(self) -> ResponseMessage | None:
+    async def _read_response(self) -> SystemInfo | None:
         _LOGGER.debug("Waiting for response")
         resp = await self._client.read_bytes(MessageLength.RESPONSE)
         _LOGGER.debug("Got response")
         if not resp:
             return None
 
         if self._dump_responses:
             # blocks but is only used for dev and debugging
             with open('response_' + datetime.now().strftime("%m-%d-%Y_%H-%M-%S") + '.dump', 'wb') as f:
                 f.write(resp)
 
-        return ResponseMessage.from_bytes(resp)
+        return SystemInfo.from_bytes(resp)
 
     async def _handle_one_message(self) -> None:
-        resp = await self._read_response()
-        if not resp:
+        system_info = await self._read_response()
+        if not system_info:
             # something went wrong
-            _LOGGER.info("Reading message failed")
+            _LOGGER.info("Reading response message failed")
             return
 
+        _LOGGER.debug(f"SystemInfo: {system_info}")
         # ACs
-        if not self.aircons:
-            # TODO: Support multiple aircons
-            self.aircons.append(At2Aircon(0, self, resp))
-            _LOGGER.debug(self.aircons[0])
-            for callback in self._new_ac_callbacks:
-                callback()
-        else:
-            for aircon in self.aircons:
-                aircon.update(resp)
-                _LOGGER.debug(aircon)
+        for id, ac_info in system_info.aircons_by_id.items():
+            if id not in self.aircons_by_id:
+                self.aircons_by_id[id] = At2Aircon(self, ac_info)
+                for callback in self._new_ac_callbacks:
+                    callback()
+            else:
+                self.aircons_by_id[id].update(ac_info)
+
         # Groups
-        if not self.groups or len(self.groups) != resp.num_groups:
-            # this clear will cause problems for anything using the groups
-            self.groups.clear()
-            for i in range(resp.num_groups):
-                self.groups.append(At2Group(self, i, resp))
-                _LOGGER.debug(self.groups[i])
-        else:
-            for group in self.groups:
-                group.update(resp)
-                _LOGGER.debug(group)
+        for id, group_info in system_info.groups_by_id.items():
+            if id not in self.groups_by_id:
+                self.groups_by_id[id] = At2Group(self, group_info)
+                for callback in self._new_group_callbacks:
+                    callback()
+            else:
+                self.groups_by_id[id].update(group_info)
```

### Comparing `airtouch2-0.7.6/src/airtouch2/at2/At2Group.py` & `airtouch2-0.7.7/src/airtouch2/at2/At2Group.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,96 +1,55 @@
 from __future__ import annotations
-from itertools import compress
-from typing import TYPE_CHECKING, Callable
-from airtouch2.protocol.at2.messages import ResponseMessage
-
+from typing import TYPE_CHECKING
+from airtouch2.protocol.at2.messages.SystemInfo import GroupInfo
 from airtouch2.protocol.at2.messages import ChangeDamper, ToggleGroup
+from airtouch2.common.interfaces import Publisher, Callback, add_callback
 if TYPE_CHECKING:
     from airtouch2.at2.At2Client import At2Client
-import logging
 
 
-_LOGGER = logging.getLogger(__name__)
+class At2Group(Publisher):
+    info: GroupInfo
 
+    def __init__(self, client: At2Client, info: GroupInfo):
+        self.info = info
 
-class At2Group:
-    def __init__(self, client: At2Client, number: int, response: ResponseMessage):
         self._client = client
-        self.number = number
-        self._callbacks: list[Callable] = []
-        self.update(response)
-
-    def update(self, response: ResponseMessage):
-        self.name = response.group_names[self.number]
-        [start_zone, num_zones] = response.group_zones[self.number]
-        # 0 to 10 steps of 10%
-        self.damp = response.zone_damps[start_zone]
-        self.spill = response.zone_spills[start_zone]
-        self.on = response.zone_ons[start_zone]
-        mismatches: set[str] = set()
-        for i in range(start_zone+1, start_zone + num_zones):
-            # this group is spilling if any of its zones are
-            self.spill = response.zone_spills[i]
-            # these should match for all zones that comprise this group
-            if (self.damp != response.zone_damps[i]):
-                mismatches.add("open percents")
-            if (self.on != response.zone_ons[i]):
-                mismatches.add("on/offs")
-            if mismatches:
-                _LOGGER.warning(f"Zones of group '{self.name}' have mismatching {', '.join(mismatches)}")
+        self._callbacks: list[Callback] = []
 
-        self.turbo = True if response.turbo_group == self.number else False
+    def update(self, status: GroupInfo):
+        self.info = status
 
         for func in self._callbacks:
             func()
 
-    def add_callback(self, func: Callable) -> Callable:
-        self._callbacks.append(func)
-
-        def remove_callback() -> None:
-            if func in self._callbacks:
-                self._callbacks.remove(func)
-
-        return remove_callback
+    def add_callback(self, callback: Callback) -> Callback:
+        return add_callback(callback, self._callbacks)
 
     async def inc_dec_damp(self, inc: bool):
-        await self._client.send(ChangeDamper(self.number, inc))
+        await self._client.send(ChangeDamper(self.info.number, inc))
 
     async def set_damp(self, new_damp: int):
         if new_damp < 0 or new_damp > 10:
             raise ValueError("Dampers can only be set from 0 to 10")
         # Set to 0 is equivalent to turning off
         if new_damp == 0:
             await self.turn_off()
         else:
             await self.turn_on()
-            damp_diff = new_damp - self.damp
+            damp_diff = new_damp - self.info.damp
             inc = damp_diff > 0
             for i in range(abs(damp_diff)):
                 await self.inc_dec_damp(inc)
 
     async def _turn_on_off(self, on: bool):
-        if self.on != on:
-            await self._client.send(ToggleGroup(self.number))
+        if self.info.active != on:
+            await self._client.send(ToggleGroup(self.info.number))
 
     async def turn_off(self):
         await self._turn_on_off(False)
 
     async def turn_on(self):
         await self._turn_on_off(True)
 
-    def get_status_strings(self):
-        flags = [self.spill, self.turbo]
-        flag_names = ['SPILL', 'TURBO']
-        statuses = list(compress(flag_names, flags))
-        if not statuses:
-            statuses.append('NORMAL')
-        return statuses
-
     def __str__(self):
-        return f"""
-        Group Name:\t{self.name}
-        Group Number:\t{self.number}
-        On:\t\t{self.on}
-        Status:\t\t{self.get_status_strings()}
-        Damper:\t\t{f'{self.damp*10}%'}
-        """
+        return str(self.info)
```

### Comparing `airtouch2-0.7.6/src/airtouch2/at2plus/At2PlusAircon.py` & `airtouch2-0.7.7/src/airtouch2/at2plus/At2PlusAircon.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.6/src/airtouch2/at2plus/At2PlusClient.py` & `airtouch2-0.7.7/src/airtouch2/at2plus/At2PlusClient.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.6/src/airtouch2/common/Buffer.py` & `airtouch2-0.7.7/src/airtouch2/common/Buffer.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.6/src/airtouch2/common/NetClient.py` & `airtouch2-0.7.7/src/airtouch2/common/NetClient.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.6/src/airtouch2/helpers/diff_bytes.py` & `airtouch2-0.7.7/src/airtouch2/helpers/diff_bytes.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.6/src/airtouch2/protocol/at2/constants.py` & `airtouch2-0.7.7/src/airtouch2/protocol/at2/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,49 @@
 from enum import IntEnum
 
+
 class MessageLength(IntEnum):
     UNDETERMINED = 0
     COMMAND = 13
     RESPONSE = 395
 
+
 class CommandMessageConstants(IntEnum):
-    BYTE_0 = 85             # Byte 0 of command always fixed
-    BYTE_2 = 12             # Byte 2 of command always fixed
-    TOGGLE = 128            # toggle is common to both ACCommands and GroupCommands
+    BYTE_0 = 85   # Byte 0 of command always fixed
+    BYTE_2 = 12   # Byte 2 of command always fixed
+    TOGGLE = 128  # toggle is common to both ACCommands and GroupCommands
+
 
-# Go in byte 1 of command messages
 class CommandMessageType(IntEnum):
+    # Go in byte 1 of command messages
     REQUEST_STATE = 1
     GROUP_CONTROL = 129
     AC_CONTROL = 134
 
-# Go in byte 4 of CommandMessageType.AC_CONTROL messages
+
 class ACCommands(IntEnum):
+    # Go in byte 4 of CommandMessageType.AC_CONTROL messages
     SET_MODE = 129
     SET_FAN_SPEED = 130
     TEMP_DEC = 147
     TEMP_INC = 163
 
+
 class GroupCommands(IntEnum):
-    CHANGE_DAMP = 1      # 1 goes in byte 5 for change damp
-    TOGGLE = 0           # 0 goes in byte 5 for toggle
-    DAMP_DEC = 1         # Damper decrement (10% down) in byte 4
-    DAMP_INC = 2         # Damper increment (10% up) in byte 4
+    CHANGE_DAMP = 1  # 1 goes in byte 5 for change damp
+    TOGGLE = 0       # 0 goes in byte 5 for toggle
+    DAMP_DEC = 1     # Damper decrement (10% down) in byte 4
+    DAMP_INC = 2     # Damper increment (10% up) in byte 4
 
 
 class ResponseMessageConstants(IntEnum):
     LONG_STRING_LENGTH = 16
     SHORT_STRING_LENGTH = 8
 
-# Thanks to home-assistant.io user Radebe2k
+
 class ResponseMessageOffsets(IntEnum):
     # Header is 2 bytes
     HEADER = 0
     # There are 16 zones
     # zone names are 8 bytes (ResponseMessageConstants.SHORT_STRING_LENGTH)
     GROUP_NAMES_START = 100
     # zone statuses are 1 byte each
@@ -48,33 +53,25 @@
     GROUP_ZONES_START = 244
     # Zone strengths are 1 byte each
     ZONE_DAMPS_START = 276
     NUM_GROUPS = 292
     TURBO_GROUP = 297
     # Contains isTurbo, isSafety, isSpill bits of the 2 ACs
     ACs_STATUS = 299
-    TOUCHPAD_TEMP = 323 # I think?? Idk what happens when there's 2 touchpads then...
+    TOUCHPAD_TEMP = 323  # I think?? Idk what happens when there's 2 touchpads then...
     # System name is 16 bytes (ResponseMessageConstants.LONG_STRING_LENGTH)
     SYSTEM_NAME = 324
+    # The following have 2 consecutuve bytes of each type, 1 for each AC.
     # On/Off, isError, 'Auto off' enabled, 'thermistor on AC', program number
-    AC1_STATUS = 354
-    #AC2_STATUS = 355
-    AC1_BRAND = 356
-    #AC2_BRAND = 357
-    AC1_MODE = 358
-    #AC2_MODE = 359
-    AC1_FAN_SPEED = 360
-    #AC2_FAN_SPEED = 361
-    AC1_SET_TEMP = 362
-    #AC2_SET_TEMP = 363
-    AC1_MEASURED_TEMP = 364
-    #AC2_MEASURED_TEMP = 365
-    AC1_ERROR_CODE = 366
-    #AC2_ERROR_CODE = 367
-    AC1_GATEWAY_ID = 368
-    #AC2_GATEWAY_ID = 369
-    # AC names are 8 bytes (ResponseMessageConstants.SHORT_STRING_LENGTH)
-    AC1_NAME_START = 370
-    #AC2_NAME_START = 378
+    AC_STATUS_START = 354
+    AC_BRAND_START = 356
+    AC_MODE_START = 358
+    AC_FAN_SPEED_START = 360
+    AC_SET_TEMP_START = 362
+    AC_MEASURED_TEMP_START = 364
+    AC_ERROR_CODE_START = 366
+    AC_GATEWAY_ID_START = 368
+    AC_NAME_START = 370  # AC names are 8 bytes (ResponseMessageConstants.SHORT_STRING_LENGTH)
     HASH = 394
 
+
 OPEN_ISSUE_TEXT = "please open an issue and detail your system:\n\thttps://github.com/nathanvdh/airtouch2-python/issues/new"
```

### Comparing `airtouch2-0.7.6/src/airtouch2/protocol/at2/conversions.py` & `airtouch2-0.7.7/src/airtouch2/protocol/at2/conversions.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,65 +1,30 @@
 
 import logging
 from airtouch2.protocol.at2.constants import OPEN_ISSUE_TEXT
-from airtouch2.protocol.at2.enums import ACBrand, ACFanSpeedReference
+from airtouch2.protocol.at2.enums import ACBrand, ACFanSpeed
 from airtouch2.protocol.at2.lookups import GATEWAYID_BRAND_LOOKUP
 
 _LOGGER = logging.getLogger(__name__)
 
-# TODO: read through app smali code more and do this more properly
-# Currently I'm assuming:
-#   4 speed is always LOW, MED, HIGH, POWERFUL (EXCEPT for fujitsus with 4 speeds)
-#   3 speed is always LOW, MED, HIGH
-#   2 speed is always LOW, HIGH
-#   Daikins have no Auto
-#   Gateway ID 0x14 has no Auto
-#   Gateway IDs 0xFF with 3 speed have no Auto
-# This is based on the app decompiled code
-
-
-def supported_fan_speeds(brand: ACBrand, num_supported_speeds: int, gateway_id: int) -> list[ACFanSpeedReference]:
-    all_speeds: list[ACFanSpeedReference] = list(ACFanSpeedReference.__members__.values())
-    supported_speeds: list[ACFanSpeedReference] = []
-
-    if brand == ACBrand.FUJITSU and num_supported_speeds == 4:
-        supported_speeds = all_speeds[:5]
-        return supported_speeds
-
-    # Check cases that don't support Auto mode
-    if (brand == ACBrand.DAIKIN or (gateway_id == 0xFF and num_supported_speeds == 3) or gateway_id == 0x14):
-        supported_speeds = []
-    else:
-        supported_speeds = [ACFanSpeedReference.AUTO]
-
-    if num_supported_speeds > 2:
-        supported_speeds += all_speeds[2:2+num_supported_speeds]
-    elif num_supported_speeds == 2:
-        supported_speeds += [ACFanSpeedReference.LOW, ACFanSpeedReference.HIGH]
-    elif num_supported_speeds < 2:
-        _LOGGER.warning(
-            f"AC reports less than 2 supported fan speeds, this is unusual - " + OPEN_ISSUE_TEXT)
-
-    return supported_speeds
-
 
-def fan_speed_from_val(supported_speeds: list[ACFanSpeedReference], speed_val: int) -> ACFanSpeedReference:
+def fan_speed_from_val(supported_speeds: list[ACFanSpeed], speed_val: int) -> ACFanSpeed:
     if speed_val < 5:
         # Units with no Auto speed still start with low == 1
-        if ACFanSpeedReference.AUTO not in supported_speeds:
+        if ACFanSpeed.AUTO not in supported_speeds:
             speed_val -= 1
         return supported_speeds[speed_val]
     else:
-        return ACFanSpeedReference.AUTO
+        return ACFanSpeed.AUTO
 
 
-def val_from_fan_speed(supported_speeds: list[ACFanSpeedReference], speed: ACFanSpeedReference):
+def val_from_fan_speed(supported_speeds: list[ACFanSpeed], speed: ACFanSpeed):
     speed_val = supported_speeds.index(speed)
     # Units with no Auto speed still start with low == 1
-    if ACFanSpeedReference.AUTO not in supported_speeds:
+    if ACFanSpeed.AUTO not in supported_speeds:
         speed_val += 1
     return speed_val
 
 
 def brand_from_gateway_id(gateway_id: int) -> ACBrand | None:
     if gateway_id > 0:
         if gateway_id in GATEWAYID_BRAND_LOOKUP:
```

### Comparing `airtouch2-0.7.6/src/airtouch2/protocol/at2/enums.py` & `airtouch2-0.7.7/src/airtouch2/protocol/at2/enums.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 from enum import IntEnum
 
+
 class ACMode(IntEnum):
     AUTO = 0
     HEAT = 1
     DRY = 2
     FAN = 3
     COOL = 4
 
     def __str__(self):
         return self._name_
 
-class ACFanSpeedReference(IntEnum):
+
+class ACFanSpeed(IntEnum):
     AUTO = 0
     QUIET = 1
     LOW = 2
     MEDIUM = 3
     HIGH = 4
     POWERFUL = 5
 
     def __str__(self):
         return self._name_
 
 # From adding AC2 on the panel and cycling through brands
+
+
 class ACBrand(IntEnum):
     NONE = 0
     DAIKIN = 1
     FUJITSU = 2
     HITACHI = 3
     LG = 4
     MITSUBISHI_ELECTRIC = 5
```

### Comparing `airtouch2-0.7.6/src/airtouch2/protocol/at2/lookups.py` & `airtouch2-0.7.7/src/airtouch2/protocol/at2/lookups.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.6/src/airtouch2/protocol/at2/messages/RequestState.py` & `airtouch2-0.7.7/src/airtouch2/protocol/at2/messages/RequestState.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.6/src/airtouch2/protocol/at2/messages/ac_commands.py` & `airtouch2-0.7.7/src/airtouch2/protocol/at2/messages/ac_commands.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from airtouch2.protocol.at2.conversions import val_from_fan_speed
 from airtouch2.protocol.at2.message_common import add_checksum_message_buffer
 from airtouch2.protocol.at2.constants import ACCommands, CommandMessageConstants, CommandMessageType, MessageLength
-from airtouch2.protocol.at2.enums import ACMode
+from airtouch2.protocol.at2.enums import ACFanSpeed, ACMode
 from airtouch2.common.Buffer import Buffer
 from airtouch2.common.interfaces import Serializable
 
 
 def prime_ac_control_message_buffer(target_ac: int) -> Buffer:
     buffer = Buffer(MessageLength.COMMAND)
     buffer.append_bytes(CommandMessageConstants.BYTE_0.to_bytes(1, 'little'))
@@ -30,32 +31,29 @@
 
 class ToggleAc(Serializable):
     def __init__(self, target_ac_number: int):
         self.target_ac = target_ac_number
 
     def to_bytes(self) -> bytes:
         buffer = prime_ac_control_message_buffer(self.target_ac)
-        # buffer.append_bytes(bytes([0]))
         buffer.append_bytes(CommandMessageConstants.TOGGLE.to_bytes(1, 'little'))
         buffer.append_bytes(bytes([0, 0, 0, 0, 0, 0, 0]))
         add_checksum_message_buffer(buffer)
         return buffer.to_bytes()
 
-# needs investigation
-
 
 class SetFanSpeed(Serializable):
-    def __init__(self, target_ac_number: int, fan_speed: int):
+    def __init__(self, target_ac_number: int, supported_fan_speeds: list[ACFanSpeed], fan_speed: ACFanSpeed):
         self.target_ac = target_ac_number
-        self.fan_speed = fan_speed
+        self.fan_speed_val: int = val_from_fan_speed(supported_fan_speeds, fan_speed)
 
     def to_bytes(self) -> bytes:
         buffer = prime_ac_control_message_buffer(self.target_ac)
         buffer.append_bytes(ACCommands.SET_FAN_SPEED.to_bytes(1, 'little'))
-        buffer.append_bytes(self.fan_speed.to_bytes(1, 'little'))
+        buffer.append_bytes(self.fan_speed_val.to_bytes(1, 'little'))
         buffer.append_bytes(bytes([0, 0, 0, 0, 0, 0]))
         add_checksum_message_buffer(buffer)
         return buffer.to_bytes()
 
 
 class SetMode(Serializable):
     def __init__(self, target_ac_number: int, mode: ACMode):
```

### Comparing `airtouch2-0.7.6/src/airtouch2/protocol/at2/messages/group_commands.py` & `airtouch2-0.7.7/src/airtouch2/protocol/at2/messages/group_commands.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.6/src/airtouch2/protocol/at2plus/control_status_common.py` & `airtouch2-0.7.7/src/airtouch2/protocol/at2plus/control_status_common.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.6/src/airtouch2/protocol/at2plus/conversions.py` & `airtouch2-0.7.7/src/airtouch2/protocol/at2plus/conversions.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.6/src/airtouch2/protocol/at2plus/crc16_modbus.py` & `airtouch2-0.7.7/src/airtouch2/protocol/at2plus/crc16_modbus.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.6/src/airtouch2/protocol/at2plus/enums.py` & `airtouch2-0.7.7/src/airtouch2/protocol/at2plus/enums.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.6/src/airtouch2/protocol/at2plus/extended_common.py` & `airtouch2-0.7.7/src/airtouch2/protocol/at2plus/extended_common.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.6/src/airtouch2/protocol/at2plus/message_common.py` & `airtouch2-0.7.7/src/airtouch2/protocol/at2plus/message_common.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.6/src/airtouch2/protocol/at2plus/messages/AcAbilityMessage.py` & `airtouch2-0.7.7/src/airtouch2/protocol/at2plus/messages/AcAbilityMessage.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.6/src/airtouch2/protocol/at2plus/messages/AcControl.py` & `airtouch2-0.7.7/src/airtouch2/protocol/at2plus/messages/AcControl.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.6/src/airtouch2/protocol/at2plus/messages/AcStatus.py` & `airtouch2-0.7.7/src/airtouch2/protocol/at2plus/messages/AcStatus.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.6/src/airtouch2.egg-info/PKG-INFO` & `airtouch2-0.7.7/src/airtouch2.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airtouch2
-Version: 0.7.6
+Version: 0.7.7
 Summary: API for the monitoring and control of a Polyaire Airtouch 2 system over the local network
 Author-email: Nathan Van der Hoek <nathan.vanderhoek@student.adelaide.edu.au>
 License: MIT License
         
         Copyright (c) 2022 Nathan Van der Hoek
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,15 +35,15 @@
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Software Development :: Embedded Systems
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # airtouch2_python
-In-development Python client for the Polyaire AirTouch 2 airconditioning system
+In-development Python client for the Polyaire AirTouch 2 and 2+ airconditioning systems.
 
 ## Thanks to
 https://github.com/tonymyatt/airtouch3api
 
 https://github.com/ozczecho/vzduch-dotek
 
 https://community.home-assistant.io/t/polyaire-air-touch-2-or-3/19650/44
```

### Comparing `airtouch2-0.7.6/src/airtouch2.egg-info/SOURCES.txt` & `airtouch2-0.7.7/src/airtouch2.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 src/airtouch2/protocol/at2/__init__.py
 src/airtouch2/protocol/at2/constants.py
 src/airtouch2/protocol/at2/conversions.py
 src/airtouch2/protocol/at2/enums.py
 src/airtouch2/protocol/at2/lookups.py
 src/airtouch2/protocol/at2/message_common.py
 src/airtouch2/protocol/at2/messages/RequestState.py
-src/airtouch2/protocol/at2/messages/ResponseMessage.py
+src/airtouch2/protocol/at2/messages/SystemInfo.py
 src/airtouch2/protocol/at2/messages/__init__.py
 src/airtouch2/protocol/at2/messages/ac_commands.py
 src/airtouch2/protocol/at2/messages/group_commands.py
 src/airtouch2/protocol/at2plus/constants.py
 src/airtouch2/protocol/at2plus/control_status_common.py
 src/airtouch2/protocol/at2plus/conversions.py
 src/airtouch2/protocol/at2plus/crc16_modbus.py
```

