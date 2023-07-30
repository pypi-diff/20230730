# Comparing `tmp/nonebot_plugin_poke-0.1.0.tar.gz` & `tmp/nonebot_plugin_poke-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_poke-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_poke-0.1.1.tar", max compression
```

## Comparing `nonebot_plugin_poke-0.1.0.tar` & `nonebot_plugin_poke-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-07-05 10:29:18.679132 nonebot_plugin_poke-0.1.0/LICENSE
--rw-r--r--   0        0        0     3045 2023-07-05 10:29:18.679132 nonebot_plugin_poke-0.1.0/README.md
--rw-r--r--   0        0        0     5053 2023-07-05 10:29:18.679132 nonebot_plugin_poke-0.1.0/nonebot_plugin_poke/__init__.py
--rw-r--r--   0        0        0      753 2023-07-05 10:29:18.679132 nonebot_plugin_poke-0.1.0/nonebot_plugin_poke/config.py
--rw-r--r--   0        0        0     1234 2023-07-05 10:29:18.679132 nonebot_plugin_poke-0.1.0/nonebot_plugin_poke/matcher.py
--rw-r--r--   0        0        0     5068 2023-07-05 10:29:18.679132 nonebot_plugin_poke-0.1.0/nonebot_plugin_poke/utils.py
--rw-r--r--   0        0        0      931 2023-07-05 10:29:18.683132 nonebot_plugin_poke-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3895 1970-01-01 00:00:00.000000 nonebot_plugin_poke-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-30 15:54:55.968021 nonebot_plugin_poke-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3045 2023-07-30 15:54:55.968021 nonebot_plugin_poke-0.1.1/README.md
+-rw-r--r--   0        0        0     5209 2023-07-30 15:54:55.968021 nonebot_plugin_poke-0.1.1/nonebot_plugin_poke/__init__.py
+-rw-r--r--   0        0        0      727 2023-07-30 15:54:55.968021 nonebot_plugin_poke-0.1.1/nonebot_plugin_poke/config.py
+-rw-r--r--   0        0        0     1280 2023-07-30 15:54:55.972021 nonebot_plugin_poke-0.1.1/nonebot_plugin_poke/matcher.py
+-rw-r--r--   0        0        0     5115 2023-07-30 15:54:55.972021 nonebot_plugin_poke-0.1.1/nonebot_plugin_poke/utils.py
+-rw-r--r--   0        0        0     1682 2023-07-30 15:54:55.972021 nonebot_plugin_poke-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4028 1970-01-01 00:00:00.000000 nonebot_plugin_poke-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_poke-0.1.0/LICENSE` & `nonebot_plugin_poke-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_poke-0.1.0/README.md` & `nonebot_plugin_poke-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_poke-0.1.0/nonebot_plugin_poke/__init__.py` & `nonebot_plugin_poke-0.1.1/nonebot_plugin_poke/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-from nonebot import on_command
-from nonebot.params import CommandArg
-from nonebot.rule import to_me
+import imghdr
+from datetime import datetime
+from typing import List
+
+from nonebot.adapters import Message
+from nonebot.adapters.onebot.v11 import MessageEvent, PokeNotifyEvent
 from nonebot.matcher import Matcher
 from nonebot.plugin import PluginMetadata
-from nonebot.plugin.on import  on_notice,on_command
-from nonebot.adapters.onebot.v11 import PokeNotifyEvent,MessageEvent
-
-from datetime import datetime
-import imghdr
+from nonebot.plugin.on import on_command, on_notice
 
-from .utils import *
-from .matcher import *
+from .matcher import poke_reply
+from .utils import config, get_data, poke_rule
 
-logo ="""
+logo = """
     ......                  ` .]]@@@@@@@@@@@@@@@@@@@@@@@@@@@@@OO^       
     ......                ,/@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@OO^       
     ......            /O@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@OO^       
     `.....           ,@^=.OOO\/\@@@@@@@@@@@@@@@@@@@@OO//@@@@@/OO\]]]OO\]
     ``....          ,@@/=^OOOOOOOO@@@@@@@@@@@\]OOOOOOO^^=@@@@OOOOOOOOOOO
     `.....          O@O^==OOOOOOOO@@@/.,@@@OOOOOOOOOOO\O,@@@@OOOOOOOOO@@
     ......    ,    .@@@^=`OOOOOOOOO/  ,O@@OOOOOOOOOOOOOO.O@@@OO/[[[[[[[.
@@ -46,70 +45,77 @@
     @OO\ooO....,*/@^,@@@\..@^[\@@@@@@O]*]//[`@^*^*=OOOOOO^..=OO\...\^.\@
     OOooo^..`./oOO@/ =^\/^.^\\....=]......,/@@^O^*O.... .,][],OO\....\`.
     @Oooo\/]OOOOOO/  .  \.=^....,..........[.,OO^=^.    /    ,`\OO`.....
     """
 __version__ = "0.1.0"
 __plugin_meta__ = PluginMetadata(
     name="戳一戳事件",
-    description='自定义群聊戳一戳事件',
+    description="自定义群聊戳一戳事件",
     usage=logo,
     type="application",
     homepage="https://github.com/Agnes4m/nonebot_plugin_poke",
     supported_adapters={"~onebot.v11"},
     extra={
         "version": __version__,
         "author": "Agnes4m <Z735803792@163.com>",
     },
 )
 
-poke_ = on_notice(block=config.poke_block, 
-                  priority=config.poke_priority, rule=poke_rule)
+poke_ = on_notice(block=config.poke_block, priority=config.poke_priority, rule=poke_rule)
 
 
 @poke_.handle()
-async def _(event: PokeNotifyEvent,matcher:Matcher):
-    await poke_reply(event,matcher)
-    
+async def _(event: PokeNotifyEvent, matcher: Matcher):
+    await poke_reply(event, matcher)
+
+
+add_pic = on_command("zq", aliases={"抓图"}, priority=30)
+
 
-add_pic = on_command('zq',aliases={'抓图'},priority=30)
 @add_pic.handle()
-async def _(event:MessageEvent,matcher:Matcher):
+async def _(event: MessageEvent, matcher: Matcher):
     images: List[bytes] = []
     images_name: List[str] = []
 
     success: int = 0
     fail: int = 0
     if event.reply:
-        for pic in event.reply.message['image']:
+        for pic in event.reply.message["image"]:
             try:
                 _img = await get_data(str(pic.data.get("url", "")))
+                if not _img:
+                    return
                 success += 1
                 images.append(_img)
-            except:
+            except Exception:
                 fail += 1
-                
+
             msg: Message = event.dict()["message"]
             for msg_seg in msg:
                 if msg_seg.type == "image":
                     try:
                         _img = await get_data(str(msg_seg.data.get("url", "")))
                         success += 1
+                        if not _img:
+                            return
                         images.append(_img)
-                    except:
+                    except Exception:
                         fail += 1
 
-            
             base = 0
             while len(images_name) < len(images):
-                images_name.append(str(int(datetime.now().timestamp())+base))
+                images_name.append(str(int(datetime.now().timestamp()) + base))
                 base += 1
-            images_name = images_name[:len(images)]
-            images_name = [f"{img_name}.{imghdr.what(None, h=images[i])}" for i,img_name in enumerate(images_name)]
+            images_name = images_name[: len(images)]
+            images_name = [
+                f"{img_name}.{imghdr.what(None, h=images[i])}"
+                for i, img_name in enumerate(images_name)
+            ]
 
-            path = config.poke_path.joinpath('pic')
-            for i,img in enumerate(images):
+            path = config.poke_path.joinpath("pic")
+            for i, img in enumerate(images):
                 img_path = path / images_name[i]
                 with img_path.open("wb+") as f:
                     f.write(img)
 
             tosend = f"添加完成，成功{success}张，失败{fail}张，可用于戳戳随机图"
-            await matcher.send(message=tosend,at_sender=True)
+            await matcher.send(message=tosend, at_sender=True)
```

### Comparing `nonebot_plugin_poke-0.1.0/nonebot_plugin_poke/config.py` & `nonebot_plugin_poke-0.1.1/nonebot_plugin_poke/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 from pathlib import Path
 from typing import List
 
 from nonebot import get_driver
-from nonebot.log import logger
 from pydantic import BaseSettings
 
 
 class Config(BaseSettings):
-    bot_nickname: str = '宁宁'
+    bot_nickname: str = "宁宁"
     poke_black: bool = True
-    poke_ban_group:List[str] = []
-    poke_allow_group:List[str] = []
+    poke_ban_group: List[str] = []
+    poke_allow_group: List[str] = []
     poke_send_pic: bool = False
     poke_send_poke: bool = True
     poke_send_text: bool = False
     poke_send_acc: bool = False
-    poke_path:Path = Path('data/poke')
-    poke_priority:int = 1
-    poke_block:bool = True
-
+    poke_path: Path = Path("data/poke")
+    poke_priority: int = 1
+    poke_block: bool = True
 
     class Config:
         extra = "ignore"
 
 
 config = Config.parse_obj(get_driver().config)
 
 
 if not config.poke_path.exists() or not config.poke_path.is_dir():
-    config.poke_path.mkdir(0o755, parents=True, exist_ok=True)
+    config.poke_path.mkdir(0o755, parents=True, exist_ok=True)
```

### Comparing `nonebot_plugin_poke-0.1.0/nonebot_plugin_poke/matcher.py` & `nonebot_plugin_poke-0.1.1/nonebot_plugin_poke/matcher.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,37 @@
+import random
+
+from nonebot.adapters.onebot.v11 import PokeNotifyEvent
 from nonebot.matcher import Matcher
-from nonebot.adapters.onebot.v11 import PokeNotifyEvent,MessageSegment
 
-from .utils import *
+from .utils import acc_send, config, pic_or_text, pic_send, poke_send, text_send
+
 
-async def poke_reply(event:PokeNotifyEvent,matcher:Matcher):
+async def poke_reply(event: PokeNotifyEvent, matcher: Matcher):
     if config.poke_send_poke:
-        await poke_send(event,matcher)
+        await poke_send(event, matcher)
 
     if config.poke_send_acc and (config.poke_send_pic or config.poke_send_text):
         roll = random.random()
         if roll > 0.5:
             await acc_send(matcher)
         else:
-            await matcher_pic_text(event,matcher)
+            await matcher_pic_text(matcher)
     elif config.poke_send_acc and not (config.poke_send_pic or config.poke_send_text):
         await acc_send(matcher)
     elif not config.poke_send_acc and (config.poke_send_pic or config.poke_send_text):
-        await matcher_pic_text(event,matcher)
+        await matcher_pic_text(matcher)
     else:
         return
-    
-async def matcher_pic_text(event,matcher):
+
+
+async def matcher_pic_text(matcher):
     if config.poke_send_pic and config.poke_send_text:
-        await pic_or_text(await pic_send(event,matcher),await text_send(event,matcher),matcher)
+        await pic_or_text(
+            await pic_send(),
+            await text_send(),
+            matcher,
+        )
     elif config.poke_send_pic and not config.poke_send_text:
-        await pic_or_text(await pic_send(event,matcher),None,matcher)
+        await pic_or_text(await pic_send(), None, matcher)
     elif not config.poke_send_pic and config.poke_send_text:
-        await pic_or_text(None,await text_send(event,matcher),matcher)
+        await pic_or_text(None, await text_send(), matcher)
```

### Comparing `nonebot_plugin_poke-0.1.0/nonebot_plugin_poke/utils.py` & `nonebot_plugin_poke-0.1.1/nonebot_plugin_poke/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,135 +1,146 @@
-from nonebot.matcher import Matcher
-from nonebot.log import logger
-from nonebot.adapters.onebot.v11 import PokeNotifyEvent,MessageSegment, Message
-
 import random
-import aiohttp
-from typing import List,Optional
 from pathlib import Path
+from typing import List, Optional
+
+import aiofiles
+import aiohttp
+from nonebot.adapters.onebot.v11 import Message, MessageSegment, PokeNotifyEvent
+from nonebot.log import logger
+from nonebot.matcher import Matcher
 
 from .config import config
 
-async def get_data(url:str):
+
+async def get_data(url: str):
     """获取url内容"""
     headers = {
-    'User-Agent':'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:107.0) Gecko/20100101 Firefox/107.0'
+        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:107.0) Gecko/20100101 Firefox/107.0",
     }
     async with aiohttp.ClientSession() as session:
         async with session.get(url, headers=headers, timeout=600) as response:
             if response.status == 200:
                 return await response.read()
-            else:
-                return None
-            
-            
-async def acc_send(matcher:Matcher):
+            return None
+
+
+async def acc_send(matcher: Matcher):
     """语音部分"""
     poke_file_path = config.poke_path
-    poke_file_path.joinpath('acc').mkdir(parents=True, exist_ok=True)
-    poke_acc_list = poke_file_path.joinpath('acc').iterdir()
-    acc_file_list:List[Path] = []
+    poke_file_path.joinpath("acc").mkdir(parents=True, exist_ok=True)
+    poke_acc_list = poke_file_path.joinpath("acc").iterdir()
+    acc_file_list: List[Path] = []
     for acc_file in poke_acc_list:
-        if acc_file.is_file() and acc_file.suffix.lower() in [".wav",".mp3",".acc"]:
+        if acc_file.is_file() and acc_file.suffix.lower() in [".wav", ".mp3", ".acc"]:
             acc_file_list.append(acc_file)
     send_acc = random.choice(acc_file_list)
     await matcher.send(MessageSegment.record(file=f"file:///{send_acc.resolve()}"))
-    
-async def poke_send(event:PokeNotifyEvent,matcher:Matcher):
+
+
+async def poke_send(event: PokeNotifyEvent, matcher: Matcher):
     if config.poke_send_poke:
-        logger.success('反击戳戳')
-        await matcher.send(Message([
-        MessageSegment("poke",  {
-           "qq": f"{event.user_id}"
-       })
-    ]))
+        logger.success("反击戳戳")
+        await matcher.send(Message([MessageSegment("poke", {"qq": f"{event.user_id}"})]))
     else:
         return
-    
-async def pic_send(event:PokeNotifyEvent,matcher:Matcher):
+
+
+async def pic_send():
     """发送图片和text"""
     pic_file_path = config.poke_path
-    pic_file_path.joinpath('pic').mkdir(parents=True, exist_ok=True)
+    pic_file_path.joinpath("pic").mkdir(parents=True, exist_ok=True)
     if config.poke_send_pic:
-        logger.success('发送图片')
-        poke_pic_list = pic_file_path.joinpath('pic').iterdir()
-        pic_file_list:List[Path] = []
+        logger.success("发送图片")
+        poke_pic_list = pic_file_path.joinpath("pic").iterdir()
+        pic_file_list: List[Path] = []
         for pic_file in poke_pic_list:
-            if pic_file.is_file() and pic_file.suffix.lower() in [".png",".jpg",".jpeg",".webp",".gif"]:
+            if pic_file.is_file() and pic_file.suffix.lower() in [
+                ".png",
+                ".jpg",
+                ".jpeg",
+                ".webp",
+                ".gif",
+            ]:
                 pic_file_list.append(pic_file)
         send_pic = random.choice(pic_file_list)
     else:
         send_pic = None
     return send_pic
-        
-async def text_send(event:PokeNotifyEvent,matcher:Matcher):
-    logger.success('发送文字')
+
+
+async def text_send():
+    logger.success("发送文字")
     pic_file_path = config.poke_path
-    if pic_file_path.joinpath('poke.txt').is_file():
-        with open(pic_file_path.joinpath('poke.txt'),mode='r',encoding='utf-8')as f :
-            text_file_list:List[str] = f.read().split('/n')
+    if pic_file_path.joinpath("poke.txt").is_file():
+        async with aiofiles.open(
+            pic_file_path.joinpath("poke.txt"),
+            mode="r",
+            encoding="utf-8",
+        ) as f:
+            text_file_list: List[str] = (await f.read()).split("\n")
             send_text = random.choice(text_file_list)
     else:
-        with open(pic_file_path.joinpath('poke.txt'),mode='w',encoding='utf-8')as f :
-            text_file_list:List[str] = [
-            "lsp你再戳？",
-            "连个可爱美少女都要戳的肥宅真恶心啊。",
-            "你再戳！",
-            "？再戳试试？",
-            "别戳了别戳了再戳就坏了555",
-            "我爪巴爪巴，球球别再戳了",
-            "你戳你🐎呢？！",
-            "请不要戳我 >_<",
-            "放手啦，不给戳QAQ",
-            "喂(#`O′) 戳我干嘛！",
-            "戳坏了，赔钱！",
-            "戳坏了",
-            "嗯……不可以……啦……不要乱戳",
-            "那...那里...那里不能戳...绝对...",
-            "(。´・ω・)ん?",
-            "有事恁叫我，别天天一个劲戳戳戳！",
-            "欸很烦欸！你戳🔨呢",
-            "再戳一下试试？",
-            "正在关闭对您的所有服务...关闭成功",
-            "啊呜，太舒服刚刚竟然睡着了。什么事？",
-            "正在定位您的真实地址...定位成功。轰炸机已起飞",
+        async with aiofiles.open(
+            pic_file_path.joinpath("poke.txt"),
+            mode="w",
+            encoding="utf-8",
+        ) as f:
+            text_file_list: List[str] = [
+                "lsp你再戳？",
+                "连个可爱美少女都要戳的肥宅真恶心啊。",
+                "你再戳！",
+                "？再戳试试？",
+                "别戳了别戳了再戳就坏了555",
+                "我爪巴爪巴，球球别再戳了",
+                "你戳你🐎呢？！",
+                "请不要戳我 >_<",
+                "放手啦，不给戳QAQ",
+                "喂(#`O′) 戳我干嘛！",
+                "戳坏了，赔钱！",
+                "戳坏了",
+                "嗯……不可以……啦……不要乱戳",
+                "那...那里...那里不能戳...绝对...",
+                "(。´・ω・)ん?",
+                "有事恁叫我，别天天一个劲戳戳戳！",
+                "欸很烦欸！你戳🔨呢",
+                "再戳一下试试？",
+                "正在关闭对您的所有服务...关闭成功",
+                "啊呜，太舒服刚刚竟然睡着了。什么事？",
+                "正在定位您的真实地址...定位成功。轰炸机已起飞",
             ]
-            f.write('/n'.join(text_file_list))
+            await f.write("/n".join(text_file_list))
             send_text = random.choice(text_file_list)
-    send_text.replace('我',config.bot_nickname)
+    send_text.replace("我", config.bot_nickname)
     return send_text
 
-async def pic_or_text(send_pic:Optional[Path],send_text:Optional[str],matcher:Matcher):
+
+async def pic_or_text(
+    send_pic: Optional[Path],
+    send_text: Optional[str],
+    matcher: Matcher,
+):
     if send_pic and send_text:
-        await matcher.send(MessageSegment.image(file=f"file:///{send_pic.resolve()}")+send_text)
-        return
+        await matcher.send(
+            MessageSegment.image(file=f"file:///{send_pic.resolve()}") + send_text,
+        )
     elif send_pic and not send_text:
         await matcher.send(MessageSegment.image(file=f"file:///{send_pic.resolve()}"))
-        return
     elif not send_pic and send_text:
         await matcher.send(send_text)
-        return
-    else:
-        return
+    return
+
 
-async def poke_rule(event:PokeNotifyEvent):
+async def poke_rule(event: PokeNotifyEvent):
     """黑白名单判断"""
-    if isinstance(event,PokeNotifyEvent) and event.target_id == event.self_id:
+    if isinstance(event, PokeNotifyEvent) and event.target_id == event.self_id:
         group = event.group_id
-        if config.poke_black:
-            if group in config.poke_ban_group:
-                return False
-            else:
-                return True
-        else:
-            if group in config.poke_allow_group:
-                return True
-            else:
-                return False
-    else:
-        return False
+        return (
+            (group not in set(config.poke_ban_group))
+            if config.poke_black
+            else (group in set(config.poke_allow_group))
+        )
+    return False
 
 
 async def add_pic():
-    pic_file_path = config.poke_path.joinpath('pic')
+    pic_file_path = config.poke_path.joinpath("pic")
     pic_file_path.mkdir(parents=True, exist_ok=True)
-
```

### Comparing `nonebot_plugin_poke-0.1.0/PKG-INFO` & `nonebot_plugin_poke-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-poke
-Version: 0.1.0
+Version: 0.1.1
 Summary: 自定义群聊戳戳事件 plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_poke
 License: MIT
 Keywords: nonebot2,plugin,event
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
+Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.1.5)
 Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/Agnes4m/nonebot_plugin_poke
 Description-Content-Type: text/markdown
 
 <div align="center">
   <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-poke Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-poke Version: 0.1.1 Summary:
 èªå®ä¹ç¾¤èæ³æ³äºä»¶ plugin for NoneBot2 Home-page: https://github.com/
 Agnes4m/nonebot_plugin_poke License: MIT Keywords: nonebot2,plugin,event
 Author: Agnes_Digital Author-email: Z735803792@163.com Requires-Python:
->=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
+>=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Dist: nonebot-
-adapter-onebot (>=2.1.5) Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Project-URL:
-Repository, https://github.com/Agnes4m/nonebot_plugin_poke Description-Content-
-Type: text/markdown
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Dist: aiofiles (>=23.1.0,<24.0.0) Requires-
+Dist: aiohttp (>=3.8.5,<4.0.0) Requires-Dist: nonebot-adapter-onebot (>=2.1.5)
+Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Project-URL: Repository, https://
+github.com/Agnes4m/nonebot_plugin_poke Description-Content-Type: text/markdown
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
   # nonebot_plugin_poke _â¨Nonebot & èªå®ä¹æ³æ³ç¾¤èäºä»¶â¨_ [GitHub
        stars] [GitHub_issues] [QQ_Chat_Group] [pypi] [python] [NoneBot]
 ## å®è£ æ¹æ³ä¸ï¼ nb plugin install nonebot_plugin_poke æ¹æ³äºï¼ pip
 install nonebot_plugin_poke
 åæå¨æ·»å `nonebot_plugin_poke`å°botæä»¶ä¸`pyproject.toml`æä»¶ä¸­ ##
```

