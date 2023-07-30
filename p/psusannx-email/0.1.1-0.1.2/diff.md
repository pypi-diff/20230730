# Comparing `tmp/psusannx_email-0.1.1.tar.gz` & `tmp/psusannx_email-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psusannx_email-0.1.1.tar", last modified: Sun Jul 30 21:08:38 2023, max compression
+gzip compressed data, was "psusannx_email-0.1.2.tar", last modified: Sun Jul 30 21:21:19 2023, max compression
```

## Comparing `psusannx_email-0.1.1.tar` & `psusannx_email-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 21:08:38.384994 psusannx_email-0.1.1/
--rw-rw-rw-   0        0        0     1090 2022-03-24 22:10:42.000000 psusannx_email-0.1.1/LICENSE
--rw-rw-rw-   0        0        0       34 2022-03-24 22:10:55.000000 psusannx_email-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1734 2023-07-30 21:08:38.384994 psusannx_email-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1506 2023-07-30 20:29:02.000000 psusannx_email-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 21:08:38.366299 psusannx_email-0.1.1/psusannx_email/
--rw-rw-rw-   0        0        0       52 2022-03-24 22:03:52.000000 psusannx_email-0.1.1/psusannx_email/__init__.py
--rw-rw-rw-   0        0        0     1351 2023-07-30 20:04:57.000000 psusannx_email-0.1.1/psusannx_email/sendgrid_email.py
-drwxrwxrwx   0        0        0        0 2023-07-30 21:08:38.384994 psusannx_email-0.1.1/psusannx_email.egg-info/
--rw-rw-rw-   0        0        0     1734 2023-07-30 21:08:38.000000 psusannx_email-0.1.1/psusannx_email.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-07-30 21:08:38.000000 psusannx_email-0.1.1/psusannx_email.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 21:08:38.000000 psusannx_email-0.1.1/psusannx_email.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-30 21:08:38.000000 psusannx_email-0.1.1/psusannx_email.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-30 21:08:38.000000 psusannx_email-0.1.1/psusannx_email.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-30 21:08:38.384994 psusannx_email-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      685 2023-07-30 20:37:54.000000 psusannx_email-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:21:19.110248 psusannx_email-0.1.2/
+-rw-rw-rw-   0        0        0     1090 2022-03-24 22:10:42.000000 psusannx_email-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0       34 2022-03-24 22:10:55.000000 psusannx_email-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1734 2023-07-30 21:21:19.110248 psusannx_email-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1506 2023-07-30 20:29:02.000000 psusannx_email-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 21:21:19.088231 psusannx_email-0.1.2/psusannx_email/
+-rw-rw-rw-   0        0        0       52 2022-03-24 22:03:52.000000 psusannx_email-0.1.2/psusannx_email/__init__.py
+-rw-rw-rw-   0        0        0     1351 2023-07-30 20:04:57.000000 psusannx_email-0.1.2/psusannx_email/sendgrid_email.py
+drwxrwxrwx   0        0        0        0 2023-07-30 21:21:19.110248 psusannx_email-0.1.2/psusannx_email.egg-info/
+-rw-rw-rw-   0        0        0     1734 2023-07-30 21:21:18.000000 psusannx_email-0.1.2/psusannx_email.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-07-30 21:21:18.000000 psusannx_email-0.1.2/psusannx_email.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 21:21:18.000000 psusannx_email-0.1.2/psusannx_email.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-30 21:21:18.000000 psusannx_email-0.1.2/psusannx_email.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-30 21:21:18.000000 psusannx_email-0.1.2/psusannx_email.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 21:21:19.110248 psusannx_email-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      685 2023-07-30 21:17:49.000000 psusannx_email-0.1.2/setup.py
```

### Comparing `psusannx_email-0.1.1/LICENSE` & `psusannx_email-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `psusannx_email-0.1.1/PKG-INFO` & `psusannx_email-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psusannx_email
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package with a function for sending emails easily using sendgrid.
 Author: Jamie O'Brien
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # psusannx_email
```

### Comparing `psusannx_email-0.1.1/README.md` & `psusannx_email-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `psusannx_email-0.1.1/psusannx_email/sendgrid_email.py` & `psusannx_email-0.1.2/psusannx_email/sendgrid_email.py`

 * *Files identical despite different names*

### Comparing `psusannx_email-0.1.1/psusannx_email.egg-info/PKG-INFO` & `psusannx_email-0.1.2/psusannx_email.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psusannx-email
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package with a function for sending emails easily using sendgrid.
 Author: Jamie O'Brien
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # psusannx_email
```

### Comparing `psusannx_email-0.1.1/setup.py` & `psusannx_email-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 # Set up the package metadata
 setup(
     name="psusannx_email",
     author="Jamie O'Brien",
     description="A package with a function for sending emails easily using sendgrid.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.1.1",
+    version="0.1.2",
     packages=find_packages(include=["psusannx_email", "psusannx_email.*"]),
     install_requires=["sendgrid>=6.9.7"]
 )
```

