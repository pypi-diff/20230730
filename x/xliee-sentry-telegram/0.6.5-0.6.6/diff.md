# Comparing `tmp/xliee_sentry_telegram-0.6.5.tar.gz` & `tmp/xliee_sentry_telegram-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xliee_sentry_telegram-0.6.5.tar", last modified: Sun Jul 30 16:56:41 2023, max compression
+gzip compressed data, was "xliee_sentry_telegram-0.6.6.tar", last modified: Sun Jul 30 17:02:22 2023, max compression
```

## Comparing `xliee_sentry_telegram-0.6.5.tar` & `xliee_sentry_telegram-0.6.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-30 16:56:41.301664 xliee_sentry_telegram-0.6.5/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1075 2023-07-30 16:53:12.000000 xliee_sentry_telegram-0.6.5/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     2652 2023-07-30 16:56:41.301664 xliee_sentry_telegram-0.6.5/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1671 2023-07-30 16:53:12.000000 xliee_sentry_telegram-0.6.5/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-07-30 16:56:41.301664 xliee_sentry_telegram-0.6.5/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1468 2023-07-30 16:53:12.000000 xliee_sentry_telegram-0.6.5/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-30 16:56:41.301664 xliee_sentry_telegram-0.6.5/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3405 2023-07-30 16:53:12.000000 xliee_sentry_telegram-0.6.5/tests/test_base.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-30 16:56:41.301664 xliee_sentry_telegram-0.6.5/xliee_sentry_telegram/
--rw-rw-r--   0 travis    (2000) travis    (2000)      146 2023-07-30 16:53:12.000000 xliee_sentry_telegram-0.6.5/xliee_sentry_telegram/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7161 2023-07-30 16:53:12.000000 xliee_sentry_telegram-0.6.5/xliee_sentry_telegram/plugin.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-30 16:56:41.301664 xliee_sentry_telegram-0.6.5/xliee_sentry_telegram.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2652 2023-07-30 16:56:41.000000 xliee_sentry_telegram-0.6.5/xliee_sentry_telegram.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      340 2023-07-30 16:56:41.000000 xliee_sentry_telegram-0.6.5/xliee_sentry_telegram.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-30 16:56:41.000000 xliee_sentry_telegram-0.6.5/xliee_sentry_telegram.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       98 2023-07-30 16:56:41.000000 xliee_sentry_telegram-0.6.5/xliee_sentry_telegram.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2023-07-30 16:56:41.000000 xliee_sentry_telegram-0.6.5/xliee_sentry_telegram.egg-info/top_level.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-30 17:02:22.815364 xliee_sentry_telegram-0.6.6/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1075 2023-07-30 16:59:03.000000 xliee_sentry_telegram-0.6.6/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2652 2023-07-30 17:02:22.815364 xliee_sentry_telegram-0.6.6/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1671 2023-07-30 16:59:03.000000 xliee_sentry_telegram-0.6.6/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-07-30 17:02:22.815364 xliee_sentry_telegram-0.6.6/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1468 2023-07-30 16:59:03.000000 xliee_sentry_telegram-0.6.6/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-30 17:02:22.815364 xliee_sentry_telegram-0.6.6/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3405 2023-07-30 16:59:03.000000 xliee_sentry_telegram-0.6.6/tests/test_base.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-30 17:02:22.815364 xliee_sentry_telegram-0.6.6/xliee_sentry_telegram/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      146 2023-07-30 16:59:03.000000 xliee_sentry_telegram-0.6.6/xliee_sentry_telegram/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7153 2023-07-30 16:59:03.000000 xliee_sentry_telegram-0.6.6/xliee_sentry_telegram/plugin.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-30 17:02:22.815364 xliee_sentry_telegram-0.6.6/xliee_sentry_telegram.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2652 2023-07-30 17:02:22.000000 xliee_sentry_telegram-0.6.6/xliee_sentry_telegram.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      340 2023-07-30 17:02:22.000000 xliee_sentry_telegram-0.6.6/xliee_sentry_telegram.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-30 17:02:22.000000 xliee_sentry_telegram-0.6.6/xliee_sentry_telegram.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       98 2023-07-30 17:02:22.000000 xliee_sentry_telegram-0.6.6/xliee_sentry_telegram.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       22 2023-07-30 17:02:22.000000 xliee_sentry_telegram-0.6.6/xliee_sentry_telegram.egg-info/top_level.txt
```

### Comparing `xliee_sentry_telegram-0.6.5/LICENSE` & `xliee_sentry_telegram-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xliee_sentry_telegram-0.6.5/PKG-INFO` & `xliee_sentry_telegram-0.6.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xliee_sentry_telegram
-Version: 0.6.5
+Version: 0.6.6
 Summary: Plugin for Sentry which allows sending notification via Telegram messenger.
 Home-page: https://github.com/xliee/sentry-telegram
 Author: Xliee
 Author-email: info@xliee.es
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `xliee_sentry_telegram-0.6.5/README.rst` & `xliee_sentry_telegram-0.6.6/README.rst`

 * *Files identical despite different names*

### Comparing `xliee_sentry_telegram-0.6.5/setup.py` & `xliee_sentry_telegram-0.6.6/setup.py`

 * *Files identical despite different names*

### Comparing `xliee_sentry_telegram-0.6.5/tests/test_base.py` & `xliee_sentry_telegram-0.6.6/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `xliee_sentry_telegram-0.6.5/xliee_sentry_telegram/plugin.py` & `xliee_sentry_telegram-0.6.6/xliee_sentry_telegram/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         widget=forms.CheckboxInput(),
         initial=False,  
     )
 
 
 
 class TelegramNotificationsPlugin(CorePluginMixin, notify.NotificationPlugin):
-    title = 'Telegram Notifications (xliee)'
+    title = 'Telegram Notifications'
     slug = 'xliee_sentry_telegram'
     description = package_doc
     version = __version__
     author = 'xliee'
     author_url = 'https://github.com/xliee/sentry-telegram'
     resource_links = [
         ('Source', 'https://github.com/xliee/sentry-telegram'),
```

### Comparing `xliee_sentry_telegram-0.6.5/xliee_sentry_telegram.egg-info/PKG-INFO` & `xliee_sentry_telegram-0.6.6/xliee_sentry_telegram.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xliee-sentry-telegram
-Version: 0.6.5
+Version: 0.6.6
 Summary: Plugin for Sentry which allows sending notification via Telegram messenger.
 Home-page: https://github.com/xliee/sentry-telegram
 Author: Xliee
 Author-email: info@xliee.es
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

