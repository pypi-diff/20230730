# Comparing `tmp/aksharify-0.1.9.tar.gz` & `tmp/aksharify-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aksharify-0.1.9.tar", max compression
+gzip compressed data, was "aksharify-0.2.0.tar", max compression
```

## Comparing `aksharify-0.1.9.tar` & `aksharify-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1094 2023-07-22 05:33:48.477839 aksharify-0.1.9/LICENSE.md
--rw-r--r--   0        0        0      674 2023-07-27 05:39:03.743172 aksharify-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     5977 2023-07-26 18:35:45.363211 aksharify-0.1.9/README.md
--rw-r--r--   0        0        0       63 2023-07-26 19:10:39.011428 aksharify-0.1.9/src/aksharify/__init__.py
--rw-r--r--   0        0        0     5632 2023-07-26 09:23:20.805879 aksharify-0.1.9/src/aksharify/aksharify.py
--rw-r--r--   0        0        0     5327 2023-07-25 04:07:23.752855 aksharify-0.1.9/src/aksharify/distributions.py
--rw-r--r--   0        0        0     1615 2023-07-24 16:06:14.067631 aksharify-0.1.9/src/aksharify/image.py
--rw-r--r--   0        0        0     1191 2023-07-25 06:47:53.889912 aksharify-0.1.9/src/aksharify/interactive.py
--rw-r--r--   0        0        0     4946 2023-07-24 12:43:24.100266 aksharify-0.1.9/src/aksharify/outputs.py
--rw-r--r--   0        0        0     6648 1970-01-01 00:00:00.000000 aksharify-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-07-22 05:33:48.477839 aksharify-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0      691 2023-07-30 07:41:52.449997 aksharify-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5977 2023-07-26 18:35:45.363211 aksharify-0.2.0/README.md
+-rw-r--r--   0        0        0     1828 2023-07-27 09:55:42.412864 aksharify-0.2.0/src/aksharify/.ipynb_checkpoints/image-checkpoint.py
+-rw-r--r--   0        0        0       72 2023-07-30 07:32:06.237127 aksharify-0.2.0/src/aksharify/__init__.py
+-rw-r--r--   0        0        0     6542 2023-07-29 16:43:30.891830 aksharify-0.2.0/src/aksharify/aksharify.py
+-rw-r--r--   0        0        0     5550 2023-07-30 04:53:04.214539 aksharify-0.2.0/src/aksharify/distributions.py
+-rw-r--r--   0        0        0     1828 2023-07-27 09:55:42.412864 aksharify-0.2.0/src/aksharify/image.py
+-rw-r--r--   0        0        0     4946 2023-07-24 12:43:24.100266 aksharify-0.2.0/src/aksharify/outputs.py
+-rw-r--r--   0        0        0     1788 2023-07-29 20:22:14.648987 aksharify-0.2.0/src/aksharify/paramestimators.py
+-rw-r--r--   0        0        0     6648 1970-01-01 00:00:00.000000 aksharify-0.2.0/PKG-INFO
```

### Comparing `aksharify-0.1.9/LICENSE.md` & `aksharify-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.9/pyproject.toml` & `aksharify-0.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "aksharify"
-version = "0.1.9"
+version = "0.2.0"
 description = "Ascii Art + Emoji Art python Package"
 authors = ["Prime Patel <primespatel@gmail.com>"]
 readme = "README.md"
 packages = [{include = "aksharify", from = "src"}]
 license = "MIT"
 homepage = "https://primepatel.github.io/aksharify/"
 repository = "https://github.com/primepatel/aksharify"
 keywords = ["Ascii Art","Emoji Art","Prime Patel","primepatel"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-pillow = "^8.4.0"
-scikit-image = "^0.19.3"
-matplotlib = "^3.7.1"
-cairosvg = "^2.7.0"
-ipython = "^7.34.0"
+pillow = "9.4.0"
+scikit-image = "0.19.3"
+matplotlib = "3.7.1"
+cairosvg = "2.7.0"
+ipython = "7.34.0"
+ipywidgets = "7.7.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `aksharify-0.1.9/README.md` & `aksharify-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.9/src/aksharify/aksharify.py` & `aksharify-0.2.0/src/aksharify/aksharify.py`

 * *Files 10% similar despite different names*

```diff
@@ -120,10 +120,37 @@
         svg2eps(file_obj=svg_io, write_to=eps.file_name + ".eps")
     
     def html_output(self, config):
         html = config
         with open(html.file_name + ".html", "w", encoding="utf-8") as file:
             file.write(html.generate_art(self.matrix, self.image.image))
 
+        
+class EdgeArt(AksharArt):
+    
+    def __init__(self, image, dist) -> None:
+        super().__init__(image, dist)
+        self.image = image
+        self.dist = dist
+        
+    def aksharify(self, bg_char=" ", show=False) -> None:
+        self.matrix = []
+        for x in range(self.image.edges.shape[0]):
+            line = []
+            for y in range(self.image.edges.shape[1]):
+                if self.image.edges[x, y]:
+                    line.append(self.dist.char_dict[int(self.image.bwimg[x, y]*255)])
+                else:
+                    line.append(bg_char)
+            self.matrix.append(line) 
+        if show:
+            self.show()
+    
+    def show(self):
+        svg = SVG()
+        svg.background_color = "#ffffff"
+        svg.fill_color = "#000000"
+        art = svg.generate_art(self.matrix, self.image.image)
+        ipd.display(ipd.SVG(art))
 
 def hexify(color:str):
     return cnames[color]
```

### Comparing `aksharify-0.1.9/src/aksharify/distributions.py` & `aksharify-0.2.0/src/aksharify/distributions.py`

 * *Files 14% similar despite different names*

```diff
@@ -85,27 +85,36 @@
 class Exponential(Linear):
     def __init__(self, chars="@%#*+=;:-,. ", power=1, order=False, unique=False) -> None:
         super().__init__(chars, order, unique)
         self.hex_to_normal()
         self.list = self.list**power
         self.normal_to_hex()
         self.y = lambda x: x**power
-        self.generate_char_dict()  
+        self.generate_char_dict()
+        self.a = -3
+        self.b = 3
+        self.s = 0.1
         
 class Normal(Linear):
     def __init__(self, chars="@%#*+=;:-,. ", mean=0.5, var=1, order=False, unique=False) -> None:
         super().__init__(chars, order, unique)
         self.mean = mean
         self.var = var
         self.hex_to_normal()
         self.list[0], self.list[-1] = 0.0001, 0.9999
         self.list = self.normalizer(self.list)
         self.normal_to_hex()
         self.y = self.normalizer
         self.generate_char_dict()
+        self.a_mean = 0.0001
+        self.b_mean = 0.9999
+        self.s_mean = 0.1
+        self.a_var = -3
+        self.b_var = 3
+        self.s_var = 0.1
     
     def normalizer(self, x):
         inv = (x*(1-self.mean))/(self.mean*(1-x))
         inv **= -self.var
         inv += 1
         return inv**(-1)
```

### Comparing `aksharify-0.1.9/src/aksharify/image.py` & `aksharify-0.2.0/src/aksharify/.ipynb_checkpoints/image-checkpoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,8 +39,15 @@
         else:
             w, h = width, height
         self.image = ski.transform.resize(self.obj, (h, w), anti_aliasing=True)
         self.bwimg = ski.color.rgb2gray(self.image[:,:,:3])
     
     def normalize(self):
         self.bwimg = np.subtract(self.bwimg, np.min(self.bwimg))
-        self.bwimg = np.divide(self.bwimg, np.max(self.bwimg))
+        self.bwimg = np.divide(self.bwimg, np.max(self.bwimg))
+    
+    def edgefy(self, show=False):
+        self.edges = ski.feature.canny(self.bwimg)
+        if show:
+            plt.axis('off')
+            plt.imshow(self.edges, cmap='gray')
+            plt.show()
```

### Comparing `aksharify-0.1.9/src/aksharify/outputs.py` & `aksharify-0.2.0/src/aksharify/outputs.py`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.9/PKG-INFO` & `aksharify-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: aksharify
-Version: 0.1.9
+Version: 0.2.0
 Summary: Ascii Art + Emoji Art python Package
 Home-page: https://primepatel.github.io/aksharify/
 License: MIT
 Keywords: Ascii Art,Emoji Art,Prime Patel,primepatel
 Author: Prime Patel
 Author-email: primespatel@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: cairosvg (>=2.7.0,<3.0.0)
-Requires-Dist: ipython (>=7.34.0,<8.0.0)
-Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
-Requires-Dist: pillow (>=8.4.0,<9.0.0)
-Requires-Dist: scikit-image (>=0.19.3,<0.20.0)
+Requires-Dist: cairosvg (==2.7.0)
+Requires-Dist: ipython (==7.34.0)
+Requires-Dist: ipywidgets (==7.7.1)
+Requires-Dist: matplotlib (==3.7.1)
+Requires-Dist: pillow (==9.4.0)
+Requires-Dist: scikit-image (==0.19.3)
 Project-URL: Repository, https://github.com/primepatel/aksharify
 Description-Content-Type: text/markdown
 
 <a name="readme-top"></a>
 
 # __Aksharify__
```

