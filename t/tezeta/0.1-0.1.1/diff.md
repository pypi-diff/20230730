# Comparing `tmp/tezeta-0.1.tar.gz` & `tmp/tezeta-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tezeta-0.1.tar", last modified: Sun Jul 30 07:55:36 2023, max compression
+gzip compressed data, was "tezeta-0.1.1.tar", last modified: Sun Jul 30 08:16:22 2023, max compression
```

## Comparing `tezeta-0.1.tar` & `tezeta-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 07:55:36.940434 tezeta-0.1/
--rw-rw-rw-   0        0        0     1091 2023-07-28 02:40:23.000000 tezeta-0.1/LICENSE
--rw-rw-rw-   0        0        0      930 2023-07-30 07:55:36.939433 tezeta-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2255 2023-07-30 07:51:09.000000 tezeta-0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-30 07:55:36.940434 tezeta-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1157 2023-07-30 07:46:39.000000 tezeta-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-30 07:55:36.912428 tezeta-0.1/tezeta/
--rw-rw-rw-   0        0        0     1188 2023-07-30 07:34:17.000000 tezeta-0.1/tezeta/__init__.py
--rw-rw-rw-   0        0        0     3608 2023-07-30 07:42:14.000000 tezeta-0.1/tezeta/chats.py
--rw-rw-rw-   0        0        0       30 2023-07-28 02:33:24.000000 tezeta-0.1/tezeta/text.py
--rw-rw-rw-   0        0        0      587 2023-07-30 07:33:45.000000 tezeta-0.1/tezeta/tokens.py
-drwxrwxrwx   0        0        0        0 2023-07-30 07:55:36.938433 tezeta-0.1/tezeta.egg-info/
--rw-rw-rw-   0        0        0      930 2023-07-30 07:55:36.000000 tezeta-0.1/tezeta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-07-30 07:55:36.000000 tezeta-0.1/tezeta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 07:55:36.000000 tezeta-0.1/tezeta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-07-30 07:55:36.000000 tezeta-0.1/tezeta.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-30 07:55:36.000000 tezeta-0.1/tezeta.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 08:16:22.492894 tezeta-0.1.1/
+-rw-rw-rw-   0        0        0     1091 2023-07-28 02:40:23.000000 tezeta-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3232 2023-07-30 08:16:22.491894 tezeta-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2255 2023-07-30 07:51:09.000000 tezeta-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-30 08:16:22.492894 tezeta-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1380 2023-07-30 08:16:03.000000 tezeta-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 08:16:22.476890 tezeta-0.1.1/tezeta/
+-rw-rw-rw-   0        0        0     1188 2023-07-30 07:34:17.000000 tezeta-0.1.1/tezeta/__init__.py
+-rw-rw-rw-   0        0        0     3608 2023-07-30 07:42:14.000000 tezeta-0.1.1/tezeta/chats.py
+-rw-rw-rw-   0        0        0       30 2023-07-28 02:33:24.000000 tezeta-0.1.1/tezeta/text.py
+-rw-rw-rw-   0        0        0      587 2023-07-30 07:33:45.000000 tezeta-0.1.1/tezeta/tokens.py
+drwxrwxrwx   0        0        0        0 2023-07-30 08:16:22.490893 tezeta-0.1.1/tezeta.egg-info/
+-rw-rw-rw-   0        0        0     3232 2023-07-30 08:16:22.000000 tezeta-0.1.1/tezeta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-07-30 08:16:22.000000 tezeta-0.1.1/tezeta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 08:16:22.000000 tezeta-0.1.1/tezeta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-30 08:16:22.000000 tezeta-0.1.1/tezeta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-30 08:16:22.000000 tezeta-0.1.1/tezeta.egg-info/top_level.txt
```

### Comparing `tezeta-0.1/LICENSE` & `tezeta-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tezeta-0.1/README.md` & `tezeta-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tezeta-0.1/setup.py` & `tezeta-0.1.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from setuptools import setup, find_packages
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='tezeta',
-    version='0.1',
+    version='0.1.1',
     packages=find_packages(),
     description='A package for memory in chatbots and LLM requests that uses relevance to maximize context window utilization.',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     author='Rediat Shamsu',
     author_email='rediatbrook@gmail.com',
     url='https://github.com/rediatbrook/tezeta',
     classifiers=[
         'Development Status :: 1 - Planning',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
```

### Comparing `tezeta-0.1/tezeta/__init__.py` & `tezeta-0.1.1/tezeta/__init__.py`

 * *Files identical despite different names*

### Comparing `tezeta-0.1/tezeta/chats.py` & `tezeta-0.1.1/tezeta/chats.py`

 * *Files identical despite different names*

### Comparing `tezeta-0.1/tezeta/tokens.py` & `tezeta-0.1.1/tezeta/tokens.py`

 * *Files identical despite different names*

