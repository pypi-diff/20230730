# Comparing `tmp/hibp_downloader-0.1.1.tar.gz` & `tmp/hibp_downloader-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hibp_downloader-0.1.1.tar", max compression
+gzip compressed data, was "hibp_downloader-0.1.2.tar", max compression
```

## Comparing `hibp_downloader-0.1.1.tar` & `hibp_downloader-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1565 2023-07-26 04:14:23.983439 hibp_downloader-0.1.1/LICENSE
--rw-r--r--   0        0        0     2532 2023-07-30 14:07:43.989599 hibp_downloader-0.1.1/README.md
--rw-r--r--   0        0        0     2963 2023-07-30 14:42:58.593629 hibp_downloader-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1548 2023-07-30 14:09:50.191095 hibp_downloader-0.1.1/src/hibp_downloader/__init__.py
--rw-r--r--   0        0        0    10806 2023-07-30 11:09:59.800056 hibp_downloader-0.1.1/src/hibp_downloader/commands/hibp_download.py
--rw-r--r--   0        0        0     3813 2023-07-30 11:12:13.966653 hibp_downloader-0.1.1/src/hibp_downloader/commands/hibp_generate.py
--rw-r--r--   0        0        0      568 2023-07-26 04:18:19.902342 hibp_downloader-0.1.1/src/hibp_downloader/exceptions.py
--rw-r--r--   0        0        0     4268 2023-07-30 12:12:56.451940 hibp_downloader-0.1.1/src/hibp_downloader/lib/app.py
--rw-r--r--   0        0        0     3741 2023-07-30 13:34:36.549050 hibp_downloader-0.1.1/src/hibp_downloader/lib/filedata.py
--rw-r--r--   0        0        0      657 2023-07-29 09:39:32.590020 hibp_downloader-0.1.1/src/hibp_downloader/lib/generators.py
--rw-r--r--   0        0        0     1858 2023-07-30 07:01:44.988273 hibp_downloader-0.1.1/src/hibp_downloader/lib/http.py
--rw-r--r--   0        0        0     3281 2023-07-30 13:34:36.552050 hibp_downloader-0.1.1/src/hibp_downloader/lib/logger.py
--rw-r--r--   0        0        0     1285 2023-07-30 06:49:39.677165 hibp_downloader-0.1.1/src/hibp_downloader/main.py
--rw-r--r--   0        0        0      214 2023-07-30 03:31:02.403390 hibp_downloader-0.1.1/src/hibp_downloader/models/__init__.py
--rw-r--r--   0        0        0      395 2023-07-30 13:34:36.556051 hibp_downloader-0.1.1/src/hibp_downloader/models/app_context.py
--rw-r--r--   0        0        0       87 2023-07-29 11:47:32.763631 hibp_downloader-0.1.1/src/hibp_downloader/models/hash_type.py
--rw-r--r--   0        0        0     1829 2023-07-30 13:34:36.559051 hibp_downloader-0.1.1/src/hibp_downloader/models/prefix_metadata.py
--rw-r--r--   0        0        0     5456 2023-07-30 13:34:36.562051 hibp_downloader-0.1.1/src/hibp_downloader/models/stats.py
--rw-r--r--   0        0        0        0 2023-07-26 00:51:50.083564 hibp_downloader-0.1.1/src/hibp_downloader/py.typed
--rw-r--r--   0        0        0     3804 1970-01-01 00:00:00.000000 hibp_downloader-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1565 2023-07-26 04:14:23.983439 hibp_downloader-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2597 2023-07-30 15:00:09.957823 hibp_downloader-0.1.2/README.md
+-rw-r--r--   0        0        0     2937 2023-07-30 15:00:09.963823 hibp_downloader-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1548 2023-07-30 15:00:09.975823 hibp_downloader-0.1.2/src/hibp_downloader/__init__.py
+-rw-r--r--   0        0        0    10806 2023-07-30 11:09:59.800056 hibp_downloader-0.1.2/src/hibp_downloader/commands/hibp_download.py
+-rw-r--r--   0        0        0     3813 2023-07-30 11:12:13.966653 hibp_downloader-0.1.2/src/hibp_downloader/commands/hibp_generate.py
+-rw-r--r--   0        0        0      568 2023-07-26 04:18:19.902342 hibp_downloader-0.1.2/src/hibp_downloader/exceptions.py
+-rw-r--r--   0        0        0     4268 2023-07-30 12:12:56.451940 hibp_downloader-0.1.2/src/hibp_downloader/lib/app.py
+-rw-r--r--   0        0        0     3741 2023-07-30 13:34:36.549050 hibp_downloader-0.1.2/src/hibp_downloader/lib/filedata.py
+-rw-r--r--   0        0        0      657 2023-07-29 09:39:32.590020 hibp_downloader-0.1.2/src/hibp_downloader/lib/generators.py
+-rw-r--r--   0        0        0     1858 2023-07-30 07:01:44.988273 hibp_downloader-0.1.2/src/hibp_downloader/lib/http.py
+-rw-r--r--   0        0        0     3281 2023-07-30 13:34:36.552050 hibp_downloader-0.1.2/src/hibp_downloader/lib/logger.py
+-rw-r--r--   0        0        0     1285 2023-07-30 06:49:39.677165 hibp_downloader-0.1.2/src/hibp_downloader/main.py
+-rw-r--r--   0        0        0      214 2023-07-30 03:31:02.403390 hibp_downloader-0.1.2/src/hibp_downloader/models/__init__.py
+-rw-r--r--   0        0        0      395 2023-07-30 13:34:36.556051 hibp_downloader-0.1.2/src/hibp_downloader/models/app_context.py
+-rw-r--r--   0        0        0       87 2023-07-29 11:47:32.763631 hibp_downloader-0.1.2/src/hibp_downloader/models/hash_type.py
+-rw-r--r--   0        0        0     1829 2023-07-30 13:34:36.559051 hibp_downloader-0.1.2/src/hibp_downloader/models/prefix_metadata.py
+-rw-r--r--   0        0        0     5456 2023-07-30 13:34:36.562051 hibp_downloader-0.1.2/src/hibp_downloader/models/stats.py
+-rw-r--r--   0        0        0        0 2023-07-26 00:51:50.083564 hibp_downloader-0.1.2/src/hibp_downloader/py.typed
+-rw-r--r--   0        0        0     3843 1970-01-01 00:00:00.000000 hibp_downloader-0.1.2/PKG-INFO
```

### Comparing `hibp_downloader-0.1.1/LICENSE` & `hibp_downloader-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hibp_downloader-0.1.1/README.md` & `hibp_downloader-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 ## Install
 ```commandline
 pip install --upgrade hibp-downloader
 ```
 
 ## Usage
-![screenshot-help.png](docs%2Fassets%2Fscreenshot-help.png)
+![screenshot-help.png](https://raw.githubusercontent.com/threatpatrols/hibp-downloader/main/docs/assets/screenshot-help.png)
 
 ## Runtime Logs
 Sample download activity logs 
 ```text
 2023-07-30T21:42:06+1000 | INFO | hibp-downloader | prefix=65747 source=[lc:207328 et:0 rc:56672 ro:0 xx:0] runtime_rate=[10.3MBit/s 79req/s ~65602H/s] runtime=0.2hr download=922.5MB
 2023-07-30T21:42:07+1000 | INFO | hibp-downloader | prefix=29da7 source=[lc:207328 et:0 rc:56792 ro:0 xx:0] runtime_rate=[10.4MBit/s 79req/s ~65646H/s] runtime=0.2hr download=924.5MB
 2023-07-30T21:42:09+1000 | INFO | hibp-downloader | prefix=43c7f source=[lc:207328 et:0 rc:56912 ro:0 xx:0] runtime_rate=[10.3MBit/s 79req/s ~65617H/s] runtime=0.2hr download=926.5MB
```

### Comparing `hibp_downloader-0.1.1/pyproject.toml` & `hibp_downloader-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hibp-downloader"
-version = "0.1.1"
-description = "Efficiently download new data for a local-copy of the pwned password hashes from api[.]pwnedpasswords[.]com"
+version = "0.1.2"
+description = "Efficiently download HIBP new pwned password data by hash-prefix for a local-copy"
 authors = ["Nicholas de Jong <contact@threatpatrols.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 packages = [{ include = "hibp_downloader", from = "src" }]
 classifiers = [
     "Environment :: Console",
     "Intended Audience :: System Administrators",
```

### Comparing `hibp_downloader-0.1.1/src/hibp_downloader/__init__.py` & `hibp_downloader-0.1.2/src/hibp_downloader/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from os import cpu_count, getenv
 from sys import argv
 
 from .lib.logger import logger_get
 from .models import AppContext
 
 __title__ = "HIBP Downloader"
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __logger_name__ = "hibp-downloader"
 __pwnedpasswords_api_url__ = "https://api.pwnedpasswords.com"
 __local_cache_ttl_default__ = 86400
 __multiprocessing_processes_default__ = cpu_count()
 __multiprocessing_prefixes_chunk_size__ = cpu_count() * 2
 __approx_gzip_bytes_per_hash__ = 20.674
 __logging_info_event_modulus__ = 5
```

### Comparing `hibp_downloader-0.1.1/src/hibp_downloader/commands/hibp_download.py` & `hibp_downloader-0.1.2/src/hibp_downloader/commands/hibp_download.py`

 * *Files identical despite different names*

### Comparing `hibp_downloader-0.1.1/src/hibp_downloader/commands/hibp_generate.py` & `hibp_downloader-0.1.2/src/hibp_downloader/commands/hibp_generate.py`

 * *Files identical despite different names*

### Comparing `hibp_downloader-0.1.1/src/hibp_downloader/exceptions.py` & `hibp_downloader-0.1.2/src/hibp_downloader/exceptions.py`

 * *Files identical despite different names*

### Comparing `hibp_downloader-0.1.1/src/hibp_downloader/lib/app.py` & `hibp_downloader-0.1.2/src/hibp_downloader/lib/app.py`

 * *Files identical despite different names*

### Comparing `hibp_downloader-0.1.1/src/hibp_downloader/lib/filedata.py` & `hibp_downloader-0.1.2/src/hibp_downloader/lib/filedata.py`

 * *Files identical despite different names*

### Comparing `hibp_downloader-0.1.1/src/hibp_downloader/lib/generators.py` & `hibp_downloader-0.1.2/src/hibp_downloader/lib/generators.py`

 * *Files identical despite different names*

### Comparing `hibp_downloader-0.1.1/src/hibp_downloader/lib/http.py` & `hibp_downloader-0.1.2/src/hibp_downloader/lib/http.py`

 * *Files identical despite different names*

### Comparing `hibp_downloader-0.1.1/src/hibp_downloader/lib/logger.py` & `hibp_downloader-0.1.2/src/hibp_downloader/lib/logger.py`

 * *Files identical despite different names*

### Comparing `hibp_downloader-0.1.1/src/hibp_downloader/main.py` & `hibp_downloader-0.1.2/src/hibp_downloader/main.py`

 * *Files identical despite different names*

### Comparing `hibp_downloader-0.1.1/src/hibp_downloader/models/prefix_metadata.py` & `hibp_downloader-0.1.2/src/hibp_downloader/models/prefix_metadata.py`

 * *Files identical despite different names*

### Comparing `hibp_downloader-0.1.1/src/hibp_downloader/models/stats.py` & `hibp_downloader-0.1.2/src/hibp_downloader/models/stats.py`

 * *Files identical despite different names*

### Comparing `hibp_downloader-0.1.1/PKG-INFO` & `hibp_downloader-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: hibp-downloader
-Version: 0.1.1
-Summary: Efficiently download new data for a local-copy of the pwned password hashes from api[.]pwnedpasswords[.]com
+Version: 0.1.2
+Summary: Efficiently download HIBP new pwned password data by hash-prefix for a local-copy
 License: BSD-3-Clause
 Keywords: hibp-downloader,hibp,haveibeenpwned,haveibeenpwned-downloader,sha1,ntlm
 Author: Nicholas de Jong
 Author-email: contact@threatpatrols.com
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
@@ -41,15 +41,15 @@
 
 ## Install
 ```commandline
 pip install --upgrade hibp-downloader
 ```
 
 ## Usage
-![screenshot-help.png](docs%2Fassets%2Fscreenshot-help.png)
+![screenshot-help.png](https://raw.githubusercontent.com/threatpatrols/hibp-downloader/main/docs/assets/screenshot-help.png)
 
 ## Runtime Logs
 Sample download activity logs 
 ```text
 2023-07-30T21:42:06+1000 | INFO | hibp-downloader | prefix=65747 source=[lc:207328 et:0 rc:56672 ro:0 xx:0] runtime_rate=[10.3MBit/s 79req/s ~65602H/s] runtime=0.2hr download=922.5MB
 2023-07-30T21:42:07+1000 | INFO | hibp-downloader | prefix=29da7 source=[lc:207328 et:0 rc:56792 ro:0 xx:0] runtime_rate=[10.4MBit/s 79req/s ~65646H/s] runtime=0.2hr download=924.5MB
 2023-07-30T21:42:09+1000 | INFO | hibp-downloader | prefix=43c7f source=[lc:207328 et:0 rc:56912 ro:0 xx:0] runtime_rate=[10.3MBit/s 79req/s ~65617H/s] runtime=0.2hr download=926.5MB
```

