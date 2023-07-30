# Comparing `tmp/SGtSNEpiPy-1.1.3.tar.gz` & `tmp/SGtSNEpiPy-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SGtSNEpiPy-1.1.3.tar", last modified: Sun Jul 30 04:56:41 2023, max compression
+gzip compressed data, was "SGtSNEpiPy-1.1.4.tar", last modified: Sun Jul 30 04:59:13 2023, max compression
```

## Comparing `SGtSNEpiPy-1.1.3.tar` & `SGtSNEpiPy-1.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-30 04:56:41.106984 SGtSNEpiPy-1.1.3/
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)     9024 2023-07-30 04:56:41.107088 SGtSNEpiPy-1.1.3/PKG-INFO
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)     8630 2023-07-30 04:54:29.000000 SGtSNEpiPy-1.1.3/README.md
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       38 2023-07-30 04:56:41.107432 SGtSNEpiPy-1.1.3/setup.cfg
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      808 2023-07-30 04:56:15.000000 SGtSNEpiPy-1.1.3/setup.py
-drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-30 04:56:41.104944 SGtSNEpiPy-1.1.3/src/
-drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-30 04:56:41.106029 SGtSNEpiPy-1.1.3/src/SGtSNEpiPy/
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)     2055 2023-07-28 17:34:50.000000 SGtSNEpiPy-1.1.3/src/SGtSNEpiPy/SGtSNEpiPy.py
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 02:34:15.000000 SGtSNEpiPy-1.1.3/src/SGtSNEpiPy/__init__.py
-drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-30 04:56:41.106823 SGtSNEpiPy-1.1.3/src/SGtSNEpiPy.egg-info/
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)     9024 2023-07-30 04:56:41.000000 SGtSNEpiPy-1.1.3/src/SGtSNEpiPy.egg-info/PKG-INFO
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      273 2023-07-30 04:56:41.000000 SGtSNEpiPy-1.1.3/src/SGtSNEpiPy.egg-info/SOURCES.txt
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)        1 2023-07-30 04:56:41.000000 SGtSNEpiPy-1.1.3/src/SGtSNEpiPy.egg-info/dependency_links.txt
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       18 2023-07-30 04:56:41.000000 SGtSNEpiPy-1.1.3/src/SGtSNEpiPy.egg-info/requires.txt
--rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       11 2023-07-30 04:56:41.000000 SGtSNEpiPy-1.1.3/src/SGtSNEpiPy.egg-info/top_level.txt
+drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-30 04:59:13.987742 SGtSNEpiPy-1.1.4/
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)     9046 2023-07-30 04:59:13.987854 SGtSNEpiPy-1.1.4/PKG-INFO
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)     8652 2023-07-30 04:58:55.000000 SGtSNEpiPy-1.1.4/README.md
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       38 2023-07-30 04:59:13.988199 SGtSNEpiPy-1.1.4/setup.cfg
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      808 2023-07-30 04:58:50.000000 SGtSNEpiPy-1.1.4/setup.py
+drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-30 04:59:13.985775 SGtSNEpiPy-1.1.4/src/
+drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-30 04:59:13.986801 SGtSNEpiPy-1.1.4/src/SGtSNEpiPy/
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)     2055 2023-07-28 17:34:50.000000 SGtSNEpiPy-1.1.4/src/SGtSNEpiPy/SGtSNEpiPy.py
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-10 02:34:15.000000 SGtSNEpiPy-1.1.4/src/SGtSNEpiPy/__init__.py
+drwxr-xr-x   0 chenshuhaoqin   (501) staff       (20)        0 2023-07-30 04:59:13.987578 SGtSNEpiPy-1.1.4/src/SGtSNEpiPy.egg-info/
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)     9046 2023-07-30 04:59:13.000000 SGtSNEpiPy-1.1.4/src/SGtSNEpiPy.egg-info/PKG-INFO
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)      273 2023-07-30 04:59:13.000000 SGtSNEpiPy-1.1.4/src/SGtSNEpiPy.egg-info/SOURCES.txt
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)        1 2023-07-30 04:59:13.000000 SGtSNEpiPy-1.1.4/src/SGtSNEpiPy.egg-info/dependency_links.txt
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       18 2023-07-30 04:59:13.000000 SGtSNEpiPy-1.1.4/src/SGtSNEpiPy.egg-info/requires.txt
+-rw-r--r--   0 chenshuhaoqin   (501) staff       (20)       11 2023-07-30 04:59:13.000000 SGtSNEpiPy-1.1.4/src/SGtSNEpiPy.egg-info/top_level.txt
```

### Comparing `SGtSNEpiPy-1.1.3/PKG-INFO` & `SGtSNEpiPy-1.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SGtSNEpiPy
-Version: 1.1.3
+Version: 1.1.4
 Summary: SGtSNEpiPy is a Python interface to SG-t-SNE-П, a powerful tool for visualizing large, sparse, stochastic graphs.
 Author: ['Chenshuhao Qin', 'Yihua Zhong']
 Author-email: cq27@duke.edu, yz737@duke.edu,
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
 
@@ -42,162 +42,162 @@
 **Note**: The rest of the content remains unchanged as it does not contain any reST-specific elements.
 
 
 See **[the full documentation](https://fcdimitr.github.io/SGtSNEpi.jl/stable)** for moredetails.
 
 
 
-##Parameters
+## Parameters
 
 **SGtSNEpiPy.SGtSNEpiPy.sgtsnepipy**
 
 This package only has one method currently.
 
 
 ```
     sgtsnepi(A)
 ```
 
 
-###A: the input CSR sparse matrix representing the data points' pairwise similarities. (Mandatory)
+### A: the input CSR sparse matrix representing the data points' pairwise similarities. (Mandatory)
 
 <ul>
 <li>Data Type: **scipy.sparse.csr.csr_matrix** (The matrix includes row, value, value, whose type are all **numpy.ndarray** with three arrays of **numpy.int32, numpy.int32, numpy.int64**)</li>
 <li>A CSR sparse matrix generated by package scipy.</li>
 </ul>
 
-###d: the number of dimensions of the embedding space. (Optional)
+### d: the number of dimensions of the embedding space. (Optional)
 
 <ul>
 <li>Data Type: Integer</li>
 <li>Default Value: 2</li>
 </ul>
 
-###λ: SG-t-SNE scaling factor. (Optional)
+### λ: SG-t-SNE scaling factor. (Optional)
 
 <ul>
 <li>Data Type: Integer or Float</li>
 <li>Default Value: 10</li>
 </ul>
 
-###max_iter: the maximum number of iterations for the optimization process. (Optional)
+### max_iter: the maximum number of iterations for the optimization process. (Optional)
 
 <ul>
 <li>Data Type: Integer</li>
 <li>Default Value: 1000</li>
 </ul>
 
-###early_exag: the number of early exageration iterations. (Optional)
+### early_exag: the number of early exageration iterations. (Optional)
 
 <ul>
 <li>Data Type: Integer</li>
 <li>Default Value: 250</li>
 </ul>
 
-###Y0: initial distribution in embedding space (randomly generated if nothing).(Optional)
+### Y0: initial distribution in embedding space (randomly generated if nothing).(Optional)
 
 <ul>
 <li>Data Type: A numpy array of shape (number of data points, d).</li>
 <li>Default Value: None</li>
 <li>You should set this parameter to generate reproducible results.</li>
 </ul>
 
-###profile: whether to enable profiling for the algorithm. (Optional)
+### profile: whether to enable profiling for the algorithm. (Optional)
 
 <ul>
 <li>Data Type: Boolean</li>
 <li>Default Value: False</li>
 <li>Meaning: disable/enable profiling. If enabled the function return a 3-tuple: (Y, t, g), where Y is the embedding coordinates, t are the execution times of each module per iteration (size 6 x max_iter) and g contains the grid size, the embedding domain size (maximum(Y) - minimum(Y)), and the scaling factor s_k for the band-limited version, per dimension (size 3 x max_iter).</li>
 </ul>
 
-###np: number of threads (set to 0 to use all available cores) (Optional)
+### np: number of threads (set to 0 to use all available cores) (Optional)
 
 <ul>
 <li>Data Type: Integer</li>
 <li>Default Value: threading.active_count(), which returns the number of active threads in the current process.</li>
 </ul>
 
-###h: grid side length (Optional)
+### h: grid side length (Optional)
 
 <ul>
 <li>Data Type: Float</li>
 <li>Default Value: 1.0</li>
 </ul>
 
-###u: either perplexity or value of λ (Optional)
+### u: either perplexity or value of λ (Optional)
 
 <ul>
 <li>Data Type: Integer</li>
 <li>Default Value: 10</li>
 </ul>
 
-###k: number of nearest neighbors (for kNN formation) (Optional)
+### k: number of nearest neighbors (for kNN formation) (Optional)
 
 <ul>
 <li>Data Type: Integer</li>
 <li>Default Value: 30</li>
 </ul>
 
-###eta: learning parameter (Optional)
+### eta: learning parameter (Optional)
 
 <ul>
 <li>Data Type: Integer or Float</li>
 <li>Default Value: 200.0</li>
 </ul>
 
-###alpha: exaggeration strength (applicable for first early_exag iterations). (Optional)
+### alpha: exaggeration strength (applicable for first early_exag iterations). (Optional)
 
 <ul>
 <li>Data Type: Integer or Float</li>
 <li>Default Value: 12</li>
 </ul>
 
-###fftw_single: Whether to use single-precision FFTW (Fast Fourier Transform) library. (Optional)
+### fftw_single: Whether to use single-precision FFTW (Fast Fourier Transform) library. (Optional)
 
 <ul>
 <li>Data Type: Boolean</li>
 <li>Default Value: False</li>
 </ul>
 
-###drop_leaf: remove edges connecting to leaf nodes. (Optional)
+### drop_leaf: remove edges connecting to leaf nodes. (Optional)
 
 <ul>
 <li>Data Type: Boolean</li>
 <li>Default Value: False</li>
 </ul>
 
-###list_grid_size: the list of allowed grid size along each dimension. (Optional)
+### list_grid_size: the list of allowed grid size along each dimension. (Optional)
 
 <ul>
 <li>Data Type: A list of integers</li>
 <li>Default Value: False.</li>
 <li>Affects FFT performance; most efficient if the size is a product of small primes. </li>
 </ul>
 
 **Warning:** 
 
 Because there is currently no replacement for Enum type in SGtSNEpy, we are missing the reduction of parameter you can change in Julia: **version**. Thus, the value will be its default value in Python.
 
-###version: the version of the algorithm for computing repulsive terms. (Optional)
+### version: the version of the algorithm for computing repulsive terms. (Optional)
 
 <ul>
 <li>Data Type: Enum (Julia)</li>
 <li>Default Value: NUCONV_BL</li>
 <li>Options are:
 </ul>
 <li>SGtSNEpi.NUCONV_BL (default): band-limited, approximated via non-uniform convolution</li>
 <li>SGtSNEpi.NUCONV: approximated via non-uniform convolution (higher resolution than SGtSNEpi.NUCONV_BL, slower execution time)</li>
 <li>SGtSNEpi.EXACT: no approximation; quadratic complexity, use only with small datasets</li>
 </ul>
 
-##Returns
+## Returns
 
 - Data Type: **numpy.ndarray** with three arrays: **numpy.int32, numpy.int32, numpy.float4**
 
-##Examples
+## Examples
 Here is an example to use function sgtsnepipy to generate a 2D embedding of an ER model.
 You have to use import networkx to generate a ER graph and matplotlib to visualize the embedding
 
 
 ```
     from SGtSNEpiPy.SGtSNEpiPy import sgtsnepipy
     import networkx as nx
@@ -226,22 +226,22 @@
     plt.colorbar(label='Node degree')
     plt.title("2D embedding of ER model (n = 1000, p = 0.2, seed = 170)")
 
     plt.show()
 ```
 
 
-##Contact
+## Contact
 
 Chenshuhao(Cody) Qin: chenshuhao.qin@duke.edu
 
 Yihua(Aaron) Zhong: yihua.zhong@duke.edu
 
 
-##Citation
+## Citation
 
 - Nikos Pitsianis, Alexandros-Stavros Iliopoulos, Dimitris Floros, Xiaobai Sun, **[Spaceland Embedding of Sparse Stochastic Graphs](https://doi.org/10.1109/HPEC.2019.8916505)**, In IEEE High Performance Extreme Computing Conference, 2019.
 - Nikos Pitsianis, Dimitris Floros, Alexandros-Stavros Iliopoulos, Xiaobai Sun, **[SG-t-SNE-Π: Swift Neighbor Embedding of Sparse Stochastic Graphs](https://doi.org/10.21105/joss.01577)**, Journal of Open Source Software, 4(39), 1577, 2019.
 
 If you use this software, please cite the following paper.
 
 ```
```

### Comparing `SGtSNEpiPy-1.1.3/README.md` & `SGtSNEpiPy-1.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,162 +32,162 @@
 **Note**: The rest of the content remains unchanged as it does not contain any reST-specific elements.
 
 
 See **[the full documentation](https://fcdimitr.github.io/SGtSNEpi.jl/stable)** for moredetails.
 
 
 
-##Parameters
+## Parameters
 
 **SGtSNEpiPy.SGtSNEpiPy.sgtsnepipy**
 
 This package only has one method currently.
 
 
 ```
     sgtsnepi(A)
 ```
 
 
-###A: the input CSR sparse matrix representing the data points' pairwise similarities. (Mandatory)
+### A: the input CSR sparse matrix representing the data points' pairwise similarities. (Mandatory)
 
 <ul>
 <li>Data Type: **scipy.sparse.csr.csr_matrix** (The matrix includes row, value, value, whose type are all **numpy.ndarray** with three arrays of **numpy.int32, numpy.int32, numpy.int64**)</li>
 <li>A CSR sparse matrix generated by package scipy.</li>
 </ul>
 
-###d: the number of dimensions of the embedding space. (Optional)
+### d: the number of dimensions of the embedding space. (Optional)
 
 <ul>
 <li>Data Type: Integer</li>
 <li>Default Value: 2</li>
 </ul>
 
-###λ: SG-t-SNE scaling factor. (Optional)
+### λ: SG-t-SNE scaling factor. (Optional)
 
 <ul>
 <li>Data Type: Integer or Float</li>
 <li>Default Value: 10</li>
 </ul>
 
-###max_iter: the maximum number of iterations for the optimization process. (Optional)
+### max_iter: the maximum number of iterations for the optimization process. (Optional)
 
 <ul>
 <li>Data Type: Integer</li>
 <li>Default Value: 1000</li>
 </ul>
 
-###early_exag: the number of early exageration iterations. (Optional)
+### early_exag: the number of early exageration iterations. (Optional)
 
 <ul>
 <li>Data Type: Integer</li>
 <li>Default Value: 250</li>
 </ul>
 
-###Y0: initial distribution in embedding space (randomly generated if nothing).(Optional)
+### Y0: initial distribution in embedding space (randomly generated if nothing).(Optional)
 
 <ul>
 <li>Data Type: A numpy array of shape (number of data points, d).</li>
 <li>Default Value: None</li>
 <li>You should set this parameter to generate reproducible results.</li>
 </ul>
 
-###profile: whether to enable profiling for the algorithm. (Optional)
+### profile: whether to enable profiling for the algorithm. (Optional)
 
 <ul>
 <li>Data Type: Boolean</li>
 <li>Default Value: False</li>
 <li>Meaning: disable/enable profiling. If enabled the function return a 3-tuple: (Y, t, g), where Y is the embedding coordinates, t are the execution times of each module per iteration (size 6 x max_iter) and g contains the grid size, the embedding domain size (maximum(Y) - minimum(Y)), and the scaling factor s_k for the band-limited version, per dimension (size 3 x max_iter).</li>
 </ul>
 
-###np: number of threads (set to 0 to use all available cores) (Optional)
+### np: number of threads (set to 0 to use all available cores) (Optional)
 
 <ul>
 <li>Data Type: Integer</li>
 <li>Default Value: threading.active_count(), which returns the number of active threads in the current process.</li>
 </ul>
 
-###h: grid side length (Optional)
+### h: grid side length (Optional)
 
 <ul>
 <li>Data Type: Float</li>
 <li>Default Value: 1.0</li>
 </ul>
 
-###u: either perplexity or value of λ (Optional)
+### u: either perplexity or value of λ (Optional)
 
 <ul>
 <li>Data Type: Integer</li>
 <li>Default Value: 10</li>
 </ul>
 
-###k: number of nearest neighbors (for kNN formation) (Optional)
+### k: number of nearest neighbors (for kNN formation) (Optional)
 
 <ul>
 <li>Data Type: Integer</li>
 <li>Default Value: 30</li>
 </ul>
 
-###eta: learning parameter (Optional)
+### eta: learning parameter (Optional)
 
 <ul>
 <li>Data Type: Integer or Float</li>
 <li>Default Value: 200.0</li>
 </ul>
 
-###alpha: exaggeration strength (applicable for first early_exag iterations). (Optional)
+### alpha: exaggeration strength (applicable for first early_exag iterations). (Optional)
 
 <ul>
 <li>Data Type: Integer or Float</li>
 <li>Default Value: 12</li>
 </ul>
 
-###fftw_single: Whether to use single-precision FFTW (Fast Fourier Transform) library. (Optional)
+### fftw_single: Whether to use single-precision FFTW (Fast Fourier Transform) library. (Optional)
 
 <ul>
 <li>Data Type: Boolean</li>
 <li>Default Value: False</li>
 </ul>
 
-###drop_leaf: remove edges connecting to leaf nodes. (Optional)
+### drop_leaf: remove edges connecting to leaf nodes. (Optional)
 
 <ul>
 <li>Data Type: Boolean</li>
 <li>Default Value: False</li>
 </ul>
 
-###list_grid_size: the list of allowed grid size along each dimension. (Optional)
+### list_grid_size: the list of allowed grid size along each dimension. (Optional)
 
 <ul>
 <li>Data Type: A list of integers</li>
 <li>Default Value: False.</li>
 <li>Affects FFT performance; most efficient if the size is a product of small primes. </li>
 </ul>
 
 **Warning:** 
 
 Because there is currently no replacement for Enum type in SGtSNEpy, we are missing the reduction of parameter you can change in Julia: **version**. Thus, the value will be its default value in Python.
 
-###version: the version of the algorithm for computing repulsive terms. (Optional)
+### version: the version of the algorithm for computing repulsive terms. (Optional)
 
 <ul>
 <li>Data Type: Enum (Julia)</li>
 <li>Default Value: NUCONV_BL</li>
 <li>Options are:
 </ul>
 <li>SGtSNEpi.NUCONV_BL (default): band-limited, approximated via non-uniform convolution</li>
 <li>SGtSNEpi.NUCONV: approximated via non-uniform convolution (higher resolution than SGtSNEpi.NUCONV_BL, slower execution time)</li>
 <li>SGtSNEpi.EXACT: no approximation; quadratic complexity, use only with small datasets</li>
 </ul>
 
-##Returns
+## Returns
 
 - Data Type: **numpy.ndarray** with three arrays: **numpy.int32, numpy.int32, numpy.float4**
 
-##Examples
+## Examples
 Here is an example to use function sgtsnepipy to generate a 2D embedding of an ER model.
 You have to use import networkx to generate a ER graph and matplotlib to visualize the embedding
 
 
 ```
     from SGtSNEpiPy.SGtSNEpiPy import sgtsnepipy
     import networkx as nx
@@ -216,22 +216,22 @@
     plt.colorbar(label='Node degree')
     plt.title("2D embedding of ER model (n = 1000, p = 0.2, seed = 170)")
 
     plt.show()
 ```
 
 
-##Contact
+## Contact
 
 Chenshuhao(Cody) Qin: chenshuhao.qin@duke.edu
 
 Yihua(Aaron) Zhong: yihua.zhong@duke.edu
 
 
-##Citation
+## Citation
 
 - Nikos Pitsianis, Alexandros-Stavros Iliopoulos, Dimitris Floros, Xiaobai Sun, **[Spaceland Embedding of Sparse Stochastic Graphs](https://doi.org/10.1109/HPEC.2019.8916505)**, In IEEE High Performance Extreme Computing Conference, 2019.
 - Nikos Pitsianis, Dimitris Floros, Alexandros-Stavros Iliopoulos, Xiaobai Sun, **[SG-t-SNE-Π: Swift Neighbor Embedding of Sparse Stochastic Graphs](https://doi.org/10.21105/joss.01577)**, Journal of Open Source Software, 4(39), 1577, 2019.
 
 If you use this software, please cite the following paper.
 
 ```
```

### Comparing `SGtSNEpiPy-1.1.3/setup.py` & `SGtSNEpiPy-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 with open("readme.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='SGtSNEpiPy',
-    version='1.1.3',
+    version='1.1.4',
     description='SGtSNEpiPy is a Python interface to SG-t-SNE-П, a powerful tool for visualizing large, sparse, stochastic graphs.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author=['Chenshuhao Qin','Yihua Zhong'],
     author_email="cq27@duke.edu, yz737@duke.edu,",
     classifiers=[
                 'Programming Language :: Python',
```

### Comparing `SGtSNEpiPy-1.1.3/src/SGtSNEpiPy/SGtSNEpiPy.py` & `SGtSNEpiPy-1.1.4/src/SGtSNEpiPy/SGtSNEpiPy.py`

 * *Files identical despite different names*

### Comparing `SGtSNEpiPy-1.1.3/src/SGtSNEpiPy.egg-info/PKG-INFO` & `SGtSNEpiPy-1.1.4/src/SGtSNEpiPy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SGtSNEpiPy
-Version: 1.1.3
+Version: 1.1.4
 Summary: SGtSNEpiPy is a Python interface to SG-t-SNE-П, a powerful tool for visualizing large, sparse, stochastic graphs.
 Author: ['Chenshuhao Qin', 'Yihua Zhong']
 Author-email: cq27@duke.edu, yz737@duke.edu,
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
 
@@ -42,162 +42,162 @@
 **Note**: The rest of the content remains unchanged as it does not contain any reST-specific elements.
 
 
 See **[the full documentation](https://fcdimitr.github.io/SGtSNEpi.jl/stable)** for moredetails.
 
 
 
-##Parameters
+## Parameters
 
 **SGtSNEpiPy.SGtSNEpiPy.sgtsnepipy**
 
 This package only has one method currently.
 
 
 ```
     sgtsnepi(A)
 ```
 
 
-###A: the input CSR sparse matrix representing the data points' pairwise similarities. (Mandatory)
+### A: the input CSR sparse matrix representing the data points' pairwise similarities. (Mandatory)
 
 <ul>
 <li>Data Type: **scipy.sparse.csr.csr_matrix** (The matrix includes row, value, value, whose type are all **numpy.ndarray** with three arrays of **numpy.int32, numpy.int32, numpy.int64**)</li>
 <li>A CSR sparse matrix generated by package scipy.</li>
 </ul>
 
-###d: the number of dimensions of the embedding space. (Optional)
+### d: the number of dimensions of the embedding space. (Optional)
 
 <ul>
 <li>Data Type: Integer</li>
 <li>Default Value: 2</li>
 </ul>
 
-###λ: SG-t-SNE scaling factor. (Optional)
+### λ: SG-t-SNE scaling factor. (Optional)
 
 <ul>
 <li>Data Type: Integer or Float</li>
 <li>Default Value: 10</li>
 </ul>
 
-###max_iter: the maximum number of iterations for the optimization process. (Optional)
+### max_iter: the maximum number of iterations for the optimization process. (Optional)
 
 <ul>
 <li>Data Type: Integer</li>
 <li>Default Value: 1000</li>
 </ul>
 
-###early_exag: the number of early exageration iterations. (Optional)
+### early_exag: the number of early exageration iterations. (Optional)
 
 <ul>
 <li>Data Type: Integer</li>
 <li>Default Value: 250</li>
 </ul>
 
-###Y0: initial distribution in embedding space (randomly generated if nothing).(Optional)
+### Y0: initial distribution in embedding space (randomly generated if nothing).(Optional)
 
 <ul>
 <li>Data Type: A numpy array of shape (number of data points, d).</li>
 <li>Default Value: None</li>
 <li>You should set this parameter to generate reproducible results.</li>
 </ul>
 
-###profile: whether to enable profiling for the algorithm. (Optional)
+### profile: whether to enable profiling for the algorithm. (Optional)
 
 <ul>
 <li>Data Type: Boolean</li>
 <li>Default Value: False</li>
 <li>Meaning: disable/enable profiling. If enabled the function return a 3-tuple: (Y, t, g), where Y is the embedding coordinates, t are the execution times of each module per iteration (size 6 x max_iter) and g contains the grid size, the embedding domain size (maximum(Y) - minimum(Y)), and the scaling factor s_k for the band-limited version, per dimension (size 3 x max_iter).</li>
 </ul>
 
-###np: number of threads (set to 0 to use all available cores) (Optional)
+### np: number of threads (set to 0 to use all available cores) (Optional)
 
 <ul>
 <li>Data Type: Integer</li>
 <li>Default Value: threading.active_count(), which returns the number of active threads in the current process.</li>
 </ul>
 
-###h: grid side length (Optional)
+### h: grid side length (Optional)
 
 <ul>
 <li>Data Type: Float</li>
 <li>Default Value: 1.0</li>
 </ul>
 
-###u: either perplexity or value of λ (Optional)
+### u: either perplexity or value of λ (Optional)
 
 <ul>
 <li>Data Type: Integer</li>
 <li>Default Value: 10</li>
 </ul>
 
-###k: number of nearest neighbors (for kNN formation) (Optional)
+### k: number of nearest neighbors (for kNN formation) (Optional)
 
 <ul>
 <li>Data Type: Integer</li>
 <li>Default Value: 30</li>
 </ul>
 
-###eta: learning parameter (Optional)
+### eta: learning parameter (Optional)
 
 <ul>
 <li>Data Type: Integer or Float</li>
 <li>Default Value: 200.0</li>
 </ul>
 
-###alpha: exaggeration strength (applicable for first early_exag iterations). (Optional)
+### alpha: exaggeration strength (applicable for first early_exag iterations). (Optional)
 
 <ul>
 <li>Data Type: Integer or Float</li>
 <li>Default Value: 12</li>
 </ul>
 
-###fftw_single: Whether to use single-precision FFTW (Fast Fourier Transform) library. (Optional)
+### fftw_single: Whether to use single-precision FFTW (Fast Fourier Transform) library. (Optional)
 
 <ul>
 <li>Data Type: Boolean</li>
 <li>Default Value: False</li>
 </ul>
 
-###drop_leaf: remove edges connecting to leaf nodes. (Optional)
+### drop_leaf: remove edges connecting to leaf nodes. (Optional)
 
 <ul>
 <li>Data Type: Boolean</li>
 <li>Default Value: False</li>
 </ul>
 
-###list_grid_size: the list of allowed grid size along each dimension. (Optional)
+### list_grid_size: the list of allowed grid size along each dimension. (Optional)
 
 <ul>
 <li>Data Type: A list of integers</li>
 <li>Default Value: False.</li>
 <li>Affects FFT performance; most efficient if the size is a product of small primes. </li>
 </ul>
 
 **Warning:** 
 
 Because there is currently no replacement for Enum type in SGtSNEpy, we are missing the reduction of parameter you can change in Julia: **version**. Thus, the value will be its default value in Python.
 
-###version: the version of the algorithm for computing repulsive terms. (Optional)
+### version: the version of the algorithm for computing repulsive terms. (Optional)
 
 <ul>
 <li>Data Type: Enum (Julia)</li>
 <li>Default Value: NUCONV_BL</li>
 <li>Options are:
 </ul>
 <li>SGtSNEpi.NUCONV_BL (default): band-limited, approximated via non-uniform convolution</li>
 <li>SGtSNEpi.NUCONV: approximated via non-uniform convolution (higher resolution than SGtSNEpi.NUCONV_BL, slower execution time)</li>
 <li>SGtSNEpi.EXACT: no approximation; quadratic complexity, use only with small datasets</li>
 </ul>
 
-##Returns
+## Returns
 
 - Data Type: **numpy.ndarray** with three arrays: **numpy.int32, numpy.int32, numpy.float4**
 
-##Examples
+## Examples
 Here is an example to use function sgtsnepipy to generate a 2D embedding of an ER model.
 You have to use import networkx to generate a ER graph and matplotlib to visualize the embedding
 
 
 ```
     from SGtSNEpiPy.SGtSNEpiPy import sgtsnepipy
     import networkx as nx
@@ -226,22 +226,22 @@
     plt.colorbar(label='Node degree')
     plt.title("2D embedding of ER model (n = 1000, p = 0.2, seed = 170)")
 
     plt.show()
 ```
 
 
-##Contact
+## Contact
 
 Chenshuhao(Cody) Qin: chenshuhao.qin@duke.edu
 
 Yihua(Aaron) Zhong: yihua.zhong@duke.edu
 
 
-##Citation
+## Citation
 
 - Nikos Pitsianis, Alexandros-Stavros Iliopoulos, Dimitris Floros, Xiaobai Sun, **[Spaceland Embedding of Sparse Stochastic Graphs](https://doi.org/10.1109/HPEC.2019.8916505)**, In IEEE High Performance Extreme Computing Conference, 2019.
 - Nikos Pitsianis, Dimitris Floros, Alexandros-Stavros Iliopoulos, Xiaobai Sun, **[SG-t-SNE-Π: Swift Neighbor Embedding of Sparse Stochastic Graphs](https://doi.org/10.21105/joss.01577)**, Journal of Open Source Software, 4(39), 1577, 2019.
 
 If you use this software, please cite the following paper.
 
 ```
```

