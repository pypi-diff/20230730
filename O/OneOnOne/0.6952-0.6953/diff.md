# Comparing `tmp/OneOnOne-0.6952.tar.gz` & `tmp/OneOnOne-0.6953.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OneOnOne-0.6952.tar", last modified: Sun Jul 30 06:34:42 2023, max compression
+gzip compressed data, was "OneOnOne-0.6953.tar", last modified: Sun Jul 30 06:38:08 2023, max compression
```

## Comparing `OneOnOne-0.6952.tar` & `OneOnOne-0.6953.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-30 06:34:42.546010 OneOnOne-0.6952/
--rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6952/LICENSE
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-30 06:34:42.540622 OneOnOne-0.6952/OneOnOne/
--rw-r--r--   0 sohinib    (501) staff       (20)    70532 2023-07-30 06:33:55.000000 OneOnOne-0.6952/OneOnOne/__init__.py
--rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6952/OneOnOne/classes.py
--rw-r--r--   0 sohinib    (501) staff       (20)    14251 2023-07-28 06:59:10.000000 OneOnOne-0.6952/OneOnOne/classification.py
--rw-r--r--   0 sohinib    (501) staff       (20)     7164 2023-07-29 12:25:37.000000 OneOnOne-0.6952/OneOnOne/clustering.py
--rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.6952/OneOnOne/contextdecider.py
--rw-r--r--   0 sohinib    (501) staff       (20)     3403 2023-07-29 18:08:15.000000 OneOnOne-0.6952/OneOnOne/conversation.py
--rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.6952/OneOnOne/htmlparser.py
--rw-r--r--   0 sohinib    (501) staff       (20)     1930 2023-07-29 18:38:09.000000 OneOnOne-0.6952/OneOnOne/imagetranslator.py
--rw-r--r--   0 sohinib    (501) staff       (20)      995 2023-07-29 18:59:58.000000 OneOnOne-0.6952/OneOnOne/pdftotext.py
--rw-r--r--   0 sohinib    (501) staff       (20)     1880 2023-07-28 06:59:09.000000 OneOnOne-0.6952/OneOnOne/pretrainedmodel.py
--rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.6952/OneOnOne/questionanswer.py
--rw-r--r--   0 sohinib    (501) staff       (20)    23928 2023-07-28 06:59:10.000000 OneOnOne-0.6952/OneOnOne/sampling.py
--rw-r--r--   0 sohinib    (501) staff       (20)      888 2023-07-29 17:53:14.000000 OneOnOne-0.6952/OneOnOne/texttranslator.py
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-30 06:34:42.544413 OneOnOne-0.6952/OneOnOne.egg-info/
--rw-r--r--   0 sohinib    (501) staff       (20)     1597 2023-07-30 06:34:42.000000 OneOnOne-0.6952/OneOnOne.egg-info/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)      504 2023-07-30 06:34:42.000000 OneOnOne-0.6952/OneOnOne.egg-info/SOURCES.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-30 06:34:42.000000 OneOnOne-0.6952/OneOnOne.egg-info/dependency_links.txt
--rw-r--r--   0 sohinib    (501) staff       (20)      205 2023-07-30 06:34:42.000000 OneOnOne-0.6952/OneOnOne.egg-info/requires.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-30 06:34:42.000000 OneOnOne-0.6952/OneOnOne.egg-info/top_level.txt
--rw-r--r--   0 sohinib    (501) staff       (20)     1597 2023-07-30 06:34:42.545225 OneOnOne-0.6952/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)     3701 2023-07-29 19:02:55.000000 OneOnOne-0.6952/README.md
--rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-30 06:34:42.546487 OneOnOne-0.6952/setup.cfg
--rw-r--r--   0 sohinib    (501) staff       (20)     2038 2023-07-30 06:34:37.000000 OneOnOne-0.6952/setup.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-30 06:38:08.259418 OneOnOne-0.6953/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6953/LICENSE
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-30 06:38:08.256011 OneOnOne-0.6953/OneOnOne/
+-rw-r--r--   0 sohinib    (501) staff       (20)    70545 2023-07-30 06:36:45.000000 OneOnOne-0.6953/OneOnOne/__init__.py
+-rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6953/OneOnOne/classes.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    14251 2023-07-28 06:59:10.000000 OneOnOne-0.6953/OneOnOne/classification.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     7164 2023-07-29 12:25:37.000000 OneOnOne-0.6953/OneOnOne/clustering.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.6953/OneOnOne/contextdecider.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     3403 2023-07-29 18:08:15.000000 OneOnOne-0.6953/OneOnOne/conversation.py
+-rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.6953/OneOnOne/htmlparser.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     1930 2023-07-29 18:38:09.000000 OneOnOne-0.6953/OneOnOne/imagetranslator.py
+-rw-r--r--   0 sohinib    (501) staff       (20)      995 2023-07-29 18:59:58.000000 OneOnOne-0.6953/OneOnOne/pdftotext.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     1880 2023-07-28 06:59:09.000000 OneOnOne-0.6953/OneOnOne/pretrainedmodel.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.6953/OneOnOne/questionanswer.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    23928 2023-07-28 06:59:10.000000 OneOnOne-0.6953/OneOnOne/sampling.py
+-rw-r--r--   0 sohinib    (501) staff       (20)      888 2023-07-29 17:53:14.000000 OneOnOne-0.6953/OneOnOne/texttranslator.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-30 06:38:08.258566 OneOnOne-0.6953/OneOnOne.egg-info/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1597 2023-07-30 06:38:08.000000 OneOnOne-0.6953/OneOnOne.egg-info/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)      504 2023-07-30 06:38:08.000000 OneOnOne-0.6953/OneOnOne.egg-info/SOURCES.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-30 06:38:08.000000 OneOnOne-0.6953/OneOnOne.egg-info/dependency_links.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)      226 2023-07-30 06:38:08.000000 OneOnOne-0.6953/OneOnOne.egg-info/requires.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-30 06:38:08.000000 OneOnOne-0.6953/OneOnOne.egg-info/top_level.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)     1597 2023-07-30 06:38:08.259014 OneOnOne-0.6953/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)     3701 2023-07-29 19:02:55.000000 OneOnOne-0.6953/README.md
+-rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-30 06:38:08.259531 OneOnOne-0.6953/setup.cfg
+-rw-r--r--   0 sohinib    (501) staff       (20)     2061 2023-07-30 06:37:57.000000 OneOnOne-0.6953/setup.py
```

### Comparing `OneOnOne-0.6952/LICENSE` & `OneOnOne-0.6953/LICENSE`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6952/OneOnOne/__init__.py` & `OneOnOne-0.6953/OneOnOne/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -441,15 +441,15 @@
         return keys, total_list_parameter_history
 
     def evaluate(self):
         loss, accuracy = self.model.evaluate(self.val_it, batch_size=self.batch_size, verbose=1)
 
 
 class Sampling:
-    def __init__(self, samplingtype, dataset="cifar10", model_type = "resnet50", goal=99, jump=5000, validation_split=0.3, first_data_samples=10000, batch_size = 16, epochs = 250, shuffle_bool = True, early_stopping_patience = 10, lr_reducer_patience = 10):
+    def __init__(self, samplingtype="mixedbayes", dataset="cifar10", model_type = "resnet50", goal=99, jump=5000, validation_split=0.3, first_data_samples=10000, batch_size = 16, epochs = 250, shuffle_bool = True, early_stopping_patience = 10, lr_reducer_patience = 10):
         warnings.filterwarnings("ignore")
 
         self.validation_split=validation_split
         self.model_type = model_type.lower()
         self.epochs=epochs
         self.jump = jump
         self.samplingtype = samplingtype.lower()
```

### Comparing `OneOnOne-0.6952/OneOnOne/classes.py` & `OneOnOne-0.6953/OneOnOne/classes.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6952/OneOnOne/classification.py` & `OneOnOne-0.6953/OneOnOne/classification.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6952/OneOnOne/clustering.py` & `OneOnOne-0.6953/OneOnOne/clustering.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6952/OneOnOne/contextdecider.py` & `OneOnOne-0.6953/OneOnOne/contextdecider.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6952/OneOnOne/conversation.py` & `OneOnOne-0.6953/OneOnOne/conversation.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6952/OneOnOne/htmlparser.py` & `OneOnOne-0.6953/OneOnOne/htmlparser.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6952/OneOnOne/imagetranslator.py` & `OneOnOne-0.6953/OneOnOne/imagetranslator.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6952/OneOnOne/pdftotext.py` & `OneOnOne-0.6953/OneOnOne/pdftotext.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6952/OneOnOne/pretrainedmodel.py` & `OneOnOne-0.6953/OneOnOne/pretrainedmodel.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6952/OneOnOne/questionanswer.py` & `OneOnOne-0.6953/OneOnOne/questionanswer.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6952/OneOnOne/sampling.py` & `OneOnOne-0.6953/OneOnOne/sampling.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6952/OneOnOne/texttranslator.py` & `OneOnOne-0.6953/OneOnOne/texttranslator.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6952/OneOnOne.egg-info/PKG-INFO` & `OneOnOne-0.6953/OneOnOne.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.6952
+Version: 0.6953
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,speech-recognition,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.6952/PKG-INFO` & `OneOnOne-0.6953/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.6952
+Version: 0.6953
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,speech-recognition,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.6952/README.md` & `OneOnOne-0.6953/README.md`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6952/setup.py` & `OneOnOne-0.6953/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
-VERSION=0.6952
+VERSION=0.6953
 
 DESCRIPTION="A package for pre-trained image classification and context-decider for question-answering chatbots."
 LONG_DESCRIPTION="Your one-stop destination to utilize image-classification models with just one line of code. A library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, no need to worry! This library has got you covered. Along with that for simple-bridging and basic into NLP, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset. This library is being actively updated and new features are being added frequently. New datasets and pre-trained models will be updated soon. Feel free to share your feedback! I would really appreciate it!"
 CLASSIFIERS=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Education',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
-setup(name="OneOnOne",version=VERSION,description=DESCRIPTION, long_description=LONG_DESCRIPTION,author="Sohini Bhattacharya",author_email="mail.sohinibhattacharya@gmail.com",License="MIT",packages=find_packages(),keywords=["python","image-classification","active-learning-sampling","question-answering","pre-trained models","tiny-image-net","speech-recognition","cifar10"],classifiers=CLASSIFIERS,install_requires=["wget","pytesseract","bayesian-optimization","speechrecognition","pyttsx3","pydub","torch","transformers","gdown","numpy","pandas","tensorflow==2.12.0","datetime","keras==2.12.0","tensorflow_datasets==4.9.2","scipy==1.10.1","tqdm==4.65.0"])
+setup(name="OneOnOne",version=VERSION,description=DESCRIPTION, long_description=LONG_DESCRIPTION,author="Sohini Bhattacharya",author_email="mail.sohinibhattacharya@gmail.com",License="MIT",packages=find_packages(),keywords=["python","image-classification","active-learning-sampling","question-answering","pre-trained models","tiny-image-net","speech-recognition","cifar10"],classifiers=CLASSIFIERS,install_requires=["wget","pytesseract","bayesian-optimization","googletrans==3.1.0a0","speechrecognition","pyttsx3","pydub","torch","transformers","gdown","numpy","pandas","tensorflow==2.12.0","datetime","keras==2.12.0","tensorflow_datasets==4.9.2","scipy==1.10.1","tqdm==4.65.0"])
```

