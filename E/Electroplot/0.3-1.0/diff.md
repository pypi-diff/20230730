# Comparing `tmp/Electroplot-0.3.tar.gz` & `tmp/Electroplot-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Electroplot-0.3.tar", last modified: Tue Jul  6 17:15:20 2021, max compression
+gzip compressed data, was "dist\Electroplot-1.0.tar", last modified: Sun Jul 30 14:59:25 2023, max compression
```

## Comparing `Electroplot-0.3.tar` & `Electroplot-1.0.tar`

### file list

```diff
@@ -1,30 +1,22 @@
-drwxrwxrwx   0        0        0        0 2021-07-06 17:15:19.000000 Electroplot-0.3/
-drwxrwxrwx   0        0        0        0 2021-07-06 17:15:19.000000 Electroplot-0.3/Electroplot/
--rw-rw-rw-   0        0        0    14147 2020-11-28 16:34:06.000000 Electroplot-0.3/Electroplot/Electroplot.py
-drwxrwxrwx   0        0        0        0 2021-07-06 17:15:19.000000 Electroplot-0.3/Electroplot/Functions/
--rw-rw-rw-   0        0        0     3739 2020-09-26 14:30:38.000000 Electroplot-0.3/Electroplot/Functions/Arranger.py
--rw-rw-rw-   0        0        0      715 2020-07-09 22:07:26.000000 Electroplot-0.3/Electroplot/Functions/Graphical.py
--rw-rw-rw-   0        0        0        0 2020-07-09 22:07:26.000000 Electroplot-0.3/Electroplot/Functions/__init__.py
--rw-rw-rw-   0        0        0     3730 2020-11-28 13:23:56.000000 Electroplot-0.3/Electroplot/Functions/dataGrabber.py
--rw-rw-rw-   0        0        0     1721 2020-08-19 11:21:20.000000 Electroplot-0.3/Electroplot/Functions/masks.py
--rw-rw-rw-   0        0        0     4757 2020-11-28 16:35:40.000000 Electroplot-0.3/Electroplot/Functions/maths.py
--rw-rw-rw-   0        0        0      857 2020-11-28 13:33:42.000000 Electroplot-0.3/Electroplot/Functions/threadingtest.py
--rw-rw-rw-   0        0        0        0 2020-07-09 22:07:26.000000 Electroplot-0.3/Electroplot/__init__.py
--rw-rw-rw-   0        0        0     1619 2020-11-28 18:11:22.000000 Electroplot-0.3/Electroplot/testnov.py
-drwxrwxrwx   0        0        0        0 2021-07-06 17:15:19.000000 Electroplot-0.3/Electroplot/tests/
--rw-rw-rw-   0        0        0       36 2020-11-28 12:19:36.000000 Electroplot-0.3/Electroplot/tests/#testnov.py
--rw-rw-rw-   0        0        0        0 2020-09-26 11:09:46.000000 Electroplot-0.3/Electroplot/tests/__init__.py
--rw-rw-rw-   0        0        0     4281 2020-07-15 23:54:16.000000 Electroplot-0.3/Electroplot/tests/cursortest.py
--rw-rw-rw-   0        0        0      172 2020-09-26 13:05:16.000000 Electroplot-0.3/Electroplot/tests/divisionTest.py
--rw-rw-rw-   0        0        0     6906 2020-11-28 12:27:26.000000 Electroplot-0.3/Electroplot/tests/example.py
--rw-rw-rw-   0        0        0      602 2020-11-28 18:40:06.000000 Electroplot-0.3/Electroplot/tests/microscope_emulator.py
-drwxrwxrwx   0        0        0        0 2021-07-06 17:15:19.000000 Electroplot-0.3/Electroplot.egg-info/
--rw-rw-rw-   0        0        0      727 2021-07-06 17:15:20.000000 Electroplot-0.3/Electroplot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      713 2021-07-06 17:15:20.000000 Electroplot-0.3/Electroplot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-07-06 17:15:20.000000 Electroplot-0.3/Electroplot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2021-07-06 17:15:20.000000 Electroplot-0.3/Electroplot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2021-07-06 17:15:20.000000 Electroplot-0.3/Electroplot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      727 2021-07-06 17:15:22.000000 Electroplot-0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2020-10-05 19:39:06.000000 Electroplot-0.3/README.md
--rw-rw-rw-   0        0        0       86 2021-07-06 17:15:22.000000 Electroplot-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1571 2021-07-06 17:15:08.000000 Electroplot-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:59:25.000000 Electroplot-1.0/
+drwxrwxrwx   0        0        0        0 2023-07-30 14:59:24.000000 Electroplot-1.0/Electroplot/
+-rw-rw-rw-   0        0        0    10772 2022-08-05 12:47:38.000000 Electroplot-1.0/Electroplot/Electroplot.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:59:25.000000 Electroplot-1.0/Electroplot/Functions/
+-rw-rw-rw-   0        0        0     3739 2022-08-02 14:32:14.000000 Electroplot-1.0/Electroplot/Functions/Arranger.py
+-rw-rw-rw-   0        0        0      715 2020-07-03 17:04:22.000000 Electroplot-1.0/Electroplot/Functions/Graphical.py
+-rw-rw-rw-   0        0        0        0 2020-07-03 17:04:22.000000 Electroplot-1.0/Electroplot/Functions/__init__.py
+-rw-rw-rw-   0        0        0     3058 2022-08-19 15:50:57.000000 Electroplot-1.0/Electroplot/Functions/dataGrabber.py
+-rw-rw-rw-   0        0        0     1802 2020-07-03 17:04:22.000000 Electroplot-1.0/Electroplot/Functions/masks.py
+-rw-rw-rw-   0        0        0     1354 2022-08-03 12:39:32.000000 Electroplot-1.0/Electroplot/Functions/models.py
+-rw-rw-rw-   0        0        0        0 2020-07-03 17:04:22.000000 Electroplot-1.0/Electroplot/__init__.py
+-rw-rw-rw-   0        0        0     3096 2023-07-28 08:10:51.000000 Electroplot-1.0/Electroplot/example.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:59:24.000000 Electroplot-1.0/Electroplot.egg-info/
+-rw-rw-rw-   0        0        0      727 2023-07-30 14:59:22.000000 Electroplot-1.0/Electroplot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      479 2023-07-30 14:59:23.000000 Electroplot-1.0/Electroplot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 14:59:22.000000 Electroplot-1.0/Electroplot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-07-30 14:59:22.000000 Electroplot-1.0/Electroplot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-30 14:59:22.000000 Electroplot-1.0/Electroplot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      727 2023-07-30 14:59:25.000000 Electroplot-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2020-10-05 19:39:06.000000 Electroplot-1.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-30 14:59:25.000000 Electroplot-1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1571 2023-07-30 14:57:56.000000 Electroplot-1.0/setup.py
```

### Comparing `Electroplot-0.3/Electroplot/Electroplot.py` & `Electroplot-1.0/Electroplot/Electroplot.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,205 +1,134 @@
 ## Electroplot.py
+
 import os
 from tifffile import TiffFile
 from tkinter import filedialog
 import numpy as np
-from Functions.dataGrabber import grabMetadata, grabImageJdata, grabData, tif2png
-#from Functions.masks import logTransform
+import numpy.ma as ma
+from Functions.dataGrabber import grabMetadata, grabTifdata, grabImageJdata, grabData, tif2png
+from Functions.masks import logTransform
 from matplotlib import pyplot as plt
+import matplotlib.patches as mpatches
 from Functions.masks import applyMask
-from PIL import Image
+
 import moviepy.editor as mp
 import Functions.Arranger as ar
-import Functions.maths
-import math
-from Misc.Errors import DatasetTypeError as DatasetTypeError
-import threading, queue
-from natsort import natsorted
-import concurrent.futures
-import time
-
-# Initialise the data to be analysed. 
-# example: condition1 = ep.Dataset('Control', imagetype = 'image')
-
 class Dataset(object):
-    def __init__(self, name, path = None, imagetype = 'stack', outputpath = None): 
-        self.name = name        #variable name of data set for internal reference
-        self.raw = []           #contains raw image data
-        self.data = []          #contains pixel values for image(s) as arrays
+    def __init__(self, name, path = None, imagetype = 'stack'): 
+        self.name = name
+        self.base = []
+        self.raw = []
+        self.stack = []
+        self.tifData = []
+        self.type = imagetype
+        self.base = []
+        self.map = []
         
-        self.type = imagetype   #property that describes whether dataset is a single image or an entire stack.
-        self.metadata = None    #metadata property declaration
-        self.outputpath = outputpath
-
-        if path == None:        # if no path to the dataset is specified then a filedialog is automatically created. 
+        if path == None: 
             if self.type == 'stack': 
-                self.path = filedialog.askdirectory()                      #if a stack asks to select a folder
+                self.path = filedialog.askdirectory()
             else: 
-                self.path = filedialog.askopenfilename()                   #if an image asks to select a file
+                self.path = filedialog.askopenfilename()
         else:
-            self.path = path                                               #if path argument specified skips above.
+            self.path = path 
 
-        if self.type == 'stack':
-            stack = os.listdir(self.path)
-            stack = natsorted(stack)
-            print(time.perf_counter())
-            with concurrent.futures.ThreadPoolExecutor() as executor:      #multithreaded image load
-                futures = [executor.submit(grabData, (self.path+'\\'+image)) for image in stack]
-            for f in futures: 
-                try:
-                    self.metadata = f.result()['ImageJ']
-                    self.data.append(f.result()['Pixels'])
-                except TypeError:
-                    pass
-            print(time.perf_counter())
-                
-                 
-            '''   
-            for f in futures:
-                print(type(f))
-                 
-            for f in futures:
-                print(f)
-                pass
-                #print(type(f.result[0]))
-            data = [f.result() for f in futures] 
-            print([data[1]])
-            #print(raw)
-            '''                      
-        else:                                                               # single image loading cycle
+        if self.type == 'stack':        
+            #print('loop test')   
+            for file in os.listdir(self.path):  
+                if file.endswith('.tiff') or file.endswith('.tif'):
+                    if file == 'map.tiff':
+                        self.raw = grabData(str(self.path + file))
+                        self.map.append(self.raw['Pixels'])
+                        print('map')
+                    #if file == 'map.tiff' or 'map.tif': 
+                    #    self.map = grabData(self.path + file)
+                    #print('test')
+                    #print(grabTifdata(str(self.path + file)))
+                    #print(grabTifdata(str(self.path + file)))
+                    #else:
+                    else:
+                        self.raw = grabData(str(self.path + file))
+                        #print(self.raw)
+                        self.metadata = self.raw['ImageJ']
+                        #self.metadata = None
+                        self.tifData.append(self.raw['Pixels'])
+                        self.base.append(grabTifdata(self.path + file))   
+                          
+        else:
             self.raw = grabData(str(self.path))
-            for item in self.raw['Pixels']:
-                if item == None:                                            #skips Nones
-                    pass
-                else:
-                    self.data.append(item) 
-            self.size = len(self.data)
-            try:
-                self.metadata = self.raw['ImageJ']                          #if 'ImageJ' metadata non-existent, skips this step. 
-            except TypeError:
-                pass
-        
-        if self.metadata == None:
-            print('Warn: no metadata detected in dataset')        
-            
-            
-        self.size = len(self.data)
-        self.data = np.array(self.data)                         #convert self.data from list to numpy array
-        self.previous = self.data                               #establish back ups for undo and reset
-        self.original = self.data
-        
-        #Error Catching
-        a  = TypeError('the Electroplot dataset <' + str(self.name) + '> is an ' + str(self.type) + ' and cannot be divided.'), 
-        self.errorParams = [a]
-        
-        print('Successfully loaded data at ' + str(self.path) + ' into a dataset object')
-    
-    
-    def mask(self, threshold = 1000, masktype = 'edges' ): 
-        self.previous = self.data
+            #print(self.raw)
+            self.tifData.append(self.raw['Pixels'])
+            self.metadata = self.raw['ImageJ']
+            self.base = grabTifdata(self.path)
+
+    def applyMask(self, threshold, masktype = 'edges', show = False): 
         if self.type == 'stack':
-            masked = applyMask(self.data, threshold, masktype)
-            self.data = masked
-            return masked
-                
+            for image in os.listdir(self.path):
+                masked = applyMask(image, threshold, masktype, show)
+                image = masked 
+        else:
+            masked = applyMask(self.path, threshold, masktype, show)
+            self.tifData = masked
+    def transform(self, transformer, *args):
+        if self.type == 'stack':
+            for i in self.tifData:
+                output = transformer(i, *args)
         elif self.type == 'image':
-            
-            masked = applyMask(self.data, threshold, masktype)
-            self.data = masked
-            return masked
-    #note: on image datasets stacks cannot be passed as operators
-    #Divide the dataset by either another stack, another image, or a determined value.
-    def divide(self, divider):                              
-        self.previous = self.data
-        divided = Functions.maths.datasetOperation(self.data, operator = divider, operation='divide' )
-        self.data = divided
-        return divided
-      
-    #Multiply the dataset by either another stack, another image, or a determined value.
-    def multiply(self, multiplier):
-        self.previous = self.data
-        multiplied = Functions.maths.datasetOperation(self.data, operator = multiplier, operation = 'multiply')
-        self.data = multiplied
-        return multiplied
-    
-    #Add another stack, image or value to the dataset.
-    def add(self, multiplier):
-        self.previous = self.data
-        summed = Functions.maths.datasetOperation(self.data, operator = multiplier, operation = 'addition')
-        self.data = summed
-        return summed
-    
-    #Subtract another stack, image or value from the dataset
-    def subtract(self, multiplier):
-        self.previous = self.data
-        subtracted = Functions.maths.datasetOperation(self.data, operator = multiplier, operation = 'subtract')
-        self.data = subtracted
-        return subtracted
-                
-    def transform(self, transformer, *args): #need to add rotation
-        #add rotation code
-        return("transformation code still needs adding.")
-    def undo(self):
-        self.data = self.previous
-        return("Last operation on dataset undone.")
+            output = transformer(self.tifData, *args)
+        return output
     
-    def wipe(self):
-        self.data = self.original
-        return ("Dataset wiped back to origin.")
-    
-    def getZprofile(self, plot = True, mask = None):
+    def getZprofile(self, plot = False, mask = None):
         zprofile = []
         i = 0
         if self.type == 'stack': 
             if mask == None: 
-                for image in self.data: 
+                for image in self.tifData: 
                     zprofile.append(np.average(image))
             elif mask == 'log':
-                    zprofile.append(logTransform(self.data, 10))
+                    zprofile.append(logTransform(self.tifData, 10))
+            elif mask == 'map':
+                tifDat = np.array(self.tifData)
+                map = np.array(self.map, dtype = bool)
+                for image in tifDat: 
+                    mx = ma.masked_array(image, mask=~map)
+                    zprofile.append(mx.mean())
+                    
             else: 
                 print('bork')
+
+                            
+                
                     #process(self.data['Pixels'], **kwargs           
         else: 
             zprofile = print('getZprofile: This dataset is a' + str(self.type) + ', not a stack!')
         if plot == True:
-            plot = plt.plot(zprofile)
+            x = np.arange(0, len(self.tifData), 1)
+            xtick = np.arange(0, len(self.tifData)+1, 5)
+            
+            plt.xlabel("Frames")
+            plt.ylabel("Fluorescence (A.U.)")
+            plt.title("Time series of " +str(self.name))
+            minYAxis=(min(zprofile)-50)
+            maxYAxis=(max(zprofile)+50)
+            YaxisDiff = maxYAxis - minYAxis
+            plt.xticks(xtick)
+            rect=mpatches.Rectangle((15,minYAxis),2.5,YaxisDiff, 
+                        fill = True,
+                        color = "yellow",
+                        linewidth = 2)
+            plt.gca().add_patch(rect)
+            plot = plt.plot(x, zprofile)
+            plt.show()
+            
             zprofileplot = plt.savefig('zprofile.png')
-            return zprofileplot
+            return plot
         else:
             return zprofile
-    
-    def visualise(self):
-        img = Image.fromarray(self.data[0], 'I;16')
-        img.show()
-    
-    def save(self, path = None, format = '.TIF'):
-        #if self.outputpath == None: 
-        #    self.outputpath = filedialog.askdirectory()
-        if path == None:
-            path = filedialog.askdirectory()
-        try:
-            os.makedirs(path)
-        except OSError as e:
-            #specific error catch
-            pass
-        if self.type == 'stack':
-            iterator = 0
-            for array in self.data: 
-                iterator +=1
-                image = Image.fromarray(array, 'I;16')
-                image.save(path + str(self.name) + str(iterator) + str(format))
-            return(str(len(self.data)) + '.TIF images were saved at ' + str(self.outputpath))   
-        elif self.type == 'image':
-            image = Image.fromarray(self.data, 'I;16')
-            
-        else: 
-            raise DatasetTypeError('Dataset type not found! Consider reloading data', self.type)
-        #return(str(format) + )
-        
+
 class Figure(): 
     def __init__(self, name, *datasets, rows = None, columns = None, duration = None ):
         #initialise containers for subfigure objects and positional array
         subfigures = []                                         
         positions = []
         total = int
         
@@ -210,15 +139,15 @@
             columns = 1
         if total != rows * columns:
             Exception('the total number of subfigures is out of bounds!')
         
         #create subfigures from datasets, and append to array
         for i in datasets:
             subfigure = ar.subFigure(i, i.name, 
-                                i.data, 
+                                i.tifData, 
                                 i.metadata,
                                 )
             subfigures.append(subfigure)
         self.subfigures = np.array(subfigures)
         
         #figure parameter dictionary (base)
         self.figureParams = {   'name' : name,
```

### Comparing `Electroplot-0.3/Electroplot/Functions/Arranger.py` & `Electroplot-1.0/Electroplot/Functions/Arranger.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,26 +31,26 @@
         except FileExistsError:
             print(self.images)
             for i in os.listdir(self.temp_path):
                 print(i)
             print("Files found at " + str(self.temp_path))
             pass
               
-    def makeSubfigure(self, fps , duration):
+    def makeSubfigure(self, fps, duration):
         if self.subtype == 'image':
             plot = plt.plot(self.images)
             if self.epObjects.type == 'stack':
                 #print(self.images)
                 image = os.listdir(self.images)[1]
                 print(self.temp_path)
                 print(image)
                 print(self.temp_path + image)
                 
                 self.clip = mp.ImageClip(self.temp_path + image).set_duration(duration)
-            elif self.epObjects.type == 'image':
+            elif self.epoObjects.type == 'image':
                 print('image success')
                 self.clip = mp.ImageClip(self.images)
                 
                 self.clip = self.clip.set_duration(10)
                 
         elif self.subtype == 'movie': #makes movie --working
             self.clip = mp.ImageSequenceClip(self.images, fps, load_images = True, with_mask = False)
```

### Comparing `Electroplot-0.3/Electroplot/Functions/Graphical.py` & `Electroplot-1.0/Electroplot/Functions/Graphical.py`

 * *Files identical despite different names*

### Comparing `Electroplot-0.3/Electroplot/Functions/masks.py` & `Electroplot-1.0/Electroplot/Functions/masks.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,62 @@
 # masks.py -> write custom mask functions for the z-profile
-import skimage
 from skimage import io
 from skimage import feature
 from skimage.filters import sobel
 from skimage.exposure import histogram
 import numpy as np
 # logarithm 
 from scipy import ndimage as ndi
 from skimage.segmentation import watershed
 import matplotlib.pyplot as plt
 
 def applyMask(image, threshold = 1500, masktype = 'edges', show = False):
-    if masktype == 'edges': 
-        image = image[0]
-        edges = feature.canny(image/threshold)  
-        print(edges)
+    if masktype == 'edges':
+        im = io.imread(image)
+        edges = feature.canny(im/threshold)  
         mask = ndi.binary_fill_holes(edges)
-        print(mask)
-        
-        combined = mask * image
-        print(combined)
-        
-        return mask
+        combined = mask * im
+        if show == True: 
+            io.imshow(combined)
+            io.show()  
+
     elif masktype == 'region': 
-        im = image[0]
-        #hist, hist_centers = histogram(im)
-        #print(hist)
-        #plt.plot(hist)
-        #plt.show()
+        im = io.imread(image)
+        hist, hist_centers = histogram(im)
+        print(hist)
+        plt.plot(hist)
+        plt.show()
         elevation_map = sobel(im)
         markers = np.zeros_like(im)
-        markers[im < 100] = 1
-        markers[im > 4000] = 2 
+        markers[im < 30] = 1
+        markers[im > 1500] = 2 
         segmentation = watershed(elevation_map)
         segmentation = ndi.binary_fill_holes(segmentation - 1)
-        #io.imshow(segmentation)
-        #io.show()
-        return segmentation
+        io.imshow(segmentation)
+        io.show()
+
     elif masktype == 'electrode':
-        for i in image[0]:
-            if i == 'test':
-                print(str(masktype))
+        print(str(masktype))
 
     elif masktype == 'hyperpolarised':
         print(str(masktype))
 
     elif masktype == 'depolarised':
         print(str(masktype))
 
     else:
         raise Exception("< 'masktype = " + str(masktype) + " > \n unknown mask type, choose from 'edges', 'electrode', 'hyperpolarise', 'depolarise' ")
     
     return combined
 
+def logTransform(stack, divframe):
+    #stack = stack / stack[divframe]
+    out = []
+    for image in stack: 
+        image = image / stack[divframe]
+        out.append(np.log(image))
+    
+    return out
```

### Comparing `Electroplot-0.3/Electroplot.egg-info/PKG-INFO` & `Electroplot-1.0/Electroplot.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: Electroplot
-Version: 0.3
+Version: 1.0
 Summary: Handling TIFF files and figure generation from timelapse experiments.
 Home-page: https://github.com/ConorEd/
 Author: Conor Edwards
 Author-email: conorlo@hotmail.co.uk
 License: MIT
 Description: UNKNOWN
 Keywords: IMAGE ANALYSIS,TIFF,TIMELAPSE
```

### Comparing `Electroplot-0.3/PKG-INFO` & `Electroplot-1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: Electroplot
-Version: 0.3
+Version: 1.0
 Summary: Handling TIFF files and figure generation from timelapse experiments.
 Home-page: https://github.com/ConorEd/
 Author: Conor Edwards
 Author-email: conorlo@hotmail.co.uk
 License: MIT
 Description: UNKNOWN
 Keywords: IMAGE ANALYSIS,TIFF,TIMELAPSE
```

### Comparing `Electroplot-0.3/setup.py` & `Electroplot-1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 #from distutils.core import setup, find_packages
 from setuptools import setup, find_packages
 setup(
   name = 'Electroplot',         # How you named your package folder (MyLib)
   packages = find_packages(include=['Electroplot', 'Electroplot.*']), 
-  version = '0.3',      # Start with a small number and increase it with every change you make
+  version = '1.0',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Handling TIFF files and figure generation from timelapse experiments.',   # Give a short description about your library
   author = 'Conor Edwards',                   # Type in your name
   author_email = 'conorlo@hotmail.co.uk',      # Type in your E-Mail
   url = 'https://github.com/ConorEd/',   # Provide either the link to your github or to your website
   #download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['IMAGE ANALYSIS', 'TIFF', 'TIMELAPSE'],   # Keywords that define your package best
```

