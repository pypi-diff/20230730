# Comparing `tmp/examon_beginners_package-0.0.9.tar.gz` & `tmp/examon_beginners_package-0.1.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "examon_beginners_package-0.0.9.tar", max compression
+gzip compressed data, was "examon_beginners_package-0.1.11.tar", max compression
```

## Comparing `examon_beginners_package-0.0.9.tar` & `examon_beginners_package-0.1.11.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       24 2023-07-16 20:33:56.622876 examon_beginners_package-0.0.9/examon_beginners_package/__init__.py
--rw-r--r--   0        0        0     1573 2023-07-18 20:43:28.888259 examon_beginners_package-0.0.9/examon_beginners_package/beginners.py
--rw-r--r--   0        0        0      338 2023-07-21 22:00:34.115561 examon_beginners_package-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      399 1970-01-01 00:00:00.000000 examon_beginners_package-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0       24 2023-07-16 20:33:56.622876 examon_beginners_package-0.1.11/examon_beginners_package/__init__.py
+-rw-r--r--   0        0        0     1573 2023-07-18 20:43:28.888259 examon_beginners_package-0.1.11/examon_beginners_package/beginners.py
+-rw-r--r--   0        0        0      339 2023-07-30 19:30:35.730223 examon_beginners_package-0.1.11/pyproject.toml
+-rw-r--r--   0        0        0      400 1970-01-01 00:00:00.000000 examon_beginners_package-0.1.11/PKG-INFO
```

### Comparing `examon_beginners_package-0.0.9/examon_beginners_package/beginners.py` & `examon_beginners_package-0.1.11/examon_beginners_package/beginners.py`

 * *Files identical despite different names*

