# Comparing `tmp/Python_Print_Tools-0.1.1-py3-none-any.whl.zip` & `tmp/Python_Print_Tools-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,11 @@
-Zip file size: 15810 bytes, number of entries: 10
--rw-rw-r--  2.0 unx       23 b- defN 22-Sep-17 22:05 python_print_tools/__init__.py
--rw-rw-r--  2.0 unx       23 b- defN 22-Sep-17 22:05 python_print_tools/main/__init__.py
--rw-rw-r--  2.0 unx     3130 b- defN 22-Sep-21 17:10 python_print_tools/main/python_print_tools.py
--rw-rw-r--  2.0 unx       23 b- defN 22-Sep-17 22:05 python_print_tools/test/__init__.py
--rw-rw-r--  2.0 unx      668 b- defN 22-Sep-21 17:10 python_print_tools/test/test_python_print_tools.py
--rw-rw-r--  2.0 unx    35149 b- defN 22-Sep-21 17:19 Python_Print_Tools-0.1.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx      549 b- defN 22-Sep-21 17:19 Python_Print_Tools-0.1.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Sep-21 17:19 Python_Print_Tools-0.1.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       19 b- defN 22-Sep-21 17:19 Python_Print_Tools-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      914 b- defN 22-Sep-21 17:19 Python_Print_Tools-0.1.1.dist-info/RECORD
-10 files, 40590 bytes uncompressed, 14210 bytes compressed:  65.0%
+Zip file size: 15574 bytes, number of entries: 9
+-rw-r--r--  2.0 unx       23 b- defN 23-Jul-30 20:50 python_print_tools/__init__.py
+-rw-r--r--  2.0 unx     3133 b- defN 23-Jul-30 20:55 python_print_tools/printer.py
+-rw-r--r--  2.0 unx       23 b- defN 23-Jul-30 20:50 python_print_tools/tests/__init__.py
+-rw-r--r--  2.0 unx      719 b- defN 23-Jul-30 20:58 python_print_tools/tests/test_printer.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jul-30 21:00 Python_Print_Tools-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      549 b- defN 23-Jul-30 21:00 Python_Print_Tools-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-30 21:00 Python_Print_Tools-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-Jul-30 21:00 Python_Print_Tools-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      799 b- defN 23-Jul-30 21:00 Python_Print_Tools-0.2.0.dist-info/RECORD
+9 files, 40506 bytes uncompressed, 14170 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -1,31 +1,28 @@
 Filename: python_print_tools/__init__.py
 Comment: 
 
-Filename: python_print_tools/main/__init__.py
+Filename: python_print_tools/printer.py
 Comment: 
 
-Filename: python_print_tools/main/python_print_tools.py
+Filename: python_print_tools/tests/__init__.py
 Comment: 
 
-Filename: python_print_tools/test/__init__.py
+Filename: python_print_tools/tests/test_printer.py
 Comment: 
 
-Filename: python_print_tools/test/test_python_print_tools.py
+Filename: Python_Print_Tools-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: Python_Print_Tools-0.1.1.dist-info/LICENSE
+Filename: Python_Print_Tools-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: Python_Print_Tools-0.1.1.dist-info/METADATA
+Filename: Python_Print_Tools-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: Python_Print_Tools-0.1.1.dist-info/WHEEL
+Filename: Python_Print_Tools-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: Python_Print_Tools-0.1.1.dist-info/top_level.txt
-Comment: 
-
-Filename: Python_Print_Tools-0.1.1.dist-info/RECORD
+Filename: Python_Print_Tools-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `python_print_tools/main/python_print_tools.py` & `python_print_tools/printer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-from os.path import abspath
+import os.path
 from typing import List
 
 def get_color_code(color:str) -> str:
     """
     Returns an ANSI color code for a given color.
     white: "w", red: "r", green: "g" blue: "b"
     black: "k", cyan: "c", yellow: "y", magenta: "m"
@@ -73,16 +73,16 @@
     :type base_dir: str, required
     :param file: Given file to truncate
     :type file: str, required
     :return: Relative path of the given file
     :rtype: str
     """
     # Return file unaltered if not inside the base directory
-    full_base = abspath(base_dir)
-    full_file = abspath(file)
+    full_base = os.path.abspath(base_dir)
+    full_file = os.path.abspath(file)
     if full_base == full_file or not full_file.startswith(full_base):
         return full_file
     # Truncate the path of the given file
     truncated = full_file[len(full_base):]
     return f"...{truncated}"
 
 def print_files(base_dir:str, files:List[str]):
```

## Comparing `Python_Print_Tools-0.1.1.dist-info/LICENSE` & `Python_Print_Tools-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `Python_Print_Tools-0.1.1.dist-info/METADATA` & `Python_Print_Tools-0.2.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Python-Print-Tools
-Version: 0.1.1
+Version: 0.2.0
 Summary: Basic utility for printing info to console.
 Home-page: https://github.com/Drakovek/Python-Print-Tools
 Author: Drakovek
 Author-email: DrakovekMail@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

## Comparing `Python_Print_Tools-0.1.1.dist-info/RECORD` & `Python_Print_Tools-0.2.0.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 python_print_tools/__init__.py,sha256=1oLL20yLB1GL9IbFiZD8OReDqiCpFr-yetIR6x1cNkI,23
-python_print_tools/main/__init__.py,sha256=1oLL20yLB1GL9IbFiZD8OReDqiCpFr-yetIR6x1cNkI,23
-python_print_tools/main/python_print_tools.py,sha256=qpLitcjAasG9j-UUVkB3u3sDMhAQgqioGiMmktgYWeY,3130
-python_print_tools/test/__init__.py,sha256=1oLL20yLB1GL9IbFiZD8OReDqiCpFr-yetIR6x1cNkI,23
-python_print_tools/test/test_python_print_tools.py,sha256=UEFGHAuqYC8xyNqSjYEvshKupzCDyk3qYyKcp3OcikA,668
-Python_Print_Tools-0.1.1.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-Python_Print_Tools-0.1.1.dist-info/METADATA,sha256=arT_IEc9AzEipy00WgsfjQfnSlnRLH3HerM6qoAgUNA,549
-Python_Print_Tools-0.1.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-Python_Print_Tools-0.1.1.dist-info/top_level.txt,sha256=GhsLKeoLYN3PXsejqKu21kMsygGusDEtlnLCuFaq5gc,19
-Python_Print_Tools-0.1.1.dist-info/RECORD,,
+python_print_tools/printer.py,sha256=ZVNVz672FsOTZ-5RxnUPAjCg4XHXMHTZgvRRVMZteaU,3133
+python_print_tools/tests/__init__.py,sha256=1oLL20yLB1GL9IbFiZD8OReDqiCpFr-yetIR6x1cNkI,23
+python_print_tools/tests/test_printer.py,sha256=_gznCA1mU02A1sDK7BxICzpVwG3lthuQV--tM_Zzm1c,719
+Python_Print_Tools-0.2.0.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+Python_Print_Tools-0.2.0.dist-info/METADATA,sha256=3Omdx7yctEvP39Wz9YzmCaeoSGcMcSp2HOs96EZThec,549
+Python_Print_Tools-0.2.0.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+Python_Print_Tools-0.2.0.dist-info/top_level.txt,sha256=GhsLKeoLYN3PXsejqKu21kMsygGusDEtlnLCuFaq5gc,19
+Python_Print_Tools-0.2.0.dist-info/RECORD,,
```

