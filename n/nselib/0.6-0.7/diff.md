# Comparing `tmp/nselib-0.6.tar.gz` & `tmp/nselib-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nselib-0.6.tar", last modified: Sun Jul  2 18:16:47 2023, max compression
+gzip compressed data, was "nselib-0.7.tar", last modified: Sun Jul 30 08:02:20 2023, max compression
```

## Comparing `nselib-0.6.tar` & `nselib-0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 18:16:47.012832 nselib-0.6/
--rw-rw-rw-   0        0        0    11558 2023-06-18 02:00:39.000000 nselib-0.6/LICENSE
--rw-rw-rw-   0        0        0        0 2023-06-18 00:57:58.000000 nselib-0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     4060 2023-07-02 18:16:47.012832 nselib-0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3367 2023-07-02 18:13:29.000000 nselib-0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 18:16:46.784550 nselib-0.6/nselib/
--rw-rw-rw-   0        0        0       68 2023-07-02 18:09:49.000000 nselib-0.6/nselib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 18:16:46.866511 nselib-0.6/nselib/capital_market/
--rw-rw-rw-   0        0        0      356 2023-07-02 12:56:09.000000 nselib-0.6/nselib/capital_market/__init__.py
--rw-rw-rw-   0        0        0    24350 2023-07-02 13:11:04.000000 nselib-0.6/nselib/capital_market/capital_market_data.py
--rw-rw-rw-   0        0        0     2556 2023-06-24 10:49:29.000000 nselib-0.6/nselib/constants.py
-drwxrwxrwx   0        0        0        0 2023-07-02 18:16:46.907686 nselib-0.6/nselib/debt/
--rw-rw-rw-   0        0        0        0 2023-06-18 00:50:56.000000 nselib-0.6/nselib/debt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 18:16:46.974428 nselib-0.6/nselib/derivatives/
--rw-rw-rw-   0        0        0      273 2023-06-24 14:43:31.000000 nselib-0.6/nselib/derivatives/__init__.py
--rw-rw-rw-   0        0        0    16743 2023-07-02 12:58:11.000000 nselib-0.6/nselib/derivatives/derivative_data.py
--rw-rw-rw-   0        0        0     4841 2023-06-24 10:07:44.000000 nselib-0.6/nselib/libutil.py
--rw-rw-rw-   0        0        0      438 2023-06-18 06:43:26.000000 nselib-0.6/nselib/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-02 18:16:46.825862 nselib-0.6/nselib.egg-info/
--rw-rw-rw-   0        0        0     4060 2023-07-02 18:16:46.000000 nselib-0.6/nselib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      443 2023-07-02 18:16:46.000000 nselib-0.6/nselib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 18:16:46.000000 nselib-0.6/nselib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-07-02 18:16:46.000000 nselib-0.6/nselib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-02 18:16:46.000000 nselib-0.6/nselib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-02 18:16:47.013832 nselib-0.6/setup.cfg
--rw-rw-rw-   0        0        0     1011 2023-07-02 18:10:38.000000 nselib-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 08:02:20.025783 nselib-0.7/
+-rw-rw-rw-   0        0        0    11558 2023-07-30 07:38:40.000000 nselib-0.7/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-06-18 00:57:58.000000 nselib-0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     4183 2023-07-30 08:02:20.026784 nselib-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3490 2023-07-30 07:57:49.000000 nselib-0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 08:02:19.789482 nselib-0.7/nselib/
+-rw-rw-rw-   0        0        0       68 2023-07-30 07:57:49.000000 nselib-0.7/nselib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 08:02:19.877902 nselib-0.7/nselib/capital_market/
+-rw-rw-rw-   0        0        0      356 2023-07-30 07:38:40.000000 nselib-0.7/nselib/capital_market/__init__.py
+-rw-rw-rw-   0        0        0    24350 2023-07-30 07:57:49.000000 nselib-0.7/nselib/capital_market/capital_market_data.py
+-rw-rw-rw-   0        0        0     2556 2023-07-30 07:38:40.000000 nselib-0.7/nselib/constants.py
+drwxrwxrwx   0        0        0        0 2023-07-30 08:02:19.917911 nselib-0.7/nselib/debt/
+-rw-rw-rw-   0        0        0        0 2023-06-18 00:50:56.000000 nselib-0.7/nselib/debt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 08:02:19.986481 nselib-0.7/nselib/derivatives/
+-rw-rw-rw-   0        0        0      273 2023-07-30 07:38:40.000000 nselib-0.7/nselib/derivatives/__init__.py
+-rw-rw-rw-   0        0        0    17470 2023-07-30 07:57:49.000000 nselib-0.7/nselib/derivatives/derivative_data.py
+-rw-rw-rw-   0        0        0     4841 2023-07-30 07:38:40.000000 nselib-0.7/nselib/libutil.py
+-rw-rw-rw-   0        0        0      438 2023-07-30 07:38:40.000000 nselib-0.7/nselib/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-30 08:02:19.835585 nselib-0.7/nselib.egg-info/
+-rw-rw-rw-   0        0        0     4183 2023-07-30 08:02:19.000000 nselib-0.7/nselib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      443 2023-07-30 08:02:19.000000 nselib-0.7/nselib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 08:02:19.000000 nselib-0.7/nselib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-30 08:02:19.000000 nselib-0.7/nselib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-30 08:02:19.000000 nselib-0.7/nselib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-30 08:02:20.027782 nselib-0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1011 2023-07-30 07:57:49.000000 nselib-0.7/setup.py
```

### Comparing `nselib-0.6/LICENSE` & `nselib-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nselib-0.6/PKG-INFO` & `nselib-0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nselib
-Version: 0.6
+Version: 0.7
 Summary: library to get NSE India data
 Home-page: https://github.com/RuchiTanmay/nselib
 Author: RuchiTanmay
 Author-email: ruchitanmay@gmail.com
 Keywords: nseindia,nse,python,sdk,trading,stock markets
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # NSElib 0.6
+
 Python Library to get publicly available data on new NSE india website.
 
 Release Notes
 * Compatible and Tested with Python 3.8 and above 
 * Future release will be done on requirement basic
 
 ## Libraries Required
@@ -99,14 +100,16 @@
 
 data = derivatives.future_price_volume_data(symbol='SBIN', instrument='FUTSTK', from_date='01-06-2023', to_date='10-06-2023')
 
 OR
 
 data = derivatives.price_volume_and_deliverable_position_data(symbol='BANKNIFTY', instrument='FUTIDX', period='1M')
 
+Note: instrument type ( future index = FUTIDX, future stocks = FUTSTK, option index = OPTIDX, option stocks = OPTSTK)
+
 More functions will be available in future releases...
 
 ### Debt
 
 More functions will be available in future releases...
```

### Comparing `nselib-0.6/README.md` & `nselib-0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # NSElib 0.6
+
 Python Library to get publicly available data on new NSE india website.
 
 Release Notes
 * Compatible and Tested with Python 3.8 and above 
 * Future release will be done on requirement basic
 
 ## Libraries Required
@@ -81,14 +82,16 @@
 
 data = derivatives.future_price_volume_data(symbol='SBIN', instrument='FUTSTK', from_date='01-06-2023', to_date='10-06-2023')
 
 OR
 
 data = derivatives.price_volume_and_deliverable_position_data(symbol='BANKNIFTY', instrument='FUTIDX', period='1M')
 
+Note: instrument type ( future index = FUTIDX, future stocks = FUTSTK, option index = OPTIDX, option stocks = OPTSTK)
+
 More functions will be available in future releases...
 
 ### Debt
 
 More functions will be available in future releases...
```

### Comparing `nselib-0.6/nselib/capital_market/capital_market_data.py` & `nselib-0.7/nselib/capital_market/capital_market_data.py`

 * *Files identical despite different names*

### Comparing `nselib-0.6/nselib/constants.py` & `nselib-0.7/nselib/constants.py`

 * *Files identical despite different names*

### Comparing `nselib-0.6/nselib/derivatives/derivative_data.py` & `nselib-0.7/nselib/derivatives/derivative_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     data_df.columns = cleaning_column_name(data_df.columns)
     # print(data_df.columns)
     return data_df[future_price_volume_data_column]
 
 
 def fno_bhav_copy(trade_date: str):
     """
-    NSE future option bhav copy
+    NSE future option bhav copy from 2008 on wards
     :param trade_date: eg:'01-06-2023'
     :return: pandas Data frame
     """
     trade_date = datetime.strptime(trade_date, dd_mm_yyyy)
     url = 'https://archives.nseindia.com/content/historical/DERIVATIVES/'
     payload = f"{str(trade_date.strftime('%Y'))}/{str(trade_date.strftime('%b').upper())}/" \
               f"fo{str(trade_date.strftime('%d%b%Y').upper())}bhav.csv.zip"
@@ -135,15 +135,26 @@
     bhav_df = pd.DataFrame()
     if request_bhav.status_code == 200:
         zip_bhav = zipfile.ZipFile(BytesIO(request_bhav.content), 'r')
         for file_name in zip_bhav.filelist:
             if file_name:
                 bhav_df = pd.read_csv(zip_bhav.open(file_name))
     elif request_bhav.status_code == 403:
-        raise FileNotFoundError(f' Data not found, change the date...')
+        url2="https://www.nseindia.com/api/reports?archives=" \
+             "%5B%7B%22name%22%3A%22F%26O%20-%20Bhavcopy(csv)%22%2C%22type%22%3A%22archives%22%2C%22category%22" \
+             f"%3A%22derivatives%22%2C%22section%22%3A%22equity%22%7D%5D&date={str(trade_date.strftime('%d-%b-%Y'))}" \
+             f"&type=equity&mode=single"
+        request_bhav = nse_urlfetch(url2)
+        if request_bhav.status_code == 200:
+            zip_bhav = zipfile.ZipFile(BytesIO(request_bhav.content), 'r')
+            for file_name in zip_bhav.filelist:
+                if file_name:
+                    bhav_df = pd.read_csv(zip_bhav.open(file_name))
+        elif request_bhav.status_code == 403:
+            raise FileNotFoundError(f' Data not found, change the date...')
     bhav_df = bhav_df[['INSTRUMENT', 'SYMBOL', 'EXPIRY_DT', 'STRIKE_PR', 'OPTION_TYP', 'OPEN', 'HIGH', 'LOW',
                        'CLOSE', 'SETTLE_PR', 'CONTRACTS', 'VAL_INLAKH', 'OPEN_INT', 'CHG_IN_OI', 'TIMESTAMP']]
     return bhav_df
 
 
 def participant_wise_open_interest(trade_date: str):
     """
```

### Comparing `nselib-0.6/nselib/libutil.py` & `nselib-0.7/nselib/libutil.py`

 * *Files identical despite different names*

### Comparing `nselib-0.6/nselib.egg-info/PKG-INFO` & `nselib-0.7/nselib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nselib
-Version: 0.6
+Version: 0.7
 Summary: library to get NSE India data
 Home-page: https://github.com/RuchiTanmay/nselib
 Author: RuchiTanmay
 Author-email: ruchitanmay@gmail.com
 Keywords: nseindia,nse,python,sdk,trading,stock markets
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # NSElib 0.6
+
 Python Library to get publicly available data on new NSE india website.
 
 Release Notes
 * Compatible and Tested with Python 3.8 and above 
 * Future release will be done on requirement basic
 
 ## Libraries Required
@@ -99,14 +100,16 @@
 
 data = derivatives.future_price_volume_data(symbol='SBIN', instrument='FUTSTK', from_date='01-06-2023', to_date='10-06-2023')
 
 OR
 
 data = derivatives.price_volume_and_deliverable_position_data(symbol='BANKNIFTY', instrument='FUTIDX', period='1M')
 
+Note: instrument type ( future index = FUTIDX, future stocks = FUTSTK, option index = OPTIDX, option stocks = OPTSTK)
+
 More functions will be available in future releases...
 
 ### Debt
 
 More functions will be available in future releases...
```

### Comparing `nselib-0.6/setup.py` & `nselib-0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='nselib',
     packages=setuptools.find_packages(),
-    version='0.6',
+    version='0.7',
     include_package_data=True,
     description='library to get NSE India data',
     long_description=long_description,
     long_description_content_type="text/markdown", author='RuchiTanmay',
     author_email='ruchitanmay@gmail.com',
     url='https://github.com/RuchiTanmay/nselib',
     install_requires=['requests', 'pandas', 'scipy'],
```

