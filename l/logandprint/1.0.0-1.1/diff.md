# Comparing `tmp/logandprint-1.0.0.tar.gz` & `tmp/logandprint-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logandprint-1.0.0.tar", last modified: Sun Jul  3 03:04:48 2022, max compression
+gzip compressed data, was "logandprint-1.1.tar", last modified: Sun Jul 30 19:56:16 2023, max compression
```

## Comparing `logandprint-1.0.0.tar` & `logandprint-1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2022-07-03 03:04:48.562976 logandprint-1.0.0/
--rw-rw-rw-   0        0        0     1094 2022-07-02 19:59:22.000000 logandprint-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2247 2022-07-03 03:04:48.562976 logandprint-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-07-03 03:04:48.546983 logandprint-1.0.0/logandprint/
--rw-rw-rw-   0        0        0       56 2022-07-03 02:16:50.000000 logandprint-1.0.0/logandprint/__init__.py
--rw-rw-rw-   0        0        0     3158 2022-07-03 02:15:58.000000 logandprint-1.0.0/logandprint/main.py
-drwxrwxrwx   0        0        0        0 2022-07-03 03:04:48.562976 logandprint-1.0.0/logandprint.egg-info/
--rw-rw-rw-   0        0        0     2247 2022-07-03 03:04:48.000000 logandprint-1.0.0/logandprint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2022-07-03 03:04:48.000000 logandprint-1.0.0/logandprint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-03 03:04:48.000000 logandprint-1.0.0/logandprint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2022-07-03 03:04:48.000000 logandprint-1.0.0/logandprint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-07-03 03:04:48.562976 logandprint-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1156 2022-07-03 03:04:13.000000 logandprint-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:56:16.425874 logandprint-1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-30 19:56:04.000000 logandprint-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-30 19:56:16.425874 logandprint-1.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:56:16.421874 logandprint-1.1/logandprint/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-30 19:56:04.000000 logandprint-1.1/logandprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-07-30 19:56:04.000000 logandprint-1.1/logandprint/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:56:16.425874 logandprint-1.1/logandprint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-30 19:56:16.000000 logandprint-1.1/logandprint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-30 19:56:16.000000 logandprint-1.1/logandprint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 19:56:16.000000 logandprint-1.1/logandprint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-30 19:56:16.000000 logandprint-1.1/logandprint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 19:56:16.425874 logandprint-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-30 19:56:04.000000 logandprint-1.1/setup.py
```

### Comparing `logandprint-1.0.0/LICENSE` & `logandprint-1.1/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Guilherme Saldanha
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2022 Guilherme Saldanha
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

