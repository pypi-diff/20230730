# Comparing `tmp/commutauto-0.3.0.tar.gz` & `tmp/commutauto-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commutauto-0.3.0.tar", last modified: Mon May 29 00:54:23 2023, max compression
+gzip compressed data, was "commutauto-0.3.1.tar", last modified: Sat Jul 29 23:34:19 2023, max compression
```

## Comparing `commutauto-0.3.0.tar` & `commutauto-0.3.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:23.971437 commutauto-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-29 00:54:23.971437 commutauto-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-05-29 00:54:07.000000 commutauto-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:23.971437 commutauto-0.3.0/commutauto/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:23.971437 commutauto-0.3.0/commutauto/booking_service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/booking_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/booking_service/date_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/booking_service/flex.py
--rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/booking_service/payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/booking_service/retriers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15016 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/booking_service/station.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:23.971437 commutauto-0.3.0/commutauto/client/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/client/auth_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:23.971437 commutauto-0.3.0/commutauto/model/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/model/flex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/model/flex_booking.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/model/reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/model/station.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:23.971437 commutauto-0.3.0/commutauto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-29 00:54:23.000000 commutauto-0.3.0/commutauto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-29 00:54:23.000000 commutauto-0.3.0/commutauto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 00:54:23.000000 commutauto-0.3.0/commutauto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-29 00:54:23.000000 commutauto-0.3.0/commutauto.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-29 00:54:23.000000 commutauto-0.3.0/commutauto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-29 00:54:23.000000 commutauto-0.3.0/commutauto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 00:54:23.971437 commutauto-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-29 00:54:07.000000 commutauto-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 23:34:19.547669 commutauto-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-29 23:34:19.543669 commutauto-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-07-29 23:34:05.000000 commutauto-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 23:34:19.539669 commutauto-0.3.1/commutauto/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-29 23:34:05.000000 commutauto-0.3.1/commutauto/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-29 23:34:05.000000 commutauto-0.3.1/commutauto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-07-29 23:34:05.000000 commutauto-0.3.1/commutauto/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 23:34:19.543669 commutauto-0.3.1/commutauto/booking_service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 23:34:05.000000 commutauto-0.3.1/commutauto/booking_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-29 23:34:05.000000 commutauto-0.3.1/commutauto/booking_service/date_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-07-29 23:34:05.000000 commutauto-0.3.1/commutauto/booking_service/flex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-07-29 23:34:05.000000 commutauto-0.3.1/commutauto/booking_service/payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-07-29 23:34:05.000000 commutauto-0.3.1/commutauto/booking_service/retriers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15016 2023-07-29 23:34:05.000000 commutauto-0.3.1/commutauto/booking_service/station.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 23:34:19.543669 commutauto-0.3.1/commutauto/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-29 23:34:05.000000 commutauto-0.3.1/commutauto/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-29 23:34:05.000000 commutauto-0.3.1/commutauto/client/auth_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12779 2023-07-29 23:34:05.000000 commutauto-0.3.1/commutauto/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-07-29 23:34:05.000000 commutauto-0.3.1/commutauto/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-29 23:34:05.000000 commutauto-0.3.1/commutauto/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 23:34:19.543669 commutauto-0.3.1/commutauto/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-29 23:34:05.000000 commutauto-0.3.1/commutauto/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-29 23:34:05.000000 commutauto-0.3.1/commutauto/model/flex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-29 23:34:05.000000 commutauto-0.3.1/commutauto/model/flex_booking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-29 23:34:05.000000 commutauto-0.3.1/commutauto/model/reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-29 23:34:05.000000 commutauto-0.3.1/commutauto/model/station.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 23:34:19.543669 commutauto-0.3.1/commutauto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-29 23:34:19.000000 commutauto-0.3.1/commutauto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-29 23:34:19.000000 commutauto-0.3.1/commutauto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 23:34:19.000000 commutauto-0.3.1/commutauto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-29 23:34:19.000000 commutauto-0.3.1/commutauto.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-29 23:34:19.000000 commutauto-0.3.1/commutauto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-29 23:34:19.000000 commutauto-0.3.1/commutauto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 23:34:19.547669 commutauto-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-29 23:34:05.000000 commutauto-0.3.1/setup.py
```

### Comparing `commutauto-0.3.0/PKG-INFO` & `commutauto-0.3.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commutauto
-Version: 0.3.0
+Version: 0.3.1
 Summary: CLI to interact with your car sharing service API. Search for available vehicles, manage your bookings and more...
 Home-page: https://github.com/elbuco1/commutauto
 Author: Laurent Boucaud
 Author-email: lrtboucaud@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
```

### Comparing `commutauto-0.3.0/README.md` & `commutauto-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `commutauto-0.3.0/commutauto/__main__.py` & `commutauto-0.3.1/commutauto/__main__.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.3.0/commutauto/booking_service/date_manager.py` & `commutauto-0.3.1/commutauto/booking_service/date_manager.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.3.0/commutauto/booking_service/flex.py` & `commutauto-0.3.1/commutauto/booking_service/flex.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.3.0/commutauto/booking_service/payload.py` & `commutauto-0.3.1/commutauto/booking_service/payload.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.3.0/commutauto/booking_service/retriers.py` & `commutauto-0.3.1/commutauto/booking_service/retriers.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.3.0/commutauto/booking_service/station.py` & `commutauto-0.3.1/commutauto/booking_service/station.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.3.0/commutauto/client/auth_token.py` & `commutauto-0.3.1/commutauto/client/auth_token.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.3.0/commutauto/client/client.py` & `commutauto-0.3.1/commutauto/client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 logger = logging.getLogger(__name__)
 
 class CommutautoClient():
     def __init__(self, 
             commutauto_security_api_endpoint = "https://securityservice.reservauto.net",
             authentication_header_value = "Basic Q29tbXVuYXV0b01vYmlsZUFwcDI6dUVWbEM0dzdiUkMyWlZtQWRjWG9xeXUxdQ==", 
-            token_file_path="token.json",
+            token_file_path=os.environ.get('COMMUTAUTO_TOKEN_FILE', "token.json"),
             authenticated=True):
         
         logger.info(f"Create CommutautoClient. Authentication is {'enabled' if authenticated else 'disabled'}.")
 
         load_dotenv()
         self.token_file_path = token_file_path
         self.commutauto_security_api_endpoint = commutauto_security_api_endpoint
```

### Comparing `commutauto-0.3.0/commutauto/constants.py` & `commutauto-0.3.1/commutauto/constants.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.3.0/commutauto/exceptions.py` & `commutauto-0.3.1/commutauto/exceptions.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.3.0/commutauto/model/flex.py` & `commutauto-0.3.1/commutauto/model/flex.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.3.0/commutauto/model/flex_booking.py` & `commutauto-0.3.1/commutauto/model/flex_booking.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.3.0/commutauto/model/reservation.py` & `commutauto-0.3.1/commutauto/model/reservation.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.3.0/commutauto/model/station.py` & `commutauto-0.3.1/commutauto/model/station.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.3.0/commutauto.egg-info/PKG-INFO` & `commutauto-0.3.1/commutauto.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commutauto
-Version: 0.3.0
+Version: 0.3.1
 Summary: CLI to interact with your car sharing service API. Search for available vehicles, manage your bookings and more...
 Home-page: https://github.com/elbuco1/commutauto
 Author: Laurent Boucaud
 Author-email: lrtboucaud@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
```

### Comparing `commutauto-0.3.0/commutauto.egg-info/SOURCES.txt` & `commutauto-0.3.1/commutauto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `commutauto-0.3.0/setup.py` & `commutauto-0.3.1/setup.py`

 * *Files identical despite different names*

