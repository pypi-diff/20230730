# Comparing `tmp/OneOnOne-0.704.tar.gz` & `tmp/OneOnOne-0.705.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OneOnOne-0.704.tar", last modified: Sun Jul 30 09:29:22 2023, max compression
+gzip compressed data, was "OneOnOne-0.705.tar", last modified: Sun Jul 30 09:46:07 2023, max compression
```

## Comparing `OneOnOne-0.704.tar` & `OneOnOne-0.705.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-30 09:29:22.544707 OneOnOne-0.704/
--rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.704/LICENSE
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-30 09:29:22.541402 OneOnOne-0.704/OneOnOne/
--rw-r--r--   0 sohinib    (501) staff       (20)    71817 2023-07-30 09:29:17.000000 OneOnOne-0.704/OneOnOne/__init__.py
--rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.704/OneOnOne/classes.py
--rw-r--r--   0 sohinib    (501) staff       (20)    14251 2023-07-28 06:59:10.000000 OneOnOne-0.704/OneOnOne/classification.py
--rw-r--r--   0 sohinib    (501) staff       (20)     7164 2023-07-29 12:25:37.000000 OneOnOne-0.704/OneOnOne/clustering.py
--rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.704/OneOnOne/contextdecider.py
--rw-r--r--   0 sohinib    (501) staff       (20)     3403 2023-07-29 18:08:15.000000 OneOnOne-0.704/OneOnOne/conversation.py
--rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.704/OneOnOne/htmlparser.py
--rw-r--r--   0 sohinib    (501) staff       (20)     2190 2023-07-30 08:22:15.000000 OneOnOne-0.704/OneOnOne/imagetranslator.py
--rw-r--r--   0 sohinib    (501) staff       (20)      995 2023-07-29 18:59:58.000000 OneOnOne-0.704/OneOnOne/pdftotext.py
--rw-r--r--   0 sohinib    (501) staff       (20)     1880 2023-07-28 06:59:09.000000 OneOnOne-0.704/OneOnOne/pretrainedmodel.py
--rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.704/OneOnOne/questionanswer.py
--rw-r--r--   0 sohinib    (501) staff       (20)    23928 2023-07-28 06:59:10.000000 OneOnOne-0.704/OneOnOne/sampling.py
--rw-r--r--   0 sohinib    (501) staff       (20)      888 2023-07-29 17:53:14.000000 OneOnOne-0.704/OneOnOne/texttranslator.py
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-30 09:29:22.543877 OneOnOne-0.704/OneOnOne.egg-info/
--rw-r--r--   0 sohinib    (501) staff       (20)     1596 2023-07-30 09:29:22.000000 OneOnOne-0.704/OneOnOne.egg-info/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)      504 2023-07-30 09:29:22.000000 OneOnOne-0.704/OneOnOne.egg-info/SOURCES.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-30 09:29:22.000000 OneOnOne-0.704/OneOnOne.egg-info/dependency_links.txt
--rw-r--r--   0 sohinib    (501) staff       (20)      233 2023-07-30 09:29:22.000000 OneOnOne-0.704/OneOnOne.egg-info/requires.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-30 09:29:22.000000 OneOnOne-0.704/OneOnOne.egg-info/top_level.txt
--rw-r--r--   0 sohinib    (501) staff       (20)     1596 2023-07-30 09:29:22.544296 OneOnOne-0.704/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)     3701 2023-07-29 19:02:55.000000 OneOnOne-0.704/README.md
--rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-30 09:29:22.544891 OneOnOne-0.704/setup.cfg
--rw-r--r--   0 sohinib    (501) staff       (20)     2069 2023-07-30 09:29:17.000000 OneOnOne-0.704/setup.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-30 09:46:07.865174 OneOnOne-0.705/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.705/LICENSE
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-30 09:46:07.861504 OneOnOne-0.705/OneOnOne/
+-rw-r--r--   0 sohinib    (501) staff       (20)    72995 2023-07-30 09:45:59.000000 OneOnOne-0.705/OneOnOne/__init__.py
+-rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.705/OneOnOne/classes.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    14251 2023-07-28 06:59:10.000000 OneOnOne-0.705/OneOnOne/classification.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     7164 2023-07-29 12:25:37.000000 OneOnOne-0.705/OneOnOne/clustering.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.705/OneOnOne/contextdecider.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     3403 2023-07-29 18:08:15.000000 OneOnOne-0.705/OneOnOne/conversation.py
+-rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.705/OneOnOne/htmlparser.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     2190 2023-07-30 08:22:15.000000 OneOnOne-0.705/OneOnOne/imagetranslator.py
+-rw-r--r--   0 sohinib    (501) staff       (20)      995 2023-07-29 18:59:58.000000 OneOnOne-0.705/OneOnOne/pdftotext.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     1880 2023-07-28 06:59:09.000000 OneOnOne-0.705/OneOnOne/pretrainedmodel.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.705/OneOnOne/questionanswer.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    23928 2023-07-28 06:59:10.000000 OneOnOne-0.705/OneOnOne/sampling.py
+-rw-r--r--   0 sohinib    (501) staff       (20)      888 2023-07-29 17:53:14.000000 OneOnOne-0.705/OneOnOne/texttranslator.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-30 09:46:07.864403 OneOnOne-0.705/OneOnOne.egg-info/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1596 2023-07-30 09:46:07.000000 OneOnOne-0.705/OneOnOne.egg-info/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)      504 2023-07-30 09:46:07.000000 OneOnOne-0.705/OneOnOne.egg-info/SOURCES.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-30 09:46:07.000000 OneOnOne-0.705/OneOnOne.egg-info/dependency_links.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)      233 2023-07-30 09:46:07.000000 OneOnOne-0.705/OneOnOne.egg-info/requires.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-30 09:46:07.000000 OneOnOne-0.705/OneOnOne.egg-info/top_level.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)     1596 2023-07-30 09:46:07.864822 OneOnOne-0.705/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)     3701 2023-07-29 19:02:55.000000 OneOnOne-0.705/README.md
+-rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-30 09:46:07.865293 OneOnOne-0.705/setup.cfg
+-rw-r--r--   0 sohinib    (501) staff       (20)     2069 2023-07-30 09:46:02.000000 OneOnOne-0.705/setup.py
```

### Comparing `OneOnOne-0.704/LICENSE` & `OneOnOne-0.705/LICENSE`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.704/OneOnOne/__init__.py` & `OneOnOne-0.705/OneOnOne/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1137,14 +1137,15 @@
 
             img = img.reshape(1, 32, 32, 3)
             # img = iio.imread(os.getcwd()+f"{path}")
             self.pred = self.contextmodel.predict_generator(img)
         else:
             # random.randint(1, 3000)
             # np.ceil(self.number_of_val_samples / self.batch_size)
+            # , steps = self.batch_size
             self.pred = self.contextmodel.predict_generator(self.val_it, steps = self.batch_size)
 
     def get_datagen(self):
 
         datagen = ImageDataGenerator(
             featurewise_center=False,
             samplewise_center=False,
@@ -1165,25 +1166,45 @@
             rescale=None,
             preprocessing_function=None,
             data_format=None,
             validation_split=self.validation_split)
 
         return datagen
 
+    def preprocess_image_input(self, input_images):
+        if self.model_type == "efficientnetb6":
+            input_images = input_images.astype('float32')
+            output_ims = tf.keras.applications.efficientnet.preprocess_input(input_images)
+        elif self.model_type == "resnet50":
+            input_images = input_images.astype('float32')
+            output_ims = tf.keras.applications.resnet50.preprocess_input(input_images)
+        elif self.model_type == "densenet":
+            input_images = input_images.astype('float32')
+            output_ims = tf.keras.applications.densenet.preprocess_input(input_images)
+        elif self.model_type == "vgg19":
+            input_images = input_images.astype('float32')
+            output_ims = tf.keras.applications.vgg19.preprocess_input(input_images)
+        else:
+            input_images = input_images.astype('float32')
+            output_ims = tf.keras.applications.resnet50.preprocess_input(input_images)
+
+        return output_ims
+
+
     def decide_context(self):
 
         from classes import i2d
 
         predicted_list = []
         prediction_index = []
         final_classes = []
 
         output = []
 
-        labels = self.train_it.class_indices
+        labels = self.combined_it.class_indices
         labels2 = dict((v, k) for k, v in labels.items())
 
         for i in range(0, self.pred.shape[0]):
             classes_prob_list = []
             for j in range(0, self.output_layer_classes):
                 classes_prob_list.append([int(j), self.pred[i][j]])
 
@@ -1237,14 +1258,17 @@
         if self.dataset == "tinyimagenet":
             train_it = self.datagen.flow_from_directory(os.getcwd() + '/tiny-imagenet-200/train',
                                                         batch_size=self.batch_size, subset="training",
                                                         shuffle=self.shuffle_bool,seed=random.randint(1,100))
             val_it = self.datagen.flow_from_directory(os.getcwd() + '/tiny-imagenet-200/train',
                                                       batch_size=self.batch_size,
                                                       subset="validation", shuffle=self.shuffle_bool,seed=random.randint(1,100))
+
+            self.combined_it = self.datagen.flow_from_directory(os.getcwd() + '/tiny-imagenet-200/train', batch_size=self.batch_size,)
+
             train_filenames = train_it.filenames
             val_filenames = val_it.filenames
             self.number_of_val_samples = len(val_filenames)
             number_of_train_samples = len(train_filenames)
             # class_mode='categorical',
             # print(number_of_train_samples)
             # print(number_of_val_samples)
```

### Comparing `OneOnOne-0.704/OneOnOne/classes.py` & `OneOnOne-0.705/OneOnOne/classes.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.704/OneOnOne/classification.py` & `OneOnOne-0.705/OneOnOne/classification.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.704/OneOnOne/clustering.py` & `OneOnOne-0.705/OneOnOne/clustering.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.704/OneOnOne/contextdecider.py` & `OneOnOne-0.705/OneOnOne/contextdecider.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.704/OneOnOne/conversation.py` & `OneOnOne-0.705/OneOnOne/conversation.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.704/OneOnOne/htmlparser.py` & `OneOnOne-0.705/OneOnOne/htmlparser.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.704/OneOnOne/imagetranslator.py` & `OneOnOne-0.705/OneOnOne/imagetranslator.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.704/OneOnOne/pdftotext.py` & `OneOnOne-0.705/OneOnOne/pdftotext.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.704/OneOnOne/pretrainedmodel.py` & `OneOnOne-0.705/OneOnOne/pretrainedmodel.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.704/OneOnOne/questionanswer.py` & `OneOnOne-0.705/OneOnOne/questionanswer.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.704/OneOnOne/sampling.py` & `OneOnOne-0.705/OneOnOne/sampling.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.704/OneOnOne/texttranslator.py` & `OneOnOne-0.705/OneOnOne/texttranslator.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.704/OneOnOne.egg-info/PKG-INFO` & `OneOnOne-0.705/OneOnOne.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.704
+Version: 0.705
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,speech-recognition,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.704/PKG-INFO` & `OneOnOne-0.705/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.704
+Version: 0.705
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,speech-recognition,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.704/README.md` & `OneOnOne-0.705/README.md`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.704/setup.py` & `OneOnOne-0.705/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION=0.704
+VERSION=0.705
 
 DESCRIPTION="A package for pre-trained image classification and context-decider for question-answering chatbots."
 LONG_DESCRIPTION="Your one-stop destination to utilize image-classification models with just one line of code. A library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, no need to worry! This library has got you covered. Along with that for simple-bridging and basic into NLP, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset. This library is being actively updated and new features are being added frequently. New datasets and pre-trained models will be updated soon. Feel free to share your feedback! I would really appreciate it!"
 CLASSIFIERS=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Education',
     'License :: OSI Approved :: MIT License',
```

