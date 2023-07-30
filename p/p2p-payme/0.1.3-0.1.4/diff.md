# Comparing `tmp/p2p-payme-0.1.3.tar.gz` & `tmp/p2p-payme-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p2p-payme-0.1.3.tar", last modified: Sat Jul 29 17:41:07 2023, max compression
+gzip compressed data, was "p2p-payme-0.1.4.tar", last modified: Sun Jul 30 10:13:30 2023, max compression
```

## Comparing `p2p-payme-0.1.3.tar` & `p2p-payme-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-29 17:41:07.714169 p2p-payme-0.1.3/
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     5345 2023-07-29 17:41:07.714169 p2p-payme-0.1.3/PKG-INFO
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     5026 2023-07-29 16:07:27.000000 p2p-payme-0.1.3/README.md
-drwxrwxr-x   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-29 17:41:07.710169 p2p-payme-0.1.3/p2p_payme/
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-29 14:17:48.000000 p2p-payme-0.1.3/p2p_payme/__init__.py
-drwxrwxr-x   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-29 17:41:07.710169 p2p-payme-0.1.3/p2p_payme/api/
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-26 18:16:05.000000 p2p-payme-0.1.3/p2p_payme/api/__init__.py
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     2682 2023-07-29 16:47:54.000000 p2p-payme-0.1.3/p2p_payme/api/base.py
-drwxrwxr-x   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-29 17:41:07.714169 p2p-payme-0.1.3/p2p_payme/auth/
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-29 14:55:35.000000 p2p-payme-0.1.3/p2p_payme/auth/__init__.py
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     2916 2023-07-29 16:46:41.000000 p2p-payme-0.1.3/p2p_payme/auth/api.py
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)      244 2023-07-29 13:25:34.000000 p2p-payme-0.1.3/p2p_payme/auth/scheme.py
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)      876 2023-07-29 16:00:45.000000 p2p-payme-0.1.3/p2p_payme/cli.py
-drwxrwxr-x   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-29 17:41:07.714169 p2p-payme-0.1.3/p2p_payme/client/
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)       35 2023-07-27 08:47:24.000000 p2p-payme-0.1.3/p2p_payme/client/__init__.py
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     2544 2023-07-29 12:35:31.000000 p2p-payme-0.1.3/p2p_payme/client/manager.py
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     3048 2023-07-29 17:32:06.000000 p2p-payme-0.1.3/p2p_payme/client/operations.py
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     1496 2023-07-29 13:24:23.000000 p2p-payme-0.1.3/p2p_payme/client/scheme.py
-drwxrwxr-x   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-29 17:41:07.714169 p2p-payme-0.1.3/p2p_payme/config/
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-26 18:16:05.000000 p2p-payme-0.1.3/p2p_payme/config/__init__.py
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)      114 2023-07-28 10:09:34.000000 p2p-payme-0.1.3/p2p_payme/config/constants.py
-drwxrwxr-x   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-29 17:41:07.710169 p2p-payme-0.1.3/p2p_payme.egg-info/
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     5345 2023-07-29 17:41:07.000000 p2p-payme-0.1.3/p2p_payme.egg-info/PKG-INFO
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)      553 2023-07-29 17:41:07.000000 p2p-payme-0.1.3/p2p_payme.egg-info/SOURCES.txt
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)        1 2023-07-29 17:41:07.000000 p2p-payme-0.1.3/p2p_payme.egg-info/dependency_links.txt
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)       45 2023-07-29 17:41:07.000000 p2p-payme-0.1.3/p2p_payme.egg-info/entry_points.txt
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)      256 2023-07-29 17:41:07.000000 p2p-payme-0.1.3/p2p_payme.egg-info/requires.txt
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)       10 2023-07-29 17:41:07.000000 p2p-payme-0.1.3/p2p_payme.egg-info/top_level.txt
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)       38 2023-07-29 17:41:07.714169 p2p-payme-0.1.3/setup.cfg
--rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     1122 2023-07-29 17:40:31.000000 p2p-payme-0.1.3/setup.py
+drwxrwxr-x   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-30 10:13:30.773873 p2p-payme-0.1.4/
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     5345 2023-07-30 10:13:30.773873 p2p-payme-0.1.4/PKG-INFO
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     5026 2023-07-29 16:07:27.000000 p2p-payme-0.1.4/README.md
+drwxrwxr-x   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-30 10:13:30.769873 p2p-payme-0.1.4/p2p_payme/
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-29 14:17:48.000000 p2p-payme-0.1.4/p2p_payme/__init__.py
+drwxrwxr-x   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-30 10:13:30.769873 p2p-payme-0.1.4/p2p_payme/api/
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-26 18:16:05.000000 p2p-payme-0.1.4/p2p_payme/api/__init__.py
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     2682 2023-07-29 16:47:54.000000 p2p-payme-0.1.4/p2p_payme/api/base.py
+drwxrwxr-x   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-30 10:13:30.769873 p2p-payme-0.1.4/p2p_payme/auth/
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-29 14:55:35.000000 p2p-payme-0.1.4/p2p_payme/auth/__init__.py
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     2916 2023-07-29 16:46:41.000000 p2p-payme-0.1.4/p2p_payme/auth/api.py
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)      244 2023-07-29 13:25:34.000000 p2p-payme-0.1.4/p2p_payme/auth/scheme.py
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)      876 2023-07-29 16:00:45.000000 p2p-payme-0.1.4/p2p_payme/cli.py
+drwxrwxr-x   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-30 10:13:30.769873 p2p-payme-0.1.4/p2p_payme/client/
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)       35 2023-07-27 08:47:24.000000 p2p-payme-0.1.4/p2p_payme/client/__init__.py
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     2544 2023-07-29 12:35:31.000000 p2p-payme-0.1.4/p2p_payme/client/manager.py
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     3048 2023-07-29 17:32:06.000000 p2p-payme-0.1.4/p2p_payme/client/operations.py
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     1496 2023-07-29 13:24:23.000000 p2p-payme-0.1.4/p2p_payme/client/scheme.py
+drwxrwxr-x   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-30 10:13:30.773873 p2p-payme-0.1.4/p2p_payme/config/
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-26 18:16:05.000000 p2p-payme-0.1.4/p2p_payme/config/__init__.py
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)      114 2023-07-28 10:09:34.000000 p2p-payme-0.1.4/p2p_payme/config/constants.py
+drwxrwxr-x   0 abdulvoris  (1000) abdulvoris  (1000)        0 2023-07-30 10:13:30.769873 p2p-payme-0.1.4/p2p_payme.egg-info/
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)     5345 2023-07-30 10:13:30.000000 p2p-payme-0.1.4/p2p_payme.egg-info/PKG-INFO
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)      553 2023-07-30 10:13:30.000000 p2p-payme-0.1.4/p2p_payme.egg-info/SOURCES.txt
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)        1 2023-07-30 10:13:30.000000 p2p-payme-0.1.4/p2p_payme.egg-info/dependency_links.txt
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)       45 2023-07-30 10:13:30.000000 p2p-payme-0.1.4/p2p_payme.egg-info/entry_points.txt
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)      152 2023-07-30 10:13:30.000000 p2p-payme-0.1.4/p2p_payme.egg-info/requires.txt
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)       10 2023-07-30 10:13:30.000000 p2p-payme-0.1.4/p2p_payme.egg-info/top_level.txt
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)       38 2023-07-30 10:13:30.773873 p2p-payme-0.1.4/setup.cfg
+-rw-rw-r--   0 abdulvoris  (1000) abdulvoris  (1000)      952 2023-07-30 10:13:03.000000 p2p-payme-0.1.4/setup.py
```

### Comparing `p2p-payme-0.1.3/PKG-INFO` & `p2p-payme-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p2p-payme
-Version: 0.1.3
+Version: 0.1.4
 Summary: P2P automation
 Home-page: https://github.com/Abdulvoris101/p2p-payme
 Author: Abdulvoris Erkinov
 Author-email: erkinovabdulvoris101@gmail.com
 License: UNKNOWN
 Keywords: python payme p2p automation
 Platform: UNKNOWN
```

### Comparing `p2p-payme-0.1.3/README.md` & `p2p-payme-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `p2p-payme-0.1.3/p2p_payme/api/base.py` & `p2p-payme-0.1.4/p2p_payme/api/base.py`

 * *Files identical despite different names*

### Comparing `p2p-payme-0.1.3/p2p_payme/auth/api.py` & `p2p-payme-0.1.4/p2p_payme/auth/api.py`

 * *Files identical despite different names*

### Comparing `p2p-payme-0.1.3/p2p_payme/cli.py` & `p2p-payme-0.1.4/p2p_payme/cli.py`

 * *Files identical despite different names*

### Comparing `p2p-payme-0.1.3/p2p_payme/client/manager.py` & `p2p-payme-0.1.4/p2p_payme/client/manager.py`

 * *Files identical despite different names*

### Comparing `p2p-payme-0.1.3/p2p_payme/client/operations.py` & `p2p-payme-0.1.4/p2p_payme/client/operations.py`

 * *Files identical despite different names*

### Comparing `p2p-payme-0.1.3/p2p_payme/client/scheme.py` & `p2p-payme-0.1.4/p2p_payme/client/scheme.py`

 * *Files identical despite different names*

### Comparing `p2p-payme-0.1.3/p2p_payme.egg-info/PKG-INFO` & `p2p-payme-0.1.4/p2p_payme.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p2p-payme
-Version: 0.1.3
+Version: 0.1.4
 Summary: P2P automation
 Home-page: https://github.com/Abdulvoris101/p2p-payme
 Author: Abdulvoris Erkinov
 Author-email: erkinovabdulvoris101@gmail.com
 License: UNKNOWN
 Keywords: python payme p2p automation
 Platform: UNKNOWN
```

### Comparing `p2p-payme-0.1.3/p2p_payme.egg-info/SOURCES.txt` & `p2p-payme-0.1.4/p2p_payme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `p2p-payme-0.1.3/setup.py` & `p2p-payme-0.1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,28 +2,22 @@
 
 def get_long_description():
     with open('README.md', mode='r', encoding='utf8') as f:
         return f.read()
 
 setup(
     name='p2p-payme',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     install_requires=[
-        'annotated-types==0.5.0',
-        'certifi==2023.7.22',
-        'charset-normalizer==3.2.0',
-        'idna==3.4',
-        'pydantic==2.1.1',
+        'pydantic>=1.7.4,<2.0.0',
         'pydantic-collections==0.5.0',
-        'pydantic_core==2.4.0',
         'python-dateutil==2.8.2',
         'python-dotenv==1.0.0',
         'requests==2.31.0',
-        'six==1.16.0',
         'typing_extensions==4.7.1',
         'urllib3==2.0.4'
     ],
     # Additional metadata (optional)
     author='Abdulvoris Erkinov',
     author_email='erkinovabdulvoris101@gmail.com',
     description='P2P automation',
```

