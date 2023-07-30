# Comparing `tmp/galaxy-web-stack-23.0.4.tar.gz` & `tmp/galaxy-web-stack-23.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/web_stack/dist/.tmp-w8yrgk8n/galaxy-web-stack-23.0.4.tar", last modified: Fri Jun 30 22:07:36 2023, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/web_stack/dist/.tmp-4xolj2v_/galaxy-web-stack-23.0.5.tar", last modified: Sun Jul 30 10:53:59 2023, max compression
```

## Comparing `galaxy-web-stack-23.0.4.tar` & `galaxy-web-stack-23.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:07:36.000000 galaxy-web-stack-23.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-30 22:00:50.000000 galaxy-web-stack-23.0.4/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-30 22:00:49.000000 galaxy-web-stack-23.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-30 22:00:50.000000 galaxy-web-stack-23.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-30 22:07:36.000000 galaxy-web-stack-23.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-30 22:00:50.000000 galaxy-web-stack-23.0.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-30 22:00:50.000000 galaxy-web-stack-23.0.4/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:07:36.000000 galaxy-web-stack-23.0.4/galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-30 22:00:50.000000 galaxy-web-stack-23.0.4/galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:00:50.000000 galaxy-web-stack-23.0.4/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:07:36.000000 galaxy-web-stack-23.0.4/galaxy/web_stack/
--rw-r--r--   0 runner    (1001) docker     (123)    12414 2023-06-30 22:00:50.000000 galaxy-web-stack-23.0.4/galaxy/web_stack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-30 22:00:50.000000 galaxy-web-stack-23.0.4/galaxy/web_stack/gunicorn_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    21744 2023-06-30 22:00:50.000000 galaxy-web-stack-23.0.4/galaxy/web_stack/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-06-30 22:00:50.000000 galaxy-web-stack-23.0.4/galaxy/web_stack/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-30 22:00:50.000000 galaxy-web-stack-23.0.4/galaxy/web_stack/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:07:36.000000 galaxy-web-stack-23.0.4/galaxy_web_stack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-30 22:07:36.000000 galaxy-web-stack-23.0.4/galaxy_web_stack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-30 22:07:36.000000 galaxy-web-stack-23.0.4/galaxy_web_stack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 22:07:36.000000 galaxy-web-stack-23.0.4/galaxy_web_stack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-30 22:07:36.000000 galaxy-web-stack-23.0.4/galaxy_web_stack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 22:07:36.000000 galaxy-web-stack-23.0.4/galaxy_web_stack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-30 22:00:50.000000 galaxy-web-stack-23.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-30 22:07:36.000000 galaxy-web-stack-23.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 22:00:50.000000 galaxy-web-stack-23.0.4/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:53:59.000000 galaxy-web-stack-23.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-30 10:47:08.000000 galaxy-web-stack-23.0.5/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-07-30 10:47:07.000000 galaxy-web-stack-23.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-30 10:47:08.000000 galaxy-web-stack-23.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-30 10:53:59.000000 galaxy-web-stack-23.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-30 10:47:08.000000 galaxy-web-stack-23.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-30 10:47:08.000000 galaxy-web-stack-23.0.5/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:53:59.000000 galaxy-web-stack-23.0.5/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-30 10:47:08.000000 galaxy-web-stack-23.0.5/galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:47:08.000000 galaxy-web-stack-23.0.5/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:53:59.000000 galaxy-web-stack-23.0.5/galaxy/web_stack/
+-rw-r--r--   0 runner    (1001) docker     (123)    12414 2023-07-30 10:47:08.000000 galaxy-web-stack-23.0.5/galaxy/web_stack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-30 10:47:08.000000 galaxy-web-stack-23.0.5/galaxy/web_stack/gunicorn_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21742 2023-07-30 10:47:08.000000 galaxy-web-stack-23.0.5/galaxy/web_stack/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-30 10:47:08.000000 galaxy-web-stack-23.0.5/galaxy/web_stack/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-30 10:47:08.000000 galaxy-web-stack-23.0.5/galaxy/web_stack/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:53:59.000000 galaxy-web-stack-23.0.5/galaxy_web_stack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-30 10:53:59.000000 galaxy-web-stack-23.0.5/galaxy_web_stack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-30 10:53:59.000000 galaxy-web-stack-23.0.5/galaxy_web_stack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 10:53:59.000000 galaxy-web-stack-23.0.5/galaxy_web_stack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-30 10:53:59.000000 galaxy-web-stack-23.0.5/galaxy_web_stack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-30 10:53:59.000000 galaxy-web-stack-23.0.5/galaxy_web_stack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-30 10:47:08.000000 galaxy-web-stack-23.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-30 10:53:59.000000 galaxy-web-stack-23.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-30 10:47:08.000000 galaxy-web-stack-23.0.5/test-requirements.txt
```

### Comparing `galaxy-web-stack-23.0.4/LICENSE` & `galaxy-web-stack-23.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-web-stack-23.0.4/PKG-INFO` & `galaxy-web-stack-23.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-web-stack
-Version: 23.0.4
+Version: 23.0.5
 Summary: Galaxy web stack abstraction
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,14 +42,25 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.5 (2023-07-29)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Don't attempt to call a bool when using mem-self handler assignment. by `@natefoo <https://github.com/natefoo>`_ in `#16359 <https://github.com/galaxyproject/galaxy/pull/16359>`_
+
+-------------------
 23.0.4 (2023-06-30)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.3 (2023-06-26)
```

### Comparing `galaxy-web-stack-23.0.4/galaxy/web_stack/__init__.py` & `galaxy-web-stack-23.0.5/galaxy/web_stack/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-stack-23.0.4/galaxy/web_stack/gunicorn_config.py` & `galaxy-web-stack-23.0.5/galaxy/web_stack/gunicorn_config.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-stack-23.0.4/galaxy/web_stack/handlers.py` & `galaxy-web-stack-23.0.5/galaxy/web_stack/handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -331,15 +331,15 @@
             log.warning(
                 "(%s) Ignoring handler assignment to '%s' because configured handler assignment method"
                 " '' overrides per-tool handler assignment",
                 obj.log_str(),
                 HANDLER_ASSIGNMENT_METHODS.MEM_SELF,
                 configured,
             )
-        if flush():
+        if flush:
             _timed_flush_obj(obj)
         queue_callback()
         return self.app.config.server_name
 
     def _assign_db_self_handler(self, obj, method, configured, flush=True, **kwargs):
         """Assign object to this process by setting its ``handler`` column in the database to this process.
```

### Comparing `galaxy-web-stack-23.0.4/galaxy/web_stack/message.py` & `galaxy-web-stack-23.0.5/galaxy/web_stack/message.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-stack-23.0.4/galaxy/web_stack/transport.py` & `galaxy-web-stack-23.0.5/galaxy/web_stack/transport.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-stack-23.0.4/galaxy_web_stack.egg-info/PKG-INFO` & `galaxy-web-stack-23.0.5/galaxy_web_stack.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-web-stack
-Version: 23.0.4
+Version: 23.0.5
 Summary: Galaxy web stack abstraction
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,14 +42,25 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.5 (2023-07-29)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Don't attempt to call a bool when using mem-self handler assignment. by `@natefoo <https://github.com/natefoo>`_ in `#16359 <https://github.com/galaxyproject/galaxy/pull/16359>`_
+
+-------------------
 23.0.4 (2023-06-30)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.3 (2023-06-26)
```

### Comparing `galaxy-web-stack-23.0.4/setup.cfg` & `galaxy-web-stack-23.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-web-stack
 url = https://github.com/galaxyproject/galaxy
-version = 23.0.4
+version = 23.0.5
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-util
 	SQLAlchemy>=1.4.25,<2
 packages = find:
```

