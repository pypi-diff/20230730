# Comparing `tmp/py_mrm-1.0.3.tar.gz` & `tmp/py_mrm-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_mrm-1.0.3.tar", last modified: Sun Jul 30 10:06:22 2023, max compression
+gzip compressed data, was "py_mrm-1.0.4.tar", last modified: Sun Jul 30 19:44:17 2023, max compression
```

## Comparing `py_mrm-1.0.3.tar` & `py_mrm-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 10:06:22.190984 py_mrm-1.0.3/
--rw-rw-rw-   0        0        0      166 2023-07-30 10:06:22.189984 py_mrm-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     6332 2023-07-13 10:27:23.000000 py_mrm-1.0.3/README.md
--rw-rw-rw-   0        0        0     2003 2023-07-30 10:05:52.000000 py_mrm-1.0.3/conf.py
-drwxrwxrwx   0        0        0        0 2023-07-30 10:06:22.165010 py_mrm-1.0.3/py_mrm/
--rw-rw-rw-   0        0        0      152 2023-07-30 09:49:16.000000 py_mrm-1.0.3/py_mrm/__init__.py
--rw-rw-rw-   0        0        0    22717 2023-07-30 09:52:42.000000 py_mrm-1.0.3/py_mrm/py_mrm.py
-drwxrwxrwx   0        0        0        0 2023-07-30 10:06:22.180982 py_mrm-1.0.3/py_mrm.egg-info/
--rw-rw-rw-   0        0        0      166 2023-07-30 10:06:21.000000 py_mrm-1.0.3/py_mrm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-07-30 10:06:22.000000 py_mrm-1.0.3/py_mrm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 10:06:21.000000 py_mrm-1.0.3/py_mrm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-30 10:06:21.000000 py_mrm-1.0.3/py_mrm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-30 10:06:21.000000 py_mrm-1.0.3/py_mrm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-30 10:06:22.191984 py_mrm-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      334 2023-07-30 10:06:15.000000 py_mrm-1.0.3/setup.py
--rw-rw-rw-   0        0        0     1330 2023-07-30 08:10:02.000000 py_mrm-1.0.3/test_mrm.py
+drwxrwxrwx   0        0        0        0 2023-07-30 19:44:17.791519 py_mrm-1.0.4/
+-rw-rw-rw-   0        0        0      166 2023-07-30 19:44:17.790520 py_mrm-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6332 2023-07-13 10:27:23.000000 py_mrm-1.0.4/README.md
+-rw-rw-rw-   0        0        0     2003 2023-07-30 10:05:52.000000 py_mrm-1.0.4/conf.py
+drwxrwxrwx   0        0        0        0 2023-07-30 19:44:17.704521 py_mrm-1.0.4/py_mrm/
+-rw-rw-rw-   0        0        0      152 2023-07-30 09:49:16.000000 py_mrm-1.0.4/py_mrm/__init__.py
+-rw-rw-rw-   0        0        0    22714 2023-07-30 19:43:34.000000 py_mrm-1.0.4/py_mrm/py_mrm.py
+drwxrwxrwx   0        0        0        0 2023-07-30 19:44:17.787526 py_mrm-1.0.4/py_mrm.egg-info/
+-rw-rw-rw-   0        0        0      166 2023-07-30 19:44:16.000000 py_mrm-1.0.4/py_mrm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-07-30 19:44:17.000000 py_mrm-1.0.4/py_mrm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 19:44:16.000000 py_mrm-1.0.4/py_mrm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-30 19:44:16.000000 py_mrm-1.0.4/py_mrm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-30 19:44:16.000000 py_mrm-1.0.4/py_mrm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 19:44:17.792518 py_mrm-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      334 2023-07-30 19:43:52.000000 py_mrm-1.0.4/setup.py
+-rw-rw-rw-   0        0        0     1330 2023-07-30 08:10:02.000000 py_mrm-1.0.4/test_mrm.py
```

### Comparing `py_mrm-1.0.3/README.md` & `py_mrm-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `py_mrm-1.0.3/conf.py` & `py_mrm-1.0.4/conf.py`

 * *Files identical despite different names*

### Comparing `py_mrm-1.0.3/py_mrm/py_mrm.py` & `py_mrm-1.0.4/py_mrm/py_mrm.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         sz (tuple): Size of the domain.
         x_c (ndarray): Cell center coordinates.
         x_f (ndarray): Face coordinates.
         bc (dict): Boundary conditions.
 
     Returns:
         csr_array: Gradient matrix (Grad).
-        csc_array: Contribtion of the inhomogeneous BC to the gradient (grad_bc).
+        csc_array: Contribution of the inhomogeneous BC to the gradient (grad_bc).
     """
     # Trick: Reshape sizes to triplet sz_t
     if not isinstance(sz, (list, tuple)):
         sz_f = [sz]
     else:
         sz_f = list(sz)
     sz_t = [math.prod(sz_f[0:axis]), math.prod(
@@ -152,15 +152,15 @@
     num_f = math.prod(sz_f_t);
     i_f = np.repeat(np.arange(num_f),2)
     Grad = csc_array((values.flatten(), (i_f, i_c.flatten())), 
                       shape=(num_f, math.prod(sz_t)))
     Grad.sort_indices()
         
     grad_bc = csc_array((values_bc.flatten(), i_f_bc.flatten(), [
-                         0, i_f_bc.size]), shape=(math.prod(sz_f_t), 1))
+                         0, i_f_bc.size]), shape=(math.prod(sz_f_t),))
 
     return Grad, grad_bc
 
 
 def construct_div(axis, sz, x_f, nu):
     """
     Construct the Div matrix based on the given parameters.
@@ -351,15 +351,15 @@
             ~fltr_v_pos[:, -1, :] * v[:, -1, :]
         values_bc[:, -1, :] = d_fctr * v[:, -1, :] * ~fltr_v_pos[:, -1, :]
         Conv = csc_array((values.flatten(), (i_f.flatten(), i_c.flatten())), shape=(
             math.prod(sz_f_t), math.prod(sz_t)))
         Conv.sort_indices()
 
     conv_bc = csc_array((values_bc.flatten(), i_f_bc.flatten(), [
-                         0, i_f_bc.size]), shape=(math.prod(sz_f_t), 1))
+                         0, i_f_bc.size]), shape=(math.prod(sz_f_t),))
     return Conv, conv_bc
 
 def numjac_local(axis, f, c, eps_jac=1e-6):
     """
     Compute the local numerical Jacobian matrix and function values for the given function and initial values.
     The function f is assumed local, f can be dependent on other components in the array dimension 'axis'.
     numjac_local can be used to compute Jacobians of e.g. reaction, accumulation or mass transfer terms, where there
```

### Comparing `py_mrm-1.0.3/test_mrm.py` & `py_mrm-1.0.4/test_mrm.py`

 * *Files identical despite different names*

