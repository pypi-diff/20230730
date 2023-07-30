# Comparing `tmp/apollon-0.1.3.tar.gz` & `tmp/apollon-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apollon-0.1.3.tar", last modified: Tue Jun 27 13:15:55 2023, max compression
+gzip compressed data, was "apollon-0.1.4.tar", last modified: Sun Jul 30 09:34:33 2023, max compression
```

## Comparing `apollon-0.1.3.tar` & `apollon-0.1.4.tar`

### file list

```diff
@@ -1,76 +1,70 @@
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-06-27 13:15:55.962967 apollon-0.1.3/
--rw-r--r--   0 pmind      (502) staff       (20)     1484 2023-06-11 11:45:26.000000 apollon-0.1.3/CONTRIBUTING.md
--rw-r--r--   0 pmind      (502) staff       (20)     1522 2023-06-27 09:43:23.000000 apollon-0.1.3/LICENSE.txt
--rw-r--r--   0 pmind      (502) staff       (20)       74 2023-06-11 11:45:26.000000 apollon-0.1.3/MANIFEST.in
--rw-r--r--   0 pmind      (502) staff       (20)     3337 2023-06-27 13:15:55.961408 apollon-0.1.3/PKG-INFO
--rw-r--r--   0 pmind      (502) staff       (20)      517 2023-06-11 11:45:26.000000 apollon-0.1.3/README.md
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-06-27 13:15:55.907177 apollon-0.1.3/include/
--rw-r--r--   0 pmind      (502) staff       (20)     1774 2023-06-11 11:45:26.000000 apollon-0.1.3/include/cdim.h
--rw-r--r--   0 pmind      (502) staff       (20)      543 2023-06-11 11:45:26.000000 apollon-0.1.3/include/correlogram.h
--rw-r--r--   0 pmind      (502) staff       (20)      269 2023-06-11 11:45:26.000000 apollon-0.1.3/include/distance.h
--rw-r--r--   0 pmind      (502) staff       (20)     1256 2023-06-27 11:02:41.000000 apollon-0.1.3/pyproject.toml
--rw-r--r--   0 pmind      (502) staff       (20)       38 2023-06-27 13:15:55.963478 apollon-0.1.3/setup.cfg
--rw-r--r--   0 pmind      (502) staff       (20)      551 2023-06-27 11:01:01.000000 apollon-0.1.3/setup.py
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-06-27 13:15:55.896547 apollon-0.1.3/src/
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-06-27 13:15:55.914255 apollon-0.1.3/src/apollon/
--rw-r--r--   0 pmind      (502) staff       (20)      324 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/__init__.py
--rw-r--r--   0 pmind      (502) staff       (20)      678 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/_defaults.py
--rw-r--r--   0 pmind      (502) staff       (20)     8339 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/aplot.py
--rw-r--r--   0 pmind      (502) staff       (20)     4355 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/audio.py
--rw-r--r--   0 pmind      (502) staff       (20)     4988 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/container.py
--rw-r--r--   0 pmind      (502) staff       (20)      945 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/datasets.py
--rw-r--r--   0 pmind      (502) staff       (20)     3829 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/fractal.py
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-06-27 13:15:55.919115 apollon-0.1.3/src/apollon/hmm/
--rw-r--r--   0 pmind      (502) staff       (20)        0 2023-06-11 11:45:26.000000 apollon-0.1.3/src/apollon/hmm/__init__.py
--rw-r--r--   0 pmind      (502) staff       (20)    14664 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/hmm/poisson.py
--rw-r--r--   0 pmind      (502) staff       (20)    14319 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/hmm/utilities.py
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-06-27 13:15:55.922001 apollon-0.1.3/src/apollon/io/
--rw-r--r--   0 pmind      (502) staff       (20)       19 2023-06-11 11:45:26.000000 apollon-0.1.3/src/apollon/io/__init__.py
--rw-r--r--   0 pmind      (502) staff       (20)     6240 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/io/io.py
--rw-r--r--   0 pmind      (502) staff       (20)     3927 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/io/json.py
--rw-r--r--   0 pmind      (502) staff       (20)     8907 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/onsets.py
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-06-27 13:15:55.928967 apollon-0.1.3/src/apollon/schema/
--rw-r--r--   0 pmind      (502) staff       (20)      934 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/schema/corrdim.schema.json
--rw-r--r--   0 pmind      (502) staff       (20)      725 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/schema/corrgram.schema.json
--rw-r--r--   0 pmind      (502) staff       (20)      793 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/schema/dft_params.schema.json
--rw-r--r--   0 pmind      (502) staff       (20)      784 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/schema/ndarray.schema.json
--rw-r--r--   0 pmind      (502) staff       (20)     1461 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/schema/stft_params.schema.json
--rw-r--r--   0 pmind      (502) staff       (20)    15145 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/segment.py
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-06-27 13:15:55.938725 apollon-0.1.3/src/apollon/signal/
--rw-r--r--   0 pmind      (502) staff       (20)      265 2023-06-11 11:45:26.000000 apollon-0.1.3/src/apollon/signal/__init__.py
--rw-r--r--   0 pmind      (502) staff       (20)     6605 2023-06-11 11:45:26.000000 apollon-0.1.3/src/apollon/signal/_features_module.c
--rw-r--r--   0 pmind      (502) staff       (20)     8864 2023-06-11 11:45:26.000000 apollon-0.1.3/src/apollon/signal/cdim.c
--rw-r--r--   0 pmind      (502) staff       (20)     1274 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/signal/container.py
--rw-r--r--   0 pmind      (502) staff       (20)     1741 2023-06-11 11:45:26.000000 apollon-0.1.3/src/apollon/signal/correlogram.c
--rw-r--r--   0 pmind      (502) staff       (20)     3281 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/signal/critical_bands.py
--rw-r--r--   0 pmind      (502) staff       (20)    13736 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/signal/features.py
--rw-r--r--   0 pmind      (502) staff       (20)     1342 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/signal/filter.py
--rw-r--r--   0 pmind      (502) staff       (20)     8291 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/signal/spectral.py
--rw-r--r--   0 pmind      (502) staff       (20)     7506 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/signal/tools.py
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-06-27 13:15:55.952423 apollon-0.1.3/src/apollon/som/
--rw-r--r--   0 pmind      (502) staff       (20)      143 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/som/__init__.py
--rw-r--r--   0 pmind      (502) staff       (20)     4346 2023-06-11 11:45:26.000000 apollon-0.1.3/src/apollon/som/_distance_module.c
--rw-r--r--   0 pmind      (502) staff       (20)     1565 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/som/datasets.py
--rw-r--r--   0 pmind      (502) staff       (20)      194 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/som/defaults.py
--rw-r--r--   0 pmind      (502) staff       (20)      673 2023-06-11 11:45:26.000000 apollon-0.1.3/src/apollon/som/distance.c
--rw-r--r--   0 pmind      (502) staff       (20)     4335 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/som/neighbors.py
--rw-r--r--   0 pmind      (502) staff       (20)     7303 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/som/plot.py
--rw-r--r--   0 pmind      (502) staff       (20)    14153 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/som/som.py
--rw-r--r--   0 pmind      (502) staff       (20)     1367 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/som/topologies.py
--rw-r--r--   0 pmind      (502) staff       (20)     8448 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/som/utilities.py
--rw-r--r--   0 pmind      (502) staff       (20)     8182 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/tools.py
--rw-r--r--   0 pmind      (502) staff       (20)      723 2023-06-27 09:43:23.000000 apollon-0.1.3/src/apollon/types.py
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-06-27 13:15:55.917319 apollon-0.1.3/src/apollon.egg-info/
--rw-r--r--   0 pmind      (502) staff       (20)     3337 2023-06-27 13:15:55.000000 apollon-0.1.3/src/apollon.egg-info/PKG-INFO
--rw-r--r--   0 pmind      (502) staff       (20)     1653 2023-06-27 13:15:55.000000 apollon-0.1.3/src/apollon.egg-info/SOURCES.txt
--rw-r--r--   0 pmind      (502) staff       (20)        1 2023-06-27 13:15:55.000000 apollon-0.1.3/src/apollon.egg-info/dependency_links.txt
--rw-r--r--   0 pmind      (502) staff       (20)      112 2023-06-27 13:15:55.000000 apollon-0.1.3/src/apollon.egg-info/requires.txt
--rw-r--r--   0 pmind      (502) staff       (20)       28 2023-06-27 13:15:55.000000 apollon-0.1.3/src/apollon.egg-info/top_level.txt
-drwxr-xr-x   0 pmind      (502) staff       (20)        0 2023-06-27 13:15:55.960322 apollon-0.1.3/tests/
--rw-r--r--   0 pmind      (502) staff       (20)     2698 2023-06-11 11:45:26.000000 apollon-0.1.3/tests/test_audio.py
--rw-r--r--   0 pmind      (502) staff       (20)      917 2023-06-27 09:43:23.000000 apollon-0.1.3/tests/test_container.py
--rw-r--r--   0 pmind      (502) staff       (20)     1985 2023-06-27 10:58:49.000000 apollon-0.1.3/tests/test_io.py
--rw-r--r--   0 pmind      (502) staff       (20)     1494 2023-06-27 09:43:23.000000 apollon-0.1.3/tests/test_onsets.py
--rw-r--r--   0 pmind      (502) staff       (20)     3362 2023-06-27 09:43:23.000000 apollon-0.1.3/tests/test_schema.py
--rw-r--r--   0 pmind      (502) staff       (20)     5042 2023-06-27 09:43:23.000000 apollon-0.1.3/tests/test_segment.py
--rw-r--r--   0 pmind      (502) staff       (20)      445 2023-06-11 11:45:26.000000 apollon-0.1.3/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:34:33.769096 apollon-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-30 09:34:16.000000 apollon-0.1.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-30 09:34:16.000000 apollon-0.1.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-30 09:34:16.000000 apollon-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-30 09:34:33.769096 apollon-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-30 09:34:16.000000 apollon-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:34:33.761096 apollon-0.1.4/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-30 09:34:16.000000 apollon-0.1.4/include/cdim.h
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-30 09:34:16.000000 apollon-0.1.4/include/correlogram.h
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-30 09:34:16.000000 apollon-0.1.4/include/distance.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-30 09:34:16.000000 apollon-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 09:34:33.769096 apollon-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-30 09:34:16.000000 apollon-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:34:33.761096 apollon-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:34:33.761096 apollon-0.1.4/src/apollon/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/aplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/fractal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:34:33.765096 apollon-0.1.4/src/apollon/hmm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/hmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14664 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/hmm/poisson.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14319 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/hmm/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:34:33.765096 apollon-0.1.4/src/apollon/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/io/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/io/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/onsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15145 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/segment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:34:33.765096 apollon-0.1.4/src/apollon/signal/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/signal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/signal/_features_module.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/signal/cdim.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/signal/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/signal/correlogram.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/signal/critical_bands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/signal/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/signal/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8291 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/signal/spectral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/signal/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:34:33.765096 apollon-0.1.4/src/apollon/som/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/som/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/som/_distance_module.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/som/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/som/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/som/distance.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/som/neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/som/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14153 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/som/som.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/som/topologies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/som/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-30 09:34:16.000000 apollon-0.1.4/src/apollon/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:34:33.765096 apollon-0.1.4/src/apollon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-30 09:34:33.000000 apollon-0.1.4/src/apollon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-30 09:34:33.000000 apollon-0.1.4/src/apollon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 09:34:33.000000 apollon-0.1.4/src/apollon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-30 09:34:33.000000 apollon-0.1.4/src/apollon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-30 09:34:33.000000 apollon-0.1.4/src/apollon.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:34:33.769096 apollon-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-30 09:34:16.000000 apollon-0.1.4/tests/test_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-30 09:34:16.000000 apollon-0.1.4/tests/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-30 09:34:16.000000 apollon-0.1.4/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-30 09:34:16.000000 apollon-0.1.4/tests/test_onsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-07-30 09:34:16.000000 apollon-0.1.4/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-07-30 09:34:16.000000 apollon-0.1.4/tests/test_segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-30 09:34:16.000000 apollon-0.1.4/tests/test_tools.py
```

### Comparing `apollon-0.1.3/CONTRIBUTING.md` & `apollon-0.1.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/LICENSE.txt` & `apollon-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/PKG-INFO` & `apollon-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollon
-Version: 0.1.3
+Version: 0.1.4
 Summary: Feature extraction frame work for content-based music analysis
 Author-email: Michael Blaß <mblass@posteo.net>
 License: BSD 3-Clause License
         
         Copyright (c) 2019, Michael Blaß 
         All rights reserved.
         
@@ -57,17 +57,20 @@
 estimation. It includes subpackages for
 
 * Audio feature extraction
 * Hidden Markov Models
 * Self-Organizing Map
 
 ## 1. Installation
-### 1.1 Install from PyPi
-The latest version of apollon is available on PyPi. Just open a terminal an run
+### 1.1 Install from PyPI
+The latest version of apollon is available on PyPI. Just open a terminal an run
 the following command to download and install apollon:
 
 ```
 pip install apollon 
 ```
 
+We currently provide wheels for macOS and Windows; GNU/Linux users have to
+build apollon from source.
+
 ## 2. Documentation
 Full [documentation](https://apollon.readthedocs.io) is available on readthedocs.
```

### Comparing `apollon-0.1.3/README.md` & `apollon-0.1.4/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -3,17 +3,20 @@
 estimation. It includes subpackages for
 
 * Audio feature extraction
 * Hidden Markov Models
 * Self-Organizing Map
 
 ## 1. Installation
-### 1.1 Install from PyPi
-The latest version of apollon is available on PyPi. Just open a terminal an run
+### 1.1 Install from PyPI
+The latest version of apollon is available on PyPI. Just open a terminal an run
 the following command to download and install apollon:
 
 ```
 pip install apollon 
 ```
 
+We currently provide wheels for macOS and Windows; GNU/Linux users have to
+build apollon from source.
+
 ## 2. Documentation
 Full [documentation](https://apollon.readthedocs.io) is available on readthedocs.
```

### Comparing `apollon-0.1.3/include/cdim.h` & `apollon-0.1.4/include/cdim.h`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/include/correlogram.h` & `apollon-0.1.4/include/correlogram.h`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/pyproject.toml` & `apollon-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "apollon"
-version = "0.1.3"
+version = "0.1.4"
 description = "Feature extraction frame work for content-based music analysis"
 authors = [ {name="Michael Blaß", email="mblass@posteo.net"} ]
 license = { file="LICENSE.txt" }
 readme = "README.md"
 keywords = ["music", "analysis", "feature extraction"]
 classifiers = [
 	"License :: OSI Approved :: BSD License",
```

### Comparing `apollon-0.1.3/setup.py` & `apollon-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/src/apollon/_defaults.py` & `apollon-0.1.4/src/apollon/_defaults.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/src/apollon/aplot.py` & `apollon-0.1.4/src/apollon/aplot.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/src/apollon/audio.py` & `apollon-0.1.4/src/apollon/audio.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/src/apollon/container.py` & `apollon-0.1.4/src/apollon/container.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/src/apollon/datasets.py` & `apollon-0.1.4/src/apollon/datasets.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/src/apollon/fractal.py` & `apollon-0.1.4/src/apollon/fractal.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/src/apollon/hmm/poisson.py` & `apollon-0.1.4/src/apollon/hmm/poisson.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/src/apollon/hmm/utilities.py` & `apollon-0.1.4/src/apollon/hmm/utilities.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/src/apollon/io/io.py` & `apollon-0.1.4/src/apollon/io/io.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/src/apollon/io/json.py` & `apollon-0.1.4/src/apollon/io/json.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/src/apollon/onsets.py` & `apollon-0.1.4/src/apollon/onsets.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/src/apollon/segment.py` & `apollon-0.1.4/src/apollon/segment.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/src/apollon/signal/_features_module.c` & `apollon-0.1.4/src/apollon/signal/_features_module.c`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/src/apollon/signal/cdim.c` & `apollon-0.1.4/src/apollon/signal/cdim.c`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/src/apollon/signal/container.py` & `apollon-0.1.4/src/apollon/signal/container.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/src/apollon/signal/correlogram.c` & `apollon-0.1.4/src/apollon/signal/correlogram.c`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/src/apollon/signal/critical_bands.py` & `apollon-0.1.4/src/apollon/signal/critical_bands.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/src/apollon/signal/features.py` & `apollon-0.1.4/src/apollon/signal/features.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/src/apollon/signal/filter.py` & `apollon-0.1.4/src/apollon/signal/filter.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/src/apollon/signal/spectral.py` & `apollon-0.1.4/src/apollon/signal/spectral.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/src/apollon/signal/tools.py` & `apollon-0.1.4/src/apollon/signal/tools.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/src/apollon/som/_distance_module.c` & `apollon-0.1.4/src/apollon/som/_distance_module.c`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/src/apollon/som/datasets.py` & `apollon-0.1.4/src/apollon/som/datasets.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/src/apollon/som/distance.c` & `apollon-0.1.4/src/apollon/som/distance.c`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/src/apollon/som/neighbors.py` & `apollon-0.1.4/src/apollon/som/neighbors.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/src/apollon/som/plot.py` & `apollon-0.1.4/src/apollon/som/plot.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/src/apollon/som/som.py` & `apollon-0.1.4/src/apollon/som/som.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/src/apollon/som/topologies.py` & `apollon-0.1.4/src/apollon/som/topologies.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/src/apollon/som/utilities.py` & `apollon-0.1.4/src/apollon/som/utilities.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/src/apollon/tools.py` & `apollon-0.1.4/src/apollon/tools.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/src/apollon/types.py` & `apollon-0.1.4/src/apollon/types.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/src/apollon.egg-info/PKG-INFO` & `apollon-0.1.4/src/apollon.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollon
-Version: 0.1.3
+Version: 0.1.4
 Summary: Feature extraction frame work for content-based music analysis
 Author-email: Michael Blaß <mblass@posteo.net>
 License: BSD 3-Clause License
         
         Copyright (c) 2019, Michael Blaß 
         All rights reserved.
         
@@ -57,17 +57,20 @@
 estimation. It includes subpackages for
 
 * Audio feature extraction
 * Hidden Markov Models
 * Self-Organizing Map
 
 ## 1. Installation
-### 1.1 Install from PyPi
-The latest version of apollon is available on PyPi. Just open a terminal an run
+### 1.1 Install from PyPI
+The latest version of apollon is available on PyPI. Just open a terminal an run
 the following command to download and install apollon:
 
 ```
 pip install apollon 
 ```
 
+We currently provide wheels for macOS and Windows; GNU/Linux users have to
+build apollon from source.
+
 ## 2. Documentation
 Full [documentation](https://apollon.readthedocs.io) is available on readthedocs.
```

### Comparing `apollon-0.1.3/src/apollon.egg-info/SOURCES.txt` & `apollon-0.1.4/src/apollon.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -25,19 +25,14 @@
 src/apollon.egg-info/top_level.txt
 src/apollon/hmm/__init__.py
 src/apollon/hmm/poisson.py
 src/apollon/hmm/utilities.py
 src/apollon/io/__init__.py
 src/apollon/io/io.py
 src/apollon/io/json.py
-src/apollon/schema/corrdim.schema.json
-src/apollon/schema/corrgram.schema.json
-src/apollon/schema/dft_params.schema.json
-src/apollon/schema/ndarray.schema.json
-src/apollon/schema/stft_params.schema.json
 src/apollon/signal/__init__.py
 src/apollon/signal/_features_module.c
 src/apollon/signal/cdim.c
 src/apollon/signal/container.py
 src/apollon/signal/correlogram.c
 src/apollon/signal/critical_bands.py
 src/apollon/signal/features.py
```

### Comparing `apollon-0.1.3/tests/test_audio.py` & `apollon-0.1.4/tests/test_audio.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/tests/test_container.py` & `apollon-0.1.4/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/tests/test_io.py` & `apollon-0.1.4/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/tests/test_onsets.py` & `apollon-0.1.4/tests/test_onsets.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/tests/test_schema.py` & `apollon-0.1.4/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `apollon-0.1.3/tests/test_segment.py` & `apollon-0.1.4/tests/test_segment.py`

 * *Files identical despite different names*

