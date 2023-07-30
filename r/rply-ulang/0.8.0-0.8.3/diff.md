# Comparing `tmp/rply-ulang-0.8.0.tar.gz` & `tmp/rply-ulang-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rply-ulang-0.8.0.tar", last modified: Wed Sep 29 17:14:47 2021, max compression
+gzip compressed data, was "rply-ulang-0.8.3.tar", last modified: Sun Jul 30 14:16:43 2023, max compression
```

## Comparing `rply-ulang-0.8.0.tar` & `rply-ulang-0.8.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 xuanwu     (501) staff       (20)        0 2021-09-29 17:14:47.000000 rply-ulang-0.8.0/
--rw-r--r--   0 xuanwu     (501) staff       (20)     1535 2021-07-01 21:15:16.000000 rply-ulang-0.8.0/LICENSE
--rw-r--r--   0 xuanwu     (501) staff       (20)       35 2021-07-01 21:15:16.000000 rply-ulang-0.8.0/MANIFEST.in
--rw-r--r--   0 xuanwu     (501) staff       (20)     6162 2021-09-29 17:14:47.000000 rply-ulang-0.8.0/PKG-INFO
--rw-r--r--   0 xuanwu     (501) staff       (20)     4756 2021-09-29 17:14:40.000000 rply-ulang-0.8.0/README.rst
-drwxr-xr-x   0 xuanwu     (501) staff       (20)        0 2021-09-29 17:14:47.000000 rply-ulang-0.8.0/rply/
--rw-r--r--   0 xuanwu     (501) staff       (20)      553 2021-09-29 16:11:12.000000 rply-ulang-0.8.0/rply/__init__.py
--rw-r--r--   0 xuanwu     (501) staff       (20)      143 2021-07-01 21:15:16.000000 rply-ulang-0.8.0/rply/errors.py
--rw-r--r--   0 xuanwu     (501) staff       (20)      462 2021-08-18 07:29:35.000000 rply-ulang-0.8.0/rply/lexergenerator.py
--rw-r--r--   0 xuanwu     (501) staff       (20)      438 2021-08-18 07:29:35.000000 rply-ulang-0.8.0/rply/parsergenerator.py
--rw-r--r--   0 xuanwu     (501) staff       (20)       90 2021-08-18 07:29:35.000000 rply-ulang-0.8.0/rply/token.py
--rw-r--r--   0 xuanwu     (501) staff       (20)     8465 2021-09-28 08:11:36.000000 rply-ulang-0.8.0/rply/分词器.py
--rw-r--r--   0 xuanwu     (501) staff       (20)     2808 2021-09-19 16:36:56.000000 rply-ulang-0.8.0/rply/分词器母机.py
--rw-r--r--   0 xuanwu     (501) staff       (20)     1257 2021-08-18 07:29:35.000000 rply-ulang-0.8.0/rply/功用.py
--rw-r--r--   0 xuanwu     (501) staff       (20)     1427 2021-09-23 08:37:39.000000 rply-ulang-0.8.0/rply/报错.py
--rw-r--r--   0 xuanwu     (501) staff       (20)     2399 2021-08-18 07:29:35.000000 rply-ulang-0.8.0/rply/词.py
--rw-r--r--   0 xuanwu     (501) staff       (20)     7920 2021-08-18 07:29:35.000000 rply-ulang-0.8.0/rply/语法.py
--rw-r--r--   0 xuanwu     (501) staff       (20)     7281 2021-09-23 23:40:46.000000 rply-ulang-0.8.0/rply/语法分析器.py
--rw-r--r--   0 xuanwu     (501) staff       (20)    24074 2021-08-18 07:29:35.000000 rply-ulang-0.8.0/rply/语法分析器母机.py
-drwxr-xr-x   0 xuanwu     (501) staff       (20)        0 2021-09-29 17:14:47.000000 rply-ulang-0.8.0/rply_ulang.egg-info/
--rw-r--r--   0 xuanwu     (501) staff       (20)     6162 2021-09-29 17:14:47.000000 rply-ulang-0.8.0/rply_ulang.egg-info/PKG-INFO
--rw-r--r--   0 xuanwu     (501) staff       (20)      464 2021-09-29 17:14:47.000000 rply-ulang-0.8.0/rply_ulang.egg-info/SOURCES.txt
--rw-r--r--   0 xuanwu     (501) staff       (20)        1 2021-09-29 17:14:47.000000 rply-ulang-0.8.0/rply_ulang.egg-info/dependency_links.txt
--rw-r--r--   0 xuanwu     (501) staff       (20)        8 2021-09-29 17:14:47.000000 rply-ulang-0.8.0/rply_ulang.egg-info/requires.txt
--rw-r--r--   0 xuanwu     (501) staff       (20)        5 2021-09-29 17:14:47.000000 rply-ulang-0.8.0/rply_ulang.egg-info/top_level.txt
--rw-r--r--   0 xuanwu     (501) staff       (20)      104 2021-09-29 17:14:47.000000 rply-ulang-0.8.0/setup.cfg
--rw-r--r--   0 xuanwu     (501) staff       (20)      528 2021-09-29 16:10:59.000000 rply-ulang-0.8.0/setup.py
+drwxr-xr-x   0 xuanwu     (501) staff       (20)        0 2023-07-30 14:16:43.799268 rply-ulang-0.8.3/
+-rw-r--r--   0 xuanwu     (501) staff       (20)     1535 2021-07-01 21:15:16.000000 rply-ulang-0.8.3/LICENSE
+-rw-r--r--   0 xuanwu     (501) staff       (20)       35 2021-07-01 21:15:16.000000 rply-ulang-0.8.3/MANIFEST.in
+-rw-r--r--   0 xuanwu     (501) staff       (20)     6162 2023-07-30 14:16:43.799409 rply-ulang-0.8.3/PKG-INFO
+-rw-r--r--   0 xuanwu     (501) staff       (20)     4756 2021-09-29 19:20:31.000000 rply-ulang-0.8.3/README.rst
+drwxr-xr-x   0 xuanwu     (501) staff       (20)        0 2023-07-30 14:16:43.797617 rply-ulang-0.8.3/rply/
+-rw-r--r--   0 xuanwu     (501) staff       (20)      553 2021-09-29 19:20:31.000000 rply-ulang-0.8.3/rply/__init__.py
+-rw-r--r--   0 xuanwu     (501) staff       (20)      143 2021-07-01 21:15:16.000000 rply-ulang-0.8.3/rply/errors.py
+-rw-r--r--   0 xuanwu     (501) staff       (20)      462 2021-08-18 07:29:35.000000 rply-ulang-0.8.3/rply/lexergenerator.py
+-rw-r--r--   0 xuanwu     (501) staff       (20)      438 2021-08-18 07:29:35.000000 rply-ulang-0.8.3/rply/parsergenerator.py
+-rw-r--r--   0 xuanwu     (501) staff       (20)       90 2021-08-18 07:29:35.000000 rply-ulang-0.8.3/rply/token.py
+-rw-r--r--   0 xuanwu     (501) staff       (20)     8465 2023-07-30 14:16:02.000000 rply-ulang-0.8.3/rply/分词器.py
+-rw-r--r--   0 xuanwu     (501) staff       (20)     2808 2021-09-29 19:20:31.000000 rply-ulang-0.8.3/rply/分词器母机.py
+-rw-r--r--   0 xuanwu     (501) staff       (20)     1257 2021-08-18 07:29:35.000000 rply-ulang-0.8.3/rply/功用.py
+-rw-r--r--   0 xuanwu     (501) staff       (20)     1427 2021-09-29 19:20:31.000000 rply-ulang-0.8.3/rply/报错.py
+-rw-r--r--   0 xuanwu     (501) staff       (20)     2399 2021-08-18 07:29:35.000000 rply-ulang-0.8.3/rply/词.py
+-rw-r--r--   0 xuanwu     (501) staff       (20)     7920 2021-08-18 07:29:35.000000 rply-ulang-0.8.3/rply/语法.py
+-rw-r--r--   0 xuanwu     (501) staff       (20)     7297 2023-07-30 14:15:46.000000 rply-ulang-0.8.3/rply/语法分析器.py
+-rw-r--r--   0 xuanwu     (501) staff       (20)    24134 2023-02-18 15:32:43.000000 rply-ulang-0.8.3/rply/语法分析器母机.py
+drwxr-xr-x   0 xuanwu     (501) staff       (20)        0 2023-07-30 14:16:43.799143 rply-ulang-0.8.3/rply_ulang.egg-info/
+-rw-r--r--   0 xuanwu     (501) staff       (20)     6162 2023-07-30 14:16:43.000000 rply-ulang-0.8.3/rply_ulang.egg-info/PKG-INFO
+-rw-r--r--   0 xuanwu     (501) staff       (20)      464 2023-07-30 14:16:43.000000 rply-ulang-0.8.3/rply_ulang.egg-info/SOURCES.txt
+-rw-r--r--   0 xuanwu     (501) staff       (20)        1 2023-07-30 14:16:43.000000 rply-ulang-0.8.3/rply_ulang.egg-info/dependency_links.txt
+-rw-r--r--   0 xuanwu     (501) staff       (20)        8 2023-07-30 14:16:43.000000 rply-ulang-0.8.3/rply_ulang.egg-info/requires.txt
+-rw-r--r--   0 xuanwu     (501) staff       (20)        5 2023-07-30 14:16:43.000000 rply-ulang-0.8.3/rply_ulang.egg-info/top_level.txt
+-rw-r--r--   0 xuanwu     (501) staff       (20)      104 2023-07-30 14:16:43.799847 rply-ulang-0.8.3/setup.cfg
+-rw-r--r--   0 xuanwu     (501) staff       (20)      528 2023-07-30 14:16:17.000000 rply-ulang-0.8.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rply-ulang-0.8.0/LICENSE` & `rply-ulang-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rply-ulang-0.8.0/PKG-INFO` & `rply-ulang-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: rply-ulang
-Version: 0.8.0
+Version: 0.8.3
 Summary: RPly 木兰编程语言定制版
 Home-page: UNKNOWN
 Author: Xuan Wu
 Author-email: mulanrevive@gmail.com
 License: BSD 3-Clause License
 Project-URL: Source, https://github.com/nobodxbodon/rply
 Description: RPLY 木兰定制版
```

### Comparing `rply-ulang-0.8.0/README.rst` & `rply-ulang-0.8.3/README.rst`

 * *Files identical despite different names*

### Comparing `rply-ulang-0.8.0/rply/__init__.py` & `rply-ulang-0.8.3/rply/__init__.py`

 * *Files identical despite different names*

### Comparing `rply-ulang-0.8.0/rply/分词器.py` & `rply-ulang-0.8.3/rply/分词器.py`

 * *Files identical despite different names*

### Comparing `rply-ulang-0.8.0/rply/分词器母机.py` & `rply-ulang-0.8.3/rply/分词器母机.py`

 * *Files identical despite different names*

### Comparing `rply-ulang-0.8.0/rply/功用.py` & `rply-ulang-0.8.3/rply/功用.py`

 * *Files identical despite different names*

### Comparing `rply-ulang-0.8.0/rply/报错.py` & `rply-ulang-0.8.3/rply/报错.py`

 * *Files identical despite different names*

### Comparing `rply-ulang-0.8.0/rply/词.py` & `rply-ulang-0.8.3/rply/词.py`

 * *Files identical despite different names*

### Comparing `rply-ulang-0.8.0/rply/语法.py` & `rply-ulang-0.8.3/rply/语法.py`

 * *Files identical despite different names*

### Comparing `rply-ulang-0.8.0/rply/语法分析器.py` & `rply-ulang-0.8.3/rply/语法分析器.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
                     当前状态 = 自身._reduce_production(
                         t, 符号栈, 状态栈, state
                     )
                     continue
                 else:
                     #调试输出('为0')
                     n = 符号栈[-1]
-                    print(f"回退次数：{分词器.回退次数}")
+                    调试输出(f"分词器回退次数：{分词器.回退次数}")
                     return n
             else:
                 调试输出('不在状态')
                 # TODO: actual error handling here
                 if 自身.error_handler is not None:
                     调试输出("错误处理")
                     if state is None:
```

### Comparing `rply-ulang-0.8.0/rply/语法分析器母机.py` & `rply-ulang-0.8.3/rply/语法分析器母机.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,16 @@
             表 = LRTable.from语法(语法细节)
 
             if 自身.cache_id is not None:
                 自身._write_cache(cache_dir, cache_file, 表)
 
         if 表.取合不定:
             歧义 = 表.取合不定
-            细节 = '\n\n'.join(['词' + str(i[1]) + '有歧义，默认进行 ' + i[2] + '\n歧义序列：\n' + 输出序列(i[3]) for i in 歧义])
+            # 仅 shift2 有细节
+            细节 = '\n\n'.join(['词' + str(i[1]) + '有歧义，默认进行 ' + i[2] + ('\n歧义序列：\n' + 输出序列(i[3]) if len(i) == 4 else "") for i in 歧义])
             warnings.warn(
                 "如下 %d 种情形取下个词还是合而为一？\n%s" % (
                     len(歧义),
                     细节,
                 ),
                 ParserGeneratorWarning,
                 stacklevel=2,
```

### Comparing `rply-ulang-0.8.0/rply_ulang.egg-info/PKG-INFO` & `rply-ulang-0.8.3/rply_ulang.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: rply-ulang
-Version: 0.8.0
+Version: 0.8.3
 Summary: RPly 木兰编程语言定制版
 Home-page: UNKNOWN
 Author: Xuan Wu
 Author-email: mulanrevive@gmail.com
 License: BSD 3-Clause License
 Project-URL: Source, https://github.com/nobodxbodon/rply
 Description: RPLY 木兰定制版
```

### Comparing `rply-ulang-0.8.0/setup.py` & `rply-ulang-0.8.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,13 +9,13 @@
     name="rply-ulang",
     description="RPly 木兰编程语言定制版",
     long_description=readme,
     # duplicated in docs/conf.py and rply/__init__.py
     project_urls={
         "Source": "https://github.com/nobodxbodon/rply",
     },
-    version="0.8.0",
+    version="0.8.3",
     author="Xuan Wu",
     author_email="mulanrevive@gmail.com",
     packages=["rply"],
     install_requires=["appdirs"],
 )
```

