# Comparing `tmp/nsj_queue_lib-0.5.5.tar.gz` & `tmp/nsj_queue_lib-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_queue_lib-0.5.5.tar", last modified: Sun Jul 30 00:55:28 2023, max compression
+gzip compressed data, was "nsj_queue_lib-0.5.6.tar", last modified: Sun Jul 30 01:22:10 2023, max compression
```

## Comparing `nsj_queue_lib-0.5.5.tar` & `nsj_queue_lib-0.5.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-30 00:55:28.411855 nsj_queue_lib-0.5.5/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    37367 2023-07-30 00:55:28.411855 nsj_queue_lib-0.5.5/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    36802 2023-07-26 23:49:53.000000 nsj_queue_lib-0.5.5/README.md
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-30 00:55:28.411855 nsj_queue_lib-0.5.5/nsj_queue_lib/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-19 18:24:10.000000 nsj_queue_lib-0.5.5/nsj_queue_lib/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2954 2023-07-26 23:38:36.000000 nsj_queue_lib-0.5.5/nsj_queue_lib/db_gen.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       98 2023-07-25 22:33:41.000000 nsj_queue_lib-0.5.5/nsj_queue_lib/exception.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1090 2023-07-22 22:37:18.000000 nsj_queue_lib-0.5.5/nsj_queue_lib/lock_dao.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    10845 2023-07-26 20:42:13.000000 nsj_queue_lib-0.5.5/nsj_queue_lib/main_thread.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4814 2023-07-26 20:46:48.000000 nsj_queue_lib-0.5.5/nsj_queue_lib/notify_thread.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3243 2023-07-22 23:57:02.000000 nsj_queue_lib-0.5.5/nsj_queue_lib/purge_thread.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4684 2023-07-29 19:47:12.000000 nsj_queue_lib-0.5.5/nsj_queue_lib/queue_client.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4913 2023-07-22 23:57:41.000000 nsj_queue_lib-0.5.5/nsj_queue_lib/retry_thread.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     5259 2023-07-26 18:39:19.000000 nsj_queue_lib-0.5.5/nsj_queue_lib/retry_util.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2588 2023-07-30 00:55:00.000000 nsj_queue_lib-0.5.5/nsj_queue_lib/settings.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     9746 2023-07-26 20:45:47.000000 nsj_queue_lib-0.5.5/nsj_queue_lib/tarefa_dao.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1756 2023-07-26 17:45:30.000000 nsj_queue_lib-0.5.5/nsj_queue_lib/worker_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      580 2023-07-26 21:58:04.000000 nsj_queue_lib-0.5.5/nsj_queue_lib/worker_fila_teste.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3204 2023-07-26 23:08:43.000000 nsj_queue_lib-0.5.5/nsj_queue_lib/worker_pub_sub_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1392 2023-07-28 17:51:07.000000 nsj_queue_lib-0.5.5/nsj_queue_lib/worker_pub_sub_teste.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2162 2023-07-26 17:51:34.000000 nsj_queue_lib-0.5.5/nsj_queue_lib/worker_webhook.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-30 00:55:28.411855 nsj_queue_lib-0.5.5/nsj_queue_lib.egg-info/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    37367 2023-07-30 00:55:28.000000 nsj_queue_lib-0.5.5/nsj_queue_lib.egg-info/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      768 2023-07-30 00:55:28.000000 nsj_queue_lib-0.5.5/nsj_queue_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-07-30 00:55:28.000000 nsj_queue_lib-0.5.5/nsj_queue_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      110 2023-07-30 00:55:28.000000 nsj_queue_lib-0.5.5/nsj_queue_lib.egg-info/requires.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       14 2023-07-30 00:55:28.000000 nsj_queue_lib-0.5.5/nsj_queue_lib.egg-info/top_level.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-21 22:32:09.000000 nsj_queue_lib-0.5.5/pyproject.toml
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      834 2023-07-30 00:55:28.411855 nsj_queue_lib-0.5.5/setup.cfg
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-30 01:22:10.717744 nsj_queue_lib-0.5.6/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    37387 2023-07-30 01:22:10.717744 nsj_queue_lib-0.5.6/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    36822 2023-07-30 00:57:07.000000 nsj_queue_lib-0.5.6/README.md
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-30 01:22:10.717744 nsj_queue_lib-0.5.6/nsj_queue_lib/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-19 18:24:10.000000 nsj_queue_lib-0.5.6/nsj_queue_lib/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2954 2023-07-26 23:38:36.000000 nsj_queue_lib-0.5.6/nsj_queue_lib/db_gen.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       98 2023-07-25 22:33:41.000000 nsj_queue_lib-0.5.6/nsj_queue_lib/exception.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1090 2023-07-22 22:37:18.000000 nsj_queue_lib-0.5.6/nsj_queue_lib/lock_dao.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    10845 2023-07-26 20:42:13.000000 nsj_queue_lib-0.5.6/nsj_queue_lib/main_thread.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4814 2023-07-26 20:46:48.000000 nsj_queue_lib-0.5.6/nsj_queue_lib/notify_thread.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3243 2023-07-22 23:57:02.000000 nsj_queue_lib-0.5.6/nsj_queue_lib/purge_thread.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4684 2023-07-29 19:47:12.000000 nsj_queue_lib-0.5.6/nsj_queue_lib/queue_client.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4913 2023-07-22 23:57:41.000000 nsj_queue_lib-0.5.6/nsj_queue_lib/retry_thread.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     5259 2023-07-26 18:39:19.000000 nsj_queue_lib-0.5.6/nsj_queue_lib/retry_util.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2623 2023-07-30 01:20:54.000000 nsj_queue_lib-0.5.6/nsj_queue_lib/settings.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     9746 2023-07-26 20:45:47.000000 nsj_queue_lib-0.5.6/nsj_queue_lib/tarefa_dao.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1756 2023-07-26 17:45:30.000000 nsj_queue_lib-0.5.6/nsj_queue_lib/worker_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      580 2023-07-26 21:58:04.000000 nsj_queue_lib-0.5.6/nsj_queue_lib/worker_fila_teste.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3204 2023-07-26 23:08:43.000000 nsj_queue_lib-0.5.6/nsj_queue_lib/worker_pub_sub_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1392 2023-07-28 17:51:07.000000 nsj_queue_lib-0.5.6/nsj_queue_lib/worker_pub_sub_teste.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2162 2023-07-26 17:51:34.000000 nsj_queue_lib-0.5.6/nsj_queue_lib/worker_webhook.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-30 01:22:10.717744 nsj_queue_lib-0.5.6/nsj_queue_lib.egg-info/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    37387 2023-07-30 01:22:10.000000 nsj_queue_lib-0.5.6/nsj_queue_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      768 2023-07-30 01:22:10.000000 nsj_queue_lib-0.5.6/nsj_queue_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-07-30 01:22:10.000000 nsj_queue_lib-0.5.6/nsj_queue_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      110 2023-07-30 01:22:10.000000 nsj_queue_lib-0.5.6/nsj_queue_lib.egg-info/requires.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       14 2023-07-30 01:22:10.000000 nsj_queue_lib-0.5.6/nsj_queue_lib.egg-info/top_level.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-21 22:32:09.000000 nsj_queue_lib-0.5.6/pyproject.toml
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      834 2023-07-30 01:22:10.717744 nsj_queue_lib-0.5.6/setup.cfg
```

### Comparing `nsj_queue_lib-0.5.5/PKG-INFO` & `nsj_queue_lib-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj_queue_lib
-Version: 0.5.5
+Version: 0.5.6
 Summary: Biblioteca para facilitar a implementação de filas e workers.
 Home-page: https://github.com/Nasajon/nsj-queue-lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj-queue-lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -349,24 +349,24 @@
 
 **Obs.: Note que é preciso ter cuidado com a coluna `dead` na implementação de queries de monitooramento da fila.**
 
 ### Variáveis de Ambiente
 
 Seguem as principais variáveis de ambiente a serem consideradas na implementação de uma fila (obrigatórias em seu projeto):
 
-|        Variável        | Descrição                                                                                                                          |
-| :--------------------: | ---------------------------------------------------------------------------------------------------------------------------------- |
-|        DB_HOST         | IP ou nome do host de banco de dados.                                                                                              |
-|        DB_PORT         | Porta do banco de dados.                                                                                                           |
-|        DB_BASE         | Nome da base de dados.                                                                                                             |
-|        DB_USER         | Usuário para acesso ao banco de dados.                                                                                             |
-|        DB_PASS         | Seenha para acesso ao banco de dados.                                                                                              |
-|       QUEUE_NAME       | Nome da fila (não precisa ser igual ao nome da tabela, mas, pode ser; na prática representa o canal sobre o qual rodará o notify). |
-|      QUEUE_TABLE       | Nome da tabela da fila no banco de dados.                                                                                          |
-| QUEUE_SUBSCRIBER_TABLE | Nome da tabela de assinaturas, para filas PubSub no banco de dados (opcional).                                                     |
+|         Variável         | Descrição                                                                                                                          |
+| :----------------------: | ---------------------------------------------------------------------------------------------------------------------------------- |
+| DB_HOST ou DATABASE_HOST | IP ou nome do host de banco de dados.                                                                                              |
+| DB_PORT ou DATABASE_PORT | Porta do banco de dados.                                                                                                           |
+| DB_BASE ou DATABASE_NAME | Nome da base de dados.                                                                                                             |
+| DB_USER ou DATABASE_USER | Usuário para acesso ao banco de dados.                                                                                             |
+| DB_PASS ou DATABASE_PASS | Seenha para acesso ao banco de dados.                                                                                              |
+|        QUEUE_NAME        | Nome da fila (não precisa ser igual ao nome da tabela, mas, pode ser; na prática representa o canal sobre o qual rodará o notify). |
+|       QUEUE_TABLE        | Nome da tabela da fila no banco de dados.                                                                                          |
+|  QUEUE_SUBSCRIBER_TABLE  | Nome da tabela de assinaturas, para filas PubSub no banco de dados (opcional).                                                     |
 
 Seguem, agora, as variáveis opcionais, que permite customização mais avançada sobre o controle de filas:
 
 |          Variável          | Descrição                                                                                                                                                         | Padrão                                              |
 | :------------------------: | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------- |
 |         LOG_DEBUG          | Flag para indicar se os logs de debug serão impressos ou não.                                                                                                     | False                                               |
 |      QUEUE_MAX_RETRY       | Máximo de tentativas de uma tarefa na fila.                                                                                                                       | 100                                                 |
```

### Comparing `nsj_queue_lib-0.5.5/README.md` & `nsj_queue_lib-0.5.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -334,24 +334,24 @@
 
 **Obs.: Note que é preciso ter cuidado com a coluna `dead` na implementação de queries de monitooramento da fila.**
 
 ### Variáveis de Ambiente
 
 Seguem as principais variáveis de ambiente a serem consideradas na implementação de uma fila (obrigatórias em seu projeto):
 
-|        Variável        | Descrição                                                                                                                          |
-| :--------------------: | ---------------------------------------------------------------------------------------------------------------------------------- |
-|        DB_HOST         | IP ou nome do host de banco de dados.                                                                                              |
-|        DB_PORT         | Porta do banco de dados.                                                                                                           |
-|        DB_BASE         | Nome da base de dados.                                                                                                             |
-|        DB_USER         | Usuário para acesso ao banco de dados.                                                                                             |
-|        DB_PASS         | Seenha para acesso ao banco de dados.                                                                                              |
-|       QUEUE_NAME       | Nome da fila (não precisa ser igual ao nome da tabela, mas, pode ser; na prática representa o canal sobre o qual rodará o notify). |
-|      QUEUE_TABLE       | Nome da tabela da fila no banco de dados.                                                                                          |
-| QUEUE_SUBSCRIBER_TABLE | Nome da tabela de assinaturas, para filas PubSub no banco de dados (opcional).                                                     |
+|         Variável         | Descrição                                                                                                                          |
+| :----------------------: | ---------------------------------------------------------------------------------------------------------------------------------- |
+| DB_HOST ou DATABASE_HOST | IP ou nome do host de banco de dados.                                                                                              |
+| DB_PORT ou DATABASE_PORT | Porta do banco de dados.                                                                                                           |
+| DB_BASE ou DATABASE_NAME | Nome da base de dados.                                                                                                             |
+| DB_USER ou DATABASE_USER | Usuário para acesso ao banco de dados.                                                                                             |
+| DB_PASS ou DATABASE_PASS | Seenha para acesso ao banco de dados.                                                                                              |
+|        QUEUE_NAME        | Nome da fila (não precisa ser igual ao nome da tabela, mas, pode ser; na prática representa o canal sobre o qual rodará o notify). |
+|       QUEUE_TABLE        | Nome da tabela da fila no banco de dados.                                                                                          |
+|  QUEUE_SUBSCRIBER_TABLE  | Nome da tabela de assinaturas, para filas PubSub no banco de dados (opcional).                                                     |
 
 Seguem, agora, as variáveis opcionais, que permite customização mais avançada sobre o controle de filas:
 
 |          Variável          | Descrição                                                                                                                                                         | Padrão                                              |
 | :------------------------: | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------- |
 |         LOG_DEBUG          | Flag para indicar se os logs de debug serão impressos ou não.                                                                                                     | False                                               |
 |      QUEUE_MAX_RETRY       | Máximo de tentativas de uma tarefa na fila.                                                                                                                       | 100                                                 |
```

### Comparing `nsj_queue_lib-0.5.5/nsj_queue_lib/db_gen.py` & `nsj_queue_lib-0.5.6/nsj_queue_lib/db_gen.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.5/nsj_queue_lib/lock_dao.py` & `nsj_queue_lib-0.5.6/nsj_queue_lib/lock_dao.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.5/nsj_queue_lib/main_thread.py` & `nsj_queue_lib-0.5.6/nsj_queue_lib/main_thread.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.5/nsj_queue_lib/notify_thread.py` & `nsj_queue_lib-0.5.6/nsj_queue_lib/notify_thread.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.5/nsj_queue_lib/purge_thread.py` & `nsj_queue_lib-0.5.6/nsj_queue_lib/purge_thread.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.5/nsj_queue_lib/queue_client.py` & `nsj_queue_lib-0.5.6/nsj_queue_lib/queue_client.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.5/nsj_queue_lib/retry_thread.py` & `nsj_queue_lib-0.5.6/nsj_queue_lib/retry_thread.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.5/nsj_queue_lib/retry_util.py` & `nsj_queue_lib-0.5.6/nsj_queue_lib/retry_util.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.5/nsj_queue_lib/settings.py` & `nsj_queue_lib-0.5.6/nsj_queue_lib/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,24 +55,23 @@
 # Configurando o logger
 logger = logging.getLogger(WORKER_NAME)
 if LOG_DEBUG:
     logger.setLevel(logging.DEBUG)
 else:
     logger.setLevel(logging.INFO)
 
+log_format = logging.Formatter(
+    "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
+)
+
 console_handler = logging.StreamHandler(sys.stdout)
-if GRAFANA_URL is not None:
+console_handler.setFormatter(log_format)
+logger.addHandler(console_handler)
+
+if GRAFANA_URL is not None and GRAFANA_URL.strip() != "":
     loki_handler = logging_loki.LokiHandler(
         url=GRAFANA_URL,
         tags={ENV.upper() + "_flask_api_skeleton": ENV.lower() + "_log"},
         version="1",
     )
-
-console_format = logging.Formatter(
-    "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
-)
-
-console_handler.setFormatter(console_format)
-
-logger.addHandler(console_handler)
-if GRAFANA_URL is not None:
+    loki_handler.setFormatter(log_format)
     logger.addHandler(loki_handler)
```

### Comparing `nsj_queue_lib-0.5.5/nsj_queue_lib/tarefa_dao.py` & `nsj_queue_lib-0.5.6/nsj_queue_lib/tarefa_dao.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.5/nsj_queue_lib/worker_base.py` & `nsj_queue_lib-0.5.6/nsj_queue_lib/worker_base.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.5/nsj_queue_lib/worker_fila_teste.py` & `nsj_queue_lib-0.5.6/nsj_queue_lib/worker_fila_teste.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.5/nsj_queue_lib/worker_pub_sub_base.py` & `nsj_queue_lib-0.5.6/nsj_queue_lib/worker_pub_sub_base.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.5/nsj_queue_lib/worker_pub_sub_teste.py` & `nsj_queue_lib-0.5.6/nsj_queue_lib/worker_pub_sub_teste.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.5/nsj_queue_lib/worker_webhook.py` & `nsj_queue_lib-0.5.6/nsj_queue_lib/worker_webhook.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.5/nsj_queue_lib.egg-info/PKG-INFO` & `nsj_queue_lib-0.5.6/nsj_queue_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj-queue-lib
-Version: 0.5.5
+Version: 0.5.6
 Summary: Biblioteca para facilitar a implementação de filas e workers.
 Home-page: https://github.com/Nasajon/nsj-queue-lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj-queue-lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -349,24 +349,24 @@
 
 **Obs.: Note que é preciso ter cuidado com a coluna `dead` na implementação de queries de monitooramento da fila.**
 
 ### Variáveis de Ambiente
 
 Seguem as principais variáveis de ambiente a serem consideradas na implementação de uma fila (obrigatórias em seu projeto):
 
-|        Variável        | Descrição                                                                                                                          |
-| :--------------------: | ---------------------------------------------------------------------------------------------------------------------------------- |
-|        DB_HOST         | IP ou nome do host de banco de dados.                                                                                              |
-|        DB_PORT         | Porta do banco de dados.                                                                                                           |
-|        DB_BASE         | Nome da base de dados.                                                                                                             |
-|        DB_USER         | Usuário para acesso ao banco de dados.                                                                                             |
-|        DB_PASS         | Seenha para acesso ao banco de dados.                                                                                              |
-|       QUEUE_NAME       | Nome da fila (não precisa ser igual ao nome da tabela, mas, pode ser; na prática representa o canal sobre o qual rodará o notify). |
-|      QUEUE_TABLE       | Nome da tabela da fila no banco de dados.                                                                                          |
-| QUEUE_SUBSCRIBER_TABLE | Nome da tabela de assinaturas, para filas PubSub no banco de dados (opcional).                                                     |
+|         Variável         | Descrição                                                                                                                          |
+| :----------------------: | ---------------------------------------------------------------------------------------------------------------------------------- |
+| DB_HOST ou DATABASE_HOST | IP ou nome do host de banco de dados.                                                                                              |
+| DB_PORT ou DATABASE_PORT | Porta do banco de dados.                                                                                                           |
+| DB_BASE ou DATABASE_NAME | Nome da base de dados.                                                                                                             |
+| DB_USER ou DATABASE_USER | Usuário para acesso ao banco de dados.                                                                                             |
+| DB_PASS ou DATABASE_PASS | Seenha para acesso ao banco de dados.                                                                                              |
+|        QUEUE_NAME        | Nome da fila (não precisa ser igual ao nome da tabela, mas, pode ser; na prática representa o canal sobre o qual rodará o notify). |
+|       QUEUE_TABLE        | Nome da tabela da fila no banco de dados.                                                                                          |
+|  QUEUE_SUBSCRIBER_TABLE  | Nome da tabela de assinaturas, para filas PubSub no banco de dados (opcional).                                                     |
 
 Seguem, agora, as variáveis opcionais, que permite customização mais avançada sobre o controle de filas:
 
 |          Variável          | Descrição                                                                                                                                                         | Padrão                                              |
 | :------------------------: | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------- |
 |         LOG_DEBUG          | Flag para indicar se os logs de debug serão impressos ou não.                                                                                                     | False                                               |
 |      QUEUE_MAX_RETRY       | Máximo de tentativas de uma tarefa na fila.                                                                                                                       | 100                                                 |
```

### Comparing `nsj_queue_lib-0.5.5/nsj_queue_lib.egg-info/SOURCES.txt` & `nsj_queue_lib-0.5.6/nsj_queue_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.5.5/setup.cfg` & `nsj_queue_lib-0.5.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nsj_queue_lib
-version = 0.5.5
+version = 0.5.6
 author = Nasajon Sistemas
 author_email = contact.dev@nasajon.com.br
 description = Biblioteca para facilitar a implementação de filas e workers.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Nasajon/nsj-queue-lib
 project_urls =
```

