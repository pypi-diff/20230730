# Comparing `tmp/swolfpy_inputdata-1.0.0.tar.gz` & `tmp/swolfpy_inputdata-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swolfpy_inputdata-1.0.0.tar", last modified: Sun Jun  4 17:38:05 2023, max compression
+gzip compressed data, was "C:\Users\msa75\Documents\Repos\github\swolfpy-inputdata\dist\.tmp-j_itrc7q\swolfpy_inputdata-1.1.0.tar", last modified: Sun Jul 30 16:13:53 2023, max compression
```

## Comparing `swolfpy_inputdata-1.0.0.tar` & `swolfpy_inputdata-1.1.0.tar`

### file list

```diff
@@ -1,93 +1,97 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 17:38:05.599866 swolfpy_inputdata-1.0.0/
--rw-rw-rw-   0        0        0      748 2023-06-04 17:34:09.000000 swolfpy_inputdata-1.0.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     1629 2022-11-26 02:47:46.000000 swolfpy_inputdata-1.0.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      739 2023-06-04 17:34:09.000000 swolfpy_inputdata-1.0.0/HISTORY.rst
--rw-rw-rw-   0        0        0    18431 2022-11-25 05:19:43.000000 swolfpy_inputdata-1.0.0/LICENSE.md
--rw-rw-rw-   0        0        0      319 2023-06-04 17:34:09.000000 swolfpy_inputdata-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     6878 2023-06-04 17:38:05.597895 swolfpy_inputdata-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4773 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/README.rst
--rw-rw-rw-   0        0        0    10351 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      109 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 17:38:05.599866 swolfpy_inputdata-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-04 17:38:04.698908 swolfpy_inputdata-1.0.0/swolfpy_inputdata/
--rw-rw-rw-   0        0        0      845 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/AD_Input.py
--rw-rw-rw-   0        0        0      896 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/AnF_Input.py
--rw-rw-rw-   0        0        0      904 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/COM_Col_Input.py
--rw-rw-rw-   0        0        0     3393 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/CommonData.py
--rw-rw-rw-   0        0        0      898 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/Comp_Input.py
--rw-rw-rw-   0        0        0      845 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/GC_Input.py
--rw-rw-rw-   0        0        0      897 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/HC_Input.py
--rw-rw-rw-   0        0        0     4142 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/InputData.py
--rw-rw-rw-   0        0        0     1505 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/LF_Input.py
--rw-rw-rw-   0        0        0     4213 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/MC.py
--rw-rw-rw-   0        0        0      900 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/MF_Col_Input.py
--rw-rw-rw-   0        0        0      851 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/RDF_Input.py
--rw-rw-rw-   0        0        0      537 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/Reproc_Input.py
--rw-rw-rw-   0        0        0      900 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/SF_Col_Input.py
--rw-rw-rw-   0        0        0      900 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/SS_MRF_Input.py
--rw-rw-rw-   0        0        0      574 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/TS_Input.py
--rw-rw-rw-   0        0        0     1400 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/Technosphere_Input.py
--rw-rw-rw-   0        0        0      849 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/WTE_Input.py
--rw-rw-rw-   0        0        0     1147 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 17:38:05.322090 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/
--rw-rw-rw-   0        0        0    13013 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/AD_Input.csv
--rw-rw-rw-   0        0        0     4069 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/AD_Input_MaterialDependent.csv
--rw-rw-rw-   0        0        0    13078 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/AnF_Input.csv
--rw-rw-rw-   0        0        0     1313 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/AnF_Input_MaterialDependent.csv
--rw-rw-rw-   0        0        0    11442 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/COM_Col_Input.csv
--rw-rw-rw-   0        0        0     2734 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/COM_Col_Input_MaterialDependent.csv
--rw-rw-rw-   0        0        0     5998 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/CommonData.csv
--rw-rw-rw-   0        0        0    10725 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/Comp_Input.csv
--rw-rw-rw-   0        0        0     4136 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/Comp_Input_MaterialDependent.csv
--rw-rw-rw-   0        0        0       75 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/Distance.csv
--rw-rw-rw-   0        0        0     3040 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/GC_Input.csv
--rw-rw-rw-   0        0        0     1023 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/GC_Input_MaterialDependent.csv
--rw-rw-rw-   0        0        0     1679 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/HC_Input.csv
--rw-rw-rw-   0        0        0     1739 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/HC_Input_MaterialDependent.csv
--rw-rw-rw-   0        0        0      505 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/LF_GasColPlan.csv
--rw-rw-rw-   0        0        0     8510 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/LF_Gas_emission_factors.csv
--rw-rw-rw-   0        0        0    10918 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/LF_Input.csv
--rw-rw-rw-   0        0        0     1239 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/LF_Input_MaterialDependent.csv
--rw-rw-rw-   0        0        0     5508 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/LF_Leachate_Quality.csv
--rw-rw-rw-   0        0        0    11011 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/MF_Col_Input.csv
--rw-rw-rw-   0        0        0     2614 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/MF_Col_Input_MaterialDependent.csv
--rw-rw-rw-   0        0        0    10890 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/Material properties.csv
--rw-rw-rw-   0        0        0    18551 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/RDF_Input.csv
--rw-rw-rw-   0        0        0     1635 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/RDF_Input_MaterialDependent.csv
--rw-rw-rw-   0        0        0     3343 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/References.csv
--rw-rw-rw-   0        0        0    53452 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/Reprocessing_Input.csv
--rw-rw-rw-   0        0        0    10939 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/SF_Col_Input.csv
--rw-rw-rw-   0        0        0     2821 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/SF_Col_Input_MaterialDependent.csv
--rw-rw-rw-   0        0        0    48925 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/SS_MRF_Input.csv
--rw-rw-rw-   0        0        0     3824 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/SS_MRF_Input_MaterialDependent.csv
--rw-rw-rw-   0        0        0     3206 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/TS_Input.csv
--rw-rw-rw-   0        0        0   781594 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/Technosphere_LCI.csv
--rw-rw-rw-   0        0        0     2126 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/Technosphere_References.csv
--rw-rw-rw-   0        0        0     5618 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/WTE_Input.csv
--rw-rw-rw-   0        0        0     2092 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/WTE_Input_MaterialDependent.csv
--rw-rw-rw-   0        0        0   230942 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/keys.csv
-drwxrwxrwx   0        0        0        0 2023-06-04 17:38:05.550862 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/
--rw-rw-rw-   0        0        0    13531 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('CML (v4.4) SwolfPy', 'resources', 'depletion of abiotic resources - elements, ultimate reserves').csv
--rw-rw-rw-   0        0        0    30907 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('IPCC 2007, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=0').csv
--rw-rw-rw-   0        0        0    30899 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('IPCC 2007, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=1').csv
--rw-rw-rw-   0        0        0    32831 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('IPCC 2013, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=0').csv
--rw-rw-rw-   0        0        0    32831 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('IPCC 2013, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=0, C1_36').csv
--rw-rw-rw-   0        0        0    32828 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('IPCC 2013, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=1').csv
--rw-rw-rw-   0        0        0    32828 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('IPCC 2013, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=1, C1_36').csv
--rw-rw-rw-   0        0        0      101 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('SwolfPy_Capital_Cost', 'SwolfPy').csv
--rw-rw-rw-   0        0        0      472 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('SwolfPy_Operational_Cost', 'SwolfPy').csv
--rw-rw-rw-   0        0        0      541 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('SwolfPy_Total_Cost', 'SwolfPy').csv
--rw-rw-rw-   0        0        0     5933 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('TRACI (2.1) SwolfPy', 'environmental impact', 'acidification').csv
--rw-rw-rw-   0        0        0     4899 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('TRACI (2.1) SwolfPy', 'environmental impact', 'eutrophication').csv
--rw-rw-rw-   0        0        0    16120 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('TRACI (2.1) SwolfPy', 'environmental impact', 'photochemical smog').csv
-drwxrwxrwx   0        0        0        0 2023-06-04 17:38:04.734859 swolfpy_inputdata-1.0.0/swolfpy_inputdata.egg-info/
--rw-rw-rw-   0        0        0     6878 2023-06-04 17:38:04.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3993 2023-06-04 17:38:04.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 17:38:04.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2023-06-04 17:38:04.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-04 17:38:04.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-04 17:38:05.594875 swolfpy_inputdata-1.0.0/tests/
--rw-rw-rw-   0        0        0      373 2022-11-26 05:55:39.000000 swolfpy_inputdata-1.0.0/tests/Test_Input.csv
--rw-rw-rw-   0        0        0       50 2022-11-25 05:49:34.000000 swolfpy_inputdata-1.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0     1811 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/tests/test_inputdata.py
--rw-rw-rw-   0        0        0      600 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/tests/test_inputs.py
+drwxrwxrwx   0        0        0        0 2023-07-30 16:13:53.000000 swolfpy_inputdata-1.1.0/
+-rw-rw-rw-   0        0        0      748 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1629 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      812 2023-07-30 15:37:05.000000 swolfpy_inputdata-1.1.0/HISTORY.rst
+-rw-rw-rw-   0        0        0    18431 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/LICENSE.md
+-rw-rw-rw-   0        0        0      319 2023-07-30 15:49:03.000000 swolfpy_inputdata-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6948 2023-07-30 16:13:53.000000 swolfpy_inputdata-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4772 2023-07-30 15:37:17.000000 swolfpy_inputdata-1.1.0/README.rst
+-rw-rw-rw-   0        0        0    10270 2023-07-30 15:55:52.000000 swolfpy_inputdata-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      109 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 16:13:53.000000 swolfpy_inputdata-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-30 16:13:53.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/
+-rw-rw-rw-   0        0        0      845 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/AD_Input.py
+-rw-rw-rw-   0        0        0      896 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/AnF_Input.py
+-rw-rw-rw-   0        0        0      904 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/COM_Col_Input.py
+-rw-rw-rw-   0        0        0     3393 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/CommonData.py
+-rw-rw-rw-   0        0        0      898 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/Comp_Input.py
+drwxrwxrwx   0        0        0        0 2023-07-30 16:13:53.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/Ecospold2/
+-rw-rw-rw-   0        0        0        0 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/Ecospold2/__init__.py
+-rw-rw-rw-   0        0        0      845 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/GC_Input.py
+-rw-rw-rw-   0        0        0      897 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/HC_Input.py
+-rw-rw-rw-   0        0        0     4142 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/InputData.py
+-rw-rw-rw-   0        0        0     1505 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/LF_Input.py
+-rw-rw-rw-   0        0        0     4213 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/MC.py
+-rw-rw-rw-   0        0        0      900 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/MF_Col_Input.py
+-rw-rw-rw-   0        0        0      851 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/RDF_Input.py
+-rw-rw-rw-   0        0        0      537 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/Reproc_Input.py
+-rw-rw-rw-   0        0        0      900 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/SF_Col_Input.py
+-rw-rw-rw-   0        0        0      900 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/SS_MRF_Input.py
+-rw-rw-rw-   0        0        0      574 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/TS_Input.py
+-rw-rw-rw-   0        0        0     1400 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/Technosphere_Input.py
+-rw-rw-rw-   0        0        0      849 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/WTE_Input.py
+-rw-rw-rw-   0        0        0     1147 2023-07-30 16:12:28.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 16:13:53.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/
+-rw-rw-rw-   0        0        0    13013 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/AD_Input.csv
+-rw-rw-rw-   0        0        0     4069 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/AD_Input_MaterialDependent.csv
+-rw-rw-rw-   0        0        0    13078 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/AnF_Input.csv
+-rw-rw-rw-   0        0        0     1313 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/AnF_Input_MaterialDependent.csv
+-rw-rw-rw-   0        0        0    11442 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/COM_Col_Input.csv
+-rw-rw-rw-   0        0        0     2734 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/COM_Col_Input_MaterialDependent.csv
+-rw-rw-rw-   0        0        0     5998 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/CommonData.csv
+-rw-rw-rw-   0        0        0    10725 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/Comp_Input.csv
+-rw-rw-rw-   0        0        0     4136 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/Comp_Input_MaterialDependent.csv
+-rw-rw-rw-   0        0        0       75 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/Distance.csv
+-rw-rw-rw-   0        0        0     3040 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/GC_Input.csv
+-rw-rw-rw-   0        0        0     1023 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/GC_Input_MaterialDependent.csv
+-rw-rw-rw-   0        0        0     1679 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/HC_Input.csv
+-rw-rw-rw-   0        0        0     1739 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/HC_Input_MaterialDependent.csv
+-rw-rw-rw-   0        0        0      505 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/LF_GasColPlan.csv
+-rw-rw-rw-   0        0        0     8510 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/LF_Gas_emission_factors.csv
+-rw-rw-rw-   0        0        0    10918 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/LF_Input.csv
+-rw-rw-rw-   0        0        0     1239 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/LF_Input_MaterialDependent.csv
+-rw-rw-rw-   0        0        0     5508 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/LF_Leachate_Quality.csv
+-rw-rw-rw-   0        0        0    11011 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/MF_Col_Input.csv
+-rw-rw-rw-   0        0        0     2614 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/MF_Col_Input_MaterialDependent.csv
+-rw-rw-rw-   0        0        0    10890 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/Material properties.csv
+-rw-rw-rw-   0        0        0    18551 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/RDF_Input.csv
+-rw-rw-rw-   0        0        0     1635 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/RDF_Input_MaterialDependent.csv
+-rw-rw-rw-   0        0        0     3343 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/References.csv
+-rw-rw-rw-   0        0        0    53452 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/Reprocessing_Input.csv
+-rw-rw-rw-   0        0        0    10939 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/SF_Col_Input.csv
+-rw-rw-rw-   0        0        0     2821 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/SF_Col_Input_MaterialDependent.csv
+-rw-rw-rw-   0        0        0    48925 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/SS_MRF_Input.csv
+-rw-rw-rw-   0        0        0     3824 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/SS_MRF_Input_MaterialDependent.csv
+-rw-rw-rw-   0        0        0     3206 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/TS_Input.csv
+-rw-rw-rw-   0        0        0   781594 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/Technosphere_LCI.csv
+-rw-rw-rw-   0        0        0     2126 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/Technosphere_References.csv
+-rw-rw-rw-   0        0        0     5618 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/WTE_Input.csv
+-rw-rw-rw-   0        0        0     2092 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/WTE_Input_MaterialDependent.csv
+-rw-rw-rw-   0        0        0        0 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/__init__.py
+-rw-rw-rw-   0        0        0   230942 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/keys.csv
+drwxrwxrwx   0        0        0        0 2023-07-30 16:13:53.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/lcia_methods/
+-rw-rw-rw-   0        0        0    13531 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/lcia_methods/('CML (v4.4) SwolfPy', 'resources', 'depletion of abiotic resources - elements, ultimate reserves').csv
+-rw-rw-rw-   0        0        0    30907 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/lcia_methods/('IPCC 2007, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=0').csv
+-rw-rw-rw-   0        0        0    30899 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/lcia_methods/('IPCC 2007, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=1').csv
+-rw-rw-rw-   0        0        0    32831 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/lcia_methods/('IPCC 2013, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=0').csv
+-rw-rw-rw-   0        0        0    32831 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/lcia_methods/('IPCC 2013, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=0, C1_36').csv
+-rw-rw-rw-   0        0        0    32828 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/lcia_methods/('IPCC 2013, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=1').csv
+-rw-rw-rw-   0        0        0    32828 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/lcia_methods/('IPCC 2013, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=1, C1_36').csv
+-rw-rw-rw-   0        0        0      101 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/lcia_methods/('SwolfPy_Capital_Cost', 'SwolfPy').csv
+-rw-rw-rw-   0        0        0      472 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/lcia_methods/('SwolfPy_Operational_Cost', 'SwolfPy').csv
+-rw-rw-rw-   0        0        0      541 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/lcia_methods/('SwolfPy_Total_Cost', 'SwolfPy').csv
+-rw-rw-rw-   0        0        0     5933 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/lcia_methods/('TRACI (2.1) SwolfPy', 'environmental impact', 'acidification').csv
+-rw-rw-rw-   0        0        0     4899 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/lcia_methods/('TRACI (2.1) SwolfPy', 'environmental impact', 'eutrophication').csv
+-rw-rw-rw-   0        0        0    16120 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/lcia_methods/('TRACI (2.1) SwolfPy', 'environmental impact', 'photochemical smog').csv
+-rw-rw-rw-   0        0        0        0 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/lcia_methods/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 16:13:53.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata.egg-info/
+-rw-rw-rw-   0        0        0     6948 2023-07-30 16:13:53.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4116 2023-07-30 16:13:53.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 16:13:53.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2023-07-30 16:13:53.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-30 16:13:53.000000 swolfpy_inputdata-1.1.0/swolfpy_inputdata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 16:13:53.000000 swolfpy_inputdata-1.1.0/tests/
+-rw-rw-rw-   0        0        0      373 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/tests/Test_Input.csv
+-rw-rw-rw-   0        0        0       50 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     1811 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/tests/test_inputdata.py
+-rw-rw-rw-   0        0        0      600 2023-06-20 02:21:39.000000 swolfpy_inputdata-1.1.0/tests/test_inputs.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `swolfpy_inputdata-1.0.0/AUTHORS.rst` & `swolfpy_inputdata-1.1.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/CONTRIBUTING.rst` & `swolfpy_inputdata-1.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/HISTORY.rst` & `swolfpy_inputdata-1.1.0/HISTORY.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =======
 History
 =======
 
+1.1.0 (2023-07-30)
+------------------
+
+* Downgrade to Python 3.9
+
+
 1.0.0 (2023-06-03)
 ------------------
 
 * Upgrade to Python 3.10
 * Add PreCommit
```

### Comparing `swolfpy_inputdata-1.0.0/LICENSE.md` & `swolfpy_inputdata-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/PKG-INFO` & `swolfpy_inputdata-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: swolfpy_inputdata
-Version: 1.0.0
+Version: 1.1.0
 Summary: Input data for swolfpy's life-cycle process models (swolfpy_inputdata).
 Author-email: Mojtaba Sardarmehni <msardar2@alumni.ncsu.edu>
 Maintainer-email: Mojtaba Sardarmehni <msardar2@alumni.ncsu.edu>
 License: GNU GENERAL PUBLIC LICENSE V2
 Project-URL: Homepage, https://swolfpy-project.github.io/
 Project-URL: Documentation, https://swolfpy.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/SwolfPy-Project/swolfpy-inputdata
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
 
 ======================================================================
@@ -139,15 +139,15 @@
 
 2- Update conda in a terminal window or anaconda prompt::
 
         conda update conda
 
 3- Create a new environment for swolfpy::
 
-        conda create --name swolfpy python=3.10
+        conda create --name swolfpy python=3.9
 
 4- Activate the environment::
 
         conda activate swolfpy
 
 5- Install swolfpy_inputdata in the environment::
 
@@ -165,14 +165,20 @@
 
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
 1.0.0 (2023-06-03)
 ------------------
 
 * Upgrade to Python 3.10
 * Add PreCommit
```

### Comparing `swolfpy_inputdata-1.0.0/README.rst` & `swolfpy_inputdata-1.1.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
 2- Update conda in a terminal window or anaconda prompt::
 
         conda update conda
 
 3- Create a new environment for swolfpy::
 
-        conda create --name swolfpy python=3.10
+        conda create --name swolfpy python=3.9
 
 4- Activate the environment::
 
         conda activate swolfpy
 
 5- Install swolfpy_inputdata in the environment::
```

### Comparing `swolfpy_inputdata-1.0.0/pyproject.toml` & `swolfpy_inputdata-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,633 +15,628 @@
 000000e0: 2d63 7963 6c65 2070 726f 6365 7373 206d  -cycle process m
 000000f0: 6f64 656c 7320 2873 776f 6c66 7079 5f69  odels (swolfpy_i
 00000100: 6e70 7574 6461 7461 292e 220d 0a6c 6963  nputdata)."..lic
 00000110: 656e 7365 203d 207b 7465 7874 203d 2022  ense = {text = "
 00000120: 474e 5520 4745 4e45 5241 4c20 5055 424c  GNU GENERAL PUBL
 00000130: 4943 204c 4943 454e 5345 2056 3222 7d0d  IC LICENSE V2"}.
 00000140: 0a72 6571 7569 7265 732d 7079 7468 6f6e  .requires-python
-00000150: 203d 2022 3e3d 332e 3130 220d 0a61 7574   = ">=3.10"..aut
-00000160: 686f 7273 203d 205b 0d0a 2020 7b6e 616d  hors = [..  {nam
-00000170: 6520 3d20 224d 6f6a 7461 6261 2053 6172  e = "Mojtaba Sar
-00000180: 6461 726d 6568 6e69 222c 2065 6d61 696c  darmehni", email
-00000190: 203d 2022 6d73 6172 6461 7232 4061 6c75   = "msardar2@alu
-000001a0: 6d6e 692e 6e63 7375 2e65 6475 227d 2c0d  mni.ncsu.edu"},.
-000001b0: 0a5d 0d0a 6d61 696e 7461 696e 6572 7320  .]..maintainers 
-000001c0: 3d20 5b0d 0a20 207b 6e61 6d65 203d 2022  = [..  {name = "
-000001d0: 4d6f 6a74 6162 6120 5361 7264 6172 6d65  Mojtaba Sardarme
-000001e0: 686e 6922 2c20 656d 6169 6c20 3d20 226d  hni", email = "m
-000001f0: 7361 7264 6172 3240 616c 756d 6e69 2e6e  sardar2@alumni.n
-00000200: 6373 752e 6564 7522 7d2c 0d0a 5d0d 0a6b  csu.edu"},..]..k
-00000210: 6579 776f 7264 7320 3d20 5b0d 0a20 2020  eywords = [..   
-00000220: 2022 4c43 4122 2c0d 0a20 2020 2022 736f   "LCA",..    "so
-00000230: 6c69 645f 7761 7374 6522 2c0d 0a20 2020  lid_waste",..   
-00000240: 2022 7761 7374 655f 6d61 6e61 6765 6d65   "waste_manageme
-00000250: 6e74 222c 0d0a 2020 2020 2273 776f 6c66  nt",..    "swolf
-00000260: 7079 222c 0d0a 2020 2020 2262 7269 6768  py",..    "brigh
-00000270: 7477 6179 3222 2c0d 0a5d 0d0a 636c 6173  tway2",..]..clas
-00000280: 7369 6669 6572 7320 3d20 5b0d 0a20 2020  sifiers = [..   
-00000290: 2027 4465 7665 6c6f 706d 656e 7420 5374   'Development St
-000002a0: 6174 7573 203a 3a20 3520 2d20 5072 6f64  atus :: 5 - Prod
-000002b0: 7563 7469 6f6e 2f53 7461 626c 6527 2c0d  uction/Stable',.
-000002c0: 0a20 2020 2027 496e 7465 6e64 6564 2041  .    'Intended A
-000002d0: 7564 6965 6e63 6520 3a3a 2045 6475 6361  udience :: Educa
-000002e0: 7469 6f6e 272c 0d0a 2020 2020 2749 6e74  tion',..    'Int
-000002f0: 656e 6465 6420 4175 6469 656e 6365 203a  ended Audience :
-00000300: 3a20 5363 6965 6e63 652f 5265 7365 6172  : Science/Resear
-00000310: 6368 272c 0d0a 2020 2020 274c 6963 656e  ch',..    'Licen
-00000320: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
-00000330: 6564 203a 3a20 474e 5520 4765 6e65 7261  ed :: GNU Genera
-00000340: 6c20 5075 626c 6963 204c 6963 656e 7365  l Public License
-00000350: 2076 3220 2847 504c 7632 2927 2c0d 0a20   v2 (GPLv2)',.. 
-00000360: 2020 2027 4e61 7475 7261 6c20 4c61 6e67     'Natural Lang
-00000370: 7561 6765 203a 3a20 456e 676c 6973 6827  uage :: English'
-00000380: 2c0d 0a20 2020 2027 5072 6f67 7261 6d6d  ,..    'Programm
-00000390: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000003a0: 5079 7468 6f6e 203a 3a20 332e 3130 272c  Python :: 3.10',
-000003b0: 0d0a 2020 2020 274f 7065 7261 7469 6e67  ..    'Operating
-000003c0: 2053 7973 7465 6d20 3a3a 204d 6163 4f53   System :: MacOS
-000003d0: 203a 3a20 4d61 634f 5320 5827 2c0d 0a20   :: MacOS X',.. 
-000003e0: 2020 2027 4f70 6572 6174 696e 6720 5379     'Operating Sy
-000003f0: 7374 656d 203a 3a20 4d69 6372 6f73 6f66  stem :: Microsof
-00000400: 7420 3a3a 2057 696e 646f 7773 272c 0d0a  t :: Windows',..
-00000410: 2020 2020 2754 6f70 6963 203a 3a20 5363      'Topic :: Sc
-00000420: 6965 6e74 6966 6963 2f45 6e67 696e 6565  ientific/Enginee
-00000430: 7269 6e67 203a 3a20 496e 666f 726d 6174  ring :: Informat
-00000440: 696f 6e20 416e 616c 7973 6973 272c 0d0a  ion Analysis',..
-00000450: 2020 2020 2754 6f70 6963 203a 3a20 5363      'Topic :: Sc
-00000460: 6965 6e74 6966 6963 2f45 6e67 696e 6565  ientific/Enginee
-00000470: 7269 6e67 203a 3a20 4d61 7468 656d 6174  ring :: Mathemat
-00000480: 6963 7327 2c0d 0a20 2020 2027 546f 7069  ics',..    'Topi
-00000490: 6320 3a3a 2053 6369 656e 7469 6669 632f  c :: Scientific/
-000004a0: 456e 6769 6e65 6572 696e 6720 3a3a 2056  Engineering :: V
-000004b0: 6973 7561 6c69 7a61 7469 6f6e 272c 0d0a  isualization',..
-000004c0: 2020 2020 274e 6174 7572 616c 204c 616e      'Natural Lan
-000004d0: 6775 6167 6520 3a3a 2045 6e67 6c69 7368  guage :: English
-000004e0: 272c 0d0a 5d0d 0a0d 0a5b 7072 6f6a 6563  ',..]....[projec
-000004f0: 742e 7572 6c73 5d0d 0a48 6f6d 6570 6167  t.urls]..Homepag
-00000500: 6520 3d20 2268 7474 7073 3a2f 2f73 776f  e = "https://swo
-00000510: 6c66 7079 2d70 726f 6a65 6374 2e67 6974  lfpy-project.git
-00000520: 6875 622e 696f 2f22 0d0a 446f 6375 6d65  hub.io/"..Docume
-00000530: 6e74 6174 696f 6e20 3d20 2268 7474 7073  ntation = "https
-00000540: 3a2f 2f73 776f 6c66 7079 2e72 6561 6474  ://swolfpy.readt
-00000550: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
-00000560: 6573 742f 220d 0a22 536f 7572 6365 2043  est/".."Source C
-00000570: 6f64 6522 203d 2022 6874 7470 733a 2f2f  ode" = "https://
-00000580: 6769 7468 7562 2e63 6f6d 2f53 776f 6c66  github.com/Swolf
-00000590: 5079 2d50 726f 6a65 6374 2f73 776f 6c66  Py-Project/swolf
-000005a0: 7079 2d69 6e70 7574 6461 7461 220d 0a0d  py-inputdata"...
-000005b0: 0a5b 746f 6f6c 2e73 6574 7570 746f 6f6c  .[tool.setuptool
-000005c0: 732e 6479 6e61 6d69 635d 0d0a 7665 7273  s.dynamic]..vers
-000005d0: 696f 6e20 3d20 7b61 7474 7220 3d20 2273  ion = {attr = "s
-000005e0: 776f 6c66 7079 5f69 6e70 7574 6461 7461  wolfpy_inputdata
-000005f0: 2e5f 5f76 6572 7369 6f6e 5f5f 227d 0d0a  .__version__"}..
-00000600: 7265 6164 6d65 203d 207b 6669 6c65 203d  readme = {file =
-00000610: 205b 2252 4541 444d 452e 7273 7422 2c20   ["README.rst", 
-00000620: 2248 4953 544f 5259 2e72 7374 225d 7d0d  "HISTORY.rst"]}.
-00000630: 0a64 6570 656e 6465 6e63 6965 7320 3d20  .dependencies = 
-00000640: 7b66 696c 6520 3d20 2272 6571 7569 7265  {file = "require
-00000650: 6d65 6e74 732e 7478 7422 7d0d 0a0d 0a5b  ments.txt"}....[
-00000660: 746f 6f6c 2e73 6574 7570 746f 6f6c 735d  tool.setuptools]
-00000670: 0d0a 7061 636b 6167 6573 203d 205b 2273  ..packages = ["s
-00000680: 776f 6c66 7079 5f69 6e70 7574 6461 7461  wolfpy_inputdata
-00000690: 225d 0d0a 696e 636c 7564 652d 7061 636b  "]..include-pack
-000006a0: 6167 652d 6461 7461 203d 2074 7275 650d  age-data = true.
-000006b0: 0a0d 0a5b 746f 6f6c 2e73 6574 7570 746f  ...[tool.setupto
-000006c0: 6f6c 732e 7061 636b 6167 652d 6461 7461  ols.package-data
-000006d0: 5d0d 0a70 6163 6b61 6765 5f69 6e70 7574  ]..package_input
-000006e0: 5f64 6174 6120 3d20 5b0d 0a20 2020 2022  _data = [..    "
-000006f0: 6461 7461 2f2a 2e63 7376 222c 0d0a 2020  data/*.csv",..  
-00000700: 2020 2264 6174 612f 6c63 6961 5f6d 6574    "data/lcia_met
-00000710: 686f 6473 2f2a 2e63 7376 222c 0d0a 2020  hods/*.csv",..  
-00000720: 2020 5d0d 0a0d 0a5b 746f 6f6c 2e62 6c61    ]....[tool.bla
-00000730: 636b 5d0d 0a6c 696e 652d 6c65 6e67 7468  ck]..line-length
-00000740: 203d 2031 3030 0d0a 7072 6576 6965 7720   = 100..preview 
-00000750: 3d20 6661 6c73 650d 0a0d 0a5b 746f 6f6c  = false....[tool
-00000760: 2e69 736f 7274 5d0d 0a70 726f 6669 6c65  .isort]..profile
-00000770: 203d 2022 626c 6163 6b22 0d0a 6c69 6e65   = "black"..line
-00000780: 5f6c 656e 6774 6820 3d20 3130 300d 0a0d  _length = 100...
-00000790: 0a5b 746f 6f6c 2e70 7974 6573 742e 696e  .[tool.pytest.in
-000007a0: 695f 6f70 7469 6f6e 735d 0d0a 6d69 6e76  i_options]..minv
-000007b0: 6572 7369 6f6e 203d 2037 2e30 0d0a 7465  ersion = 7.0..te
-000007c0: 7374 7061 7468 7320 3d20 5b0d 0a20 2022  stpaths = [..  "
-000007d0: 7465 7374 7322 0d0a 5d0d 0a70 7974 686f  tests"..]..pytho
-000007e0: 6e5f 6669 6c65 7320 3d20 5b20 2023 2061  n_files = [  # a
-000007f0: 206c 6973 7420 6f66 2070 6174 7465 726e   list of pattern
-00000800: 7320 746f 2075 7365 2074 6f20 636f 6c6c  s to use to coll
-00000810: 6563 7420 7465 7374 206d 6f64 756c 6573  ect test modules
-00000820: 0d0a 2020 2274 6573 7473 2f74 6573 745f  ..  "tests/test_
-00000830: 2a2e 7079 220d 0a5d 0d0a 6164 646f 7074  *.py"..]..addopt
-00000840: 7320 3d20 222d 2d63 6f76 3d73 776f 6c66  s = "--cov=swolf
-00000850: 7079 5f69 6e70 7574 6461 7461 202d 2d63  py_inputdata --c
-00000860: 6f76 2d72 6570 6f72 743d 786d 6c20 2d2d  ov-report=xml --
-00000870: 6469 7361 626c 652d 7761 726e 696e 6773  disable-warnings
-00000880: 202d 2d69 676e 6f72 6520 2a2e 6373 7620   --ignore *.csv 
-00000890: 2d2d 636f 6c6f 723d 7965 7322 0d0a 0d0a  --color=yes"....
-000008a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000008b0: 2323 2323 2323 2323 2323 2323 230d 0a23  #############..#
-000008c0: 2323 2323 2323 2020 2020 7079 6c69 6e74  ######    pylint
-000008d0: 2020 2020 2023 2323 2323 2323 0d0a 2323       #######..##
-000008e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000008f0: 2323 2323 2323 2323 2323 230d 0a23 2053  ###########..# S
-00000900: 6f75 7263 6520 666f 7220 7079 6c69 6e74  ource for pylint
-00000910: 2073 6574 7469 6e67 733a 2068 7474 7073   settings: https
-00000920: 3a2f 2f67 6974 6875 622e 636f 6d2f 5079  ://github.com/Py
-00000930: 4351 412f 7079 6c69 6e74 2f62 6c6f 622f  CQA/pylint/blob/
-00000940: 6d61 696e 2f65 7861 6d70 6c65 732f 7079  main/examples/py
-00000950: 7072 6f6a 6563 742e 746f 6d6c 0d0a 0d0a  project.toml....
-00000960: 5b74 6f6f 6c2e 7079 6c69 6e74 2e6d 6169  [tool.pylint.mai
-00000970: 6e5d 0d0a 2320 5370 6563 6966 7920 6120  n]..# Specify a 
-00000980: 7363 6f72 6520 7468 7265 7368 6f6c 6420  score threshold 
-00000990: 756e 6465 7220 7768 6963 6820 7468 6520  under which the 
-000009a0: 7072 6f67 7261 6d20 7769 6c6c 2065 7869  program will exi
-000009b0: 7420 7769 7468 2065 7272 6f72 2e0d 0a66  t with error...f
-000009c0: 6169 6c2d 756e 6465 7220 3d20 3130 0d0a  ail-under = 10..
-000009d0: 0d0a 2320 4669 6c65 7320 6f72 2064 6972  ..# Files or dir
-000009e0: 6563 746f 7269 6573 2074 6f20 6265 2073  ectories to be s
-000009f0: 6b69 7070 6564 2e20 5468 6579 2073 686f  kipped. They sho
-00000a00: 756c 6420 6265 2062 6173 6520 6e61 6d65  uld be base name
-00000a10: 732c 206e 6f74 2070 6174 6873 2e0d 0a69  s, not paths...i
-00000a20: 676e 6f72 6520 3d20 5b22 4356 5322 5d0d  gnore = ["CVS"].
-00000a30: 0a0d 0a23 2041 6464 2066 696c 6573 206f  ...# Add files o
-00000a40: 7220 6469 7265 6374 6f72 6965 7320 6d61  r directories ma
-00000a50: 7463 6869 6e67 2074 6865 2072 6567 756c  tching the regul
-00000a60: 6172 2065 7870 7265 7373 696f 6e73 2070  ar expressions p
-00000a70: 6174 7465 726e 7320 746f 2074 6865 0d0a  atterns to the..
-00000a80: 2320 6967 6e6f 7265 2d6c 6973 742e 2054  # ignore-list. T
-00000a90: 6865 2072 6567 6578 206d 6174 6368 6573  he regex matches
-00000aa0: 2061 6761 696e 7374 2070 6174 6873 2061   against paths a
-00000ab0: 6e64 2063 616e 2062 6520 696e 2050 6f73  nd can be in Pos
-00000ac0: 6978 206f 7220 5769 6e64 6f77 730d 0a23  ix or Windows..#
-00000ad0: 2066 6f72 6d61 742e 2042 6563 6175 7365   format. Because
-00000ae0: 2027 5c27 2072 6570 7265 7365 6e74 7320   '\' represents 
-00000af0: 7468 6520 6469 7265 6374 6f72 7920 6465  the directory de
-00000b00: 6c69 6d69 7465 7220 6f6e 2057 696e 646f  limiter on Windo
-00000b10: 7773 2073 7973 7465 6d73 2c20 6974 0d0a  ws systems, it..
-00000b20: 2320 6361 6e27 7420 6265 2075 7365 6420  # can't be used 
-00000b30: 6173 2061 6e20 6573 6361 7065 2063 6861  as an escape cha
-00000b40: 7261 6374 6572 2e0d 0a23 2069 676e 6f72  racter...# ignor
-00000b50: 652d 7061 7468 7320 3d0d 0a0d 0a23 2046  e-paths =....# F
-00000b60: 696c 6573 206f 7220 6469 7265 6374 6f72  iles or director
-00000b70: 6965 7320 6d61 7463 6869 6e67 2074 6865  ies matching the
-00000b80: 2072 6567 756c 6172 2065 7870 7265 7373   regular express
-00000b90: 696f 6e20 7061 7474 6572 6e73 2061 7265  ion patterns are
-00000ba0: 2073 6b69 7070 6564 2e20 5468 650d 0a23   skipped. The..#
-00000bb0: 2072 6567 6578 206d 6174 6368 6573 2061   regex matches a
-00000bc0: 6761 696e 7374 2062 6173 6520 6e61 6d65  gainst base name
-00000bd0: 732c 206e 6f74 2070 6174 6873 2e20 5468  s, not paths. Th
-00000be0: 6520 6465 6661 756c 7420 7661 6c75 6520  e default value 
-00000bf0: 6967 6e6f 7265 7320 456d 6163 730d 0a23  ignores Emacs..#
-00000c00: 2066 696c 6520 6c6f 636b 730d 0a69 676e   file locks..ign
-00000c10: 6f72 652d 7061 7474 6572 6e73 203d 205b  ore-patterns = [
-00000c20: 225e 5c5c 2e23 225d 0d0a 0d0a 2320 4c69  "^\\.#"]....# Li
-00000c30: 7374 206f 6620 6d6f 6475 6c65 206e 616d  st of module nam
-00000c40: 6573 2066 6f72 2077 6869 6368 206d 656d  es for which mem
-00000c50: 6265 7220 6174 7472 6962 7574 6573 2073  ber attributes s
-00000c60: 686f 756c 6420 6e6f 7420 6265 2063 6865  hould not be che
-00000c70: 636b 6564 2028 7573 6566 756c 0d0a 2320  cked (useful..# 
-00000c80: 666f 7220 6d6f 6475 6c65 732f 7072 6f6a  for modules/proj
-00000c90: 6563 7473 2077 6865 7265 206e 616d 6573  ects where names
-00000ca0: 7061 6365 7320 6172 6520 6d61 6e69 7075  paces are manipu
-00000cb0: 6c61 7465 6420 6475 7269 6e67 2072 756e  lated during run
-00000cc0: 7469 6d65 2061 6e64 2074 6875 730d 0a23  time and thus..#
-00000cd0: 2065 7869 7374 696e 6720 6d65 6d62 6572   existing member
-00000ce0: 2061 7474 7269 6275 7465 7320 6361 6e6e   attributes cann
-00000cf0: 6f74 2062 6520 6465 6475 6365 6420 6279  ot be deduced by
-00000d00: 2073 7461 7469 6320 616e 616c 7973 6973   static analysis
-00000d10: 292e 2049 7420 7375 7070 6f72 7473 0d0a  ). It supports..
-00000d20: 2320 7175 616c 6966 6965 6420 6d6f 6475  # qualified modu
-00000d30: 6c65 206e 616d 6573 2c20 6173 2077 656c  le names, as wel
-00000d40: 6c20 6173 2055 6e69 7820 7061 7474 6572  l as Unix patter
-00000d50: 6e20 6d61 7463 6869 6e67 2e0d 0a23 2069  n matching...# i
-00000d60: 676e 6f72 6564 2d6d 6f64 756c 6573 203d  gnored-modules =
-00000d70: 0d0a 0d0a 2320 5573 6520 6d75 6c74 6970  ....# Use multip
-00000d80: 6c65 2070 726f 6365 7373 6573 2074 6f20  le processes to 
-00000d90: 7370 6565 6420 7570 2050 796c 696e 742e  speed up Pylint.
-00000da0: 2053 7065 6369 6679 696e 6720 3020 7769   Specifying 0 wi
-00000db0: 6c6c 2061 7574 6f2d 6465 7465 6374 2074  ll auto-detect t
-00000dc0: 6865 0d0a 2320 6e75 6d62 6572 206f 6620  he..# number of 
-00000dd0: 7072 6f63 6573 736f 7273 2061 7661 696c  processors avail
-00000de0: 6162 6c65 2074 6f20 7573 652c 2061 6e64  able to use, and
-00000df0: 2077 696c 6c20 6361 7020 7468 6520 636f   will cap the co
-00000e00: 756e 7420 6f6e 2057 696e 646f 7773 2074  unt on Windows t
-00000e10: 6f0d 0a23 2061 766f 6964 2068 616e 6773  o..# avoid hangs
-00000e20: 2e0d 0a6a 6f62 7320 3d20 320d 0a0d 0a23  ...jobs = 2....#
-00000e30: 2043 6f6e 7472 6f6c 2074 6865 2061 6d6f   Control the amo
-00000e40: 756e 7420 6f66 2070 6f74 656e 7469 616c  unt of potential
-00000e50: 2069 6e66 6572 7265 6420 7661 6c75 6573   inferred values
-00000e60: 2077 6865 6e20 696e 6665 7272 696e 6720   when inferring 
-00000e70: 6120 7369 6e67 6c65 206f 626a 6563 742e  a single object.
-00000e80: 0d0a 2320 5468 6973 2063 616e 2068 656c  ..# This can hel
-00000e90: 7020 7468 6520 7065 7266 6f72 6d61 6e63  p the performanc
-00000ea0: 6520 7768 656e 2064 6561 6c69 6e67 2077  e when dealing w
-00000eb0: 6974 6820 6c61 7267 6520 6675 6e63 7469  ith large functi
-00000ec0: 6f6e 7320 6f72 2063 6f6d 706c 6578 2c0d  ons or complex,.
-00000ed0: 0a23 206e 6573 7465 6420 636f 6e64 6974  .# nested condit
-00000ee0: 696f 6e73 2e0d 0a6c 696d 6974 2d69 6e66  ions...limit-inf
-00000ef0: 6572 656e 6365 2d72 6573 756c 7473 203d  erence-results =
-00000f00: 2031 3030 0d0a 0d0a 2320 5069 636b 6c65   100....# Pickle
-00000f10: 2063 6f6c 6c65 6374 6564 2064 6174 6120   collected data 
-00000f20: 666f 7220 6c61 7465 7220 636f 6d70 6172  for later compar
-00000f30: 6973 6f6e 732e 0d0a 7065 7273 6973 7465  isons...persiste
-00000f40: 6e74 203d 2074 7275 650d 0a0d 0a23 2057  nt = true....# W
-00000f50: 6865 6e20 656e 6162 6c65 642c 2070 796c  hen enabled, pyl
-00000f60: 696e 7420 776f 756c 6420 6174 7465 6d70  int would attemp
-00000f70: 7420 746f 2067 7565 7373 2063 6f6d 6d6f  t to guess commo
-00000f80: 6e20 6d69 7363 6f6e 6669 6775 7261 7469  n misconfigurati
-00000f90: 6f6e 2061 6e64 2065 6d69 740d 0a23 2075  on and emit..# u
-00000fa0: 7365 722d 6672 6965 6e64 6c79 2068 696e  ser-friendly hin
-00000fb0: 7473 2069 6e73 7465 6164 206f 6620 6661  ts instead of fa
-00000fc0: 6c73 652d 706f 7369 7469 7665 2065 7272  lse-positive err
-00000fd0: 6f72 206d 6573 7361 6765 732e 0d0a 7375  or messages...su
-00000fe0: 6767 6573 7469 6f6e 2d6d 6f64 6520 3d20  ggestion-mode = 
-00000ff0: 7472 7565 0d0a 0d0a 5b74 6f6f 6c2e 7079  true....[tool.py
-00001000: 6c69 6e74 2e62 6173 6963 5d0d 0a23 204e  lint.basic]..# N
-00001010: 616d 696e 6720 7374 796c 6520 6d61 7463  aming style matc
-00001020: 6869 6e67 2063 6f72 7265 6374 2061 7267  hing correct arg
-00001030: 756d 656e 7420 6e61 6d65 732e 0d0a 6172  ument names...ar
-00001040: 6775 6d65 6e74 2d6e 616d 696e 672d 7374  gument-naming-st
-00001050: 796c 6520 3d20 2273 6e61 6b65 5f63 6173  yle = "snake_cas
-00001060: 6522 0d0a 0d0a 2320 4e61 6d69 6e67 2073  e"....# Naming s
-00001070: 7479 6c65 206d 6174 6368 696e 6720 636f  tyle matching co
-00001080: 7272 6563 7420 6174 7472 6962 7574 6520  rrect attribute 
-00001090: 6e61 6d65 732e 0d0a 6174 7472 2d6e 616d  names...attr-nam
-000010a0: 696e 672d 7374 796c 6520 3d20 2273 6e61  ing-style = "sna
-000010b0: 6b65 5f63 6173 6522 0d0a 0d0a 2320 4261  ke_case"....# Ba
-000010c0: 6420 7661 7269 6162 6c65 206e 616d 6573  d variable names
-000010d0: 2077 6869 6368 2073 686f 756c 6420 616c   which should al
-000010e0: 7761 7973 2062 6520 7265 6675 7365 642c  ways be refused,
-000010f0: 2073 6570 6172 6174 6564 2062 7920 6120   separated by a 
-00001100: 636f 6d6d 612e 0d0a 6261 642d 6e61 6d65  comma...bad-name
-00001110: 7320 3d20 5b22 666f 6f22 2c20 2262 6172  s = ["foo", "bar
-00001120: 222c 2022 6261 7a22 2c20 2274 6f74 6f22  ", "baz", "toto"
-00001130: 2c20 2274 7574 7522 2c20 2274 6174 6122  , "tutu", "tata"
-00001140: 5d0d 0a0d 0a23 204e 616d 696e 6720 7374  ]....# Naming st
-00001150: 796c 6520 6d61 7463 6869 6e67 2063 6f72  yle matching cor
-00001160: 7265 6374 2063 6c61 7373 2061 7474 7269  rect class attri
-00001170: 6275 7465 206e 616d 6573 2e0d 0a63 6c61  bute names...cla
-00001180: 7373 2d61 7474 7269 6275 7465 2d6e 616d  ss-attribute-nam
-00001190: 696e 672d 7374 796c 6520 3d20 2261 6e79  ing-style = "any
-000011a0: 220d 0a0d 0a23 204e 616d 696e 6720 7374  "....# Naming st
-000011b0: 796c 6520 6d61 7463 6869 6e67 2063 6f72  yle matching cor
-000011c0: 7265 6374 2063 6c61 7373 2063 6f6e 7374  rect class const
-000011d0: 616e 7420 6e61 6d65 732e 0d0a 636c 6173  ant names...clas
-000011e0: 732d 636f 6e73 742d 6e61 6d69 6e67 2d73  s-const-naming-s
-000011f0: 7479 6c65 203d 2022 5550 5045 525f 4341  tyle = "UPPER_CA
-00001200: 5345 220d 0a0d 0a23 204e 616d 696e 6720  SE"....# Naming 
-00001210: 7374 796c 6520 6d61 7463 6869 6e67 2063  style matching c
-00001220: 6f72 7265 6374 2063 6c61 7373 206e 616d  orrect class nam
-00001230: 6573 2e0d 0a63 6c61 7373 2d6e 616d 696e  es...class-namin
-00001240: 672d 7374 796c 6520 3d20 2250 6173 6361  g-style = "Pasca
-00001250: 6c43 6173 6522 0d0a 0d0a 2320 4e61 6d69  lCase"....# Nami
-00001260: 6e67 2073 7479 6c65 206d 6174 6368 696e  ng style matchin
-00001270: 6720 636f 7272 6563 7420 636f 6e73 7461  g correct consta
-00001280: 6e74 206e 616d 6573 2e0d 0a63 6f6e 7374  nt names...const
-00001290: 2d6e 616d 696e 672d 7374 796c 6520 3d20  -naming-style = 
-000012a0: 2255 5050 4552 5f43 4153 4522 0d0a 0d0a  "UPPER_CASE"....
-000012b0: 2320 4d69 6e69 6d75 6d20 6c69 6e65 206c  # Minimum line l
-000012c0: 656e 6774 6820 666f 7220 6675 6e63 7469  ength for functi
-000012d0: 6f6e 732f 636c 6173 7365 7320 7468 6174  ons/classes that
-000012e0: 2072 6571 7569 7265 2064 6f63 7374 7269   require docstri
-000012f0: 6e67 732c 2073 686f 7274 6572 206f 6e65  ngs, shorter one
-00001300: 730d 0a23 2061 7265 2065 7865 6d70 742e  s..# are exempt.
-00001310: 0d0a 646f 6373 7472 696e 672d 6d69 6e2d  ..docstring-min-
-00001320: 6c65 6e67 7468 203d 202d 310d 0a0d 0a23  length = -1....#
-00001330: 204e 616d 696e 6720 7374 796c 6520 6d61   Naming style ma
-00001340: 7463 6869 6e67 2063 6f72 7265 6374 2066  tching correct f
-00001350: 756e 6374 696f 6e20 6e61 6d65 732e 0d0a  unction names...
-00001360: 6675 6e63 7469 6f6e 2d6e 616d 696e 672d  function-naming-
-00001370: 7374 796c 6520 3d20 2273 6e61 6b65 5f63  style = "snake_c
-00001380: 6173 6522 0d0a 0d0a 2320 476f 6f64 2076  ase"....# Good v
-00001390: 6172 6961 626c 6520 6e61 6d65 7320 7768  ariable names wh
-000013a0: 6963 6820 7368 6f75 6c64 2061 6c77 6179  ich should alway
-000013b0: 7320 6265 2061 6363 6570 7465 642c 2073  s be accepted, s
-000013c0: 6570 6172 6174 6564 2062 7920 6120 636f  eparated by a co
-000013d0: 6d6d 612e 0d0a 676f 6f64 2d6e 616d 6573  mma...good-names
-000013e0: 203d 205b 2269 222c 2022 6a22 2c20 226b   = ["i", "j", "k
-000013f0: 222c 2022 6578 222c 2022 5275 6e22 2c20  ", "ex", "Run", 
-00001400: 225f 225d 0d0a 0d0a 2320 4e61 6d69 6e67  "_"]....# Naming
-00001410: 2073 7479 6c65 206d 6174 6368 696e 6720   style matching 
-00001420: 636f 7272 6563 7420 6d65 7468 6f64 206e  correct method n
-00001430: 616d 6573 2e0d 0a6d 6574 686f 642d 6e61  ames...method-na
-00001440: 6d69 6e67 2d73 7479 6c65 203d 2022 736e  ming-style = "sn
-00001450: 616b 655f 6361 7365 220d 0a0d 0a23 204e  ake_case"....# N
-00001460: 616d 696e 6720 7374 796c 6520 6d61 7463  aming style matc
-00001470: 6869 6e67 2063 6f72 7265 6374 206d 6f64  hing correct mod
-00001480: 756c 6520 6e61 6d65 732e 0d0a 6d6f 6475  ule names...modu
-00001490: 6c65 2d6e 616d 696e 672d 7374 796c 6520  le-naming-style 
-000014a0: 3d20 2273 6e61 6b65 5f63 6173 6522 0d0a  = "snake_case"..
-000014b0: 0d0a 2320 5265 6775 6c61 7220 6578 7072  ..# Regular expr
-000014c0: 6573 7369 6f6e 2077 6869 6368 2073 686f  ession which sho
-000014d0: 756c 6420 6f6e 6c79 206d 6174 6368 2066  uld only match f
-000014e0: 756e 6374 696f 6e20 6f72 2063 6c61 7373  unction or class
-000014f0: 206e 616d 6573 2074 6861 7420 646f 206e   names that do n
-00001500: 6f74 0d0a 2320 7265 7175 6972 6520 6120  ot..# require a 
-00001510: 646f 6373 7472 696e 672e 0d0a 6e6f 2d64  docstring...no-d
-00001520: 6f63 7374 7269 6e67 2d72 6778 203d 2022  ocstring-rgx = "
-00001530: 5e5f 220d 0a0d 0a23 204c 6973 7420 6f66  ^_"....# List of
-00001540: 2064 6563 6f72 6174 6f72 7320 7468 6174   decorators that
-00001550: 2070 726f 6475 6365 2070 726f 7065 7274   produce propert
-00001560: 6965 732c 2073 7563 6820 6173 2061 6263  ies, such as abc
-00001570: 2e61 6273 7472 6163 7470 726f 7065 7274  .abstractpropert
-00001580: 792e 2041 6464 0d0a 2320 746f 2074 6869  y. Add..# to thi
-00001590: 7320 6c69 7374 2074 6f20 7265 6769 7374  s list to regist
-000015a0: 6572 206f 7468 6572 2064 6563 6f72 6174  er other decorat
-000015b0: 6f72 7320 7468 6174 2070 726f 6475 6365  ors that produce
-000015c0: 2076 616c 6964 2070 726f 7065 7274 6965   valid propertie
-000015d0: 732e 2054 6865 7365 0d0a 2320 6465 636f  s. These..# deco
-000015e0: 7261 746f 7273 2061 7265 2074 616b 656e  rators are taken
-000015f0: 2069 6e20 636f 6e73 6964 6572 6174 696f   in consideratio
-00001600: 6e20 6f6e 6c79 2066 6f72 2069 6e76 616c  n only for inval
-00001610: 6964 2d6e 616d 652e 0d0a 7072 6f70 6572  id-name...proper
-00001620: 7479 2d63 6c61 7373 6573 203d 205b 2261  ty-classes = ["a
-00001630: 6263 2e61 6273 7472 6163 7470 726f 7065  bc.abstractprope
-00001640: 7274 7922 5d0d 0a0d 0a23 204e 616d 696e  rty"]....# Namin
-00001650: 6720 7374 796c 6520 6d61 7463 6869 6e67  g style matching
-00001660: 2063 6f72 7265 6374 2076 6172 6961 626c   correct variabl
-00001670: 6520 6e61 6d65 732e 0d0a 7661 7269 6162  e names...variab
-00001680: 6c65 2d6e 616d 696e 672d 7374 796c 6520  le-naming-style 
-00001690: 3d20 2273 6e61 6b65 5f63 6173 6522 0d0a  = "snake_case"..
-000016a0: 0d0a 5b74 6f6f 6c2e 7079 6c69 6e74 2e63  ..[tool.pylint.c
-000016b0: 6c61 7373 6573 5d0d 0a23 2057 6172 6e20  lasses]..# Warn 
-000016c0: 6162 6f75 7420 7072 6f74 6563 7465 6420  about protected 
-000016d0: 6174 7472 6962 7574 6520 6163 6365 7373  attribute access
-000016e0: 2069 6e73 6964 6520 7370 6563 6961 6c20   inside special 
-000016f0: 6d65 7468 6f64 730d 0a23 2063 6865 636b  methods..# check
-00001700: 2d70 726f 7465 6374 6564 2d61 6363 6573  -protected-acces
-00001710: 732d 696e 2d73 7065 6369 616c 2d6d 6574  s-in-special-met
-00001720: 686f 6473 203d 0d0a 0d0a 2320 4c69 7374  hods =....# List
-00001730: 206f 6620 6d65 7468 6f64 206e 616d 6573   of method names
-00001740: 2075 7365 6420 746f 2064 6563 6c61 7265   used to declare
-00001750: 2028 692e 652e 2061 7373 6967 6e29 2069   (i.e. assign) i
-00001760: 6e73 7461 6e63 6520 6174 7472 6962 7574  nstance attribut
-00001770: 6573 2e0d 0a64 6566 696e 696e 672d 6174  es...defining-at
-00001780: 7472 2d6d 6574 686f 6473 203d 205b 225f  tr-methods = ["_
-00001790: 5f69 6e69 745f 5f22 2c20 225f 5f6e 6577  _init__", "__new
-000017a0: 5f5f 222c 2022 7365 7455 7022 2c20 225f  __", "setUp", "_
-000017b0: 5f70 6f73 745f 696e 6974 5f5f 225d 0d0a  _post_init__"]..
-000017c0: 0d0a 2320 4c69 7374 206f 6620 6d65 6d62  ..# List of memb
-000017d0: 6572 206e 616d 6573 2c20 7768 6963 6820  er names, which 
-000017e0: 7368 6f75 6c64 2062 6520 6578 636c 7564  should be exclud
-000017f0: 6564 2066 726f 6d20 7468 6520 7072 6f74  ed from the prot
-00001800: 6563 7465 6420 6163 6365 7373 0d0a 2320  ected access..# 
-00001810: 7761 726e 696e 672e 0d0a 6578 636c 7564  warning...exclud
-00001820: 652d 7072 6f74 6563 7465 6420 3d20 5b22  e-protected = ["
-00001830: 5f61 7364 6963 7422 2c20 225f 6669 656c  _asdict", "_fiel
-00001840: 6473 222c 2022 5f72 6570 6c61 6365 222c  ds", "_replace",
-00001850: 2022 5f73 6f75 7263 6522 2c20 225f 6d61   "_source", "_ma
-00001860: 6b65 225d 0d0a 0d0a 2320 4c69 7374 206f  ke"]....# List o
-00001870: 6620 7661 6c69 6420 6e61 6d65 7320 666f  f valid names fo
-00001880: 7220 7468 6520 6669 7273 7420 6172 6775  r the first argu
-00001890: 6d65 6e74 2069 6e20 6120 636c 6173 7320  ment in a class 
-000018a0: 6d65 7468 6f64 2e0d 0a76 616c 6964 2d63  method...valid-c
-000018b0: 6c61 7373 6d65 7468 6f64 2d66 6972 7374  lassmethod-first
-000018c0: 2d61 7267 203d 205b 2263 6c73 225d 0d0a  -arg = ["cls"]..
-000018d0: 0d0a 2320 4c69 7374 206f 6620 7661 6c69  ..# List of vali
-000018e0: 6420 6e61 6d65 7320 666f 7220 7468 6520  d names for the 
-000018f0: 6669 7273 7420 6172 6775 6d65 6e74 2069  first argument i
-00001900: 6e20 6120 6d65 7461 636c 6173 7320 636c  n a metaclass cl
-00001910: 6173 7320 6d65 7468 6f64 2e0d 0a76 616c  ass method...val
-00001920: 6964 2d6d 6574 6163 6c61 7373 2d63 6c61  id-metaclass-cla
-00001930: 7373 6d65 7468 6f64 2d66 6972 7374 2d61  ssmethod-first-a
-00001940: 7267 203d 205b 226d 6373 225d 0d0a 0d0a  rg = ["mcs"]....
-00001950: 5b74 6f6f 6c2e 7079 6c69 6e74 2e64 6573  [tool.pylint.des
-00001960: 6967 6e5d 0d0a 2320 4d61 7869 6d75 6d20  ign]..# Maximum 
-00001970: 6e75 6d62 6572 206f 6620 6172 6775 6d65  number of argume
-00001980: 6e74 7320 666f 7220 6675 6e63 7469 6f6e  nts for function
-00001990: 202f 206d 6574 686f 642e 0d0a 6d61 782d   / method...max-
-000019a0: 6172 6773 203d 2035 0d0a 0d0a 2320 4d61  args = 5....# Ma
-000019b0: 7869 6d75 6d20 6e75 6d62 6572 206f 6620  ximum number of 
-000019c0: 6174 7472 6962 7574 6573 2066 6f72 2061  attributes for a
-000019d0: 2063 6c61 7373 2028 7365 6520 5230 3930   class (see R090
-000019e0: 3229 2e0d 0a6d 6178 2d61 7474 7269 6275  2)...max-attribu
-000019f0: 7465 7320 3d20 370d 0a0d 0a23 204d 6178  tes = 7....# Max
-00001a00: 696d 756d 206e 756d 6265 7220 6f66 2062  imum number of b
-00001a10: 6f6f 6c65 616e 2065 7870 7265 7373 696f  oolean expressio
-00001a20: 6e73 2069 6e20 616e 2069 6620 7374 6174  ns in an if stat
-00001a30: 656d 656e 7420 2873 6565 2052 3039 3136  ement (see R0916
-00001a40: 292e 0d0a 6d61 782d 626f 6f6c 2d65 7870  )...max-bool-exp
-00001a50: 7220 3d20 350d 0a0d 0a23 204d 6178 696d  r = 5....# Maxim
-00001a60: 756d 206e 756d 6265 7220 6f66 2062 7261  um number of bra
-00001a70: 6e63 6820 666f 7220 6675 6e63 7469 6f6e  nch for function
-00001a80: 202f 206d 6574 686f 6420 626f 6479 2e0d   / method body..
-00001a90: 0a6d 6178 2d62 7261 6e63 6865 7320 3d20  .max-branches = 
-00001aa0: 3132 0d0a 0d0a 2320 4d61 7869 6d75 6d20  12....# Maximum 
-00001ab0: 6e75 6d62 6572 206f 6620 6c6f 6361 6c73  number of locals
-00001ac0: 2066 6f72 2066 756e 6374 696f 6e20 2f20   for function / 
-00001ad0: 6d65 7468 6f64 2062 6f64 792e 0d0a 6d61  method body...ma
-00001ae0: 782d 6c6f 6361 6c73 203d 2031 350d 0a0d  x-locals = 15...
-00001af0: 0a23 204d 6178 696d 756d 206e 756d 6265  .# Maximum numbe
-00001b00: 7220 6f66 2070 6172 656e 7473 2066 6f72  r of parents for
-00001b10: 2061 2063 6c61 7373 2028 7365 6520 5230   a class (see R0
-00001b20: 3930 3129 2e0d 0a6d 6178 2d70 6172 656e  901)...max-paren
-00001b30: 7473 203d 2037 0d0a 0d0a 2320 4d61 7869  ts = 7....# Maxi
-00001b40: 6d75 6d20 6e75 6d62 6572 206f 6620 7075  mum number of pu
-00001b50: 626c 6963 206d 6574 686f 6473 2066 6f72  blic methods for
-00001b60: 2061 2063 6c61 7373 2028 7365 6520 5230   a class (see R0
-00001b70: 3930 3429 2e0d 0a6d 6178 2d70 7562 6c69  904)...max-publi
-00001b80: 632d 6d65 7468 6f64 7320 3d20 3230 0d0a  c-methods = 20..
-00001b90: 0d0a 2320 4d61 7869 6d75 6d20 6e75 6d62  ..# Maximum numb
-00001ba0: 6572 206f 6620 7265 7475 726e 202f 2079  er of return / y
-00001bb0: 6965 6c64 2066 6f72 2066 756e 6374 696f  ield for functio
-00001bc0: 6e20 2f20 6d65 7468 6f64 2062 6f64 792e  n / method body.
-00001bd0: 0d0a 6d61 782d 7265 7475 726e 7320 3d20  ..max-returns = 
-00001be0: 360d 0a0d 0a23 204d 6178 696d 756d 206e  6....# Maximum n
-00001bf0: 756d 6265 7220 6f66 2073 7461 7465 6d65  umber of stateme
-00001c00: 6e74 7320 696e 2066 756e 6374 696f 6e20  nts in function 
-00001c10: 2f20 6d65 7468 6f64 2062 6f64 792e 0d0a  / method body...
-00001c20: 6d61 782d 7374 6174 656d 656e 7473 203d  max-statements =
-00001c30: 2035 300d 0a0d 0a23 204d 696e 696d 756d   50....# Minimum
-00001c40: 206e 756d 6265 7220 6f66 2070 7562 6c69   number of publi
-00001c50: 6320 6d65 7468 6f64 7320 666f 7220 6120  c methods for a 
-00001c60: 636c 6173 7320 2873 6565 2052 3039 3033  class (see R0903
-00001c70: 292e 0d0a 6d69 6e2d 7075 626c 6963 2d6d  )...min-public-m
-00001c80: 6574 686f 6473 203d 2031 0d0a 0d0a 5b74  ethods = 1....[t
-00001c90: 6f6f 6c2e 7079 6c69 6e74 2e65 7863 6570  ool.pylint.excep
-00001ca0: 7469 6f6e 735d 0d0a 2320 4578 6365 7074  tions]..# Except
-00001cb0: 696f 6e73 2074 6861 7420 7769 6c6c 2065  ions that will e
-00001cc0: 6d69 7420 6120 7761 726e 696e 6720 7768  mit a warning wh
-00001cd0: 656e 2063 6175 6768 742e 0d0a 6f76 6572  en caught...over
-00001ce0: 6765 6e65 7261 6c2d 6578 6365 7074 696f  general-exceptio
-00001cf0: 6e73 203d 205b 2262 7569 6c74 696e 732e  ns = ["builtins.
-00001d00: 4261 7365 4578 6365 7074 696f 6e22 2c20  BaseException", 
-00001d10: 2262 7569 6c74 696e 732e 4578 6365 7074  "builtins.Except
-00001d20: 696f 6e22 5d0d 0a0d 0a5b 746f 6f6c 2e70  ion"]....[tool.p
-00001d30: 796c 696e 742e 666f 726d 6174 5d0d 0a23  ylint.format]..#
-00001d40: 2052 6567 6578 7020 666f 7220 6120 6c69   Regexp for a li
-00001d50: 6e65 2074 6861 7420 6973 2061 6c6c 6f77  ne that is allow
-00001d60: 6564 2074 6f20 6265 206c 6f6e 6765 7220  ed to be longer 
-00001d70: 7468 616e 2074 6865 206c 696d 6974 2e0d  than the limit..
-00001d80: 0a69 676e 6f72 652d 6c6f 6e67 2d6c 696e  .ignore-long-lin
-00001d90: 6573 203d 2022 5e5c 5c73 2a28 2320 293f  es = "^\\s*(# )?
-00001da0: 3c3f 6874 7470 733f 3a2f 2f5c 5c53 2b3e  <?https?://\\S+>
-00001db0: 3f24 220d 0a0d 0a23 204e 756d 6265 7220  ?$"....# Number 
-00001dc0: 6f66 2073 7061 6365 7320 6f66 2069 6e64  of spaces of ind
-00001dd0: 656e 7420 7265 7175 6972 6564 2069 6e73  ent required ins
-00001de0: 6964 6520 6120 6861 6e67 696e 6720 6f72  ide a hanging or
-00001df0: 2063 6f6e 7469 6e75 6564 206c 696e 652e   continued line.
-00001e00: 0d0a 696e 6465 6e74 2d61 6674 6572 2d70  ..indent-after-p
-00001e10: 6172 656e 203d 2034 0d0a 0d0a 2320 5374  aren = 4....# St
-00001e20: 7269 6e67 2075 7365 6420 6173 2069 6e64  ring used as ind
-00001e30: 656e 7461 7469 6f6e 2075 6e69 742e 2054  entation unit. T
-00001e40: 6869 7320 6973 2075 7375 616c 6c79 2022  his is usually "
-00001e50: 2020 2020 2220 2834 2073 7061 6365 7329      " (4 spaces)
-00001e60: 206f 7220 225c 7422 2028 310d 0a23 2074   or "\t" (1..# t
-00001e70: 6162 292e 0d0a 696e 6465 6e74 2d73 7472  ab)...indent-str
-00001e80: 696e 6720 3d20 2220 2020 2022 0d0a 0d0a  ing = "    "....
-00001e90: 2320 4d61 7869 6d75 6d20 6e75 6d62 6572  # Maximum number
-00001ea0: 206f 6620 6368 6172 6163 7465 7273 206f   of characters o
-00001eb0: 6e20 6120 7369 6e67 6c65 206c 696e 652e  n a single line.
-00001ec0: 0d0a 6d61 782d 6c69 6e65 2d6c 656e 6774  ..max-line-lengt
-00001ed0: 6820 3d20 3130 300d 0a0d 0a23 204d 6178  h = 100....# Max
-00001ee0: 696d 756d 206e 756d 6265 7220 6f66 206c  imum number of l
-00001ef0: 696e 6573 2069 6e20 6120 6d6f 6475 6c65  ines in a module
-00001f00: 2e0d 0a6d 6178 2d6d 6f64 756c 652d 6c69  ...max-module-li
-00001f10: 6e65 7320 3d20 3130 3030 0d0a 0d0a 5b74  nes = 1000....[t
-00001f20: 6f6f 6c2e 7079 6c69 6e74 2e6d 6973 6365  ool.pylint.misce
-00001f30: 6c6c 616e 656f 7573 5d0d 0a23 204c 6973  llaneous]..# Lis
-00001f40: 7420 6f66 206e 6f74 6520 7461 6773 2074  t of note tags t
-00001f50: 6f20 7461 6b65 2069 6e20 636f 6e73 6964  o take in consid
-00001f60: 6572 6174 696f 6e2c 2073 6570 6172 6174  eration, separat
-00001f70: 6564 2062 7920 6120 636f 6d6d 612e 0d0a  ed by a comma...
-00001f80: 6e6f 7465 7320 3d20 5b22 4649 584d 4522  notes = ["FIXME"
-00001f90: 2c20 2258 5858 222c 2022 544f 444f 225d  , "XXX", "TODO"]
-00001fa0: 0d0a 0d0a 5b74 6f6f 6c2e 7079 6c69 6e74  ....[tool.pylint
-00001fb0: 2e72 6566 6163 746f 7269 6e67 5d0d 0a23  .refactoring]..#
-00001fc0: 204d 6178 696d 756d 206e 756d 6265 7220   Maximum number 
-00001fd0: 6f66 206e 6573 7465 6420 626c 6f63 6b73  of nested blocks
-00001fe0: 2066 6f72 2066 756e 6374 696f 6e20 2f20   for function / 
-00001ff0: 6d65 7468 6f64 2062 6f64 790d 0a6d 6178  method body..max
-00002000: 2d6e 6573 7465 642d 626c 6f63 6b73 203d  -nested-blocks =
-00002010: 2035 0d0a 0d0a 2320 436f 6d70 6c65 7465   5....# Complete
-00002020: 206e 616d 6520 6f66 2066 756e 6374 696f   name of functio
-00002030: 6e73 2074 6861 7420 6e65 7665 7220 7265  ns that never re
-00002040: 7475 726e 732e 2057 6865 6e20 6368 6563  turns. When chec
-00002050: 6b69 6e67 2066 6f72 2069 6e63 6f6e 7369  king for inconsi
-00002060: 7374 656e 742d 0d0a 2320 7265 7475 726e  stent-..# return
-00002070: 2d73 7461 7465 6d65 6e74 7320 6966 2061  -statements if a
-00002080: 206e 6576 6572 2072 6574 7572 6e69 6e67   never returning
-00002090: 2066 756e 6374 696f 6e20 6973 2063 616c   function is cal
-000020a0: 6c65 6420 7468 656e 2069 7420 7769 6c6c  led then it will
-000020b0: 2062 650d 0a23 2063 6f6e 7369 6465 7265   be..# considere
-000020c0: 6420 6173 2061 6e20 6578 706c 6963 6974  d as an explicit
-000020d0: 2072 6574 7572 6e20 7374 6174 656d 656e   return statemen
-000020e0: 7420 616e 6420 6e6f 206d 6573 7361 6765  t and no message
-000020f0: 2077 696c 6c20 6265 2070 7269 6e74 6564   will be printed
-00002100: 2e0d 0a6e 6576 6572 2d72 6574 7572 6e69  ...never-returni
-00002110: 6e67 2d66 756e 6374 696f 6e73 203d 205b  ng-functions = [
-00002120: 2273 7973 2e65 7869 7422 2c20 2261 7267  "sys.exit", "arg
-00002130: 7061 7273 652e 7061 7273 655f 6572 726f  parse.parse_erro
-00002140: 7222 5d0d 0a0d 0a5b 746f 6f6c 2e70 796c  r"]....[tool.pyl
-00002150: 696e 742e 7369 6d69 6c61 7269 7469 6573  int.similarities
-00002160: 5d0d 0a23 2043 6f6d 6d65 6e74 7320 6172  ]..# Comments ar
-00002170: 6520 7265 6d6f 7665 6420 6672 6f6d 2074  e removed from t
-00002180: 6865 2073 696d 696c 6172 6974 7920 636f  he similarity co
-00002190: 6d70 7574 6174 696f 6e0d 0a69 676e 6f72  mputation..ignor
-000021a0: 652d 636f 6d6d 656e 7473 203d 2074 7275  e-comments = tru
-000021b0: 650d 0a0d 0a23 2044 6f63 7374 7269 6e67  e....# Docstring
-000021c0: 7320 6172 6520 7265 6d6f 7665 6420 6672  s are removed fr
-000021d0: 6f6d 2074 6865 2073 696d 696c 6172 6974  om the similarit
-000021e0: 7920 636f 6d70 7574 6174 696f 6e0d 0a69  y computation..i
-000021f0: 676e 6f72 652d 646f 6373 7472 696e 6773  gnore-docstrings
-00002200: 203d 2074 7275 650d 0a0d 0a23 2049 6d70   = true....# Imp
-00002210: 6f72 7473 2061 7265 2072 656d 6f76 6564  orts are removed
-00002220: 2066 726f 6d20 7468 6520 7369 6d69 6c61   from the simila
-00002230: 7269 7479 2063 6f6d 7075 7461 7469 6f6e  rity computation
-00002240: 0d0a 6967 6e6f 7265 2d69 6d70 6f72 7473  ..ignore-imports
-00002250: 203d 2074 7275 650d 0a0d 0a23 2053 6967   = true....# Sig
-00002260: 6e61 7475 7265 7320 6172 6520 7265 6d6f  natures are remo
-00002270: 7665 6420 6672 6f6d 2074 6865 2073 696d  ved from the sim
-00002280: 696c 6172 6974 7920 636f 6d70 7574 6174  ilarity computat
-00002290: 696f 6e0d 0a69 676e 6f72 652d 7369 676e  ion..ignore-sign
-000022a0: 6174 7572 6573 203d 2074 7275 650d 0a0d  atures = true...
-000022b0: 0a23 204d 696e 696d 756d 206c 696e 6573  .# Minimum lines
-000022c0: 206e 756d 6265 7220 6f66 2061 2073 696d   number of a sim
-000022d0: 696c 6172 6974 792e 0d0a 6d69 6e2d 7369  ilarity...min-si
-000022e0: 6d69 6c61 7269 7479 2d6c 696e 6573 203d  milarity-lines =
-000022f0: 2038 0d0a 0d0a 5b74 6f6f 6c2e 7079 6c69   8....[tool.pyli
-00002300: 6e74 2e73 7065 6c6c 696e 675d 0d0a 2320  nt.spelling]..# 
-00002310: 4c69 6d69 7473 2063 6f75 6e74 206f 6620  Limits count of 
-00002320: 656d 6974 7465 6420 7375 6767 6573 7469  emitted suggesti
-00002330: 6f6e 7320 666f 7220 7370 656c 6c69 6e67  ons for spelling
-00002340: 206d 6973 7461 6b65 732e 0d0a 6d61 782d   mistakes...max-
-00002350: 7370 656c 6c69 6e67 2d73 7567 6765 7374  spelling-suggest
-00002360: 696f 6e73 203d 2034 0d0a 0d0a 5b74 6f6f  ions = 4....[too
-00002370: 6c2e 7079 6c69 6e74 2e76 6172 6961 626c  l.pylint.variabl
-00002380: 6573 5d0d 0a23 2054 656c 6c73 2077 6865  es]..# Tells whe
-00002390: 7468 6572 2075 6e75 7365 6420 676c 6f62  ther unused glob
-000023a0: 616c 2076 6172 6961 626c 6573 2073 686f  al variables sho
-000023b0: 756c 6420 6265 2074 7265 6174 6564 2061  uld be treated a
-000023c0: 7320 6120 7669 6f6c 6174 696f 6e2e 0d0a  s a violation...
-000023d0: 616c 6c6f 772d 676c 6f62 616c 2d75 6e75  allow-global-unu
-000023e0: 7365 642d 7661 7269 6162 6c65 7320 3d20  sed-variables = 
-000023f0: 7472 7565 0d0a 0d0a 2320 4c69 7374 206f  true....# List o
-00002400: 6620 7374 7269 6e67 7320 7768 6963 6820  f strings which 
-00002410: 6361 6e20 6964 656e 7469 6679 2061 2063  can identify a c
-00002420: 616c 6c62 6163 6b20 6675 6e63 7469 6f6e  allback function
-00002430: 2062 7920 6e61 6d65 2e20 4120 6361 6c6c   by name. A call
-00002440: 6261 636b 206e 616d 650d 0a23 206d 7573  back name..# mus
-00002450: 7420 7374 6172 7420 6f72 2065 6e64 2077  t start or end w
-00002460: 6974 6820 6f6e 6520 6f66 2074 686f 7365  ith one of those
-00002470: 2073 7472 696e 6773 2e0d 0a63 616c 6c62   strings...callb
-00002480: 6163 6b73 203d 205b 2263 625f 222c 2022  acks = ["cb_", "
-00002490: 5f63 6222 5d0d 0a0d 0a23 2041 2072 6567  _cb"]....# A reg
-000024a0: 756c 6172 2065 7870 7265 7373 696f 6e20  ular expression 
-000024b0: 6d61 7463 6869 6e67 2074 6865 206e 616d  matching the nam
-000024c0: 6520 6f66 2064 756d 6d79 2076 6172 6961  e of dummy varia
-000024d0: 626c 6573 2028 692e 652e 2065 7870 6563  bles (i.e. expec
-000024e0: 7465 6420 746f 206e 6f74 0d0a 2320 6265  ted to not..# be
-000024f0: 2075 7365 6429 2e0d 0a64 756d 6d79 2d76   used)...dummy-v
-00002500: 6172 6961 626c 6573 2d72 6778 203d 2022  ariables-rgx = "
-00002510: 5f2b 247c 285f 5b61 2d7a 412d 5a30 2d39  _+$|(_[a-zA-Z0-9
-00002520: 5f5d 2a5b 612d 7a41 2d5a 302d 395d 2b3f  _]*[a-zA-Z0-9]+?
-00002530: 2429 7c64 756d 6d79 7c5e 6967 6e6f 7265  $)|dummy|^ignore
-00002540: 645f 7c5e 756e 7573 6564 5f22 0d0a 0d0a  d_|^unused_"....
-00002550: 2320 4172 6775 6d65 6e74 206e 616d 6573  # Argument names
-00002560: 2074 6861 7420 6d61 7463 6820 7468 6973   that match this
-00002570: 2065 7870 7265 7373 696f 6e20 7769 6c6c   expression will
-00002580: 2062 6520 6967 6e6f 7265 642e 0d0a 6967   be ignored...ig
-00002590: 6e6f 7265 642d 6172 6775 6d65 6e74 2d6e  nored-argument-n
-000025a0: 616d 6573 203d 2022 5f2e 2a7c 5e69 676e  ames = "_.*|^ign
-000025b0: 6f72 6564 5f7c 5e75 6e75 7365 645f 220d  ored_|^unused_".
-000025c0: 0a0d 0a23 204c 6973 7420 6f66 2071 7561  ...# List of qua
-000025d0: 6c69 6669 6564 206d 6f64 756c 6520 6e61  lified module na
-000025e0: 6d65 7320 7768 6963 6820 6361 6e20 6861  mes which can ha
-000025f0: 7665 206f 626a 6563 7473 2074 6861 7420  ve objects that 
-00002600: 6361 6e20 7265 6465 6669 6e65 0d0a 2320  can redefine..# 
-00002610: 6275 696c 7469 6e73 2e0d 0a72 6564 6566  builtins...redef
-00002620: 696e 696e 672d 6275 696c 7469 6e73 2d6d  ining-builtins-m
-00002630: 6f64 756c 6573 203d 205b 2273 6978 2e6d  odules = ["six.m
-00002640: 6f76 6573 222c 2022 7061 7374 2e62 7569  oves", "past.bui
-00002650: 6c74 696e 7322 2c20 2266 7574 7572 652e  ltins", "future.
-00002660: 6275 696c 7469 6e73 222c 2022 6275 696c  builtins", "buil
-00002670: 7469 6e73 222c 2022 696f 225d 0d0a 0d0a  tins", "io"]....
-00002680: 5b74 6f6f 6c2e 7079 6c69 6e74 2e6d 6573  [tool.pylint.mes
-00002690: 7361 6765 735f 636f 6e74 726f 6c5d 0d0a  sages_control]..
-000026a0: 6469 7361 626c 6520 3d20 5b0d 0a20 2022  disable = [..  "
-000026b0: 6c69 6e65 2d74 6f6f 2d6c 6f6e 6722 2c0d  line-too-long",.
-000026c0: 0a20 2022 696e 7661 6c69 642d 6e61 6d65  .  "invalid-name
-000026d0: 222c 0d0a 2020 226d 6973 7369 6e67 2d66  ",..  "missing-f
-000026e0: 756e 6374 696f 6e2d 646f 6373 7472 696e  unction-docstrin
-000026f0: 6722 2c0d 0a20 2022 6d69 7373 696e 672d  g",..  "missing-
-00002700: 636c 6173 732d 646f 6373 7472 696e 6722  class-docstring"
-00002710: 2c0d 0a20 2022 6174 7472 6962 7574 652d  ,..  "attribute-
-00002720: 6465 6669 6e65 642d 6f75 7473 6964 652d  defined-outside-
-00002730: 696e 6974 222c 0d0a 2020 2265 7865 632d  init",..  "exec-
-00002740: 7573 6564 222c 0d0a 2020 2263 6f6e 7369  used",..  "consi
-00002750: 6465 722d 7573 696e 672d 662d 7374 7269  der-using-f-stri
-00002760: 6e67 222c 0d0a 2020 2272 6564 6566 696e  ng",..  "redefin
-00002770: 6564 2d6f 7574 6572 2d6e 616d 6522 2c0d  ed-outer-name",.
-00002780: 0a20 2022 6475 706c 6963 6174 652d 636f  .  "duplicate-co
-00002790: 6465 222c 0d0a 2020 2274 6f6f 2d66 6577  de",..  "too-few
-000027a0: 2d70 7562 6c69 632d 6d65 7468 6f64 7322  -public-methods"
-000027b0: 2c0d 0a20 2022 746f 6f2d 6d61 6e79 2d69  ,..  "too-many-i
-000027c0: 6e73 7461 6e63 652d 6174 7472 6962 7574  nstance-attribut
-000027d0: 6573 222c 0d0a 2020 2263 6f6e 7369 6465  es",..  "conside
-000027e0: 722d 6974 6572 6174 696e 672d 6469 6374  r-iterating-dict
-000027f0: 696f 6e61 7279 222c 0d0a 2020 2263 6f6e  ionary",..  "con
-00002800: 7369 6465 722d 7573 696e 672d 6469 6374  sider-using-dict
-00002810: 2d69 7465 6d73 222c 0d0a 2020 2274 6f6f  -items",..  "too
-00002820: 2d6d 616e 792d 6272 616e 6368 6573 222c  -many-branches",
-00002830: 0d0a 2020 2273 7570 6572 2d69 6e69 742d  ..  "super-init-
-00002840: 6e6f 742d 6361 6c6c 6564 222c 0d0a 2020  not-called",..  
-00002850: 226d 6973 7369 6e67 2d6d 6f64 756c 652d  "missing-module-
-00002860: 646f 6373 7472 696e 6722 0d0a 5d0d 0a    docstring"..]..
+00000150: 203d 2022 3e3d 332e 3922 0d0a 6175 7468   = ">=3.9"..auth
+00000160: 6f72 7320 3d20 5b0d 0a20 207b 6e61 6d65  ors = [..  {name
+00000170: 203d 2022 4d6f 6a74 6162 6120 5361 7264   = "Mojtaba Sard
+00000180: 6172 6d65 686e 6922 2c20 656d 6169 6c20  armehni", email 
+00000190: 3d20 226d 7361 7264 6172 3240 616c 756d  = "msardar2@alum
+000001a0: 6e69 2e6e 6373 752e 6564 7522 7d2c 0d0a  ni.ncsu.edu"},..
+000001b0: 5d0d 0a6d 6169 6e74 6169 6e65 7273 203d  ]..maintainers =
+000001c0: 205b 0d0a 2020 7b6e 616d 6520 3d20 224d   [..  {name = "M
+000001d0: 6f6a 7461 6261 2053 6172 6461 726d 6568  ojtaba Sardarmeh
+000001e0: 6e69 222c 2065 6d61 696c 203d 2022 6d73  ni", email = "ms
+000001f0: 6172 6461 7232 4061 6c75 6d6e 692e 6e63  ardar2@alumni.nc
+00000200: 7375 2e65 6475 227d 2c0d 0a5d 0d0a 6b65  su.edu"},..]..ke
+00000210: 7977 6f72 6473 203d 205b 0d0a 2020 2020  ywords = [..    
+00000220: 224c 4341 222c 0d0a 2020 2020 2273 6f6c  "LCA",..    "sol
+00000230: 6964 5f77 6173 7465 222c 0d0a 2020 2020  id_waste",..    
+00000240: 2277 6173 7465 5f6d 616e 6167 656d 656e  "waste_managemen
+00000250: 7422 2c0d 0a20 2020 2022 7377 6f6c 6670  t",..    "swolfp
+00000260: 7922 2c0d 0a20 2020 2022 6272 6967 6874  y",..    "bright
+00000270: 7761 7932 222c 0d0a 5d0d 0a63 6c61 7373  way2",..]..class
+00000280: 6966 6965 7273 203d 205b 0d0a 2020 2020  ifiers = [..    
+00000290: 2744 6576 656c 6f70 6d65 6e74 2053 7461  'Development Sta
+000002a0: 7475 7320 3a3a 2035 202d 2050 726f 6475  tus :: 5 - Produ
+000002b0: 6374 696f 6e2f 5374 6162 6c65 272c 0d0a  ction/Stable',..
+000002c0: 2020 2020 2749 6e74 656e 6465 6420 4175      'Intended Au
+000002d0: 6469 656e 6365 203a 3a20 4564 7563 6174  dience :: Educat
+000002e0: 696f 6e27 2c0d 0a20 2020 2027 496e 7465  ion',..    'Inte
+000002f0: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
+00000300: 2053 6369 656e 6365 2f52 6573 6561 7263   Science/Researc
+00000310: 6827 2c0d 0a20 2020 2027 4c69 6365 6e73  h',..    'Licens
+00000320: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+00000330: 6420 3a3a 2047 4e55 2047 656e 6572 616c  d :: GNU General
+00000340: 2050 7562 6c69 6320 4c69 6365 6e73 6520   Public License 
+00000350: 7632 2028 4750 4c76 3229 272c 0d0a 2020  v2 (GPLv2)',..  
+00000360: 2020 274e 6174 7572 616c 204c 616e 6775    'Natural Langu
+00000370: 6167 6520 3a3a 2045 6e67 6c69 7368 272c  age :: English',
+00000380: 0d0a 2020 2020 2750 726f 6772 616d 6d69  ..    'Programmi
+00000390: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000003a0: 7974 686f 6e20 3a3a 2033 2e39 272c 0d0a  ython :: 3.9',..
+000003b0: 2020 2020 274f 7065 7261 7469 6e67 2053      'Operating S
+000003c0: 7973 7465 6d20 3a3a 204d 6163 4f53 203a  ystem :: MacOS :
+000003d0: 3a20 4d61 634f 5320 5827 2c0d 0a20 2020  : MacOS X',..   
+000003e0: 2027 4f70 6572 6174 696e 6720 5379 7374   'Operating Syst
+000003f0: 656d 203a 3a20 4d69 6372 6f73 6f66 7420  em :: Microsoft 
+00000400: 3a3a 2057 696e 646f 7773 272c 0d0a 2020  :: Windows',..  
+00000410: 2020 2754 6f70 6963 203a 3a20 5363 6965    'Topic :: Scie
+00000420: 6e74 6966 6963 2f45 6e67 696e 6565 7269  ntific/Engineeri
+00000430: 6e67 203a 3a20 496e 666f 726d 6174 696f  ng :: Informatio
+00000440: 6e20 416e 616c 7973 6973 272c 0d0a 2020  n Analysis',..  
+00000450: 2020 2754 6f70 6963 203a 3a20 5363 6965    'Topic :: Scie
+00000460: 6e74 6966 6963 2f45 6e67 696e 6565 7269  ntific/Engineeri
+00000470: 6e67 203a 3a20 4d61 7468 656d 6174 6963  ng :: Mathematic
+00000480: 7327 2c0d 0a20 2020 2027 546f 7069 6320  s',..    'Topic 
+00000490: 3a3a 2053 6369 656e 7469 6669 632f 456e  :: Scientific/En
+000004a0: 6769 6e65 6572 696e 6720 3a3a 2056 6973  gineering :: Vis
+000004b0: 7561 6c69 7a61 7469 6f6e 272c 0d0a 2020  ualization',..  
+000004c0: 2020 274e 6174 7572 616c 204c 616e 6775    'Natural Langu
+000004d0: 6167 6520 3a3a 2045 6e67 6c69 7368 272c  age :: English',
+000004e0: 0d0a 5d0d 0a0d 0a5b 7072 6f6a 6563 742e  ..]....[project.
+000004f0: 7572 6c73 5d0d 0a48 6f6d 6570 6167 6520  urls]..Homepage 
+00000500: 3d20 2268 7474 7073 3a2f 2f73 776f 6c66  = "https://swolf
+00000510: 7079 2d70 726f 6a65 6374 2e67 6974 6875  py-project.githu
+00000520: 622e 696f 2f22 0d0a 446f 6375 6d65 6e74  b.io/"..Document
+00000530: 6174 696f 6e20 3d20 2268 7474 7073 3a2f  ation = "https:/
+00000540: 2f73 776f 6c66 7079 2e72 6561 6474 6865  /swolfpy.readthe
+00000550: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
+00000560: 742f 220d 0a22 536f 7572 6365 2043 6f64  t/".."Source Cod
+00000570: 6522 203d 2022 6874 7470 733a 2f2f 6769  e" = "https://gi
+00000580: 7468 7562 2e63 6f6d 2f53 776f 6c66 5079  thub.com/SwolfPy
+00000590: 2d50 726f 6a65 6374 2f73 776f 6c66 7079  -Project/swolfpy
+000005a0: 2d69 6e70 7574 6461 7461 220d 0a0d 0a5b  -inputdata"....[
+000005b0: 746f 6f6c 2e73 6574 7570 746f 6f6c 732e  tool.setuptools.
+000005c0: 6479 6e61 6d69 635d 0d0a 7665 7273 696f  dynamic]..versio
+000005d0: 6e20 3d20 7b61 7474 7220 3d20 2273 776f  n = {attr = "swo
+000005e0: 6c66 7079 5f69 6e70 7574 6461 7461 2e5f  lfpy_inputdata._
+000005f0: 5f76 6572 7369 6f6e 5f5f 227d 0d0a 7265  _version__"}..re
+00000600: 6164 6d65 203d 207b 6669 6c65 203d 205b  adme = {file = [
+00000610: 2252 4541 444d 452e 7273 7422 2c20 2248  "README.rst", "H
+00000620: 4953 544f 5259 2e72 7374 225d 7d0d 0a64  ISTORY.rst"]}..d
+00000630: 6570 656e 6465 6e63 6965 7320 3d20 7b66  ependencies = {f
+00000640: 696c 6520 3d20 2272 6571 7569 7265 6d65  ile = "requireme
+00000650: 6e74 732e 7478 7422 7d0d 0a0d 0a5b 746f  nts.txt"}....[to
+00000660: 6f6c 2e73 6574 7570 746f 6f6c 735d 0d0a  ol.setuptools]..
+00000670: 696e 636c 7564 652d 7061 636b 6167 652d  include-package-
+00000680: 6461 7461 203d 2074 7275 650d 0a0d 0a5b  data = true....[
+00000690: 746f 6f6c 2e73 6574 7570 746f 6f6c 732e  tool.setuptools.
+000006a0: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
+000006b0: 696e 636c 7564 6520 3d20 5b22 7377 6f6c  include = ["swol
+000006c0: 6670 795f 696e 7075 7464 6174 612a 225d  fpy_inputdata*"]
+000006d0: 0d0a 0d0a 0d0a 5b74 6f6f 6c2e 626c 6163  ......[tool.blac
+000006e0: 6b5d 0d0a 6c69 6e65 2d6c 656e 6774 6820  k]..line-length 
+000006f0: 3d20 3130 300d 0a70 7265 7669 6577 203d  = 100..preview =
+00000700: 2066 616c 7365 0d0a 0d0a 5b74 6f6f 6c2e   false....[tool.
+00000710: 6973 6f72 745d 0d0a 7072 6f66 696c 6520  isort]..profile 
+00000720: 3d20 2262 6c61 636b 220d 0a6c 696e 655f  = "black"..line_
+00000730: 6c65 6e67 7468 203d 2031 3030 0d0a 0d0a  length = 100....
+00000740: 5b74 6f6f 6c2e 7079 7465 7374 2e69 6e69  [tool.pytest.ini
+00000750: 5f6f 7074 696f 6e73 5d0d 0a6d 696e 7665  _options]..minve
+00000760: 7273 696f 6e20 3d20 372e 300d 0a74 6573  rsion = 7.0..tes
+00000770: 7470 6174 6873 203d 205b 0d0a 2020 2274  tpaths = [..  "t
+00000780: 6573 7473 220d 0a5d 0d0a 7079 7468 6f6e  ests"..]..python
+00000790: 5f66 696c 6573 203d 205b 2020 2320 6120  _files = [  # a 
+000007a0: 6c69 7374 206f 6620 7061 7474 6572 6e73  list of patterns
+000007b0: 2074 6f20 7573 6520 746f 2063 6f6c 6c65   to use to colle
+000007c0: 6374 2074 6573 7420 6d6f 6475 6c65 730d  ct test modules.
+000007d0: 0a20 2022 7465 7374 732f 7465 7374 5f2a  .  "tests/test_*
+000007e0: 2e70 7922 0d0a 5d0d 0a61 6464 6f70 7473  .py"..]..addopts
+000007f0: 203d 2022 2d2d 636f 763d 7377 6f6c 6670   = "--cov=swolfp
+00000800: 795f 696e 7075 7464 6174 6120 2d2d 636f  y_inputdata --co
+00000810: 762d 7265 706f 7274 3d78 6d6c 202d 2d64  v-report=xml --d
+00000820: 6973 6162 6c65 2d77 6172 6e69 6e67 7320  isable-warnings 
+00000830: 2d2d 6967 6e6f 7265 202a 2e63 7376 202d  --ignore *.csv -
+00000840: 2d63 6f6c 6f72 3d79 6573 220d 0a0d 0a23  -color=yes"....#
+00000850: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000860: 2323 2323 2323 2323 2323 2323 0d0a 2323  ############..##
+00000870: 2323 2323 2320 2020 2070 796c 696e 7420  #####    pylint 
+00000880: 2020 2020 2323 2323 2323 230d 0a23 2323      #######..###
+00000890: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000008a0: 2323 2323 2323 2323 2323 0d0a 2320 536f  ##########..# So
+000008b0: 7572 6365 2066 6f72 2070 796c 696e 7420  urce for pylint 
+000008c0: 7365 7474 696e 6773 3a20 6874 7470 733a  settings: https:
+000008d0: 2f2f 6769 7468 7562 2e63 6f6d 2f50 7943  //github.com/PyC
+000008e0: 5141 2f70 796c 696e 742f 626c 6f62 2f6d  QA/pylint/blob/m
+000008f0: 6169 6e2f 6578 616d 706c 6573 2f70 7970  ain/examples/pyp
+00000900: 726f 6a65 6374 2e74 6f6d 6c0d 0a0d 0a5b  roject.toml....[
+00000910: 746f 6f6c 2e70 796c 696e 742e 6d61 696e  tool.pylint.main
+00000920: 5d0d 0a23 2053 7065 6369 6679 2061 2073  ]..# Specify a s
+00000930: 636f 7265 2074 6872 6573 686f 6c64 2075  core threshold u
+00000940: 6e64 6572 2077 6869 6368 2074 6865 2070  nder which the p
+00000950: 726f 6772 616d 2077 696c 6c20 6578 6974  rogram will exit
+00000960: 2077 6974 6820 6572 726f 722e 0d0a 6661   with error...fa
+00000970: 696c 2d75 6e64 6572 203d 2031 300d 0a0d  il-under = 10...
+00000980: 0a23 2046 696c 6573 206f 7220 6469 7265  .# Files or dire
+00000990: 6374 6f72 6965 7320 746f 2062 6520 736b  ctories to be sk
+000009a0: 6970 7065 642e 2054 6865 7920 7368 6f75  ipped. They shou
+000009b0: 6c64 2062 6520 6261 7365 206e 616d 6573  ld be base names
+000009c0: 2c20 6e6f 7420 7061 7468 732e 0d0a 6967  , not paths...ig
+000009d0: 6e6f 7265 203d 205b 2243 5653 225d 0d0a  nore = ["CVS"]..
+000009e0: 0d0a 2320 4164 6420 6669 6c65 7320 6f72  ..# Add files or
+000009f0: 2064 6972 6563 746f 7269 6573 206d 6174   directories mat
+00000a00: 6368 696e 6720 7468 6520 7265 6775 6c61  ching the regula
+00000a10: 7220 6578 7072 6573 7369 6f6e 7320 7061  r expressions pa
+00000a20: 7474 6572 6e73 2074 6f20 7468 650d 0a23  tterns to the..#
+00000a30: 2069 676e 6f72 652d 6c69 7374 2e20 5468   ignore-list. Th
+00000a40: 6520 7265 6765 7820 6d61 7463 6865 7320  e regex matches 
+00000a50: 6167 6169 6e73 7420 7061 7468 7320 616e  against paths an
+00000a60: 6420 6361 6e20 6265 2069 6e20 506f 7369  d can be in Posi
+00000a70: 7820 6f72 2057 696e 646f 7773 0d0a 2320  x or Windows..# 
+00000a80: 666f 726d 6174 2e20 4265 6361 7573 6520  format. Because 
+00000a90: 275c 2720 7265 7072 6573 656e 7473 2074  '\' represents t
+00000aa0: 6865 2064 6972 6563 746f 7279 2064 656c  he directory del
+00000ab0: 696d 6974 6572 206f 6e20 5769 6e64 6f77  imiter on Window
+00000ac0: 7320 7379 7374 656d 732c 2069 740d 0a23  s systems, it..#
+00000ad0: 2063 616e 2774 2062 6520 7573 6564 2061   can't be used a
+00000ae0: 7320 616e 2065 7363 6170 6520 6368 6172  s an escape char
+00000af0: 6163 7465 722e 0d0a 2320 6967 6e6f 7265  acter...# ignore
+00000b00: 2d70 6174 6873 203d 0d0a 0d0a 2320 4669  -paths =....# Fi
+00000b10: 6c65 7320 6f72 2064 6972 6563 746f 7269  les or directori
+00000b20: 6573 206d 6174 6368 696e 6720 7468 6520  es matching the 
+00000b30: 7265 6775 6c61 7220 6578 7072 6573 7369  regular expressi
+00000b40: 6f6e 2070 6174 7465 726e 7320 6172 6520  on patterns are 
+00000b50: 736b 6970 7065 642e 2054 6865 0d0a 2320  skipped. The..# 
+00000b60: 7265 6765 7820 6d61 7463 6865 7320 6167  regex matches ag
+00000b70: 6169 6e73 7420 6261 7365 206e 616d 6573  ainst base names
+00000b80: 2c20 6e6f 7420 7061 7468 732e 2054 6865  , not paths. The
+00000b90: 2064 6566 6175 6c74 2076 616c 7565 2069   default value i
+00000ba0: 676e 6f72 6573 2045 6d61 6373 0d0a 2320  gnores Emacs..# 
+00000bb0: 6669 6c65 206c 6f63 6b73 0d0a 6967 6e6f  file locks..igno
+00000bc0: 7265 2d70 6174 7465 726e 7320 3d20 5b22  re-patterns = ["
+00000bd0: 5e5c 5c2e 2322 5d0d 0a0d 0a23 204c 6973  ^\\.#"]....# Lis
+00000be0: 7420 6f66 206d 6f64 756c 6520 6e61 6d65  t of module name
+00000bf0: 7320 666f 7220 7768 6963 6820 6d65 6d62  s for which memb
+00000c00: 6572 2061 7474 7269 6275 7465 7320 7368  er attributes sh
+00000c10: 6f75 6c64 206e 6f74 2062 6520 6368 6563  ould not be chec
+00000c20: 6b65 6420 2875 7365 6675 6c0d 0a23 2066  ked (useful..# f
+00000c30: 6f72 206d 6f64 756c 6573 2f70 726f 6a65  or modules/proje
+00000c40: 6374 7320 7768 6572 6520 6e61 6d65 7370  cts where namesp
+00000c50: 6163 6573 2061 7265 206d 616e 6970 756c  aces are manipul
+00000c60: 6174 6564 2064 7572 696e 6720 7275 6e74  ated during runt
+00000c70: 696d 6520 616e 6420 7468 7573 0d0a 2320  ime and thus..# 
+00000c80: 6578 6973 7469 6e67 206d 656d 6265 7220  existing member 
+00000c90: 6174 7472 6962 7574 6573 2063 616e 6e6f  attributes canno
+00000ca0: 7420 6265 2064 6564 7563 6564 2062 7920  t be deduced by 
+00000cb0: 7374 6174 6963 2061 6e61 6c79 7369 7329  static analysis)
+00000cc0: 2e20 4974 2073 7570 706f 7274 730d 0a23  . It supports..#
+00000cd0: 2071 7561 6c69 6669 6564 206d 6f64 756c   qualified modul
+00000ce0: 6520 6e61 6d65 732c 2061 7320 7765 6c6c  e names, as well
+00000cf0: 2061 7320 556e 6978 2070 6174 7465 726e   as Unix pattern
+00000d00: 206d 6174 6368 696e 672e 0d0a 2320 6967   matching...# ig
+00000d10: 6e6f 7265 642d 6d6f 6475 6c65 7320 3d0d  nored-modules =.
+00000d20: 0a0d 0a23 2055 7365 206d 756c 7469 706c  ...# Use multipl
+00000d30: 6520 7072 6f63 6573 7365 7320 746f 2073  e processes to s
+00000d40: 7065 6564 2075 7020 5079 6c69 6e74 2e20  peed up Pylint. 
+00000d50: 5370 6563 6966 7969 6e67 2030 2077 696c  Specifying 0 wil
+00000d60: 6c20 6175 746f 2d64 6574 6563 7420 7468  l auto-detect th
+00000d70: 650d 0a23 206e 756d 6265 7220 6f66 2070  e..# number of p
+00000d80: 726f 6365 7373 6f72 7320 6176 6169 6c61  rocessors availa
+00000d90: 626c 6520 746f 2075 7365 2c20 616e 6420  ble to use, and 
+00000da0: 7769 6c6c 2063 6170 2074 6865 2063 6f75  will cap the cou
+00000db0: 6e74 206f 6e20 5769 6e64 6f77 7320 746f  nt on Windows to
+00000dc0: 0d0a 2320 6176 6f69 6420 6861 6e67 732e  ..# avoid hangs.
+00000dd0: 0d0a 6a6f 6273 203d 2032 0d0a 0d0a 2320  ..jobs = 2....# 
+00000de0: 436f 6e74 726f 6c20 7468 6520 616d 6f75  Control the amou
+00000df0: 6e74 206f 6620 706f 7465 6e74 6961 6c20  nt of potential 
+00000e00: 696e 6665 7272 6564 2076 616c 7565 7320  inferred values 
+00000e10: 7768 656e 2069 6e66 6572 7269 6e67 2061  when inferring a
+00000e20: 2073 696e 676c 6520 6f62 6a65 6374 2e0d   single object..
+00000e30: 0a23 2054 6869 7320 6361 6e20 6865 6c70  .# This can help
+00000e40: 2074 6865 2070 6572 666f 726d 616e 6365   the performance
+00000e50: 2077 6865 6e20 6465 616c 696e 6720 7769   when dealing wi
+00000e60: 7468 206c 6172 6765 2066 756e 6374 696f  th large functio
+00000e70: 6e73 206f 7220 636f 6d70 6c65 782c 0d0a  ns or complex,..
+00000e80: 2320 6e65 7374 6564 2063 6f6e 6469 7469  # nested conditi
+00000e90: 6f6e 732e 0d0a 6c69 6d69 742d 696e 6665  ons...limit-infe
+00000ea0: 7265 6e63 652d 7265 7375 6c74 7320 3d20  rence-results = 
+00000eb0: 3130 300d 0a0d 0a23 2050 6963 6b6c 6520  100....# Pickle 
+00000ec0: 636f 6c6c 6563 7465 6420 6461 7461 2066  collected data f
+00000ed0: 6f72 206c 6174 6572 2063 6f6d 7061 7269  or later compari
+00000ee0: 736f 6e73 2e0d 0a70 6572 7369 7374 656e  sons...persisten
+00000ef0: 7420 3d20 7472 7565 0d0a 0d0a 2320 5768  t = true....# Wh
+00000f00: 656e 2065 6e61 626c 6564 2c20 7079 6c69  en enabled, pyli
+00000f10: 6e74 2077 6f75 6c64 2061 7474 656d 7074  nt would attempt
+00000f20: 2074 6f20 6775 6573 7320 636f 6d6d 6f6e   to guess common
+00000f30: 206d 6973 636f 6e66 6967 7572 6174 696f   misconfiguratio
+00000f40: 6e20 616e 6420 656d 6974 0d0a 2320 7573  n and emit..# us
+00000f50: 6572 2d66 7269 656e 646c 7920 6869 6e74  er-friendly hint
+00000f60: 7320 696e 7374 6561 6420 6f66 2066 616c  s instead of fal
+00000f70: 7365 2d70 6f73 6974 6976 6520 6572 726f  se-positive erro
+00000f80: 7220 6d65 7373 6167 6573 2e0d 0a73 7567  r messages...sug
+00000f90: 6765 7374 696f 6e2d 6d6f 6465 203d 2074  gestion-mode = t
+00000fa0: 7275 650d 0a0d 0a5b 746f 6f6c 2e70 796c  rue....[tool.pyl
+00000fb0: 696e 742e 6261 7369 635d 0d0a 2320 4e61  int.basic]..# Na
+00000fc0: 6d69 6e67 2073 7479 6c65 206d 6174 6368  ming style match
+00000fd0: 696e 6720 636f 7272 6563 7420 6172 6775  ing correct argu
+00000fe0: 6d65 6e74 206e 616d 6573 2e0d 0a61 7267  ment names...arg
+00000ff0: 756d 656e 742d 6e61 6d69 6e67 2d73 7479  ument-naming-sty
+00001000: 6c65 203d 2022 736e 616b 655f 6361 7365  le = "snake_case
+00001010: 220d 0a0d 0a23 204e 616d 696e 6720 7374  "....# Naming st
+00001020: 796c 6520 6d61 7463 6869 6e67 2063 6f72  yle matching cor
+00001030: 7265 6374 2061 7474 7269 6275 7465 206e  rect attribute n
+00001040: 616d 6573 2e0d 0a61 7474 722d 6e61 6d69  ames...attr-nami
+00001050: 6e67 2d73 7479 6c65 203d 2022 736e 616b  ng-style = "snak
+00001060: 655f 6361 7365 220d 0a0d 0a23 2042 6164  e_case"....# Bad
+00001070: 2076 6172 6961 626c 6520 6e61 6d65 7320   variable names 
+00001080: 7768 6963 6820 7368 6f75 6c64 2061 6c77  which should alw
+00001090: 6179 7320 6265 2072 6566 7573 6564 2c20  ays be refused, 
+000010a0: 7365 7061 7261 7465 6420 6279 2061 2063  separated by a c
+000010b0: 6f6d 6d61 2e0d 0a62 6164 2d6e 616d 6573  omma...bad-names
+000010c0: 203d 205b 2266 6f6f 222c 2022 6261 7222   = ["foo", "bar"
+000010d0: 2c20 2262 617a 222c 2022 746f 746f 222c  , "baz", "toto",
+000010e0: 2022 7475 7475 222c 2022 7461 7461 225d   "tutu", "tata"]
+000010f0: 0d0a 0d0a 2320 4e61 6d69 6e67 2073 7479  ....# Naming sty
+00001100: 6c65 206d 6174 6368 696e 6720 636f 7272  le matching corr
+00001110: 6563 7420 636c 6173 7320 6174 7472 6962  ect class attrib
+00001120: 7574 6520 6e61 6d65 732e 0d0a 636c 6173  ute names...clas
+00001130: 732d 6174 7472 6962 7574 652d 6e61 6d69  s-attribute-nami
+00001140: 6e67 2d73 7479 6c65 203d 2022 616e 7922  ng-style = "any"
+00001150: 0d0a 0d0a 2320 4e61 6d69 6e67 2073 7479  ....# Naming sty
+00001160: 6c65 206d 6174 6368 696e 6720 636f 7272  le matching corr
+00001170: 6563 7420 636c 6173 7320 636f 6e73 7461  ect class consta
+00001180: 6e74 206e 616d 6573 2e0d 0a63 6c61 7373  nt names...class
+00001190: 2d63 6f6e 7374 2d6e 616d 696e 672d 7374  -const-naming-st
+000011a0: 796c 6520 3d20 2255 5050 4552 5f43 4153  yle = "UPPER_CAS
+000011b0: 4522 0d0a 0d0a 2320 4e61 6d69 6e67 2073  E"....# Naming s
+000011c0: 7479 6c65 206d 6174 6368 696e 6720 636f  tyle matching co
+000011d0: 7272 6563 7420 636c 6173 7320 6e61 6d65  rrect class name
+000011e0: 732e 0d0a 636c 6173 732d 6e61 6d69 6e67  s...class-naming
+000011f0: 2d73 7479 6c65 203d 2022 5061 7363 616c  -style = "Pascal
+00001200: 4361 7365 220d 0a0d 0a23 204e 616d 696e  Case"....# Namin
+00001210: 6720 7374 796c 6520 6d61 7463 6869 6e67  g style matching
+00001220: 2063 6f72 7265 6374 2063 6f6e 7374 616e   correct constan
+00001230: 7420 6e61 6d65 732e 0d0a 636f 6e73 742d  t names...const-
+00001240: 6e61 6d69 6e67 2d73 7479 6c65 203d 2022  naming-style = "
+00001250: 5550 5045 525f 4341 5345 220d 0a0d 0a23  UPPER_CASE"....#
+00001260: 204d 696e 696d 756d 206c 696e 6520 6c65   Minimum line le
+00001270: 6e67 7468 2066 6f72 2066 756e 6374 696f  ngth for functio
+00001280: 6e73 2f63 6c61 7373 6573 2074 6861 7420  ns/classes that 
+00001290: 7265 7175 6972 6520 646f 6373 7472 696e  require docstrin
+000012a0: 6773 2c20 7368 6f72 7465 7220 6f6e 6573  gs, shorter ones
+000012b0: 0d0a 2320 6172 6520 6578 656d 7074 2e0d  ..# are exempt..
+000012c0: 0a64 6f63 7374 7269 6e67 2d6d 696e 2d6c  .docstring-min-l
+000012d0: 656e 6774 6820 3d20 2d31 0d0a 0d0a 2320  ength = -1....# 
+000012e0: 4e61 6d69 6e67 2073 7479 6c65 206d 6174  Naming style mat
+000012f0: 6368 696e 6720 636f 7272 6563 7420 6675  ching correct fu
+00001300: 6e63 7469 6f6e 206e 616d 6573 2e0d 0a66  nction names...f
+00001310: 756e 6374 696f 6e2d 6e61 6d69 6e67 2d73  unction-naming-s
+00001320: 7479 6c65 203d 2022 736e 616b 655f 6361  tyle = "snake_ca
+00001330: 7365 220d 0a0d 0a23 2047 6f6f 6420 7661  se"....# Good va
+00001340: 7269 6162 6c65 206e 616d 6573 2077 6869  riable names whi
+00001350: 6368 2073 686f 756c 6420 616c 7761 7973  ch should always
+00001360: 2062 6520 6163 6365 7074 6564 2c20 7365   be accepted, se
+00001370: 7061 7261 7465 6420 6279 2061 2063 6f6d  parated by a com
+00001380: 6d61 2e0d 0a67 6f6f 642d 6e61 6d65 7320  ma...good-names 
+00001390: 3d20 5b22 6922 2c20 226a 222c 2022 6b22  = ["i", "j", "k"
+000013a0: 2c20 2265 7822 2c20 2252 756e 222c 2022  , "ex", "Run", "
+000013b0: 5f22 5d0d 0a0d 0a23 204e 616d 696e 6720  _"]....# Naming 
+000013c0: 7374 796c 6520 6d61 7463 6869 6e67 2063  style matching c
+000013d0: 6f72 7265 6374 206d 6574 686f 6420 6e61  orrect method na
+000013e0: 6d65 732e 0d0a 6d65 7468 6f64 2d6e 616d  mes...method-nam
+000013f0: 696e 672d 7374 796c 6520 3d20 2273 6e61  ing-style = "sna
+00001400: 6b65 5f63 6173 6522 0d0a 0d0a 2320 4e61  ke_case"....# Na
+00001410: 6d69 6e67 2073 7479 6c65 206d 6174 6368  ming style match
+00001420: 696e 6720 636f 7272 6563 7420 6d6f 6475  ing correct modu
+00001430: 6c65 206e 616d 6573 2e0d 0a6d 6f64 756c  le names...modul
+00001440: 652d 6e61 6d69 6e67 2d73 7479 6c65 203d  e-naming-style =
+00001450: 2022 736e 616b 655f 6361 7365 220d 0a0d   "snake_case"...
+00001460: 0a23 2052 6567 756c 6172 2065 7870 7265  .# Regular expre
+00001470: 7373 696f 6e20 7768 6963 6820 7368 6f75  ssion which shou
+00001480: 6c64 206f 6e6c 7920 6d61 7463 6820 6675  ld only match fu
+00001490: 6e63 7469 6f6e 206f 7220 636c 6173 7320  nction or class 
+000014a0: 6e61 6d65 7320 7468 6174 2064 6f20 6e6f  names that do no
+000014b0: 740d 0a23 2072 6571 7569 7265 2061 2064  t..# require a d
+000014c0: 6f63 7374 7269 6e67 2e0d 0a6e 6f2d 646f  ocstring...no-do
+000014d0: 6373 7472 696e 672d 7267 7820 3d20 225e  cstring-rgx = "^
+000014e0: 5f22 0d0a 0d0a 2320 4c69 7374 206f 6620  _"....# List of 
+000014f0: 6465 636f 7261 746f 7273 2074 6861 7420  decorators that 
+00001500: 7072 6f64 7563 6520 7072 6f70 6572 7469  produce properti
+00001510: 6573 2c20 7375 6368 2061 7320 6162 632e  es, such as abc.
+00001520: 6162 7374 7261 6374 7072 6f70 6572 7479  abstractproperty
+00001530: 2e20 4164 640d 0a23 2074 6f20 7468 6973  . Add..# to this
+00001540: 206c 6973 7420 746f 2072 6567 6973 7465   list to registe
+00001550: 7220 6f74 6865 7220 6465 636f 7261 746f  r other decorato
+00001560: 7273 2074 6861 7420 7072 6f64 7563 6520  rs that produce 
+00001570: 7661 6c69 6420 7072 6f70 6572 7469 6573  valid properties
+00001580: 2e20 5468 6573 650d 0a23 2064 6563 6f72  . These..# decor
+00001590: 6174 6f72 7320 6172 6520 7461 6b65 6e20  ators are taken 
+000015a0: 696e 2063 6f6e 7369 6465 7261 7469 6f6e  in consideration
+000015b0: 206f 6e6c 7920 666f 7220 696e 7661 6c69   only for invali
+000015c0: 642d 6e61 6d65 2e0d 0a70 726f 7065 7274  d-name...propert
+000015d0: 792d 636c 6173 7365 7320 3d20 5b22 6162  y-classes = ["ab
+000015e0: 632e 6162 7374 7261 6374 7072 6f70 6572  c.abstractproper
+000015f0: 7479 225d 0d0a 0d0a 2320 4e61 6d69 6e67  ty"]....# Naming
+00001600: 2073 7479 6c65 206d 6174 6368 696e 6720   style matching 
+00001610: 636f 7272 6563 7420 7661 7269 6162 6c65  correct variable
+00001620: 206e 616d 6573 2e0d 0a76 6172 6961 626c   names...variabl
+00001630: 652d 6e61 6d69 6e67 2d73 7479 6c65 203d  e-naming-style =
+00001640: 2022 736e 616b 655f 6361 7365 220d 0a0d   "snake_case"...
+00001650: 0a5b 746f 6f6c 2e70 796c 696e 742e 636c  .[tool.pylint.cl
+00001660: 6173 7365 735d 0d0a 2320 5761 726e 2061  asses]..# Warn a
+00001670: 626f 7574 2070 726f 7465 6374 6564 2061  bout protected a
+00001680: 7474 7269 6275 7465 2061 6363 6573 7320  ttribute access 
+00001690: 696e 7369 6465 2073 7065 6369 616c 206d  inside special m
+000016a0: 6574 686f 6473 0d0a 2320 6368 6563 6b2d  ethods..# check-
+000016b0: 7072 6f74 6563 7465 642d 6163 6365 7373  protected-access
+000016c0: 2d69 6e2d 7370 6563 6961 6c2d 6d65 7468  -in-special-meth
+000016d0: 6f64 7320 3d0d 0a0d 0a23 204c 6973 7420  ods =....# List 
+000016e0: 6f66 206d 6574 686f 6420 6e61 6d65 7320  of method names 
+000016f0: 7573 6564 2074 6f20 6465 636c 6172 6520  used to declare 
+00001700: 2869 2e65 2e20 6173 7369 676e 2920 696e  (i.e. assign) in
+00001710: 7374 616e 6365 2061 7474 7269 6275 7465  stance attribute
+00001720: 732e 0d0a 6465 6669 6e69 6e67 2d61 7474  s...defining-att
+00001730: 722d 6d65 7468 6f64 7320 3d20 5b22 5f5f  r-methods = ["__
+00001740: 696e 6974 5f5f 222c 2022 5f5f 6e65 775f  init__", "__new_
+00001750: 5f22 2c20 2273 6574 5570 222c 2022 5f5f  _", "setUp", "__
+00001760: 706f 7374 5f69 6e69 745f 5f22 5d0d 0a0d  post_init__"]...
+00001770: 0a23 204c 6973 7420 6f66 206d 656d 6265  .# List of membe
+00001780: 7220 6e61 6d65 732c 2077 6869 6368 2073  r names, which s
+00001790: 686f 756c 6420 6265 2065 7863 6c75 6465  hould be exclude
+000017a0: 6420 6672 6f6d 2074 6865 2070 726f 7465  d from the prote
+000017b0: 6374 6564 2061 6363 6573 730d 0a23 2077  cted access..# w
+000017c0: 6172 6e69 6e67 2e0d 0a65 7863 6c75 6465  arning...exclude
+000017d0: 2d70 726f 7465 6374 6564 203d 205b 225f  -protected = ["_
+000017e0: 6173 6469 6374 222c 2022 5f66 6965 6c64  asdict", "_field
+000017f0: 7322 2c20 225f 7265 706c 6163 6522 2c20  s", "_replace", 
+00001800: 225f 736f 7572 6365 222c 2022 5f6d 616b  "_source", "_mak
+00001810: 6522 5d0d 0a0d 0a23 204c 6973 7420 6f66  e"]....# List of
+00001820: 2076 616c 6964 206e 616d 6573 2066 6f72   valid names for
+00001830: 2074 6865 2066 6972 7374 2061 7267 756d   the first argum
+00001840: 656e 7420 696e 2061 2063 6c61 7373 206d  ent in a class m
+00001850: 6574 686f 642e 0d0a 7661 6c69 642d 636c  ethod...valid-cl
+00001860: 6173 736d 6574 686f 642d 6669 7273 742d  assmethod-first-
+00001870: 6172 6720 3d20 5b22 636c 7322 5d0d 0a0d  arg = ["cls"]...
+00001880: 0a23 204c 6973 7420 6f66 2076 616c 6964  .# List of valid
+00001890: 206e 616d 6573 2066 6f72 2074 6865 2066   names for the f
+000018a0: 6972 7374 2061 7267 756d 656e 7420 696e  irst argument in
+000018b0: 2061 206d 6574 6163 6c61 7373 2063 6c61   a metaclass cla
+000018c0: 7373 206d 6574 686f 642e 0d0a 7661 6c69  ss method...vali
+000018d0: 642d 6d65 7461 636c 6173 732d 636c 6173  d-metaclass-clas
+000018e0: 736d 6574 686f 642d 6669 7273 742d 6172  smethod-first-ar
+000018f0: 6720 3d20 5b22 6d63 7322 5d0d 0a0d 0a5b  g = ["mcs"]....[
+00001900: 746f 6f6c 2e70 796c 696e 742e 6465 7369  tool.pylint.desi
+00001910: 676e 5d0d 0a23 204d 6178 696d 756d 206e  gn]..# Maximum n
+00001920: 756d 6265 7220 6f66 2061 7267 756d 656e  umber of argumen
+00001930: 7473 2066 6f72 2066 756e 6374 696f 6e20  ts for function 
+00001940: 2f20 6d65 7468 6f64 2e0d 0a6d 6178 2d61  / method...max-a
+00001950: 7267 7320 3d20 350d 0a0d 0a23 204d 6178  rgs = 5....# Max
+00001960: 696d 756d 206e 756d 6265 7220 6f66 2061  imum number of a
+00001970: 7474 7269 6275 7465 7320 666f 7220 6120  ttributes for a 
+00001980: 636c 6173 7320 2873 6565 2052 3039 3032  class (see R0902
+00001990: 292e 0d0a 6d61 782d 6174 7472 6962 7574  )...max-attribut
+000019a0: 6573 203d 2037 0d0a 0d0a 2320 4d61 7869  es = 7....# Maxi
+000019b0: 6d75 6d20 6e75 6d62 6572 206f 6620 626f  mum number of bo
+000019c0: 6f6c 6561 6e20 6578 7072 6573 7369 6f6e  olean expression
+000019d0: 7320 696e 2061 6e20 6966 2073 7461 7465  s in an if state
+000019e0: 6d65 6e74 2028 7365 6520 5230 3931 3629  ment (see R0916)
+000019f0: 2e0d 0a6d 6178 2d62 6f6f 6c2d 6578 7072  ...max-bool-expr
+00001a00: 203d 2035 0d0a 0d0a 2320 4d61 7869 6d75   = 5....# Maximu
+00001a10: 6d20 6e75 6d62 6572 206f 6620 6272 616e  m number of bran
+00001a20: 6368 2066 6f72 2066 756e 6374 696f 6e20  ch for function 
+00001a30: 2f20 6d65 7468 6f64 2062 6f64 792e 0d0a  / method body...
+00001a40: 6d61 782d 6272 616e 6368 6573 203d 2031  max-branches = 1
+00001a50: 320d 0a0d 0a23 204d 6178 696d 756d 206e  2....# Maximum n
+00001a60: 756d 6265 7220 6f66 206c 6f63 616c 7320  umber of locals 
+00001a70: 666f 7220 6675 6e63 7469 6f6e 202f 206d  for function / m
+00001a80: 6574 686f 6420 626f 6479 2e0d 0a6d 6178  ethod body...max
+00001a90: 2d6c 6f63 616c 7320 3d20 3135 0d0a 0d0a  -locals = 15....
+00001aa0: 2320 4d61 7869 6d75 6d20 6e75 6d62 6572  # Maximum number
+00001ab0: 206f 6620 7061 7265 6e74 7320 666f 7220   of parents for 
+00001ac0: 6120 636c 6173 7320 2873 6565 2052 3039  a class (see R09
+00001ad0: 3031 292e 0d0a 6d61 782d 7061 7265 6e74  01)...max-parent
+00001ae0: 7320 3d20 370d 0a0d 0a23 204d 6178 696d  s = 7....# Maxim
+00001af0: 756d 206e 756d 6265 7220 6f66 2070 7562  um number of pub
+00001b00: 6c69 6320 6d65 7468 6f64 7320 666f 7220  lic methods for 
+00001b10: 6120 636c 6173 7320 2873 6565 2052 3039  a class (see R09
+00001b20: 3034 292e 0d0a 6d61 782d 7075 626c 6963  04)...max-public
+00001b30: 2d6d 6574 686f 6473 203d 2032 300d 0a0d  -methods = 20...
+00001b40: 0a23 204d 6178 696d 756d 206e 756d 6265  .# Maximum numbe
+00001b50: 7220 6f66 2072 6574 7572 6e20 2f20 7969  r of return / yi
+00001b60: 656c 6420 666f 7220 6675 6e63 7469 6f6e  eld for function
+00001b70: 202f 206d 6574 686f 6420 626f 6479 2e0d   / method body..
+00001b80: 0a6d 6178 2d72 6574 7572 6e73 203d 2036  .max-returns = 6
+00001b90: 0d0a 0d0a 2320 4d61 7869 6d75 6d20 6e75  ....# Maximum nu
+00001ba0: 6d62 6572 206f 6620 7374 6174 656d 656e  mber of statemen
+00001bb0: 7473 2069 6e20 6675 6e63 7469 6f6e 202f  ts in function /
+00001bc0: 206d 6574 686f 6420 626f 6479 2e0d 0a6d   method body...m
+00001bd0: 6178 2d73 7461 7465 6d65 6e74 7320 3d20  ax-statements = 
+00001be0: 3530 0d0a 0d0a 2320 4d69 6e69 6d75 6d20  50....# Minimum 
+00001bf0: 6e75 6d62 6572 206f 6620 7075 626c 6963  number of public
+00001c00: 206d 6574 686f 6473 2066 6f72 2061 2063   methods for a c
+00001c10: 6c61 7373 2028 7365 6520 5230 3930 3329  lass (see R0903)
+00001c20: 2e0d 0a6d 696e 2d70 7562 6c69 632d 6d65  ...min-public-me
+00001c30: 7468 6f64 7320 3d20 310d 0a0d 0a5b 746f  thods = 1....[to
+00001c40: 6f6c 2e70 796c 696e 742e 6578 6365 7074  ol.pylint.except
+00001c50: 696f 6e73 5d0d 0a23 2045 7863 6570 7469  ions]..# Excepti
+00001c60: 6f6e 7320 7468 6174 2077 696c 6c20 656d  ons that will em
+00001c70: 6974 2061 2077 6172 6e69 6e67 2077 6865  it a warning whe
+00001c80: 6e20 6361 7567 6874 2e0d 0a6f 7665 7267  n caught...overg
+00001c90: 656e 6572 616c 2d65 7863 6570 7469 6f6e  eneral-exception
+00001ca0: 7320 3d20 5b22 6275 696c 7469 6e73 2e42  s = ["builtins.B
+00001cb0: 6173 6545 7863 6570 7469 6f6e 222c 2022  aseException", "
+00001cc0: 6275 696c 7469 6e73 2e45 7863 6570 7469  builtins.Excepti
+00001cd0: 6f6e 225d 0d0a 0d0a 5b74 6f6f 6c2e 7079  on"]....[tool.py
+00001ce0: 6c69 6e74 2e66 6f72 6d61 745d 0d0a 2320  lint.format]..# 
+00001cf0: 5265 6765 7870 2066 6f72 2061 206c 696e  Regexp for a lin
+00001d00: 6520 7468 6174 2069 7320 616c 6c6f 7765  e that is allowe
+00001d10: 6420 746f 2062 6520 6c6f 6e67 6572 2074  d to be longer t
+00001d20: 6861 6e20 7468 6520 6c69 6d69 742e 0d0a  han the limit...
+00001d30: 6967 6e6f 7265 2d6c 6f6e 672d 6c69 6e65  ignore-long-line
+00001d40: 7320 3d20 225e 5c5c 732a 2823 2029 3f3c  s = "^\\s*(# )?<
+00001d50: 3f68 7474 7073 3f3a 2f2f 5c5c 532b 3e3f  ?https?://\\S+>?
+00001d60: 2422 0d0a 0d0a 2320 4e75 6d62 6572 206f  $"....# Number o
+00001d70: 6620 7370 6163 6573 206f 6620 696e 6465  f spaces of inde
+00001d80: 6e74 2072 6571 7569 7265 6420 696e 7369  nt required insi
+00001d90: 6465 2061 2068 616e 6769 6e67 206f 7220  de a hanging or 
+00001da0: 636f 6e74 696e 7565 6420 6c69 6e65 2e0d  continued line..
+00001db0: 0a69 6e64 656e 742d 6166 7465 722d 7061  .indent-after-pa
+00001dc0: 7265 6e20 3d20 340d 0a0d 0a23 2053 7472  ren = 4....# Str
+00001dd0: 696e 6720 7573 6564 2061 7320 696e 6465  ing used as inde
+00001de0: 6e74 6174 696f 6e20 756e 6974 2e20 5468  ntation unit. Th
+00001df0: 6973 2069 7320 7573 7561 6c6c 7920 2220  is is usually " 
+00001e00: 2020 2022 2028 3420 7370 6163 6573 2920     " (4 spaces) 
+00001e10: 6f72 2022 5c74 2220 2831 0d0a 2320 7461  or "\t" (1..# ta
+00001e20: 6229 2e0d 0a69 6e64 656e 742d 7374 7269  b)...indent-stri
+00001e30: 6e67 203d 2022 2020 2020 220d 0a0d 0a23  ng = "    "....#
+00001e40: 204d 6178 696d 756d 206e 756d 6265 7220   Maximum number 
+00001e50: 6f66 2063 6861 7261 6374 6572 7320 6f6e  of characters on
+00001e60: 2061 2073 696e 676c 6520 6c69 6e65 2e0d   a single line..
+00001e70: 0a6d 6178 2d6c 696e 652d 6c65 6e67 7468  .max-line-length
+00001e80: 203d 2031 3030 0d0a 0d0a 2320 4d61 7869   = 100....# Maxi
+00001e90: 6d75 6d20 6e75 6d62 6572 206f 6620 6c69  mum number of li
+00001ea0: 6e65 7320 696e 2061 206d 6f64 756c 652e  nes in a module.
+00001eb0: 0d0a 6d61 782d 6d6f 6475 6c65 2d6c 696e  ..max-module-lin
+00001ec0: 6573 203d 2031 3030 300d 0a0d 0a5b 746f  es = 1000....[to
+00001ed0: 6f6c 2e70 796c 696e 742e 6d69 7363 656c  ol.pylint.miscel
+00001ee0: 6c61 6e65 6f75 735d 0d0a 2320 4c69 7374  laneous]..# List
+00001ef0: 206f 6620 6e6f 7465 2074 6167 7320 746f   of note tags to
+00001f00: 2074 616b 6520 696e 2063 6f6e 7369 6465   take in conside
+00001f10: 7261 7469 6f6e 2c20 7365 7061 7261 7465  ration, separate
+00001f20: 6420 6279 2061 2063 6f6d 6d61 2e0d 0a6e  d by a comma...n
+00001f30: 6f74 6573 203d 205b 2246 4958 4d45 222c  otes = ["FIXME",
+00001f40: 2022 5858 5822 2c20 2254 4f44 4f22 5d0d   "XXX", "TODO"].
+00001f50: 0a0d 0a5b 746f 6f6c 2e70 796c 696e 742e  ...[tool.pylint.
+00001f60: 7265 6661 6374 6f72 696e 675d 0d0a 2320  refactoring]..# 
+00001f70: 4d61 7869 6d75 6d20 6e75 6d62 6572 206f  Maximum number o
+00001f80: 6620 6e65 7374 6564 2062 6c6f 636b 7320  f nested blocks 
+00001f90: 666f 7220 6675 6e63 7469 6f6e 202f 206d  for function / m
+00001fa0: 6574 686f 6420 626f 6479 0d0a 6d61 782d  ethod body..max-
+00001fb0: 6e65 7374 6564 2d62 6c6f 636b 7320 3d20  nested-blocks = 
+00001fc0: 350d 0a0d 0a23 2043 6f6d 706c 6574 6520  5....# Complete 
+00001fd0: 6e61 6d65 206f 6620 6675 6e63 7469 6f6e  name of function
+00001fe0: 7320 7468 6174 206e 6576 6572 2072 6574  s that never ret
+00001ff0: 7572 6e73 2e20 5768 656e 2063 6865 636b  urns. When check
+00002000: 696e 6720 666f 7220 696e 636f 6e73 6973  ing for inconsis
+00002010: 7465 6e74 2d0d 0a23 2072 6574 7572 6e2d  tent-..# return-
+00002020: 7374 6174 656d 656e 7473 2069 6620 6120  statements if a 
+00002030: 6e65 7665 7220 7265 7475 726e 696e 6720  never returning 
+00002040: 6675 6e63 7469 6f6e 2069 7320 6361 6c6c  function is call
+00002050: 6564 2074 6865 6e20 6974 2077 696c 6c20  ed then it will 
+00002060: 6265 0d0a 2320 636f 6e73 6964 6572 6564  be..# considered
+00002070: 2061 7320 616e 2065 7870 6c69 6369 7420   as an explicit 
+00002080: 7265 7475 726e 2073 7461 7465 6d65 6e74  return statement
+00002090: 2061 6e64 206e 6f20 6d65 7373 6167 6520   and no message 
+000020a0: 7769 6c6c 2062 6520 7072 696e 7465 642e  will be printed.
+000020b0: 0d0a 6e65 7665 722d 7265 7475 726e 696e  ..never-returnin
+000020c0: 672d 6675 6e63 7469 6f6e 7320 3d20 5b22  g-functions = ["
+000020d0: 7379 732e 6578 6974 222c 2022 6172 6770  sys.exit", "argp
+000020e0: 6172 7365 2e70 6172 7365 5f65 7272 6f72  arse.parse_error
+000020f0: 225d 0d0a 0d0a 5b74 6f6f 6c2e 7079 6c69  "]....[tool.pyli
+00002100: 6e74 2e73 696d 696c 6172 6974 6965 735d  nt.similarities]
+00002110: 0d0a 2320 436f 6d6d 656e 7473 2061 7265  ..# Comments are
+00002120: 2072 656d 6f76 6564 2066 726f 6d20 7468   removed from th
+00002130: 6520 7369 6d69 6c61 7269 7479 2063 6f6d  e similarity com
+00002140: 7075 7461 7469 6f6e 0d0a 6967 6e6f 7265  putation..ignore
+00002150: 2d63 6f6d 6d65 6e74 7320 3d20 7472 7565  -comments = true
+00002160: 0d0a 0d0a 2320 446f 6373 7472 696e 6773  ....# Docstrings
+00002170: 2061 7265 2072 656d 6f76 6564 2066 726f   are removed fro
+00002180: 6d20 7468 6520 7369 6d69 6c61 7269 7479  m the similarity
+00002190: 2063 6f6d 7075 7461 7469 6f6e 0d0a 6967   computation..ig
+000021a0: 6e6f 7265 2d64 6f63 7374 7269 6e67 7320  nore-docstrings 
+000021b0: 3d20 7472 7565 0d0a 0d0a 2320 496d 706f  = true....# Impo
+000021c0: 7274 7320 6172 6520 7265 6d6f 7665 6420  rts are removed 
+000021d0: 6672 6f6d 2074 6865 2073 696d 696c 6172  from the similar
+000021e0: 6974 7920 636f 6d70 7574 6174 696f 6e0d  ity computation.
+000021f0: 0a69 676e 6f72 652d 696d 706f 7274 7320  .ignore-imports 
+00002200: 3d20 7472 7565 0d0a 0d0a 2320 5369 676e  = true....# Sign
+00002210: 6174 7572 6573 2061 7265 2072 656d 6f76  atures are remov
+00002220: 6564 2066 726f 6d20 7468 6520 7369 6d69  ed from the simi
+00002230: 6c61 7269 7479 2063 6f6d 7075 7461 7469  larity computati
+00002240: 6f6e 0d0a 6967 6e6f 7265 2d73 6967 6e61  on..ignore-signa
+00002250: 7475 7265 7320 3d20 7472 7565 0d0a 0d0a  tures = true....
+00002260: 2320 4d69 6e69 6d75 6d20 6c69 6e65 7320  # Minimum lines 
+00002270: 6e75 6d62 6572 206f 6620 6120 7369 6d69  number of a simi
+00002280: 6c61 7269 7479 2e0d 0a6d 696e 2d73 696d  larity...min-sim
+00002290: 696c 6172 6974 792d 6c69 6e65 7320 3d20  ilarity-lines = 
+000022a0: 380d 0a0d 0a5b 746f 6f6c 2e70 796c 696e  8....[tool.pylin
+000022b0: 742e 7370 656c 6c69 6e67 5d0d 0a23 204c  t.spelling]..# L
+000022c0: 696d 6974 7320 636f 756e 7420 6f66 2065  imits count of e
+000022d0: 6d69 7474 6564 2073 7567 6765 7374 696f  mitted suggestio
+000022e0: 6e73 2066 6f72 2073 7065 6c6c 696e 6720  ns for spelling 
+000022f0: 6d69 7374 616b 6573 2e0d 0a6d 6178 2d73  mistakes...max-s
+00002300: 7065 6c6c 696e 672d 7375 6767 6573 7469  pelling-suggesti
+00002310: 6f6e 7320 3d20 340d 0a0d 0a5b 746f 6f6c  ons = 4....[tool
+00002320: 2e70 796c 696e 742e 7661 7269 6162 6c65  .pylint.variable
+00002330: 735d 0d0a 2320 5465 6c6c 7320 7768 6574  s]..# Tells whet
+00002340: 6865 7220 756e 7573 6564 2067 6c6f 6261  her unused globa
+00002350: 6c20 7661 7269 6162 6c65 7320 7368 6f75  l variables shou
+00002360: 6c64 2062 6520 7472 6561 7465 6420 6173  ld be treated as
+00002370: 2061 2076 696f 6c61 7469 6f6e 2e0d 0a61   a violation...a
+00002380: 6c6c 6f77 2d67 6c6f 6261 6c2d 756e 7573  llow-global-unus
+00002390: 6564 2d76 6172 6961 626c 6573 203d 2074  ed-variables = t
+000023a0: 7275 650d 0a0d 0a23 204c 6973 7420 6f66  rue....# List of
+000023b0: 2073 7472 696e 6773 2077 6869 6368 2063   strings which c
+000023c0: 616e 2069 6465 6e74 6966 7920 6120 6361  an identify a ca
+000023d0: 6c6c 6261 636b 2066 756e 6374 696f 6e20  llback function 
+000023e0: 6279 206e 616d 652e 2041 2063 616c 6c62  by name. A callb
+000023f0: 6163 6b20 6e61 6d65 0d0a 2320 6d75 7374  ack name..# must
+00002400: 2073 7461 7274 206f 7220 656e 6420 7769   start or end wi
+00002410: 7468 206f 6e65 206f 6620 7468 6f73 6520  th one of those 
+00002420: 7374 7269 6e67 732e 0d0a 6361 6c6c 6261  strings...callba
+00002430: 636b 7320 3d20 5b22 6362 5f22 2c20 225f  cks = ["cb_", "_
+00002440: 6362 225d 0d0a 0d0a 2320 4120 7265 6775  cb"]....# A regu
+00002450: 6c61 7220 6578 7072 6573 7369 6f6e 206d  lar expression m
+00002460: 6174 6368 696e 6720 7468 6520 6e61 6d65  atching the name
+00002470: 206f 6620 6475 6d6d 7920 7661 7269 6162   of dummy variab
+00002480: 6c65 7320 2869 2e65 2e20 6578 7065 6374  les (i.e. expect
+00002490: 6564 2074 6f20 6e6f 740d 0a23 2062 6520  ed to not..# be 
+000024a0: 7573 6564 292e 0d0a 6475 6d6d 792d 7661  used)...dummy-va
+000024b0: 7269 6162 6c65 732d 7267 7820 3d20 225f  riables-rgx = "_
+000024c0: 2b24 7c28 5f5b 612d 7a41 2d5a 302d 395f  +$|(_[a-zA-Z0-9_
+000024d0: 5d2a 5b61 2d7a 412d 5a30 2d39 5d2b 3f24  ]*[a-zA-Z0-9]+?$
+000024e0: 297c 6475 6d6d 797c 5e69 676e 6f72 6564  )|dummy|^ignored
+000024f0: 5f7c 5e75 6e75 7365 645f 220d 0a0d 0a23  _|^unused_"....#
+00002500: 2041 7267 756d 656e 7420 6e61 6d65 7320   Argument names 
+00002510: 7468 6174 206d 6174 6368 2074 6869 7320  that match this 
+00002520: 6578 7072 6573 7369 6f6e 2077 696c 6c20  expression will 
+00002530: 6265 2069 676e 6f72 6564 2e0d 0a69 676e  be ignored...ign
+00002540: 6f72 6564 2d61 7267 756d 656e 742d 6e61  ored-argument-na
+00002550: 6d65 7320 3d20 225f 2e2a 7c5e 6967 6e6f  mes = "_.*|^igno
+00002560: 7265 645f 7c5e 756e 7573 6564 5f22 0d0a  red_|^unused_"..
+00002570: 0d0a 2320 4c69 7374 206f 6620 7175 616c  ..# List of qual
+00002580: 6966 6965 6420 6d6f 6475 6c65 206e 616d  ified module nam
+00002590: 6573 2077 6869 6368 2063 616e 2068 6176  es which can hav
+000025a0: 6520 6f62 6a65 6374 7320 7468 6174 2063  e objects that c
+000025b0: 616e 2072 6564 6566 696e 650d 0a23 2062  an redefine..# b
+000025c0: 7569 6c74 696e 732e 0d0a 7265 6465 6669  uiltins...redefi
+000025d0: 6e69 6e67 2d62 7569 6c74 696e 732d 6d6f  ning-builtins-mo
+000025e0: 6475 6c65 7320 3d20 5b22 7369 782e 6d6f  dules = ["six.mo
+000025f0: 7665 7322 2c20 2270 6173 742e 6275 696c  ves", "past.buil
+00002600: 7469 6e73 222c 2022 6675 7475 7265 2e62  tins", "future.b
+00002610: 7569 6c74 696e 7322 2c20 2262 7569 6c74  uiltins", "built
+00002620: 696e 7322 2c20 2269 6f22 5d0d 0a0d 0a5b  ins", "io"]....[
+00002630: 746f 6f6c 2e70 796c 696e 742e 6d65 7373  tool.pylint.mess
+00002640: 6167 6573 5f63 6f6e 7472 6f6c 5d0d 0a64  ages_control]..d
+00002650: 6973 6162 6c65 203d 205b 0d0a 2020 226c  isable = [..  "l
+00002660: 696e 652d 746f 6f2d 6c6f 6e67 222c 0d0a  ine-too-long",..
+00002670: 2020 2269 6e76 616c 6964 2d6e 616d 6522    "invalid-name"
+00002680: 2c0d 0a20 2022 6d69 7373 696e 672d 6675  ,..  "missing-fu
+00002690: 6e63 7469 6f6e 2d64 6f63 7374 7269 6e67  nction-docstring
+000026a0: 222c 0d0a 2020 226d 6973 7369 6e67 2d63  ",..  "missing-c
+000026b0: 6c61 7373 2d64 6f63 7374 7269 6e67 222c  lass-docstring",
+000026c0: 0d0a 2020 2261 7474 7269 6275 7465 2d64  ..  "attribute-d
+000026d0: 6566 696e 6564 2d6f 7574 7369 6465 2d69  efined-outside-i
+000026e0: 6e69 7422 2c0d 0a20 2022 6578 6563 2d75  nit",..  "exec-u
+000026f0: 7365 6422 2c0d 0a20 2022 636f 6e73 6964  sed",..  "consid
+00002700: 6572 2d75 7369 6e67 2d66 2d73 7472 696e  er-using-f-strin
+00002710: 6722 2c0d 0a20 2022 7265 6465 6669 6e65  g",..  "redefine
+00002720: 642d 6f75 7465 722d 6e61 6d65 222c 0d0a  d-outer-name",..
+00002730: 2020 2264 7570 6c69 6361 7465 2d63 6f64    "duplicate-cod
+00002740: 6522 2c0d 0a20 2022 746f 6f2d 6665 772d  e",..  "too-few-
+00002750: 7075 626c 6963 2d6d 6574 686f 6473 222c  public-methods",
+00002760: 0d0a 2020 2274 6f6f 2d6d 616e 792d 696e  ..  "too-many-in
+00002770: 7374 616e 6365 2d61 7474 7269 6275 7465  stance-attribute
+00002780: 7322 2c0d 0a20 2022 636f 6e73 6964 6572  s",..  "consider
+00002790: 2d69 7465 7261 7469 6e67 2d64 6963 7469  -iterating-dicti
+000027a0: 6f6e 6172 7922 2c0d 0a20 2022 636f 6e73  onary",..  "cons
+000027b0: 6964 6572 2d75 7369 6e67 2d64 6963 742d  ider-using-dict-
+000027c0: 6974 656d 7322 2c0d 0a20 2022 746f 6f2d  items",..  "too-
+000027d0: 6d61 6e79 2d62 7261 6e63 6865 7322 2c0d  many-branches",.
+000027e0: 0a20 2022 7375 7065 722d 696e 6974 2d6e  .  "super-init-n
+000027f0: 6f74 2d63 616c 6c65 6422 2c0d 0a20 2022  ot-called",..  "
+00002800: 6d69 7373 696e 672d 6d6f 6475 6c65 2d64  missing-module-d
+00002810: 6f63 7374 7269 6e67 220d 0a5d 0d0a       ocstring"..]..
```

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/AD_Input.py` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/AD_Input.py`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/AnF_Input.py` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/AnF_Input.py`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/COM_Col_Input.py` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/COM_Col_Input.py`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/CommonData.py` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/CommonData.py`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/Comp_Input.py` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/Comp_Input.py`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/GC_Input.py` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/GC_Input.py`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/HC_Input.py` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/HC_Input.py`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/InputData.py` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/InputData.py`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/LF_Input.py` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/LF_Input.py`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/MC.py` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/MC.py`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/MF_Col_Input.py` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/MF_Col_Input.py`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/RDF_Input.py` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/RDF_Input.py`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/Reproc_Input.py` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/Reproc_Input.py`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/SF_Col_Input.py` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/SF_Col_Input.py`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/SS_MRF_Input.py` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/SS_MRF_Input.py`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/TS_Input.py` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/TS_Input.py`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/Technosphere_Input.py` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/Technosphere_Input.py`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/WTE_Input.py` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/WTE_Input.py`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/__init__.py` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,8 +40,8 @@
     "TS_Input",
     "HC_Input",
     "GC_Input",
     "RDF_Input",
     "AnF_Input",
 ]
 
-__version__ = "1.0.0"
+__version__ = "1.1.0"
```

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/AD_Input.csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/AD_Input.csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/AD_Input_MaterialDependent.csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/AD_Input_MaterialDependent.csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/AnF_Input.csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/AnF_Input.csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/AnF_Input_MaterialDependent.csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/AnF_Input_MaterialDependent.csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/COM_Col_Input.csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/COM_Col_Input.csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/COM_Col_Input_MaterialDependent.csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/COM_Col_Input_MaterialDependent.csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/CommonData.csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/CommonData.csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/Comp_Input.csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/Comp_Input.csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/Comp_Input_MaterialDependent.csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/Comp_Input_MaterialDependent.csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/GC_Input.csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/GC_Input.csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/GC_Input_MaterialDependent.csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/GC_Input_MaterialDependent.csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/HC_Input.csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/HC_Input.csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/HC_Input_MaterialDependent.csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/HC_Input_MaterialDependent.csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/LF_Gas_emission_factors.csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/LF_Gas_emission_factors.csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/LF_Input.csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/LF_Input.csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/LF_Input_MaterialDependent.csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/LF_Input_MaterialDependent.csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/LF_Leachate_Quality.csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/LF_Leachate_Quality.csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/MF_Col_Input.csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/MF_Col_Input.csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/MF_Col_Input_MaterialDependent.csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/MF_Col_Input_MaterialDependent.csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/Material properties.csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/Material properties.csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/RDF_Input.csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/RDF_Input.csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/RDF_Input_MaterialDependent.csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/RDF_Input_MaterialDependent.csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/References.csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/References.csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/Reprocessing_Input.csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/Reprocessing_Input.csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/SF_Col_Input.csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/SF_Col_Input.csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/SF_Col_Input_MaterialDependent.csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/SF_Col_Input_MaterialDependent.csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/SS_MRF_Input.csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/SS_MRF_Input.csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/SS_MRF_Input_MaterialDependent.csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/SS_MRF_Input_MaterialDependent.csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/TS_Input.csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/TS_Input.csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/Technosphere_LCI.csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/Technosphere_LCI.csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/Technosphere_References.csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/Technosphere_References.csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/WTE_Input.csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/WTE_Input.csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/WTE_Input_MaterialDependent.csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/WTE_Input_MaterialDependent.csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/keys.csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/keys.csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('CML (v4.4) SwolfPy', 'resources', 'depletion of abiotic resources - elements, ultimate reserves').csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/lcia_methods/('CML (v4.4) SwolfPy', 'resources', 'depletion of abiotic resources - elements, ultimate reserves').csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('IPCC 2007, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=0').csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/lcia_methods/('IPCC 2007, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=0').csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('IPCC 2007, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=1').csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/lcia_methods/('IPCC 2007, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=1').csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('IPCC 2013, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=0').csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/lcia_methods/('IPCC 2013, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=0').csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('IPCC 2013, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=0, C1_36').csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/lcia_methods/('IPCC 2013, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=0, C1_36').csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('IPCC 2013, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=1').csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/lcia_methods/('IPCC 2013, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=1').csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('IPCC 2013, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=1, C1_36').csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/lcia_methods/('IPCC 2013, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=1, C1_36').csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('SwolfPy_Total_Cost', 'SwolfPy').csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/lcia_methods/('SwolfPy_Total_Cost', 'SwolfPy').csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('TRACI (2.1) SwolfPy', 'environmental impact', 'acidification').csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/lcia_methods/('TRACI (2.1) SwolfPy', 'environmental impact', 'acidification').csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('TRACI (2.1) SwolfPy', 'environmental impact', 'eutrophication').csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/lcia_methods/('TRACI (2.1) SwolfPy', 'environmental impact', 'eutrophication').csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('TRACI (2.1) SwolfPy', 'environmental impact', 'photochemical smog').csv` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata/data/lcia_methods/('TRACI (2.1) SwolfPy', 'environmental impact', 'photochemical smog').csv`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata.egg-info/PKG-INFO` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: swolfpy-inputdata
-Version: 1.0.0
+Version: 1.1.0
 Summary: Input data for swolfpy's life-cycle process models (swolfpy_inputdata).
 Author-email: Mojtaba Sardarmehni <msardar2@alumni.ncsu.edu>
 Maintainer-email: Mojtaba Sardarmehni <msardar2@alumni.ncsu.edu>
 License: GNU GENERAL PUBLIC LICENSE V2
 Project-URL: Homepage, https://swolfpy-project.github.io/
 Project-URL: Documentation, https://swolfpy.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/SwolfPy-Project/swolfpy-inputdata
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
 
 ======================================================================
@@ -139,15 +139,15 @@
 
 2- Update conda in a terminal window or anaconda prompt::
 
         conda update conda
 
 3- Create a new environment for swolfpy::
 
-        conda create --name swolfpy python=3.10
+        conda create --name swolfpy python=3.9
 
 4- Activate the environment::
 
         conda activate swolfpy
 
 5- Install swolfpy_inputdata in the environment::
 
@@ -165,14 +165,20 @@
 
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
 1.0.0 (2023-06-03)
 ------------------
 
 * Upgrade to Python 3.10
 * Add PreCommit
```

### Comparing `swolfpy_inputdata-1.0.0/swolfpy_inputdata.egg-info/SOURCES.txt` & `swolfpy_inputdata-1.1.0/swolfpy_inputdata.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 swolfpy_inputdata/WTE_Input.py
 swolfpy_inputdata/__init__.py
 swolfpy_inputdata.egg-info/PKG-INFO
 swolfpy_inputdata.egg-info/SOURCES.txt
 swolfpy_inputdata.egg-info/dependency_links.txt
 swolfpy_inputdata.egg-info/requires.txt
 swolfpy_inputdata.egg-info/top_level.txt
+swolfpy_inputdata/Ecospold2/__init__.py
 swolfpy_inputdata/data/AD_Input.csv
 swolfpy_inputdata/data/AD_Input_MaterialDependent.csv
 swolfpy_inputdata/data/AnF_Input.csv
 swolfpy_inputdata/data/AnF_Input_MaterialDependent.csv
 swolfpy_inputdata/data/COM_Col_Input.csv
 swolfpy_inputdata/data/COM_Col_Input_MaterialDependent.csv
 swolfpy_inputdata/data/CommonData.csv
@@ -61,25 +62,27 @@
 swolfpy_inputdata/data/SS_MRF_Input.csv
 swolfpy_inputdata/data/SS_MRF_Input_MaterialDependent.csv
 swolfpy_inputdata/data/TS_Input.csv
 swolfpy_inputdata/data/Technosphere_LCI.csv
 swolfpy_inputdata/data/Technosphere_References.csv
 swolfpy_inputdata/data/WTE_Input.csv
 swolfpy_inputdata/data/WTE_Input_MaterialDependent.csv
+swolfpy_inputdata/data/__init__.py
 swolfpy_inputdata/data/keys.csv
 swolfpy_inputdata/data/lcia_methods/('CML (v4.4) SwolfPy', 'resources', 'depletion of abiotic resources - elements, ultimate reserves').csv
 swolfpy_inputdata/data/lcia_methods/('IPCC 2007, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=0').csv
 swolfpy_inputdata/data/lcia_methods/('IPCC 2007, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=1').csv
 swolfpy_inputdata/data/lcia_methods/('IPCC 2013, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=0').csv
 swolfpy_inputdata/data/lcia_methods/('IPCC 2013, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=0, C1_36').csv
 swolfpy_inputdata/data/lcia_methods/('IPCC 2013, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=1').csv
 swolfpy_inputdata/data/lcia_methods/('IPCC 2013, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=1, C1_36').csv
 swolfpy_inputdata/data/lcia_methods/('SwolfPy_Capital_Cost', 'SwolfPy').csv
 swolfpy_inputdata/data/lcia_methods/('SwolfPy_Operational_Cost', 'SwolfPy').csv
 swolfpy_inputdata/data/lcia_methods/('SwolfPy_Total_Cost', 'SwolfPy').csv
 swolfpy_inputdata/data/lcia_methods/('TRACI (2.1) SwolfPy', 'environmental impact', 'acidification').csv
 swolfpy_inputdata/data/lcia_methods/('TRACI (2.1) SwolfPy', 'environmental impact', 'eutrophication').csv
 swolfpy_inputdata/data/lcia_methods/('TRACI (2.1) SwolfPy', 'environmental impact', 'photochemical smog').csv
+swolfpy_inputdata/data/lcia_methods/__init__.py
 tests/Test_Input.csv
 tests/__init__.py
 tests/test_inputdata.py
 tests/test_inputs.py
```

### Comparing `swolfpy_inputdata-1.0.0/tests/test_inputdata.py` & `swolfpy_inputdata-1.1.0/tests/test_inputdata.py`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-1.0.0/tests/test_inputs.py` & `swolfpy_inputdata-1.1.0/tests/test_inputs.py`

 * *Files identical despite different names*

