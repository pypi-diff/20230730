# Comparing `tmp/bodhi_client-7.2.0.tar.gz` & `tmp/bodhi_client-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bodhi_client-7.2.0.tar", max compression
+gzip compressed data, was "bodhi_client-7.2.1.tar", max compression
```

## Comparing `bodhi_client-7.2.0.tar` & `bodhi_client-7.2.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0    18018 2023-04-29 08:07:12.000000 bodhi_client-7.2.0/COPYING
--rw-r--r--   0        0        0      935 2023-04-29 08:07:12.000000 bodhi_client-7.2.0/bodhi/client/__init__.py
--rw-r--r--   0        0        0    41042 2023-04-29 08:07:12.000000 bodhi_client-7.2.0/bodhi/client/bindings.py
--rw-r--r--   0        0        0    54744 2023-04-29 08:18:48.000000 bodhi_client-7.2.0/bodhi/client/cli.py
--rw-r--r--   0        0        0      628 2023-04-29 08:07:12.000000 bodhi_client-7.2.0/bodhi/client/constants.py
--rw-r--r--   0        0        0    12718 2023-04-29 08:07:12.000000 bodhi_client-7.2.0/bodhi/client/oidcclient.py
--rwxr-xr-x   0        0        0      236 2023-04-29 08:07:12.000000 bodhi_client-7.2.0/bodhi-client.bash
--rw-r--r--   0        0        0      776 2023-04-29 08:07:12.000000 bodhi_client-7.2.0/docs/Makefile
--rw-r--r--   0        0        0     1115 2023-04-29 08:07:12.000000 bodhi_client-7.2.0/docs/conf.py
--rw-r--r--   0        0        0        0 2023-04-29 08:07:12.000000 bodhi_client-7.2.0/docs/index.rst
--rw-r--r--   0        0        0    18967 2023-04-29 08:07:12.000000 bodhi_client-7.2.0/docs/man_pages/bodhi.rst
--rw-r--r--   0        0        0     1721 2023-04-30 06:59:12.000000 bodhi_client-7.2.0/pyproject.toml
--rw-r--r--   0        0        0       35 2023-04-29 08:07:12.000000 bodhi_client-7.2.0/tests/__init__.py
--rw-r--r--   0        0        0    46000 2023-04-29 08:07:12.000000 bodhi_client-7.2.0/tests/fixtures.py
--rw-r--r--   0        0        0    75076 2023-04-29 08:18:48.000000 bodhi_client-7.2.0/tests/test_bindings.py
--rw-r--r--   0        0        0   119695 2023-04-29 08:18:48.000000 bodhi_client-7.2.0/tests/test_cli.py
--rw-r--r--   0        0        0    15528 2023-04-29 08:07:12.000000 bodhi_client-7.2.0/tests/test_oidcclient.py
--rw-r--r--   0        0        0     2327 2023-04-29 08:07:12.000000 bodhi_client-7.2.0/tests/utils.py
--rw-r--r--   0        0        0     1434 1970-01-01 00:00:00.000000 bodhi_client-7.2.0/PKG-INFO
+-rw-r--r--   0        0        0    18018 2023-05-13 08:55:56.000000 bodhi_client-7.2.1/COPYING
+-rw-r--r--   0        0        0      935 2023-05-13 08:55:56.000000 bodhi_client-7.2.1/bodhi/client/__init__.py
+-rw-r--r--   0        0        0    41077 2023-07-30 14:37:08.000000 bodhi_client-7.2.1/bodhi/client/bindings.py
+-rw-r--r--   0        0        0    54744 2023-05-13 08:55:56.000000 bodhi_client-7.2.1/bodhi/client/cli.py
+-rw-r--r--   0        0        0      628 2023-05-13 08:55:56.000000 bodhi_client-7.2.1/bodhi/client/constants.py
+-rw-r--r--   0        0        0    12718 2023-05-13 08:55:56.000000 bodhi_client-7.2.1/bodhi/client/oidcclient.py
+-rwxr-xr-x   0        0        0      236 2023-05-13 08:55:56.000000 bodhi_client-7.2.1/bodhi-client.bash
+-rw-r--r--   0        0        0      776 2023-05-13 08:55:56.000000 bodhi_client-7.2.1/docs/Makefile
+-rw-r--r--   0        0        0     1115 2023-05-13 08:55:56.000000 bodhi_client-7.2.1/docs/conf.py
+-rw-r--r--   0        0        0        0 2023-05-13 08:55:56.000000 bodhi_client-7.2.1/docs/index.rst
+-rw-r--r--   0        0        0    18967 2023-05-13 08:55:56.000000 bodhi_client-7.2.1/docs/man_pages/bodhi.rst
+-rw-r--r--   0        0        0     1769 2023-07-30 14:38:50.000000 bodhi_client-7.2.1/pyproject.toml
+-rw-r--r--   0        0        0       35 2023-05-13 08:55:56.000000 bodhi_client-7.2.1/tests/__init__.py
+-rw-r--r--   0        0        0    46000 2023-05-13 08:55:56.000000 bodhi_client-7.2.1/tests/fixtures.py
+-rw-r--r--   0        0        0    75076 2023-05-13 08:55:56.000000 bodhi_client-7.2.1/tests/test_bindings.py
+-rw-r--r--   0        0        0   119695 2023-05-13 08:55:56.000000 bodhi_client-7.2.1/tests/test_cli.py
+-rw-r--r--   0        0        0    15528 2023-05-13 08:55:56.000000 bodhi_client-7.2.1/tests/test_oidcclient.py
+-rw-r--r--   0        0        0     2327 2023-05-13 08:55:56.000000 bodhi_client-7.2.1/tests/utils.py
+-rw-r--r--   0        0        0      916 1970-01-01 00:00:00.000000 bodhi_client-7.2.1/setup.py
+-rw-r--r--   0        0        0     1184 1970-01-01 00:00:00.000000 bodhi_client-7.2.1/PKG-INFO
```

### Comparing `bodhi_client-7.2.0/COPYING` & `bodhi_client-7.2.1/COPYING`

 * *Files identical despite different names*

### Comparing `bodhi_client-7.2.0/bodhi/client/__init__.py` & `bodhi_client-7.2.1/bodhi/client/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_client-7.2.0/bodhi/client/bindings.py` & `bodhi_client-7.2.1/bodhi/client/bindings.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,17 @@
             client_id = STG_CLIENT_ID
 
         if base_url[-1] != '/':
             base_url = base_url + '/'
         self.base_url = base_url
         self.csrf_token = ''
         self.oidc_storage_path = (
-            oidc_storage_path or os.path.join(os.environ["HOME"], ".config", "bodhi", "client.json")
+            oidc_storage_path or os.path.join(
+                os.path.expanduser("~"), ".config", "bodhi", "client.json"
+            )
         )
         self._build_oidc_client(client_id, id_provider)
 
     def _build_oidc_client(self, client_id, id_provider):
         self.oidc = OIDCClient(
             client_id,
             SCOPE,
```

### Comparing `bodhi_client-7.2.0/bodhi/client/cli.py` & `bodhi_client-7.2.1/bodhi/client/cli.py`

 * *Files identical despite different names*

### Comparing `bodhi_client-7.2.0/bodhi/client/constants.py` & `bodhi_client-7.2.1/bodhi/client/constants.py`

 * *Files identical despite different names*

### Comparing `bodhi_client-7.2.0/bodhi/client/oidcclient.py` & `bodhi_client-7.2.1/bodhi/client/oidcclient.py`

 * *Files identical despite different names*

### Comparing `bodhi_client-7.2.0/docs/Makefile` & `bodhi_client-7.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bodhi_client-7.2.0/docs/conf.py` & `bodhi_client-7.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bodhi_client-7.2.0/docs/man_pages/bodhi.rst` & `bodhi_client-7.2.1/docs/man_pages/bodhi.rst`

 * *Files identical despite different names*

### Comparing `bodhi_client-7.2.0/pyproject.toml` & `bodhi_client-7.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bodhi-client"
-version = "7.2.0"
+version = "7.2.1"
 description = "Bodhi client"
 authors = ["Fedora Infrastructure team"]
 maintainers = ["Fedora Infrastructure Team <infrastructure@lists.fedoraproject.org>"]
 homepage = "https://bodhi.fedoraproject.org/"
 repository = "https://github.com/fedora-infra/bodhi"
 keywords = ["fedora"]
 license = "GPL-2.0-or-later"
@@ -29,14 +29,17 @@
 include = [
     { path = "docs", format = "sdist" },
     { path = "bodhi-client.bash", format = "sdist" },
     { path = "COPYING", format = "sdist" },
 ]
 exclude = ["docs/_build"]
 
+[tool.poetry.build]
+generate-setup-file = true
+
 [tool.poetry.dev-dependencies]
 Sphinx = ">=3.4.3"
 pytest = ">=6.0.0"
 pytest-cov = ">=2.11.1"
 pytest-mock = ">=3.5.1"
 diff-cover = ">=4.2.1"
```

### Comparing `bodhi_client-7.2.0/tests/fixtures.py` & `bodhi_client-7.2.1/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `bodhi_client-7.2.0/tests/test_bindings.py` & `bodhi_client-7.2.1/tests/test_bindings.py`

 * *Files identical despite different names*

### Comparing `bodhi_client-7.2.0/tests/test_cli.py` & `bodhi_client-7.2.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `bodhi_client-7.2.0/tests/test_oidcclient.py` & `bodhi_client-7.2.1/tests/test_oidcclient.py`

 * *Files identical despite different names*

### Comparing `bodhi_client-7.2.0/tests/utils.py` & `bodhi_client-7.2.1/tests/utils.py`

 * *Files identical despite different names*

