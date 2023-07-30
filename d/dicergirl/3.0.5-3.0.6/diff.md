# Comparing `tmp/dicergirl-3.0.5.tar.gz` & `tmp/dicergirl-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicergirl-3.0.5.tar", last modified: Sun Jul 30 06:43:58 2023, max compression
+gzip compressed data, was "dicergirl-3.0.6.tar", last modified: Sun Jul 30 07:01:15 2023, max compression
```

## Comparing `dicergirl-3.0.5.tar` & `dicergirl-3.0.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 06:43:58.623759 dicergirl-3.0.5/
--rw-rw-rw-   0        0        0    11558 2023-07-29 07:34:15.000000 dicergirl-3.0.5/LICENSE
--rw-rw-rw-   0        0        0     9351 2023-07-30 06:43:58.622761 dicergirl-3.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     8766 2023-07-30 06:15:15.000000 dicergirl-3.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 06:43:58.567721 dicergirl-3.0.5/dicergirl/
--rw-rw-rw-   0        0        0    18998 2023-07-30 05:42:11.000000 dicergirl-3.0.5/dicergirl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 06:43:58.609752 dicergirl-3.0.5/dicergirl/coc/
--rw-rw-rw-   0        0        0        0 2023-07-29 07:34:15.000000 dicergirl-3.0.5/dicergirl/coc/__init__.py
--rw-rw-rw-   0        0        0     4362 2023-07-30 05:42:11.000000 dicergirl-3.0.5/dicergirl/coc/coccards.py
--rw-rw-rw-   0        0        0     9147 2023-07-30 05:42:11.000000 dicergirl-3.0.5/dicergirl/coc/cocutils.py
--rw-rw-rw-   0        0        0     6020 2023-07-29 10:23:31.000000 dicergirl-3.0.5/dicergirl/coc/investigator.py
--rw-rw-rw-   0        0        0    16499 2023-07-30 05:42:11.000000 dicergirl-3.0.5/dicergirl/main.py
--rw-rw-rw-   0        0        0     3081 2023-07-29 11:48:51.000000 dicergirl-3.0.5/dicergirl/run.py
-drwxrwxrwx   0        0        0        0 2023-07-30 06:43:58.612760 dicergirl-3.0.5/dicergirl/scp/
--rw-rw-rw-   0        0        0        0 2023-07-29 07:34:15.000000 dicergirl-3.0.5/dicergirl/scp/__init__.py
--rw-rw-rw-   0        0        0     3285 2023-07-30 05:42:11.000000 dicergirl-3.0.5/dicergirl/scp/agent.py
--rw-rw-rw-   0        0        0     2832 2023-07-30 05:42:11.000000 dicergirl-3.0.5/dicergirl/scp/scpcards.py
--rw-rw-rw-   0        0        0     5191 2023-07-30 05:42:11.000000 dicergirl-3.0.5/dicergirl/scp/scputils.py
-drwxrwxrwx   0        0        0        0 2023-07-30 06:43:58.621760 dicergirl-3.0.5/dicergirl/utils/
--rw-rw-rw-   0        0        0        0 2023-07-29 07:34:15.000000 dicergirl-3.0.5/dicergirl/utils/__init__.py
--rw-rw-rw-   0        0        0     4384 2023-07-29 07:34:15.000000 dicergirl-3.0.5/dicergirl/utils/chat.py
--rw-rw-rw-   0        0        0     1934 2023-07-29 07:34:15.000000 dicergirl-3.0.5/dicergirl/utils/decorators.py
--rw-rw-rw-   0        0        0     7129 2023-07-30 06:42:58.000000 dicergirl-3.0.5/dicergirl/utils/dicer.py
--rw-rw-rw-   0        0        0    16252 2023-07-30 05:42:11.000000 dicergirl-3.0.5/dicergirl/utils/handlers.py
--rw-rw-rw-   0        0        0    23148 2023-07-30 05:42:11.000000 dicergirl-3.0.5/dicergirl/utils/messages.py
--rw-rw-rw-   0        0        0     1275 2023-07-30 05:42:11.000000 dicergirl-3.0.5/dicergirl/utils/settings.py
--rw-rw-rw-   0        0        0     5220 2023-07-30 06:16:09.000000 dicergirl-3.0.5/dicergirl/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-30 06:43:58.605311 dicergirl-3.0.5/dicergirl.egg-info/
--rw-rw-rw-   0        0        0     9351 2023-07-30 06:43:58.000000 dicergirl-3.0.5/dicergirl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      672 2023-07-30 06:43:58.000000 dicergirl-3.0.5/dicergirl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 06:43:58.000000 dicergirl-3.0.5/dicergirl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-07-30 06:43:58.000000 dicergirl-3.0.5/dicergirl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-30 06:43:58.000000 dicergirl-3.0.5/dicergirl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-30 06:43:58.623759 dicergirl-3.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1093 2023-07-30 05:42:11.000000 dicergirl-3.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:01:15.314479 dicergirl-3.0.6/
+-rw-rw-rw-   0        0        0    11558 2023-07-29 07:34:15.000000 dicergirl-3.0.6/LICENSE
+-rw-rw-rw-   0        0        0     9351 2023-07-30 07:01:15.314479 dicergirl-3.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     8766 2023-07-30 06:15:15.000000 dicergirl-3.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 07:01:15.283583 dicergirl-3.0.6/dicergirl/
+-rw-rw-rw-   0        0        0    18998 2023-07-30 05:42:11.000000 dicergirl-3.0.6/dicergirl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:01:15.301333 dicergirl-3.0.6/dicergirl/coc/
+-rw-rw-rw-   0        0        0        0 2023-07-29 07:34:15.000000 dicergirl-3.0.6/dicergirl/coc/__init__.py
+-rw-rw-rw-   0        0        0     4362 2023-07-30 05:42:11.000000 dicergirl-3.0.6/dicergirl/coc/coccards.py
+-rw-rw-rw-   0        0        0     9147 2023-07-30 05:42:11.000000 dicergirl-3.0.6/dicergirl/coc/cocutils.py
+-rw-rw-rw-   0        0        0     6020 2023-07-29 10:23:31.000000 dicergirl-3.0.6/dicergirl/coc/investigator.py
+-rw-rw-rw-   0        0        0    16467 2023-07-30 06:57:07.000000 dicergirl-3.0.6/dicergirl/main.py
+-rw-rw-rw-   0        0        0     3430 2023-07-30 07:00:21.000000 dicergirl-3.0.6/dicergirl/run.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:01:15.306275 dicergirl-3.0.6/dicergirl/scp/
+-rw-rw-rw-   0        0        0        0 2023-07-29 07:34:15.000000 dicergirl-3.0.6/dicergirl/scp/__init__.py
+-rw-rw-rw-   0        0        0     3285 2023-07-30 05:42:11.000000 dicergirl-3.0.6/dicergirl/scp/agent.py
+-rw-rw-rw-   0        0        0     2832 2023-07-30 05:42:11.000000 dicergirl-3.0.6/dicergirl/scp/scpcards.py
+-rw-rw-rw-   0        0        0     5191 2023-07-30 05:42:11.000000 dicergirl-3.0.6/dicergirl/scp/scputils.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:01:15.313479 dicergirl-3.0.6/dicergirl/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-29 07:34:15.000000 dicergirl-3.0.6/dicergirl/utils/__init__.py
+-rw-rw-rw-   0        0        0     4384 2023-07-29 07:34:15.000000 dicergirl-3.0.6/dicergirl/utils/chat.py
+-rw-rw-rw-   0        0        0     1934 2023-07-29 07:34:15.000000 dicergirl-3.0.6/dicergirl/utils/decorators.py
+-rw-rw-rw-   0        0        0     7129 2023-07-30 06:42:58.000000 dicergirl-3.0.6/dicergirl/utils/dicer.py
+-rw-rw-rw-   0        0        0    16252 2023-07-30 05:42:11.000000 dicergirl-3.0.6/dicergirl/utils/handlers.py
+-rw-rw-rw-   0        0        0    23148 2023-07-30 05:42:11.000000 dicergirl-3.0.6/dicergirl/utils/messages.py
+-rw-rw-rw-   0        0        0     1275 2023-07-30 05:42:11.000000 dicergirl-3.0.6/dicergirl/utils/settings.py
+-rw-rw-rw-   0        0        0     5220 2023-07-30 07:01:05.000000 dicergirl-3.0.6/dicergirl/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:01:15.298876 dicergirl-3.0.6/dicergirl.egg-info/
+-rw-rw-rw-   0        0        0     9351 2023-07-30 07:01:15.000000 dicergirl-3.0.6/dicergirl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      672 2023-07-30 07:01:15.000000 dicergirl-3.0.6/dicergirl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 07:01:15.000000 dicergirl-3.0.6/dicergirl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-07-30 07:01:15.000000 dicergirl-3.0.6/dicergirl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-30 07:01:15.000000 dicergirl-3.0.6/dicergirl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 07:01:15.315480 dicergirl-3.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1093 2023-07-30 05:42:11.000000 dicergirl-3.0.6/setup.py
```

### Comparing `dicergirl-3.0.5/LICENSE` & `dicergirl-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.5/PKG-INFO` & `dicergirl-3.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicergirl
-Version: 3.0.5
+Version: 3.0.6
 Summary: 跑团骰娘机器人欧若可, 支持 QQ频道 及 Nonebot2 部署.
 Home-page: https://gitee.com/unvisitor/dicer
 Author: Night Resurgent <fu050409@163.com>
 Author-email: fu050409@163.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://gitee.com/unvisitor/dicer/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dicergirl-3.0.5/README.md` & `dicergirl-3.0.6/README.md`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.5/dicergirl/__init__.py` & `dicergirl-3.0.6/dicergirl/__init__.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.5/dicergirl/coc/coccards.py` & `dicergirl-3.0.6/dicergirl/coc/coccards.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.5/dicergirl/coc/cocutils.py` & `dicergirl-3.0.6/dicergirl/coc/cocutils.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.5/dicergirl/coc/investigator.py` & `dicergirl-3.0.6/dicergirl/coc/investigator.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.5/dicergirl/main.py` & `dicergirl-3.0.6/dicergirl/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from botpy.message import Message
-from botpy.ext.cog_yaml import read
 from botpy.types.message import MarkdownPayload
 from botpy.api import BotAPI
 from botpy.logging import get_logger
 from pathlib import Path
 
 from utils.settings import set_package, get_package
 set_package("qqguild")
@@ -24,14 +23,15 @@
 import logging
 import sys
 
 DEBUG = False
 current_dir = Path(__file__).resolve().parent
 config = get_config()
 mode = "scp"
+
 get_logger().setLevel(logging.CRITICAL)
 logger.remove()
 logger.add(
     sys.stdout,
     level = "INFO"
 )
 package = get_package()
@@ -288,15 +288,15 @@
     await message.reply(content=ra(args, message))
     return True
 
 
 @Commands(name=(".rh"))
 async def rhhandler(api: BotAPI, message: Message, params=None):
     args = format_str(message, begin=".rh")
-    await message.reply(content="[Oracle] 暗骰: 命运的骰子在滚动.")
+    await message.reply(content="[Oracle] 暗骰: 命运的齿轮在转动.")
     await api.post_dms(guild_id=message.guild_id, msg_id=message.id, content=rd0(args))
 
 @Commands(name=(".rha"))
 async def rhahandler(api: BotAPI, message: Message, params=None):
     args = format_msg(message, begin=".rha")
     await message.reply(content="[Oracle] 暗骰: 命运的骰子在滚动.")
     await api.post_dms(guild_id=message.guild_id, msg_id=message.id, content=ra(args, message))
@@ -423,15 +423,15 @@
                 sys.stdout,
                 level = "DEBUG"
             )
             logger.info("DEBUG 模式已启动.")
         init()
         cards.load()
         scp_cards.load()
-        logger.info("机器人启动成功, 将进行心跳维持链接.")
+        logger.success("机器人启动成功, 将进行心跳维持链接.")
 
     async def on_at_message_create(self, message: Message):
         is_command = False
         for handler in self.handlers:
             if await handler(api=self.api, message=message, params=None):
                 isbot = "玩家" if message.author.bot == False else "机器人"
                 logger.info(f"[dicer] 执行指令: {message.content} 指令来源: {message.channel_id} : {message.author.id} : {message.author.username} : {isbot}")
```

### Comparing `dicergirl-3.0.5/dicergirl/run.py` & `dicergirl-3.0.6/dicergirl/run.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from loguru import logger
 from pathlib import Path
 from watchdog.observers import Observer
 from watchdog.events import FileSystemEventHandler
 from multiprocessing import Process, freeze_support
 try:
     from .utils.settings import package
+    from .utils.utils import version
 except ImportError:
-    from utils.settings import package
+    from dicergirl.utils.settings import package
+    from .utils.utils import version
 
 import sys
 import runpy
 import time
 import os
 
 current_dir = Path(__file__).resolve().parent
@@ -26,49 +28,51 @@
         )
     sys.exit()
 
 class FileModifiedHandler(FileSystemEventHandler):
     def __init__(self):
         super(FileModifiedHandler, self).__init__()
         self.is_modified: bool = False
-        self.modified_module: str = None
+        self.modified_module: str = ""
+        self.modified_file: str = ""
 
     def on_modified(self, event):
         if not event.is_directory:
             split = os.path.basename(event.src_path).split(".")
             if len(split) == 1:
                 return
             if split[1] == "py":
                 self.is_modified = True
                 self.modified_module = split[0]
+                self.modified_file = event.src_path
 
 def monitor_folder(folder_path, target=None):
     thread = Process(target=target)
     thread.daemon = True
 
     event_handler = FileModifiedHandler()
     observer = Observer()
     observer.schedule(event_handler, folder_path, recursive=True)
     observer.start()
-    logger.info("文件监视器已启动, `QQGuild`机器人已开启热重载模式.")
+    logger.success("文件监视器已启动, `QQGuild`机器人已开启热重载模式.")
     logger.info(f"监视目录: {folder_path}")
 
     thread.start()
     logger.info("开始启动`QQGuild`机器人...")
 
     try:
         while True:
             if event_handler.is_modified:
                 event_handler.is_modified = False
                 if target:
                     if thread.is_alive():
-                        logger.info(f"模块`{event_handler.modified_module}`被更改, 开始终止主程序.")
+                        logger.info(f"文件`{event_handler.modified_file}`被更改, 开始终止主程序.")
                         thread.terminate()
                         thread.join()
-                    logger.info("主线程已终止, 重启中.")
+                    logger.success("主线程已终止, 重启中...")
                     thread = Process(target=target)
                     thread.daemon = True
                     thread.start()
                 else:
                     raise ValueError("监视线程未传入.")
             time.sleep(0.5)
     except KeyboardInterrupt:
@@ -76,14 +80,17 @@
         sys.exit()
 
 def run():
     sys.path.insert(0, str(current_dir))
     runpy.run_module(MODULE_TO_RELOAD, run_name="__main__", alter_sys=True)
  
 def main():
+    logger.info(f"Dicer Girl {version}")
+    logger.info("Copyright © 2011-2023 Unknown Visitor. All Rights Reserved.")
+    logger.info("开始初始化环境...")
     freeze_support()
     try:
         monitor_folder(current_dir, target=run)
     except KeyboardInterrupt:
         logger.info("用户要求退出.")
         sys.exit()
     except Exception as e:
```

### Comparing `dicergirl-3.0.5/dicergirl/scp/agent.py` & `dicergirl-3.0.6/dicergirl/scp/agent.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.5/dicergirl/scp/scpcards.py` & `dicergirl-3.0.6/dicergirl/scp/scpcards.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.5/dicergirl/scp/scputils.py` & `dicergirl-3.0.6/dicergirl/scp/scputils.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.5/dicergirl/utils/chat.py` & `dicergirl-3.0.6/dicergirl/utils/chat.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.5/dicergirl/utils/decorators.py` & `dicergirl-3.0.6/dicergirl/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.5/dicergirl/utils/dicer.py` & `dicergirl-3.0.6/dicergirl/utils/dicer.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.5/dicergirl/utils/handlers.py` & `dicergirl-3.0.6/dicergirl/utils/handlers.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.5/dicergirl/utils/messages.py` & `dicergirl-3.0.6/dicergirl/utils/messages.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.5/dicergirl/utils/settings.py` & `dicergirl-3.0.6/dicergirl/utils/settings.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.5/dicergirl/utils/utils.py` & `dicergirl-3.0.6/dicergirl/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 from pathlib import Path
 from loguru import logger
 from typing import Union
 
+import json
+import os
+import uuid
+import re
+import inspect
+
 try:
     from dicergirl.utils.decorators import translate_punctuation
     from dicergirl.utils.settings import package, setconfig, getconfig
 except ImportError:
     from .decorators import translate_punctuation
     from .settings import package, setconfig, getconfig
 
@@ -28,29 +34,23 @@
     try:
         from botpy.message import Message
     except ModuleNotFoundError:
         logger.warning("未找到依赖`qq-botpy`, 请检查你的配置.")
         class Message:
             pass
 
-import json
-import os
-import uuid
-import re
-import inspect
-
 current_dir = Path(__file__).resolve().parent
 dicer_girl_dir = Path.home() / ".dicergirl"
 data_dir = dicer_girl_dir / "data"
 _coc_cachepath = data_dir / "coc_cards.json"
 _scp_cachepath = data_dir / "scp_cards.json"
 _super_user = data_dir / "super_user.json"
 _log = logger
 su_uuid = (str(uuid.uuid1()) + str(uuid.uuid4())).replace("-", "")
-version = "3.0.5"
+version = "3.0.6"
 
 def init():
     if not dicer_girl_dir.exists():
         _log.info("Dicer Girl 文件夹未建立, 建立它.")
         dicer_girl_dir.mkdir()
     if not data_dir.exists():
         _log.info("Dicer Girl 数据文件夹未建立, 建立它.")
```

### Comparing `dicergirl-3.0.5/dicergirl.egg-info/PKG-INFO` & `dicergirl-3.0.6/dicergirl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicergirl
-Version: 3.0.5
+Version: 3.0.6
 Summary: 跑团骰娘机器人欧若可, 支持 QQ频道 及 Nonebot2 部署.
 Home-page: https://gitee.com/unvisitor/dicer
 Author: Night Resurgent <fu050409@163.com>
 Author-email: fu050409@163.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://gitee.com/unvisitor/dicer/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dicergirl-3.0.5/dicergirl.egg-info/SOURCES.txt` & `dicergirl-3.0.6/dicergirl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.5/setup.py` & `dicergirl-3.0.6/setup.py`

 * *Files identical despite different names*

