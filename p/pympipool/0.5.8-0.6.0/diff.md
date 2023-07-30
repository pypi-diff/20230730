# Comparing `tmp/pympipool-0.5.8.tar.gz` & `tmp/pympipool-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pympipool-0.5.8.tar", last modified: Thu Jul 27 23:36:19 2023, max compression
+gzip compressed data, was "pympipool-0.6.0.tar", last modified: Sun Jul 30 15:42:18 2023, max compression
```

## Comparing `pympipool-0.5.8.tar` & `pympipool-0.6.0.tar`

### file list

```diff
@@ -1,59 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:19.940517 pympipool-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-27 23:36:17.000000 pympipool-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-27 23:36:17.000000 pympipool-0.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-27 23:36:19.940517 pympipool-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-07-27 23:36:17.000000 pympipool-0.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:19.940517 pympipool-0.5.8/pympipool/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-27 23:36:19.940517 pympipool-0.5.8/pympipool/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:19.936517 pympipool-0.5.8/pympipool/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/backend/mpiexec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:19.936517 pympipool-0.5.8/pympipool/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/interfaces/taskbroker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/interfaces/taskexecutor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:19.936517 pympipool-0.5.8/pympipool/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:19.936517 pympipool-0.5.8/pympipool/legacy/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/legacy/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/legacy/backend/mpipool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:19.936517 pympipool-0.5.8/pympipool/legacy/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/legacy/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/legacy/interfaces/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/legacy/interfaces/pool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:19.936517 pympipool-0.5.8/pympipool/legacy/shared/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/legacy/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/legacy/shared/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8668 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/legacy/shared/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:19.936517 pympipool-0.5.8/pympipool/shared/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/shared/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/shared/broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/shared/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/shared/taskexecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-27 23:36:17.000000 pympipool-0.5.8/pympipool/shared/thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:19.936517 pympipool-0.5.8/pympipool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-27 23:36:19.000000 pympipool-0.5.8/pympipool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-27 23:36:19.000000 pympipool-0.5.8/pympipool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 23:36:19.000000 pympipool-0.5.8/pympipool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-27 23:36:19.000000 pympipool-0.5.8/pympipool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-27 23:36:19.000000 pympipool-0.5.8/pympipool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-27 23:36:19.940517 pympipool-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-27 23:36:19.000000 pympipool-0.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:36:19.940517 pympipool-0.5.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-27 23:36:17.000000 pympipool-0.5.8/tests/test_communicator_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-07-27 23:36:17.000000 pympipool-0.5.8/tests/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-27 23:36:17.000000 pympipool-0.5.8/tests/test_future.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-27 23:36:17.000000 pympipool-0.5.8/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-27 23:36:17.000000 pympipool-0.5.8/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-27 23:36:17.000000 pympipool-0.5.8/tests/test_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-27 23:36:17.000000 pympipool-0.5.8/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-27 23:36:17.000000 pympipool-0.5.8/tests/test_parse_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-27 23:36:17.000000 pympipool-0.5.8/tests/test_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-27 23:36:17.000000 pympipool-0.5.8/tests/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-27 23:36:17.000000 pympipool-0.5.8/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-07-27 23:36:17.000000 pympipool-0.5.8/tests/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-27 23:36:17.000000 pympipool-0.5.8/tests/test_worker_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-27 23:36:17.000000 pympipool-0.5.8/tests/test_zmq.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-27 23:36:17.000000 pympipool-0.5.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:42:18.830976 pympipool-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-30 15:42:15.000000 pympipool-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-30 15:42:15.000000 pympipool-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-07-30 15:42:18.830976 pympipool-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10300 2023-07-30 15:42:15.000000 pympipool-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:42:18.830976 pympipool-0.6.0/pympipool/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-30 15:42:18.830976 pympipool-0.6.0/pympipool/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:42:18.826976 pympipool-0.6.0/pympipool/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/backend/mpiexec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:42:18.826976 pympipool-0.6.0/pympipool/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/interfaces/taskbroker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/interfaces/taskexecutor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:42:18.826976 pympipool-0.6.0/pympipool/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:42:18.826976 pympipool-0.6.0/pympipool/legacy/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/legacy/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/legacy/backend/mpipool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:42:18.826976 pympipool-0.6.0/pympipool/legacy/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/legacy/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/legacy/interfaces/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8788 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/legacy/interfaces/pool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:42:18.826976 pympipool-0.6.0/pympipool/legacy/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/legacy/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/legacy/shared/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/legacy/shared/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:42:18.830976 pympipool-0.6.0/pympipool/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/shared/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/shared/broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/shared/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/shared/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/shared/taskexecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/shared/thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:42:18.826976 pympipool-0.6.0/pympipool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-07-30 15:42:18.000000 pympipool-0.6.0/pympipool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-30 15:42:18.000000 pympipool-0.6.0/pympipool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 15:42:18.000000 pympipool-0.6.0/pympipool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-30 15:42:18.000000 pympipool-0.6.0/pympipool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-30 15:42:18.000000 pympipool-0.6.0/pympipool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-30 15:42:18.830976 pympipool-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-30 15:42:18.000000 pympipool-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:42:18.830976 pympipool-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-30 15:42:15.000000 pympipool-0.6.0/tests/test_communicator_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-30 15:42:15.000000 pympipool-0.6.0/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-07-30 15:42:15.000000 pympipool-0.6.0/tests/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-30 15:42:15.000000 pympipool-0.6.0/tests/test_future.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-30 15:42:15.000000 pympipool-0.6.0/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-30 15:42:15.000000 pympipool-0.6.0/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-30 15:42:15.000000 pympipool-0.6.0/tests/test_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-30 15:42:15.000000 pympipool-0.6.0/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-30 15:42:15.000000 pympipool-0.6.0/tests/test_parse_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-30 15:42:15.000000 pympipool-0.6.0/tests/test_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-30 15:42:15.000000 pympipool-0.6.0/tests/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-30 15:42:15.000000 pympipool-0.6.0/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-30 15:42:15.000000 pympipool-0.6.0/tests/test_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-07-30 15:42:15.000000 pympipool-0.6.0/tests/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-30 15:42:15.000000 pympipool-0.6.0/tests/test_worker_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-30 15:42:15.000000 pympipool-0.6.0/tests/test_zmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-30 15:42:15.000000 pympipool-0.6.0/versioneer.py
```

### Comparing `pympipool-0.5.8/LICENSE` & `pympipool-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.8/PKG-INFO` & `pympipool-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympipool
-Version: 0.5.8
+Version: 0.6.0
 Summary: pympipool - scale python functions over multiple compute nodes
 Home-page: https://github.com/jan-janssen/pympipool
 Author-email: jan.janssen@outlook.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
@@ -55,15 +55,21 @@
 the executor interface defined by the [`concurrent.futures.Executor`](https://docs.python.org/3/library/concurrent.futures.html#module-concurrent.futures).
 So functions are submitted to the `pympipool.Executor` using the `submit()` function, which returns an 
 [`concurrent.futures.Future`](https://docs.python.org/3/library/concurrent.futures.html#future-objects) object. With 
 these [`concurrent.futures.Future`](https://docs.python.org/3/library/concurrent.futures.html#future-objects) objects 
 asynchronous workflows can be constructed which periodically check if the computation is completed `done()` and then
 query the results using the `result()` function. The limitation of the `pympipool.Executor` is lack of load balancing, 
 each `pympipool.Executor` acts as a serial first in first out (FIFO) queue. So it is the task of the user to balance the
-load of many different tasks over multiple `pympipool.Executor` instances. 
+load of many different tasks over multiple `pympipool.Executor` instances.
+* [`pympipool.HPCExecutor`](https://pympipool.readthedocs.io/en/latest/interfaces.html#hpcexecutor>): To address the 
+limitation of the `pympipool.Executor` that only a single task is executed at any time, the `pympipool.HPCExecutor` 
+provides a wrapper around multiple `pympipool.Executor` objects. It balances the queues of the individual 
+`pympipool.Executor` objects to maximize the throughput for the given resources. This functionality comes with an 
+additional overhead of another thread, acting as a broker between the task queue of the `pympipool.HPCExecutor` and the
+individual `pympipool.Executor` objects. 
 * [`pympipool.PoolExecutor`](https://pympipool.readthedocs.io/en/latest/interfaces.html#poolexecutor): To combine the 
 functionality of the `pympipool.Pool` and the `pympipool.Executor` the `pympipool.PoolExecutor` again connects to the
 [`mpi4py.futures.MPIPoolExecutor`](https://mpi4py.readthedocs.io/en/stable/mpi4py.futures.html#mpipoolexecutor).
 Still in contrast to the `pympipool.Pool` it does not implement the `map()` and `starmap()` functions but rather the 
 `submit()` function based on the [`concurrent.futures.Executor`](https://docs.python.org/3/library/concurrent.futures.html#module-concurrent.futures)
 interface. In this case the load balancing happens internally and the maximum number of workers `max_workers` defines
 the maximum number of parallel tasks. But only serial python tasks can be executed in contrast to the `pympipool.Executor`
@@ -93,21 +99,24 @@
 # Documentation
 * [Installation](https://pympipool.readthedocs.io/en/latest/installation.html) 
   * [pypi-based installation](https://pympipool.readthedocs.io/en/latest/installation.html#pypi-based-installation)
   * [conda-based installation](https://pympipool.readthedocs.io/en/latest/installation.html#conda-based-installation)
 * [Interfaces](https://pympipool.readthedocs.io/en/latest/interfaces.html) 
   * [Pool](https://pympipool.readthedocs.io/en/latest/interfaces.html#pool)
   * [Executor](https://pympipool.readthedocs.io/en/latest/interfaces.html#executor)
+  * [HPCExecutor](https://pympipool.readthedocs.io/en/latest/interfaces.html#hpcexecutor>)
   * [ParallelExecutor](https://pympipool.readthedocs.io/en/latest/interfaces.html#poolexecutor)
   * [MPISpawnPool](https://pympipool.readthedocs.io/en/latest/interfaces.html#mpispawnpool)
   * [SocketInterface](https://pympipool.readthedocs.io/en/latest/interfaces.html#socketinterface)
 * [Development](https://pympipool.readthedocs.io/en/latest/development.html) 
 
 # License
-`pympipool` is released under the BSD license https://github.com/pyiron/pympipool/blob/main/LICENSE . It is a spin-off of the `pyiron` project https://github.com/pyiron/pyiron therefore if you use `pympipool` for calculation which result in a scientific publication, please cite: 
+`pympipool` is released under the BSD license https://github.com/pyiron/pympipool/blob/main/LICENSE . It is a spin-off 
+of the `pyiron` project https://github.com/pyiron/pyiron therefore if you use `pympipool` for calculation which result 
+in a scientific publication, please cite: 
 
     @article{pyiron-paper,
       title = {pyiron: An integrated development environment for computational materials science},
       journal = {Computational Materials Science},
       volume = {163},
       pages = {24 - 36},
       year = {2019},
```

### Comparing `pympipool-0.5.8/README.md` & `pympipool-0.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,21 @@
 the executor interface defined by the [`concurrent.futures.Executor`](https://docs.python.org/3/library/concurrent.futures.html#module-concurrent.futures).
 So functions are submitted to the `pympipool.Executor` using the `submit()` function, which returns an 
 [`concurrent.futures.Future`](https://docs.python.org/3/library/concurrent.futures.html#future-objects) object. With 
 these [`concurrent.futures.Future`](https://docs.python.org/3/library/concurrent.futures.html#future-objects) objects 
 asynchronous workflows can be constructed which periodically check if the computation is completed `done()` and then
 query the results using the `result()` function. The limitation of the `pympipool.Executor` is lack of load balancing, 
 each `pympipool.Executor` acts as a serial first in first out (FIFO) queue. So it is the task of the user to balance the
-load of many different tasks over multiple `pympipool.Executor` instances. 
+load of many different tasks over multiple `pympipool.Executor` instances.
+* [`pympipool.HPCExecutor`](https://pympipool.readthedocs.io/en/latest/interfaces.html#hpcexecutor>): To address the 
+limitation of the `pympipool.Executor` that only a single task is executed at any time, the `pympipool.HPCExecutor` 
+provides a wrapper around multiple `pympipool.Executor` objects. It balances the queues of the individual 
+`pympipool.Executor` objects to maximize the throughput for the given resources. This functionality comes with an 
+additional overhead of another thread, acting as a broker between the task queue of the `pympipool.HPCExecutor` and the
+individual `pympipool.Executor` objects. 
 * [`pympipool.PoolExecutor`](https://pympipool.readthedocs.io/en/latest/interfaces.html#poolexecutor): To combine the 
 functionality of the `pympipool.Pool` and the `pympipool.Executor` the `pympipool.PoolExecutor` again connects to the
 [`mpi4py.futures.MPIPoolExecutor`](https://mpi4py.readthedocs.io/en/stable/mpi4py.futures.html#mpipoolexecutor).
 Still in contrast to the `pympipool.Pool` it does not implement the `map()` and `starmap()` functions but rather the 
 `submit()` function based on the [`concurrent.futures.Executor`](https://docs.python.org/3/library/concurrent.futures.html#module-concurrent.futures)
 interface. In this case the load balancing happens internally and the maximum number of workers `max_workers` defines
 the maximum number of parallel tasks. But only serial python tasks can be executed in contrast to the `pympipool.Executor`
@@ -75,21 +81,24 @@
 # Documentation
 * [Installation](https://pympipool.readthedocs.io/en/latest/installation.html) 
   * [pypi-based installation](https://pympipool.readthedocs.io/en/latest/installation.html#pypi-based-installation)
   * [conda-based installation](https://pympipool.readthedocs.io/en/latest/installation.html#conda-based-installation)
 * [Interfaces](https://pympipool.readthedocs.io/en/latest/interfaces.html) 
   * [Pool](https://pympipool.readthedocs.io/en/latest/interfaces.html#pool)
   * [Executor](https://pympipool.readthedocs.io/en/latest/interfaces.html#executor)
+  * [HPCExecutor](https://pympipool.readthedocs.io/en/latest/interfaces.html#hpcexecutor>)
   * [ParallelExecutor](https://pympipool.readthedocs.io/en/latest/interfaces.html#poolexecutor)
   * [MPISpawnPool](https://pympipool.readthedocs.io/en/latest/interfaces.html#mpispawnpool)
   * [SocketInterface](https://pympipool.readthedocs.io/en/latest/interfaces.html#socketinterface)
 * [Development](https://pympipool.readthedocs.io/en/latest/development.html) 
 
 # License
-`pympipool` is released under the BSD license https://github.com/pyiron/pympipool/blob/main/LICENSE . It is a spin-off of the `pyiron` project https://github.com/pyiron/pyiron therefore if you use `pympipool` for calculation which result in a scientific publication, please cite: 
+`pympipool` is released under the BSD license https://github.com/pyiron/pympipool/blob/main/LICENSE . It is a spin-off 
+of the `pyiron` project https://github.com/pyiron/pyiron therefore if you use `pympipool` for calculation which result 
+in a scientific publication, please cite: 
 
     @article{pyiron-paper,
       title = {pyiron: An integrated development environment for computational materials science},
       journal = {Computational Materials Science},
       volume = {163},
       pages = {24 - 36},
       year = {2019},
```

### Comparing `pympipool-0.5.8/pympipool/__init__.py` & `pympipool-0.6.0/pympipool/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from pympipool.shared.communication import (
     SocketInterface,
-    connect_to_socket_interface,
-    send_result,
-    close_connection,
-    receive_instruction,
+    interface_connect,
+    interface_bootup,
+    interface_send,
+    interface_shutdown,
+    interface_receive,
 )
 from pympipool.interfaces.taskbroker import HPCExecutor
 from pympipool.interfaces.taskexecutor import Executor
 from pympipool.legacy.interfaces.executor import PoolExecutor
 from pympipool.legacy.interfaces.pool import Pool, MPISpawnPool
 from pympipool.shared.thread import RaisingThread
 from pympipool.shared.taskexecutor import cancel_items_in_queue
```

### Comparing `pympipool-0.5.8/pympipool/backend/mpiexec.py` & `pympipool-0.6.0/pympipool/backend/mpiexec.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from os.path import abspath
 import pickle
 import sys
 
 import cloudpickle
 
 from pympipool.shared.communication import (
-    connect_to_socket_interface,
-    send_result,
-    close_connection,
-    receive_instruction,
+    interface_connect,
+    interface_send,
+    interface_shutdown,
+    interface_receive,
 )
 from pympipool.shared.backend import call_funct, parse_arguments
 
 
 def main():
     from mpi4py import MPI
 
@@ -22,15 +22,15 @@
         pickle.HIGHEST_PROTOCOL,
     )
     mpi_rank_zero = MPI.COMM_WORLD.Get_rank() == 0
     mpi_size_larger_one = MPI.COMM_WORLD.Get_size() > 1
 
     argument_dict = parse_arguments(argument_lst=sys.argv)
     if mpi_rank_zero:
-        context, socket = connect_to_socket_interface(
+        context, socket = interface_connect(
             host=argument_dict["host"], port=argument_dict["zmqport"]
         )
     else:
         context = None
         socket = None
 
     memory = None
@@ -39,24 +39,24 @@
     cwd = abspath(".")
     if cwd not in sys.path:
         sys.path.insert(1, cwd)
 
     while True:
         # Read from socket
         if mpi_rank_zero:
-            input_dict = receive_instruction(socket=socket)
+            input_dict = interface_receive(socket=socket)
         else:
             input_dict = None
         input_dict = MPI.COMM_WORLD.bcast(input_dict, root=0)
 
         # Parse input
         if "shutdown" in input_dict.keys() and input_dict["shutdown"]:
             if mpi_rank_zero:
-                send_result(socket=socket, result_dict={"result": True})
-                close_connection(socket=socket, context=context)
+                interface_send(socket=socket, result_dict={"result": True})
+                interface_shutdown(socket=socket, context=context)
             break
         elif (
             "fn" in input_dict.keys()
             and "init" not in input_dict.keys()
             and "args" in input_dict.keys()
             and "kwargs" in input_dict.keys()
         ):
@@ -65,22 +65,22 @@
                 output = call_funct(input_dict=input_dict, funct=None, memory=memory)
                 if mpi_size_larger_one:
                     output_reply = MPI.COMM_WORLD.gather(output, root=0)
                 else:
                     output_reply = output
             except Exception as error:
                 if mpi_rank_zero:
-                    send_result(
+                    interface_send(
                         socket=socket,
                         result_dict={"error": error, "error_type": str(type(error))},
                     )
             else:
                 # Send output
                 if mpi_rank_zero:
-                    send_result(socket=socket, result_dict={"result": output_reply})
+                    interface_send(socket=socket, result_dict={"result": output_reply})
         elif (
             "init" in input_dict.keys()
             and input_dict["init"]
             and "args" in input_dict.keys()
             and "kwargs" in input_dict.keys()
         ):
             memory = call_funct(input_dict=input_dict, funct=None)
```

### Comparing `pympipool-0.5.8/pympipool/interfaces/taskbroker.py` & `pympipool-0.6.0/pympipool/interfaces/taskbroker.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.8/pympipool/interfaces/taskexecutor.py` & `pympipool-0.6.0/pympipool/interfaces/taskexecutor.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.8/pympipool/legacy/backend/mpipool.py` & `pympipool-0.6.0/pympipool/legacy/backend/mpipool.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from os.path import abspath
 import pickle
 import sys
 
 import cloudpickle
 
 from pympipool.shared.communication import (
-    connect_to_socket_interface,
-    send_result,
-    close_connection,
-    receive_instruction,
+    interface_connect,
+    interface_send,
+    interface_shutdown,
+    interface_receive,
 )
 from pympipool.legacy.shared.backend import parse_socket_communication, parse_arguments
 
 
 def main():
     from mpi4py import MPI
 
@@ -32,32 +32,32 @@
         sys.path.insert(1, cwd)
 
     with MPIPoolExecutor(
         max_workers=int(argument_dict["total_cores"]),
         path=sys.path,  # required for flux interface - otherwise the current path is not included in the python path
     ) as executor:
         if executor is not None:
-            context, socket = connect_to_socket_interface(
+            context, socket = interface_connect(
                 host=argument_dict["host"], port=argument_dict["zmqport"]
             )
             while True:
                 output = parse_socket_communication(
                     executor=executor,
-                    input_dict=receive_instruction(socket=socket),
+                    input_dict=interface_receive(socket=socket),
                     future_dict=future_dict,
                     cores_per_task=int(argument_dict["cores_per_task"]),
                 )
                 if "exit" in output.keys() and output["exit"]:
                     if "result" in output.keys():
-                        send_result(
+                        interface_send(
                             socket=socket, result_dict={"result": output["result"]}
                         )
                     else:
-                        send_result(socket=socket, result_dict={"result": True})
-                    close_connection(socket=socket, context=context)
+                        interface_send(socket=socket, result_dict={"result": True})
+                    interface_shutdown(socket=socket, context=context)
                     break
                 elif isinstance(output, dict):
-                    send_result(socket=socket, result_dict=output)
+                    interface_send(socket=socket, result_dict=output)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pympipool-0.5.8/pympipool/legacy/interfaces/executor.py` & `pympipool-0.6.0/pympipool/legacy/interfaces/executor.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.8/pympipool/legacy/interfaces/pool.py` & `pympipool-0.6.0/pympipool/legacy/interfaces/pool.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from abc import ABC
 
-from pympipool.shared.communication import SocketInterface
+from pympipool.shared.communication import interface_bootup
 from pympipool.shared.taskexecutor import cloudpickle_register
-from pympipool.legacy.shared.interface import get_parallel_subprocess_command
+from pympipool.legacy.shared.interface import get_pool_command
 
 
 class PoolBase(ABC):
     """
     Base class for the Pool and MPISpawnPool classes defined below. The PoolBase class is not intended to be used
     alone. Rather it implements the __enter__(), __exit__() and shutdown() function shared between the derived classes.
     """
 
-    def __init__(self, queue_adapter=None, queue_adapter_kwargs=None):
+    def __init__(self):
         self._future_dict = {}
-        self._interface = SocketInterface(
-            queue_adapter=queue_adapter, queue_adapter_kwargs=queue_adapter_kwargs
-        )
+        self._interface = None
         cloudpickle_register(ind=3)
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.shutdown(wait=True)
@@ -67,31 +65,25 @@
         oversubscribe=False,
         enable_flux_backend=False,
         enable_slurm_backend=False,
         cwd=None,
         queue_adapter=None,
         queue_adapter_kwargs=None,
     ):
-        super().__init__(
-            queue_adapter=queue_adapter, queue_adapter_kwargs=queue_adapter_kwargs
-        )
-        self._interface.bootup(
-            command_lst=get_parallel_subprocess_command(
-                port_selected=self._interface.bind_to_random_port(),
-                cores=max_workers,
-                cores_per_task=1,
-                gpus_per_task=gpus_per_task,
-                oversubscribe=oversubscribe,
-                enable_flux_backend=enable_flux_backend,
-                enable_slurm_backend=enable_slurm_backend,
-                enable_mpi4py_backend=True,
-                enable_multi_host=queue_adapter is not None,
-            ),
+        super().__init__()
+        self._interface = interface_bootup(
+            command_lst=get_pool_command(cores_total=max_workers, ranks_per_task=1)[0],
             cwd=cwd,
             cores=max_workers,
+            gpus_per_core=gpus_per_task,
+            oversubscribe=oversubscribe,
+            enable_flux_backend=enable_flux_backend,
+            enable_slurm_backend=enable_slurm_backend,
+            queue_adapter=queue_adapter,
+            queue_adapter_kwargs=queue_adapter_kwargs,
         )
 
     def map(self, func, iterable, chunksize=None):
         """
         Map a given function on a list of attributes.
 
         Args:
@@ -174,31 +166,28 @@
         ranks_per_task=1,
         gpus_per_task=0,
         oversubscribe=False,
         cwd=None,
         queue_adapter=None,
         queue_adapter_kwargs=None,
     ):
-        super().__init__(
-            queue_adapter=queue_adapter, queue_adapter_kwargs=queue_adapter_kwargs
+        super().__init__()
+        command_lst, cores = get_pool_command(
+            cores_total=max_ranks, ranks_per_task=ranks_per_task
         )
-        self._interface.bootup(
-            command_lst=get_parallel_subprocess_command(
-                port_selected=self._interface.bind_to_random_port(),
-                cores=max_ranks,
-                cores_per_task=ranks_per_task,
-                gpus_per_task=gpus_per_task,
-                oversubscribe=oversubscribe,
-                enable_flux_backend=False,
-                enable_slurm_backend=False,
-                enable_mpi4py_backend=True,
-                enable_multi_host=queue_adapter is not None,
-            ),
+        self._interface = interface_bootup(
+            command_lst=command_lst,
             cwd=cwd,
-            cores=max_ranks,
+            cores=cores,
+            gpus_per_core=gpus_per_task,
+            oversubscribe=oversubscribe,
+            enable_flux_backend=False,
+            enable_slurm_backend=False,
+            queue_adapter=queue_adapter,
+            queue_adapter_kwargs=queue_adapter_kwargs,
         )
 
     def map(self, func, iterable, chunksize=None):
         """
         Map a given function on a list of attributes.
 
         Args:
```

### Comparing `pympipool-0.5.8/pympipool/legacy/shared/backend.py` & `pympipool-0.6.0/pympipool/legacy/shared/backend.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.8/pympipool/shared/backend.py` & `pympipool-0.6.0/pympipool/shared/backend.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.8/pympipool/shared/broker.py` & `pympipool-0.6.0/pympipool/shared/broker.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.8/pympipool/shared/communication.py` & `pympipool-0.6.0/pympipool/shared/communication.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-import subprocess
-
 import cloudpickle
+import socket
 import zmq
 
+from pympipool.shared.connections import get_connection_interface
+
 
 class SocketInterface(object):
     """
     The SocketInterface is an abstraction layer on top of the zero message queue.
 
     Args:
-        queue_adapter (pysqa.queueadapter.QueueAdapter): generalized interface to various queuing systems
-        queue_adapter_kwargs (dict/None): keyword arguments for the submit_job() function of the queue adapter
+        interface (pympipool.shared.connections.BaseInterface): Interface for starting the parallel process
     """
 
-    def __init__(self, queue_adapter=None, queue_adapter_kwargs=None):
+    def __init__(self, interface=None):
         self._context = zmq.Context()
         self._socket = self._context.socket(zmq.PAIR)
         self._process = None
-        self._queue_adapter = queue_adapter
-        self._queue_adapter_kwargs = queue_adapter_kwargs
+        self._interface = interface
 
     def send_dict(self, input_dict):
         """
         Send a dictionary with instructions to a connected client process.
 
         Args:
             input_dict (dict): dictionary of commands to be communicated. The key "shutdown" is reserved to stop the
@@ -64,109 +63,116 @@
         processes can then connect to this port to receive instructions and send results.
 
         Returns:
             int: port the SocketInterface instance is bound to.
         """
         return self._socket.bind_to_random_port("tcp://*")
 
-    def bootup(self, command_lst, cwd=None, cores=None):
+    def bootup(self, command_lst):
         """
         Boot up the client process to connect to the SocketInterface.
 
         Args:
             command_lst (list): list of strings to start the client process
-            cwd (str/None): current working directory where the parallel python task is executed
-            cores (str/ None): if the job is submitted to a queuing system using the pysqa.queueadapter.QueueAdapter
-                then cores defines the number of cores to be used for the specific queuing system allocation to execute
-                the client process.
-        """
-        if self._queue_adapter is not None:
-            self._queue_adapter.submit_job(
-                working_directory=cwd,
-                cores=cores,
-                command=" ".join(command_lst),
-                **self._queue_adapter_kwargs
-            )
-        else:
-            self._process = subprocess.Popen(
-                args=command_lst,
-                stdout=subprocess.PIPE,
-                stderr=subprocess.PIPE,
-                stdin=subprocess.PIPE,
-                cwd=cwd,
-            )
+        """
+        self._interface.bootup(command_lst=command_lst)
 
     def shutdown(self, wait=True):
         result = None
-        if self._process is not None and self._process.poll() is None:
-            result = self.send_and_receive_dict(
-                input_dict={"shutdown": True, "wait": wait}
-            )
-            self._process_close(wait=wait)
-        elif self._queue_adapter is not None and self._socket is not None:
+        if self._interface.poll():
             result = self.send_and_receive_dict(
                 input_dict={"shutdown": True, "wait": wait}
             )
+            self._interface.shutdown(wait=wait)
         if self._socket is not None:
             self._socket.close()
         if self._context is not None:
             self._context.term()
         self._process = None
         self._socket = None
         self._context = None
         return result
 
-    def _process_close(self, wait=True):
-        self._process.terminate()
-        self._process.stdout.close()
-        self._process.stdin.close()
-        self._process.stderr.close()
-        if wait:
-            self._process.wait()
-
     def __del__(self):
         self.shutdown(wait=True)
 
 
-def connect_to_socket_interface(host, port):
+def interface_bootup(
+    command_lst,
+    cwd=None,
+    cores=1,
+    gpus_per_core=0,
+    oversubscribe=False,
+    enable_flux_backend=False,
+    enable_slurm_backend=False,
+    queue_adapter=None,
+    queue_type=None,
+    queue_adapter_kwargs=None,
+):
+    if enable_flux_backend or enable_slurm_backend or queue_adapter is not None:
+        command_lst += [
+            "--host",
+            socket.gethostname(),
+        ]
+    connections = get_connection_interface(
+        cwd=cwd,
+        cores=cores,
+        gpus_per_core=gpus_per_core,
+        oversubscribe=oversubscribe,
+        enable_flux_backend=enable_flux_backend,
+        enable_slurm_backend=enable_slurm_backend,
+        queue_adapter=queue_adapter,
+        queue_type=queue_type,
+        queue_adapter_kwargs=queue_adapter_kwargs,
+    )
+    interface = SocketInterface(interface=connections)
+    command_lst += [
+        "--zmqport",
+        str(interface.bind_to_random_port()),
+    ]
+    interface.bootup(command_lst=command_lst)
+    return interface
+
+
+def interface_connect(host, port):
     """
     Connect to an existing SocketInterface instance by providing the hostname and the port as strings.
 
     Args:
         host (str): hostname of the host running the SocketInterface instance to connect to.
         port (str): port on the host the SocketInterface instance is running on.
     """
     context = zmq.Context()
     socket = context.socket(zmq.PAIR)
     socket.connect("tcp://" + host + ":" + port)
     return context, socket
 
 
-def send_result(socket, result_dict):
+def interface_send(socket, result_dict):
     """
     Send results to a SocketInterface instance.
 
     Args:
         socket (zmq.Socket): socket for the connection
         result_dict (dict): dictionary to be sent, supported keys are result, error and error_type.
     """
     socket.send(cloudpickle.dumps(result_dict))
 
 
-def receive_instruction(socket):
+def interface_receive(socket):
     """
     Receive instructions from a SocketInterface instance.
 
     Args:
         socket (zmq.Socket): socket for the connection
     """
     return cloudpickle.loads(socket.recv())
 
 
-def close_connection(socket, context):
+def interface_shutdown(socket, context):
     """
     Close the connection to a SocketInterface instance.
 
     Args:
         socket (zmq.Socket): socket for the connection
         context (zmq.sugar.context.Context): context for the connection
     """
```

### Comparing `pympipool-0.5.8/pympipool/shared/taskexecutor.py` & `pympipool-0.6.0/pympipool/shared/taskexecutor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import inspect
 import os
-import socket
 import queue
 
 import cloudpickle
 
-from pympipool.shared.communication import SocketInterface
+from pympipool.shared.communication import interface_bootup
 
 
 def cancel_items_in_queue(que):
     """
     Cancel items which are still waiting in the queue. If the executor is busy tasks remain in the queue, so the future
     objects have to be cancelled when the executor shuts down.
 
@@ -42,69 +41,14 @@
     """
     try:  # When executed in a jupyter notebook this can cause a ValueError - in this case we just ignore it.
         cloudpickle.register_pickle_by_value(inspect.getmodule(inspect.stack()[ind][0]))
     except ValueError:
         pass
 
 
-def command_line_options(
-    hostname,
-    port_selected,
-    path,
-    cores,
-    gpus_per_task=0,
-    oversubscribe=False,
-    enable_flux_backend=False,
-    enable_slurm_backend=False,
-    enable_multi_host=False,
-):
-    """
-    Translate the individual parameters to command line options.
-
-    Args:
-        hostname (str): name of the host where the SocketInterface instance runs the client process should conenct to.
-        port_selected (int): port the SocketInterface instance runs on.
-        path (str): path to the python script which should be executed as client process.
-        cores (int): defines the total number of MPI ranks to use
-        cores_per_task (int): number of MPI ranks per task - defaults to 1
-        gpus_per_task (int): number of GPUs per MPI rank - defaults to 0
-        oversubscribe (bool): enable of disable the oversubscribe feature of OpenMPI - defaults to False
-        enable_flux_backend (bool): enable the flux-framework as backend - defaults to False
-        enable_slurm_backend (bool): enable the SLURM queueing system as backend - defaults to False
-        enable_mpi4py_backend (bool): enable the mpi4py.futures module - defaults to True
-        enable_multi_host (bool): communicate the host to connect to - defaults to False
-
-    Returns:
-        list: list of strings to be executed on the command line
-    """
-    if enable_flux_backend:
-        command_lst = ["flux", "run"]
-    elif enable_slurm_backend:
-        command_lst = ["srun"]
-    else:
-        command_lst = ["mpiexec"]
-    if gpus_per_task > 0 and (enable_flux_backend or enable_slurm_backend):
-        command_lst += ["--gpus-per-task=" + str(gpus_per_task)]
-    elif gpus_per_task > 0:
-        raise ValueError("GPU binding is only supported for flux and SLURM backend.")
-    if oversubscribe:
-        command_lst += ["--oversubscribe"]
-    command_lst += ["-n", str(cores), "python", path]
-    if enable_flux_backend or enable_slurm_backend or enable_multi_host:
-        command_lst += [
-            "--host",
-            hostname,
-        ]
-    command_lst += [
-        "--zmqport",
-        str(port_selected),
-    ]
-    return command_lst
-
-
 def execute_parallel_tasks(
     future_queue,
     cores,
     gpus_per_task=0,
     oversubscribe=False,
     enable_flux_backend=False,
     enable_slurm_backend=False,
@@ -122,33 +66,28 @@
        oversubscribe (bool): enable of disable the oversubscribe feature of OpenMPI - defaults to False
        enable_flux_backend (bool): enable the flux-framework as backend - defaults to False
        enable_slurm_backend (bool): enable the SLURM queueing system as backend - defaults to False
        cwd (str/None): current working directory where the parallel python task is executed
        queue_adapter (pysqa.queueadapter.QueueAdapter): generalized interface to various queuing systems
        queue_adapter_kwargs (dict/None): keyword arguments for the submit_job() function of the queue adapter
     """
-    interface = SocketInterface(
-        queue_adapter=queue_adapter, queue_adapter_kwargs=queue_adapter_kwargs
-    )
-    interface.bootup(
-        command_lst=command_line_options(
-            hostname=socket.gethostname(),
-            port_selected=interface.bind_to_random_port(),
-            path=os.path.abspath(
-                os.path.join(__file__, "..", "..", "backend", "mpiexec.py")
-            ),
-            cores=cores,
-            gpus_per_task=gpus_per_task,
-            oversubscribe=oversubscribe,
-            enable_flux_backend=enable_flux_backend,
-            enable_slurm_backend=enable_slurm_backend,
-            enable_multi_host=queue_adapter is not None,
-        ),
+    command_lst = [
+        "python",
+        os.path.abspath(os.path.join(__file__, "..", "..", "backend", "mpiexec.py")),
+    ]
+    interface = interface_bootup(
+        command_lst=command_lst,
         cwd=cwd,
         cores=cores,
+        gpus_per_core=gpus_per_task,
+        oversubscribe=oversubscribe,
+        enable_flux_backend=enable_flux_backend,
+        enable_slurm_backend=enable_slurm_backend,
+        queue_adapter=queue_adapter,
+        queue_adapter_kwargs=queue_adapter_kwargs,
     )
     _execute_parallel_tasks_loop(interface=interface, future_queue=future_queue)
 
 
 def _execute_parallel_tasks_loop(interface, future_queue):
     while True:
         task_dict = future_queue.get()
```

### Comparing `pympipool-0.5.8/pympipool/shared/thread.py` & `pympipool-0.6.0/pympipool/shared/thread.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.8/pympipool.egg-info/PKG-INFO` & `pympipool-0.6.0/pympipool.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympipool
-Version: 0.5.8
+Version: 0.6.0
 Summary: pympipool - scale python functions over multiple compute nodes
 Home-page: https://github.com/jan-janssen/pympipool
 Author-email: jan.janssen@outlook.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
@@ -55,15 +55,21 @@
 the executor interface defined by the [`concurrent.futures.Executor`](https://docs.python.org/3/library/concurrent.futures.html#module-concurrent.futures).
 So functions are submitted to the `pympipool.Executor` using the `submit()` function, which returns an 
 [`concurrent.futures.Future`](https://docs.python.org/3/library/concurrent.futures.html#future-objects) object. With 
 these [`concurrent.futures.Future`](https://docs.python.org/3/library/concurrent.futures.html#future-objects) objects 
 asynchronous workflows can be constructed which periodically check if the computation is completed `done()` and then
 query the results using the `result()` function. The limitation of the `pympipool.Executor` is lack of load balancing, 
 each `pympipool.Executor` acts as a serial first in first out (FIFO) queue. So it is the task of the user to balance the
-load of many different tasks over multiple `pympipool.Executor` instances. 
+load of many different tasks over multiple `pympipool.Executor` instances.
+* [`pympipool.HPCExecutor`](https://pympipool.readthedocs.io/en/latest/interfaces.html#hpcexecutor>): To address the 
+limitation of the `pympipool.Executor` that only a single task is executed at any time, the `pympipool.HPCExecutor` 
+provides a wrapper around multiple `pympipool.Executor` objects. It balances the queues of the individual 
+`pympipool.Executor` objects to maximize the throughput for the given resources. This functionality comes with an 
+additional overhead of another thread, acting as a broker between the task queue of the `pympipool.HPCExecutor` and the
+individual `pympipool.Executor` objects. 
 * [`pympipool.PoolExecutor`](https://pympipool.readthedocs.io/en/latest/interfaces.html#poolexecutor): To combine the 
 functionality of the `pympipool.Pool` and the `pympipool.Executor` the `pympipool.PoolExecutor` again connects to the
 [`mpi4py.futures.MPIPoolExecutor`](https://mpi4py.readthedocs.io/en/stable/mpi4py.futures.html#mpipoolexecutor).
 Still in contrast to the `pympipool.Pool` it does not implement the `map()` and `starmap()` functions but rather the 
 `submit()` function based on the [`concurrent.futures.Executor`](https://docs.python.org/3/library/concurrent.futures.html#module-concurrent.futures)
 interface. In this case the load balancing happens internally and the maximum number of workers `max_workers` defines
 the maximum number of parallel tasks. But only serial python tasks can be executed in contrast to the `pympipool.Executor`
@@ -93,21 +99,24 @@
 # Documentation
 * [Installation](https://pympipool.readthedocs.io/en/latest/installation.html) 
   * [pypi-based installation](https://pympipool.readthedocs.io/en/latest/installation.html#pypi-based-installation)
   * [conda-based installation](https://pympipool.readthedocs.io/en/latest/installation.html#conda-based-installation)
 * [Interfaces](https://pympipool.readthedocs.io/en/latest/interfaces.html) 
   * [Pool](https://pympipool.readthedocs.io/en/latest/interfaces.html#pool)
   * [Executor](https://pympipool.readthedocs.io/en/latest/interfaces.html#executor)
+  * [HPCExecutor](https://pympipool.readthedocs.io/en/latest/interfaces.html#hpcexecutor>)
   * [ParallelExecutor](https://pympipool.readthedocs.io/en/latest/interfaces.html#poolexecutor)
   * [MPISpawnPool](https://pympipool.readthedocs.io/en/latest/interfaces.html#mpispawnpool)
   * [SocketInterface](https://pympipool.readthedocs.io/en/latest/interfaces.html#socketinterface)
 * [Development](https://pympipool.readthedocs.io/en/latest/development.html) 
 
 # License
-`pympipool` is released under the BSD license https://github.com/pyiron/pympipool/blob/main/LICENSE . It is a spin-off of the `pyiron` project https://github.com/pyiron/pyiron therefore if you use `pympipool` for calculation which result in a scientific publication, please cite: 
+`pympipool` is released under the BSD license https://github.com/pyiron/pympipool/blob/main/LICENSE . It is a spin-off 
+of the `pyiron` project https://github.com/pyiron/pyiron therefore if you use `pympipool` for calculation which result 
+in a scientific publication, please cite: 
 
     @article{pyiron-paper,
       title = {pyiron: An integrated development environment for computational materials science},
       journal = {Computational Materials Science},
       volume = {163},
       pages = {24 - 36},
       year = {2019},
```

### Comparing `pympipool-0.5.8/pympipool.egg-info/SOURCES.txt` & `pympipool-0.6.0/pympipool.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -25,23 +25,26 @@
 pympipool/legacy/shared/__init__.py
 pympipool/legacy/shared/backend.py
 pympipool/legacy/shared/interface.py
 pympipool/shared/__init__.py
 pympipool/shared/backend.py
 pympipool/shared/broker.py
 pympipool/shared/communication.py
+pympipool/shared/connections.py
 pympipool/shared/taskexecutor.py
 pympipool/shared/thread.py
 tests/test_communicator_split.py
+tests/test_connection.py
 tests/test_executor.py
 tests/test_future.py
 tests/test_interface.py
 tests/test_meta.py
 tests/test_multitask.py
 tests/test_parse.py
 tests/test_parse_legacy.py
 tests/test_pool.py
 tests/test_queue.py
 tests/test_task.py
+tests/test_thread.py
 tests/test_worker.py
 tests/test_worker_memory.py
 tests/test_zmq.py
```

### Comparing `pympipool-0.5.8/setup.py` & `pympipool-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.8/tests/test_communicator_split.py` & `pympipool-0.6.0/tests/test_communicator_split.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.8/tests/test_executor.py` & `pympipool-0.6.0/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.8/tests/test_future.py` & `pympipool-0.6.0/tests/test_future.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.8/tests/test_interface.py` & `pympipool-0.6.0/tests/test_interface.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import os
-import socket
 
 import numpy as np
 import unittest
 from pympipool.shared.communication import SocketInterface
-from pympipool.shared.taskexecutor import command_line_options, cloudpickle_register
+from pympipool.shared.taskexecutor import cloudpickle_register
+from pympipool.shared.connections import MpiExecInterface
 
 
 def calc(i):
     return np.array(i ** 2)
 
 
 class TestInterface(unittest.TestCase):
     def test_interface(self):
         cloudpickle_register(ind=1)
         task_dict = {"fn": calc, 'args': (), "kwargs": {"i": 2}}
-        interface = SocketInterface(queue_adapter=None, queue_adapter_kwargs=None)
-        interface.bootup(
-            command_lst=command_line_options(
-                hostname=socket.gethostname(),
-                port_selected=interface.bind_to_random_port(),
-                path=os.path.abspath(os.path.join(__file__, "..", "..", "pympipool", "backend", "mpiexec.py")),
+        interface = SocketInterface(
+            interface=MpiExecInterface(
+                cwd=None,
                 cores=1,
-                gpus_per_task=0,
-                oversubscribe=False,
-                enable_flux_backend=False,
-                enable_slurm_backend=False,
-                enable_multi_host=False,
+                gpus_per_core=0,
+                oversubscribe=False
             )
         )
+        interface.bootup(command_lst=[
+            "python",
+            os.path.abspath(os.path.join(__file__, "..", "..", "pympipool", "backend", "mpiexec.py")),
+            "--zmqport",
+            str(interface.bind_to_random_port()),
+        ])
         self.assertEqual(interface.send_and_receive_dict(input_dict=task_dict), np.array(4))
         interface.shutdown(wait=True)
```

### Comparing `pympipool-0.5.8/tests/test_meta.py` & `pympipool-0.6.0/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.8/tests/test_multitask.py` & `pympipool-0.6.0/tests/test_multitask.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.8/tests/test_parse_legacy.py` & `pympipool-0.6.0/tests/test_parse_legacy.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,74 @@
 import unittest
+import os
 from pympipool.legacy.shared.backend import parse_arguments
-from pympipool.legacy.shared.interface import command_line_options
+from pympipool.shared.connections import MpiExecInterface, FluxCmdInterface
 
 
 class TestParser(unittest.TestCase):
     def test_command_local(self):
         result_dict = {
             'host': 'localhost',
             'total_cores': '2',
             'zmqport': '22',
             'cores_per_task': '1'
         }
         command_lst = [
-            'mpiexec', '--oversubscribe',
+            'mpiexec',
             '-n', result_dict['total_cores'],
+            '--oversubscribe',
             'python', '-m', 'mpi4py.futures', '/',
             '--zmqport', result_dict['zmqport'],
             '--cores-per-task', result_dict['cores_per_task'],
             '--cores-total', result_dict['total_cores']
         ]
-        self.assertEqual(command_lst, command_line_options(
-            hostname=result_dict['host'],
-            port_selected=result_dict['zmqport'],
-            path="/",
-            cores=int(result_dict['total_cores']),
-            cores_per_task=int(result_dict['cores_per_task']),
-            oversubscribe=True,
-            enable_flux_backend=False,
-        ))
+        interface = MpiExecInterface(
+            cwd=None,
+            cores=2,
+            gpus_per_core=0,
+            oversubscribe=True
+        )
+        self.assertEqual(
+            command_lst,
+            interface.generate_command(
+                command_lst=[
+                    'python', '-m', 'mpi4py.futures', '/',
+                    '--zmqport', result_dict['zmqport'],
+                    '--cores-per-task', '1', '--cores-total', '2'
+                ]
+            )
+        )
         self.assertEqual(result_dict, parse_arguments(command_lst))
 
     def test_command_flux(self):
         result_dict = {
             'host': "127.0.0.1",
             'total_cores': '2',
             'zmqport': '22',
             'cores_per_task': '2'
         }
         command_lst = [
-            'flux', 'run', '-n', '1', 'python', '/',
+            'flux', 'run', '-n', '1',
+            "--cwd=" + os.path.abspath("."),
+            'python', '/',
             '--host', result_dict['host'],
             '--zmqport', result_dict['zmqport'],
             '--cores-per-task', result_dict['cores_per_task'],
             '--cores-total', result_dict['total_cores']
         ]
-        self.assertEqual(command_lst, command_line_options(
-            hostname=result_dict['host'],
-            port_selected=result_dict['zmqport'],
-            path="/",
-            cores=int(result_dict['total_cores']),
-            cores_per_task=int(result_dict['cores_per_task']),
-            oversubscribe=False,
-            enable_flux_backend=True,
-        ))
+        interface = FluxCmdInterface(
+            cwd=os.path.abspath("."),
+            cores=1,
+            gpus_per_core=0,
+            oversubscribe=False
+        )
+        self.assertEqual(
+            command_lst,
+            interface.generate_command(
+                command_lst=[
+                    'python', '/', '--host', result_dict['host'],
+                    '--zmqport', result_dict['zmqport'],
+                    '--cores-per-task', '2', '--cores-total', '2'
+                ]
+            )
+        )
         self.assertEqual(result_dict, parse_arguments(command_lst))
```

### Comparing `pympipool-0.5.8/tests/test_pool.py` & `pympipool-0.6.0/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.8/tests/test_queue.py` & `pympipool-0.6.0/tests/test_queue.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.8/tests/test_task.py` & `pympipool-0.6.0/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.8/tests/test_worker.py` & `pympipool-0.6.0/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.8/tests/test_worker_memory.py` & `pympipool-0.6.0/tests/test_worker_memory.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.8/versioneer.py` & `pympipool-0.6.0/versioneer.py`

 * *Files identical despite different names*

