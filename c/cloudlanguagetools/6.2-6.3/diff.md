# Comparing `tmp/cloudlanguagetools-6.2.tar.gz` & `tmp/cloudlanguagetools-6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudlanguagetools-6.2.tar", last modified: Sat Jul 22 00:24:48 2023, max compression
+gzip compressed data, was "cloudlanguagetools-6.3.tar", last modified: Sun Jul 30 06:46:14 2023, max compression
```

## Comparing `cloudlanguagetools-6.2.tar` & `cloudlanguagetools-6.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-07-22 00:24:48.979308 cloudlanguagetools-6.2/
--rw-r--r--   0 luc       (1000) luc       (1000)    35149 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/LICENSE
--rw-r--r--   0 luc       (1000) luc       (1000)      640 2023-07-22 00:24:48.979308 cloudlanguagetools-6.2/PKG-INFO
--rw-r--r--   0 luc       (1000) luc       (1000)      169 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/README.rst
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-07-22 00:24:48.979308 cloudlanguagetools-6.2/cloudlanguagetools/
--rw-r--r--   0 luc       (1000) luc       (1000)        0 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/__init__.py
--rw-r--r--   0 luc       (1000) luc       (1000)    13412 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/amazon.py
--rw-r--r--   0 luc       (1000) luc       (1000)     2667 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/argostranslate.py
--rw-r--r--   0 luc       (1000) luc       (1000)    23928 2023-07-14 14:25:16.000000 cloudlanguagetools-6.2/cloudlanguagetools/azure.py
--rw-r--r--   0 luc       (1000) luc       (1000)     4388 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/cereproc.py
--rw-r--r--   0 luc       (1000) luc       (1000)    17838 2023-07-22 00:24:24.000000 cloudlanguagetools-6.2/cloudlanguagetools/chatapi.py
--rw-r--r--   0 luc       (1000) luc       (1000)     2165 2023-07-14 14:25:16.000000 cloudlanguagetools-6.2/cloudlanguagetools/constants.py
--rw-r--r--   0 luc       (1000) luc       (1000)     4023 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/deepl.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1232 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/dictionarylookup.py
--rw-r--r--   0 luc       (1000) luc       (1000)     9171 2023-07-05 00:37:32.000000 cloudlanguagetools-6.2/cloudlanguagetools/easypronunciation.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6883 2023-07-14 14:25:16.000000 cloudlanguagetools-6.2/cloudlanguagetools/elevenlabs.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1052 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/encryption.py
--rw-r--r--   0 luc       (1000) luc       (1000)     7015 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/epitran.py
--rw-r--r--   0 luc       (1000) luc       (1000)      218 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/errors.py
--rw-r--r--   0 luc       (1000) luc       (1000)    13308 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/forvo.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6310 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/fptai.py
--rw-r--r--   0 luc       (1000) luc       (1000)     8801 2023-07-14 14:25:16.000000 cloudlanguagetools-6.2/cloudlanguagetools/google.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6355 2023-07-14 14:25:16.000000 cloudlanguagetools-6.2/cloudlanguagetools/keys.py
--rw-r--r--   0 luc       (1000) luc       (1000)    14056 2023-07-14 14:25:16.000000 cloudlanguagetools-6.2/cloudlanguagetools/languages.py
--rw-r--r--   0 luc       (1000) luc       (1000)     2806 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/libretranslate.py
--rw-r--r--   0 luc       (1000) luc       (1000)     3980 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/mandarincantonese.py
--rw-r--r--   0 luc       (1000) luc       (1000)    18680 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/naver.py
--rw-r--r--   0 luc       (1000) luc       (1000)     2511 2023-07-14 14:25:16.000000 cloudlanguagetools-6.2/cloudlanguagetools/openai.py
--rw-r--r--   0 luc       (1000) luc       (1000)      339 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/options.py
--rw-r--r--   0 luc       (1000) luc       (1000)     3310 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/pythainlp.py
--rw-r--r--   0 luc       (1000) luc       (1000)      432 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/service.py
--rw-r--r--   0 luc       (1000) luc       (1000)    18797 2023-07-14 14:25:16.000000 cloudlanguagetools-6.2/cloudlanguagetools/servicemanager.py
--rw-r--r--   0 luc       (1000) luc       (1000)     3006 2023-07-14 14:25:16.000000 cloudlanguagetools-6.2/cloudlanguagetools/spacy.py
--rw-r--r--   0 luc       (1000) luc       (1000)     5539 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/test_services.py
--rw-r--r--   0 luc       (1000) luc       (1000)      528 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/tokenization.py
--rw-r--r--   0 luc       (1000) luc       (1000)      515 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/translationlanguage.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1187 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/transliterationlanguage.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1239 2023-07-14 14:25:16.000000 cloudlanguagetools-6.2/cloudlanguagetools/ttsvoice.py
--rw-r--r--   0 luc       (1000) luc       (1000)    30649 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/vocalware.py
--rw-r--r--   0 luc       (1000) luc       (1000)     5479 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/voicen.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6491 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/watson.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6384 2023-05-24 03:51:37.000000 cloudlanguagetools-6.2/cloudlanguagetools/wenlin.py
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-07-22 00:24:48.979308 cloudlanguagetools-6.2/cloudlanguagetools.egg-info/
--rw-r--r--   0 luc       (1000) luc       (1000)      640 2023-07-22 00:24:48.000000 cloudlanguagetools-6.2/cloudlanguagetools.egg-info/PKG-INFO
--rw-r--r--   0 luc       (1000) luc       (1000)     1430 2023-07-22 00:24:48.000000 cloudlanguagetools-6.2/cloudlanguagetools.egg-info/SOURCES.txt
--rw-r--r--   0 luc       (1000) luc       (1000)        1 2023-07-22 00:24:48.000000 cloudlanguagetools-6.2/cloudlanguagetools.egg-info/dependency_links.txt
--rw-r--r--   0 luc       (1000) luc       (1000)       59 2023-07-22 00:24:48.000000 cloudlanguagetools-6.2/cloudlanguagetools.egg-info/requires.txt
--rw-r--r--   0 luc       (1000) luc       (1000)       19 2023-07-22 00:24:48.000000 cloudlanguagetools-6.2/cloudlanguagetools.egg-info/top_level.txt
--rw-r--r--   0 luc       (1000) luc       (1000)       38 2023-07-22 00:24:48.979308 cloudlanguagetools-6.2/setup.cfg
--rwxr-xr-x   0 luc       (1000) luc       (1000)      931 2023-07-22 00:24:45.000000 cloudlanguagetools-6.2/setup.py
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-07-30 06:46:14.936644 cloudlanguagetools-6.3/
+-rw-r--r--   0 luc       (1000) luc       (1000)    35149 2023-05-24 03:51:37.000000 cloudlanguagetools-6.3/LICENSE
+-rw-r--r--   0 luc       (1000) luc       (1000)      640 2023-07-30 06:46:14.936644 cloudlanguagetools-6.3/PKG-INFO
+-rw-r--r--   0 luc       (1000) luc       (1000)      169 2023-05-24 03:51:37.000000 cloudlanguagetools-6.3/README.rst
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-07-30 06:46:14.936644 cloudlanguagetools-6.3/cloudlanguagetools/
+-rw-r--r--   0 luc       (1000) luc       (1000)        0 2023-05-24 03:51:37.000000 cloudlanguagetools-6.3/cloudlanguagetools/__init__.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    13412 2023-05-24 03:51:37.000000 cloudlanguagetools-6.3/cloudlanguagetools/amazon.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     2667 2023-05-24 03:51:37.000000 cloudlanguagetools-6.3/cloudlanguagetools/argostranslate.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    23928 2023-07-14 14:25:16.000000 cloudlanguagetools-6.3/cloudlanguagetools/azure.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     4388 2023-05-24 03:51:37.000000 cloudlanguagetools-6.3/cloudlanguagetools/cereproc.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    17838 2023-07-22 00:24:24.000000 cloudlanguagetools-6.3/cloudlanguagetools/chatapi.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     2165 2023-07-14 14:25:16.000000 cloudlanguagetools-6.3/cloudlanguagetools/constants.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     4023 2023-05-24 03:51:37.000000 cloudlanguagetools-6.3/cloudlanguagetools/deepl.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     1232 2023-05-24 03:51:37.000000 cloudlanguagetools-6.3/cloudlanguagetools/dictionarylookup.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     9171 2023-07-05 00:37:32.000000 cloudlanguagetools-6.3/cloudlanguagetools/easypronunciation.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6621 2023-07-30 06:45:40.000000 cloudlanguagetools-6.3/cloudlanguagetools/elevenlabs.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     1052 2023-05-24 03:51:37.000000 cloudlanguagetools-6.3/cloudlanguagetools/encryption.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     7015 2023-05-24 03:51:37.000000 cloudlanguagetools-6.3/cloudlanguagetools/epitran.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      218 2023-05-24 03:51:37.000000 cloudlanguagetools-6.3/cloudlanguagetools/errors.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    13308 2023-05-24 03:51:37.000000 cloudlanguagetools-6.3/cloudlanguagetools/forvo.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6310 2023-05-24 03:51:37.000000 cloudlanguagetools-6.3/cloudlanguagetools/fptai.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     8801 2023-07-14 14:25:16.000000 cloudlanguagetools-6.3/cloudlanguagetools/google.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6355 2023-07-14 14:25:16.000000 cloudlanguagetools-6.3/cloudlanguagetools/keys.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    14056 2023-07-14 14:25:16.000000 cloudlanguagetools-6.3/cloudlanguagetools/languages.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     2806 2023-05-24 03:51:37.000000 cloudlanguagetools-6.3/cloudlanguagetools/libretranslate.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     3980 2023-05-24 03:51:37.000000 cloudlanguagetools-6.3/cloudlanguagetools/mandarincantonese.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    18680 2023-05-24 03:51:37.000000 cloudlanguagetools-6.3/cloudlanguagetools/naver.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     2511 2023-07-14 14:25:16.000000 cloudlanguagetools-6.3/cloudlanguagetools/openai.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      339 2023-05-24 03:51:37.000000 cloudlanguagetools-6.3/cloudlanguagetools/options.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     3310 2023-05-24 03:51:37.000000 cloudlanguagetools-6.3/cloudlanguagetools/pythainlp.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      432 2023-05-24 03:51:37.000000 cloudlanguagetools-6.3/cloudlanguagetools/service.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    18797 2023-07-14 14:25:16.000000 cloudlanguagetools-6.3/cloudlanguagetools/servicemanager.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     3006 2023-07-14 14:25:16.000000 cloudlanguagetools-6.3/cloudlanguagetools/spacy.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     5539 2023-05-24 03:51:37.000000 cloudlanguagetools-6.3/cloudlanguagetools/test_services.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      528 2023-05-24 03:51:37.000000 cloudlanguagetools-6.3/cloudlanguagetools/tokenization.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      515 2023-05-24 03:51:37.000000 cloudlanguagetools-6.3/cloudlanguagetools/translationlanguage.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     1187 2023-05-24 03:51:37.000000 cloudlanguagetools-6.3/cloudlanguagetools/transliterationlanguage.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     1239 2023-07-14 14:25:16.000000 cloudlanguagetools-6.3/cloudlanguagetools/ttsvoice.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    30649 2023-05-24 03:51:37.000000 cloudlanguagetools-6.3/cloudlanguagetools/vocalware.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     5479 2023-05-24 03:51:37.000000 cloudlanguagetools-6.3/cloudlanguagetools/voicen.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6491 2023-05-24 03:51:37.000000 cloudlanguagetools-6.3/cloudlanguagetools/watson.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6384 2023-05-24 03:51:37.000000 cloudlanguagetools-6.3/cloudlanguagetools/wenlin.py
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-07-30 06:46:14.936644 cloudlanguagetools-6.3/cloudlanguagetools.egg-info/
+-rw-r--r--   0 luc       (1000) luc       (1000)      640 2023-07-30 06:46:14.000000 cloudlanguagetools-6.3/cloudlanguagetools.egg-info/PKG-INFO
+-rw-r--r--   0 luc       (1000) luc       (1000)     1430 2023-07-30 06:46:14.000000 cloudlanguagetools-6.3/cloudlanguagetools.egg-info/SOURCES.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)        1 2023-07-30 06:46:14.000000 cloudlanguagetools-6.3/cloudlanguagetools.egg-info/dependency_links.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)       59 2023-07-30 06:46:14.000000 cloudlanguagetools-6.3/cloudlanguagetools.egg-info/requires.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)       19 2023-07-30 06:46:14.000000 cloudlanguagetools-6.3/cloudlanguagetools.egg-info/top_level.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)       38 2023-07-30 06:46:14.936644 cloudlanguagetools-6.3/setup.cfg
+-rwxr-xr-x   0 luc       (1000) luc       (1000)      931 2023-07-30 06:46:12.000000 cloudlanguagetools-6.3/setup.py
```

### Comparing `cloudlanguagetools-6.2/LICENSE` & `cloudlanguagetools-6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.2/PKG-INFO` & `cloudlanguagetools-6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudlanguagetools
-Version: 6.2
+Version: 6.3
 Summary: Interface with various cloud APIs for language processing such as translation, text to speech
 Home-page: https://github.com/Language-Tools/cloud-language-tools-core
 Author: Luc
 Author-email: languagetools@mailc.net
 License: GPL
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools/amazon.py` & `cloudlanguagetools-6.3/cloudlanguagetools/amazon.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools/argostranslate.py` & `cloudlanguagetools-6.3/cloudlanguagetools/argostranslate.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools/azure.py` & `cloudlanguagetools-6.3/cloudlanguagetools/azure.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools/cereproc.py` & `cloudlanguagetools-6.3/cloudlanguagetools/cereproc.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools/chatapi.py` & `cloudlanguagetools-6.3/cloudlanguagetools/chatapi.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools/constants.py` & `cloudlanguagetools-6.3/cloudlanguagetools/constants.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools/deepl.py` & `cloudlanguagetools-6.3/cloudlanguagetools/deepl.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools/dictionarylookup.py` & `cloudlanguagetools-6.3/cloudlanguagetools/dictionarylookup.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools/easypronunciation.py` & `cloudlanguagetools-6.3/cloudlanguagetools/easypronunciation.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools/elevenlabs.py` & `cloudlanguagetools-6.3/cloudlanguagetools/elevenlabs.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,38 +15,29 @@
 import cloudlanguagetools.transliterationlanguage
 import cloudlanguagetools.errors
 
 
 DEFAULT_STABILITY = 0.75
 DEFAULT_SIMILARITY_BOOST = 0.75
 
-
 GENDER_MAP = {
-    'Rachel': cloudlanguagetools.constants.Gender.Female,
-    'Domi': cloudlanguagetools.constants.Gender.Female,
-    'Bella': cloudlanguagetools.constants.Gender.Female,
-    'Antoni': cloudlanguagetools.constants.Gender.Male,
-    'Elli': cloudlanguagetools.constants.Gender.Female,
-    'Josh': cloudlanguagetools.constants.Gender.Male,
-    'Arnold': cloudlanguagetools.constants.Gender.Male,
-    'Adam': cloudlanguagetools.constants.Gender.Male,
-    'Sam': cloudlanguagetools.constants.Gender.Male
+    'male': cloudlanguagetools.constants.Gender.Male,
+    'female': cloudlanguagetools.constants.Gender.Female,
 }
 
-
 class ElevenLabsVoice(cloudlanguagetools.ttsvoice.TtsVoice):
     def __init__(self, voice_data, language, model_id, model_short_name):
         # pprint.pprint(voice_data)
         self.service = cloudlanguagetools.constants.Service.ElevenLabs
         self.service_fee = cloudlanguagetools.constants.ServiceFee.paid
         self.voice_id = voice_data['voice_id']
         self.model_id = model_id
         self.model_short_name = model_short_name
         self.name = voice_data['name']
-        self.gender = GENDER_MAP.get(self.name, cloudlanguagetools.constants.Gender.Male)
+        self.gender = GENDER_MAP.get(voice_data['labels']['gender'], cloudlanguagetools.constants.Gender.Male)
         self.audio_language = language
 
     def get_voice_key(self):
         return {
             'voice_id': self.voice_id,
             'model_id': self.model_id
         }
@@ -99,15 +90,15 @@
             "model_id": voice_key['model_id'],
             "voice_settings": {
                 "stability": options.get('stability', DEFAULT_STABILITY),
                 "similarity_boost": options.get('similarity_boost', DEFAULT_SIMILARITY_BOOST)
             }
         }
 
-        response = requests.post(url, json=data, headers=headers)
+        response = requests.post(url, json=data, headers=headers, timeout=cloudlanguagetools.constants.RequestTimeout)
         response.raise_for_status()
         
         output_temp_file = tempfile.NamedTemporaryFile()
         output_temp_filename = output_temp_file.name
 
         with open(output_temp_filename, 'wb') as f:
             for chunk in response.iter_content(chunk_size=CHUNK_SIZE):
@@ -164,15 +155,15 @@
         #         
 
 
         # now, retrieve voice list
         # call elevenlabs API to list TTS voices
         url = "https://api.elevenlabs.io/v1/voices"
 
-        response = requests.get(url, headers=self.get_headers())
+        response = requests.get(url, headers=self.get_headers(), timeout=cloudlanguagetools.constants.RequestTimeout)
         response.raise_for_status()
 
         data = response.json()
 
         for model in model_data:
             model_id = model['model_id']
             model_name = model['name']
```

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools/encryption.py` & `cloudlanguagetools-6.3/cloudlanguagetools/encryption.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools/epitran.py` & `cloudlanguagetools-6.3/cloudlanguagetools/epitran.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools/forvo.py` & `cloudlanguagetools-6.3/cloudlanguagetools/forvo.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools/fptai.py` & `cloudlanguagetools-6.3/cloudlanguagetools/fptai.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools/google.py` & `cloudlanguagetools-6.3/cloudlanguagetools/google.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools/keys.py` & `cloudlanguagetools-6.3/cloudlanguagetools/keys.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools/languages.py` & `cloudlanguagetools-6.3/cloudlanguagetools/languages.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools/libretranslate.py` & `cloudlanguagetools-6.3/cloudlanguagetools/libretranslate.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools/mandarincantonese.py` & `cloudlanguagetools-6.3/cloudlanguagetools/mandarincantonese.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools/naver.py` & `cloudlanguagetools-6.3/cloudlanguagetools/naver.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools/openai.py` & `cloudlanguagetools-6.3/cloudlanguagetools/openai.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools/pythainlp.py` & `cloudlanguagetools-6.3/cloudlanguagetools/pythainlp.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools/servicemanager.py` & `cloudlanguagetools-6.3/cloudlanguagetools/servicemanager.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools/spacy.py` & `cloudlanguagetools-6.3/cloudlanguagetools/spacy.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools/test_services.py` & `cloudlanguagetools-6.3/cloudlanguagetools/test_services.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools/tokenization.py` & `cloudlanguagetools-6.3/cloudlanguagetools/tokenization.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools/translationlanguage.py` & `cloudlanguagetools-6.3/cloudlanguagetools/translationlanguage.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools/transliterationlanguage.py` & `cloudlanguagetools-6.3/cloudlanguagetools/transliterationlanguage.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools/ttsvoice.py` & `cloudlanguagetools-6.3/cloudlanguagetools/ttsvoice.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools/vocalware.py` & `cloudlanguagetools-6.3/cloudlanguagetools/vocalware.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools/voicen.py` & `cloudlanguagetools-6.3/cloudlanguagetools/voicen.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools/watson.py` & `cloudlanguagetools-6.3/cloudlanguagetools/watson.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools/wenlin.py` & `cloudlanguagetools-6.3/cloudlanguagetools/wenlin.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools.egg-info/PKG-INFO` & `cloudlanguagetools-6.3/cloudlanguagetools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudlanguagetools
-Version: 6.2
+Version: 6.3
 Summary: Interface with various cloud APIs for language processing such as translation, text to speech
 Home-page: https://github.com/Language-Tools/cloud-language-tools-core
 Author: Luc
 Author-email: languagetools@mailc.net
 License: GPL
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cloudlanguagetools-6.2/cloudlanguagetools.egg-info/SOURCES.txt` & `cloudlanguagetools-6.3/cloudlanguagetools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-6.2/setup.py` & `cloudlanguagetools-6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools.command.install import install
 
 # build instructions
 # python setup.py sdist
 # twine upload dist/*
 
 setup(name='cloudlanguagetools',
-      version='6.2',
+      version='6.3',
       description='Interface with various cloud APIs for language processing such as translation, text to speech',
       long_description=open('README.rst', encoding='utf-8').read(),
       url='https://github.com/Language-Tools/cloud-language-tools-core',
       author='Luc',
       author_email='languagetools@mailc.net',
       classifiers=[
         'Programming Language :: Python :: 3.7',
```

