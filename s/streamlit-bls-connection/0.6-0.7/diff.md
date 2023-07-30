# Comparing `tmp/streamlit_bls_connection-0.6.tar.gz` & `tmp/streamlit_bls_connection-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_bls_connection-0.6.tar", last modified: Sat Jul 29 21:11:12 2023, max compression
+gzip compressed data, was "streamlit_bls_connection-0.7.tar", last modified: Sun Jul 30 01:43:15 2023, max compression
```

## Comparing `streamlit_bls_connection-0.6.tar` & `streamlit_bls_connection-0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 21:11:12.990549 streamlit_bls_connection-0.6/
--rw-rw-rw-   0        0        0     1089 2023-07-29 16:30:01.000000 streamlit_bls_connection-0.6/LICENSE
--rw-rw-rw-   0        0        0     2263 2023-07-29 21:11:12.990549 streamlit_bls_connection-0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1412 2023-07-29 21:07:32.000000 streamlit_bls_connection-0.6/README.md
--rw-rw-rw-   0        0        0      389 2023-07-29 21:09:36.000000 streamlit_bls_connection-0.6/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-07-29 21:11:12.991558 streamlit_bls_connection-0.6/setup.cfg
--rw-rw-rw-   0        0        0     1188 2023-07-29 21:09:23.000000 streamlit_bls_connection-0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 21:11:12.940014 streamlit_bls_connection-0.6/streamlit_bls_connection/
--rw-rw-rw-   0        0        0       65 2023-07-29 16:22:24.000000 streamlit_bls_connection-0.6/streamlit_bls_connection/__init__.py
--rw-rw-rw-   0        0        0     3645 2023-07-25 22:28:07.000000 streamlit_bls_connection-0.6/streamlit_bls_connection/bls_connection.py
--rw-rw-rw-   0        0        0       33 2023-07-29 21:09:47.000000 streamlit_bls_connection-0.6/streamlit_bls_connection/version.py
-drwxrwxrwx   0        0        0        0 2023-07-29 21:11:12.989531 streamlit_bls_connection-0.6/streamlit_bls_connection.egg-info/
--rw-rw-rw-   0        0        0     2263 2023-07-29 21:11:12.000000 streamlit_bls_connection-0.6/streamlit_bls_connection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2023-07-29 21:11:12.000000 streamlit_bls_connection-0.6/streamlit_bls_connection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 21:11:12.000000 streamlit_bls_connection-0.6/streamlit_bls_connection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-07-29 21:11:12.000000 streamlit_bls_connection-0.6/streamlit_bls_connection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-07-29 21:11:12.000000 streamlit_bls_connection-0.6/streamlit_bls_connection.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 01:43:15.689288 streamlit_bls_connection-0.7/
+-rw-rw-rw-   0        0        0     1089 2023-07-29 16:30:01.000000 streamlit_bls_connection-0.7/LICENSE
+-rw-rw-rw-   0        0        0     4452 2023-07-30 01:43:15.689288 streamlit_bls_connection-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3562 2023-07-30 01:36:49.000000 streamlit_bls_connection-0.7/README.md
+-rw-rw-rw-   0        0        0      389 2023-07-30 01:42:35.000000 streamlit_bls_connection-0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-07-30 01:43:15.690286 streamlit_bls_connection-0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1188 2023-07-30 01:42:17.000000 streamlit_bls_connection-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 01:43:15.649024 streamlit_bls_connection-0.7/streamlit_bls_connection/
+-rw-rw-rw-   0        0        0       65 2023-07-29 16:22:24.000000 streamlit_bls_connection-0.7/streamlit_bls_connection/__init__.py
+-rw-rw-rw-   0        0        0     3601 2023-07-30 01:29:28.000000 streamlit_bls_connection-0.7/streamlit_bls_connection/bls_connection.py
+-rw-rw-rw-   0        0        0       33 2023-07-30 01:42:56.000000 streamlit_bls_connection-0.7/streamlit_bls_connection/version.py
+drwxrwxrwx   0        0        0        0 2023-07-30 01:43:15.689288 streamlit_bls_connection-0.7/streamlit_bls_connection.egg-info/
+-rw-rw-rw-   0        0        0     4452 2023-07-30 01:43:15.000000 streamlit_bls_connection-0.7/streamlit_bls_connection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2023-07-30 01:43:15.000000 streamlit_bls_connection-0.7/streamlit_bls_connection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 01:43:15.000000 streamlit_bls_connection-0.7/streamlit_bls_connection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-07-30 01:43:15.000000 streamlit_bls_connection-0.7/streamlit_bls_connection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-07-30 01:43:15.000000 streamlit_bls_connection-0.7/streamlit_bls_connection.egg-info/top_level.txt
```

### Comparing `streamlit_bls_connection-0.6/LICENSE` & `streamlit_bls_connection-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_bls_connection-0.6/setup.py` & `streamlit_bls_connection-0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='streamlit_bls_connection',
-    version='0.6',
+    version='0.7',
     license='MIT',  
     description='A package to fetch Bureau of Labor Statistics data using Streamlit',
     long_description=long_description,  
     long_description_content_type='text/markdown',
     author='Tony Hollaar',
     author_email='thollaar@gmail.com',
     url='https://github.com/tonyhollaar/',
```

### Comparing `streamlit_bls_connection-0.6/streamlit_bls_connection/bls_connection.py` & `streamlit_bls_connection-0.7/streamlit_bls_connection/bls_connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,10 +66,10 @@
         # This method will be called by the Streamlit app to retrieve data using the custom connection.
         # You can implement any caching logic or other data processing here.
         connection = BLSConnection("bls_connection")
         try:
             return connection.fetch_data(series_id, start_year, end_year)
         except KeyError:
             with st.sidebar:
-                st.error("😒 **Error**: Failed to fetch latest data. Daily query limit is exceeded, retrieving stored data from backup source.")
+                st.error("😒 **Error**: Failed to fetch latest data. Daily query limit is exceeded")
            #st.stop()  # Stop the app execution and display the error message to the user
             return None
```

