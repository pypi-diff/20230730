# Comparing `tmp/budgeteer-0.1.0.tar.gz` & `tmp/budgeteer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "budgeteer-0.1.0.tar", last modified: Sun Jul 30 12:49:38 2023, max compression
+gzip compressed data, was "budgeteer-0.1.1.tar", last modified: Sun Jul 30 15:16:26 2023, max compression
```

## Comparing `budgeteer-0.1.0.tar` & `budgeteer-0.1.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:49:38.189586 budgeteer-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-30 12:49:12.000000 budgeteer-0.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-30 12:49:12.000000 budgeteer-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-07-30 12:49:38.189586 budgeteer-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-07-30 12:49:12.000000 budgeteer-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:49:38.185586 budgeteer-0.1.0/budgeteer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 12:49:12.000000 budgeteer-0.1.0/budgeteer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-07-30 12:49:12.000000 budgeteer-0.1.0/budgeteer/budget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:49:38.185586 budgeteer-0.1.0/budgeteer/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 12:49:12.000000 budgeteer-0.1.0/budgeteer/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-30 12:49:12.000000 budgeteer-0.1.0/budgeteer/providers/common_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-07-30 12:49:12.000000 budgeteer-0.1.0/budgeteer/providers/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:49:38.185586 budgeteer-0.1.0/budgeteer/providers/http_requests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 12:49:12.000000 budgeteer-0.1.0/budgeteer/providers/http_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-07-30 12:49:12.000000 budgeteer-0.1.0/budgeteer/providers/http_requests/cache_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-07-30 12:49:12.000000 budgeteer-0.1.0/budgeteer/providers/http_requests/cloudflare_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-07-30 12:49:12.000000 budgeteer-0.1.0/budgeteer/providers/http_requests/request_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-30 12:49:12.000000 budgeteer-0.1.0/budgeteer/providers/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-07-30 12:49:12.000000 budgeteer-0.1.0/budgeteer/providers/sqlite_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-07-30 12:49:12.000000 budgeteer-0.1.0/budgeteer/providers/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:49:38.185586 budgeteer-0.1.0/budgeteer/web_interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 12:49:12.000000 budgeteer-0.1.0/budgeteer/web_interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:49:38.185586 budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:49:38.185586 budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:49:38.189586 budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    85787 2023-07-30 12:49:37.000000 budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/@formkit-606708a1.js
--rw-r--r--   0 runner    (1001) docker     (123)    20752 2023-07-30 12:49:37.000000 budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/@popperjs-8746c87e.js
--rw-r--r--   0 runner    (1001) docker     (123)    64371 2023-07-30 12:49:37.000000 budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/@vue-de7d3d24.js
--rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-07-30 12:49:37.000000 budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/@vueuse-0fe84a4c.js
--rw-r--r--   0 runner    (1001) docker     (123)    28960 2023-07-30 12:49:37.000000 budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/axios-4a70c6fc.js
--rw-r--r--   0 runner    (1001) docker     (123)   231964 2023-07-30 12:49:37.000000 budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-39a9ac22.css
--rw-r--r--   0 runner    (1001) docker     (123)    60654 2023-07-30 12:49:37.000000 budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-85852bd1.js
--rw-r--r--   0 runner    (1001) docker     (123)   164360 2023-07-30 12:49:37.000000 budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff
--rw-r--r--   0 runner    (1001) docker     (123)    76081 2023-07-30 12:49:37.000000 budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-abbba2f8.css
--rw-r--r--   0 runner    (1001) docker     (123)   121340 2023-07-30 12:49:37.000000 budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    22677 2023-07-30 12:49:37.000000 budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/index-a0b4997d.js
--rw-r--r--   0 runner    (1001) docker     (123)    10556 2023-07-30 12:49:37.000000 budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/index-e2d31524.css
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-30 12:49:37.000000 budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 12:49:37.000000 budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-4ed993c7.js
--rw-r--r--   0 runner    (1001) docker     (123)    22835 2023-07-30 12:49:37.000000 budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-router-4cd13335.js
--rw-r--r--   0 runner    (1001) docker     (123)    51150 2023-07-30 12:49:37.000000 budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-tippy-7086acf8.js
--rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-07-30 12:49:37.000000 budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css
--rw-r--r--   0 runner    (1001) docker     (123)    18088 2023-07-30 12:49:37.000000 budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-6aa87443.js
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-07-30 12:49:37.000000 budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/vuex-636235de.js
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-07-30 12:49:37.000000 budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-30 12:49:37.000000 budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-07-30 12:49:12.000000 budgeteer-0.1.0/budgeteer/web_interface/web_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:49:38.185586 budgeteer-0.1.0/budgeteer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-07-30 12:49:38.000000 budgeteer-0.1.0/budgeteer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-30 12:49:38.000000 budgeteer-0.1.0/budgeteer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 12:49:38.000000 budgeteer-0.1.0/budgeteer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-30 12:49:38.000000 budgeteer-0.1.0/budgeteer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 12:49:38.000000 budgeteer-0.1.0/budgeteer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 12:49:38.000000 budgeteer-0.1.0/budgeteer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-30 12:49:38.000000 budgeteer-0.1.0/budgeteer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 12:49:38.189586 budgeteer-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-30 12:49:12.000000 budgeteer-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:16:26.543699 budgeteer-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-30 15:16:04.000000 budgeteer-0.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-30 15:16:04.000000 budgeteer-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-07-30 15:16:26.543699 budgeteer-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-07-30 15:16:04.000000 budgeteer-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:16:26.539699 budgeteer-0.1.1/budgeteer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:16:04.000000 budgeteer-0.1.1/budgeteer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-07-30 15:16:04.000000 budgeteer-0.1.1/budgeteer/budget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:16:26.539699 budgeteer-0.1.1/budgeteer/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:16:04.000000 budgeteer-0.1.1/budgeteer/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-30 15:16:04.000000 budgeteer-0.1.1/budgeteer/providers/common_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-07-30 15:16:04.000000 budgeteer-0.1.1/budgeteer/providers/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:16:26.539699 budgeteer-0.1.1/budgeteer/providers/http_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:16:04.000000 budgeteer-0.1.1/budgeteer/providers/http_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-07-30 15:16:04.000000 budgeteer-0.1.1/budgeteer/providers/http_requests/cache_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-07-30 15:16:04.000000 budgeteer-0.1.1/budgeteer/providers/http_requests/cloudflare_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-07-30 15:16:04.000000 budgeteer-0.1.1/budgeteer/providers/http_requests/request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-30 15:16:04.000000 budgeteer-0.1.1/budgeteer/providers/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-07-30 15:16:04.000000 budgeteer-0.1.1/budgeteer/providers/sqlite_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-07-30 15:16:04.000000 budgeteer-0.1.1/budgeteer/providers/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:16:26.539699 budgeteer-0.1.1/budgeteer/web_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:16:04.000000 budgeteer-0.1.1/budgeteer/web_interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:16:26.539699 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:16:26.539699 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:16:26.543699 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    85787 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/@formkit-606708a1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20752 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/@popperjs-8746c87e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    64371 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/@vue-de7d3d24.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/@vueuse-0fe84a4c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28960 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/axios-4a70c6fc.js
+-rw-r--r--   0 runner    (1001) docker     (123)   231964 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-39a9ac22.css
+-rw-r--r--   0 runner    (1001) docker     (123)    60654 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-85852bd1.js
+-rw-r--r--   0 runner    (1001) docker     (123)   164360 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    76081 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-abbba2f8.css
+-rw-r--r--   0 runner    (1001) docker     (123)   121340 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    23411 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/index-1f8a0d9a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10556 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/index-e2d31524.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-4ed993c7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22835 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-router-4cd13335.js
+-rw-r--r--   0 runner    (1001) docker     (123)    51150 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-tippy-7086acf8.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css
+-rw-r--r--   0 runner    (1001) docker     (123)    18088 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-6aa87443.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vuex-636235de.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-30 15:16:25.000000 budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-07-30 15:16:04.000000 budgeteer-0.1.1/budgeteer/web_interface/web_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:16:26.539699 budgeteer-0.1.1/budgeteer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-07-30 15:16:26.000000 budgeteer-0.1.1/budgeteer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-30 15:16:26.000000 budgeteer-0.1.1/budgeteer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 15:16:26.000000 budgeteer-0.1.1/budgeteer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-30 15:16:26.000000 budgeteer-0.1.1/budgeteer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 15:16:26.000000 budgeteer-0.1.1/budgeteer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 15:16:26.000000 budgeteer-0.1.1/budgeteer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-30 15:16:26.000000 budgeteer-0.1.1/budgeteer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 15:16:26.543699 budgeteer-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-30 15:16:04.000000 budgeteer-0.1.1/setup.py
```

### Comparing `budgeteer-0.1.0/LICENSE.md` & `budgeteer-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.0/PKG-INFO` & `budgeteer-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: budgeteer
-Version: 0.1.0
+Version: 0.1.1
 Summary: Einfacher Überblick über das eigene Budget
 Home-page: https://github.com/rix1337/BudgeTeer
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `budgeteer-0.1.0/README.md` & `budgeteer-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.0/budgeteer/budget.py` & `budgeteer-0.1.1/budgeteer/budget.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.0/budgeteer/providers/common_functions.py` & `budgeteer-0.1.1/budgeteer/providers/common_functions.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.0/budgeteer/providers/config.py` & `budgeteer-0.1.1/budgeteer/providers/config.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.0/budgeteer/providers/http_requests/cache_handler.py` & `budgeteer-0.1.1/budgeteer/providers/http_requests/cache_handler.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.0/budgeteer/providers/http_requests/cloudflare_handlers.py` & `budgeteer-0.1.1/budgeteer/providers/http_requests/cloudflare_handlers.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.0/budgeteer/providers/http_requests/request_handler.py` & `budgeteer-0.1.1/budgeteer/providers/http_requests/request_handler.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.0/budgeteer/providers/shared_state.py` & `budgeteer-0.1.1/budgeteer/providers/shared_state.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.0/budgeteer/providers/sqlite_database.py` & `budgeteer-0.1.1/budgeteer/providers/sqlite_database.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.0/budgeteer/providers/version.py` & `budgeteer-0.1.1/budgeteer/providers/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import re
 from distutils.version import StrictVersion
 from urllib.request import urlopen
 
 
 def get_version():
-    return "0.1.0"
+    return "0.1.1"
 
 
 def create_version_file():
     version = get_version()
     version_clean = re.sub('[^\d\.]', '', version)
     if "a" in version:
         suffix = version.split("a")[1]
```

### Comparing `budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/@formkit-606708a1.js` & `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/@formkit-606708a1.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/@popperjs-8746c87e.js` & `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/@popperjs-8746c87e.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/@vue-de7d3d24.js` & `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/@vue-de7d3d24.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/@vueuse-0fe84a4c.js` & `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/@vueuse-0fe84a4c.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/axios-4a70c6fc.js` & `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/axios-4a70c6fc.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-39a9ac22.css` & `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-39a9ac22.css`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-85852bd1.js` & `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-85852bd1.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff` & `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-abbba2f8.css` & `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-abbba2f8.css`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2` & `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/index-a0b4997d.js` & `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/index-1f8a0d9a.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,44 +1,44 @@
 import {
     b as j,
-    r as C,
+    r as V,
     c as O,
     U as a,
     F as i,
     N as e,
-    q as S,
-    P as V,
-    O as U,
+    q as B,
+    P as D,
+    O as N,
     S as L,
-    _ as D,
-    $ as B,
+    _ as w,
+    $ as S,
     u as s,
     a0 as W,
-    M as k,
+    M as v,
     s as P,
     W as $,
     J as I,
     X as z
 } from "./@vue-de7d3d24.js";
 import {
-    u as T,
+    u as M,
     c as R
 } from "./vuex-636235de.js";
 import {
-    a as w
+    a as C
 } from "./axios-4a70c6fc.js";
 import {
     c as A,
     a as H
 } from "./vue-router-4cd13335.js";
 import "./bootstrap-85852bd1.js"; /* empty css                        */
 import {
     u as E,
     s as q,
-    T as M
+    T
 } from "./vue-toastification-6aa87443.js";
 import {
     s as Y,
     p as G,
     d as J,
     a as X
 } from "./@formkit-606708a1.js";
@@ -53,15 +53,15 @@
 (function() {
     const t = document.createElement("link").relList;
     if (t && t.supports && t.supports("modulepreload")) return;
     for (const d of document.querySelectorAll('link[rel="modulepreload"]')) m(d);
     new MutationObserver(d => {
         for (const c of d)
             if (c.type === "childList")
-                for (const b of c.addedNodes) b.tagName === "LINK" && b.rel === "modulepreload" && m(b)
+                for (const p of c.addedNodes) p.tagName === "LINK" && p.rel === "modulepreload" && m(p)
     }).observe(document, {
         childList: !0,
         subtree: !0
     });
 
     function f(d) {
         const c = {};
@@ -105,16 +105,16 @@
     dt = {
         class: "input-group"
     },
     rt = {
         class: "input-group-prepend"
     },
     ut = ["disabled", "onUpdate:modelValue"],
-    pt = ["disabled", "onUpdate:modelValue"],
-    bt = e("div", {
+    bt = ["disabled", "onUpdate:modelValue"],
+    pt = e("div", {
         class: "input-group-append"
     }, [e("span", {
         class: "input-group-text"
     }, " €")], -1),
     _t = {
         key: 0,
         class: "input-group-append"
@@ -142,35 +142,35 @@
     }, null, -1),
     Vt = [Ct],
     Dt = ["onClick"],
     St = e("i", {
         class: "bi bi-trash3"
     }, null, -1),
     Bt = [St],
-    Nt = {
+    Ut = {
         key: 0,
         class: "row justify-content-center mt-2"
     },
-    Ut = {
+    Nt = {
         __name: "Head",
         setup(_) {
-            const t = T(),
+            const t = M(),
                 f = E();
             t.commit("getBalances"), j(() => {
-                b(), setInterval(b, 300 * 1e3)
+                p(), setInterval(p, 300 * 1e3)
             });
 
             function m() {
                 window.open("https://github.com/rix1337/BudgeTeer/releases/latest", "_blank")
             }
-            const d = C(""),
-                c = C(!1);
+            const d = V(""),
+                c = V(!1);
 
-            function b() {
-                w.get("api/version/").then(function(n) {
+            function p() {
+                C.get("api/version/").then(function(n) {
                     d.value = n.data.version.ver, console.info("%c BudgeTeer %c ".concat(d.value, " "), "color: white; background: #303030; font-weight: 700; font-size: 24px; font-family: Monospace;", "color: #303030; background: white; font-weight: 700; font-size: 24px; font-family: Monospace;"), console.info("%c ❤ Projekt unterstützen %c ".concat("https://github.com/sponsors/rix1337 ❤", " "), "color: white; background: #dc3545; font-weight: 700;", "color: #dc3545; background: white; font-weight: 700;"), c.value = n.data.version.update_ready, t.commit("setDocker", n.data.version.docker), c.value && (h("BudgeTeer - Update verfügbar! - "), console.log("Update steht bereit! Weitere Informationen unter https://github.com/rix1337/BudgeTeer/releases/latest"), f.info(`Update steht bereit! Weitere Informationen unter:
 https://github.com/rix1337/BudgeTeer/releases/latest`, {
                         timeout: 15e3,
                         onClick: m
                     }))
                 }, function() {
                     console.log("Konnte Version nicht abrufen!"), f.error("Konnte Version nicht abrufen!")
@@ -193,95 +193,95 @@
                     for (let r = 0; r < t.state.data.balances.length; r++) {
                         let l = parseFloat(t.state.data.balances[r].balance);
                         !isNaN(l) && t.state.data.balances[r].type === "checking" && (g += l)
                     }
                     let o = 0;
                     for (let r = 0; r < t.state.data.budgets.length; r++)
                         for (let l = 0; l < t.state.data.budgets[r].entries.length; l++) {
-                            let v = parseFloat(t.state.data.budgets[r].entries[l].amount);
-                            !isNaN(v) && y(t.state.data.budgets[r].entries[l]) && (o += v)
+                            let k = parseFloat(t.state.data.budgets[r].entries[l].amount);
+                            !isNaN(k) && y(t.state.data.budgets[r].entries[l]) && (o += k)
                         }
                     return (g + n + o).toFixed(2)
                 }
             });
 
             function y(n) {
                 if (!n.booked) {
                     let g = new Date,
                         o = new Date("1970-01-01"),
                         r = new Date("2100-01-01");
                     return n.valid_from_to[0] !== null && (o = new Date(n.valid_from_to[0])), n.valid_from_to[1] !== null && (r = new Date(n.valid_from_to[1])), g >= o && g <= r
                 }
                 return !1
             }
-            const p = C(new Date().toLocaleString("default", {
+            const b = V(new Date().toLocaleString("default", {
                 month: "long"
             }));
-            return (n, g) => (a(), i("div", tt, [e("div", et, [e("div", st, [e("div", ot, [e("div", nt, [e("h1", null, [at, S(" Verfügbar im " + V(p.value) + ": " + V(u.value) + " €", 1)])]), e("div", it, [e("div", lt, [e("div", ct, [(a(!0), i(U, null, L(s(t).state.data.balances, (o, r) => (a(), i("div", {
+            return (n, g) => (a(), i("div", tt, [e("div", et, [e("div", st, [e("div", ot, [e("div", nt, [e("h1", null, [at, B(" Verfügbar im " + D(b.value) + ": " + D(u.value) + " €", 1)])]), e("div", it, [e("div", lt, [e("div", ct, [(a(!0), i(N, null, L(s(t).state.data.balances, (o, r) => (a(), i("div", {
                 key: o,
                 class: "balance"
-            }, [e("div", dt, [e("div", rt, [D(e("input", {
+            }, [e("div", dt, [e("div", rt, [w(e("input", {
                 disabled: s(t).state.locked,
                 "onUpdate:modelValue": l => s(t).state.data.balances[r].label = l,
                 class: "form-control"
             }, null, 8, ut), [
-                [B, s(t).state.data.balances[r].label]
-            ])]), D(e("input", {
+                [S, s(t).state.data.balances[r].label]
+            ])]), w(e("input", {
                 disabled: s(t).state.locked,
                 "onUpdate:modelValue": l => s(t).state.data.balances[r].balance = l,
                 type: "number",
                 step: "0.01",
                 class: "form-control"
-            }, null, 8, pt), [
-                [B, s(t).state.data.balances[r].balance]
-            ]), bt, s(t).state.locked ? k("", !0) : (a(), i("div", _t, [D(e("select", {
+            }, null, 8, bt), [
+                [S, s(t).state.data.balances[r].balance]
+            ]), pt, s(t).state.locked ? v("", !0) : (a(), i("div", _t, [w(e("select", {
                 disabled: s(t).state.locked,
                 "onUpdate:modelValue": l => s(t).state.data.balances[r].type = l,
                 class: "form-control"
             }, ft, 8, mt), [
                 [W, s(t).state.data.balances[r].type]
-            ])])), s(t).state.locked ? k("", !0) : (a(), i("div", vt, [e("button", {
+            ])])), s(t).state.locked ? v("", !0) : (a(), i("div", vt, [e("button", {
                 class: "btn btn-outline-primary",
                 type: "button",
                 onClick: l => s(t).state.data.balances.splice(r - 1, 0, s(t).state.data.balances.splice(r, 1)[0])
             }, yt, 8, kt), e("button", {
                 class: "btn btn-outline-primary",
                 type: "button",
                 onClick: l => s(t).state.data.balances.splice(r + 1, 0, s(t).state.data.balances.splice(r, 1)[0])
             }, Vt, 8, wt), e("button", {
                 class: "btn btn-outline-danger",
                 type: "button",
                 onClick: l => s(t).state.data.balances.splice(r, 1)
-            }, Bt, 8, Dt)]))])]))), 128)), s(t).state.locked ? k("", !0) : (a(), i("div", Nt, [e("button", {
+            }, Bt, 8, Dt)]))])]))), 128)), s(t).state.locked ? v("", !0) : (a(), i("div", Ut, [e("button", {
                 class: "btn btn-outline-primary",
                 type: "button",
                 onClick: g[0] || (g[0] = o => s(t).state.data.balances.push({
                     label: "",
                     amount: ""
                 }))
             }, " Konto hinzufügen ")]))])])])])])])]))
         }
     };
-const Tt = {
+const Mt = {
         class: "text-center"
     },
-    Mt = {
+    Tt = {
         id: "offcanvasBottomSettings",
         "aria-labelledby": "offcanvasBottomSettingsLabel",
         class: "offcanvas offcanvas-bottom",
         tabindex: "-1"
     },
     Kt = e("div", {
         class: "offcanvas-header"
     }, [e("h3", {
         id: "offcanvasBottomSettingsLabel",
         class: "offcanvas-title"
     }, [e("i", {
         class: "bi bi-gear"
-    }), S(" Einstellungen")]), e("button", {
+    }), B(" Einstellungen")]), e("button", {
         "aria-label": "Close",
         class: "btn-close text-reset",
         "data-bs-dismiss": "offcanvas",
         type: "button"
     })], -1),
     Lt = {
         class: "offcanvas-body"
@@ -313,43 +313,43 @@
     It = e("span", {
         class: "spinner-border spinner-border-sm",
         role: "status"
     }, null, -1),
     zt = {
         __name: "Settings",
         setup(_) {
-            const t = T(),
+            const t = M(),
                 f = E();
 
             function m() {
-                d.value = !0, w.post("api/settings/", t.state.settings).then(function() {
+                d.value = !0, C.post("api/settings/", t.state.settings).then(function() {
                     console.log("Einstellungen gespeichert! Neustart des BudgeTeers wird dringend empfohlen!"), f.success("Einstellungen gespeichert! Neustart des BudgeTeers wird dringend empfohlen!"), t.commit("getSettings"), d.value = !1
                 }, function() {
                     t.commit("getSettings"), d.value = !1, console.log("Konnte Einstellungen nicht speichern! Bitte die angegebenen Werte auf Richtigkeit prüfen."), f.error("Konnte Einstellungen nicht speichern! Bitte die angegebenen Werte auf Richtigkeit prüfen.")
                 })
             }
-            const d = C(!1),
+            const d = V(!1),
                 c = O(() => t.state.settings.general.auth_hash.length > 0);
 
-            function b() {
+            function p() {
                 Y("settings")
             }
             return (h, u) => {
                 const y = P("FormKit");
-                return a(), i("div", Tt, [e("div", Mt, [Kt, e("div", Lt, [s(t).state.misc.loaded_settings ? k("", !0) : (a(), i("h4", Et, "Einstellungen werden geladen...")), s(t).state.misc.loaded_settings ? (a(), i("div", Ft, [$(y, {
+                return a(), i("div", Mt, [e("div", Tt, [Kt, e("div", Lt, [s(t).state.misc.loaded_settings ? v("", !0) : (a(), i("h4", Et, "Einstellungen werden geladen...")), s(t).state.misc.loaded_settings ? (a(), i("div", Ft, [$(y, {
                     id: "settings",
                     actions: !1,
                     "incomplete-message": "Es müssen alle Felder korrekt ausgefüllt werden! Fehler sind rot markiert.",
                     "messages-class": "text-danger mt-4",
                     type: "form",
-                    onSubmit: u[4] || (u[4] = p => m())
+                    onSubmit: u[4] || (u[4] = b => m())
                 }, {
                     default: I(({
-                        value: p
-                    }) => [s(t).state.misc.docker ? k("", !0) : (a(), i("div", Ot, [$(y, {
+                        value: b
+                    }) => [s(t).state.misc.docker ? v("", !0) : (a(), i("div", Ot, [$(y, {
                         modelValue: s(t).state.settings.general.port,
                         "onUpdate:modelValue": u[0] || (u[0] = n => s(t).state.settings.general.port = n),
                         help: "Hier den Port des Webservers wählen.",
                         "help-class": "text-muted",
                         "input-class": "form-control bg-light mb-2",
                         label: "Port",
                         "messages-class": "text-danger",
@@ -363,53 +363,53 @@
                         "onUpdate:modelValue": u[1] || (u[1] = n => s(t).state.settings.general.prefix = n),
                         help: "Hier den Prefix des Webservers wählen (nützlich für Reverse-Proxies).",
                         "help-class": "text-muted",
                         "input-class": "form-control bg-light mb-2",
                         label: "Prefix",
                         "messages-class": "text-danger",
                         "outer-class": "mb-4",
-                        placeholder: "Bspw. feedcrawler",
+                        placeholder: "Bspw. budgeteer",
                         type: "text",
                         validation: "alpha",
                         "validation-visibility": "live"
                     }, null, 8, ["modelValue"]), $(y, {
                         modelValue: s(t).state.settings.general.auth_user,
                         "onUpdate:modelValue": u[2] || (u[2] = n => s(t).state.settings.general.auth_user = n),
-                        validation: p.auth_hash ? "required" : "",
+                        validation: b.auth_hash ? "required" : "",
                         help: "Hier den Nutzernamen für BudgeTeer eingeben.",
                         "help-class": "text-muted",
                         "input-class": "form-control bg-light mb-2",
                         label: "Nutzername",
                         "messages-class": "text-danger",
                         name: "auth_user",
                         "outer-class": "mb-4",
                         placeholder: "Bspw. rix1337",
                         type: "text"
                     }, null, 8, ["modelValue", "validation"]), $(y, {
                         modelValue: s(t).state.settings.general.auth_hash,
                         "onUpdate:modelValue": u[3] || (u[3] = n => s(t).state.settings.general.auth_hash = n),
-                        validation: c.value && p.auth_user ? "required|length:6" : "",
+                        validation: c.value && b.auth_user ? "required|length:6" : "",
                         help: "Hier das Passwort für BudgeTeer angeben.",
                         "help-class": "text-muted",
                         "input-class": "form-control bg-light mb-2",
                         label: "Passwort",
                         "messages-class": "text-danger",
                         name: "auth_hash",
                         "outer-class": "mb-4",
                         placeholder: "Bspw. ●●●●●●●●",
                         type: "password",
                         "validation-visibility": "live"
                     }, null, 8, ["modelValue", "validation"])]),
                     _: 1
-                })])) : k("", !0), e("div", null, [s(t).state.misc.loaded_settings ? (a(), i("button", {
+                })])) : v("", !0), e("div", null, [s(t).state.misc.loaded_settings ? (a(), i("button", {
                     key: 0,
                     class: "btn btn-primary mt-4",
                     type: "submit",
-                    onClick: b
-                }, [d.value ? (a(), i("span", Pt)) : k("", !0), d.value ? k("", !0) : (a(), i("i", jt)), S(" Speichern ")])) : (a(), i("button", Wt, [It, S(" Lädt... ")]))])])])])
+                    onClick: p
+                }, [d.value ? (a(), i("span", Pt)) : v("", !0), d.value ? v("", !0) : (a(), i("i", jt)), B(" Speichern ")])) : (a(), i("button", Wt, [It, B(" Lädt... ")]))])])])])
             }
         }
     },
     Rt = {
         class: "container"
     },
     At = {
@@ -421,15 +421,15 @@
     qt = {
         class: "card text-center shadow my-3"
     },
     Yt = e("div", {
         class: "card-header"
     }, [e("h1", null, [e("i", {
         class: "bi bi-clock-history"
-    }), S(" Offene Transaktionen ")])], -1),
+    }), B(" Offene Transaktionen ")])], -1),
     Gt = {
         class: "card-body"
     },
     Jt = {
         class: "row justify-content-center mt-2"
     },
     Xt = {
@@ -463,58 +463,59 @@
         class: "input-group-append"
     },
     de = ["onClick"],
     re = e("i", {
         class: "bi bi-trash3"
     }, null, -1),
     ue = [re],
-    pe = {
+    be = {
         class: "row justify-content-center mt-2"
     },
-    be = {
+    pe = {
         __name: "Transactions",
         setup(_) {
-            const t = T();
-            return t.commit("getOpenTransactions"), (f, m) => (a(), i("div", Rt, [e("div", At, [e("div", Ht, [e("div", qt, [Yt, e("div", Gt, [e("div", Jt, [(a(!0), i(U, null, L(s(t).state.data.open_transactions, (d, c) => (a(), i("div", {
+            const t = M();
+            return t.commit("getOpenTransactions"), (f, m) => (a(), i("div", Rt, [e("div", At, [e("div", Ht, [e("div", qt, [Yt, e("div", Gt, [e("div", Jt, [(a(!0), i(N, null, L(s(t).state.data.open_transactions, (d, c) => (a(), i("div", {
                 key: d,
                 class: "transaction"
-            }, [e("div", Xt, [e("div", Qt, [D(e("input", {
+            }, [e("div", Xt, [e("div", Qt, [w(e("input", {
                 disabled: s(t).state.locked,
-                "onUpdate:modelValue": b => s(t).state.data.open_transactions[c].label = b,
+                "onUpdate:modelValue": p => s(t).state.data.open_transactions[c].label = p,
                 class: "form-control"
             }, null, 8, Zt), [
-                [B, s(t).state.data.open_transactions[c].label]
-            ])]), D(e("input", {
+                [S, s(t).state.data.open_transactions[c].label]
+            ])]), w(e("input", {
                 disabled: s(t).state.locked,
-                "onUpdate:modelValue": b => s(t).state.data.open_transactions[c].amount = b,
+                "onUpdate:modelValue": p => s(t).state.data.open_transactions[c].amount = p,
                 type: "number",
                 step: "0.01",
                 class: "form-control"
             }, null, 8, xt), [
-                [B, s(t).state.data.open_transactions[c].amount]
-            ]), te, s(t).state.locked ? k("", !0) : (a(), i("div", ee, [e("button", {
+                [S, s(t).state.data.open_transactions[c].amount]
+            ]), te, s(t).state.locked ? v("", !0) : (a(), i("div", ee, [e("button", {
                 class: "btn btn-outline-primary",
                 type: "button",
-                onClick: b => s(t).state.data.open_transactions.splice(c - 1, 0, s(t).state.data.open_transactions.splice(c, 1)[0])
+                onClick: p => s(t).state.data.open_transactions.splice(c - 1, 0, s(t).state.data.open_transactions.splice(c, 1)[0])
             }, ne, 8, se), e("button", {
                 class: "btn btn-outline-primary",
                 type: "button",
-                onClick: b => s(t).state.data.open_transactions.splice(c + 1, 0, s(t).state.data.open_transactions.splice(c, 1)[0])
+                onClick: p => s(t).state.data.open_transactions.splice(c + 1, 0, s(t).state.data.open_transactions.splice(c, 1)[0])
             }, le, 8, ae)])), e("div", ce, [e("button", {
                 class: "btn btn-outline-danger",
                 type: "button",
-                onClick: b => s(t).state.data.open_transactions.splice(c, 1) && s(t).commit("setModifiedWhileLocked", !0)
-            }, ue, 8, de)])])]))), 128)), e("div", pe, [e("button", {
+                onClick: p => s(t).state.data.open_transactions.splice(c, 1) && s(t).commit("setModifiedWhileLocked", !0)
+            }, ue, 8, de)])])]))), 128)), e("div", be, [s(t).state.locked ? v("", !0) : (a(), i("button", {
+                key: 0,
                 class: "btn btn-outline-primary",
                 type: "button",
                 onClick: m[0] || (m[0] = d => s(t).state.data.open_transactions.push({
                     label: "",
                     amount: ""
                 }))
-            }, " Transaktion hinzufügen ")])])])])])])]))
+            }, " Transaktion hinzufügen "))])])])])])])]))
         }
     },
     _e = {
         class: "col-md-auto p-1"
     },
     me = e("i", {
         class: "bi bi-arrow-left"
@@ -537,38 +538,38 @@
             modelValue: String
         },
         emits: ["update:modelValue"],
         setup(_, {
             emit: t
         }) {
             const f = _,
-                m = C(f.modelValue);
+                m = V(f.modelValue);
 
-            function d(b) {
+            function d(p) {
                 m.value === null && (m.value = new Date().toLocaleDateString("en-CA", {
                     year: "numeric",
                     month: "2-digit"
                 }));
                 const h = new Date(m.value);
-                h.setMonth(h.getMonth() + b), h.setDate(1);
+                h.setMonth(h.getMonth() + p), h.setDate(1);
                 const u = h.toLocaleDateString("en-CA", {
                     year: "numeric",
                     month: "2-digit"
                 });
                 m.value = u, t("update:modelValue", u)
             }
 
             function c() {
                 m.value = null, t("update:modelValue", null)
             }
-            return (b, h) => (a(), i("div", _e, [e("button", {
+            return (p, h) => (a(), i("div", _e, [e("button", {
                 class: "btn btn-outline-primary",
                 type: "button",
                 onClick: h[0] || (h[0] = u => d(-1))
-            }, he), S(V(f.title) + " ", 1), _.modelValue !== null ? (a(), i("span", ge, V(_.modelValue), 1)) : (a(), i("span", fe, "∞ ")), e("button", {
+            }, he), B(D(f.title) + " ", 1), _.modelValue !== null ? (a(), i("span", ge, D(_.modelValue), 1)) : (a(), i("span", fe, "∞ ")), e("button", {
                 class: "btn btn-outline-primary",
                 type: "button",
                 onClick: h[1] || (h[1] = u => d(1))
             }, ke), e("button", {
                 class: "btn btn-outline-secondary",
                 onClick: c
             }, " ∞ ")]))
@@ -592,20 +593,20 @@
     De = e("i", {
         class: "bi bi-receipt-cutoff"
     }, null, -1),
     Se = ["disabled"],
     Be = e("i", {
         class: "bi bi-arrow-left"
     }, null, -1),
-    Ne = [Be],
-    Ue = ["disabled"],
-    Te = e("i", {
+    Ue = [Be],
+    Ne = ["disabled"],
+    Me = e("i", {
         class: "bi bi-arrow-right"
     }, null, -1),
-    Me = [Te],
+    Te = [Me],
     Ke = e("div", {
         class: "col-md-auto p-1"
     }, null, -1),
     Le = {
         class: "card-body"
     },
     Ee = {
@@ -613,305 +614,332 @@
     },
     Fe = {
         class: "accordion",
         id: "accordionBudgets"
     },
     Oe = ["id"],
     Pe = ["data-bs-target", "aria-controls"],
-    je = ["id", "aria-labelledby"],
-    We = {
+    je = ["data-bs-target", "aria-controls"],
+    We = ["onUpdate:modelValue"],
+    Ie = ["onClick"],
+    ze = e("i", {
+        class: "bi bi-trash3"
+    }, null, -1),
+    Re = [ze],
+    Ae = ["id", "aria-labelledby"],
+    He = {
         class: "accordion-body"
     },
-    Ie = {
+    qe = {
         key: 0,
         class: "input-group"
     },
-    ze = {
+    Ye = {
         class: "input-group-prepend"
     },
-    Re = ["disabled", "onUpdate:modelValue"],
-    Ae = ["disabled", "onUpdate:modelValue"],
-    He = e("div", {
+    Ge = ["disabled", "onUpdate:modelValue"],
+    Je = ["disabled", "onUpdate:modelValue"],
+    Xe = e("div", {
         class: "input-group-append"
     }, [e("span", {
         class: "input-group-text"
     }, " €")], -1),
-    qe = {
+    Qe = {
         key: 0,
         class: "input-group-append"
     },
-    Ye = ["onClick"],
-    Ge = e("i", {
+    Ze = ["onClick"],
+    xe = e("i", {
         class: "bi bi-x"
     }, null, -1),
-    Je = [Ge],
-    Xe = ["onClick"],
-    Qe = e("i", {
+    ts = [xe],
+    es = ["onClick"],
+    ss = e("i", {
         class: "bi bi-arrow-up"
     }, null, -1),
-    Ze = [Qe],
-    xe = ["onClick"],
-    ts = e("i", {
+    os = [ss],
+    ns = ["onClick"],
+    as = e("i", {
         class: "bi bi-arrow-down"
     }, null, -1),
-    es = [ts],
-    ss = ["onClick"],
-    os = e("i", {
+    is = [as],
+    ls = ["onClick"],
+    cs = e("i", {
         class: "bi bi-trash3"
     }, null, -1),
-    ns = [os],
-    as = {
+    ds = [cs],
+    rs = {
         class: "input-group-append"
     },
-    is = ["onClick"],
-    ls = e("i", {
+    us = ["onClick"],
+    bs = e("i", {
         class: "bi bi-check"
     }, null, -1),
-    cs = [ls],
-    ds = ["onClick"],
-    rs = {
+    ps = [bs],
+    _s = ["onClick"],
+    ms = {
         class: "row justify-content-center mt-2"
     },
-    us = {
+    hs = {
         __name: "Budgets",
         setup(_) {
-            const t = T();
+            const t = M();
             t.commit("getBudgets");
 
-            function f(p) {
-                return parseFloat(p).toFixed(2)
+            function f(b) {
+                return parseFloat(b).toFixed(2)
             }
 
-            function m(p) {
+            function m(b) {
                 let n = 0;
-                for (let g = 0; g < t.state.data.budgets[p].entries.length; g++)
-                    if (u(t.state.data.budgets[p].entries[g])) {
-                        let o = parseFloat(t.state.data.budgets[p].entries[g].amount);
+                for (let g = 0; g < t.state.data.budgets[b].entries.length; g++)
+                    if (u(t.state.data.budgets[b].entries[g])) {
+                        let o = parseFloat(t.state.data.budgets[b].entries[g].amount);
                         isNaN(o) || (n += o)
                     } return f(n)
             }
 
             function d() {
-                let p = new Date(c.value),
+                let b = new Date(c.value),
                     n = new Date;
-                return p.getMonth() === n.getMonth() && p.getFullYear() === n.getFullYear()
+                return b.getMonth() === n.getMonth() && b.getFullYear() === n.getFullYear()
             }
-            const c = C(new Date().toISOString().slice(0, 7)),
-                b = C(0);
+            const c = V(new Date().toISOString().slice(0, 7)),
+                p = V(0);
 
-            function h(p) {
-                b.value += p;
-                let n = new Date().setMonth(new Date().getMonth() + b.value);
+            function h(b) {
+                p.value += b;
+                let n = new Date().setMonth(new Date().getMonth() + p.value);
                 c.value = new Date(n).toISOString().slice(0, 7)
             }
 
-            function u(p) {
-                return t.state.locked && d() ? !p.booked && y(p) : p
+            function u(b) {
+                return t.state.locked && d() ? !b.booked && y(b) : b
             }
 
-            function y(p) {
+            function y(b) {
                 let n = new Date(c.value),
                     g = new Date("1970-01-01"),
                     o = new Date("2100-01-01");
-                return p.valid_from_to[0] !== null && (g = new Date(p.valid_from_to[0])), p.valid_from_to[1] !== null && (o = new Date(p.valid_from_to[1])), n >= g && n <= o
+                return b.valid_from_to[0] !== null && (g = new Date(b.valid_from_to[0])), b.valid_from_to[1] !== null && (o = new Date(b.valid_from_to[1])), n >= g && n <= o
             }
-            return (p, n) => (a(), i("div", $e, [e("div", ye, [e("div", we, [e("div", Ce, [e("div", Ve, [e("h1", null, [De, S(" Budgets " + V(c.value) + " ", 1), e("button", {
-                disabled: b.value <= 0,
+            return (b, n) => (a(), i("div", $e, [e("div", ye, [e("div", we, [e("div", Ce, [e("div", Ve, [e("h1", null, [De, B(" Budgets " + D(c.value) + " ", 1), e("button", {
+                disabled: p.value <= 0,
                 class: "btn btn-outline-primary m-1",
                 type: "button",
                 onClick: n[0] || (n[0] = g => h(-1))
-            }, Ne, 8, Se), e("button", {
-                disabled: b.value >= 13,
+            }, Ue, 8, Se), e("button", {
+                disabled: p.value >= 13,
                 class: "btn btn-outline-primary",
                 type: "button",
                 onClick: n[1] || (n[1] = g => h(1))
-            }, Me, 8, Ue)]), Ke]), e("div", Le, [e("div", Ee, [e("div", Fe, [(a(!0), i(U, null, L(s(t).state.data.budgets, (g, o) => (a(), i("div", {
+            }, Te, 8, Ne)]), Ke]), e("div", Le, [e("div", Ee, [e("div", Fe, [(a(!0), i(N, null, L(s(t).state.data.budgets, (g, o) => (a(), i("div", {
                 key: g,
                 class: "accordion-item"
             }, [e("h2", {
                 class: "accordion-header",
                 id: "heading" + o
-            }, [e("button", {
+            }, [s(t).state.locked ? (a(), i("button", {
+                key: 0,
                 class: "accordion-button collapsed",
                 type: "button",
                 "data-bs-toggle": "collapse",
                 "data-bs-target": "#collapse" + o,
                 "aria-expanded": "false",
                 "aria-controls": "collapse" + o
-            }, V(s(t).state.data.budgets[o].category) + ": " + V(m(o)) + " € ", 9, Pe)], 8, Oe), e("div", {
+            }, D(s(t).state.data.budgets[o].category) + ": " + D(m(o)) + " € ", 9, Pe)) : (a(), i("button", {
+                key: 1,
+                class: "accordion-button collapsed",
+                type: "button",
+                "data-bs-toggle": "collapse",
+                "data-bs-target": "#collapse" + o,
+                "aria-expanded": "false",
+                "aria-controls": "collapse" + o
+            }, [w(e("input", {
+                type: "text",
+                class: "form-control",
+                placeholder: "Kategorie",
+                "onUpdate:modelValue": r => s(t).state.data.budgets[o].category = r
+            }, null, 8, We), [
+                [S, s(t).state.data.budgets[o].category]
+            ]), e("button", {
+                class: "btn btn-outline-danger",
+                type: "button",
+                onClick: r => s(t).state.data.budgets.splice(o, 1) && s(t).commit("setModifiedWhileLocked", !0)
+            }, Re, 8, Ie)], 8, je))], 8, Oe), e("div", {
                 id: "collapse" + o,
                 class: "accordion-collapse collapse",
                 "aria-labelledby": "heading" + o,
                 "data-bs-parent": "#accordionBudgets"
-            }, [e("div", We, [(a(!0), i(U, null, L(s(t).state.data.budgets[o].entries, (r, l) => (a(), i("div", {
+            }, [e("div", He, [(a(!0), i(N, null, L(s(t).state.data.budgets[o].entries, (r, l) => (a(), i("div", {
                 key: r
-            }, [u(s(t).state.data.budgets[o].entries[l]) ? (a(), i("div", Ie, [e("div", ze, [D(e("input", {
+            }, [u(s(t).state.data.budgets[o].entries[l]) ? (a(), i("div", qe, [e("div", Ye, [w(e("input", {
                 disabled: s(t).state.locked,
-                "onUpdate:modelValue": v => s(t).state.data.budgets[o].entries[l].label = v,
+                "onUpdate:modelValue": k => s(t).state.data.budgets[o].entries[l].label = k,
                 class: "form-control"
-            }, null, 8, Re), [
-                [B, s(t).state.data.budgets[o].entries[l].label]
-            ])]), D(e("input", {
+            }, null, 8, Ge), [
+                [S, s(t).state.data.budgets[o].entries[l].label]
+            ])]), w(e("input", {
                 disabled: s(t).state.locked,
-                "onUpdate:modelValue": v => s(t).state.data.budgets[o].entries[l].amount = v,
+                "onUpdate:modelValue": k => s(t).state.data.budgets[o].entries[l].amount = k,
                 type: "number",
                 step: "0.01",
                 class: "form-control"
-            }, null, 8, Ae), [
-                [B, s(t).state.data.budgets[o].entries[l].amount]
-            ]), He, s(t).state.locked ? k("", !0) : (a(), i("div", qe, [d() && s(t).state.data.budgets[o].entries[l].booked ? (a(), i("button", {
+            }, null, 8, Je), [
+                [S, s(t).state.data.budgets[o].entries[l].amount]
+            ]), Xe, s(t).state.locked ? v("", !0) : (a(), i("div", Qe, [d() && s(t).state.data.budgets[o].entries[l].booked ? (a(), i("button", {
                 key: 0,
                 class: "btn btn-outline-danger",
                 type: "button",
-                onClick: v => s(t).state.data.budgets[o].entries[l].booked = !1
-            }, Je, 8, Ye)) : k("", !0), e("button", {
+                onClick: k => s(t).state.data.budgets[o].entries[l].booked = !1
+            }, ts, 8, Ze)) : v("", !0), e("button", {
                 class: "btn btn-outline-primary",
                 type: "button",
-                onClick: v => s(t).state.data.budgets[o].entries.splice(l - 1, 0, s(t).state.data.budgets[o].entries.splice(l, 1)[o])
-            }, Ze, 8, Xe), e("button", {
+                onClick: k => s(t).state.data.budgets[o].entries.splice(l - 1, 0, s(t).state.data.budgets[o].entries.splice(l, 1)[o])
+            }, os, 8, es), e("button", {
                 class: "btn btn-outline-primary",
                 type: "button",
-                onClick: v => s(t).state.data.budgets[o].entries.splice(l + 1, 0, s(t).state.data.budgets[o].entries.splice(l, 1)[o])
-            }, es, 8, xe), e("button", {
+                onClick: k => s(t).state.data.budgets[o].entries.splice(l + 1, 0, s(t).state.data.budgets[o].entries.splice(l, 1)[o])
+            }, is, 8, ns), e("button", {
                 class: "btn btn-outline-danger",
                 type: "button",
-                onClick: v => s(t).state.data.budgets[o].entries.splice(l, 1)
-            }, ns, 8, ss), $(F, {
+                onClick: k => s(t).state.data.budgets[o].entries.splice(l, 1)
+            }, ds, 8, ls), $(F, {
                 title: "von",
                 modelValue: s(t).state.data.budgets[o].entries[l].valid_from_to[0],
-                "onUpdate:modelValue": v => s(t).state.data.budgets[o].entries[l].valid_from_to[0] = v
+                "onUpdate:modelValue": k => s(t).state.data.budgets[o].entries[l].valid_from_to[0] = k
             }, null, 8, ["modelValue", "onUpdate:modelValue"]), $(F, {
                 title: "bis",
                 modelValue: s(t).state.data.budgets[o].entries[l].valid_from_to[1],
-                "onUpdate:modelValue": v => s(t).state.data.budgets[o].entries[l].valid_from_to[1] = v
-            }, null, 8, ["modelValue", "onUpdate:modelValue"])])), e("div", as, [d() && s(t).state.locked && !s(t).state.data.budgets[o].entries[l].booked ? (a(), i("button", {
+                "onUpdate:modelValue": k => s(t).state.data.budgets[o].entries[l].valid_from_to[1] = k
+            }, null, 8, ["modelValue", "onUpdate:modelValue"])])), e("div", rs, [d() && s(t).state.locked && !s(t).state.data.budgets[o].entries[l].booked ? (a(), i("button", {
                 key: 0,
                 class: "btn btn-outline-success",
                 type: "button",
-                onClick: v => {
+                onClick: k => {
                     s(t).commit("setModifiedWhileLocked", !0), s(t).state.data.budgets[o].entries[l].booked = !0
                 }
-            }, cs, 8, is)) : k("", !0)])])) : k("", !0)]))), 128)), s(t).state.locked ? k("", !0) : (a(), i("button", {
+            }, ps, 8, us)) : v("", !0)])])) : v("", !0)]))), 128)), s(t).state.locked ? v("", !0) : (a(), i("button", {
                 key: 0,
                 class: "btn btn-outline-primary",
                 type: "button",
                 onClick: r => s(t).state.data.budgets[o].entries.push({
                     label: "",
                     amount: "",
                     valid_from_to: [null, null],
                     booked: !1
                 })
-            }, " Eintrag hinzufügen ", 8, ds))])], 8, je)]))), 128))]), e("div", rs, [s(t).state.locked ? k("", !0) : (a(), i("button", {
+            }, " Eintrag hinzufügen ", 8, _s))])], 8, Ae)]))), 128))]), e("div", ms, [s(t).state.locked ? v("", !0) : (a(), i("button", {
                 key: 0,
                 class: "btn btn-outline-primary",
                 type: "button",
                 onClick: n[2] || (n[2] = g => s(t).state.data.budgets.push({
-                    category: "ToDo",
+                    category: "Kategorie",
                     amount: "",
                     entries: []
                 }))
             }, " Kategorie hinzufügen "))])])])])])])]))
         }
     },
-    ps = {
+    gs = {
         __name: "_Main",
         setup(_) {
-            return (t, f) => (a(), i("main", null, [$(Ut), $(be), $(us), $(zt)]))
+            return (t, f) => (a(), i("main", null, [$(Nt), $(pe), $(hs), $(zt)]))
         }
     },
-    bs = A({
+    fs = A({
         history: H(),
         routes: [{
             path: "/:pathMatch(.*)*",
-            component: ps
+            component: gs
         }]
     });
-const _s = {
+const vs = {
         class: "sticky-bottom float-end"
     },
-    ms = {
+    ks = {
         class: "col-md-auto p-1"
     },
-    hs = e("i", {
+    $s = e("i", {
         class: "bi bi-save"
     }, null, -1),
-    gs = [hs],
-    fs = e("i", {
+    ys = [$s],
+    ws = e("i", {
         class: "bi bi-unlock"
     }, null, -1),
-    vs = [fs],
-    ks = e("i", {
+    Cs = [ws],
+    Vs = e("i", {
         class: "bi bi-lock"
     }, null, -1),
-    $s = [ks],
-    ys = {
+    Ds = [Vs],
+    Ss = {
         key: 0,
         class: "bi bi-sun"
     },
-    ws = {
+    Bs = {
         key: 1,
         class: "bi bi-moon-stars"
     },
-    Cs = e("i", {
+    Us = e("i", {
         class: "bi bi-gear"
     }, null, -1),
-    Vs = [Cs],
-    Ds = {
+    Ns = [Us],
+    Ms = {
         __name: "App",
         setup(_) {
             const t = Z(),
                 f = x(t),
-                m = T(),
+                m = M(),
                 d = E();
 
             function c(h) {
-                w.post("api/json/" + h + "/", m.state.data[h]).then(function() {
+                C.post("api/json/" + h + "/", m.state.data[h]).then(function() {
                     console.log(h + " gespeichert.")
                 }, function() {
                     console.log("Konnte " + h + " nicht speichern!"), d.error("Konnte " + h + " nicht speichern!")
                 })
             }
 
-            function b() {
+            function p() {
                 c("balances"), c("budgets"), c("open_transactions"), m.commit("setLocked", !0), m.commit("setModifiedWhileLocked", !1)
             }
             return (h, u) => {
                 const y = P("router-view");
-                return a(), i(U, null, [$(y), e("div", _s, [e("div", ms, [s(m).state.modified_while_locked ? (a(), i("button", {
+                return a(), i(N, null, [$(y), e("div", vs, [e("div", ks, [s(m).state.modified_while_locked ? (a(), i("button", {
                     key: 0,
                     class: "btn btn-outline-warning bg-dark m-1",
                     type: "button",
-                    onClick: u[0] || (u[0] = p => b())
-                }, gs)) : s(m).state.locked ? (a(), i("button", {
+                    onClick: u[0] || (u[0] = b => p())
+                }, ys)) : s(m).state.locked ? (a(), i("button", {
                     key: 1,
                     class: "btn btn-outline-success bg-dark m-1",
                     type: "button",
-                    onClick: u[1] || (u[1] = p => s(m).commit("setLocked", !1))
-                }, vs)) : (a(), i("button", {
+                    onClick: u[1] || (u[1] = b => s(m).commit("setLocked", !1))
+                }, Cs)) : (a(), i("button", {
                     key: 2,
                     class: "btn btn-outline-danger bg-dark m-1",
                     type: "button",
-                    onClick: u[2] || (u[2] = p => b())
-                }, $s)), e("button", {
+                    onClick: u[2] || (u[2] = b => p())
+                }, Ds)), e("button", {
                     type: "button",
                     class: "btn btn-outline-secondary bg-dark text-warning m-1",
-                    onClick: u[3] || (u[3] = p => s(f)())
-                }, [s(t) ? (a(), i("i", ys)) : (a(), i("i", ws))]), e("button", {
+                    onClick: u[3] || (u[3] = b => s(f)())
+                }, [s(t) ? (a(), i("i", Ss)) : (a(), i("i", Bs))]), e("button", {
                     "aria-controls": "offcanvasBottomSettings",
                     class: "btn btn-outline-primary bg-dark m-1",
                     "data-bs-target": "#offcanvasBottomSettings",
                     "data-bs-toggle": "offcanvas",
                     type: "button",
-                    onClick: u[4] || (u[4] = p => s(m).commit("getSettings"))
-                }, Vs)])])], 64)
+                    onClick: u[4] || (u[4] = b => s(m).commit("getSettings"))
+                }, Ns)])])], 64)
             }
         }
     },
     K = E(),
-    Ss = R({
+    Ts = R({
         state() {
             return {
                 data: {
                     balances: [],
                     open_transactions: [],
                     budgets: []
                 },
@@ -922,36 +950,36 @@
                     loaded_settings: !1,
                     docker: !1
                 }
             }
         },
         mutations: {
             getSettings(_) {
-                w.get("api/settings/").then(function(t) {
+                C.get("api/settings/").then(function(t) {
                     _.settings = t.data.settings, _.misc.loaded_settings = !0
                 }, function() {
                     console.log("Konnte Einstellungen nicht abrufen!"), K.error("Konnte Einstellungen nicht abrufen!")
                 })
             },
             getBalances(_) {
-                w.get("api/json/balances/").then(function(t) {
+                C.get("api/json/balances/").then(function(t) {
                     _.data.balances = t.data.balances
                 }, function() {
                     console.log("Konnte Kontostände nicht abrufen!"), K.error("Konnte Kontostände nicht abrufen!")
                 })
             },
             getOpenTransactions(_) {
-                w.get("api/json/open_transactions/").then(function(t) {
+                C.get("api/json/open_transactions/").then(function(t) {
                     _.data.open_transactions = t.data.open_transactions
                 }, function() {
                     console.log("Konnte offene Transaktionen nicht abrufen!"), K.error("Konnte offene Transaktionen nicht abrufen!")
                 })
             },
             getBudgets(_) {
-                w.get("api/json/budgets/").then(function(t) {
+                C.get("api/json/budgets/").then(function(t) {
                     _.data.budgets = t.data.budgets
                 }, function() {
                     console.log("Konnte Budgets nicht abrufen!"), K.error("Konnte Budgets nicht abrufen!")
                 })
             },
             setDocker(_, t) {
                 _.misc.docker = t
@@ -960,39 +988,39 @@
                 _.locked = t
             },
             setModifiedWhileLocked(_, t) {
                 _.modified_while_locked = t
             }
         }
     }),
-    N = z(Ds);
-N.use(Ss);
-N.use(bs);
-N.use(q, {
+    U = z(Ms);
+U.use(Ts);
+U.use(fs);
+U.use(q, {
     position: "top-center",
     draggable: !1,
     maxToasts: 1,
     bodyClassName: ["toast-body"],
     toastDefaults: {
-        [M.ERROR]: {
+        [T.ERROR]: {
             icon: "bi bi-exclamation-triangle"
         },
-        [M.WARNING]: {
+        [T.WARNING]: {
             icon: "bi bi-exclamation-circle"
         },
-        [M.INFO]: {
+        [T.INFO]: {
             icon: "bi bi-info-circle"
         },
-        [M.SUCCESS]: {
+        [T.SUCCESS]: {
             icon: "bi bi-check-circle-fill",
             timeout: 3e3
         }
     }
 });
-N.use(Q);
-N.use(G, J({
+U.use(Q);
+U.use(G, J({
     locales: {
         de: X
     },
     locale: "de"
 }));
-N.mount("#app");
+U.mount("#app");
```

### Comparing `budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/index-e2d31524.css` & `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/index-e2d31524.css`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css` & `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-router-4cd13335.js` & `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-router-4cd13335.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-tippy-7086acf8.js` & `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-tippy-7086acf8.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css` & `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-6aa87443.js` & `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-6aa87443.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/assets/vuex-636235de.js` & `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/assets/vuex-636235de.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/favicon.ico` & `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.0/budgeteer/web_interface/vuejs_frontend/dist/index.html` & `budgeteer-0.1.1/budgeteer/web_interface/vuejs_frontend/dist/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 <head>
     <meta charset="UTF-8">
     <meta content="width=device-width, initial-scale=1, shrink-to-fit=no" name="viewport">
 
     <link href="./favicon.ico" rel="icon" type="image/x-icon">
 
     <title>BudgeTeer</title>
-  <script type="module" crossorigin src="./assets/index-a0b4997d.js"></script>
+  <script type="module" crossorigin src="./assets/index-1f8a0d9a.js"></script>
   <link rel="modulepreload" crossorigin href="./assets/@vue-de7d3d24.js">
   <link rel="modulepreload" crossorigin href="./assets/vuex-636235de.js">
   <link rel="modulepreload" crossorigin href="./assets/axios-4a70c6fc.js">
   <link rel="modulepreload" crossorigin href="./assets/vue-router-4cd13335.js">
   <link rel="modulepreload" crossorigin href="./assets/@popperjs-8746c87e.js">
   <link rel="modulepreload" crossorigin href="./assets/bootstrap-85852bd1.js">
   <link rel="modulepreload" crossorigin href="./assets/vue-toastification-6aa87443.js">
```

### Comparing `budgeteer-0.1.0/budgeteer/web_interface/web_server.py` & `budgeteer-0.1.1/budgeteer/web_interface/web_server.py`

 * *Files 14% similar despite different names*

```diff
@@ -220,36 +220,18 @@
         except:
             return abort(400, "Failed")
 
     @app.get(prefix + "/api/json/<name>/")
     @auth_basic(is_authenticated_user)
     def get_json(name):
         try:
-            # balances = {
-            #     "balances": [
-            #         {
-            #             "label": 'Girokonto',
-            #             "balance": prettify_amount("888.2"),
-            #             "type": 'checking'
-            #         },
-            #         {
-            #             "label": 'Urlaub',
-            #             "balance": prettify_amount("9999.99"),
-            #             "type": 'savings'
-            #         },
-            #         {
-            #             "label": 'Notfall', "balance": prettify_amount("1000"),
-            #             "type": 'savings'
-            #         }
-            #     ]
-            # }
             try:
                 data = json.loads(BudgetDB("json").retrieve(name))
             except:
-                data = {}
+                data = []
             return {
                 name: data
             }
         except:
             return abort(400, "Failed to load " + name)
 
     @app.post(prefix + "/api/json/<name>/")
```

### Comparing `budgeteer-0.1.0/budgeteer.egg-info/PKG-INFO` & `budgeteer-0.1.1/budgeteer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: budgeteer
-Version: 0.1.0
+Version: 0.1.1
 Summary: Einfacher Überblick über das eigene Budget
 Home-page: https://github.com/rix1337/BudgeTeer
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `budgeteer-0.1.0/budgeteer.egg-info/SOURCES.txt` & `budgeteer-0.1.1/budgeteer.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 budgeteer/web_interface/vuejs_frontend/dist/assets/@vueuse-0fe84a4c.js
 budgeteer/web_interface/vuejs_frontend/dist/assets/axios-4a70c6fc.js
 budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-39a9ac22.css
 budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-85852bd1.js
 budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff
 budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-abbba2f8.css
 budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2
-budgeteer/web_interface/vuejs_frontend/dist/assets/index-a0b4997d.js
+budgeteer/web_interface/vuejs_frontend/dist/assets/index-1f8a0d9a.js
 budgeteer/web_interface/vuejs_frontend/dist/assets/index-e2d31524.css
 budgeteer/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css
 budgeteer/web_interface/vuejs_frontend/dist/assets/vue-4ed993c7.js
 budgeteer/web_interface/vuejs_frontend/dist/assets/vue-router-4cd13335.js
 budgeteer/web_interface/vuejs_frontend/dist/assets/vue-tippy-7086acf8.js
 budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css
 budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-6aa87443.js
```

### Comparing `budgeteer-0.1.0/setup.py` & `budgeteer-0.1.1/setup.py`

 * *Files identical despite different names*

