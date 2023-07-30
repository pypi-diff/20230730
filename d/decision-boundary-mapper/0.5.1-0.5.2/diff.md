# Comparing `tmp/decision-boundary-mapper-0.5.1.tar.gz` & `tmp/decision-boundary-mapper-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decision-boundary-mapper-0.5.1.tar", last modified: Sun Jul  9 17:30:53 2023, max compression
+gzip compressed data, was "decision-boundary-mapper-0.5.2.tar", last modified: Sun Jul 30 10:42:07 2023, max compression
```

## Comparing `decision-boundary-mapper-0.5.1.tar` & `decision-boundary-mapper-0.5.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-07-09 17:30:53.796658 decision-boundary-mapper-0.5.1/
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     1071 2023-03-30 08:17:56.000000 decision-boundary-mapper-0.5.1/LICENSE.txt
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     3730 2023-07-09 17:30:53.797084 decision-boundary-mapper-0.5.1/PKG-INFO
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     2818 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/README.md
--rw-r--r--   0 cristiangrosu   (501) staff       (20)      107 2023-07-09 17:30:53.797559 decision-boundary-mapper-0.5.1/setup.cfg
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     1737 2023-07-09 17:30:46.000000 decision-boundary-mapper-0.5.1/setup.py
-drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-07-09 17:30:53.782154 decision-boundary-mapper-0.5.1/src/
-drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-07-09 17:30:53.785012 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/
-drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-07-09 17:30:53.788188 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/
--rw-r--r--   0 cristiangrosu   (501) staff       (20)    51902 2023-07-09 08:46:17.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/AbstractDBM.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     5735 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/AbstractNN.py
-drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-07-09 17:30:53.789394 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/DBM/
--rw-r--r--   0 cristiangrosu   (501) staff       (20)    12647 2023-07-09 08:44:46.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/DBM/DBM.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     5108 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/DBM/NNInv.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)      600 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/DBM/__init__.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     1519 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/DBM/projections.py
-drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-07-09 17:30:53.790573 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/SDBM/
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     7062 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/SDBM/Autoencoder.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     9850 2023-05-19 14:34:10.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/SDBM/SDBM.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     7841 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/SDBM/SSNP.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)      618 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/SDBM/__init__.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)      753 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/__init__.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)    13280 2023-05-29 12:45:43.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/tools.py
-drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-07-09 17:30:53.792638 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/GUI/
--rw-r--r--   0 cristiangrosu   (501) staff       (20)    28939 2023-07-09 11:12:41.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/GUI/DBMPlotterController.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)    25700 2023-07-09 11:13:27.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/GUI/DBMPlotterGUI.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)    20600 2023-05-20 06:01:02.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/GUI/GUI.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)    13781 2023-05-20 06:01:02.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/GUI/GUIController.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)      641 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/GUI/__init__.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     1906 2023-05-20 06:01:02.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/GUI/utils.py
-drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-07-09 17:30:53.794093 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/Logger/
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     2872 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/Logger/Logger.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     3096 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/Logger/LoggerGUI.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     1006 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/Logger/LoggerInterface.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     1794 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/Logger/LoggerModel.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)      721 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/Logger/__init__.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)      826 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/__init__.py
-drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-07-09 17:30:53.795258 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/examples/
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     6454 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/examples/DBM_usage_example.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     4718 2023-05-19 14:34:53.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/examples/SDBM_usage_example.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)      726 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/examples/__init__.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     3279 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/examples/utils.py
-drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-07-09 17:30:53.796402 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/utils/
--rw-r--r--   0 cristiangrosu   (501) staff       (20)      753 2023-05-20 06:01:02.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/utils/__init__.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     1351 2023-05-20 06:01:02.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/utils/config.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     4123 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/utils/dataReader.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     1296 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/utils/tools.py
-drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-07-09 17:30:53.786795 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper.egg-info/
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     3730 2023-07-09 17:30:53.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper.egg-info/PKG-INFO
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     1842 2023-07-09 17:30:53.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper.egg-info/SOURCES.txt
--rw-r--r--   0 cristiangrosu   (501) staff       (20)        1 2023-07-09 17:30:53.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper.egg-info/dependency_links.txt
--rw-r--r--   0 cristiangrosu   (501) staff       (20)      144 2023-07-09 17:30:53.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper.egg-info/requires.txt
--rw-r--r--   0 cristiangrosu   (501) staff       (20)       25 2023-07-09 17:30:53.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper.egg-info/top_level.txt
+drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-07-30 10:42:07.125591 decision-boundary-mapper-0.5.2/
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     1071 2023-03-30 08:17:56.000000 decision-boundary-mapper-0.5.2/LICENSE.txt
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     3732 2023-07-30 10:42:07.125826 decision-boundary-mapper-0.5.2/PKG-INFO
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     2820 2023-07-30 10:41:12.000000 decision-boundary-mapper-0.5.2/README.md
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)      107 2023-07-30 10:42:07.126480 decision-boundary-mapper-0.5.2/setup.cfg
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     1737 2023-07-30 10:41:34.000000 decision-boundary-mapper-0.5.2/setup.py
+drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-07-30 10:42:07.099966 decision-boundary-mapper-0.5.2/src/
+drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-07-30 10:42:07.104024 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/
+drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-07-30 10:42:07.108772 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/DBM/
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)    51957 2023-07-13 18:43:15.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/DBM/AbstractDBM.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     5726 2023-07-15 11:44:05.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/DBM/AbstractNN.py
+drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-07-30 10:42:07.110184 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/DBM/DBM/
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)    12786 2023-07-15 11:36:12.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/DBM/DBM/DBM.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     5160 2023-07-15 11:58:35.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/DBM/DBM/NNInv.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)      600 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/DBM/DBM/__init__.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     1519 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/DBM/DBM/projections.py
+drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-07-30 10:42:07.114552 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/DBM/SDBM/
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     7114 2023-07-15 11:58:54.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/DBM/SDBM/Autoencoder.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)    10009 2023-07-15 11:35:57.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/DBM/SDBM/SDBM.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     7893 2023-07-15 11:59:09.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/DBM/SDBM/SSNP.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)      618 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/DBM/SDBM/__init__.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)      753 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/DBM/__init__.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)    13280 2023-05-29 12:45:43.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/DBM/tools.py
+drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-07-30 10:42:07.119425 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/GUI/
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)    29084 2023-07-15 12:36:22.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/GUI/DBMPlotterController.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)    26013 2023-07-13 17:02:14.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/GUI/DBMPlotterGUI.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)    21394 2023-07-13 18:29:21.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/GUI/GUI.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)    14655 2023-07-15 12:45:06.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/GUI/GUIController.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)      641 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/GUI/__init__.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     1906 2023-05-20 06:01:02.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/GUI/utils.py
+drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-07-30 10:42:07.121645 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/Logger/
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     2854 2023-07-15 11:47:35.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/Logger/Logger.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     2966 2023-07-15 11:49:48.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/Logger/LoggerGUI.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     1006 2023-07-15 11:38:24.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/Logger/LoggerInterface.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     1951 2023-07-15 12:02:21.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/Logger/LoggerModel.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)      721 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/Logger/__init__.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)      826 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/__init__.py
+drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-07-30 10:42:07.123448 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/examples/
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     6454 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/examples/DBM_usage_example.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     4718 2023-07-30 10:40:16.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/examples/SDBM_usage_example.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)      726 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/examples/__init__.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     3279 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/examples/utils.py
+drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-07-30 10:42:07.125210 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/utils/
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)      804 2023-07-13 16:57:54.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/utils/__init__.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     1351 2023-07-13 18:41:18.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/utils/config.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     5049 2023-07-13 19:41:33.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/utils/dataReader.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     1670 2023-07-13 19:59:16.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/utils/tools.py
+drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-07-30 10:42:07.106869 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper.egg-info/
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     3732 2023-07-30 10:42:07.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper.egg-info/PKG-INFO
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     1842 2023-07-30 10:42:07.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper.egg-info/SOURCES.txt
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)        1 2023-07-30 10:42:07.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper.egg-info/dependency_links.txt
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)      144 2023-07-30 10:42:07.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper.egg-info/requires.txt
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)       25 2023-07-30 10:42:07.000000 decision-boundary-mapper-0.5.2/src/decision_boundary_mapper.egg-info/top_level.txt
```

### Comparing `decision-boundary-mapper-0.5.1/LICENSE.txt` & `decision-boundary-mapper-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.1/PKG-INFO` & `decision-boundary-mapper-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decision-boundary-mapper
-Version: 0.5.1
+Version: 0.5.2
 Summary: A tool for visualizing the decision boundary of a machine learning model.
 Home-page: https://github.com/cristi2019255/MasterThesis2023
 Author: Cristian Grosu
 Author-email: c.grosu@students.uu.nl
 License: MIT
 Description: # Short Description
         
@@ -32,18 +32,18 @@
         
         2. The package comes with two examples of complete pipelines for visualizing the decision boundaries of a classifier.
         Both examples use `MNIST` (handwritten digits) dataset.
         The first example `DBM_usage_example` uses `t-SNE` to project the data from the `nD` space to the `2D` space, then neural network is trained to fit the inverse projection from `2D` to `nD` and the decision boundaries are visualized using the `2D` projection. The second example `SDBM_usage_example` uses a neural network with an autoencoder architecture to learn the projection and the inverse projection. After which a simple classifier is used to color each point of the `2D` projection.
         The examples can be found in the `examples` folder.
         
         ```python
-        from decision_boundary_mapper import DBM_usage_example, SDM_usage_example
+        from decision_boundary_mapper import DBM_usage_example, SDBM_usage_example
         
         DBM_usage_example() # run the first example
-        SDM_usage_example() # run the second example
+        SDBM_usage_example() # run the second example
         ```
         
         1. The package main functionality comes in two classes `DBM` (i.e. learns inverse projection when a 2D projection is given) and `SDBM` (i.e. learns both the projection and the inverse projection).
         The classes can be used as follows:
         
         ```python
         from decision_boundary_mapper import DBM, SDBM
```

### Comparing `decision-boundary-mapper-0.5.1/README.md` & `decision-boundary-mapper-0.5.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 
 2. The package comes with two examples of complete pipelines for visualizing the decision boundaries of a classifier.
 Both examples use `MNIST` (handwritten digits) dataset.
 The first example `DBM_usage_example` uses `t-SNE` to project the data from the `nD` space to the `2D` space, then neural network is trained to fit the inverse projection from `2D` to `nD` and the decision boundaries are visualized using the `2D` projection. The second example `SDBM_usage_example` uses a neural network with an autoencoder architecture to learn the projection and the inverse projection. After which a simple classifier is used to color each point of the `2D` projection.
 The examples can be found in the `examples` folder.
 
 ```python
-from decision_boundary_mapper import DBM_usage_example, SDM_usage_example
+from decision_boundary_mapper import DBM_usage_example, SDBM_usage_example
 
 DBM_usage_example() # run the first example
-SDM_usage_example() # run the second example
+SDBM_usage_example() # run the second example
 ```
 
 1. The package main functionality comes in two classes `DBM` (i.e. learns inverse projection when a 2D projection is given) and `SDBM` (i.e. learns both the projection and the inverse projection).
 The classes can be used as follows:
 
 ```python
 from decision_boundary_mapper import DBM, SDBM
```

### Comparing `decision-boundary-mapper-0.5.1/setup.py` & `decision-boundary-mapper-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # remove the old documentation folder
 rmtree('docs', ignore_errors=True)
 
 os.system("pdoc --html src/decision_boundary_mapper -o docs")
 
 setup(
     name='decision-boundary-mapper',
-    version='0.5.1',
+    version='0.5.2',
     license='MIT',
     author="Cristian Grosu",
     author_email='c.grosu@students.uu.nl',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://github.com/cristi2019255/MasterThesis2023',
     keywords='Decision Boundary Mapper',
```

### Comparing `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/AbstractDBM.py` & `decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/DBM/AbstractDBM.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,17 @@
 DBM_DEFAULT_RESOLUTION = 256
 DEFAULT_WINDOW_SIZE = 8
 DBM_IMAGE_NAME = "boundary_map"
 DBM_CONFIDENCE_IMAGE_NAME = "boundary_map_confidence"
 
 PROJECTION_ERRORS_NEIGHBORS_NUMBER = 10
 
+DEFAULT_TRAINING_EPOCHS = 10
+DEFAULT_BATCH_SIZE = 128
+
 time_tracker_console = Logger(name="Decision Boundary Mapper - DBM", info_color="cyan", show_init=False)
 
 class FAST_DBM_STRATEGIES(Enum):
     NONE = "none"
     BINARY = "binary_split"
     CONFIDENCE_BASED = "confidence_split"
     CONFIDENCE_INTERPOLATION = "confidence_interpolation"
```

### Comparing `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/AbstractNN.py` & `decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/DBM/AbstractNN.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         self.save_folder_path = folder_path
         self.nn_name = nn_name
         self.neural_network = None
 
         try:
             self.load()
         except Exception as e:
-            self.console.error("Error loading the model: {}".format(e))
+            self.console.warn("Model not found, {}".format(e))
             self.console.warn("The model will be built and trained from scratch.")
 
     def load(self):
         """
             Loads an auto encoder from the specified folder path. With the .h5 extension.
             Args:
                 folder_path (str): The path to the folder where the model is saved.
```

### Comparing `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/DBM/DBM.py` & `decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/DBM/DBM/DBM.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import json
 import os
 import numpy as np
 
 from .NNInv import DEFAULT_MODEL_PATH, NNInv
 from .projections import PROJECTION_METHODS
 
 
-from ..AbstractDBM import AbstractDBM, DBM_DEFAULT_RESOLUTION, FAST_DBM_STRATEGIES
+from ..AbstractDBM import AbstractDBM, DBM_DEFAULT_RESOLUTION, DEFAULT_TRAINING_EPOCHS, DEFAULT_BATCH_SIZE, FAST_DBM_STRATEGIES
 
 from ...utils import track_time_wrapper, TRAIN_DATA_POINT_MARKER, TEST_DATA_POINT_MARKER, TRAIN_2D_FILE_NAME, TEST_2D_FILE_NAME
 from ...Logger import LoggerInterface, Logger
 time_tracker_console = Logger(name="Decision Boundary Mapper - DBM", info_color="cyan", show_init=False)
 
 CUSTOM_PROJECTION_NAME = "Custom"
 
@@ -57,42 +56,42 @@
         """
         super().__init__(classifier, logger)
         self.neural_network = None  # type: ignore
 
     @track_time_wrapper(logger=time_tracker_console)
     def fit(self,
             X2d: np.ndarray, Xnd: np.ndarray,
-            epochs: int = 300, batch_size: int = 32,
+            epochs: int = DEFAULT_TRAINING_EPOCHS, batch_size: int = DEFAULT_BATCH_SIZE,
             load_folder: str = DEFAULT_MODEL_PATH):
         """ 
         Learns the inverse projection on the given data set.
 
         Args:
             X2d (np.ndarray): Training data set 2D data got from the projection of the original data (e.g. PCA, t-SNE, UMAP)
             Xnd (np.ndarray): Training data set nD data (e.g. MNIST, CIFAR10) (i.e. the original data)
             epochs (int, optional): The number of epochs for which the DBM is trained. Defaults to 300.
             batch_size (int, optional): Train batch size. Defaults to 32.
 
         Returns:
             inverse_porjection_NN (NNInv): The trained inverse projection neural network.
         """
 
-        inverse_projection_NN = NNInv(folder_path=load_folder)
+        inverse_projection_NN = NNInv(folder_path=load_folder, logger=self.console)
         inverse_projection_NN.fit(X2d, Xnd,
                                   epochs=epochs,
                                   batch_size=batch_size)
         return inverse_projection_NN
 
     def generate_boundary_map(self,
                               Xnd_train: np.ndarray,
                               Xnd_test: np.ndarray,
                               X2d_train: np.ndarray | None = None,
                               X2d_test: np.ndarray | None = None,
-                              nn_train_epochs: int = 300,
-                              nn_train_batch_size: int = 32,
+                              nn_train_epochs: int = DEFAULT_TRAINING_EPOCHS,
+                              nn_train_batch_size: int = DEFAULT_BATCH_SIZE,
                               resolution: int = DBM_DEFAULT_RESOLUTION,
                               fast_decoding_strategy: FAST_DBM_STRATEGIES = FAST_DBM_STRATEGIES.NONE,
                               load_folder: str = DEFAULT_MODEL_PATH,
                               projection: str = 't-SNE'):
         """ 
         Generates a 2D boundary map of the classifier's decision boundary.
 
@@ -119,26 +118,27 @@
             >>> img, img_confidence, _, _ = dbm.generate_boundary_map(X_train, X_test)
             >>> fig, [ax1, ax2] = plt.subplots(1, 2, figsize=(10, 5))
             >>> ax1.imshow(img)
             >>> ax2.imshow(img_confidence)
             >>> plt.show()
         """
        
+        # adding projection method to the end of the load_folder path
+        if projection != load_folder.split(os.sep)[-1]:
+            load_folder = os.path.join(load_folder, projection)
+            
         if X2d_train is None or X2d_test is None:
             assert projection in PROJECTION_METHODS.keys()
             Xnd_train_flatten = Xnd_train.reshape((Xnd_train.shape[0], -1))
             Xnd_test_flatten = Xnd_test.reshape((Xnd_test.shape[0], -1))
             X2d_train, X2d_test = self.__transform_2d__(Xnd_train_flatten, Xnd_test_flatten, load_folder, projection)
         else:
             # Normalize the data to be in the range of [0,1]
             X2d_train, X2d_test = self.__normalize_2d__(X2d_train, X2d_test)
             
-        # adding projection method to the end of the load_folder path
-        if projection != load_folder.split(os.sep)[-1]:
-            load_folder = os.path.join(load_folder, projection)
 
         # creating a folder for the model if not present
         if not os.path.exists(os.path.join(load_folder)):
             os.makedirs(os.path.join(load_folder))
 
 
         if self.neural_network is None:
```

### Comparing `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/DBM/NNInv.py` & `decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/DBM/DBM/NNInv.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,15 +74,15 @@
                                                     name=NNINV_NAME)
 
         self.neural_network.compile(optimizer=tf.keras.optimizers.Adam(),
                                     loss=DECODER_LOSS,
                                     metrics=["accuracy"])
 
         if show_summary:
-            self.neural_network.summary()
+            self.neural_network.summary(print_fn=self.console.log)
 
     def fit(self,
             x2d: np.ndarray, xNd: np.ndarray,
             epochs: int = 300, batch_size: int = 32):
         """ 
         Fits the model to the specified data.
 
@@ -96,15 +96,15 @@
             self.console.log("Model already loaded. Skipping build.")
             return
 
         self.console.log("Building model according to the data shape.")
         self.__build__(output_shape=xNd.shape[1:], show_summary=True)
 
         stopping_callback = tf.keras.callbacks.EarlyStopping(monitor='val_loss', mode='min', patience=20, restore_best_weights=True)
-        logger_callback = LoggerModel(name=NNINV_NAME, show_init=False, epochs=epochs)
+        logger_callback = LoggerModel(name=NNINV_NAME, show_init=False, epochs=epochs, print_fn=self.console.log)
         self.console.log("Fitting model...")
 
         hist = self.neural_network.fit(x2d, xNd,
                                        epochs=epochs,
                                        batch_size=batch_size,
                                        shuffle=True,
                                        validation_split=0.2,
```

### Comparing `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/DBM/__init__.py` & `decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/DBM/DBM/__init__.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/DBM/projections.py` & `decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/DBM/DBM/projections.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/SDBM/Autoencoder.py` & `decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/DBM/SDBM/Autoencoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
                                                     name=AUTOENCODER_NAME)
 
         self.neural_network.compile(optimizer=tf.keras.optimizers.Adam(),
                                     loss=LOSS,
                                     metrics=["accuracy"])
 
         if show_summary:
-            self.neural_network.summary()
+            self.neural_network.summary(print_fn=self.console.log)
 
     def fit(self, X: np.ndarray,
             epochs: int = 10,
             batch_size: int = 128):
         """ 
         Fits the model to the specified data.
 
@@ -113,15 +113,15 @@
             self.decoder = self.neural_network.get_layer(DECODER_NAME)
             return
 
         self.console.log("Building model according to the data shape.")
         self.__build__(input_shape=X.shape[1:], show_summary=True)
 
         stopping_callback = tf.keras.callbacks.EarlyStopping(monitor='val_loss', mode='min', patience=20, restore_best_weights=True)
-        logger_callback = LoggerModel(name=AUTOENCODER_NAME, show_init=False, epochs=epochs)
+        logger_callback = LoggerModel(name=AUTOENCODER_NAME, show_init=False, epochs=epochs, print_fn=self.console.log)
 
         self.console.log("Fitting model...")
 
         history = self.neural_network.fit(X, X,
                                           epochs=epochs,
                                           batch_size=batch_size,
                                           shuffle=True,
```

### Comparing `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/SDBM/SDBM.py` & `decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/DBM/SDBM/SDBM.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import json
 import os
 import numpy as np
 from enum import Enum
 
 from .Autoencoder import Autoencoder
 from .SSNP import SSNP
-from ..AbstractDBM import AbstractDBM, DBM_DEFAULT_RESOLUTION, FAST_DBM_STRATEGIES
+from ..AbstractDBM import AbstractDBM, DBM_DEFAULT_RESOLUTION, DEFAULT_TRAINING_EPOCHS, DEFAULT_BATCH_SIZE, FAST_DBM_STRATEGIES
 
 from ...utils import track_time_wrapper, TEST_DATA_POINT_MARKER, TRAIN_DATA_POINT_MARKER
 from ...Logger import LoggerInterface, Logger
 
 time_tracker_console = Logger(name="Decision Boundary Mapper - DBM", info_color="cyan", show_init=False)
 
 DEFAULT_MODEL_PATH = os.path.join("tmp", "SDBM")
@@ -65,15 +65,15 @@
         super().__init__(classifier, logger)
         self.neural_network = None  # type: ignore
 
     @track_time_wrapper(logger=time_tracker_console)
     def fit(self,
             X: np.ndarray, Y: np.ndarray,
             architecture: NNArchitecture = NNArchitecture.AUTOENCODER,
-            epochs: int = 300, batch_size: int = 32,
+            epochs: int = DEFAULT_TRAINING_EPOCHS, batch_size: int = DEFAULT_BATCH_SIZE,
             load_folder: str = DEFAULT_MODEL_PATH):
         """
         Train a neural network that will contain the direct projection and the inverse projection.
         This neural network will be used to reduce the dimensionality of the data (nD -> 2D) and decode the 2D space to nD.
 
         Args:
             X (np.ndarray): Training data
@@ -84,27 +84,27 @@
             load_folder (str, optional): The folder path which contains a pre-trained network or will be used to store it if not exists. Defaults to DEFAULT_MODEL_PATH.
 
         Returns:
             neural_network (Autoencoder | SSNP): The trained neural network.
         """
         match architecture:
             case NNArchitecture.SSNP:
-                ssnp = SSNP(folder_path=load_folder)
+                ssnp = SSNP(folder_path=load_folder, logger=self.console)
                 ssnp.fit(X, Y, epochs, batch_size)
                 return ssnp
             case _:
-                autoencoder = Autoencoder(folder_path=load_folder)
+                autoencoder = Autoencoder(folder_path=load_folder, logger=self.console)
                 autoencoder.fit(X, epochs, batch_size)
                 return autoencoder
 
     def generate_boundary_map(self,
                               X_train: np.ndarray, Y_train: np.ndarray,
                               X_test: np.ndarray, Y_test: np.ndarray,
-                              nn_train_epochs: int = 300, 
-                              nn_train_batch_size: int = 32,
+                              nn_train_epochs: int = DEFAULT_TRAINING_EPOCHS, 
+                              nn_train_batch_size: int = DEFAULT_BATCH_SIZE,
                               nn_architecture: NNArchitecture = NNArchitecture.AUTOENCODER,
                               resolution: int = DBM_DEFAULT_RESOLUTION,
                               fast_decoding_strategy: FAST_DBM_STRATEGIES = FAST_DBM_STRATEGIES.NONE,
                               load_folder: str = DEFAULT_MODEL_PATH,
                               ):
         """Generate the decision boundary map
```

### Comparing `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/SDBM/SSNP.py` & `decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/DBM/SDBM/SSNP.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
                                     loss={DECODER_NAME: DECODER_LOSS,
                                           CLASSIFIER_NAME: CLASSIFIER_LOSS},
                                     loss_weights={DECODER_NAME: DECODER_LOSS_WEIGHT,
                                                   CLASSIFIER_NAME: CLASSIFIER_LOSS_WEIGHT},
                                     metrics={DECODER_NAME: "accuracy", CLASSIFIER_NAME: "accuracy"})
 
         if show_summary:
-            self.neural_network.summary()
+            self.neural_network.summary(print_fn=self.console.log)
 
     def fit(self, X: np.ndarray, Y: np.ndarray,
             epochs: int = 10, batch_size: int = 128):
         """ Fits the model to the specified data.
 
         Args:
             X (np.ndarray): Train input values
@@ -125,15 +125,15 @@
             return
 
         self.console.log("Building model according to the data shape.")
         num_classes = len(np.unique(Y))
         self.__build__(input_shape=X.shape[1:], num_classes=num_classes, show_summary=True)
 
         stopping_callback = tf.keras.callbacks.EarlyStopping(monitor='val_loss', mode='min', patience=20, restore_best_weights=True)
-        logger_callback = LoggerModel(name=SSNP_NAME, show_init=False, epochs=epochs)
+        logger_callback = LoggerModel(name=SSNP_NAME, show_init=False, epochs=epochs, print_fn=self.console.log)
 
         self.console.log("Fitting model...")
 
         history = self.neural_network.fit(X, [X, Y],
                                           epochs=epochs,
                                           batch_size=batch_size,
                                           shuffle=True,
```

### Comparing `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/SDBM/__init__.py` & `decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/DBM/SDBM/__init__.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/__init__.py` & `decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/DBM/__init__.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/tools.py` & `decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/DBM/tools.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/GUI/DBMPlotterController.py` & `decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/GUI/DBMPlotterController.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     def build_2D_image(self, colors_mapper, class_name_mapper=lambda x: str(x)):
         """Combines the img and the img_confidence into a single image.
 
         Args:
             img (np.ndarray): Label image.
             img_confidence (np.ndarray): Confidence image.
             colors_mapper (dict): Mapper of labels to colors.
-            class_name_mapper (function, optional): Describes how to map the data labels. Defaults to lambdax:str(x).
+            class_name_mapper (function, optional): Describes how to map the data labels. Defaults to lambda x:str(x).
             
         Returns:
             np.ndarray: The combined image.
             patches: The legend patches.
         """
         img = self.img
         color_img = np.zeros((img.shape[0], img.shape[1], 3))
@@ -470,14 +470,16 @@
             annImage.set_visible(True)
             # place it at the position of the event scatter point
             annImage.xy = (j, i)
 
             x_data, y_data = find_data_point(i, j)
             if x_data is not None:
                 annImage.set_visible(True)
+                resize_factor = int(len(x_data) / 50 + 1)
+                annImage.xybox = (50. * ws * resize_factor, 50. * hs * resize_factor)
                 image.set_data(x_data)
             else:
                 annImage.set_visible(False)
 
             if y_data is not None:
                 annLabels.set_visible(True)
                 annLabels.xy = (j, i)
```

### Comparing `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/GUI/DBMPlotterGUI.py` & `decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/GUI/DBMPlotterGUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,15 @@
                  X_test, Y_test,
                  encoded_train, encoded_test,
                  save_folder,
                  X_train_2d = None, X_test_2d = None,
                  projection_technique=None,
                  logger=None,
                  main_gui=None,
+                 class_name_mapper= lambda x: str(x)
                  ):
         """[summary] DBMPlotterGUI is a GUI that allows the user to visualize the decision boundary map and the errors of the DBM model.
         It also allows the user to change the labels of the data points and see the impact of the changes on the model.
 
         Args:
             dbm_model (DBM or SDBM): The DBM model that will be used to generate the decision boundary map.
             img (np.ndarray): The decision boundary map image.
@@ -129,17 +130,19 @@
             encoded_train (np.ndarray): Positions of the training data points in the 2D embedding space.
             encoded_test (np.ndarray): Positions of the test data points in the 2D embedding space.
             spaceNd (np.ndarray): This is a list of lists of size resolution*resolution. Each point in this list is an nd data point which can be a vector, a matrix or a multidimensional matrix.
             save_folder (string): The folder where all the DBM model related files will be saved.
             projection_technique (string, optional): The projection technique the user wants to use if DBM is used as dbm_model. Defaults to None.
             logger (Logger, optional): The logger which is meant for logging the info messages. Defaults to None.
             main_gui (GUI, optional): The GUI that started the DBMPlotterGUI if any. Defaults to None.
+            class_name_mapper (function, optional): The function which is meant for mapping class names to their corresponding values. Defaults to lambda x -> str(x).
         """
         
         self.main_gui = main_gui  # reference to main window
+        self.class_name_mapper = class_name_mapper
         if logger is None:
             self.console = Logger(name="DBMPlotterGUI")
         else:
             self.console = logger
         
         self.controller = DBMPlotterController(logger,
                                                 dbm_model,
@@ -150,15 +153,15 @@
                                                 encoded_train, encoded_test,
                                                 save_folder,
                                                 projection_technique)
         self.initialize()
         
 
     def initialize(self):
-        self.color_img, legend = self.controller.build_2D_image(colors_mapper=COLORS_MAPPER)
+        self.color_img, legend = self.controller.build_2D_image(colors_mapper=COLORS_MAPPER, class_name_mapper=self.class_name_mapper)
         # --------------------- Plotter related ---------------------
         self.classifier_performance_fig, self.classifier_performance_ax = self._build_plot_()
         self.fig, self.ax = self._build_plot_()
         self.controller.build_annotation_mapper(self.fig, self.ax)
         self.fig.legend(handles=legend, borderaxespad=0.)
 
     def _initialize_gui_(self):
```

### Comparing `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/GUI/GUI.py` & `decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/GUI/GUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             ],
             [
                 sg.Button("Upload FASHION MNIST Data set", button_color=(WHITE_COLOR, APP_PRIMARY_COLOR), font=APP_FONT, expand_x=True, key="-UPLOAD FASHION MNIST DATA BTN-"),
             ],
             [
                 sg.Button("Upload CIFAR10 Data set", button_color=(WHITE_COLOR, APP_PRIMARY_COLOR), font=APP_FONT, expand_x=True, key="-UPLOAD CIFAR10 DATA BTN-"),
             ],
-            [ sg.HSeparator()],
+            [ sg.HSeparator() ],
             [
                 Collapsible([
                     [
                         sg.Text(text="Choose the data folder: ", font=APP_FONT),
                         sg.In(enable_events=True, key="-DATA FOLDER-", visible=False),
                         sg.Button("Browse folder", 
                           button_type=sg.BUTTON_TYPE_BROWSE_FOLDER, 
@@ -90,14 +90,20 @@
                         ), 
                     ],
                     [
                         sg.Text("Choose the data file from the list: ", font=APP_FONT, expand_x=True),
                     ],
                     [
                        sg.pin(sg.Column([
+                            [sg.Text(key="-DATA FOLDER TOUT-", font=APP_FONT, expand_x=True)],
+                           ], key="-DATA FOLDER TOUT PIN-", visible=False, expand_x=True), 
+                        shrink=True, expand_x=True), 
+                    ],
+                    [
+                       sg.pin(sg.Column([
                             [sg.Text(key="-DATA FILE TOUT-", font=APP_FONT, expand_x=True)],
                            ], key="-DATA FILE TOUT PIN-", visible=False, expand_x=True), 
                         shrink=True, expand_x=True), 
                     ],
                     [
                         sg.Listbox(
                             values=[], enable_events=True, key="-DATA FILE LIST-", 
@@ -105,17 +111,21 @@
                             expand_x=True, size=(10, 10), font=APP_FONT_BOLD,
                         )
                     ],
                     [
                         sg.Button("Upload train data for DBM", button_color=(WHITE_COLOR, APP_PRIMARY_COLOR), font=APP_FONT, expand_x=True, key="-UPLOAD TRAIN DATA BTN-"),
                         sg.Button("Upload test data for DBM", button_color=(WHITE_COLOR, APP_PRIMARY_COLOR), font=APP_FONT, expand_x=True, key="-UPLOAD TEST DATA BTN-"),
                     ],
+                    [
+                        sg.Button("Upload Data set as folder", button_color=(WHITE_COLOR, APP_PRIMARY_COLOR), font=APP_FONT, expand_x=True, key="-UPLOAD FOLDER DATASET BTN-"),
+                    ],
+            
                 ], "-UPLOAD DATA COLLAPSABLE-", "Upload the dataset from a folder", collapsed=True, visible=True), 
             ],
-            [ sg.HSeparator()],
+            [ sg.HSeparator() ],
             [
                 sg.Text("Training data file: ", font=APP_FONT, key="-TRAIN DATA FILE-",  expand_x=True),
             ],
             [
                 sg.Text("Training data shape: ", font=APP_FONT, key="-TRAIN DATA SHAPE-", expand_x=True),
             ],
             [
@@ -306,14 +316,16 @@
             "-UPLOAD 2D TRAIN DATA BTN-": self.controller.handle_upload_2d_data_event,
             "-UPLOAD 2D TEST DATA BTN-": self.controller.handle_upload_2d_data_event,
             "-UPLOAD TRAIN DATA BTN-": self.controller.handle_upload_train_data_event,
             "-UPLOAD TEST DATA BTN-": self.controller.handle_upload_test_data_event,
             "-UPLOAD MNIST DATA BTN-": self.controller.handle_upload_known_data_event,
             "-UPLOAD FASHION MNIST DATA BTN-": self.controller.handle_upload_known_data_event,
             "-UPLOAD CIFAR10 DATA BTN-": self.controller.handle_upload_known_data_event,
+            "-UPLOAD FOLDER DATASET BTN-": self.controller.handle_upload_folder_dataset_event,
+            
             "-UPLOAD CLASSIFIER-": self.controller.handle_upload_classifier_event,
             
             # collapsable components
             "-DATA 2D COLLAPSABLE-/-BUTTON-": self.handle_collapse_event,
             "-DATA 2D COLLAPSABLE-/-TITLE-": self.handle_collapse_event,
             "-UPLOAD DATA COLLAPSABLE-/-BUTTON-": self.handle_collapse_event,
             "-UPLOAD DATA COLLAPSABLE-/-TITLE-": self.handle_collapse_event,
@@ -330,14 +342,16 @@
 
     def handle_2d_file_list_event(self, event, values):
         filename = os.path.join(values["-DATA 2D FOLDER-"], values["-DATA 2D FILE LIST-"][0])
         self.gui_logger.log(f"Selected file: {filename}")
         
     def handle_select_data_folder_event(self, event, values):
         folder = values["-DATA FOLDER-"]
+        self.window["-DATA FOLDER TOUT-"].update(folder)
+        self.switch_visibility(["-DATA FOLDER TOUT PIN-"], True)
         files = self.controller.handle_select_data_folder(folder)
         self.window["-DATA FILE LIST-"].update(files)
         
     def handle_select_2d_data_folder_event(self, event, values):
         folder = values["-DATA 2D FOLDER-"]
         files = self.controller.handle_select_data_folder(folder)
         self.window["-DATA 2D FILE LIST-"].update(files)
```

### Comparing `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/GUI/GUIController.py` & `decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/GUI/GUIController.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from shutil import rmtree
 import tensorflow as tf
 import numpy as np
 
 from .DBMPlotterGUI import DBMPlotterGUI
 from ..DBM import SDBM, DBM, NNArchitecture
 from ..Logger import Logger
-from ..utils import import_dataset, import_mnist_dataset, import_cifar10_dataset, import_fashion_mnist_dataset, TRAIN_2D_FILE_NAME, TEST_2D_FILE_NAME
+from ..utils import import_dataset, import_mnist_dataset, import_cifar10_dataset, import_fashion_mnist_dataset, import_folder_dataset, generate_class_name_mapper, TRAIN_2D_FILE_NAME, TEST_2D_FILE_NAME
 
 DBM_NNINV_TECHNIQUE = "nnInv"
 SDBM_SSNP_TECHNIQUE = "ssnp"
 SDBM_AUTOENCODER_TECHNIQUE = "autoencoder"
 
 DBM_TECHNIQUES = {
     SDBM_AUTOENCODER_TECHNIQUE: SDBM,
@@ -79,15 +79,16 @@
         self.X_test, self.Y_test = None, None
         self.X_train_2d, self.X_test_2d = None, None
 
         # --------------- Classifier --------------
         self.classifier = None
         
         # --------------- Others ---------------------
-        self.data_shape = (28, 28) # this is the shape of the data, it is used to reshape the data when importing it
+        self.data_shape = (28, 28) # this is the shape of the data, it is used to reshape the data when importing it from a csv file
+        self.class_names_mapper = lambda x: str(x)
        
     def stop(self):
         self.logger.log("Clearing resources...")
         # self.logger.log("Removing tmp folder...")
         # self.remove_tmp_folder()
         
     def create_tmp_folder(self):
@@ -210,23 +211,40 @@
 
         X_train, Y_train = X_train[:int(0.7*SAMPLES_LIMIT)], Y_train[:int(0.7*SAMPLES_LIMIT)]
         X_test, Y_test = X_test[:int(0.3*SAMPLES_LIMIT)], Y_test[:int(0.3*SAMPLES_LIMIT)]
 
         self.X_train, self.Y_train, self.X_test, self.Y_test = X_train, Y_train, X_test, Y_test
         self._post_uploading_processing_()
     
+    def handle_upload_folder_dataset_event(self, event, values):
+        folder = values["-DATA FOLDER-"]
+        self.dataset_name = "_".join(folder.split(os.sep)[-2:])
+        (X_train, Y_train), (X_test, Y_test) = import_folder_dataset(folder)
+
+        X_train = X_train.astype('float32') / 255
+        X_test = X_test.astype('float32') / 255
+
+        self.X_train, self.Y_train, self.X_test, self.Y_test = X_train, Y_train, X_test, Y_test
+        
+        self.class_names_mapper = generate_class_name_mapper(os.path.join(folder, "..", "classes.txt"))
+        
+        self._post_uploading_processing_()
+
+    
     def _post_uploading_processing_(self):
         self.num_classes = np.unique(self.Y_train).shape[0]
 
         self.window["-TRAIN DATA FILE-"].update(f"Training data: {self.dataset_name}")
         self.window["-TRAIN DATA SHAPE-"].update(f"Training data shape: X {self.X_train.shape} Y {self.Y_train.shape}")
 
         self.window["-TEST DATA FILE-"].update(f"Testing data: {self.dataset_name}")
         self.window["-TEST DATA SHAPE-"].update(f"Testing data shape: X {self.X_test.shape} Y {self.Y_test.shape}")
-
+        
+        self.window["-UPLOAD DATA COLLAPSABLE-"].update(visible=False)
+        
         if self.classifier is not None:
             self.switch_visibility(["-DBM BTN-"], True)
 
     def fetch_2d_data_from_folder(self, folder_path):
         if not os.path.exists(os.path.join(folder_path, TRAIN_2D_FILE_NAME)):
             X_train_2d = None
         else:
@@ -318,9 +336,10 @@
             X_test=self.X_test,
             Y_test=self.Y_test,
             X_train_2d=self.X_train_2d,
             X_test_2d=self.X_test_2d,
             main_gui=self.gui,  # reference to the main GUI
             save_folder=save_folder,
             projection_technique=projection_technique,
+            class_name_mapper=self.class_names_mapper
         )
```

### Comparing `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/GUI/__init__.py` & `decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/GUI/__init__.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/GUI/utils.py` & `decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/GUI/utils.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/Logger/Logger.py` & `decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/Logger/Logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,40 +35,40 @@
         """
         self.active = active
         self.name = name
         self.info_color = info_color
 
         if show_init:
             sep = "=" * 30
-            time = datetime.now().strftime("%H:%M:%S:%f")
+            time = datetime.now().strftime("%H:%M:%S")
             print(colored(f"[INFO] [{time}] [{self.name}] {sep}", self.info_color))
             print(colored(f"[INFO] [{time}] [{self.name}] {self.name} initialized", self.info_color))
             print(colored(f"[INFO] [{time}] [{self.name}] {sep}", self.info_color))
 
     def log(self, message: str):
         """ Log a message to the console
             Args:
                 message (str): the message to log
         """
         if self.active:
-            time = datetime.now().strftime("%H:%M:%S:%f")
+            time = datetime.now().strftime("%H:%M:%S")
             print(colored(f"[INFO] [{time}] [{self.name}] {message}", self.info_color))
 
     def warn(self, message: str):
         if self.active:
-            time = datetime.now().strftime("%H:%M:%S:%f")
+            time = datetime.now().strftime("%H:%M:%S")
             print(colored(f"[WARNING] [{time}] [{self.name}] {message}", "yellow"))
 
     def error(self, message: str):
         if self.active:
-            time = datetime.now().strftime("%H:%M:%S:%f")
+            time = datetime.now().strftime("%H:%M:%S")
             print(colored(f"[ERROR] [{time}] [{self.name}] {message}", "red"))
 
     def debug(self, message: str):
         if self.active:
-            time = datetime.now().strftime("%H:%M:%S:%f")
+            time = datetime.now().strftime("%H:%M:%S")
             print(colored(f"[DEBUG] [{time}] [{self.name}] {message}", "blue"))
 
     def success(self, message: str):
         if self.active:
-            time = datetime.now().strftime("%H:%M:%S:%f")
+            time = datetime.now().strftime("%H:%M:%S")
             print(colored(f"[SUCCESS] [{time}] [{self.name}] {message}", "green"))
```

### Comparing `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/Logger/LoggerGUI.py` & `decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/Logger/LoggerGUI.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,37 +42,37 @@
             self.update_callback = update_callback
         else:
             print("No output provided for LoggerGUI. LoggerGUI will not print anything.")
             self.active = False
 
         if show_init and self.active:
             sep = "=" * 30
-            time = datetime.now().strftime("%H:%M:%S:%f")
+            time = datetime.now().strftime("%H:%M:%S")
 
-            self.print(f"[INFO] [{time}] [{self.name}] {sep}", self.info_color)
-            self.print(f"[INFO] [{time}] [{self.name}] {self.name} initialized", self.info_color)
-            self.print(f"[INFO] [{time}] [{self.name}] {sep}", self.info_color)
+            self.print(f"[INFO] [{time}] {sep}", self.info_color)
+            self.print(f"[INFO] [{time}] {self.name} initialized", self.info_color)
+            self.print(f"[INFO] [{time}] {sep}", self.info_color)
 
     def print(self, message: str, color: str = 'magenta'):
         if self.active:
             self.output.print(message, text_color=color)
             self.update_callback()
 
     def log(self, message: str):
-        time = datetime.now().strftime("%H:%M:%S:%f")
-        self.print(f"[INFO] [{time}] [{self.name}] {message}", self.info_color)
+        time = datetime.now().strftime("%H:%M:%S")
+        self.print(f"[INFO] [{time}] {message}", self.info_color)
 
     def warn(self, message: str):
-        time = datetime.now().strftime("%H:%M:%S:%f")
-        self.print(f"[WARNING] [{time}] [{self.name}] {message}", "yellow")
+        time = datetime.now().strftime("%H:%M:%S")
+        self.print(f"[WARNING] [{time}] {message}", "orange")
 
     def error(self, message: str):
-        time = datetime.now().strftime("%H:%M:%S:%f")
-        self.print(f"[ERROR] [{time}] [{self.name}] {message}", "red")
+        time = datetime.now().strftime("%H:%M:%S")
+        self.print(f"[ERROR] [{time}] {message}", "red")
 
     def debug(self, message: str):
-        time = datetime.now().strftime("%H:%M:%S:%f")
-        self.print(f"[DEBUG] [{time}] [{self.name}] {message}", "blue")
+        time = datetime.now().strftime("%H:%M:%S")
+        self.print(f"[DEBUG] [{time}] {message}", "blue")
 
     def success(self, message: str):
-        time = datetime.now().strftime("%H:%M:%S:%f")
-        self.print(f"[SUCCESS] [{time}] [{self.name}] {message}", "green")
+        time = datetime.now().strftime("%H:%M:%S")
+        self.print(f"[SUCCESS] [{time}] {message}", "green")
```

### Comparing `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/Logger/LoggerInterface.py` & `decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/Logger/LoggerInterface.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/Logger/LoggerModel.py` & `decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/Logger/LoggerModel.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,29 +14,32 @@
 
 from datetime import datetime
 from termcolor import colored
 from tensorflow.keras.callbacks import Callback
 
 
 class LoggerModel(Callback):
-    def __init__(self, active: bool = True, name: str = "Neural Network", info_color: str = "magenta", show_init: bool = True, epochs: int = 100):
+    def __init__(self, active: bool = True, name: str = "Neural Network", info_color: str = "magenta", show_init: bool = True, epochs: int = 100, print_fn=None):
         """ Initialize the logger
 
         Args:
             active (bool, optional): Defaults to True.
             name (str, optional): Defaults to "Logger".
         """
         self.active = active
         self.name = name
         self.info_color = info_color
         self.epochs = epochs
+        self.print_fn = print_fn
         if show_init:
             sep = "=" * 30
-            time = datetime.now().strftime("%H:%M:%S:%f")
+            time = datetime.now().strftime("%H:%M:%S")
             print(colored(f"[INFO] [{time}] [{self.name}] {sep}", self.info_color))
             print(colored(f"[INFO] [{time}] [{self.name}] {self.name} initialized", self.info_color))
             print(colored(f"[INFO] [{time}] [{self.name}] {sep}", self.info_color))
 
     def on_epoch_end(self, epoch, logs={}):
         if self.active:
             logs = ", ".join([f"{key}: {value:.4f}" for key, value in logs.items()])
             print(colored(f"[INFO] [{self.name}] [Epoch {epoch}/{self.epochs}] {logs}", self.info_color))
+            if self.print_fn is not None:
+                self.print_fn(f"[Epoch {epoch}/{self.epochs}] {logs}")
```

### Comparing `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/Logger/__init__.py` & `decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/Logger/__init__.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/__init__.py` & `decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/examples/DBM_usage_example.py` & `decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/examples/DBM_usage_example.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/examples/SDBM_usage_example.py` & `decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/examples/SDBM_usage_example.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/examples/__init__.py` & `decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/examples/utils.py` & `decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/examples/utils.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/utils/__init__.py` & `decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/utils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,10 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .dataReader import import_dataset, import_mnist_dataset, import_cifar10_dataset, import_fashion_mnist_dataset
-from .tools import track_time_wrapper
+from .dataReader import import_dataset, import_mnist_dataset, import_cifar10_dataset, import_fashion_mnist_dataset, import_folder_dataset
+from .tools import track_time_wrapper, generate_class_name_mapper
 from .config import *
```

### Comparing `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/utils/config.py` & `decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/utils/config.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/utils/dataReader.py` & `decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/utils/dataReader.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import numpy as np
 from keras.datasets import fashion_mnist, mnist, cifar10
 import os
 import pandas as pd
+from PIL import Image
 
 from .. import Logger
 
 ALLOWED_DATA_FORMATS = [".csv", ".txt", ".npy"]
 
 
 def import_mnist_dataset() -> tuple:
@@ -59,14 +60,35 @@
     console = Logger(name="CIFAR10 dataset importer")
     (train_X, train_y), (test_X, test_y) = cifar10.load_data()
     console.log("CIFAR10 dataset imported")
     console.log(f"Train set: {train_X.shape}")
     console.log(f"Test set: {test_X.shape}")
     return (train_X, train_y), (test_X, test_y)
 
+def import_folder_dataset(dir:str, train_test_split = 0.8) -> tuple:
+    console = Logger(name="Dataset importer")
+    
+    file_list = [os.path.join(dir, file) for file in os.listdir(dir)]
+    Y = np.array([int(fname.split("_")[0]) - 1 for fname in os.listdir(dir)]) 
+    X = np.array([np.array(Image.open(fname)) for fname in file_list])
+    console.log(f"Dataset imported from {dir}")
+    console.log(f"Dataset shape: X {X.shape}, Y {Y.shape}")
+    
+    size = len(Y)
+    #np.random.seed(42)
+    #indices = np.random.permutation(X.shape[0])
+    #X, Y = X[indices], Y[indices]
+    (train_X, test_X) = X[:int(train_test_split*size)], X[int(train_test_split*size):]
+    (train_Y, test_Y) = Y[:int(train_test_split*size)], Y[int(train_test_split*size):]
+    
+    console.log(f"Train set: {train_X.shape}")
+    console.log(f"Test set: {test_X.shape}")
+    return (train_X, train_Y), (test_X, test_Y)
+
+    
 def import_dataset(file_path:str,
                    labels_index: int | None = 0,
                    limit: int | None = None,
                    shape: tuple | None = None,
                    ) -> tuple:       
     """Imports a dataset from a file"""
     if not os.path.exists(file_path):
```

### Comparing `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/utils/tools.py` & `decision-boundary-mapper-0.5.2/src/decision_boundary_mapper/utils/tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,7 +29,19 @@
             if logger is None:
                 print(f"{func.__name__} took {end-start} seconds")
             else:
                 logger.log(f"{func.__name__} took {end-start} seconds")
             return result
         return wrapper
     return function_wrapper
+
+def generate_class_name_mapper(file: str):
+    mapper = {}
+    with open(file, "r") as f:
+        lines = f.readlines()
+    for line in lines:
+        class_num, class_name = int(line.split(" ")[0]) - 1, line.split(" ")[1].replace("\n", "")
+        mapper[class_num] = class_name
+    
+    def class_name_mapper(x: int):
+        return mapper[x]
+    return class_name_mapper
```

### Comparing `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper.egg-info/PKG-INFO` & `decision-boundary-mapper-0.5.2/src/decision_boundary_mapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decision-boundary-mapper
-Version: 0.5.1
+Version: 0.5.2
 Summary: A tool for visualizing the decision boundary of a machine learning model.
 Home-page: https://github.com/cristi2019255/MasterThesis2023
 Author: Cristian Grosu
 Author-email: c.grosu@students.uu.nl
 License: MIT
 Description: # Short Description
         
@@ -32,18 +32,18 @@
         
         2. The package comes with two examples of complete pipelines for visualizing the decision boundaries of a classifier.
         Both examples use `MNIST` (handwritten digits) dataset.
         The first example `DBM_usage_example` uses `t-SNE` to project the data from the `nD` space to the `2D` space, then neural network is trained to fit the inverse projection from `2D` to `nD` and the decision boundaries are visualized using the `2D` projection. The second example `SDBM_usage_example` uses a neural network with an autoencoder architecture to learn the projection and the inverse projection. After which a simple classifier is used to color each point of the `2D` projection.
         The examples can be found in the `examples` folder.
         
         ```python
-        from decision_boundary_mapper import DBM_usage_example, SDM_usage_example
+        from decision_boundary_mapper import DBM_usage_example, SDBM_usage_example
         
         DBM_usage_example() # run the first example
-        SDM_usage_example() # run the second example
+        SDBM_usage_example() # run the second example
         ```
         
         1. The package main functionality comes in two classes `DBM` (i.e. learns inverse projection when a 2D projection is given) and `SDBM` (i.e. learns both the projection and the inverse projection).
         The classes can be used as follows:
         
         ```python
         from decision_boundary_mapper import DBM, SDBM
```

### Comparing `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper.egg-info/SOURCES.txt` & `decision-boundary-mapper-0.5.2/src/decision_boundary_mapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

