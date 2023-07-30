# Comparing `tmp/sewar-0.4.5.tar.gz` & `tmp/sewar-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sewar-0.4.5.tar", last modified: Sun Mar 20 14:59:01 2022, max compression
+gzip compressed data, was "sewar-0.4.6.tar", last modified: Sun Jul 30 17:07:40 2023, max compression
```

## Comparing `sewar-0.4.5.tar` & `sewar-0.4.6.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 andrewekhalel   (501) staff       (20)        0 2022-03-20 14:59:01.859570 sewar-0.4.5/
--rw-r--r--   0 andrewekhalel   (501) staff       (20)       18 2022-03-20 11:22:47.000000 sewar-0.4.5/MANIFEST.in
--rw-r--r--   0 andrewekhalel   (501) staff       (20)     5413 2022-03-20 14:59:01.859444 sewar-0.4.5/PKG-INFO
--rw-r--r--   0 andrewekhalel   (501) staff       (20)     3734 2022-03-20 11:22:47.000000 sewar-0.4.5/README.md
--rw-r--r--   0 andrewekhalel   (501) staff       (20)       38 2022-03-20 14:59:01.859639 sewar-0.4.5/setup.cfg
--rw-r--r--   0 andrewekhalel   (501) staff       (20)     1371 2022-03-20 14:58:34.000000 sewar-0.4.5/setup.py
-drwxr-xr-x   0 andrewekhalel   (501) staff       (20)        0 2022-03-20 14:59:01.858368 sewar-0.4.5/sewar/
--rw-r--r--   0 andrewekhalel   (501) staff       (20)      580 2022-03-20 11:22:47.000000 sewar-0.4.5/sewar/__init__.py
--rw-r--r--   0 andrewekhalel   (501) staff       (20)     2780 2022-03-20 11:22:47.000000 sewar-0.4.5/sewar/command_line.py
--rw-r--r--   0 andrewekhalel   (501) staff       (20)    10861 2022-03-20 13:37:03.000000 sewar-0.4.5/sewar/full_ref.py
--rw-r--r--   0 andrewekhalel   (501) staff       (20)     2424 2022-03-20 14:13:42.000000 sewar-0.4.5/sewar/no_ref.py
--rw-r--r--   0 andrewekhalel   (501) staff       (20)     3853 2022-03-20 11:22:47.000000 sewar-0.4.5/sewar/utils.py
-drwxr-xr-x   0 andrewekhalel   (501) staff       (20)        0 2022-03-20 14:59:01.859252 sewar-0.4.5/sewar.egg-info/
--rw-r--r--   0 andrewekhalel   (501) staff       (20)     5413 2022-03-20 14:59:01.000000 sewar-0.4.5/sewar.egg-info/PKG-INFO
--rw-r--r--   0 andrewekhalel   (501) staff       (20)      323 2022-03-20 14:59:01.000000 sewar-0.4.5/sewar.egg-info/SOURCES.txt
--rw-r--r--   0 andrewekhalel   (501) staff       (20)        1 2022-03-20 14:59:01.000000 sewar-0.4.5/sewar.egg-info/dependency_links.txt
--rw-r--r--   0 andrewekhalel   (501) staff       (20)       63 2022-03-20 14:59:01.000000 sewar-0.4.5/sewar.egg-info/entry_points.txt
--rw-r--r--   0 andrewekhalel   (501) staff       (20)        1 2022-03-20 14:56:49.000000 sewar-0.4.5/sewar.egg-info/not-zip-safe
--rw-r--r--   0 andrewekhalel   (501) staff       (20)       19 2022-03-20 14:59:01.000000 sewar-0.4.5/sewar.egg-info/requires.txt
--rw-r--r--   0 andrewekhalel   (501) staff       (20)        6 2022-03-20 14:59:01.000000 sewar-0.4.5/sewar.egg-info/top_level.txt
+drwxr-xr-x   0 andrewekhalel   (501) staff       (20)        0 2023-07-30 17:07:40.548172 sewar-0.4.6/
+-rw-r--r--   0 andrewekhalel   (501) staff       (20)     1070 2022-03-20 11:22:47.000000 sewar-0.4.6/LICENSE
+-rw-r--r--   0 andrewekhalel   (501) staff       (20)       18 2022-03-20 11:22:47.000000 sewar-0.4.6/MANIFEST.in
+-rw-r--r--   0 andrewekhalel   (501) staff       (20)     4856 2023-07-30 17:07:40.547880 sewar-0.4.6/PKG-INFO
+-rw-r--r--   0 andrewekhalel   (501) staff       (20)     3734 2023-07-30 15:48:13.000000 sewar-0.4.6/README.md
+-rw-r--r--   0 andrewekhalel   (501) staff       (20)       38 2023-07-30 17:07:40.548227 sewar-0.4.6/setup.cfg
+-rw-r--r--   0 andrewekhalel   (501) staff       (20)     1371 2023-07-30 17:05:36.000000 sewar-0.4.6/setup.py
+drwxr-xr-x   0 andrewekhalel   (501) staff       (20)        0 2023-07-30 17:07:40.546543 sewar-0.4.6/sewar/
+-rw-r--r--   0 andrewekhalel   (501) staff       (20)      580 2022-03-20 11:22:47.000000 sewar-0.4.6/sewar/__init__.py
+-rw-r--r--   0 andrewekhalel   (501) staff       (20)     2780 2022-03-20 11:22:47.000000 sewar-0.4.6/sewar/command_line.py
+-rw-r--r--   0 andrewekhalel   (501) staff       (20)    10763 2023-07-30 16:54:30.000000 sewar-0.4.6/sewar/full_ref.py
+-rw-r--r--   0 andrewekhalel   (501) staff       (20)     2424 2022-03-20 14:13:42.000000 sewar-0.4.6/sewar/no_ref.py
+-rw-r--r--   0 andrewekhalel   (501) staff       (20)     3853 2022-03-20 11:22:47.000000 sewar-0.4.6/sewar/utils.py
+drwxr-xr-x   0 andrewekhalel   (501) staff       (20)        0 2023-07-30 17:07:40.547646 sewar-0.4.6/sewar.egg-info/
+-rw-r--r--   0 andrewekhalel   (501) staff       (20)     4856 2023-07-30 17:07:40.000000 sewar-0.4.6/sewar.egg-info/PKG-INFO
+-rw-r--r--   0 andrewekhalel   (501) staff       (20)      331 2023-07-30 17:07:40.000000 sewar-0.4.6/sewar.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewekhalel   (501) staff       (20)        1 2023-07-30 17:07:40.000000 sewar-0.4.6/sewar.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewekhalel   (501) staff       (20)       63 2023-07-30 17:07:40.000000 sewar-0.4.6/sewar.egg-info/entry_points.txt
+-rw-r--r--   0 andrewekhalel   (501) staff       (20)        1 2022-03-20 14:56:49.000000 sewar-0.4.6/sewar.egg-info/not-zip-safe
+-rw-r--r--   0 andrewekhalel   (501) staff       (20)       19 2023-07-30 17:07:40.000000 sewar-0.4.6/sewar.egg-info/requires.txt
+-rw-r--r--   0 andrewekhalel   (501) staff       (20)        6 2023-07-30 17:07:40.000000 sewar-0.4.6/sewar.egg-info/top_level.txt
```

### Comparing `sewar-0.4.5/PKG-INFO` & `sewar-0.4.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,87 +1,15 @@
 Metadata-Version: 2.1
 Name: sewar
-Version: 0.4.5
+Version: 0.4.6
 Summary: All image quality metrics you need in one package.
 Home-page: https://github.com/andrewekhalel/sewar
 Author: Andrew Khalel
 Author-email: andrewekhalel@gmail.com
 License: MIT
-Description: <a href="https://www.buymeacoffee.com/khalel" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>
-        
-        # Sewar
-        
-        [![Build Status](https://travis-ci.org/sachinpuranik99/sewar.svg?branch=master)](https://travis-ci.org/sachinpuranik99/sewar)
-        [![codecov](https://codecov.io/gh/sachinpuranik99/sewar/branch/master/graph/badge.svg)](https://codecov.io/gh/sachinpuranik99/sewar)
-        
-        Sewar is a python package for image quality assessment using different metrics. You can check documentation [here](http://sewar.readthedocs.io/).
-        
-        
-        ## Implemented metrics
-        - [x] Mean Squared Error (MSE) 
-        - [x] Root Mean Sqaured Error (RMSE)
-        - [x] Peak Signal-to-Noise Ratio (PSNR) [[1]](https://ieeexplore.ieee.org/abstract/document/1284395/)
-        - [x] Structural Similarity Index (SSIM) [[1]](https://ieeexplore.ieee.org/abstract/document/1284395/)
-        - [x] Universal Quality Image Index (UQI) [[2]](https://ieeexplore.ieee.org/document/995823/)
-        - [x] Multi-scale Structural Similarity Index (MS-SSIM) [[3]](https://ieeexplore.ieee.org/abstract/document/1292216/)
-        - [x] Erreur Relative Globale Adimensionnelle de Synthèse (ERGAS) [[4]](https://hal.archives-ouvertes.fr/hal-00395027/)
-        - [x] Spatial Correlation Coefficient (SCC) [[5]](https://www.tandfonline.com/doi/abs/10.1080/014311698215973)
-        - [x] Relative Average Spectral Error (RASE) [[6]](https://ieeexplore.ieee.org/document/1304896/)
-        - [x] Spectral Angle Mapper (SAM) [[7]](https://ntrs.nasa.gov/search.jsp?R=19940012238)
-        - [x] Spectral Distortion Index (D_lambda) [[8]](https://www.ingentaconnect.com/content/asprs/pers/2008/00000074/00000002/art00003)
-        - [x] Spatial Distortion Index (D_S) [[8]](https://www.ingentaconnect.com/content/asprs/pers/2008/00000074/00000002/art00003)
-        - [x] Quality with No Reference (QNR) [[8]](https://www.ingentaconnect.com/content/asprs/pers/2008/00000074/00000002/art00003)
-        - [x] Visual Information Fidelity (VIF) [[9]](https://ieeexplore.ieee.org/abstract/document/1576816/)
-        - [x] Block Sensitive - Peak Signal-to-Noise Ratio (PSNR-B) [[10]](https://ieeexplore.ieee.org/abstract/document/5535179/)
-        
-        ## Todo
-        - [ ] Add command-line support for No-reference metrics
-        
-        ## Installation
-        Just as simple as
-        ```
-        pip install sewar
-        ```
-        ## Example usage
-        a simple example to use UQI
-        ```python
-        >>> from sewar.full_ref import uqi
-        >>> uqi(img1,img2)
-        0.9586952304831419
-        ```
-        
-        ## Example usage for command line interface
-        ```
-        sewar [metric] [GT path] [P path] (any extra parameters)
-        ```
-        An example to use SSIM
-        ```shell
-        foo@bar:~$ sewar ssim images/ground_truth.tif images/deformed.tif -ws 13
-        ssim : 0.8947009811410856
-        ```
-        Available metrics list
-        ```
-        mse, rmse, psnr, rmse_sw, uqi, ssim, ergas, scc, rase, sam, msssim, vifp, psnrb 
-        ```
-        
-        ## Contributors
-        Special thanks to @sachinpuranik99 and @sunwj.
-        
-        ## References
-        [1] "Image quality assessment: from error visibility to structural similarity." 2004)<br/>
-        [2] "A universal image quality index." (2002)<br/>
-        [3] "Multiscale structural similarity for image quality assessment." (2003)<br/>
-        [4] "Quality of high resolution synthesised images: Is there a simple criterion?." (2000)<br/>
-        [5] "A wavelet transform method to merge Landsat TM and SPOT panchromatic data." (1998)<br/>
-        [6] "Fusion of multispectral and panchromatic images using improved IHS and PCA mergers based on wavelet decomposition." (2004)<br/>
-        [7] "Discrimination among semi-arid landscape endmembers using the spectral angle mapper (SAM) algorithm." (1992)<br/>
-        [8] "Multispectral and panchromatic data fusion assessment without reference." (2008)<br/>
-        [9] "Image information and visual quality." (2006)<br/>
-        [10] "Quality Assessment of Deblocked Images" (2011)<br/>
-        
 Keywords: image quality performance metric measure ergas q psnr pansharpening
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
@@ -92,7 +20,82 @@
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Multimedia :: Graphics
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<a href="https://www.buymeacoffee.com/khalel" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>
+
+# Sewar
+
+[![Build Status](https://travis-ci.org/sachinpuranik99/sewar.svg?branch=master)](https://travis-ci.org/sachinpuranik99/sewar)
+[![codecov](https://codecov.io/gh/sachinpuranik99/sewar/branch/master/graph/badge.svg)](https://codecov.io/gh/sachinpuranik99/sewar)
+
+Sewar is a python package for image quality assessment using different metrics. You can check documentation [here](http://sewar.readthedocs.io/).
+
+
+## Implemented metrics
+- [x] Mean Squared Error (MSE) 
+- [x] Root Mean Squared Error (RMSE)
+- [x] Peak Signal-to-Noise Ratio (PSNR) [[1]](https://ieeexplore.ieee.org/abstract/document/1284395/)
+- [x] Structural Similarity Index (SSIM) [[1]](https://ieeexplore.ieee.org/abstract/document/1284395/)
+- [x] Universal Quality Image Index (UQI) [[2]](https://ieeexplore.ieee.org/document/995823/)
+- [x] Multi-scale Structural Similarity Index (MS-SSIM) [[3]](https://ieeexplore.ieee.org/abstract/document/1292216/)
+- [x] Erreur Relative Globale Adimensionnelle de Synthèse (ERGAS) [[4]](https://hal.archives-ouvertes.fr/hal-00395027/)
+- [x] Spatial Correlation Coefficient (SCC) [[5]](https://www.tandfonline.com/doi/abs/10.1080/014311698215973)
+- [x] Relative Average Spectral Error (RASE) [[6]](https://ieeexplore.ieee.org/document/1304896/)
+- [x] Spectral Angle Mapper (SAM) [[7]](https://ntrs.nasa.gov/search.jsp?R=19940012238)
+- [x] Spectral Distortion Index (D_lambda) [[8]](https://www.ingentaconnect.com/content/asprs/pers/2008/00000074/00000002/art00003)
+- [x] Spatial Distortion Index (D_S) [[8]](https://www.ingentaconnect.com/content/asprs/pers/2008/00000074/00000002/art00003)
+- [x] Quality with No Reference (QNR) [[8]](https://www.ingentaconnect.com/content/asprs/pers/2008/00000074/00000002/art00003)
+- [x] Visual Information Fidelity (VIF) [[9]](https://ieeexplore.ieee.org/abstract/document/1576816/)
+- [x] Block Sensitive - Peak Signal-to-Noise Ratio (PSNR-B) [[10]](https://ieeexplore.ieee.org/abstract/document/5535179/)
+
+## Todo
+- [ ] Add command-line support for No-reference metrics
+
+## Installation
+Just as simple as
+```
+pip install sewar
+```
+## Example usage
+a simple example to use UQI
+```python
+>>> from sewar.full_ref import uqi
+>>> uqi(img1,img2)
+0.9586952304831419
+```
+
+## Example usage for command line interface
+```
+sewar [metric] [GT path] [P path] (any extra parameters)
+```
+An example to use SSIM
+```shell
+foo@bar:~$ sewar ssim images/ground_truth.tif images/deformed.tif -ws 13
+ssim : 0.8947009811410856
+```
+Available metrics list
+```
+mse, rmse, psnr, rmse_sw, uqi, ssim, ergas, scc, rase, sam, msssim, vifp, psnrb 
+```
+
+## Contributors
+Special thanks to @sachinpuranik99 and @sunwj.
+
+## References
+[1] "Image quality assessment: from error visibility to structural similarity." 2004)<br/>
+[2] "A universal image quality index." (2002)<br/>
+[3] "Multiscale structural similarity for image quality assessment." (2003)<br/>
+[4] "Quality of high resolution synthesised images: Is there a simple criterion?." (2000)<br/>
+[5] "A wavelet transform method to merge Landsat TM and SPOT panchromatic data." (1998)<br/>
+[6] "Fusion of multispectral and panchromatic images using improved IHS and PCA mergers based on wavelet decomposition." (2004)<br/>
+[7] "Discrimination among semi-arid landscape endmembers using the spectral angle mapper (SAM) algorithm." (1992)<br/>
+[8] "Multispectral and panchromatic data fusion assessment without reference." (2008)<br/>
+[9] "Image information and visual quality." (2006)<br/>
+[10] "Quality Assessment of Deblocked Images" (2011)<br/>
+
+
```

#### html2text {}

```diff
@@ -1,66 +1,66 @@
-Metadata-Version: 2.1 Name: sewar Version: 0.4.5 Summary: All image quality
+Metadata-Version: 2.1 Name: sewar Version: 0.4.6 Summary: All image quality
 metrics you need in one package. Home-page: https://github.com/andrewekhalel/
 sewar Author: Andrew Khalel Author-email: andrewekhalel@gmail.com License: MIT
-Description: [Buy_Me_A_Coffee] # Sewar [![Build Status](https://travis-ci.org/
-sachinpuranik99/sewar.svg?branch=master)](https://travis-ci.org/
-sachinpuranik99/sewar) [![codecov](https://codecov.io/gh/sachinpuranik99/sewar/
-branch/master/graph/badge.svg)](https://codecov.io/gh/sachinpuranik99/sewar)
-Sewar is a python package for image quality assessment using different metrics.
-You can check documentation [here](http://sewar.readthedocs.io/). ##
-Implemented metrics - [x] Mean Squared Error (MSE) - [x] Root Mean Sqaured
-Error (RMSE) - [x] Peak Signal-to-Noise Ratio (PSNR) [[1]](https://
-ieeexplore.ieee.org/abstract/document/1284395/) - [x] Structural Similarity
-Index (SSIM) [[1]](https://ieeexplore.ieee.org/abstract/document/1284395/) -
-[x] Universal Quality Image Index (UQI) [[2]](https://ieeexplore.ieee.org/
-document/995823/) - [x] Multi-scale Structural Similarity Index (MS-SSIM) [[3]]
-(https://ieeexplore.ieee.org/abstract/document/1292216/) - [x] Erreur Relative
-Globale Adimensionnelle de SynthÃ¨se (ERGAS) [[4]](https://hal.archives-
-ouvertes.fr/hal-00395027/) - [x] Spatial Correlation Coefficient (SCC) [[5]]
-(https://www.tandfonline.com/doi/abs/10.1080/014311698215973) - [x] Relative
-Average Spectral Error (RASE) [[6]](https://ieeexplore.ieee.org/document/
-1304896/) - [x] Spectral Angle Mapper (SAM) [[7]](https://ntrs.nasa.gov/
-search.jsp?R=19940012238) - [x] Spectral Distortion Index (D_lambda) [[8]]
-(https://www.ingentaconnect.com/content/asprs/pers/2008/00000074/00000002/
-art00003) - [x] Spatial Distortion Index (D_S) [[8]](https://
+Keywords: image quality performance metric measure ergas q psnr pansharpening
+Platform: UNKNOWN Classifier: Development Status :: 2 - Pre-Alpha Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python Classifier: Programming
+Language :: Python :: 2 Classifier: Programming Language :: Python :: 2.6
+Classifier: Programming Language :: Python :: 2.7 Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.1
+Classifier: Programming Language :: Python :: 3.2 Classifier: Programming
+Language :: Python :: 3.3 Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5 Classifier: Programming
+Language :: Python :: 3.6 Classifier: Topic :: Multimedia :: Graphics
+Description-Content-Type: text/markdown License-File: LICENSE [Buy_Me_A_Coffee]
+# Sewar [![Build Status](https://travis-ci.org/sachinpuranik99/
+sewar.svg?branch=master)](https://travis-ci.org/sachinpuranik99/sewar) [!
+[codecov](https://codecov.io/gh/sachinpuranik99/sewar/branch/master/graph/
+badge.svg)](https://codecov.io/gh/sachinpuranik99/sewar) Sewar is a python
+package for image quality assessment using different metrics. You can check
+documentation [here](http://sewar.readthedocs.io/). ## Implemented metrics -
+[x] Mean Squared Error (MSE) - [x] Root Mean Squared Error (RMSE) - [x] Peak
+Signal-to-Noise Ratio (PSNR) [[1]](https://ieeexplore.ieee.org/abstract/
+document/1284395/) - [x] Structural Similarity Index (SSIM) [[1]](https://
+ieeexplore.ieee.org/abstract/document/1284395/) - [x] Universal Quality Image
+Index (UQI) [[2]](https://ieeexplore.ieee.org/document/995823/) - [x] Multi-
+scale Structural Similarity Index (MS-SSIM) [[3]](https://ieeexplore.ieee.org/
+abstract/document/1292216/) - [x] Erreur Relative Globale Adimensionnelle de
+SynthÃ¨se (ERGAS) [[4]](https://hal.archives-ouvertes.fr/hal-00395027/) - [x]
+Spatial Correlation Coefficient (SCC) [[5]](https://www.tandfonline.com/doi/
+abs/10.1080/014311698215973) - [x] Relative Average Spectral Error (RASE) [[6]]
+(https://ieeexplore.ieee.org/document/1304896/) - [x] Spectral Angle Mapper
+(SAM) [[7]](https://ntrs.nasa.gov/search.jsp?R=19940012238) - [x] Spectral
+Distortion Index (D_lambda) [[8]](https://www.ingentaconnect.com/content/asprs/
+pers/2008/00000074/00000002/art00003) - [x] Spatial Distortion Index (D_S) [
+[8]](https://www.ingentaconnect.com/content/asprs/pers/2008/00000074/00000002/
+art00003) - [x] Quality with No Reference (QNR) [[8]](https://
 www.ingentaconnect.com/content/asprs/pers/2008/00000074/00000002/art00003) -
-[x] Quality with No Reference (QNR) [[8]](https://www.ingentaconnect.com/
-content/asprs/pers/2008/00000074/00000002/art00003) - [x] Visual Information
-Fidelity (VIF) [[9]](https://ieeexplore.ieee.org/abstract/document/1576816/) -
-[x] Block Sensitive - Peak Signal-to-Noise Ratio (PSNR-B) [[10]](https://
-ieeexplore.ieee.org/abstract/document/5535179/) ## Todo - [ ] Add command-line
-support for No-reference metrics ## Installation Just as simple as ``` pip
-install sewar ``` ## Example usage a simple example to use UQI ```python >>>
-from sewar.full_ref import uqi >>> uqi(img1,img2) 0.9586952304831419 ``` ##
-Example usage for command line interface ``` sewar [metric] [GT path] [P path]
-(any extra parameters) ``` An example to use SSIM ```shell foo@bar:~$ sewar
-ssim images/ground_truth.tif images/deformed.tif -ws 13 ssim :
-0.8947009811410856 ``` Available metrics list ``` mse, rmse, psnr, rmse_sw,
-uqi, ssim, ergas, scc, rase, sam, msssim, vifp, psnrb ``` ## Contributors
-Special thanks to @sachinpuranik99 and @sunwj. ## References [1] "Image quality
-assessment: from error visibility to structural similarity." 2004)
+[x] Visual Information Fidelity (VIF) [[9]](https://ieeexplore.ieee.org/
+abstract/document/1576816/) - [x] Block Sensitive - Peak Signal-to-Noise Ratio
+(PSNR-B) [[10]](https://ieeexplore.ieee.org/abstract/document/5535179/) ## Todo
+- [ ] Add command-line support for No-reference metrics ## Installation Just as
+simple as ``` pip install sewar ``` ## Example usage a simple example to use
+UQI ```python >>> from sewar.full_ref import uqi >>> uqi(img1,img2)
+0.9586952304831419 ``` ## Example usage for command line interface ``` sewar
+[metric] [GT path] [P path] (any extra parameters) ``` An example to use SSIM
+```shell foo@bar:~$ sewar ssim images/ground_truth.tif images/deformed.tif -ws
+13 ssim : 0.8947009811410856 ``` Available metrics list ``` mse, rmse, psnr,
+rmse_sw, uqi, ssim, ergas, scc, rase, sam, msssim, vifp, psnrb ``` ##
+Contributors Special thanks to @sachinpuranik99 and @sunwj. ## References [1]
+"Image quality assessment: from error visibility to structural similarity."
+2004)
 [2] "A universal image quality index." (2002)
 [3] "Multiscale structural similarity for image quality assessment." (2003)
 [4] "Quality of high resolution synthesised images: Is there a simple
 criterion?." (2000)
 [5] "A wavelet transform method to merge Landsat TM and SPOT panchromatic
 data." (1998)
 [6] "Fusion of multispectral and panchromatic images using improved IHS and PCA
 mergers based on wavelet decomposition." (2004)
 [7] "Discrimination among semi-arid landscape endmembers using the spectral
 angle mapper (SAM) algorithm." (1992)
 [8] "Multispectral and panchromatic data fusion assessment without reference."
 (2008)
 [9] "Image information and visual quality." (2006)
 [10] "Quality Assessment of Deblocked Images" (2011)
-Keywords: image quality performance metric measure ergas q psnr pansharpening
-Platform: UNKNOWN Classifier: Development Status :: 2 - Pre-Alpha Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 2 Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7 Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.1
-Classifier: Programming Language :: Python :: 3.2 Classifier: Programming
-Language :: Python :: 3.3 Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5 Classifier: Programming
-Language :: Python :: 3.6 Classifier: Topic :: Multimedia :: Graphics
-Description-Content-Type: text/markdown
```

### Comparing `sewar-0.4.5/README.md` & `sewar-0.4.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![codecov](https://codecov.io/gh/sachinpuranik99/sewar/branch/master/graph/badge.svg)](https://codecov.io/gh/sachinpuranik99/sewar)
 
 Sewar is a python package for image quality assessment using different metrics. You can check documentation [here](http://sewar.readthedocs.io/).
 
 
 ## Implemented metrics
 - [x] Mean Squared Error (MSE) 
-- [x] Root Mean Sqaured Error (RMSE)
+- [x] Root Mean Squared Error (RMSE)
 - [x] Peak Signal-to-Noise Ratio (PSNR) [[1]](https://ieeexplore.ieee.org/abstract/document/1284395/)
 - [x] Structural Similarity Index (SSIM) [[1]](https://ieeexplore.ieee.org/abstract/document/1284395/)
 - [x] Universal Quality Image Index (UQI) [[2]](https://ieeexplore.ieee.org/document/995823/)
 - [x] Multi-scale Structural Similarity Index (MS-SSIM) [[3]](https://ieeexplore.ieee.org/abstract/document/1292216/)
 - [x] Erreur Relative Globale Adimensionnelle de Synthèse (ERGAS) [[4]](https://hal.archives-ouvertes.fr/hal-00395027/)
 - [x] Spatial Correlation Coefficient (SCC) [[5]](https://www.tandfonline.com/doi/abs/10.1080/014311698215973)
 - [x] Relative Average Spectral Error (RASE) [[6]](https://ieeexplore.ieee.org/document/1304896/)
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 [Buy_Me_A_Coffee] # Sewar [![Build Status](https://travis-ci.org/
 sachinpuranik99/sewar.svg?branch=master)](https://travis-ci.org/
 sachinpuranik99/sewar) [![codecov](https://codecov.io/gh/sachinpuranik99/sewar/
 branch/master/graph/badge.svg)](https://codecov.io/gh/sachinpuranik99/sewar)
 Sewar is a python package for image quality assessment using different metrics.
 You can check documentation [here](http://sewar.readthedocs.io/). ##
-Implemented metrics - [x] Mean Squared Error (MSE) - [x] Root Mean Sqaured
+Implemented metrics - [x] Mean Squared Error (MSE) - [x] Root Mean Squared
 Error (RMSE) - [x] Peak Signal-to-Noise Ratio (PSNR) [[1]](https://
 ieeexplore.ieee.org/abstract/document/1284395/) - [x] Structural Similarity
 Index (SSIM) [[1]](https://ieeexplore.ieee.org/abstract/document/1284395/) -
 [x] Universal Quality Image Index (UQI) [[2]](https://ieeexplore.ieee.org/
 document/995823/) - [x] Multi-scale Structural Similarity Index (MS-SSIM) [[3]]
 (https://ieeexplore.ieee.org/abstract/document/1292216/) - [x] Erreur Relative
 Globale Adimensionnelle de SynthÃ¨se (ERGAS) [[4]](https://hal.archives-
```

### Comparing `sewar-0.4.5/setup.py` & `sewar-0.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def readme():
 	with open('README.md', encoding='UTF-8') as f:
 		return f.read()
 
 
 setup(name='sewar',
-	version='0.4.5',
+	version='0.4.6',
 	description='All image quality metrics you need in one package.',
 	long_description=readme(),
 	long_description_content_type="text/markdown",
 	classifiers=[
 	'Development Status :: 2 - Pre-Alpha',
 	'License :: OSI Approved :: MIT License',
 	'Operating System :: OS Independent',
```

### Comparing `sewar-0.4.5/sewar/__init__.py` & `sewar-0.4.6/sewar/__init__.py`

 * *Files identical despite different names*

### Comparing `sewar-0.4.5/sewar/command_line.py` & `sewar-0.4.6/sewar/command_line.py`

 * *Files identical despite different names*

### Comparing `sewar-0.4.5/sewar/full_ref.py` & `sewar-0.4.6/sewar/full_ref.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,43 +156,37 @@
 	for i in range(GT.shape[2]):
 		ssim,cs = _ssim_single(GT[:,:,i],P[:,:,i],ws,C1,C2,fltr_specs,mode)
 		ssims.append(ssim)
 		css.append(cs)
 	return np.mean(ssims),np.mean(css)
 
 
-def ergas(GT,P,r=4,ws=8):
+def ergas(GT,P,r=0.25):
 	"""calculates erreur relative globale adimensionnelle de synthese (ergas).
 
 	:param GT: first (original) input image.
 	:param P: second (deformed) input image.
-	:param r: ratio of high resolution to low resolution (default=4).
-	:param ws: sliding window size (default = 8).
+	:param r: ratio of high resolution to low resolution (default=1/4).
 
 	:returns:  float -- ergas value.
 	"""
 	GT,P = _initial_check(GT,P)
 
-	rmse_map = None
-	nb = 1
+	nb = GT.shape[2]
 
-	_,rmse_map = rmse_sw(GT,P,ws)
+	GT_means_per_band = np.mean(GT, axis=(0,1))
 
-	means_map = uniform_filter(GT,ws)/ws**2
-
-	# Avoid division by zero
-	idx = means_map == 0
-	means_map[idx] = 1
-	rmse_map[idx] = 0
-
-	ergasroot = np.sqrt(np.sum(((rmse_map**2)/(means_map**2)),axis=2)/nb)
-	ergas_map = 100*r*ergasroot;
-
-	s = int(np.round(ws/2))
-	return np.mean(ergas_map[s:-s,s:-s])
+	rmse_per_band = np.zeros(nb)
+	for b in range(nb):
+		rmse_per_band[b] = rmse(GT[:,:,b],P[:,:,b])
+	
+	presratio = 100*r
+	div = (rmse_per_band**2) / (GT_means_per_band**2)
+	ergasroot = np.sqrt( np.sum(div)/ nb )
+	return presratio*ergasroot
 
 def _scc_single(GT,P,win,ws):
 	def _scc_filter(inp, axis, output, mode, cval):
 		return correlate(inp, win , output, mode, cval, 0)
 
 	GT_hp = generic_laplace(GT.astype(np.float64), _scc_filter)
 	P_hp = generic_laplace(P.astype(np.float64), _scc_filter)
```

### Comparing `sewar-0.4.5/sewar/no_ref.py` & `sewar-0.4.6/sewar/no_ref.py`

 * *Files identical despite different names*

### Comparing `sewar-0.4.5/sewar/utils.py` & `sewar-0.4.6/sewar/utils.py`

 * *Files identical despite different names*

### Comparing `sewar-0.4.5/sewar.egg-info/PKG-INFO` & `sewar-0.4.6/sewar.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,87 +1,15 @@
 Metadata-Version: 2.1
 Name: sewar
-Version: 0.4.5
+Version: 0.4.6
 Summary: All image quality metrics you need in one package.
 Home-page: https://github.com/andrewekhalel/sewar
 Author: Andrew Khalel
 Author-email: andrewekhalel@gmail.com
 License: MIT
-Description: <a href="https://www.buymeacoffee.com/khalel" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>
-        
-        # Sewar
-        
-        [![Build Status](https://travis-ci.org/sachinpuranik99/sewar.svg?branch=master)](https://travis-ci.org/sachinpuranik99/sewar)
-        [![codecov](https://codecov.io/gh/sachinpuranik99/sewar/branch/master/graph/badge.svg)](https://codecov.io/gh/sachinpuranik99/sewar)
-        
-        Sewar is a python package for image quality assessment using different metrics. You can check documentation [here](http://sewar.readthedocs.io/).
-        
-        
-        ## Implemented metrics
-        - [x] Mean Squared Error (MSE) 
-        - [x] Root Mean Sqaured Error (RMSE)
-        - [x] Peak Signal-to-Noise Ratio (PSNR) [[1]](https://ieeexplore.ieee.org/abstract/document/1284395/)
-        - [x] Structural Similarity Index (SSIM) [[1]](https://ieeexplore.ieee.org/abstract/document/1284395/)
-        - [x] Universal Quality Image Index (UQI) [[2]](https://ieeexplore.ieee.org/document/995823/)
-        - [x] Multi-scale Structural Similarity Index (MS-SSIM) [[3]](https://ieeexplore.ieee.org/abstract/document/1292216/)
-        - [x] Erreur Relative Globale Adimensionnelle de Synthèse (ERGAS) [[4]](https://hal.archives-ouvertes.fr/hal-00395027/)
-        - [x] Spatial Correlation Coefficient (SCC) [[5]](https://www.tandfonline.com/doi/abs/10.1080/014311698215973)
-        - [x] Relative Average Spectral Error (RASE) [[6]](https://ieeexplore.ieee.org/document/1304896/)
-        - [x] Spectral Angle Mapper (SAM) [[7]](https://ntrs.nasa.gov/search.jsp?R=19940012238)
-        - [x] Spectral Distortion Index (D_lambda) [[8]](https://www.ingentaconnect.com/content/asprs/pers/2008/00000074/00000002/art00003)
-        - [x] Spatial Distortion Index (D_S) [[8]](https://www.ingentaconnect.com/content/asprs/pers/2008/00000074/00000002/art00003)
-        - [x] Quality with No Reference (QNR) [[8]](https://www.ingentaconnect.com/content/asprs/pers/2008/00000074/00000002/art00003)
-        - [x] Visual Information Fidelity (VIF) [[9]](https://ieeexplore.ieee.org/abstract/document/1576816/)
-        - [x] Block Sensitive - Peak Signal-to-Noise Ratio (PSNR-B) [[10]](https://ieeexplore.ieee.org/abstract/document/5535179/)
-        
-        ## Todo
-        - [ ] Add command-line support for No-reference metrics
-        
-        ## Installation
-        Just as simple as
-        ```
-        pip install sewar
-        ```
-        ## Example usage
-        a simple example to use UQI
-        ```python
-        >>> from sewar.full_ref import uqi
-        >>> uqi(img1,img2)
-        0.9586952304831419
-        ```
-        
-        ## Example usage for command line interface
-        ```
-        sewar [metric] [GT path] [P path] (any extra parameters)
-        ```
-        An example to use SSIM
-        ```shell
-        foo@bar:~$ sewar ssim images/ground_truth.tif images/deformed.tif -ws 13
-        ssim : 0.8947009811410856
-        ```
-        Available metrics list
-        ```
-        mse, rmse, psnr, rmse_sw, uqi, ssim, ergas, scc, rase, sam, msssim, vifp, psnrb 
-        ```
-        
-        ## Contributors
-        Special thanks to @sachinpuranik99 and @sunwj.
-        
-        ## References
-        [1] "Image quality assessment: from error visibility to structural similarity." 2004)<br/>
-        [2] "A universal image quality index." (2002)<br/>
-        [3] "Multiscale structural similarity for image quality assessment." (2003)<br/>
-        [4] "Quality of high resolution synthesised images: Is there a simple criterion?." (2000)<br/>
-        [5] "A wavelet transform method to merge Landsat TM and SPOT panchromatic data." (1998)<br/>
-        [6] "Fusion of multispectral and panchromatic images using improved IHS and PCA mergers based on wavelet decomposition." (2004)<br/>
-        [7] "Discrimination among semi-arid landscape endmembers using the spectral angle mapper (SAM) algorithm." (1992)<br/>
-        [8] "Multispectral and panchromatic data fusion assessment without reference." (2008)<br/>
-        [9] "Image information and visual quality." (2006)<br/>
-        [10] "Quality Assessment of Deblocked Images" (2011)<br/>
-        
 Keywords: image quality performance metric measure ergas q psnr pansharpening
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
@@ -92,7 +20,82 @@
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Multimedia :: Graphics
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<a href="https://www.buymeacoffee.com/khalel" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>
+
+# Sewar
+
+[![Build Status](https://travis-ci.org/sachinpuranik99/sewar.svg?branch=master)](https://travis-ci.org/sachinpuranik99/sewar)
+[![codecov](https://codecov.io/gh/sachinpuranik99/sewar/branch/master/graph/badge.svg)](https://codecov.io/gh/sachinpuranik99/sewar)
+
+Sewar is a python package for image quality assessment using different metrics. You can check documentation [here](http://sewar.readthedocs.io/).
+
+
+## Implemented metrics
+- [x] Mean Squared Error (MSE) 
+- [x] Root Mean Squared Error (RMSE)
+- [x] Peak Signal-to-Noise Ratio (PSNR) [[1]](https://ieeexplore.ieee.org/abstract/document/1284395/)
+- [x] Structural Similarity Index (SSIM) [[1]](https://ieeexplore.ieee.org/abstract/document/1284395/)
+- [x] Universal Quality Image Index (UQI) [[2]](https://ieeexplore.ieee.org/document/995823/)
+- [x] Multi-scale Structural Similarity Index (MS-SSIM) [[3]](https://ieeexplore.ieee.org/abstract/document/1292216/)
+- [x] Erreur Relative Globale Adimensionnelle de Synthèse (ERGAS) [[4]](https://hal.archives-ouvertes.fr/hal-00395027/)
+- [x] Spatial Correlation Coefficient (SCC) [[5]](https://www.tandfonline.com/doi/abs/10.1080/014311698215973)
+- [x] Relative Average Spectral Error (RASE) [[6]](https://ieeexplore.ieee.org/document/1304896/)
+- [x] Spectral Angle Mapper (SAM) [[7]](https://ntrs.nasa.gov/search.jsp?R=19940012238)
+- [x] Spectral Distortion Index (D_lambda) [[8]](https://www.ingentaconnect.com/content/asprs/pers/2008/00000074/00000002/art00003)
+- [x] Spatial Distortion Index (D_S) [[8]](https://www.ingentaconnect.com/content/asprs/pers/2008/00000074/00000002/art00003)
+- [x] Quality with No Reference (QNR) [[8]](https://www.ingentaconnect.com/content/asprs/pers/2008/00000074/00000002/art00003)
+- [x] Visual Information Fidelity (VIF) [[9]](https://ieeexplore.ieee.org/abstract/document/1576816/)
+- [x] Block Sensitive - Peak Signal-to-Noise Ratio (PSNR-B) [[10]](https://ieeexplore.ieee.org/abstract/document/5535179/)
+
+## Todo
+- [ ] Add command-line support for No-reference metrics
+
+## Installation
+Just as simple as
+```
+pip install sewar
+```
+## Example usage
+a simple example to use UQI
+```python
+>>> from sewar.full_ref import uqi
+>>> uqi(img1,img2)
+0.9586952304831419
+```
+
+## Example usage for command line interface
+```
+sewar [metric] [GT path] [P path] (any extra parameters)
+```
+An example to use SSIM
+```shell
+foo@bar:~$ sewar ssim images/ground_truth.tif images/deformed.tif -ws 13
+ssim : 0.8947009811410856
+```
+Available metrics list
+```
+mse, rmse, psnr, rmse_sw, uqi, ssim, ergas, scc, rase, sam, msssim, vifp, psnrb 
+```
+
+## Contributors
+Special thanks to @sachinpuranik99 and @sunwj.
+
+## References
+[1] "Image quality assessment: from error visibility to structural similarity." 2004)<br/>
+[2] "A universal image quality index." (2002)<br/>
+[3] "Multiscale structural similarity for image quality assessment." (2003)<br/>
+[4] "Quality of high resolution synthesised images: Is there a simple criterion?." (2000)<br/>
+[5] "A wavelet transform method to merge Landsat TM and SPOT panchromatic data." (1998)<br/>
+[6] "Fusion of multispectral and panchromatic images using improved IHS and PCA mergers based on wavelet decomposition." (2004)<br/>
+[7] "Discrimination among semi-arid landscape endmembers using the spectral angle mapper (SAM) algorithm." (1992)<br/>
+[8] "Multispectral and panchromatic data fusion assessment without reference." (2008)<br/>
+[9] "Image information and visual quality." (2006)<br/>
+[10] "Quality Assessment of Deblocked Images" (2011)<br/>
+
+
```

#### html2text {}

```diff
@@ -1,66 +1,66 @@
-Metadata-Version: 2.1 Name: sewar Version: 0.4.5 Summary: All image quality
+Metadata-Version: 2.1 Name: sewar Version: 0.4.6 Summary: All image quality
 metrics you need in one package. Home-page: https://github.com/andrewekhalel/
 sewar Author: Andrew Khalel Author-email: andrewekhalel@gmail.com License: MIT
-Description: [Buy_Me_A_Coffee] # Sewar [![Build Status](https://travis-ci.org/
-sachinpuranik99/sewar.svg?branch=master)](https://travis-ci.org/
-sachinpuranik99/sewar) [![codecov](https://codecov.io/gh/sachinpuranik99/sewar/
-branch/master/graph/badge.svg)](https://codecov.io/gh/sachinpuranik99/sewar)
-Sewar is a python package for image quality assessment using different metrics.
-You can check documentation [here](http://sewar.readthedocs.io/). ##
-Implemented metrics - [x] Mean Squared Error (MSE) - [x] Root Mean Sqaured
-Error (RMSE) - [x] Peak Signal-to-Noise Ratio (PSNR) [[1]](https://
-ieeexplore.ieee.org/abstract/document/1284395/) - [x] Structural Similarity
-Index (SSIM) [[1]](https://ieeexplore.ieee.org/abstract/document/1284395/) -
-[x] Universal Quality Image Index (UQI) [[2]](https://ieeexplore.ieee.org/
-document/995823/) - [x] Multi-scale Structural Similarity Index (MS-SSIM) [[3]]
-(https://ieeexplore.ieee.org/abstract/document/1292216/) - [x] Erreur Relative
-Globale Adimensionnelle de SynthÃ¨se (ERGAS) [[4]](https://hal.archives-
-ouvertes.fr/hal-00395027/) - [x] Spatial Correlation Coefficient (SCC) [[5]]
-(https://www.tandfonline.com/doi/abs/10.1080/014311698215973) - [x] Relative
-Average Spectral Error (RASE) [[6]](https://ieeexplore.ieee.org/document/
-1304896/) - [x] Spectral Angle Mapper (SAM) [[7]](https://ntrs.nasa.gov/
-search.jsp?R=19940012238) - [x] Spectral Distortion Index (D_lambda) [[8]]
-(https://www.ingentaconnect.com/content/asprs/pers/2008/00000074/00000002/
-art00003) - [x] Spatial Distortion Index (D_S) [[8]](https://
+Keywords: image quality performance metric measure ergas q psnr pansharpening
+Platform: UNKNOWN Classifier: Development Status :: 2 - Pre-Alpha Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python Classifier: Programming
+Language :: Python :: 2 Classifier: Programming Language :: Python :: 2.6
+Classifier: Programming Language :: Python :: 2.7 Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.1
+Classifier: Programming Language :: Python :: 3.2 Classifier: Programming
+Language :: Python :: 3.3 Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5 Classifier: Programming
+Language :: Python :: 3.6 Classifier: Topic :: Multimedia :: Graphics
+Description-Content-Type: text/markdown License-File: LICENSE [Buy_Me_A_Coffee]
+# Sewar [![Build Status](https://travis-ci.org/sachinpuranik99/
+sewar.svg?branch=master)](https://travis-ci.org/sachinpuranik99/sewar) [!
+[codecov](https://codecov.io/gh/sachinpuranik99/sewar/branch/master/graph/
+badge.svg)](https://codecov.io/gh/sachinpuranik99/sewar) Sewar is a python
+package for image quality assessment using different metrics. You can check
+documentation [here](http://sewar.readthedocs.io/). ## Implemented metrics -
+[x] Mean Squared Error (MSE) - [x] Root Mean Squared Error (RMSE) - [x] Peak
+Signal-to-Noise Ratio (PSNR) [[1]](https://ieeexplore.ieee.org/abstract/
+document/1284395/) - [x] Structural Similarity Index (SSIM) [[1]](https://
+ieeexplore.ieee.org/abstract/document/1284395/) - [x] Universal Quality Image
+Index (UQI) [[2]](https://ieeexplore.ieee.org/document/995823/) - [x] Multi-
+scale Structural Similarity Index (MS-SSIM) [[3]](https://ieeexplore.ieee.org/
+abstract/document/1292216/) - [x] Erreur Relative Globale Adimensionnelle de
+SynthÃ¨se (ERGAS) [[4]](https://hal.archives-ouvertes.fr/hal-00395027/) - [x]
+Spatial Correlation Coefficient (SCC) [[5]](https://www.tandfonline.com/doi/
+abs/10.1080/014311698215973) - [x] Relative Average Spectral Error (RASE) [[6]]
+(https://ieeexplore.ieee.org/document/1304896/) - [x] Spectral Angle Mapper
+(SAM) [[7]](https://ntrs.nasa.gov/search.jsp?R=19940012238) - [x] Spectral
+Distortion Index (D_lambda) [[8]](https://www.ingentaconnect.com/content/asprs/
+pers/2008/00000074/00000002/art00003) - [x] Spatial Distortion Index (D_S) [
+[8]](https://www.ingentaconnect.com/content/asprs/pers/2008/00000074/00000002/
+art00003) - [x] Quality with No Reference (QNR) [[8]](https://
 www.ingentaconnect.com/content/asprs/pers/2008/00000074/00000002/art00003) -
-[x] Quality with No Reference (QNR) [[8]](https://www.ingentaconnect.com/
-content/asprs/pers/2008/00000074/00000002/art00003) - [x] Visual Information
-Fidelity (VIF) [[9]](https://ieeexplore.ieee.org/abstract/document/1576816/) -
-[x] Block Sensitive - Peak Signal-to-Noise Ratio (PSNR-B) [[10]](https://
-ieeexplore.ieee.org/abstract/document/5535179/) ## Todo - [ ] Add command-line
-support for No-reference metrics ## Installation Just as simple as ``` pip
-install sewar ``` ## Example usage a simple example to use UQI ```python >>>
-from sewar.full_ref import uqi >>> uqi(img1,img2) 0.9586952304831419 ``` ##
-Example usage for command line interface ``` sewar [metric] [GT path] [P path]
-(any extra parameters) ``` An example to use SSIM ```shell foo@bar:~$ sewar
-ssim images/ground_truth.tif images/deformed.tif -ws 13 ssim :
-0.8947009811410856 ``` Available metrics list ``` mse, rmse, psnr, rmse_sw,
-uqi, ssim, ergas, scc, rase, sam, msssim, vifp, psnrb ``` ## Contributors
-Special thanks to @sachinpuranik99 and @sunwj. ## References [1] "Image quality
-assessment: from error visibility to structural similarity." 2004)
+[x] Visual Information Fidelity (VIF) [[9]](https://ieeexplore.ieee.org/
+abstract/document/1576816/) - [x] Block Sensitive - Peak Signal-to-Noise Ratio
+(PSNR-B) [[10]](https://ieeexplore.ieee.org/abstract/document/5535179/) ## Todo
+- [ ] Add command-line support for No-reference metrics ## Installation Just as
+simple as ``` pip install sewar ``` ## Example usage a simple example to use
+UQI ```python >>> from sewar.full_ref import uqi >>> uqi(img1,img2)
+0.9586952304831419 ``` ## Example usage for command line interface ``` sewar
+[metric] [GT path] [P path] (any extra parameters) ``` An example to use SSIM
+```shell foo@bar:~$ sewar ssim images/ground_truth.tif images/deformed.tif -ws
+13 ssim : 0.8947009811410856 ``` Available metrics list ``` mse, rmse, psnr,
+rmse_sw, uqi, ssim, ergas, scc, rase, sam, msssim, vifp, psnrb ``` ##
+Contributors Special thanks to @sachinpuranik99 and @sunwj. ## References [1]
+"Image quality assessment: from error visibility to structural similarity."
+2004)
 [2] "A universal image quality index." (2002)
 [3] "Multiscale structural similarity for image quality assessment." (2003)
 [4] "Quality of high resolution synthesised images: Is there a simple
 criterion?." (2000)
 [5] "A wavelet transform method to merge Landsat TM and SPOT panchromatic
 data." (1998)
 [6] "Fusion of multispectral and panchromatic images using improved IHS and PCA
 mergers based on wavelet decomposition." (2004)
 [7] "Discrimination among semi-arid landscape endmembers using the spectral
 angle mapper (SAM) algorithm." (1992)
 [8] "Multispectral and panchromatic data fusion assessment without reference."
 (2008)
 [9] "Image information and visual quality." (2006)
 [10] "Quality Assessment of Deblocked Images" (2011)
-Keywords: image quality performance metric measure ergas q psnr pansharpening
-Platform: UNKNOWN Classifier: Development Status :: 2 - Pre-Alpha Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 2 Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7 Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.1
-Classifier: Programming Language :: Python :: 3.2 Classifier: Programming
-Language :: Python :: 3.3 Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5 Classifier: Programming
-Language :: Python :: 3.6 Classifier: Topic :: Multimedia :: Graphics
-Description-Content-Type: text/markdown
```

