# Comparing `tmp/pyarmor.cli.core.themida-4.3.0-cp39-none-any.whl.zip` & `tmp/pyarmor.cli.core.themida-4.3.dev1-cp39-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7857091 bytes, number of entries: 7
--rw-r--r--  2.0 unx       22 b- defN 23-Jul-29 00:47 pyarmor/cli/core/themida/__init__.py
--rwxr-xr-x  2.0 unx  3786782 b- defN 23-Jul-29 00:47 pyarmor/cli/core/themida/windows/x86/pyarmor_runtime.pyd
--rwxr-xr-x  2.0 unx  5015568 b- defN 23-Jul-29 00:47 pyarmor/cli/core/themida/windows/x86_64/pyarmor_runtime.pyd
--rw-r--r--  2.0 unx      809 b- defN 23-Jul-29 00:47 pyarmor.cli.core.themida-4.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       93 b- defN 23-Jul-29 00:47 pyarmor.cli.core.themida-4.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-29 00:47 pyarmor.cli.core.themida-4.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      690 b- defN 23-Jul-29 00:47 pyarmor.cli.core.themida-4.3.0.dist-info/RECORD
-7 files, 8803972 bytes uncompressed, 7855843 bytes compressed:  10.8%
+Zip file size: 7722018 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       25 b- defN 23-Jul-23 12:59 pyarmor/cli/core/themida/__init__.py
+-rwxr-xr-x  2.0 unx  3787806 b- defN 23-Jul-23 12:59 pyarmor/cli/core/themida/windows/x86/pyarmor_runtime.pyd
+-rwxr-xr-x  2.0 unx  4879888 b- defN 23-Jul-23 12:59 pyarmor/cli/core/themida/windows/x86_64/pyarmor_runtime.pyd
+-rw-r--r--  2.0 unx      812 b- defN 23-Jul-23 12:59 pyarmor.cli.core.themida-4.3.dev1.dist-info/METADATA
+-rw-r--r--  2.0 unx       93 b- defN 23-Jul-23 12:59 pyarmor.cli.core.themida-4.3.dev1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-23 12:59 pyarmor.cli.core.themida-4.3.dev1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      702 b- defN 23-Jul-23 12:59 pyarmor.cli.core.themida-4.3.dev1.dist-info/RECORD
+7 files, 8669334 bytes uncompressed, 7720746 bytes compressed:  10.9%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: pyarmor/cli/core/themida/windows/x86/pyarmor_runtime.pyd
 Comment: 
 
 Filename: pyarmor/cli/core/themida/windows/x86_64/pyarmor_runtime.pyd
 Comment: 
 
-Filename: pyarmor.cli.core.themida-4.3.0.dist-info/METADATA
+Filename: pyarmor.cli.core.themida-4.3.dev1.dist-info/METADATA
 Comment: 
 
-Filename: pyarmor.cli.core.themida-4.3.0.dist-info/WHEEL
+Filename: pyarmor.cli.core.themida-4.3.dev1.dist-info/WHEEL
 Comment: 
 
-Filename: pyarmor.cli.core.themida-4.3.0.dist-info/top_level.txt
+Filename: pyarmor.cli.core.themida-4.3.dev1.dist-info/top_level.txt
 Comment: 
 
-Filename: pyarmor.cli.core.themida-4.3.0.dist-info/RECORD
+Filename: pyarmor.cli.core.themida-4.3.dev1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyarmor/cli/core/themida/__init__.py

```diff
@@ -1 +1 @@
-__VERSION__ = '4.3.0'
+__VERSION__ = '4.3.dev1'
```

## Comparing `pyarmor.cli.core.themida-4.3.0.dist-info/METADATA` & `pyarmor.cli.core.themida-4.3.dev1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarmor.cli.core.themida
-Version: 4.3.0
+Version: 4.3.dev1
 Summary: Provide pre-built extension module `pyarmor_runtime` protected by Themida for Pyarmor
 Home-page: https://github.com/dashingsoft/pyarmor
 Author: Jondy Zhao
 Author-email: pyarmor@163.com
 License: Free To Use But Restricted
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `pyarmor.cli.core.themida-4.3.0.dist-info/RECORD` & `pyarmor.cli.core.themida-4.3.dev1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-pyarmor/cli/core/themida/__init__.py,sha256=CDPRinTnSD2xTY7mjTAtyXcMyIiRXVKcho3q-rEYva8,22
-pyarmor/cli/core/themida/windows/x86/pyarmor_runtime.pyd,sha256=fV7RZIftodLmir_57-WkUhBmXsHr0cSDj2uVMD6rJq4,3786782
-pyarmor/cli/core/themida/windows/x86_64/pyarmor_runtime.pyd,sha256=15sgCrgjXByYgBj8x7PZRo5HaX-J4UiwzGVeTB3_dl0,5015568
-pyarmor.cli.core.themida-4.3.0.dist-info/METADATA,sha256=yZa2IQGsO7GSztnGgp8vWEhrNOVLLO0sAqb6oFdaf68,809
-pyarmor.cli.core.themida-4.3.0.dist-info/WHEEL,sha256=QbbyyBnlPXzoGKd-349G69XkCwSd1NFnt4kuAN58gNs,93
-pyarmor.cli.core.themida-4.3.0.dist-info/top_level.txt,sha256=UE1ovZ_90YzwF_lZ3LV7o8HKLe-RgzUaUUvdH5UTUus,8
-pyarmor.cli.core.themida-4.3.0.dist-info/RECORD,,
+pyarmor/cli/core/themida/__init__.py,sha256=-ZsoB3RONIDHw9_pOlDaLpAfTbSGcr3JIbok364TpcQ,25
+pyarmor/cli/core/themida/windows/x86/pyarmor_runtime.pyd,sha256=VFXdP4Q3srnpZUFoLYyBkf-C4O57uZhUqdMjZ-Ukx7Y,3787806
+pyarmor/cli/core/themida/windows/x86_64/pyarmor_runtime.pyd,sha256=kKj6zogQ42Rovho6SuL2_J8MBIEwLQnKXTPgSkjKMMs,4879888
+pyarmor.cli.core.themida-4.3.dev1.dist-info/METADATA,sha256=JL6F-FkwVmypgDmLPsY0yvLur9AqXZIfMB-oT6CKNqI,812
+pyarmor.cli.core.themida-4.3.dev1.dist-info/WHEEL,sha256=QbbyyBnlPXzoGKd-349G69XkCwSd1NFnt4kuAN58gNs,93
+pyarmor.cli.core.themida-4.3.dev1.dist-info/top_level.txt,sha256=UE1ovZ_90YzwF_lZ3LV7o8HKLe-RgzUaUUvdH5UTUus,8
+pyarmor.cli.core.themida-4.3.dev1.dist-info/RECORD,,
```

