# Comparing `tmp/diagnostic-1.0.0.tar.gz` & `tmp/diagnostic-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diagnostic-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "diagnostic-1.0.1.tar", last modified: Sun Jul 30 15:47:22 2023, max compression
```

## Comparing `diagnostic-1.0.0.tar` & `diagnostic-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1080 2023-07-28 11:21:27.518573 diagnostic-1.0.0/LICENSE
--rw-r--r--   0        0        0     1214 2023-07-28 11:21:27.523451 diagnostic-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      288 2023-07-28 11:24:13.694905 diagnostic-1.0.0/src/diagnostic/__init__.py
--rw-r--r--   0        0        0     8974 2023-07-28 11:21:27.524003 diagnostic-1.0.0/src/diagnostic/_base.py
--rw-r--r--   0        0        0     7306 2023-07-28 11:21:27.524238 diagnostic-1.0.0/src/diagnostic/_check_docs.py
--rw-r--r--   0        0        0     1110 2023-07-28 11:21:27.524423 diagnostic-1.0.0/src/diagnostic/_concrete.py
--rw-r--r--   0        0        0     7283 2023-07-28 11:21:27.524647 diagnostic-1.0.0/src/diagnostic/_parsers.py
--rw-r--r--   0        0        0      174 2023-07-28 11:21:27.524848 diagnostic-1.0.0/src/diagnostic/check-docs.py
--rw-r--r--   0        0        0     1014 1970-01-01 00:00:00.000000 diagnostic-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-07-30 15:47:22.000000 diagnostic-1.0.1/LICENSE
+-rw-r--r--   0        0        0      911 2023-07-30 15:47:22.000000 diagnostic-1.0.1/README.md
+-rw-r--r--   0        0        0     1235 2023-07-30 15:47:22.000000 diagnostic-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      288 2023-07-30 15:47:22.000000 diagnostic-1.0.1/src/diagnostic/__init__.py
+-rw-r--r--   0        0        0     8974 2023-07-30 15:47:22.000000 diagnostic-1.0.1/src/diagnostic/_base.py
+-rw-r--r--   0        0        0     7306 2023-07-30 15:47:22.000000 diagnostic-1.0.1/src/diagnostic/_check_docs.py
+-rw-r--r--   0        0        0     1110 2023-07-30 15:47:22.000000 diagnostic-1.0.1/src/diagnostic/_concrete.py
+-rw-r--r--   0        0        0     7283 2023-07-30 15:47:22.000000 diagnostic-1.0.1/src/diagnostic/_parsers.py
+-rw-r--r--   0        0        0      174 2023-07-30 15:47:22.000000 diagnostic-1.0.1/src/diagnostic/check-docs.py
+-rw-r--r--   0        0        0     1967 1970-01-01 00:00:00.000000 diagnostic-1.0.1/PKG-INFO
```

### Comparing `diagnostic-1.0.0/LICENSE` & `diagnostic-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `diagnostic-1.0.0/pyproject.toml` & `diagnostic-1.0.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     "rich",
     "markdown-it-py",
     "typing_extensions; python_version < '3.10'",
     "docutils",
 ]
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
+readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: Implementation :: CPython",
```

### Comparing `diagnostic-1.0.0/src/diagnostic/_base.py` & `diagnostic-1.0.1/src/diagnostic/_base.py`

 * *Files identical despite different names*

### Comparing `diagnostic-1.0.0/src/diagnostic/_check_docs.py` & `diagnostic-1.0.1/src/diagnostic/_check_docs.py`

 * *Files identical despite different names*

### Comparing `diagnostic-1.0.0/src/diagnostic/_concrete.py` & `diagnostic-1.0.1/src/diagnostic/_concrete.py`

 * *Files identical despite different names*

### Comparing `diagnostic-1.0.0/src/diagnostic/_parsers.py` & `diagnostic-1.0.1/src/diagnostic/_parsers.py`

 * *Files identical despite different names*

