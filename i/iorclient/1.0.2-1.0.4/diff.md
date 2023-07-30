# Comparing `tmp/iorclient-1.0.2.tar.gz` & `tmp/iorclient-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iorclient-1.0.2.tar", last modified: Thu Jul 20 17:21:06 2023, max compression
+gzip compressed data, was "iorclient-1.0.4.tar", last modified: Sun Jul 30 09:23:26 2023, max compression
```

## Comparing `iorclient-1.0.2.tar` & `iorclient-1.0.4.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 17:21:06.538165 iorclient-1.0.2/
--rw-rw-rw-   0        0        0     1091 2023-07-08 13:48:47.000000 iorclient-1.0.2/LICENSE
--rw-rw-rw-   0        0        0       45 2023-07-11 07:20:58.000000 iorclient-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      994 2023-07-20 17:21:06.537168 iorclient-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-20 17:21:06.511251 iorclient-1.0.2/ior/
--rw-rw-rw-   0        0        0        0 2023-07-08 13:44:53.000000 iorclient-1.0.2/ior/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-20 17:21:06.521221 iorclient-1.0.2/ior/client/
--rw-rw-rw-   0        0        0        0 2023-03-26 12:54:42.000000 iorclient-1.0.2/ior/client/__init__.py
--rw-rw-rw-   0        0        0    12857 2023-07-19 16:53:06.000000 iorclient-1.0.2/ior/client/certificate_service.py
--rw-rw-rw-   0        0        0     5302 2023-07-20 08:17:33.000000 iorclient-1.0.2/ior/client/contract_template_service.py
--rw-rw-rw-   0        0        0     2539 2023-07-19 05:14:32.000000 iorclient-1.0.2/ior/client/exchange_service.py
--rw-rw-rw-   0        0        0     5052 2023-07-20 17:16:49.000000 iorclient-1.0.2/ior/client/permission_control_service.py
--rw-rw-rw-   0        0        0     5816 2023-07-19 05:30:38.000000 iorclient-1.0.2/ior/client/role_control_service.py
--rw-rw-rw-   0        0        0     5430 2023-07-19 05:15:05.000000 iorclient-1.0.2/ior/client/template_control_service.py
--rw-rw-rw-   0        0        0     2328 2023-07-20 15:58:18.000000 iorclient-1.0.2/ior/iorsdk.py
-drwxrwxrwx   0        0        0        0 2023-07-20 17:21:06.525209 iorclient-1.0.2/ior/util/
--rw-rw-rw-   0        0        0        0 2023-03-26 12:54:52.000000 iorclient-1.0.2/ior/util/__init__.py
--rw-rw-rw-   0        0        0     1490 2023-07-19 15:12:23.000000 iorclient-1.0.2/ior/util/result_utils.py
--rw-rw-rw-   0        0        0     4047 2023-07-17 18:09:55.000000 iorclient-1.0.2/ior/util/web3_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-20 17:21:06.530188 iorclient-1.0.2/iorclient.egg-info/
--rw-rw-rw-   0        0        0      994 2023-07-20 17:21:06.000000 iorclient-1.0.2/iorclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      577 2023-07-20 17:21:06.000000 iorclient-1.0.2/iorclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 17:21:06.000000 iorclient-1.0.2/iorclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-20 17:21:06.000000 iorclient-1.0.2/iorclient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-20 17:21:06.538165 iorclient-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      621 2023-07-20 17:18:58.000000 iorclient-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-20 17:21:06.535171 iorclient-1.0.2/test/
--rw-rw-rw-   0        0        0        0 2023-07-17 16:15:26.000000 iorclient-1.0.2/test/__init__.py
--rw-rw-rw-   0        0        0     2054 2023-07-20 09:55:38.000000 iorclient-1.0.2/test/test_cert.py
--rw-rw-rw-   0        0        0     3820 2023-07-20 09:55:42.000000 iorclient-1.0.2/test/test_role.py
--rw-rw-rw-   0        0        0     2843 2023-07-20 09:55:45.000000 iorclient-1.0.2/test/test_template.py
+drwxrwxrwx   0        0        0        0 2023-07-30 09:23:26.363894 iorclient-1.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-07-08 13:48:47.000000 iorclient-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0       45 2023-07-11 07:20:58.000000 iorclient-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      994 2023-07-30 09:23:26.362893 iorclient-1.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-30 09:23:26.335577 iorclient-1.0.4/ior/
+-rw-rw-rw-   0        0        0        0 2023-07-08 13:44:53.000000 iorclient-1.0.4/ior/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 09:23:26.346435 iorclient-1.0.4/ior/client/
+-rw-rw-rw-   0        0        0        0 2023-03-26 12:54:42.000000 iorclient-1.0.4/ior/client/__init__.py
+-rw-rw-rw-   0        0        0    12857 2023-07-19 16:53:06.000000 iorclient-1.0.4/ior/client/certificate_service.py
+-rw-rw-rw-   0        0        0     5302 2023-07-20 08:17:33.000000 iorclient-1.0.4/ior/client/contract_template_service.py
+-rw-rw-rw-   0        0        0     2539 2023-07-19 05:14:32.000000 iorclient-1.0.4/ior/client/exchange_service.py
+-rw-rw-rw-   0        0        0     5052 2023-07-20 17:16:49.000000 iorclient-1.0.4/ior/client/permission_control_service.py
+-rw-rw-rw-   0        0        0     5816 2023-07-19 05:30:38.000000 iorclient-1.0.4/ior/client/role_control_service.py
+-rw-rw-rw-   0        0        0     5430 2023-07-19 05:15:05.000000 iorclient-1.0.4/ior/client/template_control_service.py
+-rw-rw-rw-   0        0        0     6550 2023-07-30 08:59:32.000000 iorclient-1.0.4/ior/client/vote_delegation_template_service.py
+-rw-rw-rw-   0        0        0     5884 2023-07-30 09:03:10.000000 iorclient-1.0.4/ior/client/vote_template_service.py
+-rw-rw-rw-   0        0        0     2328 2023-07-20 15:58:18.000000 iorclient-1.0.4/ior/iorsdk.py
+drwxrwxrwx   0        0        0        0 2023-07-30 09:23:26.349936 iorclient-1.0.4/ior/util/
+-rw-rw-rw-   0        0        0        0 2023-03-26 12:54:52.000000 iorclient-1.0.4/ior/util/__init__.py
+-rw-rw-rw-   0        0        0     1490 2023-07-19 15:12:23.000000 iorclient-1.0.4/ior/util/result_utils.py
+-rw-rw-rw-   0        0        0     4047 2023-07-17 18:09:55.000000 iorclient-1.0.4/ior/util/web3_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-30 09:23:26.356917 iorclient-1.0.4/iorclient.egg-info/
+-rw-rw-rw-   0        0        0      994 2023-07-30 09:23:26.000000 iorclient-1.0.4/iorclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      660 2023-07-30 09:23:26.000000 iorclient-1.0.4/iorclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 09:23:26.000000 iorclient-1.0.4/iorclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-30 09:23:26.000000 iorclient-1.0.4/iorclient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 09:23:26.363894 iorclient-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      621 2023-07-30 09:21:55.000000 iorclient-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 09:23:26.361900 iorclient-1.0.4/test/
+-rw-rw-rw-   0        0        0        0 2023-07-17 16:15:26.000000 iorclient-1.0.4/test/__init__.py
+-rw-rw-rw-   0        0        0     2054 2023-07-20 09:55:38.000000 iorclient-1.0.4/test/test_cert.py
+-rw-rw-rw-   0        0        0     3820 2023-07-20 09:55:42.000000 iorclient-1.0.4/test/test_role.py
+-rw-rw-rw-   0        0        0     2843 2023-07-20 09:55:45.000000 iorclient-1.0.4/test/test_template.py
```

### Comparing `iorclient-1.0.2/LICENSE` & `iorclient-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `iorclient-1.0.2/PKG-INFO` & `iorclient-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iorclient
-Version: 1.0.2
+Version: 1.0.4
 Summary: ior client sdk for ior standard
 Home-page: https://github.com/tzspace-ior/iorclient
 Author: Jie Guan
 Author-email: jguanisme@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `iorclient-1.0.2/ior/client/certificate_service.py` & `iorclient-1.0.4/ior/client/certificate_service.py`

 * *Files identical despite different names*

### Comparing `iorclient-1.0.2/ior/client/contract_template_service.py` & `iorclient-1.0.4/ior/client/contract_template_service.py`

 * *Files identical despite different names*

### Comparing `iorclient-1.0.2/ior/client/exchange_service.py` & `iorclient-1.0.4/ior/client/exchange_service.py`

 * *Files identical despite different names*

### Comparing `iorclient-1.0.2/ior/client/permission_control_service.py` & `iorclient-1.0.4/ior/client/permission_control_service.py`

 * *Files identical despite different names*

### Comparing `iorclient-1.0.2/ior/client/role_control_service.py` & `iorclient-1.0.4/ior/client/role_control_service.py`

 * *Files identical despite different names*

### Comparing `iorclient-1.0.2/ior/client/template_control_service.py` & `iorclient-1.0.4/ior/client/template_control_service.py`

 * *Files identical despite different names*

### Comparing `iorclient-1.0.2/ior/iorsdk.py` & `iorclient-1.0.4/ior/iorsdk.py`

 * *Files identical despite different names*

### Comparing `iorclient-1.0.2/ior/util/result_utils.py` & `iorclient-1.0.4/ior/util/result_utils.py`

 * *Files identical despite different names*

### Comparing `iorclient-1.0.2/ior/util/web3_utils.py` & `iorclient-1.0.4/ior/util/web3_utils.py`

 * *Files identical despite different names*

### Comparing `iorclient-1.0.2/iorclient.egg-info/PKG-INFO` & `iorclient-1.0.4/iorclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iorclient
-Version: 1.0.2
+Version: 1.0.4
 Summary: ior client sdk for ior standard
 Home-page: https://github.com/tzspace-ior/iorclient
 Author: Jie Guan
 Author-email: jguanisme@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `iorclient-1.0.2/iorclient.egg-info/SOURCES.txt` & `iorclient-1.0.4/iorclient.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 ior/client/__init__.py
 ior/client/certificate_service.py
 ior/client/contract_template_service.py
 ior/client/exchange_service.py
 ior/client/permission_control_service.py
 ior/client/role_control_service.py
 ior/client/template_control_service.py
+ior/client/vote_delegation_template_service.py
+ior/client/vote_template_service.py
 ior/util/__init__.py
 ior/util/result_utils.py
 ior/util/web3_utils.py
 iorclient.egg-info/PKG-INFO
 iorclient.egg-info/SOURCES.txt
 iorclient.egg-info/dependency_links.txt
 iorclient.egg-info/top_level.txt
```

### Comparing `iorclient-1.0.2/setup.py` & `iorclient-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.MD", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="iorclient",
-  version="1.0.2",
+  version="1.0.4",
   author="Jie Guan",
   author_email="jguanisme@163.com",
   description="ior client sdk for ior standard",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/tzspace-ior/iorclient",
   packages=setuptools.find_packages(),
```

### Comparing `iorclient-1.0.2/test/test_cert.py` & `iorclient-1.0.4/test/test_cert.py`

 * *Files identical despite different names*

### Comparing `iorclient-1.0.2/test/test_role.py` & `iorclient-1.0.4/test/test_role.py`

 * *Files identical despite different names*

### Comparing `iorclient-1.0.2/test/test_template.py` & `iorclient-1.0.4/test/test_template.py`

 * *Files identical despite different names*

