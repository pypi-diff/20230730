# Comparing `tmp/distool-0.1.9.tar.gz` & `tmp/distool-0.1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "distool-0.1.9.tar", last modified: Sun Jul 30 14:26:21 2023, max compression
+gzip compressed data, was "distool-0.1.9.1.tar", last modified: Sun Jul 30 14:30:01 2023, max compression
```

## Comparing `distool-0.1.9.tar` & `distool-0.1.9.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:26:21.745195 distool-0.1.9/
--rw-r--r--   0 michilegorov   (501) staff       (20)     1068 2023-07-16 22:12:30.000000 distool-0.1.9/LICENSE.txt
--rw-r--r--   0 michilegorov   (501) staff       (20)     5973 2023-07-30 14:26:21.745404 distool-0.1.9/PKG-INFO
--rw-r--r--   0 michilegorov   (501) staff       (20)     5129 2023-07-16 22:12:30.000000 distool-0.1.9/README.md
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:26:21.724411 distool-0.1.9/distool/
--rw-r--r--   0 michilegorov   (501) staff       (20)      836 2023-07-16 22:12:30.000000 distool-0.1.9/distool/__init__.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:26:21.727619 distool-0.1.9/distool/base/
--rw-r--r--   0 michilegorov   (501) staff       (20)      248 2023-07-16 22:12:30.000000 distool-0.1.9/distool/base/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     2511 2023-07-16 22:12:30.000000 distool-0.1.9/distool/base/estimators.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:26:21.728101 distool-0.1.9/distool/data/
--rw-r--r--   0 michilegorov   (501) staff       (20)   240820 2023-07-16 22:12:30.000000 distool-0.1.9/distool/data/symptoms.json
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:26:21.730334 distool-0.1.9/distool/estimators/
--rw-r--r--   0 michilegorov   (501) staff       (20)      441 2023-07-16 22:12:30.000000 distool-0.1.9/distool/estimators/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     4943 2023-07-16 22:12:30.000000 distool-0.1.9/distool/estimators/classifiers.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:26:21.733921 distool-0.1.9/distool/feature_extraction/
--rw-r--r--   0 michilegorov   (501) staff       (20)      586 2023-07-16 22:12:30.000000 distool-0.1.9/distool/feature_extraction/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     3880 2023-07-16 22:12:30.000000 distool-0.1.9/distool/feature_extraction/anamnesis.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     2000 2023-07-16 22:12:30.000000 distool-0.1.9/distool/feature_extraction/dumb_extractor.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     6538 2023-07-16 22:12:30.000000 distool-0.1.9/distool/feature_extraction/smart_extractor.py
--rw-r--r--   0 michilegorov   (501) staff       (20)      917 2023-07-16 22:12:30.000000 distool-0.1.9/distool/feature_extraction/symptom.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     3525 2023-07-16 22:12:30.000000 distool-0.1.9/distool/feature_extraction/symptom_collection.py
--rw-r--r--   0 michilegorov   (501) staff       (20)      547 2023-07-16 22:12:30.000000 distool-0.1.9/distool/feature_extraction/symptom_status.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:26:21.735244 distool-0.1.9/distool/interpretation/
--rw-r--r--   0 michilegorov   (501) staff       (20)      279 2023-07-16 22:12:30.000000 distool-0.1.9/distool/interpretation/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     3442 2023-07-16 22:12:30.000000 distool-0.1.9/distool/interpretation/explainer.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:26:21.735795 distool-0.1.9/distool/metrics/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 distool-0.1.9/distool/metrics/__init__.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:26:21.737060 distool-0.1.9/distool/metrics/extractor/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 distool-0.1.9/distool/metrics/extractor/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     2475 2023-07-16 22:12:30.000000 distool-0.1.9/distool/metrics/extractor/compute.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     7709 2023-07-16 22:12:30.000000 distool-0.1.9/distool/metrics/extractor/create_showcase.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:26:21.738088 distool-0.1.9/distool/models/
--rw-r--r--   0 michilegorov   (501) staff       (20)      152 2023-07-16 22:12:30.000000 distool-0.1.9/distool/models/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     3360 2023-07-16 22:12:30.000000 distool-0.1.9/distool/models/urgency_classifier.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:26:21.739872 distool-0.1.9/distool/tests/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 distool-0.1.9/distool/tests/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)      959 2023-07-16 22:12:30.000000 distool-0.1.9/distool/tests/conftest.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:26:21.741738 distool-0.1.9/distool/tests/estimators/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 distool-0.1.9/distool/tests/estimators/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)      419 2023-07-16 22:12:30.000000 distool-0.1.9/distool/tests/estimators/test_classifier.py
--rw-r--r--   0 michilegorov   (501) staff       (20)      787 2023-07-16 22:12:30.000000 distool-0.1.9/distool/tests/estimators/test_fedot_classifier.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:26:21.742740 distool-0.1.9/distool/tests/explainer/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 distool-0.1.9/distool/tests/explainer/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     1346 2023-07-16 22:12:30.000000 distool-0.1.9/distool/tests/explainer/test_explainer.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:26:21.743592 distool-0.1.9/distool/tests/extractors/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 distool-0.1.9/distool/tests/extractors/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     1630 2023-07-16 22:12:30.000000 distool-0.1.9/distool/tests/extractors/test_symptom_extractor.py
--rw-r--r--   0 michilegorov   (501) staff       (20)       37 2023-07-16 22:12:30.000000 distool-0.1.9/distool/tests/test_base.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:26:21.726630 distool-0.1.9/distool.egg-info/
--rw-r--r--   0 michilegorov   (501) staff       (20)     5973 2023-07-30 14:26:21.000000 distool-0.1.9/distool.egg-info/PKG-INFO
--rw-r--r--   0 michilegorov   (501) staff       (20)     1384 2023-07-30 14:26:21.000000 distool-0.1.9/distool.egg-info/SOURCES.txt
--rw-r--r--   0 michilegorov   (501) staff       (20)        1 2023-07-30 14:26:21.000000 distool-0.1.9/distool.egg-info/dependency_links.txt
--rw-r--r--   0 michilegorov   (501) staff       (20)       64 2023-07-30 14:26:21.000000 distool-0.1.9/distool.egg-info/requires.txt
--rw-r--r--   0 michilegorov   (501) staff       (20)       17 2023-07-30 14:26:21.000000 distool-0.1.9/distool.egg-info/top_level.txt
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:26:21.744515 distool-0.1.9/examples/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-02-04 10:03:31.000000 distool-0.1.9/examples/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     1116 2023-07-16 22:12:30.000000 distool-0.1.9/examples/pipeline_example.py
--rw-r--r--   0 michilegorov   (501) staff       (20)      253 2023-07-30 14:26:16.000000 distool-0.1.9/pyproject.toml
--rw-r--r--   0 michilegorov   (501) staff       (20)       79 2023-07-30 14:26:21.746189 distool-0.1.9/setup.cfg
--rw-r--r--   0 michilegorov   (501) staff       (20)     1332 2023-07-30 14:23:43.000000 distool-0.1.9/setup.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:30:01.248784 distool-0.1.9.1/
+-rw-r--r--   0 michilegorov   (501) staff       (20)     1068 2023-07-16 22:12:30.000000 distool-0.1.9.1/LICENSE.txt
+-rw-r--r--   0 michilegorov   (501) staff       (20)     5975 2023-07-30 14:30:01.248965 distool-0.1.9.1/PKG-INFO
+-rw-r--r--   0 michilegorov   (501) staff       (20)     5129 2023-07-16 22:12:30.000000 distool-0.1.9.1/README.md
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:30:01.226158 distool-0.1.9.1/distool/
+-rw-r--r--   0 michilegorov   (501) staff       (20)      836 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/__init__.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:30:01.229639 distool-0.1.9.1/distool/base/
+-rw-r--r--   0 michilegorov   (501) staff       (20)      248 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/base/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     2511 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/base/estimators.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:30:01.230414 distool-0.1.9.1/distool/data/
+-rw-r--r--   0 michilegorov   (501) staff       (20)   240820 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/data/symptoms.json
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:30:01.232741 distool-0.1.9.1/distool/estimators/
+-rw-r--r--   0 michilegorov   (501) staff       (20)      441 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/estimators/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     4943 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/estimators/classifiers.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:30:01.236264 distool-0.1.9.1/distool/feature_extraction/
+-rw-r--r--   0 michilegorov   (501) staff       (20)      586 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/feature_extraction/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     3880 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/feature_extraction/anamnesis.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     2000 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/feature_extraction/dumb_extractor.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     6538 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/feature_extraction/smart_extractor.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)      917 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/feature_extraction/symptom.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     3525 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/feature_extraction/symptom_collection.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)      547 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/feature_extraction/symptom_status.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:30:01.237249 distool-0.1.9.1/distool/interpretation/
+-rw-r--r--   0 michilegorov   (501) staff       (20)      279 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/interpretation/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     3442 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/interpretation/explainer.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:30:01.238114 distool-0.1.9.1/distool/metrics/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/metrics/__init__.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:30:01.239994 distool-0.1.9.1/distool/metrics/extractor/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/metrics/extractor/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     2475 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/metrics/extractor/compute.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     7709 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/metrics/extractor/create_showcase.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:30:01.243215 distool-0.1.9.1/distool/models/
+-rw-r--r--   0 michilegorov   (501) staff       (20)      152 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/models/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     3360 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/models/urgency_classifier.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:30:01.244670 distool-0.1.9.1/distool/tests/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/tests/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)      959 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/tests/conftest.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:30:01.245863 distool-0.1.9.1/distool/tests/estimators/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/tests/estimators/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)      419 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/tests/estimators/test_classifier.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)      787 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/tests/estimators/test_fedot_classifier.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:30:01.246626 distool-0.1.9.1/distool/tests/explainer/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/tests/explainer/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     1346 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/tests/explainer/test_explainer.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:30:01.247480 distool-0.1.9.1/distool/tests/extractors/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/tests/extractors/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     1630 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/tests/extractors/test_symptom_extractor.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)       37 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/tests/test_base.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:30:01.228407 distool-0.1.9.1/distool.egg-info/
+-rw-r--r--   0 michilegorov   (501) staff       (20)     5975 2023-07-30 14:30:01.000000 distool-0.1.9.1/distool.egg-info/PKG-INFO
+-rw-r--r--   0 michilegorov   (501) staff       (20)     1384 2023-07-30 14:30:01.000000 distool-0.1.9.1/distool.egg-info/SOURCES.txt
+-rw-r--r--   0 michilegorov   (501) staff       (20)        1 2023-07-30 14:30:01.000000 distool-0.1.9.1/distool.egg-info/dependency_links.txt
+-rw-r--r--   0 michilegorov   (501) staff       (20)       64 2023-07-30 14:30:01.000000 distool-0.1.9.1/distool.egg-info/requires.txt
+-rw-r--r--   0 michilegorov   (501) staff       (20)       17 2023-07-30 14:30:01.000000 distool-0.1.9.1/distool.egg-info/top_level.txt
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:30:01.248342 distool-0.1.9.1/examples/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-02-04 10:03:31.000000 distool-0.1.9.1/examples/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     1116 2023-07-16 22:12:30.000000 distool-0.1.9.1/examples/pipeline_example.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)      295 2023-07-30 14:29:57.000000 distool-0.1.9.1/pyproject.toml
+-rw-r--r--   0 michilegorov   (501) staff       (20)       79 2023-07-30 14:30:01.249551 distool-0.1.9.1/setup.cfg
+-rw-r--r--   0 michilegorov   (501) staff       (20)     1332 2023-07-30 14:23:43.000000 distool-0.1.9.1/setup.py
```

### Comparing `distool-0.1.9/LICENSE.txt` & `distool-0.1.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `distool-0.1.9/PKG-INFO` & `distool-0.1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: distool
-Version: 0.1.9
+Version: 0.1.9.1
 Summary: Disease processing tool kit in Russian
 Home-page: https://github.com/nirma-patient-intake/disease/
 Download-URL: https://github.com/NIRMA-PATIENT-INTAKE/disease/archive/refs/tags/distool.tar.gz
 Author: NIRMA Team of ITMO University
 Author-email: egorovmichil9@gmail.com
 License: MIT
 Keywords: NLP,Disease,Health Condition
```

### Comparing `distool-0.1.9/README.md` & `distool-0.1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `distool-0.1.9/distool/__init__.py` & `distool-0.1.9.1/distool/__init__.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9/distool/base/estimators.py` & `distool-0.1.9.1/distool/base/estimators.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9/distool/data/symptoms.json` & `distool-0.1.9.1/distool/data/symptoms.json`

 * *Files identical despite different names*

### Comparing `distool-0.1.9/distool/estimators/classifiers.py` & `distool-0.1.9.1/distool/estimators/classifiers.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9/distool/feature_extraction/__init__.py` & `distool-0.1.9.1/distool/feature_extraction/__init__.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9/distool/feature_extraction/anamnesis.py` & `distool-0.1.9.1/distool/feature_extraction/anamnesis.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9/distool/feature_extraction/dumb_extractor.py` & `distool-0.1.9.1/distool/feature_extraction/dumb_extractor.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9/distool/feature_extraction/smart_extractor.py` & `distool-0.1.9.1/distool/feature_extraction/smart_extractor.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9/distool/feature_extraction/symptom.py` & `distool-0.1.9.1/distool/feature_extraction/symptom.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9/distool/feature_extraction/symptom_collection.py` & `distool-0.1.9.1/distool/feature_extraction/symptom_collection.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9/distool/feature_extraction/symptom_status.py` & `distool-0.1.9.1/distool/feature_extraction/symptom_status.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9/distool/interpretation/explainer.py` & `distool-0.1.9.1/distool/interpretation/explainer.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9/distool/metrics/extractor/compute.py` & `distool-0.1.9.1/distool/metrics/extractor/compute.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9/distool/metrics/extractor/create_showcase.py` & `distool-0.1.9.1/distool/metrics/extractor/create_showcase.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9/distool/models/urgency_classifier.py` & `distool-0.1.9.1/distool/models/urgency_classifier.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9/distool/tests/conftest.py` & `distool-0.1.9.1/distool/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9/distool/tests/estimators/test_fedot_classifier.py` & `distool-0.1.9.1/distool/tests/estimators/test_fedot_classifier.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9/distool/tests/explainer/test_explainer.py` & `distool-0.1.9.1/distool/tests/explainer/test_explainer.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9/distool/tests/extractors/test_symptom_extractor.py` & `distool-0.1.9.1/distool/tests/extractors/test_symptom_extractor.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9/distool.egg-info/PKG-INFO` & `distool-0.1.9.1/distool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: distool
-Version: 0.1.9
+Version: 0.1.9.1
 Summary: Disease processing tool kit in Russian
 Home-page: https://github.com/nirma-patient-intake/disease/
 Download-URL: https://github.com/NIRMA-PATIENT-INTAKE/disease/archive/refs/tags/distool.tar.gz
 Author: NIRMA Team of ITMO University
 Author-email: egorovmichil9@gmail.com
 License: MIT
 Keywords: NLP,Disease,Health Condition
```

### Comparing `distool-0.1.9/distool.egg-info/SOURCES.txt` & `distool-0.1.9.1/distool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `distool-0.1.9/examples/pipeline_example.py` & `distool-0.1.9.1/examples/pipeline_example.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9/setup.py` & `distool-0.1.9.1/setup.py`

 * *Files identical despite different names*

