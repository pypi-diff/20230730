# Comparing `tmp/py_mrm-1.0.0.tar.gz` & `tmp/py_mrm-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_mrm-1.0.0.tar", last modified: Sat Jul 29 15:51:45 2023, max compression
+gzip compressed data, was "py_mrm-1.0.3.tar", last modified: Sun Jul 30 10:06:22 2023, max compression
```

## Comparing `py_mrm-1.0.0.tar` & `py_mrm-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 15:51:45.131839 py_mrm-1.0.0/
--rw-rw-rw-   0        0        0      245 2023-07-29 15:51:45.130867 py_mrm-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     6332 2023-07-13 10:27:23.000000 py_mrm-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 15:51:45.112878 py_mrm-1.0.0/py_mrm/
--rw-rw-rw-   0        0        0        0 2023-07-13 13:02:10.000000 py_mrm-1.0.0/py_mrm/__init__.py
--rw-rw-rw-   0        0        0    20657 2023-07-29 15:49:14.000000 py_mrm-1.0.0/py_mrm/py_mrm.py
-drwxrwxrwx   0        0        0        0 2023-07-29 15:51:45.129866 py_mrm-1.0.0/py_mrm.egg-info/
--rw-rw-rw-   0        0        0      245 2023-07-29 15:51:44.000000 py_mrm-1.0.0/py_mrm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-07-29 15:51:45.000000 py_mrm-1.0.0/py_mrm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 15:51:44.000000 py_mrm-1.0.0/py_mrm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-29 15:51:44.000000 py_mrm-1.0.0/py_mrm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-29 15:51:44.000000 py_mrm-1.0.0/py_mrm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 15:51:45.131839 py_mrm-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      334 2023-07-29 15:12:12.000000 py_mrm-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 10:06:22.190984 py_mrm-1.0.3/
+-rw-rw-rw-   0        0        0      166 2023-07-30 10:06:22.189984 py_mrm-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6332 2023-07-13 10:27:23.000000 py_mrm-1.0.3/README.md
+-rw-rw-rw-   0        0        0     2003 2023-07-30 10:05:52.000000 py_mrm-1.0.3/conf.py
+drwxrwxrwx   0        0        0        0 2023-07-30 10:06:22.165010 py_mrm-1.0.3/py_mrm/
+-rw-rw-rw-   0        0        0      152 2023-07-30 09:49:16.000000 py_mrm-1.0.3/py_mrm/__init__.py
+-rw-rw-rw-   0        0        0    22717 2023-07-30 09:52:42.000000 py_mrm-1.0.3/py_mrm/py_mrm.py
+drwxrwxrwx   0        0        0        0 2023-07-30 10:06:22.180982 py_mrm-1.0.3/py_mrm.egg-info/
+-rw-rw-rw-   0        0        0      166 2023-07-30 10:06:21.000000 py_mrm-1.0.3/py_mrm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-07-30 10:06:22.000000 py_mrm-1.0.3/py_mrm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 10:06:21.000000 py_mrm-1.0.3/py_mrm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-30 10:06:21.000000 py_mrm-1.0.3/py_mrm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-30 10:06:21.000000 py_mrm-1.0.3/py_mrm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 10:06:22.191984 py_mrm-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      334 2023-07-30 10:06:15.000000 py_mrm-1.0.3/setup.py
+-rw-rw-rw-   0        0        0     1330 2023-07-30 08:10:02.000000 py_mrm-1.0.3/test_mrm.py
```

### Comparing `py_mrm-1.0.0/README.md` & `py_mrm-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `py_mrm-1.0.0/py_mrm/py_mrm.py` & `py_mrm-1.0.3/py_mrm/py_mrm.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,25 +9,27 @@
 Functions:
 
 - construct_grad(axis, sz, x_c, x_f, bc): Construct the gradient matrix.
 - construct_div(axis, sz, x_f, nu): Construct the divergence matrix based on the given parameters.
 - construct_convflux_upwind(axis, sz, x_c, x_f, bc, v): Construct the convective flux matrix based on the given parameters.
 - numjac_local(axis, f, c, eps_jac=1e-6): Compute the local numerical Jacobian matrix and function values for the given function and initial values.
 - interp_stagg_to_cntr(axis, c_f, x_c, x_f): Interpolate values at staggered positions to cell-centers using linear interpolation.
+- interp_cntr_to_stagg(axis, c_f, x_c, x_f): Interpolate values at cell-centered positions to staggered positions using linear interpolation and extrapolation at wall.
 - non_uniform_grid(x_L, x_R, n, dx_inf, factor): Generate a non-uniform grid of points in the interval [x_L, x_R].
 - unwrap_bc(sz, bc): Unwrap the boundary conditions for a given size.
 
 Usage:
 1. Use `construct_grad` to construct the gradient matrix.
 2. Use `construct_div` to construct the Div matrix based on the given parameters.
 3. Use `construct_convflux_upwind` to construct the Conv and conv_bc matrices based on the given parameters.
 4. Use `numjac_local` to compute the local numerical Jacobian matrix and function values for the given function and initial values.
 5. Use `interp_stagg_to_cntr` to interpolate values at staggered positions to cell-centers using linear interpolation.
-6. Use `non_uniform_grid` to generate a non-uniform grid of points in the interval [x_L, x_R].
-7. Use `unwrap_bc` to unwrap the boundary conditions for a given size. Mostly used by other functions
+6. Use `interp_cntr_to_stagg` to interpolate values at cell-centers positions to staggered positions using linear interpolation.
+7. Use `non_uniform_grid` to generate a non-uniform grid of points in the interval [x_L, x_R].
+8. Use `unwrap_bc` to unwrap the boundary conditions for a given size. Mostly used by other functions
 
 """
 
 import numpy as np
 from scipy.sparse import csc_array
 import math
 
@@ -44,25 +46,28 @@
         bc (dict): Boundary conditions.
 
     Returns:
         csr_array: Gradient matrix (Grad).
         csc_array: Contribtion of the inhomogeneous BC to the gradient (grad_bc).
     """
     # Trick: Reshape sizes to triplet sz_t
-    sz_t = [math.prod(sz[0:axis]), math.prod(
-        sz[axis:axis+1]), math.prod(sz[axis+1:])]
+    if not isinstance(sz, (list, tuple)):
+        sz_f = [sz]
+    else:
+        sz_f = list(sz)
+    sz_t = [math.prod(sz_f[0:axis]), math.prod(
+        sz_f[axis:axis+1]), math.prod(sz_f[axis+1:])]
 
-    # Create face arrays
-    sz_f = list(sz)
+    # Create face arrays  
     sz_f[axis] = sz_f[axis] + 1
-    sz_f_t = list(sz_t.copy())
+    sz_f_t = sz_t.copy()
     sz_f_t[1] = sz_t[1] + 1
 
     # Create boundary quantity sizes
-    sz_bc = list(sz)
+    sz_bc = sz_f.copy()
     sz_bc[axis] = 1
     sz_bc_d = [sz_t[0], sz_t[2]]
 
     a, b, d = unwrap_bc(sz, bc)
 
     # Handle special case with one cell in the dimension axis
     if sz_t[1] == 1:
@@ -70,17 +75,17 @@
             (0, 0)).reshape((1, -1, 1)) + np.arange(sz_t[2]).reshape((1, 1, -1))
         values = np.zeros(sz_f_t)
         alpha_1 = (x_f[1] - x_f[0]) / ((x_c[0] - x_f[0]) * (x_f[1] - x_c[0]))
         alpha_2L = (x_c[0] - x_f[0]) / ((x_f[1] - x_f[0]) * (x_f[1] - x_c[0]))
         alpha_0L = alpha_1 - alpha_2L
         alpha_2R = -(x_c[0] - x_f[1]) / ((x_f[0] - x_f[1]) * (x_f[0] - x_c[0]))
         alpha_0R = alpha_1 - alpha_2R
-        fctr = 1 / ((b[0] + alpha_0L * a[0]) * (b[1] +
+        fctr = ((b[0] + alpha_0L * a[0]) * (b[1] +
                     alpha_0R * a[1]) - alpha_2L * alpha_2R * a[0] * a[1])
-        fctr[~np.isfinite(fctr)] = 0
+        np.divide(1, fctr, out=fctr, where=(fctr != 0))
         value = alpha_1 * \
             b[0] * (a[1] * (alpha_0R - alpha_2L) + b[1]) * fctr + np.zeros(sz)
         values[:, 0, :] = np.reshape(value, sz_bc_d)
         value = alpha_1 * \
             b[1] * (a[0] * (-alpha_0L + alpha_2R) - b[0]) * fctr + np.zeros(sz)
         values[:, 1, :] = np.reshape(value, sz_bc_d)
 
@@ -110,16 +115,16 @@
         values[:, 1:-1, :, 0] = -dx_inv
         values[:, 1:-1, :, 1] = dx_inv
 
         alpha_1 = (x_c[1] - x_f[0]) / ((x_c[0] - x_f[0]) * (x_c[1] - x_c[0]))
         alpha_2 = (x_c[0] - x_f[0]) / ((x_c[1] - x_f[0]) * (x_c[1] - x_c[0]))
         alpha_0 = alpha_1 - alpha_2
         b[0] = b[0] / alpha_0
-        fctr = 1 / (a[0] + b[0])
-        fctr[~np.isfinite(fctr)] = 0
+        fctr = (a[0] + b[0])
+        np.divide(1, fctr, out=fctr, where=(fctr != 0))
         b_fctr = b[0] * fctr
         b_fctr = b_fctr + np.zeros(sz_bc)
         b_fctr = np.reshape(b_fctr, sz_bc_d)
         d_fctr = d[0] * fctr
         d_fctr = d_fctr + np.zeros(sz_bc)
         d_fctr = np.reshape(d_fctr, sz_bc_d)
         values[:, 0, :, 0] = b_fctr * alpha_1
@@ -128,16 +133,16 @@
 
         alpha_1 = -(x_c[-2] - x_f[-1]) / \
             ((x_c[-1] - x_f[-1]) * (x_c[-2] - x_c[-1]))
         alpha_2 = -(x_c[-1] - x_f[-1]) / \
             ((x_c[-2] - x_f[-1]) * (x_c[-2] - x_c[-1]))
         alpha_0 = alpha_1 - alpha_2
         b[-1] = b[-1] / alpha_0
-        fctr = 1 / (a[-1] + b[-1])
-        fctr[~np.isfinite(fctr)] = 0
+        fctr = (a[-1] + b[-1])
+        np.divide(1, fctr, out=fctr, where=(fctr != 0))
         b_fctr = b[-1] * fctr
         b_fctr = b_fctr + np.zeros(sz_bc)
         b_fctr = np.reshape(b_fctr, sz_bc_d)
         d_fctr = d[-1] * fctr
         d_fctr = d_fctr + np.zeros(sz_bc)
         d_fctr = np.reshape(d_fctr, sz_bc_d)
         values[:, -1, :, 0] = b_fctr * alpha_2
@@ -167,19 +172,22 @@
         nu (callable or int): The function or integer representing nu.
 
     Returns:
         csc_array: The Div matrix.
 
     """
     # Trick: Reshape sizes to triplet sz_t
-    sz_t = [math.prod(sz[0:axis]), math.prod(
-        sz[axis:axis + 1]), math.prod(sz[axis + 1:])]
+    if not isinstance(sz, (list, tuple)):
+        sz_f = [sz]
+    else:
+        sz_f = list(sz)
+    sz_t = [math.prod(sz_f[0:axis]), math.prod(
+        sz_f[axis:axis + 1]), math.prod(sz_f[axis + 1:])]
 
     # Create face arrays
-    sz_f = list(sz)
     sz_f[axis] += 1
     sz_f_t = sz_t.copy()
     sz_f_t[1] += 1
 
     i_f = (
         sz_f_t[1] * sz_f_t[2] *
         np.arange(sz_t[0]).reshape((-1, 1, 1, 1))
@@ -234,23 +242,26 @@
         v (ndarray): The velocity array.
 
     Returns:
         csc_array: The Conv matrix.
         csc_array: The conv_bc matrix.
 
     """
-    sz_t = [math.prod(sz[0:axis]), math.prod(
-        sz[axis:axis+1]), math.prod(sz[axis+1:])]
+    if not isinstance(sz, (list, tuple)):
+        sz_f = [sz]
+    else:
+        sz_f = list(sz)
+    sz_t = [math.prod(sz_f[0:axis]), math.prod(
+        sz_f[axis:axis+1]), math.prod(sz_f[axis+1:])]
 
-    sz_f = list(sz)
     sz_f[axis] = sz_f[axis] + 1
     sz_f_t = sz_t.copy()
     sz_f_t[1] = sz_t[1] + 1
 
-    sz_bc = list(sz)
+    sz_bc = sz_f.copy()
     sz_bc[axis] = 1
     sz_bc_d = [sz_t[0], sz_t[2]]
 
     a, b, d = unwrap_bc(sz, bc)
 
     v = np.array(v) + np.zeros(sz_f)
     v = v.reshape(sz_f_t)
@@ -261,17 +272,17 @@
             (0, 0)).reshape((1, -1, 1)) + np.arange(sz_t[2]).reshape((1, 1, -1))
         values = np.zeros(sz_f_t)
         alpha_1 = (x_f[1] - x_f[0]) / ((x_c[0] - x_f[0]) * (x_f[1] - x_c[0]))
         alpha_2L = (x_c[0] - x_f[0]) / ((x_f[1] - x_f[0]) * (x_f[1] - x_c[0]))
         alpha_0L = alpha_1 - alpha_2L
         alpha_2R = -(x_c[0] - x_f[1]) / ((x_f[0] - x_f[1]) * (x_f[0] - x_c[0]))
         alpha_0R = alpha_1 - alpha_2R
-        fctr = 1. / ((b[0] + alpha_0L * a[0]) * (b[1] +
+        fctr = ((b[0] + alpha_0L * a[0]) * (b[1] +
                      alpha_0R * a[1]) - alpha_2L * alpha_2R * a[0] * a[1])
-        fctr[~np.isfinite(fctr)] = 0
+        np.divide(1, fctr, out=fctr, where=(fctr != 0))
         values[:, 0, :] = ((alpha_1 * a[0] * (a[1] * (alpha_0R - alpha_2L) + b[1])
                            * fctr + np.zeros(sz)).reshape(sz_bc_d) - 1) * fltr_v_pos[:, 0, :] + 1
         values[:, 1, :] = ((alpha_1 * a[1] * (a[0] * (alpha_0L - alpha_2R) + b[0])
                            * fctr + np.zeros(sz)).reshape(sz_bc_d) - 1) * ~fltr_v_pos[:, -1, :] + 1
         values = values * v
         Conv = csr_array((values.flatten(), i_c.flatten(), np.arange(
             0, i_c.size + 1)), shape=(math.prod(sz_f_t), math.prod(sz_t)))
@@ -304,16 +315,16 @@
         values = np.zeros((sz_f_t[0], sz_f_t[1] + 2, sz_f_t[2]))
         values[:, 2:-2, :] = v[:, 1:-1, :]
         values_bc = np.zeros((sz_f_t[0], 2, sz_f_t[2]))
 
         alpha_1 = (x_c[0] - x_f[0]) / ((x_c[0] - x_f[0]) * (x_c[1] - x_c[0]))
         alpha_2 = (x_c[1] - x_f[0]) / ((x_c[0] - x_f[0]) * (x_c[1] - x_c[0]))
         alpha_0 = alpha_1 - alpha_2
-        fctr = 1 / (alpha_0 * a[0] + b[0])
-        fctr[~np.isfinite(fctr)] = 0
+        fctr = (alpha_0 * a[0] + b[0])
+        np.divide(1, fctr, out=fctr, where=(fctr != 0))
         a_fctr = a[0] * fctr
         a_fctr = a_fctr + np.zeros(sz_bc)
         a_fctr = np.reshape(a_fctr, sz_bc_d)
         d_fctr = d[0] * fctr
         d_fctr = d_fctr + np.zeros(sz_bc)
         d_fctr = np.reshape(d_fctr, sz_bc_d)
         values[:, 0, :] = (1 + (a_fctr * alpha_1 - 1) *
@@ -322,16 +333,16 @@
         values_bc[:, 0, :] = d_fctr * v[:, 0, :] * fltr_v_pos[:, 0, :]
 
         alpha_1 = -(x_c[-2] - x_f[-1]) / \
             ((x_c[-1] - x_f[-1]) * (x_c[-2] - x_c[-1]))
         alpha_2 = -(x_c[-1] - x_f[-1]) / \
             ((x_c[-2] - x_f[-1]) * (x_c[-2] - x_c[-1]))
         alpha_0 = alpha_1 - alpha_2
-        fctr = 1 / (alpha_0 * a[-1] + b[-1])
-        fctr[~np.isfinite(fctr)] = 0
+        fctr = (alpha_0 * a[-1] + b[-1])
+        np.divide(1, fctr, out=fctr, where=(fctr != 0))
         a_fctr = a[-1] * fctr
         a_fctr = a_fctr + np.zeros(sz_bc)
         a_fctr = np.reshape(a_fctr, sz_bc_d)
         d_fctr = d[-1] * fctr
         d_fctr = d_fctr + np.zeros(sz_bc)
         d_fctr = np.reshape(d_fctr, sz_bc_d)
         values[:, -1, :] = (1 + (a_fctr * alpha_1 - 1) * ~
@@ -390,20 +401,20 @@
 
 def interp_stagg_to_cntr(axis, c_f, x_c, x_f):
     """
     Interpolate values at staggered positions to cell-centers using linear interpolation.
 
     Args:
         axis (int): Dimension that is interpolated.
-        c_f (ndarray): Quantities at cell centered positions.
+        c_f (ndarray): Quantities at staggered positions.
         x_c (ndarray): Cell-centered positions.
         x_f (ndarray): Positions of cell-faces (numel(x_f) = numel(x_c) + 1).
 
     Returns:
-        ndarray: Interpolated concentrations at the staggered positions.
+        ndarray: Interpolated concentrations at the cell-centered positions.
 
     """
     sz_f = list(c_f.shape)
     sz_f = sz_f + [1,] * (1 + axis - len(sz_f))  # size padded with extra 1's if needed
     sz_f_t = [math.prod(sz_f[:axis]), sz_f[axis], math.prod(sz_f[axis + 1:])]  # sizes for reshape as a triplet
     sz = sz_f.copy()
     sz[axis] = sz[axis] - 1
@@ -412,14 +423,44 @@
     wght = (x_c - x_f[:-1]) / (x_f[1:] - x_f[:-1])
     c_f = c_f.reshape(sz_f_t)
     c_c = c_f[:, :-1, :] + wght.reshape((1,-1,1)) * (c_f[:, 1:, :] - c_f[:, :-1, :])
     c_c = c_c.reshape(sz)
 
     return c_c
 
+def interp_cntr_to_stagg(axis, c_c, x_c, x_f):
+    """
+    Interpolate values at cell-centers to staggered positions using linear interpolation and extrapolation at the wall.
+
+    Args:
+        axis (int): Dimension that is interpolated.
+        c_f (ndarray): Quantities at staggered positions.
+        x_c (ndarray): Cell-centered positions.
+        x_f (ndarray): Positions of cell-faces (numel(x_f) = numel(x_c) + 1).
+
+    Returns:
+        ndarray: Interpolated concentrations at the cell-centered positions.
+
+    """
+    sz = list(c_c.shape)
+    sz = sz + [1,] * (1 + axis - len(sz))  # size padded with extra 1's if needed
+    sz_t = [math.prod(sz[:axis]), sz[axis], math.prod(sz[axis + 1:])]  # sizes for reshape as a triplet
+    sz_f = sz.copy()
+    sz_f[axis] = sz[axis] + 1
+    sz_f_t = sz_t.copy()
+    sz_f_t[1] = sz_f[axis]
+    wght = (x_f[1:-1] - x_c[:-1]) / (x_c[1:] - x_c[:-1])
+    c_c = c_c.reshape(sz_t)
+    c_f = np.empty(sz_f_t)
+    c_f[:,1:-1,:] = c_c[:, :-1, :] + wght.reshape((1,-1,1)) * (c_c[:, 1:, :] - c_c[:, :-1, :])
+    c_f[:,0,:] = (c_c[:,0,:]*(x_c[1]-x_f[0]) - c_c[:,1,:]*(x_c[0]-x_f[0]))/(x_c[1]-x_c[0])
+    c_f[:,-1,:] = (c_c[:,-1,:]*(x_f[-1]-x_c[-2]) - c_c[:,-2,:]*(x_f[-1]-x_c[-1]))/(x_c[-1]-x_c[-2])
+    c_f = c_f.reshape(sz_f)
+    return c_f
+
 
 def non_uniform_grid(x_L, x_R, n, dx_inf, factor):
     """
     Generate a non-uniform grid of points in the interval [x_L, x_R]
     With factor > 1 the refinement will be at the left wall, 
     with 1/factor you will get the same refinement at the right wall.
     
@@ -448,23 +489,28 @@
     Args:
         sz (tuple): Size of the domain.
         bc (dict): Boundary conditions.
 
     Returns:
         tuple: Unwrapped boundary conditions (a, b, d).
     """
+    if not isinstance(sz, (list,tuple)):
+        lgth_sz = 1
+    else:
+        lgth_sz = len(sz)
+    
     a = [None, None]
     a[0] = np.array(bc['a'][0])
-    a[0] = a[0][(..., *([np.newaxis]*(len(sz)-a[0].ndim)))]
+    a[0] = a[0][(..., *([np.newaxis]*(lgth_sz-a[0].ndim)))]
     a[1] = np.array(bc['a'][1])
-    a[1] = a[1][(..., *([np.newaxis]*(len(sz)-a[1].ndim)))]
+    a[1] = a[1][(..., *([np.newaxis]*(lgth_sz-a[1].ndim)))]
     b = [None, None]
     b[0] = np.array(bc['b'][0])
-    b[0] = b[0][(..., *([np.newaxis]*(len(sz)-b[0].ndim)))]
+    b[0] = b[0][(..., *([np.newaxis]*(lgth_sz-b[0].ndim)))]
     b[1] = np.array(bc['b'][1])
-    b[1] = b[1][(..., *([np.newaxis]*(len(sz)-b[1].ndim)))]
+    b[1] = b[1][(..., *([np.newaxis]*(lgth_sz-b[1].ndim)))]
     d = [None, None]
     d[0] = np.array(bc['d'][0])
-    d[0] = d[0][(..., *([np.newaxis]*(len(sz)-d[0].ndim)))]
+    d[0] = d[0][(..., *([np.newaxis]*(lgth_sz-d[0].ndim)))]
     d[1] = np.array(bc['d'][1])
-    d[1] = d[1][(..., *([np.newaxis]*(len(sz)-d[1].ndim)))]
+    d[1] = d[1][(..., *([np.newaxis]*(lgth_sz-d[1].ndim)))]
     return a, b, d
```

