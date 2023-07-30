# Comparing `tmp/wassncplot-2.1.1.tar.gz` & `tmp/wassncplot-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/fibe/projects/wassncplot/dist/.tmp-l1sx6y0m/wassncplot-2.1.1.tar", last modified: Fri Mar 17 13:22:07 2023, max compression
+gzip compressed data, was "wassncplot-2.2.0.tar", last modified: Sun Jul 30 13:31:45 2023, max compression
```

## Comparing `wassncplot-2.1.1.tar` & `wassncplot-2.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2023-03-17 13:22:07.975988 wassncplot-2.1.1/
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     4263 2023-03-17 13:22:07.975988 wassncplot-2.1.1/PKG-INFO
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     3777 2022-09-20 15:29:25.000000 wassncplot-2.1.1/README.md
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     1214 2022-09-21 13:02:46.000000 wassncplot-2.1.1/pyproject.toml
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       38 2023-03-17 13:22:07.975988 wassncplot-2.1.1/setup.cfg
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2023-03-17 13:22:07.971988 wassncplot-2.1.1/src/
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2023-03-17 13:22:07.975988 wassncplot-2.1.1/src/wassncplot/
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2023-03-17 13:22:07.975988 wassncplot-2.1.1/src/wassncplot/WaveFieldVisualize/
--rw-rw-r--   0 fibe      (1000) fibe      (1000)        0 2022-09-01 10:26:19.000000 wassncplot-2.1.1/src/wassncplot/WaveFieldVisualize/__init__.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     8265 2022-09-20 15:26:45.000000 wassncplot-2.1.1/src/wassncplot/WaveFieldVisualize/waveview2.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       32 2022-09-01 10:26:19.000000 wassncplot-2.1.1/src/wassncplot/__init.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       91 2022-09-01 10:26:19.000000 wassncplot-2.1.1/src/wassncplot/__main__.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     6750 2022-09-01 10:26:19.000000 wassncplot-2.1.1/src/wassncplot/wassncplot.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     7781 2023-03-17 13:21:04.000000 wassncplot-2.1.1/src/wassncplot/wassncplot2.py
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2023-03-17 13:22:07.975988 wassncplot-2.1.1/src/wassncplot.egg-info/
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     4263 2023-03-17 13:22:07.000000 wassncplot-2.1.1/src/wassncplot.egg-info/PKG-INFO
--rw-rw-r--   0 fibe      (1000) fibe      (1000)      458 2023-03-17 13:22:07.000000 wassncplot-2.1.1/src/wassncplot.egg-info/SOURCES.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)        1 2023-03-17 13:22:07.000000 wassncplot-2.1.1/src/wassncplot.egg-info/dependency_links.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       70 2023-03-17 13:22:07.000000 wassncplot-2.1.1/src/wassncplot.egg-info/entry_points.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)      107 2023-03-17 13:22:07.000000 wassncplot-2.1.1/src/wassncplot.egg-info/requires.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       11 2023-03-17 13:22:07.000000 wassncplot-2.1.1/src/wassncplot.egg-info/top_level.txt
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2023-07-30 13:31:45.235523 wassncplot-2.2.0/
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     4263 2023-07-30 13:31:45.235523 wassncplot-2.2.0/PKG-INFO
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     3777 2023-07-29 13:20:24.000000 wassncplot-2.2.0/README.md
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     1214 2023-07-29 13:20:24.000000 wassncplot-2.2.0/pyproject.toml
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       38 2023-07-30 13:31:45.235523 wassncplot-2.2.0/setup.cfg
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2023-07-30 13:31:45.231523 wassncplot-2.2.0/src/
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2023-07-30 13:31:45.231523 wassncplot-2.2.0/src/wassncplot/
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2023-07-30 13:31:45.235523 wassncplot-2.2.0/src/wassncplot/WaveFieldVisualize/
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)        0 2023-07-29 13:20:24.000000 wassncplot-2.2.0/src/wassncplot/WaveFieldVisualize/__init__.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     8265 2023-07-29 13:20:24.000000 wassncplot-2.2.0/src/wassncplot/WaveFieldVisualize/waveview2.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       32 2023-07-29 13:20:24.000000 wassncplot-2.2.0/src/wassncplot/__init.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       91 2023-07-29 13:20:24.000000 wassncplot-2.2.0/src/wassncplot/__main__.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     6750 2023-07-29 13:20:24.000000 wassncplot-2.2.0/src/wassncplot/wassncplot.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     9843 2023-07-30 13:28:02.000000 wassncplot-2.2.0/src/wassncplot/wassncplot2.py
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2023-07-30 13:31:45.235523 wassncplot-2.2.0/src/wassncplot.egg-info/
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     4263 2023-07-30 13:31:45.000000 wassncplot-2.2.0/src/wassncplot.egg-info/PKG-INFO
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)      458 2023-07-30 13:31:45.000000 wassncplot-2.2.0/src/wassncplot.egg-info/SOURCES.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)        1 2023-07-30 13:31:45.000000 wassncplot-2.2.0/src/wassncplot.egg-info/dependency_links.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       70 2023-07-30 13:31:45.000000 wassncplot-2.2.0/src/wassncplot.egg-info/entry_points.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)      107 2023-07-30 13:31:45.000000 wassncplot-2.2.0/src/wassncplot.egg-info/requires.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       11 2023-07-30 13:31:45.000000 wassncplot-2.2.0/src/wassncplot.egg-info/top_level.txt
```

### Comparing `wassncplot-2.1.1/PKG-INFO` & `wassncplot-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wassncplot
-Version: 2.1.1
+Version: 2.2.0
 Summary: WASSncplot is a small tool to plot NetCDF 3D data generated with WASS on top of the original image files.
 Author: Filippo Bergamasco
 Author-email: filippo.bergamasco@unive.it
 License: GPL3
 Project-URL: repository, https://github.com/fbergama/wassncplot
 Keywords: WASS
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wassncplot-2.1.1/README.md` & `wassncplot-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `wassncplot-2.1.1/pyproject.toml` & `wassncplot-2.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wassncplot-2.1.1/src/wassncplot/WaveFieldVisualize/waveview2.py` & `wassncplot-2.2.0/src/wassncplot/WaveFieldVisualize/waveview2.py`

 * *Files identical despite different names*

### Comparing `wassncplot-2.1.1/src/wassncplot/wassncplot.py` & `wassncplot-2.2.0/src/wassncplot/wassncplot.py`

 * *Files identical despite different names*

### Comparing `wassncplot-2.1.1/src/wassncplot/wassncplot2.py` & `wassncplot-2.2.0/src/wassncplot/wassncplot2.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 from .WaveFieldVisualize.waveview2 import WaveView
 from tqdm import tqdm
 import sys
 import os
 import argparse
 import glob
 import scipy.io
+from scipy.interpolate import LinearNDInterpolator
 
 
-VERSION="2.1.1"
+VERSION="2.2.0"
 
 
 
 def wassncplot_main():
 
     print(" wassncplot v.", VERSION )
     print("=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-\nCopyright (C) Filippo Bergamasco 2023 \n")
@@ -37,14 +38,16 @@
     parser.add_argument("--text_prefix", default="", help="Bottom overlay text prefix")
     parser.add_argument("--wireframe", dest="wireframe", action="store_true", help="Render surface in wireframe (default)")
     parser.add_argument("--upscale2x", dest="upscale2x", action="store_true", help="Upscale the input image before rendering")
     parser.add_argument("--applymask", dest="applymask", action="store_true", help="Apply user-defined mask if available")
     parser.add_argument("--no-wireframe", dest="wireframe", action="store_false", help="Render shaded surface")
     parser.add_argument("--no-textoverlay", dest="textoverlay", action="store_false", help="Add text overlay at the bottom of the frame")
     parser.add_argument("--savexyz", dest="savexyz", action="store_true", help="Save mapping between image pixels and 3D coordinates as numpy data file")
+    parser.add_argument("--create-texture", dest="createtx", action="store_true", help="Compute sea surface radiance for each grid point and store it into the input NetCDF file.")
+    parser.add_argument("--save-texture", dest="savetx", action="store_true", help="Save each sea surface radiance texture to a png image (data is also stored in the NetCDF)")
     parser.add_argument("--saveimg", dest="saveimg", action="store_true", help="Save the undistorted image (without the superimposed grid)")
     parser.add_argument("--ffmpeg", dest="ffmpeg", action="store_true", help="Call ffmpeg to create a sequence video file")
     parser.add_argument("--ffmpeg-delete-frames", dest="ffmpegdelete", action="store_true", help="Delete the produced frames after running ffmpeg")
     parser.add_argument("--ffmpeg-fps", dest="ffmpeg_fps", default=10.0, type=float, help="Sequence framerate")
     parser.set_defaults(wireframe=True)
     args = parser.parse_args()
 
@@ -53,16 +56,16 @@
     if not os.path.isdir( outdir ):
         print("Output dir does not exist")
         sys.exit( -1 )
     else:
         print("Output renderings and data will be saved in: ", outdir)
 
 
-    print("Opening netcdf file ", args.ncfile)
-    rootgrp = Dataset( args.ncfile, mode="r")
+    print("Opening NetCDF file ", args.ncfile)
+    rootgrp = Dataset( args.ncfile, mode="a" if args.createtx else "r" )
 
     if args.baseline != None:
         stereo_baseline = args.baseline
     else:
         print("Loading baseline from netcdf")
         stereo_baseline = rootgrp["scale"][0]
 
@@ -106,17 +109,31 @@
     print("Range: %f"%zrange)
 
     if args.last_index > 0:
         nframes = args.last_index
 
     waveview = None
 
+
+    # Create a new radiance variable if not existing in the input NetCDF file
+    #
+    if args.createtx:
+        if not "radiance" in rootgrp.variables:
+            radiance = rootgrp.createVariable("radiance","u8",( rootgrp.dimensions["count"], 
+                                                                rootgrp.dimensions["X"], 
+                                                                rootgrp.dimensions["Y"]),
+                                                                fill_value=0 )
+            radiance.long_name = "Sea surface radiance for each grid point"
+
+
+
+    # Main processing loop
+    #
     print("Rendering grid data...")
     pbar = tqdm( range(args.first_index, nframes, args.step_index), file=sys.stdout, unit="frames" )
-
     data_idx = args.first_index
     output_image_size = None
 
     for image_idx in pbar:
 
         I0 = cv.imdecode( rootgrp["cam0images"][image_idx], cv.IMREAD_GRAYSCALE )
         if args.upscale2x:
@@ -136,14 +153,40 @@
         ZZ_data = np.squeeze( np.array( ZZ[data_idx,:,:] ) )/1000.0 - zmean
         #mask = (ZZ_data == 0.0)
         #ZZ_dil = cv.dilate( ZZ_data, np.ones((3,3)))
         #ZZ_data[mask]=ZZ_dil
 
         img, img_xyz = waveview.render( I0, ZZ_data )
 
+        #%%
+        if args.createtx:
+            if not "radiance" in rootgrp.variables:
+                radiance = rootgrp.createVariable("radiance","u8",( rootgrp.dimensions["count"], 
+                                                                    rootgrp.dimensions["X"], 
+                                                                    rootgrp.dimensions["Y"]),
+                                                                    fill_value=0 )
+                radiance.long_name = "Sea surface radiance for each grid point"
+
+
+            interp = LinearNDInterpolator( np.reshape( img_xyz[:,:,0:2], [-1,2]), I0.flatten(), 0 )
+            tx = interp( XX, YY ).astype( np.uint8 )
+
+            # Add texture to NetCDF
+            (rootgrp["radiance"])[image_idx,:,:] = np.expand_dims( tx, axis=0 )
+
+            # Optional: save to a png image
+            if args.savetx:
+                cv.imwrite( "%s/radiance_%08d.png"%(outdir,image_idx), tx )
+
+
+        
+
+
+        #%% 
+
         if args.savexyz:
             scipy.io.savemat( '%s/%08d'%(outdir,image_idx), {"px_2_3D": img_xyz} )
 
         img = (img*255).astype( np.uint8 )
         img = (I0mask>0)*img + ((I0mask==0)*np.expand_dims(I0, axis=-1))
         img = cv.cvtColor( img, cv.COLOR_RGB2BGR )
 
@@ -179,7 +222,10 @@
         subprocess.run(callarr)
 
         if args.ffmpegdelete:
             img_files = glob.glob( "%s/*.png"%outdir )
             for imgfile in img_files:
                 os.remove( imgfile )
 
+
+    rootgrp.close()
+
```

### Comparing `wassncplot-2.1.1/src/wassncplot.egg-info/PKG-INFO` & `wassncplot-2.2.0/src/wassncplot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wassncplot
-Version: 2.1.1
+Version: 2.2.0
 Summary: WASSncplot is a small tool to plot NetCDF 3D data generated with WASS on top of the original image files.
 Author: Filippo Bergamasco
 Author-email: filippo.bergamasco@unive.it
 License: GPL3
 Project-URL: repository, https://github.com/fbergama/wassncplot
 Keywords: WASS
 Classifier: Programming Language :: Python :: 3
```

