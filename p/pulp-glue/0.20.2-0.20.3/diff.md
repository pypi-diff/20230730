# Comparing `tmp/pulp-glue-0.20.2.tar.gz` & `tmp/pulp-glue-0.20.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp-glue-0.20.2.tar", last modified: Wed Jul 19 11:35:51 2023, max compression
+gzip compressed data, was "pulp-glue-0.20.3.tar", last modified: Fri Jul 28 15:30:58 2023, max compression
```

## Comparing `pulp-glue-0.20.2.tar` & `pulp-glue-0.20.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:35:51.233203 pulp-glue-0.20.2/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-19 11:35:51.229203 pulp-glue-0.20.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-19 11:35:38.000000 pulp-glue-0.20.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:35:51.229203 pulp-glue-0.20.2/pulp_glue/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:35:51.229203 pulp-glue-0.20.2/pulp_glue/ansible/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 11:35:38.000000 pulp-glue-0.20.2/pulp_glue/ansible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-19 11:35:38.000000 pulp-glue-0.20.2/pulp_glue/ansible/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 11:35:38.000000 pulp-glue-0.20.2/pulp_glue/ansible/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:35:51.229203 pulp-glue-0.20.2/pulp_glue/certguard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 11:35:38.000000 pulp-glue-0.20.2/pulp_glue/certguard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-19 11:35:38.000000 pulp-glue-0.20.2/pulp_glue/certguard/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 11:35:38.000000 pulp-glue-0.20.2/pulp_glue/certguard/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:35:51.229203 pulp-glue-0.20.2/pulp_glue/common/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-19 11:35:38.000000 pulp-glue-0.20.2/pulp_glue/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38240 2023-07-19 11:35:38.000000 pulp-glue-0.20.2/pulp_glue/common/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-19 11:35:38.000000 pulp-glue-0.20.2/pulp_glue/common/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)    25040 2023-07-19 11:35:38.000000 pulp-glue-0.20.2/pulp_glue/common/openapi.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 11:35:38.000000 pulp-glue-0.20.2/pulp_glue/common/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:35:51.229203 pulp-glue-0.20.2/pulp_glue/container/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 11:35:38.000000 pulp-glue-0.20.2/pulp_glue/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-07-19 11:35:38.000000 pulp-glue-0.20.2/pulp_glue/container/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 11:35:38.000000 pulp-glue-0.20.2/pulp_glue/container/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:35:51.229203 pulp-glue-0.20.2/pulp_glue/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 11:35:38.000000 pulp-glue-0.20.2/pulp_glue/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19068 2023-07-19 11:35:38.000000 pulp-glue-0.20.2/pulp_glue/core/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 11:35:38.000000 pulp-glue-0.20.2/pulp_glue/core/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:35:51.229203 pulp-glue-0.20.2/pulp_glue/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 11:35:38.000000 pulp-glue-0.20.2/pulp_glue/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-07-19 11:35:38.000000 pulp-glue-0.20.2/pulp_glue/file/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 11:35:38.000000 pulp-glue-0.20.2/pulp_glue/file/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:35:51.229203 pulp-glue-0.20.2/pulp_glue/python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 11:35:38.000000 pulp-glue-0.20.2/pulp_glue/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-07-19 11:35:38.000000 pulp-glue-0.20.2/pulp_glue/python/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 11:35:38.000000 pulp-glue-0.20.2/pulp_glue/python/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:35:51.229203 pulp-glue-0.20.2/pulp_glue/rpm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 11:35:38.000000 pulp-glue-0.20.2/pulp_glue/rpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-07-19 11:35:38.000000 pulp-glue-0.20.2/pulp_glue/rpm/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 11:35:38.000000 pulp-glue-0.20.2/pulp_glue/rpm/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:35:51.229203 pulp-glue-0.20.2/pulp_glue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-19 11:35:51.000000 pulp-glue-0.20.2/pulp_glue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-19 11:35:51.000000 pulp-glue-0.20.2/pulp_glue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 11:35:51.000000 pulp-glue-0.20.2/pulp_glue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-19 11:35:51.000000 pulp-glue-0.20.2/pulp_glue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-19 11:35:51.000000 pulp-glue-0.20.2/pulp_glue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-19 11:35:38.000000 pulp-glue-0.20.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 11:35:51.233203 pulp-glue-0.20.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-19 11:35:38.000000 pulp-glue-0.20.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:58.136000 pulp-glue-0.20.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-28 15:30:58.136000 pulp-glue-0.20.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:58.132000 pulp-glue-0.20.3/pulp_glue/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:58.132000 pulp-glue-0.20.3/pulp_glue/ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/ansible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/ansible/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/ansible/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:58.132000 pulp-glue-0.20.3/pulp_glue/certguard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/certguard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/certguard/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/certguard/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:58.132000 pulp-glue-0.20.3/pulp_glue/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38246 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/common/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/common/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25040 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/common/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/common/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:58.132000 pulp-glue-0.20.3/pulp_glue/container/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/container/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/container/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:58.132000 pulp-glue-0.20.3/pulp_glue/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19068 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/core/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:58.132000 pulp-glue-0.20.3/pulp_glue/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/file/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/file/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:58.136000 pulp-glue-0.20.3/pulp_glue/python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/python/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/python/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:58.136000 pulp-glue-0.20.3/pulp_glue/rpm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/rpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/rpm/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/rpm/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:58.132000 pulp-glue-0.20.3/pulp_glue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-28 15:30:58.000000 pulp-glue-0.20.3/pulp_glue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-28 15:30:58.000000 pulp-glue-0.20.3/pulp_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 15:30:58.000000 pulp-glue-0.20.3/pulp_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-28 15:30:58.000000 pulp-glue-0.20.3/pulp_glue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-28 15:30:58.000000 pulp-glue-0.20.3/pulp_glue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 15:30:58.136000 pulp-glue-0.20.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/setup.py
```

### Comparing `pulp-glue-0.20.2/PKG-INFO` & `pulp-glue-0.20.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulp-glue
-Version: 0.20.2
+Version: 0.20.3
 Summary: Version agnostic glue library to talk to pulpcore's REST API.
 Home-page: https://github.com/pulp/pulp-cli
 Author: Pulp Team
 Author-email: pulp-list@redhat.com
 License: GPLv2+
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
```

### Comparing `pulp-glue-0.20.2/pulp_glue/ansible/context.py` & `pulp-glue-0.20.3/pulp_glue/ansible/context.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.20.2/pulp_glue/certguard/context.py` & `pulp-glue-0.20.3/pulp_glue/certguard/context.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.20.2/pulp_glue/common/context.py` & `pulp-glue-0.20.3/pulp_glue/common/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
                             and parameter["schema"]["type"] == "string"
                         ):
                             parameter["schema"] = {"type": "array", "items": {"type": "string"}}
         if self.has_plugin(PluginRequirement("file", specifier=">=1.10.0,<1.11.0")):
             operation = api_spec["paths"]["{file_file_alternate_content_source_href}refresh/"][
                 "post"
             ]
-            operation.pop("requestBody")
+            operation.pop("requestBody", None)
         if self.has_plugin(
             PluginRequirement("python", specifier="<99.99.0.dev")
         ):  # TODO Add version bounds
             python_remote_serializer = api_spec["components"]["schemas"]["python.PythonRemote"]
             patched_python_remote_serializer = api_spec["components"]["schemas"][
                 "Patchedpython.PythonRemote"
             ]
```

### Comparing `pulp-glue-0.20.2/pulp_glue/common/i18n.py` & `pulp-glue-0.20.3/pulp_glue/common/i18n.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.20.2/pulp_glue/common/openapi.py` & `pulp-glue-0.20.3/pulp_glue/common/openapi.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.20.2/pulp_glue/container/context.py` & `pulp-glue-0.20.3/pulp_glue/container/context.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.20.2/pulp_glue/core/context.py` & `pulp-glue-0.20.3/pulp_glue/core/context.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.20.2/pulp_glue/file/context.py` & `pulp-glue-0.20.3/pulp_glue/file/context.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.20.2/pulp_glue/python/context.py` & `pulp-glue-0.20.3/pulp_glue/python/context.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.20.2/pulp_glue/rpm/context.py` & `pulp-glue-0.20.3/pulp_glue/rpm/context.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.20.2/pulp_glue.egg-info/PKG-INFO` & `pulp-glue-0.20.3/pulp_glue.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulp-glue
-Version: 0.20.2
+Version: 0.20.3
 Summary: Version agnostic glue library to talk to pulpcore's REST API.
 Home-page: https://github.com/pulp/pulp-cli
 Author: Pulp Team
 Author-email: pulp-list@redhat.com
 License: GPLv2+
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
```

### Comparing `pulp-glue-0.20.2/pulp_glue.egg-info/SOURCES.txt` & `pulp-glue-0.20.3/pulp_glue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.20.2/setup.py` & `pulp-glue-0.20.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     name="pulp-glue",
     description="Version agnostic glue library to talk to pulpcore's REST API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Pulp Team",
     author_email="pulp-list@redhat.com",
     url="https://github.com/pulp/pulp-cli",
-    version="0.20.2",
+    version="0.20.3",
     packages=plugin_packages,
     package_data={"": ["py.typed"]},
     python_requires=">=3.6",
     install_requires=[
         "packaging>=20.0,<24",
         "requests>=2.24.0,<2.32",
     ],
```

