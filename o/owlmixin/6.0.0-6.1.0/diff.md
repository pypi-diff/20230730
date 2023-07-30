# Comparing `tmp/owlmixin-6.0.0-py3-none-any.whl.zip` & `tmp/owlmixin-6.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 20324 bytes, number of entries: 12
+Zip file size: 20333 bytes, number of entries: 12
 -rw-r--r--  2.0 fat    34064 b- defN 80-Jan-01 00:00 owlmixin/__init__.py
 -rw-r--r--  2.0 fat     3228 b- defN 80-Jan-01 00:00 owlmixin/errors.py
 -rw-r--r--  2.0 fat    26595 b- defN 80-Jan-01 00:00 owlmixin/owlcollections.py
 -rw-r--r--  2.0 fat     1450 b- defN 80-Jan-01 00:00 owlmixin/owlenum.py
 -rw-r--r--  2.0 fat     4413 b- defN 80-Jan-01 00:00 owlmixin/owloption.py
 -rw-r--r--  2.0 fat      796 b- defN 80-Jan-01 00:00 owlmixin/samples.py
 -rw-r--r--  2.0 fat    15548 b- defN 80-Jan-01 00:00 owlmixin/transformers.py
 -rw-r--r--  2.0 fat     8093 b- defN 80-Jan-01 00:00 owlmixin/util.py
--rw-r--r--  2.0 fat     1071 b- defN 80-Jan-01 00:00 owlmixin-6.0.0.dist-info/LICENSE
-?rw-r--r--  2.0 fat       83 b- defN 16-Jan-01 00:00 owlmixin-6.0.0.dist-info/WHEEL
-?rw-r--r--  2.0 fat     5773 b- defN 16-Jan-01 00:00 owlmixin-6.0.0.dist-info/METADATA
-?rw-r--r--  2.0 fat      919 b- defN 16-Jan-01 00:00 owlmixin-6.0.0.dist-info/RECORD
-12 files, 102033 bytes uncompressed, 18812 bytes compressed:  81.6%
+-rw-r--r--  2.0 fat     1071 b- defN 80-Jan-01 00:00 owlmixin-6.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 fat     5824 b- defN 80-Jan-01 00:00 owlmixin-6.1.0.dist-info/METADATA
+-rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 owlmixin-6.1.0.dist-info/WHEEL
+?rw-r--r--  2.0 fat      919 b- defN 16-Jan-01 00:00 owlmixin-6.1.0.dist-info/RECORD
+12 files, 102089 bytes uncompressed, 18821 bytes compressed:  81.6%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: owlmixin/transformers.py
 Comment: 
 
 Filename: owlmixin/util.py
 Comment: 
 
-Filename: owlmixin-6.0.0.dist-info/LICENSE
+Filename: owlmixin-6.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: owlmixin-6.0.0.dist-info/WHEEL
+Filename: owlmixin-6.1.0.dist-info/METADATA
 Comment: 
 
-Filename: owlmixin-6.0.0.dist-info/METADATA
+Filename: owlmixin-6.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: owlmixin-6.0.0.dist-info/RECORD
+Filename: owlmixin-6.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `owlmixin-6.0.0.dist-info/LICENSE` & `owlmixin-6.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `owlmixin-6.0.0.dist-info/METADATA` & `owlmixin-6.1.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: owlmixin
-Version: 6.0.0
+Version: 6.1.0
 Summary: Mixin which converts ``data class instance`` and others each other more simple.
 Home-page: https://github.com/tadashi-aikawa/owlmixin
 License: MIT
 Keywords: dict,json,yaml,parser,mixin
 Author: tadashi-aikawa
 Author-email: syou.maman@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
-Requires-Dist: pyyaml (>=5.1,<6.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
 Project-URL: Documentation, https://tadashi-aikawa.github.io/owlmixin/
 Project-URL: Repository, https://github.com/tadashi-aikawa/owlmixin
 Description-Content-Type: text/markdown
 
 OwlMixin
 ========
```

## Comparing `owlmixin-6.0.0.dist-info/RECORD` & `owlmixin-6.1.0.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -2,11 +2,11 @@
 owlmixin/errors.py,sha256=k_sfJ0EOdgM-w3AAt0Z8zQ8Hor1qeuRuJV9XWtzAbx4,3228
 owlmixin/owlcollections.py,sha256=3KHvNUH0Da4VPNRNPCD6aZO-iI-m15fZTbBU-DLBJV8,26595
 owlmixin/owlenum.py,sha256=wBZYkjQtPrOQ18XLTH83cQl_TwCvol8tJYPIRQjJf4U,1450
 owlmixin/owloption.py,sha256=MNHMCOE3Rdhu297_0R4KGG2oQpaJoLU_iXrrui5bvRE,4413
 owlmixin/samples.py,sha256=410ugbfgk-MRMhYLL8hvTcaVdBFwCJHJFWH9mLtTFSw,796
 owlmixin/transformers.py,sha256=OpAeF4UKMoZkq7-RU585v0UkAgu2pVFyMB6Xf65jTAE,15548
 owlmixin/util.py,sha256=1W812EoceklAwQS-0Pmv_sEoHCoqcysio6DocEU_6Hc,8093
-owlmixin-6.0.0.dist-info/LICENSE,sha256=m8HbUtjSkJ7qDYcQDtCkQBGvx-w0aL-UEUiA2J0tSrg,1071
-owlmixin-6.0.0.dist-info/WHEEL,sha256=DA86_h4QwwzGeRoz62o1svYt5kGEXpoUTuTtwzoTb30,83
-owlmixin-6.0.0.dist-info/METADATA,sha256=U44S_67UMZqVA093vT7khHpFC5qz32IOCtC8EZw4svk,5773
-owlmixin-6.0.0.dist-info/RECORD,,
+owlmixin-6.1.0.dist-info/LICENSE,sha256=m8HbUtjSkJ7qDYcQDtCkQBGvx-w0aL-UEUiA2J0tSrg,1071
+owlmixin-6.1.0.dist-info/METADATA,sha256=RaBUSyfd28Fj5qIuCEmCVdHSNWOrhna6jeYBMw8a118,5824
+owlmixin-6.1.0.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+owlmixin-6.1.0.dist-info/RECORD,,
```

