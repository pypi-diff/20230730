# Comparing `tmp/stadata-0.1.0.tar.gz` & `tmp/stadata-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stadata-0.1.0.tar", last modified: Sun Jul 30 04:23:12 2023, max compression
+gzip compressed data, was "stadata-0.1.1.tar", last modified: Sun Jul 30 04:30:50 2023, max compression
```

## Comparing `stadata-0.1.0.tar` & `stadata-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 mac202129   (501) staff       (20)        0 2023-07-30 04:23:12.128374 stadata-0.1.0/
--rw-r--r--   0 mac202129   (501) staff       (20)     6148 2023-07-29 16:19:14.000000 stadata-0.1.0/.DS_Store
--rw-r--r--   0 mac202129   (501) staff       (20)       86 2023-07-29 16:17:36.000000 stadata-0.1.0/.gitignore
--rw-r--r--   0 mac202129   (501) staff       (20)     1074 2023-07-15 08:24:13.000000 stadata-0.1.0/LICENCSE
--rw-r--r--   0 mac202129   (501) staff       (20)    14412 2023-07-30 04:23:12.128041 stadata-0.1.0/PKG-INFO
--rw-r--r--   0 mac202129   (501) staff       (20)    13413 2023-07-30 04:12:16.000000 stadata-0.1.0/README.md
--rw-r--r--   0 mac202129   (501) staff       (20)     1584 2023-07-30 04:22:55.000000 stadata-0.1.0/pyproject.toml
--rw-r--r--   0 mac202129   (501) staff       (20)       31 2023-07-23 09:32:54.000000 stadata-0.1.0/requirements.txt
--rw-r--r--   0 mac202129   (501) staff       (20)       38 2023-07-30 04:23:12.128460 stadata-0.1.0/setup.cfg
-drwxr-xr-x   0 mac202129   (501) staff       (20)        0 2023-07-30 04:23:12.125962 stadata-0.1.0/stadata/
--rw-r--r--   0 mac202129   (501) staff       (20)     6148 2023-07-29 14:59:20.000000 stadata-0.1.0/stadata/.DS_Store
--rw-r--r--   0 mac202129   (501) staff       (20)       24 2023-07-15 07:53:40.000000 stadata-0.1.0/stadata/__init__.py
--rw-r--r--   0 mac202129   (501) staff       (20)    21482 2023-07-30 04:22:38.000000 stadata-0.1.0/stadata/main.py
--rw-r--r--   0 mac202129   (501) staff       (20)      460 2023-07-26 15:06:41.000000 stadata-0.1.0/stadata/material.py
-drwxr-xr-x   0 mac202129   (501) staff       (20)        0 2023-07-30 04:23:12.127644 stadata-0.1.0/stadata.egg-info/
--rw-r--r--   0 mac202129   (501) staff       (20)    14412 2023-07-30 04:23:12.000000 stadata-0.1.0/stadata.egg-info/PKG-INFO
--rw-r--r--   0 mac202129   (501) staff       (20)      299 2023-07-30 04:23:12.000000 stadata-0.1.0/stadata.egg-info/SOURCES.txt
--rw-r--r--   0 mac202129   (501) staff       (20)        1 2023-07-30 04:23:12.000000 stadata-0.1.0/stadata.egg-info/dependency_links.txt
--rw-r--r--   0 mac202129   (501) staff       (20)       32 2023-07-30 04:23:12.000000 stadata-0.1.0/stadata.egg-info/requires.txt
--rw-r--r--   0 mac202129   (501) staff       (20)        8 2023-07-30 04:23:12.000000 stadata-0.1.0/stadata.egg-info/top_level.txt
+drwxr-xr-x   0 mac202129   (501) staff       (20)        0 2023-07-30 04:30:50.556564 stadata-0.1.1/
+-rw-r--r--   0 mac202129   (501) staff       (20)     6148 2023-07-29 16:19:14.000000 stadata-0.1.1/.DS_Store
+-rw-r--r--   0 mac202129   (501) staff       (20)       86 2023-07-29 16:17:36.000000 stadata-0.1.1/.gitignore
+-rw-r--r--   0 mac202129   (501) staff       (20)     1074 2023-07-15 08:24:13.000000 stadata-0.1.1/LICENCSE
+-rw-r--r--   0 mac202129   (501) staff       (20)    14412 2023-07-30 04:30:50.556232 stadata-0.1.1/PKG-INFO
+-rw-r--r--   0 mac202129   (501) staff       (20)    13413 2023-07-30 04:12:16.000000 stadata-0.1.1/README.md
+-rw-r--r--   0 mac202129   (501) staff       (20)     1584 2023-07-30 04:29:27.000000 stadata-0.1.1/pyproject.toml
+-rw-r--r--   0 mac202129   (501) staff       (20)       31 2023-07-23 09:32:54.000000 stadata-0.1.1/requirements.txt
+-rw-r--r--   0 mac202129   (501) staff       (20)       38 2023-07-30 04:30:50.556647 stadata-0.1.1/setup.cfg
+drwxr-xr-x   0 mac202129   (501) staff       (20)        0 2023-07-30 04:30:50.554266 stadata-0.1.1/stadata/
+-rw-r--r--   0 mac202129   (501) staff       (20)     6148 2023-07-29 14:59:20.000000 stadata-0.1.1/stadata/.DS_Store
+-rw-r--r--   0 mac202129   (501) staff       (20)       24 2023-07-15 07:53:40.000000 stadata-0.1.1/stadata/__init__.py
+-rw-r--r--   0 mac202129   (501) staff       (20)    21839 2023-07-30 04:29:18.000000 stadata-0.1.1/stadata/main.py
+-rw-r--r--   0 mac202129   (501) staff       (20)      460 2023-07-26 15:06:41.000000 stadata-0.1.1/stadata/material.py
+drwxr-xr-x   0 mac202129   (501) staff       (20)        0 2023-07-30 04:30:50.555743 stadata-0.1.1/stadata.egg-info/
+-rw-r--r--   0 mac202129   (501) staff       (20)    14412 2023-07-30 04:30:50.000000 stadata-0.1.1/stadata.egg-info/PKG-INFO
+-rw-r--r--   0 mac202129   (501) staff       (20)      299 2023-07-30 04:30:50.000000 stadata-0.1.1/stadata.egg-info/SOURCES.txt
+-rw-r--r--   0 mac202129   (501) staff       (20)        1 2023-07-30 04:30:50.000000 stadata-0.1.1/stadata.egg-info/dependency_links.txt
+-rw-r--r--   0 mac202129   (501) staff       (20)       32 2023-07-30 04:30:50.000000 stadata-0.1.1/stadata.egg-info/requires.txt
+-rw-r--r--   0 mac202129   (501) staff       (20)        8 2023-07-30 04:30:50.000000 stadata-0.1.1/stadata.egg-info/top_level.txt
```

### Comparing `stadata-0.1.0/.DS_Store` & `stadata-0.1.1/.DS_Store`

 * *Files identical despite different names*

### Comparing `stadata-0.1.0/LICENCSE` & `stadata-0.1.1/LICENCSE`

 * *Files identical despite different names*

### Comparing `stadata-0.1.0/PKG-INFO` & `stadata-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stadata
-Version: 0.1.0
+Version: 0.1.1
 Summary: API for get all statistics data from BPS
 Author-email: Ignatius Sandyawan <isandyawan@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/bps-statistics/stadata
 Keywords: bps dataset utility indonesia
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `stadata-0.1.0/README.md` & `stadata-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `stadata-0.1.0/pyproject.toml` & `stadata-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stadata"
-version = "0.1.0"
+version = "0.1.1"
 description = "API for get all statistics data from BPS"
 urls = {homepage = "https://github.com/bps-statistics/stadata"}
 requires-python = ">=3.7"
 authors = [
     {name = "Ignatius Sandyawan", email = "isandyawan@gmail.com"}
 ]
 license = {text = "MIT"}
```

### Comparing `stadata-0.1.0/stadata/.DS_Store` & `stadata-0.1.1/stadata/.DS_Store`

 * *Files identical despite different names*

### Comparing `stadata-0.1.0/stadata/main.py` & `stadata-0.1.1/stadata/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,18 @@
         if(res.status_code!=200):
             warnings.warn("Connection failed")
         else:
             res = res.json()
             if(res['status']!='OK'):
                 raise Exception(res['message'])
             return res
+    
+    def __format_list(self,list):
+        list['domain'] = list['domain'].map('{0:0>4}'.format)
+        return list
         
     def __get_variable(self,domain='0000'):
         """
         Based Method to get all variable of dynamic table
         :param domain: ID domain data
         """
         page = 1
@@ -302,14 +306,15 @@
                 res = self.__get_statictable(domain=row)
                 res['domain'] = row
                 if(index==0):
                     allStaticTable = res
                 else:
                     allStaticTable = pd.concat([allStaticTable,res])
                 index += 1
+        allStaticTable = self.__format_list(allStaticTable)
         return allStaticTable
     
     def list_dynamictable(self, all=False, domain=[],latest=False):
         """
         Method to get all dynamic table
         :param domain: array of ID domain data
         :param all: get all data from whole domain or not
@@ -331,14 +336,15 @@
                 res = self.__get_variable(domain=row)
                 res['domain'] = row
                 if(index==0):
                     allVariable = res
                 else:
                     allVariable = pd.concat([allVariable,res])
                 index += 1
+        allVariable = self.__format_list(allVariable)
         return allVariable
     
     def list_pressrelease(self, all=True, domain=[], month="",year="",latest=False):
         """
         Method to get all press release
         :param domain: array of ID domain data
         :param all: get all data from whole domain or not
@@ -362,14 +368,15 @@
                 res = self.__get_pressRelease(domain=row,month=month,year=year)
                 res['domain'] = row
                 if(index==0):
                     allPressRelease = res
                 else:
                     allPressRelease = pd.concat([allPressRelease,res])
                 index += 1
+        allPressRelease = self.__format_list(allPressRelease)
         return allPressRelease
     
     def list_publication(self, all=True, domain=[], month="",year="",latest=False):
         """
         Method to get all publication
         :param domain: array of ID domain data
         :param all: get all data from whole domain or not
@@ -393,14 +400,15 @@
                 res = self.__get_publication(domain=row,month=month,year=year)
                 res['domain'] = row
                 if(index==0):
                     allPublication = res
                 else:
                     allPublication = pd.concat([allPublication,res])
                 index += 1
+        allPublication = self.__format_list(allPublication)
         return allPublication
 
     def list_domain(self):
         """
         Method to get all domain ID in level country till city
         """
         res = requests.get(f'{BASE_URL}api/domain/type/all/key/'f'{self.TOKEN}/')
```

### Comparing `stadata-0.1.0/stadata.egg-info/PKG-INFO` & `stadata-0.1.1/stadata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stadata
-Version: 0.1.0
+Version: 0.1.1
 Summary: API for get all statistics data from BPS
 Author-email: Ignatius Sandyawan <isandyawan@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/bps-statistics/stadata
 Keywords: bps dataset utility indonesia
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

