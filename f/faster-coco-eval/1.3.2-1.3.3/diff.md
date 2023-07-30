# Comparing `tmp/faster-coco-eval-1.3.2.tar.gz` & `tmp/faster-coco-eval-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faster-coco-eval-1.3.2.tar", last modified: Sat May 20 11:10:37 2023, max compression
+gzip compressed data, was "faster-coco-eval-1.3.3.tar", last modified: Sun Jul 30 17:20:32 2023, max compression
```

## Comparing `faster-coco-eval-1.3.2.tar` & `faster-coco-eval-1.3.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 11:10:37.729842 faster-coco-eval-1.3.2/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4833 2023-05-20 11:10:37.729842 faster-coco-eval-1.3.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4166 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 11:10:37.629842 faster-coco-eval-1.3.2/csrc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 11:10:37.649842 faster-coco-eval-1.3.2/csrc/faster_eval_api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 11:10:37.649842 faster-coco-eval-1.3.2/csrc/faster_eval_api/coco_eval/
--rw-r--r--   0 root         (0) root         (0)    25495 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/csrc/faster_eval_api/coco_eval/cocoeval.cpp
--rw-r--r--   0 root         (0) root         (0)     3968 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/csrc/faster_eval_api/coco_eval/cocoeval.h
--rw-r--r--   0 root         (0) root         (0)     1630 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/csrc/faster_eval_api/faster_eval_api.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 11:10:37.629842 faster-coco-eval-1.3.2/csrc/mask/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 11:10:37.669842 faster-coco-eval-1.3.2/csrc/mask/common/
--rw-r--r--   0 root         (0) root         (0)     8308 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/csrc/mask/common/maskApi.c
--rw-r--r--   0 root         (0) root         (0)     2176 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/csrc/mask/common/maskApi.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 11:10:37.669842 faster-coco-eval-1.3.2/csrc/mask/pycocotools/
--rw-r--r--   0 root         (0) root         (0)   655761 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/csrc/mask/pycocotools/_mask.c
--rw-r--r--   0 root         (0) root         (0)    11440 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/csrc/mask/pycocotools/_mask.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 11:10:37.679842 faster-coco-eval-1.3.2/faster_coco_eval/
--rw-r--r--   0 root         (0) root         (0)      123 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/faster_coco_eval/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 11:10:37.689842 faster-coco-eval-1.3.2/faster_coco_eval/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/faster_coco_eval/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15122 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/faster_coco_eval/core/coco.py
--rw-r--r--   0 root         (0) root         (0)    25709 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/faster_coco_eval/core/cocoeval.py
--rw-r--r--   0 root         (0) root         (0)    12261 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/faster_coco_eval/core/faster_eval_api.py
--rw-r--r--   0 root         (0) root         (0)     3074 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/faster_coco_eval/core/mask.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 11:10:37.729842 faster-coco-eval-1.3.2/faster_coco_eval/extra/
--rw-r--r--   0 root         (0) root         (0)       62 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/faster_coco_eval/extra/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3411 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/faster_coco_eval/extra/curves.py
--rw-r--r--   0 root         (0) root         (0)     9288 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/faster_coco_eval/extra/display.py
--rw-r--r--   0 root         (0) root         (0)     1366 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/faster_coco_eval/extra/extra.py
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/faster_coco_eval/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 11:10:37.679842 faster-coco-eval-1.3.2/faster_coco_eval.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4833 2023-05-20 11:10:37.000000 faster-coco-eval-1.3.2/faster_coco_eval.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      855 2023-05-20 11:10:37.000000 faster-coco-eval-1.3.2/faster_coco_eval.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-20 11:10:37.000000 faster-coco-eval-1.3.2/faster_coco_eval.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-20 11:10:37.000000 faster-coco-eval-1.3.2/faster_coco_eval.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-05-20 11:10:37.000000 faster-coco-eval-1.3.2/faster_coco_eval.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      175 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-20 11:10:37.729842 faster-coco-eval-1.3.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     5851 2023-05-20 11:10:16.000000 faster-coco-eval-1.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 17:20:32.843786 faster-coco-eval-1.3.3/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-30 17:20:22.000000 faster-coco-eval-1.3.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-30 17:20:22.000000 faster-coco-eval-1.3.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5041 2023-07-30 17:20:32.843786 faster-coco-eval-1.3.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4382 2023-07-30 17:20:22.000000 faster-coco-eval-1.3.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 17:20:32.839786 faster-coco-eval-1.3.3/csrc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 17:20:32.843786 faster-coco-eval-1.3.3/csrc/faster_eval_api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 17:20:32.843786 faster-coco-eval-1.3.3/csrc/faster_eval_api/coco_eval/
+-rw-r--r--   0 root         (0) root         (0)    25495 2023-07-30 17:20:22.000000 faster-coco-eval-1.3.3/csrc/faster_eval_api/coco_eval/cocoeval.cpp
+-rw-r--r--   0 root         (0) root         (0)     3968 2023-07-30 17:20:22.000000 faster-coco-eval-1.3.3/csrc/faster_eval_api/coco_eval/cocoeval.h
+-rw-r--r--   0 root         (0) root         (0)     1630 2023-07-30 17:20:22.000000 faster-coco-eval-1.3.3/csrc/faster_eval_api/faster_eval_api.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 17:20:32.839786 faster-coco-eval-1.3.3/csrc/mask/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 17:20:32.843786 faster-coco-eval-1.3.3/csrc/mask/common/
+-rw-r--r--   0 root         (0) root         (0)     8308 2023-07-30 17:20:22.000000 faster-coco-eval-1.3.3/csrc/mask/common/maskApi.c
+-rw-r--r--   0 root         (0) root         (0)     2176 2023-07-30 17:20:22.000000 faster-coco-eval-1.3.3/csrc/mask/common/maskApi.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 17:20:32.843786 faster-coco-eval-1.3.3/csrc/mask/pycocotools/
+-rw-r--r--   0 root         (0) root         (0)   655761 2023-07-30 17:20:22.000000 faster-coco-eval-1.3.3/csrc/mask/pycocotools/_mask.c
+-rw-r--r--   0 root         (0) root         (0)    11397 2023-07-30 17:20:22.000000 faster-coco-eval-1.3.3/csrc/mask/pycocotools/_mask.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 17:20:32.843786 faster-coco-eval-1.3.3/faster_coco_eval/
+-rw-r--r--   0 root         (0) root         (0)      123 2023-07-30 17:20:22.000000 faster-coco-eval-1.3.3/faster_coco_eval/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 17:20:32.843786 faster-coco-eval-1.3.3/faster_coco_eval/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-30 17:20:22.000000 faster-coco-eval-1.3.3/faster_coco_eval/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15122 2023-07-30 17:20:22.000000 faster-coco-eval-1.3.3/faster_coco_eval/core/coco.py
+-rw-r--r--   0 root         (0) root         (0)    25709 2023-07-30 17:20:22.000000 faster-coco-eval-1.3.3/faster_coco_eval/core/cocoeval.py
+-rw-r--r--   0 root         (0) root         (0)    12617 2023-07-30 17:20:22.000000 faster-coco-eval-1.3.3/faster_coco_eval/core/faster_eval_api.py
+-rw-r--r--   0 root         (0) root         (0)     3074 2023-07-30 17:20:22.000000 faster-coco-eval-1.3.3/faster_coco_eval/core/mask.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 17:20:32.843786 faster-coco-eval-1.3.3/faster_coco_eval/extra/
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-30 17:20:22.000000 faster-coco-eval-1.3.3/faster_coco_eval/extra/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3411 2023-07-30 17:20:22.000000 faster-coco-eval-1.3.3/faster_coco_eval/extra/curves.py
+-rw-r--r--   0 root         (0) root         (0)     9295 2023-07-30 17:20:22.000000 faster-coco-eval-1.3.3/faster_coco_eval/extra/display.py
+-rw-r--r--   0 root         (0) root         (0)     1366 2023-07-30 17:20:22.000000 faster-coco-eval-1.3.3/faster_coco_eval/extra/extra.py
+-rw-r--r--   0 root         (0) root         (0)       47 2023-07-30 17:20:22.000000 faster-coco-eval-1.3.3/faster_coco_eval/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 17:20:32.843786 faster-coco-eval-1.3.3/faster_coco_eval.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5041 2023-07-30 17:20:32.000000 faster-coco-eval-1.3.3/faster_coco_eval.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      855 2023-07-30 17:20:32.000000 faster-coco-eval-1.3.3/faster_coco_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-30 17:20:32.000000 faster-coco-eval-1.3.3/faster_coco_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-30 17:20:32.000000 faster-coco-eval-1.3.3/faster_coco_eval.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-30 17:20:32.000000 faster-coco-eval-1.3.3/faster_coco_eval.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      176 2023-07-30 17:20:22.000000 faster-coco-eval-1.3.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-30 17:20:32.843786 faster-coco-eval-1.3.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     5921 2023-07-30 17:20:22.000000 faster-coco-eval-1.3.3/setup.py
```

### Comparing `faster-coco-eval-1.3.2/LICENSE` & `faster-coco-eval-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `faster-coco-eval-1.3.2/PKG-INFO` & `faster-coco-eval-1.3.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faster-coco-eval
-Version: 1.3.2
+Version: 1.3.3
 Summary: Faster interpretation of the original COCOEval
 Home-page: https://github.com/MiXaiLL76/faster_coco_eval
 Author: MiXaiLL76
 Author-email: mike.milos@yandex.ru
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -75,14 +75,22 @@
 ## Setup dependencies
 
 - numpy
 - plotly (optional if extra.Curve usage)  
 
 ## history
 
+### v1.3.3
+
+- [x] fix by ViTrox <https://github.com/vitrox-technologies/faster_coco_eval>
+    - missing file issue
+    - issue discovered by torchmetric
+    - fstring for python3.7
+    - Windows compilation
+
 ### v1.3.2
 
 - [x] rework math_matches function. moved to faster_eval_api
 - [x] Moved calculations from python to c++
 - [x] Separated extra classes
 - [x] Added new sample data
 - [x] append mIoU based on TP pred.
```

### Comparing `faster-coco-eval-1.3.2/README.md` & `faster-coco-eval-1.3.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,22 @@
 ## Setup dependencies
 
 - numpy
 - plotly (optional if extra.Curve usage)  
 
 ## history
 
+### v1.3.3
+
+- [x] fix by ViTrox <https://github.com/vitrox-technologies/faster_coco_eval>
+    - missing file issue
+    - issue discovered by torchmetric
+    - fstring for python3.7
+    - Windows compilation
+
 ### v1.3.2
 
 - [x] rework math_matches function. moved to faster_eval_api
 - [x] Moved calculations from python to c++
 - [x] Separated extra classes
 - [x] Added new sample data
 - [x] append mIoU based on TP pred.
```

### Comparing `faster-coco-eval-1.3.2/csrc/faster_eval_api/coco_eval/cocoeval.cpp` & `faster-coco-eval-1.3.3/csrc/faster_eval_api/coco_eval/cocoeval.cpp`

 * *Files identical despite different names*

### Comparing `faster-coco-eval-1.3.2/csrc/faster_eval_api/coco_eval/cocoeval.h` & `faster-coco-eval-1.3.3/csrc/faster_eval_api/coco_eval/cocoeval.h`

 * *Files identical despite different names*

### Comparing `faster-coco-eval-1.3.2/csrc/faster_eval_api/faster_eval_api.cpp` & `faster-coco-eval-1.3.3/csrc/faster_eval_api/faster_eval_api.cpp`

 * *Files identical despite different names*

### Comparing `faster-coco-eval-1.3.2/csrc/mask/common/maskApi.c` & `faster-coco-eval-1.3.3/csrc/mask/common/maskApi.c`

 * *Files identical despite different names*

### Comparing `faster-coco-eval-1.3.2/csrc/mask/common/maskApi.h` & `faster-coco-eval-1.3.3/csrc/mask/common/maskApi.h`

 * *Files identical despite different names*

### Comparing `faster-coco-eval-1.3.2/csrc/mask/pycocotools/_mask.c` & `faster-coco-eval-1.3.3/csrc/mask/pycocotools/_mask.c`

 * *Files identical despite different names*

### Comparing `faster-coco-eval-1.3.2/csrc/mask/pycocotools/_mask.pyx` & `faster-coco-eval-1.3.3/csrc/mask/pycocotools/_mask.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # distutils: language = c
-# distutils: sources = ../common/maskApi.c
 
 #**************************************************************************
 # Microsoft COCO Toolbox.      version 2.0
 # Data, paper, and tutorials available at:  http://mscoco.org/
 # Code written by Piotr Dollar and Tsung-Yi Lin, 2015.
 # Licensed under the Simplified BSD License [see coco/license.txt]
 #**************************************************************************
```

### Comparing `faster-coco-eval-1.3.2/faster_coco_eval/core/coco.py` & `faster-coco-eval-1.3.3/faster_coco_eval/core/coco.py`

 * *Files identical despite different names*

### Comparing `faster-coco-eval-1.3.2/faster_coco_eval/core/cocoeval.py` & `faster-coco-eval-1.3.3/faster_coco_eval/core/cocoeval.py`

 * *Files identical despite different names*

### Comparing `faster-coco-eval-1.3.2/faster_coco_eval/core/faster_eval_api.py` & `faster-coco-eval-1.3.3/faster_coco_eval/core/faster_eval_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,15 +176,19 @@
                             _dt_ann['tp'] = True
                             _dt_ann['gt_id'] = gt_id
                             _dt_ann['iou'] = iou
 
                             _gt_ann['dt_id'] = dt_id
                             _gt_ann['matched'] = True
                         else:
-                            _old_dt_ann = self.cocoDt.anns[_gt_ann['dt_id']]
+                            # TODO: Непонятно почему не находит. Проверить на тестовых данных
+                            _old_dt_ann = self.cocoDt.anns.get(_gt_ann['dt_id'])
+                            if _old_dt_ann is None:
+                                continue
+
                             if _old_dt_ann['id'] == _dt_ann['id']:
                                 continue
                             else:
                                 if (_old_dt_ann.get('iou', self.computeAnnIoU(_gt_ann, _old_dt_ann)) < iou) or (_old_dt_ann['score'] < _dt_ann['score']):
                                     _dt_ann['tp'] = True
                                     _dt_ann['gt_id'] = gt_id
                                     _dt_ann['iou'] = iou
@@ -231,16 +235,21 @@
                     elif self.params.iouType == 'bbox':
                         g.append(gt_ann['bbox'])
                         d.append(dt_ann['bbox'])
                     else:
                         raise Exception('unknown iouType for iou computation')
 
         iscrowd = [0 for o in g]
-        ious = maskUtils.iou(d, g, iscrowd).diagonal()
-        return ious.mean()
+        
+        ious = maskUtils.iou(d, g, iscrowd)
+        if len(ious) == 0:
+            return 0
+        else:
+            ious = ious.diagonal()
+            return ious.mean()
     
     def compute_mAUC(self):
         aucs = []
 
         for K in range(self.eval['counts'][2]):
             for A in range(self.eval['counts'][3]):            
                 precision_list = self.eval['precision'][0, :, K, A, :].ravel()
@@ -264,15 +273,15 @@
             self.all_stats = np.append(self.all_stats, self.compute_mAUC())
 
     
     @property
     def stats_as_dict(self):
         iouType = self.params.iouType
         assert (iouType == 'segm' or iouType ==
-                'bbox'), f'{iouType=} not supported'
+                'bbox'), f'iouType={iouType} not supported'
 
         labels = [
             "AP_all", "AP_50", "AP_75",
             "AP_small", "AP_medium", "AP_large",
             "AR_all", "AR_second", "AR_third",
             "AR_small", "AR_medium", "AR_large", "AR_50", "AR_75"]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `faster-coco-eval-1.3.2/faster_coco_eval/core/mask.py` & `faster-coco-eval-1.3.3/faster_coco_eval/core/mask.py`

 * *Files identical despite different names*

### Comparing `faster-coco-eval-1.3.2/faster_coco_eval/extra/curves.py` & `faster-coco-eval-1.3.3/faster_coco_eval/extra/curves.py`

 * *Files identical despite different names*

### Comparing `faster-coco-eval-1.3.2/faster_coco_eval/extra/display.py` & `faster-coco-eval-1.3.3/faster_coco_eval/extra/display.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
             cm[enum_id][-1] = fn.get(category_id, 0)
 
         return cm
 
     def compute_confusion_matrix(self):
         if self.useCats:
             logger.warning(
-                f"The calculation may not be accurate. No intersection of classes. {self.useCats=}")
+                f"The calculation may not be accurate. No intersection of classes. useCats={self.useCats}")
 
         y_true = []
         y_pred = []
 
         fn = {}
         fp = {}
```

### Comparing `faster-coco-eval-1.3.2/faster_coco_eval/extra/extra.py` & `faster-coco-eval-1.3.3/faster_coco_eval/extra/extra.py`

 * *Files identical despite different names*

### Comparing `faster-coco-eval-1.3.2/faster_coco_eval.egg-info/PKG-INFO` & `faster-coco-eval-1.3.3/faster_coco_eval.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faster-coco-eval
-Version: 1.3.2
+Version: 1.3.3
 Summary: Faster interpretation of the original COCOEval
 Home-page: https://github.com/MiXaiLL76/faster_coco_eval
 Author: MiXaiLL76
 Author-email: mike.milos@yandex.ru
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -75,14 +75,22 @@
 ## Setup dependencies
 
 - numpy
 - plotly (optional if extra.Curve usage)  
 
 ## history
 
+### v1.3.3
+
+- [x] fix by ViTrox <https://github.com/vitrox-technologies/faster_coco_eval>
+    - missing file issue
+    - issue discovered by torchmetric
+    - fstring for python3.7
+    - Windows compilation
+
 ### v1.3.2
 
 - [x] rework math_matches function. moved to faster_eval_api
 - [x] Moved calculations from python to c++
 - [x] Separated extra classes
 - [x] Added new sample data
 - [x] append mIoU based on TP pred.
```

### Comparing `faster-coco-eval-1.3.2/faster_coco_eval.egg-info/SOURCES.txt` & `faster-coco-eval-1.3.3/faster_coco_eval.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `faster-coco-eval-1.3.2/setup.py` & `faster-coco-eval-1.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/python3
 
+import platform
 import setuptools
 from setuptools import setup, Extension
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 import numpy as np
 
 
 def readme():
@@ -123,15 +124,16 @@
     print(f"Include: {include_dirs}")
 
     ext_modules += [
         Extension(
             'faster_coco_eval.mask_api_cpp',
             sources=sources,
             include_dirs=include_dirs,
-            extra_compile_args=[
+            extra_compile_args=[] if platform.system()=='Windows' else
+            [
                 '-Wno-cpp',
                 '-Wno-unused-function',
                 '-std=c99',
                 '-O3',
                 '-Wno-misleading-indentation',
             ],
             extra_link_args=[],
```

