# Comparing `tmp/cymysql-0.9.8.tar.gz` & `tmp/cymysql-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cymysql-0.9.8.tar", last modified: Mon May 14 08:16:37 2018, max compression
+gzip compressed data, was "dist/cymysql-0.9.9.tar", last modified: Fri May 18 12:50:38 2018, max compression
```

## Comparing `cymysql-0.9.8.tar` & `cymysql-0.9.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 nakagami  (1000) nakagami  (1000)        0 2018-05-14 08:16:37.000000 cymysql-0.9.8/
-drwxrwxr-x   0 nakagami  (1000) nakagami  (1000)        0 2018-05-14 08:16:37.000000 cymysql-0.9.8/cymysql/
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)    20694 2018-05-14 08:05:57.000000 cymysql-0.9.8/cymysql/connections.py
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)    17752 2018-05-06 14:55:00.000000 cymysql-0.9.8/cymysql/charset.py
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)     9775 2018-05-06 15:08:35.000000 cymysql-0.9.8/cymysql/converters.py
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)    12819 2018-05-06 14:19:40.000000 cymysql-0.9.8/cymysql/packet.pyx
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)     3639 2018-05-14 08:09:39.000000 cymysql-0.9.8/cymysql/__init__.py
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)     9117 2018-05-06 15:04:35.000000 cymysql-0.9.8/cymysql/cursors.py
-drwxrwxr-x   0 nakagami  (1000) nakagami  (1000)        0 2018-05-14 08:16:37.000000 cymysql-0.9.8/cymysql/tests/
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)      578 2018-02-07 02:00:36.000000 cymysql-0.9.8/cymysql/tests/base.py
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)      363 2018-02-07 02:00:36.000000 cymysql-0.9.8/cymysql/tests/__init__.py
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)     2621 2018-02-07 02:00:36.000000 cymysql-0.9.8/cymysql/tests/test_DictCursor.py
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)    11016 2018-02-07 02:00:36.000000 cymysql-0.9.8/cymysql/tests/test_basic.py
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)    11082 2018-02-07 02:00:36.000000 cymysql-0.9.8/cymysql/tests/test_issues.py
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)     3641 2018-02-07 02:00:36.000000 cymysql-0.9.8/cymysql/tests/test_SSCursor.py
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)      649 2018-02-07 02:00:36.000000 cymysql-0.9.8/cymysql/tests/test_example.py
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)      359 2018-05-06 14:54:36.000000 cymysql-0.9.8/cymysql/times.py
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)     4444 2018-05-06 15:01:00.000000 cymysql-0.9.8/cymysql/err.py
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)    11916 2018-05-06 14:19:15.000000 cymysql-0.9.8/cymysql/packet.py
-drwxrwxr-x   0 nakagami  (1000) nakagami  (1000)        0 2018-05-14 08:16:37.000000 cymysql-0.9.8/cymysql/constants/
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)     2213 2018-02-07 02:00:36.000000 cymysql-0.9.8/cymysql/constants/CR.py
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)      452 2018-02-07 02:00:36.000000 cymysql-0.9.8/cymysql/constants/COMMAND.py
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)        0 2018-02-07 02:00:36.000000 cymysql-0.9.8/cymysql/constants/__init__.py
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)    31142 2018-02-07 02:00:36.000000 cymysql-0.9.8/cymysql/constants/ER.py
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)      372 2018-02-07 02:00:36.000000 cymysql-0.9.8/cymysql/constants/FIELD_TYPE.py
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)      214 2018-02-07 02:00:36.000000 cymysql-0.9.8/cymysql/constants/FLAG.py
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)      335 2018-05-01 12:52:29.000000 cymysql-0.9.8/cymysql/constants/SERVER_STATUS.py
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)      615 2018-05-03 03:03:49.000000 cymysql-0.9.8/cymysql/constants/CLIENT.py
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)     1069 2018-02-07 02:00:36.000000 cymysql-0.9.8/LICENSE
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)     2079 2018-02-07 02:00:36.000000 cymysql-0.9.8/setup.py
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)     2061 2018-05-14 08:16:37.000000 cymysql-0.9.8/PKG-INFO
--rw-rw-r--   0 nakagami  (1000) nakagami  (1000)     1108 2018-05-01 12:52:29.000000 cymysql-0.9.8/README.rst
+drwxrwxr-x   0 nakagami  (1000) nakagami  (1000)        0 2018-05-18 12:50:38.000000 cymysql-0.9.9/
+drwxrwxr-x   0 nakagami  (1000) nakagami  (1000)        0 2018-05-18 12:50:38.000000 cymysql-0.9.9/cymysql/
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)    20716 2018-05-17 08:34:41.000000 cymysql-0.9.9/cymysql/connections.py
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)    17752 2018-05-15 03:05:50.000000 cymysql-0.9.9/cymysql/charset.py
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)     9775 2018-05-15 03:05:50.000000 cymysql-0.9.9/cymysql/converters.py
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)    12819 2018-05-15 03:05:50.000000 cymysql-0.9.9/cymysql/packet.pyx
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)     3639 2018-05-18 12:46:35.000000 cymysql-0.9.9/cymysql/__init__.py
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)     9117 2018-05-15 03:05:50.000000 cymysql-0.9.9/cymysql/cursors.py
+drwxrwxr-x   0 nakagami  (1000) nakagami  (1000)        0 2018-05-18 12:50:38.000000 cymysql-0.9.9/cymysql/tests/
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)      578 2018-02-07 02:00:36.000000 cymysql-0.9.9/cymysql/tests/base.py
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)      363 2018-02-07 02:00:36.000000 cymysql-0.9.9/cymysql/tests/__init__.py
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)     2621 2018-02-07 02:00:36.000000 cymysql-0.9.9/cymysql/tests/test_DictCursor.py
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)    11016 2018-02-07 02:00:36.000000 cymysql-0.9.9/cymysql/tests/test_basic.py
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)    11082 2018-02-07 02:00:36.000000 cymysql-0.9.9/cymysql/tests/test_issues.py
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)     3641 2018-02-07 02:00:36.000000 cymysql-0.9.9/cymysql/tests/test_SSCursor.py
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)      649 2018-02-07 02:00:36.000000 cymysql-0.9.9/cymysql/tests/test_example.py
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)      359 2018-05-15 03:05:50.000000 cymysql-0.9.9/cymysql/times.py
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)     4444 2018-05-15 03:05:50.000000 cymysql-0.9.9/cymysql/err.py
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)    11916 2018-05-15 03:05:50.000000 cymysql-0.9.9/cymysql/packet.py
+drwxrwxr-x   0 nakagami  (1000) nakagami  (1000)        0 2018-05-18 12:50:38.000000 cymysql-0.9.9/cymysql/constants/
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)     2213 2018-02-07 02:00:36.000000 cymysql-0.9.9/cymysql/constants/CR.py
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)      452 2018-02-07 02:00:36.000000 cymysql-0.9.9/cymysql/constants/COMMAND.py
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)        0 2018-02-07 02:00:36.000000 cymysql-0.9.9/cymysql/constants/__init__.py
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)    31142 2018-02-07 02:00:36.000000 cymysql-0.9.9/cymysql/constants/ER.py
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)      372 2018-02-07 02:00:36.000000 cymysql-0.9.9/cymysql/constants/FIELD_TYPE.py
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)      214 2018-02-07 02:00:36.000000 cymysql-0.9.9/cymysql/constants/FLAG.py
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)      335 2018-05-01 12:52:29.000000 cymysql-0.9.9/cymysql/constants/SERVER_STATUS.py
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)      615 2018-05-03 03:03:49.000000 cymysql-0.9.9/cymysql/constants/CLIENT.py
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)     1069 2018-02-07 02:00:36.000000 cymysql-0.9.9/LICENSE
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)     2079 2018-02-07 02:00:36.000000 cymysql-0.9.9/setup.py
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)     2061 2018-05-18 12:50:38.000000 cymysql-0.9.9/PKG-INFO
+-rw-rw-r--   0 nakagami  (1000) nakagami  (1000)     1108 2018-05-01 12:52:29.000000 cymysql-0.9.9/README.rst
```

### Comparing `cymysql-0.9.8/cymysql/connections.py` & `cymysql-0.9.9/cymysql/connections.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,18 +58,21 @@
         return chr(n & 0xFF) + chr((n >> 8) & 0xFF) + chr((n >> 16) & 0xFF)
 
 
 SCRAMBLE_LENGTH = 20
 
 
 def _xor(data1, data2):
-    assert len(data1) == len(data2)
-    return bytes(
-        [byte2int(data1[i:i+1]) ^ byte2int(data2[i:i+1]) for i in range(len(data1))]
-    )
+    result = b''
+    for i in range(len(data1)):
+        j = i % len(data2)
+        x = (struct.unpack('B', data1[i:i+1])[0] ^ \
+             struct.unpack('B', data2[j:j+1])[0])
+        result += struct.pack('B', x)
+    return result
 
 
 def _mysql_native_password_scramble(password, message):
     if password is None or len(password) == 0:
         return b''
     message2 = sha_new(password).digest()
     stage2 = sha_new(message2).digest()
@@ -529,17 +532,15 @@
             response = self.read_packet()
             public_pem = response.get_all_data()[1:]
 
             from Crypto.PublicKey import RSA
             from Crypto.Cipher import PKCS1_OAEP
             key = RSA.importKey(public_pem)
             cipher = PKCS1_OAEP.new(key)
-            password = (
-                self.password.encode(self.charset) + b'\x00' * SCRAMBLE_LENGTH
-            )[:SCRAMBLE_LENGTH]
+            password = self.password.encode(self.charset) + b'\x00'
             data = cipher.encrypt(_xor(password, self.salt))
 
         data = pack_int24(len(data)) + int2byte(next_packet) + data
         next_packet += 2
         self.socket.sendall(data)
 
         self.read_packet()
```

### Comparing `cymysql-0.9.8/cymysql/charset.py` & `cymysql-0.9.9/cymysql/charset.py`

 * *Files identical despite different names*

### Comparing `cymysql-0.9.8/cymysql/converters.py` & `cymysql-0.9.9/cymysql/converters.py`

 * *Files identical despite different names*

### Comparing `cymysql-0.9.8/cymysql/packet.pyx` & `cymysql-0.9.9/cymysql/packet.pyx`

 * *Files identical despite different names*

### Comparing `cymysql-0.9.8/cymysql/__init__.py` & `cymysql-0.9.9/cymysql/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
      DatabaseError, OperationalError, IntegrityError, InternalError, \
      NotSupportedError, ProgrammingError, MySQLError
 from cymysql.times import Date, Time, Timestamp, \
     DateFromTicks, TimeFromTicks, TimestampFromTicks
 from cymysql.connections import Connection
 from cymysql.constants import FIELD_TYPE
 
-VERSION = (0, 9, 8)
+VERSION = (0, 9, 9)
 threadsafety = 1
 apilevel = "2.0"
 paramstyle = "format"
 
 
 class DBAPISet(frozenset):
```

### Comparing `cymysql-0.9.8/cymysql/cursors.py` & `cymysql-0.9.9/cymysql/cursors.py`

 * *Files identical despite different names*

### Comparing `cymysql-0.9.8/cymysql/tests/base.py` & `cymysql-0.9.9/cymysql/tests/base.py`

 * *Files identical despite different names*

### Comparing `cymysql-0.9.8/cymysql/tests/test_DictCursor.py` & `cymysql-0.9.9/cymysql/tests/test_DictCursor.py`

 * *Files identical despite different names*

### Comparing `cymysql-0.9.8/cymysql/tests/test_basic.py` & `cymysql-0.9.9/cymysql/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `cymysql-0.9.8/cymysql/tests/test_issues.py` & `cymysql-0.9.9/cymysql/tests/test_issues.py`

 * *Files identical despite different names*

### Comparing `cymysql-0.9.8/cymysql/tests/test_SSCursor.py` & `cymysql-0.9.9/cymysql/tests/test_SSCursor.py`

 * *Files identical despite different names*

### Comparing `cymysql-0.9.8/cymysql/tests/test_example.py` & `cymysql-0.9.9/cymysql/tests/test_example.py`

 * *Files identical despite different names*

### Comparing `cymysql-0.9.8/cymysql/err.py` & `cymysql-0.9.9/cymysql/err.py`

 * *Files identical despite different names*

### Comparing `cymysql-0.9.8/cymysql/packet.py` & `cymysql-0.9.9/cymysql/packet.py`

 * *Files identical despite different names*

### Comparing `cymysql-0.9.8/cymysql/constants/CR.py` & `cymysql-0.9.9/cymysql/constants/CR.py`

 * *Files identical despite different names*

### Comparing `cymysql-0.9.8/cymysql/constants/ER.py` & `cymysql-0.9.9/cymysql/constants/ER.py`

 * *Files identical despite different names*

### Comparing `cymysql-0.9.8/cymysql/constants/CLIENT.py` & `cymysql-0.9.9/cymysql/constants/CLIENT.py`

 * *Files identical despite different names*

### Comparing `cymysql-0.9.8/LICENSE` & `cymysql-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cymysql-0.9.8/setup.py` & `cymysql-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `cymysql-0.9.8/PKG-INFO` & `cymysql-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cymysql
-Version: 0.9.8
+Version: 0.9.9
 Summary: Python MySQL Driver using Cython
 Home-page: https://github.com/nakagami/CyMySQL/
 Author: Hajime Nakagami
 Author-email: nakagami@gmail.com
 License: MIT
 Description: ========
         CyMySQL
```

### Comparing `cymysql-0.9.8/README.rst` & `cymysql-0.9.9/README.rst`

 * *Files identical despite different names*

