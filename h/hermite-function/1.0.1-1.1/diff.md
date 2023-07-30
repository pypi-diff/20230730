# Comparing `tmp/hermite-function-1.0.1.tar.gz` & `tmp/hermite-function-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hermite-function-1.0.1.tar", last modified: Sun Jul 30 21:13:31 2023, max compression
+gzip compressed data, was "hermite-function-1.1.tar", last modified: Sun Jul 30 21:16:19 2023, max compression
```

## Comparing `hermite-function-1.0.1.tar` & `hermite-function-1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 goessl     (501) staff       (20)        0 2023-07-30 21:13:31.981893 hermite-function-1.0.1/
--rw-r--r--   0 goessl     (501) staff       (20)     1073 2023-07-27 01:16:40.000000 hermite-function-1.0.1/LICENSE
--rw-r--r--   0 goessl     (501) staff       (20)     5214 2023-07-30 21:13:31.981794 hermite-function-1.0.1/PKG-INFO
--rw-r--r--   0 goessl     (501) staff       (20)     4746 2023-07-27 01:16:40.000000 hermite-function-1.0.1/README.md
-drwxr-xr-x   0 goessl     (501) staff       (20)        0 2023-07-30 21:13:31.981638 hermite-function-1.0.1/hermite_function.egg-info/
--rw-r--r--   0 goessl     (501) staff       (20)     5214 2023-07-30 21:13:31.000000 hermite-function-1.0.1/hermite_function.egg-info/PKG-INFO
--rw-r--r--   0 goessl     (501) staff       (20)      244 2023-07-30 21:13:31.000000 hermite-function-1.0.1/hermite_function.egg-info/SOURCES.txt
--rw-r--r--   0 goessl     (501) staff       (20)        1 2023-07-30 21:13:31.000000 hermite-function-1.0.1/hermite_function.egg-info/dependency_links.txt
--rw-r--r--   0 goessl     (501) staff       (20)       12 2023-07-30 21:13:31.000000 hermite-function-1.0.1/hermite_function.egg-info/requires.txt
--rw-r--r--   0 goessl     (501) staff       (20)       16 2023-07-30 21:13:31.000000 hermite-function-1.0.1/hermite_function.egg-info/top_level.txt
--rw-r--r--   0 goessl     (501) staff       (20)     4541 2023-07-27 01:16:40.000000 hermite-function-1.0.1/hermitefunction.py
--rw-r--r--   0 goessl     (501) staff       (20)       38 2023-07-30 21:13:31.981927 hermite-function-1.0.1/setup.cfg
--rw-r--r--   0 goessl     (501) staff       (20)      819 2023-07-30 21:13:02.000000 hermite-function-1.0.1/setup.py
+drwxr-xr-x   0 goessl     (501) staff       (20)        0 2023-07-30 21:16:19.299620 hermite-function-1.1/
+-rw-r--r--   0 goessl     (501) staff       (20)     1073 2023-07-30 12:11:14.000000 hermite-function-1.1/LICENSE
+-rw-r--r--   0 goessl     (501) staff       (20)     6163 2023-07-30 21:16:19.299519 hermite-function-1.1/PKG-INFO
+-rw-r--r--   0 goessl     (501) staff       (20)     5697 2023-07-30 12:11:14.000000 hermite-function-1.1/README.md
+drwxr-xr-x   0 goessl     (501) staff       (20)        0 2023-07-30 21:16:19.299367 hermite-function-1.1/hermite_function.egg-info/
+-rw-r--r--   0 goessl     (501) staff       (20)     6163 2023-07-30 21:16:19.000000 hermite-function-1.1/hermite_function.egg-info/PKG-INFO
+-rw-r--r--   0 goessl     (501) staff       (20)      244 2023-07-30 21:16:19.000000 hermite-function-1.1/hermite_function.egg-info/SOURCES.txt
+-rw-r--r--   0 goessl     (501) staff       (20)        1 2023-07-30 21:16:19.000000 hermite-function-1.1/hermite_function.egg-info/dependency_links.txt
+-rw-r--r--   0 goessl     (501) staff       (20)       12 2023-07-30 21:16:19.000000 hermite-function-1.1/hermite_function.egg-info/requires.txt
+-rw-r--r--   0 goessl     (501) staff       (20)       16 2023-07-30 21:16:19.000000 hermite-function-1.1/hermite_function.egg-info/top_level.txt
+-rw-r--r--   0 goessl     (501) staff       (20)     5198 2023-07-30 12:11:14.000000 hermite-function-1.1/hermitefunction.py
+-rw-r--r--   0 goessl     (501) staff       (20)       38 2023-07-30 21:16:19.299654 hermite-function-1.1/setup.cfg
+-rw-r--r--   0 goessl     (501) staff       (20)      817 2023-07-30 21:16:12.000000 hermite-function-1.1/setup.py
```

### Comparing `hermite-function-1.0.1/LICENSE` & `hermite-function-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hermite-function-1.0.1/PKG-INFO` & `hermite-function-1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hermite-function
-Version: 1.0.1
+Version: 1.1
 Summary: A Hermite function series module.
 Home-page: https://github.com/goessl/hermite-function
 Author: Sebastian Gössl
 Author-email: goessl@student.tugraz.at
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
@@ -127,12 +127,36 @@
         &= \sum_{k=0}^\infty \sqrt{\frac{k+1}{2}}f_{k+1} h_k - \sum_{k=0}^\infty \sqrt{\frac{k}{2}}f_{k-1} h_k \\
         &= \sum_k \left( \sqrt{\frac{k+1}{2}}f_{k+1} - \sqrt{\frac{k}{2}}f_{k-1} \right) h_k
     \end{aligned}
 $$
 
 With $h'\_k=\sqrt{\frac{k}{2}}h_{k+1}-\sqrt{\frac{k+1}{2}}h_{k-1}$ from [Wikipedia - Hermite functions](https://en.wikipedia.org/wiki/Hermite_polynomials\#Hermite_functions).
 
+### Integration
+
+With the same relation as above we get
+
+$$
+    \begin{aligned}
+        h_k' &= \sqrt{\frac{k}{2}}h_{k-1} - \sqrt{\frac{k+1}{2}}h_{k+1} \\
+        &\qquad\mid +\sqrt{\frac{k+1}{2}}h_{k+1} - h_k' \\
+        \sqrt{\frac{k+1}{2}}h_{k+1} &= \sqrt{\frac{k}{2}}h_{k-1} - h_k' \\
+        &\qquad\mid \cdot\sqrt{\frac{2}{k+1}} \\
+        h_{k+1} &= \sqrt{\frac{k}{k+1}}h_{k-1} - \sqrt{\frac{2}{k+1}}h_k' \\
+        &\qquad\mid k+1 \to k \\
+        h_k &= \sqrt{\frac{k-1}{k}}h_{k-2} - \sqrt{\frac{2}{k}}h_{k-1}' \\
+        &\qquad\mid \int \\
+        H_k &= \sqrt{\frac{k-1}{k}}H_{k-2} - \sqrt{\frac{2}{k}}h_{k-1}
+    \end{aligned}
+$$
+
+which can be applied from the highest to the lowest order. For $h_0$ we then get
+
+$$
+    H_0(x) = \int_{-\infty}^xh_0(x')dx' = \int_{-\infty}^x\frac{e^{-\frac{x'^2}{2}}}{\sqrt[4]{\pi}}dx' = \sqrt{\frac{\sqrt{\pi}}{2}}\text{erf}\left(\frac{x}{\sqrt{2}}\right) \ \left(+\sqrt{\frac{\sqrt{\pi}}{2}}\right)
+$$
+
 ### Kinetic energy
 
 $$
     \left\langle\frac{-\hat{P}^2}{2}\right\rangle = -\frac{1}{2}\int_{\mathbb{R}}f^*(x)\frac{d^2}{dx^2}f(x)dx = +\frac{1}{2}\int_{\mathbb{R}}|f'(x)|^2dx = \frac{1}{2}||f'||\_{L_{\mathbb{R}}^2}^2
 $$
```

### Comparing `hermite-function-1.0.1/README.md` & `hermite-function-1.1/hermite_function.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: hermite-function
+Version: 1.1
+Summary: A Hermite function series module.
+Home-page: https://github.com/goessl/hermite-function
+Author: Sebastian Gössl
+Author-email: goessl@student.tugraz.at
+License: MIT
+Classifier: Programming Language :: Python :: 3.7
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Hermite Function Series
 
 A Hermite function series package.
 ```python
 from hermitefunction import HermiteFunction
 import numpy as np
 import matplotlib.pyplot as plt
@@ -112,12 +127,36 @@
         &= \sum_{k=0}^\infty \sqrt{\frac{k+1}{2}}f_{k+1} h_k - \sum_{k=0}^\infty \sqrt{\frac{k}{2}}f_{k-1} h_k \\
         &= \sum_k \left( \sqrt{\frac{k+1}{2}}f_{k+1} - \sqrt{\frac{k}{2}}f_{k-1} \right) h_k
     \end{aligned}
 $$
 
 With $h'\_k=\sqrt{\frac{k}{2}}h_{k+1}-\sqrt{\frac{k+1}{2}}h_{k-1}$ from [Wikipedia - Hermite functions](https://en.wikipedia.org/wiki/Hermite_polynomials\#Hermite_functions).
 
+### Integration
+
+With the same relation as above we get
+
+$$
+    \begin{aligned}
+        h_k' &= \sqrt{\frac{k}{2}}h_{k-1} - \sqrt{\frac{k+1}{2}}h_{k+1} \\
+        &\qquad\mid +\sqrt{\frac{k+1}{2}}h_{k+1} - h_k' \\
+        \sqrt{\frac{k+1}{2}}h_{k+1} &= \sqrt{\frac{k}{2}}h_{k-1} - h_k' \\
+        &\qquad\mid \cdot\sqrt{\frac{2}{k+1}} \\
+        h_{k+1} &= \sqrt{\frac{k}{k+1}}h_{k-1} - \sqrt{\frac{2}{k+1}}h_k' \\
+        &\qquad\mid k+1 \to k \\
+        h_k &= \sqrt{\frac{k-1}{k}}h_{k-2} - \sqrt{\frac{2}{k}}h_{k-1}' \\
+        &\qquad\mid \int \\
+        H_k &= \sqrt{\frac{k-1}{k}}H_{k-2} - \sqrt{\frac{2}{k}}h_{k-1}
+    \end{aligned}
+$$
+
+which can be applied from the highest to the lowest order. For $h_0$ we then get
+
+$$
+    H_0(x) = \int_{-\infty}^xh_0(x')dx' = \int_{-\infty}^x\frac{e^{-\frac{x'^2}{2}}}{\sqrt[4]{\pi}}dx' = \sqrt{\frac{\sqrt{\pi}}{2}}\text{erf}\left(\frac{x}{\sqrt{2}}\right) \ \left(+\sqrt{\frac{\sqrt{\pi}}{2}}\right)
+$$
+
 ### Kinetic energy
 
 $$
     \left\langle\frac{-\hat{P}^2}{2}\right\rangle = -\frac{1}{2}\int_{\mathbb{R}}f^*(x)\frac{d^2}{dx^2}f(x)dx = +\frac{1}{2}\int_{\mathbb{R}}|f'(x)|^2dx = \frac{1}{2}||f'||\_{L_{\mathbb{R}}^2}^2
 $$
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hermite-function-1.0.1/hermite_function.egg-info/PKG-INFO` & `hermite-function-1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: hermite-function
-Version: 1.0.1
-Summary: A Hermite function series module.
-Home-page: https://github.com/goessl/hermite-function
-Author: Sebastian Gössl
-Author-email: goessl@student.tugraz.at
-License: MIT
-Classifier: Programming Language :: Python :: 3.7
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Hermite Function Series
 
 A Hermite function series package.
 ```python
 from hermitefunction import HermiteFunction
 import numpy as np
 import matplotlib.pyplot as plt
@@ -127,12 +112,36 @@
         &= \sum_{k=0}^\infty \sqrt{\frac{k+1}{2}}f_{k+1} h_k - \sum_{k=0}^\infty \sqrt{\frac{k}{2}}f_{k-1} h_k \\
         &= \sum_k \left( \sqrt{\frac{k+1}{2}}f_{k+1} - \sqrt{\frac{k}{2}}f_{k-1} \right) h_k
     \end{aligned}
 $$
 
 With $h'\_k=\sqrt{\frac{k}{2}}h_{k+1}-\sqrt{\frac{k+1}{2}}h_{k-1}$ from [Wikipedia - Hermite functions](https://en.wikipedia.org/wiki/Hermite_polynomials\#Hermite_functions).
 
+### Integration
+
+With the same relation as above we get
+
+$$
+    \begin{aligned}
+        h_k' &= \sqrt{\frac{k}{2}}h_{k-1} - \sqrt{\frac{k+1}{2}}h_{k+1} \\
+        &\qquad\mid +\sqrt{\frac{k+1}{2}}h_{k+1} - h_k' \\
+        \sqrt{\frac{k+1}{2}}h_{k+1} &= \sqrt{\frac{k}{2}}h_{k-1} - h_k' \\
+        &\qquad\mid \cdot\sqrt{\frac{2}{k+1}} \\
+        h_{k+1} &= \sqrt{\frac{k}{k+1}}h_{k-1} - \sqrt{\frac{2}{k+1}}h_k' \\
+        &\qquad\mid k+1 \to k \\
+        h_k &= \sqrt{\frac{k-1}{k}}h_{k-2} - \sqrt{\frac{2}{k}}h_{k-1}' \\
+        &\qquad\mid \int \\
+        H_k &= \sqrt{\frac{k-1}{k}}H_{k-2} - \sqrt{\frac{2}{k}}h_{k-1}
+    \end{aligned}
+$$
+
+which can be applied from the highest to the lowest order. For $h_0$ we then get
+
+$$
+    H_0(x) = \int_{-\infty}^xh_0(x')dx' = \int_{-\infty}^x\frac{e^{-\frac{x'^2}{2}}}{\sqrt[4]{\pi}}dx' = \sqrt{\frac{\sqrt{\pi}}{2}}\text{erf}\left(\frac{x}{\sqrt{2}}\right) \ \left(+\sqrt{\frac{\sqrt{\pi}}{2}}\right)
+$$
+
 ### Kinetic energy
 
 $$
     \left\langle\frac{-\hat{P}^2}{2}\right\rangle = -\frac{1}{2}\int_{\mathbb{R}}f^*(x)\frac{d^2}{dx^2}f(x)dx = +\frac{1}{2}\int_{\mathbb{R}}|f'(x)|^2dx = \frac{1}{2}||f'||\_{L_{\mathbb{R}}^2}^2
 $$
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hermite-function-1.0.1/hermitefunction.py` & `hermite-function-1.1/hermitefunction.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 from numpy.polynomial.hermite import hermval, hermfit
-from scipy.special import factorial, binom
+from scipy.special import factorial, binom, erf
 from itertools import starmap, zip_longest
 import operator
 from functools import cached_property
 
 
 
 class HermiteFunction:
@@ -126,14 +126,30 @@
         """Returns the n-th derivative of this series."""
         res = self
         for _ in range(n):
             res = (np.sqrt((i+1)/2) for i in range(len(res)-1)) * (res<<1) \
                     - (np.sqrt(i/2) for i in range(len(res)+1)) * (res>>1)
         return res
     
+    def antider(self):
+        """Returns F, r so that the antiderivative of this series is of form
+        F(x) + r*HermiteFunction.zeroth_antiderivative(x)
+        where F is also a Hermite series."""
+        tmp = list(self)
+        F = (len(self)-1) * [0]
+        for i in reversed(range(1, len(self))):
+            F[i-1] -= tmp[i] * np.sqrt(2/i)
+            tmp[i-2] += tmp[i] * np.sqrt((i-1)/i)
+        return HermiteFunction(F), tmp[0]
+    
+    @staticmethod
+    def zeroth_antiderivative(x):
+        """Evaluation of the antiderivative of the zeroth Hermite function."""
+        return np.sqrt(np.sqrt(np.pi)/2) * (erf(x/np.sqrt(2)) + 1)
+    
     @cached_property
     def kin(self):
         """The kinetic energy of this series."""
         #return -1/2 * self.dot(self.der(2))
         return abs(self.der())**2 / 2
```

### Comparing `hermite-function-1.0.1/setup.py` & `hermite-function-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
   
 setup(
     name = 'hermite-function',
-    version = '1.0.1',
+    version = '1.1',
     description = 'A Hermite function series module.',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     
     author = 'Sebastian Gössl',
     author_email = 'goessl@student.tugraz.at',
     license = 'MIT',
```

