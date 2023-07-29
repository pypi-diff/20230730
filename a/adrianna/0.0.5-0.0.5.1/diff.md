# Comparing `tmp/adrianna-0.0.5-py3-none-any.whl.zip` & `tmp/adrianna-0.0.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,8 @@
-Zip file size: 2682 bytes, number of entries: 5
--rw-rw-r--  2.0 unx     1497 b- defN 23-Jul-21 16:36 adrianna-0.0.5.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1783 b- defN 23-Jul-21 16:36 adrianna-0.0.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-21 16:36 adrianna-0.0.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx        1 b- defN 23-Jul-21 16:36 adrianna-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      390 b- defN 23-Jul-21 16:36 adrianna-0.0.5.dist-info/RECORD
-5 files, 3763 bytes uncompressed, 1952 bytes compressed:  48.1%
+Zip file size: 2859 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-29 23:04 adrianna/__init__.py
+-rw-rw-r--  2.0 unx     1497 b- defN 23-Jul-29 23:12 adrianna-0.0.5.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1770 b- defN 23-Jul-29 23:12 adrianna-0.0.5.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-29 23:12 adrianna-0.0.5.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-Jul-29 23:12 adrianna-0.0.5.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      474 b- defN 23-Jul-29 23:12 adrianna-0.0.5.1.dist-info/RECORD
+6 files, 3842 bytes uncompressed, 1993 bytes compressed:  48.1%
```

## zipnote {}

```diff
@@ -1,16 +1,19 @@
-Filename: adrianna-0.0.5.dist-info/LICENSE
+Filename: adrianna/__init__.py
 Comment: 
 
-Filename: adrianna-0.0.5.dist-info/METADATA
+Filename: adrianna-0.0.5.1.dist-info/LICENSE
 Comment: 
 
-Filename: adrianna-0.0.5.dist-info/WHEEL
+Filename: adrianna-0.0.5.1.dist-info/METADATA
 Comment: 
 
-Filename: adrianna-0.0.5.dist-info/top_level.txt
+Filename: adrianna-0.0.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: adrianna-0.0.5.dist-info/RECORD
+Filename: adrianna-0.0.5.1.dist-info/top_level.txt
+Comment: 
+
+Filename: adrianna-0.0.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `adrianna-0.0.5.dist-info/LICENSE` & `adrianna-0.0.5.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `adrianna-0.0.5.dist-info/METADATA` & `adrianna-0.0.5.1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: adrianna
-Version: 0.0.5
+Version: 0.0.5.1
 Summary: lib for development with machine learning
 Home-page: https://github.com/reinanbr/adriana
 Author: Reinan Br
 Author-email: slimchatuba@gmail.com
 License: MIT License
 Keywords: ia machine learning math
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 
  <div align='center'>
 
- <img  height='400px' width='460px' src='https://github.com/reinanbr/logos/blob/main/IMG_20230717_013052.png?raw=true'>
+ <img  height='400px' width='460px' src='https://github.com/reinanbr/logos/blob/main/logo.jpg?raw=true'>
 
 <h1>Adriana</h1>
 
 <p> A powerfull lib, for development in machine learning</p>
 <a href='#'><img alt="CodeFactor Grade" src="https://img.shields.io/codefactor/grade/github/reinanbr/dreams?logo=codefactor">
 </a><img alt="CircleCI" src="https://img.shields.io/circleci/build/github/reinanbr/dreams">
 <img alt="Code Climate maintainability" src="https://img.shields.io/codeclimate/maintainability-percentage/reinanbr/dreams">
```

### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: adrianna Version: 0.0.5 Summary: lib for
+Metadata-Version: 2.1 Name: adrianna Version: 0.0.5.1 Summary: lib for
 development with machine learning Home-page: https://github.com/reinanbr/
 adriana Author: Reinan Br Author-email: slimchatuba@gmail.com License: MIT
 License Keywords: ia machine learning math Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: numpy Requires-Dist: scipy
-[https://github.com/reinanbr/logos/blob/main/IMG_20230717_013052.png?raw=true]
+        [https://github.com/reinanbr/logos/blob/main/logo.jpg?raw=true]
                              ****** Adriana ******
              A powerfull lib, for development in machine learning
         [CodeFactor_Grade][CircleCI] [Code Climate maintainability]
 [https://shields.io/badge/insta-reysofts-darkviolet?logo=instagram&style=flat]
 
 [Buy_Me_A_Coffee]
 ===============================================================================
```

