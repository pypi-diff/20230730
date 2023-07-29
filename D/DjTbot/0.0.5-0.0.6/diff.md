# Comparing `tmp/DjTbot-0.0.5.tar.gz` & `tmp/DjTbot-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\DjTbot-0.0.5.tar", last modified: Sat Jul 29 20:44:07 2023, max compression
+gzip compressed data, was "dist\DjTbot-0.0.6.tar", last modified: Sat Jul 29 22:02:03 2023, max compression
```

## Comparing `DjTbot-0.0.5.tar` & `DjTbot-0.0.6.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 20:44:07.150381 DjTbot-0.0.5/
-drwxrwxrwx   0        0        0        0 2023-07-29 20:44:06.677742 DjTbot-0.0.5/DjTbot/
--rw-rw-rw-   0        0        0        0 2023-07-29 18:39:20.000000 DjTbot-0.0.5/DjTbot/__init__.py
--rw-rw-rw-   0        0        0      375 2023-07-29 18:46:39.000000 DjTbot-0.0.5/DjTbot/admin.py
--rw-rw-rw-   0        0        0      602 2023-07-29 18:46:39.000000 DjTbot-0.0.5/DjTbot/arguments.py
--rw-rw-rw-   0        0        0     3146 2023-07-29 18:46:39.000000 DjTbot-0.0.5/DjTbot/commands.py
-drwxrwxrwx   0        0        0        0 2023-07-29 20:44:06.897732 DjTbot-0.0.5/DjTbot/core/
--rw-rw-rw-   0        0        0        0 2023-07-29 18:05:12.000000 DjTbot-0.0.5/DjTbot/core/__init__.py
--rw-rw-rw-   0        0        0      620 2023-07-29 18:05:21.000000 DjTbot-0.0.5/DjTbot/core/argumentparser.py
--rw-rw-rw-   0        0        0     4695 2023-07-29 18:42:49.000000 DjTbot-0.0.5/DjTbot/core/commands.py
--rw-rw-rw-   0        0        0      188 2023-07-29 20:23:29.000000 DjTbot-0.0.5/DjTbot/core/errors.py
--rw-rw-rw-   0        0        0     3747 2023-07-29 18:06:27.000000 DjTbot-0.0.5/DjTbot/core/giphy.py
--rw-rw-rw-   0        0        0      321 2023-07-29 18:46:39.000000 DjTbot-0.0.5/DjTbot/core/listeners.py
--rw-rw-rw-   0        0        0      591 2023-07-29 18:07:09.000000 DjTbot-0.0.5/DjTbot/core/network.py
--rw-rw-rw-   0        0        0     3350 2023-07-29 18:46:39.000000 DjTbot-0.0.5/DjTbot/core/telegram_lib.py
-drwxrwxrwx   0        0        0        0 2023-07-29 20:44:06.898733 DjTbot-0.0.5/DjTbot/management/
--rw-rw-rw-   0        0        0        0 2023-07-29 18:08:30.000000 DjTbot-0.0.5/DjTbot/management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 20:44:07.131292 DjTbot-0.0.5/DjTbot/management/commands/
--rw-rw-rw-   0        0        0        0 2023-07-29 18:08:48.000000 DjTbot-0.0.5/DjTbot/management/commands/__init__.py
--rw-rw-rw-   0        0        0      339 2023-07-29 18:46:39.000000 DjTbot-0.0.5/DjTbot/management/commands/addgroup.py
--rw-rw-rw-   0        0        0      398 2023-07-29 18:46:39.000000 DjTbot-0.0.5/DjTbot/management/commands/adduser.py
--rw-rw-rw-   0        0        0      489 2023-07-29 18:46:39.000000 DjTbot-0.0.5/DjTbot/management/commands/addusertogroup.py
--rw-rw-rw-   0        0        0      489 2023-07-29 18:10:06.000000 DjTbot-0.0.5/DjTbot/management/commands/clear_api_key.py
--rw-rw-rw-   0        0        0      472 2023-07-29 18:46:39.000000 DjTbot-0.0.5/DjTbot/management/commands/createbotadmin.py
--rw-rw-rw-   0        0        0      325 2023-07-29 18:46:39.000000 DjTbot-0.0.5/DjTbot/management/commands/lsgroups.py
--rw-rw-rw-   0        0        0      317 2023-07-29 18:46:39.000000 DjTbot-0.0.5/DjTbot/management/commands/lsusers.py
--rw-rw-rw-   0        0        0      497 2023-07-29 18:46:39.000000 DjTbot-0.0.5/DjTbot/management/commands/removeuserfromgroup.py
--rw-rw-rw-   0        0        0      415 2023-07-29 18:46:39.000000 DjTbot-0.0.5/DjTbot/management/commands/rmgroup.py
--rw-rw-rw-   0        0        0      414 2023-07-29 18:46:39.000000 DjTbot-0.0.5/DjTbot/management/commands/rmuser.py
--rw-rw-rw-   0        0        0     1245 2023-07-29 20:42:47.000000 DjTbot-0.0.5/DjTbot/management/commands/runbot.py
--rw-rw-rw-   0        0        0     1769 2023-07-29 18:46:39.000000 DjTbot-0.0.5/DjTbot/management/commands/sendmessage.py
-drwxrwxrwx   0        0        0        0 2023-07-29 20:44:07.149382 DjTbot-0.0.5/DjTbot/migrations/
--rw-rw-rw-   0        0        0      868 2023-07-29 20:23:29.000000 DjTbot-0.0.5/DjTbot/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-07-29 18:14:38.000000 DjTbot-0.0.5/DjTbot/migrations/__init__.py
--rw-rw-rw-   0        0        0      423 2023-07-29 18:02:41.000000 DjTbot-0.0.5/DjTbot/models.py
--rw-rw-rw-   0        0        0     2102 2023-07-29 20:17:46.000000 DjTbot-0.0.5/DjTbot/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-29 20:44:06.727647 DjTbot-0.0.5/DjTbot.egg-info/
--rw-rw-rw-   0        0        0     5847 2023-07-29 20:44:06.000000 DjTbot-0.0.5/DjTbot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1106 2023-07-29 20:44:06.000000 DjTbot-0.0.5/DjTbot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 20:44:06.000000 DjTbot-0.0.5/DjTbot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2023-07-29 20:44:06.000000 DjTbot-0.0.5/DjTbot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-29 20:44:06.000000 DjTbot-0.0.5/DjTbot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5847 2023-07-29 20:44:07.150381 DjTbot-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     5050 2023-07-29 18:40:39.000000 DjTbot-0.0.5/README.md
--rw-rw-rw-   0        0        0       86 2023-07-29 20:44:07.152421 DjTbot-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     2290 2023-07-29 20:43:31.000000 DjTbot-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 22:02:03.472982 DjTbot-0.0.6/
+drwxrwxrwx   0        0        0        0 2023-07-29 22:02:02.999732 DjTbot-0.0.6/DjTbot/
+-rw-rw-rw-   0        0        0        0 2023-07-29 18:39:20.000000 DjTbot-0.0.6/DjTbot/__init__.py
+-rw-rw-rw-   0        0        0      375 2023-07-29 18:46:39.000000 DjTbot-0.0.6/DjTbot/admin.py
+-rw-rw-rw-   0        0        0      602 2023-07-29 18:46:39.000000 DjTbot-0.0.6/DjTbot/arguments.py
+-rw-rw-rw-   0        0        0     3149 2023-07-29 21:41:24.000000 DjTbot-0.0.6/DjTbot/commands.py
+drwxrwxrwx   0        0        0        0 2023-07-29 22:02:03.153572 DjTbot-0.0.6/DjTbot/core/
+-rw-rw-rw-   0        0        0        0 2023-07-29 18:05:12.000000 DjTbot-0.0.6/DjTbot/core/__init__.py
+-rw-rw-rw-   0        0        0      620 2023-07-29 18:05:21.000000 DjTbot-0.0.6/DjTbot/core/argumentparser.py
+-rw-rw-rw-   0        0        0     4753 2023-07-29 22:00:22.000000 DjTbot-0.0.6/DjTbot/core/commands.py
+-rw-rw-rw-   0        0        0      188 2023-07-29 20:23:29.000000 DjTbot-0.0.6/DjTbot/core/errors.py
+-rw-rw-rw-   0        0        0     3747 2023-07-29 18:06:27.000000 DjTbot-0.0.6/DjTbot/core/giphy.py
+-rw-rw-rw-   0        0        0      321 2023-07-29 18:46:39.000000 DjTbot-0.0.6/DjTbot/core/listeners.py
+-rw-rw-rw-   0        0        0      591 2023-07-29 18:07:09.000000 DjTbot-0.0.6/DjTbot/core/network.py
+-rw-rw-rw-   0        0        0     3727 2023-07-29 21:48:48.000000 DjTbot-0.0.6/DjTbot/core/telegram_lib.py
+drwxrwxrwx   0        0        0        0 2023-07-29 22:02:03.155614 DjTbot-0.0.6/DjTbot/management/
+-rw-rw-rw-   0        0        0        0 2023-07-29 18:08:30.000000 DjTbot-0.0.6/DjTbot/management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 22:02:03.457170 DjTbot-0.0.6/DjTbot/management/commands/
+-rw-rw-rw-   0        0        0        0 2023-07-29 18:08:48.000000 DjTbot-0.0.6/DjTbot/management/commands/__init__.py
+-rw-rw-rw-   0        0        0      339 2023-07-29 18:46:39.000000 DjTbot-0.0.6/DjTbot/management/commands/addgroup.py
+-rw-rw-rw-   0        0        0      398 2023-07-29 18:46:39.000000 DjTbot-0.0.6/DjTbot/management/commands/adduser.py
+-rw-rw-rw-   0        0        0      489 2023-07-29 18:46:39.000000 DjTbot-0.0.6/DjTbot/management/commands/addusertogroup.py
+-rw-rw-rw-   0        0        0      489 2023-07-29 18:10:06.000000 DjTbot-0.0.6/DjTbot/management/commands/clear_api_key.py
+-rw-rw-rw-   0        0        0      472 2023-07-29 18:46:39.000000 DjTbot-0.0.6/DjTbot/management/commands/createbotadmin.py
+-rw-rw-rw-   0        0        0      325 2023-07-29 18:46:39.000000 DjTbot-0.0.6/DjTbot/management/commands/lsgroups.py
+-rw-rw-rw-   0        0        0      317 2023-07-29 18:46:39.000000 DjTbot-0.0.6/DjTbot/management/commands/lsusers.py
+-rw-rw-rw-   0        0        0      497 2023-07-29 18:46:39.000000 DjTbot-0.0.6/DjTbot/management/commands/removeuserfromgroup.py
+-rw-rw-rw-   0        0        0      415 2023-07-29 18:46:39.000000 DjTbot-0.0.6/DjTbot/management/commands/rmgroup.py
+-rw-rw-rw-   0        0        0      414 2023-07-29 18:46:39.000000 DjTbot-0.0.6/DjTbot/management/commands/rmuser.py
+-rw-rw-rw-   0        0        0     1194 2023-07-29 20:55:21.000000 DjTbot-0.0.6/DjTbot/management/commands/runbot.py
+-rw-rw-rw-   0        0        0     1769 2023-07-29 18:46:39.000000 DjTbot-0.0.6/DjTbot/management/commands/sendmessage.py
+drwxrwxrwx   0        0        0        0 2023-07-29 22:02:03.471982 DjTbot-0.0.6/DjTbot/migrations/
+-rw-rw-rw-   0        0        0      868 2023-07-29 20:23:29.000000 DjTbot-0.0.6/DjTbot/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-07-29 18:14:38.000000 DjTbot-0.0.6/DjTbot/migrations/__init__.py
+-rw-rw-rw-   0        0        0      423 2023-07-29 18:02:41.000000 DjTbot-0.0.6/DjTbot/models.py
+-rw-rw-rw-   0        0        0     2102 2023-07-29 20:17:46.000000 DjTbot-0.0.6/DjTbot/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-29 22:02:03.027361 DjTbot-0.0.6/DjTbot.egg-info/
+-rw-rw-rw-   0        0        0     5847 2023-07-29 22:02:02.000000 DjTbot-0.0.6/DjTbot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1106 2023-07-29 22:02:02.000000 DjTbot-0.0.6/DjTbot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 22:02:02.000000 DjTbot-0.0.6/DjTbot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-07-29 22:02:02.000000 DjTbot-0.0.6/DjTbot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-29 22:02:02.000000 DjTbot-0.0.6/DjTbot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5847 2023-07-29 22:02:03.472982 DjTbot-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5050 2023-07-29 18:40:39.000000 DjTbot-0.0.6/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-29 22:02:03.475067 DjTbot-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     2365 2023-07-29 22:01:41.000000 DjTbot-0.0.6/setup.py
```

### Comparing `DjTbot-0.0.5/DjTbot/arguments.py` & `DjTbot-0.0.6/DjTbot/arguments.py`

 * *Files identical despite different names*

### Comparing `DjTbot-0.0.5/DjTbot/commands.py` & `DjTbot-0.0.6/DjTbot/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
-from core.commands import Command, HELP, CommandWithArgumentsMixin
+from .core.commands import Command, HELP, CommandWithArgumentsMixin
 from .arguments import TBotArgumentParser
 from DjTbot.utils import get_group_members, create_user, addgroup, get_user
 from DjTbot.models import TBotUser
 
 
-logger = logging.getLogger("tbot")
+logger = logging.getLogger("DjTbot")
 # Todo: Refactor with CommandWithArgumentsMixin
 # Todo: Delete user
 # Todo: Remove user from group
 
 
 # Todo: Refactor with TBotCommandWithArgumentsMixin
 class TBotCommandWithArgumentsMixin(CommandWithArgumentsMixin):
```

### Comparing `DjTbot-0.0.5/DjTbot/core/argumentparser.py` & `DjTbot-0.0.6/DjTbot/core/argumentparser.py`

 * *Files identical despite different names*

### Comparing `DjTbot-0.0.5/DjTbot/core/commands.py` & `DjTbot-0.0.6/DjTbot/core/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import random
 from abc import ABCMeta, abstractmethod
 from .errors import TelegramBotError, MethodNotDefinedError
 from .giphy import giphy
-from DjTbot.utils import get_group_members, get_user_groups
+from DjTbot.utils import get_group_members, get_user_groups, get_all_ids
 
 logger = logging.getLogger("tbot")
 
 HELP = {}
 
 
 class AuthorizedCommand(object, metaclass=ABCMeta):
@@ -29,15 +29,16 @@
         bot.sendDocument(document=self.denied_giphy(), chat_id=chat_id)
         unauthorized_message = 'Unauthorized access: chat_id = {}'.format(chat_id)
         self.admin_broadcast(bot, unauthorized_message)
         logger.warning(unauthorized_message)
 
     def authorized(self, chat_id):
         if chat_id in self.restricted_to or '*' in self.allowed_groups:
-            return True
+            if chat_id in get_all_ids():
+                return True
         return False
 
     def denied_giphy(self):
         if self.denied_giphy_set:
             return self.random_giphy(self.denied_giphy_set)
         else:
             return self.random_giphy()
```

### Comparing `DjTbot-0.0.5/DjTbot/core/giphy.py` & `DjTbot-0.0.6/DjTbot/core/giphy.py`

 * *Files identical despite different names*

### Comparing `DjTbot-0.0.5/DjTbot/core/network.py` & `DjTbot-0.0.6/DjTbot/core/network.py`

 * *Files identical despite different names*

### Comparing `DjTbot-0.0.5/DjTbot/core/telegram_lib.py` & `DjTbot-0.0.6/DjTbot/core/telegram_lib.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,25 +6,40 @@
 from .network import wait_for_internet
 from .commands import Command, HELP
 from .listeners import Listener
 from telegram.ext import Updater, CommandHandler, MessageHandler
 from django.conf import settings
 from DjTbot.utils import get_group_members
 
-for app in settings.INSTALLED_APPS:
+logger = logging.getLogger("DjTbot")
+
+
+def load_app_commands(app):
     try:
         import_module(app + '.commands')
+        logger.info(f'Loaded telegram commands from {app}')
     except ModuleNotFoundError:
-        pass
+        logger.debug(f'No commands found in {app}')
+
+
+def load_app_listeners(app):
     try:
         import_module(app + '.listeners')
+        logger.info(f'Loaded telegram listeners from {app}')
     except ModuleNotFoundError:
-        pass
+        logger.debug(f'No commands found in {app}')
+
+
+def load_app_handlers():
+    for app in settings.INSTALLED_APPS:
+        load_app_commands(app)
+        load_app_listeners(app)
+
 
-logger = logging.getLogger("tbot")
+load_app_handlers()
 
 
 class Bot(object):
     def __init__(self, api_key, http_proxy=None, daemon=True):
         if http_proxy:
             self.updater = Updater(token=api_key, request_kwargs=self.proxy(http_proxy), use_context=True)
         else:
```

### Comparing `DjTbot-0.0.5/DjTbot/management/commands/runbot.py` & `DjTbot-0.0.6/DjTbot/management/commands/runbot.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from django.core.management.base import BaseCommand
 import logging
 from django.conf import settings
 from DjTbot.core.telegram_lib import Bot
 from DjTbot.core.errors import ConfigurationError
 from DjTbot.utils import setting_or_env
 
-logger = logging.getLogger("{{ cookiecutter.project_name|lower()|replace(' ', '_') }}")
+logger = logging.getLogger("DjTbot")
 
 
 class Command(BaseCommand):
     help = """
     Run your bot, there can only be one running command
     """
```

### Comparing `DjTbot-0.0.5/DjTbot/management/commands/sendmessage.py` & `DjTbot-0.0.6/DjTbot/management/commands/sendmessage.py`

 * *Files identical despite different names*

### Comparing `DjTbot-0.0.5/DjTbot/migrations/0001_initial.py` & `DjTbot-0.0.6/DjTbot/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `DjTbot-0.0.5/DjTbot/utils.py` & `DjTbot-0.0.6/DjTbot/utils.py`

 * *Files identical despite different names*

### Comparing `DjTbot-0.0.5/DjTbot.egg-info/PKG-INFO` & `DjTbot-0.0.6/DjTbot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DjTbot
-Version: 0.0.5
+Version: 0.0.6
 Summary: Django Telegram Bot
 Home-page: https://git.herrerosolis.com/bots/DjTbot
 Download-URL: https://git.herrerosolis.com/bots/DjTbot/-/archive/master/DjTbot-master.tar.gz
 Author: Rafael Herrero Solis
 Author-email: rafahsolis@hotmail.com
 License: License :: OSI Approved :: MIT License
 Keywords: Django,Telegram,Bot
```

### Comparing `DjTbot-0.0.5/DjTbot.egg-info/SOURCES.txt` & `DjTbot-0.0.6/DjTbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DjTbot-0.0.5/PKG-INFO` & `DjTbot-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DjTbot
-Version: 0.0.5
+Version: 0.0.6
 Summary: Django Telegram Bot
 Home-page: https://git.herrerosolis.com/bots/DjTbot
 Download-URL: https://git.herrerosolis.com/bots/DjTbot/-/archive/master/DjTbot-master.tar.gz
 Author: Rafael Herrero Solis
 Author-email: rafahsolis@hotmail.com
 License: License :: OSI Approved :: MIT License
 Keywords: Django,Telegram,Bot
```

### Comparing `DjTbot-0.0.5/README.md` & `DjTbot-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `DjTbot-0.0.5/setup.py` & `DjTbot-0.0.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 import os
 from setuptools import setup, find_packages
 
-__version__ = '0.0.5'
+__version__ = '0.0.6'
 
 """
+Upload to pypi:
 python setup.py sdist bdist_wheel
 python -m twine upload dist/*
 """
 
+"""
+Developer mode install
+python -m pip install -e .
+"""
+
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 
 def here(name):
     return os.path.join(
         os.path.dirname(os.path.abspath(__file__)),
```

