# Comparing `tmp/nonebot-plugin-mcversion-0.2.1.tar.gz` & `tmp/nonebot-plugin-mcversion-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-mcversion-0.2.1.tar", last modified: Sun Jun 18 11:39:41 2023, max compression
+gzip compressed data, was "nonebot-plugin-mcversion-0.2.2.tar", last modified: Sun Jul 30 06:21:02 2023, max compression
```

## Comparing `nonebot-plugin-mcversion-0.2.1.tar` & `nonebot-plugin-mcversion-0.2.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1065 2023-06-18 11:39:28.122224 nonebot-plugin-mcversion-0.2.1/LICENSE
--rw-r--r--   0        0        0     1931 2023-06-18 11:39:28.122224 nonebot-plugin-mcversion-0.2.1/README.md
--rw-r--r--   0        0        0     2583 2023-06-18 11:39:28.122224 nonebot-plugin-mcversion-0.2.1/nonebot_plugin_mcversion/__init__.py
--rw-r--r--   0        0        0      621 2023-06-18 11:39:28.122224 nonebot-plugin-mcversion-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2314 1970-01-01 00:00:00.000000 nonebot-plugin-mcversion-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-30 06:20:51.911943 nonebot-plugin-mcversion-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1931 2023-07-30 06:20:51.911943 nonebot-plugin-mcversion-0.2.2/README.md
+-rw-r--r--   0        0        0     2497 2023-07-30 06:20:51.911943 nonebot-plugin-mcversion-0.2.2/nonebot_plugin_mcversion/__init__.py
+-rw-r--r--   0        0        0      621 2023-07-30 06:20:51.911943 nonebot-plugin-mcversion-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2314 1970-01-01 00:00:00.000000 nonebot-plugin-mcversion-0.2.2/PKG-INFO
```

### Comparing `nonebot-plugin-mcversion-0.2.1/LICENSE` & `nonebot-plugin-mcversion-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcversion-0.2.1/README.md` & `nonebot-plugin-mcversion-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcversion-0.2.1/nonebot_plugin_mcversion/__init__.py` & `nonebot-plugin-mcversion-0.2.2/nonebot_plugin_mcversion/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # 导入必要的库
 import os
-import requests
+import httpx
 from datetime import datetime
 from nonebot import on_command, get_driver, require, Config
 from nonebot.adapters.onebot.v11 import Bot
 from nonebot.adapters.onebot.v11.message import Message
 
 env_config = Config(**get_driver().config.dict())
 mcver_group_id = list(env_config.mcver_group_id)
@@ -12,54 +12,50 @@
 # 定义命令“mcver”
 mcver = on_command('mcver', aliases={'mcversion', 'MC版本'}, priority=50)
 
 # 处理命令“mcver”
 @mcver.handle()
 async def mcver_handle():
     # 获取Minecraft版本信息
-    url = 'https://launchermeta.mojang.com/mc/game/version_manifest.json'
-    response = requests.get(url)
+    async with httpx.AsyncClient() as client:
+        response = await client.get("http://launchermeta.mojang.com/mc/game/version_manifest.json")
     data = response.json()
     latest_release = data['latest']['release']
     latest_snapshot = data['latest']['snapshot']
     # 发送消息
     await mcver.finish(message = Message(f'最新正式版：{latest_release}\n最新快照版：{latest_snapshot}'))
 
 # 获取nonebot的调度器
 scheduler = require('nonebot_plugin_apscheduler').scheduler
 
 # 定义异步函数，用于检查Minecraft更新
 async def check_mc_update(bot: Bot):
     # 获取Minecraft版本信息
-    url = 'https://launchermeta.mojang.com/mc/game/version_manifest.json'
-    response = requests.get(url)
+    async with httpx.AsyncClient() as client:
+        response = await client.get("http://launchermeta.mojang.com/mc/game/version_manifest.json")
     data = response.json()
-    latest_version = data["versions"][0]["id"]
+    version = data["versions"][0]
     if not os.path.exists('data/latest_version.txt'):
         with open('data/latest_version.txt', 'w') as f:
-            f.write(latest_version)
+            f.write(version["id"])
     with open('data/latest_version.txt', 'r') as f:
         old_version = f.read()
-    if latest_version != old_version:
-        with open('data/latest_version.txt', 'w') as f:
-            f.write(latest_version)
-        release_time =''
-        for version in data["versions"]:
-            if version["id"] == latest_version:
-                release_time = version["releaseTime"]
-                break
+    if version["id"] != old_version:
+        release_time = version["releaseTime"]
         release_time = datetime.strptime(release_time, '%Y-%m-%dT%H:%M:%S%z')
         release_time = release_time.replace(hour=release_time.hour+8)
         release_time = release_time.strftime('%Y-%m-%dT%H:%M:%S+08')
         for i in mcver_group_id:
             int (i)
             await bot.send_group_msg(
                 group_id=i,
-                message=Message(f'发现MC更新：{latest_version} ({version["type"]})\n时间：{release_time}')
+                message=Message(f'发现MC更新：{version["id"]} ({version["type"]})\n时间：{release_time}')
             )
+        with open('data/latest_version.txt', 'w') as f:
+            f.write(version["id"])
 
 # 获取nonebot的机器人实例
 from nonebot import get_bots
 # 定义定时任务，每分钟检查一次Minecraft更新
 @scheduler.scheduled_job('interval', minutes=1)
 async def mc_update_check():
     (bot, ) = get_bots().values()
```

### Comparing `nonebot-plugin-mcversion-0.2.1/pyproject.toml` & `nonebot-plugin-mcversion-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-mcversion"
-version = "0.2.1"
+version = "0.2.2"
 description = "NoneBot2 plugin for CheckMCupdate"
 authors = [
     { name = "CN171-1", email = "3428166361@qq.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0rc2",
     "nonebot-adapter-onebot>=2.1.5",
```

### Comparing `nonebot-plugin-mcversion-0.2.1/PKG-INFO` & `nonebot-plugin-mcversion-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mcversion
-Version: 0.2.1
+Version: 0.2.2
 Summary: NoneBot2 plugin for CheckMCupdate
 License: MIT
 Author-email: CN171-1 <3428166361@qq.com>
 Requires-Python: >=3.8
 Project-URL: Homepage, https://github.com/CN171-1/nonebot-plugin-mcversion
 Project-URL: Repository, https://github.com/CN171-1/nonebot-plugin-mcversion
 Description-Content-Type: text/markdown
```

