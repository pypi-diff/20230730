# Comparing `tmp/nsj_queue_lib-0.5.3.tar.gz` & `tmp/nsj_queue_lib-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_queue_lib-0.5.3.tar", last modified: Sat Jul 29 19:47:20 2023, max compression
+gzip compressed data, was "nsj_queue_lib-0.5.4.tar", last modified: Sat Jul 29 21:25:09 2023, max compression
```

## Comparing `nsj_queue_lib-0.5.3.tar` & `nsj_queue_lib-0.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-29 19:47:20.709307 nsj_queue_lib-0.5.3/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    37367 2023-07-29 19:47:20.709307 nsj_queue_lib-0.5.3/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    36802 2023-07-26 23:49:53.000000 nsj_queue_lib-0.5.3/README.md
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-29 19:47:20.709307 nsj_queue_lib-0.5.3/nsj_queue_lib/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-19 18:24:10.000000 nsj_queue_lib-0.5.3/nsj_queue_lib/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2954 2023-07-26 23:38:36.000000 nsj_queue_lib-0.5.3/nsj_queue_lib/db_gen.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       98 2023-07-25 22:33:41.000000 nsj_queue_lib-0.5.3/nsj_queue_lib/exception.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1090 2023-07-22 22:37:18.000000 nsj_queue_lib-0.5.3/nsj_queue_lib/lock_dao.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    10845 2023-07-26 20:42:13.000000 nsj_queue_lib-0.5.3/nsj_queue_lib/main_thread.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4814 2023-07-26 20:46:48.000000 nsj_queue_lib-0.5.3/nsj_queue_lib/notify_thread.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3243 2023-07-22 23:57:02.000000 nsj_queue_lib-0.5.3/nsj_queue_lib/purge_thread.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4684 2023-07-29 19:47:12.000000 nsj_queue_lib-0.5.3/nsj_queue_lib/queue_client.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4913 2023-07-22 23:57:41.000000 nsj_queue_lib-0.5.3/nsj_queue_lib/retry_thread.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     5259 2023-07-26 18:39:19.000000 nsj_queue_lib-0.5.3/nsj_queue_lib/retry_util.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2032 2023-07-26 20:47:28.000000 nsj_queue_lib-0.5.3/nsj_queue_lib/settings.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     9746 2023-07-26 20:45:47.000000 nsj_queue_lib-0.5.3/nsj_queue_lib/tarefa_dao.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1756 2023-07-26 17:45:30.000000 nsj_queue_lib-0.5.3/nsj_queue_lib/worker_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      580 2023-07-26 21:58:04.000000 nsj_queue_lib-0.5.3/nsj_queue_lib/worker_fila_teste.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3204 2023-07-26 23:08:43.000000 nsj_queue_lib-0.5.3/nsj_queue_lib/worker_pub_sub_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1392 2023-07-28 17:51:07.000000 nsj_queue_lib-0.5.3/nsj_queue_lib/worker_pub_sub_teste.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2162 2023-07-26 17:51:34.000000 nsj_queue_lib-0.5.3/nsj_queue_lib/worker_webhook.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-29 19:47:20.709307 nsj_queue_lib-0.5.3/nsj_queue_lib.egg-info/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    37367 2023-07-29 19:47:20.000000 nsj_queue_lib-0.5.3/nsj_queue_lib.egg-info/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      768 2023-07-29 19:47:20.000000 nsj_queue_lib-0.5.3/nsj_queue_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-07-29 19:47:20.000000 nsj_queue_lib-0.5.3/nsj_queue_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      110 2023-07-29 19:47:20.000000 nsj_queue_lib-0.5.3/nsj_queue_lib.egg-info/requires.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       14 2023-07-29 19:47:20.000000 nsj_queue_lib-0.5.3/nsj_queue_lib.egg-info/top_level.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-21 22:32:09.000000 nsj_queue_lib-0.5.3/pyproject.toml
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      834 2023-07-29 19:47:20.709307 nsj_queue_lib-0.5.3/setup.cfg
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-29 21:25:09.881403 nsj_queue_lib-0.5.4/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    37367 2023-07-29 21:25:09.881403 nsj_queue_lib-0.5.4/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    36802 2023-07-26 23:49:53.000000 nsj_queue_lib-0.5.4/README.md
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-29 21:25:09.881403 nsj_queue_lib-0.5.4/nsj_queue_lib/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-19 18:24:10.000000 nsj_queue_lib-0.5.4/nsj_queue_lib/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2954 2023-07-26 23:38:36.000000 nsj_queue_lib-0.5.4/nsj_queue_lib/db_gen.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       98 2023-07-25 22:33:41.000000 nsj_queue_lib-0.5.4/nsj_queue_lib/exception.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1090 2023-07-22 22:37:18.000000 nsj_queue_lib-0.5.4/nsj_queue_lib/lock_dao.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    10845 2023-07-26 20:42:13.000000 nsj_queue_lib-0.5.4/nsj_queue_lib/main_thread.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4814 2023-07-26 20:46:48.000000 nsj_queue_lib-0.5.4/nsj_queue_lib/notify_thread.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3243 2023-07-22 23:57:02.000000 nsj_queue_lib-0.5.4/nsj_queue_lib/purge_thread.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4684 2023-07-29 19:47:12.000000 nsj_queue_lib-0.5.4/nsj_queue_lib/queue_client.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4913 2023-07-22 23:57:41.000000 nsj_queue_lib-0.5.4/nsj_queue_lib/retry_thread.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     5259 2023-07-26 18:39:19.000000 nsj_queue_lib-0.5.4/nsj_queue_lib/retry_util.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2032 2023-07-26 20:47:28.000000 nsj_queue_lib-0.5.4/nsj_queue_lib/settings.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     9746 2023-07-26 20:45:47.000000 nsj_queue_lib-0.5.4/nsj_queue_lib/tarefa_dao.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1756 2023-07-26 17:45:30.000000 nsj_queue_lib-0.5.4/nsj_queue_lib/worker_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      580 2023-07-26 21:58:04.000000 nsj_queue_lib-0.5.4/nsj_queue_lib/worker_fila_teste.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3204 2023-07-26 23:08:43.000000 nsj_queue_lib-0.5.4/nsj_queue_lib/worker_pub_sub_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1392 2023-07-28 17:51:07.000000 nsj_queue_lib-0.5.4/nsj_queue_lib/worker_pub_sub_teste.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2162 2023-07-26 17:51:34.000000 nsj_queue_lib-0.5.4/nsj_queue_lib/worker_webhook.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-29 21:25:09.881403 nsj_queue_lib-0.5.4/nsj_queue_lib.egg-info/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    37367 2023-07-29 21:25:09.000000 nsj_queue_lib-0.5.4/nsj_queue_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      768 2023-07-29 21:25:09.000000 nsj_queue_lib-0.5.4/nsj_queue_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-07-29 21:25:09.000000 nsj_queue_lib-0.5.4/nsj_queue_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      110 2023-07-29 21:25:09.000000 nsj_queue_lib-0.5.4/nsj_queue_lib.egg-info/requires.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       14 2023-07-29 21:25:09.000000 nsj_queue_lib-0.5.4/nsj_queue_lib.egg-info/top_level.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-21 22:32:09.000000 nsj_queue_lib-0.5.4/pyproject.toml
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      834 2023-07-29 21:25:09.881403 nsj_queue_lib-0.5.4/setup.cfg
```

### Comparing `nsj_queue_lib-0.5.3/PKG-INFO` & `nsj_queue_lib-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj_queue_lib
-Version: 0.5.3
+Version: 0.5.4
 Summary: Biblioteca para facilitar a implementação de filas e workers.
 Home-page: https://github.com/Nasajon/nsj-queue-lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj-queue-lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_queue_lib-0.5.3/README.md` & `nsj_queue_lib-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.3/nsj_queue_lib/db_gen.py` & `nsj_queue_lib-0.5.4/nsj_queue_lib/db_gen.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.3/nsj_queue_lib/lock_dao.py` & `nsj_queue_lib-0.5.4/nsj_queue_lib/lock_dao.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.3/nsj_queue_lib/main_thread.py` & `nsj_queue_lib-0.5.4/nsj_queue_lib/main_thread.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.3/nsj_queue_lib/notify_thread.py` & `nsj_queue_lib-0.5.4/nsj_queue_lib/notify_thread.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.3/nsj_queue_lib/purge_thread.py` & `nsj_queue_lib-0.5.4/nsj_queue_lib/purge_thread.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.3/nsj_queue_lib/queue_client.py` & `nsj_queue_lib-0.5.4/nsj_queue_lib/queue_client.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.3/nsj_queue_lib/retry_thread.py` & `nsj_queue_lib-0.5.4/nsj_queue_lib/retry_thread.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.3/nsj_queue_lib/retry_util.py` & `nsj_queue_lib-0.5.4/nsj_queue_lib/retry_util.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.3/nsj_queue_lib/settings.py` & `nsj_queue_lib-0.5.4/nsj_queue_lib/settings.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.3/nsj_queue_lib/tarefa_dao.py` & `nsj_queue_lib-0.5.4/nsj_queue_lib/tarefa_dao.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.3/nsj_queue_lib/worker_base.py` & `nsj_queue_lib-0.5.4/nsj_queue_lib/worker_base.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.3/nsj_queue_lib/worker_fila_teste.py` & `nsj_queue_lib-0.5.4/nsj_queue_lib/worker_fila_teste.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.3/nsj_queue_lib/worker_pub_sub_base.py` & `nsj_queue_lib-0.5.4/nsj_queue_lib/worker_pub_sub_base.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.3/nsj_queue_lib/worker_pub_sub_teste.py` & `nsj_queue_lib-0.5.4/nsj_queue_lib/worker_pub_sub_teste.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.3/nsj_queue_lib/worker_webhook.py` & `nsj_queue_lib-0.5.4/nsj_queue_lib/worker_webhook.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.3/nsj_queue_lib.egg-info/PKG-INFO` & `nsj_queue_lib-0.5.4/nsj_queue_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj-queue-lib
-Version: 0.5.3
+Version: 0.5.4
 Summary: Biblioteca para facilitar a implementação de filas e workers.
 Home-page: https://github.com/Nasajon/nsj-queue-lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj-queue-lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_queue_lib-0.5.3/nsj_queue_lib.egg-info/SOURCES.txt` & `nsj_queue_lib-0.5.4/nsj_queue_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.3/setup.cfg` & `nsj_queue_lib-0.5.4/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nsj_queue_lib
-version = 0.5.3
+version = 0.5.4
 author = Nasajon Sistemas
 author_email = contact.dev@nasajon.com.br
 description = Biblioteca para facilitar a implementação de filas e workers.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Nasajon/nsj-queue-lib
 project_urls = 
@@ -20,15 +20,15 @@
 	= ./
 packages = find:
 python_requires = >=3.4
 install_requires = 
 	psycopg2_binary>=2.9.6
 	python-logging-loki>=0.3.1
 	pytest>=7.1.3
-	nsj_sql_utils_lib>=0.0.1
+	nsj_sql_utils_lib>=0.0.4
 	nsj_gcf_utils>=1.0.6
 
 [options.packages.find]
 where = ./
 
 [egg_info]
 tag_build =
```

