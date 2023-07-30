# Comparing `tmp/cryptounifier-1.0.3.tar.gz` & `tmp/cryptounifier-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptounifier-1.0.3.tar", last modified: Sun Mar 12 04:12:58 2023, max compression
+gzip compressed data, was "cryptounifier-1.0.4.tar", last modified: Sun Jul 30 02:50:40 2023, max compression
```

## Comparing `cryptounifier-1.0.3.tar` & `cryptounifier-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 miguel    (1000) miguel    (1000)        0 2023-03-12 04:12:58.146631 cryptounifier-1.0.3/
--rw-r--r--   0 miguel    (1000) miguel    (1000)     1067 2023-03-12 04:00:03.000000 cryptounifier-1.0.3/LICENSE.md
--rw-r--r--   0 miguel    (1000) miguel    (1000)     1716 2023-03-12 04:12:58.146631 cryptounifier-1.0.3/PKG-INFO
--rw-r--r--   0 miguel    (1000) miguel    (1000)      989 2023-03-12 04:09:42.000000 cryptounifier-1.0.3/README.md
--rw-r--r--   0 miguel    (1000) miguel    (1000)       38 2023-03-12 04:12:58.146631 cryptounifier-1.0.3/setup.cfg
--rw-r--r--   0 miguel    (1000) miguel    (1000)     1058 2023-03-12 04:10:40.000000 cryptounifier-1.0.3/setup.py
-drwxr-xr-x   0 miguel    (1000) miguel    (1000)        0 2023-03-12 04:12:58.144631 cryptounifier-1.0.3/src/
-drwxr-xr-x   0 miguel    (1000) miguel    (1000)        0 2023-03-12 04:12:58.145631 cryptounifier-1.0.3/src/cryptounifier/
--rw-r--r--   0 miguel    (1000) miguel    (1000)      969 2023-03-12 04:09:13.000000 cryptounifier-1.0.3/src/cryptounifier/BaseApi.py
--rw-r--r--   0 miguel    (1000) miguel    (1000)     2178 2023-03-12 04:09:25.000000 cryptounifier-1.0.3/src/cryptounifier/MerchantApi.py
--rw-r--r--   0 miguel    (1000) miguel    (1000)     1493 2023-03-12 04:00:03.000000 cryptounifier-1.0.3/src/cryptounifier/WalletApi.py
--rw-r--r--   0 miguel    (1000) miguel    (1000)     1133 2023-03-12 04:00:03.000000 cryptounifier-1.0.3/src/cryptounifier/WalletTokenApi.py
--rw-r--r--   0 miguel    (1000) miguel    (1000)        0 2023-03-12 04:00:03.000000 cryptounifier-1.0.3/src/cryptounifier/__init__.py
-drwxr-xr-x   0 miguel    (1000) miguel    (1000)        0 2023-03-12 04:12:58.146631 cryptounifier-1.0.3/src/cryptounifier.egg-info/
--rw-r--r--   0 miguel    (1000) miguel    (1000)     1716 2023-03-12 04:12:58.000000 cryptounifier-1.0.3/src/cryptounifier.egg-info/PKG-INFO
--rw-r--r--   0 miguel    (1000) miguel    (1000)      392 2023-03-12 04:12:58.000000 cryptounifier-1.0.3/src/cryptounifier.egg-info/SOURCES.txt
--rw-r--r--   0 miguel    (1000) miguel    (1000)        1 2023-03-12 04:12:58.000000 cryptounifier-1.0.3/src/cryptounifier.egg-info/dependency_links.txt
--rw-r--r--   0 miguel    (1000) miguel    (1000)        9 2023-03-12 04:12:58.000000 cryptounifier-1.0.3/src/cryptounifier.egg-info/requires.txt
--rw-r--r--   0 miguel    (1000) miguel    (1000)       14 2023-03-12 04:12:58.000000 cryptounifier-1.0.3/src/cryptounifier.egg-info/top_level.txt
+drwxr-xr-x   0 miguel    (1000) miguel    (1000)        0 2023-07-30 02:50:40.921686 cryptounifier-1.0.4/
+-rw-r--r--   0 miguel    (1000) miguel    (1000)     1067 2023-07-30 02:46:02.000000 cryptounifier-1.0.4/LICENSE.md
+-rw-r--r--   0 miguel    (1000) miguel    (1000)     1716 2023-07-30 02:50:40.921686 cryptounifier-1.0.4/PKG-INFO
+-rw-r--r--   0 miguel    (1000) miguel    (1000)      989 2023-07-30 02:46:02.000000 cryptounifier-1.0.4/README.md
+-rw-r--r--   0 miguel    (1000) miguel    (1000)       38 2023-07-30 02:50:40.921686 cryptounifier-1.0.4/setup.cfg
+-rw-r--r--   0 miguel    (1000) miguel    (1000)     1058 2023-07-30 02:47:40.000000 cryptounifier-1.0.4/setup.py
+drwxr-xr-x   0 miguel    (1000) miguel    (1000)        0 2023-07-30 02:50:40.920685 cryptounifier-1.0.4/src/
+drwxr-xr-x   0 miguel    (1000) miguel    (1000)        0 2023-07-30 02:50:40.921686 cryptounifier-1.0.4/src/cryptounifier/
+-rw-r--r--   0 miguel    (1000) miguel    (1000)      969 2023-07-30 02:46:02.000000 cryptounifier-1.0.4/src/cryptounifier/BaseApi.py
+-rw-r--r--   0 miguel    (1000) miguel    (1000)     2178 2023-07-30 02:46:02.000000 cryptounifier-1.0.4/src/cryptounifier/MerchantApi.py
+-rw-r--r--   0 miguel    (1000) miguel    (1000)     1576 2023-07-30 02:46:31.000000 cryptounifier-1.0.4/src/cryptounifier/WalletApi.py
+-rw-r--r--   0 miguel    (1000) miguel    (1000)     1133 2023-07-30 02:46:02.000000 cryptounifier-1.0.4/src/cryptounifier/WalletTokenApi.py
+-rw-r--r--   0 miguel    (1000) miguel    (1000)        0 2023-07-30 02:46:02.000000 cryptounifier-1.0.4/src/cryptounifier/__init__.py
+drwxr-xr-x   0 miguel    (1000) miguel    (1000)        0 2023-07-30 02:50:40.921686 cryptounifier-1.0.4/src/cryptounifier.egg-info/
+-rw-r--r--   0 miguel    (1000) miguel    (1000)     1716 2023-07-30 02:50:40.000000 cryptounifier-1.0.4/src/cryptounifier.egg-info/PKG-INFO
+-rw-r--r--   0 miguel    (1000) miguel    (1000)      392 2023-07-30 02:50:40.000000 cryptounifier-1.0.4/src/cryptounifier.egg-info/SOURCES.txt
+-rw-r--r--   0 miguel    (1000) miguel    (1000)        1 2023-07-30 02:50:40.000000 cryptounifier-1.0.4/src/cryptounifier.egg-info/dependency_links.txt
+-rw-r--r--   0 miguel    (1000) miguel    (1000)        9 2023-07-30 02:50:40.000000 cryptounifier-1.0.4/src/cryptounifier.egg-info/requires.txt
+-rw-r--r--   0 miguel    (1000) miguel    (1000)       14 2023-07-30 02:50:40.000000 cryptounifier-1.0.4/src/cryptounifier.egg-info/top_level.txt
```

### Comparing `cryptounifier-1.0.3/LICENSE.md` & `cryptounifier-1.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cryptounifier-1.0.3/PKG-INFO` & `cryptounifier-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptounifier
-Version: 1.0.3
+Version: 1.0.4
 Summary: CryptoUnifier API Python Integration.
 Home-page: https://github.com/cryptounifier/python-sdk
 Author: https://cryptounifier.io/
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/cryptounifier/python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cryptounifier-1.0.3/README.md` & `cryptounifier-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cryptounifier-1.0.3/setup.py` & `cryptounifier-1.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='cryptounifier',
-    version='1.0.3',
+    version='1.0.4',
     description='CryptoUnifier API Python Integration.',
     author='https://cryptounifier.io/',
     license='MIT License',
     install_requires=['requests'],
 
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `cryptounifier-1.0.3/src/cryptounifier/BaseApi.py` & `cryptounifier-1.0.4/src/cryptounifier/BaseApi.py`

 * *Files identical despite different names*

### Comparing `cryptounifier-1.0.3/src/cryptounifier/MerchantApi.py` & `cryptounifier-1.0.4/src/cryptounifier/MerchantApi.py`

 * *Files identical despite different names*

### Comparing `cryptounifier-1.0.3/src/cryptounifier/WalletApi.py` & `cryptounifier-1.0.4/src/cryptounifier/WalletApi.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,17 +18,18 @@
 
     def getTransactionInfo(self, txid):
         return self.executeRequest('GET', 'transaction-info', {'txid': txid})
 
     def getDepositAddresses(self):
         return self.executeRequest('GET', 'deposit-addresses')
 
-    def validateAddresses(self, addresses):
+    def validateAddresses(self, addresses, validateActivation = None):
         return self.executeRequest('POST', 'validate-addresses',{
-            'addresses' : json.dumps(addresses)
+            'addresses' : json.dumps(addresses),
+            'validate_activation' : validateActivation
         })
     
     def estimateFee(self, destinations, feePerByte = None, extraField = None):
         return self.executeRequest('POST', 'estimate-fee',{
             'destination' : json.dumps(destinations),
             'fee_per_byte' : feePerByte,
             'extra_field' : extraField
```

### Comparing `cryptounifier-1.0.3/src/cryptounifier/WalletTokenApi.py` & `cryptounifier-1.0.4/src/cryptounifier/WalletTokenApi.py`

 * *Files identical despite different names*

### Comparing `cryptounifier-1.0.3/src/cryptounifier.egg-info/PKG-INFO` & `cryptounifier-1.0.4/src/cryptounifier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptounifier
-Version: 1.0.3
+Version: 1.0.4
 Summary: CryptoUnifier API Python Integration.
 Home-page: https://github.com/cryptounifier/python-sdk
 Author: https://cryptounifier.io/
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/cryptounifier/python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

