# Comparing `tmp/shoobx.mocks3-4.2.3.tar.gz` & `tmp/shoobx.mocks3-4.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shoobx.mocks3-4.2.3.tar", last modified: Mon Jun 26 06:03:06 2023, max compression
+gzip compressed data, was "shoobx.mocks3-4.2.4.tar", last modified: Sun Jul 30 01:13:13 2023, max compression
```

## Comparing `shoobx.mocks3-4.2.3.tar` & `shoobx.mocks3-4.2.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2023-06-26 06:03:06.466111 shoobx.mocks3-4.2.3/
--rw-rw-r--   0 adi       (1000) adi       (1000)       71 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/.coveragerc
--rw-rw-r--   0 adi       (1000) adi       (1000)     2896 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/CHANGES.rst
--rw-rw-r--   0 adi       (1000) adi       (1000)      290 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/MANIFEST.in
--rw-rw-r--   0 adi       (1000) adi       (1000)     1755 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/Makefile
--rw-rw-r--   0 adi       (1000) adi       (1000)     1988 2023-06-26 06:03:06.466111 shoobx.mocks3-4.2.3/PKG-INFO
--rw-rw-r--   0 adi       (1000) adi       (1000)      943 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/README.rst
-drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2023-06-26 06:03:06.462110 shoobx.mocks3-4.2.3/config/
--rw-rw-r--   0 adi       (1000) adi       (1000)      153 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/config/mocks3.cfg
--rw-rw-r--   0 adi       (1000) adi       (1000)      221 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/config/uwsgi.ini
--rw-rw-r--   0 adi       (1000) adi       (1000)       16 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/requirements.in
--rw-rw-r--   0 adi       (1000) adi       (1000)       27 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/requirements.txt
-drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2023-06-26 06:03:06.462110 shoobx.mocks3-4.2.3/scripts/
--rw-rw-r--   0 adi       (1000) adi       (1000)     1147 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/scripts/performance.py
--rw-rw-r--   0 adi       (1000) adi       (1000)       38 2023-06-26 06:03:06.466111 shoobx.mocks3-4.2.3/setup.cfg
--rw-rw-r--   0 adi       (1000) adi       (1000)     2431 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/setup.py
-drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2023-06-26 06:03:06.462110 shoobx.mocks3-4.2.3/src/
-drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2023-06-26 06:03:06.462110 shoobx.mocks3-4.2.3/src/shoobx/
--rw-rw-r--   0 adi       (1000) adi       (1000)       64 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx/__init__.py
-drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2023-06-26 06:03:06.466111 shoobx.mocks3-4.2.3/src/shoobx/mocks3/
--rw-rw-r--   0 adi       (1000) adi       (1000)      928 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx/mocks3/__init__.py
--rw-rw-r--   0 adi       (1000) adi       (1000)     2340 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx/mocks3/config.py
--rw-rw-r--   0 adi       (1000) adi       (1000)    24572 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx/mocks3/models.py
--rw-rw-r--   0 adi       (1000) adi       (1000)      664 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx/mocks3/responses.py
--rw-rw-r--   0 adi       (1000) adi       (1000)     2141 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx/mocks3/run.py
-drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2023-06-26 06:03:06.466111 shoobx.mocks3-4.2.3/src/shoobx/mocks3/tests/
--rw-rw-r--   0 adi       (1000) adi       (1000)       18 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx/mocks3/tests/__init__.py
--rw-rw-r--   0 adi       (1000) adi       (1000)     1276 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx/mocks3/tests/test_config.py
--rw-rw-r--   0 adi       (1000) adi       (1000)    34069 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx/mocks3/tests/test_s3_boto3.py
--rw-rw-r--   0 adi       (1000) adi       (1000)     1051 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx/mocks3/urls.py
--rw-rw-r--   0 adi       (1000) adi       (1000)      473 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx/mocks3/wsgi.py
-drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2023-06-26 06:03:06.466111 shoobx.mocks3-4.2.3/src/shoobx.mocks3.egg-info/
--rw-rw-r--   0 adi       (1000) adi       (1000)     1988 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx.mocks3.egg-info/PKG-INFO
--rw-rw-r--   0 adi       (1000) adi       (1000)      784 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx.mocks3.egg-info/SOURCES.txt
--rw-rw-r--   0 adi       (1000) adi       (1000)        1 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx.mocks3.egg-info/dependency_links.txt
--rw-rw-r--   0 adi       (1000) adi       (1000)       61 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx.mocks3.egg-info/entry_points.txt
--rw-rw-r--   0 adi       (1000) adi       (1000)        1 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx.mocks3.egg-info/not-zip-safe
--rw-rw-r--   0 adi       (1000) adi       (1000)      137 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx.mocks3.egg-info/requires.txt
--rw-rw-r--   0 adi       (1000) adi       (1000)        7 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/src/shoobx.mocks3.egg-info/top_level.txt
--rw-rw-r--   0 adi       (1000) adi       (1000)      291 2023-06-26 06:03:06.000000 shoobx.mocks3-4.2.3/tox.ini
+drwxr-xr-x   0 a745565   (1000) a745565   (1000)        0 2023-07-30 01:13:13.550500 shoobx.mocks3-4.2.4/
+-rw-r--r--   0 a745565   (1000) a745565   (1000)       71 2023-07-30 01:13:13.000000 shoobx.mocks3-4.2.4/.coveragerc
+-rw-r--r--   0 a745565   (1000) a745565   (1000)     2965 2023-07-30 01:13:13.000000 shoobx.mocks3-4.2.4/CHANGES.rst
+-rw-r--r--   0 a745565   (1000) a745565   (1000)      290 2023-07-30 01:13:13.000000 shoobx.mocks3-4.2.4/MANIFEST.in
+-rw-r--r--   0 a745565   (1000) a745565   (1000)     1755 2023-07-30 01:13:13.000000 shoobx.mocks3-4.2.4/Makefile
+-rw-r--r--   0 a745565   (1000) a745565   (1000)     1988 2023-07-30 01:13:13.550500 shoobx.mocks3-4.2.4/PKG-INFO
+-rw-r--r--   0 a745565   (1000) a745565   (1000)      943 2023-07-30 01:13:13.000000 shoobx.mocks3-4.2.4/README.rst
+drwxr-xr-x   0 a745565   (1000) a745565   (1000)        0 2023-07-30 01:13:13.550500 shoobx.mocks3-4.2.4/config/
+-rw-r--r--   0 a745565   (1000) a745565   (1000)      153 2023-07-30 01:13:13.000000 shoobx.mocks3-4.2.4/config/mocks3.cfg
+-rw-r--r--   0 a745565   (1000) a745565   (1000)      221 2023-07-30 01:13:13.000000 shoobx.mocks3-4.2.4/config/uwsgi.ini
+-rw-r--r--   0 a745565   (1000) a745565   (1000)       16 2023-07-30 01:13:13.000000 shoobx.mocks3-4.2.4/requirements.in
+-rw-r--r--   0 a745565   (1000) a745565   (1000)       27 2023-07-30 01:13:13.000000 shoobx.mocks3-4.2.4/requirements.txt
+drwxr-xr-x   0 a745565   (1000) a745565   (1000)        0 2023-07-30 01:13:13.550500 shoobx.mocks3-4.2.4/scripts/
+-rw-r--r--   0 a745565   (1000) a745565   (1000)     1147 2023-07-30 01:13:13.000000 shoobx.mocks3-4.2.4/scripts/performance.py
+-rw-r--r--   0 a745565   (1000) a745565   (1000)      440 2023-07-30 01:13:13.550500 shoobx.mocks3-4.2.4/setup.cfg
+-rw-r--r--   0 a745565   (1000) a745565   (1000)     2432 2023-07-30 01:13:13.000000 shoobx.mocks3-4.2.4/setup.py
+drwxr-xr-x   0 a745565   (1000) a745565   (1000)        0 2023-07-30 01:13:13.550500 shoobx.mocks3-4.2.4/src/
+drwxr-xr-x   0 a745565   (1000) a745565   (1000)        0 2023-07-30 01:13:13.550500 shoobx.mocks3-4.2.4/src/shoobx/
+-rw-r--r--   0 a745565   (1000) a745565   (1000)       64 2023-07-30 01:13:13.000000 shoobx.mocks3-4.2.4/src/shoobx/__init__.py
+drwxr-xr-x   0 a745565   (1000) a745565   (1000)        0 2023-07-30 01:13:13.550500 shoobx.mocks3-4.2.4/src/shoobx/mocks3/
+-rw-r--r--   0 a745565   (1000) a745565   (1000)      928 2023-07-30 01:13:13.000000 shoobx.mocks3-4.2.4/src/shoobx/mocks3/__init__.py
+-rw-r--r--   0 a745565   (1000) a745565   (1000)     2340 2023-07-30 01:13:13.000000 shoobx.mocks3-4.2.4/src/shoobx/mocks3/config.py
+-rw-r--r--   0 a745565   (1000) a745565   (1000)    24966 2023-07-30 01:13:13.000000 shoobx.mocks3-4.2.4/src/shoobx/mocks3/models.py
+-rw-r--r--   0 a745565   (1000) a745565   (1000)      664 2023-07-30 01:13:13.000000 shoobx.mocks3-4.2.4/src/shoobx/mocks3/responses.py
+-rw-r--r--   0 a745565   (1000) a745565   (1000)     2141 2023-07-30 01:13:13.000000 shoobx.mocks3-4.2.4/src/shoobx/mocks3/run.py
+drwxr-xr-x   0 a745565   (1000) a745565   (1000)        0 2023-07-30 01:13:13.550500 shoobx.mocks3-4.2.4/src/shoobx/mocks3/tests/
+-rw-r--r--   0 a745565   (1000) a745565   (1000)       18 2023-07-30 01:13:13.000000 shoobx.mocks3-4.2.4/src/shoobx/mocks3/tests/__init__.py
+-rw-r--r--   0 a745565   (1000) a745565   (1000)     1284 2023-07-30 01:13:13.000000 shoobx.mocks3-4.2.4/src/shoobx/mocks3/tests/test_config.py
+-rw-r--r--   0 a745565   (1000) a745565   (1000)    34109 2023-07-30 01:13:13.000000 shoobx.mocks3-4.2.4/src/shoobx/mocks3/tests/test_s3_boto3.py
+-rw-r--r--   0 a745565   (1000) a745565   (1000)     1051 2023-07-30 01:13:13.000000 shoobx.mocks3-4.2.4/src/shoobx/mocks3/urls.py
+-rw-r--r--   0 a745565   (1000) a745565   (1000)      473 2023-07-30 01:13:13.000000 shoobx.mocks3-4.2.4/src/shoobx/mocks3/wsgi.py
+drwxr-xr-x   0 a745565   (1000) a745565   (1000)        0 2023-07-30 01:13:13.550500 shoobx.mocks3-4.2.4/src/shoobx.mocks3.egg-info/
+-rw-r--r--   0 a745565   (1000) a745565   (1000)     1988 2023-07-30 01:13:13.000000 shoobx.mocks3-4.2.4/src/shoobx.mocks3.egg-info/PKG-INFO
+-rw-r--r--   0 a745565   (1000) a745565   (1000)      794 2023-07-30 01:13:13.000000 shoobx.mocks3-4.2.4/src/shoobx.mocks3.egg-info/SOURCES.txt
+-rw-r--r--   0 a745565   (1000) a745565   (1000)        1 2023-07-30 01:13:13.000000 shoobx.mocks3-4.2.4/src/shoobx.mocks3.egg-info/dependency_links.txt
+-rw-r--r--   0 a745565   (1000) a745565   (1000)       61 2023-07-30 01:13:13.000000 shoobx.mocks3-4.2.4/src/shoobx.mocks3.egg-info/entry_points.txt
+-rw-r--r--   0 a745565   (1000) a745565   (1000)        1 2023-07-30 01:13:13.000000 shoobx.mocks3-4.2.4/src/shoobx.mocks3.egg-info/not-zip-safe
+-rw-r--r--   0 a745565   (1000) a745565   (1000)      137 2023-07-30 01:13:13.000000 shoobx.mocks3-4.2.4/src/shoobx.mocks3.egg-info/requires.txt
+-rw-r--r--   0 a745565   (1000) a745565   (1000)        7 2023-07-30 01:13:13.000000 shoobx.mocks3-4.2.4/src/shoobx.mocks3.egg-info/top_level.txt
+-rw-r--r--   0 a745565   (1000) a745565   (1000)      291 2023-07-30 01:13:13.000000 shoobx.mocks3-4.2.4/tox.ini
```

### Comparing `shoobx.mocks3-4.2.3/CHANGES.rst` & `shoobx.mocks3-4.2.4/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 =========
 CHANGELOG
 =========
 
 
+4.2.4 (2023-07-29)
+------------------
+
+- Updates to moto and boto.
+
+
 4.2.3 (2023-06-26)
 ------------------
 
 - Add checksum attributes to class Key
 
 
 4.2.2 (2023-03-21)
```

### Comparing `shoobx.mocks3-4.2.3/Makefile` & `shoobx.mocks3-4.2.4/Makefile`

 * *Files identical despite different names*

### Comparing `shoobx.mocks3-4.2.3/PKG-INFO` & `shoobx.mocks3-4.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shoobx.mocks3
-Version: 4.2.3
+Version: 4.2.4
 Summary: Shoobx Mock S3 Implementation
 Home-page: http://shoobx.com/
 Author: Shoobx, Inc.
 Author-email: dev@shoobx.com
 License: Proprietary
 Keywords: amazon aws s3 mock moto
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `shoobx.mocks3-4.2.3/README.rst` & `shoobx.mocks3-4.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `shoobx.mocks3-4.2.3/scripts/performance.py` & `shoobx.mocks3-4.2.4/scripts/performance.py`

 * *Files identical despite different names*

### Comparing `shoobx.mocks3-4.2.3/setup.py` & `shoobx.mocks3-4.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,18 @@
 # Utility function to read the README file.
 # Used for the long_description.  It's nice, because now 1) we have a top level
 # README file and 2) it's easier to type in the README file than to put a raw
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
+
 setup(
     name="shoobx.mocks3",
-    version='4.2.3',
+    version='4.2.4',
     author="Shoobx, Inc.",
     author_email="dev@shoobx.com",
     description="Shoobx Mock S3 Implementation",
     long_description=read('README.rst'),
     keywords="amazon aws s3 mock moto",
     license='Proprietary',
     url="http://shoobx.com/",
```

### Comparing `shoobx.mocks3-4.2.3/src/shoobx/mocks3/__init__.py` & `shoobx.mocks3-4.2.4/src/shoobx/mocks3/__init__.py`

 * *Files identical despite different names*

### Comparing `shoobx.mocks3-4.2.3/src/shoobx/mocks3/config.py` & `shoobx.mocks3-4.2.4/src/shoobx/mocks3/config.py`

 * *Files identical despite different names*

### Comparing `shoobx.mocks3-4.2.3/src/shoobx/mocks3/models.py` & `shoobx.mocks3-4.2.4/src/shoobx/mocks3/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,14 @@
                 for grant in value.grants
             ]
         with open(inst._info_path, "w") as file:
             json.dump(info, file)
 
 
 class Key(models.FakeKey):
-
     _last_modified = _InfoProperty("last_modified")
     storage_class = _InfoProperty("storage_class")
     metadata = _InfoProperty("metadata")
     _etag = _InfoProperty("etag")
     expiry_date = _InfoProperty("expiry_date")
     acl = _AclProperty("acl")
 
@@ -137,17 +136,15 @@
         self.kms_key_id = kms_key_id
         self.bucket_key_enabled = bucket_key_enabled
         self.lock_mode = lock_mode
         self.lock_legal_status = lock_legal_status
         self.lock_until = lock_until
         self._tick = 0
         self.disposed = None
-        self.checksum_value = checksum_value
-        self.checksum_algorithm = None
-
+        self.checksum_algorithm = "md5"
 
     def __getstate__(self):
         return self.__dict__.copy()
 
     def __setstate__(self, state):
         self.__dict__.update({k: v for k, v in state.items() if k != "value"})
 
@@ -179,14 +176,23 @@
                 file_hash = hashlib.md5()
                 while chunk := file.read(8192):
                     file_hash.update(chunk)
                 self._etag = file_hash.hexdigest()
         return f'"{self._etag}"'
 
     @property
+    def checksum_value(self):
+        return self._etag
+
+    @checksum_value.setter
+    def checksum_value(self, value):
+        # self.etag already generates an md5 hash if needed.
+        self.etag
+
+    @property
     def last_modified(self):
         return datetime.datetime.strptime(self._last_modified, "%Y-%m-%dT%H:%M:%S.%fZ")
 
     @property
     def last_modified_ISO8601(self):
         return self._last_modified
 
@@ -327,15 +333,14 @@
 
     def iterlists(self):
         for name in self.keys():
             yield name, self.getlist(name)
 
 
 class Part:
-
     _last_modified = _InfoProperty("last_modified")
     etag = _InfoProperty("etag")
 
     def __init__(self, multipart, name):
         self.multipart = multipart
         self.name = name
         self._path = os.path.join(multipart._path, str(name) + ".part")
@@ -397,15 +402,14 @@
         self.value = value
 
     def delete(self):
         shutil.rmtree(self._path)
 
 
 class Multipart:
-
     key_name = _InfoProperty("key_name")
     metadata = _InfoProperty("metadata")
     tags = _InfoProperty("tags")
     acl = _InfoProperty("acl")
     sse_encryption = _InfoProperty("sse_encryption")
     kms_key_id = _InfoProperty("kms_key_id")
 
@@ -515,15 +519,14 @@
         yield from os.listdir(self._path)
 
     def __len__(self):
         return len(os.listdir(self._path))
 
 
 class Bucket(models.FakeBucket):
-
     policy = _InfoProperty("policy")
     versioning_status = _InfoProperty("versioning_status")
     acl = _AclProperty("acl")
 
     def __init__(self, s3, name):
         self.s3 = s3
         self.name = name
@@ -575,24 +578,32 @@
             return []
         rules = []
         with open(self._lifecyle_path) as file:
             raw_rules = json.load(file)
         for rule in raw_rules:
             exp = rule.get("Expiration")
             tran = rule.get("Transition")
+            tranisitions = []
+            if tran:
+                tranisitions.append(
+                    models.LifecycleTransition(
+                        date=tran.get("Date") or None,
+                        days=tran["Days"],
+                        storage_class=tran["StorageClass"],
+                    )
+                )
             rules.append(
                 models.LifecycleRule(
                     rule_id=rule.get("ID"),
                     prefix=rule["Prefix"],
                     status=rule["Status"],
                     expiration_days=exp.get("Days") if exp else None,
                     expiration_date=exp.get("Date") if exp else None,
-                    transition_days=tran.get("Days") if tran else None,
-                    transition_date=tran.get("Date") if tran else None,
-                    storage_class=tran["StorageClass"] if tran else None,
+                    transitions=tranisitions,
+                    noncurrent_version_transitions=[],
                 )
             )
         return rules
 
     @property
     def website_configuration(self):
         if not os.path.exists(self._ws_config_path):
@@ -774,16 +785,17 @@
     def complete_multipart_upload(self, bucket_name, multipart_id, body):
         bucket = self.get_bucket(bucket_name)
         multipart = bucket.multiparts[multipart_id]
         value, etag = multipart.complete(body)
         return multipart, value, etag
 
     def reset(self):
-        # For every key and multipart, Moto opens a TemporaryFile to write the value of those keys
-        # Ensure that these TemporaryFile-objects are closed, and leave no filehandles open
+        # For every key and multipart, Moto opens a TemporaryFile to write the value of
+        # those keys. Ensure that these TemporaryFile-objects are closed, and leave no
+        # filehandles open
         for bucket in self.buckets.values():
             for key in bucket.keys.values():
                 if isinstance(key, Key):
                     key._value_buffer.close()
                     if key.multipart is not None:
                         for part in key.multipart.parts.values():
                             part._value_buffer.close()
```

### Comparing `shoobx.mocks3-4.2.3/src/shoobx/mocks3/responses.py` & `shoobx.mocks3-4.2.4/src/shoobx/mocks3/responses.py`

 * *Files identical despite different names*

### Comparing `shoobx.mocks3-4.2.3/src/shoobx/mocks3/run.py` & `shoobx.mocks3-4.2.4/src/shoobx/mocks3/run.py`

 * *Files identical despite different names*

### Comparing `shoobx.mocks3-4.2.3/src/shoobx/mocks3/tests/test_config.py` & `shoobx.mocks3-4.2.4/src/shoobx/mocks3/tests/test_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ###############################################################################
 #
 # Copyright 2018 by Shoobx, Inc.
 #
 ###############################################################################
 """Shoobx S3 Config Test
 """
-import mock
 import os
 import shutil
 import tempfile
 import unittest
+from unittest import mock
 
 from shoobx.mocks3 import config
 
 TEST_CONFIG = """
 [shoobx:mocks3]
 log-level = INFO
 directory = %s
@@ -39,8 +39,8 @@
 
     @mock.patch.object(os, "environ", {"name": "Jane", "NAME": "Joe"})
     def test_configure_dupe_env_key(self):
         config_path = os.path.join(self._dir, "config.ini")
         with open(config_path, "w") as file:
             file.write(TEST_CONFIG % self._dir)
         # Ensure loading does not fail.
-        app = config.configure(config_path)
+        config.configure(config_path)
```

### Comparing `shoobx.mocks3-4.2.3/src/shoobx/mocks3/tests/test_s3_boto3.py` & `shoobx.mocks3-4.2.4/src/shoobx/mocks3/tests/test_s3_boto3.py`

 * *Files 1% similar despite different names*

```diff
@@ -902,9 +902,12 @@
                     "Transitions": [{"Days": 90, "StorageClass": "STANDARD_IA"}],
                     "ID": "rule1",
                     "Prefix": "path/",
                     "Status": "Enabled",
                 }
             ]
         }
-        self.bucket.LifecycleConfiguration().put(LifecycleConfiguration=cfg)
+
+        self.assertTrue(
+            self.bucket.LifecycleConfiguration().put(LifecycleConfiguration=cfg)
+        )
         self.assertEqual(cfg["Rules"], self.bucket.LifecycleConfiguration().rules)
```

### Comparing `shoobx.mocks3-4.2.3/src/shoobx/mocks3/urls.py` & `shoobx.mocks3-4.2.4/src/shoobx/mocks3/urls.py`

 * *Files identical despite different names*

### Comparing `shoobx.mocks3-4.2.3/src/shoobx.mocks3.egg-info/PKG-INFO` & `shoobx.mocks3-4.2.4/src/shoobx.mocks3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shoobx.mocks3
-Version: 4.2.3
+Version: 4.2.4
 Summary: Shoobx Mock S3 Implementation
 Home-page: http://shoobx.com/
 Author: Shoobx, Inc.
 Author-email: dev@shoobx.com
 License: Proprietary
 Keywords: amazon aws s3 mock moto
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `shoobx.mocks3-4.2.3/src/shoobx.mocks3.egg-info/SOURCES.txt` & `shoobx.mocks3-4.2.4/src/shoobx.mocks3.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .coveragerc
 CHANGES.rst
 MANIFEST.in
 Makefile
 README.rst
 requirements.in
 requirements.txt
+setup.cfg
 setup.py
 tox.ini
 config/mocks3.cfg
 config/uwsgi.ini
 scripts/performance.py
 src/shoobx/__init__.py
 src/shoobx.mocks3.egg-info/PKG-INFO
```

