# Comparing `tmp/logpie-3.0.3.tar.gz` & `tmp/logpie-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logpie-3.0.3.tar", last modified: Tue Jan  3 19:06:14 2023, max compression
+gzip compressed data, was "logpie-4.0.0.tar", last modified: Sun Jul 30 20:16:58 2023, max compression
```

## Comparing `logpie-3.0.3.tar` & `logpie-4.0.0.tar`

### file list

```diff
@@ -1,31 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-01-03 19:06:14.499315 logpie-3.0.3/
--rw-rw-rw-   0        0        0     1090 2022-09-04 16:28:17.000000 logpie-3.0.3/LICENSE
--rw-rw-rw-   0        0        0        0 2022-08-01 15:43:54.000000 logpie-3.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3817 2023-01-03 19:06:14.499315 logpie-3.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2872 2022-11-07 23:07:45.000000 logpie-3.0.3/README.md
--rw-rw-rw-   0        0        0       93 2022-08-10 18:07:14.000000 logpie-3.0.3/pyproject.toml
--rw-rw-rw-   0        0        0     1179 2023-01-03 19:06:14.514940 logpie-3.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-01-03 19:06:14.483669 logpie-3.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-01-03 19:06:14.499315 logpie-3.0.3/src/logpie/
--rw-rw-rw-   0        0        0      366 2022-12-30 11:12:21.000000 logpie-3.0.3/src/logpie/__init__.py
--rw-rw-rw-   0        0        0     2214 2023-01-03 11:00:31.000000 logpie-3.0.3/src/logpie/constants.py
--rw-rw-rw-   0        0        0     1251 2023-01-03 14:00:37.000000 logpie-3.0.3/src/logpie/descriptors.py
--rw-rw-rw-   0        0        0      693 2022-12-05 13:16:35.000000 logpie-3.0.3/src/logpie/exceptions.py
--rw-rw-rw-   0        0        0     5234 2022-11-09 16:31:45.000000 logpie-3.0.3/src/logpie/filehandlers.py
-drwxrwxrwx   0        0        0        0 2023-01-03 19:06:14.499315 logpie-3.0.3/src/logpie/filelockers/
--rw-rw-rw-   0        0        0      358 2022-07-30 18:57:43.000000 logpie-3.0.3/src/logpie/filelockers/__init__.py
--rw-rw-rw-   0        0        0      871 2022-11-07 21:15:50.000000 logpie-3.0.3/src/logpie/filelockers/constants.py
--rw-rw-rw-   0        0        0     4011 2022-07-25 08:09:02.000000 logpie-3.0.3/src/logpie/filelockers/core.py
--rw-rw-rw-   0        0        0      737 2022-08-18 13:31:16.000000 logpie-3.0.3/src/logpie/filelockers/exceptions.py
--rw-rw-rw-   0        0        0     2147 2022-11-07 21:15:50.000000 logpie-3.0.3/src/logpie/filelockers/handlers.py
--rw-rw-rw-   0        0        0    18595 2023-01-03 18:53:03.000000 logpie-3.0.3/src/logpie/handlers.py
--rw-rw-rw-   0        0        0     2340 2022-11-04 15:54:51.000000 logpie-3.0.3/src/logpie/registry.py
--rw-rw-rw-   0        0        0     2087 2022-12-02 16:02:36.000000 logpie-3.0.3/src/logpie/stackframe.py
--rw-rw-rw-   0        0        0     9487 2023-01-03 11:00:31.000000 logpie-3.0.3/src/logpie/utils.py
-drwxrwxrwx   0        0        0        0 2023-01-03 19:06:14.499315 logpie-3.0.3/src/logpie.egg-info/
--rw-rw-rw-   0        0        0     3817 2023-01-03 19:06:14.000000 logpie-3.0.3/src/logpie.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      646 2023-01-03 19:06:14.000000 logpie-3.0.3/src/logpie.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-03 19:06:14.000000 logpie-3.0.3/src/logpie.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-11-07 23:13:27.000000 logpie-3.0.3/src/logpie.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       77 2023-01-03 19:06:14.000000 logpie-3.0.3/src/logpie.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-01-03 19:06:14.000000 logpie-3.0.3/src/logpie.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 20:16:58.388157 logpie-4.0.0/
+-rw-rw-rw-   0        0        0     1090 2022-09-04 16:28:17.000000 logpie-4.0.0/LICENSE
+-rw-rw-rw-   0        0        0       14 2023-05-04 22:14:01.000000 logpie-4.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    11197 2023-07-30 20:16:58.388157 logpie-4.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10401 2023-07-30 20:10:16.000000 logpie-4.0.0/README.md
+-rw-rw-rw-   0        0        0       93 2022-08-10 18:07:14.000000 logpie-4.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      956 2023-07-30 20:16:58.388157 logpie-4.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-30 20:16:58.371535 logpie-4.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-30 20:16:58.388157 logpie-4.0.0/src/logpie/
+-rw-rw-rw-   0        0        0      275 2023-07-08 00:44:24.000000 logpie-4.0.0/src/logpie/__init__.py
+-rw-rw-rw-   0        0        0     1220 2023-07-08 00:44:24.000000 logpie-4.0.0/src/logpie/constants.py
+-rw-rw-rw-   0        0        0      649 2023-07-08 00:44:24.000000 logpie-4.0.0/src/logpie/exceptions.py
+-rw-rw-rw-   0        0        0    32749 2023-07-30 20:10:16.000000 logpie-4.0.0/src/logpie/handlers.py
+-rw-rw-rw-   0        0        0      562 2023-07-08 00:44:24.000000 logpie-4.0.0/src/logpie/mapping.py
+-rw-rw-rw-   0        0        0     2376 2023-07-08 00:44:24.000000 logpie-4.0.0/src/logpie/stackframe.py
+-rw-rw-rw-   0        0        0     1525 2023-07-08 00:44:24.000000 logpie-4.0.0/src/logpie/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-30 20:16:58.388157 logpie-4.0.0/src/logpie.egg-info/
+-rw-rw-rw-   0        0        0    11197 2023-07-30 20:16:58.000000 logpie-4.0.0/src/logpie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-07-30 20:16:58.000000 logpie-4.0.0/src/logpie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 20:16:58.000000 logpie-4.0.0/src/logpie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-11-07 23:13:27.000000 logpie-4.0.0/src/logpie.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-07-30 20:16:58.000000 logpie-4.0.0/src/logpie.egg-info/top_level.txt
```

### Comparing `logpie-3.0.3/LICENSE` & `logpie-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logpie-3.0.3/setup.cfg` & `logpie-4.0.0/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -1,74 +1,60 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 6f67 7069 650d 0a76 6572 7369   = logpie..versi
-00000020: 6f6e 203d 2033 2e30 2e33 0d0a 6175 7468  on = 3.0.3..auth
+00000020: 6f6e 203d 2034 2e30 2e30 0d0a 6175 7468  on = 4.0.0..auth
 00000030: 6f72 203d 2043 6c61 7564 6975 2044 5255  or = Claudiu DRU
 00000040: 470d 0a61 7574 686f 725f 656d 6169 6c20  G..author_email 
 00000050: 3d20 636c 6175 6469 752e 6472 7567 406f  = claudiu.drug@o
 00000060: 7574 6c6f 6f6b 2e63 6f6d 0d0a 6c69 6365  utlook.com..lice
 00000070: 6e73 6520 3d20 4d49 5420 4c69 6365 6e73  nse = MIT Licens
 00000080: 650d 0a64 6573 6372 6970 7469 6f6e 203d  e..description =
-00000090: 204c 6f67 6769 6e67 206d 6164 6520 7369   Logging made si
-000000a0: 6d70 6c65 2e0d 0a6c 6f6e 675f 6465 7363  mple...long_desc
-000000b0: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
-000000c0: 5245 4144 4d45 2e6d 640d 0a6c 6f6e 675f  README.md..long_
-000000d0: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
-000000e0: 656e 745f 7479 7065 203d 2074 6578 742f  ent_type = text/
-000000f0: 6d61 726b 646f 776e 0d0a 7572 6c20 3d20  markdown..url = 
-00000100: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000110: 6f6d 2f43 6c61 7564 6975 4472 7567 2f6c  om/ClaudiuDrug/l
-00000120: 6f67 7069 650d 0a70 726f 6a65 6374 5f75  ogpie..project_u
-00000130: 726c 7320 3d20 0d0a 0942 7567 2054 7261  rls = ...Bug Tra
-00000140: 636b 6572 203d 2068 7474 7073 3a2f 2f67  cker = https://g
-00000150: 6974 6875 622e 636f 6d2f 436c 6175 6469  ithub.com/Claudi
-00000160: 7544 7275 672f 6c6f 6770 6965 2f69 7373  uDrug/logpie/iss
-00000170: 7565 730d 0a63 6c61 7373 6966 6965 7273  ues..classifiers
-00000180: 203d 200d 0a09 5072 6f67 7261 6d6d 696e   = ...Programmin
-00000190: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000001a0: 7468 6f6e 203a 3a20 332e 370d 0a09 5072  thon :: 3.7...Pr
-000001b0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000001c0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000001d0: 332e 380d 0a09 5072 6f67 7261 6d6d 696e  3.8...Programmin
-000001e0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000001f0: 7468 6f6e 203a 3a20 332e 390d 0a09 5072  thon :: 3.9...Pr
-00000200: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000210: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000220: 332e 3130 0d0a 094c 6963 656e 7365 203a  3.10...License :
-00000230: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-00000240: 3a20 4d49 5420 4c69 6365 6e73 650d 0a09  : MIT License...
-00000250: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
-00000260: 203a 3a20 4d69 6372 6f73 6f66 7420 3a3a   :: Microsoft ::
-00000270: 2057 696e 646f 7773 203a 3a20 5769 6e64   Windows :: Wind
-00000280: 6f77 7320 3130 0d0a 094f 7065 7261 7469  ows 10...Operati
-00000290: 6e67 2053 7973 7465 6d20 3a3a 2050 4f53  ng System :: POS
-000002a0: 4958 203a 3a20 4c69 6e75 780d 0a09 496e  IX :: Linux...In
-000002b0: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
-000002c0: 3a3a 2044 6576 656c 6f70 6572 730d 0a09  :: Developers...
-000002d0: 4e61 7475 7261 6c20 4c61 6e67 7561 6765  Natural Language
-000002e0: 203a 3a20 456e 676c 6973 680d 0a09 546f   :: English...To
-000002f0: 7069 6320 3a3a 2053 6f66 7477 6172 6520  pic :: Software 
-00000300: 4465 7665 6c6f 706d 656e 7420 3a3a 204c  Development :: L
-00000310: 6962 7261 7269 6573 203a 3a20 5079 7468  ibraries :: Pyth
-00000320: 6f6e 204d 6f64 756c 6573 0d0a 0954 6f70  on Modules...Top
-00000330: 6963 203a 3a20 5574 696c 6974 6965 730d  ic :: Utilities.
-00000340: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 7a69  ...[options]..zi
-00000350: 705f 7361 6665 203d 2046 616c 7365 0d0a  p_safe = False..
-00000360: 7061 636b 6167 6573 203d 2066 696e 645f  packages = find_
-00000370: 6e61 6d65 7370 6163 653a 0d0a 7061 636b  namespace:..pack
-00000380: 6167 655f 6469 7220 3d20 0d0a 093d 2073  age_dir = ...= s
-00000390: 7263 0d0a 696e 636c 7564 655f 7061 636b  rc..include_pack
-000003a0: 6167 655f 6461 7461 203d 2054 7275 650d  age_data = True.
-000003b0: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
-000003c0: 203d 203e 3d20 332e 370d 0a69 6e73 7461   = >= 3.7..insta
-000003d0: 6c6c 5f72 6571 7569 7265 7320 3d20 0d0a  ll_requires = ..
-000003e0: 0963 6667 7069 6520 3d3d 2032 2e33 2e31  .cfgpie == 2.3.1
-000003f0: 300d 0a09 636f 6c6f 7270 6965 203d 3d20  0...colorpie == 
-00000400: 302e 302e 310d 0a09 7079 7769 6e33 3220  0.0.1...pywin32 
-00000410: 3d3d 2033 3035 3b20 706c 6174 666f 726d  == 305; platform
-00000420: 5f73 7973 7465 6d20 3d3d 2027 5769 6e64  _system == 'Wind
-00000430: 6f77 7327 0d0a 0d0a 5b6f 7074 696f 6e73  ows'....[options
-00000440: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
-00000450: 0a77 6865 7265 203d 2073 7263 0d0a 6578  .where = src..ex
-00000460: 636c 7564 6520 3d20 7465 7374 730d 0a0d  clude = tests...
-00000470: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
-00000480: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
-00000490: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
+00000090: 2053 696d 706c 6520 6c6f 6767 696e 6720   Simple logging 
+000000a0: 6672 616d 6577 6f72 6b2e 0d0a 6c6f 6e67  framework...long
+000000b0: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
+000000c0: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
+000000d0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+000000e0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
+000000f0: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
+00000100: 726c 203d 2068 7474 7073 3a2f 2f67 6974  rl = https://git
+00000110: 6875 622e 636f 6d2f 436c 6175 6469 7544  hub.com/ClaudiuD
+00000120: 7275 672f 6c6f 6770 6965 0d0a 7072 6f6a  rug/logpie..proj
+00000130: 6563 745f 7572 6c73 203d 200d 0a09 4275  ect_urls = ...Bu
+00000140: 6720 5472 6163 6b65 7220 3d20 6874 7470  g Tracker = http
+00000150: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f43  s://github.com/C
+00000160: 6c61 7564 6975 4472 7567 2f6c 6f67 7069  laudiuDrug/logpi
+00000170: 652f 6973 7375 6573 0d0a 636c 6173 7369  e/issues..classi
+00000180: 6669 6572 7320 3d20 0d0a 0950 726f 6772  fiers = ...Progr
+00000190: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+000001a0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e37  :: Python :: 3.7
+000001b0: 0d0a 094c 6963 656e 7365 203a 3a20 4f53  ...License :: OS
+000001c0: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
+000001d0: 5420 4c69 6365 6e73 650d 0a09 4f70 6572  T License...Oper
+000001e0: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
+000001f0: 4d69 6372 6f73 6f66 7420 3a3a 2057 696e  Microsoft :: Win
+00000200: 646f 7773 203a 3a20 5769 6e64 6f77 7320  dows :: Windows 
+00000210: 3130 0d0a 094f 7065 7261 7469 6e67 2053  10...Operating S
+00000220: 7973 7465 6d20 3a3a 2050 4f53 4958 203a  ystem :: POSIX :
+00000230: 3a20 4c69 6e75 780d 0a09 496e 7465 6e64  : Linux...Intend
+00000240: 6564 2041 7564 6965 6e63 6520 3a3a 2044  ed Audience :: D
+00000250: 6576 656c 6f70 6572 730d 0a09 4e61 7475  evelopers...Natu
+00000260: 7261 6c20 4c61 6e67 7561 6765 203a 3a20  ral Language :: 
+00000270: 456e 676c 6973 680d 0a09 546f 7069 6320  English...Topic 
+00000280: 3a3a 2053 6f66 7477 6172 6520 4465 7665  :: Software Deve
+00000290: 6c6f 706d 656e 7420 3a3a 204c 6962 7261  lopment :: Libra
+000002a0: 7269 6573 203a 3a20 5079 7468 6f6e 204d  ries :: Python M
+000002b0: 6f64 756c 6573 0d0a 0954 6f70 6963 203a  odules...Topic :
+000002c0: 3a20 5574 696c 6974 6965 730d 0a0d 0a5b  : Utilities....[
+000002d0: 6f70 7469 6f6e 735d 0d0a 7a69 705f 7361  options]..zip_sa
+000002e0: 6665 203d 2046 616c 7365 0d0a 7061 636b  fe = False..pack
+000002f0: 6167 6573 203d 2066 696e 645f 6e61 6d65  ages = find_name
+00000300: 7370 6163 653a 0d0a 7061 636b 6167 655f  space:..package_
+00000310: 6469 7220 3d20 0d0a 093d 2073 7263 0d0a  dir = ...= src..
+00000320: 696e 636c 7564 655f 7061 636b 6167 655f  include_package_
+00000330: 6461 7461 203d 2054 7275 650d 0a70 7974  data = True..pyt
+00000340: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
+00000350: 3d20 332e 370d 0a0d 0a5b 6f70 7469 6f6e  = 3.7....[option
+00000360: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
+00000370: 0d0a 7768 6572 6520 3d20 7372 630d 0a65  ..where = src..e
+00000380: 7863 6c75 6465 203d 2074 6573 7473 0d0a  xclude = tests..
+00000390: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
+000003a0: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
+000003b0: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
```

### Comparing `logpie-3.0.3/src/logpie/stackframe.py` & `logpie-4.0.0/src/logpie/stackframe.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 # -*- coding: UTF-8 -*-
 
 from os.path import basename
 from sys import exc_info, _getframe as get_frame
 from typing import Union
 
-from .constants import FRAME
+from .mapping import Traceback, Frame
 
+__all__ = [
+    "get_traceback",
+    "get_caller",
+    "get_file",
+    "get_code",
+    "get_message",
+]
 
-def get_traceback(exception: Union[BaseException, tuple, bool]) -> FRAME:
+
+def get_traceback(exception: Union[BaseException, tuple, bool]) -> Traceback:
     """
     Get information about the most recent exception caught by an except clause
     in the current stack frame or in an older stack frame.
 
     :param exception: If enabled it will return info about the most recent exception caught.
     :return: The file name, line number, name of code object and traceback message.
     :raise AttributeError: If exception is enabled and no traceback is found.
@@ -23,39 +31,39 @@
         exception = exc_info()
 
     try:
         tb_frame = exception[-1].tb_frame
     except AttributeError:
         raise
     else:
-        return FRAME(
+        return Traceback(
             file=get_file(tb_frame),
             line=exception[-1].tb_lineno,
             code=get_code(tb_frame),
-            traceback=f"{exception[0].__name__}({exception[1]})",
+            message=get_message(exception),
         )
 
 
-def get_caller(depth: int) -> FRAME:
+def get_caller(depth: int) -> Frame:
     """
     Get information about the frame object from the call stack.
 
     :param depth: Number of calls below the top of the stack.
     :return: The file name, line number and name of code object.
     """
     try:
         frame = get_frame(depth)
     except ValueError:
-        raise
+        depth -= 1
+        return get_caller(depth)
     else:
-        return FRAME(
+        return Frame(
             file=get_file(frame),
             line=frame.f_lineno,
             code=get_code(frame),
-            traceback=None,
         )
 
 
 def get_file(frame) -> str:
     """Frame file name getter."""
     return basename(frame.f_code.co_filename)
 
@@ -64,7 +72,12 @@
     """Frame object name getter."""
     try:
         co_class = frame.f_locals["self"].__class__.__name__
     except KeyError:
         return frame.f_code.co_name
     else:
         return f"{co_class}.{frame.f_code.co_name}"
+
+
+def get_message(exception: tuple) -> str:
+    """Extract the traceback message from the given `exception`."""
+    return f"{exception[0].__name__}({exception[1]})"
```

