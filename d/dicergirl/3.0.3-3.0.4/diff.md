# Comparing `tmp/dicergirl-3.0.3.tar.gz` & `tmp/dicergirl-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicergirl-3.0.3.tar", last modified: Sat Jul 29 15:50:35 2023, max compression
+gzip compressed data, was "dicergirl-3.0.4.tar", last modified: Sun Jul 30 02:05:15 2023, max compression
```

## Comparing `dicergirl-3.0.3.tar` & `dicergirl-3.0.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 15:50:35.585603 dicergirl-3.0.3/
--rw-r--r--   0 root         (0) root         (0)    11558 2023-07-29 15:34:24.000000 dicergirl-3.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5380 2023-07-29 15:50:35.585603 dicergirl-3.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4907 2023-07-29 15:34:24.000000 dicergirl-3.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 15:50:35.581603 dicergirl-3.0.3/dicergirl/
--rw-r--r--   0 root         (0) root         (0)    17795 2023-07-29 15:45:59.000000 dicergirl-3.0.3/dicergirl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 15:50:35.581603 dicergirl-3.0.3/dicergirl/coc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-29 15:34:24.000000 dicergirl-3.0.3/dicergirl/coc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4240 2023-07-29 15:41:51.000000 dicergirl-3.0.3/dicergirl/coc/coccards.py
--rw-r--r--   0 root         (0) root         (0)     8857 2023-07-29 15:42:59.000000 dicergirl-3.0.3/dicergirl/coc/cocutils.py
--rw-r--r--   0 root         (0) root         (0)     5850 2023-07-29 15:34:24.000000 dicergirl-3.0.3/dicergirl/coc/investigator.py
--rw-r--r--   0 root         (0) root         (0)    16006 2023-07-29 15:34:24.000000 dicergirl-3.0.3/dicergirl/main.py
--rw-r--r--   0 root         (0) root         (0)     2987 2023-07-29 15:34:24.000000 dicergirl-3.0.3/dicergirl/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 15:50:35.581603 dicergirl-3.0.3/dicergirl/scp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-29 15:34:24.000000 dicergirl-3.0.3/dicergirl/scp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3168 2023-07-29 15:40:43.000000 dicergirl-3.0.3/dicergirl/scp/agent.py
--rw-r--r--   0 root         (0) root         (0)     2753 2023-07-29 15:41:00.000000 dicergirl-3.0.3/dicergirl/scp/scpcards.py
--rw-r--r--   0 root         (0) root         (0)     5038 2023-07-29 15:41:26.000000 dicergirl-3.0.3/dicergirl/scp/scputils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 15:50:35.585603 dicergirl-3.0.3/dicergirl/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-29 15:34:24.000000 dicergirl-3.0.3/dicergirl/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4326 2023-07-29 15:34:24.000000 dicergirl-3.0.3/dicergirl/utils/chat.py
--rw-r--r--   0 root         (0) root         (0)     1874 2023-07-29 15:34:24.000000 dicergirl-3.0.3/dicergirl/utils/decorators.py
--rw-r--r--   0 root         (0) root         (0)     6304 2023-07-29 15:34:24.000000 dicergirl-3.0.3/dicergirl/utils/dicer.py
--rw-r--r--   0 root         (0) root         (0)    15907 2023-07-29 15:38:26.000000 dicergirl-3.0.3/dicergirl/utils/handlers.py
--rw-r--r--   0 root         (0) root         (0)    22812 2023-07-29 15:36:29.000000 dicergirl-3.0.3/dicergirl/utils/messages.py
--rw-r--r--   0 root         (0) root         (0)     1193 2023-07-29 15:34:24.000000 dicergirl-3.0.3/dicergirl/utils/settings.py
--rw-r--r--   0 root         (0) root         (0)     4676 2023-07-29 15:48:22.000000 dicergirl-3.0.3/dicergirl/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 15:50:35.581603 dicergirl-3.0.3/dicergirl.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5380 2023-07-29 15:50:35.000000 dicergirl-3.0.3/dicergirl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      672 2023-07-29 15:50:35.000000 dicergirl-3.0.3/dicergirl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 15:50:35.000000 dicergirl-3.0.3/dicergirl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-29 15:50:35.000000 dicergirl-3.0.3/dicergirl.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-29 15:50:35.000000 dicergirl-3.0.3/dicergirl.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-29 15:50:35.585603 dicergirl-3.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1044 2023-07-29 15:34:24.000000 dicergirl-3.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 02:05:15.976572 dicergirl-3.0.4/
+-rw-r--r--   0 root         (0) root         (0)    11558 2023-07-30 01:54:59.000000 dicergirl-3.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5361 2023-07-30 02:05:15.976572 dicergirl-3.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4907 2023-07-30 01:54:59.000000 dicergirl-3.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 02:05:15.944571 dicergirl-3.0.4/dicergirl/
+-rw-r--r--   0 root         (0) root         (0)    17860 2023-07-30 02:03:36.000000 dicergirl-3.0.4/dicergirl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 02:05:15.952571 dicergirl-3.0.4/dicergirl/coc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-30 01:55:34.000000 dicergirl-3.0.4/dicergirl/coc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4240 2023-07-30 01:55:34.000000 dicergirl-3.0.4/dicergirl/coc/coccards.py
+-rw-r--r--   0 root         (0) root         (0)     8857 2023-07-30 01:55:34.000000 dicergirl-3.0.4/dicergirl/coc/cocutils.py
+-rw-r--r--   0 root         (0) root         (0)     5850 2023-07-30 01:55:34.000000 dicergirl-3.0.4/dicergirl/coc/investigator.py
+-rw-r--r--   0 root         (0) root         (0)    16006 2023-07-30 01:55:34.000000 dicergirl-3.0.4/dicergirl/main.py
+-rw-r--r--   0 root         (0) root         (0)     2987 2023-07-30 01:55:34.000000 dicergirl-3.0.4/dicergirl/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 02:05:15.956571 dicergirl-3.0.4/dicergirl/scp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-30 01:55:34.000000 dicergirl-3.0.4/dicergirl/scp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3168 2023-07-30 01:55:34.000000 dicergirl-3.0.4/dicergirl/scp/agent.py
+-rw-r--r--   0 root         (0) root         (0)     2753 2023-07-30 01:55:34.000000 dicergirl-3.0.4/dicergirl/scp/scpcards.py
+-rw-r--r--   0 root         (0) root         (0)     5038 2023-07-30 01:55:34.000000 dicergirl-3.0.4/dicergirl/scp/scputils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 02:05:15.972572 dicergirl-3.0.4/dicergirl/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-30 01:55:34.000000 dicergirl-3.0.4/dicergirl/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4326 2023-07-30 01:55:34.000000 dicergirl-3.0.4/dicergirl/utils/chat.py
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-07-30 01:55:34.000000 dicergirl-3.0.4/dicergirl/utils/decorators.py
+-rw-r--r--   0 root         (0) root         (0)     6304 2023-07-30 01:55:34.000000 dicergirl-3.0.4/dicergirl/utils/dicer.py
+-rw-r--r--   0 root         (0) root         (0)    15907 2023-07-30 01:55:34.000000 dicergirl-3.0.4/dicergirl/utils/handlers.py
+-rw-r--r--   0 root         (0) root         (0)    22812 2023-07-30 01:55:34.000000 dicergirl-3.0.4/dicergirl/utils/messages.py
+-rw-r--r--   0 root         (0) root         (0)     1193 2023-07-30 01:55:34.000000 dicergirl-3.0.4/dicergirl/utils/settings.py
+-rw-r--r--   0 root         (0) root         (0)     5053 2023-07-30 02:05:13.000000 dicergirl-3.0.4/dicergirl/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 02:05:15.948571 dicergirl-3.0.4/dicergirl.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5361 2023-07-30 02:05:15.000000 dicergirl-3.0.4/dicergirl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      672 2023-07-30 02:05:15.000000 dicergirl-3.0.4/dicergirl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-30 02:05:15.000000 dicergirl-3.0.4/dicergirl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-30 02:05:15.000000 dicergirl-3.0.4/dicergirl.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-30 02:05:15.000000 dicergirl-3.0.4/dicergirl.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-30 02:05:15.976572 dicergirl-3.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1056 2023-07-30 01:58:01.000000 dicergirl-3.0.4/setup.py
```

### Comparing `dicergirl-3.0.3/LICENSE` & `dicergirl-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.3/PKG-INFO` & `dicergirl-3.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: dicergirl
-Version: 3.0.3
+Version: 3.0.4
 Summary: 跑团骰娘机器人欧若可, 支持 QQ频道 及 Nonebot2 部署.
 Home-page: https://gitee.com/unvisitor/dicer
 Author: Night Resurgent <fu050409@163.com>
 Author-email: fu050409@163.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://gitee.com/unvisitor/dicer/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -126,8 +125,7 @@
 ## 使用
 你可以在部署完成后, 在相应的 QQ 群或者 QQ 频道发送消息`.help`来查看使用方法.
 
 目前已兼容 COC 跑团与 SCP 跑团的大部分指令.
 
 ## 声明
 此项目由 Apache-2.0 协议开源, 使用代码时, 请注意遵照开源协议.
-
```

### Comparing `dicergirl-3.0.3/README.md` & `dicergirl-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.3/dicergirl/__init__.py` & `dicergirl-3.0.4/dicergirl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,12 @@
 from pathlib import Path
 from loguru import logger
 
 from .utils.settings import set_package, package
-from .coc.investigator import Investigator
-from .scp.agent import Agent
-from .coc.cocutils import sc, st, at, dam, en, rd0, ra, ti, li, rb, rp
-from .coc.coccards import cards, cache_cards, sa_handler
-from .scp.scpcards import scp_cards, scp_cache_cards
-from .scp.scputils import sra, scp_dam, at as sat
-from .utils.messages import help_message, version
-from .utils.utils import logger as _log, init, is_super_user, add_super_user, rm_super_user, su_uuid, format_msg, format_str, version
-from .utils.handlers import scp_set_handler, scp_show_handler, scp_del_handler, set_handler, show_handler, del_handler
-from .utils.chat import chat
+from .utils.utils import version
 
 import logging
 import nonebot
 import sys
 
 DEBUG = False
 current_dir = Path(__file__).resolve().parent
@@ -26,14 +17,25 @@
     set_package("nonebot2")
 except ValueError:
     utilless = True
 else:
     utilless = False
 
 if package == "nonebot2" and not utilless:
+    from .coc.investigator import Investigator
+    from .scp.agent import Agent
+    from .coc.cocutils import sc, st, at, dam, en, rd0, ra, ti, li, rb, rp
+    from .coc.coccards import cards, cache_cards, sa_handler
+    from .scp.scpcards import scp_cards, scp_cache_cards
+    from .scp.scputils import sra, scp_dam, at as sat
+    from .utils.messages import help_message
+    from .utils.utils import logger as _log, init, is_super_user, add_super_user, rm_super_user, su_uuid, format_msg, format_str, version
+    from .utils.handlers import scp_set_handler, scp_show_handler, scp_del_handler, set_handler, show_handler, del_handler
+    from .utils.chat import chat
+
     from nonebot.rule import Rule
     from nonebot.matcher import Matcher
     from nonebot.plugin import on_startswith
     from nonebot.adapters import Bot as Bot
     from nonebot.adapters.onebot.v11 import Bot as V11Bot
     from nonebot.adapters.onebot.v12 import Bot as V12Bot
```

### Comparing `dicergirl-3.0.3/dicergirl/coc/coccards.py` & `dicergirl-3.0.4/dicergirl/coc/coccards.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.3/dicergirl/coc/cocutils.py` & `dicergirl-3.0.4/dicergirl/coc/cocutils.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.3/dicergirl/coc/investigator.py` & `dicergirl-3.0.4/dicergirl/coc/investigator.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.3/dicergirl/main.py` & `dicergirl-3.0.4/dicergirl/main.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.3/dicergirl/run.py` & `dicergirl-3.0.4/dicergirl/run.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.3/dicergirl/scp/agent.py` & `dicergirl-3.0.4/dicergirl/scp/agent.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.3/dicergirl/scp/scpcards.py` & `dicergirl-3.0.4/dicergirl/scp/scpcards.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.3/dicergirl/scp/scputils.py` & `dicergirl-3.0.4/dicergirl/scp/scputils.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.3/dicergirl/utils/chat.py` & `dicergirl-3.0.4/dicergirl/utils/chat.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.3/dicergirl/utils/decorators.py` & `dicergirl-3.0.4/dicergirl/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.3/dicergirl/utils/dicer.py` & `dicergirl-3.0.4/dicergirl/utils/dicer.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.3/dicergirl/utils/handlers.py` & `dicergirl-3.0.4/dicergirl/utils/handlers.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.3/dicergirl/utils/messages.py` & `dicergirl-3.0.4/dicergirl/utils/messages.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.3/dicergirl/utils/settings.py` & `dicergirl-3.0.4/dicergirl/utils/settings.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.3/dicergirl/utils/utils.py` & `dicergirl-3.0.4/dicergirl/utils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,35 @@
     from dicergirl.utils.decorators import translate_punctuation
     from dicergirl.utils.settings import package, setconfig, getconfig
 except ImportError:
     from .decorators import translate_punctuation
     from .settings import package, setconfig, getconfig
 
 if package == "nonebot2":
-    from nonebot.adapters.onebot.v11 import MessageEvent, GroupMessageEvent
     class Message:
         pass
+    try:
+        from nonebot.adapters.onebot.v11 import MessageEvent, GroupMessageEvent
+    except ModuleNotFoundError:
+        logger.warning("未找到依赖`Nonebot2`, 请检查你的配置.")
+        class MessageEvent:
+            pass
+        class GroupMessageEvent:
+            pass
 elif package == "qqguild":
-    from botpy.message import Message
     class MessageEvent:
         pass
     class GroupMessageEvent:
         pass
+    try:
+        from botpy.message import Message
+    except ModuleNotFoundError:
+        logger.warning("未找到依赖`qq-botpy`, 请检查你的配置.")
+        class Message:
+            pass
 
 import json
 import os
 import uuid
 import re
 import inspect
 
@@ -30,15 +42,15 @@
 dicer_girl_dir = Path.home() / ".dicergirl"
 data_dir = dicer_girl_dir / "data"
 _coc_cachepath = data_dir / "coc_cards.json"
 _scp_cachepath = data_dir / "scp_cards.json"
 _super_user = data_dir / "super_user.json"
 _log = logger
 su_uuid = (str(uuid.uuid1()) + str(uuid.uuid4())).replace("-", "")
-version = "3.0.3"
+version = "3.0.4"
 
 def init():
     if not dicer_girl_dir.exists():
         _log.info("Dicer Girl 文件夹未建立, 建立它.")
         dicer_girl_dir.mkdir()
     if not data_dir.exists():
         _log.info("Dicer Girl 数据文件夹未建立, 建立它.")
```

### Comparing `dicergirl-3.0.3/dicergirl.egg-info/PKG-INFO` & `dicergirl-3.0.4/dicergirl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: dicergirl
-Version: 3.0.3
+Version: 3.0.4
 Summary: 跑团骰娘机器人欧若可, 支持 QQ频道 及 Nonebot2 部署.
 Home-page: https://gitee.com/unvisitor/dicer
 Author: Night Resurgent <fu050409@163.com>
 Author-email: fu050409@163.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://gitee.com/unvisitor/dicer/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -126,8 +125,7 @@
 ## 使用
 你可以在部署完成后, 在相应的 QQ 群或者 QQ 频道发送消息`.help`来查看使用方法.
 
 目前已兼容 COC 跑团与 SCP 跑团的大部分指令.
 
 ## 声明
 此项目由 Apache-2.0 协议开源, 使用代码时, 请注意遵照开源协议.
-
```

### Comparing `dicergirl-3.0.3/dicergirl.egg-info/SOURCES.txt` & `dicergirl-3.0.4/dicergirl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.3/setup.py` & `dicergirl-3.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dicergirl import version
+from dicergirl.utils.utils import version
 
 import setuptools
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
```

