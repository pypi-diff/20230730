# Comparing `tmp/innovationmerge-1.0.6.tar.gz` & `tmp/innovationmerge-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "innovationmerge-1.0.6.tar", max compression
+gzip compressed data, was "innovationmerge-1.0.7.tar", max compression
```

## Comparing `innovationmerge-1.0.6.tar` & `innovationmerge-1.0.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      180 2023-06-11 12:39:59.490310 innovationmerge-1.0.6/innovationmerge/__init__.py
--rw-r--r--   0        0        0      986 2023-06-04 12:33:31.912374 innovationmerge-1.0.6/innovationmerge/app/__init__.py
--rw-r--r--   0        0        0      339 2023-06-04 12:33:31.896708 innovationmerge-1.0.6/innovationmerge/app/exceptions.py
--rw-r--r--   0        0        0      776 2023-06-04 12:33:31.912374 innovationmerge-1.0.6/innovationmerge/app/logger/__init__.py
--rw-r--r--   0        0        0     1342 2023-06-04 12:33:31.912374 innovationmerge-1.0.6/innovationmerge/app/middleware/__init__.py
--rw-r--r--   0        0        0      655 2023-06-04 12:33:31.927958 innovationmerge-1.0.6/innovationmerge/app/routers/__init__.py
--rw-r--r--   0        0        0     1414 2023-06-04 12:33:31.912374 innovationmerge-1.0.6/innovationmerge/app/routers/authenticate.py
--rw-r--r--   0        0        0     1520 2023-06-04 12:33:31.927958 innovationmerge-1.0.6/innovationmerge/app/routers/sample_route.py
--rw-r--r--   0        0        0       46 2023-06-04 12:33:31.896708 innovationmerge-1.0.6/innovationmerge/app/sample.py
--rw-r--r--   0        0        0      104 2023-06-04 12:33:31.927958 innovationmerge-1.0.6/innovationmerge/app/schemas/sample_schema.py
--rw-r--r--   0        0        0      459 2023-06-04 12:33:31.927958 innovationmerge-1.0.6/innovationmerge/app/schemas/user_schema.py
--rw-r--r--   0        0        0     3226 2023-06-04 12:33:31.912374 innovationmerge-1.0.6/innovationmerge/app/security.py
--rw-r--r--   0        0        0     1836 2023-06-04 12:33:31.881091 innovationmerge-1.0.6/innovationmerge/config.py
--rw-r--r--   0        0        0       94 2023-06-11 07:21:11.268905 innovationmerge-1.0.6/innovationmerge/configurations/constants.py
--rw-r--r--   0        0        0     1300 2023-06-04 12:33:31.943618 innovationmerge-1.0.6/innovationmerge/docs/api_doc.py
--rw-r--r--   0        0        0        0 2023-06-04 12:33:31.943618 innovationmerge-1.0.6/innovationmerge/docs/file.md
--rw-r--r--   0        0        0        0 2023-06-04 12:33:31.943618 innovationmerge-1.0.6/innovationmerge/scripts/test.sh
--rw-r--r--   0        0        0        0 2023-06-04 13:48:12.834202 innovationmerge-1.0.6/innovationmerge/src/ai/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 13:48:12.834202 innovationmerge-1.0.6/innovationmerge/src/ai/cpu/__init__.py
--rw-r--r--   0        0        0     8690 2023-06-11 12:37:12.329152 innovationmerge-1.0.6/innovationmerge/src/ai/cpu/object_detection.py
--rw-r--r--   0        0        0        0 2023-06-04 16:01:26.589721 innovationmerge-1.0.6/innovationmerge/src/ai/edge/__init__.py
--rw-r--r--   0        0        0      148 2023-06-04 14:35:41.131565 innovationmerge-1.0.6/innovationmerge/src/ai/edge/object_detection.py
--rw-r--r--   0        0        0     2598 2023-06-13 17:52:52.825884 innovationmerge-1.0.6/innovationmerge/src/utils/responses.py
--rw-r--r--   0        0        0      153 2023-06-04 12:33:31.943618 innovationmerge-1.0.6/innovationmerge/tests/__init__.py
--rw-r--r--   0        0        0     3188 2023-06-04 12:33:31.943618 innovationmerge-1.0.6/innovationmerge/tests/sample.py
--rw-r--r--   0        0        0     1193 2023-06-11 12:39:40.887778 innovationmerge-1.0.6/innovationmerge/tests/test_object_detection.py
--rw-r--r--   0        0        0      925 2023-06-13 17:56:28.680663 innovationmerge-1.0.6/pyproject.toml
--rw-r--r--   0        0        0      447 2023-06-04 14:30:02.127230 innovationmerge-1.0.6/README.md
--rw-r--r--   0        0        0     1500 1970-01-01 00:00:00.000000 innovationmerge-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0      125 2023-07-30 06:01:46.671515 innovationmerge-1.0.7/innovationmerge/__init__.py
+-rw-r--r--   0        0        0      986 2023-06-04 12:33:31.912374 innovationmerge-1.0.7/innovationmerge/app/__init__.py
+-rw-r--r--   0        0        0      339 2023-06-04 12:33:31.896708 innovationmerge-1.0.7/innovationmerge/app/exceptions.py
+-rw-r--r--   0        0        0      776 2023-06-04 12:33:31.912374 innovationmerge-1.0.7/innovationmerge/app/logger/__init__.py
+-rw-r--r--   0        0        0     1342 2023-06-04 12:33:31.912374 innovationmerge-1.0.7/innovationmerge/app/middleware/__init__.py
+-rw-r--r--   0        0        0      655 2023-06-04 12:33:31.927958 innovationmerge-1.0.7/innovationmerge/app/routers/__init__.py
+-rw-r--r--   0        0        0     1414 2023-06-04 12:33:31.912374 innovationmerge-1.0.7/innovationmerge/app/routers/authenticate.py
+-rw-r--r--   0        0        0     1520 2023-06-04 12:33:31.927958 innovationmerge-1.0.7/innovationmerge/app/routers/sample_route.py
+-rw-r--r--   0        0        0       46 2023-06-04 12:33:31.896708 innovationmerge-1.0.7/innovationmerge/app/sample.py
+-rw-r--r--   0        0        0      104 2023-06-04 12:33:31.927958 innovationmerge-1.0.7/innovationmerge/app/schemas/sample_schema.py
+-rw-r--r--   0        0        0      459 2023-06-04 12:33:31.927958 innovationmerge-1.0.7/innovationmerge/app/schemas/user_schema.py
+-rw-r--r--   0        0        0     3226 2023-06-04 12:33:31.912374 innovationmerge-1.0.7/innovationmerge/app/security.py
+-rw-r--r--   0        0        0     1836 2023-06-04 12:33:31.881091 innovationmerge-1.0.7/innovationmerge/config.py
+-rw-r--r--   0        0        0      139 2023-07-30 04:58:31.941326 innovationmerge-1.0.7/innovationmerge/configurations/constants.py
+-rw-r--r--   0        0        0     1300 2023-06-04 12:33:31.943618 innovationmerge-1.0.7/innovationmerge/docs/api_doc.py
+-rw-r--r--   0        0        0        0 2023-06-04 12:33:31.943618 innovationmerge-1.0.7/innovationmerge/docs/file.md
+-rw-r--r--   0        0        0        0 2023-06-04 12:33:31.943618 innovationmerge-1.0.7/innovationmerge/scripts/test.sh
+-rw-r--r--   0        0        0        0 2023-06-04 13:48:12.834202 innovationmerge-1.0.7/innovationmerge/src/ai/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 13:48:12.834202 innovationmerge-1.0.7/innovationmerge/src/ai/cpu/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 16:01:26.589721 innovationmerge-1.0.7/innovationmerge/src/ai/edge/__init__.py
+-rw-r--r--   0        0        0     5134 2023-07-30 06:10:03.387248 innovationmerge-1.0.7/innovationmerge/src/ai/edge/object_detection.py
+-rw-r--r--   0        0        0        0 2023-06-04 16:01:26.589721 innovationmerge-1.0.7/innovationmerge/src/ai/gpu/__init__.py
+-rw-r--r--   0        0        0     3509 2023-07-30 06:13:21.652023 innovationmerge-1.0.7/innovationmerge/src/utils/responses.py
+-rw-r--r--   0        0        0      153 2023-06-04 12:33:31.943618 innovationmerge-1.0.7/innovationmerge/tests/__init__.py
+-rw-r--r--   0        0        0     3188 2023-06-04 12:33:31.943618 innovationmerge-1.0.7/innovationmerge/tests/sample.py
+-rw-r--r--   0        0        0     1193 2023-06-11 12:39:40.887778 innovationmerge-1.0.7/innovationmerge/tests/test_object_detection.py
+-rw-r--r--   0        0        0      925 2023-07-30 06:17:16.769911 innovationmerge-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0      498 2023-07-30 06:15:28.128763 innovationmerge-1.0.7/README.md
+-rw-r--r--   0        0        0     1551 1970-01-01 00:00:00.000000 innovationmerge-1.0.7/PKG-INFO
```

### Comparing `innovationmerge-1.0.6/innovationmerge/app/__init__.py` & `innovationmerge-1.0.7/innovationmerge/app/__init__.py`

 * *Files identical despite different names*

### Comparing `innovationmerge-1.0.6/innovationmerge/app/logger/__init__.py` & `innovationmerge-1.0.7/innovationmerge/app/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `innovationmerge-1.0.6/innovationmerge/app/middleware/__init__.py` & `innovationmerge-1.0.7/innovationmerge/app/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `innovationmerge-1.0.6/innovationmerge/app/routers/__init__.py` & `innovationmerge-1.0.7/innovationmerge/app/routers/__init__.py`

 * *Files identical despite different names*

### Comparing `innovationmerge-1.0.6/innovationmerge/app/routers/authenticate.py` & `innovationmerge-1.0.7/innovationmerge/app/routers/authenticate.py`

 * *Files identical despite different names*

### Comparing `innovationmerge-1.0.6/innovationmerge/app/routers/sample_route.py` & `innovationmerge-1.0.7/innovationmerge/app/routers/sample_route.py`

 * *Files identical despite different names*

### Comparing `innovationmerge-1.0.6/innovationmerge/app/security.py` & `innovationmerge-1.0.7/innovationmerge/app/security.py`

 * *Files identical despite different names*

### Comparing `innovationmerge-1.0.6/innovationmerge/config.py` & `innovationmerge-1.0.7/innovationmerge/config.py`

 * *Files identical despite different names*

### Comparing `innovationmerge-1.0.6/innovationmerge/docs/api_doc.py` & `innovationmerge-1.0.7/innovationmerge/docs/api_doc.py`

 * *Files identical despite different names*

### Comparing `innovationmerge-1.0.6/innovationmerge/src/ai/cpu/object_detection.py` & `innovationmerge-1.0.7/innovationmerge/src/ai/edge/object_detection.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import tensorflow as tf
 import cv2
 import numpy as np
 import time
-from innovationmerge.configurations.constants import IMAGE_DETECTION_RESPONSE
+from innovationmerge.configurations.constants import DETECTION_RESPONSE_BB, DETECTION_RESPONSE
 
-class cpuObjectDetectionTfLite():
+class EdgeObjectDetectionTfLite():
     """
     Object detection inference using Tensorflow Lite models. 
     This class includes loading the model, preparing input data, invoking the interpreter, and extracting output results. 
     """
     def __init__(self, model_file_path):
         # Load the TensorFlow Lite model
         self.interpreter = tf.lite.Interpreter(model_path=model_file_path)
         self.interpreter.allocate_tensors()
 
         # Set input normalization parameters
         self.input_mean = 127.5
         self.input_std = 127.5
 
-    def detect(self, cv2_image, labels_list, threshold=0.1):
+    def detect(self, cv2_image, labels_list, threshold, model_type="ssd"):
         """
         Parameters:
             cv2_image: OpenCV 2 Image
             labels_list: labels list
             threshold: minimum score
         Returns:
             Array of Detections(Label, Bounding Box, Confidence score)
@@ -65,120 +65,41 @@
         # Determine the indices for accessing the output tensor.The specific indices for accessing the output tensors depend on whether the model is a TensorFlow 1.x or TensorFlow 2.x model.
         out_name = output_details[0]['name']
         if ('StatefulPartitionedCall' in out_name): # This is a TF2 model
             boxes_idx, classes_idx, scores_idx = 1, 3, 0
         else: # This is a TF1 model
             boxes_idx, classes_idx, scores_idx = 0, 1, 2
 
-        # Retrieve detection results
-        boxes = self.interpreter.get_tensor(output_details[boxes_idx]['index'])[0] # Bounding box coordinates of detected objects
-        classes = self.interpreter.get_tensor(output_details[classes_idx]['index'])[0] # Class index of detected objects
-        scores = self.interpreter.get_tensor(output_details[scores_idx]['index'])[0] # Confidence of detected objects
-
-        # Create custom response
-        detection_response = {}
-        detection_list = []
-        for i in range(len(scores)):
-            label_dict = IMAGE_DETECTION_RESPONSE.copy()
-            if ((scores[i] > 0.6) and (scores[i] <= 1.0)):
-                ymin = int(max(1,(boxes[i][0] * input_img_height)))
-                xmin = int(max(1,(boxes[i][1] * input_img_width)))
-                ymax = int(min(input_img_height,(boxes[i][2] * input_img_height)))
-                xmax = int(min(input_img_width,(boxes[i][3] * input_img_width)))
-                label_dict["confidence"] = scores[i]
-                label_dict["label_bounding_box"] = [{"x": xmin, "y": ymin}, {"x": xmax, "y": ymax}]
-                label_dict["label_class_name"] = labels_list[int(classes[i])]
-                detection_list.append(label_dict)
-        processing_time = stop_time - start_time
-        detection_response= {"detection": detection_list, "processing_time": processing_time}
-        return detection_response
-
-
-class edgeObjectDetectionTfLite():
-    """
-    Object detection inference using Tensorflow Lite models. 
-    This class includes loading the model, preparing input data, invoking the interpreter, and extracting output results. 
-    """
-    def __init__(self, model_file_path):
-        # Load the TensorFlow Lite model
-        self.interpreter = tf.lite.Interpreter(model_path=model_file_path)
-        self.interpreter.allocate_tensors()
-
-        # Set input normalization parameters
-        self.input_mean = 127.5
-        self.input_std = 127.5
-
-    def detect(self, cv2_image, labels_list, threshold=0.1):
-        """
-        Parameters:
-            cv2_image: OpenCV 2 Image
-            labels_list: labels list
-            threshold: minimum score
-        Returns:
-            Array of Detections(Label, Bounding Box, Confidence score)
-        """
-        # # Get input and output details from the interpreter
-        input_details = self.interpreter.get_input_details()
-        output_details = self.interpreter.get_output_details()
-
-        # Convert the input image to RGB format
-        normalize_height = input_details[0]['shape'][1]
-        normalize_width = input_details[0]['shape'][2]
-
-        # convert input image to gray scale
-        image_rgb = cv2.cvtColor(cv2_image, cv2.COLOR_BGR2RGB)
-        input_img_height, input_img_width, _ = image_rgb.shape
-
-        # Resize the input image to match the model's input requirements
-        image_resized = cv2.resize(image_rgb, (normalize_width, normalize_height))
-
-        # Add an extra dimension to the input data
-        input_data = np.expand_dims(image_resized, axis=0)
-
-        # Check if the model expects floating-point input
-        floating_model = (input_details[0]['dtype'] == np.float32)
-        if input_details[0]['dtype'] == type(np.float32(1.0)):
-            floating_model = True
-
-        # Normalize the input data if floating_model is True
-        if floating_model:
-            input_data = (np.float32(input_data) - self.input_mean) / self.input_std
-        
-        # Set the input tensor for the interpreter
-        self.interpreter.set_tensor(input_details[0]['index'], input_data)
-
-        # Perform the model inference
-        start_time = time.time()
-        self.interpreter.invoke()
-        stop_time = time.time()
-
-        # Determine the indices for accessing the output tensor.The specific indices for accessing the output tensors depend on whether the model is a TensorFlow 1.x or TensorFlow 2.x model.
-        out_name = output_details[0]['name']
-        if ('StatefulPartitionedCall' in out_name): # This is a TF2 model
-            boxes_idx, classes_idx, scores_idx = 1, 3, 0
-        else: # This is a TF1 model
-            boxes_idx, classes_idx, scores_idx = 0, 1, 2
-
-        # Retrieve detection results
-        boxes = self.interpreter.get_tensor(output_details[boxes_idx]['index'])[0] # Bounding box coordinates of detected objects
-        classes = self.interpreter.get_tensor(output_details[classes_idx]['index'])[0] # Class index of detected objects
-        scores = self.interpreter.get_tensor(output_details[scores_idx]['index'])[0] # Confidence of detected objects
-
-        # Create custom response
-        detection_response = {}
-        detection_list = []
-        for i in range(len(scores)):
-            label_dict = IMAGE_DETECTION_RESPONSE.copy()
-            if ((scores[i] > 0.6) and (scores[i] <= 1.0)):
-                ymin = int(max(1,(boxes[i][0] * input_img_height)))
-                xmin = int(max(1,(boxes[i][1] * input_img_width)))
-                ymax = int(min(input_img_height,(boxes[i][2] * input_img_height)))
-                xmax = int(min(input_img_width,(boxes[i][3] * input_img_width)))
-                label_dict["confidence"] = scores[i]
-                label_dict["label_bounding_box"] = [{"x": xmin, "y": ymin}, {"x": xmax, "y": ymax}]
-                label_dict["label_class_name"] = labels_list[int(classes[i])]
-                detection_list.append(label_dict)
-        processing_time = stop_time - start_time
-        detection_response= {"detection": detection_list, "processing_time": processing_time}
-        return detection_response
-
-
+        if model_type == "ssd":
+            # Retrieve detection results
+            boxes = self.interpreter.get_tensor(output_details[boxes_idx]['index'])[0] # Bounding box coordinates of detected objects
+            classes = self.interpreter.get_tensor(output_details[classes_idx]['index'])[0] # Class index of detected objects
+            scores = self.interpreter.get_tensor(output_details[scores_idx]['index'])[0] # Confidence of detected objects
+
+            # Create custom response
+            detection_response = {}
+            detection_list = []
+            for i in range(len(scores)):
+                label_dict = DETECTION_RESPONSE_BB.copy()
+                if ((scores[i] > threshold) and (scores[i] <= 1.0)):
+                    ymin = int(max(1,(boxes[i][0] * input_img_height)))
+                    xmin = int(max(1,(boxes[i][1] * input_img_width)))
+                    ymax = int(min(input_img_height,(boxes[i][2] * input_img_height)))
+                    xmax = int(min(input_img_width,(boxes[i][3] * input_img_width)))
+                    label_dict["confidence"] = scores[i]
+                    label_dict["label_bounding_box"] = [{"x": xmin, "y": ymin}, {"x": xmax, "y": ymax}]
+                    label_dict["label_class_name"] = labels_list[int(classes[i])]
+                    detection_list.append(label_dict)
+            processing_time = stop_time - start_time
+            detection_response= {"detection": detection_list, "processing_time": processing_time}
+            return detection_response
+        else:
+            output_data = self.interpreter.get_tensor(output_details[0]['index'])
+            results = np.squeeze(output_data)
+            top_k = results.argsort()[-5:][::-1]
+            detection_list = []
+            for i in top_k:
+                print(labels_list[i])
+                detection_list.append(' '.join(labels_list[i].split()[1:]))
+            processing_time = stop_time - start_time
+            detection_response = {"detection": detection_list, "processing_time": processing_time}
+            return detection_response
```

### Comparing `innovationmerge-1.0.6/innovationmerge/src/utils/responses.py` & `innovationmerge-1.0.7/innovationmerge/src/utils/responses.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,30 +26,53 @@
        labelSize, baseLine = cv2.getTextSize(label, cv2.FONT_HERSHEY_SIMPLEX, 0.7, 2)
        label_ymin = max(ymin, labelSize[1] + 10)
        cv2.rectangle(cv2_image, (xmin, label_ymin-labelSize[1]-10), (xmin+labelSize[0], label_ymin+baseLine-10), (255, 255, 255), cv2.FILLED)
        cv2.putText(cv2_image, label, (xmin, label_ymin-7), cv2.FONT_HERSHEY_SIMPLEX, 0.7, (0, 0, 0), 2)
     return cv2_image
 
 
-def save_detection_image(detections, cv2_image, output_image_path):
-    for detection in detections.get("detection"):
-       xmin = detection.get("label_bounding_box")[0].get("x")
-       ymin = detection.get("label_bounding_box")[0].get("y")
-       xmax = detection.get("label_bounding_box")[1].get("x")
-       ymax = detection.get("label_bounding_box")[1].get("y")
-       cv2.rectangle(cv2_image, (xmin, ymin), (xmax, ymax), (10, 255, 0), 2)
-        # Draw label
-       object_name = detection["label_class_name"]
-       confidence = detection["confidence"]
-       label = '%s: %d%%' % (object_name, int(confidence*100))
-       labelSize, baseLine = cv2.getTextSize(label, cv2.FONT_HERSHEY_SIMPLEX, 0.7, 2)
-       label_ymin = max(ymin, labelSize[1] + 10)
-       cv2.rectangle(cv2_image, (xmin, label_ymin-labelSize[1]-10), (xmin+labelSize[0], label_ymin+baseLine-10), (255, 255, 255), cv2.FILLED)
-       cv2.putText(cv2_image, label, (xmin, label_ymin-7), cv2.FONT_HERSHEY_SIMPLEX, 0.7, (0, 0, 0), 2)
-    cv2.imwrite(output_image_path, cv2_image)
+def save_detection_image(detections : dict, cv2_image, output_image_path: str, model_type: str = "ssd"):
+
+    if model_type == "ssd":
+        for detection in detections.get("detection"):
+            xmin = detection.get("label_bounding_box")[0].get("x")
+            ymin = detection.get("label_bounding_box")[0].get("y")
+            xmax = detection.get("label_bounding_box")[1].get("x")
+            ymax = detection.get("label_bounding_box")[1].get("y")
+            cv2.rectangle(cv2_image, (xmin, ymin), (xmax, ymax), (10, 255, 0), 2)
+            # Draw label
+            object_name = detection["label_class_name"]
+            confidence = detection["confidence"]
+            label = '%s: %d%%' % (object_name, int(confidence*100))
+            labelSize, baseLine = cv2.getTextSize(label, cv2.FONT_HERSHEY_SIMPLEX, 0.7, 2)
+            label_ymin = max(ymin, labelSize[1] + 10)
+            cv2.rectangle(cv2_image, (xmin, label_ymin-labelSize[1]-10), (xmin+labelSize[0], label_ymin+baseLine-10), (255, 255, 255), cv2.FILLED)
+            cv2.putText(cv2_image, label, (xmin, label_ymin-7), cv2.FONT_HERSHEY_SIMPLEX, 0.7, (0, 0, 0), 2)
+        cv2.imwrite(output_image_path, cv2_image)
+    else:
+        position = (30, 30)
+        font_scale = 0.75
+        color = (255, 255, 255)
+        thickness = 2
+        font = cv2.FONT_HERSHEY_SIMPLEX
+        line_type = cv2.LINE_AA
+        x, y0 = position
+        for i, line in enumerate(detections.get("detection")):
+            text_size, _ = cv2.getTextSize(line, font, font_scale, thickness)
+            line_height = text_size[1] + 5
+            y = y0 + i * line_height
+            cv2.putText(cv2_image,
+                        line,
+                        (x, y),
+                        font,
+                        font_scale,
+                        color,
+                        thickness,
+                        line_type)
+        cv2.imwrite(output_image_path, cv2_image)
 
 
 def show_detection_image(cv2_image):
     cv2.imshow('Detection', cv2_image)
     # Press any key to continue to next image, or press 'q' to quit
     if cv2.waitKey(0) == ord('q'):
         time.sleep(10)
```

### Comparing `innovationmerge-1.0.6/innovationmerge/tests/sample.py` & `innovationmerge-1.0.7/innovationmerge/tests/sample.py`

 * *Files identical despite different names*

### Comparing `innovationmerge-1.0.6/innovationmerge/tests/test_object_detection.py` & `innovationmerge-1.0.7/innovationmerge/tests/test_object_detection.py`

 * *Files identical despite different names*

### Comparing `innovationmerge-1.0.6/pyproject.toml` & `innovationmerge-1.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "innovationmerge"
-version = "1.0.6"
+version = "1.0.7"
 description = "innovationmerge core components"
 authors = ["innovationmerge"]
 readme = "README.md"
 packages = [{include = "innovationmerge"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
```

### Comparing `innovationmerge-1.0.6/PKG-INFO` & `innovationmerge-1.0.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: innovationmerge
-Version: 1.0.6
+Version: 1.0.7
 Summary: innovationmerge core components
 Author: innovationmerge
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -42,8 +42,8 @@
 
 ## Install using pip
 - `poetry add innovationmerge`
 
 ## Components
 
 ### Edge Computing
-1. `Object Detection`
+1. `Object Detection` - Currently SSD and MobileNet models are supported
```

