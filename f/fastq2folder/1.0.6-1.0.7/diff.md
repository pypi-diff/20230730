# Comparing `tmp/fastq2folder-1.0.6.tar.gz` & `tmp/fastq2folder-1.0.7.tar.gz`

## Comparing `fastq2folder-1.0.6.tar` & `fastq2folder-1.0.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastq2folder-1.0.6/src/fastq2folder/__init__.py
--rw-r--r--   0        0        0     9241 2020-02-02 00:00:00.000000 fastq2folder-1.0.6/src/fastq2folder/fastq2folder.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 fastq2folder-1.0.6/LICENSE
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 fastq2folder-1.0.6/README.md
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 fastq2folder-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 fastq2folder-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastq2folder-1.0.7/src/fastq2folder/__init__.py
+-rw-r--r--   0        0        0     9929 2020-02-02 00:00:00.000000 fastq2folder-1.0.7/src/fastq2folder/fastq2folder.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 fastq2folder-1.0.7/LICENSE
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 fastq2folder-1.0.7/README.md
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 fastq2folder-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 fastq2folder-1.0.7/PKG-INFO
```

### Comparing `fastq2folder-1.0.6/src/fastq2folder/fastq2folder.py` & `fastq2folder-1.0.7/src/fastq2folder/fastq2folder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-# In[1]:
+# In[35]:
 
 
 import os
 import gzip
 import shutil
 import tkinter as tk
 from tkinter import filedialog
 import pandas as pd
 from Bio import SeqIO
 from scipy import stats
 import numpy as np
+import re
 
 #Create a new folder for the unzipped and binned files to go
 #base_dir = r"C:\Users\egar1\OneDrive\Desktop"
 base_dir = input('Enter path to source directory: ')
 if os.path.isdir(base_dir):
     print('The directory exists')
 else:
@@ -35,39 +36,49 @@
     os.mkdir(destination_dir)
     print('folder created')
     
 for foldername, subfolders, filenames in os.walk(source_dir):
     #print('foldername', foldername)
     #print('subfolders', subfolders)
     #print('filenames', filenames)
-    for filename in filenames:
-        shutil.copy(os.path.join(foldername, filename), destination_dir)
+    barcode = re.findall('barcode\d\d', foldername)
+    if barcode: 
+        print('barcode', barcode[0])
+        for filename in filenames:
+            # Change the filename to include the barcode as prefix
+            new_filename = barcode[0] + "_" + filename
+            shutil.copy(os.path.join(foldername, filename), os.path.join(destination_dir, new_filename))
+    else:  # Added this to handle cases where there is no barcode match
+        for filename in filenames:
+            shutil.copy(os.path.join(foldername, filename), destination_dir)
 
 # Create a dictionary to store the barcode folders
 barcode_folders = {}
 
+# Adjust the decompression function to also handle renaming
 def decompress_gz_files_in_dir(directory):
     for item in os.listdir(directory):
         if item.endswith('.gz'):
             print('decompressing ', item)
             file_name = os.path.join(directory, item)
             with gzip.open(file_name, 'rb') as f_in:
-                with open(file_name[:-3], 'wb') as f_out:  # Remove the '.gz' from the output file name
+                # We keep the filename as is, without '.gz', since it has already been renamed with the barcode
+                with open(file_name[:-3], 'wb') as f_out:
                     shutil.copyfileobj(f_in, f_out)
+            os.remove(file_name)  # <-- Remove the original .gz file after decompression
     print('decompression complete')
 
 # Call the function and provide the directory you want to decompress .gz files in
 decompress_gz_files_in_dir(destination_dir)
 
 
-# In[2]:
+# In[37]:
 
 
 import glob
-import re
 
 output_directory = os.path.join(destination_dir, 'pooledFiles')
 print('output dir', output_directory)
 
 # Ensure that the output directory exists
 os.makedirs(output_directory, exist_ok=True)
 
@@ -95,15 +106,15 @@
     with open(os.path.join(output_directory, f'{barcode}_combined.fastq'), 'w') as outfile:
         for file in files:
             with open(file) as infile:
                 for line in infile:
                     outfile.write(line)
 
 
-# In[3]:
+# In[38]:
 
 
 ##VERSION2
 from collections import Counter
 import numpy as np
 import scipy.stats as stats
 
@@ -167,17 +178,18 @@
         os.makedirs(new_dir, exist_ok=True)
 
         shutil.copy2(fastq_file, os.path.join(new_dir, file))
 
 df = pd.DataFrame(results)
 print(df)
 print('Binning complete')
+print('Please wait')
 
 
-# In[4]:
+# In[39]:
 
 
 import matplotlib.backends.backend_pdf
 import matplotlib.gridspec as gridspec
 import seaborn as sns
 
 from matplotlib import pyplot as plt
```

### Comparing `fastq2folder-1.0.6/LICENSE` & `fastq2folder-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fastq2folder-1.0.6/README.md` & `fastq2folder-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `fastq2folder-1.0.6/pyproject.toml` & `fastq2folder-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 00000010: 7265 7175 6972 6573 203d 205b 2268 6174  requires = ["hat
 00000020: 6368 6c69 6e67 225d 0d0a 6275 696c 642d  chling"]..build-
 00000030: 6261 636b 656e 6420 3d20 2268 6174 6368  backend = "hatch
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 6661 7374 7132 666f 6c64 6572 220d   "fastq2folder".
 00000070: 0a76 6572 7369 6f6e 203d 2022 312e 302e  .version = "1.0.
-00000080: 3622 0d0a 6175 7468 6f72 7320 3d20 5b0d  6"..authors = [.
+00000080: 3722 0d0a 6175 7468 6f72 7320 3d20 5b0d  7"..authors = [.
 00000090: 0a20 207b 206e 616d 653d 2245 6c69 7a61  .  { name="Eliza
 000000a0: 6265 7468 2047 6172 646e 6572 222c 2065  beth Gardner", e
 000000b0: 6d61 696c 3d22 6567 6172 3138 3131 3140  mail="egar18111@
 000000c0: 676d 6169 6c2e 636f 6d22 207d 2c0d 0a5d  gmail.com" },..]
 000000d0: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 000000e0: 2253 6372 6970 7420 746f 2070 726f 6365  "Script to proce
 000000f0: 7373 2066 6173 7471 2066 696c 6573 2062  ss fastq files b
```

### Comparing `fastq2folder-1.0.6/PKG-INFO` & `fastq2folder-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastq2folder
-Version: 1.0.6
+Version: 1.0.7
 Summary: Script to process fastq files before epi2me analysis
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Elizabeth Gardner <egar18111@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

