# Comparing `tmp/OneOnOne-0.6959.tar.gz` & `tmp/OneOnOne-0.696.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OneOnOne-0.6959.tar", last modified: Sun Jul 30 08:17:08 2023, max compression
+gzip compressed data, was "OneOnOne-0.696.tar", last modified: Sun Jul 30 08:22:27 2023, max compression
```

## Comparing `OneOnOne-0.6959.tar` & `OneOnOne-0.696.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-30 08:17:08.095329 OneOnOne-0.6959/
--rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6959/LICENSE
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-30 08:17:08.092190 OneOnOne-0.6959/OneOnOne/
--rw-r--r--   0 sohinib    (501) staff       (20)    70706 2023-07-30 08:09:11.000000 OneOnOne-0.6959/OneOnOne/__init__.py
--rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6959/OneOnOne/classes.py
--rw-r--r--   0 sohinib    (501) staff       (20)    14251 2023-07-28 06:59:10.000000 OneOnOne-0.6959/OneOnOne/classification.py
--rw-r--r--   0 sohinib    (501) staff       (20)     7164 2023-07-29 12:25:37.000000 OneOnOne-0.6959/OneOnOne/clustering.py
--rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.6959/OneOnOne/contextdecider.py
--rw-r--r--   0 sohinib    (501) staff       (20)     3403 2023-07-29 18:08:15.000000 OneOnOne-0.6959/OneOnOne/conversation.py
--rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.6959/OneOnOne/htmlparser.py
--rw-r--r--   0 sohinib    (501) staff       (20)     2178 2023-07-30 08:17:03.000000 OneOnOne-0.6959/OneOnOne/imagetranslator.py
--rw-r--r--   0 sohinib    (501) staff       (20)      995 2023-07-29 18:59:58.000000 OneOnOne-0.6959/OneOnOne/pdftotext.py
--rw-r--r--   0 sohinib    (501) staff       (20)     1880 2023-07-28 06:59:09.000000 OneOnOne-0.6959/OneOnOne/pretrainedmodel.py
--rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.6959/OneOnOne/questionanswer.py
--rw-r--r--   0 sohinib    (501) staff       (20)    23928 2023-07-28 06:59:10.000000 OneOnOne-0.6959/OneOnOne/sampling.py
--rw-r--r--   0 sohinib    (501) staff       (20)      888 2023-07-29 17:53:14.000000 OneOnOne-0.6959/OneOnOne/texttranslator.py
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-30 08:17:08.094225 OneOnOne-0.6959/OneOnOne.egg-info/
--rw-r--r--   0 sohinib    (501) staff       (20)     1597 2023-07-30 08:17:07.000000 OneOnOne-0.6959/OneOnOne.egg-info/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)      504 2023-07-30 08:17:08.000000 OneOnOne-0.6959/OneOnOne.egg-info/SOURCES.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-30 08:17:07.000000 OneOnOne-0.6959/OneOnOne.egg-info/dependency_links.txt
--rw-r--r--   0 sohinib    (501) staff       (20)      233 2023-07-30 08:17:07.000000 OneOnOne-0.6959/OneOnOne.egg-info/requires.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-30 08:17:07.000000 OneOnOne-0.6959/OneOnOne.egg-info/top_level.txt
--rw-r--r--   0 sohinib    (501) staff       (20)     1597 2023-07-30 08:17:08.094650 OneOnOne-0.6959/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)     3701 2023-07-29 19:02:55.000000 OneOnOne-0.6959/README.md
--rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-30 08:17:08.095516 OneOnOne-0.6959/setup.cfg
--rw-r--r--   0 sohinib    (501) staff       (20)     2070 2023-07-30 08:17:03.000000 OneOnOne-0.6959/setup.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-30 08:22:27.413336 OneOnOne-0.696/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.696/LICENSE
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-30 08:22:27.410493 OneOnOne-0.696/OneOnOne/
+-rw-r--r--   0 sohinib    (501) staff       (20)    71822 2023-07-30 08:22:15.000000 OneOnOne-0.696/OneOnOne/__init__.py
+-rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.696/OneOnOne/classes.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    14251 2023-07-28 06:59:10.000000 OneOnOne-0.696/OneOnOne/classification.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     7164 2023-07-29 12:25:37.000000 OneOnOne-0.696/OneOnOne/clustering.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.696/OneOnOne/contextdecider.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     3403 2023-07-29 18:08:15.000000 OneOnOne-0.696/OneOnOne/conversation.py
+-rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.696/OneOnOne/htmlparser.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     2190 2023-07-30 08:22:15.000000 OneOnOne-0.696/OneOnOne/imagetranslator.py
+-rw-r--r--   0 sohinib    (501) staff       (20)      995 2023-07-29 18:59:58.000000 OneOnOne-0.696/OneOnOne/pdftotext.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     1880 2023-07-28 06:59:09.000000 OneOnOne-0.696/OneOnOne/pretrainedmodel.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.696/OneOnOne/questionanswer.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    23928 2023-07-28 06:59:10.000000 OneOnOne-0.696/OneOnOne/sampling.py
+-rw-r--r--   0 sohinib    (501) staff       (20)      888 2023-07-29 17:53:14.000000 OneOnOne-0.696/OneOnOne/texttranslator.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-30 08:22:27.412539 OneOnOne-0.696/OneOnOne.egg-info/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1596 2023-07-30 08:22:27.000000 OneOnOne-0.696/OneOnOne.egg-info/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)      504 2023-07-30 08:22:27.000000 OneOnOne-0.696/OneOnOne.egg-info/SOURCES.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-30 08:22:27.000000 OneOnOne-0.696/OneOnOne.egg-info/dependency_links.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)      233 2023-07-30 08:22:27.000000 OneOnOne-0.696/OneOnOne.egg-info/requires.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-30 08:22:27.000000 OneOnOne-0.696/OneOnOne.egg-info/top_level.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)     1596 2023-07-30 08:22:27.412960 OneOnOne-0.696/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)     3701 2023-07-29 19:02:55.000000 OneOnOne-0.696/README.md
+-rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-30 08:22:27.413443 OneOnOne-0.696/setup.cfg
+-rw-r--r--   0 sohinib    (501) staff       (20)     2069 2023-07-30 08:22:19.000000 OneOnOne-0.696/setup.py
```

### Comparing `OneOnOne-0.6959/LICENSE` & `OneOnOne-0.696/LICENSE`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6959/OneOnOne/__init__.py` & `OneOnOne-0.696/OneOnOne/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1402,18 +1402,35 @@
     def __init__(self, file_bool=False,filepath="", translate_from_language="ben", translate_to_language="en", speak_bool=False):
         self.file_bool=file_bool
         self.filepath=filepath
         self.translate_from_language = translate_from_language
         self.translate_to_language = translate_to_language
         self.speak_bool = speak_bool
 
-        sudo
-        apt
-        install
-        portaudio19 - dev
+        if self.speak_bool:
+            try:
+                os.system("sudo apt install espeak")
+                os.system("sudo apt install libespeak-dev")
+                os.system("pip install pyaudio")
+                os.system("sudo apt install python3-pyaudio")
+                os.system("sudo apt install portaudio19 - dev")
+
+            except:
+                os.system("!sudo apt install espeak")
+                os.system("!sudo apt install libespeak-dev")
+                os.system("!pip install pyaudio")
+                os.system("!sudo apt install python3-pyaudio")
+                os.system("!sudo apt install portaudio19 - dev")
+
+    def speak(self, command):
+        engine = pyttsx3.init()
+        engine.say(command)
+        engine.runAndWait()
+
+    def translate(self):
 
         if self.file_bool:
             file = open(os.getcwd()+f"/{self.filepath}","r")
             text=file.readlines()[0]
             print(file.readlines())
         else:
             text=input("What do you want to translate?:     ")
@@ -1430,28 +1447,38 @@
 class ImageTranslator:
     def __init__(self, imgpath, translate_from_language="ben", translate_to_language="en", speak_bool=False):
         self.translate_from_language=translate_from_language
         self.translate_to_language=translate_to_language
         self.imgpath=imgpath
         self.speak_bool=speak_bool
 
-    def speak(self, command):
 
-        engine = pyttsx3.init()
-        engine.say(command)
-        engine.runAndWait()
 
-        if speak:
+        if self.speak_bool:
             try:
                 os.system("sudo apt install espeak")
                 os.system("sudo apt install libespeak-dev")
+                os.system("pip install pyaudio")
+                os.system("sudo apt install python3-pyaudio")
+                os.system("sudo apt install portaudio19 - dev")
+
             except:
                 os.system("!sudo apt install espeak")
                 os.system("!sudo apt install libespeak-dev")
+                os.system("!pip install pyaudio")
+                os.system("!sudo apt install python3-pyaudio")
+                os.system("!sudo apt install portaudio19 - dev")
+
+    def speak(self, command):
+
+        engine = pyttsx3.init()
+        engine.say(command)
+        engine.runAndWait()
 
+    def translate(self):
 
         try:
             os.system("sudo apt install tesseract-ocr")
             os.system("apt install libtesseract-dev")
             os.system(f"apt install tesseract-ocr-{self.translate_from_language}")
             os.system(f"apt install tesseract-ocr-{self.translate_to_language}")
         except:
```

### Comparing `OneOnOne-0.6959/OneOnOne/classes.py` & `OneOnOne-0.696/OneOnOne/classes.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6959/OneOnOne/classification.py` & `OneOnOne-0.696/OneOnOne/classification.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6959/OneOnOne/clustering.py` & `OneOnOne-0.696/OneOnOne/clustering.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6959/OneOnOne/contextdecider.py` & `OneOnOne-0.696/OneOnOne/contextdecider.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6959/OneOnOne/conversation.py` & `OneOnOne-0.696/OneOnOne/conversation.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6959/OneOnOne/htmlparser.py` & `OneOnOne-0.696/OneOnOne/htmlparser.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6959/OneOnOne/imagetranslator.py` & `OneOnOne-0.696/OneOnOne/imagetranslator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 class ImageTranslator:
     def __init__(self, imgpath, translate_from_language="ben", translate_to_language="en", speak_bool=False):
         self.translate_from_language=translate_from_language
         self.translate_to_language=translate_to_language
         self.imgpath=imgpath
         self.speak_bool=speak_bool
 
-    def speak(self, command):
-
-        engine = pyttsx3.init()
-        engine.say(command)
-        engine.runAndWait()
-
-        if speak:
+        if self.speak_bool:
             try:
                 os.system("sudo apt install espeak")
                 os.system("sudo apt install libespeak-dev")
                 os.system("pip install pyaudio")
                 os.system("sudo apt install python3-pyaudio")
             except:
                 os.system("!sudo apt install espeak")
                 os.system("!sudo apt install libespeak-dev")
                 os.system("!pip install pyaudio")
                 os.system("!sudo apt install python3-pyaudio")
 
+    def speak(self, command):
+
+        engine = pyttsx3.init()
+        engine.say(command)
+        engine.runAndWait()
+
+
+
     def translate(self):
         try:
             os.system("sudo apt install tesseract-ocr")
             os.system("apt install libtesseract-dev")
             os.system(f"apt install tesseract-ocr-{self.translate_from_language}")
             os.system(f"apt install tesseract-ocr-{self.translate_to_language}")
         except:
```

### Comparing `OneOnOne-0.6959/OneOnOne/pdftotext.py` & `OneOnOne-0.696/OneOnOne/pdftotext.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6959/OneOnOne/pretrainedmodel.py` & `OneOnOne-0.696/OneOnOne/pretrainedmodel.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6959/OneOnOne/questionanswer.py` & `OneOnOne-0.696/OneOnOne/questionanswer.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6959/OneOnOne/sampling.py` & `OneOnOne-0.696/OneOnOne/sampling.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6959/OneOnOne/texttranslator.py` & `OneOnOne-0.696/OneOnOne/texttranslator.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6959/OneOnOne.egg-info/PKG-INFO` & `OneOnOne-0.696/OneOnOne.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.6959
+Version: 0.696
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,speech-recognition,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.6959/PKG-INFO` & `OneOnOne-0.696/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.6959
+Version: 0.696
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,speech-recognition,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.6959/README.md` & `OneOnOne-0.696/README.md`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6959/setup.py` & `OneOnOne-0.696/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION=0.6959
+VERSION=0.696
 
 DESCRIPTION="A package for pre-trained image classification and context-decider for question-answering chatbots."
 LONG_DESCRIPTION="Your one-stop destination to utilize image-classification models with just one line of code. A library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, no need to worry! This library has got you covered. Along with that for simple-bridging and basic into NLP, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset. This library is being actively updated and new features are being added frequently. New datasets and pre-trained models will be updated soon. Feel free to share your feedback! I would really appreciate it!"
 CLASSIFIERS=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Education',
     'License :: OSI Approved :: MIT License',
```

