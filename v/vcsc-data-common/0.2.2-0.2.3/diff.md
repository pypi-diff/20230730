# Comparing `tmp/vcsc_data_common-0.2.2.tar.gz` & `tmp/vcsc_data_common-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcsc_data_common-0.2.2.tar", last modified: Mon Jul 10 09:41:07 2023, max compression
+gzip compressed data, was "vcsc_data_common-0.2.3.tar", last modified: Sun Jul 30 15:33:16 2023, max compression
```

## Comparing `vcsc_data_common-0.2.2.tar` & `vcsc_data_common-0.2.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-10 09:41:07.857734 vcsc_data_common-0.2.2/
--rw-r--r--   0 pd         (501) staff       (20)      300 2023-07-10 09:41:07.857818 vcsc_data_common-0.2.2/PKG-INFO
--rw-r--r--   0 pd         (501) staff       (20)      143 2023-02-22 09:16:04.000000 vcsc_data_common-0.2.2/README.md
--rw-r--r--   0 pd         (501) staff       (20)      799 2023-03-23 03:54:32.000000 vcsc_data_common-0.2.2/pyproject.toml
--rw-r--r--   0 pd         (501) staff       (20)      339 2023-07-10 09:41:07.858140 vcsc_data_common-0.2.2/setup.cfg
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-10 09:41:07.853096 vcsc_data_common-0.2.2/vcsc_data_common/
--rw-r--r--   0 pd         (501) staff       (20)      108 2023-02-22 09:07:01.000000 vcsc_data_common-0.2.2/vcsc_data_common/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-10 09:41:07.854748 vcsc_data_common-0.2.2/vcsc_data_common/ai_framework/
--rw-r--r--   0 pd         (501) staff       (20)       48 2023-02-22 09:02:01.000000 vcsc_data_common-0.2.2/vcsc_data_common/ai_framework/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     5081 2023-06-08 06:24:22.000000 vcsc_data_common-0.2.2/vcsc_data_common/ai_framework/interval_fetching.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-10 09:41:07.855240 vcsc_data_common-0.2.2/vcsc_data_common/backtest/
--rw-r--r--   0 pd         (501) staff       (20)     2537 2023-05-12 03:24:29.000000 vcsc_data_common-0.2.2/vcsc_data_common/backtest/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-10 09:41:07.855552 vcsc_data_common-0.2.2/vcsc_data_common/fiin_data/
--rw-r--r--   0 pd         (501) staff       (20)     2225 2023-07-05 03:00:30.000000 vcsc_data_common-0.2.2/vcsc_data_common/fiin_data/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-10 09:41:07.855866 vcsc_data_common-0.2.2/vcsc_data_common/live_price_data/
--rw-r--r--   0 pd         (501) staff       (20)     2341 2023-05-04 06:36:10.000000 vcsc_data_common-0.2.2/vcsc_data_common/live_price_data/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-10 09:41:07.856152 vcsc_data_common-0.2.2/vcsc_data_common/offline_price_data/
--rw-r--r--   0 pd         (501) staff       (20)      880 2023-03-14 02:58:59.000000 vcsc_data_common-0.2.2/vcsc_data_common/offline_price_data/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-10 09:41:07.856438 vcsc_data_common-0.2.2/vcsc_data_common/oneday_portfolio/
--rw-r--r--   0 pd         (501) staff       (20)      516 2023-05-24 09:25:19.000000 vcsc_data_common-0.2.2/vcsc_data_common/oneday_portfolio/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-10 09:41:07.856709 vcsc_data_common-0.2.2/vcsc_data_common/order/
--rw-r--r--   0 pd         (501) staff       (20)     3875 2023-06-08 02:36:37.000000 vcsc_data_common-0.2.2/vcsc_data_common/order/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-10 09:41:07.856984 vcsc_data_common-0.2.2/vcsc_data_common/portfolio_info/
--rw-r--r--   0 pd         (501) staff       (20)     3868 2023-06-13 08:25:14.000000 vcsc_data_common-0.2.2/vcsc_data_common/portfolio_info/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-10 09:41:07.857258 vcsc_data_common-0.2.2/vcsc_data_common/proprietary_trading/
--rw-r--r--   0 pd         (501) staff       (20)      740 2023-07-10 09:38:54.000000 vcsc_data_common-0.2.2/vcsc_data_common/proprietary_trading/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-10 09:41:07.857511 vcsc_data_common-0.2.2/vcsc_data_common/signals/
--rw-r--r--   0 pd         (501) staff       (20)     1513 2023-06-01 10:35:44.000000 vcsc_data_common-0.2.2/vcsc_data_common/signals/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-10 09:41:07.853969 vcsc_data_common-0.2.2/vcsc_data_common.egg-info/
--rw-r--r--   0 pd         (501) staff       (20)      300 2023-07-10 09:41:07.000000 vcsc_data_common-0.2.2/vcsc_data_common.egg-info/PKG-INFO
--rw-r--r--   0 pd         (501) staff       (20)      736 2023-07-10 09:41:07.000000 vcsc_data_common-0.2.2/vcsc_data_common.egg-info/SOURCES.txt
--rw-r--r--   0 pd         (501) staff       (20)        1 2023-07-10 09:41:07.000000 vcsc_data_common-0.2.2/vcsc_data_common.egg-info/dependency_links.txt
--rw-r--r--   0 pd         (501) staff       (20)      140 2023-07-10 09:41:07.000000 vcsc_data_common-0.2.2/vcsc_data_common.egg-info/requires.txt
--rw-r--r--   0 pd         (501) staff       (20)       17 2023-07-10 09:41:07.000000 vcsc_data_common-0.2.2/vcsc_data_common.egg-info/top_level.txt
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-30 15:33:16.120073 vcsc_data_common-0.2.3/
+-rw-r--r--   0 pd         (501) staff       (20)      300 2023-07-30 15:33:16.120181 vcsc_data_common-0.2.3/PKG-INFO
+-rw-r--r--   0 pd         (501) staff       (20)      143 2023-02-22 09:16:04.000000 vcsc_data_common-0.2.3/README.md
+-rw-r--r--   0 pd         (501) staff       (20)      799 2023-03-23 03:54:32.000000 vcsc_data_common-0.2.3/pyproject.toml
+-rw-r--r--   0 pd         (501) staff       (20)      339 2023-07-30 15:33:16.120691 vcsc_data_common-0.2.3/setup.cfg
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-30 15:33:16.113367 vcsc_data_common-0.2.3/vcsc_data_common/
+-rw-r--r--   0 pd         (501) staff       (20)      108 2023-02-22 09:07:01.000000 vcsc_data_common-0.2.3/vcsc_data_common/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-30 15:33:16.115213 vcsc_data_common-0.2.3/vcsc_data_common/ai_framework/
+-rw-r--r--   0 pd         (501) staff       (20)       48 2023-02-22 09:02:01.000000 vcsc_data_common-0.2.3/vcsc_data_common/ai_framework/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     5081 2023-06-08 06:24:22.000000 vcsc_data_common-0.2.3/vcsc_data_common/ai_framework/interval_fetching.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-30 15:33:16.115901 vcsc_data_common-0.2.3/vcsc_data_common/backtest/
+-rw-r--r--   0 pd         (501) staff       (20)     2537 2023-05-12 03:24:29.000000 vcsc_data_common-0.2.3/vcsc_data_common/backtest/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-30 15:33:16.116228 vcsc_data_common-0.2.3/vcsc_data_common/fiin_data/
+-rw-r--r--   0 pd         (501) staff       (20)     2228 2023-07-30 15:31:52.000000 vcsc_data_common-0.2.3/vcsc_data_common/fiin_data/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-30 15:33:16.116493 vcsc_data_common-0.2.3/vcsc_data_common/live_price_data/
+-rw-r--r--   0 pd         (501) staff       (20)     2347 2023-07-30 15:32:22.000000 vcsc_data_common-0.2.3/vcsc_data_common/live_price_data/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-30 15:33:16.116769 vcsc_data_common-0.2.3/vcsc_data_common/offline_price_data/
+-rw-r--r--   0 pd         (501) staff       (20)      886 2023-07-30 15:32:20.000000 vcsc_data_common-0.2.3/vcsc_data_common/offline_price_data/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-30 15:33:16.117149 vcsc_data_common-0.2.3/vcsc_data_common/oneday_portfolio/
+-rw-r--r--   0 pd         (501) staff       (20)      516 2023-05-24 09:25:19.000000 vcsc_data_common-0.2.3/vcsc_data_common/oneday_portfolio/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-30 15:33:16.117575 vcsc_data_common-0.2.3/vcsc_data_common/order/
+-rw-r--r--   0 pd         (501) staff       (20)     3875 2023-06-08 02:36:37.000000 vcsc_data_common-0.2.3/vcsc_data_common/order/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-30 15:33:16.118261 vcsc_data_common-0.2.3/vcsc_data_common/portfolio_info/
+-rw-r--r--   0 pd         (501) staff       (20)     3868 2023-06-13 08:25:14.000000 vcsc_data_common-0.2.3/vcsc_data_common/portfolio_info/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-30 15:33:16.118755 vcsc_data_common-0.2.3/vcsc_data_common/proprietary_trading/
+-rw-r--r--   0 pd         (501) staff       (20)      740 2023-07-10 09:38:54.000000 vcsc_data_common-0.2.3/vcsc_data_common/proprietary_trading/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-30 15:33:16.119086 vcsc_data_common-0.2.3/vcsc_data_common/signals/
+-rw-r--r--   0 pd         (501) staff       (20)     1513 2023-06-01 10:35:44.000000 vcsc_data_common-0.2.3/vcsc_data_common/signals/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-30 15:33:16.114433 vcsc_data_common-0.2.3/vcsc_data_common.egg-info/
+-rw-r--r--   0 pd         (501) staff       (20)      300 2023-07-30 15:33:16.000000 vcsc_data_common-0.2.3/vcsc_data_common.egg-info/PKG-INFO
+-rw-r--r--   0 pd         (501) staff       (20)      736 2023-07-30 15:33:16.000000 vcsc_data_common-0.2.3/vcsc_data_common.egg-info/SOURCES.txt
+-rw-r--r--   0 pd         (501) staff       (20)        1 2023-07-30 15:33:16.000000 vcsc_data_common-0.2.3/vcsc_data_common.egg-info/dependency_links.txt
+-rw-r--r--   0 pd         (501) staff       (20)      140 2023-07-30 15:33:16.000000 vcsc_data_common-0.2.3/vcsc_data_common.egg-info/requires.txt
+-rw-r--r--   0 pd         (501) staff       (20)       17 2023-07-30 15:33:16.000000 vcsc_data_common-0.2.3/vcsc_data_common.egg-info/top_level.txt
```

### Comparing `vcsc_data_common-0.2.2/pyproject.toml` & `vcsc_data_common-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.2.2/vcsc_data_common/ai_framework/interval_fetching.py` & `vcsc_data_common-0.2.3/vcsc_data_common/ai_framework/interval_fetching.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.2.2/vcsc_data_common/backtest/__init__.py` & `vcsc_data_common-0.2.3/vcsc_data_common/backtest/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.2.2/vcsc_data_common/fiin_data/__init__.py` & `vcsc_data_common-0.2.3/vcsc_data_common/fiin_data/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pyarrow as pa
 import datetime
 
 class FiinDataFetcher():
     def __init__(self, aws_access_key: str, aws_secret_key: str) -> None:
         self.aws_access_key = aws_access_key
         self.aws_secret_key = aws_secret_key
-        self.table_parent_path = 's3://vcsc-ai/prod/fiin'
+        self.table_parent_path = 's3://vietcap-ai/prod/fiin'
 
     def __fetch_data(self,table_name:str, filter_condition):
 
         uri = f"{self.table_parent_path}/{table_name}"
 
         dt = DeltaTable(uri, storage_options={
             "AWS_ACCESS_KEY_ID": self.aws_access_key,
```

### Comparing `vcsc_data_common-0.2.2/vcsc_data_common/live_price_data/__init__.py` & `vcsc_data_common-0.2.3/vcsc_data_common/live_price_data/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     def __init__(self, aws_access_key: str, aws_secret_key: str, time_frame: str, is_fill_gap: bool) -> None:
         self.aws_access_key = aws_access_key
         self.aws_secret_key = aws_secret_key
         self.time_frame = time_frame
         self.is_fill_gap = is_fill_gap
 
-        self.uri = f"s3://vcsc-ai/prod/price_data/{self.time_frame}_none_gap_intraday" if is_fill_gap else f"s3://vcsc-ai/prod/price_data/{self.time_frame}_intraday"
+        self.uri = f"s3://vietcap-ai/prod/price_data/{self.time_frame}_none_gap_intraday" if is_fill_gap else f"s3://vietcap-ai/prod/price_data/{self.time_frame}_intraday"
 
     def get_data(self) -> pd.DataFrame:
         dt = DeltaTable(self.uri, storage_options={
             "AWS_ACCESS_KEY_ID": self.aws_access_key,
             "AWS_SECRET_ACCESS_KEY": self.aws_secret_key,
             'AWS_REGION': "ap-southeast-1"
         })
```

### Comparing `vcsc_data_common-0.2.2/vcsc_data_common/offline_price_data/__init__.py` & `vcsc_data_common-0.2.3/vcsc_data_common/offline_price_data/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
     def __init__(self, aws_access_key: str, aws_secret_key: str, time_frame: str, is_fill_gap: bool) -> None:
         self.aws_access_key = aws_access_key
         self.aws_secret_key = aws_secret_key
         self.time_frame = time_frame
         self.is_fill_gap = is_fill_gap
 
-        self.uri = f"s3://vcsc-ai/prod/price_data/{self.time_frame}_none_gap" if is_fill_gap else f"s3://vcsc-ai/prod/price_data/{self.time_frame}"
+        self.uri = f"s3://vietcap-ai/prod/price_data/{self.time_frame}_none_gap" if is_fill_gap else f"s3://vietcap-ai/prod/price_data/{self.time_frame}"
 
     def get_data(self) -> pd.DataFrame:
 
         dt = DeltaTable(self.uri, storage_options={
             "AWS_ACCESS_KEY_ID": self.aws_access_key,
             "AWS_SECRET_ACCESS_KEY": self.aws_secret_key,
             'AWS_REGION': "ap-southeast-1"
```

### Comparing `vcsc_data_common-0.2.2/vcsc_data_common/oneday_portfolio/__init__.py` & `vcsc_data_common-0.2.3/vcsc_data_common/oneday_portfolio/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.2.2/vcsc_data_common/order/__init__.py` & `vcsc_data_common-0.2.3/vcsc_data_common/order/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.2.2/vcsc_data_common/portfolio_info/__init__.py` & `vcsc_data_common-0.2.3/vcsc_data_common/portfolio_info/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.2.2/vcsc_data_common/proprietary_trading/__init__.py` & `vcsc_data_common-0.2.3/vcsc_data_common/proprietary_trading/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.2.2/vcsc_data_common/signals/__init__.py` & `vcsc_data_common-0.2.3/vcsc_data_common/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.2.2/vcsc_data_common.egg-info/SOURCES.txt` & `vcsc_data_common-0.2.3/vcsc_data_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

