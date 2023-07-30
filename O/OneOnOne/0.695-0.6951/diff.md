# Comparing `tmp/OneOnOne-0.695.tar.gz` & `tmp/OneOnOne-0.6951.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OneOnOne-0.695.tar", last modified: Sun Jul 30 06:09:35 2023, max compression
+gzip compressed data, was "OneOnOne-0.6951.tar", last modified: Sun Jul 30 06:31:11 2023, max compression
```

## Comparing `OneOnOne-0.695.tar` & `OneOnOne-0.6951.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-30 06:09:35.849641 OneOnOne-0.695/
--rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.695/LICENSE
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-30 06:09:35.844023 OneOnOne-0.695/OneOnOne/
--rw-r--r--   0 sohinib    (501) staff       (20)    70464 2023-07-29 19:06:01.000000 OneOnOne-0.695/OneOnOne/__init__.py
--rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.695/OneOnOne/classes.py
--rw-r--r--   0 sohinib    (501) staff       (20)    14251 2023-07-28 06:59:10.000000 OneOnOne-0.695/OneOnOne/classification.py
--rw-r--r--   0 sohinib    (501) staff       (20)     7164 2023-07-29 12:25:37.000000 OneOnOne-0.695/OneOnOne/clustering.py
--rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.695/OneOnOne/contextdecider.py
--rw-r--r--   0 sohinib    (501) staff       (20)     3403 2023-07-29 18:08:15.000000 OneOnOne-0.695/OneOnOne/conversation.py
--rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.695/OneOnOne/htmlparser.py
--rw-r--r--   0 sohinib    (501) staff       (20)     1930 2023-07-29 18:38:09.000000 OneOnOne-0.695/OneOnOne/imagetranslator.py
--rw-r--r--   0 sohinib    (501) staff       (20)      995 2023-07-29 18:59:58.000000 OneOnOne-0.695/OneOnOne/pdftotext.py
--rw-r--r--   0 sohinib    (501) staff       (20)     1880 2023-07-28 06:59:09.000000 OneOnOne-0.695/OneOnOne/pretrainedmodel.py
--rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.695/OneOnOne/questionanswer.py
--rw-r--r--   0 sohinib    (501) staff       (20)    23928 2023-07-28 06:59:10.000000 OneOnOne-0.695/OneOnOne/sampling.py
--rw-r--r--   0 sohinib    (501) staff       (20)      888 2023-07-29 17:53:14.000000 OneOnOne-0.695/OneOnOne/texttranslator.py
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-30 06:09:35.847917 OneOnOne-0.695/OneOnOne.egg-info/
--rw-r--r--   0 sohinib    (501) staff       (20)     1596 2023-07-30 06:09:35.000000 OneOnOne-0.695/OneOnOne.egg-info/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)      504 2023-07-30 06:09:35.000000 OneOnOne-0.695/OneOnOne.egg-info/SOURCES.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-30 06:09:35.000000 OneOnOne-0.695/OneOnOne.egg-info/dependency_links.txt
--rw-r--r--   0 sohinib    (501) staff       (20)      213 2023-07-30 06:09:35.000000 OneOnOne-0.695/OneOnOne.egg-info/requires.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-30 06:09:35.000000 OneOnOne-0.695/OneOnOne.egg-info/top_level.txt
--rw-r--r--   0 sohinib    (501) staff       (20)     1596 2023-07-30 06:09:35.849026 OneOnOne-0.695/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)     3701 2023-07-29 19:02:55.000000 OneOnOne-0.695/README.md
--rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-30 06:09:35.849835 OneOnOne-0.695/setup.cfg
--rw-r--r--   0 sohinib    (501) staff       (20)     2047 2023-07-30 06:09:28.000000 OneOnOne-0.695/setup.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-30 06:31:11.171913 OneOnOne-0.6951/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6951/LICENSE
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-30 06:31:11.163370 OneOnOne-0.6951/OneOnOne/
+-rw-r--r--   0 sohinib    (501) staff       (20)    70464 2023-07-29 19:06:01.000000 OneOnOne-0.6951/OneOnOne/__init__.py
+-rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6951/OneOnOne/classes.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    14251 2023-07-28 06:59:10.000000 OneOnOne-0.6951/OneOnOne/classification.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     7164 2023-07-29 12:25:37.000000 OneOnOne-0.6951/OneOnOne/clustering.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.6951/OneOnOne/contextdecider.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     3403 2023-07-29 18:08:15.000000 OneOnOne-0.6951/OneOnOne/conversation.py
+-rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.6951/OneOnOne/htmlparser.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     1930 2023-07-29 18:38:09.000000 OneOnOne-0.6951/OneOnOne/imagetranslator.py
+-rw-r--r--   0 sohinib    (501) staff       (20)      995 2023-07-29 18:59:58.000000 OneOnOne-0.6951/OneOnOne/pdftotext.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     1880 2023-07-28 06:59:09.000000 OneOnOne-0.6951/OneOnOne/pretrainedmodel.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.6951/OneOnOne/questionanswer.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    23928 2023-07-28 06:59:10.000000 OneOnOne-0.6951/OneOnOne/sampling.py
+-rw-r--r--   0 sohinib    (501) staff       (20)      888 2023-07-29 17:53:14.000000 OneOnOne-0.6951/OneOnOne/texttranslator.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-30 06:31:11.169531 OneOnOne-0.6951/OneOnOne.egg-info/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1597 2023-07-30 06:31:11.000000 OneOnOne-0.6951/OneOnOne.egg-info/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)      504 2023-07-30 06:31:11.000000 OneOnOne-0.6951/OneOnOne.egg-info/SOURCES.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-30 06:31:11.000000 OneOnOne-0.6951/OneOnOne.egg-info/dependency_links.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)      221 2023-07-30 06:31:11.000000 OneOnOne-0.6951/OneOnOne.egg-info/requires.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-30 06:31:11.000000 OneOnOne-0.6951/OneOnOne.egg-info/top_level.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)     1597 2023-07-30 06:31:11.170954 OneOnOne-0.6951/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)     3701 2023-07-29 19:02:55.000000 OneOnOne-0.6951/README.md
+-rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-30 06:31:11.172130 OneOnOne-0.6951/setup.cfg
+-rw-r--r--   0 sohinib    (501) staff       (20)     2056 2023-07-30 06:31:06.000000 OneOnOne-0.6951/setup.py
```

### Comparing `OneOnOne-0.695/LICENSE` & `OneOnOne-0.6951/LICENSE`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.695/OneOnOne/__init__.py` & `OneOnOne-0.6951/OneOnOne/__init__.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.695/OneOnOne/classes.py` & `OneOnOne-0.6951/OneOnOne/classes.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.695/OneOnOne/classification.py` & `OneOnOne-0.6951/OneOnOne/classification.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.695/OneOnOne/clustering.py` & `OneOnOne-0.6951/OneOnOne/clustering.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.695/OneOnOne/contextdecider.py` & `OneOnOne-0.6951/OneOnOne/contextdecider.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.695/OneOnOne/conversation.py` & `OneOnOne-0.6951/OneOnOne/conversation.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.695/OneOnOne/htmlparser.py` & `OneOnOne-0.6951/OneOnOne/htmlparser.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.695/OneOnOne/imagetranslator.py` & `OneOnOne-0.6951/OneOnOne/imagetranslator.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.695/OneOnOne/pdftotext.py` & `OneOnOne-0.6951/OneOnOne/pdftotext.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.695/OneOnOne/pretrainedmodel.py` & `OneOnOne-0.6951/OneOnOne/pretrainedmodel.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.695/OneOnOne/questionanswer.py` & `OneOnOne-0.6951/OneOnOne/questionanswer.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.695/OneOnOne/sampling.py` & `OneOnOne-0.6951/OneOnOne/sampling.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.695/OneOnOne/texttranslator.py` & `OneOnOne-0.6951/OneOnOne/texttranslator.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.695/OneOnOne.egg-info/PKG-INFO` & `OneOnOne-0.6951/OneOnOne.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.695
+Version: 0.6951
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,speech-recognition,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.695/PKG-INFO` & `OneOnOne-0.6951/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.695
+Version: 0.6951
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,speech-recognition,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.695/README.md` & `OneOnOne-0.6951/README.md`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.695/setup.py` & `OneOnOne-0.6951/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
-VERSION=0.695
+VERSION=0.6951
 
 DESCRIPTION="A package for pre-trained image classification and context-decider for question-answering chatbots."
 LONG_DESCRIPTION="Your one-stop destination to utilize image-classification models with just one line of code. A library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, no need to worry! This library has got you covered. Along with that for simple-bridging and basic into NLP, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset. This library is being actively updated and new features are being added frequently. New datasets and pre-trained models will be updated soon. Feel free to share your feedback! I would really appreciate it!"
 CLASSIFIERS=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Education',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
-setup(name="OneOnOne",version=VERSION,description=DESCRIPTION, long_description=LONG_DESCRIPTION,author="Sohini Bhattacharya",author_email="mail.sohinibhattacharya@gmail.com",License="MIT",packages=find_packages(),keywords=["python","image-classification","active-learning-sampling","question-answering","pre-trained models","tiny-image-net","speech-recognition","cifar10"],classifiers=CLASSIFIERS,install_requires=["wget","pytesseract","bayesian-optimization","speechrecognition","pyttsx3","pydub","pyaudio","torch","transformers","gdown","numpy","pandas","tensorflow==2.12.0","datetime","keras==2.12.0","tensorflow_datasets==4.9.2","scipy==1.10.1","tqdm==4.65.0"])
+setup(name="OneOnOne",version=VERSION,description=DESCRIPTION, long_description=LONG_DESCRIPTION,author="Sohini Bhattacharya",author_email="mail.sohinibhattacharya@gmail.com",License="MIT",packages=find_packages(),keywords=["python","image-classification","active-learning-sampling","question-answering","pre-trained models","tiny-image-net","speech-recognition","cifar10"],classifiers=CLASSIFIERS,install_requires=["wget","pytesseract","bayesian-optimization","speechrecognition","pyttsx3","pyaudio==0.2.13","pydub","torch","transformers","gdown","numpy","pandas","tensorflow==2.12.0","datetime","keras==2.12.0","tensorflow_datasets==4.9.2","scipy==1.10.1","tqdm==4.65.0"])
```

