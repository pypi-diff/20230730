# Comparing `tmp/cogdb-3.0.6.tar.gz` & `tmp/cogdb-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cogdb-3.0.6.tar", last modified: Mon Jul 24 02:52:08 2023, max compression
+gzip compressed data, was "cogdb-3.0.7.tar", last modified: Sun Jul 30 02:04:29 2023, max compression
```

## Comparing `cogdb-3.0.6.tar` & `cogdb-3.0.7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:52:08.153014 cogdb-3.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-24 02:51:58.000000 cogdb-3.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-24 02:52:08.153014 cogdb-3.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-07-24 02:51:58.000000 cogdb-3.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:52:08.149014 cogdb-3.0.6/cog/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-24 02:51:58.000000 cogdb-3.0.6/cog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-24 02:51:58.000000 cogdb-3.0.6/cog/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-24 02:51:58.000000 cogdb-3.0.6/cog/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20251 2023-07-24 02:51:58.000000 cogdb-3.0.6/cog/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    17393 2023-07-24 02:51:58.000000 cogdb-3.0.6/cog/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    24044 2023-07-24 02:51:58.000000 cogdb-3.0.6/cog/torque.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-24 02:51:58.000000 cogdb-3.0.6/cog/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:52:08.153014 cogdb-3.0.6/cogdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-24 02:52:08.000000 cogdb-3.0.6/cogdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-24 02:52:08.000000 cogdb-3.0.6/cogdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 02:52:08.000000 cogdb-3.0.6/cogdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 02:52:08.000000 cogdb-3.0.6/cogdb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-24 02:52:08.000000 cogdb-3.0.6/cogdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-24 02:52:08.000000 cogdb-3.0.6/cogdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 02:52:08.153014 cogdb-3.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-24 02:51:58.000000 cogdb-3.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 02:52:08.153014 cogdb-3.0.6/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-24 02:51:58.000000 cogdb-3.0.6/test/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    11646 2023-07-24 02:51:58.000000 cogdb-3.0.6/test/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-24 02:51:58.000000 cogdb-3.0.6/test/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-24 02:51:58.000000 cogdb-3.0.6/test/test_db_2.py
--rw-r--r--   0 runner    (1001) docker     (123)    20460 2023-07-24 02:51:58.000000 cogdb-3.0.6/test/test_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-24 02:51:58.000000 cogdb-3.0.6/test/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-24 02:51:58.000000 cogdb-3.0.6/test/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-24 02:51:58.000000 cogdb-3.0.6/test/test_indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-24 02:51:58.000000 cogdb-3.0.6/test/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    22167 2023-07-24 02:51:58.000000 cogdb-3.0.6/test/test_sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-07-24 02:51:58.000000 cogdb-3.0.6/test/test_torque.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-24 02:51:58.000000 cogdb-3.0.6/test/test_torque2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-24 02:51:58.000000 cogdb-3.0.6/test/test_torque3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-24 02:51:58.000000 cogdb-3.0.6/test/test_torque4.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-24 02:51:58.000000 cogdb-3.0.6/test/test_torque5.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-07-24 02:51:58.000000 cogdb-3.0.6/test/test_torque6.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:04:29.792465 cogdb-3.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-30 02:04:20.000000 cogdb-3.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-30 02:04:29.792465 cogdb-3.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-07-30 02:04:20.000000 cogdb-3.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:04:29.788465 cogdb-3.0.7/cog/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-30 02:04:20.000000 cogdb-3.0.7/cog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-30 02:04:20.000000 cogdb-3.0.7/cog/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-30 02:04:20.000000 cogdb-3.0.7/cog/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20251 2023-07-30 02:04:20.000000 cogdb-3.0.7/cog/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17558 2023-07-30 02:04:20.000000 cogdb-3.0.7/cog/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24044 2023-07-30 02:04:20.000000 cogdb-3.0.7/cog/torque.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-30 02:04:20.000000 cogdb-3.0.7/cog/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:04:29.788465 cogdb-3.0.7/cogdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-30 02:04:29.000000 cogdb-3.0.7/cogdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-30 02:04:29.000000 cogdb-3.0.7/cogdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 02:04:29.000000 cogdb-3.0.7/cogdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 02:04:29.000000 cogdb-3.0.7/cogdb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-30 02:04:29.000000 cogdb-3.0.7/cogdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-30 02:04:29.000000 cogdb-3.0.7/cogdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 02:04:29.792465 cogdb-3.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-30 02:04:20.000000 cogdb-3.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:04:29.792465 cogdb-3.0.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-30 02:04:20.000000 cogdb-3.0.7/test/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11646 2023-07-30 02:04:20.000000 cogdb-3.0.7/test/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-30 02:04:20.000000 cogdb-3.0.7/test/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-07-30 02:04:20.000000 cogdb-3.0.7/test/test_db_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20460 2023-07-30 02:04:20.000000 cogdb-3.0.7/test/test_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-30 02:04:20.000000 cogdb-3.0.7/test/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-30 02:04:20.000000 cogdb-3.0.7/test/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-30 02:04:20.000000 cogdb-3.0.7/test/test_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-30 02:04:20.000000 cogdb-3.0.7/test/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22167 2023-07-30 02:04:20.000000 cogdb-3.0.7/test/test_sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-07-30 02:04:20.000000 cogdb-3.0.7/test/test_torque.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-30 02:04:20.000000 cogdb-3.0.7/test/test_torque2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-30 02:04:20.000000 cogdb-3.0.7/test/test_torque3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-30 02:04:20.000000 cogdb-3.0.7/test/test_torque4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-30 02:04:20.000000 cogdb-3.0.7/test/test_torque5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-07-30 02:04:20.000000 cogdb-3.0.7/test/test_torque6.py
```

### Comparing `cogdb-3.0.6/LICENSE` & `cogdb-3.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cogdb-3.0.6/README.md` & `cogdb-3.0.7/README.md`

 * *Files identical despite different names*

### Comparing `cogdb-3.0.6/cog/cache.py` & `cogdb-3.0.7/cog/cache.py`

 * *Files identical despite different names*

### Comparing `cogdb-3.0.6/cog/config.py` & `cogdb-3.0.7/cog/config.py`

 * *Files identical despite different names*

### Comparing `cogdb-3.0.6/cog/core.py` & `cogdb-3.0.7/cog/core.py`

 * *Files identical despite different names*

### Comparing `cogdb-3.0.6/cog/database.py` & `cogdb-3.0.7/cog/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,41 +238,46 @@
         position = self.current_table.store.save(new_record)
         self.current_table.indexer.put(new_record.key, position, self.current_table.store)
 
     def put_set(self, data):
         assert isinstance(data.key, str), "Only string type is supported."
         assert isinstance(data.value, str), "Only string type is supported."
 
-        # use (table name, key) as the cache key
         cache_key = (self.current_table.table_meta.name, data.key)
 
         if cache_key in self.cache:
             record = self.cache[cache_key]
         else:
             record = self.current_table.indexer.get(data.key, self.current_table.store)
             if len(self.cache) > self.config.LEVEL_2_CACHE_SIZE:
                 self.cache.popitem(last=False)
 
         new_record = Record(data.key, data.value, value_type='l')
+        position = None  # initialize position
 
-        if record is not None and data.value not in record.value:
-            new_record.set_value_link(record.store_position)
+        if record is None:
             position = self.current_table.store.save(new_record)
             self.current_table.indexer.put(new_record.key, position, self.current_table.store)
+        else:
+            if data.value not in record.value:
+                new_record.set_value_link(record.store_position)
+                position = self.current_table.store.save(new_record)
+                self.current_table.indexer.put(new_record.key, position, self.current_table.store)
 
-            if cache_key in self.cache and data.value not in self.cache[cache_key].value:
+        if cache_key in self.cache:
+            if record and data.value not in self.cache[cache_key].value:
                 self.cache[cache_key].value.add(data.value)
-                self.cache[cache_key].store_position = position
+                if position is not None:  # Update position if new record saved
+                    self.cache[cache_key].store_position = position
+        else:
+            if record:
+                self.cache[cache_key] = CacheData(record.store_position, set(record.value))
             else:
                 self.cache[cache_key] = CacheData(position, {data.value})
 
-        elif record is None:
-            position = self.current_table.store.save(new_record)
-            self.current_table.indexer.put(new_record.key, position, self.current_table.store)
-            self.cache[cache_key] = CacheData(position, {data.value})
         self.cache.move_to_end(cache_key)
 
     def get(self, key):
         if key in self.cache:
             return self.cache[key]
         return self.current_table.indexer.get(key, self.current_table.store)
```

### Comparing `cogdb-3.0.6/cog/torque.py` & `cogdb-3.0.7/cog/torque.py`

 * *Files identical despite different names*

### Comparing `cogdb-3.0.6/cog/view.py` & `cogdb-3.0.7/cog/view.py`

 * *Files identical despite different names*

### Comparing `cogdb-3.0.6/cogdb.egg-info/SOURCES.txt` & `cogdb-3.0.7/cogdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cogdb-3.0.6/test/test_cache.py` & `cogdb-3.0.7/test/test_cache.py`

 * *Files identical despite different names*

### Comparing `cogdb-3.0.6/test/test_core.py` & `cogdb-3.0.7/test/test_core.py`

 * *Files identical despite different names*

### Comparing `cogdb-3.0.6/test/test_db.py` & `cogdb-3.0.7/test/test_db.py`

 * *Files identical despite different names*

### Comparing `cogdb-3.0.6/test/test_db_2.py` & `cogdb-3.0.7/test/test_db_2.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,11 +56,34 @@
         cogdb.put_set(Record('key1', 'value5'))
 
         record = cogdb.get('key1')
         self.assertEqual(sorted(record.value), sorted(['value1', 'value2', 'value3', 'value4', 'value5']))
 
         cogdb.close()
 
+    def test_put_same_value_multiple_times(self):
+        db_path = '/tmp/cogtestdb4'
+        try:
+            os.makedirs(db_path)
+        except OSError:
+            if not os.path.isdir(db_path):
+                raise
+        config.CUSTOM_COG_DB_PATH = db_path
+
+        cogdb = Cog()
+        cogdb.create_or_load_namespace("my_namespace_5")
+        cogdb.create_table("new_db", "my_namespace_5")
+
+        cogdb.put_set(Record('key1', 'value1'))
+        cogdb.put_set(Record('key1', 'value1'))
+        cogdb.put_set(Record('key1', 'value2'))
+
+        record = cogdb.get('key1')
+        self.assertEqual(record.value, ['value2', 'value1'])
+
+        cogdb.close()
+
     def test_zzz_after_all_tests(self):
         shutil.rmtree('/tmp/cogtestdb2')
         shutil.rmtree('/tmp/cogtestdb3')
+        shutil.rmtree('/tmp/cogtestdb4')
         print("*** deleted test data.")
```

### Comparing `cogdb-3.0.6/test/test_embeddings.py` & `cogdb-3.0.7/test/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `cogdb-3.0.6/test/test_functions.py` & `cogdb-3.0.7/test/test_functions.py`

 * *Files identical despite different names*

### Comparing `cogdb-3.0.6/test/test_index.py` & `cogdb-3.0.7/test/test_index.py`

 * *Files identical despite different names*

### Comparing `cogdb-3.0.6/test/test_indexer.py` & `cogdb-3.0.7/test/test_indexer.py`

 * *Files identical despite different names*

### Comparing `cogdb-3.0.6/test/test_lib.py` & `cogdb-3.0.7/test/test_lib.py`

 * *Files identical despite different names*

### Comparing `cogdb-3.0.6/test/test_sim.py` & `cogdb-3.0.7/test/test_sim.py`

 * *Files identical despite different names*

### Comparing `cogdb-3.0.6/test/test_torque.py` & `cogdb-3.0.7/test/test_torque.py`

 * *Files identical despite different names*

### Comparing `cogdb-3.0.6/test/test_torque2.py` & `cogdb-3.0.7/test/test_torque2.py`

 * *Files identical despite different names*

### Comparing `cogdb-3.0.6/test/test_torque3.py` & `cogdb-3.0.7/test/test_torque3.py`

 * *Files identical despite different names*

### Comparing `cogdb-3.0.6/test/test_torque4.py` & `cogdb-3.0.7/test/test_torque4.py`

 * *Files identical despite different names*

### Comparing `cogdb-3.0.6/test/test_torque5.py` & `cogdb-3.0.7/test/test_torque5.py`

 * *Files identical despite different names*

### Comparing `cogdb-3.0.6/test/test_torque6.py` & `cogdb-3.0.7/test/test_torque6.py`

 * *Files identical despite different names*

