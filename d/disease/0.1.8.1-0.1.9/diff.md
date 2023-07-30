# Comparing `tmp/disease-0.1.8.1.tar.gz` & `tmp/disease-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disease-0.1.8.1.tar", last modified: Sun Jul 30 14:22:27 2023, max compression
+gzip compressed data, was "disease-0.1.9.tar", last modified: Sun Jul 30 14:23:47 2023, max compression
```

## Comparing `disease-0.1.8.1.tar` & `disease-0.1.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:22:27.098575 disease-0.1.8.1/
--rw-r--r--   0 michilegorov   (501) staff       (20)     1068 2023-07-16 22:12:30.000000 disease-0.1.8.1/LICENSE.txt
--rw-r--r--   0 michilegorov   (501) staff       (20)     5975 2023-07-30 14:22:27.098755 disease-0.1.8.1/PKG-INFO
--rw-r--r--   0 michilegorov   (501) staff       (20)     5129 2023-07-16 22:12:30.000000 disease-0.1.8.1/README.md
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:22:27.082423 disease-0.1.8.1/disease.egg-info/
--rw-r--r--   0 michilegorov   (501) staff       (20)     5975 2023-07-30 14:22:27.000000 disease-0.1.8.1/disease.egg-info/PKG-INFO
--rw-r--r--   0 michilegorov   (501) staff       (20)     1384 2023-07-30 14:22:27.000000 disease-0.1.8.1/disease.egg-info/SOURCES.txt
--rw-r--r--   0 michilegorov   (501) staff       (20)        1 2023-07-30 14:22:27.000000 disease-0.1.8.1/disease.egg-info/dependency_links.txt
--rw-r--r--   0 michilegorov   (501) staff       (20)       64 2023-07-30 14:22:27.000000 disease-0.1.8.1/disease.egg-info/requires.txt
--rw-r--r--   0 michilegorov   (501) staff       (20)       17 2023-07-30 14:22:27.000000 disease-0.1.8.1/disease.egg-info/top_level.txt
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:22:27.082795 disease-0.1.8.1/distool/
--rw-r--r--   0 michilegorov   (501) staff       (20)      836 2023-07-16 22:12:30.000000 disease-0.1.8.1/distool/__init__.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:22:27.083999 disease-0.1.8.1/distool/base/
--rw-r--r--   0 michilegorov   (501) staff       (20)      248 2023-07-16 22:12:30.000000 disease-0.1.8.1/distool/base/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     2511 2023-07-16 22:12:30.000000 disease-0.1.8.1/distool/base/estimators.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:22:27.084558 disease-0.1.8.1/distool/data/
--rw-r--r--   0 michilegorov   (501) staff       (20)   240820 2023-07-16 22:12:30.000000 disease-0.1.8.1/distool/data/symptoms.json
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:22:27.086462 disease-0.1.8.1/distool/estimators/
--rw-r--r--   0 michilegorov   (501) staff       (20)      441 2023-07-16 22:12:30.000000 disease-0.1.8.1/distool/estimators/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     4943 2023-07-16 22:12:30.000000 disease-0.1.8.1/distool/estimators/classifiers.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:22:27.089666 disease-0.1.8.1/distool/feature_extraction/
--rw-r--r--   0 michilegorov   (501) staff       (20)      586 2023-07-16 22:12:30.000000 disease-0.1.8.1/distool/feature_extraction/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     3880 2023-07-16 22:12:30.000000 disease-0.1.8.1/distool/feature_extraction/anamnesis.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     2000 2023-07-16 22:12:30.000000 disease-0.1.8.1/distool/feature_extraction/dumb_extractor.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     6538 2023-07-16 22:12:30.000000 disease-0.1.8.1/distool/feature_extraction/smart_extractor.py
--rw-r--r--   0 michilegorov   (501) staff       (20)      917 2023-07-16 22:12:30.000000 disease-0.1.8.1/distool/feature_extraction/symptom.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     3525 2023-07-16 22:12:30.000000 disease-0.1.8.1/distool/feature_extraction/symptom_collection.py
--rw-r--r--   0 michilegorov   (501) staff       (20)      547 2023-07-16 22:12:30.000000 disease-0.1.8.1/distool/feature_extraction/symptom_status.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:22:27.090529 disease-0.1.8.1/distool/interpretation/
--rw-r--r--   0 michilegorov   (501) staff       (20)      279 2023-07-16 22:12:30.000000 disease-0.1.8.1/distool/interpretation/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     3442 2023-07-16 22:12:30.000000 disease-0.1.8.1/distool/interpretation/explainer.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:22:27.090988 disease-0.1.8.1/distool/metrics/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 disease-0.1.8.1/distool/metrics/__init__.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:22:27.092041 disease-0.1.8.1/distool/metrics/extractor/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 disease-0.1.8.1/distool/metrics/extractor/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     2475 2023-07-16 22:12:30.000000 disease-0.1.8.1/distool/metrics/extractor/compute.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     7709 2023-07-16 22:12:30.000000 disease-0.1.8.1/distool/metrics/extractor/create_showcase.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:22:27.092834 disease-0.1.8.1/distool/models/
--rw-r--r--   0 michilegorov   (501) staff       (20)      152 2023-07-16 22:12:30.000000 disease-0.1.8.1/distool/models/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     3360 2023-07-16 22:12:30.000000 disease-0.1.8.1/distool/models/urgency_classifier.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:22:27.094148 disease-0.1.8.1/distool/tests/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 disease-0.1.8.1/distool/tests/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)      959 2023-07-16 22:12:30.000000 disease-0.1.8.1/distool/tests/conftest.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:22:27.095350 disease-0.1.8.1/distool/tests/estimators/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 disease-0.1.8.1/distool/tests/estimators/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)      419 2023-07-16 22:12:30.000000 disease-0.1.8.1/distool/tests/estimators/test_classifier.py
--rw-r--r--   0 michilegorov   (501) staff       (20)      787 2023-07-16 22:12:30.000000 disease-0.1.8.1/distool/tests/estimators/test_fedot_classifier.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:22:27.096326 disease-0.1.8.1/distool/tests/explainer/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 disease-0.1.8.1/distool/tests/explainer/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     1346 2023-07-16 22:12:30.000000 disease-0.1.8.1/distool/tests/explainer/test_explainer.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:22:27.097318 disease-0.1.8.1/distool/tests/extractors/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 disease-0.1.8.1/distool/tests/extractors/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     1630 2023-07-16 22:12:30.000000 disease-0.1.8.1/distool/tests/extractors/test_symptom_extractor.py
--rw-r--r--   0 michilegorov   (501) staff       (20)       37 2023-07-16 22:12:30.000000 disease-0.1.8.1/distool/tests/test_base.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:22:27.098156 disease-0.1.8.1/examples/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-02-04 10:03:31.000000 disease-0.1.8.1/examples/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     1116 2023-07-16 22:12:30.000000 disease-0.1.8.1/examples/pipeline_example.py
--rw-r--r--   0 michilegorov   (501) staff       (20)      135 2023-07-30 14:18:22.000000 disease-0.1.8.1/pyproject.toml
--rw-r--r--   0 michilegorov   (501) staff       (20)       79 2023-07-30 14:22:27.099342 disease-0.1.8.1/setup.cfg
--rw-r--r--   0 michilegorov   (501) staff       (20)     1330 2023-07-30 14:22:20.000000 disease-0.1.8.1/setup.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:23:47.460664 disease-0.1.9/
+-rw-r--r--   0 michilegorov   (501) staff       (20)     1068 2023-07-16 22:12:30.000000 disease-0.1.9/LICENSE.txt
+-rw-r--r--   0 michilegorov   (501) staff       (20)     5973 2023-07-30 14:23:47.460915 disease-0.1.9/PKG-INFO
+-rw-r--r--   0 michilegorov   (501) staff       (20)     5129 2023-07-16 22:12:30.000000 disease-0.1.9/README.md
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:23:47.437022 disease-0.1.9/disease.egg-info/
+-rw-r--r--   0 michilegorov   (501) staff       (20)     5973 2023-07-30 14:23:47.000000 disease-0.1.9/disease.egg-info/PKG-INFO
+-rw-r--r--   0 michilegorov   (501) staff       (20)     1384 2023-07-30 14:23:47.000000 disease-0.1.9/disease.egg-info/SOURCES.txt
+-rw-r--r--   0 michilegorov   (501) staff       (20)        1 2023-07-30 14:23:47.000000 disease-0.1.9/disease.egg-info/dependency_links.txt
+-rw-r--r--   0 michilegorov   (501) staff       (20)       64 2023-07-30 14:23:47.000000 disease-0.1.9/disease.egg-info/requires.txt
+-rw-r--r--   0 michilegorov   (501) staff       (20)       17 2023-07-30 14:23:47.000000 disease-0.1.9/disease.egg-info/top_level.txt
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:23:47.437533 disease-0.1.9/distool/
+-rw-r--r--   0 michilegorov   (501) staff       (20)      836 2023-07-16 22:12:30.000000 disease-0.1.9/distool/__init__.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:23:47.438962 disease-0.1.9/distool/base/
+-rw-r--r--   0 michilegorov   (501) staff       (20)      248 2023-07-16 22:12:30.000000 disease-0.1.9/distool/base/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     2511 2023-07-16 22:12:30.000000 disease-0.1.9/distool/base/estimators.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:23:47.439524 disease-0.1.9/distool/data/
+-rw-r--r--   0 michilegorov   (501) staff       (20)   240820 2023-07-16 22:12:30.000000 disease-0.1.9/distool/data/symptoms.json
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:23:47.443489 disease-0.1.9/distool/estimators/
+-rw-r--r--   0 michilegorov   (501) staff       (20)      441 2023-07-16 22:12:30.000000 disease-0.1.9/distool/estimators/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     4943 2023-07-16 22:12:30.000000 disease-0.1.9/distool/estimators/classifiers.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:23:47.448335 disease-0.1.9/distool/feature_extraction/
+-rw-r--r--   0 michilegorov   (501) staff       (20)      586 2023-07-16 22:12:30.000000 disease-0.1.9/distool/feature_extraction/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     3880 2023-07-16 22:12:30.000000 disease-0.1.9/distool/feature_extraction/anamnesis.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     2000 2023-07-16 22:12:30.000000 disease-0.1.9/distool/feature_extraction/dumb_extractor.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     6538 2023-07-16 22:12:30.000000 disease-0.1.9/distool/feature_extraction/smart_extractor.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)      917 2023-07-16 22:12:30.000000 disease-0.1.9/distool/feature_extraction/symptom.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     3525 2023-07-16 22:12:30.000000 disease-0.1.9/distool/feature_extraction/symptom_collection.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)      547 2023-07-16 22:12:30.000000 disease-0.1.9/distool/feature_extraction/symptom_status.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:23:47.449890 disease-0.1.9/distool/interpretation/
+-rw-r--r--   0 michilegorov   (501) staff       (20)      279 2023-07-16 22:12:30.000000 disease-0.1.9/distool/interpretation/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     3442 2023-07-16 22:12:30.000000 disease-0.1.9/distool/interpretation/explainer.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:23:47.450519 disease-0.1.9/distool/metrics/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 disease-0.1.9/distool/metrics/__init__.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:23:47.452096 disease-0.1.9/distool/metrics/extractor/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 disease-0.1.9/distool/metrics/extractor/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     2475 2023-07-16 22:12:30.000000 disease-0.1.9/distool/metrics/extractor/compute.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     7709 2023-07-16 22:12:30.000000 disease-0.1.9/distool/metrics/extractor/create_showcase.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:23:47.453444 disease-0.1.9/distool/models/
+-rw-r--r--   0 michilegorov   (501) staff       (20)      152 2023-07-16 22:12:30.000000 disease-0.1.9/distool/models/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     3360 2023-07-16 22:12:30.000000 disease-0.1.9/distool/models/urgency_classifier.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:23:47.455416 disease-0.1.9/distool/tests/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 disease-0.1.9/distool/tests/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)      959 2023-07-16 22:12:30.000000 disease-0.1.9/distool/tests/conftest.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:23:47.457205 disease-0.1.9/distool/tests/estimators/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 disease-0.1.9/distool/tests/estimators/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)      419 2023-07-16 22:12:30.000000 disease-0.1.9/distool/tests/estimators/test_classifier.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)      787 2023-07-16 22:12:30.000000 disease-0.1.9/distool/tests/estimators/test_fedot_classifier.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:23:47.458244 disease-0.1.9/distool/tests/explainer/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 disease-0.1.9/distool/tests/explainer/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     1346 2023-07-16 22:12:30.000000 disease-0.1.9/distool/tests/explainer/test_explainer.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:23:47.459177 disease-0.1.9/distool/tests/extractors/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 disease-0.1.9/distool/tests/extractors/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     1630 2023-07-16 22:12:30.000000 disease-0.1.9/distool/tests/extractors/test_symptom_extractor.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)       37 2023-07-16 22:12:30.000000 disease-0.1.9/distool/tests/test_base.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:23:47.460118 disease-0.1.9/examples/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-02-04 10:03:31.000000 disease-0.1.9/examples/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     1116 2023-07-16 22:12:30.000000 disease-0.1.9/examples/pipeline_example.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)      133 2023-07-30 14:23:43.000000 disease-0.1.9/pyproject.toml
+-rw-r--r--   0 michilegorov   (501) staff       (20)       79 2023-07-30 14:23:47.461617 disease-0.1.9/setup.cfg
+-rw-r--r--   0 michilegorov   (501) staff       (20)     1332 2023-07-30 14:23:43.000000 disease-0.1.9/setup.py
```

### Comparing `disease-0.1.8.1/LICENSE.txt` & `disease-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `disease-0.1.8.1/PKG-INFO` & `disease-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disease
-Version: 0.1.8.1
+Version: 0.1.9
 Summary: Disease processing tool kit in Russian
 Home-page: https://github.com/nirma-patient-intake/disease/
 Download-URL: https://github.com/NIRMA-PATIENT-INTAKE/disease/archive/refs/tags/distool.tar.gz
 Author: NIRMA Team of ITMO University
 Author-email: egorovmichil9@gmail.com
 License: MIT
 Keywords: NLP,Disease,Health Condition
```

### Comparing `disease-0.1.8.1/README.md` & `disease-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `disease-0.1.8.1/disease.egg-info/PKG-INFO` & `disease-0.1.9/disease.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disease
-Version: 0.1.8.1
+Version: 0.1.9
 Summary: Disease processing tool kit in Russian
 Home-page: https://github.com/nirma-patient-intake/disease/
 Download-URL: https://github.com/NIRMA-PATIENT-INTAKE/disease/archive/refs/tags/distool.tar.gz
 Author: NIRMA Team of ITMO University
 Author-email: egorovmichil9@gmail.com
 License: MIT
 Keywords: NLP,Disease,Health Condition
```

### Comparing `disease-0.1.8.1/disease.egg-info/SOURCES.txt` & `disease-0.1.9/disease.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `disease-0.1.8.1/distool/__init__.py` & `disease-0.1.9/distool/__init__.py`

 * *Files identical despite different names*

### Comparing `disease-0.1.8.1/distool/base/estimators.py` & `disease-0.1.9/distool/base/estimators.py`

 * *Files identical despite different names*

### Comparing `disease-0.1.8.1/distool/data/symptoms.json` & `disease-0.1.9/distool/data/symptoms.json`

 * *Files identical despite different names*

### Comparing `disease-0.1.8.1/distool/estimators/classifiers.py` & `disease-0.1.9/distool/estimators/classifiers.py`

 * *Files identical despite different names*

### Comparing `disease-0.1.8.1/distool/feature_extraction/__init__.py` & `disease-0.1.9/distool/feature_extraction/__init__.py`

 * *Files identical despite different names*

### Comparing `disease-0.1.8.1/distool/feature_extraction/anamnesis.py` & `disease-0.1.9/distool/feature_extraction/anamnesis.py`

 * *Files identical despite different names*

### Comparing `disease-0.1.8.1/distool/feature_extraction/dumb_extractor.py` & `disease-0.1.9/distool/feature_extraction/dumb_extractor.py`

 * *Files identical despite different names*

### Comparing `disease-0.1.8.1/distool/feature_extraction/smart_extractor.py` & `disease-0.1.9/distool/feature_extraction/smart_extractor.py`

 * *Files identical despite different names*

### Comparing `disease-0.1.8.1/distool/feature_extraction/symptom.py` & `disease-0.1.9/distool/feature_extraction/symptom.py`

 * *Files identical despite different names*

### Comparing `disease-0.1.8.1/distool/feature_extraction/symptom_collection.py` & `disease-0.1.9/distool/feature_extraction/symptom_collection.py`

 * *Files identical despite different names*

### Comparing `disease-0.1.8.1/distool/feature_extraction/symptom_status.py` & `disease-0.1.9/distool/feature_extraction/symptom_status.py`

 * *Files identical despite different names*

### Comparing `disease-0.1.8.1/distool/interpretation/explainer.py` & `disease-0.1.9/distool/interpretation/explainer.py`

 * *Files identical despite different names*

### Comparing `disease-0.1.8.1/distool/metrics/extractor/compute.py` & `disease-0.1.9/distool/metrics/extractor/compute.py`

 * *Files identical despite different names*

### Comparing `disease-0.1.8.1/distool/metrics/extractor/create_showcase.py` & `disease-0.1.9/distool/metrics/extractor/create_showcase.py`

 * *Files identical despite different names*

### Comparing `disease-0.1.8.1/distool/models/urgency_classifier.py` & `disease-0.1.9/distool/models/urgency_classifier.py`

 * *Files identical despite different names*

### Comparing `disease-0.1.8.1/distool/tests/conftest.py` & `disease-0.1.9/distool/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `disease-0.1.8.1/distool/tests/estimators/test_fedot_classifier.py` & `disease-0.1.9/distool/tests/estimators/test_fedot_classifier.py`

 * *Files identical despite different names*

### Comparing `disease-0.1.8.1/distool/tests/explainer/test_explainer.py` & `disease-0.1.9/distool/tests/explainer/test_explainer.py`

 * *Files identical despite different names*

### Comparing `disease-0.1.8.1/distool/tests/extractors/test_symptom_extractor.py` & `disease-0.1.9/distool/tests/extractors/test_symptom_extractor.py`

 * *Files identical despite different names*

### Comparing `disease-0.1.8.1/examples/pipeline_example.py` & `disease-0.1.9/examples/pipeline_example.py`

 * *Files identical despite different names*

### Comparing `disease-0.1.8.1/setup.py` & `disease-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     name="distool",
     description="Disease processing tool kit in Russian",
     packages=find_packages(),
     package_data={"distool": ["data/symptoms.json"]},
     include_package_data=True,
     long_description=open("./README.md").read(),
     long_description_content_type="text/markdown",
-    version="0.1.9",
+    # version="0.1.9",
     license="MIT",
     author="NIRMA Team of ITMO University",
     author_email="egorovmichil9@gmail.com",
     url="https://github.com/nirma-patient-intake/disease/",
     download_url="https://github.com/NIRMA-PATIENT-INTAKE/disease/archive/refs/tags/distool.tar.gz",
     keywords=[
         "NLP",
```

