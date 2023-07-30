# Comparing `tmp/python-logstash-async-2.5.0.tar.gz` & `tmp/python-logstash-async-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-logstash-async-2.5.0.tar", last modified: Sat Apr 16 08:36:04 2022, max compression
+gzip compressed data, was "python-logstash-async-2.6.0.tar", last modified: Sun Jul 30 14:34:36 2023, max compression
```

## Comparing `python-logstash-async-2.5.0.tar` & `python-logstash-async-2.6.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2022-04-16 08:36:04.655058 python-logstash-async-2.5.0/
--rw-r--r--   0 enrico    (1000) enrico    (1000)     1120 2019-11-12 21:49:57.000000 python-logstash-async-2.5.0/LICENSE
--rw-r--r--   0 enrico    (1000) enrico    (1000)      181 2016-12-31 11:55:15.000000 python-logstash-async-2.5.0/MANIFEST.in
--rw-r--r--   0 enrico    (1000) enrico    (1000)     3258 2022-04-16 08:36:04.655058 python-logstash-async-2.5.0/PKG-INFO
--rw-r--r--   0 enrico    (1000) enrico    (1000)     2272 2021-10-24 14:47:50.000000 python-logstash-async-2.5.0/README.rst
-drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2022-04-16 08:36:04.651058 python-logstash-async-2.5.0/docs/
--rw-r--r--   0 enrico    (1000) enrico    (1000)      622 2019-09-29 17:33:17.000000 python-logstash-async-2.5.0/docs/Makefile
--rw-r--r--   0 enrico    (1000) enrico    (1000)     8742 2022-04-16 08:32:58.000000 python-logstash-async-2.5.0/docs/about.rst
--rw-r--r--   0 enrico    (1000) enrico    (1000)     4918 2019-01-05 12:54:22.000000 python-logstash-async-2.5.0/docs/conf.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)    10199 2022-04-02 15:59:27.000000 python-logstash-async-2.5.0/docs/config.rst
--rw-r--r--   0 enrico    (1000) enrico    (1000)     1543 2020-10-03 12:25:27.000000 python-logstash-async-2.5.0/docs/config_logstash.rst
--rw-r--r--   0 enrico    (1000) enrico    (1000)      890 2019-01-05 14:36:07.000000 python-logstash-async-2.5.0/docs/index.rst
--rw-r--r--   0 enrico    (1000) enrico    (1000)      254 2016-12-25 23:40:02.000000 python-logstash-async-2.5.0/docs/installation.rst
--rw-r--r--   0 enrico    (1000) enrico    (1000)     1364 2018-12-31 14:58:27.000000 python-logstash-async-2.5.0/docs/persistence.rst
--rw-r--r--   0 enrico    (1000) enrico    (1000)    11894 2020-12-05 10:27:00.000000 python-logstash-async-2.5.0/docs/usage.rst
--rw-r--r--   0 enrico    (1000) enrico    (1000)     1081 2017-10-21 12:25:31.000000 python-logstash-async-2.5.0/example1.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)     1186 2017-10-21 12:25:31.000000 python-logstash-async-2.5.0/example2.py
-drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2022-04-16 08:36:04.655058 python-logstash-async-2.5.0/logstash_async/
--rw-r--r--   0 enrico    (1000) enrico    (1000)      302 2022-04-16 08:34:35.000000 python-logstash-async-2.5.0/logstash_async/__init__.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)     1798 2020-08-16 16:59:24.000000 python-logstash-async-2.5.0/logstash_async/cache.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)     2782 2020-11-03 23:28:22.000000 python-logstash-async-2.5.0/logstash_async/constants.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)     5931 2022-04-16 08:27:34.000000 python-logstash-async-2.5.0/logstash_async/database.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)    14295 2022-04-03 08:31:39.000000 python-logstash-async-2.5.0/logstash_async/formatter.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)     8891 2021-10-24 13:10:35.000000 python-logstash-async-2.5.0/logstash_async/handler.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)     3703 2021-10-24 13:08:47.000000 python-logstash-async-2.5.0/logstash_async/memory_cache.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)    12669 2021-05-16 14:53:21.000000 python-logstash-async-2.5.0/logstash_async/transport.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)     2147 2021-10-24 13:10:06.000000 python-logstash-async-2.5.0/logstash_async/utils.py
--rw-r--r--   0 enrico    (1000) enrico    (1000)    14183 2022-04-16 08:26:37.000000 python-logstash-async-2.5.0/logstash_async/worker.py
-drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2022-04-16 08:36:04.655058 python-logstash-async-2.5.0/python_logstash_async.egg-info/
--rw-r--r--   0 enrico    (1000) enrico    (1000)     3258 2022-04-16 08:36:04.000000 python-logstash-async-2.5.0/python_logstash_async.egg-info/PKG-INFO
--rw-r--r--   0 enrico    (1000) enrico    (1000)      721 2022-04-16 08:36:04.000000 python-logstash-async-2.5.0/python_logstash_async.egg-info/SOURCES.txt
--rw-r--r--   0 enrico    (1000) enrico    (1000)        1 2022-04-16 08:36:04.000000 python-logstash-async-2.5.0/python_logstash_async.egg-info/dependency_links.txt
--rw-r--r--   0 enrico    (1000) enrico    (1000)       26 2022-04-16 08:36:04.000000 python-logstash-async-2.5.0/python_logstash_async.egg-info/requires.txt
--rw-r--r--   0 enrico    (1000) enrico    (1000)       15 2022-04-16 08:36:04.000000 python-logstash-async-2.5.0/python_logstash_async.egg-info/top_level.txt
--rw-r--r--   0 enrico    (1000) enrico    (1000)     1277 2022-04-16 08:36:04.655058 python-logstash-async-2.5.0/setup.cfg
--rw-r--r--   0 enrico    (1000) enrico    (1000)     1980 2022-04-16 08:34:20.000000 python-logstash-async-2.5.0/setup.py
+drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-07-30 14:34:36.679560 python-logstash-async-2.6.0/
+-rw-r--r--   0 enrico    (1000) enrico    (1000)     1120 2019-11-12 21:49:57.000000 python-logstash-async-2.6.0/LICENSE
+-rw-r--r--   0 enrico    (1000) enrico    (1000)      181 2016-12-31 11:55:15.000000 python-logstash-async-2.6.0/MANIFEST.in
+-rw-r--r--   0 enrico    (1000) enrico    (1000)     3238 2023-07-30 14:34:36.679560 python-logstash-async-2.6.0/PKG-INFO
+-rw-r--r--   0 enrico    (1000) enrico    (1000)     2272 2021-10-24 14:47:50.000000 python-logstash-async-2.6.0/README.rst
+drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-07-30 14:34:36.679560 python-logstash-async-2.6.0/docs/
+-rw-r--r--   0 enrico    (1000) enrico    (1000)      622 2019-09-29 17:33:17.000000 python-logstash-async-2.6.0/docs/Makefile
+-rw-r--r--   0 enrico    (1000) enrico    (1000)     8926 2023-07-30 14:33:01.000000 python-logstash-async-2.6.0/docs/about.rst
+-rw-r--r--   0 enrico    (1000) enrico    (1000)     4918 2023-07-30 12:25:08.000000 python-logstash-async-2.6.0/docs/conf.py
+-rw-r--r--   0 enrico    (1000) enrico    (1000)    10199 2022-04-02 15:59:27.000000 python-logstash-async-2.6.0/docs/config.rst
+-rw-r--r--   0 enrico    (1000) enrico    (1000)     1543 2020-10-03 12:25:27.000000 python-logstash-async-2.6.0/docs/config_logstash.rst
+-rw-r--r--   0 enrico    (1000) enrico    (1000)      890 2019-01-05 14:36:07.000000 python-logstash-async-2.6.0/docs/index.rst
+-rw-r--r--   0 enrico    (1000) enrico    (1000)      254 2016-12-25 23:40:02.000000 python-logstash-async-2.6.0/docs/installation.rst
+-rw-r--r--   0 enrico    (1000) enrico    (1000)     1364 2018-12-31 14:58:27.000000 python-logstash-async-2.6.0/docs/persistence.rst
+-rw-r--r--   0 enrico    (1000) enrico    (1000)    11894 2020-12-05 10:27:00.000000 python-logstash-async-2.6.0/docs/usage.rst
+-rw-r--r--   0 enrico    (1000) enrico    (1000)     1081 2017-10-21 12:25:31.000000 python-logstash-async-2.6.0/example1.py
+-rw-r--r--   0 enrico    (1000) enrico    (1000)     1186 2017-10-21 12:25:31.000000 python-logstash-async-2.6.0/example2.py
+drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-07-30 14:34:36.679560 python-logstash-async-2.6.0/logstash_async/
+-rw-r--r--   0 enrico    (1000) enrico    (1000)      302 2023-07-30 14:33:23.000000 python-logstash-async-2.6.0/logstash_async/__init__.py
+-rw-r--r--   0 enrico    (1000) enrico    (1000)     1798 2020-08-16 16:59:24.000000 python-logstash-async-2.6.0/logstash_async/cache.py
+-rw-r--r--   0 enrico    (1000) enrico    (1000)     2782 2023-07-30 12:44:28.000000 python-logstash-async-2.6.0/logstash_async/constants.py
+-rw-r--r--   0 enrico    (1000) enrico    (1000)     5931 2022-04-16 08:27:34.000000 python-logstash-async-2.6.0/logstash_async/database.py
+-rw-r--r--   0 enrico    (1000) enrico    (1000)    14295 2022-04-03 08:31:39.000000 python-logstash-async-2.6.0/logstash_async/formatter.py
+-rw-r--r--   0 enrico    (1000) enrico    (1000)     8891 2023-07-30 12:29:25.000000 python-logstash-async-2.6.0/logstash_async/handler.py
+-rw-r--r--   0 enrico    (1000) enrico    (1000)     3703 2021-10-24 13:08:47.000000 python-logstash-async-2.6.0/logstash_async/memory_cache.py
+-rw-r--r--   0 enrico    (1000) enrico    (1000)    12722 2023-07-30 13:43:37.000000 python-logstash-async-2.6.0/logstash_async/transport.py
+-rw-r--r--   0 enrico    (1000) enrico    (1000)     2147 2021-10-24 13:10:06.000000 python-logstash-async-2.6.0/logstash_async/utils.py
+-rw-r--r--   0 enrico    (1000) enrico    (1000)    14512 2023-07-30 12:25:08.000000 python-logstash-async-2.6.0/logstash_async/worker.py
+drwxr-xr-x   0 enrico    (1000) enrico    (1000)        0 2023-07-30 14:34:36.679560 python-logstash-async-2.6.0/python_logstash_async.egg-info/
+-rw-r--r--   0 enrico    (1000) enrico    (1000)     3238 2023-07-30 14:34:36.000000 python-logstash-async-2.6.0/python_logstash_async.egg-info/PKG-INFO
+-rw-r--r--   0 enrico    (1000) enrico    (1000)      721 2023-07-30 14:34:36.000000 python-logstash-async-2.6.0/python_logstash_async.egg-info/SOURCES.txt
+-rw-r--r--   0 enrico    (1000) enrico    (1000)        1 2023-07-30 14:34:36.000000 python-logstash-async-2.6.0/python_logstash_async.egg-info/dependency_links.txt
+-rw-r--r--   0 enrico    (1000) enrico    (1000)       26 2023-07-30 14:34:36.000000 python-logstash-async-2.6.0/python_logstash_async.egg-info/requires.txt
+-rw-r--r--   0 enrico    (1000) enrico    (1000)       15 2023-07-30 14:34:36.000000 python-logstash-async-2.6.0/python_logstash_async.egg-info/top_level.txt
+-rw-r--r--   0 enrico    (1000) enrico    (1000)     1350 2023-07-30 14:34:36.683560 python-logstash-async-2.6.0/setup.cfg
+-rw-r--r--   0 enrico    (1000) enrico    (1000)     1980 2023-07-30 14:33:17.000000 python-logstash-async-2.6.0/setup.py
```

### Comparing `python-logstash-async-2.5.0/LICENSE` & `python-logstash-async-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-logstash-async-2.5.0/PKG-INFO` & `python-logstash-async-2.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: python-logstash-async
-Version: 2.5.0
+Version: 2.6.0
 Summary: Asynchronous Python logging handler for Logstash.
 Home-page: https://github.com/eht16/python-logstash-async
 Author: Enrico Tröger
 Author-email: enrico.troeger@uvena.de
 License: MIT
 Project-URL: Source code, https://github.com/eht16/python-logstash-async/
 Project-URL: Documentation, https://python-logstash-async.readthedocs.io/en/stable/
 Keywords: logging logstash asynchronous
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP
@@ -90,9 +89,7 @@
 https://github.com/eht16/python-logstash-async/issues.
 
 
 Author
 ------
 
 Enrico Tröger <enrico.troeger@uvena.de>
-
-
```

### Comparing `python-logstash-async-2.5.0/README.rst` & `python-logstash-async-2.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-logstash-async-2.5.0/docs/Makefile` & `python-logstash-async-2.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python-logstash-async-2.5.0/docs/about.rst` & `python-logstash-async-2.6.0/docs/about.rst`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,21 @@
 .. literalinclude:: ../LICENSE
     :language: none
 
 
 ChangeLog
 ---------
 
+2.6.0 (Jul 30 2023)
++++++++++++++++++++
+
+  * Load certificate chain only if a certificate was specified (#79).
+  * Handle network errors raised by "requests" in HttpTransport (#75).
+
+
 2.5.0 (Apr 16 2022)
 +++++++++++++++++++
 
   * Handle database disk errors (#72, Peter Mazarovich).
   * Use Python's PriorityQueue to reduce memory consumption
     (#73, Peter Mazarovich).
```

### Comparing `python-logstash-async-2.5.0/docs/conf.py` & `python-logstash-async-2.6.0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = 'en'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 # The name of the Pygments (syntax highlighting) style to use.
```

### Comparing `python-logstash-async-2.5.0/docs/config.rst` & `python-logstash-async-2.6.0/docs/config.rst`

 * *Files identical despite different names*

### Comparing `python-logstash-async-2.5.0/docs/config_logstash.rst` & `python-logstash-async-2.6.0/docs/config_logstash.rst`

 * *Files identical despite different names*

### Comparing `python-logstash-async-2.5.0/docs/index.rst` & `python-logstash-async-2.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python-logstash-async-2.5.0/docs/persistence.rst` & `python-logstash-async-2.6.0/docs/persistence.rst`

 * *Files identical despite different names*

### Comparing `python-logstash-async-2.5.0/docs/usage.rst` & `python-logstash-async-2.6.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `python-logstash-async-2.5.0/example1.py` & `python-logstash-async-2.6.0/example1.py`

 * *Files identical despite different names*

### Comparing `python-logstash-async-2.5.0/example2.py` & `python-logstash-async-2.6.0/example2.py`

 * *Files identical despite different names*

### Comparing `python-logstash-async-2.5.0/logstash_async/cache.py` & `python-logstash-async-2.6.0/logstash_async/cache.py`

 * *Files identical despite different names*

### Comparing `python-logstash-async-2.5.0/logstash_async/constants.py` & `python-logstash-async-2.6.0/logstash_async/constants.py`

 * *Files identical despite different names*

### Comparing `python-logstash-async-2.5.0/logstash_async/database.py` & `python-logstash-async-2.6.0/logstash_async/database.py`

 * *Files identical despite different names*

### Comparing `python-logstash-async-2.5.0/logstash_async/formatter.py` & `python-logstash-async-2.6.0/logstash_async/formatter.py`

 * *Files identical despite different names*

### Comparing `python-logstash-async-2.5.0/logstash_async/handler.py` & `python-logstash-async-2.6.0/logstash_async/handler.py`

 * *Files identical despite different names*

### Comparing `python-logstash-async-2.5.0/logstash_async/memory_cache.py` & `python-logstash-async-2.6.0/logstash_async/memory_cache.py`

 * *Files identical despite different names*

### Comparing `python-logstash-async-2.5.0/logstash_async/transport.py` & `python-logstash-async-2.6.0/logstash_async/transport.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,17 +172,18 @@
             ssl_context = ssl.create_default_context(cafile=self._ca_certs)
             if not self._ssl_verify:
                 if self._ca_certs:
                     cert_reqs = ssl.CERT_OPTIONAL
                 else:
                     cert_reqs = ssl.CERT_NONE
 
-            ssl_context.verify_mode = cert_reqs
             ssl_context.check_hostname = False
-            ssl_context.load_cert_chain(self._certfile, self._keyfile)
+            ssl_context.verify_mode = cert_reqs
+            if self._certfile and self._keyfile:
+                ssl_context.load_cert_chain(self._certfile, self._keyfile)
             self._sock = ssl_context.wrap_socket(self._sock, server_side=False)
         except socket.error:
             self._close()
             raise
 
     # ----------------------------------------------------------------------
     def _send_via_socket(self, data):
```

### Comparing `python-logstash-async-2.5.0/logstash_async/utils.py` & `python-logstash-async-2.6.0/logstash_async/utils.py`

 * *Files identical despite different names*

### Comparing `python-logstash-async-2.5.0/logstash_async/worker.py` & `python-logstash-async-2.6.0/logstash_async/worker.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,21 +8,38 @@
 from queue import Empty, PriorityQueue
 from socket import gaierror as socket_gaierror
 from threading import Event, Thread
 
 from limits import parse as parse_rate_limit
 from limits.storage import MemoryStorage
 from limits.strategies import FixedWindowRateLimiter
+from requests.exceptions import ConnectionError as RequestsConnectionError
+from requests.exceptions import ConnectTimeout, HTTPError, ProxyError, RetryError, Timeout
 
 from logstash_async.constants import constants
 from logstash_async.database import DatabaseCache, DatabaseDiskIOError, DatabaseLockedError
 from logstash_async.memory_cache import MemoryCache
 from logstash_async.utils import safe_log_via_print
 
 
+NETWORK_EXCEPTIONS = (
+    # Python
+    ConnectionError,
+    TimeoutError,
+    socket_gaierror,
+    # Requests
+    ConnectTimeout,
+    RequestsConnectionError,
+    HTTPError,
+    ProxyError,
+    RetryError,
+    Timeout,
+)
+
+
 class ProcessingError(Exception):
     """"""
 
 
 class LogProcessingWorker(Thread):  # pylint: disable=too-many-instance-attributes
     """"""
 
@@ -216,15 +233,15 @@
             if not queued_events:
                 break
 
             try:
                 events = [event['event_text'] for event in queued_events]
                 self._send_events(events)
             # Log connection and network errors as warnings as they are rather harmless
-            except (ConnectionError, TimeoutError, socket_gaierror) as exc:
+            except NETWORK_EXCEPTIONS as exc:
                 self._safe_log(
                     'warning',
                     'An error occurred while sending events: %s',
                     exc)
                 self._database.requeue_queued_events(queued_events)
                 break
             except Exception as exc:
@@ -313,15 +330,15 @@
             # increase the rate limit counter for the key
             self._rate_limit_strategy.hit(self._rate_limit_item, key)
             return remaining
 
         return 2  # any value greater than 1 means allowed
 
     # ----------------------------------------------------------------------
-    def _factor_rate_limit_key(self, exc):  # pylint: disable=no-self-use
+    def _factor_rate_limit_key(self, exc):
         module_name = getattr(exc, '__module__', '__no_module__')
         class_name = exc.__class__.__name__
         key_items = [module_name, class_name]
         if hasattr(exc, 'errno') and isinstance(exc.errno, int):
             # in case of socket.error, include the errno as rate limiting key
             key_items.append(str(exc.errno))
         return '.'.join(key_items)
```

### Comparing `python-logstash-async-2.5.0/python_logstash_async.egg-info/PKG-INFO` & `python-logstash-async-2.6.0/python_logstash_async.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: python-logstash-async
-Version: 2.5.0
+Version: 2.6.0
 Summary: Asynchronous Python logging handler for Logstash.
 Home-page: https://github.com/eht16/python-logstash-async
 Author: Enrico Tröger
 Author-email: enrico.troeger@uvena.de
 License: MIT
 Project-URL: Source code, https://github.com/eht16/python-logstash-async/
 Project-URL: Documentation, https://python-logstash-async.readthedocs.io/en/stable/
 Keywords: logging logstash asynchronous
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP
@@ -90,9 +89,7 @@
 https://github.com/eht16/python-logstash-async/issues.
 
 
 Author
 ------
 
 Enrico Tröger <enrico.troeger@uvena.de>
-
-
```

### Comparing `python-logstash-async-2.5.0/python_logstash_async.egg-info/SOURCES.txt` & `python-logstash-async-2.6.0/python_logstash_async.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-logstash-async-2.5.0/setup.py` & `python-logstash-async-2.6.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from os import path
 from setuptools import setup
 from shutil import rmtree
 import sys
 
 NAME = 'python-logstash-async'
-VERSION = '2.5.0'
+VERSION = '2.6.0'
 
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.rst'), 'rb') as f:
     LONG_DESCRIPTION = f.read().decode('utf-8')
 
 
 if 'bdist_wheel' in sys.argv:
```

