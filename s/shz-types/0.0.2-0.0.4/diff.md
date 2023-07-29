# Comparing `tmp/shz_types-0.0.2.tar.gz` & `tmp/shz_types-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shz_types-0.0.2.tar", last modified: Fri Jul 28 02:16:38 2023, max compression
+gzip compressed data, was "shz_types-0.0.4.tar", last modified: Sat Jul 29 22:25:31 2023, max compression
```

## Comparing `shz_types-0.0.2.tar` & `shz_types-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 02:16:38.690714 shz_types-0.0.2/
--rw-rw-rw-   0        0        0     1078 2023-07-25 13:56:48.000000 shz_types-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      285 2023-07-28 02:16:38.690714 shz_types-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-25 13:57:15.000000 shz_types-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-28 02:16:38.691804 shz_types-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      564 2023-07-28 02:16:29.000000 shz_types-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-28 02:16:38.672319 shz_types-0.0.2/shz_types/
--rw-rw-rw-   0        0        0        0 2023-07-27 14:18:08.000000 shz_types-0.0.2/shz_types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 02:16:38.690714 shz_types-0.0.2/shz_types/datasets/
--rw-rw-rw-   0        0        0       25 2023-07-27 14:43:20.000000 shz_types-0.0.2/shz_types/datasets/__init__.py
--rw-rw-rw-   0        0        0      148 2023-07-27 14:39:45.000000 shz_types-0.0.2/shz_types/datasets/anyDataset.py
-drwxrwxrwx   0        0        0        0 2023-07-28 02:16:38.689703 shz_types-0.0.2/shz_types.egg-info/
--rw-rw-rw-   0        0        0      285 2023-07-28 02:16:38.000000 shz_types-0.0.2/shz_types.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-07-28 02:16:38.000000 shz_types-0.0.2/shz_types.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 02:16:38.000000 shz_types-0.0.2/shz_types.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-07-28 02:16:38.000000 shz_types-0.0.2/shz_types.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-28 02:16:38.000000 shz_types-0.0.2/shz_types.egg-info/top_level.txt
+drwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-29 22:25:31.629573 shz_types-0.0.4/
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)     1078 2023-07-29 22:22:39.000000 shz_types-0.0.4/LICENSE
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      275 2023-07-29 22:25:31.629245 shz_types-0.0.4/PKG-INFO
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-29 22:22:39.000000 shz_types-0.0.4/README.md
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)       38 2023-07-29 22:25:31.629687 shz_types-0.0.4/setup.cfg
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      564 2023-07-29 22:23:15.000000 shz_types-0.0.4/setup.py
+drwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-29 22:25:31.625810 shz_types-0.0.4/shz_types/
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)       65 2023-07-29 22:22:39.000000 shz_types-0.0.4/shz_types/__init__.py
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      148 2023-07-29 22:22:39.000000 shz_types-0.0.4/shz_types/anyDataset.py
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)       55 2023-07-29 22:22:39.000000 shz_types-0.0.4/shz_types/numbers.py
+drwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-29 22:25:31.628589 shz_types-0.0.4/shz_types.egg-info/
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      275 2023-07-29 22:25:31.000000 shz_types-0.0.4/shz_types.egg-info/PKG-INFO
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      257 2023-07-29 22:25:31.000000 shz_types-0.0.4/shz_types.egg-info/SOURCES.txt
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        1 2023-07-29 22:25:31.000000 shz_types-0.0.4/shz_types.egg-info/dependency_links.txt
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)       28 2023-07-29 22:25:31.000000 shz_types-0.0.4/shz_types.egg-info/requires.txt
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)       10 2023-07-29 22:25:31.000000 shz_types-0.0.4/shz_types.egg-info/top_level.txt
```

### Comparing `shz_types-0.0.2/LICENSE` & `shz_types-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `shz_types-0.0.2/setup.py` & `shz_types-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 project_name = 'shz_types'
 
 setup(name=project_name,
-      version='0.0.2',
+      version='0.0.4',
       license='MIT License',
       author='Eliseu Brito',
       long_description=readme,
       long_description_content_type="text/markdown",
       author_email='eliseubrito776@gmail.com',
       keywords='shz types shztypes shz_types',
       description=u'Personal types for my projects',
```

