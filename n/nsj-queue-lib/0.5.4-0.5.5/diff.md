# Comparing `tmp/nsj_queue_lib-0.5.4.tar.gz` & `tmp/nsj_queue_lib-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_queue_lib-0.5.4.tar", last modified: Sat Jul 29 21:25:09 2023, max compression
+gzip compressed data, was "nsj_queue_lib-0.5.5.tar", last modified: Sun Jul 30 00:55:28 2023, max compression
```

## Comparing `nsj_queue_lib-0.5.4.tar` & `nsj_queue_lib-0.5.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-29 21:25:09.881403 nsj_queue_lib-0.5.4/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    37367 2023-07-29 21:25:09.881403 nsj_queue_lib-0.5.4/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    36802 2023-07-26 23:49:53.000000 nsj_queue_lib-0.5.4/README.md
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-29 21:25:09.881403 nsj_queue_lib-0.5.4/nsj_queue_lib/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-19 18:24:10.000000 nsj_queue_lib-0.5.4/nsj_queue_lib/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2954 2023-07-26 23:38:36.000000 nsj_queue_lib-0.5.4/nsj_queue_lib/db_gen.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       98 2023-07-25 22:33:41.000000 nsj_queue_lib-0.5.4/nsj_queue_lib/exception.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1090 2023-07-22 22:37:18.000000 nsj_queue_lib-0.5.4/nsj_queue_lib/lock_dao.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    10845 2023-07-26 20:42:13.000000 nsj_queue_lib-0.5.4/nsj_queue_lib/main_thread.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4814 2023-07-26 20:46:48.000000 nsj_queue_lib-0.5.4/nsj_queue_lib/notify_thread.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3243 2023-07-22 23:57:02.000000 nsj_queue_lib-0.5.4/nsj_queue_lib/purge_thread.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4684 2023-07-29 19:47:12.000000 nsj_queue_lib-0.5.4/nsj_queue_lib/queue_client.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4913 2023-07-22 23:57:41.000000 nsj_queue_lib-0.5.4/nsj_queue_lib/retry_thread.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     5259 2023-07-26 18:39:19.000000 nsj_queue_lib-0.5.4/nsj_queue_lib/retry_util.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2032 2023-07-26 20:47:28.000000 nsj_queue_lib-0.5.4/nsj_queue_lib/settings.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     9746 2023-07-26 20:45:47.000000 nsj_queue_lib-0.5.4/nsj_queue_lib/tarefa_dao.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1756 2023-07-26 17:45:30.000000 nsj_queue_lib-0.5.4/nsj_queue_lib/worker_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      580 2023-07-26 21:58:04.000000 nsj_queue_lib-0.5.4/nsj_queue_lib/worker_fila_teste.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3204 2023-07-26 23:08:43.000000 nsj_queue_lib-0.5.4/nsj_queue_lib/worker_pub_sub_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1392 2023-07-28 17:51:07.000000 nsj_queue_lib-0.5.4/nsj_queue_lib/worker_pub_sub_teste.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2162 2023-07-26 17:51:34.000000 nsj_queue_lib-0.5.4/nsj_queue_lib/worker_webhook.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-29 21:25:09.881403 nsj_queue_lib-0.5.4/nsj_queue_lib.egg-info/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    37367 2023-07-29 21:25:09.000000 nsj_queue_lib-0.5.4/nsj_queue_lib.egg-info/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      768 2023-07-29 21:25:09.000000 nsj_queue_lib-0.5.4/nsj_queue_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-07-29 21:25:09.000000 nsj_queue_lib-0.5.4/nsj_queue_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      110 2023-07-29 21:25:09.000000 nsj_queue_lib-0.5.4/nsj_queue_lib.egg-info/requires.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       14 2023-07-29 21:25:09.000000 nsj_queue_lib-0.5.4/nsj_queue_lib.egg-info/top_level.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-21 22:32:09.000000 nsj_queue_lib-0.5.4/pyproject.toml
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      834 2023-07-29 21:25:09.881403 nsj_queue_lib-0.5.4/setup.cfg
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-30 00:55:28.411855 nsj_queue_lib-0.5.5/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    37367 2023-07-30 00:55:28.411855 nsj_queue_lib-0.5.5/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    36802 2023-07-26 23:49:53.000000 nsj_queue_lib-0.5.5/README.md
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-30 00:55:28.411855 nsj_queue_lib-0.5.5/nsj_queue_lib/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-19 18:24:10.000000 nsj_queue_lib-0.5.5/nsj_queue_lib/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2954 2023-07-26 23:38:36.000000 nsj_queue_lib-0.5.5/nsj_queue_lib/db_gen.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       98 2023-07-25 22:33:41.000000 nsj_queue_lib-0.5.5/nsj_queue_lib/exception.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1090 2023-07-22 22:37:18.000000 nsj_queue_lib-0.5.5/nsj_queue_lib/lock_dao.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    10845 2023-07-26 20:42:13.000000 nsj_queue_lib-0.5.5/nsj_queue_lib/main_thread.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4814 2023-07-26 20:46:48.000000 nsj_queue_lib-0.5.5/nsj_queue_lib/notify_thread.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3243 2023-07-22 23:57:02.000000 nsj_queue_lib-0.5.5/nsj_queue_lib/purge_thread.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4684 2023-07-29 19:47:12.000000 nsj_queue_lib-0.5.5/nsj_queue_lib/queue_client.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4913 2023-07-22 23:57:41.000000 nsj_queue_lib-0.5.5/nsj_queue_lib/retry_thread.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     5259 2023-07-26 18:39:19.000000 nsj_queue_lib-0.5.5/nsj_queue_lib/retry_util.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2588 2023-07-30 00:55:00.000000 nsj_queue_lib-0.5.5/nsj_queue_lib/settings.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     9746 2023-07-26 20:45:47.000000 nsj_queue_lib-0.5.5/nsj_queue_lib/tarefa_dao.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1756 2023-07-26 17:45:30.000000 nsj_queue_lib-0.5.5/nsj_queue_lib/worker_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      580 2023-07-26 21:58:04.000000 nsj_queue_lib-0.5.5/nsj_queue_lib/worker_fila_teste.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3204 2023-07-26 23:08:43.000000 nsj_queue_lib-0.5.5/nsj_queue_lib/worker_pub_sub_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1392 2023-07-28 17:51:07.000000 nsj_queue_lib-0.5.5/nsj_queue_lib/worker_pub_sub_teste.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2162 2023-07-26 17:51:34.000000 nsj_queue_lib-0.5.5/nsj_queue_lib/worker_webhook.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-30 00:55:28.411855 nsj_queue_lib-0.5.5/nsj_queue_lib.egg-info/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    37367 2023-07-30 00:55:28.000000 nsj_queue_lib-0.5.5/nsj_queue_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      768 2023-07-30 00:55:28.000000 nsj_queue_lib-0.5.5/nsj_queue_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-07-30 00:55:28.000000 nsj_queue_lib-0.5.5/nsj_queue_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      110 2023-07-30 00:55:28.000000 nsj_queue_lib-0.5.5/nsj_queue_lib.egg-info/requires.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       14 2023-07-30 00:55:28.000000 nsj_queue_lib-0.5.5/nsj_queue_lib.egg-info/top_level.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-21 22:32:09.000000 nsj_queue_lib-0.5.5/pyproject.toml
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      834 2023-07-30 00:55:28.411855 nsj_queue_lib-0.5.5/setup.cfg
```

### Comparing `nsj_queue_lib-0.5.4/PKG-INFO` & `nsj_queue_lib-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj_queue_lib
-Version: 0.5.4
+Version: 0.5.5
 Summary: Biblioteca para facilitar a implementação de filas e workers.
 Home-page: https://github.com/Nasajon/nsj-queue-lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj-queue-lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_queue_lib-0.5.4/README.md` & `nsj_queue_lib-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.4/nsj_queue_lib/db_gen.py` & `nsj_queue_lib-0.5.5/nsj_queue_lib/db_gen.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.4/nsj_queue_lib/lock_dao.py` & `nsj_queue_lib-0.5.5/nsj_queue_lib/lock_dao.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.4/nsj_queue_lib/main_thread.py` & `nsj_queue_lib-0.5.5/nsj_queue_lib/main_thread.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.4/nsj_queue_lib/notify_thread.py` & `nsj_queue_lib-0.5.5/nsj_queue_lib/notify_thread.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.4/nsj_queue_lib/purge_thread.py` & `nsj_queue_lib-0.5.5/nsj_queue_lib/purge_thread.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.4/nsj_queue_lib/queue_client.py` & `nsj_queue_lib-0.5.5/nsj_queue_lib/queue_client.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.4/nsj_queue_lib/retry_thread.py` & `nsj_queue_lib-0.5.5/nsj_queue_lib/retry_thread.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.4/nsj_queue_lib/retry_util.py` & `nsj_queue_lib-0.5.5/nsj_queue_lib/retry_util.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.4/nsj_queue_lib/settings.py` & `nsj_queue_lib-0.5.5/nsj_queue_lib/settings.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,30 @@
 import logging
 import logging_loki
 import os
 import sys
 import uuid
 
 # Resolvendo as variáveis de ambiente
-DB_HOST = os.environ["DB_HOST"]
-DB_PORT = int(os.environ["DB_PORT"])
-DB_BASE = os.environ["DB_BASE"]
-DB_USER = os.environ["DB_USER"]
-DB_PASS = os.environ["DB_PASS"]
+DB_HOST = os.getenv("DB_HOST") or os.getenv("DATABASE_HOST")
+DB_PORT = int(os.getenv("DB_PORT") or os.getenv("DATABASE_PORT"))
+DB_BASE = os.getenv("DB_BASE") or os.getenv("DATABASE_NAME")
+DB_USER = os.getenv("DB_USER") or os.getenv("DATABASE_USER")
+DB_PASS = os.getenv("DB_PASS") or os.getenv("DATABASE_PASS")
+
+if DB_HOST is None:
+    raise Exception("Faltando variável de ambiente DB_HOST")
+if DB_PORT is None:
+    raise Exception("Faltando variável de ambiente DB_PORT")
+if DB_BASE is None:
+    raise Exception("Faltando variável de ambiente DB_BASE")
+if DB_USER is None:
+    raise Exception("Faltando variável de ambiente DB_USER")
+if DB_PASS is None:
+    raise Exception("Faltando variável de ambiente DB_PASS")
 
 QUEUE_NAME = os.environ["QUEUE_NAME"]
 QUEUE_TABLE = os.environ["QUEUE_TABLE"]
 QUEUE_SUBSCRIBER_TABLE = os.getenv("QUEUE_SUBSCRIBER_TABLE")
 
 QUEUE_MAX_RETRY = int(os.getenv("QUEUE_MAX_RETRY", "100"))
 QUEUE_BASE_INTERVAL_RETRY = int(os.getenv("QUEUE_BASE_INTERVAL_RETRY", "5"))
```

### Comparing `nsj_queue_lib-0.5.4/nsj_queue_lib/tarefa_dao.py` & `nsj_queue_lib-0.5.5/nsj_queue_lib/tarefa_dao.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.4/nsj_queue_lib/worker_base.py` & `nsj_queue_lib-0.5.5/nsj_queue_lib/worker_base.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.4/nsj_queue_lib/worker_fila_teste.py` & `nsj_queue_lib-0.5.5/nsj_queue_lib/worker_fila_teste.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.4/nsj_queue_lib/worker_pub_sub_base.py` & `nsj_queue_lib-0.5.5/nsj_queue_lib/worker_pub_sub_base.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.4/nsj_queue_lib/worker_pub_sub_teste.py` & `nsj_queue_lib-0.5.5/nsj_queue_lib/worker_pub_sub_teste.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.4/nsj_queue_lib/worker_webhook.py` & `nsj_queue_lib-0.5.5/nsj_queue_lib/worker_webhook.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.4/nsj_queue_lib.egg-info/PKG-INFO` & `nsj_queue_lib-0.5.5/nsj_queue_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj-queue-lib
-Version: 0.5.4
+Version: 0.5.5
 Summary: Biblioteca para facilitar a implementação de filas e workers.
 Home-page: https://github.com/Nasajon/nsj-queue-lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj-queue-lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_queue_lib-0.5.4/nsj_queue_lib.egg-info/SOURCES.txt` & `nsj_queue_lib-0.5.5/nsj_queue_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.4/setup.cfg` & `nsj_queue_lib-0.5.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nsj_queue_lib
-version = 0.5.4
+version = 0.5.5
 author = Nasajon Sistemas
 author_email = contact.dev@nasajon.com.br
 description = Biblioteca para facilitar a implementação de filas e workers.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Nasajon/nsj-queue-lib
 project_urls =
```

