# Comparing `tmp/settus-0.0.1.tar.gz` & `tmp/settus-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "settus-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "settus-0.0.2.tar", last modified: Sun Jul 30 06:43:53 2023, max compression
```

## Comparing `settus-0.0.1.tar` & `settus-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,26 @@
--rw-r--r--   0        0        0      710 2023-07-16 07:23:49.336724 settus-0.0.1/.github/workflows/release.yml
--rw-r--r--   0        0        0      720 2023-07-16 07:23:49.336724 settus-0.0.1/.github/workflows/test.yml
--rw-r--r--   0        0        0     1319 2023-07-16 07:23:49.336724 settus-0.0.1/.gitignore
--rw-r--r--   0        0        0       76 2023-07-16 07:23:49.336724 settus-0.0.1/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-07-16 07:23:49.336724 settus-0.0.1/LICENSE
--rw-r--r--   0        0        0      228 2023-07-16 07:23:49.336724 settus-0.0.1/Makefile
--rw-r--r--   0        0        0       85 2023-07-16 07:23:49.336724 settus-0.0.1/README.md
--rw-r--r--   0        0        0      890 2023-07-16 07:23:49.336724 settus-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      928 2023-07-16 07:23:49.336724 settus-0.0.1/settus/__init__.py
--rw-r--r--   0        0        0       18 2023-07-16 07:23:49.336724 settus-0.0.1/settus/_version.py
--rw-r--r--   0        0        0      107 2023-07-16 07:23:49.336724 settus-0.0.1/settus/basesettings.py
--rw-r--r--   0        0        0        0 2023-07-16 07:23:49.336724 settus-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      324 2023-07-16 07:23:49.336724 settus-0.0.1/tests/test_basesettings.py
--rw-r--r--   0        0        0      938 1970-01-01 00:00:00.000000 settus-0.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:43:53.614146 settus-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:43:53.614146 settus-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:43:53.614146 settus-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-30 06:43:39.000000 settus-0.0.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-30 06:43:39.000000 settus-0.0.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-30 06:43:39.000000 settus-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-30 06:43:39.000000 settus-0.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-30 06:43:39.000000 settus-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-30 06:43:39.000000 settus-0.0.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-30 06:43:53.614146 settus-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-30 06:43:39.000000 settus-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-30 06:43:39.000000 settus-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:43:53.614146 settus-0.0.2/settus/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-30 06:43:39.000000 settus-0.0.2/settus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-30 06:43:39.000000 settus-0.0.2/settus/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-30 06:43:39.000000 settus-0.0.2/settus/basesettings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:43:53.614146 settus-0.0.2/settus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-30 06:43:53.000000 settus-0.0.2/settus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-30 06:43:53.000000 settus-0.0.2/settus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 06:43:53.000000 settus-0.0.2/settus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-30 06:43:53.000000 settus-0.0.2/settus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-30 06:43:53.000000 settus-0.0.2/settus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 06:43:53.614146 settus-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:43:53.614146 settus-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 06:43:39.000000 settus-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-30 06:43:39.000000 settus-0.0.2/tests/test_basesettings.py
```

### Comparing `settus-0.0.1/.github/workflows/test.yml` & `settus-0.0.2/.github/workflows/test.yml`

 * *Files 26% similar despite different names*

```diff
@@ -26,15 +26,12 @@
 #      - name: Unshallow
 #        run: git fetch --prune --unshallow
 
       - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.pyVersion }}
 
-      - name: Install flit
-        run: pip install flit
-
       - name: Run tests
-        run: make dev install test
+        run: make dev test
 
 #      - name: Publish test coverage
 #        uses: codecov/codecov-action@v1
```

### Comparing `settus-0.0.1/.gitignore` & `settus-0.0.2/.gitignore`

 * *Files 14% similar despite different names*

```diff
@@ -13,19 +13,20 @@
 # PyCharm configuration
 **/.idea/**
 
 # Local settings and environment variables
 #settings_local/*.*
 
 # --------------------------------------------------------------------------- #
-# Installation                                                                #
+# Installation and build                                                      #
 # --------------------------------------------------------------------------- #
 
 #**/*.egg-info/**
 dist
+build
 #**/dist/**
 
 # --------------------------------------------------------------------------- #
 # Testing and coverage                                                        #
 # --------------------------------------------------------------------------- #
 
 # Coverage
```

### Comparing `settus-0.0.1/LICENSE` & `settus-0.0.2/LICENSE`

 * *Files identical despite different names*

