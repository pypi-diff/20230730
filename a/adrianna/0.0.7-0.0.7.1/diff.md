# Comparing `tmp/adrianna-0.0.7-py3-none-any.whl.zip` & `tmp/adrianna-0.0.7.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3272 bytes, number of entries: 6
+Zip file size: 3509 bytes, number of entries: 6
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jul-29 23:04 adrianna/__init__.py
--rw-rw-r--  2.0 unx     1497 b- defN 23-Jul-29 23:18 adrianna-0.0.7.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2645 b- defN 23-Jul-29 23:18 adrianna-0.0.7.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-29 23:18 adrianna-0.0.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-Jul-29 23:18 adrianna-0.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      464 b- defN 23-Jul-29 23:18 adrianna-0.0.7.dist-info/RECORD
-6 files, 4707 bytes uncompressed, 2426 bytes compressed:  48.5%
+-rw-rw-r--  2.0 unx     1497 b- defN 23-Jul-29 23:22 adrianna-0.0.7.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3268 b- defN 23-Jul-29 23:22 adrianna-0.0.7.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-29 23:22 adrianna-0.0.7.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-Jul-29 23:22 adrianna-0.0.7.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      474 b- defN 23-Jul-29 23:23 adrianna-0.0.7.1.dist-info/RECORD
+6 files, 5340 bytes uncompressed, 2643 bytes compressed:  50.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: adrianna/__init__.py
 Comment: 
 
-Filename: adrianna-0.0.7.dist-info/LICENSE
+Filename: adrianna-0.0.7.1.dist-info/LICENSE
 Comment: 
 
-Filename: adrianna-0.0.7.dist-info/METADATA
+Filename: adrianna-0.0.7.1.dist-info/METADATA
 Comment: 
 
-Filename: adrianna-0.0.7.dist-info/WHEEL
+Filename: adrianna-0.0.7.1.dist-info/WHEEL
 Comment: 
 
-Filename: adrianna-0.0.7.dist-info/top_level.txt
+Filename: adrianna-0.0.7.1.dist-info/top_level.txt
 Comment: 
 
-Filename: adrianna-0.0.7.dist-info/RECORD
+Filename: adrianna-0.0.7.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `adrianna-0.0.7.dist-info/LICENSE` & `adrianna-0.0.7.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `adrianna-0.0.7.dist-info/METADATA` & `adrianna-0.0.7.1.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adrianna
-Version: 0.0.7
+Version: 0.0.7.1
 Summary: lib for development with machine learning
 Home-page: https://github.com/reinanbr/adriana
 Author: Reinan Br
 Author-email: slimchatuba@gmail.com
 License: MIT License
 Keywords: ia machine learning math
 Description-Content-Type: text/markdown
@@ -76,7 +76,40 @@
     # Fazendo previsões
     predictions = neural_net.predict(X)
     predictions = np.round(predictions).astype(int)
     print("Predictions:")
     print(predictions)
 
 ```
+Results:
+
+```sh
+...
+Epoch 8000, Loss: 0.2617957
+Epoch 8100, Loss: 0.1830651
+Epoch 8200, Loss: 0.1800935
+Epoch 8300, Loss: 0.2585192
+Epoch 8400, Loss: 0.3310709
+Epoch 8500, Loss: 0.3215849
+Epoch 8600, Loss: 0.1803035
+Epoch 8700, Loss: 0.1802555
+Epoch 8800, Loss: 0.1807692
+Epoch 8900, Loss: 0.3312975
+Epoch 9000, Loss: 0.1800601
+Epoch 9100, Loss: 0.2642676
+Epoch 9200, Loss: 0.1930688
+Epoch 9300, Loss: 0.3279387
+Epoch 9400, Loss: 0.1871483
+Epoch 9500, Loss: 0.1809427
+Epoch 9600, Loss: 0.2635577
+Epoch 9700, Loss: 0.1855325
+Epoch 9800, Loss: 0.1796770
+Epoch 9900, Loss: 0.1800897
+
+Predictions:
+[[1]
+ [0]
+ [1]
+ [1]]
+
+
+```
```

