# Comparing `tmp/okserve-0.1.0.tar.gz` & `tmp/okserve-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okserve-0.1.0.tar", max compression
+gzip compressed data, was "okserve-0.1.1.tar", max compression
```

## Comparing `okserve-0.1.0.tar` & `okserve-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35149 2023-07-23 17:32:24.517774 okserve-0.1.0/LICENSE
--rw-r--r--   0        0        0        9 2023-07-23 17:34:37.820409 okserve-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-23 17:32:47.811694 okserve-0.1.0/okserve/__init__.py
--rw-r--r--   0        0        0      263 2023-07-23 17:39:42.980291 okserve-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      291 1970-01-01 00:00:00.000000 okserve-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-23 17:32:24.517774 okserve-0.1.1/LICENSE
+-rw-r--r--   0        0        0        9 2023-07-30 20:12:10.932812 okserve-0.1.1/README.md
+-rw-r--r--   0        0        0       81 2023-07-30 19:38:33.259104 okserve-0.1.1/okserve/__init__.py
+-rw-r--r--   0        0        0      375 2023-07-30 19:57:41.945351 okserve-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      335 1970-01-01 00:00:00.000000 okserve-0.1.1/PKG-INFO
```

### Comparing `okserve-0.1.0/LICENSE` & `okserve-0.1.1/LICENSE`

 * *Files identical despite different names*

