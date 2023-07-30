# Comparing `tmp/elsarec-0.1.3.tar.gz` & `tmp/elsarec-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elsarec-0.1.3.tar", last modified: Fri Sep 16 09:17:38 2022, max compression
+gzip compressed data, was "elsarec-0.1.4.tar", last modified: Sun Jul 30 05:41:57 2023, max compression
```

## Comparing `elsarec-0.1.3.tar` & `elsarec-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 09:17:38.395605 elsarec-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-09-16 09:17:25.000000 elsarec-0.1.3/LICENCE
--rw-r--r--   0 runner    (1001) docker     (121)     3982 2022-09-16 09:17:38.395605 elsarec-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3104 2022-09-16 09:17:25.000000 elsarec-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 09:17:38.395605 elsarec-0.1.3/elsa/
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-09-16 09:17:25.000000 elsarec-0.1.3/elsa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21966 2022-09-16 09:17:25.000000 elsarec-0.1.3/elsa/elsa.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 09:17:38.395605 elsarec-0.1.3/elsarec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3982 2022-09-16 09:17:38.000000 elsarec-0.1.3/elsarec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-09-16 09:17:38.000000 elsarec-0.1.3/elsarec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-16 09:17:38.000000 elsarec-0.1.3/elsarec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-09-16 09:17:38.000000 elsarec-0.1.3/elsarec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-16 09:17:38.000000 elsarec-0.1.3/elsarec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-09-16 09:17:25.000000 elsarec-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-16 09:17:38.395605 elsarec-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1263 2022-09-16 09:17:25.000000 elsarec-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:41:57.441350 elsarec-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-30 05:41:47.000000 elsarec-0.1.4/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-07-30 05:41:57.441350 elsarec-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-30 05:41:47.000000 elsarec-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:41:57.437350 elsarec-0.1.4/elsa/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-30 05:41:47.000000 elsarec-0.1.4/elsa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21921 2023-07-30 05:41:47.000000 elsarec-0.1.4/elsa/elsa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:41:57.441350 elsarec-0.1.4/elsarec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-07-30 05:41:57.000000 elsarec-0.1.4/elsarec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-30 05:41:57.000000 elsarec-0.1.4/elsarec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 05:41:57.000000 elsarec-0.1.4/elsarec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-30 05:41:57.000000 elsarec-0.1.4/elsarec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-30 05:41:57.000000 elsarec-0.1.4/elsarec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-30 05:41:47.000000 elsarec-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 05:41:57.441350 elsarec-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-30 05:41:47.000000 elsarec-0.1.4/setup.py
```

### Comparing `elsarec-0.1.3/LICENCE` & `elsarec-0.1.4/LICENCE`

 * *Files identical despite different names*

### Comparing `elsarec-0.1.3/PKG-INFO` & `elsarec-0.1.4/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: elsarec
-Version: 0.1.3
-Summary: Scalable Linear Shallow Autoencoder for Collaborative Filtering
-Author: Recombee
-Author-email: vojtech.vancura@recombee.com
-License: MIT
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Software Development
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENCE
-
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 # ELSA
 
 This is an official implementation of our paper [Scalable Linear Shallow Autoencoder for Collaborative Filtering](https://dl.acm.org/doi/10.1145/3523227.3551482).
 
 ### Requirements
@@ -56,15 +33,14 @@
 
 items_cnt = X_csr.shape[1]
 factors = 256 
 num_epochs = 5
 batch_size = 128
 
 model = ELSA(n_items=items_cnt, device=device, n_dims=factors)
-model.compile()
 
 model.fit(X_csr, batch_size=batch_size, epochs=num_epochs)
 
 # save item embeddings into np array
 A = torch.nn.functional.normalize(model.get_items_embeddings(), dim=-1).cpu().numpy()
 
 # get predictions in PyTorch
@@ -78,15 +54,17 @@
 related = model.similar_items(N=100, batch_size=128, sources=itemids)
 ```
 
 ## Notes
 
 ### Reproducibility
 
-Please get in touch with us if you want to reproduce the results from our paper. 
+Instructions for reproducing the results from the paper on the MovieLens20M dataset are in the branch `reproduce_movielens` https://github.com/recombee/ELSA/tree/reproduce_movielens.
+
+Reproducibility instructions for Netflix and Goodbooks10k datasets will follow soon.
 
 ### Tensorflow users
 
 We decided to implement ELSA in PyTorch, but implementation in TensorFlow is simple and straightforward. One can, for example, implement ELSA as a Keras layer:
 
 ```python
 class ELSA(tf.keras.layers.Layer):
@@ -102,16 +80,40 @@
         A = tf.math.l2_normalize(self.A, axis=-1)
         return A.numpy()
     
     @tf.function
     def call(self, x):
         A = tf.math.l2_normalize(self.A, axis=-1)
         xA = tf.matmul(x, A, transpose_b=False)
-        xAAT = tf.matmul(xA, feature, transpose_b=True)
+        xAAT = tf.matmul(xA, A, transpose_b=True)
         return xAAT - x
 ```
 
 ### Licence
 [MIT licence](https://github.com/recombee/ELSA/blob/main/LICENCE)
 
 ### Troubleshooting
 If you encounter a problem or have a question about ELSA, do not hesitate to create an issue and ask. In case of an implementation problem, please include the Python, PyTorch and CUDA versions in the description of the issue.
+
+### Cite us
+
+Please consider citing our paper:
+
+```
+@inproceedings{10.1145/3523227.3551482,
+author = {Van\v{c}ura, Vojt\v{e}ch and Alves, Rodrigo and Kasalick\'{y}, Petr and Kord\'{\i}k, Pavel},
+title = {Scalable Linear Shallow Autoencoder for Collaborative Filtering},
+year = {2022},
+isbn = {9781450392785},
+publisher = {Association for Computing Machinery},
+address = {New York, NY, USA},
+url = {https://doi.org/10.1145/3523227.3551482},
+doi = {10.1145/3523227.3551482},
+abstract = {Recently, the RS research community has witnessed a surge in popularity for shallow autoencoder-based CF methods. Due to its straightforward implementation and high accuracy$
+booktitle = {Proceedings of the 16th ACM Conference on Recommender Systems},
+pages = {604–609},
+numpages = {6},
+keywords = {Linear models, Shallow autoencoders, Implicit feedback recommendation},
+location = {Seattle, WA, USA},
+series = {RecSys '22}
+}
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `elsarec-0.1.3/elsa/elsa.py` & `elsarec-0.1.4/elsa/elsa.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,60 +1,53 @@
 import time
 import typing
 import logging
 
 import numpy as np
 import torch
-import torch.nn as nn
 import scipy
 
 logger = logging.getLogger(__name__)
 
-# TODO:
-# Implement partial_fit_items method
 
-
-class ELSA(nn.Module):
+class ELSA(torch.nn.Module):
     """
     Scalable Linear Shallow Autoencoder for Collaborative Filtering
     """
 
-    def __init__(self, n_items: int, n_dims: int, device: torch.device = None):
+    def __init__(self, n_items: int, n_dims: int, device: torch.device = None, lr: float = 0.1):
         """
         Train model with given training data
 
         Parameters
         ----------
         n_items : int
             Number of items recognized by ELSA (in the paper denotes as 'I')
         n_dims : int
             Size of the items' latent space (in the paper denotes as 'r')
         device : torch.device, optional
             ELSA's weights will allocated on this device
         """
         super(ELSA, self).__init__()
-        W = nn.Parameter(torch.nn.init.xavier_uniform_(torch.empty([n_items, n_dims])).detach().clone())
-        W.requires_grad = True
-        self.W_list = nn.ParameterList([W])
+        W = torch.nn.Parameter(torch.nn.init.xavier_uniform_(torch.empty([n_items, n_dims])).detach().clone())
+        self.__W_list = torch.nn.ParameterList([W])
         self.__device = device or torch.device("cuda")
         self.__items_cnt = n_items
-
-    def compile(self, lr: float = 0.1):
-        self.to(self.__device)
-        self.optimizer = torch.optim.NAdam(self.parameters(), lr=lr)
+        self.__optimizer = torch.optim.NAdam(self.parameters(), lr=lr)
         # Loss function of ELSA is NMSE, but PyTorch implements only MSE. Normalization is done manually in train_step function
-        self.criterion = nn.MSELoss()
-        self.cosine = torch.nn.CosineSimilarity(dim=1, eps=1e-08)
+        self.__criterion = torch.nn.MSELoss()
+        self.__cosine = torch.nn.CosineSimilarity(dim=1, eps=1e-08)
+        self.to(self.__device)
 
     def train_step(self, x, y):
         self.zero_grad()
         output = self(x)
-        loss = self.criterion(nn.functional.normalize(output, dim=-1), nn.functional.normalize(y, dim=-1))
+        loss = self.__criterion(torch.nn.functional.normalize(output, dim=-1), torch.nn.functional.normalize(y, dim=-1))
         loss.backward()
-        self.optimizer.step()
+        self.__optimizer.step()
         return loss, output
 
     def fit(
         self,
         train_data: typing.Union[
             torch.utils.data.dataloader.DataLoader,
             np.ndarray,
@@ -120,15 +113,15 @@
                 # Check that io_batch.shape[1] is the same as number of items in ELSA. If not, print reasonable error
                 if io_batch.shape[1] != self.__items_cnt:
                     raise ValueError(
                         f"Number of items recognized by ELSA model is {self.__items_cnt}, but given data/dataloader yields data with second dimension {io_batch.shape[1]}."
                     )
                 loss, predictions = self.train_step(io_batch, io_batch)  # Input is also output, since ELSA is an autoencoder
                 nmse_losses_per_epoch.append(loss.item())
-                cosine_losses_per_epoch.append(1 - torch.mean(self.cosine(io_batch, predictions), dim=-1).item())
+                cosine_losses_per_epoch.append(1 - torch.mean(self.__cosine(io_batch, predictions), dim=-1).item())
                 if verbose:
                     log_dict = {
                         "Epoch": f"{epoch_index}/{epochs}",
                         "Step": f"{step}/{total_steps}",
                         "nmse_train": round(np.mean(cosine_losses_per_epoch), 4),
                         "cosine_train": round(np.mean(cosine_losses_per_epoch), 4),
                         "time": f"{(time.time()-epoch_start):2f}s",
@@ -150,20 +143,20 @@
                 epoch_start = time.time()
                 nmse_losses_per_epoch = []
                 cosine_losses_per_epoch = []
                 with torch.no_grad():
                     for step, io_batch in enumerate(validation_dataloader, start=1):
                         output = self(io_batch)
                         nmse_losses_per_epoch.append(
-                            self.criterion(
-                                nn.functional.normalize(output, dim=-1),
-                                nn.functional.normalize(io_batch, dim=-1),
+                            self.__criterion(
+                                torch.nn.functional.normalize(output, dim=-1),
+                                torch.nn.functional.normalize(io_batch, dim=-1),
                             ).item()
                         )
-                        cosine_losses_per_epoch.append(1 - torch.mean(self.cosine(io_batch, output), dim=-1).item())
+                        cosine_losses_per_epoch.append(1 - torch.mean(self.__cosine(io_batch, output), dim=-1).item())
 
                 losses["nmse_val"].append(np.mean(nmse_losses_per_epoch))
                 losses["cosine_val"].append(np.mean(cosine_losses_per_epoch))
 
                 log_dict = {
                     **log_dict,
                     **{
@@ -189,17 +182,17 @@
         device : str or torch.device
         """
         if isinstance(device, str):
             device = torch.device(device)
         elif not isinstance(device, torch.device):
             raise ValueError(f"Device must be specified by string or by torch.device instance, but '{type(device)}' was given.")
         self.__device = device
-        for i, W in enumerate(self.W_list):
+        for i, W in enumerate(self.__W_list):
             if W.device != self.__device:
-                self.W_list[i] = W.to(self.__device)
+                self.__W_list[i] = W.to(self.__device)
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         """
         Give tensor 'x' to forward pass ELSA by computing (xAA^T - x) where A is a tensor of item embeddings
 
         Parameters
         ----------
@@ -207,15 +200,15 @@
             Input two-dimensional tensor where second dimension is required to be 'num_items'
 
         Returns
         -------
         torch.Tensor
             Predicted tensor with the same shape as input tensor 'x'
         """
-        A = nn.functional.normalize(self.__get_weights(), dim=-1)
+        A = torch.nn.functional.normalize(self.__get_weights(), dim=-1)
         xA = torch.matmul(x, A)
         xAAT = torch.matmul(xA, A.T)
         return xAAT - x
 
     def get_items_embeddings(self, as_numpy: bool = False) -> typing.Union[torch.Tensor, np.ndarray]:
         """
         Get embeddings for all items as 2-dimensional Tensor (or numpy array if as_numpy=True) with dimensions (n_items, n_dims)
@@ -387,15 +380,15 @@
             if input_batch.shape[1] != self.__items_cnt:
                 raise ValueError(
                     f"Number of items recognized by ELSA model is {self.__items_cnt}, but given data/dataloader yields data with second dimension {input_batch.shape[1]}."
                 )
             yield self.forward(input_batch).detach()
 
     def __get_weights(self):
-        return torch.vstack([param.to(self.__device) for param in self.W_list])
+        return torch.vstack([param.to(self.__device) for param in self.__W_list])
 
     @staticmethod
     def __convert_data_to_dataloader(
         data: typing.Union[
             torch.utils.data.dataloader.DataLoader,
             np.ndarray,
             torch.Tensor,
```

### Comparing `elsarec-0.1.3/elsarec.egg-info/PKG-INFO` & `elsarec-0.1.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elsarec
-Version: 0.1.3
+Version: 0.1.4
 Summary: Scalable Linear Shallow Autoencoder for Collaborative Filtering
 Author: Recombee
 Author-email: vojtech.vancura@recombee.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -13,14 +13,15 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 # ELSA
@@ -56,15 +57,14 @@
 
 items_cnt = X_csr.shape[1]
 factors = 256 
 num_epochs = 5
 batch_size = 128
 
 model = ELSA(n_items=items_cnt, device=device, n_dims=factors)
-model.compile()
 
 model.fit(X_csr, batch_size=batch_size, epochs=num_epochs)
 
 # save item embeddings into np array
 A = torch.nn.functional.normalize(model.get_items_embeddings(), dim=-1).cpu().numpy()
 
 # get predictions in PyTorch
@@ -78,15 +78,17 @@
 related = model.similar_items(N=100, batch_size=128, sources=itemids)
 ```
 
 ## Notes
 
 ### Reproducibility
 
-Please get in touch with us if you want to reproduce the results from our paper. 
+Instructions for reproducing the results from the paper on the MovieLens20M dataset are in the branch `reproduce_movielens` https://github.com/recombee/ELSA/tree/reproduce_movielens.
+
+Reproducibility instructions for Netflix and Goodbooks10k datasets will follow soon.
 
 ### Tensorflow users
 
 We decided to implement ELSA in PyTorch, but implementation in TensorFlow is simple and straightforward. One can, for example, implement ELSA as a Keras layer:
 
 ```python
 class ELSA(tf.keras.layers.Layer):
@@ -102,16 +104,40 @@
         A = tf.math.l2_normalize(self.A, axis=-1)
         return A.numpy()
     
     @tf.function
     def call(self, x):
         A = tf.math.l2_normalize(self.A, axis=-1)
         xA = tf.matmul(x, A, transpose_b=False)
-        xAAT = tf.matmul(xA, feature, transpose_b=True)
+        xAAT = tf.matmul(xA, A, transpose_b=True)
         return xAAT - x
 ```
 
 ### Licence
 [MIT licence](https://github.com/recombee/ELSA/blob/main/LICENCE)
 
 ### Troubleshooting
 If you encounter a problem or have a question about ELSA, do not hesitate to create an issue and ask. In case of an implementation problem, please include the Python, PyTorch and CUDA versions in the description of the issue.
+
+### Cite us
+
+Please consider citing our paper:
+
+```
+@inproceedings{10.1145/3523227.3551482,
+author = {Van\v{c}ura, Vojt\v{e}ch and Alves, Rodrigo and Kasalick\'{y}, Petr and Kord\'{\i}k, Pavel},
+title = {Scalable Linear Shallow Autoencoder for Collaborative Filtering},
+year = {2022},
+isbn = {9781450392785},
+publisher = {Association for Computing Machinery},
+address = {New York, NY, USA},
+url = {https://doi.org/10.1145/3523227.3551482},
+doi = {10.1145/3523227.3551482},
+abstract = {Recently, the RS research community has witnessed a surge in popularity for shallow autoencoder-based CF methods. Due to its straightforward implementation and high accuracy$
+booktitle = {Proceedings of the 16th ACM Conference on Recommender Systems},
+pages = {604–609},
+numpages = {6},
+keywords = {Linear models, Shallow autoencoders, Implicit feedback recommendation},
+location = {Seattle, WA, USA},
+series = {RecSys '22}
+}
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `elsarec-0.1.3/setup.py` & `elsarec-0.1.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="elsarec",
-    version="0.1.3",
+    version="0.1.4",
     description="Scalable Linear Shallow Autoencoder for Collaborative Filtering",
     author="Recombee",
     author_email="vojtech.vancura@recombee.com",
     license="MIT",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
@@ -20,14 +20,15 @@
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     packages=find_packages(),
     # PyTorch needs to be installed manually since it is not on pypi
     install_requires=["numpy", "scipy"],
     python_requires=">=3.7",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

