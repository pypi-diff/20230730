# Comparing `tmp/brc-0.1.1.tar.gz` & `tmp/brc-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/brc-0.1.1.tar", last modified: Tue Jun  1 12:07:07 2021, max compression
+gzip compressed data, was "brc-0.1.2.tar", last modified: Sat Jul 29 21:58:50 2023, max compression
```

## Comparing `brc-0.1.1.tar` & `brc-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxr-x   0 kristian  (1000) kristian  (1000)        0 2021-06-01 12:07:07.521408 brc-0.1.1/
--rw-rw-r--   0 kristian  (1000) kristian  (1000)     2136 2021-06-01 12:07:07.521408 brc-0.1.1/PKG-INFO
--rw-rw-r--   0 kristian  (1000) kristian  (1000)     1338 2021-06-01 11:52:10.000000 brc-0.1.1/README.md
-drwxrwxr-x   0 kristian  (1000) kristian  (1000)        0 2021-06-01 12:07:07.521408 brc-0.1.1/brc.egg-info/
--rw-rw-r--   0 kristian  (1000) kristian  (1000)     2136 2021-06-01 12:07:07.000000 brc-0.1.1/brc.egg-info/PKG-INFO
--rw-rw-r--   0 kristian  (1000) kristian  (1000)      246 2021-06-01 12:07:07.000000 brc-0.1.1/brc.egg-info/SOURCES.txt
--rw-rw-r--   0 kristian  (1000) kristian  (1000)        1 2021-06-01 12:07:07.000000 brc-0.1.1/brc.egg-info/dependency_links.txt
--rw-rw-r--   0 kristian  (1000) kristian  (1000)        6 2021-06-01 12:07:07.000000 brc-0.1.1/brc.egg-info/requires.txt
--rw-rw-r--   0 kristian  (1000) kristian  (1000)       12 2021-06-01 12:07:07.000000 brc-0.1.1/brc.egg-info/top_level.txt
-drwxrwxr-x   0 kristian  (1000) kristian  (1000)        0 2021-06-01 12:07:07.521408 brc-0.1.1/brc_pytorch/
--rw-rw-r--   0 kristian  (1000) kristian  (1000)        0 2021-05-27 15:36:30.000000 brc-0.1.1/brc_pytorch/__init__.py
--rw-rw-r--   0 kristian  (1000) kristian  (1000)     2103 2021-06-01 10:07:29.000000 brc-0.1.1/brc_pytorch/benchmarks.py
--rw-rw-r--   0 kristian  (1000) kristian  (1000)     8790 2021-06-01 11:47:31.000000 brc-0.1.1/brc_pytorch/modules.py
--rw-rw-r--   0 kristian  (1000) kristian  (1000)      689 2021-05-31 15:36:52.000000 brc-0.1.1/brc_pytorch/utils.py
--rw-rw-r--   0 kristian  (1000) kristian  (1000)       38 2021-06-01 12:07:07.521408 brc-0.1.1/setup.cfg
--rw-rw-r--   0 kristian  (1000) kristian  (1000)      615 2021-06-01 12:06:44.000000 brc-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:58:50.094957 brc-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-29 21:58:50.094957 brc-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-29 21:58:40.000000 brc-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:58:50.094957 brc-0.1.2/brc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-29 21:58:50.000000 brc-0.1.2/brc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-29 21:58:50.000000 brc-0.1.2/brc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 21:58:50.000000 brc-0.1.2/brc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 21:58:50.000000 brc-0.1.2/brc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-29 21:58:50.000000 brc-0.1.2/brc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:58:50.094957 brc-0.1.2/brc_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 21:58:40.000000 brc-0.1.2/brc_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-29 21:58:40.000000 brc-0.1.2/brc_pytorch/benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-07-29 21:58:40.000000 brc-0.1.2/brc_pytorch/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-29 21:58:40.000000 brc-0.1.2/brc_pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 21:58:50.094957 brc-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-29 21:58:40.000000 brc-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:58:50.094957 brc-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-07-29 21:58:40.000000 brc-0.1.2/tests/test_modules.py
```

### Comparing `brc-0.1.1/PKG-INFO` & `brc-0.1.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,66 +1,76 @@
 Metadata-Version: 2.1
 Name: brc
-Version: 0.1.1
+Version: 0.1.2
 Summary: Implementation of the bistable recurrent cell (BRC) in PyTorch
 Home-page: https://github.com/kklemon/brc-pytorch
 Author: Kristian Klemon
 Author-email: kristian.klemon@gmail.com
 License: MIT
-Description: brc-pytorch
-        ===========
-        
-        PyTorch implementation of the bistable recurrent cell (BRC) from the paper _A bio-inspired bistable recurrent cell allows for
-        long-lasting memory_ (Vecoven et al., 2020).
-        
-        ![](./figs/neuron.png)
-        
-        Install
-        -------
-        
-        ```bash
-        pip install brc-pytorch
-        ```
-        
-        Usage
-        -----
-        
-        ```python
-        import torch
-        from brc_pytorch.modules import BRC, NBRC, StackedRNN
-        
-        brc = StackedRNN(
-            cell=BRC,  # NBRC for the neuromodulated version
-            input_size=128,
-            hidden_size=256,
-            num_layers=3
-        )
-        
-        # [ seq_len, batch_size, dim ]
-        x = torch.randn(64, 32, 128)
-        
-        init_hidden = brc.init_hidden(batch_size=32)
-        out, hidden = brc(x, init_hidden)
-        ```
-        
-        Performance
-        -----------
-        
-        The implementation is provided in TorchScript and makes use of the PyTorch JIT compiler.
-        In my not really statistically significant experiments, the implementation seems to be about half as fast as the cuDNN based reference LSTM implementation with modest batch sizes and sequence lengths which can be considered pretty solid for a non-CUDA implementation.
-        
-        References
-        ----------
-        
-        ```bibtex
-        @misc{vecoven2020bioinspired,
-            title={A bio-inspired bistable recurrent cell allows for long-lasting memory},
-            author={Nicolas Vecoven and Damien Ernst and Guillaume Drion},
-            year={2020},
-            eprint={2006.05252},
-            archivePrefix={arXiv},
-            primaryClass={cs.NE}
-        }
-        ```
 Keywords: artificial intelligence,deep learning
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+
+brc-pytorch
+===========
+
+PyTorch implementation of the bistable recurrent cell (BRC) from the paper [_A bio-inspired bistable recurrent cell allows for
+long-lasting memory_ (Vecoven et al., 2020)](https://arxiv.org/abs/2006.05252).
+
+![](./figs/neuron.png)
+
+Install
+-------
+
+```bash
+pip install brc-pytorch
+```
+
+Usage
+-----
+
+```python
+import torch
+
+from brc_pytorch import utils
+from brc_pytorch.modules import BRC, NBRC, StackedRNN
+
+brc = StackedRNN(
+    cell=BRC,  # NBRC for the neuromodulated version
+    input_size=128,
+    hidden_size=256,
+    num_layers=3
+).cuda()
+
+# [ seq_len, batch_size, dim ]
+x = torch.randn(64, 32, 128).cuda()
+
+init_hidden = brc.init_hidden(batch_size=32)
+out, hidden = brc(x, init_hidden)
+
+# Detach hidden for next call
+hidden = utils.detach_hidden(hidden)
+```
+
+Performance
+-----------
+
+The implementation is written in TorchScript (a subset of Python) and makes use of the PyTorch JIT compiler for a more efficient execution.
+
+In my not really statistically significant experiments, the implementation seems to be about half as fast as the cuDNN based reference LSTM implementation with modest batch sizes and sequence lengths which can be considered pretty solid for a non-CUDA implementation.
+
+**Update (2023/07)**
+
+A lot has happened since the last real update of this repository. [PyTorch 2.0](https://pytorch.org/blog/pytorch-2.0-release/) has introduced a new dynamic compilation system, which, to my understanding, should replace the old scripting API. After doing a quick test, it seems that the code is still working without issues with the scripting API and can in principle also be compiled with `torch.compile`. However, it does not seem to run faster, perhaps even slower, and would need an adaption to the new compilation system.
+
+References
+----------
+
+```bibtex
+@misc{vecoven2020bioinspired,
+    title={A bio-inspired bistable recurrent cell allows for long-lasting memory},
+    author={Nicolas Vecoven and Damien Ernst and Guillaume Drion},
+    year={2020},
+    eprint={2006.05252},
+    archivePrefix={arXiv},
+    primaryClass={cs.NE}
+}
+```
```

### Comparing `brc-0.1.1/brc.egg-info/PKG-INFO` & `brc-0.1.2/brc.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,66 +1,76 @@
 Metadata-Version: 2.1
 Name: brc
-Version: 0.1.1
+Version: 0.1.2
 Summary: Implementation of the bistable recurrent cell (BRC) in PyTorch
 Home-page: https://github.com/kklemon/brc-pytorch
 Author: Kristian Klemon
 Author-email: kristian.klemon@gmail.com
 License: MIT
-Description: brc-pytorch
-        ===========
-        
-        PyTorch implementation of the bistable recurrent cell (BRC) from the paper _A bio-inspired bistable recurrent cell allows for
-        long-lasting memory_ (Vecoven et al., 2020).
-        
-        ![](./figs/neuron.png)
-        
-        Install
-        -------
-        
-        ```bash
-        pip install brc-pytorch
-        ```
-        
-        Usage
-        -----
-        
-        ```python
-        import torch
-        from brc_pytorch.modules import BRC, NBRC, StackedRNN
-        
-        brc = StackedRNN(
-            cell=BRC,  # NBRC for the neuromodulated version
-            input_size=128,
-            hidden_size=256,
-            num_layers=3
-        )
-        
-        # [ seq_len, batch_size, dim ]
-        x = torch.randn(64, 32, 128)
-        
-        init_hidden = brc.init_hidden(batch_size=32)
-        out, hidden = brc(x, init_hidden)
-        ```
-        
-        Performance
-        -----------
-        
-        The implementation is provided in TorchScript and makes use of the PyTorch JIT compiler.
-        In my not really statistically significant experiments, the implementation seems to be about half as fast as the cuDNN based reference LSTM implementation with modest batch sizes and sequence lengths which can be considered pretty solid for a non-CUDA implementation.
-        
-        References
-        ----------
-        
-        ```bibtex
-        @misc{vecoven2020bioinspired,
-            title={A bio-inspired bistable recurrent cell allows for long-lasting memory},
-            author={Nicolas Vecoven and Damien Ernst and Guillaume Drion},
-            year={2020},
-            eprint={2006.05252},
-            archivePrefix={arXiv},
-            primaryClass={cs.NE}
-        }
-        ```
 Keywords: artificial intelligence,deep learning
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+
+brc-pytorch
+===========
+
+PyTorch implementation of the bistable recurrent cell (BRC) from the paper [_A bio-inspired bistable recurrent cell allows for
+long-lasting memory_ (Vecoven et al., 2020)](https://arxiv.org/abs/2006.05252).
+
+![](./figs/neuron.png)
+
+Install
+-------
+
+```bash
+pip install brc-pytorch
+```
+
+Usage
+-----
+
+```python
+import torch
+
+from brc_pytorch import utils
+from brc_pytorch.modules import BRC, NBRC, StackedRNN
+
+brc = StackedRNN(
+    cell=BRC,  # NBRC for the neuromodulated version
+    input_size=128,
+    hidden_size=256,
+    num_layers=3
+).cuda()
+
+# [ seq_len, batch_size, dim ]
+x = torch.randn(64, 32, 128).cuda()
+
+init_hidden = brc.init_hidden(batch_size=32)
+out, hidden = brc(x, init_hidden)
+
+# Detach hidden for next call
+hidden = utils.detach_hidden(hidden)
+```
+
+Performance
+-----------
+
+The implementation is written in TorchScript (a subset of Python) and makes use of the PyTorch JIT compiler for a more efficient execution.
+
+In my not really statistically significant experiments, the implementation seems to be about half as fast as the cuDNN based reference LSTM implementation with modest batch sizes and sequence lengths which can be considered pretty solid for a non-CUDA implementation.
+
+**Update (2023/07)**
+
+A lot has happened since the last real update of this repository. [PyTorch 2.0](https://pytorch.org/blog/pytorch-2.0-release/) has introduced a new dynamic compilation system, which, to my understanding, should replace the old scripting API. After doing a quick test, it seems that the code is still working without issues with the scripting API and can in principle also be compiled with `torch.compile`. However, it does not seem to run faster, perhaps even slower, and would need an adaption to the new compilation system.
+
+References
+----------
+
+```bibtex
+@misc{vecoven2020bioinspired,
+    title={A bio-inspired bistable recurrent cell allows for long-lasting memory},
+    author={Nicolas Vecoven and Damien Ernst and Guillaume Drion},
+    year={2020},
+    eprint={2006.05252},
+    archivePrefix={arXiv},
+    primaryClass={cs.NE}
+}
+```
```

### Comparing `brc-0.1.1/brc_pytorch/benchmarks.py` & `brc-0.1.2/brc_pytorch/benchmarks.py`

 * *Files identical despite different names*

### Comparing `brc-0.1.1/brc_pytorch/modules.py` & `brc-0.1.2/brc_pytorch/modules.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         with torch.no_grad():
             nn.init.xavier_uniform_(self.iw)
             self.hw.fill_(1.0)
             if self.bias is not None:
                 self.bias.zero_()
 
     def init_hidden(self, batch_size: int):
-        return [torch.zeros(batch_size, self.hidden_size)]
+        return [torch.zeros(batch_size, self.hidden_size, device=self.hw.device)]
 
     def get_hidden_activation(self, hidden: Tensor) -> List[Tensor]:
         return (torch.cat([hidden, hidden], dim=-1) * self.hw).chunk(2, dim=-1)
 
     @torch.jit.script_method
     def forward(self, input: Tensor, hidden: List[Tensor]) -> Tuple[Tensor, List[Tensor]]:
         hx, = hidden
@@ -97,18 +97,15 @@
         with torch.no_grad():
             for weight in [self.iw, self.hw]:
                 nn.init.xavier_uniform_(weight)
             if self.bias is not None:
                 self.bias.zero_()
 
     def init_hidden(self, batch_size: int):
-        return [
-            torch.zeros(batch_size, self.hidden_size),
-            torch.zeros(batch_size, self.hidden_size)
-        ]
+        return list(torch.zeros(2, batch_size, self.hidden_size, device=self.iw.device))
 
     @torch.jit.script_method
     def forward(self, input: Tensor, hidden: List[Tensor]) -> Tuple[Tensor, List[Tensor]]:
         hx, cx = hidden
         gates = (input @ self.iw) + (hx @ self.hw)
         if self.bias is not None:
             gates += self.bias
@@ -141,15 +138,15 @@
         with torch.no_grad():
             for weight in [self.iw, self.hw, self.rw]:
                 nn.init.xavier_uniform_(weight)
             if self.bias is not None:
                 self.bias.zero_()
 
     def init_hidden(self, batch_size: int):
-        return [torch.zeros(batch_size, self.hidden_size)]
+        return [torch.zeros(batch_size, self.hidden_size, device=self.iw.device)]
 
     @torch.jit.script_method
     def forward(self, input: Tensor, hidden: List[Tensor]) -> Tuple[Tensor, List[Tensor]]:
         hx, = hidden
 
         x = (input @ self.iw)
         if self.bias is not None:
```

### Comparing `brc-0.1.1/brc_pytorch/utils.py` & `brc-0.1.2/brc_pytorch/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     return nested_apply(lambda t: t.to(device), whatever)
 
 
 def to_batch_first(whatever):
     return nested_apply(lambda t: t.transpose(0, 1) if t.ndim > 2 else t, whatever)
 
 
-def repackage_hidden(hidden):
+def detach_hidden(hidden):
     return nested_apply(lambda t: t.clone().detach(), hidden)
 
 
 def split(l: List, fractions: List[float]):
     assert sum(fractions) == 1
     n = len(l)
     return [l[round(n * sum(fractions[:i])):round(n * sum(fractions[:i + 1]))] for i in range(len(fractions))]
```

