# Comparing `tmp/linfa_vi-1.1.6.tar.gz` & `tmp/linfa_vi-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linfa_vi-1.1.6.tar", last modified: Sat Jul 15 04:38:43 2023, max compression
+gzip compressed data, was "linfa_vi-1.1.7.tar", last modified: Sat Jul 29 22:48:44 2023, max compression
```

## Comparing `linfa_vi-1.1.6.tar` & `linfa_vi-1.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 04:38:43.251541 linfa_vi-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-15 04:38:28.000000 linfa_vi-1.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-07-15 04:38:43.251541 linfa_vi-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-07-15 04:38:28.000000 linfa_vi-1.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 04:38:43.251541 linfa_vi-1.1.6/linfa/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-15 04:38:28.000000 linfa_vi-1.1.6/linfa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-07-15 04:38:28.000000 linfa_vi-1.1.6/linfa/maf.py
--rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-07-15 04:38:28.000000 linfa_vi-1.1.6/linfa/nofas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-07-15 04:38:28.000000 linfa_vi-1.1.6/linfa/plot_res.py
--rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-07-15 04:38:28.000000 linfa_vi-1.1.6/linfa/run_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-15 04:38:28.000000 linfa_vi-1.1.6/linfa/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 04:38:43.251541 linfa_vi-1.1.6/linfa_vi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-07-15 04:38:43.000000 linfa_vi-1.1.6/linfa_vi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-15 04:38:43.000000 linfa_vi-1.1.6/linfa_vi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 04:38:43.000000 linfa_vi-1.1.6/linfa_vi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-15 04:38:43.000000 linfa_vi-1.1.6/linfa_vi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-15 04:38:43.000000 linfa_vi-1.1.6/linfa_vi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-15 04:38:28.000000 linfa_vi-1.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 04:38:43.251541 linfa_vi-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 04:38:28.000000 linfa_vi-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:48:44.491121 linfa_vi-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-29 22:48:33.000000 linfa_vi-1.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-07-29 22:48:44.491121 linfa_vi-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-07-29 22:48:33.000000 linfa_vi-1.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:48:44.487121 linfa_vi-1.1.7/linfa/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-29 22:48:33.000000 linfa_vi-1.1.7/linfa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-07-29 22:48:33.000000 linfa_vi-1.1.7/linfa/maf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17362 2023-07-29 22:48:33.000000 linfa_vi-1.1.7/linfa/nofas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-07-29 22:48:33.000000 linfa_vi-1.1.7/linfa/plot_res.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-07-29 22:48:33.000000 linfa_vi-1.1.7/linfa/run_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-29 22:48:33.000000 linfa_vi-1.1.7/linfa/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 22:48:44.491121 linfa_vi-1.1.7/linfa_vi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-07-29 22:48:44.000000 linfa_vi-1.1.7/linfa_vi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-29 22:48:44.000000 linfa_vi-1.1.7/linfa_vi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 22:48:44.000000 linfa_vi-1.1.7/linfa_vi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-29 22:48:44.000000 linfa_vi-1.1.7/linfa_vi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 22:48:44.000000 linfa_vi-1.1.7/linfa_vi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-29 22:48:33.000000 linfa_vi-1.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 22:48:44.491121 linfa_vi-1.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 22:48:33.000000 linfa_vi-1.1.7/setup.py
```

### Comparing `linfa_vi-1.1.6/LICENSE` & `linfa_vi-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.6/PKG-INFO` & `linfa_vi-1.1.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linfa_vi
-Version: 1.1.6
+Version: 1.1.7
 Summary: A Python library for inference with normalizing flow and annealing
 Author-email: resDesLab  <daniele.schiavazzi@gmail.com>
 License: Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -114,15 +114,14 @@
 
 A step by step [tutorial](tutorial/TutorialwithPhys.ipynb) is also available which will guide you through the an inference problem for a ballistic simulation. 
 
 ### Citation
 
 Did you use LINFA? Please cite our paper using:
 ```
-@misc{TO BE FINALIZED!!!,
-      title={LINFA: a Python library for variational inference with normalizing flow and annealing}, 
-      author={Yu Wang, Emma R. Cobian, Fang Liu, Jonathan D. Hauenstein, Daniele E. Schiavazzi},
-      year={2022},
-      eprint={2201.03715},
-      archivePrefix={arXiv},
-      primaryClass={eess.IV}
+@article{linfa-vi-paper,
+  title={LINFA: a Python library for variational inference with normalizing flow and annealing},
+  author={Wang, Yu and Cobian, Emma R and Lee, Jubilee and Liu, Fang and Hauenstein, Jonathan D and Schiavazzi, Daniele E},
+  journal={arXiv preprint arXiv:2307.04675},
+  year={2023}
 }
+```
```

### Comparing `linfa_vi-1.1.6/README.md` & `linfa_vi-1.1.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -92,15 +92,14 @@
 
 A step by step [tutorial](tutorial/TutorialwithPhys.ipynb) is also available which will guide you through the an inference problem for a ballistic simulation. 
 
 ### Citation
 
 Did you use LINFA? Please cite our paper using:
 ```
-@misc{TO BE FINALIZED!!!,
-      title={LINFA: a Python library for variational inference with normalizing flow and annealing}, 
-      author={Yu Wang, Emma R. Cobian, Fang Liu, Jonathan D. Hauenstein, Daniele E. Schiavazzi},
-      year={2022},
-      eprint={2201.03715},
-      archivePrefix={arXiv},
-      primaryClass={eess.IV}
-}
+@article{linfa-vi-paper,
+  title={LINFA: a Python library for variational inference with normalizing flow and annealing},
+  author={Wang, Yu and Cobian, Emma R and Lee, Jubilee and Liu, Fang and Hauenstein, Jonathan D and Schiavazzi, Daniele E},
+  journal={arXiv preprint arXiv:2307.04675},
+  year={2023}
+}
+```
```

### Comparing `linfa_vi-1.1.6/linfa/maf.py` & `linfa_vi-1.1.7/linfa/maf.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.6/linfa/nofas.py` & `linfa_vi-1.1.7/linfa/run_experiment.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,340 +1,265 @@
+import os
 import torch
-import torch.nn as nn
-import torch.nn.functional as F
 import numpy as np
-from os import path
+from linfa.maf import MAF, RealNVP
 
 torch.set_default_tensor_type(torch.DoubleTensor)
 
-class FNN(nn.Module):
-    """Fully Connected Neural Network"""
-
-    def __init__(self, input_size, output_size, device):
-        """
-        Args:
-            input_size (int): Input size for FNN
-            output_size (int): Output size for FNN
-        """
-        super().__init__()
-        self.fc1 = nn.Linear(input_size, 64).to(device)
-        self.fc2 = nn.Linear(64, 32).to(device)
-        self.fc3 = nn.Linear(32, output_size).to(device)
-
-    def forward(self, x):
-        """
-        Args:
-            x (torch.Tensor): [num_samples, input_size], assumed to be a batch.
-
-        Returns:
-            torch.Tensor. Assumed to be a batch.
-        """
-        x = F.relu(self.fc1(x))
-        x = F.relu(self.fc2(x))
-        # x = F.relu(self.fc3(x))
-        x = self.fc3(x)
-        return x
-
-
-class Surrogate:
-    """Class to create surrogate models for inference with NoFAS
-
-       Args:
-            model_name (string): name of the true model to be approximated
-            model_func (function): with only one input of torch.Tensor
-            input_size (int): input dimension of true model.
-            output_size (int): output dimension of true model.
-            limits (list or lists): bounds for all inputs, in format of [[low_0, high_0], [low_1, high_1], ... ]
-            memory_len (int): the maximal number of batches stored in buffer. Default: 20
-            surrogate (None or torch.nn.Module): the implementation of surrogate model used. Default: FNN
+class experiment:
+    """Defines an instance of variational inference
 
+    This class is the core class of the LINFA library
+    and defines all the default hyperparameter values and 
+    and functions used for inference. 
     """
-    def __init__(self, model_name, model_func, input_size, output_size, model_folder='./', limits=None, memory_len=20, surrogate=None, device='cpu'):
-        self.device = device
-        self.input_size = input_size
-        self.output_size = output_size
-        self.model_name = model_name
-        self.model_folder = model_folder
-        self.mf = model_func
-        self.pre_out = None
-        self.m = None
-        self.sd = None
-        self.tm = None
-        self.tsd = None
-        self.limits = limits
-        self.pre_grid = None
-        self.surrogate = FNN(input_size, output_size, self.device) if surrogate is None else surrogate
-        self.beta_0 = 0.5
-        self.beta_1 = 0.1        
-
-        self.memory_grid = []
-        self.memory_out = []
-        self.memory_len = memory_len
-        self.weights = torch.Tensor([np.exp(-self.beta_1 * i) for i in range(memory_len)]).to(self.device)
-        self.grid_record = None
-        
-
-    @property
-    def limits(self):
-        """Retrieves the limits of all inputs
-        """
-        return self.__limits
-
-    @limits.setter
-    def limits(self, limits):
-        """Sets the limits of all inputs
-        
-        Args:
-            limits (list or tuple): Lists lower and upper bound in the format *[[low_0, high_0], [low_1, high_1], ...]*
-
-        """
-        limits = torch.Tensor(limits).tolist()
-        if len(limits) != self.input_size:
-            print("Error: Invalid input size for limit. Abort.")
-            exit(-1)
-        elif any(len(item) != 2 for item in limits):
-            print("Error: Limits should be two bounds. Abort.")
-            exit(-1)
-        elif any(item[0] > item[1] for item in limits):
-            print("Error: Upper bound should not be smaller than lower bound. Abort.")
-            exit(-1)
-        self.__limits = limits
+    def __init__(self):
 
-    @property
-    def pre_grid(self):
-        return self.__pre_grid
+        # NF ARCHITECTURE parameters
+        self.name              = "Experiment"
+        self.input_size        = 3             #:int:  Number of input parameters
+        self.flow_type         = 'maf'         #:str:  Type of flow ('maf' or 'realnvp')
+        self.n_blocks          = 15            #:int:  Number of layers
+        self.hidden_size       = 100           #:int:  Hidden layer size for MADE in each layer
+        self.n_hidden          = 1             #:int:  Number of hidden layers in each MADE
+        self.activation_fn     = 'relu'        #:str:  Actication function used (either 'relu','tanh' or 'sigmoid')
+        self.input_order       = 'sequential'  #:str:  Input order for create_mask (either 'sequential' or 'random')
+        self.batch_norm_order  = True          #:bool: Uses decide if batch_norm is used
+
+        # NOFAS parameters
+        self.run_nofas          = True  #:bool:   Activate NoFAS and the use of a surrogate model
+        self.log_interval       = 10    #:int:    How often the loss statistics are printed
+        self.calibrate_interval = 300   #:int:    How often the surrogate model is updated
+        self.true_data_num      = 2     #:double: Number of true model evaluated at each surrogate update
+        self.budget             = 216   #:int:    Maximum number of allowed evaluations of the true model
+        self.surr_pre_it        = 40000 #:int:    Number of pre-training iterations for surrogate model
+        self.surr_upd_it        = 6000  #:int:    Number of iterations for the surrogate model update
+        self.surr_folder        = "./"  #:str:    Folder where the surrogate model is stored
+        self.use_new_surr       = True #:bool:   Start by pre-training a new surrogate and ignore existing surrogates
+
+        # OPTIMIZER parameters
+        self.optimizer    = 'Adam'   #:str:    Type of optimizer used (either 'Adam' or 'RMSprop')
+        self.lr           = 0.003    #:double: Learning rate
+        self.lr_decay     = 0.9999   #:double: Learning rate decay
+        self.lr_scheduler = 'StepLR' #:str:    type of lr scheduler used (either 'StepLR' or 'ExponentialLR')
+        self.lr_step      = 1000     #:int:    Number of steps for StepLR learning rate scheduler 
+        self.batch_size   = 500      #:int:    Number of batch samples generated at every iteration from the base distribution        
+        self.n_iter       = 25001    #:int:    Total number of iterations
+
+        # ANNEALING parameters
+        self.annealing    = True     #:bool:   Flag to activate an annealing scheduler
+        self.scheduler    = 'AdaAnn' #:str:    Type of annealing scheduler (either 'AdaAnn' or 'Linear')
+        # AdaAnn
+        self.tol          = 0.001    #:double: KL tolerance for AdaAnn scheduler
+        self.t0           = 0.01     #:double: Initial value for the inverse temperature
+        self.N            = 100      #:int:    Number of batch samples generated for $t<1$ at each iteration
+        self.N_1          = 1000     #:int:    number of batch samples generated for $t=1$ at each iteration
+        self.T_0          = 500      #:int:    Number of parameter updates at the initial inverse temperature $t_0$
+        self.T            = 5        #:int:    Number of parameter updates for each temperature for $t<1$
+        self.T_1          = 5001     #:int:    Number of parameter updates at $t=1$
+        self.M            = 1000     #:int:    Number of Monte Carlo  samples use to compute the denominator of the AdaAnn formula        
+        # Linear scheduler
+        self.linear_step  = 0.0001   #:double: Fixed step size for the Linear annealing scheduler
+
+        # OUTPUT parameters
+        self.output_dir          = './results/' + self.name #:str: Name of the output folder
+        self.log_file            = 'log.txt'                #:str: File name where the log profile stats are written
+        self.seed                = 35435                    #:int: Random seed
+        self.n_sample            = 5000                     #:int: Number of batch samples used to print results at save_interval
+        self.save_interval       = 200                      #:int: Save interval for all results
+        self.store_nf_interval   = 1000                     #:int: Save interval for normalizing flow parameters
+        self.store_surr_interval = None                     #:int: Save interval for surrogate model (None for no save)
+
+        # DEVICE parameters
+        self.no_cuda = True #:bool: Flag to use CPU
+
+        # Set device
+        self.device = torch.device('cuda:0' if torch.cuda.is_available() and not self.no_cuda else 'cpu')
+
+        # Local pointer to the main components for inference
+        self.transform        = None
+        self.model            = None
+        self.model_logdensity = None
+        self.surrogate        = None
+
+    def run(self):
+        """Runs instance of inference inference problem        
+
+        """
+
+        # Check is surrogate exists
+        if self.run_nofas:
+            if not os.path.exists(self.name + ".sur") or not os.path.exists(self.name + ".npz"):
+                print("Abort: NoFAS enabled, without surrogate files. \nPlease include the following surrogate files in root directory.\n{}.sur and {}.npz".format(self.name, self.name))
+                exit(0)
+        # setup file ops
+        if not os.path.isdir(self.output_dir):
+            os.makedirs(self.output_dir)
+
+        # Save a copy of the data in the result folder so it is handy
+        if hasattr(self.model,'data'):
+          np.savetxt(self.output_dir + '/' + self.name + '_data', self.model.data, newline="\n")
+
+        # setup device
+        torch.manual_seed(self.seed)
+        if self.device.type == 'cuda': torch.cuda.manual_seed(self.seed)
 
-    @pre_grid.setter
-    def pre_grid(self, pre_grid):
-        """Assign the pregrid for the surrogate model. 
-
-        f nofas is not enabled, this serves as the whole training grid.
-        
-        Args:
-            pre_grid (None or torch.Tensor): Specifies a matrix of model inputs with size [data_num, feature_dim]. If None, will try to search for *npz* containing this info.
-
-        Returns:
-            None
+        print('')
+        print('--- Running on device: '+ str(self.device))
+        print('')
 
-        """
-        if pre_grid is None:
-            if path.exists(self.model_folder + self.model_name + '.npz'):
-                container = np.load(self.model_folder + self.model_name + '.npz')
-                if 'pre_grid' in container:
-                    self.pre_grid = container['pre_grid']
-                    print("Success: Pre-Grid found.")
-            else:
-                print("Warning: " + self.model_folder + self.model_name + ".npz does not found, please generate pre-grid.")
-                print("Suggestion: Use Surrogate.gen_grid(input_limits=None, grid_num=5, store=True)")
+        # model
+        if self.flow_type == 'maf':
+            nf = MAF(self.n_blocks, self.input_size, self.hidden_size, self.n_hidden, None,
+                     self.activation_fn, self.input_order, batch_norm=self.batch_norm_order)
+        elif self.flow_type == 'realnvp':  # Under construction
+            nf = RealNVP(self.n_blocks, self.input_size, self.hidden_size, self.n_hidden, None,
+                         batch_norm=self.batch_norm_order)
         else:
-            self.__pre_grid = torch.Tensor(pre_grid).to(self.device)
-            self.m = torch.mean(self.pre_grid, 0)
-            self.sd = torch.std(self.pre_grid, 0)
-            # Evaluate model at pre-grid
-            self.pre_out = self.mf(self.pre_grid)
-            self.tm = torch.mean(self.pre_out, 0)
-            self.tsd = torch.std(self.pre_out, 0)
-            self.grid_record = self.__pre_grid.clone()
+            raise ValueError('Unrecognized model.')
 
-    def gen_grid(self, input_limits=None, grid_type='tensor', gridnum=4, store=True):
-        """Generates a pre-grid.
-        
-        Args:
-            input_limits (None or list[list]): If None, use self.limits. If list[list], rewrite self.limits and use it.
-            gridnum (int): Contains the number of grid points per dimension.
-            store (bool): Flag indicating the pre-grid is store in self.pre_grid. If False then self.pre_grid is None.
-
-        Returns:
-            torch.Tensor: Input values for the full tensor grid in *dim* dimensions stored in a matrix [gridnum ** dim, dim].
-        """
-        if (grid_type == 'tensor'):
-          
-            meshpoints = []
-            if input_limits is not None:
-                self.limits = input_limits
-                print("Warning: Input limits recorded in surrogate.")
-
-            for lim in self.limits: meshpoints.append(torch.linspace(lim[0], lim[1], steps=gridnum))
-            grid = torch.meshgrid(meshpoints,indexing='ij')
-            grid = torch.cat([item.reshape(gridnum ** len(self.limits), 1) for item in grid], 1)
-
-        elif (grid_type == 'sobol'):
-
-            # Generate sobol samples in [0,1]^d
-            soboleng = torch.quasirandom.SobolEngine(dimension=len(self.limits))
-            grid = soboleng.draw(gridnum)
-            for i,lim in enumerate(self.limits): 
-                grid[:,i] = lim[0] + (lim[1] - lim[0]) * grid[:,i]
+        nf = nf.to(self.device)
+        if self.optimizer == 'Adam':
+            optimizer = torch.optim.Adam(nf.parameters(), lr=self.lr)
+        elif self.optimizer == 'RMSprop':
+            optimizer = torch.optim.RMSprop(nf.parameters(), lr=self.lr)
+        else:
+            raise ValueError('Unrecognized optimizer.')
 
+        if self.lr_scheduler == 'StepLR':
+            scheduler = torch.optim.lr_scheduler.StepLR(optimizer, self.lr_step, self.lr_decay)
+        elif self.lr_scheduler == 'ExponentialLR':
+            scheduler = torch.optim.lr_scheduler.ExponentialLR(optimizer, self.lr_decay)
         else:
+            raise ValueError('Unrecognized learning rate scheduler.')
 
-            print('Invalid type for pre-grid generation')
-            exit(-1)
+        if self.annealing:
+            i = 1
+            prev_i = 1
+            tvals = []
+            t = self.t0
+            dt = 0.0
+            loglist = []
+            while t < 1:
+                t = min(1, t + dt)
+                tvals = np.concatenate([tvals, np.array([t])])
+                self.n_iter = self.T
+                self.batch_size = self.N
+                
+                if t == self.t0:
+                    self.n_iter = self.T_0
+                if t == 1:
+                    self.batch_size = self.N_1
+                    self.n_iter = self.T_1
+
+                while i < prev_i + self.n_iter:
+                    self.train(nf, optimizer, i, loglist, sampling=True, t=t)
+                    if t == 1:
+                        scheduler.step()
+                    i += 1
+                prev_i = i
+
+                if self.scheduler == 'AdaAnn':
+                    z0 = nf.base_dist.sample([self.M])
+                    zk, _ = nf(z0)
+                    log_qk = self.model_logdensity(zk)
+                    dt = self.tol / torch.sqrt(log_qk.var())
+                    dt = dt.detach()# .numpy()
 
-        # Store pre-grid
-        if store:
-            self.pre_grid = grid
-            self.grid_record = self.pre_grid.clone()
-            self.surrogate_save()
-        
-        # Return grid
-        return grid
+                if self.scheduler == 'Linear':
+                    dt = self.linear_step
+        else:
+            loglist = []
+            for i in range(1, self.n_iter+1):                
+                self.train(nf, optimizer, i, loglist, sampling=True)
+                scheduler.step()
 
-    def surrogate_save(self):
-        """Save surrogate model to [self.name].sur and [self.name].npz
-        
-        Returns:
-            None
+        print('')
+        print('--- Simulation completed!')        
 
-        """
-        torch.save(self.surrogate.state_dict(), self.model_folder + self.model_name + '.sur')
-        np.savez(self.model_folder + self.model_name, limits=self.limits, pre_grid=self.pre_grid.clone().cpu().numpy(),
-                 grid_record=self.grid_record.clone().cpu().numpy())
+    def train(self, nf, optimizer, iteration, log, sampling=True, t=1):
+        """Parameter update for normalizing flow and surrogate model
 
-    def surrogate_load(self):
-        """Load surrogate model from [self.name].sur and [self.name].npz
+        This is the function where the ELBO loss function is evaluated, 
+        the results are saved and the surrogate model is updated.
         
-        Returns:
-            None
-        """
-        self.surrogate.load_state_dict(torch.load(self.model_folder + self.model_name + '.sur'))
-        container = np.load(self.model_folder + self.model_name + '.npz')
-        for key in container:
-            try:
-                setattr(self, key, torch.Tensor(container[key]))
-                print("Success: [" + key + "] loaded.")
-            except:
-                print("Warning: [" + key + "] is not a surrogate variables.")
-
-    def pre_train(self, max_iters, lr, lr_exp, record_interval, store=True, reg=False):
-        """Train surrogate model with pre-grid.
-
-         Training is performed with the RMSprop optimizer and with an exponential learning rate scheduler.
-
         Args:
-            max_iters (int): The maximal number of iterations.
-            lr (double): Learning rate for RMSprop.
-            lr_exp (double): Decay factor for exponential scheduler.
-            record_interval (int): The number of iterations to print loss info
-            store (bool): If true, self.surrogate_save() will be called.
-            reg (bool): If true, L1 regularization will be used with parameter 0.0001
+            nf (instance of normalizing flow): the normalizing flow architecture used for variational inference
+            optimizer (instance of PyTorch optimizer): the selected PyTorch optimizer
+            iteration (int): current iteration number
+            log (list of lists): stores a log of [iteration, annealing temperature, loss value]
+            sampling (bool): Flag indicating the sampling stage
+            t (double): current inverse temperature for annealing scheduler
 
         Returns:
             None
         """
-        print('')
-        print('--- Pre-training surrogate model')
-        print('')
-        grid = (self.pre_grid - self.m) / self.sd
-        out = (self.pre_out - self.tm) / self.tsd
-        optimizer = torch.optim.RMSprop(self.surrogate.parameters(), lr=lr)
-        scheduler = torch.optim.lr_scheduler.ExponentialLR(optimizer, lr_exp)
-        for i in range(max_iters):
-            self.surrogate.train()            
-            y = self.surrogate(grid)
-            loss = torch.sum((y - out) ** 2) / y.size(0)
-            if reg:
-                reg_loss = 0
-                for param in self.surrogate.parameters():
-                    reg_loss += torch.abs(param).sum() * 0.0001
-                loss += reg_loss
-            optimizer.zero_grad()
-            loss.backward()
-            optimizer.step()
-            scheduler.step()
-
-            if i % record_interval == 0:
-                if reg:
-                    print('SUR: PRE: it: %7d | loss: %8.3e | reg_loss: %8.3e' % (i, loss, reg_loss))
-                else:
-                    print('SUR: PRE: it: %7d | loss: %8.3e' % (i, loss))
-        print('')
-        print('--- Surrogate model pre-train complete')
-        print('')
-        if store:
-            self.surrogate_save()
-
-    def update(self, x, max_iters=10000, lr=0.01, lr_exp=0.999, record_interval=500, store=False, tol=1e-5, reg=False):
-        """Model calibration for NoFAS.
-        
-        Fine tuning is performed with the RMSprop optimizer and an exponential learning rate scheduler.
-        
-        Args:
-            x (torch.Tensor): Input feature that needs true model output.
-            max_iters (int): Maximum number of iteration. Default 10000.
-            lr (double): Learning rate for RMSprop. Default 0.01.
-            lr_exp (double): Decay factor of exponential scheduler.
-            record_interval (int): The number of iterations to print loss information.
-            store (bool): If ture, self.surrogate_save() will be called.
-            tol (double): Optimization will be terminated if loss < tol ** 2.
-            reg (bool): If ture, L1 regularizaiton will be used with parameter 0.1.
 
-        Returns:
-            None
-        """
-        self.grid_record = torch.cat((self.grid_record.to(self.device), x), dim=0)
-        s = torch.std(x, dim=0)
-        thresh = torch.tensor(0.1).to(self.device)
-        if torch.any(s < thresh):
-            p = x[:, s < thresh]
-            x[:, s < thresh] += torch.normal(0, 1, size=tuple(p.size())).to(self.device) * thresh
-        s_aft = torch.std(x, dim=0)            
-        
-        # Print the std for each dimension before and after inflation    
-        print('')
-        print('--- Updating surrogate model')
-        print('')
-        print('Std before inflation -> Std after inflation')
-        for loopA in range(s.size(0)):
-          print("%8.3e -> %8.3e" % (s[loopA],s_aft[loopA]))
-        print('')          
-
-        if len(self.memory_grid) >= self.memory_len:
-            self.memory_grid.pop()
-            self.memory_out.pop()
-        self.memory_grid.insert(0, (x - self.m) / self.sd)
-        self.memory_out.insert(0, (self.mf(x) - self.tm) / self.tsd)
-        sizes = [list(self.pre_grid.size())[0]] + [list(item.size())[0] for item in self.memory_grid]
-
-        optimizer = torch.optim.RMSprop(self.surrogate.parameters(), lr=lr)
-        scheduler = torch.optim.lr_scheduler.ExponentialLR(optimizer, lr_exp)
-        for i in range(max_iters):
-            self.surrogate.train()            
-            y = self.surrogate(torch.cat(((self.pre_grid - self.m) / self.sd, *self.memory_grid), dim=0))
-            out = torch.cat(((self.pre_out - self.tm) / self.tsd, *self.memory_out), dim=0)
-            raw_loss = torch.stack([item.mean() for item in torch.split(torch.sum((y - out) ** 2, dim=1), sizes)])
-            loss = raw_loss[0] * 2 * self.beta_0 * self.weights[:len(self.memory_grid)].sum() + \
-                   torch.sum(raw_loss[1:] * self.weights[:len(self.memory_grid)]) * (1 - self.beta_0) * 2
-
-            # loss = raw_loss[0] * self.weights[:len(self.memory_grid)].sum() + torch.sum(
-            #     raw_loss[1:] * self.weights[:len(self.memory_grid)])
-
-            if reg:
-                for param in self.surrogate.parameters():
-                    loss += torch.abs(param).sum() * 0.1
-            optimizer.zero_grad()
-            loss.backward()
-            optimizer.step()
-            scheduler.step()
-
-            if i % record_interval == 0:
-                # print('Updating: {}\t loss {}'.format(i, loss), end='\r')
-                print('SUR: UPD: it: %7d | loss: %8.3e' % (i, loss))
-            if loss < tol ** 2: break
-        # print('                                                        ', end='\r')
-        print('')
-        print('--- Surrogate model updated')
-        print('')                  
-        if store:
-            self.surrogate_save()
+        # Set the normalizing flow in training mode
+        nf.train()
 
-    def forward(self, x):
-        """Function to evaluate the surrogate
-        
-        Args:
-            x (torch.Tensor): Contains a matrix of model inputs in the form [data_num, feature_dim]
+        # Evaluate the Jacobian terms in  loss function
+        x0 = nf.base_dist.sample([self.batch_size])
+        xk, sum_log_abs_det_jacobians = nf(x0)
+
+        # generate and save samples evaluation
+        if sampling and iteration % self.save_interval == 0:
+            print('--- Saving results at iteration '+str(iteration))
+            x00 = nf.base_dist.sample([self.n_sample])
+            xkk, _ = nf(x00)
+            # Save surrogate grid
+            if not(self.surrogate is None):
+              np.savetxt(self.output_dir + '/' + self.name + '_grid_' + str(iteration), self.surrogate.grid_record.clone().cpu().numpy(), newline="\n")
+            # Save log profile
+            np.savetxt(self.output_dir + '/' + self.log_file, np.array(log), newline="\n")
+            # Save transformed samples          
+            np.savetxt(self.output_dir + '/' + self.name + '_samples_' + str(iteration), xkk.data.clone().cpu().numpy(), newline="\n")
+            # Save samples in the original space
+            if not(self.transform is None):
+              xkk_samples = self.transform.forward(xkk).data.cpu().numpy()
+              np.savetxt(self.output_dir + '/' + self.name + '_params_' + str(iteration), xkk_samples, newline="\n")
+            else:
+              xkk_samples = xkk.data.cpu().numpy()
+              np.savetxt(self.output_dir + '/' + self.name + '_params_' + str(iteration), xkk_samples, newline="\n")
+            # Save marginal statistics
+            np.savetxt(self.output_dir + '/' + self.name + '_marginal_stats_' + str(iteration), np.concatenate((xkk_samples.mean(axis=0).reshape(-1,1),xkk_samples.std(axis=0).reshape(-1,1)),axis=1), newline="\n")
+            # Save log density at the same samples
+            np.savetxt(self.output_dir + '/' + self.name + '_logdensity_' + str(iteration), self.model_logdensity(xkk).data.cpu().numpy(), newline="\n")
+            # Save model outputs at the samples - If a model is defined
+            if not(self.transform is None):
+              stds = torch.abs(self.model.solve_t(self.model.defParam)).to(self.device) * self.model.stdRatio
+              o00 = torch.randn(x00.size(0), self.model.data.shape[0]).to(self.device)
+              noise = o00*stds.repeat(o00.size(0),1)
+              if self.surrogate:
+                np.savetxt(self.output_dir + '/' + self.name + '_outputs_' + str(iteration), (self.surrogate.forward(xkk) + noise).data.cpu().numpy(), newline="\n")
+              else:
+                np.savetxt(self.output_dir + '/' + self.name + '_outputs_' + str(iteration), (self.model.solve_t(self.transform.forward(xkk)) + noise).data.cpu().numpy(), newline="\n")
+
+        if torch.any(torch.isnan(xk)):
+            print("Error: samples xk are nan at iteration " + str(iteration))
+            print(xk)
+            np.savetxt(self.output_dir + '/' + self.log_file, np.array(log), newline="\n")
+            exit(-1)
 
-        Returns:
-            COMPLETE!!!
+        # updating surrogate model
+        if self.run_nofas and iteration % self.calibrate_interval == 0 and self.surrogate.grid_record.size(0) < self.budget:
+            xk0 = xk[:self.true_data_num, :].data.clone()            
+            # print("\n")
+            # print(list(self.surrogate.grid_record.size())[0])
+            # print(xk0)
+            self.surrogate.update(xk0, max_iters=self.surr_upd_it)
+
+        # Free energy bound
+        loss = (- torch.sum(sum_log_abs_det_jacobians, 1) - t * self.model_logdensity(xk)).mean()
+        optimizer.zero_grad()
+        loss.backward()
+        optimizer.step()
+        if iteration % self.log_interval == 0:
+            print('VI NF (t=%5.3f): it: %7d | loss: %8.3e' % (t,iteration, loss.item()))
+            log.append([t, iteration, loss.item()])
+        
+        # Save state of normalizing flow layers
+        if self.store_nf_interval > 0 and iteration % self.store_nf_interval == 0:
+            torch.save(nf.state_dict(), self.output_dir + '/' + self.name + "_" + str(iteration) + ".nf")
 
-        """
-        return self.surrogate((x - self.m) / self.sd) * self.tsd + self.tm
+        if not(self.store_surr_interval is None) and self.store_surr_interval > 0 and iteration % self.store_surr_interval == 0:
+            self.surrogate.surrogate_save() # Save surrogate model
```

### Comparing `linfa_vi-1.1.6/linfa/plot_res.py` & `linfa_vi-1.1.7/linfa/plot_res.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.6/linfa/transform.py` & `linfa_vi-1.1.7/linfa/transform.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.6/linfa_vi.egg-info/PKG-INFO` & `linfa_vi-1.1.7/linfa_vi.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linfa-vi
-Version: 1.1.6
+Version: 1.1.7
 Summary: A Python library for inference with normalizing flow and annealing
 Author-email: resDesLab  <daniele.schiavazzi@gmail.com>
 License: Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -114,15 +114,14 @@
 
 A step by step [tutorial](tutorial/TutorialwithPhys.ipynb) is also available which will guide you through the an inference problem for a ballistic simulation. 
 
 ### Citation
 
 Did you use LINFA? Please cite our paper using:
 ```
-@misc{TO BE FINALIZED!!!,
-      title={LINFA: a Python library for variational inference with normalizing flow and annealing}, 
-      author={Yu Wang, Emma R. Cobian, Fang Liu, Jonathan D. Hauenstein, Daniele E. Schiavazzi},
-      year={2022},
-      eprint={2201.03715},
-      archivePrefix={arXiv},
-      primaryClass={eess.IV}
+@article{linfa-vi-paper,
+  title={LINFA: a Python library for variational inference with normalizing flow and annealing},
+  author={Wang, Yu and Cobian, Emma R and Lee, Jubilee and Liu, Fang and Hauenstein, Jonathan D and Schiavazzi, Daniele E},
+  journal={arXiv preprint arXiv:2307.04675},
+  year={2023}
 }
+```
```

### Comparing `linfa_vi-1.1.6/pyproject.toml` & `linfa_vi-1.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "linfa_vi"
-version = "1.1.6"
+version = "1.1.7"
 description = "A Python library for inference with normalizing flow and annealing"
 readme = "README.md"
 authors = [{ name = "resDesLab ", email = "daniele.schiavazzi@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

