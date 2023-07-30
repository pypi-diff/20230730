# Comparing `tmp/pmcxcl-0.0.5-pp39-pypy39_pp73-win_amd64.whl.zip` & `tmp/pmcxcl-0.0.6-pp39-pypy39_pp73-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 870819 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat  1814528 b- defN 23-Jul-30 04:57 _pmcxcl.pypy39-pp73-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1626 b- defN 23-Jul-30 04:53 pmcxcl/__init__.py
--rw-rw-rw-  2.0 fat     1737 b- defN 23-Jul-30 04:53 pmcxcl/bench.py
--rw-rw-rw-  2.0 fat     9258 b- defN 23-Jul-30 04:57 pmcxcl-0.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat      107 b- defN 23-Jul-30 04:57 pmcxcl-0.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-Jul-30 04:57 pmcxcl-0.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      535 b- defN 23-Jul-30 04:57 pmcxcl-0.0.5.dist-info/RECORD
-7 files, 1827806 bytes uncompressed, 869885 bytes compressed:  52.4%
+Zip file size: 870843 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat  1815040 b- defN 23-Jul-30 05:40 _pmcxcl.pypy39-pp73-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     1626 b- defN 23-Jul-30 05:36 pmcxcl/__init__.py
+-rw-rw-rw-  2.0 fat     1737 b- defN 23-Jul-30 05:36 pmcxcl/bench.py
+-rw-rw-rw-  2.0 fat     9258 b- defN 23-Jul-30 05:40 pmcxcl-0.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      107 b- defN 23-Jul-30 05:40 pmcxcl-0.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-Jul-30 05:40 pmcxcl-0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      535 b- defN 23-Jul-30 05:40 pmcxcl-0.0.6.dist-info/RECORD
+7 files, 1828318 bytes uncompressed, 869909 bytes compressed:  52.4%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: pmcxcl/__init__.py
 Comment: 
 
 Filename: pmcxcl/bench.py
 Comment: 
 
-Filename: pmcxcl-0.0.5.dist-info/METADATA
+Filename: pmcxcl-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: pmcxcl-0.0.5.dist-info/WHEEL
+Filename: pmcxcl-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: pmcxcl-0.0.5.dist-info/top_level.txt
+Filename: pmcxcl-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: pmcxcl-0.0.5.dist-info/RECORD
+Filename: pmcxcl-0.0.6.dist-info/RECORD
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
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 
 __all__ = ("gpuinfo", "run", "bench")
```

## Comparing `pmcxcl-0.0.5.dist-info/METADATA` & `pmcxcl-0.0.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmcxcl
-Version: 0.0.5
+Version: 0.0.6
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
-- Version: 0.0.5
+- Version: 0.0.6
 - URL: https://pypi.org/project/pmcxcl/
 - Github: https://github.com/fangq/mcxcl
 
 ![Linux Python Module](https://github.com/fangq/mcxcl/actions/workflows/build_linux_manywheel.yml/badge.svg)\
 ![MacOS Python Module](https://github.com/fangq/mcxcl/actions/workflows/build_macos_wheel.yml/badge.svg)\
 ![Windows Python Module](https://github.com/fangq/mcxcl/actions/workflows/build_windows_wheel.yml/badge.svg)\
 ![Mex and Binaries](https://github.com/fangq/mcxcl/actions/workflows/build_all.yml/badge.svg)
```

## Comparing `pmcxcl-0.0.5.dist-info/RECORD` & `pmcxcl-0.0.6.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-_pmcxcl.pypy39-pp73-win_amd64.pyd,sha256=Ecd0mllycGGrnKLb-BJtb_LnaTrA3gvoDiR40XTHzyI,1814528
-pmcxcl/__init__.py,sha256=pWfs_bTcMcjjrxreEn2h30c9jZsNuVTKCeWYPKJv4TY,1626
+_pmcxcl.pypy39-pp73-win_amd64.pyd,sha256=dHsguR_sVMxjKnKA2_GA1IVTl1Uc6l-phEE-XFJ7c5A,1815040
+pmcxcl/__init__.py,sha256=kQSZYXODy3alMlC5XnbThUj8MKArvac9aeMvmIp96ZE,1626
 pmcxcl/bench.py,sha256=ViIdfMofDIdV9edqc9hEoNkpXMArX7oxLUwnLxHc_BA,1737
-pmcxcl-0.0.5.dist-info/METADATA,sha256=t1iFRf3JGkvh7cK2fYPK7ivGAHQ-tSg-d-dOGbFOt-8,9258
-pmcxcl-0.0.5.dist-info/WHEEL,sha256=FWw5WrGV_MgVgz_vQM6GPj9TGPn-tcb9Rh6zoPjcZec,107
-pmcxcl-0.0.5.dist-info/top_level.txt,sha256=3-gVHSwlcrGhE7o2MkqTEMT52F8ryBxG6m9vPdb3Pu8,15
-pmcxcl-0.0.5.dist-info/RECORD,,
+pmcxcl-0.0.6.dist-info/METADATA,sha256=1kHgaLS38jsWHWolN8e-M33AYv8VOsKceyTNdjzxJzw,9258
+pmcxcl-0.0.6.dist-info/WHEEL,sha256=FWw5WrGV_MgVgz_vQM6GPj9TGPn-tcb9Rh6zoPjcZec,107
+pmcxcl-0.0.6.dist-info/top_level.txt,sha256=3-gVHSwlcrGhE7o2MkqTEMT52F8ryBxG6m9vPdb3Pu8,15
+pmcxcl-0.0.6.dist-info/RECORD,,
```

