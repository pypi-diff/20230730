# Comparing `tmp/nonebot_plugin_aujob-0.1.4.tar.gz` & `tmp/nonebot_plugin_aujob-0.2.114514.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_aujob-0.1.4.tar", last modified: Sun Jul 30 04:00:28 2023, max compression
+gzip compressed data, was "nonebot_plugin_aujob-0.2.114514.tar", last modified: Sun Jul 30 04:24:19 2023, max compression
```

## Comparing `nonebot_plugin_aujob-0.1.4.tar` & `nonebot_plugin_aujob-0.2.114514.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 04:00:28.635894 nonebot_plugin_aujob-0.1.4/
--rw-rw-rw-   0        0        0      511 2023-07-30 04:00:28.635894 nonebot_plugin_aujob-0.1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-30 04:00:28.620895 nonebot_plugin_aujob-0.1.4/nonebot_plugin_aujob/
--rw-rw-rw-   0        0        0     1709 2023-07-29 12:11:37.000000 nonebot_plugin_aujob-0.1.4/nonebot_plugin_aujob/__init__.py
--rw-rw-rw-   0        0        0    11199 2023-07-29 02:41:44.000000 nonebot_plugin_aujob-0.1.4/nonebot_plugin_aujob/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-30 04:00:28.632898 nonebot_plugin_aujob-0.1.4/nonebot_plugin_aujob.egg-info/
--rw-rw-rw-   0        0        0      511 2023-07-30 04:00:28.000000 nonebot_plugin_aujob-0.1.4/nonebot_plugin_aujob.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-07-30 04:00:28.000000 nonebot_plugin_aujob-0.1.4/nonebot_plugin_aujob.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 04:00:28.000000 nonebot_plugin_aujob-0.1.4/nonebot_plugin_aujob.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-30 04:00:28.000000 nonebot_plugin_aujob-0.1.4/nonebot_plugin_aujob.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-30 04:00:28.000000 nonebot_plugin_aujob-0.1.4/nonebot_plugin_aujob.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      660 2023-07-30 04:00:10.000000 nonebot_plugin_aujob-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-30 04:00:28.635894 nonebot_plugin_aujob-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-30 04:24:19.158512 nonebot_plugin_aujob-0.2.114514/
+-rw-rw-rw-   0        0        0      516 2023-07-30 04:24:19.157515 nonebot_plugin_aujob-0.2.114514/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-30 04:24:19.141943 nonebot_plugin_aujob-0.2.114514/nonebot_plugin_aujob/
+-rw-rw-rw-   0        0        0     1709 2023-07-29 12:11:37.000000 nonebot_plugin_aujob-0.2.114514/nonebot_plugin_aujob/__init__.py
+-rw-rw-rw-   0        0        0    11631 2023-07-30 04:23:31.000000 nonebot_plugin_aujob-0.2.114514/nonebot_plugin_aujob/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-30 04:24:19.154513 nonebot_plugin_aujob-0.2.114514/nonebot_plugin_aujob.egg-info/
+-rw-rw-rw-   0        0        0      516 2023-07-30 04:24:19.000000 nonebot_plugin_aujob-0.2.114514/nonebot_plugin_aujob.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-07-30 04:24:19.000000 nonebot_plugin_aujob-0.2.114514/nonebot_plugin_aujob.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 04:24:19.000000 nonebot_plugin_aujob-0.2.114514/nonebot_plugin_aujob.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-30 04:24:19.000000 nonebot_plugin_aujob-0.2.114514/nonebot_plugin_aujob.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-30 04:24:19.000000 nonebot_plugin_aujob-0.2.114514/nonebot_plugin_aujob.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      665 2023-07-30 04:23:56.000000 nonebot_plugin_aujob-0.2.114514/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-30 04:24:19.158512 nonebot_plugin_aujob-0.2.114514/setup.cfg
```

### Comparing `nonebot_plugin_aujob-0.1.4/nonebot_plugin_aujob/__init__.py` & `nonebot_plugin_aujob-0.2.114514/nonebot_plugin_aujob/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_aujob-0.1.4/nonebot_plugin_aujob/utils.py` & `nonebot_plugin_aujob-0.2.114514/nonebot_plugin_aujob/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 dict_else = {
     "help": "欢迎使用among us职业介绍插件，输入.t 职业名 可以查看该职业的玩法\n"
     "截止TOH410所有的职业：\n\n"
     "无阵营:管理员\n\n"
     "躲猫猫职业/第三方阵营:狐狸,猎人\n\n"
-    "船员阵营：警长，诱饵，执灯人，市长，修理大师，告密者，增速者，医生，陷阱师，独裁者，灵媒，时间管理大师\n\n"
+    "船员阵营：警长，诱饵，执灯人，市长，修理大师，告密者，增速者，医生，陷阱师，独裁者，灵媒，时间管理者\n\n"
     "伪装者阵营:赏金猎人，嗜血杀手，吸血鬼，术士，女巫，黑手党，烟花商人，狙击手，梦魇，蚀时者，千面鬼，邪恶的追踪者，背叛的守卫，背叛的告密\n\n"
     "中立阵营:窥视者，纵火犯，小丑，投机者，恐怖分子，薛定谔的猫，野心家，处刑人，豺狼，恋人\n\n"
-    "效果(附加职业):绝境者"
+    "效果(附加职业):绝境者，窥视者，实干家，恋人"
 }
 
 # 角色字典
 dict_character = {
     "警长": "警长:警长(Sheriff)(船员阵营):\n警长可以击杀内鬼（根据房间设置，警长也可以击杀独立阵营玩家）。\n警长若尝试击杀船员阵营的玩家，警长将会走火自杀。\n警长没有任务。",
     "诱饵": "诱饵:诱饵(Bait)(船员阵营):\n诱饵被击杀时，击杀诱饵的凶手将被迫报告。",
     "执灯人": "执灯人:执灯人(Lighter)(船员阵营):\n执灯人完成任务后，视野会扩大，且不受照明破坏影响。",
@@ -59,9 +59,11 @@
     "傀儡师": "傀儡师:傀儡师(Puppeter)(内鬼阵营):\n傀儡师的操控对象会击杀其遇到的下一个船员。\n若后者在接触的同时死亡，则前者死亡。\n傀儡师不可以执行正常击杀。 ",
     "时间管理者": "时间管理者(TimeManager)(船员阵营):每当完成一个任务时,会议的时间会延长。",
     "千面鬼": "千面鬼(ShapeMaster)(内鬼阵营):千面鬼没有变形冷却与次数限制。PS:在默认设置下，千面鬼变形的持续时间更短(10秒)",
     "实干家": "实干家(workhorse)(效果):这个效果会赋予第一个活着完成任务的船员.会获得额外的任务。PS：不会赋予警长和告密者。",
     "狐狸": "狐狸(HASFox)(躲猫猫职业/独立阵营):狐狸活到最后便与获胜阵营一同获胜",
     "猎人": "猎人(HASTroll)(躲猫猫职业/独立阵营):若猎人被抓，则猎人单独获胜.PS:在这种情况下，即使狐狸未被抓，狐狸也会输掉游戏。",
     "绝境者": "绝境者(LastImpostor)(效果):这个效果在内鬼仅剩一人时赋予该内鬼。使其击杀冷却缩短。PS:该效果对赏金猎人、嗜血杀手以及吸血鬼不适用。",
+    "实干家":"实干家（Workhorse）(附加效果):\n该附加效果赋予给第一个完成所有任务并存活的船员。\n你需要完成额外的任务来达成任务胜利。\n此效果不会赋予那些没有任务或者通过完成任务才能使用能力的诸多职业。",
+    "窥视者":"窥视者（Watcher）(附加效果):\n會議時觀察者可以看到所有人的投票。",
     "管理员": "GM(管理员)(无阵营):GM(管理员)是房主专属的观察者职业。从游戏开始时便以幽灵状态在旁边观战。 该职业本身对游戏没有影响，且会议中对所有玩家可见(就是一个开局死的怨种(",
 }
```

### Comparing `nonebot_plugin_aujob-0.1.4/pyproject.toml` & `nonebot_plugin_aujob-0.2.114514/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nonebot_plugin_aujob"
-version = "0.1.4"
+version = "0.2.114514"
 authors = [
   { name="qwqZYLqwq", email="3422471182@qq.com" },
 ]
 description = "A nonebot plugin"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

