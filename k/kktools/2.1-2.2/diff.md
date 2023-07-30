# Comparing `tmp/kktools-2.1.tar.gz` & `tmp/kktools-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kktools-2.1.tar", last modified: Sat Jul  9 12:04:28 2022, max compression
+gzip compressed data, was "kktools-2.2.tar", last modified: Sun Jul 30 17:28:04 2023, max compression
```

## Comparing `kktools-2.1.tar` & `kktools-2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-07-09 12:04:28.967354 kktools-2.1/
--rw-rw-rw-   0        0        0     1095 2022-03-13 08:04:57.000000 kktools-2.1/LICENSE
--rw-rw-rw-   0        0        0     1416 2022-07-09 12:04:28.967354 kktools-2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1094 2022-05-15 08:54:03.000000 kktools-2.1/README.md
-drwxrwxrwx   0        0        0        0 2022-07-09 12:04:28.945970 kktools-2.1/kktools/
--rw-rw-rw-   0        0        0      172 2022-05-15 08:32:02.000000 kktools-2.1/kktools/__init__.py
--rw-rw-rw-   0        0        0     5478 2022-07-09 07:22:32.000000 kktools-2.1/kktools/core.py
-drwxrwxrwx   0        0        0        0 2022-07-09 12:04:28.966357 kktools-2.1/kktools.egg-info/
--rw-rw-rw-   0        0        0     1416 2022-07-09 12:04:28.000000 kktools-2.1/kktools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2022-07-09 12:04:28.000000 kktools-2.1/kktools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-09 12:04:28.000000 kktools-2.1/kktools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2022-07-09 12:04:28.000000 kktools-2.1/kktools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-07-09 12:04:28.000000 kktools-2.1/kktools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-07-09 12:04:28.967354 kktools-2.1/setup.cfg
--rw-rw-rw-   0        0        0      562 2022-07-09 07:22:32.000000 kktools-2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 17:28:04.119239 kktools-2.2/
+-rw-rw-rw-   0        0        0     1095 2022-03-13 08:04:57.000000 kktools-2.2/LICENSE
+-rw-rw-rw-   0        0        0     2061 2023-07-30 17:28:04.119239 kktools-2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1739 2023-07-30 17:23:59.000000 kktools-2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 17:28:04.101287 kktools-2.2/kktools/
+-rw-rw-rw-   0        0        0      178 2023-07-30 17:16:56.000000 kktools-2.2/kktools/__init__.py
+-rw-rw-rw-   0        0        0    10626 2023-07-30 17:16:56.000000 kktools-2.2/kktools/core.py
+drwxrwxrwx   0        0        0        0 2023-07-30 17:28:04.118279 kktools-2.2/kktools.egg-info/
+-rw-rw-rw-   0        0        0     2061 2023-07-30 17:28:03.000000 kktools-2.2/kktools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-07-30 17:28:03.000000 kktools-2.2/kktools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 17:28:03.000000 kktools-2.2/kktools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-07-30 17:28:03.000000 kktools-2.2/kktools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-30 17:28:03.000000 kktools-2.2/kktools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 17:28:04.119239 kktools-2.2/setup.cfg
+-rw-rw-rw-   0        0        0      570 2023-07-30 17:09:27.000000 kktools-2.2/setup.py
```

### Comparing `kktools-2.1/LICENSE` & `kktools-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kktools-2.1/PKG-INFO` & `kktools-2.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kktools
-Version: 2.1
+Version: 2.2
 Summary: Tools for finance and treasury specialists
 Home-page: https://github.com/khorevkp/KK_Tools
 Author: Konstantin Khorev
 Author-email: khorevkp@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -22,23 +22,35 @@
 `pip install kktools`
 
 ## Realized Functionality
 `get_ecb_rates("CUR", "YYYY-MM-DD")` - returns pandas dataframe with historical values for a given currency ("CUR") starting from the given date.  
 `get_last_ecb_rates()` - returns pandas dataframe with the latest valid ECB exchange rates for all published currencies.  
 `df_to_excel("file_name.xlsx", dataframe)` - exports pandas dataframe to an excel file with pretty formatting.  
 `dfs_to_excel("file_name.xlsx", list_of_dataframes)` - exports list of pandas dataframes to an excel file with pretty formatting.  
+`Camt` - class for parsing CAMT053 files (EOD bank statements, ISO20022 standard)
 
 ## Basic Usage
 
 Importing history of EUR/GBP exchange rates since 2000-01-01 and exporting it to an excel file with pretty formatting
 
 ```
 import kktools as kkt
 
 df = kkt.get_ecb_rates("GBP", "2000-01-01")
 kkt.df_to_excel("Historical_Rates.xlsx", df)
 ```
 
+Parsing CAMT053 file and getting list of balances and list of all transactions:
+```
+import kktools as kkt
+
+camt = Camt(file_name) # to create an object of Camt class you need to pass path+file_name of the CAMT053 file to be processed
+camt.get_balances() # return pandas dataframe with all the balances (OPBD/CLBD/CLAV/PRCD/FWAV) for each statement in the file
+camt.get_transactions() # return pandas dataframe with all the transactions in the file.
+# For each balance and transaction the related statement will be designated by AccountId column
+
+```
+
 ### License
 MIT licensed. Check the [`LICENSE`](https://github.com/khorevkp/KK_Tools/blob/master/LICENSE) file for full details.
```

### Comparing `kktools-2.1/README.md` & `kktools-2.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -10,21 +10,33 @@
 `pip install kktools`
 
 ## Realized Functionality
 `get_ecb_rates("CUR", "YYYY-MM-DD")` - returns pandas dataframe with historical values for a given currency ("CUR") starting from the given date.  
 `get_last_ecb_rates()` - returns pandas dataframe with the latest valid ECB exchange rates for all published currencies.  
 `df_to_excel("file_name.xlsx", dataframe)` - exports pandas dataframe to an excel file with pretty formatting.  
 `dfs_to_excel("file_name.xlsx", list_of_dataframes)` - exports list of pandas dataframes to an excel file with pretty formatting.  
+`Camt` - class for parsing CAMT053 files (EOD bank statements, ISO20022 standard)
 
 ## Basic Usage
 
 Importing history of EUR/GBP exchange rates since 2000-01-01 and exporting it to an excel file with pretty formatting
 
 ```
 import kktools as kkt
 
 df = kkt.get_ecb_rates("GBP", "2000-01-01")
 kkt.df_to_excel("Historical_Rates.xlsx", df)
 ```
 
+Parsing CAMT053 file and getting list of balances and list of all transactions:
+```
+import kktools as kkt
+
+camt = Camt(file_name) # to create an object of Camt class you need to pass path+file_name of the CAMT053 file to be processed
+camt.get_balances() # return pandas dataframe with all the balances (OPBD/CLBD/CLAV/PRCD/FWAV) for each statement in the file
+camt.get_transactions() # return pandas dataframe with all the transactions in the file.
+# For each balance and transaction the related statement will be designated by AccountId column
+
+```
+
 ### License
 MIT licensed. Check the [`LICENSE`](https://github.com/khorevkp/KK_Tools/blob/master/LICENSE) file for full details.
```

### Comparing `kktools-2.1/kktools.egg-info/PKG-INFO` & `kktools-2.2/kktools.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kktools
-Version: 2.1
+Version: 2.2
 Summary: Tools for finance and treasury specialists
 Home-page: https://github.com/khorevkp/KK_Tools
 Author: Konstantin Khorev
 Author-email: khorevkp@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -22,23 +22,35 @@
 `pip install kktools`
 
 ## Realized Functionality
 `get_ecb_rates("CUR", "YYYY-MM-DD")` - returns pandas dataframe with historical values for a given currency ("CUR") starting from the given date.  
 `get_last_ecb_rates()` - returns pandas dataframe with the latest valid ECB exchange rates for all published currencies.  
 `df_to_excel("file_name.xlsx", dataframe)` - exports pandas dataframe to an excel file with pretty formatting.  
 `dfs_to_excel("file_name.xlsx", list_of_dataframes)` - exports list of pandas dataframes to an excel file with pretty formatting.  
+`Camt` - class for parsing CAMT053 files (EOD bank statements, ISO20022 standard)
 
 ## Basic Usage
 
 Importing history of EUR/GBP exchange rates since 2000-01-01 and exporting it to an excel file with pretty formatting
 
 ```
 import kktools as kkt
 
 df = kkt.get_ecb_rates("GBP", "2000-01-01")
 kkt.df_to_excel("Historical_Rates.xlsx", df)
 ```
 
+Parsing CAMT053 file and getting list of balances and list of all transactions:
+```
+import kktools as kkt
+
+camt = Camt(file_name) # to create an object of Camt class you need to pass path+file_name of the CAMT053 file to be processed
+camt.get_balances() # return pandas dataframe with all the balances (OPBD/CLBD/CLAV/PRCD/FWAV) for each statement in the file
+camt.get_transactions() # return pandas dataframe with all the transactions in the file.
+# For each balance and transaction the related statement will be designated by AccountId column
+
+```
+
 ### License
 MIT licensed. Check the [`LICENSE`](https://github.com/khorevkp/KK_Tools/blob/master/LICENSE) file for full details.
```

### Comparing `kktools-2.1/setup.py` & `kktools-2.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='kktools',
-    version='2.1',
+    version='2.2',
     author='Konstantin Khorev',
     author_email='khorevkp@gmail.com',
     description='Tools for finance and treasury specialists',
     url='https://github.com/khorevkp/KK_Tools',
-    install_requires=['pandas', 'requests'],
+    install_requires=['pandas', 'requests', 'lxml'],
     packages=['kktools'],
     long_description=long_description,
     long_description_content_type='text/markdown'
 )
```

