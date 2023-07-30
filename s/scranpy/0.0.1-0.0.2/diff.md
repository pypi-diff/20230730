# Comparing `tmp/scranpy-0.0.1.tar.gz` & `tmp/scranpy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scranpy-0.0.1.tar", last modified: Wed Jun 28 21:55:22 2023, max compression
+gzip compressed data, was "scranpy-0.0.2.tar", last modified: Sun Jul 30 03:20:37 2023, max compression
```

## Comparing `scranpy-0.0.1.tar` & `scranpy-0.0.2.tar`

### file list

```diff
@@ -1,42 +1,236 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 21:55:22.257355 scranpy-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-28 21:54:58.000000 scranpy-0.0.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 21:55:22.249355 scranpy-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 21:55:22.257355 scranpy-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-28 21:54:58.000000 scranpy-0.0.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-28 21:54:58.000000 scranpy-0.0.1/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-28 21:54:58.000000 scranpy-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-28 21:54:58.000000 scranpy-0.0.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-28 21:54:58.000000 scranpy-0.0.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-28 21:54:58.000000 scranpy-0.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    13477 2023-06-28 21:54:58.000000 scranpy-0.0.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-28 21:54:58.000000 scranpy-0.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-06-28 21:55:22.257355 scranpy-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-28 21:54:58.000000 scranpy-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 21:55:22.257355 scranpy-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-28 21:54:58.000000 scranpy-0.0.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 21:55:22.257355 scranpy-0.0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-28 21:54:58.000000 scranpy-0.0.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-28 21:54:58.000000 scranpy-0.0.1/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-28 21:54:58.000000 scranpy-0.0.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-06-28 21:54:58.000000 scranpy-0.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-28 21:54:58.000000 scranpy-0.0.1/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-28 21:54:58.000000 scranpy-0.0.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-28 21:54:58.000000 scranpy-0.0.1/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-28 21:54:58.000000 scranpy-0.0.1/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-28 21:54:58.000000 scranpy-0.0.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-28 21:54:58.000000 scranpy-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-28 21:55:22.261355 scranpy-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-28 21:54:58.000000 scranpy-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 21:55:22.253355 scranpy-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 21:55:22.257355 scranpy-0.0.1/src/scranpy/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-28 21:54:58.000000 scranpy-0.0.1/src/scranpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 21:55:22.257355 scranpy-0.0.1/src/scranpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-06-28 21:55:22.000000 scranpy-0.0.1/src/scranpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-28 21:55:22.000000 scranpy-0.0.1/src/scranpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 21:55:22.000000 scranpy-0.0.1/src/scranpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 21:55:21.000000 scranpy-0.0.1/src/scranpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-28 21:55:22.000000 scranpy-0.0.1/src/scranpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-28 21:55:22.000000 scranpy-0.0.1/src/scranpy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 21:55:22.257355 scranpy-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-28 21:54:58.000000 scranpy-0.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-06-28 21:54:58.000000 scranpy-0.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.311781 scranpy-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-30 03:20:16.000000 scranpy-0.0.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.247779 scranpy-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.263780 scranpy-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-07-30 03:20:16.000000 scranpy-0.0.2/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-30 03:20:16.000000 scranpy-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-30 03:20:16.000000 scranpy-0.0.2/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-30 03:20:16.000000 scranpy-0.0.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-30 03:20:16.000000 scranpy-0.0.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-30 03:20:16.000000 scranpy-0.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13477 2023-07-30 03:20:16.000000 scranpy-0.0.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-30 03:20:16.000000 scranpy-0.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-30 03:20:16.000000 scranpy-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-30 03:20:37.311781 scranpy-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-30 03:20:16.000000 scranpy-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.267780 scranpy-0.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-30 03:20:16.000000 scranpy-0.0.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.267780 scranpy-0.0.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-30 03:20:16.000000 scranpy-0.0.2/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-30 03:20:16.000000 scranpy-0.0.2/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-30 03:20:16.000000 scranpy-0.0.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-07-30 03:20:16.000000 scranpy-0.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-30 03:20:16.000000 scranpy-0.0.2/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-30 03:20:16.000000 scranpy-0.0.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-30 03:20:16.000000 scranpy-0.0.2/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-30 03:20:16.000000 scranpy-0.0.2/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-30 03:20:16.000000 scranpy-0.0.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.255780 scranpy-0.0.2/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.267780 scranpy-0.0.2/extern/libscran/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-30 03:20:16.000000 scranpy-0.0.2/extern/libscran/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.251779 scranpy-0.0.2/extern/libscran/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.267780 scranpy-0.0.2/extern/libscran/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/.github/workflows/doxygenate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/.github/workflows/run-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.267780 scranpy-0.0.2/extern/libscran/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   109654 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/docs/Doxyfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.267780 scranpy-0.0.2/extern/libscran/extern/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/extern/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.267780 scranpy-0.0.2/extern/libscran/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/gallery/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/gallery/minimal.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/gallery/pca_test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.251779 scranpy-0.0.2/extern/libscran/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.267780 scranpy-0.0.2/extern/libscran/include/scran/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.271780 scranpy-0.0.2/extern/libscran/include/scran/aggregation/
+-rw-r--r--   0 runner    (1001) docker     (123)    17638 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/aggregation/AggregateAcrossCells.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12401 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/aggregation/DownsampleByNeighbors.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.271780 scranpy-0.0.2/extern/libscran/include/scran/clustering/
+-rw-r--r--   0 runner    (1001) docker     (123)    13936 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/clustering/BuildSnnGraph.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16608 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/clustering/ClusterSnnGraph.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/clustering/igraph_utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.271780 scranpy-0.0.2/extern/libscran/include/scran/differential_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)    16702 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/differential_analysis/MatrixCalculator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    29152 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/differential_analysis/PairwiseEffects.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    48761 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/differential_analysis/ScoreMarkers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/differential_analysis/SummarizeEffects.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/differential_analysis/auc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/differential_analysis/cohens_d.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/differential_analysis/simple_diff.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/differential_analysis/summarize_comparisons.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.275780 scranpy-0.0.2/extern/libscran/include/scran/dimensionality_reduction/
+-rw-r--r--   0 runner    (1001) docker     (123)    27251 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/dimensionality_reduction/MultiBatchPca.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18792 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/dimensionality_reduction/ResidualPca.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/dimensionality_reduction/ScaleByNeighbors.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/dimensionality_reduction/SimplePca.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/dimensionality_reduction/blocking.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/dimensionality_reduction/convert.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/dimensionality_reduction/utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/dimensionality_reduction/wrappers.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.275780 scranpy-0.0.2/extern/libscran/include/scran/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/feature_selection/ChooseHvgs.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/feature_selection/FitVarianceTrend.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    27677 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/feature_selection/ModelGeneVariances.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/feature_selection/blocked_variances.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.275780 scranpy-0.0.2/extern/libscran/include/scran/feature_set_enrichment/
+-rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/feature_set_enrichment/HypergeometricTail.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10260 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/feature_set_enrichment/ScoreFeatureSet.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.279780 scranpy-0.0.2/extern/libscran/include/scran/normalization/
+-rw-r--r--   0 runner    (1001) docker     (123)     9653 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/normalization/CenterSizeFactors.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/normalization/ChoosePseudoCount.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/normalization/GroupedSizeFactors.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14550 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/normalization/LogNormCounts.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13663 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/normalization/MedianSizeFactors.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/normalization/utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.283780 scranpy-0.0.2/extern/libscran/include/scran/quality_control/
+-rw-r--r--   0 runner    (1001) docker     (123)    11203 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/quality_control/ChooseOutlierFilters.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10873 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/quality_control/ComputeMedianMad.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/quality_control/FilterCells.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/quality_control/PerCellAdtQcMetrics.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/quality_control/PerCellCrisprQcMetrics.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30743 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/quality_control/PerCellQcMetrics.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/quality_control/PerCellRnaQcMetrics.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16103 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/quality_control/SuggestAdtQcFilters.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14931 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/quality_control/SuggestCrisprQcFilters.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16295 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/quality_control/SuggestRnaQcFilters.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/quality_control/utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/scran.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.283780 scranpy-0.0.2/extern/libscran/include/scran/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/utils/average_vectors.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/utils/blocking.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/utils/macros.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/utils/subset_vector.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/utils/vector_to_pointers.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.283780 scranpy-0.0.2/extern/libscran/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.255780 scranpy-0.0.2/extern/libscran/tests/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.283780 scranpy-0.0.2/extern/libscran/tests/src/aggregation/
+-rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/aggregation/AggregateAcrossCells.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/aggregation/DownsampleByNeighbors.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.283780 scranpy-0.0.2/extern/libscran/tests/src/clustering/
+-rw-r--r--   0 runner    (1001) docker     (123)     9573 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/clustering/BuildSnnGraph.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/clustering/ClusterSnnGraph.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.287780 scranpy-0.0.2/extern/libscran/tests/src/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/data/Simulator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/data/data.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/data/data_sparse.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.287780 scranpy-0.0.2/extern/libscran/tests/src/differential_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)    22508 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/differential_analysis/MatrixCalculator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18566 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/differential_analysis/PairwiseEffects.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17375 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/differential_analysis/ScoreMarkers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/differential_analysis/auc.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/differential_analysis/cohens_d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/differential_analysis/simple_diff.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14226 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/differential_analysis/summarize_comparisons.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/differential_analysis/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.291780 scranpy-0.0.2/extern/libscran/tests/src/dimensionality_reduction/
+-rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/dimensionality_reduction/MultiBatchPca.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20523 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/dimensionality_reduction/ResidualPca.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/dimensionality_reduction/ScaleByNeighbors.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/dimensionality_reduction/SimplePca.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/dimensionality_reduction/compare_pcs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/dimensionality_reduction/convert.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/dimensionality_reduction/utils.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.291780 scranpy-0.0.2/extern/libscran/tests/src/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/feature_selection/ChooseHvgs.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/feature_selection/FitVarianceTrend.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/feature_selection/ModelGeneVariances.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.291780 scranpy-0.0.2/extern/libscran/tests/src/feature_set_enrichment/
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/feature_set_enrichment/HypergeometricTail.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11121 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/feature_set_enrichment/ScoreFeatureSet.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.291780 scranpy-0.0.2/extern/libscran/tests/src/normalization/
+-rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/normalization/CenterSizeFactors.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/normalization/ChoosePseudoCount.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/normalization/GroupedSizeFactors.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/normalization/LogNormCounts.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/normalization/MedianSizeFactors.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.295780 scranpy-0.0.2/extern/libscran/tests/src/quality_control/
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/quality_control/ChooseOutlierFilters.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/quality_control/ComputeMedianMad.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/quality_control/FilterCells.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/quality_control/PerCellAdtQcMetrics.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/quality_control/PerCellCrisprQcMetrics.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15529 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/quality_control/PerCellQcMetrics.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/quality_control/PerCellRnaQcMetrics.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/quality_control/SuggestAdtQcFilters.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/quality_control/SuggestCrisprQcFilters.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/quality_control/SuggestRnaQcFilters.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/quality_control/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.299780 scranpy-0.0.2/extern/libscran/tests/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/utils/average_vectors.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/utils/blocking.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/utils/compare_almost_equal.h
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/utils/compare_vectors.h
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/utils/custom_parallel.h
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/utils/macros.h
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/utils/subset_vector.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.299780 scranpy-0.0.2/extern/weightedlowess/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.255780 scranpy-0.0.2/extern/weightedlowess/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.299780 scranpy-0.0.2/extern/weightedlowess/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/.github/workflows/compare-limma.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/.github/workflows/doxygenate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/.github/workflows/run-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.299780 scranpy-0.0.2/extern/weightedlowess/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   108663 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/docs/Doxyfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.259780 scranpy-0.0.2/extern/weightedlowess/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.299780 scranpy-0.0.2/extern/weightedlowess/include/WeightedLowess/
+-rw-r--r--   0 runner    (1001) docker     (123)    31431 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/include/WeightedLowess/WeightedLowess.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.299780 scranpy-0.0.2/extern/weightedlowess/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.303780 scranpy-0.0.2/extern/weightedlowess/tests/R/
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/tests/R/run.R
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/tests/R/test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.303780 scranpy-0.0.2/extern/weightedlowess/tests/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/tests/src/basic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/tests/src/divzero.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/tests/src/options.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/tests/src/runners.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/tests/src/ties.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/tests/src/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/tests/src/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-30 03:20:16.000000 scranpy-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-30 03:20:37.311781 scranpy-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-30 03:20:16.000000 scranpy-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.259780 scranpy-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.303780 scranpy-0.0.2/src/scranpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-30 03:20:16.000000 scranpy-0.0.2/src/scranpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-30 03:20:16.000000 scranpy-0.0.2/src/scranpy/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-30 03:20:16.000000 scranpy-0.0.2/src/scranpy/cpphelpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.307780 scranpy-0.0.2/src/scranpy/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-30 03:20:16.000000 scranpy-0.0.2/src/scranpy/feature_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-07-30 03:20:16.000000 scranpy-0.0.2/src/scranpy/feature_selection/model_gene_variances.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.307780 scranpy-0.0.2/src/scranpy/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-30 03:20:16.000000 scranpy-0.0.2/src/scranpy/lib/log_norm_counts.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-30 03:20:16.000000 scranpy-0.0.2/src/scranpy/lib/model_gene_variances.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-30 03:20:16.000000 scranpy-0.0.2/src/scranpy/lib/per_cell_rna_qc_metrics.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-30 03:20:16.000000 scranpy-0.0.2/src/scranpy/lib/suggest_rna_qc_filters.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.307780 scranpy-0.0.2/src/scranpy/normalization/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-30 03:20:16.000000 scranpy-0.0.2/src/scranpy/normalization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-07-30 03:20:16.000000 scranpy-0.0.2/src/scranpy/normalization/log_norm_counts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.307780 scranpy-0.0.2/src/scranpy/quality_control/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-30 03:20:16.000000 scranpy-0.0.2/src/scranpy/quality_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-07-30 03:20:16.000000 scranpy-0.0.2/src/scranpy/quality_control/rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-30 03:20:16.000000 scranpy-0.0.2/src/scranpy/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-30 03:20:16.000000 scranpy-0.0.2/src/scranpy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.307780 scranpy-0.0.2/src/scranpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-30 03:20:37.000000 scranpy-0.0.2/src/scranpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8835 2023-07-30 03:20:37.000000 scranpy-0.0.2/src/scranpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 03:20:37.000000 scranpy-0.0.2/src/scranpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 03:20:36.000000 scranpy-0.0.2/src/scranpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-30 03:20:37.000000 scranpy-0.0.2/src/scranpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-30 03:20:37.000000 scranpy-0.0.2/src/scranpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.311781 scranpy-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-30 03:20:16.000000 scranpy-0.0.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-30 03:20:16.000000 scranpy-0.0.2/tests/test_log_norm_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-30 03:20:16.000000 scranpy-0.0.2/tests/test_model_gene_variances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-30 03:20:16.000000 scranpy-0.0.2/tests/test_quality_control_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-30 03:20:16.000000 scranpy-0.0.2/tox.ini
```

### Comparing `scranpy-0.0.1/.coveragerc` & `scranpy-0.0.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.1/.gitignore` & `scranpy-0.0.2/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -48,9 +48,7 @@
 cover/*
 MANIFEST
 
 # Per-project virtualenvs
 .venv*/
 .conda*/
 .python-version
-
-extern/
```

### Comparing `scranpy-0.0.1/CONTRIBUTING.md` & `scranpy-0.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.1/LICENSE.txt` & `scranpy-0.0.2/extern/libscran/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-The MIT License (MIT)
+MIT License
 
-Copyright (c) 2023 jkanche
+Copyright (c) 2021 Aaron Lun
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `scranpy-0.0.1/PKG-INFO` & `scranpy-0.0.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: scranpy
-Version: 0.0.1
-Summary: Analyze multi-modal single-cell data!
-Home-page: https://github.com/pyscaffold/pyscaffold/
-Author: jkanche
-Author-email: jayaram.kancherla@gmail.com
-License: MIT
-Project-URL: Documentation, https://pyscaffold.org/
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Provides-Extra: testing
-License-File: LICENSE.txt
-
 <!-- These are examples of badges you might want to add to your README:
      please update the URLs accordingly
 
 [![Built Status](https://api.cirrus-ci.com/github/<USER>/scranpy.svg?branch=main)](https://cirrus-ci.com/github/<USER>/scranpy)
 [![ReadTheDocs](https://readthedocs.org/projects/scranpy/badge/?version=latest)](https://scranpy.readthedocs.io/en/stable/)
 [![Coveralls](https://img.shields.io/coveralls/github/<USER>/scranpy/main.svg)](https://coveralls.io/r/<USER>/scranpy)
 [![PyPI-Server](https://img.shields.io/pypi/v/scranpy.svg)](https://pypi.org/project/scranpy/)
@@ -28,13 +12,34 @@
 
 [![Project generated with PyScaffold](https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold)](https://pyscaffold.org/)
 
 # scranpy
 
 Fast multi-modal single-cell data analysis! stay tuned...
 
+## Developer Notes
+
+
+Steps to setup dependencies - 
+
+- initialize git submodules in `extern/libscran`.
+
+First one needs to build the extern library, this would generate a shared object file to `src/scranpy/core-[*].so`
+
+```shell
+python setup.py build_ext --inplace
+```
+
+For typical development workflows, run this for tests
+
+```shell
+python setup.py build_ext --inplace && tox
+```
+
+
+
 <!-- pyscaffold-notes -->
 
 ## Note
 
-This project has been set up using PyScaffold 4.3.1. For details and usage
+This project has been set up using PyScaffold 4.5. For details and usage
 information on PyScaffold see https://pyscaffold.org/.
```

### Comparing `scranpy-0.0.1/docs/Makefile` & `scranpy-0.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.1/docs/conf.py` & `scranpy-0.0.2/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "scranpy"
-copyright = "2023, jkanche"
+copyright = "2023, Jayaram Kancherla"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # version: The short X.Y version.
 # release: The full version, including alpha/beta/rc tags.
@@ -260,15 +260,15 @@
     # Additional stuff for the LaTeX preamble.
     # "preamble": "",
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual]).
 latex_documents = [
-    ("index", "user_guide.tex", "scranpy Documentation", "jkanche", "manual")
+    ("index", "user_guide.tex", "scranpy Documentation", "Jayaram Kancherla", "manual")
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 # latex_logo = ""
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
```

### Comparing `scranpy-0.0.1/docs/index.md` & `scranpy-0.0.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.1/setup.cfg` & `scranpy-0.0.2/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 [metadata]
 name = scranpy
 description = Analyze multi-modal single-cell data!
-author = jkanche
+author = "Jayaram Kancherla, Aaron Lun"
 author_email = jayaram.kancherla@gmail.com
 license = MIT
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
-url = https://github.com/pyscaffold/pyscaffold/
+url = https://github.com/biocpy/scranpy
 project_urls = 
-	Documentation = https://pyscaffold.org/
+	Documentation = https://github.com/biocpy/scranpy
 platforms = any
 classifiers = 
 	Development Status :: 4 - Beta
 	Programming Language :: Python
 
 [options]
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 install_requires = 
 	importlib-metadata; python_version<"3.8"
+	mattress
+	numpy>=1.22.4
+	BiocFrame
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
@@ -58,15 +61,15 @@
 	.tox
 	build
 	dist
 	.eggs
 	docs/conf.py
 
 [pyscaffold]
-version = 4.3.1
+version = 4.5
 package = scranpy
 extensions = 
 	markdown
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `scranpy-0.0.1/src/scranpy/__init__.py` & `scranpy-0.0.2/src/scranpy/__init__.py`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.1/tox.ini` & `scranpy-0.0.2/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,16 @@
     build: build[virtualenv]
 passenv =
     SETUPTOOLS_*
 commands =
     clean: python -c 'import shutil; [shutil.rmtree(p, True) for p in ("build", "dist", "docs/_build")]'
     clean: python -c 'import pathlib, shutil; [shutil.rmtree(p, True) for p in pathlib.Path("src").glob("*.egg-info")]'
     build: python -m build {posargs}
+# By default, both `sdist` and `wheel` are built. If your sdist is too big or you don't want
+# to make it available, consider running: `tox -e build -- --wheel`
 
 
 [testenv:{docs,doctests,linkcheck}]
 description =
     docs: Invoke sphinx-build to build the docs
     doctests: Invoke sphinx-build to run doctests
     linkcheck: Check for broken links in the documentation
```

