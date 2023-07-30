# Comparing `tmp/airtouch2-0.7.7.tar.gz` & `tmp/airtouch2-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airtouch2-0.7.7.tar", last modified: Sun Jul 30 09:24:42 2023, max compression
+gzip compressed data, was "airtouch2-0.7.8.tar", last modified: Sun Jul 30 11:41:54 2023, max compression
```

## Comparing `airtouch2-0.7.7.tar` & `airtouch2-0.7.8.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 09:24:42.943027 airtouch2-0.7.7/
--rw-r--r--   0 nathan    (1000) nathan    (1000)     1076 2023-01-10 07:31:33.000000 airtouch2-0.7.7/LICENSE
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2290 2023-07-30 09:24:42.943027 airtouch2-0.7.7/PKG-INFO
--rw-r--r--   0 nathan    (1000) nathan    (1000)      280 2023-07-20 10:35:40.000000 airtouch2-0.7.7/README.md
--rw-r--r--   0 nathan    (1000) nathan    (1000)      852 2023-07-30 09:06:41.000000 airtouch2-0.7.7/pyproject.toml
--rw-r--r--   0 nathan    (1000) nathan    (1000)       38 2023-07-30 09:24:42.943027 airtouch2-0.7.7/setup.cfg
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 09:24:42.939027 airtouch2-0.7.7/src/
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 09:24:42.939027 airtouch2-0.7.7/src/airtouch2/
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 09:24:42.939027 airtouch2-0.7.7/src/airtouch2/at2/
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2212 2023-07-30 08:39:21.000000 airtouch2-0.7.7/src/airtouch2/at2/At2Aircon.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     3741 2023-07-30 09:04:08.000000 airtouch2-0.7.7/src/airtouch2/at2/At2Client.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     1735 2023-07-30 08:39:18.000000 airtouch2-0.7.7/src/airtouch2/at2/At2Group.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      196 2023-07-30 08:38:43.000000 airtouch2-0.7.7/src/airtouch2/at2/__init__.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 09:24:42.943027 airtouch2-0.7.7/src/airtouch2/at2plus/
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2789 2023-07-25 09:38:07.000000 airtouch2-0.7.7/src/airtouch2/at2plus/At2PlusAircon.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     8423 2023-07-15 03:40:27.000000 airtouch2-0.7.7/src/airtouch2/at2plus/At2PlusClient.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      190 2023-07-10 11:17:26.000000 airtouch2-0.7.7/src/airtouch2/at2plus/__init__.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 09:24:42.943027 airtouch2-0.7.7/src/airtouch2/common/
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2457 2023-07-11 11:20:25.000000 airtouch2-0.7.7/src/airtouch2/common/Buffer.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     4810 2023-07-15 03:40:27.000000 airtouch2-0.7.7/src/airtouch2/common/NetClient.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7.7/src/airtouch2/common/__init__.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     1087 2023-07-30 08:40:29.000000 airtouch2-0.7.7/src/airtouch2/common/interfaces.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 09:24:42.943027 airtouch2-0.7.7/src/airtouch2/helpers/
--rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7.7/src/airtouch2/helpers/__init__.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      541 2023-06-25 08:46:07.000000 airtouch2-0.7.7/src/airtouch2/helpers/diff_bytes.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 09:24:42.943027 airtouch2-0.7.7/src/airtouch2/protocol/
--rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-03-19 07:06:23.000000 airtouch2-0.7.7/src/airtouch2/protocol/__init__.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 09:24:42.943027 airtouch2-0.7.7/src/airtouch2/protocol/at2/
--rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2/__init__.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2401 2023-07-30 08:43:50.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2/constants.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     1255 2023-07-30 08:43:56.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2/conversions.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      642 2023-07-30 08:44:00.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2/enums.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      865 2023-06-25 08:46:07.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2/lookups.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      308 2023-07-11 11:17:00.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2/message_common.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 09:24:42.943027 airtouch2-0.7.7/src/airtouch2/protocol/at2/messages/
--rw-r--r--   0 nathan    (1000) nathan    (1000)      849 2023-06-25 08:46:07.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2/messages/RequestState.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)    10690 2023-07-30 09:01:26.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2/messages/SystemInfo.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      330 2023-07-30 08:44:10.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2/messages/__init__.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2976 2023-07-30 08:44:31.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2/messages/ac_commands.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     1867 2023-07-30 08:33:55.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2/messages/group_commands.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 09:24:42.943027 airtouch2-0.7.7/src/airtouch2/protocol/at2plus/
--rw-r--r--   0 nathan    (1000) nathan    (1000)      148 2023-06-25 08:46:07.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2plus/constants.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2768 2023-06-25 08:46:07.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2plus/control_status_common.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     1128 2023-06-25 08:46:07.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2plus/conversions.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2359 2023-06-25 08:46:07.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2plus/crc16_modbus.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     1560 2023-06-25 08:46:07.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2plus/enums.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     1113 2023-06-25 08:46:07.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2plus/extended_common.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     3942 2023-07-11 11:17:00.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2plus/message_common.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 09:24:42.943027 airtouch2-0.7.7/src/airtouch2/protocol/at2plus/messages/
--rw-r--r--   0 nathan    (1000) nathan    (1000)     6156 2023-06-25 08:46:07.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2plus/messages/AcAbilityMessage.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     3167 2023-06-25 08:46:07.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2plus/messages/AcControl.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     4119 2023-06-25 08:46:07.000000 airtouch2-0.7.7/src/airtouch2/protocol/at2plus/messages/AcStatus.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 09:24:42.939027 airtouch2-0.7.7/src/airtouch2.egg-info/
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2290 2023-07-30 09:24:42.000000 airtouch2-0.7.7/src/airtouch2.egg-info/PKG-INFO
--rw-r--r--   0 nathan    (1000) nathan    (1000)     1644 2023-07-30 09:24:42.000000 airtouch2-0.7.7/src/airtouch2.egg-info/SOURCES.txt
--rw-r--r--   0 nathan    (1000) nathan    (1000)        1 2023-07-30 09:24:42.000000 airtouch2-0.7.7/src/airtouch2.egg-info/dependency_links.txt
--rw-r--r--   0 nathan    (1000) nathan    (1000)       10 2023-07-30 09:24:42.000000 airtouch2-0.7.7/src/airtouch2.egg-info/top_level.txt
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 11:41:54.411830 airtouch2-0.7.8/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1076 2023-01-10 07:31:33.000000 airtouch2-0.7.8/LICENSE
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2290 2023-07-30 11:41:54.411830 airtouch2-0.7.8/PKG-INFO
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      280 2023-07-20 10:35:40.000000 airtouch2-0.7.8/README.md
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      852 2023-07-30 11:41:34.000000 airtouch2-0.7.8/pyproject.toml
+-rw-r--r--   0 nathan    (1000) nathan    (1000)       38 2023-07-30 11:41:54.411830 airtouch2-0.7.8/setup.cfg
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 11:41:54.407830 airtouch2-0.7.8/src/
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 11:41:54.407830 airtouch2-0.7.8/src/airtouch2/
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 11:41:54.407830 airtouch2-0.7.8/src/airtouch2/at2/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2212 2023-07-30 08:39:21.000000 airtouch2-0.7.8/src/airtouch2/at2/At2Aircon.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     3741 2023-07-30 09:04:08.000000 airtouch2-0.7.8/src/airtouch2/at2/At2Client.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1735 2023-07-30 08:39:18.000000 airtouch2-0.7.8/src/airtouch2/at2/At2Group.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      196 2023-07-30 08:38:43.000000 airtouch2-0.7.8/src/airtouch2/at2/__init__.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 11:41:54.407830 airtouch2-0.7.8/src/airtouch2/at2plus/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2789 2023-07-25 09:38:07.000000 airtouch2-0.7.8/src/airtouch2/at2plus/At2PlusAircon.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     8686 2023-07-30 11:30:12.000000 airtouch2-0.7.8/src/airtouch2/at2plus/At2PlusClient.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      190 2023-07-10 11:17:26.000000 airtouch2-0.7.8/src/airtouch2/at2plus/__init__.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 11:41:54.407830 airtouch2-0.7.8/src/airtouch2/common/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2457 2023-07-11 11:20:25.000000 airtouch2-0.7.8/src/airtouch2/common/Buffer.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     4810 2023-07-15 03:40:27.000000 airtouch2-0.7.8/src/airtouch2/common/NetClient.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7.8/src/airtouch2/common/__init__.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1087 2023-07-30 08:40:29.000000 airtouch2-0.7.8/src/airtouch2/common/interfaces.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 11:41:54.407830 airtouch2-0.7.8/src/airtouch2/helpers/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7.8/src/airtouch2/helpers/__init__.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      541 2023-06-25 08:46:07.000000 airtouch2-0.7.8/src/airtouch2/helpers/diff_bytes.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 11:41:54.407830 airtouch2-0.7.8/src/airtouch2/protocol/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-03-19 07:06:23.000000 airtouch2-0.7.8/src/airtouch2/protocol/__init__.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 11:41:54.407830 airtouch2-0.7.8/src/airtouch2/protocol/at2/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7.8/src/airtouch2/protocol/at2/__init__.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2401 2023-07-30 08:43:50.000000 airtouch2-0.7.8/src/airtouch2/protocol/at2/constants.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1255 2023-07-30 08:43:56.000000 airtouch2-0.7.8/src/airtouch2/protocol/at2/conversions.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      642 2023-07-30 08:44:00.000000 airtouch2-0.7.8/src/airtouch2/protocol/at2/enums.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      865 2023-06-25 08:46:07.000000 airtouch2-0.7.8/src/airtouch2/protocol/at2/lookups.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      308 2023-07-11 11:17:00.000000 airtouch2-0.7.8/src/airtouch2/protocol/at2/message_common.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 11:41:54.411830 airtouch2-0.7.8/src/airtouch2/protocol/at2/messages/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      849 2023-06-25 08:46:07.000000 airtouch2-0.7.8/src/airtouch2/protocol/at2/messages/RequestState.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)    10690 2023-07-30 09:01:26.000000 airtouch2-0.7.8/src/airtouch2/protocol/at2/messages/SystemInfo.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      330 2023-07-30 08:44:10.000000 airtouch2-0.7.8/src/airtouch2/protocol/at2/messages/__init__.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2976 2023-07-30 08:44:31.000000 airtouch2-0.7.8/src/airtouch2/protocol/at2/messages/ac_commands.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1867 2023-07-30 08:33:55.000000 airtouch2-0.7.8/src/airtouch2/protocol/at2/messages/group_commands.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 11:41:54.411830 airtouch2-0.7.8/src/airtouch2/protocol/at2plus/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      148 2023-06-25 08:46:07.000000 airtouch2-0.7.8/src/airtouch2/protocol/at2plus/constants.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     3038 2023-07-30 11:26:17.000000 airtouch2-0.7.8/src/airtouch2/protocol/at2plus/control_status_common.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1128 2023-06-25 08:46:07.000000 airtouch2-0.7.8/src/airtouch2/protocol/at2plus/conversions.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2359 2023-06-25 08:46:07.000000 airtouch2-0.7.8/src/airtouch2/protocol/at2plus/crc16_modbus.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1560 2023-06-25 08:46:07.000000 airtouch2-0.7.8/src/airtouch2/protocol/at2plus/enums.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1113 2023-06-25 08:46:07.000000 airtouch2-0.7.8/src/airtouch2/protocol/at2plus/extended_common.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     3942 2023-07-11 11:17:00.000000 airtouch2-0.7.8/src/airtouch2/protocol/at2plus/message_common.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 11:41:54.411830 airtouch2-0.7.8/src/airtouch2/protocol/at2plus/messages/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     6156 2023-06-25 08:46:07.000000 airtouch2-0.7.8/src/airtouch2/protocol/at2plus/messages/AcAbilityMessage.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     3167 2023-06-25 08:46:07.000000 airtouch2-0.7.8/src/airtouch2/protocol/at2plus/messages/AcControl.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     4119 2023-06-25 08:46:07.000000 airtouch2-0.7.8/src/airtouch2/protocol/at2plus/messages/AcStatus.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-30 11:41:54.407830 airtouch2-0.7.8/src/airtouch2.egg-info/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2290 2023-07-30 11:41:54.000000 airtouch2-0.7.8/src/airtouch2.egg-info/PKG-INFO
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1644 2023-07-30 11:41:54.000000 airtouch2-0.7.8/src/airtouch2.egg-info/SOURCES.txt
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        1 2023-07-30 11:41:54.000000 airtouch2-0.7.8/src/airtouch2.egg-info/dependency_links.txt
+-rw-r--r--   0 nathan    (1000) nathan    (1000)       10 2023-07-30 11:41:54.000000 airtouch2-0.7.8/src/airtouch2.egg-info/top_level.txt
```

### Comparing `airtouch2-0.7.7/LICENSE` & `airtouch2-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.7/PKG-INFO` & `airtouch2-0.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airtouch2
-Version: 0.7.7
+Version: 0.7.8
 Summary: API for the monitoring and control of a Polyaire Airtouch 2 system over the local network
 Author-email: Nathan Van der Hoek <nathan.vanderhoek@student.adelaide.edu.au>
 License: MIT License
         
         Copyright (c) 2022 Nathan Van der Hoek
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `airtouch2-0.7.7/pyproject.toml` & `airtouch2-0.7.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=64"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "airtouch2"
 description = "API for the monitoring and control of a Polyaire Airtouch 2 system over the local network"
-version = "0.7.7"
+version = "0.7.8"
 authors = [{ name = "Nathan Van der Hoek", email = "nathan.vanderhoek@student.adelaide.edu.au" }]
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `airtouch2-0.7.7/src/airtouch2/at2/At2Aircon.py` & `airtouch2-0.7.8/src/airtouch2/at2/At2Aircon.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.7/src/airtouch2/at2/At2Client.py` & `airtouch2-0.7.8/src/airtouch2/at2/At2Client.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.7/src/airtouch2/at2/At2Group.py` & `airtouch2-0.7.8/src/airtouch2/at2/At2Group.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.7/src/airtouch2/at2plus/At2PlusAircon.py` & `airtouch2-0.7.8/src/airtouch2/at2plus/At2PlusAircon.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.7/src/airtouch2/at2plus/At2PlusClient.py` & `airtouch2-0.7.8/src/airtouch2/at2plus/At2PlusClient.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,25 +64,30 @@
 
         if message.header.type == MessageType.CONTROL_STATUS:
             subheader = ControlStatusSubHeader.from_buffer(message.data_buffer)
             if subheader.sub_type == ControlStatusSubType.AC_STATUS:
                 status_message = AcStatusMessage.from_bytes(
                     message.data_buffer.read_bytes(subheader.subdata_length.total()))
                 self._task_creator(self._handle_status_message(status_message))
+            elif subheader.sub_type == ControlStatusSubType.GROUP_STATUS:
+                # NYI
+                pass
             else:
-                _LOGGER.error(f"Unknown control/status message type: {subheader.sub_type}")
+                _LOGGER.error(
+                    f"Unknown status message type: subtype={subheader.sub_type}, data={message.data_buffer.to_bytes().hex(':')}")
         elif message.header.type == MessageType.EXTENDED:
             subheader = ExtendedSubHeader.from_buffer(message.data_buffer)
             if subheader.sub_type == ExtendedMessageSubType.ABILITY:
                 ability_message_bytes = message.data_buffer.read_remaining()
                 _LOGGER.debug(f"Creating ability message from {len(ability_message_bytes)} bytes")
                 ability = AcAbilityMessage.from_bytes(ability_message_bytes)
                 await self._ability_message_queue.put(ability)
             else:
-                _LOGGER.error(f"Unknown extended message type: {subheader.sub_type}")
+                _LOGGER.error(
+                    f"Unknown extended message type: subtype={subheader.sub_type}, data={message.data_buffer.to_bytes().hex(':')}")
         else:
             _LOGGER.error(
                 f"Unknown message type, header={message.header.to_bytes().hex(':')}, data={message.data_buffer.to_bytes().hex(':')}")
 
     async def _read_magic(self) -> bytes:
         """Search for the two header magic bytes"""
         while True:  # exit via return on successful read of header magic
```

### Comparing `airtouch2-0.7.7/src/airtouch2/common/Buffer.py` & `airtouch2-0.7.8/src/airtouch2/common/Buffer.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.7/src/airtouch2/common/NetClient.py` & `airtouch2-0.7.8/src/airtouch2/common/NetClient.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.7/src/airtouch2/common/interfaces.py` & `airtouch2-0.7.8/src/airtouch2/common/interfaces.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.7/src/airtouch2/helpers/diff_bytes.py` & `airtouch2-0.7.8/src/airtouch2/helpers/diff_bytes.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.7/src/airtouch2/protocol/at2/constants.py` & `airtouch2-0.7.8/src/airtouch2/protocol/at2/constants.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.7/src/airtouch2/protocol/at2/conversions.py` & `airtouch2-0.7.8/src/airtouch2/protocol/at2/conversions.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.7/src/airtouch2/protocol/at2/enums.py` & `airtouch2-0.7.8/src/airtouch2/protocol/at2/enums.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.7/src/airtouch2/protocol/at2/lookups.py` & `airtouch2-0.7.8/src/airtouch2/protocol/at2/lookups.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.7/src/airtouch2/protocol/at2/messages/RequestState.py` & `airtouch2-0.7.8/src/airtouch2/protocol/at2/messages/RequestState.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.7/src/airtouch2/protocol/at2/messages/SystemInfo.py` & `airtouch2-0.7.8/src/airtouch2/protocol/at2/messages/SystemInfo.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.7/src/airtouch2/protocol/at2/messages/ac_commands.py` & `airtouch2-0.7.8/src/airtouch2/protocol/at2/messages/ac_commands.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.7/src/airtouch2/protocol/at2/messages/group_commands.py` & `airtouch2-0.7.8/src/airtouch2/protocol/at2/messages/group_commands.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.7/src/airtouch2/protocol/at2plus/control_status_common.py` & `airtouch2-0.7.8/src/airtouch2/protocol/at2plus/control_status_common.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from __future__ import annotations
 from dataclasses import dataclass
 from enum import IntEnum
 from airtouch2.common.Buffer import Buffer
+import logging
 
 from airtouch2.common.interfaces import Serializable
 
 
 CONTROL_STATUS_SUBHEADER_LENGTH = 8
 SUBDATALENGTH_LENGTH = 6
 
+_LOGGER = logging.getLogger(__name__)
 
 class ControlStatusOffsets(IntEnum):
     # Control/Status messages 'data' consists of:
     # * 8 byte header with information as described below, immediately followed by:
     # * a 'normal data', which occurs once, with length described in the header.
     # * a number of 'repeat data', which each have length described by the header
     # 1st byte is one of ControlStatusSubType
@@ -64,15 +66,21 @@
     sub_type: ControlStatusSubType
     subdata_length: SubDataLength
 
     @staticmethod
     def from_bytes(subheader_bytes: bytes) -> ControlStatusSubHeader:
         if len(subheader_bytes) != CONTROL_STATUS_SUBHEADER_LENGTH:
             raise ValueError("Unexpected control/status subheader size")
-        subtype = ControlStatusSubType(subheader_bytes[0])
+        try:
+            subtype = ControlStatusSubType(subheader_bytes[0])
+        except ValueError as e:
+            _LOGGER.error(
+                f"Unknown message type in header ({hex(subheader_bytes[0])})", exc_info=e)
+            subtype = ControlStatusSubType.UNSET
+
         data_length = SubDataLength.from_bytes(subheader_bytes[2:8])
         return ControlStatusSubHeader(subtype, data_length)
 
     @staticmethod
     def from_buffer(buffer: Buffer) -> ControlStatusSubHeader:
         return ControlStatusSubHeader.from_bytes(buffer.read_bytes(CONTROL_STATUS_SUBHEADER_LENGTH))
```

### Comparing `airtouch2-0.7.7/src/airtouch2/protocol/at2plus/conversions.py` & `airtouch2-0.7.8/src/airtouch2/protocol/at2plus/conversions.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.7/src/airtouch2/protocol/at2plus/crc16_modbus.py` & `airtouch2-0.7.8/src/airtouch2/protocol/at2plus/crc16_modbus.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.7/src/airtouch2/protocol/at2plus/enums.py` & `airtouch2-0.7.8/src/airtouch2/protocol/at2plus/enums.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.7/src/airtouch2/protocol/at2plus/extended_common.py` & `airtouch2-0.7.8/src/airtouch2/protocol/at2plus/extended_common.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.7/src/airtouch2/protocol/at2plus/message_common.py` & `airtouch2-0.7.8/src/airtouch2/protocol/at2plus/message_common.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.7/src/airtouch2/protocol/at2plus/messages/AcAbilityMessage.py` & `airtouch2-0.7.8/src/airtouch2/protocol/at2plus/messages/AcAbilityMessage.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.7/src/airtouch2/protocol/at2plus/messages/AcControl.py` & `airtouch2-0.7.8/src/airtouch2/protocol/at2plus/messages/AcControl.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.7/src/airtouch2/protocol/at2plus/messages/AcStatus.py` & `airtouch2-0.7.8/src/airtouch2/protocol/at2plus/messages/AcStatus.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.7/src/airtouch2.egg-info/PKG-INFO` & `airtouch2-0.7.8/src/airtouch2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airtouch2
-Version: 0.7.7
+Version: 0.7.8
 Summary: API for the monitoring and control of a Polyaire Airtouch 2 system over the local network
 Author-email: Nathan Van der Hoek <nathan.vanderhoek@student.adelaide.edu.au>
 License: MIT License
         
         Copyright (c) 2022 Nathan Van der Hoek
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `airtouch2-0.7.7/src/airtouch2.egg-info/SOURCES.txt` & `airtouch2-0.7.8/src/airtouch2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

