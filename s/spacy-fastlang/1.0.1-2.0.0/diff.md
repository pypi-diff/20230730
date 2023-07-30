# Comparing `tmp/spacy_fastlang-1.0.1.tar.gz` & `tmp/spacy_fastlang-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy_fastlang-1.0.1.tar", max compression
+gzip compressed data, was "spacy_fastlang-2.0.0.tar", max compression
```

## Comparing `spacy_fastlang-1.0.1.tar` & `spacy_fastlang-2.0.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1072 2022-01-11 17:16:28.808563 spacy_fastlang-1.0.1/LICENSE
--rw-r--r--   0        0        0      912 2022-01-11 17:16:28.808563 spacy_fastlang-1.0.1/README.md
--rw-r--r--   0        0        0     1173 2022-01-11 17:16:28.808563 spacy_fastlang-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2687 2022-01-11 17:16:28.808563 spacy_fastlang-1.0.1/spacy_fastlang/__init__.py
--rw-r--r--   0        0        0   938013 2022-01-11 17:16:28.816563 spacy_fastlang-1.0.1/spacy_fastlang/lid.176.ftz
--rw-r--r--   0        0        0     1664 2022-01-11 17:18:10.279565 spacy_fastlang-1.0.1/setup.py
--rw-r--r--   0        0        0     2122 2022-01-11 17:18:10.280011 spacy_fastlang-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-30 19:00:25.872631 spacy_fastlang-2.0.0/LICENSE
+-rw-r--r--   0        0        0      958 2023-07-30 19:00:25.872631 spacy_fastlang-2.0.0/README.md
+-rw-r--r--   0        0        0     1184 2023-07-30 19:00:25.872631 spacy_fastlang-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2687 2023-07-30 19:00:25.872631 spacy_fastlang-2.0.0/spacy_fastlang/__init__.py
+-rw-r--r--   0        0        0   938013 2023-07-30 19:00:25.880631 spacy_fastlang-2.0.0/spacy_fastlang/lid.176.ftz
+-rw-r--r--   0        0        0     2125 1970-01-01 00:00:00.000000 spacy_fastlang-2.0.0/PKG-INFO
```

### Comparing `spacy_fastlang-1.0.1/LICENSE` & `spacy_fastlang-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy_fastlang-1.0.1/README.md` & `spacy_fastlang-2.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 The library exports a pipeline component called `language_detector` that will set two spacy extensions
 
 - doc.\_.language = ISO code of the detected language or `xx` as a fallback
 - doc.\_.language_score = confidence
 
 ```
-import spacy_fastlang
+import spacy_fastlang  # noqa: F401 # pylint: disable=unused-import
 nlp = spacy.load("...")
 nlp.add_pipe("language_detector")
 doc = nlp(en_text)
 
 doc._.language == "..."
 doc._.language_score >= ...
 ```
```

### Comparing `spacy_fastlang-1.0.1/pyproject.toml` & `spacy_fastlang-2.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [tool.poetry]
 name = "spacy_fastlang"
-version = "1.0.1"
+version = "2.0.0"
 description = "Language detection using FastText and Spacy"
 authors = ["Thomas Thiebaud <thiebaud.tom@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/thomasthiebaud/spacy-fastlang"
 repository = "https://github.com/thomasthiebaud/spacy-fastlang"
 documentation = "https://github.com/thomasthiebaud/spacy-fastlang"
 keywords = ["spacy", "fasttext", "language", "detection"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6"
-spacy = "^3.0.6"
-fasttext = "^0.9.2"
+python = "^3.8"
+spacy = "^3.6.0"
+fasttext-wheel = "^0.9.2"
 
 [tool.poetry.dev-dependencies]
-black = "^19.10b0"
-pytest = "^5.4.1"
+black = "^23.7.0"
+pytest = "^7.4.0"
 
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `spacy_fastlang-1.0.1/spacy_fastlang/__init__.py` & `spacy_fastlang-2.0.0/spacy_fastlang/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy_fastlang-1.0.1/spacy_fastlang/lid.176.ftz` & `spacy_fastlang-2.0.0/spacy_fastlang/lid.176.ftz`

 * *Files identical despite different names*

### Comparing `spacy_fastlang-1.0.1/PKG-INFO` & `spacy_fastlang-2.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: spacy-fastlang
-Version: 1.0.1
+Version: 2.0.0
 Summary: Language detection using FastText and Spacy
 Home-page: https://github.com/thomasthiebaud/spacy-fastlang
 License: MIT
 Keywords: spacy,fasttext,language,detection
 Author: Thomas Thiebaud
 Author-email: thiebaud.tom@gmail.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
-Requires-Dist: fasttext (>=0.9.2,<0.10.0)
-Requires-Dist: spacy (>=3.0.6,<4.0.0)
+Requires-Dist: fasttext-wheel (>=0.9.2,<0.10.0)
+Requires-Dist: spacy (>=3.6.0,<4.0.0)
 Project-URL: Documentation, https://github.com/thomasthiebaud/spacy-fastlang
 Project-URL: Repository, https://github.com/thomasthiebaud/spacy-fastlang
 Description-Content-Type: text/markdown
 
 # spacy_fastlang
 
 ## Install
@@ -41,15 +40,15 @@
 
 The library exports a pipeline component called `language_detector` that will set two spacy extensions
 
 - doc.\_.language = ISO code of the detected language or `xx` as a fallback
 - doc.\_.language_score = confidence
 
 ```
-import spacy_fastlang
+import spacy_fastlang  # noqa: F401 # pylint: disable=unused-import
 nlp = spacy.load("...")
 nlp.add_pipe("language_detector")
 doc = nlp(en_text)
 
 doc._.language == "..."
 doc._.language_score >= ...
 ```
```

