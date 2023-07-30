# Comparing `tmp/pmcxcl-0.0.7-pp39-pypy39_pp73-win_amd64.whl.zip` & `tmp/pmcxcl-0.0.8-pp39-pypy39_pp73-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 137504 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat   321536 b- defN 23-Jul-30 18:51 _pmcxcl.pypy39-pp73-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1626 b- defN 23-Jul-30 18:47 pmcxcl/__init__.py
--rw-rw-rw-  2.0 fat     1737 b- defN 23-Jul-30 18:47 pmcxcl/bench.py
--rw-rw-rw-  2.0 fat     9258 b- defN 23-Jul-30 18:51 pmcxcl-0.0.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat      107 b- defN 23-Jul-30 18:51 pmcxcl-0.0.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-Jul-30 18:51 pmcxcl-0.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      534 b- defN 23-Jul-30 18:51 pmcxcl-0.0.7.dist-info/RECORD
-7 files, 334813 bytes uncompressed, 136570 bytes compressed:  59.2%
+Zip file size: 871555 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat  1817600 b- defN 23-Jul-30 19:08 _pmcxcl.pypy39-pp73-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     1626 b- defN 23-Jul-30 19:05 pmcxcl/__init__.py
+-rw-rw-rw-  2.0 fat     1737 b- defN 23-Jul-30 19:05 pmcxcl/bench.py
+-rw-rw-rw-  2.0 fat     9258 b- defN 23-Jul-30 19:08 pmcxcl-0.0.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      107 b- defN 23-Jul-30 19:08 pmcxcl-0.0.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-Jul-30 19:08 pmcxcl-0.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      535 b- defN 23-Jul-30 19:08 pmcxcl-0.0.8.dist-info/RECORD
+7 files, 1830878 bytes uncompressed, 870621 bytes compressed:  52.4%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: pmcxcl/__init__.py
 Comment: 
 
 Filename: pmcxcl/bench.py
 Comment: 
 
-Filename: pmcxcl-0.0.7.dist-info/METADATA
+Filename: pmcxcl-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: pmcxcl-0.0.7.dist-info/WHEEL
+Filename: pmcxcl-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: pmcxcl-0.0.7.dist-info/top_level.txt
+Filename: pmcxcl-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: pmcxcl-0.0.7.dist-info/RECORD
+Filename: pmcxcl-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pmcxcl/__init__.py

```diff
@@ -33,10 +33,10 @@
 except ImportError:  # pragma: no cover
     print("the pmcxcl binary extension (_pmcxcl) is not compiled! please compile first")
 
 # from .utils import detweight, cwdref
 # from .files import loadmc2, loadmch, load, save
 from .bench import bench
 
-__version__ = "0.0.7"
+__version__ = "0.0.8"
 
 __all__ = ("gpuinfo", "run", "bench")
```

## Comparing `pmcxcl-0.0.7.dist-info/METADATA` & `pmcxcl-0.0.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmcxcl
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python bindings for Monte Carlo eXtreme photon transport simulator
 Home-page: https://github.com/fangq/mcxcl
 Author: Matin Raayai Ardakani, Qianqian Fang
 Author-email: raayaiardakani.m@northeastern.edu, q.fang@neu.edu
 Maintainer: Qianqian Fang
 License: GPLv3+
 Download-URL: http://mcx.space
@@ -28,15 +28,15 @@
 ![](http://mcx.space/img/mcx18_banner.png)
 
 # PMCX-CL - Python bindings for Monte Carlo eXtreme (OpenCL) photon transport simulator
 
 - Copyright: (C) Matin Raayai Ardakani (2022-2023) <raayaiardakani.m at northeastern.edu> 
 and Qianqian Fang (2019-2023) <q.fang at neu.edu>
 - License: GNU Public License V3 or later
-- Version: 0.0.7
+- Version: 0.0.8
 - URL: https://pypi.org/project/pmcxcl/
 - Github: https://github.com/fangq/mcxcl
 
 ![Linux Python Module](https://github.com/fangq/mcxcl/actions/workflows/build_linux_manywheel.yml/badge.svg)\
 ![MacOS Python Module](https://github.com/fangq/mcxcl/actions/workflows/build_macos_wheel.yml/badge.svg)\
 ![Windows Python Module](https://github.com/fangq/mcxcl/actions/workflows/build_windows_wheel.yml/badge.svg)\
 ![Mex and Binaries](https://github.com/fangq/mcxcl/actions/workflows/build_all.yml/badge.svg)
```

