# Comparing `tmp/xliee_sentry_telegram-0.6.4.tar.gz` & `tmp/xliee_sentry_telegram-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xliee_sentry_telegram-0.6.4.tar", last modified: Sun Jul 30 16:12:57 2023, max compression
+gzip compressed data, was "xliee_sentry_telegram-0.6.5.tar", last modified: Sun Jul 30 16:56:41 2023, max compression
```

## Comparing `xliee_sentry_telegram-0.6.4.tar` & `xliee_sentry_telegram-0.6.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-30 16:12:57.727125 xliee_sentry_telegram-0.6.4/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1075 2023-07-30 16:09:37.000000 xliee_sentry_telegram-0.6.4/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     2652 2023-07-30 16:12:57.723124 xliee_sentry_telegram-0.6.4/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1671 2023-07-30 16:09:37.000000 xliee_sentry_telegram-0.6.4/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-07-30 16:12:57.727125 xliee_sentry_telegram-0.6.4/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1468 2023-07-30 16:09:37.000000 xliee_sentry_telegram-0.6.4/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-30 16:12:57.723124 xliee_sentry_telegram-0.6.4/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3405 2023-07-30 16:09:37.000000 xliee_sentry_telegram-0.6.4/tests/test_base.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-30 16:12:57.723124 xliee_sentry_telegram-0.6.4/xliee_sentry_telegram/
--rw-rw-r--   0 travis    (2000) travis    (2000)      146 2023-07-30 16:09:37.000000 xliee_sentry_telegram-0.6.4/xliee_sentry_telegram/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7181 2023-07-30 16:09:37.000000 xliee_sentry_telegram-0.6.4/xliee_sentry_telegram/plugin.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-30 16:12:57.723124 xliee_sentry_telegram-0.6.4/xliee_sentry_telegram.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2652 2023-07-30 16:12:57.000000 xliee_sentry_telegram-0.6.4/xliee_sentry_telegram.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      340 2023-07-30 16:12:57.000000 xliee_sentry_telegram-0.6.4/xliee_sentry_telegram.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-30 16:12:57.000000 xliee_sentry_telegram-0.6.4/xliee_sentry_telegram.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       98 2023-07-30 16:12:57.000000 xliee_sentry_telegram-0.6.4/xliee_sentry_telegram.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2023-07-30 16:12:57.000000 xliee_sentry_telegram-0.6.4/xliee_sentry_telegram.egg-info/top_level.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-30 16:56:41.301664 xliee_sentry_telegram-0.6.5/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1075 2023-07-30 16:53:12.000000 xliee_sentry_telegram-0.6.5/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2652 2023-07-30 16:56:41.301664 xliee_sentry_telegram-0.6.5/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1671 2023-07-30 16:53:12.000000 xliee_sentry_telegram-0.6.5/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-07-30 16:56:41.301664 xliee_sentry_telegram-0.6.5/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1468 2023-07-30 16:53:12.000000 xliee_sentry_telegram-0.6.5/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-30 16:56:41.301664 xliee_sentry_telegram-0.6.5/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3405 2023-07-30 16:53:12.000000 xliee_sentry_telegram-0.6.5/tests/test_base.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-30 16:56:41.301664 xliee_sentry_telegram-0.6.5/xliee_sentry_telegram/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      146 2023-07-30 16:53:12.000000 xliee_sentry_telegram-0.6.5/xliee_sentry_telegram/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7161 2023-07-30 16:53:12.000000 xliee_sentry_telegram-0.6.5/xliee_sentry_telegram/plugin.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-30 16:56:41.301664 xliee_sentry_telegram-0.6.5/xliee_sentry_telegram.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2652 2023-07-30 16:56:41.000000 xliee_sentry_telegram-0.6.5/xliee_sentry_telegram.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      340 2023-07-30 16:56:41.000000 xliee_sentry_telegram-0.6.5/xliee_sentry_telegram.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-30 16:56:41.000000 xliee_sentry_telegram-0.6.5/xliee_sentry_telegram.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       98 2023-07-30 16:56:41.000000 xliee_sentry_telegram-0.6.5/xliee_sentry_telegram.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       22 2023-07-30 16:56:41.000000 xliee_sentry_telegram-0.6.5/xliee_sentry_telegram.egg-info/top_level.txt
```

### Comparing `xliee_sentry_telegram-0.6.4/LICENSE` & `xliee_sentry_telegram-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xliee_sentry_telegram-0.6.4/PKG-INFO` & `xliee_sentry_telegram-0.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xliee_sentry_telegram
-Version: 0.6.4
+Version: 0.6.5
 Summary: Plugin for Sentry which allows sending notification via Telegram messenger.
 Home-page: https://github.com/xliee/sentry-telegram
 Author: Xliee
 Author-email: info@xliee.es
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `xliee_sentry_telegram-0.6.4/README.rst` & `xliee_sentry_telegram-0.6.5/README.rst`

 * *Files identical despite different names*

### Comparing `xliee_sentry_telegram-0.6.4/setup.py` & `xliee_sentry_telegram-0.6.5/setup.py`

 * *Files identical despite different names*

### Comparing `xliee_sentry_telegram-0.6.4/tests/test_base.py` & `xliee_sentry_telegram-0.6.5/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `xliee_sentry_telegram-0.6.4/xliee_sentry_telegram/plugin.py` & `xliee_sentry_telegram-0.6.5/xliee_sentry_telegram/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,17 +36,16 @@
                     '{project_name}, {url}, {title}, {message}, {tag[%your_tag%]}'),
         initial='*[Sentry]* {project_name} {tag[level]}: *{title}*\n```{message}```\n{url}'
     )
 
     disable_web_preview = forms.BooleanField(
         label=_('Disable web preview'),
         help_text=_('Disable web preview for links in messages'),
-        required=False,
         widget=forms.CheckboxInput(),
-        initial=True,
+        initial=False,  
     )
 
 
 
 class TelegramNotificationsPlugin(CorePluginMixin, notify.NotificationPlugin):
     title = 'Telegram Notifications (xliee)'
     slug = 'xliee_sentry_telegram'
@@ -110,15 +109,15 @@
             {
                 'name': 'disable_web_preview',
                 'label': 'Disable web preview',
                 'type': 'bool',
                 'help': 'Disable web preview for links in messages',
                 'validators': [],
                 'required': False,
-                'default': True,
+                'default': False,
             },
 
         ]
 
     def build_message(self, group, event):
         the_tags = defaultdict(lambda: '[NA]')
         the_tags.update({k:v for k, v in event.tags})
```

### Comparing `xliee_sentry_telegram-0.6.4/xliee_sentry_telegram.egg-info/PKG-INFO` & `xliee_sentry_telegram-0.6.5/xliee_sentry_telegram.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xliee-sentry-telegram
-Version: 0.6.4
+Version: 0.6.5
 Summary: Plugin for Sentry which allows sending notification via Telegram messenger.
 Home-page: https://github.com/xliee/sentry-telegram
 Author: Xliee
 Author-email: info@xliee.es
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

