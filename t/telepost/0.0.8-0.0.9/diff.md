# Comparing `tmp/telepost-0.0.8.tar.gz` & `tmp/telepost-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/telepost-0.0.8.tar", last modified: Wed Apr 14 00:43:03 2021, max compression
+gzip compressed data, was "dist/telepost-0.0.9.tar", last modified: Wed Apr 14 01:01:29 2021, max compression
```

## Comparing `telepost-0.0.8.tar` & `telepost-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2021-04-14 00:43:02.998486 telepost-0.0.8/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     1676 2021-04-14 00:43:02.998153 telepost-0.0.8/PKG-INFO
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      887 2021-03-09 15:32:55.000000 telepost-0.0.8/README.md
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       38 2021-04-14 00:43:02.998645 telepost-0.0.8/setup.cfg
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      818 2021-04-14 00:42:58.000000 telepost-0.0.8/setup.py
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2021-04-14 00:43:02.995512 telepost-0.0.8/telepost/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     3365 2021-04-14 00:42:55.000000 telepost-0.0.8/telepost/__init__.py
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2021-04-14 00:43:02.997533 telepost-0.0.8/telepost.egg-info/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     1676 2021-04-14 00:43:02.000000 telepost-0.0.8/telepost.egg-info/PKG-INFO
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      198 2021-04-14 00:43:02.000000 telepost-0.0.8/telepost.egg-info/SOURCES.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)        1 2021-04-14 00:43:02.000000 telepost-0.0.8/telepost.egg-info/dependency_links.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       38 2021-04-14 00:43:02.000000 telepost-0.0.8/telepost.egg-info/requires.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)        9 2021-04-14 00:43:02.000000 telepost-0.0.8/telepost.egg-info/top_level.txt
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2021-04-14 01:01:29.962438 telepost-0.0.9/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     1676 2021-04-14 01:01:29.962056 telepost-0.0.9/PKG-INFO
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      887 2021-03-09 15:32:55.000000 telepost-0.0.9/README.md
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       38 2021-04-14 01:01:29.962538 telepost-0.0.9/setup.cfg
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      818 2021-04-14 01:01:27.000000 telepost-0.0.9/setup.py
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2021-04-14 01:01:29.959262 telepost-0.0.9/telepost/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     3402 2021-04-14 01:01:24.000000 telepost-0.0.9/telepost/__init__.py
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2021-04-14 01:01:29.961517 telepost-0.0.9/telepost.egg-info/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     1676 2021-04-14 01:01:29.000000 telepost-0.0.9/telepost.egg-info/PKG-INFO
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      198 2021-04-14 01:01:29.000000 telepost-0.0.9/telepost.egg-info/SOURCES.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)        1 2021-04-14 01:01:29.000000 telepost-0.0.9/telepost.egg-info/dependency_links.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       38 2021-04-14 01:01:29.000000 telepost-0.0.9/telepost.egg-info/requires.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)        9 2021-04-14 01:01:29.000000 telepost-0.0.9/telepost.egg-info/top_level.txt
```

### Comparing `telepost-0.0.8/PKG-INFO` & `telepost-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telepost
-Version: 0.0.8
+Version: 0.0.9
 Summary: Get post from telegram and make ready to repost it to other places (twitter / douban / reddit).
 Home-page: https://github.com/gaoyunzhi/telepost
 Author: Yunzhi Gao
 Author-email: gaoyunzhi@gmail.com
 License: UNKNOWN
 Description: # telepost
```

### Comparing `telepost-0.0.8/README.md` & `telepost-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `telepost-0.0.8/setup.py` & `telepost-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="telepost",
-    version="0.0.8",
+    version="0.0.9",
     author="Yunzhi Gao",
     author_email="gaoyunzhi@gmail.com",
     description="Get post from telegram and make ready to repost it to other places (twitter / douban / reddit).",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gaoyunzhi/telepost",
     packages=setuptools.find_packages(),
```

### Comparing `telepost-0.0.8/telepost/__init__.py` & `telepost-0.0.9/telepost/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -85,14 +85,16 @@
     if not post:
         return ''
     return post.text
 
 async def exitTelethon():
     if 'client' in client_cache:
         await client_cache['client'].disconnect()
+        return True
+    return False
 
 def getText(soup):
     soup = copy.copy(soup)
     for item in soup.find_all('a'):
         if item.get('href') and not isUrl(item.text):
             item.replace_with('\n\n' + item.get('href') + '\n\n')
     for item in soup.find_all('br'):
```

### Comparing `telepost-0.0.8/telepost.egg-info/PKG-INFO` & `telepost-0.0.9/telepost.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telepost
-Version: 0.0.8
+Version: 0.0.9
 Summary: Get post from telegram and make ready to repost it to other places (twitter / douban / reddit).
 Home-page: https://github.com/gaoyunzhi/telepost
 Author: Yunzhi Gao
 Author-email: gaoyunzhi@gmail.com
 License: UNKNOWN
 Description: # telepost
```

