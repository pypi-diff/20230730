# Comparing `tmp/nn4n-1.0.1.tar.gz` & `tmp/nn4n-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nn4n-1.0.1.tar", last modified: Sun Jul 30 04:34:16 2023, max compression
+gzip compressed data, was "nn4n-1.0.2.tar", last modified: Sun Jul 30 05:19:43 2023, max compression
```

## Comparing `nn4n-1.0.1.tar` & `nn4n-1.0.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 zhaoze     (501) staff       (20)        0 2023-07-30 04:34:16.500700 nn4n-1.0.1/
--rw-r--r--   0 zhaoze     (501) staff       (20)     1067 2023-06-06 17:26:01.000000 nn4n-1.0.1/LICENSE
--rw-r--r--   0 zhaoze     (501) staff       (20)     4800 2023-07-30 04:34:16.500558 nn4n-1.0.1/PKG-INFO
--rw-r--r--   0 zhaoze     (501) staff       (20)     4581 2023-07-30 04:24:49.000000 nn4n-1.0.1/README.md
-drwxr-xr-x   0 zhaoze     (501) staff       (20)        0 2023-07-30 04:34:16.496322 nn4n-1.0.1/nn4n/
--rw-r--r--   0 zhaoze     (501) staff       (20)        0 2023-06-13 19:47:30.000000 nn4n-1.0.1/nn4n/__init__.py
-drwxr-xr-x   0 zhaoze     (501) staff       (20)        0 2023-07-30 04:34:16.497664 nn4n-1.0.1/nn4n/criterion/
--rw-r--r--   0 zhaoze     (501) staff       (20)       77 2023-07-27 18:59:07.000000 nn4n-1.0.1/nn4n/criterion/__init__.py
--rw-r--r--   0 zhaoze     (501) staff       (20)     3721 2023-07-27 20:19:55.000000 nn4n-1.0.1/nn4n/criterion/rnn_loss.py
-drwxr-xr-x   0 zhaoze     (501) staff       (20)        0 2023-07-30 04:34:16.497853 nn4n-1.0.1/nn4n/model/
-drwxr-xr-x   0 zhaoze     (501) staff       (20)        0 2023-07-30 04:34:16.498741 nn4n-1.0.1/nn4n/model/CTRNN/
--rw-r--r--   0 zhaoze     (501) staff       (20)      262 2023-07-27 18:36:57.000000 nn4n-1.0.1/nn4n/model/CTRNN/__init__.py
--rw-r--r--   0 zhaoze     (501) staff       (20)     7608 2023-07-27 22:17:15.000000 nn4n-1.0.1/nn4n/model/CTRNN/ctrnn.py
--rw-r--r--   0 zhaoze     (501) staff       (20)    11237 2023-07-27 18:50:27.000000 nn4n-1.0.1/nn4n/model/CTRNN/hidden_layer.py
--rw-r--r--   0 zhaoze     (501) staff       (20)     9865 2023-07-27 21:12:23.000000 nn4n-1.0.1/nn4n/model/CTRNN/linear_layer.py
--rw-r--r--   0 zhaoze     (501) staff       (20)     7764 2023-07-29 16:14:19.000000 nn4n-1.0.1/nn4n/model/CTRNN/recurrent_layer.py
--rw-r--r--   0 zhaoze     (501) staff       (20)       70 2023-07-27 18:33:34.000000 nn4n-1.0.1/nn4n/model/__init__.py
-drwxr-xr-x   0 zhaoze     (501) staff       (20)        0 2023-07-30 04:34:16.499663 nn4n-1.0.1/nn4n/structure/
--rw-r--r--   0 zhaoze     (501) staff       (20)      206 2023-07-27 18:33:18.000000 nn4n-1.0.1/nn4n/structure/__init__.py
--rw-r--r--   0 zhaoze     (501) staff       (20)     4068 2023-07-30 03:40:50.000000 nn4n-1.0.1/nn4n/structure/base_struct.py
--rw-r--r--   0 zhaoze     (501) staff       (20)     6415 2023-07-30 03:20:15.000000 nn4n-1.0.1/nn4n/structure/multi_area.py
--rw-r--r--   0 zhaoze     (501) staff       (20)     4256 2023-07-27 19:12:25.000000 nn4n-1.0.1/nn4n/structure/multi_area_ei.py
--rw-r--r--   0 zhaoze     (501) staff       (20)     4050 2023-07-27 18:19:31.000000 nn4n-1.0.1/nn4n/structure/random_input.py
--rw-r--r--   0 zhaoze     (501) staff       (20)     1901 2023-07-30 04:00:06.000000 nn4n-1.0.1/nn4n/utils.py
-drwxr-xr-x   0 zhaoze     (501) staff       (20)        0 2023-07-30 04:34:16.497344 nn4n-1.0.1/nn4n.egg-info/
--rw-r--r--   0 zhaoze     (501) staff       (20)     4800 2023-07-30 04:34:16.000000 nn4n-1.0.1/nn4n.egg-info/PKG-INFO
--rw-r--r--   0 zhaoze     (501) staff       (20)      633 2023-07-30 04:34:16.000000 nn4n-1.0.1/nn4n.egg-info/SOURCES.txt
--rw-r--r--   0 zhaoze     (501) staff       (20)        1 2023-07-30 04:34:16.000000 nn4n-1.0.1/nn4n.egg-info/dependency_links.txt
--rw-r--r--   0 zhaoze     (501) staff       (20)       37 2023-07-30 04:34:16.000000 nn4n-1.0.1/nn4n.egg-info/requires.txt
--rw-r--r--   0 zhaoze     (501) staff       (20)        5 2023-07-30 04:34:16.000000 nn4n-1.0.1/nn4n.egg-info/top_level.txt
--rw-r--r--   0 zhaoze     (501) staff       (20)       38 2023-07-30 04:34:16.500746 nn4n-1.0.1/setup.cfg
--rw-r--r--   0 zhaoze     (501) staff       (20)      622 2023-07-30 04:34:10.000000 nn4n-1.0.1/setup.py
-drwxr-xr-x   0 zhaoze     (501) staff       (20)        0 2023-07-30 04:34:16.500322 nn4n-1.0.1/test/
--rw-r--r--   0 zhaoze     (501) staff       (20)     2014 2023-07-27 19:59:06.000000 nn4n-1.0.1/test/test_dep.py
--rw-r--r--   0 zhaoze     (501) staff       (20)     7599 2023-07-27 20:20:19.000000 nn4n-1.0.1/test/test_main.py
--rw-r--r--   0 zhaoze     (501) staff       (20)     2246 2023-07-30 04:05:55.000000 nn4n-1.0.1/test/test_utils.py
+drwxr-xr-x   0 zhaoze     (501) staff       (20)        0 2023-07-30 05:19:43.045440 nn4n-1.0.2/
+-rw-r--r--   0 zhaoze     (501) staff       (20)     1067 2023-06-06 17:26:01.000000 nn4n-1.0.2/LICENSE
+-rw-r--r--   0 zhaoze     (501) staff       (20)     4957 2023-07-30 05:19:43.045299 nn4n-1.0.2/PKG-INFO
+-rw-r--r--   0 zhaoze     (501) staff       (20)     4738 2023-07-30 05:04:21.000000 nn4n-1.0.2/README.md
+drwxr-xr-x   0 zhaoze     (501) staff       (20)        0 2023-07-30 05:19:43.041133 nn4n-1.0.2/nn4n/
+-rw-r--r--   0 zhaoze     (501) staff       (20)        0 2023-06-13 19:47:30.000000 nn4n-1.0.2/nn4n/__init__.py
+drwxr-xr-x   0 zhaoze     (501) staff       (20)        0 2023-07-30 05:19:43.042585 nn4n-1.0.2/nn4n/criterion/
+-rw-r--r--   0 zhaoze     (501) staff       (20)       77 2023-07-27 18:59:07.000000 nn4n-1.0.2/nn4n/criterion/__init__.py
+-rw-r--r--   0 zhaoze     (501) staff       (20)     3721 2023-07-27 20:19:55.000000 nn4n-1.0.2/nn4n/criterion/rnn_loss.py
+drwxr-xr-x   0 zhaoze     (501) staff       (20)        0 2023-07-30 05:19:43.042783 nn4n-1.0.2/nn4n/model/
+drwxr-xr-x   0 zhaoze     (501) staff       (20)        0 2023-07-30 05:19:43.043643 nn4n-1.0.2/nn4n/model/CTRNN/
+-rw-r--r--   0 zhaoze     (501) staff       (20)      262 2023-07-27 18:36:57.000000 nn4n-1.0.2/nn4n/model/CTRNN/__init__.py
+-rw-r--r--   0 zhaoze     (501) staff       (20)     7608 2023-07-27 22:17:15.000000 nn4n-1.0.2/nn4n/model/CTRNN/ctrnn.py
+-rw-r--r--   0 zhaoze     (501) staff       (20)    11237 2023-07-27 18:50:27.000000 nn4n-1.0.2/nn4n/model/CTRNN/hidden_layer.py
+-rw-r--r--   0 zhaoze     (501) staff       (20)     9865 2023-07-27 21:12:23.000000 nn4n-1.0.2/nn4n/model/CTRNN/linear_layer.py
+-rw-r--r--   0 zhaoze     (501) staff       (20)     7764 2023-07-29 16:14:19.000000 nn4n-1.0.2/nn4n/model/CTRNN/recurrent_layer.py
+-rw-r--r--   0 zhaoze     (501) staff       (20)       70 2023-07-27 18:33:34.000000 nn4n-1.0.2/nn4n/model/__init__.py
+drwxr-xr-x   0 zhaoze     (501) staff       (20)        0 2023-07-30 05:19:43.044547 nn4n-1.0.2/nn4n/structure/
+-rw-r--r--   0 zhaoze     (501) staff       (20)      206 2023-07-27 18:33:18.000000 nn4n-1.0.2/nn4n/structure/__init__.py
+-rw-r--r--   0 zhaoze     (501) staff       (20)     4068 2023-07-30 03:40:50.000000 nn4n-1.0.2/nn4n/structure/base_struct.py
+-rw-r--r--   0 zhaoze     (501) staff       (20)     6415 2023-07-30 03:20:15.000000 nn4n-1.0.2/nn4n/structure/multi_area.py
+-rw-r--r--   0 zhaoze     (501) staff       (20)     4256 2023-07-27 19:12:25.000000 nn4n-1.0.2/nn4n/structure/multi_area_ei.py
+-rw-r--r--   0 zhaoze     (501) staff       (20)     4050 2023-07-27 18:19:31.000000 nn4n-1.0.2/nn4n/structure/random_input.py
+-rw-r--r--   0 zhaoze     (501) staff       (20)     1901 2023-07-30 04:00:06.000000 nn4n-1.0.2/nn4n/utils.py
+drwxr-xr-x   0 zhaoze     (501) staff       (20)        0 2023-07-30 05:19:43.042191 nn4n-1.0.2/nn4n.egg-info/
+-rw-r--r--   0 zhaoze     (501) staff       (20)     4957 2023-07-30 05:19:43.000000 nn4n-1.0.2/nn4n.egg-info/PKG-INFO
+-rw-r--r--   0 zhaoze     (501) staff       (20)      633 2023-07-30 05:19:43.000000 nn4n-1.0.2/nn4n.egg-info/SOURCES.txt
+-rw-r--r--   0 zhaoze     (501) staff       (20)        1 2023-07-30 05:19:43.000000 nn4n-1.0.2/nn4n.egg-info/dependency_links.txt
+-rw-r--r--   0 zhaoze     (501) staff       (20)       37 2023-07-30 05:19:43.000000 nn4n-1.0.2/nn4n.egg-info/requires.txt
+-rw-r--r--   0 zhaoze     (501) staff       (20)        5 2023-07-30 05:19:43.000000 nn4n-1.0.2/nn4n.egg-info/top_level.txt
+-rw-r--r--   0 zhaoze     (501) staff       (20)       38 2023-07-30 05:19:43.045488 nn4n-1.0.2/setup.cfg
+-rw-r--r--   0 zhaoze     (501) staff       (20)      622 2023-07-30 05:19:41.000000 nn4n-1.0.2/setup.py
+drwxr-xr-x   0 zhaoze     (501) staff       (20)        0 2023-07-30 05:19:43.045071 nn4n-1.0.2/test/
+-rw-r--r--   0 zhaoze     (501) staff       (20)     2014 2023-07-27 19:59:06.000000 nn4n-1.0.2/test/test_dep.py
+-rw-r--r--   0 zhaoze     (501) staff       (20)     7599 2023-07-27 20:20:19.000000 nn4n-1.0.2/test/test_main.py
+-rw-r--r--   0 zhaoze     (501) staff       (20)     2246 2023-07-30 04:05:55.000000 nn4n-1.0.2/test/test_utils.py
```

### Comparing `nn4n-1.0.1/LICENSE` & `nn4n-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nn4n-1.0.1/PKG-INFO` & `nn4n-1.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: nn4n
-Version: 1.0.1
+Version: 1.0.2
 Summary: Neural Networks for Neuroscience Research
 Author: Zhaoze Wang
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # NN4N: Neural Networks for Neuroscience
 [![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI version](https://badge.fury.io/py/nn4n.svg)](https://badge.fury.io/py/nn4n)
 [![Python Package using Conda](https://github.com/zhaozewang/NN4Neurosci/actions/workflows/python-package-conda.yml/badge.svg)](https://github.com/zhaozewang/NN4Neurosci/actions/workflows/python-package-conda.yml)<br>
 Some of the most commonly used neural networks in neuroscience research are included in this project to ease the implementation process.
 
-<p align="center"><img src="./docs/images/basics/RNN_structure.png" width="400"></p>
+<p align="center"><img src="https://github.com/zhaozewang/NN4Neurosci/blob/main/docs/images/basics/RNN_structure.png" width="400"></p>
+
+[GitHub](https://github.com/zhaozewang/NN4Neurosci.git)
 
 ## Table of contents
 - [Install](#install)
     - [Install From GitHub](#install-from-github)
 - [Model](#model)
     - [CTRNN (Continuous-Time RNN)](#ctrnn)
 - [Structure](#structure)
@@ -49,42 +51,43 @@
 ```
 
 
 ## Model
 ### CTRNN
 The implementation of standard continuous-time RNN (CTRNN). This implementation supports enforcing sparsity constraint (i.e. preventing new synapses from being created) and E/I constraints (i.e. enforcing Dale's law). </br>
 
-- [Documentation](./docs/model/CTRNN/index.md)
-- [Examples](./examples/CTRNN.ipynb)
+- [Documentation](https://github.com/zhaozewang/NN4Neurosci/blob/main/docs/model/CTRNN/index.md)
+- [Examples](https://github.com/zhaozewang/NN4Neurosci/blob/main/examples/CTRNN.ipynb)
 
 ## Structure
 The detailed structure (e.g. whether its modular or hierarchical etc.) of any standard 3-layer RNN (as shown in figure above) can be specified using masks in our `model` module implementation. Easy implementations of a few RNN structures is included in the `structure` module.
-- [Documentation](./docs/structure/index.md)
+- [Documentation](https://github.com/zhaozewang/NN4Neurosci/blob/main/docs/structure/index.md)
 
 ### Multi-Area
 The HiddenLayer of a RNN is often defined using a connectivity matrix, depicting a somewhat 'random' connectivity between neurons. The connectivity matrix is often designed to imitate the connectivity of a certain brain area or a few brain areas. When modeling a single brain area, the connectivity matrix is often a fully connected matrix. </br>
 However, to model multiple brain areas, it would be more reasonable to use a connectivity matrix with multiple areas. In each areas is densely connected within itself and sparsely connected between areas. The `MultiArea` class in the `structure` module is designed to implement such a connectivity matrix. </br>
 
-- [Examples](./examples/MultiArea.ipynb)
+- [Examples](https://github.com/zhaozewang/NN4Neurosci/blob/main/examples/MultiArea.ipynb)
 
 ### Multi-Area with E/I constraints
 On top of modeling brain with multi-area hidden layer, another critical constraint would be the Dale's law, as proposed in the paper [Training Excitatory-Inhibitory Recurrent Neural Networks for Cognitive Tasks: A Simple and Flexible Framework](https://doi.org/10.1371/journal.pcbi.1004792) by Song et al. 2016. The `MultiAreaEI` class in the `structure` module is designed to implement such a connectivity matrix. </br>
 This class allows for a much easier implementation of the E/I constraints particularly when there are multiple areas in the hidden layer. It provides flexible control over the excitatory-excitatory, excitatory-inhibitory, inhibitory-excitatory, and inhibitory-inhibitory connections on top of the basic `MultiArea` features. </br>
 
-- [Examples](./examples/MultiArea.ipynb)
+- [Examples](https://github.com/zhaozewang/NN4Neurosci/blob/main/examples/MultiArea.ipynb)
 
 ### Random Input
 Neurons's dynamic receiving input will be heavily driven by the inputting signal. Injecting signal to only part of the neuron will result in more versatile and hierarchical dynamics. See [A Versatile Hub Model For Efficient Information Propagation And Feature Selection](https://arxiv.org/abs/2307.02398) <br>
 
 - Example to be added
 
 ## Criterion
 ### RNNLoss
-The loss function is modularized. Each criterion is designed in the format of $`\lambda_L L(\cdot)`$. By default, all $`\lambda_{L}`$ are set to 0 and won't be added to loss (nor the auto-grad tree). By changing the corresponding $`\lambda_{L}`$ to non-zero positive values, the corresponding loss function will be added to the total loss. The total loss is the sum of all loss functions with non-zero $`\lambda_{L}`$.
-- [Documentation](./docs/criterion/index.md)
+The loss function is modularized. The `RNNLoss` class is designed in modular fashion and included the most commonly used loss functions in neuroscience research. </br>
+
+- [Documentation](https://github.com/zhaozewang/NN4Neurosci/blob/main/docs/criterion/index.md)
 
 ## Others
 For similar projects:
 - [nn-brain](https://github.com/gyyang/nn-brain)
 
 ## Acknowledgements
 Immense thanks to Christopher J. Cueva for his mentorship in developing this project. This project can't be done without his invaluable help.
```

### Comparing `nn4n-1.0.1/README.md` & `nn4n-1.0.2/nn4n.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,26 @@
+Metadata-Version: 2.1
+Name: nn4n
+Version: 1.0.2
+Summary: Neural Networks for Neuroscience Research
+Author: Zhaoze Wang
+License: MIT
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # NN4N: Neural Networks for Neuroscience
 [![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI version](https://badge.fury.io/py/nn4n.svg)](https://badge.fury.io/py/nn4n)
 [![Python Package using Conda](https://github.com/zhaozewang/NN4Neurosci/actions/workflows/python-package-conda.yml/badge.svg)](https://github.com/zhaozewang/NN4Neurosci/actions/workflows/python-package-conda.yml)<br>
 Some of the most commonly used neural networks in neuroscience research are included in this project to ease the implementation process.
 
-<p align="center"><img src="./docs/images/basics/RNN_structure.png" width="400"></p>
+<p align="center"><img src="https://github.com/zhaozewang/NN4Neurosci/blob/main/docs/images/basics/RNN_structure.png" width="400"></p>
+
+[GitHub](https://github.com/zhaozewang/NN4Neurosci.git)
 
 ## Table of contents
 - [Install](#install)
     - [Install From GitHub](#install-from-github)
 - [Model](#model)
     - [CTRNN (Continuous-Time RNN)](#ctrnn)
 - [Structure](#structure)
@@ -39,42 +51,43 @@
 ```
 
 
 ## Model
 ### CTRNN
 The implementation of standard continuous-time RNN (CTRNN). This implementation supports enforcing sparsity constraint (i.e. preventing new synapses from being created) and E/I constraints (i.e. enforcing Dale's law). </br>
 
-- [Documentation](./docs/model/CTRNN/index.md)
-- [Examples](./examples/CTRNN.ipynb)
+- [Documentation](https://github.com/zhaozewang/NN4Neurosci/blob/main/docs/model/CTRNN/index.md)
+- [Examples](https://github.com/zhaozewang/NN4Neurosci/blob/main/examples/CTRNN.ipynb)
 
 ## Structure
 The detailed structure (e.g. whether its modular or hierarchical etc.) of any standard 3-layer RNN (as shown in figure above) can be specified using masks in our `model` module implementation. Easy implementations of a few RNN structures is included in the `structure` module.
-- [Documentation](./docs/structure/index.md)
+- [Documentation](https://github.com/zhaozewang/NN4Neurosci/blob/main/docs/structure/index.md)
 
 ### Multi-Area
 The HiddenLayer of a RNN is often defined using a connectivity matrix, depicting a somewhat 'random' connectivity between neurons. The connectivity matrix is often designed to imitate the connectivity of a certain brain area or a few brain areas. When modeling a single brain area, the connectivity matrix is often a fully connected matrix. </br>
 However, to model multiple brain areas, it would be more reasonable to use a connectivity matrix with multiple areas. In each areas is densely connected within itself and sparsely connected between areas. The `MultiArea` class in the `structure` module is designed to implement such a connectivity matrix. </br>
 
-- [Examples](./examples/MultiArea.ipynb)
+- [Examples](https://github.com/zhaozewang/NN4Neurosci/blob/main/examples/MultiArea.ipynb)
 
 ### Multi-Area with E/I constraints
 On top of modeling brain with multi-area hidden layer, another critical constraint would be the Dale's law, as proposed in the paper [Training Excitatory-Inhibitory Recurrent Neural Networks for Cognitive Tasks: A Simple and Flexible Framework](https://doi.org/10.1371/journal.pcbi.1004792) by Song et al. 2016. The `MultiAreaEI` class in the `structure` module is designed to implement such a connectivity matrix. </br>
 This class allows for a much easier implementation of the E/I constraints particularly when there are multiple areas in the hidden layer. It provides flexible control over the excitatory-excitatory, excitatory-inhibitory, inhibitory-excitatory, and inhibitory-inhibitory connections on top of the basic `MultiArea` features. </br>
 
-- [Examples](./examples/MultiArea.ipynb)
+- [Examples](https://github.com/zhaozewang/NN4Neurosci/blob/main/examples/MultiArea.ipynb)
 
 ### Random Input
 Neurons's dynamic receiving input will be heavily driven by the inputting signal. Injecting signal to only part of the neuron will result in more versatile and hierarchical dynamics. See [A Versatile Hub Model For Efficient Information Propagation And Feature Selection](https://arxiv.org/abs/2307.02398) <br>
 
 - Example to be added
 
 ## Criterion
 ### RNNLoss
-The loss function is modularized. Each criterion is designed in the format of $`\lambda_L L(\cdot)`$. By default, all $`\lambda_{L}`$ are set to 0 and won't be added to loss (nor the auto-grad tree). By changing the corresponding $`\lambda_{L}`$ to non-zero positive values, the corresponding loss function will be added to the total loss. The total loss is the sum of all loss functions with non-zero $`\lambda_{L}`$.
-- [Documentation](./docs/criterion/index.md)
+The loss function is modularized. The `RNNLoss` class is designed in modular fashion and included the most commonly used loss functions in neuroscience research. </br>
+
+- [Documentation](https://github.com/zhaozewang/NN4Neurosci/blob/main/docs/criterion/index.md)
 
 ## Others
 For similar projects:
 - [nn-brain](https://github.com/gyyang/nn-brain)
 
 ## Acknowledgements
-Immense thanks to Christopher J. Cueva for his mentorship in developing this project. This project can't be done without his invaluable help.
+Immense thanks to Christopher J. Cueva for his mentorship in developing this project. This project can't be done without his invaluable help.
```

### Comparing `nn4n-1.0.1/nn4n/criterion/rnn_loss.py` & `nn4n-1.0.2/nn4n/criterion/rnn_loss.py`

 * *Files identical despite different names*

### Comparing `nn4n-1.0.1/nn4n/model/CTRNN/ctrnn.py` & `nn4n-1.0.2/nn4n/model/CTRNN/ctrnn.py`

 * *Files identical despite different names*

### Comparing `nn4n-1.0.1/nn4n/model/CTRNN/hidden_layer.py` & `nn4n-1.0.2/nn4n/model/CTRNN/hidden_layer.py`

 * *Files identical despite different names*

### Comparing `nn4n-1.0.1/nn4n/model/CTRNN/linear_layer.py` & `nn4n-1.0.2/nn4n/model/CTRNN/linear_layer.py`

 * *Files identical despite different names*

### Comparing `nn4n-1.0.1/nn4n/model/CTRNN/recurrent_layer.py` & `nn4n-1.0.2/nn4n/model/CTRNN/recurrent_layer.py`

 * *Files identical despite different names*

### Comparing `nn4n-1.0.1/nn4n/structure/base_struct.py` & `nn4n-1.0.2/nn4n/structure/base_struct.py`

 * *Files identical despite different names*

### Comparing `nn4n-1.0.1/nn4n/structure/multi_area.py` & `nn4n-1.0.2/nn4n/structure/multi_area.py`

 * *Files identical despite different names*

### Comparing `nn4n-1.0.1/nn4n/structure/multi_area_ei.py` & `nn4n-1.0.2/nn4n/structure/multi_area_ei.py`

 * *Files identical despite different names*

### Comparing `nn4n-1.0.1/nn4n/structure/random_input.py` & `nn4n-1.0.2/nn4n/structure/random_input.py`

 * *Files identical despite different names*

### Comparing `nn4n-1.0.1/nn4n/utils.py` & `nn4n-1.0.2/nn4n/utils.py`

 * *Files identical despite different names*

### Comparing `nn4n-1.0.1/nn4n.egg-info/PKG-INFO` & `nn4n-1.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,16 @@
-Metadata-Version: 2.1
-Name: nn4n
-Version: 1.0.1
-Summary: Neural Networks for Neuroscience Research
-Author: Zhaoze Wang
-License: MIT
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # NN4N: Neural Networks for Neuroscience
 [![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI version](https://badge.fury.io/py/nn4n.svg)](https://badge.fury.io/py/nn4n)
 [![Python Package using Conda](https://github.com/zhaozewang/NN4Neurosci/actions/workflows/python-package-conda.yml/badge.svg)](https://github.com/zhaozewang/NN4Neurosci/actions/workflows/python-package-conda.yml)<br>
 Some of the most commonly used neural networks in neuroscience research are included in this project to ease the implementation process.
 
-<p align="center"><img src="./docs/images/basics/RNN_structure.png" width="400"></p>
+<p align="center"><img src="https://github.com/zhaozewang/NN4Neurosci/blob/main/docs/images/basics/RNN_structure.png" width="400"></p>
+
+[GitHub](https://github.com/zhaozewang/NN4Neurosci.git)
 
 ## Table of contents
 - [Install](#install)
     - [Install From GitHub](#install-from-github)
 - [Model](#model)
     - [CTRNN (Continuous-Time RNN)](#ctrnn)
 - [Structure](#structure)
@@ -49,42 +41,43 @@
 ```
 
 
 ## Model
 ### CTRNN
 The implementation of standard continuous-time RNN (CTRNN). This implementation supports enforcing sparsity constraint (i.e. preventing new synapses from being created) and E/I constraints (i.e. enforcing Dale's law). </br>
 
-- [Documentation](./docs/model/CTRNN/index.md)
-- [Examples](./examples/CTRNN.ipynb)
+- [Documentation](https://github.com/zhaozewang/NN4Neurosci/blob/main/docs/model/CTRNN/index.md)
+- [Examples](https://github.com/zhaozewang/NN4Neurosci/blob/main/examples/CTRNN.ipynb)
 
 ## Structure
 The detailed structure (e.g. whether its modular or hierarchical etc.) of any standard 3-layer RNN (as shown in figure above) can be specified using masks in our `model` module implementation. Easy implementations of a few RNN structures is included in the `structure` module.
-- [Documentation](./docs/structure/index.md)
+- [Documentation](https://github.com/zhaozewang/NN4Neurosci/blob/main/docs/structure/index.md)
 
 ### Multi-Area
 The HiddenLayer of a RNN is often defined using a connectivity matrix, depicting a somewhat 'random' connectivity between neurons. The connectivity matrix is often designed to imitate the connectivity of a certain brain area or a few brain areas. When modeling a single brain area, the connectivity matrix is often a fully connected matrix. </br>
 However, to model multiple brain areas, it would be more reasonable to use a connectivity matrix with multiple areas. In each areas is densely connected within itself and sparsely connected between areas. The `MultiArea` class in the `structure` module is designed to implement such a connectivity matrix. </br>
 
-- [Examples](./examples/MultiArea.ipynb)
+- [Examples](https://github.com/zhaozewang/NN4Neurosci/blob/main/examples/MultiArea.ipynb)
 
 ### Multi-Area with E/I constraints
 On top of modeling brain with multi-area hidden layer, another critical constraint would be the Dale's law, as proposed in the paper [Training Excitatory-Inhibitory Recurrent Neural Networks for Cognitive Tasks: A Simple and Flexible Framework](https://doi.org/10.1371/journal.pcbi.1004792) by Song et al. 2016. The `MultiAreaEI` class in the `structure` module is designed to implement such a connectivity matrix. </br>
 This class allows for a much easier implementation of the E/I constraints particularly when there are multiple areas in the hidden layer. It provides flexible control over the excitatory-excitatory, excitatory-inhibitory, inhibitory-excitatory, and inhibitory-inhibitory connections on top of the basic `MultiArea` features. </br>
 
-- [Examples](./examples/MultiArea.ipynb)
+- [Examples](https://github.com/zhaozewang/NN4Neurosci/blob/main/examples/MultiArea.ipynb)
 
 ### Random Input
 Neurons's dynamic receiving input will be heavily driven by the inputting signal. Injecting signal to only part of the neuron will result in more versatile and hierarchical dynamics. See [A Versatile Hub Model For Efficient Information Propagation And Feature Selection](https://arxiv.org/abs/2307.02398) <br>
 
 - Example to be added
 
 ## Criterion
 ### RNNLoss
-The loss function is modularized. Each criterion is designed in the format of $`\lambda_L L(\cdot)`$. By default, all $`\lambda_{L}`$ are set to 0 and won't be added to loss (nor the auto-grad tree). By changing the corresponding $`\lambda_{L}`$ to non-zero positive values, the corresponding loss function will be added to the total loss. The total loss is the sum of all loss functions with non-zero $`\lambda_{L}`$.
-- [Documentation](./docs/criterion/index.md)
+The loss function is modularized. The `RNNLoss` class is designed in modular fashion and included the most commonly used loss functions in neuroscience research. </br>
+
+- [Documentation](https://github.com/zhaozewang/NN4Neurosci/blob/main/docs/criterion/index.md)
 
 ## Others
 For similar projects:
 - [nn-brain](https://github.com/gyyang/nn-brain)
 
 ## Acknowledgements
-Immense thanks to Christopher J. Cueva for his mentorship in developing this project. This project can't be done without his invaluable help.
+Immense thanks to Christopher J. Cueva for his mentorship in developing this project. This project can't be done without his invaluable help.
```

### Comparing `nn4n-1.0.1/nn4n.egg-info/SOURCES.txt` & `nn4n-1.0.2/nn4n.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nn4n-1.0.1/setup.py` & `nn4n-1.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='nn4n',
-    version='1.0.1',
+    version='1.0.2',
     description='Neural Networks for Neuroscience Research',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Zhaoze Wang',
     license='MIT',
 
     packages=find_packages(),
```

### Comparing `nn4n-1.0.1/test/test_dep.py` & `nn4n-1.0.2/test/test_dep.py`

 * *Files identical despite different names*

### Comparing `nn4n-1.0.1/test/test_main.py` & `nn4n-1.0.2/test/test_main.py`

 * *Files identical despite different names*

### Comparing `nn4n-1.0.1/test/test_utils.py` & `nn4n-1.0.2/test/test_utils.py`

 * *Files identical despite different names*

