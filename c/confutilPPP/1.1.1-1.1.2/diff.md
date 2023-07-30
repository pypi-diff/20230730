# Comparing `tmp/confutilPPP-1.1.1.tar.gz` & `tmp/confutilPPP-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confutilPPP-1.1.1.tar", last modified: Sun Jul 30 11:12:15 2023, max compression
+gzip compressed data, was "confutilPPP-1.1.2.tar", last modified: Sun Jul 30 11:48:45 2023, max compression
```

## Comparing `confutilPPP-1.1.1.tar` & `confutilPPP-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:12:15.659235 confutilPPP-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-30 11:12:15.659235 confutilPPP-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-30 11:12:03.000000 confutilPPP-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:12:15.655235 confutilPPP-1.1.1/confutilPPP.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-30 11:12:15.000000 confutilPPP-1.1.1/confutilPPP.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-30 11:12:15.000000 confutilPPP-1.1.1/confutilPPP.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 11:12:15.000000 confutilPPP-1.1.1/confutilPPP.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-30 11:12:15.000000 confutilPPP-1.1.1/confutilPPP.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-30 11:12:15.000000 confutilPPP-1.1.1/confutilPPP.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 11:12:15.659235 confutilPPP-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-30 11:12:03.000000 confutilPPP-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:12:15.655235 confutilPPP-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:12:15.655235 confutilPPP-1.1.1/src/confutilPPP/
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-30 11:12:03.000000 confutilPPP-1.1.1/src/confutilPPP/__confutil__.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-30 11:12:03.000000 confutilPPP-1.1.1/src/confutilPPP/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:48:45.412942 confutilPPP-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-30 11:48:45.412942 confutilPPP-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-30 11:48:34.000000 confutilPPP-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:48:45.412942 confutilPPP-1.1.2/confutilPPP.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-30 11:48:45.000000 confutilPPP-1.1.2/confutilPPP.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-30 11:48:45.000000 confutilPPP-1.1.2/confutilPPP.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 11:48:45.000000 confutilPPP-1.1.2/confutilPPP.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-30 11:48:45.000000 confutilPPP-1.1.2/confutilPPP.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-30 11:48:45.000000 confutilPPP-1.1.2/confutilPPP.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 11:48:45.412942 confutilPPP-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-30 11:48:34.000000 confutilPPP-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:48:45.412942 confutilPPP-1.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:48:45.412942 confutilPPP-1.1.2/src/confutilPPP/
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-30 11:48:34.000000 confutilPPP-1.1.2/src/confutilPPP/__confutil__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-30 11:48:34.000000 confutilPPP-1.1.2/src/confutilPPP/__init__.py
```

### Comparing `confutilPPP-1.1.1/PKG-INFO` & `confutilPPP-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confutilPPP
-Version: 1.1.1
+Version: 1.1.2
 Summary: A simple configuration file tool
 Home-page: https://github.com/Aurorax-own/confutilPPP
 Author: Aurorax-own
 Author-email: 15047150695@163.com
 Project-URL: Source, https://github.com/Aurorax-own/confutilPPP
 Project-URL: Tracker, https://github.com/Aurorax-own/confutilPPP/issues
 Description-Content-Type: text/markdown
```

### Comparing `confutilPPP-1.1.1/README.md` & `confutilPPP-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `confutilPPP-1.1.1/confutilPPP.egg-info/PKG-INFO` & `confutilPPP-1.1.2/confutilPPP.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confutilPPP
-Version: 1.1.1
+Version: 1.1.2
 Summary: A simple configuration file tool
 Home-page: https://github.com/Aurorax-own/confutilPPP
 Author: Aurorax-own
 Author-email: 15047150695@163.com
 Project-URL: Source, https://github.com/Aurorax-own/confutilPPP
 Project-URL: Tracker, https://github.com/Aurorax-own/confutilPPP/issues
 Description-Content-Type: text/markdown
```

### Comparing `confutilPPP-1.1.1/setup.py` & `confutilPPP-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,14 @@
     author='Aurorax-own',
     author_email='15047150695@163.com',
     packages=find_packages('src'),
     package_dir={'confutilPPP': 'src/confutilPPP'},
     include_package_data=True,
     install_requires=[
         'PyYAML==6.0.1',
-        'logPPP==1.1.1'
+        'logPPP==1.1.2'
     ],
     project_urls={
         'Source': URL,
         'Tracker': f'{URL}/issues',
     },
 )
```

### Comparing `confutilPPP-1.1.1/src/confutilPPP/__confutil__.py` & `confutilPPP-1.1.2/src/confutilPPP/__confutil__.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         pass
 
     # 获取参数
     @staticmethod
     def _parse_arguments():
         parser = argparse.ArgumentParser()
         default_config_path = os.path.join(os.getcwd(), 'config.yaml')
-        parser.add_argument("--configpath", "-c", default=default_config_path, nargs=1, help="配置文件")
+        parser.add_argument("--configpath", "-c", default=[default_config_path], nargs=1, help="配置文件")
         return parser.parse_args()
 
     # 检查解析参数
     @staticmethod
     def check_config(_object=None, _filename='config'):
         try:
             # 解析参数
```

