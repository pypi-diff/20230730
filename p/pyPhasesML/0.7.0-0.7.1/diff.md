# Comparing `tmp/pyPhasesML-0.7.0.tar.gz` & `tmp/pyPhasesML-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPhasesML-0.7.0.tar", last modified: Sat Jul 29 16:54:39 2023, max compression
+gzip compressed data, was "pyPhasesML-0.7.1.tar", last modified: Sun Jul 30 14:51:17 2023, max compression
```

## Comparing `pyPhasesML-0.7.0.tar` & `pyPhasesML-0.7.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:54:39.606605 pyPhasesML-0.7.0/
--rw-rw-rw-   0 root         (0) root         (0)     1065 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3690 2023-07-29 16:54:39.606605 pyPhasesML-0.7.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3183 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:54:39.600605 pyPhasesML-0.7.0/pyPhasesML/
--rw-rw-rw-   0 root         (0) root         (0)     2410 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/DataAugmentation.py
--rw-rw-rw-   0 root         (0) root         (0)      895 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/DataSet.py
--rw-rw-rw-   0 root         (0) root         (0)     3849 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/DataversionManager.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/FeatureExtraction.py
--rw-rw-rw-   0 root         (0) root         (0)     4077 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/Model.py
--rw-rw-rw-   0 root         (0) root         (0)       94 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/ModelAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)     4952 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/ModelManager.py
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/Plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     4566 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/SignalPreprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)      391 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:54:39.602605 pyPhasesML-0.7.0/pyPhasesML/adapter/
--rw-rw-rw-   0 root         (0) root         (0)    10255 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/adapter/ModelKerasAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)     7159 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/adapter/ModelTf1Adapter.py
--rw-rw-rw-   0 root         (0) root         (0)     9901 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/adapter/ModelTorchAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/adapter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:54:39.603605 pyPhasesML-0.7.0/pyPhasesML/adapter/torch/
--rw-rw-rw-   0 root         (0) root         (0)      734 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/adapter/torch/CSVLogger.py
--rw-rw-rw-   0 root         (0) root         (0)      999 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/adapter/torch/Callback.py
--rw-rw-rw-   0 root         (0) root         (0)     3654 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/adapter/torch/CheckPoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1452 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/adapter/torch/CyclicLearningrate.py
--rw-rw-rw-   0 root         (0) root         (0)     2038 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/adapter/torch/FindLearningRate.py
--rw-rw-rw-   0 root         (0) root         (0)     1262 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/adapter/torch/LoadOptimizer.py
--rw-rw-rw-   0 root         (0) root         (0)     2582 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/adapter/torch/SystemCheckPoint.py
--rw-rw-rw-   0 root         (0) root         (0)       97 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/adapter/torch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1106 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:54:39.604605 pyPhasesML-0.7.0/pyPhasesML/datapipes/
--rw-rw-rw-   0 root         (0) root         (0)      464 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/datapipes/Augmentor.py
--rw-rw-rw-   0 root         (0) root         (0)      626 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/datapipes/DatasetXY.py
--rw-rw-rw-   0 root         (0) root         (0)      995 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/datapipes/FoldMapper.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/datapipes/RecordMap.py
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/datapipes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:54:39.605605 pyPhasesML-0.7.0/pyPhasesML/exporter/
--rw-rw-rw-   0 root         (0) root         (0)     5385 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/exporter/MemmapRecordExporter.py
--rw-rw-rw-   0 root         (0) root         (0)     3201 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/exporter/ModelExporter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/exporter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:54:39.605605 pyPhasesML-0.7.0/pyPhasesML/scorer/
--rw-rw-rw-   0 root         (0) root         (0)    19017 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/scorer/Scorer.py
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/scorer/ScorerTF.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/scorer/ScorerTorch.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyPhasesML/scorer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 16:54:39.601605 pyPhasesML-0.7.0/pyPhasesML.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3690 2023-07-29 16:54:39.000000 pyPhasesML-0.7.0/pyPhasesML.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1398 2023-07-29 16:54:39.000000 pyPhasesML-0.7.0/pyPhasesML.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 16:54:39.000000 pyPhasesML-0.7.0/pyPhasesML.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-29 16:54:39.000000 pyPhasesML-0.7.0/pyPhasesML.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-07-29 16:54:39.000000 pyPhasesML-0.7.0/pyPhasesML.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      484 2023-07-29 16:54:22.000000 pyPhasesML-0.7.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-29 16:54:39.606605 pyPhasesML-0.7.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      842 2023-07-29 16:54:24.000000 pyPhasesML-0.7.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 14:51:17.385240 pyPhasesML-0.7.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3690 2023-07-30 14:51:17.384240 pyPhasesML-0.7.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3183 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 14:51:17.380240 pyPhasesML-0.7.1/pyPhasesML/
+-rw-rw-rw-   0 root         (0) root         (0)     2410 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/DataAugmentation.py
+-rw-rw-rw-   0 root         (0) root         (0)      895 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/DataSet.py
+-rw-rw-rw-   0 root         (0) root         (0)     3849 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/DataversionManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/FeatureExtraction.py
+-rw-rw-rw-   0 root         (0) root         (0)     4077 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/Model.py
+-rw-rw-rw-   0 root         (0) root         (0)       94 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/ModelAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     4952 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/ModelManager.py
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/Plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4566 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/SignalPreprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)      391 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 14:51:17.381240 pyPhasesML-0.7.1/pyPhasesML/adapter/
+-rw-rw-rw-   0 root         (0) root         (0)    10255 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/adapter/ModelKerasAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     7159 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/adapter/ModelTf1Adapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     9901 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/adapter/ModelTorchAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/adapter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 14:51:17.382240 pyPhasesML-0.7.1/pyPhasesML/adapter/torch/
+-rw-rw-rw-   0 root         (0) root         (0)      734 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/adapter/torch/CSVLogger.py
+-rw-rw-rw-   0 root         (0) root         (0)      999 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/adapter/torch/Callback.py
+-rw-rw-rw-   0 root         (0) root         (0)     3654 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/adapter/torch/CheckPoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1452 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/adapter/torch/CyclicLearningrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2038 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/adapter/torch/FindLearningRate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/adapter/torch/LoadOptimizer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2622 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/adapter/torch/SystemCheckPoint.py
+-rw-rw-rw-   0 root         (0) root         (0)       97 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/adapter/torch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 14:51:17.383240 pyPhasesML-0.7.1/pyPhasesML/datapipes/
+-rw-rw-rw-   0 root         (0) root         (0)      464 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/datapipes/Augmentor.py
+-rw-rw-rw-   0 root         (0) root         (0)      626 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/datapipes/DatasetXY.py
+-rw-rw-rw-   0 root         (0) root         (0)      995 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/datapipes/FoldMapper.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/datapipes/RecordMap.py
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/datapipes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 14:51:17.384240 pyPhasesML-0.7.1/pyPhasesML/exporter/
+-rw-rw-rw-   0 root         (0) root         (0)     5385 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/exporter/MemmapRecordExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3201 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/exporter/ModelExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/exporter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 14:51:17.384240 pyPhasesML-0.7.1/pyPhasesML/scorer/
+-rw-rw-rw-   0 root         (0) root         (0)    19017 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/scorer/Scorer.py
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/scorer/ScorerTF.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/scorer/ScorerTorch.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyPhasesML/scorer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 14:51:17.380240 pyPhasesML-0.7.1/pyPhasesML.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3690 2023-07-30 14:51:17.000000 pyPhasesML-0.7.1/pyPhasesML.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1398 2023-07-30 14:51:17.000000 pyPhasesML-0.7.1/pyPhasesML.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-30 14:51:17.000000 pyPhasesML-0.7.1/pyPhasesML.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-30 14:51:17.000000 pyPhasesML-0.7.1/pyPhasesML.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-30 14:51:17.000000 pyPhasesML-0.7.1/pyPhasesML.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      484 2023-07-30 14:50:59.000000 pyPhasesML-0.7.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-30 14:51:17.385240 pyPhasesML-0.7.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      842 2023-07-30 14:51:01.000000 pyPhasesML-0.7.1/setup.py
```

### Comparing `pyPhasesML-0.7.0/LICENSE` & `pyPhasesML-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.0/PKG-INFO` & `pyPhasesML-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.7.0/README.md` & `pyPhasesML-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.0/pyPhasesML/DataAugmentation.py` & `pyPhasesML-0.7.1/pyPhasesML/DataAugmentation.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.0/pyPhasesML/DataSet.py` & `pyPhasesML-0.7.1/pyPhasesML/DataSet.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.0/pyPhasesML/DataversionManager.py` & `pyPhasesML-0.7.1/pyPhasesML/DataversionManager.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.0/pyPhasesML/FeatureExtraction.py` & `pyPhasesML-0.7.1/pyPhasesML/FeatureExtraction.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.0/pyPhasesML/Model.py` & `pyPhasesML-0.7.1/pyPhasesML/Model.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.0/pyPhasesML/ModelManager.py` & `pyPhasesML-0.7.1/pyPhasesML/ModelManager.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.0/pyPhasesML/Plugin.py` & `pyPhasesML-0.7.1/pyPhasesML/Plugin.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.0/pyPhasesML/SignalPreprocessing.py` & `pyPhasesML-0.7.1/pyPhasesML/SignalPreprocessing.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.0/pyPhasesML/adapter/ModelKerasAdapter.py` & `pyPhasesML-0.7.1/pyPhasesML/adapter/ModelKerasAdapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.0/pyPhasesML/adapter/ModelTf1Adapter.py` & `pyPhasesML-0.7.1/pyPhasesML/adapter/ModelTf1Adapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.0/pyPhasesML/adapter/ModelTorchAdapter.py` & `pyPhasesML-0.7.1/pyPhasesML/adapter/ModelTorchAdapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.0/pyPhasesML/adapter/torch/CSVLogger.py` & `pyPhasesML-0.7.1/pyPhasesML/adapter/torch/CSVLogger.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.0/pyPhasesML/adapter/torch/Callback.py` & `pyPhasesML-0.7.1/pyPhasesML/adapter/torch/Callback.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.0/pyPhasesML/adapter/torch/CheckPoint.py` & `pyPhasesML-0.7.1/pyPhasesML/adapter/torch/CheckPoint.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.0/pyPhasesML/adapter/torch/CyclicLearningrate.py` & `pyPhasesML-0.7.1/pyPhasesML/adapter/torch/CyclicLearningrate.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.0/pyPhasesML/adapter/torch/FindLearningRate.py` & `pyPhasesML-0.7.1/pyPhasesML/adapter/torch/FindLearningRate.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.0/pyPhasesML/adapter/torch/LoadOptimizer.py` & `pyPhasesML-0.7.1/pyPhasesML/adapter/torch/LoadOptimizer.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.0/pyPhasesML/adapter/torch/SystemCheckPoint.py` & `pyPhasesML-0.7.1/pyPhasesML/adapter/torch/SystemCheckPoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 class SystemCheckPoint(Callback):
     def __init__(self, config: ModelConfig) -> None:
         super().__init__(config)
         signal.signal(signal.SIGTERM, self.shutdown)
         self.shutdownRequest = False
 
     def shutdown(self, signum, frame):
+        self.shutdownRequest = True
         self.logError("Shutdown requested received, waiting for the next checkpoint")
 
     def onTrainingStart(self, model, dataset):
         restorePath = self.getLogPath()
 
         if Path(f"{restorePath}/.resumeModel").exists():
             self.logSuccess("Restore training")
@@ -40,17 +41,17 @@
             # delete all resume files
             Path(f"{restorePath}/.resumeModel").unlink()
             Path(f"{restorePath}/.resumeOptimizer").unlink()
             Path(f"{restorePath}/.resumeBatchScheduler").unlink(missing_ok=True)
             Path(f"{restorePath}/.resumeAdapter").unlink()
 
     def onValidationEnd(self, model, results, scorer):
-        restorePath = self.getLogPath()
         # If a checkpoint is reached and shutdown signal received, exit gracefully
         if self.shutdownRequest:
+            restorePath = self.getLogPath()
             self.logSuccess("Shutdown ... Saving everything")
             torch.save(model.model.state_dict(), f"{restorePath}.resumeModel")
             torch.save(model.optimizer.state_dict(), f"{restorePath}.resumeOptimizer")
             if model.batchScheduler is not None:
                 torch.save(model.batchScheduler.state_dict(), f"{restorePath}.resumeBatchScheduler")
 
             with open(f"{restorePath}.resumeAdapter", "wb") as f:
```

### Comparing `pyPhasesML-0.7.0/pyPhasesML/config.yaml` & `pyPhasesML-0.7.1/pyPhasesML/config.yaml`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.0/pyPhasesML/datapipes/DatasetXY.py` & `pyPhasesML-0.7.1/pyPhasesML/datapipes/DatasetXY.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.0/pyPhasesML/datapipes/FoldMapper.py` & `pyPhasesML-0.7.1/pyPhasesML/datapipes/FoldMapper.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.0/pyPhasesML/exporter/MemmapRecordExporter.py` & `pyPhasesML-0.7.1/pyPhasesML/exporter/MemmapRecordExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.0/pyPhasesML/exporter/ModelExporter.py` & `pyPhasesML-0.7.1/pyPhasesML/exporter/ModelExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.0/pyPhasesML/scorer/Scorer.py` & `pyPhasesML-0.7.1/pyPhasesML/scorer/Scorer.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.0/pyPhasesML.egg-info/PKG-INFO` & `pyPhasesML-0.7.1/pyPhasesML.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.7.0/pyPhasesML.egg-info/SOURCES.txt` & `pyPhasesML-0.7.1/pyPhasesML.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.7.0/setup.py` & `pyPhasesML-0.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyPhasesML",
-    version="v0.7.0"[1:],
+    version="v0.7.1"[1:],
     author="Franz Ehrlich",
     author_email="fehrlichd@gmail.com",
     description="A Framework for creating a boilerplate template for ai projects that are ready for MLOps",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/",
     packages=setuptools.find_packages(),
```

