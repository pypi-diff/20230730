# Comparing `tmp/innovationmerge-1.0.7.tar.gz` & `tmp/innovationmerge-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "innovationmerge-1.0.7.tar", max compression
+gzip compressed data, was "innovationmerge-1.0.8.tar", max compression
```

## Comparing `innovationmerge-1.0.7.tar` & `innovationmerge-1.0.8.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0      125 2023-07-30 06:01:46.671515 innovationmerge-1.0.7/innovationmerge/__init__.py
--rw-r--r--   0        0        0      986 2023-06-04 12:33:31.912374 innovationmerge-1.0.7/innovationmerge/app/__init__.py
--rw-r--r--   0        0        0      339 2023-06-04 12:33:31.896708 innovationmerge-1.0.7/innovationmerge/app/exceptions.py
--rw-r--r--   0        0        0      776 2023-06-04 12:33:31.912374 innovationmerge-1.0.7/innovationmerge/app/logger/__init__.py
--rw-r--r--   0        0        0     1342 2023-06-04 12:33:31.912374 innovationmerge-1.0.7/innovationmerge/app/middleware/__init__.py
--rw-r--r--   0        0        0      655 2023-06-04 12:33:31.927958 innovationmerge-1.0.7/innovationmerge/app/routers/__init__.py
--rw-r--r--   0        0        0     1414 2023-06-04 12:33:31.912374 innovationmerge-1.0.7/innovationmerge/app/routers/authenticate.py
--rw-r--r--   0        0        0     1520 2023-06-04 12:33:31.927958 innovationmerge-1.0.7/innovationmerge/app/routers/sample_route.py
--rw-r--r--   0        0        0       46 2023-06-04 12:33:31.896708 innovationmerge-1.0.7/innovationmerge/app/sample.py
--rw-r--r--   0        0        0      104 2023-06-04 12:33:31.927958 innovationmerge-1.0.7/innovationmerge/app/schemas/sample_schema.py
--rw-r--r--   0        0        0      459 2023-06-04 12:33:31.927958 innovationmerge-1.0.7/innovationmerge/app/schemas/user_schema.py
--rw-r--r--   0        0        0     3226 2023-06-04 12:33:31.912374 innovationmerge-1.0.7/innovationmerge/app/security.py
--rw-r--r--   0        0        0     1836 2023-06-04 12:33:31.881091 innovationmerge-1.0.7/innovationmerge/config.py
--rw-r--r--   0        0        0      139 2023-07-30 04:58:31.941326 innovationmerge-1.0.7/innovationmerge/configurations/constants.py
--rw-r--r--   0        0        0     1300 2023-06-04 12:33:31.943618 innovationmerge-1.0.7/innovationmerge/docs/api_doc.py
--rw-r--r--   0        0        0        0 2023-06-04 12:33:31.943618 innovationmerge-1.0.7/innovationmerge/docs/file.md
--rw-r--r--   0        0        0        0 2023-06-04 12:33:31.943618 innovationmerge-1.0.7/innovationmerge/scripts/test.sh
--rw-r--r--   0        0        0        0 2023-06-04 13:48:12.834202 innovationmerge-1.0.7/innovationmerge/src/ai/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 13:48:12.834202 innovationmerge-1.0.7/innovationmerge/src/ai/cpu/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 16:01:26.589721 innovationmerge-1.0.7/innovationmerge/src/ai/edge/__init__.py
--rw-r--r--   0        0        0     5134 2023-07-30 06:10:03.387248 innovationmerge-1.0.7/innovationmerge/src/ai/edge/object_detection.py
--rw-r--r--   0        0        0        0 2023-06-04 16:01:26.589721 innovationmerge-1.0.7/innovationmerge/src/ai/gpu/__init__.py
--rw-r--r--   0        0        0     3509 2023-07-30 06:13:21.652023 innovationmerge-1.0.7/innovationmerge/src/utils/responses.py
--rw-r--r--   0        0        0      153 2023-06-04 12:33:31.943618 innovationmerge-1.0.7/innovationmerge/tests/__init__.py
--rw-r--r--   0        0        0     3188 2023-06-04 12:33:31.943618 innovationmerge-1.0.7/innovationmerge/tests/sample.py
--rw-r--r--   0        0        0     1193 2023-06-11 12:39:40.887778 innovationmerge-1.0.7/innovationmerge/tests/test_object_detection.py
--rw-r--r--   0        0        0      925 2023-07-30 06:17:16.769911 innovationmerge-1.0.7/pyproject.toml
--rw-r--r--   0        0        0      498 2023-07-30 06:15:28.128763 innovationmerge-1.0.7/README.md
--rw-r--r--   0        0        0     1551 1970-01-01 00:00:00.000000 innovationmerge-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0      210 2023-07-30 08:39:33.540959 innovationmerge-1.0.8/CHANGELOG.md
+-rw-r--r--   0        0        0      125 2023-07-30 06:01:46.671515 innovationmerge-1.0.8/innovationmerge/__init__.py
+-rw-r--r--   0        0        0      986 2023-06-04 12:33:31.912374 innovationmerge-1.0.8/innovationmerge/app/__init__.py
+-rw-r--r--   0        0        0      339 2023-06-04 12:33:31.896708 innovationmerge-1.0.8/innovationmerge/app/exceptions.py
+-rw-r--r--   0        0        0      776 2023-06-04 12:33:31.912374 innovationmerge-1.0.8/innovationmerge/app/logger/__init__.py
+-rw-r--r--   0        0        0     1342 2023-06-04 12:33:31.912374 innovationmerge-1.0.8/innovationmerge/app/middleware/__init__.py
+-rw-r--r--   0        0        0      655 2023-06-04 12:33:31.927958 innovationmerge-1.0.8/innovationmerge/app/routers/__init__.py
+-rw-r--r--   0        0        0     1414 2023-06-04 12:33:31.912374 innovationmerge-1.0.8/innovationmerge/app/routers/authenticate.py
+-rw-r--r--   0        0        0     1520 2023-06-04 12:33:31.927958 innovationmerge-1.0.8/innovationmerge/app/routers/sample_route.py
+-rw-r--r--   0        0        0       46 2023-06-04 12:33:31.896708 innovationmerge-1.0.8/innovationmerge/app/sample.py
+-rw-r--r--   0        0        0      104 2023-06-04 12:33:31.927958 innovationmerge-1.0.8/innovationmerge/app/schemas/sample_schema.py
+-rw-r--r--   0        0        0      459 2023-06-04 12:33:31.927958 innovationmerge-1.0.8/innovationmerge/app/schemas/user_schema.py
+-rw-r--r--   0        0        0     3226 2023-06-04 12:33:31.912374 innovationmerge-1.0.8/innovationmerge/app/security.py
+-rw-r--r--   0        0        0     1836 2023-06-04 12:33:31.881091 innovationmerge-1.0.8/innovationmerge/config.py
+-rw-r--r--   0        0        0      139 2023-07-30 04:58:31.941326 innovationmerge-1.0.8/innovationmerge/configurations/constants.py
+-rw-r--r--   0        0        0     1300 2023-06-04 12:33:31.943618 innovationmerge-1.0.8/innovationmerge/docs/api_doc.py
+-rw-r--r--   0        0        0        0 2023-06-04 12:33:31.943618 innovationmerge-1.0.8/innovationmerge/docs/file.md
+-rw-r--r--   0        0        0        0 2023-06-04 12:33:31.943618 innovationmerge-1.0.8/innovationmerge/scripts/test.sh
+-rw-r--r--   0        0        0        0 2023-06-04 13:48:12.834202 innovationmerge-1.0.8/innovationmerge/src/ai/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 13:48:12.834202 innovationmerge-1.0.8/innovationmerge/src/ai/cpu/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 16:01:26.589721 innovationmerge-1.0.8/innovationmerge/src/ai/edge/__init__.py
+-rw-r--r--   0        0        0     5134 2023-07-30 08:16:36.528787 innovationmerge-1.0.8/innovationmerge/src/ai/edge/object_detection.py
+-rw-r--r--   0        0        0        0 2023-06-04 16:01:26.589721 innovationmerge-1.0.8/innovationmerge/src/ai/gpu/__init__.py
+-rw-r--r--   0        0        0     2658 2023-07-30 08:22:56.913044 innovationmerge-1.0.8/innovationmerge/src/utils/responses.py
+-rw-r--r--   0        0        0      153 2023-06-04 12:33:31.943618 innovationmerge-1.0.8/innovationmerge/tests/__init__.py
+-rw-r--r--   0        0        0     3188 2023-06-04 12:33:31.943618 innovationmerge-1.0.8/innovationmerge/tests/sample.py
+-rw-r--r--   0        0        0     1586 2023-07-30 08:32:23.116204 innovationmerge-1.0.8/innovationmerge/tests/test_object_detection.py
+-rw-r--r--   0        0        0      926 2023-07-30 08:41:31.852946 innovationmerge-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0      498 2023-07-30 06:15:28.128763 innovationmerge-1.0.8/README.md
+-rw-r--r--   0        0        0     1674 1970-01-01 00:00:00.000000 innovationmerge-1.0.8/PKG-INFO
```

### Comparing `innovationmerge-1.0.7/innovationmerge/app/__init__.py` & `innovationmerge-1.0.8/innovationmerge/app/__init__.py`

 * *Files identical despite different names*

### Comparing `innovationmerge-1.0.7/innovationmerge/app/logger/__init__.py` & `innovationmerge-1.0.8/innovationmerge/app/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `innovationmerge-1.0.7/innovationmerge/app/middleware/__init__.py` & `innovationmerge-1.0.8/innovationmerge/app/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `innovationmerge-1.0.7/innovationmerge/app/routers/__init__.py` & `innovationmerge-1.0.8/innovationmerge/app/routers/__init__.py`

 * *Files identical despite different names*

### Comparing `innovationmerge-1.0.7/innovationmerge/app/routers/authenticate.py` & `innovationmerge-1.0.8/innovationmerge/app/routers/authenticate.py`

 * *Files identical despite different names*

### Comparing `innovationmerge-1.0.7/innovationmerge/app/routers/sample_route.py` & `innovationmerge-1.0.8/innovationmerge/app/routers/sample_route.py`

 * *Files identical despite different names*

### Comparing `innovationmerge-1.0.7/innovationmerge/app/security.py` & `innovationmerge-1.0.8/innovationmerge/app/security.py`

 * *Files identical despite different names*

### Comparing `innovationmerge-1.0.7/innovationmerge/config.py` & `innovationmerge-1.0.8/innovationmerge/config.py`

 * *Files identical despite different names*

### Comparing `innovationmerge-1.0.7/innovationmerge/docs/api_doc.py` & `innovationmerge-1.0.8/innovationmerge/docs/api_doc.py`

 * *Files identical despite different names*

### Comparing `innovationmerge-1.0.7/innovationmerge/src/ai/edge/object_detection.py` & `innovationmerge-1.0.8/innovationmerge/src/ai/edge/object_detection.py`

 * *Files identical despite different names*

### Comparing `innovationmerge-1.0.7/innovationmerge/src/utils/responses.py` & `innovationmerge-1.0.8/innovationmerge/src/utils/responses.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,48 +9,35 @@
 
 def load_labels(filename):
   with open(filename, 'r') as f:
     return [line.strip() for line in f.readlines()]
 
 
 def draw_detections(detections, cv2_image):
-    for detection in detections.get("detection"):
+    colors = [(61, 203, 0), (4, 39, 240), (255, 3, 0), (255, 126, 0), (41, 141, 172), (10, 255, 0)]
+    for index, detection in enumerate(detections.get("detection")):
        xmin = detection.get("label_bounding_box")[0].get("x")
        ymin = detection.get("label_bounding_box")[0].get("y")
        xmax = detection.get("label_bounding_box")[1].get("x")
        ymax = detection.get("label_bounding_box")[1].get("y")
-       cv2.rectangle(cv2_image, (xmin, ymin), (xmax, ymax), (10, 255, 0), 2)
+       cv2.rectangle(cv2_image, (xmin, ymin), (xmax, ymax), colors[index], 2)
         # Draw label
        object_name = detection["label_class_name"]
        confidence = detection["confidence"]
        label = '%s: %d%%' % (object_name, int(confidence*100))
        labelSize, baseLine = cv2.getTextSize(label, cv2.FONT_HERSHEY_SIMPLEX, 0.7, 2)
        label_ymin = max(ymin, labelSize[1] + 10)
        cv2.rectangle(cv2_image, (xmin, label_ymin-labelSize[1]-10), (xmin+labelSize[0], label_ymin+baseLine-10), (255, 255, 255), cv2.FILLED)
        cv2.putText(cv2_image, label, (xmin, label_ymin-7), cv2.FONT_HERSHEY_SIMPLEX, 0.7, (0, 0, 0), 2)
     return cv2_image
 
 
 def save_detection_image(detections : dict, cv2_image, output_image_path: str, model_type: str = "ssd"):
-
     if model_type == "ssd":
-        for detection in detections.get("detection"):
-            xmin = detection.get("label_bounding_box")[0].get("x")
-            ymin = detection.get("label_bounding_box")[0].get("y")
-            xmax = detection.get("label_bounding_box")[1].get("x")
-            ymax = detection.get("label_bounding_box")[1].get("y")
-            cv2.rectangle(cv2_image, (xmin, ymin), (xmax, ymax), (10, 255, 0), 2)
-            # Draw label
-            object_name = detection["label_class_name"]
-            confidence = detection["confidence"]
-            label = '%s: %d%%' % (object_name, int(confidence*100))
-            labelSize, baseLine = cv2.getTextSize(label, cv2.FONT_HERSHEY_SIMPLEX, 0.7, 2)
-            label_ymin = max(ymin, labelSize[1] + 10)
-            cv2.rectangle(cv2_image, (xmin, label_ymin-labelSize[1]-10), (xmin+labelSize[0], label_ymin+baseLine-10), (255, 255, 255), cv2.FILLED)
-            cv2.putText(cv2_image, label, (xmin, label_ymin-7), cv2.FONT_HERSHEY_SIMPLEX, 0.7, (0, 0, 0), 2)
+        draw_detections(detections, cv2_image)
         cv2.imwrite(output_image_path, cv2_image)
     else:
         position = (30, 30)
         font_scale = 0.75
         color = (255, 255, 255)
         thickness = 2
         font = cv2.FONT_HERSHEY_SIMPLEX
```

### Comparing `innovationmerge-1.0.7/innovationmerge/tests/sample.py` & `innovationmerge-1.0.8/innovationmerge/tests/sample.py`

 * *Files identical despite different names*

### Comparing `innovationmerge-1.0.7/innovationmerge/tests/test_object_detection.py` & `innovationmerge-1.0.8/innovationmerge/tests/test_object_detection.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 import os
-from innovationmerge import cpuObjectDetectionTfLite, edgeObjectDetectionTfLite
+from innovationmerge import EdgeObjectDetectionTfLite
 from innovationmerge.src.utils.responses import load_labels, read_image
 
 # Declare paths
 cwd = os.getcwd()
-model_path = os.path.join(cwd, "models", "ssd_mobilenet_v3_large_coco_2020_01_14")
-model_file_path = os.path.join(model_path, "model.tflite")
-labels_path = os.path.join(model_path, "labels.txt")
+
 input_image_path = os.path.join(cwd, "data", "testdata", "images.jpg")
 
 
-def test_cpu_object_detect():
+# edge object detection ssd
+def test_edge_object_detect_ssd():
+    threshold = 0.6
+    model_type="ssd"
+    model_path = os.path.join(cwd, "models", "edge", "ssd_mobilenet_v3_large_coco_2020_01_14")
+    model_file_path = os.path.join(model_path, "model.tflite")
+    labels_path = os.path.join(model_path, "labels.txt")
     labels = load_labels(labels_path)
     cv2_image = read_image(input_image_path)
-    detect_objects = cpuObjectDetectionTfLite(model_file_path)
-    detection_result = detect_objects.detect(cv2_image, labels)
+    detect_objects = EdgeObjectDetectionTfLite(model_file_path)
+    detection_result = detect_objects.detect(cv2_image, labels, threshold, model_type)
     print(detection_result)
     assert detection_result.get('detection')[0].get('label_class_name') == "cat"
 
 
-def test_edge_object_detect():
+# edge object detection mobilenet
+def test_edge_object_detect_mobilenet():
+    threshold = 0.6
+    model_type="mobilenet"
+    model_path = os.path.join(cwd, "models", "edge", "mobilenet_v2_1.0_224_quant")
+    model_file_path = os.path.join(model_path, "model.tflite")
+    labels_path = os.path.join(model_path, "labels.txt")
     labels = load_labels(labels_path)
     cv2_image = read_image(input_image_path)
-    detect_objects = edgeObjectDetectionTfLite(model_file_path)
-    detection_result = detect_objects.detect(cv2_image, labels)
+    detect_objects = EdgeObjectDetectionTfLite(model_file_path)
+    detection_result = detect_objects.detect(cv2_image, labels, threshold, model_type)
     print(detection_result)
-    assert detection_result.get('detection')[0].get('label_class_name') == "cat"
+    assert len(detection_result.get('detection')) > 0
```

### Comparing `innovationmerge-1.0.7/pyproject.toml` & `innovationmerge-1.0.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 [tool.poetry]
 name = "innovationmerge"
-version = "1.0.7"
+version = "1.0.8"
 description = "innovationmerge core components"
 authors = ["innovationmerge"]
 readme = "README.md"
 packages = [{include = "innovationmerge"}]
+repository = "https://github.com/innovationmerge/innovation-merge"
+include = ["CHANGELOG.md"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 tox = "^3.26.0"
 click = "^8.1.3"
 fastapi = "^0.85.0"
 python-multipart = "^0.0.5"
@@ -17,25 +19,21 @@
 python-dotenv = "^0.21.0"
 python-json-logger = "^2.0.4"
 requests = "^2.28.1"
 python-jose = "^3.3.0"
 passlib = "^1.7.4"
 bcrypt = "^4.0.0"
 opencv-python = "^4.7.0.72"
+tensorflow = "^2.12.0"
 
 
 [tool.poetry.dev-dependencies]
 pytest = "7.1.3"
 pytest-cov = "3.0.0"
 black = "^22.8.0"
 flake8 = "^5.0.4"
 pyinstaller = "^5.8.0"
 bandit = "^1.7.5"
 
-[tool.poetry.extras]
-cpu = ["tensorflow-cpu", "tensorflow-intel"]
-gpu = ["tf-nightly-gpu"]
-edge = ["tensorflow"]
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `innovationmerge-1.0.7/PKG-INFO` & `innovationmerge-1.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: innovationmerge
-Version: 1.0.7
+Version: 1.0.8
 Summary: innovationmerge core components
+Home-page: https://github.com/innovationmerge/innovation-merge
 Author: innovationmerge
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: cpu
-Provides-Extra: edge
-Provides-Extra: gpu
 Requires-Dist: aiofiles (>=22.1.0,<23.0.0)
 Requires-Dist: bcrypt (>=4.0.0,<5.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: fastapi (>=0.85.0,<0.86.0)
 Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0)
 Requires-Dist: passlib (>=1.7.4,<2.0.0)
 Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
 Requires-Dist: python-jose (>=3.3.0,<4.0.0)
 Requires-Dist: python-json-logger (>=2.0.4,<3.0.0)
 Requires-Dist: python-multipart (>=0.0.5,<0.0.6)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: tensorflow (>=2.12.0,<3.0.0)
 Requires-Dist: tox (>=3.26.0,<4.0.0)
 Requires-Dist: uvicorn (>=0.18.3,<0.19.0)
+Project-URL: Repository, https://github.com/innovationmerge/innovation-merge
 Description-Content-Type: text/markdown
 
 ## About
 - `Author` : innovationmerge
 - `Version`: 1.0
 - `Description`: 
     - Contains innovationmerge projects core components.
```

