# Comparing `tmp/get-music-lizhanqi-1.2.8.tar.gz` & `tmp/get-music-lizhanqi-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\???\Desktop\get_music\dist\.tmp-ibl8a653\get-music-lizhanqi-1.2.8.tar", last modified: Sat Jul 29 10:45:32 2023, max compression
+gzip compressed data, was "C:\Users\???\Desktop\get_music\dist\.tmp-pvcp5wic\get-music-lizhanqi-1.2.9.tar", last modified: Sun Jul 30 04:24:36 2023, max compression
```

## Comparing `get-music-lizhanqi-1.2.8.tar` & `get-music-lizhanqi-1.2.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 10:45:32.000000 get-music-lizhanqi-1.2.8/
--rw-rw-rw-   0        0        0     1091 2022-04-09 10:07:52.000000 get-music-lizhanqi-1.2.8/LICENSE.txt
--rw-rw-rw-   0        0        0     1660 2023-07-29 10:45:32.000000 get-music-lizhanqi-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     1246 2023-07-29 10:44:28.000000 get-music-lizhanqi-1.2.8/README.md
--rw-rw-rw-   0        0        0       86 2022-04-09 10:04:03.000000 get-music-lizhanqi-1.2.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-29 10:45:32.000000 get-music-lizhanqi-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0      952 2023-07-29 10:44:53.000000 get-music-lizhanqi-1.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 10:45:32.000000 get-music-lizhanqi-1.2.8/tests/
-drwxrwxrwx   0        0        0        0 2023-07-29 10:45:32.000000 get-music-lizhanqi-1.2.8/tests/get_music/
--rw-rw-rw-   0        0        0      266 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/__init__.py
--rw-rw-rw-   0        0        0     3092 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/baidu.py
--rw-rw-rw-   0        0        0     1938 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/download.py
--rw-rw-rw-   0        0        0     2892 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/downloads.py
--rw-rw-rw-   0        0        0     3363 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/fivesing.py
--rw-rw-rw-   0        0        0    10519 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/get_music.py
--rw-rw-rw-   0        0        0    11919 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/gui.py
--rw-rw-rw-   0        0        0     2613 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/kg_one_playerlist.py
--rw-rw-rw-   0        0        0     2570 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/kg_playerlist.py
--rw-rw-rw-   0        0        0     5305 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/kugou.py
--rw-rw-rw-   0        0        0     5575 2023-07-29 10:42:14.000000 get-music-lizhanqi-1.2.8/tests/get_music/kuwo.py
--rw-rw-rw-   0        0        0     2685 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/kw_playerlist.py
--rw-rw-rw-   0        0        0     2861 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/migu.py
--rw-rw-rw-   0        0        0     3763 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/netease.py
--rw-rw-rw-   0        0        0     2090 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/oneting.py
--rw-rw-rw-   0        0        0     3306 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/playerlist.py
--rw-rw-rw-   0        0        0     4293 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/qq.py
--rw-rw-rw-   0        0        0     2534 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/qq_playerlist.py
--rw-rw-rw-   0        0        0     2569 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/singbz.py
--rw-rw-rw-   0        0        0     6826 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/top.py
--rw-rw-rw-   0        0        0     2214 2023-07-29 10:43:41.000000 get-music-lizhanqi-1.2.8/tests/get_music/ver.py
--rw-rw-rw-   0        0        0     3119 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/wy_playerlist.py
--rw-rw-rw-   0        0        0     3692 2023-07-28 13:16:26.000000 get-music-lizhanqi-1.2.8/tests/get_music/zhidao.py
-drwxrwxrwx   0        0        0        0 2023-07-29 10:45:32.000000 get-music-lizhanqi-1.2.8/tests/get_music_lizhanqi.egg-info/
--rw-rw-rw-   0        0        0     1660 2023-07-29 10:45:32.000000 get-music-lizhanqi-1.2.8/tests/get_music_lizhanqi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      971 2023-07-29 10:45:32.000000 get-music-lizhanqi-1.2.8/tests/get_music_lizhanqi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 10:45:32.000000 get-music-lizhanqi-1.2.8/tests/get_music_lizhanqi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      101 2023-07-29 10:45:32.000000 get-music-lizhanqi-1.2.8/tests/get_music_lizhanqi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-07-29 10:45:32.000000 get-music-lizhanqi-1.2.8/tests/get_music_lizhanqi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-29 10:45:32.000000 get-music-lizhanqi-1.2.8/tests/get_music_lizhanqi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 04:24:36.000000 get-music-lizhanqi-1.2.9/
+-rw-rw-rw-   0        0        0     1091 2022-04-09 10:07:52.000000 get-music-lizhanqi-1.2.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     1868 2023-07-30 04:24:36.000000 get-music-lizhanqi-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1454 2023-07-30 04:23:57.000000 get-music-lizhanqi-1.2.9/README.md
+-rw-rw-rw-   0        0        0       86 2022-04-09 10:04:03.000000 get-music-lizhanqi-1.2.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-30 04:24:36.000000 get-music-lizhanqi-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      967 2023-07-30 04:17:35.000000 get-music-lizhanqi-1.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 04:24:35.000000 get-music-lizhanqi-1.2.9/tests/
+drwxrwxrwx   0        0        0        0 2023-07-30 04:24:36.000000 get-music-lizhanqi-1.2.9/tests/get_music/
+-rw-rw-rw-   0        0        0      266 2023-07-29 10:51:30.000000 get-music-lizhanqi-1.2.9/tests/get_music/__init__.py
+-rw-rw-rw-   0        0        0     3092 2023-07-29 10:51:30.000000 get-music-lizhanqi-1.2.9/tests/get_music/baidu.py
+-rw-rw-rw-   0        0        0     1963 2023-07-30 03:48:00.000000 get-music-lizhanqi-1.2.9/tests/get_music/download.py
+-rw-rw-rw-   0        0        0     2892 2023-07-29 10:51:30.000000 get-music-lizhanqi-1.2.9/tests/get_music/downloads.py
+-rw-rw-rw-   0        0        0     3363 2023-07-29 10:51:30.000000 get-music-lizhanqi-1.2.9/tests/get_music/fivesing.py
+-rw-rw-rw-   0        0        0    10519 2023-07-30 03:39:22.000000 get-music-lizhanqi-1.2.9/tests/get_music/get_music.py
+-rw-rw-rw-   0        0        0    11919 2023-07-29 10:51:30.000000 get-music-lizhanqi-1.2.9/tests/get_music/gui.py
+-rw-rw-rw-   0        0        0     2613 2023-07-29 10:51:30.000000 get-music-lizhanqi-1.2.9/tests/get_music/kg_one_playerlist.py
+-rw-rw-rw-   0        0        0     2570 2023-07-29 10:51:30.000000 get-music-lizhanqi-1.2.9/tests/get_music/kg_playerlist.py
+-rw-rw-rw-   0        0        0     5305 2023-07-29 10:51:30.000000 get-music-lizhanqi-1.2.9/tests/get_music/kugou.py
+-rw-rw-rw-   0        0        0     5575 2023-07-29 10:51:30.000000 get-music-lizhanqi-1.2.9/tests/get_music/kuwo.py
+-rw-rw-rw-   0        0        0     2685 2023-07-29 10:51:30.000000 get-music-lizhanqi-1.2.9/tests/get_music/kw_playerlist.py
+-rw-rw-rw-   0        0        0     2861 2023-07-29 10:51:30.000000 get-music-lizhanqi-1.2.9/tests/get_music/migu.py
+-rw-rw-rw-   0        0        0     7723 2023-07-30 03:48:21.000000 get-music-lizhanqi-1.2.9/tests/get_music/netease.py
+-rw-rw-rw-   0        0        0     2090 2023-07-29 10:51:30.000000 get-music-lizhanqi-1.2.9/tests/get_music/oneting.py
+-rw-rw-rw-   0        0        0     3306 2023-07-29 10:51:30.000000 get-music-lizhanqi-1.2.9/tests/get_music/playerlist.py
+-rw-rw-rw-   0        0        0     4564 2023-07-30 01:37:49.000000 get-music-lizhanqi-1.2.9/tests/get_music/qq.py
+-rw-rw-rw-   0        0        0     2534 2023-07-29 10:51:30.000000 get-music-lizhanqi-1.2.9/tests/get_music/qq_playerlist.py
+-rw-rw-rw-   0        0        0     2569 2023-07-29 10:51:30.000000 get-music-lizhanqi-1.2.9/tests/get_music/singbz.py
+-rw-rw-rw-   0        0        0     6936 2023-07-30 01:04:16.000000 get-music-lizhanqi-1.2.9/tests/get_music/top.py
+-rw-rw-rw-   0        0        0     2214 2023-07-30 04:17:23.000000 get-music-lizhanqi-1.2.9/tests/get_music/ver.py
+-rw-rw-rw-   0        0        0     3119 2023-07-29 10:51:30.000000 get-music-lizhanqi-1.2.9/tests/get_music/wy_playerlist.py
+-rw-rw-rw-   0        0        0     2392 2023-07-30 04:16:11.000000 get-music-lizhanqi-1.2.9/tests/get_music/zhidao.py
+drwxrwxrwx   0        0        0        0 2023-07-30 04:24:36.000000 get-music-lizhanqi-1.2.9/tests/get_music_lizhanqi.egg-info/
+-rw-rw-rw-   0        0        0     1868 2023-07-30 04:24:35.000000 get-music-lizhanqi-1.2.9/tests/get_music_lizhanqi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      971 2023-07-30 04:24:35.000000 get-music-lizhanqi-1.2.9/tests/get_music_lizhanqi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 04:24:35.000000 get-music-lizhanqi-1.2.9/tests/get_music_lizhanqi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      101 2023-07-30 04:24:35.000000 get-music-lizhanqi-1.2.9/tests/get_music_lizhanqi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2023-07-30 04:24:35.000000 get-music-lizhanqi-1.2.9/tests/get_music_lizhanqi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-30 04:24:35.000000 get-music-lizhanqi-1.2.9/tests/get_music_lizhanqi.egg-info/top_level.txt
```

### Comparing `get-music-lizhanqi-1.2.8/LICENSE.txt` & `get-music-lizhanqi-1.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.8/README.md` & `get-music-lizhanqi-1.2.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 - 这是一个可以下载和搜索音乐的python命令行工具，支持，酷狗，酷我，百度，网易云，咪咕，qq音乐，5sing，欢迎前来学习的指点
 
 ## 使用方法
 - 长话短说**get-music -help**或**get-music-lizhanqi -help**打开帮助，帮助里面有全部命令的介绍，或者前往github地址:<https://github.com/lzq-hopego/get-music-lizhanqi>
 
 
 ## 更新记录
-- 2023-07-29 完成v1.2.8版本,修复酷我音乐接口失效的错误。
+- 2023-07-30 完成v1.2.9版本,修复网易云音乐无法返回的bug，修复网易云音乐无法下载歌词和封面的bug，修复qq音乐无法下载的bug，修复qq音乐无法从歌词列表下载的问题，修复热歌榜单，修复无法从网盘资源中查找的bug
 
 
 
 
 ## THE END
 - 本脚本仅支持学习使用，如有发现有任何商业用途，一经发现您将受到法律责任。
 - 本程序使用的接口全部来源于网络，切不可有任何商业用途，或我程序中有涉及你公司利益的，你可以联系我，我会及时删除源代码，并不再更新。
```

### Comparing `get-music-lizhanqi-1.2.8/setup.py` & `get-music-lizhanqi-1.2.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="get-music-lizhanqi",
-    version="1.2.8",
+    version="1.2.9",
     author="Li Zhan Qi",
     author_email="3101978435@qq.com",
     description="可以下载音乐的包哦",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     project_urls={
@@ -18,14 +18,14 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "tests"},
     packages=setuptools.find_packages(where="tests"),
     python_requires=">=3.7",
-    install_requires=["requests",'rich'],
+    install_requires=["requests",'rich','pycryptodome'],
     entry_points={
         'console_scripts': ["get-music=get_music.get_music:main",
                             "get-music-lizhanqi=get_music.get_music:main"
             ],
     },
 )
```

### Comparing `get-music-lizhanqi-1.2.8/tests/get_music/baidu.py` & `get-music-lizhanqi-1.2.9/tests/get_music/baidu.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.8/tests/get_music/download.py` & `get-music-lizhanqi-1.2.9/tests/get_music/download.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 from rich.progress import Progress
 import rich
 from rich.console import Console
 import os
 
 
 def download(url,name,ouput=False,or_re=True):
+    url=str(url).strip('"')
     console=Console()
     if ouput==True:
         print()
     if url=='':
         console.print('[b red]下载链接为空！')
     if or_re:
         rstr = r"[\/\\\:\*\?\"\<\>\|\&]"  # '/ \ : * ? " < > |'
         name = re.sub(rstr, "_", name)  # 替换为下划线
         if os.path.exists(r"./"+name):
             yorn=console.input('[b green]“[b red]{}[/]”已下载是否重新下载(Y/N):'.format(name))
             if yorn not in ['y','Y','是']:
                 return
-    response = requests.get(url, stream = True,timeout = 0.8)  # stream=True必须写上
+    response = requests.get(url, stream = True,timeout = 3)  # stream=True必须写上
     size = 0  # 初始化已下载大小
     chunk_size = 1024  # 每次下载的数据大小
     content_size = int(response.headers['content-length'])  # 下载文件总大小
     c_size="[b green]文件总大小:[b red]{:.2f}MB[/]".format(content_size/1024/1024)
-
     with Progress(rich.progress.TextColumn("[progress.description]{task.description}")
                   ,rich.progress.BarColumn()
                   ,c_size
                   ,rich.progress.TaskProgressColumn()
                   ,rich.progress.TimeRemainingColumn()
                   ,rich.progress.TransferSpeedColumn()
                   ) as progress:
```

### Comparing `get-music-lizhanqi-1.2.8/tests/get_music/downloads.py` & `get-music-lizhanqi-1.2.9/tests/get_music/downloads.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.8/tests/get_music/fivesing.py` & `get-music-lizhanqi-1.2.9/tests/get_music/fivesing.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.8/tests/get_music/get_music.py` & `get-music-lizhanqi-1.2.9/tests/get_music/get_music.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.8/tests/get_music/gui.py` & `get-music-lizhanqi-1.2.9/tests/get_music/gui.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.8/tests/get_music/kg_one_playerlist.py` & `get-music-lizhanqi-1.2.9/tests/get_music/kg_one_playerlist.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.8/tests/get_music/kg_playerlist.py` & `get-music-lizhanqi-1.2.9/tests/get_music/kg_playerlist.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.8/tests/get_music/kugou.py` & `get-music-lizhanqi-1.2.9/tests/get_music/kugou.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.8/tests/get_music/kuwo.py` & `get-music-lizhanqi-1.2.9/tests/get_music/kuwo.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.8/tests/get_music/kw_playerlist.py` & `get-music-lizhanqi-1.2.9/tests/get_music/kw_playerlist.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.8/tests/get_music/migu.py` & `get-music-lizhanqi-1.2.9/tests/get_music/migu.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.8/tests/get_music/netease.py` & `get-music-lizhanqi-1.2.9/tests/get_music/singbz.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,93 +1,58 @@
-import requests,json
-from get_music import download
+import requests,re,json
+import urllib.parse
 from rich.console import Console
-# import download
 console=Console()
 
-class netease:
+class singbz:
     def __init__(self,p=False,l=False):
-        self.url='http://music.163.com/api/cloudsearch/pc'
-        self.headers={'referer':'http://music.163.com/',
-        'proxy':"false",
-        'user-agent':'Mozilla/5.0 (iPhone; CPU iPhone OS 9_1 like Mac OS X) AppleWebKit/601.1.46 (KHTML, like Gecko) Version/9.0 Mobile/13B143 Safari/601.1'}
-        self.data={'s':'',
-        'type':1,
-        'offset':1,
-        'limit':20}
+        self.api='5Sing伴奏'
         self.l=l
         self.p=p
-        self.api='网易云音乐'
-    def search(self,songname,page=0):
-        self.data['offset']=self.page=page
-        self.data['s']=self.song_name=songname
-        req=requests.post(self.url,headers=self.headers,data=self.data,timeout=1)
-        d=json.loads(req.text)
-        song_url=['http://music.163.com/song/media/outer/url?id=','.mp3']
-        songs=d["result"]['songs']
-        self.songname=[]
+        
+    def search(self,songname,page=1):
+        self.song_name=songname
+        self.page=page
+        songname=urllib.parse.quote(songname)
+        headers={'referer': 'http://search.5sing.kugou.com/?keyword=',
+                 'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/99.0.4844.84 Safari/537.36',
+                 "Accept" : "application/json, text/javascript, */*; q=0.01"}
+        headers['referer']=headers.get('referer')+songname
+        url='http://search.5sing.kugou.com/home/json?keyword={}&sort=1&page={}&filter=3&type=0'.format(songname,page)
+        req=requests.get(url,headers=headers,timeout=3)
+        d=req.json()
         self.songs_url=[]
+        self.songname=[]
         self.singername=[]
+        for i in d['list']:
+                    self.songs_url.append(i['songId'])
+                    self.singername.append(i['originSinger']+'-'+i['nickName'])
+                    self.songname.append(i['songName'].replace('<em class="keyword">','').replace('</em>',''))
 
-        self.id=[]
-        self.pic=[]
-        for i in songs:
-                self.songs_url.append(str(i['id']).join(song_url))
-                self.songname.append(i["name"])
-                self.singername.append(i['ar'][0]["name"])
-                self.id.append(i['id'])
-                self.pic.append(i['al']['picUrl'])
         return self.songname,self.singername,self.songs_url
-    def get_music_url(self,url):
-        if 'http:' not in url:
-            return 'http://music.163.com/song/media/outer/url?id={}.mp3'.format(url)
-        return url
-    def get_music_lrc(self,num,return_url=False):
-        headers = {
-                "user-agent" : "Mozilla/5.0",
-                "Referer" : "http://music.163.com",
-                "Host" : "music.163.com"
-            }
-        try:
-            song_id=self.id[num]
-            if not isinstance(song_id, str):
-                song_id = str(song_id)
-            url = f"http://music.163.com/api/song/lyric?id={song_id}+&lv=1&tv=-1"
-            r = requests.get(url, headers=headers,timeout=1)
-            r.raise_for_status()
-            r.encoding = r.apparent_encoding
-            json_obj = json.loads(r.text)
-            if return_url:
-                return json_obj["lrc"]["lyric"]
-            name=self.songname[num]+"-"+self.songername[num]+'-'+"歌词.txt"
-            name=name.replace(':','_').replace('?','_').replace('|','_').replace('"','_').replace('<','_').replace('>','_')
-            with open(name,'w') as f:
-                f.write(json_obj["lrc"]["lyric"])
-            console.print("[b red]\n\n歌词已下载完成,文件名称为:"+name+"\n")
-        except:
-            if type(num)==str:
-                url = f"http://music.163.com/api/song/lyric?id={num}+&lv=1&tv=-1"
-                r = requests.get(url, headers=headers,timeout=1)
-                r.raise_for_status()
-                r.encoding = r.apparent_encoding
-                json_obj = json.loads(r.text)
-                return json_obj["lrc"]["lyric"]
+    
+    def get_music_url(self,songid):
+        
+        jx='http://service.5sing.kugou.com/song/getsongurl?songid={}&songtype=bz&from=web&version=6.6.72&_=1673862766682'.format(songid)
+        headers={'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/99.0.4844.84 Safari/537.36'
+                          }
 
-            else:
-                console.print("[b red]未找到该歌曲的歌词！")
-    def get_music_pic(self,num,return_url=False):
-        try:
-            url=self.pic[num]
-            if return_url:
-                return url
-            name=self.songname[num]+"-"+self.singername[num]+'-'+"封面.jpg"
-            download.download(url,name)
-            console.print("[b red]\n歌曲封面下载完成，文件名称为:"+name)
-        except:
+        req=requests.get(jx,headers=headers,timeout=1)
+        txt=json.loads(req.text[1:-1])
+        if txt['message'] != '成功':
+            console.print('[b red]无法解析，或出现故障，故障代码:'+txt['code'])
 
-            console.print("[b red]未找到该歌曲的封面！")
-
-##测试代码
-##a=netease(l=True,p=True)
-##d=a.search("11")
-##a.prints()
-##input()
+        song_squrl=txt['data']['squrl']
+        if song_squrl=='':
+            song_squrl=txt['data']['squrl_backup']
+            
+        song_lqurl=txt['data']['lqurl']
+        if song_lqurl=='':
+            song_lqurl=txt['data']['lqurl_backup']
+        downloadurl=song_squrl
+        if downloadurl=='':
+            downloadurl=song_lqurl
+        return downloadurl
+    def get_music_lrc(self,num,return_url=False):
+        console.print('[b red]本接口不支持歌词！')
+    def get_music_pic(self,num,return_url=False):
+        console.print('[b red]本接口不支持封面！')
```

### Comparing `get-music-lizhanqi-1.2.8/tests/get_music/oneting.py` & `get-music-lizhanqi-1.2.9/tests/get_music/oneting.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.8/tests/get_music/playerlist.py` & `get-music-lizhanqi-1.2.9/tests/get_music/playerlist.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.8/tests/get_music/qq.py` & `get-music-lizhanqi-1.2.9/tests/get_music/qq.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,20 +32,26 @@
             self.singername.append(','.join([i['name'] for i in i['singer']]))
             self.songs_url.append(i['songmid'])
         return self.songname,self.singername,self.songs_url
     def prints(self):
         pass
 
     def get_music_url(self,songid):
+        head={
+        'User-Agent':'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/115.0.0.0 Safari/537.36',
+        'Host':'u.y.qq.com'
+            }
         url_part = "https://u.y.qq.com/cgi-bin/musicu.fcg?format=json&data=%7B%22req_0%22%3A%7B%22module%22%3A%22vkey.GetVkeyServer%22%2C%22method%22%3A%22CgiGetVkey%22%2C%22param%22%3A%7B%22guid%22%3A%22358840384%22%2C%22songmid%22%3A%5B%22{}%22%5D%2C%22songtype%22%3A%5B0%5D%2C%22uin%22%3A%221443481947%22%2C%22loginflag%22%3A1%2C%22platform%22%3A%2220%22%7D%7D%2C%22comm%22%3A%7B%22uin%22%3A%2218585073516%22%2C%22format%22%3A%22json%22%2C%22ct%22%3A24%2C%22cv%22%3A0%7D%7D".format(songid)
-        music_document_html_json = requests.get(url_part,timeout=1).text
+        music_document_html_json = requests.get(url_part,timeout=1,headers=head).text
         music_document_html_dict = json.loads(music_document_html_json)  #将文件从json格式转化为字典格式
         music_url_part = music_document_html_dict["req_0"]["data"]["midurlinfo"][0]["purl"]
         if music_url_part != '':
             return music_document_html_dict['req_0']['data']['sip'][0]+music_url_part
+        else:
+            return ''
 
     def get_music_pic(self,num,return_url=False):
         try:
             url='https://y.gtimg.cn/music/photo_new/T002R300x300M000'+self.mid[num]+'.jpg'
             if return_url:
                 return url
             name=self.songname[num]+"-"+self.singername[num]+'-'+"封面.jpg"
@@ -54,19 +60,20 @@
         except:
             console.print("[b red]未找到该歌曲的封面！")
     def get_music_lrc(self,num,return_url=False):
         try:
             name=self.songname[num]+"-"+self.singername[num]+'-'+"歌词.txt"
             headers={'user-agent':'Mozilla/5.0 (iPhone; CPU iPhone OS 9_1 like Mac OS X) AppleWebKit/601.1.46 (KHTML, like Gecko) Version/9.0 Mobile/13B143 Safari/601.1',
              'referer' : 'https://m.y.qq.com'}
-            url='https://c.y.qq.com/lyric/fcgi-bin/fcg_query_lyric.fcg?songmid={}&format=json&nobase64=1&songtype=0&callback=c'.format(self.song_url[num])
+            url='https://c.y.qq.com/lyric/fcgi-bin/fcg_query_lyric.fcg?songmid={}&format=json&nobase64=1&songtype=0&callback=c'.format(self.songs_url[num])
             html=requests.get(url,headers=headers,timeout=1)
             html.encoding='utf-8'
             d = unescape(html.text).split('"lyric":"')[-1][:-3]
             if return_url:
+                
                 return d
             name=name.replace(':','_').replace('?','_').replace('|','_').replace('"','_').replace('<','_').replace('>','_')
             with open(name,'w',encoding='utf-8') as f:
                 f.write(d)
             console.print("[b red]\n\n歌词已下载完成,文件名称为:"+name+"\n")
         except:
             console.print("[b red]未找到该歌曲的歌词！")
@@ -74,11 +81,11 @@
     string = urllib.parse.unquote(string)
     quoted = html.unescape(string).encode(sys.getfilesystemencoding()).decode('utf-8')
     #转成中文
     return re.sub(r'%u([a-fA-F0-9]{4}|[a-fA-F0-9]{2})', lambda m: chr(int(m.group(1), 16)), quoted)
 
 ##测试代码
 ##a=qq(l=True)
-##a.search('11')
-##a.get_music_lrc(1)
+##a.search('微微')
+##a.get_music_lrc(0)
 ##a.prints()
 ##input()
```

### Comparing `get-music-lizhanqi-1.2.8/tests/get_music/qq_playerlist.py` & `get-music-lizhanqi-1.2.9/tests/get_music/qq_playerlist.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.8/tests/get_music/top.py` & `get-music-lizhanqi-1.2.9/tests/get_music/top.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,21 +37,20 @@
            'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/92.0.4515.131 Safari/537.36 SLBrowser/8.0.0.7062 SLBChan/33',
            'Host': 'www.kuwo.cn',
            'Upgrade-Insecure-Requests': '1',
            'Connection': 'keep-alive'
            }
     head={'Accept': 'application/json, text/plain, */*',
       'Referer': 'http://www.kuwo.cn/rankList',
-      'csrf': '4M57QR4C1S8',
+      'Secret':'6d0d0d09bef3a951f058a52dd08faea944c789c5e7a765d932253fa2e6f2544c033bf066',
       'Host': 'www.kuwo.cn',
-          'Connection': 'keep-alive',
-      'Cookie': '_ga=GA1.2.1158784231.1649567141; Hm_lvt_cdb524f42f0ce19b169a8071123a4797=1671888291; Hm_lpvt_cdb524f42f0ce19b169a8071123a4797=1671888291; kw_token=4M57QR4C1S8; _gid=GA1.2.368264343.1671888291; _gat=1',
+      'Cookie': '_ga=GA1.2.438975400.1690625730; _gid=GA1.2.265176886.1690625730; Hm_lvt_cdb524f42f0ce19b169a8071123a4797=1690625730,1690678334; Hm_lpvt_cdb524f42f0ce19b169a8071123a4797=1690678334; _gat=1; _ga_ETPBRPM9ML=GS1.2.1690678334.2.0.1690678334.60.0.0; Hm_Iuvt_cdb524f42f0ce19b169b8072123a4727=3QweDwDXNcHmti7TyrpMZJYRJY3sBKCw',
       'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.81 Safari/537.36 Edg/104.0.1293.54'}
-    s.get('http://www.kuwo.cn/rankList',headers=head1)
-    html=s.get('http://www.kuwo.cn/api/www/bang/bang/musicList?bangId=16&pn=1&rn=30&httpsStatus=1&reqId=c5f29300-8373-11ed-bc47-1dc98d5c838f',headers=head).json()
+    
+    html=s.get('http://www.kuwo.cn/api/www/bang/bang/musicList?bangId=93&pn=1&rn=20&httpsStatus=1&reqId=5e0e5b60-2e73-11ee-9fdb-b195a0885957&plat=web_www&from=',headers=head).json()
 
     songname=[]
     singer=[]
     songid=[]
     for i in html['data']['musicList']:
         songname.append(i['album'])
         singer.append(i['artist'])
```

### Comparing `get-music-lizhanqi-1.2.8/tests/get_music/ver.py` & `get-music-lizhanqi-1.2.9/tests/get_music/ver.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
                 url = 'http://api.ip33.com/ip/search?s='                     
                 d = requests.get(url,timeout=1).json()                                                       
                 console.print('\n[b green]信息二:本机外网ip地址为:[b red]{}[/]，归属:[b red]{}[/]'.format(d['ip'],d['area']))
             except:
                 console.print("\n[b red]ip地址信息查二询失败！")
             return
     
-    version = '1.2.8'
+    version = '1.2.9'
     console.print("[green]当前版本:"+"v"+version)
     url = 'https://pypi.org/project/get-music-lizhanqi/#history'
     try:
         with console.status("[b green]检查最新版中..."):
             html = requests.get(url,timeout = 5)
             txt = html.text
             crad = re.findall(r' <a class="card release__card" href="/project/get-music-lizhanqi/(.*?)/">',txt,re.S)
```

### Comparing `get-music-lizhanqi-1.2.8/tests/get_music/wy_playerlist.py` & `get-music-lizhanqi-1.2.9/tests/get_music/wy_playerlist.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.8/tests/get_music_lizhanqi.egg-info/SOURCES.txt` & `get-music-lizhanqi-1.2.9/tests/get_music_lizhanqi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

