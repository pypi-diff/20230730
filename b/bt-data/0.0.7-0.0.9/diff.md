# Comparing `tmp/bt_data-0.0.7-py3-none-any.whl.zip` & `tmp/bt_data-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,21 @@
-Zip file size: 5932 bytes, number of entries: 17
--rw-r--r--  2.0 unx      124 b- defN 23-Jul-29 17:33 db/DbAdapter.py
--rw-r--r--  2.0 unx     2224 b- defN 23-Jul-29 17:33 db/PostgresqlAdapter.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-29 17:33 db/__init__.py
--rw-r--r--  2.0 unx      103 b- defN 23-Jul-29 17:33 enum/SyncType.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-29 17:33 enum/__init__.py
--rw-r--r--  2.0 unx      108 b- defN 23-Jul-29 17:33 model/Df.py
--rw-r--r--  2.0 unx     3250 b- defN 23-Jul-29 17:33 model/Instrument.py
--rw-r--r--  2.0 unx      415 b- defN 23-Jul-29 17:33 model/Model.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-29 17:33 model/__init__.py
--rw-r--r--  2.0 unx      256 b- defN 23-Jul-29 17:33 model/akshare/AKShareStockInfoACodeName.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-29 17:33 model/akshare/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-29 17:33 test/__init__.py
--rw-r--r--  2.0 unx      133 b- defN 23-Jul-29 17:33 test/test.py
--rw-r--r--  2.0 unx      701 b- defN 23-Jul-29 17:33 bt_data-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-29 17:33 bt_data-0.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-Jul-29 17:33 bt_data-0.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1257 b- defN 23-Jul-29 17:33 bt_data-0.0.7.dist-info/RECORD
-17 files, 8682 bytes uncompressed, 3882 bytes compressed:  55.3%
+Zip file size: 6458 bytes, number of entries: 19
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-29 17:42 bt_data/__init__.py
+-rw-r--r--  2.0 unx       67 b- defN 23-Jul-29 17:42 bt_data/data.py
+-rw-r--r--  2.0 unx      124 b- defN 23-Jul-29 17:42 bt_data/db/DbAdapter.py
+-rw-r--r--  2.0 unx     2224 b- defN 23-Jul-29 17:42 bt_data/db/PostgresqlAdapter.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-29 17:42 bt_data/db/__init__.py
+-rw-r--r--  2.0 unx      103 b- defN 23-Jul-29 17:42 bt_data/enum/SyncType.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-29 17:42 bt_data/enum/__init__.py
+-rw-r--r--  2.0 unx      108 b- defN 23-Jul-29 17:42 bt_data/model/Df.py
+-rw-r--r--  2.0 unx     3250 b- defN 23-Jul-29 17:42 bt_data/model/Instrument.py
+-rw-r--r--  2.0 unx      416 b- defN 23-Jul-29 17:42 bt_data/model/Model.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-29 17:42 bt_data/model/__init__.py
+-rw-r--r--  2.0 unx      256 b- defN 23-Jul-29 17:42 bt_data/model/akshare/AKShareStockInfoACodeName.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-29 17:42 bt_data/model/akshare/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-29 17:42 bt_data/test/__init__.py
+-rw-r--r--  2.0 unx      133 b- defN 23-Jul-29 17:42 bt_data/test/test.py
+-rw-r--r--  2.0 unx      701 b- defN 23-Jul-29 17:42 bt_data-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-29 17:42 bt_data-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-29 17:42 bt_data-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1503 b- defN 23-Jul-29 17:42 bt_data-0.0.9.dist-info/RECORD
+19 files, 8985 bytes uncompressed, 3980 bytes compressed:  55.7%
```

## zipnote {}

```diff
@@ -1,52 +1,58 @@
-Filename: db/DbAdapter.py
+Filename: bt_data/__init__.py
 Comment: 
 
-Filename: db/PostgresqlAdapter.py
+Filename: bt_data/data.py
 Comment: 
 
-Filename: db/__init__.py
+Filename: bt_data/db/DbAdapter.py
 Comment: 
 
-Filename: enum/SyncType.py
+Filename: bt_data/db/PostgresqlAdapter.py
 Comment: 
 
-Filename: enum/__init__.py
+Filename: bt_data/db/__init__.py
 Comment: 
 
-Filename: model/Df.py
+Filename: bt_data/enum/SyncType.py
 Comment: 
 
-Filename: model/Instrument.py
+Filename: bt_data/enum/__init__.py
 Comment: 
 
-Filename: model/Model.py
+Filename: bt_data/model/Df.py
 Comment: 
 
-Filename: model/__init__.py
+Filename: bt_data/model/Instrument.py
 Comment: 
 
-Filename: model/akshare/AKShareStockInfoACodeName.py
+Filename: bt_data/model/Model.py
 Comment: 
 
-Filename: model/akshare/__init__.py
+Filename: bt_data/model/__init__.py
 Comment: 
 
-Filename: test/__init__.py
+Filename: bt_data/model/akshare/AKShareStockInfoACodeName.py
 Comment: 
 
-Filename: test/test.py
+Filename: bt_data/model/akshare/__init__.py
 Comment: 
 
-Filename: bt_data-0.0.7.dist-info/METADATA
+Filename: bt_data/test/__init__.py
 Comment: 
 
-Filename: bt_data-0.0.7.dist-info/WHEEL
+Filename: bt_data/test/test.py
 Comment: 
 
-Filename: bt_data-0.0.7.dist-info/top_level.txt
+Filename: bt_data-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: bt_data-0.0.7.dist-info/RECORD
+Filename: bt_data-0.0.9.dist-info/WHEEL
+Comment: 
+
+Filename: bt_data-0.0.9.dist-info/top_level.txt
+Comment: 
+
+Filename: bt_data-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `db/PostgresqlAdapter.py` & `bt_data/db/PostgresqlAdapter.py`

 * *Files identical despite different names*

## Comparing `model/Instrument.py` & `bt_data/model/Instrument.py`

 * *Files identical despite different names*

## Comparing `bt_data-0.0.7.dist-info/METADATA` & `bt_data-0.0.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bt-data
-Version: 0.0.7
+Version: 0.0.9
 Summary: BotTrader Data Package
 Home-page: https://dev.azure.com/enfuture/BotTrader/_git/bt-data
 Author: heian0224
 Author-email: heian0224@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://dev.azure.com/enfuture/BotTrader/_git/bt-data/issues
 Platform: UNKNOWN
```

