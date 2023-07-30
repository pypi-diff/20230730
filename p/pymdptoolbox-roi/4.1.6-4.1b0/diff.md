# Comparing `tmp/pymdptoolbox-roi-4.1.6.tar.gz` & `tmp/pymdptoolbox-roi-4.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymdptoolbox-roi-4.1.6.tar", last modified: Sun Jul 30 13:50:13 2023, max compression
+gzip compressed data, was "dist/pymdptoolbox-roi-4.1b0.tar", last modified: Tue May 26 17:36:23 2020, max compression
```

## Comparing `pymdptoolbox-roi-4.1.6.tar` & `pymdptoolbox-roi-4.1b0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 13:50:13.648887 pymdptoolbox-roi-4.1.6/
--rw-r--r--   0 root         (0) root         (0)     1540 2023-07-30 13:47:50.000000 pymdptoolbox-roi-4.1.6/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     1486 2023-07-30 13:50:13.648887 pymdptoolbox-roi-4.1.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6871 2023-07-30 13:47:50.000000 pymdptoolbox-roi-4.1.6/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-30 13:50:13.648887 pymdptoolbox-roi-4.1.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1830 2023-07-30 13:47:50.000000 pymdptoolbox-roi-4.1.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 13:50:13.648887 pymdptoolbox-roi-4.1.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 13:50:13.648887 pymdptoolbox-roi-4.1.6/src/mdptoolbox/
--rw-r--r--   0 root         (0) root         (0)     3136 2023-07-30 13:47:50.000000 pymdptoolbox-roi-4.1.6/src/mdptoolbox/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3645 2023-07-30 13:47:50.000000 pymdptoolbox-roi-4.1.6/src/mdptoolbox/error.py
--rw-r--r--   0 root         (0) root         (0)    15234 2023-07-30 13:47:50.000000 pymdptoolbox-roi-4.1.6/src/mdptoolbox/example.py
--rw-r--r--   0 root         (0) root         (0)    60293 2023-07-30 13:47:50.000000 pymdptoolbox-roi-4.1.6/src/mdptoolbox/mdp.py
--rw-r--r--   0 root         (0) root         (0)    10500 2023-07-30 13:47:50.000000 pymdptoolbox-roi-4.1.6/src/mdptoolbox/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 13:50:13.648887 pymdptoolbox-roi-4.1.6/src/pymdptoolbox_roi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1486 2023-07-30 13:50:13.000000 pymdptoolbox-roi-4.1.6/src/pymdptoolbox_roi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      372 2023-07-30 13:50:13.000000 pymdptoolbox-roi-4.1.6/src/pymdptoolbox_roi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-30 13:50:13.000000 pymdptoolbox-roi-4.1.6/src/pymdptoolbox_roi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-30 13:50:13.000000 pymdptoolbox-roi-4.1.6/src/pymdptoolbox_roi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-30 13:50:13.000000 pymdptoolbox-roi-4.1.6/src/pymdptoolbox_roi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-26 17:36:23.000000 pymdptoolbox-roi-4.1b0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-26 17:36:23.000000 pymdptoolbox-roi-4.1b0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-26 17:36:23.000000 pymdptoolbox-roi-4.1b0/src/pymdptoolbox_roi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      360 2020-05-26 17:36:23.000000 pymdptoolbox-roi-4.1b0/src/pymdptoolbox_roi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-05-26 17:36:23.000000 pymdptoolbox-roi-4.1b0/src/pymdptoolbox_roi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2020-05-26 17:36:23.000000 pymdptoolbox-roi-4.1b0/src/pymdptoolbox_roi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2020-05-26 17:36:23.000000 pymdptoolbox-roi-4.1b0/src/pymdptoolbox_roi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1472 2020-05-26 17:36:23.000000 pymdptoolbox-roi-4.1b0/src/pymdptoolbox_roi.egg-info/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-26 17:36:23.000000 pymdptoolbox-roi-4.1b0/src/mdptoolbox/
+-rw-r--r--   0 root         (0) root         (0)     3645 2020-05-26 17:34:05.000000 pymdptoolbox-roi-4.1b0/src/mdptoolbox/error.py
+-rw-r--r--   0 root         (0) root         (0)    15234 2020-05-26 17:34:05.000000 pymdptoolbox-roi-4.1b0/src/mdptoolbox/example.py
+-rw-r--r--   0 root         (0) root         (0)    10309 2020-05-26 17:34:05.000000 pymdptoolbox-roi-4.1b0/src/mdptoolbox/util.py
+-rw-r--r--   0 root         (0) root         (0)    58404 2020-05-26 17:34:05.000000 pymdptoolbox-roi-4.1b0/src/mdptoolbox/mdp.py
+-rw-r--r--   0 root         (0) root         (0)     3136 2020-05-26 17:34:05.000000 pymdptoolbox-roi-4.1b0/src/mdptoolbox/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2020-05-26 17:34:05.000000 pymdptoolbox-roi-4.1b0/setup.py
+-rw-r--r--   0 root         (0) root         (0)       38 2020-05-26 17:36:23.000000 pymdptoolbox-roi-4.1b0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6871 2020-05-26 17:34:05.000000 pymdptoolbox-roi-4.1b0/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1472 2020-05-26 17:36:23.000000 pymdptoolbox-roi-4.1b0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pymdptoolbox-roi-4.1.6/PKG-INFO` & `pymdptoolbox-roi-4.1b0/src/pymdptoolbox_roi.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pymdptoolbox-roi
-Version: 4.1.6
+Version: 4.1b0
 Summary: Markov Decision Process (MDP) Toolbox
 Home-page: https://github.com/sawcordwell/pymdptoolbox
-Download-URL: https://pypi.python.org/pypi/pymdptoolbox
 Author: Steven A. W. Cordwell
 Author-email: steven.cordwell@uqconnect.edu.au
 License: New BSD
+Download-URL: https://pypi.python.org/pypi/pymdptoolbox
+Description: The MDP toolbox provides classes and functions for the resolution of descrete-time Markov Decision Processes. The list of algorithms that have been implemented includes backwards induction, linear programming, policy iteration, q-learning and value iteration along with several variations.
 Platform: Any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
@@ -22,10 +23,7 @@
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: LP
-License-File: LICENSE.txt
-
-The MDP toolbox provides classes and functions for the resolution of descrete-time Markov Decision Processes. The list of algorithms that have been implemented includes backwards induction, linear programming, policy iteration, q-learning and value iteration along with several variations.
```

### Comparing `pymdptoolbox-roi-4.1.6/README.rst` & `pymdptoolbox-roi-4.1b0/README.rst`

 * *Files identical despite different names*

### Comparing `pymdptoolbox-roi-4.1.6/setup.py` & `pymdptoolbox-roi-4.1b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 
 setup(name="pymdptoolbox-roi",
-      version="4.1.6",
+      version="4.1b",
       author="Steven A. W. Cordwell",
       author_email="steven.cordwell@uqconnect.edu.au",
       url="https://github.com/sawcordwell/pymdptoolbox",
       description="Markov Decision Process (MDP) Toolbox",
       long_description="The MDP toolbox provides classes and functions for "
       "the resolution of descrete-time Markov Decision Processes. The list of "
       "algorithms that have been implemented includes backwards induction, "
```

### Comparing `pymdptoolbox-roi-4.1.6/src/mdptoolbox/__init__.py` & `pymdptoolbox-roi-4.1b0/src/mdptoolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `pymdptoolbox-roi-4.1.6/src/mdptoolbox/error.py` & `pymdptoolbox-roi-4.1b0/src/mdptoolbox/error.py`

 * *Files identical despite different names*

### Comparing `pymdptoolbox-roi-4.1.6/src/mdptoolbox/example.py` & `pymdptoolbox-roi-4.1b0/src/mdptoolbox/example.py`

 * *Files identical despite different names*

### Comparing `pymdptoolbox-roi-4.1.6/src/mdptoolbox/mdp.py` & `pymdptoolbox-roi-4.1b0/src/mdptoolbox/mdp.py`

 * *Files 2% similar despite different names*

```diff
@@ -613,20 +613,20 @@
     >>> expected = (26.244000000000014, 29.484000000000016, 33.484000000000016)
     >>> all(expected[k] - pi.V[k] < 1e-12 for k in range(len(expected)))
     True
     >>> pi.policy
     (0, 0, 0)
     """
 
-    def __init__(self, transitions, reward, discount, policy0=None, epsilon=0.01,
+    def __init__(self, transitions, reward, discount, policy0=None,
                  max_iter=1000, eval_type=0, skip_check=False):
         # Initialise a policy iteration MDP.
         #
         # Set up the MDP, but don't need to worry about epsilon values
-        MDP.__init__(self, transitions, reward, discount, epsilon, max_iter,
+        MDP.__init__(self, transitions, reward, discount, None, max_iter,
                      skip_check=skip_check)
         # Check if the user has supplied an initial policy. If not make one.
         if policy0 is None:
             # Initialise the policy to the one which maximises the expected
             # immediate reward
             null = _np.zeros(self.S)
             self.policy, null = self._bellmanOperator(null)
@@ -674,63 +674,35 @@
         # policy(S) = a policy
         #
         # Evaluation
         # ----------
         # Ppolicy(SxS)  = transition matrix for policy
         # PRpolicy(S)   = reward matrix for policy
         #
-        if not _sp.issparse(self.P[0]):
-            Ppolicy = _np.empty((self.S, self.S))
-            Rpolicy = _np.zeros(self.S)
-            for aa in range(self.A):  # avoid looping over S
-                # the rows that use action a.
-                ind = (self.policy == aa).nonzero()[0]
-                # if no rows use action a, then no need to assign this
-                if ind.size > 0:
-                    try:
-                        Ppolicy[ind, :] = self.P[aa][ind, :]
-                    except ValueError:
-                        print('error, this should not happen')
-                        Ppolicy[ind, :] = self.P[aa][ind, :].todense()
-                    # PR = self._computePR() # an apparently uneeded line, and
-                    # perhaps harmful in this implementation c.f.
-                    # mdp_computePpolicyPRpolicy.m
-                    Rpolicy[ind] = self.R[aa][ind]
-            # self.R cannot be sparse with the code in its current condition, but
-            # it should be possible in the future. Also, if R is so big that its
-            # a good idea to use a sparse matrix for it, then converting PRpolicy
-            # from a dense to sparse matrix doesn't seem very memory efficient
-            #if type(self.R) is _sp.csr_matrix:
-            #    Rpolicy = _sp.csr_matrix(Rpolicy)
-
-        else:
-            Ppolicy = _sp.csr_matrix((self.S, self.S))
-            Rpolicy = _np.zeros(self.S)
-            #'''
-            for aa in range(self.A):  # avoid looping over S
-                Ppolicy += self.P[aa].multiply(_np.expand_dims(self.policy == aa, axis=1))
-                Rpolicy += _np.multiply(self.R[aa], self.policy == aa)
-            #'''
-            #for i in range(self.S):
-            #    Ppolicy[i, :] = self.P[self.policy[i]][i, :]
-            #    Rpolicy[i] = self.R[self.policy[i]][i]
-            '''
-            for aa in range(self.A):  # avoid looping over S
-                print(aa)
-                # the rows that use action a.
-                ind = (self.policy == aa).nonzero()[0]
-                # if no rows use action a, then no need to assign this
-                if ind.size > 0:
+        Ppolicy = _np.empty((self.S, self.S))
+        Rpolicy = _np.zeros(self.S)
+        for aa in range(self.A):  # avoid looping over S
+            # the rows that use action a.
+            ind = (self.policy == aa).nonzero()[0]
+            # if no rows use action a, then no need to assign this
+            if ind.size > 0:
+                try:
                     Ppolicy[ind, :] = self.P[aa][ind, :]
-                    # PR = self._computePR() # an apparently uneeded line, and
-                    # perhaps harmful in this implementation c.f.
-                    # mdp_computePpolicyPRpolicy.m
-                    Rpolicy[ind] = self.R[aa][ind]
-            '''
-
+                except ValueError:
+                    Ppolicy[ind, :] = self.P[aa][ind, :].todense()
+                # PR = self._computePR() # an apparently uneeded line, and
+                # perhaps harmful in this implementation c.f.
+                # mdp_computePpolicyPRpolicy.m
+                Rpolicy[ind] = self.R[aa][ind]
+        # self.R cannot be sparse with the code in its current condition, but
+        # it should be possible in the future. Also, if R is so big that its
+        # a good idea to use a sparse matrix for it, then converting PRpolicy
+        # from a dense to sparse matrix doesn't seem very memory efficient
+        if type(self.R) is _sp.csr_matrix:
+            Rpolicy = _sp.csr_matrix(Rpolicy)
         # self.Ppolicy = Ppolicy
         # self.Rpolicy = Rpolicy
         return (Ppolicy, Rpolicy)
 
     def _evalPolicyIterative(self, V0=0, epsilon=0.0001, max_iter=10000):
         # Evaluate a policy using iteration.
         #
@@ -796,15 +768,14 @@
                     print(_MSG_STOP_EPSILON_OPTIMAL_VALUE)
             elif itr == max_iter:
                 done = True
                 if self.verbose:
                     print(_MSG_STOP_MAX_ITER)
 
         self.V = policy_V
-        return itr
 
     def _evalPolicyMatrix(self):
         # Evaluate the value function of the policy using linear equations.
         #
         # Arguments
         # ---------
         # Let S = number of states, A = number of actions
@@ -820,28 +791,23 @@
         #
         # Evaluation
         # ----------
         # Vpolicy(S) = value function of the policy
         #
         Ppolicy, Rpolicy = self._computePpolicyPRpolicy()
         # V = PR + gPV  => (I-gP)V = PR  => V = inv(I-gP)* PR
-        if not _sp.issparse(Ppolicy):
-            self.V = _np.linalg.solve(
-                (_sp.eye(self.S, self.S) - self.discount * Ppolicy), Rpolicy)
-        else:
-            self.V = _sp.linalg.spsolve((_sp.eye(self.S, self.S) - self.discount * Ppolicy), Rpolicy)
+        self.V = _sp.linalg.solve(
+            (_sp.eye(self.S, self.S) - self.discount * Ppolicy), Rpolicy)
 
     def run(self):
         # Run the policy iteration algorithm.
         self._startRun()
 
         while True:
             self.iter += 1
-
-            Vprev = self.V.copy()
             # these _evalPolicy* functions will update the classes value
             # attribute
             if self.eval_type == "matrix":
                 self._evalPolicyMatrix()
             elif self.eval_type == "iterative":
                 self._evalPolicyIterative()
             # This should update the classes policy attribute but leave the
@@ -856,18 +822,14 @@
                 _printVerbosity(self.iter, n_different)
             # Once the policy is unchanging of the maximum number of
             # of iterations has been reached then stop
             if n_different == 0:
                 if self.verbose:
                     print(_MSG_STOP_UNCHANGING_POLICY)
                 break
-            elif _util.getSpan(self.V - Vprev) < self.epsilon:
-                if self.verbose:
-                    print(_MSG_STOP_EPSILON_OPTIMAL_POLICY)
-                break
             elif self.iter == self.max_iter:
                 if self.verbose:
                     print(_MSG_STOP_MAX_ITER)
                 break
             else:
                 self.policy = policy_next
 
@@ -930,15 +892,15 @@
         # Initialise a (modified) policy iteration MDP.
 
         # Maybe its better not to subclass from PolicyIteration, because the
         # initialisation of the two are quite different. eg there is policy0
         # being calculated here which doesn't need to be. The only thing that
         # is needed from the PolicyIteration class is the _evalPolicyIterative
         # function. Perhaps there is a better way to do it?
-        PolicyIteration.__init__(self, transitions, reward, discount, None, epsilon,
+        PolicyIteration.__init__(self, transitions, reward, discount, None,
                                  max_iter, 1, skip_check=skip_check)
 
         # PolicyIteration doesn't pass epsilon to MDP.__init__() so we will
         # check it here
         self.epsilon = float(epsilon)
         assert epsilon > 0, "'epsilon' must be greater than 0."
 
@@ -955,15 +917,14 @@
             Rmin = min(R.min() for R in self.R)
             self.V = 1 / (1 - self.discount) * Rmin * _np.ones((self.S,))
 
     def run(self):
         # Run the modified policy iteration algorithm.
 
         self._startRun()
-        self.valueIterations = 0
 
         while True:
             self.iter += 1
 
             self.policy, Vnext = self._bellmanOperator()
             # [Ppolicy, PRpolicy] = mdp_computePpolicyPRpolicy(P, PR, policy);
 
@@ -976,16 +937,15 @@
                 break
             else:
                 is_verbose = False
                 if self.verbose:
                     self.setSilent()
                     is_verbose = True
 
-                iterations = self._evalPolicyIterative(self.V, self.epsilon, self.max_iter)
-                self.valueIterations += iterations
+                self._evalPolicyIterative(self.V, self.epsilon, self.max_iter)
 
                 if is_verbose:
                     self.setVerbose()
 
         self._endRun()
 
 
@@ -1391,15 +1351,15 @@
                  max_iter=1000, initial_value=0, skip_check=False):
         # Initialise a value iteration MDP.
 
         MDP.__init__(self, transitions, reward, discount, epsilon, max_iter,
                      skip_check=skip_check)
 
         # initialization of optional arguments
-        if _np.isscalar(initial_value) and initial_value == 0:
+        if initial_value == 0:
             self.V = _np.zeros(self.S)
         else:
             assert len(initial_value) == self.S, "The initial value must be " \
                 "a vector of length S."
             self.V = _np.array(initial_value).reshape(self.S)
         if self.discount < 1:
             # compute a bound for the number of iterations and update the
```

### Comparing `pymdptoolbox-roi-4.1.6/src/mdptoolbox/util.py` & `pymdptoolbox-roi-4.1b0/src/mdptoolbox/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,15 @@
     Returns
     =======
     is_stochastic : bool
         ``True`` if ``matrix`` is row stochastic, ``False`` otherwise.
 
     """
     try:
-        absdiff = (_np.abs(matrix.sum(axis=1).flatten() - _np.ones(matrix.shape[0])))
+        absdiff = (_np.abs(matrix.sum(axis=1) - _np.ones(matrix.shape[0])))
     except AttributeError:
         matrix = _np.array(matrix)
         absdiff = (_np.abs(matrix.sum(axis=1) - _np.ones(matrix.shape[0])))
     return (absdiff.max() <= 10*_np.spacing(_np.float64(1)))
 
 
 def isNonNegative(matrix):
@@ -170,19 +170,16 @@
 
     """
     try:
         if (matrix >= 0).all():
             return True
     except (NotImplementedError, AttributeError, TypeError):
         try:
-            if not isspmatrix_lil(matrix) and (matrix.data >= 0).all():
+            if (matrix.data >= 0).all():
                 return True
-            elif isspmatrix_lil(matrix):
-                if all(all(val >= 0 for val in row) for row in matrix.data):
-                    return True
         except AttributeError:
             matrix = _np.array(matrix)
             if (matrix.data >= 0).all():
                 return True
     return False
```

### Comparing `pymdptoolbox-roi-4.1.6/src/pymdptoolbox_roi.egg-info/PKG-INFO` & `pymdptoolbox-roi-4.1b0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pymdptoolbox-roi
-Version: 4.1.6
+Version: 4.1b0
 Summary: Markov Decision Process (MDP) Toolbox
 Home-page: https://github.com/sawcordwell/pymdptoolbox
-Download-URL: https://pypi.python.org/pypi/pymdptoolbox
 Author: Steven A. W. Cordwell
 Author-email: steven.cordwell@uqconnect.edu.au
 License: New BSD
+Download-URL: https://pypi.python.org/pypi/pymdptoolbox
+Description: The MDP toolbox provides classes and functions for the resolution of descrete-time Markov Decision Processes. The list of algorithms that have been implemented includes backwards induction, linear programming, policy iteration, q-learning and value iteration along with several variations.
 Platform: Any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
@@ -22,10 +23,7 @@
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: LP
-License-File: LICENSE.txt
-
-The MDP toolbox provides classes and functions for the resolution of descrete-time Markov Decision Processes. The list of algorithms that have been implemented includes backwards induction, linear programming, policy iteration, q-learning and value iteration along with several variations.
```

