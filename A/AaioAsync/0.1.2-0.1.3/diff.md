# Comparing `tmp/AaioAsync-0.1.2.tar.gz` & `tmp/AaioAsync-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AaioAsync-0.1.2.tar", last modified: Sat Jul 29 21:38:49 2023, max compression
+gzip compressed data, was "AaioAsync-0.1.3.tar", last modified: Sat Jul 29 22:37:23 2023, max compression
```

## Comparing `AaioAsync-0.1.2.tar` & `AaioAsync-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 21:38:49.499199 AaioAsync-0.1.2/
-drwxrwxrwx   0        0        0        0 2023-07-29 21:38:49.480197 AaioAsync-0.1.2/AaioAsync/
--rw-rw-rw-   0        0        0       26 2023-07-29 17:17:54.000000 AaioAsync-0.1.2/AaioAsync/__init__.py
--rw-rw-rw-   0        0        0     8255 2023-07-29 21:10:19.000000 AaioAsync-0.1.2/AaioAsync/api.py
-drwxrwxrwx   0        0        0        0 2023-07-29 21:38:49.493201 AaioAsync-0.1.2/AaioAsync/exceptions/
--rw-rw-rw-   0        0        0       34 2023-07-29 17:44:03.000000 AaioAsync-0.1.2/AaioAsync/exceptions/__init__.py
--rw-rw-rw-   0        0        0       42 2023-07-29 17:34:35.000000 AaioAsync-0.1.2/AaioAsync/exceptions/errors.py
-drwxrwxrwx   0        0        0        0 2023-07-29 21:38:49.497201 AaioAsync-0.1.2/AaioAsync/models/
--rw-rw-rw-   0        0        0      120 2023-07-27 19:51:43.000000 AaioAsync-0.1.2/AaioAsync/models/balance.py
--rw-rw-rw-   0        0        0      731 2023-07-29 19:20:51.000000 AaioAsync-0.1.2/AaioAsync/models/order.py
--rw-rw-rw-   0        0        0      710 2023-07-29 19:07:16.000000 AaioAsync-0.1.2/AaioAsync/models/withdrawal.py
--rw-rw-rw-   0        0        0     1431 2023-07-29 20:12:10.000000 AaioAsync-0.1.2/AaioAsync/requests.py
-drwxrwxrwx   0        0        0        0 2023-07-29 21:38:49.489199 AaioAsync-0.1.2/AaioAsync.egg-info/
--rw-rw-rw-   0        0        0      261 2023-07-29 21:38:49.000000 AaioAsync-0.1.2/AaioAsync.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-07-29 21:38:49.000000 AaioAsync-0.1.2/AaioAsync.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 21:38:49.000000 AaioAsync-0.1.2/AaioAsync.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-29 21:38:49.000000 AaioAsync-0.1.2/AaioAsync.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       25 2023-07-29 21:38:49.000000 AaioAsync-0.1.2/AaioAsync.egg-info/requires.txt
--rw-rw-rw-   0        0        0       48 2023-07-29 21:38:49.000000 AaioAsync-0.1.2/AaioAsync.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      261 2023-07-29 21:38:49.499199 AaioAsync-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-29 21:38:49.500200 AaioAsync-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      439 2023-07-29 21:38:43.000000 AaioAsync-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 22:37:23.990014 AaioAsync-0.1.3/
+drwxrwxrwx   0        0        0        0 2023-07-29 22:37:23.972013 AaioAsync-0.1.3/AaioAsync/
+-rw-rw-rw-   0        0        0       26 2023-07-29 17:17:54.000000 AaioAsync-0.1.3/AaioAsync/__init__.py
+-rw-rw-rw-   0        0        0     8255 2023-07-29 21:10:19.000000 AaioAsync-0.1.3/AaioAsync/api.py
+drwxrwxrwx   0        0        0        0 2023-07-29 22:37:23.984015 AaioAsync-0.1.3/AaioAsync/exceptions/
+-rw-rw-rw-   0        0        0       34 2023-07-29 17:44:03.000000 AaioAsync-0.1.3/AaioAsync/exceptions/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-07-29 17:34:35.000000 AaioAsync-0.1.3/AaioAsync/exceptions/errors.py
+drwxrwxrwx   0        0        0        0 2023-07-29 22:37:23.988015 AaioAsync-0.1.3/AaioAsync/models/
+-rw-rw-rw-   0        0        0      120 2023-07-27 19:51:43.000000 AaioAsync-0.1.3/AaioAsync/models/balance.py
+-rw-rw-rw-   0        0        0      731 2023-07-29 19:20:51.000000 AaioAsync-0.1.3/AaioAsync/models/order.py
+-rw-rw-rw-   0        0        0      710 2023-07-29 19:07:16.000000 AaioAsync-0.1.3/AaioAsync/models/withdrawal.py
+-rw-rw-rw-   0        0        0     1431 2023-07-29 20:12:10.000000 AaioAsync-0.1.3/AaioAsync/requests.py
+drwxrwxrwx   0        0        0        0 2023-07-29 22:37:23.981015 AaioAsync-0.1.3/AaioAsync.egg-info/
+-rw-rw-rw-   0        0        0     1332 2023-07-29 22:37:23.000000 AaioAsync-0.1.3/AaioAsync.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-07-29 22:37:23.000000 AaioAsync-0.1.3/AaioAsync.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 22:37:23.000000 AaioAsync-0.1.3/AaioAsync.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-29 22:37:23.000000 AaioAsync-0.1.3/AaioAsync.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       25 2023-07-29 22:37:23.000000 AaioAsync-0.1.3/AaioAsync.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       48 2023-07-29 22:37:23.000000 AaioAsync-0.1.3/AaioAsync.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1332 2023-07-29 22:37:23.990014 AaioAsync-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-29 22:37:23.992015 AaioAsync-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1515 2023-07-29 22:37:18.000000 AaioAsync-0.1.3/setup.py
```

### Comparing `AaioAsync-0.1.2/AaioAsync/api.py` & `AaioAsync-0.1.3/AaioAsync/api.py`

 * *Files identical despite different names*

### Comparing `AaioAsync-0.1.2/AaioAsync/models/order.py` & `AaioAsync-0.1.3/AaioAsync/models/order.py`

 * *Files identical despite different names*

### Comparing `AaioAsync-0.1.2/AaioAsync/models/withdrawal.py` & `AaioAsync-0.1.3/AaioAsync/models/withdrawal.py`

 * *Files identical despite different names*

### Comparing `AaioAsync-0.1.2/AaioAsync/requests.py` & `AaioAsync-0.1.3/AaioAsync/requests.py`

 * *Files identical despite different names*

