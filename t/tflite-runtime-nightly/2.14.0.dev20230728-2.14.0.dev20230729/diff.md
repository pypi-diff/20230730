# Comparing `tmp/tflite_runtime_nightly-2.14.0.dev20230728-cp39-cp39-manylinux_2_34_armv7l.whl.zip` & `tmp/tflite_runtime_nightly-2.14.0.dev20230729-cp39-cp39-manylinux_2_34_armv7l.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 1819230 bytes, number of entries: 9
--rw-rw-r--  2.0 unx       80 b- defN 23-Jul-29 04:56 tflite_runtime/__init__.py
--rwxrwxr-x  2.0 unx  4918068 b- defN 23-Jul-29 04:58 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so
--rw-rw-r--  2.0 unx    38775 b- defN 23-Jul-29 04:56 tflite_runtime/interpreter.py
--rw-rw-r--  2.0 unx     1542 b- defN 23-Jul-29 04:56 tflite_runtime/metrics_interface.py
--rw-rw-r--  2.0 unx     2048 b- defN 23-Jul-29 04:56 tflite_runtime/metrics_portable.py
--rw-rw-r--  2.0 unx     1441 b- defN 23-Jul-29 04:58 tflite_runtime_nightly-2.14.0.dev20230728.dist-info/METADATA
--rw-rw-r--  2.0 unx      112 b- defN 23-Jul-29 04:58 tflite_runtime_nightly-2.14.0.dev20230728.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Jul-29 04:58 tflite_runtime_nightly-2.14.0.dev20230728.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      878 b- defN 23-Jul-29 04:58 tflite_runtime_nightly-2.14.0.dev20230728.dist-info/RECORD
-9 files, 4962959 bytes uncompressed, 1817684 bytes compressed:  63.4%
+Zip file size: 1819228 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx       80 b- defN 23-Jul-30 05:00 tflite_runtime/__init__.py
+-rwxrwxr-x  2.0 unx  4918068 b- defN 23-Jul-30 05:02 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so
+-rw-rw-r--  2.0 unx    38775 b- defN 23-Jul-30 05:00 tflite_runtime/interpreter.py
+-rw-rw-r--  2.0 unx     1542 b- defN 23-Jul-30 05:00 tflite_runtime/metrics_interface.py
+-rw-rw-r--  2.0 unx     2048 b- defN 23-Jul-30 05:00 tflite_runtime/metrics_portable.py
+-rw-rw-r--  2.0 unx     1441 b- defN 23-Jul-30 05:02 tflite_runtime_nightly-2.14.0.dev20230729.dist-info/METADATA
+-rw-rw-r--  2.0 unx      112 b- defN 23-Jul-30 05:02 tflite_runtime_nightly-2.14.0.dev20230729.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Jul-30 05:02 tflite_runtime_nightly-2.14.0.dev20230729.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      878 b- defN 23-Jul-30 05:02 tflite_runtime_nightly-2.14.0.dev20230729.dist-info/RECORD
+9 files, 4962959 bytes uncompressed, 1817682 bytes compressed:  63.4%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: tflite_runtime/metrics_interface.py
 Comment: 
 
 Filename: tflite_runtime/metrics_portable.py
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230728.dist-info/METADATA
+Filename: tflite_runtime_nightly-2.14.0.dev20230729.dist-info/METADATA
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230728.dist-info/WHEEL
+Filename: tflite_runtime_nightly-2.14.0.dev20230729.dist-info/WHEEL
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230728.dist-info/top_level.txt
+Filename: tflite_runtime_nightly-2.14.0.dev20230729.dist-info/top_level.txt
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230728.dist-info/RECORD
+Filename: tflite_runtime_nightly-2.14.0.dev20230729.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tflite_runtime/__init__.py

```diff
@@ -1,2 +1,2 @@
-__version__ = '2.14.0dev20230728'
-__git_version__ = '0.6.0-151400-g29e38e026a6'
+__version__ = '2.14.0dev20230729'
+__git_version__ = '0.6.0-151408-g27c7c96431b'
```

## Comparing `tflite_runtime_nightly-2.14.0.dev20230728.dist-info/METADATA` & `tflite_runtime_nightly-2.14.0.dev20230729.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tflite-runtime-nightly
-Version: 2.14.0.dev20230728
+Version: 2.14.0.dev20230729
 Summary: TensorFlow Lite is for mobile and embedded devices.
 Home-page: https://www.tensorflow.org/lite/
 Author: Google, LLC
 Author-email: packages@tensorflow.org
 License: Apache 2.0
 Keywords: tflite tensorflow tensor machine learning
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `tflite_runtime_nightly-2.14.0.dev20230728.dist-info/RECORD` & `tflite_runtime_nightly-2.14.0.dev20230729.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-tflite_runtime/__init__.py,sha256=f_nXK0S3xXGfENsgYsg39sOVckjHTH4wWLhtRUZMSMo,80
+tflite_runtime/__init__.py,sha256=WHQi_W4oBQNsDpgctJw8Wyuakn-vm91V4U3UiKota5Y,80
 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so,sha256=jcIm2EFwR1IZu_AqW2C-JitPSnwvYWVChkV9heldnkc,4918068
 tflite_runtime/interpreter.py,sha256=WdMKqxuFdoGPyOKoCsZsHbvsVQXs_81OrG7VUE8p5JU,38775
 tflite_runtime/metrics_interface.py,sha256=dVu6SmbnQUntPgE5o6BxHVMyemwli-7F6tDfVMGrlYI,1542
 tflite_runtime/metrics_portable.py,sha256=YBiMNokP9JtoQaUcCRRY1T_iFSZGeWCjr6L0iUR6eY8,2048
-tflite_runtime_nightly-2.14.0.dev20230728.dist-info/METADATA,sha256=COKhiwLJ_reaJJfRc3HyOEzpCEMz4b0Nt0zjVWawzIk,1441
-tflite_runtime_nightly-2.14.0.dev20230728.dist-info/WHEEL,sha256=6vmKKIEiIbM5qK-J-kFcH4n3gV7-okc3tX2BlV4kvDg,112
-tflite_runtime_nightly-2.14.0.dev20230728.dist-info/top_level.txt,sha256=uNbSt_JkE5qb43UeqR4Wx6_Y6A5613g6gtS49welF08,15
-tflite_runtime_nightly-2.14.0.dev20230728.dist-info/RECORD,,
+tflite_runtime_nightly-2.14.0.dev20230729.dist-info/METADATA,sha256=7TVleIVGuvcfaiitxkkFSRm0q2q-Dn1kutYoE4VoC3Q,1441
+tflite_runtime_nightly-2.14.0.dev20230729.dist-info/WHEEL,sha256=6vmKKIEiIbM5qK-J-kFcH4n3gV7-okc3tX2BlV4kvDg,112
+tflite_runtime_nightly-2.14.0.dev20230729.dist-info/top_level.txt,sha256=uNbSt_JkE5qb43UeqR4Wx6_Y6A5613g6gtS49welF08,15
+tflite_runtime_nightly-2.14.0.dev20230729.dist-info/RECORD,,
```

