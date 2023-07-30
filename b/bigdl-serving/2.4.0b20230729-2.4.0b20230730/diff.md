# Comparing `tmp/bigdl_serving-2.4.0b20230729-py2.py3-none-any.whl.zip` & `tmp/bigdl_serving-2.4.0b20230730-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 21607 bytes, number of entries: 20
+Zip file size: 21602 bytes, number of entries: 20
 -rw-------  2.0 unx      940 b- defN 23-Jul-28 02:56 bigdl/__init__.py
 -rw-------  2.0 unx     9965 b- defN 23-Jul-28 02:56 bigdl/serving/client.py
 -rw-------  2.0 unx     2268 b- defN 23-Jul-28 02:56 bigdl/serving/env.py
 -rw-------  2.0 unx     1375 b- defN 23-Jul-28 02:56 bigdl/serving/log4Error.py
 -rw-------  2.0 unx     4990 b- defN 23-Jul-28 02:56 bigdl/serving/schema.py
 -rw-------  2.0 unx     4980 b- defN 23-Jul-28 02:56 bigdl/serving/kafka/client.py
 -rw-------  2.0 unx     1864 b- defN 23-Jul-28 02:56 bigdl/serving/kafka/kafka_example.py
 -rw-------  2.0 unx       92 b- defN 23-Jul-28 02:56 bigdl/share/serving/cluster-serving-py-setup.py
 -rw-------  2.0 unx     4970 b- defN 23-Jul-28 02:56 bigdl/share/serving/perf-benchmark/e2e_throughput.py
--rwxrwxr-x  2.0 unx      644 b- defN 23-Jul-28 02:56 bigdl_serving-2.4.0b20230729.data/scripts/cluster-serving-init
--rwxr-xr-x  2.0 unx       82 b- defN 23-Jul-29 13:18 bigdl_serving-2.4.0b20230729.data/scripts/cluster-serving-py-setup.py
--rwxrwxr-x  2.0 unx      155 b- defN 23-Jul-28 02:56 bigdl_serving-2.4.0b20230729.data/scripts/cluster-serving-shutdown
--rwxrwxr-x  2.0 unx     3177 b- defN 23-Jul-28 02:56 bigdl_serving-2.4.0b20230729.data/scripts/cluster-serving-start
--rwxrwxr-x  2.0 unx     5103 b- defN 23-Jul-28 02:56 bigdl_serving-2.4.0b20230729.data/scripts/cluster-with-numactl.sh
--rwxrwxr-x  2.0 unx     1300 b- defN 23-Jul-28 02:56 bigdl_serving-2.4.0b20230729.data/scripts/config.yaml
--rwxrwxr-x  2.0 unx     2425 b- defN 23-Jul-28 02:56 bigdl_serving-2.4.0b20230729.data/scripts/download-serving-jar.sh
--rw-------  2.0 unx     1051 b- defN 23-Jul-29 13:18 bigdl_serving-2.4.0b20230729.dist-info/METADATA
--rw-------  2.0 unx      110 b- defN 23-Jul-29 13:18 bigdl_serving-2.4.0b20230729.dist-info/WHEEL
--rw-------  2.0 unx        7 b- defN 23-Jul-29 13:18 bigdl_serving-2.4.0b20230729.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1979 b- defN 23-Jul-29 13:18 bigdl_serving-2.4.0b20230729.dist-info/RECORD
-20 files, 47477 bytes uncompressed, 18257 bytes compressed:  61.5%
+-rwxrwxr-x  2.0 unx      644 b- defN 23-Jul-28 02:56 bigdl_serving-2.4.0b20230730.data/scripts/cluster-serving-init
+-rwxr-xr-x  2.0 unx       82 b- defN 23-Jul-30 13:17 bigdl_serving-2.4.0b20230730.data/scripts/cluster-serving-py-setup.py
+-rwxrwxr-x  2.0 unx      155 b- defN 23-Jul-28 02:56 bigdl_serving-2.4.0b20230730.data/scripts/cluster-serving-shutdown
+-rwxrwxr-x  2.0 unx     3177 b- defN 23-Jul-28 02:56 bigdl_serving-2.4.0b20230730.data/scripts/cluster-serving-start
+-rwxrwxr-x  2.0 unx     5103 b- defN 23-Jul-28 02:56 bigdl_serving-2.4.0b20230730.data/scripts/cluster-with-numactl.sh
+-rwxrwxr-x  2.0 unx     1300 b- defN 23-Jul-28 02:56 bigdl_serving-2.4.0b20230730.data/scripts/config.yaml
+-rwxrwxr-x  2.0 unx     2425 b- defN 23-Jul-28 02:56 bigdl_serving-2.4.0b20230730.data/scripts/download-serving-jar.sh
+-rw-------  2.0 unx     1051 b- defN 23-Jul-30 13:17 bigdl_serving-2.4.0b20230730.dist-info/METADATA
+-rw-------  2.0 unx      110 b- defN 23-Jul-30 13:17 bigdl_serving-2.4.0b20230730.dist-info/WHEEL
+-rw-------  2.0 unx        7 b- defN 23-Jul-30 13:17 bigdl_serving-2.4.0b20230730.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1979 b- defN 23-Jul-30 13:17 bigdl_serving-2.4.0b20230730.dist-info/RECORD
+20 files, 47477 bytes uncompressed, 18252 bytes compressed:  61.6%
```

## zipnote {}

```diff
@@ -21,41 +21,41 @@
 
 Filename: bigdl/share/serving/cluster-serving-py-setup.py
 Comment: 
 
 Filename: bigdl/share/serving/perf-benchmark/e2e_throughput.py
 Comment: 
 
-Filename: bigdl_serving-2.4.0b20230729.data/scripts/cluster-serving-init
+Filename: bigdl_serving-2.4.0b20230730.data/scripts/cluster-serving-init
 Comment: 
 
-Filename: bigdl_serving-2.4.0b20230729.data/scripts/cluster-serving-py-setup.py
+Filename: bigdl_serving-2.4.0b20230730.data/scripts/cluster-serving-py-setup.py
 Comment: 
 
-Filename: bigdl_serving-2.4.0b20230729.data/scripts/cluster-serving-shutdown
+Filename: bigdl_serving-2.4.0b20230730.data/scripts/cluster-serving-shutdown
 Comment: 
 
-Filename: bigdl_serving-2.4.0b20230729.data/scripts/cluster-serving-start
+Filename: bigdl_serving-2.4.0b20230730.data/scripts/cluster-serving-start
 Comment: 
 
-Filename: bigdl_serving-2.4.0b20230729.data/scripts/cluster-with-numactl.sh
+Filename: bigdl_serving-2.4.0b20230730.data/scripts/cluster-with-numactl.sh
 Comment: 
 
-Filename: bigdl_serving-2.4.0b20230729.data/scripts/config.yaml
+Filename: bigdl_serving-2.4.0b20230730.data/scripts/config.yaml
 Comment: 
 
-Filename: bigdl_serving-2.4.0b20230729.data/scripts/download-serving-jar.sh
+Filename: bigdl_serving-2.4.0b20230730.data/scripts/download-serving-jar.sh
 Comment: 
 
-Filename: bigdl_serving-2.4.0b20230729.dist-info/METADATA
+Filename: bigdl_serving-2.4.0b20230730.dist-info/METADATA
 Comment: 
 
-Filename: bigdl_serving-2.4.0b20230729.dist-info/WHEEL
+Filename: bigdl_serving-2.4.0b20230730.dist-info/WHEEL
 Comment: 
 
-Filename: bigdl_serving-2.4.0b20230729.dist-info/top_level.txt
+Filename: bigdl_serving-2.4.0b20230730.dist-info/top_level.txt
 Comment: 
 
-Filename: bigdl_serving-2.4.0b20230729.dist-info/RECORD
+Filename: bigdl_serving-2.4.0b20230730.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `bigdl_serving-2.4.0b20230729.data/scripts/cluster-serving-init` & `bigdl_serving-2.4.0b20230730.data/scripts/cluster-serving-init`

 * *Files identical despite different names*

## Comparing `bigdl_serving-2.4.0b20230729.data/scripts/cluster-serving-start` & `bigdl_serving-2.4.0b20230730.data/scripts/cluster-serving-start`

 * *Files identical despite different names*

## Comparing `bigdl_serving-2.4.0b20230729.data/scripts/cluster-with-numactl.sh` & `bigdl_serving-2.4.0b20230730.data/scripts/cluster-with-numactl.sh`

 * *Files identical despite different names*

## Comparing `bigdl_serving-2.4.0b20230729.data/scripts/config.yaml` & `bigdl_serving-2.4.0b20230730.data/scripts/config.yaml`

 * *Files identical despite different names*

## Comparing `bigdl_serving-2.4.0b20230729.data/scripts/download-serving-jar.sh` & `bigdl_serving-2.4.0b20230730.data/scripts/download-serving-jar.sh`

 * *Files identical despite different names*

## Comparing `bigdl_serving-2.4.0b20230729.dist-info/METADATA` & `bigdl_serving-2.4.0b20230730.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigdl-serving
-Version: 2.4.0b20230729
+Version: 2.4.0b20230730
 Summary: Distributed and Automated Model Inference on Big Data Streaming Frameworks
 Home-page: https://github.com/intel-analytics/BigDL
 Author: BigDL Authors
 Author-email: bigdl-user-group@googlegroups.com
 License: Apache License, Version 2.0
 Platform: mac
 Platform: linux
```

