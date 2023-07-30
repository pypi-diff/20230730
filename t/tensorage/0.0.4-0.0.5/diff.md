# Comparing `tmp/tensorage-0.0.4.tar.gz` & `tmp/tensorage-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorage-0.0.4.tar", last modified: Sun Jul 30 14:05:11 2023, max compression
+gzip compressed data, was "tensorage-0.0.5.tar", last modified: Sun Jul 30 18:30:06 2023, max compression
```

## Comparing `tensorage-0.0.4.tar` & `tensorage-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:05:11.166586 tensorage-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-07-30 14:04:59.000000 tensorage-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-30 14:04:59.000000 tensorage-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      277 2023-07-30 14:05:11.166586 tensorage-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-30 14:04:59.000000 tensorage-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-30 14:04:59.000000 tensorage-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-30 14:05:11.166586 tensorage-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      703 2023-07-30 14:04:59.000000 tensorage-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:05:11.162586 tensorage-0.0.4/tensorage/
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-07-30 14:04:59.000000 tensorage-0.0.4/tensorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-30 14:04:59.000000 tensorage-0.0.4/tensorage/__version__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2619 2023-07-30 14:04:59.000000 tensorage-0.0.4/tensorage/session.py
--rw-r--r--   0 runner    (1001) docker     (122)     6364 2023-07-30 14:04:59.000000 tensorage-0.0.4/tensorage/store.py
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-07-30 14:04:59.000000 tensorage-0.0.4/tensorage/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 14:05:11.166586 tensorage-0.0.4/tensorage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      277 2023-07-30 14:05:11.000000 tensorage-0.0.4/tensorage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-07-30 14:05:11.000000 tensorage-0.0.4/tensorage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-30 14:05:11.000000 tensorage-0.0.4/tensorage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-07-30 14:05:11.000000 tensorage-0.0.4/tensorage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-30 14:05:11.000000 tensorage-0.0.4/tensorage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 18:30:06.980695 tensorage-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-07-30 18:29:56.000000 tensorage-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-30 18:29:56.000000 tensorage-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2023-07-30 18:30:06.980695 tensorage-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-30 18:29:56.000000 tensorage-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-30 18:29:56.000000 tensorage-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-30 18:30:06.980695 tensorage-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      703 2023-07-30 18:29:56.000000 tensorage-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 18:30:06.980695 tensorage-0.0.5/tensorage/
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-07-30 18:29:56.000000 tensorage-0.0.5/tensorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-30 18:29:56.000000 tensorage-0.0.5/tensorage/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2388 2023-07-30 18:29:56.000000 tensorage-0.0.5/tensorage/db_init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2619 2023-07-30 18:29:56.000000 tensorage-0.0.5/tensorage/session.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7325 2023-07-30 18:29:56.000000 tensorage-0.0.5/tensorage/store.py
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-07-30 18:29:56.000000 tensorage-0.0.5/tensorage/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 18:30:06.980695 tensorage-0.0.5/tensorage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2023-07-30 18:30:06.000000 tensorage-0.0.5/tensorage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      346 2023-07-30 18:30:06.000000 tensorage-0.0.5/tensorage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-30 18:30:06.000000 tensorage-0.0.5/tensorage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-07-30 18:30:06.000000 tensorage-0.0.5/tensorage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-30 18:30:06.000000 tensorage-0.0.5/tensorage.egg-info/top_level.txt
```

### Comparing `tensorage-0.0.4/LICENSE` & `tensorage-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorage-0.0.4/setup.py` & `tensorage-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `tensorage-0.0.4/tensorage/session.py` & `tensorage-0.0.5/tensorage/session.py`

 * *Files identical despite different names*

### Comparing `tensorage-0.0.4/tensorage/store.py` & `tensorage-0.0.5/tensorage/store.py`

 * *Files 17% similar despite different names*

```diff
@@ -87,17 +87,36 @@
             dataset = context.insert_dataset(key, shape, dim)
 
             # insert the tensor
             context.insert_tensor(dataset.id, [chunk for chunk in value])
 
     def __delitem__(self, key: str):
         raise NotImplementedError
+    
+    def __contains__(self, key: str):
+        # get the keys
+        keys = self.keys()
 
-    def keys(self):
-        raise NotImplementedError
+        # check if key is in keys
+        return key in keys
+    
+    def __len__(self):
+        # get the keys
+        keys = self.keys()
+
+        # return the length
+        return len(keys)
+
+    def keys(self) -> List[str]:
+        # get the keys from the database
+        with self._session as context:
+            keys = context.list_tensor_keys()
+        
+        # TODO: here caching could be added
+        return keys
 
 
 @dataclass
 class StoreContext(object):
     # This is the OPENED session, as we are in the StoreContext
     backend: 'BackendSession' = field(repr=False)
     _anon_key: str = field(init=False, repr=False)
@@ -172,15 +191,34 @@
 
         # grab the data
         data = response.data[0]['tensor']
 
         # return as np.ndarray
         return np.asarray(data)
 
-    def remove_dataset(self, key: str):
-        raise NotImplementedError
+    def remove_dataset(self, key: str) -> bool:
+        # setup auth token
+        self.__setup_auth()
 
-    def list_tensor_keys(self):
-        raise NotImplementedError
+        # remove the dataset
+        self.backend.client.table('datasets').delete().eq('key', key).execute()
+
+        # restore old token
+        self.__restore_auth()
+        
+        # return
+        return True
+
+    def list_tensor_keys(self) -> List[str]:
+        # setup auth token
+        self.__setup_auth()
+
+        # get the keys
+        response = self.backend.client.table('datasets').select('key').execute()
+
+        # restore old token
+        self.__restore_auth()
+
+        return [row['key'] for row in response.data]
 
     def __del__(self):
         self.backend.logout()
```

