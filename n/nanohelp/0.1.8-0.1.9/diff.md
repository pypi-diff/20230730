# Comparing `tmp/nanohelp-0.1.8.tar.gz` & `tmp/nanohelp-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanohelp-0.1.8.tar", max compression
+gzip compressed data, was "nanohelp-0.1.9.tar", max compression
```

## Comparing `nanohelp-0.1.8.tar` & `nanohelp-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1211 2023-07-28 00:51:01.641085 nanohelp-0.1.8/LICENSE
--rw-r--r--   0        0        0     1189 2023-07-29 16:16:01.618674 nanohelp-0.1.8/README.md
--rw-r--r--   0        0        0      218 2023-07-29 20:20:01.334089 nanohelp-0.1.8/nanohelp/__init__.py
--rw-r--r--   0        0        0     6659 2023-07-29 20:19:24.134567 nanohelp-0.1.8/nanohelp/secret.py
--rw-r--r--   0        0        0     4516 2023-07-29 19:44:44.557934 nanohelp-0.1.8/nanohelp/wallet.py
--rw-r--r--   0        0        0      447 2023-07-29 20:19:57.808008 nanohelp-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1704 1970-01-01 00:00:00.000000 nanohelp-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-07-28 00:51:01.641085 nanohelp-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1189 2023-07-29 16:16:01.618674 nanohelp-0.1.9/README.md
+-rw-r--r--   0        0        0      218 2023-07-29 20:33:11.424976 nanohelp-0.1.9/nanohelp/__init__.py
+-rw-r--r--   0        0        0     6709 2023-07-29 20:32:59.043776 nanohelp-0.1.9/nanohelp/secret.py
+-rw-r--r--   0        0        0     4516 2023-07-29 19:44:44.557934 nanohelp-0.1.9/nanohelp/wallet.py
+-rw-r--r--   0        0        0      447 2023-07-29 20:33:05.824719 nanohelp-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1704 1970-01-01 00:00:00.000000 nanohelp-0.1.9/PKG-INFO
```

### Comparing `nanohelp-0.1.8/LICENSE` & `nanohelp-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nanohelp-0.1.8/README.md` & `nanohelp-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `nanohelp-0.1.8/nanohelp/secret.py` & `nanohelp-0.1.9/nanohelp/secret.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,14 +139,15 @@
             parent = f"projects/{project}"
 
             # Check if the secret exists
             secrets = self.secret_manager_client.list_secrets(
                 request=secretmanager.ListSecretsRequest(parent=parent)
             )
 
+            LOG.debug(f"Secrets List: {secrets}")
             if name not in [secret.secret_id for secret in secrets]:
                 # If the secret doesn't exist, create it
                 self.create_secret(project, name)
 
             # Create a new secret version
             secret = self.secret_manager_client.secret_path(
                 project,
```

### Comparing `nanohelp-0.1.8/nanohelp/wallet.py` & `nanohelp-0.1.9/nanohelp/wallet.py`

 * *Files identical despite different names*

### Comparing `nanohelp-0.1.8/PKG-INFO` & `nanohelp-0.1.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanohelp
-Version: 0.1.8
+Version: 0.1.9
 Summary: Business logic to abstract the raw nano node RPC logic
 Author: Nate Schultz
 Author-email: nate.schultz@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
```

