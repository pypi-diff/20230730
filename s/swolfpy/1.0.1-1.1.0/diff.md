# Comparing `tmp/swolfpy-1.0.1.tar.gz` & `tmp/swolfpy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swolfpy-1.0.1.tar", last modified: Sun Jun  4 21:39:26 2023, max compression
+gzip compressed data, was "C:\Users\msa75\Documents\Repos\github\swolfpy\dist\.tmp-dfx1lbx7\swolfpy-1.1.0.tar", last modified: Sun Jul 30 16:23:36 2023, max compression
```

## Comparing `swolfpy-1.0.1.tar` & `swolfpy-1.1.0.tar`

### file list

```diff
@@ -1,93 +1,77 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 21:39:26.536637 swolfpy-1.0.1/
--rw-rw-rw-   0        0        0      802 2023-06-04 17:35:50.000000 swolfpy-1.0.1/AUTHORS.rst
--rw-rw-rw-   0        0        0     1586 2022-11-25 03:16:38.000000 swolfpy-1.0.1/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1122 2023-06-04 17:35:50.000000 swolfpy-1.0.1/HISTORY.rst
--rw-rw-rw-   0        0        0    18431 2022-11-25 05:25:00.000000 swolfpy-1.0.1/LICENSE.md
--rw-rw-rw-   0        0        0      273 2022-11-25 05:47:32.000000 swolfpy-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     8173 2023-06-04 21:39:26.534636 swolfpy-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5711 2023-06-04 17:35:50.000000 swolfpy-1.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-04 21:39:25.946447 swolfpy-1.0.1/docs/
--rw-rw-rw-   0        0        0     9516 2023-06-04 17:35:50.000000 swolfpy-1.0.1/docs/Getting_started.rst
-drwxrwxrwx   0        0        0        0 2023-06-04 21:39:26.029451 swolfpy-1.0.1/docs/Images/
--rw-rw-rw-   0        0        0   119274 2022-11-25 05:48:12.000000 swolfpy-1.0.1/docs/Images/AddCol.png
--rw-rw-rw-   0        0        0   131147 2022-11-25 07:14:39.000000 swolfpy-1.0.1/docs/Images/AddTreat.png
--rw-rw-rw-   0        0        0   154839 2022-11-25 05:52:28.000000 swolfpy-1.0.1/docs/Images/CreateScen.png
--rw-rw-rw-   0        0        0   192895 2022-11-25 05:51:44.000000 swolfpy-1.0.1/docs/Images/DefSys.png
--rw-rw-rw-   0        0        0    33184 2022-11-25 06:11:16.000000 swolfpy-1.0.1/docs/Images/IPM_CommonData.png
--rw-rw-rw-   0        0        0    63578 2022-11-25 05:49:00.000000 swolfpy-1.0.1/docs/Images/IPM_Tech.png
--rw-rw-rw-   0        0        0   154988 2022-11-25 06:16:15.000000 swolfpy-1.0.1/docs/Images/ImportPM.png
--rw-rw-rw-   0        0        0   190612 2022-11-25 05:55:25.000000 swolfpy-1.0.1/docs/Images/LCAContr.png
--rw-rw-rw-   0        0        0   146574 2022-11-25 06:36:54.000000 swolfpy-1.0.1/docs/Images/LCARes.png
--rw-rw-rw-   0        0        0   370894 2022-11-25 05:58:53.000000 swolfpy-1.0.1/docs/Images/LCA_LCI.png
--rw-rw-rw-   0        0        0   245142 2022-11-25 05:52:10.000000 swolfpy-1.0.1/docs/Images/LCIAView.png
--rw-rw-rw-   0        0        0   283477 2022-11-25 05:54:33.000000 swolfpy-1.0.1/docs/Images/LoadProj.png
--rw-rw-rw-   0        0        0   244005 2022-11-25 05:59:15.000000 swolfpy-1.0.1/docs/Images/MC.png
--rw-rw-rw-   0        0        0   139690 2022-11-25 05:54:59.000000 swolfpy-1.0.1/docs/Images/MCData.png
--rw-rw-rw-   0        0        0   156870 2022-11-25 05:59:37.000000 swolfpy-1.0.1/docs/Images/MCPlot.png
--rw-rw-rw-   0        0        0   209580 2022-11-25 05:56:18.000000 swolfpy-1.0.1/docs/Images/Opt.png
--rw-rw-rw-   0        0        0    79408 2022-11-25 05:48:28.000000 swolfpy-1.0.1/docs/Images/OptSet.png
--rw-rw-rw-   0        0        0   133628 2022-11-25 06:00:56.000000 swolfpy-1.0.1/docs/Images/SWM_network.png
--rw-rw-rw-   0        0        0   172835 2022-11-25 05:50:46.000000 swolfpy-1.0.1/docs/Images/SetupLCA.png
--rw-rw-rw-   0        0        0   188034 2022-11-25 05:58:04.000000 swolfpy-1.0.1/docs/Images/Start.png
--rw-rw-rw-   0        0        0      628 2022-11-25 05:54:42.000000 swolfpy-1.0.1/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-06-04 21:39:25.871450 swolfpy-1.0.1/docs/_build/
-drwxrwxrwx   0        0        0        0 2023-06-04 21:39:25.875463 swolfpy-1.0.1/docs/_build/html/
-drwxrwxrwx   0        0        0        0 2023-06-04 21:39:26.406640 swolfpy-1.0.1/docs/_build/html/_images/
--rw-rw-rw-   0        0        0   119274 2022-11-25 05:48:12.000000 swolfpy-1.0.1/docs/_build/html/_images/AddCol.png
--rw-rw-rw-   0        0        0   131147 2022-11-25 07:14:39.000000 swolfpy-1.0.1/docs/_build/html/_images/AddTreat.png
--rw-rw-rw-   0        0        0   154839 2022-11-25 05:52:28.000000 swolfpy-1.0.1/docs/_build/html/_images/CreateScen.png
--rw-rw-rw-   0        0        0   192895 2022-11-25 05:51:44.000000 swolfpy-1.0.1/docs/_build/html/_images/DefSys.png
--rw-rw-rw-   0        0        0    33184 2022-11-25 06:11:16.000000 swolfpy-1.0.1/docs/_build/html/_images/IPM_CommonData.png
--rw-rw-rw-   0        0        0    63578 2022-11-25 05:49:00.000000 swolfpy-1.0.1/docs/_build/html/_images/IPM_Tech.png
--rw-rw-rw-   0        0        0   154988 2022-11-25 06:16:15.000000 swolfpy-1.0.1/docs/_build/html/_images/ImportPM.png
--rw-rw-rw-   0        0        0   190612 2022-11-25 05:55:25.000000 swolfpy-1.0.1/docs/_build/html/_images/LCAContr.png
--rw-rw-rw-   0        0        0   146574 2022-11-25 06:36:54.000000 swolfpy-1.0.1/docs/_build/html/_images/LCARes.png
--rw-rw-rw-   0        0        0   370894 2022-11-25 05:58:53.000000 swolfpy-1.0.1/docs/_build/html/_images/LCA_LCI.png
--rw-rw-rw-   0        0        0   283477 2022-11-25 05:54:33.000000 swolfpy-1.0.1/docs/_build/html/_images/LoadProj.png
--rw-rw-rw-   0        0        0   244005 2022-11-25 05:59:15.000000 swolfpy-1.0.1/docs/_build/html/_images/MC.png
--rw-rw-rw-   0        0        0   139690 2022-11-25 05:54:59.000000 swolfpy-1.0.1/docs/_build/html/_images/MCData.png
--rw-rw-rw-   0        0        0   156870 2022-11-25 05:59:37.000000 swolfpy-1.0.1/docs/_build/html/_images/MCPlot.png
--rw-rw-rw-   0        0        0   209580 2022-11-25 05:56:18.000000 swolfpy-1.0.1/docs/_build/html/_images/Opt.png
--rw-rw-rw-   0        0        0    79408 2022-11-25 05:48:28.000000 swolfpy-1.0.1/docs/_build/html/_images/OptSet.png
--rw-rw-rw-   0        0        0   172835 2022-11-25 05:50:46.000000 swolfpy-1.0.1/docs/_build/html/_images/SetupLCA.png
--rw-rw-rw-   0        0        0   188034 2022-11-25 05:58:04.000000 swolfpy-1.0.1/docs/_build/html/_images/Start.png
-drwxrwxrwx   0        0        0        0 2023-06-04 21:39:26.448639 swolfpy-1.0.1/docs/_build/html/_static/
--rw-rw-rw-   0        0        0      286 2023-06-04 18:13:11.000000 swolfpy-1.0.1/docs/_build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-06-04 18:13:11.000000 swolfpy-1.0.1/docs/_build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-06-04 18:13:11.000000 swolfpy-1.0.1/docs/_build/html/_static/plus.png
--rw-rw-rw-   0        0        0       29 2022-11-25 06:11:54.000000 swolfpy-1.0.1/docs/authors.rst
--rw-rw-rw-   0        0        0     5979 2023-06-04 17:35:50.000000 swolfpy-1.0.1/docs/conf.py
--rw-rw-rw-   0        0        0       34 2022-11-25 06:10:07.000000 swolfpy-1.0.1/docs/contributing.rst
--rw-rw-rw-   0        0        0      335 2023-06-04 17:35:50.000000 swolfpy-1.0.1/docs/doc_inputdata.rst
--rw-rw-rw-   0        0        0      271 2023-06-04 17:35:50.000000 swolfpy-1.0.1/docs/doc_processmodels.rst
--rw-rw-rw-   0        0        0      982 2023-06-04 17:35:50.000000 swolfpy-1.0.1/docs/doc_swolfpy.rst
--rw-rw-rw-   0        0        0       29 2022-11-25 05:54:53.000000 swolfpy-1.0.1/docs/history.rst
--rw-rw-rw-   0        0        0      380 2023-06-04 17:35:50.000000 swolfpy-1.0.1/docs/index.rst
--rw-rw-rw-   0        0        0       92 2023-06-04 17:35:50.000000 swolfpy-1.0.1/docs/installation.rst
--rwxrwxrwx   0        0        0      805 2022-11-25 06:03:36.000000 swolfpy-1.0.1/docs/make.bat
--rw-rw-rw-   0        0        0       84 2022-11-25 06:00:08.000000 swolfpy-1.0.1/docs/readme.rst
--rw-rw-rw-   0        0        0    10974 2023-06-04 17:35:50.000000 swolfpy-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      335 2023-06-04 17:36:27.000000 swolfpy-1.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 21:39:26.536637 swolfpy-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-04 21:39:26.484635 swolfpy-1.0.1/swolfpy/
--rw-rw-rw-   0        0        0    15980 2023-06-04 17:35:50.000000 swolfpy-1.0.1/swolfpy/LCA_matrix.py
--rw-rw-rw-   0        0        0     8197 2023-06-04 17:35:50.000000 swolfpy-1.0.1/swolfpy/Monte_Carlo.py
--rw-rw-rw-   0        0        0    25661 2023-06-04 17:35:50.000000 swolfpy-1.0.1/swolfpy/Optimization.py
--rw-rw-rw-   0        0        0    12407 2023-06-04 17:35:50.000000 swolfpy-1.0.1/swolfpy/Parameters.py
--rw-rw-rw-   0        0        0    22614 2023-06-04 17:35:50.000000 swolfpy-1.0.1/swolfpy/ProcessDB.py
--rw-rw-rw-   0        0        0    19503 2023-06-04 17:35:50.000000 swolfpy-1.0.1/swolfpy/Project.py
--rw-rw-rw-   0        0        0   119828 2023-06-04 17:35:50.000000 swolfpy-1.0.1/swolfpy/Required_keys.py
--rw-rw-rw-   0        0        0     9059 2023-06-04 17:35:50.000000 swolfpy-1.0.1/swolfpy/Technosphere.py
--rw-rw-rw-   0        0        0     1151 2023-06-04 21:38:48.000000 swolfpy-1.0.1/swolfpy/__init__.py
--rw-rw-rw-   0        0        0      980 2023-06-04 17:35:50.000000 swolfpy-1.0.1/swolfpy/swolfpy_method.py
--rw-rw-rw-   0        0        0     3070 2023-06-04 17:35:50.000000 swolfpy-1.0.1/swolfpy/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-04 21:39:26.521641 swolfpy-1.0.1/swolfpy.egg-info/
--rw-rw-rw-   0        0        0     8173 2023-06-04 21:39:25.000000 swolfpy-1.0.1/swolfpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2057 2023-06-04 21:39:25.000000 swolfpy-1.0.1/swolfpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 21:39:25.000000 swolfpy-1.0.1/swolfpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      313 2023-06-04 21:39:25.000000 swolfpy-1.0.1/swolfpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-04 21:39:25.000000 swolfpy-1.0.1/swolfpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-04 21:39:26.531634 swolfpy-1.0.1/tests/
--rw-rw-rw-   0        0        0    61440 2022-11-25 05:43:10.000000 swolfpy-1.0.1/tests/.coverage
--rw-rw-rw-   0        0        0       42 2023-06-04 17:35:50.000000 swolfpy-1.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0     4774 2023-06-04 17:35:50.000000 swolfpy-1.0.1/tests/test_swolfpy.py
+drwxrwxrwx   0        0        0        0 2023-07-30 16:23:36.000000 swolfpy-1.1.0/
+-rw-rw-rw-   0        0        0      802 2023-06-20 02:21:16.000000 swolfpy-1.1.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1586 2023-06-20 02:21:16.000000 swolfpy-1.1.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1197 2023-07-30 15:31:37.000000 swolfpy-1.1.0/HISTORY.rst
+-rw-rw-rw-   0        0        0    18431 2023-06-20 02:21:16.000000 swolfpy-1.1.0/LICENSE.md
+-rw-rw-rw-   0        0        0      273 2023-07-30 16:20:10.000000 swolfpy-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     8245 2023-07-30 16:23:36.000000 swolfpy-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5710 2023-07-30 15:30:27.000000 swolfpy-1.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-30 16:23:35.000000 swolfpy-1.1.0/docs/
+-rw-rw-rw-   0        0        0     9516 2023-06-20 02:21:16.000000 swolfpy-1.1.0/docs/Getting_started.rst
+drwxrwxrwx   0        0        0        0 2023-07-30 16:23:36.000000 swolfpy-1.1.0/docs/Images/
+-rw-rw-rw-   0        0        0   119274 2023-06-20 02:21:16.000000 swolfpy-1.1.0/docs/Images/AddCol.png
+-rw-rw-rw-   0        0        0   131147 2023-06-20 02:21:16.000000 swolfpy-1.1.0/docs/Images/AddTreat.png
+-rw-rw-rw-   0        0        0   154839 2023-06-20 02:21:16.000000 swolfpy-1.1.0/docs/Images/CreateScen.png
+-rw-rw-rw-   0        0        0   192895 2023-06-20 02:21:16.000000 swolfpy-1.1.0/docs/Images/DefSys.png
+-rw-rw-rw-   0        0        0    33184 2023-06-20 02:21:16.000000 swolfpy-1.1.0/docs/Images/IPM_CommonData.png
+-rw-rw-rw-   0        0        0    63578 2023-06-20 02:21:16.000000 swolfpy-1.1.0/docs/Images/IPM_Tech.png
+-rw-rw-rw-   0        0        0   154988 2023-06-20 02:21:16.000000 swolfpy-1.1.0/docs/Images/ImportPM.png
+-rw-rw-rw-   0        0        0   190612 2023-06-20 02:21:16.000000 swolfpy-1.1.0/docs/Images/LCAContr.png
+-rw-rw-rw-   0        0        0   146574 2023-06-20 02:21:16.000000 swolfpy-1.1.0/docs/Images/LCARes.png
+-rw-rw-rw-   0        0        0   370894 2023-06-20 02:21:16.000000 swolfpy-1.1.0/docs/Images/LCA_LCI.png
+-rw-rw-rw-   0        0        0   245142 2023-06-20 02:21:16.000000 swolfpy-1.1.0/docs/Images/LCIAView.png
+-rw-rw-rw-   0        0        0   283477 2023-06-20 02:21:16.000000 swolfpy-1.1.0/docs/Images/LoadProj.png
+-rw-rw-rw-   0        0        0   244005 2023-06-20 02:21:16.000000 swolfpy-1.1.0/docs/Images/MC.png
+-rw-rw-rw-   0        0        0   139690 2023-06-20 02:21:16.000000 swolfpy-1.1.0/docs/Images/MCData.png
+-rw-rw-rw-   0        0        0   156870 2023-06-20 02:21:16.000000 swolfpy-1.1.0/docs/Images/MCPlot.png
+-rw-rw-rw-   0        0        0   209580 2023-06-20 02:21:16.000000 swolfpy-1.1.0/docs/Images/Opt.png
+-rw-rw-rw-   0        0        0    79408 2023-06-20 02:21:16.000000 swolfpy-1.1.0/docs/Images/OptSet.png
+-rw-rw-rw-   0        0        0   133628 2023-06-20 02:21:16.000000 swolfpy-1.1.0/docs/Images/SWM_network.png
+-rw-rw-rw-   0        0        0   172835 2023-06-20 02:21:16.000000 swolfpy-1.1.0/docs/Images/SetupLCA.png
+-rw-rw-rw-   0        0        0   188034 2023-06-20 02:21:16.000000 swolfpy-1.1.0/docs/Images/Start.png
+-rw-rw-rw-   0        0        0      628 2023-06-20 02:21:16.000000 swolfpy-1.1.0/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-06-20 02:21:16.000000 swolfpy-1.1.0/docs/authors.rst
+-rw-rw-rw-   0        0        0     5979 2023-06-20 02:21:16.000000 swolfpy-1.1.0/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-06-20 02:21:16.000000 swolfpy-1.1.0/docs/contributing.rst
+-rw-rw-rw-   0        0        0      335 2023-06-20 02:21:16.000000 swolfpy-1.1.0/docs/doc_inputdata.rst
+-rw-rw-rw-   0        0        0      271 2023-06-20 02:21:16.000000 swolfpy-1.1.0/docs/doc_processmodels.rst
+-rw-rw-rw-   0        0        0      982 2023-06-20 02:21:16.000000 swolfpy-1.1.0/docs/doc_swolfpy.rst
+-rw-rw-rw-   0        0        0       29 2023-06-20 02:21:16.000000 swolfpy-1.1.0/docs/history.rst
+-rw-rw-rw-   0        0        0      380 2023-06-20 02:21:16.000000 swolfpy-1.1.0/docs/index.rst
+-rw-rw-rw-   0        0        0       92 2023-06-20 02:21:16.000000 swolfpy-1.1.0/docs/installation.rst
+-rwxrwxrwx   0        0        0      805 2023-06-20 02:21:16.000000 swolfpy-1.1.0/docs/make.bat
+-rw-rw-rw-   0        0        0       84 2023-06-20 02:21:16.000000 swolfpy-1.1.0/docs/readme.rst
+-rw-rw-rw-   0        0        0    11007 2023-07-30 15:30:41.000000 swolfpy-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      335 2023-07-29 18:45:17.000000 swolfpy-1.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 16:23:36.000000 swolfpy-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-30 16:23:36.000000 swolfpy-1.1.0/swolfpy/
+-rw-rw-rw-   0        0        0    15980 2023-06-20 02:21:16.000000 swolfpy-1.1.0/swolfpy/LCA_matrix.py
+-rw-rw-rw-   0        0        0     8197 2023-06-20 02:21:16.000000 swolfpy-1.1.0/swolfpy/Monte_Carlo.py
+-rw-rw-rw-   0        0        0    25661 2023-06-20 02:21:16.000000 swolfpy-1.1.0/swolfpy/Optimization.py
+-rw-rw-rw-   0        0        0    12407 2023-06-20 02:21:16.000000 swolfpy-1.1.0/swolfpy/Parameters.py
+-rw-rw-rw-   0        0        0    22614 2023-06-20 02:21:16.000000 swolfpy-1.1.0/swolfpy/ProcessDB.py
+-rw-rw-rw-   0        0        0    19503 2023-06-20 02:21:16.000000 swolfpy-1.1.0/swolfpy/Project.py
+-rw-rw-rw-   0        0        0   119828 2023-06-20 02:21:16.000000 swolfpy-1.1.0/swolfpy/Required_keys.py
+-rw-rw-rw-   0        0        0     9059 2023-06-20 02:21:16.000000 swolfpy-1.1.0/swolfpy/Technosphere.py
+drwxrwxrwx   0        0        0        0 2023-07-30 16:23:36.000000 swolfpy-1.1.0/swolfpy/UI/
+-rw-rw-rw-   0        0        0    11730 2023-06-20 02:21:16.000000 swolfpy-1.1.0/swolfpy/UI/MC_ui.py
+-rw-rw-rw-   0        0        0   129019 2023-06-20 02:21:16.000000 swolfpy-1.1.0/swolfpy/UI/PySWOLF_run.py
+-rw-rw-rw-   0        0        0   140761 2023-06-20 02:21:16.000000 swolfpy-1.1.0/swolfpy/UI/PySWOLF_ui.py
+-rw-rw-rw-   0        0        0  1301136 2023-06-20 02:21:16.000000 swolfpy-1.1.0/swolfpy/UI/PyWOLF_Resource_rc.py
+-rw-rw-rw-   0        0        0     3233 2023-06-20 02:21:16.000000 swolfpy-1.1.0/swolfpy/UI/Reference_ui.py
+-rw-rw-rw-   0        0        0    11470 2023-06-20 02:21:16.000000 swolfpy-1.1.0/swolfpy/UI/Table_from_pandas.py
+-rw-rw-rw-   0        0        0     3827 2023-06-20 02:21:16.000000 swolfpy-1.1.0/swolfpy/UI/Workers.py
+-rw-rw-rw-   0        0        0        0 2023-06-20 02:21:16.000000 swolfpy-1.1.0/swolfpy/UI/__init__.py
+-rw-rw-rw-   0        0        0     4341 2023-06-20 02:21:16.000000 swolfpy-1.1.0/swolfpy/UI/adv_opt_ui.py
+-rw-rw-rw-   0        0        0     1151 2023-07-30 16:20:54.000000 swolfpy-1.1.0/swolfpy/__init__.py
+-rw-rw-rw-   0        0        0      980 2023-06-20 02:21:16.000000 swolfpy-1.1.0/swolfpy/swolfpy_method.py
+-rw-rw-rw-   0        0        0     3070 2023-06-20 02:21:16.000000 swolfpy-1.1.0/swolfpy/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-30 16:23:36.000000 swolfpy-1.1.0/swolfpy.egg-info/
+-rw-rw-rw-   0        0        0     8245 2023-07-30 16:23:35.000000 swolfpy-1.1.0/swolfpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1506 2023-07-30 16:23:35.000000 swolfpy-1.1.0/swolfpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 16:23:35.000000 swolfpy-1.1.0/swolfpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      313 2023-07-30 16:23:35.000000 swolfpy-1.1.0/swolfpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-30 16:23:35.000000 swolfpy-1.1.0/swolfpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 16:23:36.000000 swolfpy-1.1.0/tests/
+-rw-rw-rw-   0        0        0       42 2023-06-20 02:21:16.000000 swolfpy-1.1.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     4774 2023-06-20 02:21:16.000000 swolfpy-1.1.0/tests/test_swolfpy.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `swolfpy-1.0.1/AUTHORS.rst` & `swolfpy-1.1.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/CONTRIBUTING.rst` & `swolfpy-1.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/HISTORY.rst` & `swolfpy-1.1.0/HISTORY.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 =======
 History
 =======
 
+1.1.0 (2023-07-30)
+------------------
+
+* Downgrade to Python 3.9
+
+
+
 1.0.0 (2023-06-03)
 ------------------
 
 * Upgrade to Python 3.10
 * Add PreCommit
```

### Comparing `swolfpy-1.0.1/LICENSE.md` & `swolfpy-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/PKG-INFO` & `swolfpy-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: swolfpy
-Version: 1.0.1
+Version: 1.1.0
 Summary: Solid Waste Optimization Life-cycle Framework in Python(SwolfPy).
 Author-email: Mojtaba Sardarmehni <msardar2@alumni.ncsu.edu>
 Maintainer-email: Mojtaba Sardarmehni <msardar2@alumni.ncsu.edu>
 License: GNU GENERAL PUBLIC LICENSE V2
 Project-URL: Homepage, https://swolfpy-project.github.io/
 Project-URL: Documentation, https://swolfpy.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/SwolfPy-Project/swolfpy
 Keywords: LCA,solid_waste,waste_management,swolfpy,brightway2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Natural Language :: English
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.md
 License-File: AUTHORS.rst
 
 .. General
 
 ================================================================
@@ -153,15 +153,15 @@
 
 2- Update conda in a terminal window or anaconda prompt::
 
         conda update conda
 
 3- Create a new environment for swolfpy::
 
-        conda create --name swolfpy python=3.10 graphviz
+        conda create --name swolfpy python=3.9 graphviz
 
 4- Add Graphviz executables to your system PATH (This step is optional; Enables plotting SWM network). You can find Graphviz executables in ``\\miniconda3\\envs\\swolfpy\\Library\\bin\\graphviz`` folder or search for ``dot.exe`` file in your system. Add the directory to the ``Path`` variable in your environment variables.
 
 5- Activate the environment::
 
         conda activate swolfpy
 
@@ -180,14 +180,21 @@
 
 .. endInstallation
 
 =======
 History
 =======
 
+1.1.0 (2023-07-30)
+------------------
+
+* Downgrade to Python 3.9
+
+
+
 1.0.0 (2023-06-03)
 ------------------
 
 * Upgrade to Python 3.10
 * Add PreCommit
```

### Comparing `swolfpy-1.0.1/README.rst` & `swolfpy-1.1.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 
 2- Update conda in a terminal window or anaconda prompt::
 
         conda update conda
 
 3- Create a new environment for swolfpy::
 
-        conda create --name swolfpy python=3.10 graphviz
+        conda create --name swolfpy python=3.9 graphviz
 
 4- Add Graphviz executables to your system PATH (This step is optional; Enables plotting SWM network). You can find Graphviz executables in ``\\miniconda3\\envs\\swolfpy\\Library\\bin\\graphviz`` folder or search for ``dot.exe`` file in your system. Add the directory to the ``Path`` variable in your environment variables.
 
 5- Activate the environment::
 
         conda activate swolfpy
```

### Comparing `swolfpy-1.0.1/docs/Getting_started.rst` & `swolfpy-1.1.0/docs/Getting_started.rst`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/docs/Images/AddCol.png` & `swolfpy-1.1.0/docs/Images/AddCol.png`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/docs/Images/AddTreat.png` & `swolfpy-1.1.0/docs/Images/AddTreat.png`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/docs/Images/CreateScen.png` & `swolfpy-1.1.0/docs/Images/CreateScen.png`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/docs/Images/DefSys.png` & `swolfpy-1.1.0/docs/Images/DefSys.png`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/docs/Images/IPM_CommonData.png` & `swolfpy-1.1.0/docs/Images/IPM_CommonData.png`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/docs/Images/IPM_Tech.png` & `swolfpy-1.1.0/docs/Images/IPM_Tech.png`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/docs/Images/ImportPM.png` & `swolfpy-1.1.0/docs/Images/ImportPM.png`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/docs/Images/LCAContr.png` & `swolfpy-1.1.0/docs/Images/LCAContr.png`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/docs/Images/LCARes.png` & `swolfpy-1.1.0/docs/Images/LCARes.png`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/docs/Images/LCA_LCI.png` & `swolfpy-1.1.0/docs/Images/LCA_LCI.png`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/docs/Images/LCIAView.png` & `swolfpy-1.1.0/docs/Images/LCIAView.png`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/docs/Images/LoadProj.png` & `swolfpy-1.1.0/docs/Images/LoadProj.png`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/docs/Images/MC.png` & `swolfpy-1.1.0/docs/Images/MC.png`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/docs/Images/MCData.png` & `swolfpy-1.1.0/docs/Images/MCData.png`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/docs/Images/MCPlot.png` & `swolfpy-1.1.0/docs/Images/MCPlot.png`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/docs/Images/Opt.png` & `swolfpy-1.1.0/docs/Images/Opt.png`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/docs/Images/OptSet.png` & `swolfpy-1.1.0/docs/Images/OptSet.png`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/docs/Images/SWM_network.png` & `swolfpy-1.1.0/docs/Images/SWM_network.png`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/docs/Images/SetupLCA.png` & `swolfpy-1.1.0/docs/Images/SetupLCA.png`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/docs/Images/Start.png` & `swolfpy-1.1.0/docs/Images/Start.png`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/docs/Makefile` & `swolfpy-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/docs/conf.py` & `swolfpy-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/docs/doc_swolfpy.rst` & `swolfpy-1.1.0/docs/doc_swolfpy.rst`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/docs/make.bat` & `swolfpy-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/pyproject.toml` & `swolfpy-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "swolfpy"
 dynamic = ["version", "readme", "dependencies"]
 description = "Solid Waste Optimization Life-cycle Framework in Python(SwolfPy)."
 license = {text = "GNU GENERAL PUBLIC LICENSE V2"}
-requires-python = ">=3.10"
+requires-python = ">=3.9"
 authors = [
   {name = "Mojtaba Sardarmehni", email = "msardar2@alumni.ncsu.edu"},
 ]
 maintainers = [
   {name = "Mojtaba Sardarmehni", email = "msardar2@alumni.ncsu.edu"},
 ]
 keywords = [
@@ -23,15 +23,15 @@
 ]
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Education',
     'Intended Audience :: Science/Research',
     'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
     'Natural Language :: English',
-    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.9',
     'Operating System :: MacOS :: MacOS X',
     'Operating System :: Microsoft :: Windows',
     'Topic :: Scientific/Engineering :: Information Analysis',
     'Topic :: Scientific/Engineering :: Mathematics',
     'Topic :: Scientific/Engineering :: Visualization',
     'Natural Language :: English',
 ]
@@ -43,20 +43,22 @@
 
 [tool.setuptools.dynamic]
 version = {attr = "swolfpy.__version__"}
 readme = {file = ["README.rst", "HISTORY.rst"]}
 dependencies = {file = "requirements.txt"}
 
 [tool.setuptools]
-packages = ["swolfpy"]
 include-package-data = true
 
 [tool.setuptools.package-data]
 package_input_data = []
 
+[tool.setuptools.packages.find]
+include = ["swolfpy*"]
+
 [tool.black]
 line-length = 100
 preview = false
 
 [tool.isort]
 profile = "black"
 line_length = 100
```

### Comparing `swolfpy-1.0.1/swolfpy/LCA_matrix.py` & `swolfpy-1.1.0/swolfpy/LCA_matrix.py`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/swolfpy/Monte_Carlo.py` & `swolfpy-1.1.0/swolfpy/Monte_Carlo.py`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/swolfpy/Optimization.py` & `swolfpy-1.1.0/swolfpy/Optimization.py`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/swolfpy/Parameters.py` & `swolfpy-1.1.0/swolfpy/Parameters.py`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/swolfpy/ProcessDB.py` & `swolfpy-1.1.0/swolfpy/ProcessDB.py`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/swolfpy/Project.py` & `swolfpy-1.1.0/swolfpy/Project.py`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/swolfpy/Required_keys.py` & `swolfpy-1.1.0/swolfpy/Required_keys.py`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/swolfpy/Technosphere.py` & `swolfpy-1.1.0/swolfpy/Technosphere.py`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/swolfpy/__init__.py` & `swolfpy-1.1.0/swolfpy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "import_methods",
     "Optimization",
     "Monte_Carlo",
     "MyQtApp",
     "swolfpy",
 ]
 
-__version__ = "1.0.1"
+__version__ = "1.1.0"
 
 
 class swolfpy:
     def __init__(self):
         if not QtWidgets.QApplication.instance():
             self.app = QtWidgets.QApplication(sys.argv)
         else:
```

### Comparing `swolfpy-1.0.1/swolfpy/swolfpy_method.py` & `swolfpy-1.1.0/swolfpy/swolfpy_method.py`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/swolfpy/utils.py` & `swolfpy-1.1.0/swolfpy/utils.py`

 * *Files identical despite different names*

### Comparing `swolfpy-1.0.1/swolfpy.egg-info/PKG-INFO` & `swolfpy-1.1.0/swolfpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: swolfpy
-Version: 1.0.1
+Version: 1.1.0
 Summary: Solid Waste Optimization Life-cycle Framework in Python(SwolfPy).
 Author-email: Mojtaba Sardarmehni <msardar2@alumni.ncsu.edu>
 Maintainer-email: Mojtaba Sardarmehni <msardar2@alumni.ncsu.edu>
 License: GNU GENERAL PUBLIC LICENSE V2
 Project-URL: Homepage, https://swolfpy-project.github.io/
 Project-URL: Documentation, https://swolfpy.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/SwolfPy-Project/swolfpy
 Keywords: LCA,solid_waste,waste_management,swolfpy,brightway2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Natural Language :: English
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.md
 License-File: AUTHORS.rst
 
 .. General
 
 ================================================================
@@ -153,15 +153,15 @@
 
 2- Update conda in a terminal window or anaconda prompt::
 
         conda update conda
 
 3- Create a new environment for swolfpy::
 
-        conda create --name swolfpy python=3.10 graphviz
+        conda create --name swolfpy python=3.9 graphviz
 
 4- Add Graphviz executables to your system PATH (This step is optional; Enables plotting SWM network). You can find Graphviz executables in ``\\miniconda3\\envs\\swolfpy\\Library\\bin\\graphviz`` folder or search for ``dot.exe`` file in your system. Add the directory to the ``Path`` variable in your environment variables.
 
 5- Activate the environment::
 
         conda activate swolfpy
 
@@ -180,14 +180,21 @@
 
 .. endInstallation
 
 =======
 History
 =======
 
+1.1.0 (2023-07-30)
+------------------
+
+* Downgrade to Python 3.9
+
+
+
 1.0.0 (2023-06-03)
 ------------------
 
 * Upgrade to Python 3.10
 * Add PreCommit
```

### Comparing `swolfpy-1.0.1/swolfpy.egg-info/SOURCES.txt` & `swolfpy-1.1.0/swolfpy.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -35,35 +35,14 @@
 docs/Images/MCData.png
 docs/Images/MCPlot.png
 docs/Images/Opt.png
 docs/Images/OptSet.png
 docs/Images/SWM_network.png
 docs/Images/SetupLCA.png
 docs/Images/Start.png
-docs/_build/html/_images/AddCol.png
-docs/_build/html/_images/AddTreat.png
-docs/_build/html/_images/CreateScen.png
-docs/_build/html/_images/DefSys.png
-docs/_build/html/_images/IPM_CommonData.png
-docs/_build/html/_images/IPM_Tech.png
-docs/_build/html/_images/ImportPM.png
-docs/_build/html/_images/LCAContr.png
-docs/_build/html/_images/LCARes.png
-docs/_build/html/_images/LCA_LCI.png
-docs/_build/html/_images/LoadProj.png
-docs/_build/html/_images/MC.png
-docs/_build/html/_images/MCData.png
-docs/_build/html/_images/MCPlot.png
-docs/_build/html/_images/Opt.png
-docs/_build/html/_images/OptSet.png
-docs/_build/html/_images/SetupLCA.png
-docs/_build/html/_images/Start.png
-docs/_build/html/_static/file.png
-docs/_build/html/_static/minus.png
-docs/_build/html/_static/plus.png
 swolfpy/LCA_matrix.py
 swolfpy/Monte_Carlo.py
 swolfpy/Optimization.py
 swolfpy/Parameters.py
 swolfpy/ProcessDB.py
 swolfpy/Project.py
 swolfpy/Required_keys.py
@@ -72,10 +51,18 @@
 swolfpy/swolfpy_method.py
 swolfpy/utils.py
 swolfpy.egg-info/PKG-INFO
 swolfpy.egg-info/SOURCES.txt
 swolfpy.egg-info/dependency_links.txt
 swolfpy.egg-info/requires.txt
 swolfpy.egg-info/top_level.txt
-tests/.coverage
+swolfpy/UI/MC_ui.py
+swolfpy/UI/PySWOLF_run.py
+swolfpy/UI/PySWOLF_ui.py
+swolfpy/UI/PyWOLF_Resource_rc.py
+swolfpy/UI/Reference_ui.py
+swolfpy/UI/Table_from_pandas.py
+swolfpy/UI/Workers.py
+swolfpy/UI/__init__.py
+swolfpy/UI/adv_opt_ui.py
 tests/__init__.py
 tests/test_swolfpy.py
```

### Comparing `swolfpy-1.0.1/tests/test_swolfpy.py` & `swolfpy-1.1.0/tests/test_swolfpy.py`

 * *Files identical despite different names*

