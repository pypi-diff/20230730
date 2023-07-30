# Comparing `tmp/tweety-ns-0.9.5.tar.gz` & `tmp/tweety-ns-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweety-ns-0.9.5.tar", last modified: Sat Jul 29 16:09:33 2023, max compression
+gzip compressed data, was "tweety-ns-0.9.6.tar", last modified: Sun Jul 30 02:00:56 2023, max compression
```

## Comparing `tweety-ns-0.9.5.tar` & `tweety-ns-0.9.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 16:09:33.962332 tweety-ns-0.9.5/
--rw-rw-rw-   0        0        0     1799 2023-07-29 16:09:33.962332 tweety-ns-0.9.5/PKG-INFO
--rw-rw-rw-   0        0        0     1088 2023-07-29 16:03:36.000000 tweety-ns-0.9.5/README.md
--rw-rw-rw-   0        0        0      108 2021-11-15 09:32:36.000000 tweety-ns-0.9.5/pyproject.toml
--rw-rw-rw-   0        0        0      701 2023-07-29 16:09:33.963234 tweety-ns-0.9.5/setup.cfg
--rw-rw-rw-   0        0        0      785 2023-07-29 16:02:59.000000 tweety-ns-0.9.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 16:09:33.924231 tweety-ns-0.9.5/src/
-drwxrwxrwx   0        0        0        0 2023-07-29 16:09:33.942231 tweety-ns-0.9.5/src/tweety/
--rw-rw-rw-   0        0        0      276 2023-07-29 16:03:51.000000 tweety-ns-0.9.5/src/tweety/__init__.py
--rw-rw-rw-   0        0        0     3251 2023-07-27 17:28:49.000000 tweety-ns-0.9.5/src/tweety/auth.py
--rw-rw-rw-   0        0        0     8655 2023-07-28 18:14:21.000000 tweety-ns-0.9.5/src/tweety/bot.py
--rw-rw-rw-   0        0        0    38979 2023-07-28 18:07:04.000000 tweety-ns-0.9.5/src/tweety/builder.py
-drwxrwxrwx   0        0        0        0 2023-07-29 16:09:33.944257 tweety-ns-0.9.5/src/tweety/events/
--rw-rw-rw-   0        0        0       42 2023-07-04 06:05:54.000000 tweety-ns-0.9.5/src/tweety/events/__init__.py
--rw-rw-rw-   0        0        0     1768 2023-07-04 10:00:32.000000 tweety-ns-0.9.5/src/tweety/events/newmessage.py
--rw-rw-rw-   0        0        0    19256 2023-07-29 08:49:51.000000 tweety-ns-0.9.5/src/tweety/exceptions_.py
--rw-rw-rw-   0        0        0      635 2023-07-27 17:30:57.000000 tweety-ns-0.9.5/src/tweety/filters.py
--rw-rw-rw-   0        0        0     7986 2023-07-29 14:39:05.000000 tweety-ns-0.9.5/src/tweety/http.py
--rw-rw-rw-   0        0        0     1510 2023-07-26 20:41:00.000000 tweety-ns-0.9.5/src/tweety/session.py
-drwxrwxrwx   0        0        0        0 2023-07-29 16:09:33.956253 tweety-ns-0.9.5/src/tweety/types/
--rw-rw-rw-   0        0        0      331 2023-07-27 10:28:18.000000 tweety-ns-0.9.5/src/tweety/types/__init__.py
--rw-rw-rw-   0        0        0      951 2023-07-29 12:04:19.000000 tweety-ns-0.9.5/src/tweety/types/base.py
--rw-rw-rw-   0        0        0     2741 2023-07-29 12:16:19.000000 tweety-ns-0.9.5/src/tweety/types/bookmarks.py
--rw-rw-rw-   0        0        0     9347 2023-07-29 12:16:19.000000 tweety-ns-0.9.5/src/tweety/types/inbox.py
--rw-rw-rw-   0        0        0     1823 2023-07-29 14:23:48.000000 tweety-ns-0.9.5/src/tweety/types/mentions.py
--rw-rw-rw-   0        0        0     6573 2023-07-28 18:32:05.000000 tweety-ns-0.9.5/src/tweety/types/n_types.py
--rw-rw-rw-   0        0        0     3982 2023-07-29 14:23:48.000000 tweety-ns-0.9.5/src/tweety/types/search.py
--rw-rw-rw-   0        0        0    29877 2023-07-29 14:44:19.000000 tweety-ns-0.9.5/src/tweety/types/twDataTypes.py
--rw-rw-rw-   0        0        0     3172 2023-07-29 14:23:48.000000 tweety-ns-0.9.5/src/tweety/types/usertweet.py
--rw-rw-rw-   0        0        0      483 2023-07-09 19:15:04.000000 tweety-ns-0.9.5/src/tweety/updates.py
--rw-rw-rw-   0        0        0     6463 2023-07-29 11:00:08.000000 tweety-ns-0.9.5/src/tweety/user.py
--rw-rw-rw-   0        0        0     3102 2023-07-28 18:30:16.000000 tweety-ns-0.9.5/src/tweety/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-29 16:09:33.961230 tweety-ns-0.9.5/src/tweety_ns.egg-info/
--rw-rw-rw-   0        0        0     1799 2023-07-29 16:09:33.000000 tweety-ns-0.9.5/src/tweety_ns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      777 2023-07-29 16:09:33.000000 tweety-ns-0.9.5/src/tweety_ns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 16:09:33.000000 tweety-ns-0.9.5/src/tweety_ns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-29 16:09:33.000000 tweety-ns-0.9.5/src/tweety_ns.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-29 16:09:33.000000 tweety-ns-0.9.5/src/tweety_ns.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 02:00:56.565903 tweety-ns-0.9.6/
+-rw-rw-rw-   0        0        0     1799 2023-07-30 02:00:56.565903 tweety-ns-0.9.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1088 2023-07-29 16:03:36.000000 tweety-ns-0.9.6/README.md
+-rw-rw-rw-   0        0        0      108 2021-11-15 09:32:36.000000 tweety-ns-0.9.6/pyproject.toml
+-rw-rw-rw-   0        0        0      701 2023-07-30 02:00:56.566904 tweety-ns-0.9.6/setup.cfg
+-rw-rw-rw-   0        0        0      785 2023-07-30 01:59:13.000000 tweety-ns-0.9.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 02:00:56.532816 tweety-ns-0.9.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-30 02:00:56.547886 tweety-ns-0.9.6/src/tweety/
+-rw-rw-rw-   0        0        0      276 2023-07-29 16:03:51.000000 tweety-ns-0.9.6/src/tweety/__init__.py
+-rw-rw-rw-   0        0        0     3251 2023-07-27 17:28:49.000000 tweety-ns-0.9.6/src/tweety/auth.py
+-rw-rw-rw-   0        0        0     8655 2023-07-28 18:14:21.000000 tweety-ns-0.9.6/src/tweety/bot.py
+-rw-rw-rw-   0        0        0    38991 2023-07-30 01:58:18.000000 tweety-ns-0.9.6/src/tweety/builder.py
+drwxrwxrwx   0        0        0        0 2023-07-30 02:00:56.548903 tweety-ns-0.9.6/src/tweety/events/
+-rw-rw-rw-   0        0        0       42 2023-07-04 06:05:54.000000 tweety-ns-0.9.6/src/tweety/events/__init__.py
+-rw-rw-rw-   0        0        0     1768 2023-07-04 10:00:32.000000 tweety-ns-0.9.6/src/tweety/events/newmessage.py
+-rw-rw-rw-   0        0        0    19256 2023-07-29 08:49:51.000000 tweety-ns-0.9.6/src/tweety/exceptions_.py
+-rw-rw-rw-   0        0        0      635 2023-07-27 17:30:57.000000 tweety-ns-0.9.6/src/tweety/filters.py
+-rw-rw-rw-   0        0        0     7986 2023-07-29 14:39:05.000000 tweety-ns-0.9.6/src/tweety/http.py
+-rw-rw-rw-   0        0        0     1510 2023-07-26 20:41:00.000000 tweety-ns-0.9.6/src/tweety/session.py
+drwxrwxrwx   0        0        0        0 2023-07-30 02:00:56.557901 tweety-ns-0.9.6/src/tweety/types/
+-rw-rw-rw-   0        0        0      331 2023-07-27 10:28:18.000000 tweety-ns-0.9.6/src/tweety/types/__init__.py
+-rw-rw-rw-   0        0        0      951 2023-07-29 12:04:19.000000 tweety-ns-0.9.6/src/tweety/types/base.py
+-rw-rw-rw-   0        0        0     2741 2023-07-29 12:16:19.000000 tweety-ns-0.9.6/src/tweety/types/bookmarks.py
+-rw-rw-rw-   0        0        0     9347 2023-07-29 12:16:19.000000 tweety-ns-0.9.6/src/tweety/types/inbox.py
+-rw-rw-rw-   0        0        0     1823 2023-07-29 14:23:48.000000 tweety-ns-0.9.6/src/tweety/types/mentions.py
+-rw-rw-rw-   0        0        0     6573 2023-07-28 18:32:05.000000 tweety-ns-0.9.6/src/tweety/types/n_types.py
+-rw-rw-rw-   0        0        0     3982 2023-07-29 14:23:48.000000 tweety-ns-0.9.6/src/tweety/types/search.py
+-rw-rw-rw-   0        0        0    29877 2023-07-29 14:44:19.000000 tweety-ns-0.9.6/src/tweety/types/twDataTypes.py
+-rw-rw-rw-   0        0        0     3172 2023-07-29 14:23:48.000000 tweety-ns-0.9.6/src/tweety/types/usertweet.py
+-rw-rw-rw-   0        0        0      483 2023-07-09 19:15:04.000000 tweety-ns-0.9.6/src/tweety/updates.py
+-rw-rw-rw-   0        0        0     6463 2023-07-29 11:00:08.000000 tweety-ns-0.9.6/src/tweety/user.py
+-rw-rw-rw-   0        0        0     3102 2023-07-28 18:30:16.000000 tweety-ns-0.9.6/src/tweety/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-30 02:00:56.564901 tweety-ns-0.9.6/src/tweety_ns.egg-info/
+-rw-rw-rw-   0        0        0     1799 2023-07-30 02:00:56.000000 tweety-ns-0.9.6/src/tweety_ns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      777 2023-07-30 02:00:56.000000 tweety-ns-0.9.6/src/tweety_ns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 02:00:56.000000 tweety-ns-0.9.6/src/tweety_ns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-30 02:00:56.000000 tweety-ns-0.9.6/src/tweety_ns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-30 02:00:56.000000 tweety-ns-0.9.6/src/tweety_ns.egg-info/top_level.txt
```

### Comparing `tweety-ns-0.9.5/PKG-INFO` & `tweety-ns-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweety-ns
-Version: 0.9.5
+Version: 0.9.6
 Summary: An easy Twitter Scraper
 Home-page: https://github.com/mahrtayyab/tweety
 Author: Tayyab Kharl
 Author-email: tayyabmahr@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mahrtayyab/tweety/issues
 Project-URL: Documentation, https://github.com/mahrtayyab/tweety
```

### Comparing `tweety-ns-0.9.5/README.md` & `tweety-ns-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `tweety-ns-0.9.5/setup.cfg` & `tweety-ns-0.9.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 7765 6574 792d 6e73 0d0a 7665   = tweety-ns..ve
-00000020: 7273 696f 6e20 3d20 302e 392e 350d 0a61  rsion = 0.9.5..a
+00000020: 7273 696f 6e20 3d20 302e 392e 360d 0a61  rsion = 0.9.6..a
 00000030: 7574 686f 7220 3d20 5461 7979 6162 204b  uthor = Tayyab K
 00000040: 6861 726c 0d0a 6175 7468 6f72 5f65 6d61  harl..author_ema
 00000050: 696c 203d 2074 6179 7961 626d 6168 7240  il = tayyabmahr@
 00000060: 676d 6169 6c2e 636f 6d0d 0a64 6573 6372  gmail.com..descr
 00000070: 6970 7469 6f6e 203d 2041 6e20 6561 7379  iption = An easy
 00000080: 2054 7769 7474 6572 2053 6372 6170 6572   Twitter Scraper
 00000090: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
```

### Comparing `tweety-ns-0.9.5/setup.py` & `tweety-ns-0.9.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name='tweety-ns',
     packages=['tweety', 'tweety.types', 'tweety.events'],
-    version='0.9.5',
+    version='0.9.6',
     license='MIT',
     description='An easy Twitter Scraper',
     author='Tayyab Kharl',
     author_email='tayyabmahr@gmail.com',
     url='https://github.com/mahrtayyab/tweety',
     keywords=['TWITTER', 'TWITTER SCRAPE', 'SCRAPE TWEETS'],
     install_requires=[
```

### Comparing `tweety-ns-0.9.5/src/tweety/auth.py` & `tweety-ns-0.9.6/src/tweety/auth.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-0.9.5/src/tweety/bot.py` & `tweety-ns-0.9.6/src/tweety/bot.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-0.9.5/src/tweety/builder.py` & `tweety-ns-0.9.6/src/tweety/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -813,15 +813,15 @@
                         "link": "next_link"
                     }
                 }
             ]
         }
 
     def LoginAcid(self, json_, username, password):
-        reason = json_['subtasks'][0]['enter_text']['secondary_text']['text']
+        reason = json_['subtasks'][0]['enter_text']['header']['secondary_text']['text']
         print(reason)
         getAlternate = input("> ")
         return {
             "flow_token": self.get_flow_token(json_),
             "subtask_inputs": [
                 {
                     "subtask_id": "LoginAcid",
@@ -830,15 +830,15 @@
                         "link": "next_link"
                     }
                 }
             ]
         }
 
     def LoginTwoFactorAuthChallenge(self, json_, username, password):
-        reason = json_['subtasks'][0]['enter_text']['header']['primary_text']['text']
+        reason = json_['subtasks'][0]['enter_text']['header']['secondary_text']['text']
         print(reason)
         getAlternate = input("> ")
         return {
             "flow_token": self.get_flow_token(json_),
             "subtask_inputs": [
                 {
                     "subtask_id": "LoginTwoFactorAuthChallenge",
```

### Comparing `tweety-ns-0.9.5/src/tweety/events/newmessage.py` & `tweety-ns-0.9.6/src/tweety/events/newmessage.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-0.9.5/src/tweety/exceptions_.py` & `tweety-ns-0.9.6/src/tweety/exceptions_.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-0.9.5/src/tweety/filters.py` & `tweety-ns-0.9.6/src/tweety/filters.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-0.9.5/src/tweety/http.py` & `tweety-ns-0.9.6/src/tweety/http.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-0.9.5/src/tweety/session.py` & `tweety-ns-0.9.6/src/tweety/session.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-0.9.5/src/tweety/types/base.py` & `tweety-ns-0.9.6/src/tweety/types/base.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-0.9.5/src/tweety/types/bookmarks.py` & `tweety-ns-0.9.6/src/tweety/types/bookmarks.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-0.9.5/src/tweety/types/inbox.py` & `tweety-ns-0.9.6/src/tweety/types/inbox.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-0.9.5/src/tweety/types/mentions.py` & `tweety-ns-0.9.6/src/tweety/types/mentions.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-0.9.5/src/tweety/types/n_types.py` & `tweety-ns-0.9.6/src/tweety/types/n_types.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-0.9.5/src/tweety/types/search.py` & `tweety-ns-0.9.6/src/tweety/types/search.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-0.9.5/src/tweety/types/twDataTypes.py` & `tweety-ns-0.9.6/src/tweety/types/twDataTypes.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-0.9.5/src/tweety/types/usertweet.py` & `tweety-ns-0.9.6/src/tweety/types/usertweet.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-0.9.5/src/tweety/user.py` & `tweety-ns-0.9.6/src/tweety/user.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-0.9.5/src/tweety/utils.py` & `tweety-ns-0.9.6/src/tweety/utils.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-0.9.5/src/tweety_ns.egg-info/PKG-INFO` & `tweety-ns-0.9.6/src/tweety_ns.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweety-ns
-Version: 0.9.5
+Version: 0.9.6
 Summary: An easy Twitter Scraper
 Home-page: https://github.com/mahrtayyab/tweety
 Author: Tayyab Kharl
 Author-email: tayyabmahr@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mahrtayyab/tweety/issues
 Project-URL: Documentation, https://github.com/mahrtayyab/tweety
```

### Comparing `tweety-ns-0.9.5/src/tweety_ns.egg-info/SOURCES.txt` & `tweety-ns-0.9.6/src/tweety_ns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

