# Comparing `tmp/codedapertures-0.6.tar.gz` & `tmp/codedapertures-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codedapertures-0.6.tar", last modified: Sat Jul 29 02:50:48 2023, max compression
+gzip compressed data, was "codedapertures-0.7.tar", last modified: Sun Jul 30 03:45:31 2023, max compression
```

## Comparing `codedapertures-0.6.tar` & `codedapertures-0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-29 02:50:48.012690 codedapertures-0.6/
--rw-r--r--   0 bbudden    (501) staff       (20)     1062 2023-01-26 02:12:38.000000 codedapertures-0.6/LICENSE
--rw-r--r--   0 bbudden    (501) staff       (20)      720 2023-07-29 02:50:48.012580 codedapertures-0.6/PKG-INFO
--rw-r--r--   0 bbudden    (501) staff       (20)     2041 2023-07-29 01:49:47.000000 codedapertures-0.6/README.md
-drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-29 02:50:48.011694 codedapertures-0.6/codedapertures/
--rw-r--r--   0 bbudden    (501) staff       (20)       30 2023-01-26 02:12:38.000000 codedapertures-0.6/codedapertures/__init__.py
--rw-r--r--   0 bbudden    (501) staff       (20)    23459 2023-07-29 02:45:59.000000 codedapertures-0.6/codedapertures/codedapertures.py
-drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-29 02:50:48.012432 codedapertures-0.6/codedapertures.egg-info/
--rw-r--r--   0 bbudden    (501) staff       (20)      720 2023-07-29 02:50:47.000000 codedapertures-0.6/codedapertures.egg-info/PKG-INFO
--rw-r--r--   0 bbudden    (501) staff       (20)      312 2023-07-29 02:50:47.000000 codedapertures-0.6/codedapertures.egg-info/SOURCES.txt
--rw-r--r--   0 bbudden    (501) staff       (20)        1 2023-07-29 02:50:47.000000 codedapertures-0.6/codedapertures.egg-info/dependency_links.txt
--rw-r--r--   0 bbudden    (501) staff       (20)        1 2023-07-06 00:30:22.000000 codedapertures-0.6/codedapertures.egg-info/not-zip-safe
--rw-r--r--   0 bbudden    (501) staff       (20)       40 2023-07-29 02:50:47.000000 codedapertures-0.6/codedapertures.egg-info/requires.txt
--rw-r--r--   0 bbudden    (501) staff       (20)       15 2023-07-29 02:50:47.000000 codedapertures-0.6/codedapertures.egg-info/top_level.txt
--rw-r--r--   0 bbudden    (501) staff       (20)       38 2023-07-29 02:50:48.012721 codedapertures-0.6/setup.cfg
--rw-r--r--   0 bbudden    (501) staff       (20)      923 2023-07-29 02:49:32.000000 codedapertures-0.6/setup.py
+drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-30 03:45:31.652292 codedapertures-0.7/
+-rw-r--r--   0 bbudden    (501) staff       (20)     1062 2023-01-26 02:12:38.000000 codedapertures-0.7/LICENSE
+-rw-r--r--   0 bbudden    (501) staff       (20)      720 2023-07-30 03:45:31.652187 codedapertures-0.7/PKG-INFO
+-rw-r--r--   0 bbudden    (501) staff       (20)     2041 2023-07-29 01:49:47.000000 codedapertures-0.7/README.md
+drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-30 03:45:31.651286 codedapertures-0.7/codedapertures/
+-rw-r--r--   0 bbudden    (501) staff       (20)       30 2023-01-26 02:12:38.000000 codedapertures-0.7/codedapertures/__init__.py
+-rw-r--r--   0 bbudden    (501) staff       (20)    31890 2023-07-30 03:30:23.000000 codedapertures-0.7/codedapertures/codedapertures.py
+drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-30 03:45:31.652033 codedapertures-0.7/codedapertures.egg-info/
+-rw-r--r--   0 bbudden    (501) staff       (20)      720 2023-07-30 03:45:31.000000 codedapertures-0.7/codedapertures.egg-info/PKG-INFO
+-rw-r--r--   0 bbudden    (501) staff       (20)      312 2023-07-30 03:45:31.000000 codedapertures-0.7/codedapertures.egg-info/SOURCES.txt
+-rw-r--r--   0 bbudden    (501) staff       (20)        1 2023-07-30 03:45:31.000000 codedapertures-0.7/codedapertures.egg-info/dependency_links.txt
+-rw-r--r--   0 bbudden    (501) staff       (20)        1 2023-07-06 00:30:22.000000 codedapertures-0.7/codedapertures.egg-info/not-zip-safe
+-rw-r--r--   0 bbudden    (501) staff       (20)       40 2023-07-30 03:45:31.000000 codedapertures-0.7/codedapertures.egg-info/requires.txt
+-rw-r--r--   0 bbudden    (501) staff       (20)       15 2023-07-30 03:45:31.000000 codedapertures-0.7/codedapertures.egg-info/top_level.txt
+-rw-r--r--   0 bbudden    (501) staff       (20)       38 2023-07-30 03:45:31.652321 codedapertures-0.7/setup.cfg
+-rw-r--r--   0 bbudden    (501) staff       (20)      923 2023-07-30 03:44:00.000000 codedapertures-0.7/setup.py
```

### Comparing `codedapertures-0.6/LICENSE` & `codedapertures-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `codedapertures-0.6/PKG-INFO` & `codedapertures-0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedapertures
-Version: 0.6
+Version: 0.7
 Summary: a python package for generating coded apertures
 Home-page: https://github.com/bpops/codedapertures
 Author: bpops
 License: MIT
 License-File: LICENSE
 
 CodedApertures is a python package that allows one to easily generate and display common coded aperture patterns. Coded apertures are a spatial encoding technique for straight-line optics, wherein traditional lensing (e.g., visible light) is not possible. Even wherein tradiational lensing is possible, there may be other advantages (infinite depth of field). Coded apertures may therefore be used for hard x-ray and gamma-ray imaging for astrophysics, medical imaging, and homeland security applications.
```

### Comparing `codedapertures-0.6/README.md` & `codedapertures-0.7/README.md`

 * *Files identical despite different names*

### Comparing `codedapertures-0.6/codedapertures/codedapertures.py` & `codedapertures-0.7/codedapertures/codedapertures.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 #
-#       _____       _       _ _____             _                            
-#      |     |___ _| |___ _| |  _  |___ ___ ___| |_ _ _ ___ ___ ___          
-#      |   --| . | . | -_| . |     | . | -_|  _|  _| | |  _| -_|_ -|         
-#      |_____|___|___|___|___|__|__|  _|___|_| |_| |___|_| |___|___|         
-#                                  |_|                                       
+#           ____                __             __
+#          /\  _`\             /\ \           /\ \
+#          \ \ \/\_\    ___    \_\ \     __   \_\ \
+#           \ \ \/_/_  / __`\  /'_` \  /'__`\ /'_` \
+#      ______\ \ \L\ \/\ \L\ \/\ \L\ \__  __//\ \L\ \
+#     /\  _  \\ \____/\ \____/\ \___,/\ \____\ \___,_\
+#     \ \ \L\ \\/_____ \/_____ \/____\/\/,_\_/______ /_ __    __    ____
+#      \ \  __ \/\ '__`\  /'__`\/\`'__\ \ \/ /\ \/\ \/\`'__\/'__`\ /',__\
+#       \ \ \/\ \ \ \L\ \/\  __/\ \ \/ \ \ \_\ \ \_\ \ \ \//\  __//\__, `\
+#        \ \_\ \_\ \ ,__/\ \____\\ \_\  \ \__\\ \____/\ \_\\ \____\/\____/
+#         \/_/\/_/\ \ \/  \/____/ \/_/   \/__/ \/___/  \/_/ \/____/\/___/
+#                  \ \_\
+#                   \/_/
 #
-#            a python package for generating coded apertures                                                                        
+#              a python package for generating coded apertures                                                                        
 #
-#                             MIT license
-#                    https://github.com/bpops/cappy
+#                               MIT license
+#                      https://github.com/bpops/cappy
 #
 
 from   commpy             import pnsequence
-import copy
 import numpy              as     np
 import matplotlib.pyplot  as     plt
 from   matplotlib.patches import RegularPolygon
 import pyprimes
 import random
 
 
@@ -336,15 +343,15 @@
         the number of times to tile the pattern in both dimensions
     quiet : bool
         if True, will print information about the array upon creation
     """
     
     def __init__(self, rank=5, quiet=False, mult=2):
         self.rank = rank
-        self.L = self.__get_prime(rank)
+        self.L = get_prime(rank)
         self.mult = mult
         
         # get r, s
         r = self.L
         s = self.L
         
         # generate C_r(I)
@@ -382,37 +389,14 @@
         
     def report(self):
         """
         Report on the mask information
         """
         print("Modified Uniformly Redundant Array")
         print(f"L: {self.L} (rank {self.rank})")
-        
-    def __get_prime(self, rank):
-        """
-        Determine prime of specified rank
-
-        Parameters
-        ----------
-        rank : int
-            the rank of prime pairs (0 -> 5, 1 -> 13, etc.)
-        """
-
-        assert rank >= 0, f"rank must be great than or equal to zero, got {rank}"
-
-        m = 1
-        this_rank = -1
-        while True:
-            L = 4*m + 1
-            if pyprimes.isprime(L):
-                this_rank += 1
-            if this_rank == rank:
-                break
-            m += 1
-        return L
     
     def show(self, inverse=False, size=8):
         """
         Plots the mask to the screen
 
         Parameters
         ----------
@@ -430,175 +414,423 @@
 
 class shura():
     """
     Skew-Hadamard Uniformly Redundant Array
 
     Parameters
     ----------
-    n : int
-        determines the order, v, where v=4n-1 (default 6)
+    rank : int
+        determines the order, v, a prime of the form v=4n-1 
+        (default 6)
     r : int
         feeds into pattern (default 5)
     quiet : bool
-        if True, will print information about the array upon creation
+        if True, will not print information about the array upon creation
     """
 
-    def __init__(self, n=6, r=5, radius=5, quiet=False):
-        self.n    = n
+    def __init__(self, rank=4, r=5, radius=5, quiet=False):
+        self.rank = rank
+        self.v    = self.get_order(self.rank)
+        self.n    = int((self.v+1)/4)
         self.r    = r
 
         # calculate mask size
         self.radius       = radius
         self.diam         = self.radius*2+1
         self.side_width   = radius + 1
 
         # create axial matrix
         self.axial_matrix = np.zeros((self.diam,self.diam))
         self.loc_matrix   = np.zeros((2,self.diam,self.diam))
 
         # calculate intermediates
-        self.v   = 4*n-1
-        self.k   = 2*n-1
-        self.lam = n-1
+        self.v   = 4*self.n-1
+        self.k   = 2*self.n-1
+        self.lam = self.n-1
 
         # construct cyclic difference set D
         self.D = np.zeros((int((self.v-1)/2)), dtype=np.int32)
         for i in range(len(self.D)):
             self.D[i] = ((i+1)**2) % self.v
 
         # determine labels
         self.rx = self.diam
         self.ry = self.diam
-        self.l = np.zeros((self.rx,self.ry))
+        self.l = np.zeros((self.rx,self.ry), dtype=np.int16)
         for i in range(self.rx):
             for j in range(self.ry):
                 self.l[i,j] = (i + r*j) % self.v
 
         # calculate mask
-        self.mask = np.zeros(self.l.shape)
+        self.mask = np.zeros(self.l.shape, dtype=np.int16)
         for i in range(self.mask.shape[0]):
             for j in range(self.mask.shape[1]):
                 if self.l[i,j] in self.D:
                     self.mask[i,j] = 1
 
         # map to axial matrix
         for i in range(self.diam):
             for j in range(self.diam):
                 if (i+j > (self.radius-1)) and (i+j < (self.diam+self.radius)):
-                    # TODO: this next line should not work correctly. 
-                    # WHY does it work?
                     self.axial_matrix[i,j] = self.mask[i,j]
                 else:
                     self.axial_matrix[i,j] = np.nan
 
         if not quiet: self.report()
 
+    def get_order(self,rank):
+        """
+        Determine order from the given rank, n. Order is defined
+        as a prime satisfying the condition v=4n-1
+
+        Parameters
+        ----------
+        rank : int
+            rank; atleast 1
+
+        Returns
+        -------
+        v : int
+            prime order
+        """
+        
+        n = 1
+        this_rank = -1
+        while True:
+            v = 4*n - 1
+            if pyprimes.isprime(v):
+                this_rank += 1
+            if this_rank == rank:
+                break
+            n += 1
+        return v
+
     def report(self):
         """
         Report the array info
         """
         print("Skew-Hadamard Uniformly Redundant Array")
-        print(f"n: {self.n}")
-        print(f"order (v): {self.v}")
-        print(f"k: {self.k}")
-        print(f"lambda: {self.lam}")
-        print(f"r: {self.r}")
-        print(f"side: {self.side_width}")
+        print(f"rank:       {self.rank}")
+        print(f"n:          {self.n}")
+        print(f"order (v):  {self.v}")
+        print(f"k:          {self.k}")
+        print(f"lambda:     {self.lam}")
+        print(f"r:          {self.r}")
+        print(f"side width: {self.side_width}")
   
-    def show_rhombus(self):
+    def show_rhombus(self, labels=False, labelsize=10):
         """
         Plot the mask rhombus
-        """
 
-        # determine open/closed pixels
-        pix_close  = np.where(self.mask == 1)
-        pix_open   = np.where(self.mask == 0)
-        
-        # determine open/closed pixels
-        x_closed = pix_close[0]
-        y_closed = pix_close[1]
-        x_opened = pix_open[0]
-        y_opened = pix_open[1]
+        Parameters
+        ----------
+        labels : bool
+            if True, will show the labels on top of each pixel
+        labelsize: int
+            fontsize for labels
+        """
 
+        # determine hex vertex-to-vertex and radius
         hex_vert = 1/(np.sqrt(3)/2)
         hex_radius = (hex_vert)/2.0
 
+        # set up plotting
         fig, ax = plt.subplots(1)
         ax.set_aspect('equal')
 
-        # closed pixels
-        for x, y in zip (x_closed, y_closed):
+        for x_i in range(self.mask.shape[0]):
+            for y_i in range(self.mask.shape[1]):
 
-            # determine patch origin
-            x += y * 0.5
-            y *= 1/hex_vert
-
-            # recenter
-            x -= (self.mask.shape[0] + self.mask.shape[1]/2.0)/2.0 -1/hex_vert
-            y -= (self.mask.shape[1] * 1/hex_vert)/2.0
-
-            # add hexagon
-            hex = RegularPolygon((x, y), numVertices=6, radius=hex_radius, 
-                                    orientation=np.radians(60), 
-                                    facecolor='k', alpha=0.6, edgecolor='k')
-            ax.add_patch(hex)
-
-        # open pixels
-        for x, y in zip (x_opened, y_opened):
-
-            # determine patch origin
-            x += y * 0.5
-            y *= np.sqrt(3)/2
-
-            # recenter
-            x -= (self.mask.shape[0] + self.mask.shape[1]/2.0)/2.0 -1/hex_vert
-            y -= (self.mask.shape[1] * 1/hex_vert)/2.0
-
-            # add hexagon
-            hex = RegularPolygon((x, y), numVertices=6, radius=hex_radius, 
-                                    orientation=np.radians(60), 
-                                    facecolor='w', alpha=0.2, edgecolor='k')
-            ax.add_patch(hex)
+                # determine patch origin
+                x = x_i + y_i * 0.5
+                y = y_i/hex_vert  
+
+                # recenter
+                x -= (self.mask.shape[0] + self.mask.shape[1]/2.0)/2.0 -1/hex_vert
+                y -= (self.mask.shape[1] * 1/hex_vert)/2.0 - hex_vert/2.0
+
+                # add hexagon
+                if self.mask[x_i,y_i] == 1:
+                    facecolor='k'
+                else:
+                    facecolor='w'
+                hex = RegularPolygon((x, y), numVertices=6, radius=hex_radius, 
+                              orientation=np.radians(60), 
+                               facecolor=facecolor, alpha=0.6, edgecolor='k')
+                ax.add_patch(hex)
+
+                # add label
+                if labels:
+                    plt.annotate(self.l[x_i,y_i], (x,y),
+                                 ha='center',va='center', fontsize=labelsize,
+                                 transform=ax.transAxes)
 
         plt.xlim(-self.rx/1.2,self.rx/1.2)
         plt.ylim(-self.ry/2.0,self.ry/2.0)
         plt.title(f"SHURA rhombus [o:{self.v}, r:{self.r}]")
         plt.show()
 
-    def show(self):
+    def show(self, labels=False, labelsize=10):
         """
         Plot the mask
+
+        Parameters
+        ----------
+        labels : bool
+            if True, will show the labels on top of each pixel
+        labelsize: int
+            fontsize for labels
         """
 
         # set up plot parameters
         fig, ax = plt.subplots(1)
         ax.set_aspect('equal')
         hex_width = 1.0 # face-to-face distance
         hex_vert  = (hex_width)*(2.0/np.sqrt(3))
 
         # draw hexagon array
         for y in range(self.diam):
             row_width = self.diam - abs(self.radius-y)
             start_i   = np.max((self.radius-y,0))
             for x in range(row_width):
                 facecolor = 'k' if self.axial_matrix[x+start_i,y] == 1 else 'w'
-                alpha     = 0.6 if self.axial_matrix[x+start_i,y] == 1 else 0.3
+                alpha     = 0.9 if self.axial_matrix[x+start_i,y] == 1 else 0.3
+                label     = self.l[x+start_i,y]
                 hex = RegularPolygon((x+0.5*abs(y-self.radius)-self.radius,
                                       ((y-self.radius)*((3/2)*hex_vert/2.0))),
                                      numVertices=6, radius=hex_vert/2.0, 
                                      orientation=np.radians(60), 
-                                     facecolor=facecolor, alpha=alpha, edgecolor='k')
+                                     facecolor=facecolor, alpha=alpha,
+                                     edgecolor='k')
                 ax.add_patch(hex)
+                if labels:
+                    plt.annotate(label, (x+0.5*abs(y-self.radius)-self.radius,
+                                         (y-self.radius)*((3/2)*hex_vert/2.0)),
+                                 ha='center',va='center', fontsize=labelsize,
+                                 transform=ax.transAxes)
 
         # set axis limits
         plt.xlim(-self.radius*hex_vert,self.radius*hex_vert)
         plt.ylim(-self.radius,self.radius)
         plt.title(f"SHURA [o:{self.v}, r:{self.r}]")
         plt.show()
 
+class hura():
+    """
+    Hexagonal Uniformly Redundant Array
+
+    Parameters
+    ----------
+    rank : int
+        determines the order, v, a prime of the form 3 or 12n+7
+    quiet : bool
+        if True, will not print information about the array upon creation
+    """
+
+    def __init__(self, rank=4, radius=5, quiet=False):
+        self.rank = rank
+        self.v    = self.get_order_from_rank(self.rank)
+        self.n    = int((self.v-7)/12)
+        self.r    = self.get_valid_r()
+
+        # calculate mask size
+        self.radius       = radius
+        self.diam         = self.radius*2+1
+        self.side_width   = radius + 1
+
+        # create axial matrix
+        self.axial_matrix = np.zeros((self.diam,self.diam))
+        self.loc_matrix   = np.zeros((2,self.diam,self.diam))
+
+        # calculate intermediates
+        self.k   = 2*self.n-1
+        self.lam = self.n-1
+
+        # construct cyclic difference set D
+        self.D = np.zeros((int((self.v-1)/2)), dtype=np.int32)
+        for i in range(len(self.D)):
+            self.D[i] = ((i+1)**2) % self.v
+
+        # determine labels
+        self.rx = self.diam
+        self.ry = self.diam
+        self.l = np.zeros((self.rx,self.ry), dtype=np.int16)
+        for i in range(self.rx):
+            for j in range(self.ry):
+                self.l[i,j] = (i + self.r*j) % self.v
+
+        # calculate mask
+        self.mask = np.zeros(self.l.shape, dtype=np.int16)
+        for i in range(self.mask.shape[0]):
+            for j in range(self.mask.shape[1]):
+                if self.l[i,j] in self.D:
+                    self.mask[i,j] = 1
+
+        # map to axial matrix
+        for i in range(self.diam):
+            for j in range(self.diam):
+                if (i+j > (self.radius-1)) and (i+j < (self.diam+self.radius)):
+                    self.axial_matrix[i,j] = self.mask[i,j]
+                else:
+                    self.axial_matrix[i,j] = np.nan
+
+        if not quiet: self.report()
+
+    def get_order_from_rank(self, rank):
+        """
+        Get the Order, v, from specified rank
+
+        Parameters
+        ----------
+        rank : int
+            rank, or nth order that satisfies 12n+7
+        """
+        if rank == 0:
+            return 3
+        else:
+            n = 0
+            this_rank = -1
+            while True:
+                v = 12*n +7
+                if pyprimes.isprime(v):
+                    this_rank += 1
+                if this_rank == rank:
+                    break
+                n += 1
+        return v
+    
+    def get_valid_r(self):
+        """
+        Determines the valid r from v
+
+        Returns
+        r : int
+            the value that satifies r**2 % v == (r-1) % v
+        """
+
+        r_not_found = True;
+        r = 0
+        while r_not_found:
+            if (r**2 % self.v) == ((r-1) % self.v):
+                r_not_found = False
+                break
+            r += 1
+        return r
+
+    def report(self):
+        """
+        Report the array info
+        """
+        print("Hexagonal Uniformly Redundant Array")
+        print(f"rank:       {self.rank}")
+        print(f"n:          {self.n}")
+        print(f"order (v):  {self.v}")
+        print(f"k:          {self.k}")
+        print(f"lambda:     {self.lam}")
+        print(f"r:          {self.r}")
+        print(f"side width: {self.side_width}")
+  
+    def show_rhombus(self, labels=False, labelsize=10):
+        """
+        Plot the mask rhombus
+
+        Parameters
+        ----------
+        labels : bool
+            if True, will show the labels on top of each pixel
+        labelsize: int
+            fontsize for labels
+        """
+
+        # determine hex vertex-to-vertex and radius
+        hex_vert = 1/(np.sqrt(3)/2)
+        hex_radius = (hex_vert)/2.0
+
+        # set up plotting
+        fig, ax = plt.subplots(1)
+        ax.set_aspect('equal')
+
+        for x_i in range(self.mask.shape[0]):
+            for y_i in range(self.mask.shape[1]):
+
+                # determine patch origin
+                x = x_i + y_i * 0.5
+                y = y_i/hex_vert  
+
+                # recenter
+                x -= (self.mask.shape[0] + self.mask.shape[1]/2.0)/2.0 -1/hex_vert
+                y -= (self.mask.shape[1] * 1/hex_vert)/2.0 - hex_vert/2.0
+
+                # add hexagon
+                if self.mask[x_i,y_i] == 1:
+                    facecolor='k'
+                else:
+                    facecolor='w'
+                hex = RegularPolygon((x, y), numVertices=6, radius=hex_radius, 
+                              orientation=np.radians(60), 
+                               facecolor=facecolor, alpha=0.6, edgecolor='k')
+                ax.add_patch(hex)
+
+                # add label
+                if labels:
+                    plt.annotate(self.l[x_i,y_i], (x,y),
+                                 ha='center',va='center', fontsize=labelsize,
+                                 transform=ax.transAxes)
+
+        plt.xlim(-self.rx/1.2,self.rx/1.2)
+        plt.ylim(-self.ry/2.0,self.ry/2.0)
+        plt.title(f"SHURA rhombus [o:{self.v}, r:{self.r}]")
+        plt.show()
+
+    def show(self, labels=False, labelsize=10):
+        """
+        Plot the mask
+
+        Parameters
+        ----------
+        labels : bool
+            if True, will show the labels on top of each pixel
+        labelsize: int
+            fontsize for labels
+        """
+
+        # set up plot parameters
+        fig, ax = plt.subplots(1)
+        ax.set_aspect('equal')
+        hex_width = 1.0 # face-to-face distance
+        hex_vert  = (hex_width)*(2.0/np.sqrt(3))
+
+        # draw hexagon array
+        for y in range(self.diam):
+            row_width = self.diam - abs(self.radius-y)
+            start_i   = np.max((self.radius-y,0))
+            for x in range(row_width):
+                facecolor = 'k' if self.axial_matrix[x+start_i,y] == 1 else 'w'
+                alpha     = 0.9 if self.axial_matrix[x+start_i,y] == 1 else 0.3
+                label     = self.l[x+start_i,y]
+                hex = RegularPolygon((x+0.5*abs(y-self.radius)-self.radius,
+                                      ((y-self.radius)*((3/2)*hex_vert/2.0))),
+                                     numVertices=6, radius=hex_vert/2.0, 
+                                     orientation=np.radians(60), 
+                                     facecolor=facecolor, alpha=alpha,
+                                     edgecolor='k')
+                ax.add_patch(hex)
+                if labels:
+                    plt.annotate(label, (x+0.5*abs(y-self.radius)-self.radius,
+                                         (y-self.radius)*((3/2)*hex_vert/2.0)),
+                                 ha='center',va='center', fontsize=labelsize,
+                                 transform=ax.transAxes)
+
+        # set axis limits
+        plt.xlim(-self.radius*hex_vert,self.radius*hex_vert)
+        plt.ylim(-self.radius,self.radius)
+        plt.title(f"HURA [o:{self.v}, r:{self.r}]")
+        plt.show()
+            
+
 class rand_hex():
     """
     Random Hexagonal Array
 
     Parameters
     ----------
     radius: int
@@ -640,19 +872,19 @@
         if not quiet: self.report()
 
     def report(self):
         """
         Report the array info
         """
         print("Random Hexagonal Array")
-        print(f"radius: {self.radius}")
-        print(f"diameter: {self.diam}")
-        print(f"side_width: {self.side_width}")
-        print(f"desired fill factor: {self.fill:.2f}")
-        print(f"actual  fill factor: {self.actual_fill:.2f}")
+        print(f"radius:       {self.radius}")
+        print(f"diameter:     {self.diam}")
+        print(f"side width:   {self.side_width}")
+        print(f"desired fill: {self.fill:.2f}")
+        print(f"actual  fill: {self.actual_fill:.2f}")
 
     def show(self):
         """
         Plot the mask
         """
 
         # set up plot parameters
@@ -668,15 +900,16 @@
             for x in range(row_width):
                 facecolor = 'k' if self.axial_matrix[x+start_i,y] == 1 else 'w'
                 alpha     = 0.6 if self.axial_matrix[x+start_i,y] == 1 else 0.3
                 hex = RegularPolygon((x+0.5*abs(y-self.radius)-self.radius,
                                       ((y-self.radius)*((3/2)*hex_vert/2.0))),
                                      numVertices=6, radius=hex_vert/2.0, 
                                      orientation=np.radians(60), 
-                                     facecolor=facecolor, alpha=alpha, edgecolor='k')
+                                     facecolor=facecolor, alpha=alpha,
+                                     edgecolor='k')
                 ax.add_patch(hex)
 
         # set axis limits
         plt.xlim(-self.radius*hex_vert,self.radius*hex_vert)
         plt.ylim(-self.radius,self.radius)
         plt.title(f"Random Hex Array [diam: {self.diam}, fill: {self.actual_fill:.2f}]")
         plt.show()
@@ -752,15 +985,15 @@
 def prim_poly(m):
     """
     Primitive Polynomial
 
     Parameters
     ----------
     m : int
-        degree
+        degree (between 1 and 40); large numbers will take a very long time
 
     Returns
     -------
     pnsequence : ndarray
         a pseudo-random sequence satisfying the primitive polynomial of the
         degree specified
     """
@@ -788,8 +1021,31 @@
     for i in h_x[m]:
         mask[m-i-1] = 1
 
     # initialize seed to match results from [MacWilliams 1976]
     seed = np.zeros(m)
     seed[0] = 1
 
-    return pnsequence(m,seed,mask,2**m-1)
+    return pnsequence(m,seed,mask,2**m-1)
+
+def get_prime(rank):
+    """
+    Determine prime of specified rank
+
+    Parameters
+    ----------
+    rank : int
+        the rank of the prime number
+    """
+
+    assert rank >= 0, f"rank must be great than or equal to zero, got {rank}"
+
+    m = 1
+    this_rank = -1
+    while True:
+        L = 4*m + 1
+        if pyprimes.isprime(L):
+            this_rank += 1
+        if this_rank == rank:
+            break
+        m += 1
+    return L
```

### Comparing `codedapertures-0.6/codedapertures.egg-info/PKG-INFO` & `codedapertures-0.7/codedapertures.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedapertures
-Version: 0.6
+Version: 0.7
 Summary: a python package for generating coded apertures
 Home-page: https://github.com/bpops/codedapertures
 Author: bpops
 License: MIT
 License-File: LICENSE
 
 CodedApertures is a python package that allows one to easily generate and display common coded aperture patterns. Coded apertures are a spatial encoding technique for straight-line optics, wherein traditional lensing (e.g., visible light) is not possible. Even wherein tradiational lensing is possible, there may be other advantages (infinite depth of field). Coded apertures may therefore be used for hard x-ray and gamma-ray imaging for astrophysics, medical imaging, and homeland security applications.
```

### Comparing `codedapertures-0.6/setup.py` & `codedapertures-0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 setuptools.setup(name='codedapertures',
-      version='0.6',
+      version='0.7',
       description='a python package for generating coded apertures',
       long_description='CodedApertures is a python package that allows one to easily generate and display common coded aperture patterns. Coded apertures are a spatial encoding technique for straight-line optics, wherein traditional lensing (e.g., visible light) is not possible. Even wherein tradiational lensing is possible, there may be other advantages (infinite depth of field). Coded apertures may therefore be used for hard x-ray and gamma-ray imaging for astrophysics, medical imaging, and homeland security applications.',
       url='https://github.com/bpops/codedapertures',
       author='bpops',
       license='MIT',
       install_requires=['pyprimes',
                 'numpy',
```

