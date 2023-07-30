# Comparing `tmp/stadata-0.0.3.tar.gz` & `tmp/stadata-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stadata-0.0.3.tar", last modified: Sun Jul 30 04:15:03 2023, max compression
+gzip compressed data, was "stadata-0.1.0.tar", last modified: Sun Jul 30 04:23:12 2023, max compression
```

## Comparing `stadata-0.0.3.tar` & `stadata-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 mac202129   (501) staff       (20)        0 2023-07-30 04:15:03.664184 stadata-0.0.3/
--rw-r--r--   0 mac202129   (501) staff       (20)     6148 2023-07-29 16:19:14.000000 stadata-0.0.3/.DS_Store
--rw-r--r--   0 mac202129   (501) staff       (20)       86 2023-07-29 16:17:36.000000 stadata-0.0.3/.gitignore
--rw-r--r--   0 mac202129   (501) staff       (20)     1074 2023-07-15 08:24:13.000000 stadata-0.0.3/LICENCSE
--rw-r--r--   0 mac202129   (501) staff       (20)    14412 2023-07-30 04:15:03.663809 stadata-0.0.3/PKG-INFO
--rw-r--r--   0 mac202129   (501) staff       (20)    13413 2023-07-30 04:12:16.000000 stadata-0.0.3/README.md
--rw-r--r--   0 mac202129   (501) staff       (20)     1584 2023-07-29 16:17:53.000000 stadata-0.0.3/pyproject.toml
--rw-r--r--   0 mac202129   (501) staff       (20)       31 2023-07-23 09:32:54.000000 stadata-0.0.3/requirements.txt
--rw-r--r--   0 mac202129   (501) staff       (20)       38 2023-07-30 04:15:03.664265 stadata-0.0.3/setup.cfg
-drwxr-xr-x   0 mac202129   (501) staff       (20)        0 2023-07-30 04:15:03.659986 stadata-0.0.3/stadata/
--rw-r--r--   0 mac202129   (501) staff       (20)     6148 2023-07-29 14:59:20.000000 stadata-0.0.3/stadata/.DS_Store
--rw-r--r--   0 mac202129   (501) staff       (20)       24 2023-07-15 07:53:40.000000 stadata-0.0.3/stadata/__init__.py
--rw-r--r--   0 mac202129   (501) staff       (20)    21646 2023-07-29 16:03:57.000000 stadata-0.0.3/stadata/main.py
--rw-r--r--   0 mac202129   (501) staff       (20)      460 2023-07-26 15:06:41.000000 stadata-0.0.3/stadata/material.py
-drwxr-xr-x   0 mac202129   (501) staff       (20)        0 2023-07-30 04:15:03.663354 stadata-0.0.3/stadata.egg-info/
--rw-r--r--   0 mac202129   (501) staff       (20)    14412 2023-07-30 04:15:03.000000 stadata-0.0.3/stadata.egg-info/PKG-INFO
--rw-r--r--   0 mac202129   (501) staff       (20)      299 2023-07-30 04:15:03.000000 stadata-0.0.3/stadata.egg-info/SOURCES.txt
--rw-r--r--   0 mac202129   (501) staff       (20)        1 2023-07-30 04:15:03.000000 stadata-0.0.3/stadata.egg-info/dependency_links.txt
--rw-r--r--   0 mac202129   (501) staff       (20)       32 2023-07-30 04:15:03.000000 stadata-0.0.3/stadata.egg-info/requires.txt
--rw-r--r--   0 mac202129   (501) staff       (20)        8 2023-07-30 04:15:03.000000 stadata-0.0.3/stadata.egg-info/top_level.txt
+drwxr-xr-x   0 mac202129   (501) staff       (20)        0 2023-07-30 04:23:12.128374 stadata-0.1.0/
+-rw-r--r--   0 mac202129   (501) staff       (20)     6148 2023-07-29 16:19:14.000000 stadata-0.1.0/.DS_Store
+-rw-r--r--   0 mac202129   (501) staff       (20)       86 2023-07-29 16:17:36.000000 stadata-0.1.0/.gitignore
+-rw-r--r--   0 mac202129   (501) staff       (20)     1074 2023-07-15 08:24:13.000000 stadata-0.1.0/LICENCSE
+-rw-r--r--   0 mac202129   (501) staff       (20)    14412 2023-07-30 04:23:12.128041 stadata-0.1.0/PKG-INFO
+-rw-r--r--   0 mac202129   (501) staff       (20)    13413 2023-07-30 04:12:16.000000 stadata-0.1.0/README.md
+-rw-r--r--   0 mac202129   (501) staff       (20)     1584 2023-07-30 04:22:55.000000 stadata-0.1.0/pyproject.toml
+-rw-r--r--   0 mac202129   (501) staff       (20)       31 2023-07-23 09:32:54.000000 stadata-0.1.0/requirements.txt
+-rw-r--r--   0 mac202129   (501) staff       (20)       38 2023-07-30 04:23:12.128460 stadata-0.1.0/setup.cfg
+drwxr-xr-x   0 mac202129   (501) staff       (20)        0 2023-07-30 04:23:12.125962 stadata-0.1.0/stadata/
+-rw-r--r--   0 mac202129   (501) staff       (20)     6148 2023-07-29 14:59:20.000000 stadata-0.1.0/stadata/.DS_Store
+-rw-r--r--   0 mac202129   (501) staff       (20)       24 2023-07-15 07:53:40.000000 stadata-0.1.0/stadata/__init__.py
+-rw-r--r--   0 mac202129   (501) staff       (20)    21482 2023-07-30 04:22:38.000000 stadata-0.1.0/stadata/main.py
+-rw-r--r--   0 mac202129   (501) staff       (20)      460 2023-07-26 15:06:41.000000 stadata-0.1.0/stadata/material.py
+drwxr-xr-x   0 mac202129   (501) staff       (20)        0 2023-07-30 04:23:12.127644 stadata-0.1.0/stadata.egg-info/
+-rw-r--r--   0 mac202129   (501) staff       (20)    14412 2023-07-30 04:23:12.000000 stadata-0.1.0/stadata.egg-info/PKG-INFO
+-rw-r--r--   0 mac202129   (501) staff       (20)      299 2023-07-30 04:23:12.000000 stadata-0.1.0/stadata.egg-info/SOURCES.txt
+-rw-r--r--   0 mac202129   (501) staff       (20)        1 2023-07-30 04:23:12.000000 stadata-0.1.0/stadata.egg-info/dependency_links.txt
+-rw-r--r--   0 mac202129   (501) staff       (20)       32 2023-07-30 04:23:12.000000 stadata-0.1.0/stadata.egg-info/requires.txt
+-rw-r--r--   0 mac202129   (501) staff       (20)        8 2023-07-30 04:23:12.000000 stadata-0.1.0/stadata.egg-info/top_level.txt
```

### Comparing `stadata-0.0.3/.DS_Store` & `stadata-0.1.0/.DS_Store`

 * *Files identical despite different names*

### Comparing `stadata-0.0.3/LICENCSE` & `stadata-0.1.0/LICENCSE`

 * *Files identical despite different names*

### Comparing `stadata-0.0.3/PKG-INFO` & `stadata-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stadata
-Version: 0.0.3
+Version: 0.1.0
 Summary: API for get all statistics data from BPS
 Author-email: Ignatius Sandyawan <isandyawan@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/bps-statistics/stadata
 Keywords: bps dataset utility indonesia
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `stadata-0.0.3/README.md` & `stadata-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `stadata-0.0.3/pyproject.toml` & `stadata-0.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stadata"
-version = "0.0.3"
+version = "0.1.0"
 description = "API for get all statistics data from BPS"
 urls = {homepage = "https://github.com/bps-statistics/stadata"}
 requires-python = ">=3.7"
 authors = [
     {name = "Ignatius Sandyawan", email = "isandyawan@gmail.com"}
 ]
 license = {text = "MIT"}
```

### Comparing `stadata-0.0.3/stadata/.DS_Store` & `stadata-0.1.0/stadata/.DS_Store`

 * *Files identical despite different names*

### Comparing `stadata-0.0.3/stadata/main.py` & `stadata-0.1.0/stadata/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -283,15 +283,15 @@
         """
         Method to get all static table
         :param domain: array of ID domain data
         :param all: get all data from whole domain or not
         :param latest:get last data from webapi
         """
         if(not latest):
-            allStaticTable = pd.read_csv('https://gist.githubusercontent.com/isandyawan/31c29bd92039c4ff7b736826a7065028/raw/1eb6e0eca9a90ce4b2f68317fd589faeef6b92d4/allStaticTable.csv',sep="|")
+            allStaticTable = pd.read_csv('https://gist.githubusercontent.com/isandyawan/31c29bd92039c4ff7b736826a7065028/raw/allStaticTable.csv',sep="|")
             if(not all):
                 domain = [int(numeric_string) for numeric_string in domain]
                 allStaticTable.loc[allStaticTable['domain'].isin(domain)]
         else: 
             if(all):
                 warnings.warn("It will take around 2 hour")
                 domain = self.list_domain()
@@ -312,15 +312,15 @@
         """
         Method to get all dynamic table
         :param domain: array of ID domain data
         :param all: get all data from whole domain or not
         :param latest:get last data from webapi
         """
         if(not latest):
-            allVariable = pd.read_csv('https://gist.githubusercontent.com/isandyawan/4d3efaeea4608c11b1e22b8a51fd0e4d/raw/479d7f098548e95a239178e87da39c7ac1b2aa36/allVariable.csv',sep="|")
+            allVariable = pd.read_csv('https://gist.githubusercontent.com/isandyawan/4d3efaeea4608c11b1e22b8a51fd0e4d/raw/allVariable.csv',sep="|")
             if(not all):
                 domain = [int(numeric_string) for numeric_string in domain]
                 allVariable.loc[allVariable['domain'].isin(domain)]
         else: 
             index = 0
             allVariable = []
             if(all):
@@ -341,15 +341,15 @@
         """
         Method to get all press release
         :param domain: array of ID domain data
         :param all: get all data from whole domain or not
         :param latest:get last data from webapi
         """
         if(not latest):
-            allPressRelease = pd.read_csv('https://gist.githubusercontent.com/isandyawan/4e67a8cf452838e914187e3597bf70c4/raw/509c4a70716d5c3c74973eb973ba99a21e11d761/allPressRelease.csv',sep="|", index_col=[0])
+            allPressRelease = pd.read_csv('https://gist.githubusercontent.com/isandyawan/4e67a8cf452838e914187e3597bf70c4/raw/allPressRelease.csv',sep="|", index_col=[0])
             if(not all):
                 domain = [int(numeric_string) for numeric_string in domain]
                 allPressRelease.loc[allPressRelease['domain'].isin(domain)]
                 if((month!="") & (year !="")):
                     allPressRelease = allPressRelease.loc[allPressRelease['rl_date'].str.contains(year+'-'+'{0:0>2}'.format(month))]
         else: 
             if(all):
@@ -372,15 +372,15 @@
         """
         Method to get all publication
         :param domain: array of ID domain data
         :param all: get all data from whole domain or not
         :param latest:get last data from webapi
         """
         if(not latest):
-            allPublication = pd.read_csv('https://gist.githubusercontent.com/isandyawan/31b48670d76a199bc88fba3ec3c0672f/raw/72d3c6941f9dc6d0674af685c0ccc5f59f20e9fa/allPublication.csv',sep="|", index_col=[0])
+            allPublication = pd.read_csv('https://gist.githubusercontent.com/isandyawan/31b48670d76a199bc88fba3ec3c0672f/raw/allPublication.csv',sep="|", index_col=[0])
             if(not all):
                 domain = [int(numeric_string) for numeric_string in domain]
                 allPublication = allPublication.loc[allPublication['domain'].isin(domain)]
                 if((month!="") & (year !="")):
                     allPublication = allPublication.loc[allPublication['rl_date'].str.contains(year+'-'+'{0:0>2}'.format(month))]
         else: 
             if(all):
```

### Comparing `stadata-0.0.3/stadata.egg-info/PKG-INFO` & `stadata-0.1.0/stadata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stadata
-Version: 0.0.3
+Version: 0.1.0
 Summary: API for get all statistics data from BPS
 Author-email: Ignatius Sandyawan <isandyawan@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/bps-statistics/stadata
 Keywords: bps dataset utility indonesia
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

