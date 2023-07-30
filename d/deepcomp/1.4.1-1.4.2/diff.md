# Comparing `tmp/deepcomp-1.4.1.tar.gz` & `tmp/deepcomp-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepcomp-1.4.1.tar", last modified: Thu Oct  7 17:21:37 2021, max compression
+gzip compressed data, was "deepcomp-1.4.2.tar", last modified: Sun Jul 30 18:25:43 2023, max compression
```

## Comparing `deepcomp-1.4.1.tar` & `deepcomp-1.4.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-07 17:21:37.880716 deepcomp-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2021-10-07 17:21:28.000000 deepcomp-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     9095 2021-10-07 17:21:37.880716 deepcomp-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8605 2021-10-07 17:21:28.000000 deepcomp-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-07 17:21:37.876716 deepcomp-1.4.1/deepcomp/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-07 17:21:28.000000 deepcomp-1.4.1/deepcomp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-07 17:21:37.876716 deepcomp-1.4.1/deepcomp/agent/
--rw-r--r--   0 runner    (1001) docker     (121)       40 2021-10-07 17:21:28.000000 deepcomp-1.4.1/deepcomp/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      571 2021-10-07 17:21:28.000000 deepcomp-1.4.1/deepcomp/agent/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3514 2021-10-07 17:21:28.000000 deepcomp-1.4.1/deepcomp/agent/brute_force.py
--rw-r--r--   0 runner    (1001) docker     (121)     2124 2021-10-07 17:21:28.000000 deepcomp-1.4.1/deepcomp/agent/dummy.py
--rw-r--r--   0 runner    (1001) docker     (121)     7649 2021-10-07 17:21:28.000000 deepcomp-1.4.1/deepcomp/agent/heuristics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-07 17:21:37.876716 deepcomp-1.4.1/deepcomp/env/
--rw-r--r--   0 runner    (1001) docker     (121)      222 2021-10-07 17:21:28.000000 deepcomp-1.4.1/deepcomp/env/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-07 17:21:37.876716 deepcomp-1.4.1/deepcomp/env/entities/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-07 17:21:28.000000 deepcomp-1.4.1/deepcomp/env/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2498 2021-10-07 17:21:28.000000 deepcomp-1.4.1/deepcomp/env/entities/map.py
--rw-r--r--   0 runner    (1001) docker     (121)    10989 2021-10-07 17:21:28.000000 deepcomp-1.4.1/deepcomp/env/entities/station.py
--rw-r--r--   0 runner    (1001) docker     (121)     9940 2021-10-07 17:21:28.000000 deepcomp-1.4.1/deepcomp/env/entities/user.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-07 17:21:37.876716 deepcomp-1.4.1/deepcomp/env/multi_ue/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-07 17:21:28.000000 deepcomp-1.4.1/deepcomp/env/multi_ue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8675 2021-10-07 17:21:28.000000 deepcomp-1.4.1/deepcomp/env/multi_ue/central.py
--rw-r--r--   0 runner    (1001) docker     (121)     8170 2021-10-07 17:21:28.000000 deepcomp-1.4.1/deepcomp/env/multi_ue/multi_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-07 17:21:37.880716 deepcomp-1.4.1/deepcomp/env/single_ue/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-07 17:21:28.000000 deepcomp-1.4.1/deepcomp/env/single_ue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    27406 2021-10-07 17:21:28.000000 deepcomp-1.4.1/deepcomp/env/single_ue/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    16302 2021-10-07 17:21:28.000000 deepcomp-1.4.1/deepcomp/env/single_ue/variants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-07 17:21:37.880716 deepcomp-1.4.1/deepcomp/env/util/
--rw-r--r--   0 runner    (1001) docker     (121)       55 2021-10-07 17:21:28.000000 deepcomp-1.4.1/deepcomp/env/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7265 2021-10-07 17:21:28.000000 deepcomp-1.4.1/deepcomp/env/util/movement.py
--rw-r--r--   0 runner    (1001) docker     (121)     2290 2021-10-07 17:21:28.000000 deepcomp-1.4.1/deepcomp/env/util/utility.py
--rw-r--r--   0 runner    (1001) docker     (121)     3937 2021-10-07 17:21:28.000000 deepcomp-1.4.1/deepcomp/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-07 17:21:37.880716 deepcomp-1.4.1/deepcomp/util/
--rw-r--r--   0 runner    (1001) docker     (121)      107 2021-10-07 17:21:28.000000 deepcomp-1.4.1/deepcomp/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2165 2021-10-07 17:21:28.000000 deepcomp-1.4.1/deepcomp/util/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (121)     9952 2021-10-07 17:21:28.000000 deepcomp-1.4.1/deepcomp/util/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     4246 2021-10-07 17:21:28.000000 deepcomp-1.4.1/deepcomp/util/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    14157 2021-10-07 17:21:28.000000 deepcomp-1.4.1/deepcomp/util/env_setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1281 2021-10-07 17:21:28.000000 deepcomp-1.4.1/deepcomp/util/logs.py
--rw-r--r--   0 runner    (1001) docker     (121)    36140 2021-10-07 17:21:28.000000 deepcomp-1.4.1/deepcomp/util/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-07 17:21:37.876716 deepcomp-1.4.1/deepcomp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9095 2021-10-07 17:21:37.000000 deepcomp-1.4.1/deepcomp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1045 2021-10-07 17:21:37.000000 deepcomp-1.4.1/deepcomp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-07 17:21:37.000000 deepcomp-1.4.1/deepcomp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-10-07 17:21:37.000000 deepcomp-1.4.1/deepcomp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-07 17:21:37.000000 deepcomp-1.4.1/deepcomp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      257 2021-10-07 17:21:37.000000 deepcomp-1.4.1/deepcomp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-10-07 17:21:37.000000 deepcomp-1.4.1/deepcomp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-07 17:21:37.880716 deepcomp-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1719 2021-10-07 17:21:28.000000 deepcomp-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:25:43.578631 deepcomp-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-30 18:25:32.000000 deepcomp-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9842 2023-07-30 18:25:43.578631 deepcomp-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-07-30 18:25:32.000000 deepcomp-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:25:43.570631 deepcomp-1.4.2/deepcomp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 18:25:32.000000 deepcomp-1.4.2/deepcomp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:25:43.574631 deepcomp-1.4.2/deepcomp/agent/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-30 18:25:32.000000 deepcomp-1.4.2/deepcomp/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-30 18:25:32.000000 deepcomp-1.4.2/deepcomp/agent/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-30 18:25:32.000000 deepcomp-1.4.2/deepcomp/agent/brute_force.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-30 18:25:32.000000 deepcomp-1.4.2/deepcomp/agent/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-07-30 18:25:32.000000 deepcomp-1.4.2/deepcomp/agent/heuristics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:25:43.574631 deepcomp-1.4.2/deepcomp/env/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-30 18:25:32.000000 deepcomp-1.4.2/deepcomp/env/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:25:43.578631 deepcomp-1.4.2/deepcomp/env/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 18:25:32.000000 deepcomp-1.4.2/deepcomp/env/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-30 18:25:32.000000 deepcomp-1.4.2/deepcomp/env/entities/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-07-30 18:25:32.000000 deepcomp-1.4.2/deepcomp/env/entities/station.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-07-30 18:25:32.000000 deepcomp-1.4.2/deepcomp/env/entities/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:25:43.578631 deepcomp-1.4.2/deepcomp/env/multi_ue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 18:25:32.000000 deepcomp-1.4.2/deepcomp/env/multi_ue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-07-30 18:25:32.000000 deepcomp-1.4.2/deepcomp/env/multi_ue/central.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-07-30 18:25:32.000000 deepcomp-1.4.2/deepcomp/env/multi_ue/multi_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:25:43.578631 deepcomp-1.4.2/deepcomp/env/single_ue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 18:25:32.000000 deepcomp-1.4.2/deepcomp/env/single_ue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27406 2023-07-30 18:25:32.000000 deepcomp-1.4.2/deepcomp/env/single_ue/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16302 2023-07-30 18:25:32.000000 deepcomp-1.4.2/deepcomp/env/single_ue/variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:25:43.578631 deepcomp-1.4.2/deepcomp/env/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-30 18:25:32.000000 deepcomp-1.4.2/deepcomp/env/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-07-30 18:25:32.000000 deepcomp-1.4.2/deepcomp/env/util/movement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-07-30 18:25:32.000000 deepcomp-1.4.2/deepcomp/env/util/utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-07-30 18:25:32.000000 deepcomp-1.4.2/deepcomp/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:25:43.578631 deepcomp-1.4.2/deepcomp/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-30 18:25:32.000000 deepcomp-1.4.2/deepcomp/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-30 18:25:32.000000 deepcomp-1.4.2/deepcomp/util/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-07-30 18:25:32.000000 deepcomp-1.4.2/deepcomp/util/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-07-30 18:25:32.000000 deepcomp-1.4.2/deepcomp/util/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14157 2023-07-30 18:25:32.000000 deepcomp-1.4.2/deepcomp/util/env_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-30 18:25:32.000000 deepcomp-1.4.2/deepcomp/util/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36140 2023-07-30 18:25:32.000000 deepcomp-1.4.2/deepcomp/util/simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:25:43.574631 deepcomp-1.4.2/deepcomp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9842 2023-07-30 18:25:43.000000 deepcomp-1.4.2/deepcomp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-30 18:25:43.000000 deepcomp-1.4.2/deepcomp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 18:25:43.000000 deepcomp-1.4.2/deepcomp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-30 18:25:43.000000 deepcomp-1.4.2/deepcomp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 18:25:43.000000 deepcomp-1.4.2/deepcomp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-30 18:25:43.000000 deepcomp-1.4.2/deepcomp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-30 18:25:43.000000 deepcomp-1.4.2/deepcomp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 18:25:43.578631 deepcomp-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-07-30 18:25:32.000000 deepcomp-1.4.2/setup.py
```

### Comparing `deepcomp-1.4.1/LICENSE` & `deepcomp-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deepcomp-1.4.1/PKG-INFO` & `deepcomp-1.4.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,59 @@
 Metadata-Version: 2.1
 Name: deepcomp
-Version: 1.4.1
+Version: 1.4.2
 Summary: DeepCoMP: Self-Learning Dynamic Multi-Cell Selection for Coordinated Multipoint (CoMP)
 Home-page: https://github.com/CN-UPB/DeepCoMP
 Author: Stefan Schneider
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8.*
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![CI](https://github.com/CN-UPB/DeepCoMP/actions/workflows/python-test.yml/badge.svg)](https://github.com/CN-UPB/DeepCoMP/actions/workflows/python-test.yml)
 [![PyPi](https://github.com/CN-UPB/DeepCoMP/actions/workflows/python-publish.yml/badge.svg?branch=v1.1.0)](https://github.com/CN-UPB/DeepCoMP/actions/workflows/python-publish.yml)
-[![Docker Cloud Build Status](https://img.shields.io/docker/cloud/build/stefanbschneider/deepcomp?label=Docker%20Build&logo=docker)](https://hub.docker.com/r/stefanbschneider/deepcomp)
 [![Docker Pulls](https://img.shields.io/docker/pulls/stefanbschneider/deepcomp?label=Docker%20Pulls&logo=docker)](https://hub.docker.com/r/stefanbschneider/deepcomp)
 [![DeepSource](https://deepsource.io/gh/CN-UPB/DeepCoMP.svg/?label=active+issues)](https://deepsource.io/gh/CN-UPB/DeepCoMP/?ref=repository-badge)
 
 
 # DeepCoMP: Self-Learning Dynamic Multi-Cell Selection for Coordinated Multipoint (CoMP)
 
-Deep reinforcement learning for dynamic multi-cell selection in CoMP scenarios.
+Multi-Agent Deep Reinforcement Learning for Coordinated Multipoint in Mobile Networks
+
 Three variants: DeepCoMP (central agent), DD-CoMP (distributed agents using central policy), D3-CoMP (distributed agents with separate policies).
 All three approaches self-learn and adapt to various scenarios in mobile networks without expert knowledge, human intervention, or detailed assumptions about the underlying system.
 Compared to other approaches, they are more flexible and achieve higher Quality of Experience.
 
+For a high-level overview of DeepCoMP, please refer to my [blog post](https://stefanbschneider.github.io/blog/deepcomp).
+More details are available in our research paper presenting DeepCoMP ([preprint](https://ris.uni-paderborn.de/download/33854/33855/preprint.pdf)).
+I also talked about DeepCoMP at the Ray Summit 2021 ([YouTube](https://youtu.be/Qy4SzJKXlGE)).
+
+The simulation environment used to train DeepCoMP is available separately as [mobile-env](https://github.com/stefanbschneider/mobile-env).
+
 <p align="center">
     <img src="https://raw.githubusercontent.com/CN-UPB/DeepCoMP/master/docs/gifs/dashboard_lossy.gif?raw=true"><br/>
     <em>Visualized cell selection policy of DeepCoMP after 2M training steps.</em><br>
     <sup><a href="https://thenounproject.com/search/?q=base+station&i=1286474" target="_blank">Base station icon</a> by Clea Doltz from the Noun Project</sup>
 </p>
 
+## Citation
+
+If you use this code, please cite our [paper (preprint; accepted at IEEE TNSM 2023)](https://ris.uni-paderborn.de/download/33854/33855):
+
+```
+@article{schneider2023deepcomp,
+	title={Multi-Agent Deep Reinforcement Learning for Coordinated Multipoint in Mobile Networks},
+	author={Schneider, Stefan and Karl, Holger and Khalili, Ramin and Hecker, Artur},
+	journal={IEEE Transactions on Network and Service Management (TNSM)},
+	year={2023},
+}
+```
+
 ## Setup
 
 You need Python 3.8+. You can install `deepcomp` either directly from [PyPi](https://pypi.org/project/deepcomp/) or manually after cloning this repository.
 
 ### Simple Installation via PyPi
 
 ```
@@ -225,9 +242,7 @@
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/CN-UPB/DeepCoMP/master/docs/logos/upb.png?raw=true" width="200" hspace="30"/>
     <img src="https://raw.githubusercontent.com/CN-UPB/DeepCoMP/master/docs/logos/huawei_horizontal.png?raw=true" width="250" hspace="30"/>
 </p>
 
 [Base station icon](https://thenounproject.com/search/?q=base+station&i=1286474) (used in rendered videos) by Clea Doltz from the Noun Project.
-
-
```

#### html2text {}

```diff
@@ -1,118 +1,126 @@
-Metadata-Version: 2.1 Name: deepcomp Version: 1.4.1 Summary: DeepCoMP: Self-
+Metadata-Version: 2.1 Name: deepcomp Version: 1.4.2 Summary: DeepCoMP: Self-
 Learning Dynamic Multi-Cell Selection for Coordinated Multipoint (CoMP) Home-
-page: https://github.com/CN-UPB/DeepCoMP Author: Stefan Schneider License:
-UNKNOWN Platform: UNKNOWN Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Requires-Python: >=3.8.* Description-Content-Type: text/
-markdown License-File: LICENSE [![CI](https://github.com/CN-UPB/DeepCoMP/
-actions/workflows/python-test.yml/badge.svg)](https://github.com/CN-UPB/
-DeepCoMP/actions/workflows/python-test.yml) [![PyPi](https://github.com/CN-UPB/
-DeepCoMP/actions/workflows/python-publish.yml/badge.svg?branch=v1.1.0)](https:/
-/github.com/CN-UPB/DeepCoMP/actions/workflows/python-publish.yml) [![Docker
-Cloud Build Status](https://img.shields.io/docker/cloud/build/stefanbschneider/
-deepcomp?label=Docker%20Build&logo=docker)](https://hub.docker.com/r/
-stefanbschneider/deepcomp) [![Docker Pulls](https://img.shields.io/docker/
-pulls/stefanbschneider/deepcomp?label=Docker%20Pulls&logo=docker)](https://
+page: https://github.com/CN-UPB/DeepCoMP Author: Stefan Schneider Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown License-File: LICENSE [![CI](https://
+github.com/CN-UPB/DeepCoMP/actions/workflows/python-test.yml/badge.svg)](https:
+//github.com/CN-UPB/DeepCoMP/actions/workflows/python-test.yml) [![PyPi](https:
+//github.com/CN-UPB/DeepCoMP/actions/workflows/python-publish.yml/
+badge.svg?branch=v1.1.0)](https://github.com/CN-UPB/DeepCoMP/actions/workflows/
+python-publish.yml) [![Docker Pulls](https://img.shields.io/docker/pulls/
+stefanbschneider/deepcomp?label=Docker%20Pulls&logo=docker)](https://
 hub.docker.com/r/stefanbschneider/deepcomp) [![DeepSource](https://
 deepsource.io/gh/CN-UPB/DeepCoMP.svg/?label=active+issues)](https://
 deepsource.io/gh/CN-UPB/DeepCoMP/?ref=repository-badge) # DeepCoMP: Self-
-Learning Dynamic Multi-Cell Selection for Coordinated Multipoint (CoMP) Deep
-reinforcement learning for dynamic multi-cell selection in CoMP scenarios.
+Learning Dynamic Multi-Cell Selection for Coordinated Multipoint (CoMP) Multi-
+Agent Deep Reinforcement Learning for Coordinated Multipoint in Mobile Networks
 Three variants: DeepCoMP (central agent), DD-CoMP (distributed agents using
 central policy), D3-CoMP (distributed agents with separate policies). All three
 approaches self-learn and adapt to various scenarios in mobile networks without
 expert knowledge, human intervention, or detailed assumptions about the
 underlying system. Compared to other approaches, they are more flexible and
-achieve higher Quality of Experience.
+achieve higher Quality of Experience. For a high-level overview of DeepCoMP,
+please refer to my [blog post](https://stefanbschneider.github.io/blog/
+deepcomp). More details are available in our research paper presenting DeepCoMP
+([preprint](https://ris.uni-paderborn.de/download/33854/33855/preprint.pdf)). I
+also talked about DeepCoMP at the Ray Summit 2021 ([YouTube](https://youtu.be/
+Qy4SzJKXlGE)). The simulation environment used to train DeepCoMP is available
+separately as [mobile-env](https://github.com/stefanbschneider/mobile-env).
      [https://raw.githubusercontent.com/CN-UPB/DeepCoMP/master/docs/gifs/
                          dashboard_lossy.gif?raw=true]
      Visualized cell selection policy of DeepCoMP after 2M training steps.
              Base_station_icon by Clea Doltz from the Noun Project
-## Setup You need Python 3.8+. You can install `deepcomp` either directly from
-[PyPi](https://pypi.org/project/deepcomp/) or manually after cloning this
-repository. ### Simple Installation via PyPi ``` sudo apt update sudo apt
-upgrade sudo apt install cmake build-essential zlib1g-dev python3-dev pip
-install deepcomp ``` ### Manual Installation from Source For adjusting or
-further developing DeepCoMP, it's better to install manually rather than from
-PyPi. Clone the repository. Then install everything, following these steps: ```
-# only on ubuntu sudo apt update sudo apt upgrade sudo apt install cmake build-
-essential zlib1g-dev python3-dev # clone git clone git@github.com:CN-UPB/
-DeepCoMP.git cd DeepCoMP # install all python dependencies pip install . #
-"python setup.py install" does not work for some reason: https://
-stackoverflow.com/a/66267232/2745116 # for development install (when changing
-code): pip install -e . ``` Tested on Ubuntu 20.04 and Windows 10 with Python
-3.8. For saving videos and gifs, you also need to install ffmpeg (not on
-Windows) and [ImageMagick](https://imagemagick.org/index.php). On Ubuntu: ```
-sudo apt install ffmpeg imagemagick ``` ### Docker There is a Docker image that
-comes with `deepcomp` preinstalled. To use the Docker image, simply pull the
-latest version from [Docker Hub](https://hub.docker.com/r/stefanbschneider/
-deepcomp): ``` docker pull stefanbschneider/deepcomp # tag image with just
-"deepcomp". alternatively, write out "stefanbschneider/deepcomp" in all
-following commands. docker tag stefanbschneider/deepcomp:latest deepcomp ```
-Alternatively, to build the Docker image manually from the `Dockerfile`, clone
-this repository and run ``` docker build -t deepcomp . ``` Use the `--no-cache`
-option is to force a rebuild of the image, pulling the latest `deepcomp`
-version from PyPI. ## Usage ``` # get an overview of all options deepcomp -
-h ``` For example: ``` deepcomp --env medium --slow-ues 3 --agent central --
-workers 2 --train-steps 50000 --seed 42 --video both ``` To run DeepCoMP, use
-`--alg ppo --agent central`. For DD-CoMP, use `--alg ppo --agent multi`, and
-for D3-CoMP, use `--alg ppo --agent multi --separate-agent-nns`. By default,
-training logs, results, videos, and trained agents are saved in `/results`,
-where `` is the root directory of DeepCoMP. If you cloned the repo from GitHub,
-this is where the Readme is. If you installed via PyPi, this is in your
-virtualenv's site packages. You can choose a custom location with `--result-dir
-`. ### Docker **Note:** By default, results within the Docker container are not
-stored persistently. To save them, copy them from the Docker container or use a
-Docker volume. #### Start the Container If you want to use the `deepcomp`
-Docker container and pulled the corresponding image from Docker Hub, you can
-use it as follows: ``` docker run -d -p 6006:6006 -p 8000:8000 --rm --shm-
-size=3gb --name deepcomp deepcomp ``` This starts the Docker container in the
-background, publishing port 6006 for TensorBoard and port 8000 for the HTTP
-server (described below). The container automatically starts TensorBoard and
-the HTTP server, so this does not need to be done manually. The `--rm` flag
-automatically removes the container once it is stopped. The `--shm-size=3gb`
-sets the size of `/dev/shm` inside the Docker container to 3 GB, which is too
-small by default. #### Use DeepCoMP on the Container To execute commands on the
-running Docker container, use `docker exec  ` as follows: ``` docker exec
-deepcomp deepcomp  ``` Here, the arguments are identical with the ones
-described above. For example, the following command lists all CLI options: ```
-docker exec deepcomp deepcomp -h ``` Or to train the central DeepCoMP agent for
-a short duration of 4000 steps: ``` docker exec -t deepcomp deepcomp --approach
-deepcomp --train-steps 4000 --batch-size 200 --ues 2 --result-dir results ```
-**Important:** Specify `--result-dir results` as argument. Otherwise, the
-results will be stored elsewhere and TensorFlow and the HTTP server will not
-find and display them. The other `deepcomp` arguments can be set as desired.
-The Docker `-t` flag ensures that the output is printed continuously during
-training, not just after completion. To inspect training progress or view
-create files (e.g., rendered videos), use TensorBoard and the HTTP server,
-which are available via `localhost:6006` and `localhost:8000`. #### Terminate
-the Container **Important:** Stopping the container will remove any files and
-training progress within the container. Stop the container with ``` docker stop
-deepcomp ``` ### Accessing results remotely When running remotely, you can
-serve the replay video by running: ``` cd results python -m http.server ```
-Then access at `:8000`. ### Tensorboard To view learning curves (and other
-metrics) when training an agent, use Tensorboard: ``` tensorboard --logdir
-results/train/ (--host 0.0.0.0) ``` Tensorboard is available at http://
-localhost:6006 (or `:6006` when running remotely). ### Scaling Up: Running
-DeepCoMP on multiple cores or a multi-node cluster To train DeepCoMP on
-multiple cores in parallel, configure the number of workers (corresponding to
-CPU cores) with `--workers`. To scale training to a multi-node cluster, adjust
-`cluster.yaml` and follow the steps described [here](https://
-stefanbschneider.github.io/blog/rllib-private-cluster). Set `--workers` to the
-total number of CPU cores you want to use on the entire cluster. ##
-Documentation API documentation is on [https://cn-upb.github.io/DeepCoMP/]
-(https://cn-upb.github.io/DeepCoMP/). Documentation is generated based on
-docstrings using [pdoc3](https://pdoc3.github.io/pdoc/): ``` # from project
-root pip install pdoc3 pdoc --force --html --output-dir docs deepcomp # move
-files to be picked up by GitHub pages mv docs/deepcomp/ docs/ # then manually
-adjust index.html to link to GitHub repo ``` ## Contributions Development:
-[@stefanbschneider](https://github.com/stefanbschneider/) Feature requests,
-questions, issues, and pull requests via GitHub are welcome. ## Acknowledgement
-DeepCoMP is an outcome of a joint project between Paderborn University,
-Germany, and Huawei Germany.
+## Citation If you use this code, please cite our [paper (preprint; accepted at
+IEEE TNSM 2023)](https://ris.uni-paderborn.de/download/33854/33855): ```
+@article{schneider2023deepcomp, title={Multi-Agent Deep Reinforcement Learning
+for Coordinated Multipoint in Mobile Networks}, author={Schneider, Stefan and
+Karl, Holger and Khalili, Ramin and Hecker, Artur}, journal={IEEE Transactions
+on Network and Service Management (TNSM)}, year={2023}, } ``` ## Setup You need
+Python 3.8+. You can install `deepcomp` either directly from [PyPi](https://
+pypi.org/project/deepcomp/) or manually after cloning this repository. ###
+Simple Installation via PyPi ``` sudo apt update sudo apt upgrade sudo apt
+install cmake build-essential zlib1g-dev python3-dev pip install deepcomp ```
+### Manual Installation from Source For adjusting or further developing
+DeepCoMP, it's better to install manually rather than from PyPi. Clone the
+repository. Then install everything, following these steps: ``` # only on
+ubuntu sudo apt update sudo apt upgrade sudo apt install cmake build-essential
+zlib1g-dev python3-dev # clone git clone git@github.com:CN-UPB/DeepCoMP.git cd
+DeepCoMP # install all python dependencies pip install . # "python setup.py
+install" does not work for some reason: https://stackoverflow.com/a/66267232/
+2745116 # for development install (when changing code): pip install -e . ```
+Tested on Ubuntu 20.04 and Windows 10 with Python 3.8. For saving videos and
+gifs, you also need to install ffmpeg (not on Windows) and [ImageMagick](https:
+//imagemagick.org/index.php). On Ubuntu: ``` sudo apt install ffmpeg
+imagemagick ``` ### Docker There is a Docker image that comes with `deepcomp`
+preinstalled. To use the Docker image, simply pull the latest version from
+[Docker Hub](https://hub.docker.com/r/stefanbschneider/deepcomp): ``` docker
+pull stefanbschneider/deepcomp # tag image with just "deepcomp". alternatively,
+write out "stefanbschneider/deepcomp" in all following commands. docker tag
+stefanbschneider/deepcomp:latest deepcomp ``` Alternatively, to build the
+Docker image manually from the `Dockerfile`, clone this repository and run ```
+docker build -t deepcomp . ``` Use the `--no-cache` option is to force a
+rebuild of the image, pulling the latest `deepcomp` version from PyPI. ## Usage
+``` # get an overview of all options deepcomp -h ``` For example: ``` deepcomp
+--env medium --slow-ues 3 --agent central --workers 2 --train-steps 50000 --
+seed 42 --video both ``` To run DeepCoMP, use `--alg ppo --agent central`. For
+DD-CoMP, use `--alg ppo --agent multi`, and for D3-CoMP, use `--alg ppo --agent
+multi --separate-agent-nns`. By default, training logs, results, videos, and
+trained agents are saved in `/results`, where `` is the root directory of
+DeepCoMP. If you cloned the repo from GitHub, this is where the Readme is. If
+you installed via PyPi, this is in your virtualenv's site packages. You can
+choose a custom location with `--result-dir `. ### Docker **Note:** By default,
+results within the Docker container are not stored persistently. To save them,
+copy them from the Docker container or use a Docker volume. #### Start the
+Container If you want to use the `deepcomp` Docker container and pulled the
+corresponding image from Docker Hub, you can use it as follows: ``` docker run
+-d -p 6006:6006 -p 8000:8000 --rm --shm-size=3gb --name deepcomp deepcomp ```
+This starts the Docker container in the background, publishing port 6006 for
+TensorBoard and port 8000 for the HTTP server (described below). The container
+automatically starts TensorBoard and the HTTP server, so this does not need to
+be done manually. The `--rm` flag automatically removes the container once it
+is stopped. The `--shm-size=3gb` sets the size of `/dev/shm` inside the Docker
+container to 3 GB, which is too small by default. #### Use DeepCoMP on the
+Container To execute commands on the running Docker container, use `docker exec
+` as follows: ``` docker exec deepcomp deepcomp  ``` Here, the arguments are
+identical with the ones described above. For example, the following command
+lists all CLI options: ``` docker exec deepcomp deepcomp -h ``` Or to train the
+central DeepCoMP agent for a short duration of 4000 steps: ``` docker exec -
+t deepcomp deepcomp --approach deepcomp --train-steps 4000 --batch-size 200 --
+ues 2 --result-dir results ``` **Important:** Specify `--result-dir results` as
+argument. Otherwise, the results will be stored elsewhere and TensorFlow and
+the HTTP server will not find and display them. The other `deepcomp` arguments
+can be set as desired. The Docker `-t` flag ensures that the output is printed
+continuously during training, not just after completion. To inspect training
+progress or view create files (e.g., rendered videos), use TensorBoard and the
+HTTP server, which are available via `localhost:6006` and `localhost:8000`.
+#### Terminate the Container **Important:** Stopping the container will remove
+any files and training progress within the container. Stop the container with
+``` docker stop deepcomp ``` ### Accessing results remotely When running
+remotely, you can serve the replay video by running: ``` cd results python -
+m http.server ``` Then access at `:8000`. ### Tensorboard To view learning
+curves (and other metrics) when training an agent, use Tensorboard: ```
+tensorboard --logdir results/train/ (--host 0.0.0.0) ``` Tensorboard is
+available at http://localhost:6006 (or `:6006` when running remotely). ###
+Scaling Up: Running DeepCoMP on multiple cores or a multi-node cluster To train
+DeepCoMP on multiple cores in parallel, configure the number of workers
+(corresponding to CPU cores) with `--workers`. To scale training to a multi-
+node cluster, adjust `cluster.yaml` and follow the steps described [here]
+(https://stefanbschneider.github.io/blog/rllib-private-cluster). Set `--
+workers` to the total number of CPU cores you want to use on the entire
+cluster. ## Documentation API documentation is on [https://cn-upb.github.io/
+DeepCoMP/](https://cn-upb.github.io/DeepCoMP/). Documentation is generated
+based on docstrings using [pdoc3](https://pdoc3.github.io/pdoc/): ``` # from
+project root pip install pdoc3 pdoc --force --html --output-dir docs deepcomp #
+move files to be picked up by GitHub pages mv docs/deepcomp/ docs/ # then
+manually adjust index.html to link to GitHub repo ``` ## Contributions
+Development: [@stefanbschneider](https://github.com/stefanbschneider/) Feature
+requests, questions, issues, and pull requests via GitHub are welcome. ##
+Acknowledgement DeepCoMP is an outcome of a joint project between Paderborn
+University, Germany, and Huawei Germany.
      [https://raw.githubusercontent.com/CN-UPB/DeepCoMP/master/docs/logos/
  upb.png?raw=true] [https://raw.githubusercontent.com/CN-UPB/DeepCoMP/master/
                   docs/logos/huawei_horizontal.png?raw=true]
 [Base station icon](https://thenounproject.com/search/
 ?q=base+station&i=1286474) (used in rendered videos) by Clea Doltz from the
 Noun Project.
```

### Comparing `deepcomp-1.4.1/README.md` & `deepcomp-1.4.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,46 @@
 [![CI](https://github.com/CN-UPB/DeepCoMP/actions/workflows/python-test.yml/badge.svg)](https://github.com/CN-UPB/DeepCoMP/actions/workflows/python-test.yml)
 [![PyPi](https://github.com/CN-UPB/DeepCoMP/actions/workflows/python-publish.yml/badge.svg?branch=v1.1.0)](https://github.com/CN-UPB/DeepCoMP/actions/workflows/python-publish.yml)
-[![Docker Cloud Build Status](https://img.shields.io/docker/cloud/build/stefanbschneider/deepcomp?label=Docker%20Build&logo=docker)](https://hub.docker.com/r/stefanbschneider/deepcomp)
 [![Docker Pulls](https://img.shields.io/docker/pulls/stefanbschneider/deepcomp?label=Docker%20Pulls&logo=docker)](https://hub.docker.com/r/stefanbschneider/deepcomp)
 [![DeepSource](https://deepsource.io/gh/CN-UPB/DeepCoMP.svg/?label=active+issues)](https://deepsource.io/gh/CN-UPB/DeepCoMP/?ref=repository-badge)
 
 
 # DeepCoMP: Self-Learning Dynamic Multi-Cell Selection for Coordinated Multipoint (CoMP)
 
-Deep reinforcement learning for dynamic multi-cell selection in CoMP scenarios.
+Multi-Agent Deep Reinforcement Learning for Coordinated Multipoint in Mobile Networks
+
 Three variants: DeepCoMP (central agent), DD-CoMP (distributed agents using central policy), D3-CoMP (distributed agents with separate policies).
 All three approaches self-learn and adapt to various scenarios in mobile networks without expert knowledge, human intervention, or detailed assumptions about the underlying system.
 Compared to other approaches, they are more flexible and achieve higher Quality of Experience.
 
+For a high-level overview of DeepCoMP, please refer to my [blog post](https://stefanbschneider.github.io/blog/deepcomp).
+More details are available in our research paper presenting DeepCoMP ([preprint](https://ris.uni-paderborn.de/download/33854/33855/preprint.pdf)).
+I also talked about DeepCoMP at the Ray Summit 2021 ([YouTube](https://youtu.be/Qy4SzJKXlGE)).
+
+The simulation environment used to train DeepCoMP is available separately as [mobile-env](https://github.com/stefanbschneider/mobile-env).
+
 <p align="center">
     <img src="https://raw.githubusercontent.com/CN-UPB/DeepCoMP/master/docs/gifs/dashboard_lossy.gif?raw=true"><br/>
     <em>Visualized cell selection policy of DeepCoMP after 2M training steps.</em><br>
     <sup><a href="https://thenounproject.com/search/?q=base+station&i=1286474" target="_blank">Base station icon</a> by Clea Doltz from the Noun Project</sup>
 </p>
 
+## Citation
+
+If you use this code, please cite our [paper (preprint; accepted at IEEE TNSM 2023)](https://ris.uni-paderborn.de/download/33854/33855):
+
+```
+@article{schneider2023deepcomp,
+	title={Multi-Agent Deep Reinforcement Learning for Coordinated Multipoint in Mobile Networks},
+	author={Schneider, Stefan and Karl, Holger and Khalili, Ramin and Hecker, Artur},
+	journal={IEEE Transactions on Network and Service Management (TNSM)},
+	year={2023},
+}
+```
+
 ## Setup
 
 You need Python 3.8+. You can install `deepcomp` either directly from [PyPi](https://pypi.org/project/deepcomp/) or manually after cloning this repository.
 
 ### Simple Installation via PyPi
 
 ```
```

#### html2text {}

```diff
@@ -1,112 +1,120 @@
 [![CI](https://github.com/CN-UPB/DeepCoMP/actions/workflows/python-test.yml/
 badge.svg)](https://github.com/CN-UPB/DeepCoMP/actions/workflows/python-
 test.yml) [![PyPi](https://github.com/CN-UPB/DeepCoMP/actions/workflows/python-
 publish.yml/badge.svg?branch=v1.1.0)](https://github.com/CN-UPB/DeepCoMP/
-actions/workflows/python-publish.yml) [![Docker Cloud Build Status](https://
-img.shields.io/docker/cloud/build/stefanbschneider/
-deepcomp?label=Docker%20Build&logo=docker)](https://hub.docker.com/r/
-stefanbschneider/deepcomp) [![Docker Pulls](https://img.shields.io/docker/
-pulls/stefanbschneider/deepcomp?label=Docker%20Pulls&logo=docker)](https://
-hub.docker.com/r/stefanbschneider/deepcomp) [![DeepSource](https://
+actions/workflows/python-publish.yml) [![Docker Pulls](https://img.shields.io/
+docker/pulls/stefanbschneider/deepcomp?label=Docker%20Pulls&logo=docker)]
+(https://hub.docker.com/r/stefanbschneider/deepcomp) [![DeepSource](https://
 deepsource.io/gh/CN-UPB/DeepCoMP.svg/?label=active+issues)](https://
 deepsource.io/gh/CN-UPB/DeepCoMP/?ref=repository-badge) # DeepCoMP: Self-
-Learning Dynamic Multi-Cell Selection for Coordinated Multipoint (CoMP) Deep
-reinforcement learning for dynamic multi-cell selection in CoMP scenarios.
+Learning Dynamic Multi-Cell Selection for Coordinated Multipoint (CoMP) Multi-
+Agent Deep Reinforcement Learning for Coordinated Multipoint in Mobile Networks
 Three variants: DeepCoMP (central agent), DD-CoMP (distributed agents using
 central policy), D3-CoMP (distributed agents with separate policies). All three
 approaches self-learn and adapt to various scenarios in mobile networks without
 expert knowledge, human intervention, or detailed assumptions about the
 underlying system. Compared to other approaches, they are more flexible and
-achieve higher Quality of Experience.
+achieve higher Quality of Experience. For a high-level overview of DeepCoMP,
+please refer to my [blog post](https://stefanbschneider.github.io/blog/
+deepcomp). More details are available in our research paper presenting DeepCoMP
+([preprint](https://ris.uni-paderborn.de/download/33854/33855/preprint.pdf)). I
+also talked about DeepCoMP at the Ray Summit 2021 ([YouTube](https://youtu.be/
+Qy4SzJKXlGE)). The simulation environment used to train DeepCoMP is available
+separately as [mobile-env](https://github.com/stefanbschneider/mobile-env).
      [https://raw.githubusercontent.com/CN-UPB/DeepCoMP/master/docs/gifs/
                          dashboard_lossy.gif?raw=true]
      Visualized cell selection policy of DeepCoMP after 2M training steps.
              Base_station_icon by Clea Doltz from the Noun Project
-## Setup You need Python 3.8+. You can install `deepcomp` either directly from
-[PyPi](https://pypi.org/project/deepcomp/) or manually after cloning this
-repository. ### Simple Installation via PyPi ``` sudo apt update sudo apt
-upgrade sudo apt install cmake build-essential zlib1g-dev python3-dev pip
-install deepcomp ``` ### Manual Installation from Source For adjusting or
-further developing DeepCoMP, it's better to install manually rather than from
-PyPi. Clone the repository. Then install everything, following these steps: ```
-# only on ubuntu sudo apt update sudo apt upgrade sudo apt install cmake build-
-essential zlib1g-dev python3-dev # clone git clone git@github.com:CN-UPB/
-DeepCoMP.git cd DeepCoMP # install all python dependencies pip install . #
-"python setup.py install" does not work for some reason: https://
-stackoverflow.com/a/66267232/2745116 # for development install (when changing
-code): pip install -e . ``` Tested on Ubuntu 20.04 and Windows 10 with Python
-3.8. For saving videos and gifs, you also need to install ffmpeg (not on
-Windows) and [ImageMagick](https://imagemagick.org/index.php). On Ubuntu: ```
-sudo apt install ffmpeg imagemagick ``` ### Docker There is a Docker image that
-comes with `deepcomp` preinstalled. To use the Docker image, simply pull the
-latest version from [Docker Hub](https://hub.docker.com/r/stefanbschneider/
-deepcomp): ``` docker pull stefanbschneider/deepcomp # tag image with just
-"deepcomp". alternatively, write out "stefanbschneider/deepcomp" in all
-following commands. docker tag stefanbschneider/deepcomp:latest deepcomp ```
-Alternatively, to build the Docker image manually from the `Dockerfile`, clone
-this repository and run ``` docker build -t deepcomp . ``` Use the `--no-cache`
-option is to force a rebuild of the image, pulling the latest `deepcomp`
-version from PyPI. ## Usage ``` # get an overview of all options deepcomp -
-h ``` For example: ``` deepcomp --env medium --slow-ues 3 --agent central --
-workers 2 --train-steps 50000 --seed 42 --video both ``` To run DeepCoMP, use
-`--alg ppo --agent central`. For DD-CoMP, use `--alg ppo --agent multi`, and
-for D3-CoMP, use `--alg ppo --agent multi --separate-agent-nns`. By default,
-training logs, results, videos, and trained agents are saved in `/results`,
-where `` is the root directory of DeepCoMP. If you cloned the repo from GitHub,
-this is where the Readme is. If you installed via PyPi, this is in your
-virtualenv's site packages. You can choose a custom location with `--result-dir
-`. ### Docker **Note:** By default, results within the Docker container are not
-stored persistently. To save them, copy them from the Docker container or use a
-Docker volume. #### Start the Container If you want to use the `deepcomp`
-Docker container and pulled the corresponding image from Docker Hub, you can
-use it as follows: ``` docker run -d -p 6006:6006 -p 8000:8000 --rm --shm-
-size=3gb --name deepcomp deepcomp ``` This starts the Docker container in the
-background, publishing port 6006 for TensorBoard and port 8000 for the HTTP
-server (described below). The container automatically starts TensorBoard and
-the HTTP server, so this does not need to be done manually. The `--rm` flag
-automatically removes the container once it is stopped. The `--shm-size=3gb`
-sets the size of `/dev/shm` inside the Docker container to 3 GB, which is too
-small by default. #### Use DeepCoMP on the Container To execute commands on the
-running Docker container, use `docker exec  ` as follows: ``` docker exec
-deepcomp deepcomp  ``` Here, the arguments are identical with the ones
-described above. For example, the following command lists all CLI options: ```
-docker exec deepcomp deepcomp -h ``` Or to train the central DeepCoMP agent for
-a short duration of 4000 steps: ``` docker exec -t deepcomp deepcomp --approach
-deepcomp --train-steps 4000 --batch-size 200 --ues 2 --result-dir results ```
-**Important:** Specify `--result-dir results` as argument. Otherwise, the
-results will be stored elsewhere and TensorFlow and the HTTP server will not
-find and display them. The other `deepcomp` arguments can be set as desired.
-The Docker `-t` flag ensures that the output is printed continuously during
-training, not just after completion. To inspect training progress or view
-create files (e.g., rendered videos), use TensorBoard and the HTTP server,
-which are available via `localhost:6006` and `localhost:8000`. #### Terminate
-the Container **Important:** Stopping the container will remove any files and
-training progress within the container. Stop the container with ``` docker stop
-deepcomp ``` ### Accessing results remotely When running remotely, you can
-serve the replay video by running: ``` cd results python -m http.server ```
-Then access at `:8000`. ### Tensorboard To view learning curves (and other
-metrics) when training an agent, use Tensorboard: ``` tensorboard --logdir
-results/train/ (--host 0.0.0.0) ``` Tensorboard is available at http://
-localhost:6006 (or `:6006` when running remotely). ### Scaling Up: Running
-DeepCoMP on multiple cores or a multi-node cluster To train DeepCoMP on
-multiple cores in parallel, configure the number of workers (corresponding to
-CPU cores) with `--workers`. To scale training to a multi-node cluster, adjust
-`cluster.yaml` and follow the steps described [here](https://
-stefanbschneider.github.io/blog/rllib-private-cluster). Set `--workers` to the
-total number of CPU cores you want to use on the entire cluster. ##
-Documentation API documentation is on [https://cn-upb.github.io/DeepCoMP/]
-(https://cn-upb.github.io/DeepCoMP/). Documentation is generated based on
-docstrings using [pdoc3](https://pdoc3.github.io/pdoc/): ``` # from project
-root pip install pdoc3 pdoc --force --html --output-dir docs deepcomp # move
-files to be picked up by GitHub pages mv docs/deepcomp/ docs/ # then manually
-adjust index.html to link to GitHub repo ``` ## Contributions Development:
-[@stefanbschneider](https://github.com/stefanbschneider/) Feature requests,
-questions, issues, and pull requests via GitHub are welcome. ## Acknowledgement
-DeepCoMP is an outcome of a joint project between Paderborn University,
-Germany, and Huawei Germany.
+## Citation If you use this code, please cite our [paper (preprint; accepted at
+IEEE TNSM 2023)](https://ris.uni-paderborn.de/download/33854/33855): ```
+@article{schneider2023deepcomp, title={Multi-Agent Deep Reinforcement Learning
+for Coordinated Multipoint in Mobile Networks}, author={Schneider, Stefan and
+Karl, Holger and Khalili, Ramin and Hecker, Artur}, journal={IEEE Transactions
+on Network and Service Management (TNSM)}, year={2023}, } ``` ## Setup You need
+Python 3.8+. You can install `deepcomp` either directly from [PyPi](https://
+pypi.org/project/deepcomp/) or manually after cloning this repository. ###
+Simple Installation via PyPi ``` sudo apt update sudo apt upgrade sudo apt
+install cmake build-essential zlib1g-dev python3-dev pip install deepcomp ```
+### Manual Installation from Source For adjusting or further developing
+DeepCoMP, it's better to install manually rather than from PyPi. Clone the
+repository. Then install everything, following these steps: ``` # only on
+ubuntu sudo apt update sudo apt upgrade sudo apt install cmake build-essential
+zlib1g-dev python3-dev # clone git clone git@github.com:CN-UPB/DeepCoMP.git cd
+DeepCoMP # install all python dependencies pip install . # "python setup.py
+install" does not work for some reason: https://stackoverflow.com/a/66267232/
+2745116 # for development install (when changing code): pip install -e . ```
+Tested on Ubuntu 20.04 and Windows 10 with Python 3.8. For saving videos and
+gifs, you also need to install ffmpeg (not on Windows) and [ImageMagick](https:
+//imagemagick.org/index.php). On Ubuntu: ``` sudo apt install ffmpeg
+imagemagick ``` ### Docker There is a Docker image that comes with `deepcomp`
+preinstalled. To use the Docker image, simply pull the latest version from
+[Docker Hub](https://hub.docker.com/r/stefanbschneider/deepcomp): ``` docker
+pull stefanbschneider/deepcomp # tag image with just "deepcomp". alternatively,
+write out "stefanbschneider/deepcomp" in all following commands. docker tag
+stefanbschneider/deepcomp:latest deepcomp ``` Alternatively, to build the
+Docker image manually from the `Dockerfile`, clone this repository and run ```
+docker build -t deepcomp . ``` Use the `--no-cache` option is to force a
+rebuild of the image, pulling the latest `deepcomp` version from PyPI. ## Usage
+``` # get an overview of all options deepcomp -h ``` For example: ``` deepcomp
+--env medium --slow-ues 3 --agent central --workers 2 --train-steps 50000 --
+seed 42 --video both ``` To run DeepCoMP, use `--alg ppo --agent central`. For
+DD-CoMP, use `--alg ppo --agent multi`, and for D3-CoMP, use `--alg ppo --agent
+multi --separate-agent-nns`. By default, training logs, results, videos, and
+trained agents are saved in `/results`, where `` is the root directory of
+DeepCoMP. If you cloned the repo from GitHub, this is where the Readme is. If
+you installed via PyPi, this is in your virtualenv's site packages. You can
+choose a custom location with `--result-dir `. ### Docker **Note:** By default,
+results within the Docker container are not stored persistently. To save them,
+copy them from the Docker container or use a Docker volume. #### Start the
+Container If you want to use the `deepcomp` Docker container and pulled the
+corresponding image from Docker Hub, you can use it as follows: ``` docker run
+-d -p 6006:6006 -p 8000:8000 --rm --shm-size=3gb --name deepcomp deepcomp ```
+This starts the Docker container in the background, publishing port 6006 for
+TensorBoard and port 8000 for the HTTP server (described below). The container
+automatically starts TensorBoard and the HTTP server, so this does not need to
+be done manually. The `--rm` flag automatically removes the container once it
+is stopped. The `--shm-size=3gb` sets the size of `/dev/shm` inside the Docker
+container to 3 GB, which is too small by default. #### Use DeepCoMP on the
+Container To execute commands on the running Docker container, use `docker exec
+` as follows: ``` docker exec deepcomp deepcomp  ``` Here, the arguments are
+identical with the ones described above. For example, the following command
+lists all CLI options: ``` docker exec deepcomp deepcomp -h ``` Or to train the
+central DeepCoMP agent for a short duration of 4000 steps: ``` docker exec -
+t deepcomp deepcomp --approach deepcomp --train-steps 4000 --batch-size 200 --
+ues 2 --result-dir results ``` **Important:** Specify `--result-dir results` as
+argument. Otherwise, the results will be stored elsewhere and TensorFlow and
+the HTTP server will not find and display them. The other `deepcomp` arguments
+can be set as desired. The Docker `-t` flag ensures that the output is printed
+continuously during training, not just after completion. To inspect training
+progress or view create files (e.g., rendered videos), use TensorBoard and the
+HTTP server, which are available via `localhost:6006` and `localhost:8000`.
+#### Terminate the Container **Important:** Stopping the container will remove
+any files and training progress within the container. Stop the container with
+``` docker stop deepcomp ``` ### Accessing results remotely When running
+remotely, you can serve the replay video by running: ``` cd results python -
+m http.server ``` Then access at `:8000`. ### Tensorboard To view learning
+curves (and other metrics) when training an agent, use Tensorboard: ```
+tensorboard --logdir results/train/ (--host 0.0.0.0) ``` Tensorboard is
+available at http://localhost:6006 (or `:6006` when running remotely). ###
+Scaling Up: Running DeepCoMP on multiple cores or a multi-node cluster To train
+DeepCoMP on multiple cores in parallel, configure the number of workers
+(corresponding to CPU cores) with `--workers`. To scale training to a multi-
+node cluster, adjust `cluster.yaml` and follow the steps described [here]
+(https://stefanbschneider.github.io/blog/rllib-private-cluster). Set `--
+workers` to the total number of CPU cores you want to use on the entire
+cluster. ## Documentation API documentation is on [https://cn-upb.github.io/
+DeepCoMP/](https://cn-upb.github.io/DeepCoMP/). Documentation is generated
+based on docstrings using [pdoc3](https://pdoc3.github.io/pdoc/): ``` # from
+project root pip install pdoc3 pdoc --force --html --output-dir docs deepcomp #
+move files to be picked up by GitHub pages mv docs/deepcomp/ docs/ # then
+manually adjust index.html to link to GitHub repo ``` ## Contributions
+Development: [@stefanbschneider](https://github.com/stefanbschneider/) Feature
+requests, questions, issues, and pull requests via GitHub are welcome. ##
+Acknowledgement DeepCoMP is an outcome of a joint project between Paderborn
+University, Germany, and Huawei Germany.
      [https://raw.githubusercontent.com/CN-UPB/DeepCoMP/master/docs/logos/
  upb.png?raw=true] [https://raw.githubusercontent.com/CN-UPB/DeepCoMP/master/
                   docs/logos/huawei_horizontal.png?raw=true]
 [Base station icon](https://thenounproject.com/search/
 ?q=base+station&i=1286474) (used in rendered videos) by Clea Doltz from the
 Noun Project.
```

### Comparing `deepcomp-1.4.1/deepcomp/agent/base.py` & `deepcomp-1.4.2/deepcomp/agent/base.py`

 * *Files identical despite different names*

### Comparing `deepcomp-1.4.1/deepcomp/agent/brute_force.py` & `deepcomp-1.4.2/deepcomp/agent/brute_force.py`

 * *Files identical despite different names*

### Comparing `deepcomp-1.4.1/deepcomp/agent/dummy.py` & `deepcomp-1.4.2/deepcomp/agent/dummy.py`

 * *Files identical despite different names*

### Comparing `deepcomp-1.4.1/deepcomp/agent/heuristics.py` & `deepcomp-1.4.2/deepcomp/agent/heuristics.py`

 * *Files identical despite different names*

### Comparing `deepcomp-1.4.1/deepcomp/env/entities/map.py` & `deepcomp-1.4.2/deepcomp/env/entities/map.py`

 * *Files identical despite different names*

### Comparing `deepcomp-1.4.1/deepcomp/env/entities/station.py` & `deepcomp-1.4.2/deepcomp/env/entities/station.py`

 * *Files identical despite different names*

### Comparing `deepcomp-1.4.1/deepcomp/env/entities/user.py` & `deepcomp-1.4.2/deepcomp/env/entities/user.py`

 * *Files identical despite different names*

### Comparing `deepcomp-1.4.1/deepcomp/env/multi_ue/central.py` & `deepcomp-1.4.2/deepcomp/env/multi_ue/central.py`

 * *Files identical despite different names*

### Comparing `deepcomp-1.4.1/deepcomp/env/multi_ue/multi_agent.py` & `deepcomp-1.4.2/deepcomp/env/multi_ue/multi_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
             self.curr_ue.id: done,
             '__all__': done,
         }
         return dones
 
     def info(self):
         """Same for info: Only for curr UE. Then increment to next UE since it's the last operation in the step"""
-        info_dict = super(MultiAgentMobileEnv, self).info()
+        info_dict = super().info()
         return {self.curr_ue.id: info_dict}
 
     def step(self, action):
         """Overwrite step to do sequential steps per agent without moving UEs and incrementing time in each step"""
         # when reaching the last UE in the order, move time, UEs, etc
         # if self.ue_order_idx >= len(self.ue_order):
         #     self.ue_order_idx = 0
```

### Comparing `deepcomp-1.4.1/deepcomp/env/single_ue/base.py` & `deepcomp-1.4.2/deepcomp/env/single_ue/base.py`

 * *Files identical despite different names*

### Comparing `deepcomp-1.4.1/deepcomp/env/single_ue/variants.py` & `deepcomp-1.4.2/deepcomp/env/single_ue/variants.py`

 * *Files identical despite different names*

### Comparing `deepcomp-1.4.1/deepcomp/env/util/movement.py` & `deepcomp-1.4.2/deepcomp/env/util/movement.py`

 * *Files identical despite different names*

### Comparing `deepcomp-1.4.1/deepcomp/env/util/utility.py` & `deepcomp-1.4.2/deepcomp/env/util/utility.py`

 * *Files identical despite different names*

### Comparing `deepcomp-1.4.1/deepcomp/main.py` & `deepcomp-1.4.2/deepcomp/main.py`

 * *Files identical despite different names*

### Comparing `deepcomp-1.4.1/deepcomp/util/callbacks.py` & `deepcomp-1.4.2/deepcomp/util/callbacks.py`

 * *Files identical despite different names*

### Comparing `deepcomp-1.4.1/deepcomp/util/cli.py` & `deepcomp-1.4.2/deepcomp/util/cli.py`

 * *Files identical despite different names*

### Comparing `deepcomp-1.4.1/deepcomp/util/constants.py` & `deepcomp-1.4.2/deepcomp/util/constants.py`

 * *Files identical despite different names*

### Comparing `deepcomp-1.4.1/deepcomp/util/env_setup.py` & `deepcomp-1.4.2/deepcomp/util/env_setup.py`

 * *Files identical despite different names*

### Comparing `deepcomp-1.4.1/deepcomp/util/logs.py` & `deepcomp-1.4.2/deepcomp/util/logs.py`

 * *Files identical despite different names*

### Comparing `deepcomp-1.4.1/deepcomp/util/simulation.py` & `deepcomp-1.4.2/deepcomp/util/simulation.py`

 * *Files identical despite different names*

### Comparing `deepcomp-1.4.1/deepcomp.egg-info/PKG-INFO` & `deepcomp-1.4.2/deepcomp.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,59 @@
 Metadata-Version: 2.1
 Name: deepcomp
-Version: 1.4.1
+Version: 1.4.2
 Summary: DeepCoMP: Self-Learning Dynamic Multi-Cell Selection for Coordinated Multipoint (CoMP)
 Home-page: https://github.com/CN-UPB/DeepCoMP
 Author: Stefan Schneider
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8.*
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![CI](https://github.com/CN-UPB/DeepCoMP/actions/workflows/python-test.yml/badge.svg)](https://github.com/CN-UPB/DeepCoMP/actions/workflows/python-test.yml)
 [![PyPi](https://github.com/CN-UPB/DeepCoMP/actions/workflows/python-publish.yml/badge.svg?branch=v1.1.0)](https://github.com/CN-UPB/DeepCoMP/actions/workflows/python-publish.yml)
-[![Docker Cloud Build Status](https://img.shields.io/docker/cloud/build/stefanbschneider/deepcomp?label=Docker%20Build&logo=docker)](https://hub.docker.com/r/stefanbschneider/deepcomp)
 [![Docker Pulls](https://img.shields.io/docker/pulls/stefanbschneider/deepcomp?label=Docker%20Pulls&logo=docker)](https://hub.docker.com/r/stefanbschneider/deepcomp)
 [![DeepSource](https://deepsource.io/gh/CN-UPB/DeepCoMP.svg/?label=active+issues)](https://deepsource.io/gh/CN-UPB/DeepCoMP/?ref=repository-badge)
 
 
 # DeepCoMP: Self-Learning Dynamic Multi-Cell Selection for Coordinated Multipoint (CoMP)
 
-Deep reinforcement learning for dynamic multi-cell selection in CoMP scenarios.
+Multi-Agent Deep Reinforcement Learning for Coordinated Multipoint in Mobile Networks
+
 Three variants: DeepCoMP (central agent), DD-CoMP (distributed agents using central policy), D3-CoMP (distributed agents with separate policies).
 All three approaches self-learn and adapt to various scenarios in mobile networks without expert knowledge, human intervention, or detailed assumptions about the underlying system.
 Compared to other approaches, they are more flexible and achieve higher Quality of Experience.
 
+For a high-level overview of DeepCoMP, please refer to my [blog post](https://stefanbschneider.github.io/blog/deepcomp).
+More details are available in our research paper presenting DeepCoMP ([preprint](https://ris.uni-paderborn.de/download/33854/33855/preprint.pdf)).
+I also talked about DeepCoMP at the Ray Summit 2021 ([YouTube](https://youtu.be/Qy4SzJKXlGE)).
+
+The simulation environment used to train DeepCoMP is available separately as [mobile-env](https://github.com/stefanbschneider/mobile-env).
+
 <p align="center">
     <img src="https://raw.githubusercontent.com/CN-UPB/DeepCoMP/master/docs/gifs/dashboard_lossy.gif?raw=true"><br/>
     <em>Visualized cell selection policy of DeepCoMP after 2M training steps.</em><br>
     <sup><a href="https://thenounproject.com/search/?q=base+station&i=1286474" target="_blank">Base station icon</a> by Clea Doltz from the Noun Project</sup>
 </p>
 
+## Citation
+
+If you use this code, please cite our [paper (preprint; accepted at IEEE TNSM 2023)](https://ris.uni-paderborn.de/download/33854/33855):
+
+```
+@article{schneider2023deepcomp,
+	title={Multi-Agent Deep Reinforcement Learning for Coordinated Multipoint in Mobile Networks},
+	author={Schneider, Stefan and Karl, Holger and Khalili, Ramin and Hecker, Artur},
+	journal={IEEE Transactions on Network and Service Management (TNSM)},
+	year={2023},
+}
+```
+
 ## Setup
 
 You need Python 3.8+. You can install `deepcomp` either directly from [PyPi](https://pypi.org/project/deepcomp/) or manually after cloning this repository.
 
 ### Simple Installation via PyPi
 
 ```
@@ -225,9 +242,7 @@
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/CN-UPB/DeepCoMP/master/docs/logos/upb.png?raw=true" width="200" hspace="30"/>
     <img src="https://raw.githubusercontent.com/CN-UPB/DeepCoMP/master/docs/logos/huawei_horizontal.png?raw=true" width="250" hspace="30"/>
 </p>
 
 [Base station icon](https://thenounproject.com/search/?q=base+station&i=1286474) (used in rendered videos) by Clea Doltz from the Noun Project.
-
-
```

#### html2text {}

```diff
@@ -1,118 +1,126 @@
-Metadata-Version: 2.1 Name: deepcomp Version: 1.4.1 Summary: DeepCoMP: Self-
+Metadata-Version: 2.1 Name: deepcomp Version: 1.4.2 Summary: DeepCoMP: Self-
 Learning Dynamic Multi-Cell Selection for Coordinated Multipoint (CoMP) Home-
-page: https://github.com/CN-UPB/DeepCoMP Author: Stefan Schneider License:
-UNKNOWN Platform: UNKNOWN Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Requires-Python: >=3.8.* Description-Content-Type: text/
-markdown License-File: LICENSE [![CI](https://github.com/CN-UPB/DeepCoMP/
-actions/workflows/python-test.yml/badge.svg)](https://github.com/CN-UPB/
-DeepCoMP/actions/workflows/python-test.yml) [![PyPi](https://github.com/CN-UPB/
-DeepCoMP/actions/workflows/python-publish.yml/badge.svg?branch=v1.1.0)](https:/
-/github.com/CN-UPB/DeepCoMP/actions/workflows/python-publish.yml) [![Docker
-Cloud Build Status](https://img.shields.io/docker/cloud/build/stefanbschneider/
-deepcomp?label=Docker%20Build&logo=docker)](https://hub.docker.com/r/
-stefanbschneider/deepcomp) [![Docker Pulls](https://img.shields.io/docker/
-pulls/stefanbschneider/deepcomp?label=Docker%20Pulls&logo=docker)](https://
+page: https://github.com/CN-UPB/DeepCoMP Author: Stefan Schneider Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown License-File: LICENSE [![CI](https://
+github.com/CN-UPB/DeepCoMP/actions/workflows/python-test.yml/badge.svg)](https:
+//github.com/CN-UPB/DeepCoMP/actions/workflows/python-test.yml) [![PyPi](https:
+//github.com/CN-UPB/DeepCoMP/actions/workflows/python-publish.yml/
+badge.svg?branch=v1.1.0)](https://github.com/CN-UPB/DeepCoMP/actions/workflows/
+python-publish.yml) [![Docker Pulls](https://img.shields.io/docker/pulls/
+stefanbschneider/deepcomp?label=Docker%20Pulls&logo=docker)](https://
 hub.docker.com/r/stefanbschneider/deepcomp) [![DeepSource](https://
 deepsource.io/gh/CN-UPB/DeepCoMP.svg/?label=active+issues)](https://
 deepsource.io/gh/CN-UPB/DeepCoMP/?ref=repository-badge) # DeepCoMP: Self-
-Learning Dynamic Multi-Cell Selection for Coordinated Multipoint (CoMP) Deep
-reinforcement learning for dynamic multi-cell selection in CoMP scenarios.
+Learning Dynamic Multi-Cell Selection for Coordinated Multipoint (CoMP) Multi-
+Agent Deep Reinforcement Learning for Coordinated Multipoint in Mobile Networks
 Three variants: DeepCoMP (central agent), DD-CoMP (distributed agents using
 central policy), D3-CoMP (distributed agents with separate policies). All three
 approaches self-learn and adapt to various scenarios in mobile networks without
 expert knowledge, human intervention, or detailed assumptions about the
 underlying system. Compared to other approaches, they are more flexible and
-achieve higher Quality of Experience.
+achieve higher Quality of Experience. For a high-level overview of DeepCoMP,
+please refer to my [blog post](https://stefanbschneider.github.io/blog/
+deepcomp). More details are available in our research paper presenting DeepCoMP
+([preprint](https://ris.uni-paderborn.de/download/33854/33855/preprint.pdf)). I
+also talked about DeepCoMP at the Ray Summit 2021 ([YouTube](https://youtu.be/
+Qy4SzJKXlGE)). The simulation environment used to train DeepCoMP is available
+separately as [mobile-env](https://github.com/stefanbschneider/mobile-env).
      [https://raw.githubusercontent.com/CN-UPB/DeepCoMP/master/docs/gifs/
                          dashboard_lossy.gif?raw=true]
      Visualized cell selection policy of DeepCoMP after 2M training steps.
              Base_station_icon by Clea Doltz from the Noun Project
-## Setup You need Python 3.8+. You can install `deepcomp` either directly from
-[PyPi](https://pypi.org/project/deepcomp/) or manually after cloning this
-repository. ### Simple Installation via PyPi ``` sudo apt update sudo apt
-upgrade sudo apt install cmake build-essential zlib1g-dev python3-dev pip
-install deepcomp ``` ### Manual Installation from Source For adjusting or
-further developing DeepCoMP, it's better to install manually rather than from
-PyPi. Clone the repository. Then install everything, following these steps: ```
-# only on ubuntu sudo apt update sudo apt upgrade sudo apt install cmake build-
-essential zlib1g-dev python3-dev # clone git clone git@github.com:CN-UPB/
-DeepCoMP.git cd DeepCoMP # install all python dependencies pip install . #
-"python setup.py install" does not work for some reason: https://
-stackoverflow.com/a/66267232/2745116 # for development install (when changing
-code): pip install -e . ``` Tested on Ubuntu 20.04 and Windows 10 with Python
-3.8. For saving videos and gifs, you also need to install ffmpeg (not on
-Windows) and [ImageMagick](https://imagemagick.org/index.php). On Ubuntu: ```
-sudo apt install ffmpeg imagemagick ``` ### Docker There is a Docker image that
-comes with `deepcomp` preinstalled. To use the Docker image, simply pull the
-latest version from [Docker Hub](https://hub.docker.com/r/stefanbschneider/
-deepcomp): ``` docker pull stefanbschneider/deepcomp # tag image with just
-"deepcomp". alternatively, write out "stefanbschneider/deepcomp" in all
-following commands. docker tag stefanbschneider/deepcomp:latest deepcomp ```
-Alternatively, to build the Docker image manually from the `Dockerfile`, clone
-this repository and run ``` docker build -t deepcomp . ``` Use the `--no-cache`
-option is to force a rebuild of the image, pulling the latest `deepcomp`
-version from PyPI. ## Usage ``` # get an overview of all options deepcomp -
-h ``` For example: ``` deepcomp --env medium --slow-ues 3 --agent central --
-workers 2 --train-steps 50000 --seed 42 --video both ``` To run DeepCoMP, use
-`--alg ppo --agent central`. For DD-CoMP, use `--alg ppo --agent multi`, and
-for D3-CoMP, use `--alg ppo --agent multi --separate-agent-nns`. By default,
-training logs, results, videos, and trained agents are saved in `/results`,
-where `` is the root directory of DeepCoMP. If you cloned the repo from GitHub,
-this is where the Readme is. If you installed via PyPi, this is in your
-virtualenv's site packages. You can choose a custom location with `--result-dir
-`. ### Docker **Note:** By default, results within the Docker container are not
-stored persistently. To save them, copy them from the Docker container or use a
-Docker volume. #### Start the Container If you want to use the `deepcomp`
-Docker container and pulled the corresponding image from Docker Hub, you can
-use it as follows: ``` docker run -d -p 6006:6006 -p 8000:8000 --rm --shm-
-size=3gb --name deepcomp deepcomp ``` This starts the Docker container in the
-background, publishing port 6006 for TensorBoard and port 8000 for the HTTP
-server (described below). The container automatically starts TensorBoard and
-the HTTP server, so this does not need to be done manually. The `--rm` flag
-automatically removes the container once it is stopped. The `--shm-size=3gb`
-sets the size of `/dev/shm` inside the Docker container to 3 GB, which is too
-small by default. #### Use DeepCoMP on the Container To execute commands on the
-running Docker container, use `docker exec  ` as follows: ``` docker exec
-deepcomp deepcomp  ``` Here, the arguments are identical with the ones
-described above. For example, the following command lists all CLI options: ```
-docker exec deepcomp deepcomp -h ``` Or to train the central DeepCoMP agent for
-a short duration of 4000 steps: ``` docker exec -t deepcomp deepcomp --approach
-deepcomp --train-steps 4000 --batch-size 200 --ues 2 --result-dir results ```
-**Important:** Specify `--result-dir results` as argument. Otherwise, the
-results will be stored elsewhere and TensorFlow and the HTTP server will not
-find and display them. The other `deepcomp` arguments can be set as desired.
-The Docker `-t` flag ensures that the output is printed continuously during
-training, not just after completion. To inspect training progress or view
-create files (e.g., rendered videos), use TensorBoard and the HTTP server,
-which are available via `localhost:6006` and `localhost:8000`. #### Terminate
-the Container **Important:** Stopping the container will remove any files and
-training progress within the container. Stop the container with ``` docker stop
-deepcomp ``` ### Accessing results remotely When running remotely, you can
-serve the replay video by running: ``` cd results python -m http.server ```
-Then access at `:8000`. ### Tensorboard To view learning curves (and other
-metrics) when training an agent, use Tensorboard: ``` tensorboard --logdir
-results/train/ (--host 0.0.0.0) ``` Tensorboard is available at http://
-localhost:6006 (or `:6006` when running remotely). ### Scaling Up: Running
-DeepCoMP on multiple cores or a multi-node cluster To train DeepCoMP on
-multiple cores in parallel, configure the number of workers (corresponding to
-CPU cores) with `--workers`. To scale training to a multi-node cluster, adjust
-`cluster.yaml` and follow the steps described [here](https://
-stefanbschneider.github.io/blog/rllib-private-cluster). Set `--workers` to the
-total number of CPU cores you want to use on the entire cluster. ##
-Documentation API documentation is on [https://cn-upb.github.io/DeepCoMP/]
-(https://cn-upb.github.io/DeepCoMP/). Documentation is generated based on
-docstrings using [pdoc3](https://pdoc3.github.io/pdoc/): ``` # from project
-root pip install pdoc3 pdoc --force --html --output-dir docs deepcomp # move
-files to be picked up by GitHub pages mv docs/deepcomp/ docs/ # then manually
-adjust index.html to link to GitHub repo ``` ## Contributions Development:
-[@stefanbschneider](https://github.com/stefanbschneider/) Feature requests,
-questions, issues, and pull requests via GitHub are welcome. ## Acknowledgement
-DeepCoMP is an outcome of a joint project between Paderborn University,
-Germany, and Huawei Germany.
+## Citation If you use this code, please cite our [paper (preprint; accepted at
+IEEE TNSM 2023)](https://ris.uni-paderborn.de/download/33854/33855): ```
+@article{schneider2023deepcomp, title={Multi-Agent Deep Reinforcement Learning
+for Coordinated Multipoint in Mobile Networks}, author={Schneider, Stefan and
+Karl, Holger and Khalili, Ramin and Hecker, Artur}, journal={IEEE Transactions
+on Network and Service Management (TNSM)}, year={2023}, } ``` ## Setup You need
+Python 3.8+. You can install `deepcomp` either directly from [PyPi](https://
+pypi.org/project/deepcomp/) or manually after cloning this repository. ###
+Simple Installation via PyPi ``` sudo apt update sudo apt upgrade sudo apt
+install cmake build-essential zlib1g-dev python3-dev pip install deepcomp ```
+### Manual Installation from Source For adjusting or further developing
+DeepCoMP, it's better to install manually rather than from PyPi. Clone the
+repository. Then install everything, following these steps: ``` # only on
+ubuntu sudo apt update sudo apt upgrade sudo apt install cmake build-essential
+zlib1g-dev python3-dev # clone git clone git@github.com:CN-UPB/DeepCoMP.git cd
+DeepCoMP # install all python dependencies pip install . # "python setup.py
+install" does not work for some reason: https://stackoverflow.com/a/66267232/
+2745116 # for development install (when changing code): pip install -e . ```
+Tested on Ubuntu 20.04 and Windows 10 with Python 3.8. For saving videos and
+gifs, you also need to install ffmpeg (not on Windows) and [ImageMagick](https:
+//imagemagick.org/index.php). On Ubuntu: ``` sudo apt install ffmpeg
+imagemagick ``` ### Docker There is a Docker image that comes with `deepcomp`
+preinstalled. To use the Docker image, simply pull the latest version from
+[Docker Hub](https://hub.docker.com/r/stefanbschneider/deepcomp): ``` docker
+pull stefanbschneider/deepcomp # tag image with just "deepcomp". alternatively,
+write out "stefanbschneider/deepcomp" in all following commands. docker tag
+stefanbschneider/deepcomp:latest deepcomp ``` Alternatively, to build the
+Docker image manually from the `Dockerfile`, clone this repository and run ```
+docker build -t deepcomp . ``` Use the `--no-cache` option is to force a
+rebuild of the image, pulling the latest `deepcomp` version from PyPI. ## Usage
+``` # get an overview of all options deepcomp -h ``` For example: ``` deepcomp
+--env medium --slow-ues 3 --agent central --workers 2 --train-steps 50000 --
+seed 42 --video both ``` To run DeepCoMP, use `--alg ppo --agent central`. For
+DD-CoMP, use `--alg ppo --agent multi`, and for D3-CoMP, use `--alg ppo --agent
+multi --separate-agent-nns`. By default, training logs, results, videos, and
+trained agents are saved in `/results`, where `` is the root directory of
+DeepCoMP. If you cloned the repo from GitHub, this is where the Readme is. If
+you installed via PyPi, this is in your virtualenv's site packages. You can
+choose a custom location with `--result-dir `. ### Docker **Note:** By default,
+results within the Docker container are not stored persistently. To save them,
+copy them from the Docker container or use a Docker volume. #### Start the
+Container If you want to use the `deepcomp` Docker container and pulled the
+corresponding image from Docker Hub, you can use it as follows: ``` docker run
+-d -p 6006:6006 -p 8000:8000 --rm --shm-size=3gb --name deepcomp deepcomp ```
+This starts the Docker container in the background, publishing port 6006 for
+TensorBoard and port 8000 for the HTTP server (described below). The container
+automatically starts TensorBoard and the HTTP server, so this does not need to
+be done manually. The `--rm` flag automatically removes the container once it
+is stopped. The `--shm-size=3gb` sets the size of `/dev/shm` inside the Docker
+container to 3 GB, which is too small by default. #### Use DeepCoMP on the
+Container To execute commands on the running Docker container, use `docker exec
+` as follows: ``` docker exec deepcomp deepcomp  ``` Here, the arguments are
+identical with the ones described above. For example, the following command
+lists all CLI options: ``` docker exec deepcomp deepcomp -h ``` Or to train the
+central DeepCoMP agent for a short duration of 4000 steps: ``` docker exec -
+t deepcomp deepcomp --approach deepcomp --train-steps 4000 --batch-size 200 --
+ues 2 --result-dir results ``` **Important:** Specify `--result-dir results` as
+argument. Otherwise, the results will be stored elsewhere and TensorFlow and
+the HTTP server will not find and display them. The other `deepcomp` arguments
+can be set as desired. The Docker `-t` flag ensures that the output is printed
+continuously during training, not just after completion. To inspect training
+progress or view create files (e.g., rendered videos), use TensorBoard and the
+HTTP server, which are available via `localhost:6006` and `localhost:8000`.
+#### Terminate the Container **Important:** Stopping the container will remove
+any files and training progress within the container. Stop the container with
+``` docker stop deepcomp ``` ### Accessing results remotely When running
+remotely, you can serve the replay video by running: ``` cd results python -
+m http.server ``` Then access at `:8000`. ### Tensorboard To view learning
+curves (and other metrics) when training an agent, use Tensorboard: ```
+tensorboard --logdir results/train/ (--host 0.0.0.0) ``` Tensorboard is
+available at http://localhost:6006 (or `:6006` when running remotely). ###
+Scaling Up: Running DeepCoMP on multiple cores or a multi-node cluster To train
+DeepCoMP on multiple cores in parallel, configure the number of workers
+(corresponding to CPU cores) with `--workers`. To scale training to a multi-
+node cluster, adjust `cluster.yaml` and follow the steps described [here]
+(https://stefanbschneider.github.io/blog/rllib-private-cluster). Set `--
+workers` to the total number of CPU cores you want to use on the entire
+cluster. ## Documentation API documentation is on [https://cn-upb.github.io/
+DeepCoMP/](https://cn-upb.github.io/DeepCoMP/). Documentation is generated
+based on docstrings using [pdoc3](https://pdoc3.github.io/pdoc/): ``` # from
+project root pip install pdoc3 pdoc --force --html --output-dir docs deepcomp #
+move files to be picked up by GitHub pages mv docs/deepcomp/ docs/ # then
+manually adjust index.html to link to GitHub repo ``` ## Contributions
+Development: [@stefanbschneider](https://github.com/stefanbschneider/) Feature
+requests, questions, issues, and pull requests via GitHub are welcome. ##
+Acknowledgement DeepCoMP is an outcome of a joint project between Paderborn
+University, Germany, and Huawei Germany.
      [https://raw.githubusercontent.com/CN-UPB/DeepCoMP/master/docs/logos/
  upb.png?raw=true] [https://raw.githubusercontent.com/CN-UPB/DeepCoMP/master/
                   docs/logos/huawei_horizontal.png?raw=true]
 [Base station icon](https://thenounproject.com/search/
 ?q=base+station&i=1286474) (used in rendered videos) by Clea Doltz from the
 Noun Project.
```

### Comparing `deepcomp-1.4.1/deepcomp.egg-info/SOURCES.txt` & `deepcomp-1.4.2/deepcomp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepcomp-1.4.1/setup.py` & `deepcomp-1.4.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,41 +14,45 @@
     'ray[rllib]==1.4.0',
     'structlog>=20.2.0',
     'structlog-round>=1.0',
     'shapely==1.7.0',
     'matplotlib==3.2.1',
     'seaborn==0.10.1',
     'numpy<1.20',
-    'gym[atari]>=0.17.1',
+    'gym[atari]>=0.17.1,<0.23.0',
     'tensorflow>=2.2.0',
     'gputil==1.4.0',
     'pandas>=1.0.5',
     'tqdm==4.47.0',
     'joblib==0.16.0',
     # extra dependencies for Ray RLlib
     # installing directly via ray[rllib] doesn't work with setup.py: https://github.com/ray-project/ray/issues/11274
     'scipy==1.4.1',
+    # need to pin protobuf to avoid import errors: https://stackoverflow.com/q/71759248/2745116
+    'protobuf==3.20.3',
+    # same for pydantic: https://github.com/aws/aws-sdk-pandas/issues/2379#issuecomment-1621178909
+    'pydantic<2.0.0',
     # 'lz4',
     'svgpath2mpl>=0.2.1',
 ]
 
 eval_requirements = [
     'jupyter>=1.0.0'
 ]
 
 setup(
     name='deepcomp',
-    version='1.4.1',
+    version='1.4.2',
     author='Stefan Schneider',
     description="DeepCoMP: Self-Learning Dynamic Multi-Cell Selection for Coordinated Multipoint (CoMP)",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/CN-UPB/DeepCoMP',
     packages=find_packages(),
-    python_requires=">=3.8.*",
+    python_requires=">=3.8.0",
     install_requires=requirements + eval_requirements,
     zip_safe=False,
     entry_points={
         'console_scripts': [
             'deepcomp=deepcomp.main:main'
         ]
     },
```

