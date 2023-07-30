# Comparing `tmp/OneOnOne-0.701.tar.gz` & `tmp/OneOnOne-0.702.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OneOnOne-0.701.tar", last modified: Sun Jul 30 08:57:12 2023, max compression
+gzip compressed data, was "OneOnOne-0.702.tar", last modified: Sun Jul 30 09:08:16 2023, max compression
```

## Comparing `OneOnOne-0.701.tar` & `OneOnOne-0.702.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-30 08:57:12.747926 OneOnOne-0.701/
--rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.701/LICENSE
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-30 08:57:12.744503 OneOnOne-0.701/OneOnOne/
--rw-r--r--   0 sohinib    (501) staff       (20)    71874 2023-07-30 08:57:06.000000 OneOnOne-0.701/OneOnOne/__init__.py
--rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.701/OneOnOne/classes.py
--rw-r--r--   0 sohinib    (501) staff       (20)    14251 2023-07-28 06:59:10.000000 OneOnOne-0.701/OneOnOne/classification.py
--rw-r--r--   0 sohinib    (501) staff       (20)     7164 2023-07-29 12:25:37.000000 OneOnOne-0.701/OneOnOne/clustering.py
--rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.701/OneOnOne/contextdecider.py
--rw-r--r--   0 sohinib    (501) staff       (20)     3403 2023-07-29 18:08:15.000000 OneOnOne-0.701/OneOnOne/conversation.py
--rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.701/OneOnOne/htmlparser.py
--rw-r--r--   0 sohinib    (501) staff       (20)     2190 2023-07-30 08:22:15.000000 OneOnOne-0.701/OneOnOne/imagetranslator.py
--rw-r--r--   0 sohinib    (501) staff       (20)      995 2023-07-29 18:59:58.000000 OneOnOne-0.701/OneOnOne/pdftotext.py
--rw-r--r--   0 sohinib    (501) staff       (20)     1880 2023-07-28 06:59:09.000000 OneOnOne-0.701/OneOnOne/pretrainedmodel.py
--rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.701/OneOnOne/questionanswer.py
--rw-r--r--   0 sohinib    (501) staff       (20)    23928 2023-07-28 06:59:10.000000 OneOnOne-0.701/OneOnOne/sampling.py
--rw-r--r--   0 sohinib    (501) staff       (20)      888 2023-07-29 17:53:14.000000 OneOnOne-0.701/OneOnOne/texttranslator.py
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-30 08:57:12.746864 OneOnOne-0.701/OneOnOne.egg-info/
--rw-r--r--   0 sohinib    (501) staff       (20)     1596 2023-07-30 08:57:12.000000 OneOnOne-0.701/OneOnOne.egg-info/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)      504 2023-07-30 08:57:12.000000 OneOnOne-0.701/OneOnOne.egg-info/SOURCES.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-30 08:57:12.000000 OneOnOne-0.701/OneOnOne.egg-info/dependency_links.txt
--rw-r--r--   0 sohinib    (501) staff       (20)      233 2023-07-30 08:57:12.000000 OneOnOne-0.701/OneOnOne.egg-info/requires.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-30 08:57:12.000000 OneOnOne-0.701/OneOnOne.egg-info/top_level.txt
--rw-r--r--   0 sohinib    (501) staff       (20)     1596 2023-07-30 08:57:12.747290 OneOnOne-0.701/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)     3701 2023-07-29 19:02:55.000000 OneOnOne-0.701/README.md
--rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-30 08:57:12.748035 OneOnOne-0.701/setup.cfg
--rw-r--r--   0 sohinib    (501) staff       (20)     2069 2023-07-30 08:57:06.000000 OneOnOne-0.701/setup.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-30 09:08:16.115242 OneOnOne-0.702/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.702/LICENSE
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-30 09:08:16.107468 OneOnOne-0.702/OneOnOne/
+-rw-r--r--   0 sohinib    (501) staff       (20)    71867 2023-07-30 09:08:08.000000 OneOnOne-0.702/OneOnOne/__init__.py
+-rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.702/OneOnOne/classes.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    14251 2023-07-28 06:59:10.000000 OneOnOne-0.702/OneOnOne/classification.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     7164 2023-07-29 12:25:37.000000 OneOnOne-0.702/OneOnOne/clustering.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.702/OneOnOne/contextdecider.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     3403 2023-07-29 18:08:15.000000 OneOnOne-0.702/OneOnOne/conversation.py
+-rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.702/OneOnOne/htmlparser.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     2190 2023-07-30 08:22:15.000000 OneOnOne-0.702/OneOnOne/imagetranslator.py
+-rw-r--r--   0 sohinib    (501) staff       (20)      995 2023-07-29 18:59:58.000000 OneOnOne-0.702/OneOnOne/pdftotext.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     1880 2023-07-28 06:59:09.000000 OneOnOne-0.702/OneOnOne/pretrainedmodel.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.702/OneOnOne/questionanswer.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    23928 2023-07-28 06:59:10.000000 OneOnOne-0.702/OneOnOne/sampling.py
+-rw-r--r--   0 sohinib    (501) staff       (20)      888 2023-07-29 17:53:14.000000 OneOnOne-0.702/OneOnOne/texttranslator.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-30 09:08:16.112985 OneOnOne-0.702/OneOnOne.egg-info/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1596 2023-07-30 09:08:15.000000 OneOnOne-0.702/OneOnOne.egg-info/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)      504 2023-07-30 09:08:15.000000 OneOnOne-0.702/OneOnOne.egg-info/SOURCES.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-30 09:08:15.000000 OneOnOne-0.702/OneOnOne.egg-info/dependency_links.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)      233 2023-07-30 09:08:15.000000 OneOnOne-0.702/OneOnOne.egg-info/requires.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-30 09:08:15.000000 OneOnOne-0.702/OneOnOne.egg-info/top_level.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)     1596 2023-07-30 09:08:16.114266 OneOnOne-0.702/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)     3701 2023-07-29 19:02:55.000000 OneOnOne-0.702/README.md
+-rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-30 09:08:16.115535 OneOnOne-0.702/setup.cfg
+-rw-r--r--   0 sohinib    (501) staff       (20)     2069 2023-07-30 09:08:08.000000 OneOnOne-0.702/setup.py
```

### Comparing `OneOnOne-0.701/LICENSE` & `OneOnOne-0.702/LICENSE`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.701/OneOnOne/__init__.py` & `OneOnOne-0.702/OneOnOne/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -554,15 +554,15 @@
         else:
             feature_extractor = self.feature_extractor(inputs)
             classification_output = self.classifier(feature_extractor)
 
         return classification_output
 
     def define_compile_model(self):
-        inputs = tf.keras.layers.Input(shape=self.input_shape)
+        inputs = tf.keras.layers.Input(shape=(32,32,3))
 
         classification_output = self.final_model(inputs)
         model = tf.keras.Model(inputs=inputs, outputs=classification_output)
 
         model.compile(optimizer='SGD',
                       loss='categorical_crossentropy',
                       metrics=['accuracy'])
```

### Comparing `OneOnOne-0.701/OneOnOne/classes.py` & `OneOnOne-0.702/OneOnOne/classes.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.701/OneOnOne/classification.py` & `OneOnOne-0.702/OneOnOne/classification.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.701/OneOnOne/clustering.py` & `OneOnOne-0.702/OneOnOne/clustering.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.701/OneOnOne/contextdecider.py` & `OneOnOne-0.702/OneOnOne/contextdecider.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.701/OneOnOne/conversation.py` & `OneOnOne-0.702/OneOnOne/conversation.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.701/OneOnOne/htmlparser.py` & `OneOnOne-0.702/OneOnOne/htmlparser.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.701/OneOnOne/imagetranslator.py` & `OneOnOne-0.702/OneOnOne/imagetranslator.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.701/OneOnOne/pdftotext.py` & `OneOnOne-0.702/OneOnOne/pdftotext.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.701/OneOnOne/pretrainedmodel.py` & `OneOnOne-0.702/OneOnOne/pretrainedmodel.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.701/OneOnOne/questionanswer.py` & `OneOnOne-0.702/OneOnOne/questionanswer.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.701/OneOnOne/sampling.py` & `OneOnOne-0.702/OneOnOne/sampling.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.701/OneOnOne/texttranslator.py` & `OneOnOne-0.702/OneOnOne/texttranslator.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.701/OneOnOne.egg-info/PKG-INFO` & `OneOnOne-0.702/OneOnOne.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.701
+Version: 0.702
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,speech-recognition,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.701/PKG-INFO` & `OneOnOne-0.702/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.701
+Version: 0.702
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,speech-recognition,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.701/README.md` & `OneOnOne-0.702/README.md`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.701/setup.py` & `OneOnOne-0.702/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION=0.701
+VERSION=0.702
 
 DESCRIPTION="A package for pre-trained image classification and context-decider for question-answering chatbots."
 LONG_DESCRIPTION="Your one-stop destination to utilize image-classification models with just one line of code. A library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, no need to worry! This library has got you covered. Along with that for simple-bridging and basic into NLP, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset. This library is being actively updated and new features are being added frequently. New datasets and pre-trained models will be updated soon. Feel free to share your feedback! I would really appreciate it!"
 CLASSIFIERS=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Education',
     'License :: OSI Approved :: MIT License',
```

