# Comparing `tmp/hermite-function-1.0.tar.gz` & `tmp/hermite-function-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hermite-function-1.0.tar", last modified: Sun Jul  9 15:34:43 2023, max compression
+gzip compressed data, was "hermite-function-1.0.1.tar", last modified: Sun Jul 30 21:13:31 2023, max compression
```

## Comparing `hermite-function-1.0.tar` & `hermite-function-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 15:34:43.132084 hermite-function-1.0/
--rw-rw-rw-   0        0        0     1094 2022-12-12 09:43:07.000000 hermite-function-1.0/LICENSE
--rw-rw-rw-   0        0        0     5098 2023-07-09 15:34:43.129076 hermite-function-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4617 2023-07-09 15:32:47.000000 hermite-function-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 15:34:43.129076 hermite-function-1.0/hermite_function.egg-info/
--rw-rw-rw-   0        0        0     5098 2023-07-09 15:34:43.000000 hermite-function-1.0/hermite_function.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-07-09 15:34:43.000000 hermite-function-1.0/hermite_function.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 15:34:43.000000 hermite-function-1.0/hermite_function.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-09 15:34:43.000000 hermite-function-1.0/hermite_function.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-09 15:34:43.000000 hermite-function-1.0/hermite_function.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4687 2023-07-09 15:31:04.000000 hermite-function-1.0/hermitefunction.py
--rw-rw-rw-   0        0        0       42 2023-07-09 15:34:43.132855 hermite-function-1.0/setup.cfg
--rw-rw-rw-   0        0        0      845 2023-07-09 15:33:45.000000 hermite-function-1.0/setup.py
+drwxr-xr-x   0 goessl     (501) staff       (20)        0 2023-07-30 21:13:31.981893 hermite-function-1.0.1/
+-rw-r--r--   0 goessl     (501) staff       (20)     1073 2023-07-27 01:16:40.000000 hermite-function-1.0.1/LICENSE
+-rw-r--r--   0 goessl     (501) staff       (20)     5214 2023-07-30 21:13:31.981794 hermite-function-1.0.1/PKG-INFO
+-rw-r--r--   0 goessl     (501) staff       (20)     4746 2023-07-27 01:16:40.000000 hermite-function-1.0.1/README.md
+drwxr-xr-x   0 goessl     (501) staff       (20)        0 2023-07-30 21:13:31.981638 hermite-function-1.0.1/hermite_function.egg-info/
+-rw-r--r--   0 goessl     (501) staff       (20)     5214 2023-07-30 21:13:31.000000 hermite-function-1.0.1/hermite_function.egg-info/PKG-INFO
+-rw-r--r--   0 goessl     (501) staff       (20)      244 2023-07-30 21:13:31.000000 hermite-function-1.0.1/hermite_function.egg-info/SOURCES.txt
+-rw-r--r--   0 goessl     (501) staff       (20)        1 2023-07-30 21:13:31.000000 hermite-function-1.0.1/hermite_function.egg-info/dependency_links.txt
+-rw-r--r--   0 goessl     (501) staff       (20)       12 2023-07-30 21:13:31.000000 hermite-function-1.0.1/hermite_function.egg-info/requires.txt
+-rw-r--r--   0 goessl     (501) staff       (20)       16 2023-07-30 21:13:31.000000 hermite-function-1.0.1/hermite_function.egg-info/top_level.txt
+-rw-r--r--   0 goessl     (501) staff       (20)     4541 2023-07-27 01:16:40.000000 hermite-function-1.0.1/hermitefunction.py
+-rw-r--r--   0 goessl     (501) staff       (20)       38 2023-07-30 21:13:31.981927 hermite-function-1.0.1/setup.cfg
+-rw-r--r--   0 goessl     (501) staff       (20)      819 2023-07-30 21:13:02.000000 hermite-function-1.0.1/setup.py
```

### Comparing `hermite-function-1.0/PKG-INFO` & `hermite-function-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,138 +1,138 @@
-Metadata-Version: 2.1
-Name: hermite-function
-Version: 1.0
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
-# Hermite Function Series
-
-A Hermite function series package.
-```python
-from hermitefunction import HermiteFunction
-import numpy as np
-import matplotlib.pyplot as plt
-
-x = np.linspace(-4, +4, 1000)
-for n in range(5):
-    f = HermiteFunction(n)
-    plt.plot(x, f(x), label=f'$h_{n}$')
-plt.legend(loc='lower right')
-plt.show()
-```
-![png](readme/hermite_functions.png)
-
-## Installation
-
-```
-pip install hermite-function
-```
-
-## Usage
-
-This package provides a single class, `HermiteFunction`, to handle Hermite function series.
-A series can be initialized in three ways:
- - With the constructor `HermiteFunction(coef)`, that takes a non-negative integer to create a pure Hermite function with the given index, or an iterable of coefficients to create a Hermite function series.
- - With the random factory `HermiteFunction.random(deg)` for a random Hermite series of a given degree.
- - By fitting data with `HermiteFunction.fit(x, y, deg)`.
-The objects are immutable (coefficients are internally stored in a tuple).
-```python
-f = HermiteFunction((1, 2, 3))
-g = HermiteFunction.random(15)
-h = HermiteFunction.fit(x, g(x), 10)
-plt.plot(x, f(x), label='$f$')
-plt.plot(x, g(x), '--', label='$g$')
-plt.plot(x, h(x), ':', label='$h$')
-plt.legend()
-plt.show()
-```
-![png](readme/initialization.png)
-The container interface is implemented so the coefficients can be
-- accessed by indexing: `f[2]` (coefficients not set return to 0),
-- iterated over: `for c in f` (stops at last set coefficient),
-- counted: `len(f)` (number of set coefficients),
-- compared: `f == g` (tuple of coefficients get compared) &
-- shifted: `f >> 1, f << 2`.
-
-Methods for functions:
-- evaluation with `f(x)`,
-- differentiation to an arbitrary degree `f.der(n)` &
-- getting the degree of the series `f.deg` are implemented.
-```python
-f_p = f.der()
-f_pp = f.der(2)
-plt.plot(x, f(x), label=rf"$f \ (\deg f={f.deg})$")
-plt.plot(x, f_p(x), '--', label=rf"$f' \ (\deg f'={f_p.deg})$")
-plt.plot(x, f_pp(x), ':', label=rf"$f'' \ (\deg f''={f_pp.deg})$")
-plt.legend()
-plt.show()
-```
-![png](readme/differentiation.png)
-Hilbert space operations are also provided, where the Hermite functions are used as an orthonormal basis of the $L_\mathbb{R}^2$ space:
-- Vector addition & subtraction `f + g, f - g`,
-- scalar multiplication & division `2 * f, f / 2`,
-- inner product & norm `f @ g, abs(f)`.
-```python
-g = HermiteFunction(4)
-h = f + g
-i = 0.5 * f
-plt.plot(x, f(x), label='$f$')
-plt.plot(x, g(x), '--', label='$g$')
-plt.plot(x, h(x), ':', label='$h$')
-plt.plot(x, i(x), '-.', label='$i$')
-plt.legend()
-plt.show()
-```
-![png](readme/arithmetic.png)
-Because this package was intended as a tool to work with quantum mechanical wavefunctions, the expectation value for the kinetic energy is also implemented ($\langle\hat{P}^2\rangle=\frac{1}{2}\int_\mathbb{R}f^*(x)f''(x)dx$, natural units):
-```python
-f.kin
-```
-
-## Proofs
-
-In the following let
-
-$$
-    f=\sum_{k=0}^\infty f_k h_k, \ g=\sum_{k=0}^\infty g_k h_k.
-$$
-
-where $h_k$ are the Hermite functions, defined by the Hermite polynomials $H_k$:
-
-$$
-    h_k(x) = \frac{e^{-\frac{x^2}{2}}}{\sqrt{2^kk!\sqrt{\pi}}} H_k(x)
-$$
-
-from [Wikipedia - Hermite functions](https://en.wikipedia.org/wiki/Hermite_polynomials\#Hermite_functions).
-
-### Differentiation
-
-$$
-    \begin{aligned}
-        f' &= \sum_k f_k h_k' \\
-        &\qquad\mid h'\_k = \sqrt{\frac{k}{2}}h_{k-1} - \sqrt{\frac{k+1}{2}}h_{k+1} \\
-        &= \sum_k f_k \left( \sqrt{\frac{k}{2}}h_{k-1} - \sqrt{\frac{k+1}{2}}h_{k+1} \right) \\
-        &= \sum_{k=0}^\infty f_k\sqrt{\frac{k}{2}} h_{k-1} - \sum_{k=0}^\infty f_k\sqrt{\frac{k+1}{2}} h_{k+1} \\
-        &\qquad\mid k-1 \to k, \ k+1 \to k \\
-        &= \sum_{k=-1}^\infty \sqrt{\frac{k+1}{2}}f_{k+1} h_k - \sum_{k=1}^\infty \sqrt{\frac{k}{2}}f_{k-1} h_k \\
-        &\qquad\mid -0+0 = -\sqrt{\frac{-1+1}{2}}f_{-1+1}h_{-1} + \sqrt{\frac{0}{2}}f_{0-1} h_0 \\
-        &= \sum_{k=0}^\infty \sqrt{\frac{k+1}{2}}f_{k+1} h_k - \sum_{k=0}^\infty \sqrt{\frac{k}{2}}f_{k-1} h_k \\
-        &= \sum_k \left( \sqrt{\frac{k+1}{2}}f_{k+1} - \sqrt{\frac{k}{2}}f_{k-1} \right) h_k
-    \end{aligned}
-$$
-
-With $h'\_k=\sqrt{\frac{k}{2}}h_{k+1}-\sqrt{\frac{k+1}{2}}h_{k-1}$ from [Wikipedia - Hermite functions](https://en.wikipedia.org/wiki/Hermite_polynomials\#Hermite_functions).
-
-### Kinetic energy
-
-$$
-    \left\langle\frac{-\hat{P}^2}{2}\right\rangle = -\frac{1}{2}\int_{\mathbb{R}}f^*(x)\frac{d^2}{dx^2}f(x)dx = +\frac{1}{2}\int_{\mathbb{R}}|f'(x)|^2dx = \frac{1}{2}||f'||\_{L_{\mathbb{R}}^2}^2
-$$
+Metadata-Version: 2.1
+Name: hermite-function
+Version: 1.0.1
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
+# Hermite Function Series
+
+A Hermite function series package.
+```python
+from hermitefunction import HermiteFunction
+import numpy as np
+import matplotlib.pyplot as plt
+
+x = np.linspace(-4, +4, 1000)
+for n in range(5):
+    f = HermiteFunction(n)
+    plt.plot(x, f(x), label=f'$h_{n}$')
+plt.legend(loc='lower right')
+plt.show()
+```
+![png](https://raw.githubusercontent.com/goessl/hermite-function/main/readme/hermite_functions.png)
+
+## Installation
+
+```
+pip install hermite-function
+```
+
+## Usage
+
+This package provides a single class, `HermiteFunction`, to handle Hermite function series.
+A series can be initialized in three ways:
+ - With the constructor `HermiteFunction(coef)`, that takes a non-negative integer to create a pure Hermite function with the given index, or an iterable of coefficients to create a Hermite function series.
+ - With the random factory `HermiteFunction.random(deg)` for a random Hermite series of a given degree.
+ - By fitting data with `HermiteFunction.fit(x, y, deg)`.
+The objects are immutable (coefficients are internally stored in a tuple).
+```python
+f = HermiteFunction((1, 2, 3))
+g = HermiteFunction.random(15)
+h = HermiteFunction.fit(x, g(x), 10)
+plt.plot(x, f(x), label='$f$')
+plt.plot(x, g(x), '--', label='$g$')
+plt.plot(x, h(x), ':', label='$h$')
+plt.legend()
+plt.show()
+```
+![png](https://raw.githubusercontent.com/goessl/hermite-function/main/readme/initialization.png)
+The container interface is implemented so the coefficients can be
+- accessed by indexing: `f[2]` (coefficients not set return to 0),
+- iterated over: `for c in f` (stops at last set coefficient),
+- counted: `len(f)` (number of set coefficients),
+- compared: `f == g` (tuple of coefficients get compared) &
+- shifted: `f >> 1, f << 2`.
+
+Methods for functions:
+- evaluation with `f(x)`,
+- differentiation to an arbitrary degree `f.der(n)` &
+- getting the degree of the series `f.deg` are implemented.
+```python
+f_p = f.der()
+f_pp = f.der(2)
+plt.plot(x, f(x), label=rf"$f \ (\deg f={f.deg})$")
+plt.plot(x, f_p(x), '--', label=rf"$f' \ (\deg f'={f_p.deg})$")
+plt.plot(x, f_pp(x), ':', label=rf"$f'' \ (\deg f''={f_pp.deg})$")
+plt.legend()
+plt.show()
+```
+![png](https://raw.githubusercontent.com/goessl/hermite-function/main/readme/differentiation.png)
+Hilbert space operations are also provided, where the Hermite functions are used as an orthonormal basis of the $L_\mathbb{R}^2$ space:
+- Vector addition & subtraction `f + g, f - g`,
+- scalar multiplication & division `2 * f, f / 2`,
+- inner product & norm `f @ g, abs(f)`.
+```python
+g = HermiteFunction(4)
+h = f + g
+i = 0.5 * f
+plt.plot(x, f(x), label='$f$')
+plt.plot(x, g(x), '--', label='$g$')
+plt.plot(x, h(x), ':', label='$h$')
+plt.plot(x, i(x), '-.', label='$i$')
+plt.legend()
+plt.show()
+```
+![png](https://raw.githubusercontent.com/goessl/hermite-function/main/readme/arithmetic.png)
+Because this package was intended as a tool to work with quantum mechanical wavefunctions, the expectation value for the kinetic energy is also implemented ($\langle\hat{P}^2\rangle=\frac{1}{2}\int_\mathbb{R}f^*(x)f''(x)dx$, natural units):
+```python
+f.kin
+```
+
+## Proofs
+
+In the following let
+
+$$
+    f=\sum_{k=0}^\infty f_k h_k, \ g=\sum_{k=0}^\infty g_k h_k.
+$$
+
+where $h_k$ are the Hermite functions, defined by the Hermite polynomials $H_k$:
+
+$$
+    h_k(x) = \frac{e^{-\frac{x^2}{2}}}{\sqrt{2^kk!\sqrt{\pi}}} H_k(x)
+$$
+
+from [Wikipedia - Hermite functions](https://en.wikipedia.org/wiki/Hermite_polynomials\#Hermite_functions).
+
+### Differentiation
+
+$$
+    \begin{aligned}
+        f' &= \sum_k f_k h_k' \\
+        &\qquad\mid h'\_k = \sqrt{\frac{k}{2}}h_{k-1} - \sqrt{\frac{k+1}{2}}h_{k+1} \\
+        &= \sum_k f_k \left( \sqrt{\frac{k}{2}}h_{k-1} - \sqrt{\frac{k+1}{2}}h_{k+1} \right) \\
+        &= \sum_{k=0}^\infty f_k\sqrt{\frac{k}{2}} h_{k-1} - \sum_{k=0}^\infty f_k\sqrt{\frac{k+1}{2}} h_{k+1} \\
+        &\qquad\mid k-1 \to k, \ k+1 \to k \\
+        &= \sum_{k=-1}^\infty \sqrt{\frac{k+1}{2}}f_{k+1} h_k - \sum_{k=1}^\infty \sqrt{\frac{k}{2}}f_{k-1} h_k \\
+        &\qquad\mid -0+0 = -\sqrt{\frac{-1+1}{2}}f_{-1+1}h_{-1} + \sqrt{\frac{0}{2}}f_{0-1} h_0 \\
+        &= \sum_{k=0}^\infty \sqrt{\frac{k+1}{2}}f_{k+1} h_k - \sum_{k=0}^\infty \sqrt{\frac{k}{2}}f_{k-1} h_k \\
+        &= \sum_k \left( \sqrt{\frac{k+1}{2}}f_{k+1} - \sqrt{\frac{k}{2}}f_{k-1} \right) h_k
+    \end{aligned}
+$$
+
+With $h'\_k=\sqrt{\frac{k}{2}}h_{k+1}-\sqrt{\frac{k+1}{2}}h_{k-1}$ from [Wikipedia - Hermite functions](https://en.wikipedia.org/wiki/Hermite_polynomials\#Hermite_functions).
+
+### Kinetic energy
+
+$$
+    \left\langle\frac{-\hat{P}^2}{2}\right\rangle = -\frac{1}{2}\int_{\mathbb{R}}f^*(x)\frac{d^2}{dx^2}f(x)dx = +\frac{1}{2}\int_{\mathbb{R}}|f'(x)|^2dx = \frac{1}{2}||f'||\_{L_{\mathbb{R}}^2}^2
+$$
```

### Comparing `hermite-function-1.0/README.md` & `hermite-function-1.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,123 +1,123 @@
-# Hermite Function Series
-
-A Hermite function series package.
-```python
-from hermitefunction import HermiteFunction
-import numpy as np
-import matplotlib.pyplot as plt
-
-x = np.linspace(-4, +4, 1000)
-for n in range(5):
-    f = HermiteFunction(n)
-    plt.plot(x, f(x), label=f'$h_{n}$')
-plt.legend(loc='lower right')
-plt.show()
-```
-![png](readme/hermite_functions.png)
-
-## Installation
-
-```
-pip install hermite-function
-```
-
-## Usage
-
-This package provides a single class, `HermiteFunction`, to handle Hermite function series.
-A series can be initialized in three ways:
- - With the constructor `HermiteFunction(coef)`, that takes a non-negative integer to create a pure Hermite function with the given index, or an iterable of coefficients to create a Hermite function series.
- - With the random factory `HermiteFunction.random(deg)` for a random Hermite series of a given degree.
- - By fitting data with `HermiteFunction.fit(x, y, deg)`.
-The objects are immutable (coefficients are internally stored in a tuple).
-```python
-f = HermiteFunction((1, 2, 3))
-g = HermiteFunction.random(15)
-h = HermiteFunction.fit(x, g(x), 10)
-plt.plot(x, f(x), label='$f$')
-plt.plot(x, g(x), '--', label='$g$')
-plt.plot(x, h(x), ':', label='$h$')
-plt.legend()
-plt.show()
-```
-![png](readme/initialization.png)
-The container interface is implemented so the coefficients can be
-- accessed by indexing: `f[2]` (coefficients not set return to 0),
-- iterated over: `for c in f` (stops at last set coefficient),
-- counted: `len(f)` (number of set coefficients),
-- compared: `f == g` (tuple of coefficients get compared) &
-- shifted: `f >> 1, f << 2`.
-
-Methods for functions:
-- evaluation with `f(x)`,
-- differentiation to an arbitrary degree `f.der(n)` &
-- getting the degree of the series `f.deg` are implemented.
-```python
-f_p = f.der()
-f_pp = f.der(2)
-plt.plot(x, f(x), label=rf"$f \ (\deg f={f.deg})$")
-plt.plot(x, f_p(x), '--', label=rf"$f' \ (\deg f'={f_p.deg})$")
-plt.plot(x, f_pp(x), ':', label=rf"$f'' \ (\deg f''={f_pp.deg})$")
-plt.legend()
-plt.show()
-```
-![png](readme/differentiation.png)
-Hilbert space operations are also provided, where the Hermite functions are used as an orthonormal basis of the $L_\mathbb{R}^2$ space:
-- Vector addition & subtraction `f + g, f - g`,
-- scalar multiplication & division `2 * f, f / 2`,
-- inner product & norm `f @ g, abs(f)`.
-```python
-g = HermiteFunction(4)
-h = f + g
-i = 0.5 * f
-plt.plot(x, f(x), label='$f$')
-plt.plot(x, g(x), '--', label='$g$')
-plt.plot(x, h(x), ':', label='$h$')
-plt.plot(x, i(x), '-.', label='$i$')
-plt.legend()
-plt.show()
-```
-![png](readme/arithmetic.png)
-Because this package was intended as a tool to work with quantum mechanical wavefunctions, the expectation value for the kinetic energy is also implemented ($\langle\hat{P}^2\rangle=\frac{1}{2}\int_\mathbb{R}f^*(x)f''(x)dx$, natural units):
-```python
-f.kin
-```
-
-## Proofs
-
-In the following let
-
-$$
-    f=\sum_{k=0}^\infty f_k h_k, \ g=\sum_{k=0}^\infty g_k h_k.
-$$
-
-where $h_k$ are the Hermite functions, defined by the Hermite polynomials $H_k$:
-
-$$
-    h_k(x) = \frac{e^{-\frac{x^2}{2}}}{\sqrt{2^kk!\sqrt{\pi}}} H_k(x)
-$$
-
-from [Wikipedia - Hermite functions](https://en.wikipedia.org/wiki/Hermite_polynomials\#Hermite_functions).
-
-### Differentiation
-
-$$
-    \begin{aligned}
-        f' &= \sum_k f_k h_k' \\
-        &\qquad\mid h'\_k = \sqrt{\frac{k}{2}}h_{k-1} - \sqrt{\frac{k+1}{2}}h_{k+1} \\
-        &= \sum_k f_k \left( \sqrt{\frac{k}{2}}h_{k-1} - \sqrt{\frac{k+1}{2}}h_{k+1} \right) \\
-        &= \sum_{k=0}^\infty f_k\sqrt{\frac{k}{2}} h_{k-1} - \sum_{k=0}^\infty f_k\sqrt{\frac{k+1}{2}} h_{k+1} \\
-        &\qquad\mid k-1 \to k, \ k+1 \to k \\
-        &= \sum_{k=-1}^\infty \sqrt{\frac{k+1}{2}}f_{k+1} h_k - \sum_{k=1}^\infty \sqrt{\frac{k}{2}}f_{k-1} h_k \\
-        &\qquad\mid -0+0 = -\sqrt{\frac{-1+1}{2}}f_{-1+1}h_{-1} + \sqrt{\frac{0}{2}}f_{0-1} h_0 \\
-        &= \sum_{k=0}^\infty \sqrt{\frac{k+1}{2}}f_{k+1} h_k - \sum_{k=0}^\infty \sqrt{\frac{k}{2}}f_{k-1} h_k \\
-        &= \sum_k \left( \sqrt{\frac{k+1}{2}}f_{k+1} - \sqrt{\frac{k}{2}}f_{k-1} \right) h_k
-    \end{aligned}
-$$
-
-With $h'\_k=\sqrt{\frac{k}{2}}h_{k+1}-\sqrt{\frac{k+1}{2}}h_{k-1}$ from [Wikipedia - Hermite functions](https://en.wikipedia.org/wiki/Hermite_polynomials\#Hermite_functions).
-
-### Kinetic energy
-
-$$
-    \left\langle\frac{-\hat{P}^2}{2}\right\rangle = -\frac{1}{2}\int_{\mathbb{R}}f^*(x)\frac{d^2}{dx^2}f(x)dx = +\frac{1}{2}\int_{\mathbb{R}}|f'(x)|^2dx = \frac{1}{2}||f'||\_{L_{\mathbb{R}}^2}^2
-$$
+# Hermite Function Series
+
+A Hermite function series package.
+```python
+from hermitefunction import HermiteFunction
+import numpy as np
+import matplotlib.pyplot as plt
+
+x = np.linspace(-4, +4, 1000)
+for n in range(5):
+    f = HermiteFunction(n)
+    plt.plot(x, f(x), label=f'$h_{n}$')
+plt.legend(loc='lower right')
+plt.show()
+```
+![png](https://raw.githubusercontent.com/goessl/hermite-function/main/readme/hermite_functions.png)
+
+## Installation
+
+```
+pip install hermite-function
+```
+
+## Usage
+
+This package provides a single class, `HermiteFunction`, to handle Hermite function series.
+A series can be initialized in three ways:
+ - With the constructor `HermiteFunction(coef)`, that takes a non-negative integer to create a pure Hermite function with the given index, or an iterable of coefficients to create a Hermite function series.
+ - With the random factory `HermiteFunction.random(deg)` for a random Hermite series of a given degree.
+ - By fitting data with `HermiteFunction.fit(x, y, deg)`.
+The objects are immutable (coefficients are internally stored in a tuple).
+```python
+f = HermiteFunction((1, 2, 3))
+g = HermiteFunction.random(15)
+h = HermiteFunction.fit(x, g(x), 10)
+plt.plot(x, f(x), label='$f$')
+plt.plot(x, g(x), '--', label='$g$')
+plt.plot(x, h(x), ':', label='$h$')
+plt.legend()
+plt.show()
+```
+![png](https://raw.githubusercontent.com/goessl/hermite-function/main/readme/initialization.png)
+The container interface is implemented so the coefficients can be
+- accessed by indexing: `f[2]` (coefficients not set return to 0),
+- iterated over: `for c in f` (stops at last set coefficient),
+- counted: `len(f)` (number of set coefficients),
+- compared: `f == g` (tuple of coefficients get compared) &
+- shifted: `f >> 1, f << 2`.
+
+Methods for functions:
+- evaluation with `f(x)`,
+- differentiation to an arbitrary degree `f.der(n)` &
+- getting the degree of the series `f.deg` are implemented.
+```python
+f_p = f.der()
+f_pp = f.der(2)
+plt.plot(x, f(x), label=rf"$f \ (\deg f={f.deg})$")
+plt.plot(x, f_p(x), '--', label=rf"$f' \ (\deg f'={f_p.deg})$")
+plt.plot(x, f_pp(x), ':', label=rf"$f'' \ (\deg f''={f_pp.deg})$")
+plt.legend()
+plt.show()
+```
+![png](https://raw.githubusercontent.com/goessl/hermite-function/main/readme/differentiation.png)
+Hilbert space operations are also provided, where the Hermite functions are used as an orthonormal basis of the $L_\mathbb{R}^2$ space:
+- Vector addition & subtraction `f + g, f - g`,
+- scalar multiplication & division `2 * f, f / 2`,
+- inner product & norm `f @ g, abs(f)`.
+```python
+g = HermiteFunction(4)
+h = f + g
+i = 0.5 * f
+plt.plot(x, f(x), label='$f$')
+plt.plot(x, g(x), '--', label='$g$')
+plt.plot(x, h(x), ':', label='$h$')
+plt.plot(x, i(x), '-.', label='$i$')
+plt.legend()
+plt.show()
+```
+![png](https://raw.githubusercontent.com/goessl/hermite-function/main/readme/arithmetic.png)
+Because this package was intended as a tool to work with quantum mechanical wavefunctions, the expectation value for the kinetic energy is also implemented ($\langle\hat{P}^2\rangle=\frac{1}{2}\int_\mathbb{R}f^*(x)f''(x)dx$, natural units):
+```python
+f.kin
+```
+
+## Proofs
+
+In the following let
+
+$$
+    f=\sum_{k=0}^\infty f_k h_k, \ g=\sum_{k=0}^\infty g_k h_k.
+$$
+
+where $h_k$ are the Hermite functions, defined by the Hermite polynomials $H_k$:
+
+$$
+    h_k(x) = \frac{e^{-\frac{x^2}{2}}}{\sqrt{2^kk!\sqrt{\pi}}} H_k(x)
+$$
+
+from [Wikipedia - Hermite functions](https://en.wikipedia.org/wiki/Hermite_polynomials\#Hermite_functions).
+
+### Differentiation
+
+$$
+    \begin{aligned}
+        f' &= \sum_k f_k h_k' \\
+        &\qquad\mid h'\_k = \sqrt{\frac{k}{2}}h_{k-1} - \sqrt{\frac{k+1}{2}}h_{k+1} \\
+        &= \sum_k f_k \left( \sqrt{\frac{k}{2}}h_{k-1} - \sqrt{\frac{k+1}{2}}h_{k+1} \right) \\
+        &= \sum_{k=0}^\infty f_k\sqrt{\frac{k}{2}} h_{k-1} - \sum_{k=0}^\infty f_k\sqrt{\frac{k+1}{2}} h_{k+1} \\
+        &\qquad\mid k-1 \to k, \ k+1 \to k \\
+        &= \sum_{k=-1}^\infty \sqrt{\frac{k+1}{2}}f_{k+1} h_k - \sum_{k=1}^\infty \sqrt{\frac{k}{2}}f_{k-1} h_k \\
+        &\qquad\mid -0+0 = -\sqrt{\frac{-1+1}{2}}f_{-1+1}h_{-1} + \sqrt{\frac{0}{2}}f_{0-1} h_0 \\
+        &= \sum_{k=0}^\infty \sqrt{\frac{k+1}{2}}f_{k+1} h_k - \sum_{k=0}^\infty \sqrt{\frac{k}{2}}f_{k-1} h_k \\
+        &= \sum_k \left( \sqrt{\frac{k+1}{2}}f_{k+1} - \sqrt{\frac{k}{2}}f_{k-1} \right) h_k
+    \end{aligned}
+$$
+
+With $h'\_k=\sqrt{\frac{k}{2}}h_{k+1}-\sqrt{\frac{k+1}{2}}h_{k-1}$ from [Wikipedia - Hermite functions](https://en.wikipedia.org/wiki/Hermite_polynomials\#Hermite_functions).
+
+### Kinetic energy
+
+$$
+    \left\langle\frac{-\hat{P}^2}{2}\right\rangle = -\frac{1}{2}\int_{\mathbb{R}}f^*(x)\frac{d^2}{dx^2}f(x)dx = +\frac{1}{2}\int_{\mathbb{R}}|f'(x)|^2dx = \frac{1}{2}||f'||\_{L_{\mathbb{R}}^2}^2
+$$
```

### Comparing `hermite-function-1.0/hermite_function.egg-info/PKG-INFO` & `hermite-function-1.0.1/hermite_function.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,138 +1,138 @@
-Metadata-Version: 2.1
-Name: hermite-function
-Version: 1.0
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
-# Hermite Function Series
-
-A Hermite function series package.
-```python
-from hermitefunction import HermiteFunction
-import numpy as np
-import matplotlib.pyplot as plt
-
-x = np.linspace(-4, +4, 1000)
-for n in range(5):
-    f = HermiteFunction(n)
-    plt.plot(x, f(x), label=f'$h_{n}$')
-plt.legend(loc='lower right')
-plt.show()
-```
-![png](readme/hermite_functions.png)
-
-## Installation
-
-```
-pip install hermite-function
-```
-
-## Usage
-
-This package provides a single class, `HermiteFunction`, to handle Hermite function series.
-A series can be initialized in three ways:
- - With the constructor `HermiteFunction(coef)`, that takes a non-negative integer to create a pure Hermite function with the given index, or an iterable of coefficients to create a Hermite function series.
- - With the random factory `HermiteFunction.random(deg)` for a random Hermite series of a given degree.
- - By fitting data with `HermiteFunction.fit(x, y, deg)`.
-The objects are immutable (coefficients are internally stored in a tuple).
-```python
-f = HermiteFunction((1, 2, 3))
-g = HermiteFunction.random(15)
-h = HermiteFunction.fit(x, g(x), 10)
-plt.plot(x, f(x), label='$f$')
-plt.plot(x, g(x), '--', label='$g$')
-plt.plot(x, h(x), ':', label='$h$')
-plt.legend()
-plt.show()
-```
-![png](readme/initialization.png)
-The container interface is implemented so the coefficients can be
-- accessed by indexing: `f[2]` (coefficients not set return to 0),
-- iterated over: `for c in f` (stops at last set coefficient),
-- counted: `len(f)` (number of set coefficients),
-- compared: `f == g` (tuple of coefficients get compared) &
-- shifted: `f >> 1, f << 2`.
-
-Methods for functions:
-- evaluation with `f(x)`,
-- differentiation to an arbitrary degree `f.der(n)` &
-- getting the degree of the series `f.deg` are implemented.
-```python
-f_p = f.der()
-f_pp = f.der(2)
-plt.plot(x, f(x), label=rf"$f \ (\deg f={f.deg})$")
-plt.plot(x, f_p(x), '--', label=rf"$f' \ (\deg f'={f_p.deg})$")
-plt.plot(x, f_pp(x), ':', label=rf"$f'' \ (\deg f''={f_pp.deg})$")
-plt.legend()
-plt.show()
-```
-![png](readme/differentiation.png)
-Hilbert space operations are also provided, where the Hermite functions are used as an orthonormal basis of the $L_\mathbb{R}^2$ space:
-- Vector addition & subtraction `f + g, f - g`,
-- scalar multiplication & division `2 * f, f / 2`,
-- inner product & norm `f @ g, abs(f)`.
-```python
-g = HermiteFunction(4)
-h = f + g
-i = 0.5 * f
-plt.plot(x, f(x), label='$f$')
-plt.plot(x, g(x), '--', label='$g$')
-plt.plot(x, h(x), ':', label='$h$')
-plt.plot(x, i(x), '-.', label='$i$')
-plt.legend()
-plt.show()
-```
-![png](readme/arithmetic.png)
-Because this package was intended as a tool to work with quantum mechanical wavefunctions, the expectation value for the kinetic energy is also implemented ($\langle\hat{P}^2\rangle=\frac{1}{2}\int_\mathbb{R}f^*(x)f''(x)dx$, natural units):
-```python
-f.kin
-```
-
-## Proofs
-
-In the following let
-
-$$
-    f=\sum_{k=0}^\infty f_k h_k, \ g=\sum_{k=0}^\infty g_k h_k.
-$$
-
-where $h_k$ are the Hermite functions, defined by the Hermite polynomials $H_k$:
-
-$$
-    h_k(x) = \frac{e^{-\frac{x^2}{2}}}{\sqrt{2^kk!\sqrt{\pi}}} H_k(x)
-$$
-
-from [Wikipedia - Hermite functions](https://en.wikipedia.org/wiki/Hermite_polynomials\#Hermite_functions).
-
-### Differentiation
-
-$$
-    \begin{aligned}
-        f' &= \sum_k f_k h_k' \\
-        &\qquad\mid h'\_k = \sqrt{\frac{k}{2}}h_{k-1} - \sqrt{\frac{k+1}{2}}h_{k+1} \\
-        &= \sum_k f_k \left( \sqrt{\frac{k}{2}}h_{k-1} - \sqrt{\frac{k+1}{2}}h_{k+1} \right) \\
-        &= \sum_{k=0}^\infty f_k\sqrt{\frac{k}{2}} h_{k-1} - \sum_{k=0}^\infty f_k\sqrt{\frac{k+1}{2}} h_{k+1} \\
-        &\qquad\mid k-1 \to k, \ k+1 \to k \\
-        &= \sum_{k=-1}^\infty \sqrt{\frac{k+1}{2}}f_{k+1} h_k - \sum_{k=1}^\infty \sqrt{\frac{k}{2}}f_{k-1} h_k \\
-        &\qquad\mid -0+0 = -\sqrt{\frac{-1+1}{2}}f_{-1+1}h_{-1} + \sqrt{\frac{0}{2}}f_{0-1} h_0 \\
-        &= \sum_{k=0}^\infty \sqrt{\frac{k+1}{2}}f_{k+1} h_k - \sum_{k=0}^\infty \sqrt{\frac{k}{2}}f_{k-1} h_k \\
-        &= \sum_k \left( \sqrt{\frac{k+1}{2}}f_{k+1} - \sqrt{\frac{k}{2}}f_{k-1} \right) h_k
-    \end{aligned}
-$$
-
-With $h'\_k=\sqrt{\frac{k}{2}}h_{k+1}-\sqrt{\frac{k+1}{2}}h_{k-1}$ from [Wikipedia - Hermite functions](https://en.wikipedia.org/wiki/Hermite_polynomials\#Hermite_functions).
-
-### Kinetic energy
-
-$$
-    \left\langle\frac{-\hat{P}^2}{2}\right\rangle = -\frac{1}{2}\int_{\mathbb{R}}f^*(x)\frac{d^2}{dx^2}f(x)dx = +\frac{1}{2}\int_{\mathbb{R}}|f'(x)|^2dx = \frac{1}{2}||f'||\_{L_{\mathbb{R}}^2}^2
-$$
+Metadata-Version: 2.1
+Name: hermite-function
+Version: 1.0.1
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
+# Hermite Function Series
+
+A Hermite function series package.
+```python
+from hermitefunction import HermiteFunction
+import numpy as np
+import matplotlib.pyplot as plt
+
+x = np.linspace(-4, +4, 1000)
+for n in range(5):
+    f = HermiteFunction(n)
+    plt.plot(x, f(x), label=f'$h_{n}$')
+plt.legend(loc='lower right')
+plt.show()
+```
+![png](https://raw.githubusercontent.com/goessl/hermite-function/main/readme/hermite_functions.png)
+
+## Installation
+
+```
+pip install hermite-function
+```
+
+## Usage
+
+This package provides a single class, `HermiteFunction`, to handle Hermite function series.
+A series can be initialized in three ways:
+ - With the constructor `HermiteFunction(coef)`, that takes a non-negative integer to create a pure Hermite function with the given index, or an iterable of coefficients to create a Hermite function series.
+ - With the random factory `HermiteFunction.random(deg)` for a random Hermite series of a given degree.
+ - By fitting data with `HermiteFunction.fit(x, y, deg)`.
+The objects are immutable (coefficients are internally stored in a tuple).
+```python
+f = HermiteFunction((1, 2, 3))
+g = HermiteFunction.random(15)
+h = HermiteFunction.fit(x, g(x), 10)
+plt.plot(x, f(x), label='$f$')
+plt.plot(x, g(x), '--', label='$g$')
+plt.plot(x, h(x), ':', label='$h$')
+plt.legend()
+plt.show()
+```
+![png](https://raw.githubusercontent.com/goessl/hermite-function/main/readme/initialization.png)
+The container interface is implemented so the coefficients can be
+- accessed by indexing: `f[2]` (coefficients not set return to 0),
+- iterated over: `for c in f` (stops at last set coefficient),
+- counted: `len(f)` (number of set coefficients),
+- compared: `f == g` (tuple of coefficients get compared) &
+- shifted: `f >> 1, f << 2`.
+
+Methods for functions:
+- evaluation with `f(x)`,
+- differentiation to an arbitrary degree `f.der(n)` &
+- getting the degree of the series `f.deg` are implemented.
+```python
+f_p = f.der()
+f_pp = f.der(2)
+plt.plot(x, f(x), label=rf"$f \ (\deg f={f.deg})$")
+plt.plot(x, f_p(x), '--', label=rf"$f' \ (\deg f'={f_p.deg})$")
+plt.plot(x, f_pp(x), ':', label=rf"$f'' \ (\deg f''={f_pp.deg})$")
+plt.legend()
+plt.show()
+```
+![png](https://raw.githubusercontent.com/goessl/hermite-function/main/readme/differentiation.png)
+Hilbert space operations are also provided, where the Hermite functions are used as an orthonormal basis of the $L_\mathbb{R}^2$ space:
+- Vector addition & subtraction `f + g, f - g`,
+- scalar multiplication & division `2 * f, f / 2`,
+- inner product & norm `f @ g, abs(f)`.
+```python
+g = HermiteFunction(4)
+h = f + g
+i = 0.5 * f
+plt.plot(x, f(x), label='$f$')
+plt.plot(x, g(x), '--', label='$g$')
+plt.plot(x, h(x), ':', label='$h$')
+plt.plot(x, i(x), '-.', label='$i$')
+plt.legend()
+plt.show()
+```
+![png](https://raw.githubusercontent.com/goessl/hermite-function/main/readme/arithmetic.png)
+Because this package was intended as a tool to work with quantum mechanical wavefunctions, the expectation value for the kinetic energy is also implemented ($\langle\hat{P}^2\rangle=\frac{1}{2}\int_\mathbb{R}f^*(x)f''(x)dx$, natural units):
+```python
+f.kin
+```
+
+## Proofs
+
+In the following let
+
+$$
+    f=\sum_{k=0}^\infty f_k h_k, \ g=\sum_{k=0}^\infty g_k h_k.
+$$
+
+where $h_k$ are the Hermite functions, defined by the Hermite polynomials $H_k$:
+
+$$
+    h_k(x) = \frac{e^{-\frac{x^2}{2}}}{\sqrt{2^kk!\sqrt{\pi}}} H_k(x)
+$$
+
+from [Wikipedia - Hermite functions](https://en.wikipedia.org/wiki/Hermite_polynomials\#Hermite_functions).
+
+### Differentiation
+
+$$
+    \begin{aligned}
+        f' &= \sum_k f_k h_k' \\
+        &\qquad\mid h'\_k = \sqrt{\frac{k}{2}}h_{k-1} - \sqrt{\frac{k+1}{2}}h_{k+1} \\
+        &= \sum_k f_k \left( \sqrt{\frac{k}{2}}h_{k-1} - \sqrt{\frac{k+1}{2}}h_{k+1} \right) \\
+        &= \sum_{k=0}^\infty f_k\sqrt{\frac{k}{2}} h_{k-1} - \sum_{k=0}^\infty f_k\sqrt{\frac{k+1}{2}} h_{k+1} \\
+        &\qquad\mid k-1 \to k, \ k+1 \to k \\
+        &= \sum_{k=-1}^\infty \sqrt{\frac{k+1}{2}}f_{k+1} h_k - \sum_{k=1}^\infty \sqrt{\frac{k}{2}}f_{k-1} h_k \\
+        &\qquad\mid -0+0 = -\sqrt{\frac{-1+1}{2}}f_{-1+1}h_{-1} + \sqrt{\frac{0}{2}}f_{0-1} h_0 \\
+        &= \sum_{k=0}^\infty \sqrt{\frac{k+1}{2}}f_{k+1} h_k - \sum_{k=0}^\infty \sqrt{\frac{k}{2}}f_{k-1} h_k \\
+        &= \sum_k \left( \sqrt{\frac{k+1}{2}}f_{k+1} - \sqrt{\frac{k}{2}}f_{k-1} \right) h_k
+    \end{aligned}
+$$
+
+With $h'\_k=\sqrt{\frac{k}{2}}h_{k+1}-\sqrt{\frac{k+1}{2}}h_{k-1}$ from [Wikipedia - Hermite functions](https://en.wikipedia.org/wiki/Hermite_polynomials\#Hermite_functions).
+
+### Kinetic energy
+
+$$
+    \left\langle\frac{-\hat{P}^2}{2}\right\rangle = -\frac{1}{2}\int_{\mathbb{R}}f^*(x)\frac{d^2}{dx^2}f(x)dx = +\frac{1}{2}\int_{\mathbb{R}}|f'(x)|^2dx = \frac{1}{2}||f'||\_{L_{\mathbb{R}}^2}^2
+$$
```

### Comparing `hermite-function-1.0/hermitefunction.py` & `hermite-function-1.0.1/hermitefunction.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-import numpy as np
-from numpy.polynomial.hermite import hermval, hermfit
-from scipy.special import factorial, binom
-from itertools import starmap, zip_longest
-import operator
-from functools import cached_property
-
-
-
-class HermiteFunction:
-    """A Hermite function series class."""
-    
-    #construction stuff
-    def __init__(self, coef):
-        """Creates a new Hermite function series with the given coefficients
-        or the i-th basis vector if an index is given."""
-        if isinstance(coef, int):
-            self.coef = (0,)*coef + (1,)
-        else:
-            self.coef = tuple(coef)
-    
-    @staticmethod
-    def random(deg, normed=True):
-        """Creates a Hermite function series of the given degree
-        with normal distributed coefficients."""
-        coef = np.random.normal(size=deg+1)
-        if normed:
-            coef /= np.linalg.norm(coef)
-        return HermiteFunction(coef)
-    
-    @staticmethod
-    def fit(x, y, deg):
-        """Creates a least squares Hermite function series fit
-        with the given degree for the given x and y values."""
-        #https://de.wikipedia.org/wiki/Multiple_lineare_Regression
-        return HermiteFunction(c * np.sqrt(2**i*factorial(i)*np.sqrt(np.pi))
-                for i, c in enumerate(hermfit(x, y/np.exp(-x**2/2), deg)))
-    
-    
-    
-    #container stuff
-    def __len__(self):
-        return len(self.coef)
-    
-    def __getitem__(self, key):
-        try:
-            return self.coef[key]
-        except IndexError:
-            return 0
-    
-    def __iter__(self):
-        return iter(self.coef)
-    
-    def __eq__(self, other):
-        return self.coef == other.coef
-    
-    
-    def __lshift__(self, other):
-        return HermiteFunction(self[1:])
-    
-    def __rshift__(self, other):
-        return HermiteFunction((0,) + self.coef)
-    
-    
-    
-    #Hilbert space stuff
-    def __abs__(self):
-        return np.sqrt(self @ self)
-    
-    def __matmul__(self, other):
-        #https://docs.python.org/3/library/itertools.html
-        return sum(starmap(operator.mul, zip(self, other)))
-    
-    
-    
-    #vector space operations
-    @staticmethod
-    def map_zip(f, v, w):
-        """Applies f(v, w) elementwise if possible,
-                otherwise elementwise in the first argument."""
-        try: #second argument iterable
-            return HermiteFunction(f(a, b) for a, b in zip(v, w))
-        except TypeError: #second argument scalar
-            return HermiteFunction(f(c, w) for c in v)
-    
-    @staticmethod
-    def map_zip_longest(f, v, w):
-        """Applies f(v, w) elementwise if possible,
-                otherwise elementwise in the first argument."""
-        try: #second argument iterable
-            return HermiteFunction(f(a, b)
-                    for a, b in zip_longest(v, w, fillvalue=0))
-        except TypeError: #second argument scalar
-            return HermiteFunction(f(c, w) for c in v)
-    
-    #implement vector space operations like they would be correct on paper:
-    #v+w, v-w, av, va, v/a
-    def __add__(self, other):
-        return HermiteFunction.map_zip_longest(operator.add, self, other)
-    
-    def __sub__(self, other):
-        return HermiteFunction.map_zip_longest(operator.sub, self, other)
-    
-    def __mul__(self, other):
-        return HermiteFunction.map_zip(operator.mul, self, other)
-    __rmul__ = __mul__
-    
-    def __truediv__(self, other):
-        return HermiteFunction.map_zip(operator.truediv, self, other)
-    
-    
-    
-    #function stuff
-    @property
-    def deg(self):
-        """Degree of this series (index of the highest set coefficient)."""
-        return len(self) - 1
-    
-    def __call__(self, x):
-        return np.exp(-x**2/2) \
-                * sum(c / np.sqrt(2**i * factorial(i) * np.sqrt(np.pi))
-                * hermval(x, (0,)*i+(1,))
-                for i, c in enumerate(self))
-    
-    def der(self, n=1):
-        """Returns the n-th derivative of this series."""
-        res = self
-        for _ in range(n):
-            res = (np.sqrt((i+1)/2) for i in range(len(res)-1)) * (res<<1) \
-                    - (np.sqrt(i/2) for i in range(len(res)+1)) * (res>>1)
-        return res
-    
-    @cached_property
-    def kin(self):
-        """The kinetic energy of this series."""
-        #return -1/2 * self.dot(self.der(2))
-        return abs(self.der())**2 / 2
-    
-    
-    
-    #python stuff
-    def __str__(self):
-        s = f'{self[0]:.1f} h_0'
-        for i, c in enumerate(self[1:]):
-            s += f' + {c:.1f} h_{i+1}'
-        return s
+import numpy as np
+from numpy.polynomial.hermite import hermval, hermfit
+from scipy.special import factorial, binom
+from itertools import starmap, zip_longest
+import operator
+from functools import cached_property
+
+
+
+class HermiteFunction:
+    """A Hermite function series class."""
+    
+    #construction stuff
+    def __init__(self, coef):
+        """Creates a new Hermite function series with the given coefficients
+        or the i-th basis vector if an index is given."""
+        if isinstance(coef, int):
+            self.coef = (0,)*coef + (1,)
+        else:
+            self.coef = tuple(coef)
+    
+    @staticmethod
+    def random(deg, normed=True):
+        """Creates a Hermite function series of the given degree
+        with normal distributed coefficients."""
+        coef = np.random.normal(size=deg+1)
+        if normed:
+            coef /= np.linalg.norm(coef)
+        return HermiteFunction(coef)
+    
+    @staticmethod
+    def fit(x, y, deg):
+        """Creates a least squares Hermite function series fit
+        with the given degree for the given x and y values."""
+        #https://de.wikipedia.org/wiki/Multiple_lineare_Regression
+        return HermiteFunction(c * np.sqrt(2**i*factorial(i)*np.sqrt(np.pi))
+                for i, c in enumerate(hermfit(x, y/np.exp(-x**2/2), deg)))
+    
+    
+    
+    #container stuff
+    def __len__(self):
+        return len(self.coef)
+    
+    def __getitem__(self, key):
+        try:
+            return self.coef[key]
+        except IndexError:
+            return 0
+    
+    def __iter__(self):
+        return iter(self.coef)
+    
+    def __eq__(self, other):
+        return self.coef == other.coef
+    
+    
+    def __lshift__(self, other):
+        return HermiteFunction(self[1:])
+    
+    def __rshift__(self, other):
+        return HermiteFunction((0,) + self.coef)
+    
+    
+    
+    #Hilbert space stuff
+    def __abs__(self):
+        return np.sqrt(self @ self)
+    
+    def __matmul__(self, other):
+        #https://docs.python.org/3/library/itertools.html
+        return sum(starmap(operator.mul, zip(self, other)))
+    
+    
+    
+    #vector space operations
+    @staticmethod
+    def map_zip(f, v, w):
+        """Applies f(v, w) elementwise if possible,
+                otherwise elementwise in the first argument."""
+        try: #second argument iterable
+            return HermiteFunction(f(a, b) for a, b in zip(v, w))
+        except TypeError: #second argument scalar
+            return HermiteFunction(f(c, w) for c in v)
+    
+    @staticmethod
+    def map_zip_longest(f, v, w):
+        """Applies f(v, w) elementwise if possible,
+                otherwise elementwise in the first argument."""
+        try: #second argument iterable
+            return HermiteFunction(f(a, b)
+                    for a, b in zip_longest(v, w, fillvalue=0))
+        except TypeError: #second argument scalar
+            return HermiteFunction(f(c, w) for c in v)
+    
+    #implement vector space operations like they would be correct on paper:
+    #v+w, v-w, av, va, v/a
+    def __add__(self, other):
+        return HermiteFunction.map_zip_longest(operator.add, self, other)
+    
+    def __sub__(self, other):
+        return HermiteFunction.map_zip_longest(operator.sub, self, other)
+    
+    def __mul__(self, other):
+        return HermiteFunction.map_zip(operator.mul, self, other)
+    __rmul__ = __mul__
+    
+    def __truediv__(self, other):
+        return HermiteFunction.map_zip(operator.truediv, self, other)
+    
+    
+    
+    #function stuff
+    @property
+    def deg(self):
+        """Degree of this series (index of the highest set coefficient)."""
+        return len(self) - 1
+    
+    def __call__(self, x):
+        return np.exp(-x**2/2) \
+                * sum(c / np.sqrt(2**i * factorial(i) * np.sqrt(np.pi))
+                * hermval(x, (0,)*i+(1,))
+                for i, c in enumerate(self))
+    
+    def der(self, n=1):
+        """Returns the n-th derivative of this series."""
+        res = self
+        for _ in range(n):
+            res = (np.sqrt((i+1)/2) for i in range(len(res)-1)) * (res<<1) \
+                    - (np.sqrt(i/2) for i in range(len(res)+1)) * (res>>1)
+        return res
+    
+    @cached_property
+    def kin(self):
+        """The kinetic energy of this series."""
+        #return -1/2 * self.dot(self.der(2))
+        return abs(self.der())**2 / 2
+    
+    
+    
+    #python stuff
+    def __str__(self):
+        s = f'{self[0]:.1f} h_0'
+        for i, c in enumerate(self[1:]):
+            s += f' + {c:.1f} h_{i+1}'
+        return s
```

