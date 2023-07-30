# Comparing `tmp/atooms_dynamics-1.1.0-py2.py3-none-any.whl.zip` & `tmp/atooms_dynamics-1.1.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 14231 bytes, number of entries: 14
+Zip file size: 14227 bytes, number of entries: 14
 -rw-rw-r--  2.0 unx      159 b- defN 21-Oct-30 16:47 atooms/__init__.py
 -rw-rw-r--  2.0 unx       51 b- defN 23-Jun-15 21:16 atooms/dynamics/__init__.py
--rw-rw-r--  2.0 unx     6037 b- defN 22-Nov-17 11:29 atooms/dynamics/api.py
+-rw-rw-r--  2.0 unx     6039 b- defN 23-Jul-30 17:13 atooms/dynamics/api.py
 -rw-rw-r--  2.0 unx     1075 b- defN 22-Feb-17 20:47 atooms/dynamics/base.py
 -rw-rw-r--  2.0 unx      579 b- defN 22-Jan-16 16:37 atooms/dynamics/helpers.py
 -rw-rw-r--  2.0 unx     9680 b- defN 22-Jan-29 20:16 atooms/dynamics/kernels_hard.f90
 -rw-rw-r--  2.0 unx     4232 b- defN 23-Jun-15 21:16 atooms/dynamics/kernels_soft.f90
 -rw-rw-r--  2.0 unx    11462 b- defN 23-Jun-15 21:16 atooms/dynamics/newtonian.py
 -rw-rw-r--  2.0 unx     3788 b- defN 23-Jun-15 21:16 atooms/dynamics/stochastic.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Jun-15 21:29 atooms_dynamics-1.1.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     3640 b- defN 23-Jun-15 21:29 atooms_dynamics-1.1.0.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Jun-15 21:29 atooms_dynamics-1.1.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       23 b- defN 23-Jun-15 21:29 atooms_dynamics-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1171 b- defN 23-Jun-15 21:29 atooms_dynamics-1.1.0.dist-info/RECORD
-14 files, 42007 bytes uncompressed, 12273 bytes compressed:  70.8%
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-30 18:26 atooms_dynamics-1.1.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3614 b- defN 23-Jul-30 18:26 atooms_dynamics-1.1.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Jul-30 18:26 atooms_dynamics-1.1.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       23 b- defN 23-Jul-30 18:26 atooms_dynamics-1.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1171 b- defN 23-Jul-30 18:26 atooms_dynamics-1.1.1.dist-info/RECORD
+14 files, 41983 bytes uncompressed, 12269 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: atooms/dynamics/newtonian.py
 Comment: 
 
 Filename: atooms/dynamics/stochastic.py
 Comment: 
 
-Filename: atooms_dynamics-1.1.0.dist-info/LICENSE
+Filename: atooms_dynamics-1.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: atooms_dynamics-1.1.0.dist-info/METADATA
+Filename: atooms_dynamics-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: atooms_dynamics-1.1.0.dist-info/WHEEL
+Filename: atooms_dynamics-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: atooms_dynamics-1.1.0.dist-info/top_level.txt
+Filename: atooms_dynamics-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: atooms_dynamics-1.1.0.dist-info/RECORD
+Filename: atooms_dynamics-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## atooms/dynamics/api.py

```diff
@@ -1,13 +1,13 @@
 import os
 import numpy
 import random
 
 from atooms.core.utils import setup_logging, mkdir, rmf
-from atooms.models import f90
+from atooms.backends import f90
 from atooms.simulation import Simulation
 from atooms.trajectory import Trajectory, TrajectoryXYZ, change_species
 from atooms.simulation.observers import write_config, write_thermo, Scheduler, target_rmsd
 
 from .newtonian import VelocityVerlet, NosePoincare
 from .stochastic import LangevinOverdamped
```

## Comparing `atooms_dynamics-1.1.0.dist-info/METADATA` & `atooms_dynamics-1.1.1.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atooms-dynamics
-Version: 1.1.0
+Version: 1.1.1
 Summary: Newtonian and stochastic dynamics backends for atooms
 Home-page: https://framagit.org/atooms/dynamics
 Author: Daniele Coslovich
 Author-email: daniele.coslovich@umontpellier.fr
 License: GPLv3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -12,17 +12,16 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: atooms-models (>=1.0.6)
-Requires-Dist: atooms (>=3.17.1)
-Requires-Dist: numpy
+Requires-Dist: atooms (>=3.19.0)
+Requires-Dist: f2py-jit (>=0.5.0)
 
 # Dynamics
 
 [![pypi](https://img.shields.io/pypi/v/atooms-dynamics.svg)](https://pypi.python.org/pypi/atooms-dynamics/)
 [![version](https://img.shields.io/pypi/pyversions/atooms-dynamics.svg)](https://pypi.python.org/pypi/atooms-dynamics/)
 [![license](https://img.shields.io/pypi/l/atooms-pp.svg)](https://en.wikipedia.org/wiki/GNU_General_Public_License)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/git/https%3A%2F%2Fframagit.org%2Fatooms%2Fdynamics/HEAD?labpath=docs%2Findex.ipynb)
```

## Comparing `atooms_dynamics-1.1.0.dist-info/RECORD` & `atooms_dynamics-1.1.1.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 atooms/__init__.py,sha256=KjHS5XygisvdXPwO7W1gPvEUCyz9TZkrHc5_d0pQQ6w,159
 atooms/dynamics/__init__.py,sha256=Be8x_McLCZckbElL-muHih_pCFvF75j6kX7icic1jL4,51
-atooms/dynamics/api.py,sha256=_xVAI3z84ZkiRBjXTpOT6DuHytz8zxYX8JUIUsQ1kYg,6037
+atooms/dynamics/api.py,sha256=gt7DO0nQ8z6OYPg3XUalKwVdzBuOtc-7odcuZ4mgq9g,6039
 atooms/dynamics/base.py,sha256=paflTzsYGxC0goXK55LYxSxwhhPgohipFfktXms3XLU,1075
 atooms/dynamics/helpers.py,sha256=v_kh7crs6xAhfZY8lk6JiTAf5TWLl432txANYMehKlo,579
 atooms/dynamics/kernels_hard.f90,sha256=I85EZ7lssxd_xpbDv4253-wv7U3pbv-ew7s0Qd7I6IU,9680
 atooms/dynamics/kernels_soft.f90,sha256=HOyN4coSWJ0ceAY1KcjCzJlPi-UNYRXmDMGo5MZPPzs,4232
 atooms/dynamics/newtonian.py,sha256=O4_A66ZxgDDbL-yw0RwPpst-BJmbnzxN6wj8W7Osy4Q,11462
 atooms/dynamics/stochastic.py,sha256=9tqvZv1f5GQFXGESdKJOU4VEpOwFdmnRD9iuXDuO1Ig,3788
-atooms_dynamics-1.1.0.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-atooms_dynamics-1.1.0.dist-info/METADATA,sha256=M5RiOPFCJ5fTYpLYXvl19wQeCAWlF9nnBvFHT6rWQt4,3640
-atooms_dynamics-1.1.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-atooms_dynamics-1.1.0.dist-info/top_level.txt,sha256=X5SmKOVrDodLIkb9MDM_Twil7tjBcvZe_YWBYdGGloQ,23
-atooms_dynamics-1.1.0.dist-info/RECORD,,
+atooms_dynamics-1.1.1.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+atooms_dynamics-1.1.1.dist-info/METADATA,sha256=n4fEPmxUsj4MkJ_IIAYxwD4xZGhOIFFcIeYGhvLhjuY,3614
+atooms_dynamics-1.1.1.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+atooms_dynamics-1.1.1.dist-info/top_level.txt,sha256=X5SmKOVrDodLIkb9MDM_Twil7tjBcvZe_YWBYdGGloQ,23
+atooms_dynamics-1.1.1.dist-info/RECORD,,
```

