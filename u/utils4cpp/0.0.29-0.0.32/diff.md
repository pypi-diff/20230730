# Comparing `tmp/utils4cpp-0.0.29.tar.gz` & `tmp/utils4cpp-0.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utils4cpp-0.0.29.tar", last modified: Thu Dec 22 15:54:10 2022, max compression
+gzip compressed data, was "dist/utils4cpp-0.0.32.tar", last modified: Sun Jul 30 14:05:49 2023, max compression
```

## Comparing `utils4cpp-0.0.29.tar` & `utils4cpp-0.0.32.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 piggy      (501) staff       (20)        0 2022-12-22 15:54:10.175786 utils4cpp-0.0.29/
--rw-r--r--   0 piggy      (501) staff       (20)      191 2022-12-22 15:54:10.175601 utils4cpp-0.0.29/PKG-INFO
--rw-r--r--   0 piggy      (501) staff       (20)       38 2022-12-22 15:54:10.175833 utils4cpp-0.0.29/setup.cfg
--rw-r--r--   0 piggy      (501) staff       (20)      405 2022-12-22 15:52:38.000000 utils4cpp-0.0.29/setup.py
-drwxr-xr-x   0 piggy      (501) staff       (20)        0 2022-12-22 15:54:10.174791 utils4cpp-0.0.29/utils4cpp/
--rw-r--r--   0 piggy      (501) staff       (20)       38 2021-03-16 07:28:39.000000 utils4cpp-0.0.29/utils4cpp/__init__.py
--rw-r--r--   0 piggy      (501) staff       (20)     5568 2022-12-22 15:53:39.000000 utils4cpp-0.0.29/utils4cpp/constants.py
--rw-r--r--   0 piggy      (501) staff       (20)    34446 2021-12-20 16:58:57.000000 utils4cpp-0.0.29/utils4cpp/flask.py
--rw-r--r--   0 piggy      (501) staff       (20)    31843 2021-12-20 16:58:57.000000 utils4cpp-0.0.29/utils4cpp/models.py
--rw-r--r--   0 piggy      (501) staff       (20)     1906 2021-03-16 07:28:39.000000 utils4cpp-0.0.29/utils4cpp/utils.py
-drwxr-xr-x   0 piggy      (501) staff       (20)        0 2022-12-22 15:54:10.175426 utils4cpp-0.0.29/utils4cpp.egg-info/
--rw-r--r--   0 piggy      (501) staff       (20)      191 2022-12-22 15:54:10.000000 utils4cpp-0.0.29/utils4cpp.egg-info/PKG-INFO
--rw-r--r--   0 piggy      (501) staff       (20)      275 2022-12-22 15:54:10.000000 utils4cpp-0.0.29/utils4cpp.egg-info/SOURCES.txt
--rw-r--r--   0 piggy      (501) staff       (20)        1 2022-12-22 15:54:10.000000 utils4cpp-0.0.29/utils4cpp.egg-info/dependency_links.txt
--rw-r--r--   0 piggy      (501) staff       (20)       54 2022-12-22 15:54:10.000000 utils4cpp-0.0.29/utils4cpp.egg-info/requires.txt
--rw-r--r--   0 piggy      (501) staff       (20)       10 2022-12-22 15:54:10.000000 utils4cpp-0.0.29/utils4cpp.egg-info/top_level.txt
+drwxr-xr-x   0 piggy      (501) staff       (20)        0 2023-07-30 14:05:49.000000 utils4cpp-0.0.32/
+-rw-r--r--   0 piggy      (501) staff       (20)      191 2023-07-30 14:05:49.000000 utils4cpp-0.0.32/PKG-INFO
+-rw-r--r--   0 piggy      (501) staff       (20)        0 2021-03-16 07:28:39.000000 utils4cpp-0.0.32/LICENSE
+drwxr-xr-x   0 piggy      (501) staff       (20)        0 2023-07-30 14:05:49.000000 utils4cpp-0.0.32/utils4cpp.egg-info/
+-rw-r--r--   0 piggy      (501) staff       (20)      191 2023-07-30 14:05:49.000000 utils4cpp-0.0.32/utils4cpp.egg-info/PKG-INFO
+-rw-r--r--   0 piggy      (501) staff       (20)      283 2023-07-30 14:05:49.000000 utils4cpp-0.0.32/utils4cpp.egg-info/SOURCES.txt
+-rw-r--r--   0 piggy      (501) staff       (20)       54 2023-07-30 14:05:49.000000 utils4cpp-0.0.32/utils4cpp.egg-info/requires.txt
+-rw-r--r--   0 piggy      (501) staff       (20)       10 2023-07-30 14:05:49.000000 utils4cpp-0.0.32/utils4cpp.egg-info/top_level.txt
+-rw-r--r--   0 piggy      (501) staff       (20)        1 2023-07-30 14:05:49.000000 utils4cpp-0.0.32/utils4cpp.egg-info/dependency_links.txt
+-rw-r--r--   0 piggy      (501) staff       (20)      405 2023-07-30 14:04:40.000000 utils4cpp-0.0.32/setup.py
+-rw-r--r--   0 piggy      (501) staff       (20)       38 2023-07-30 14:05:49.000000 utils4cpp-0.0.32/setup.cfg
+drwxr-xr-x   0 piggy      (501) staff       (20)        0 2023-07-30 14:05:49.000000 utils4cpp-0.0.32/utils4cpp/
+-rw-r--r--   0 piggy      (501) staff       (20)    31843 2021-12-20 16:58:57.000000 utils4cpp-0.0.32/utils4cpp/models.py
+-rw-r--r--   0 piggy      (501) staff       (20)    34446 2021-12-20 16:58:57.000000 utils4cpp-0.0.32/utils4cpp/flask.py
+-rw-r--r--   0 piggy      (501) staff       (20)     5613 2023-07-30 13:46:30.000000 utils4cpp-0.0.32/utils4cpp/constants.py
+-rw-r--r--   0 piggy      (501) staff       (20)       38 2021-03-16 07:28:39.000000 utils4cpp-0.0.32/utils4cpp/__init__.py
+-rw-r--r--   0 piggy      (501) staff       (20)     1906 2021-03-16 07:28:39.000000 utils4cpp-0.0.32/utils4cpp/utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `utils4cpp-0.0.29/utils4cpp/constants.py` & `utils4cpp-0.0.32/utils4cpp/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,20 +126,22 @@
     MODEL_M21G = "M21G"
 
 
 class AuthType(Enum):
     AUTH_TYPE_OTHER = '其他'
     AUTH_TYPE_SMS = '短信'
     AUTH_TYPE_ASSISTANT = '辅助'
+    AUTH_TYPE_MP = '小程序'
 
 
 class AuthTypeIds(Enum):
     AUTH_TYPE_OTHER = 0
     AUTH_TYPE_SMS = 1
     AUTH_TYPE_ASSISTANT = 2
+    AUTH_TYPE_MP = 3
 
 
 class SmsType(Enum):
     SMS_TYPE_OTHER = '其他'
     SMS_TYPE_SMS_AUTH = '短信认证'
     SMS_TYPE_APP_LOGIN = 'APP登录'
 
@@ -160,15 +162,15 @@
     AuthTypeIds.AUTH_TYPE_SMS.value: SmsTypeIds.SMS_TYPE_SMS_AUTH
 }
 
 plugin_topic_fmt = "%s/%s/%s"
 plugin_topics = {
     PluginTopic.P_BOOTSTRAP: MQTTTopic(PluginTopic.P_BOOTSTRAP),
     PluginTopic.P_DEV_CMD: MQTTTopic(PluginTopic.P_DEV_CMD),
-    PluginTopic.P_DEV_AUTH_CFG: MQTTTopic(PluginTopic.P_DEV_AUTH_CFG, retain=True),
+    PluginTopic.P_DEV_AUTH_CFG: MQTTTopic(PluginTopic.P_DEV_AUTH_CFG, True),
     PluginTopic.P_DEV_AUTH_KICK: MQTTTopic(PluginTopic.P_DEV_AUTH_KICK),
     PluginTopic.P_DEV_AUTH_CHECK: MQTTTopic(PluginTopic.P_DEV_AUTH_CHECK),
     PluginTopic.P_DEV_WIFI_CFG: MQTTTopic(PluginTopic.P_DEV_WIFI_CFG),
     PluginTopic.P_SVC_CFG: MQTTTopic(PluginTopic.P_SVC_CFG),
     PluginTopic.P_SVC_CMD: MQTTTopic(PluginTopic.P_SVC_CMD),
 }
```

### Comparing `utils4cpp-0.0.29/utils4cpp/flask.py` & `utils4cpp-0.0.32/utils4cpp/flask.py`

 * *Files identical despite different names*

### Comparing `utils4cpp-0.0.29/utils4cpp/models.py` & `utils4cpp-0.0.32/utils4cpp/models.py`

 * *Files identical despite different names*

### Comparing `utils4cpp-0.0.29/utils4cpp/utils.py` & `utils4cpp-0.0.32/utils4cpp/utils.py`

 * *Files identical despite different names*

