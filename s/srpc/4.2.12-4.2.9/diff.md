# Comparing `tmp/srpc-4.2.12-cp311-none-macosx_10_9_universal2.whl.zip` & `tmp/srpc-4.2.9-cp311-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 598666 bytes, number of entries: 11
--rw-r--r--  2.0 unx     1059 b- defN 23-Jul-30 12:08 srpc-4.2.12.dist-info/LICENSE
--rw-r--r--  2.0 unx     2176 b- defN 23-Jul-30 12:08 srpc-4.2.12.dist-info/METADATA
--rw-r--r--  2.0 unx      113 b- defN 23-Jul-30 12:08 srpc-4.2.12.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-30 12:08 srpc-4.2.12.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      376 b- defN 23-Jul-30 12:08 srpc-4.2.12.dist-info/RECORD
--rwxr-xr-x  2.0 unx   122971 b- defN 23-Jul-30 12:08 srpc/__init__.so
--rwxr-xr-x  2.0 unx   379593 b- defN 23-Jul-30 12:08 srpc/client.so
--rwxr-xr-x  2.0 unx   383035 b- defN 23-Jul-30 12:08 srpc/protocol.so
--rwxr-xr-x  2.0 unx   275415 b- defN 23-Jul-30 12:08 srpc/ring.so
--rwxr-xr-x  2.0 unx   417449 b- defN 23-Jul-30 12:07 srpc/server.so
--rwxr-xr-x  2.0 unx   469511 b- defN 23-Jul-30 12:08 srpc/ulog.so
-11 files, 2051699 bytes uncompressed, 597342 bytes compressed:  70.9%
+Zip file size: 257090 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat     1080 b- defN 23-Jun-25 23:16 srpc-4.2.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2222 b- defN 23-Jun-25 23:16 srpc-4.2.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-25 23:16 srpc-4.2.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        1 b- defN 23-Jun-25 23:16 srpc-4.2.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      371 b- defN 23-Jun-25 23:16 srpc-4.2.9.dist-info/RECORD
+-rw-rw-rw-  2.0 fat    22016 b- defN 23-Jun-25 23:16 srpc/__init__.pyd
+-rw-rw-rw-  2.0 fat   108544 b- defN 23-Jun-25 23:16 srpc/client.pyd
+-rw-rw-rw-  2.0 fat   108032 b- defN 23-Jun-25 23:16 srpc/protocol.pyd
+-rw-rw-rw-  2.0 fat    77824 b- defN 23-Jun-25 23:16 srpc/ring.pyd
+-rw-rw-rw-  2.0 fat   121344 b- defN 23-Jun-25 23:16 srpc/server.pyd
+-rw-rw-rw-  2.0 fat   129024 b- defN 23-Jun-25 23:16 srpc/ulog.pyd
+11 files, 570558 bytes uncompressed, 255764 bytes compressed:  55.2%
```

## zipnote {}

```diff
@@ -1,34 +1,34 @@
-Filename: srpc-4.2.12.dist-info/LICENSE
+Filename: srpc-4.2.9.dist-info/LICENSE
 Comment: 
 
-Filename: srpc-4.2.12.dist-info/METADATA
+Filename: srpc-4.2.9.dist-info/METADATA
 Comment: 
 
-Filename: srpc-4.2.12.dist-info/WHEEL
+Filename: srpc-4.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: srpc-4.2.12.dist-info/top_level.txt
+Filename: srpc-4.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: srpc-4.2.12.dist-info/RECORD
+Filename: srpc-4.2.9.dist-info/RECORD
 Comment: 
 
-Filename: srpc/__init__.so
+Filename: srpc/__init__.pyd
 Comment: 
 
-Filename: srpc/client.so
+Filename: srpc/client.pyd
 Comment: 
 
-Filename: srpc/protocol.so
+Filename: srpc/protocol.pyd
 Comment: 
 
-Filename: srpc/ring.so
+Filename: srpc/ring.pyd
 Comment: 
 
-Filename: srpc/server.so
+Filename: srpc/server.pyd
 Comment: 
 
-Filename: srpc/ulog.so
+Filename: srpc/ulog.pyd
 Comment: 
 
 Zip file comment:
```

## Comparing `srpc-4.2.12.dist-info/METADATA` & `srpc-4.2.9.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-Metadata-Version: 2.1
-Name: srpc
-Version: 4.2.12
-Summary: Dream It Possible!
-Author-email: YL <fengyl@pku.edu.cn>
-License: MIT License
-        
-        Copyright (c) 2021 YL
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: homepage, https://gitee.com
-Project-URL: documentation, https://gitee.com
-Project-URL: bugs, https://gitee.com
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: Chinese (Simplified)
-Classifier: Natural Language :: English
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: msgpack (>=1.0.0)
-Requires-Dist: numpy (>=1.20.0)
-
+Metadata-Version: 2.1
+Name: srpc
+Version: 4.2.9
+Summary: Dream It Possible!
+Author-email: YL <fengyl@pku.edu.cn>
+License: MIT License
+        
+        Copyright (c) 2021 YL
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: homepage, https://gitee.com
+Project-URL: documentation, https://gitee.com
+Project-URL: bugs, https://gitee.com
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: Chinese (Simplified)
+Classifier: Natural Language :: English
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Physics
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: msgpack (>=1.0.0)
+Requires-Dist: numpy (>=1.20.0)
+
```

