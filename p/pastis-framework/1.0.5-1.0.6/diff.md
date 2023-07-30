# Comparing `tmp/pastis-framework-1.0.5.tar.gz` & `tmp/pastis-framework-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pastis-framework-1.0.5.tar", last modified: Sat Jul 29 12:43:01 2023, max compression
+gzip compressed data, was "pastis-framework-1.0.6.tar", last modified: Sun Jul 30 15:22:05 2023, max compression
```

## Comparing `pastis-framework-1.0.5.tar` & `pastis-framework-1.0.6.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.748172 pastis-framework-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-29 12:43:01.748172 pastis-framework-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.744172 pastis-framework-1.0.5/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)    16489 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/bin/pastis-benchmark
--rwxr-xr-x   0 runner    (1001) docker     (123)     5813 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/bin/pastis-broker
--rwxr-xr-x   0 runner    (1001) docker     (123)     2982 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/bin/pastisd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.740172 pastis-framework-1.0.5/engines/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.740172 pastis-framework-1.0.5/engines/pastis-aflpp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.744172 pastis-framework-1.0.5/engines/pastis-aflpp/bin/
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-aflpp/bin/pastis-aflpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.740172 pastis-framework-1.0.5/engines/pastis-aflpp/broker-addon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.744172 pastis-framework-1.0.5/engines/pastis-aflpp/broker-addon/aflppbroker/
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-aflpp/broker-addon/aflppbroker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.744172 pastis-framework-1.0.5/engines/pastis-aflpp/pastisaflpp/
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-aflpp/pastisaflpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-aflpp/pastisaflpp/aflpp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12716 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-aflpp/pastisaflpp/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-aflpp/pastisaflpp/replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-aflpp/pastisaflpp/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.740172 pastis-framework-1.0.5/engines/pastis-honggfuzz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.744172 pastis-framework-1.0.5/engines/pastis-honggfuzz/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4645 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-honggfuzz/bin/pastis-honggfuzz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.740172 pastis-framework-1.0.5/engines/pastis-honggfuzz/broker-addon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.744172 pastis-framework-1.0.5/engines/pastis-honggfuzz/broker-addon/hfbroker/
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-honggfuzz/broker-addon/hfbroker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.744172 pastis-framework-1.0.5/engines/pastis-honggfuzz/pastishf/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-honggfuzz/pastishf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-honggfuzz/pastishf/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-honggfuzz/pastishf/honggfuzz.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-honggfuzz/pastishf/replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-honggfuzz/pastishf/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.740172 pastis-framework-1.0.5/engines/pastis-triton/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.744172 pastis-framework-1.0.5/engines/pastis-triton/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10128 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-triton/bin/pastis-triton
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.740172 pastis-framework-1.0.5/engines/pastis-triton/broker-addon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.744172 pastis-framework-1.0.5/engines/pastis-triton/broker-addon/pastisttbroker/
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-triton/broker-addon/pastisttbroker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.744172 pastis-framework-1.0.5/engines/pastis-triton/pastisdse/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-triton/pastisdse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41039 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/engines/pastis-triton/pastisdse/pastisdse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.744172 pastis-framework-1.0.5/libpastis/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/libpastis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21929 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/libpastis/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/libpastis/enginedesc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/libpastis/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.744172 pastis-framework-1.0.5/libpastis/proto/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/libpastis/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/libpastis/proto/message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/libpastis/sast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/libpastis/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/libpastis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.744172 pastis-framework-1.0.5/pastis_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-29 12:43:01.000000 pastis-framework-1.0.5/pastis_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-29 12:43:01.000000 pastis-framework-1.0.5/pastis_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 12:43:01.000000 pastis-framework-1.0.5/pastis_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-29 12:43:01.000000 pastis-framework-1.0.5/pastis_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-29 12:43:01.000000 pastis-framework-1.0.5/pastis_framework.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.744172 pastis-framework-1.0.5/pastisbenchmark/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/pastisbenchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/pastisbenchmark/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    18707 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/pastisbenchmark/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/pastisbenchmark/replayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14349 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/pastisbenchmark/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:01.748172 pastis-framework-1.0.5/pastisbroker/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/pastisbroker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36051 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/pastisbroker/broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/pastisbroker/client.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10706 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/pastisbroker/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/pastisbroker/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/pastisbroker/stat_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/pastisbroker/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/pastisbroker/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 12:43:01.748172 pastis-framework-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-07-29 12:43:00.000000 pastis-framework-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.775405 pastis-framework-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-30 15:22:05.775405 pastis-framework-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.771404 pastis-framework-1.0.6/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16489 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/bin/pastis-benchmark
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5813 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/bin/pastis-broker
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2982 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/bin/pastisd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.771404 pastis-framework-1.0.6/engines/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.771404 pastis-framework-1.0.6/engines/pastis-aflpp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.771404 pastis-framework-1.0.6/engines/pastis-aflpp/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-aflpp/bin/pastis-aflpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.771404 pastis-framework-1.0.6/engines/pastis-aflpp/broker-addon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.771404 pastis-framework-1.0.6/engines/pastis-aflpp/broker-addon/aflppbroker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-aflpp/broker-addon/aflppbroker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.771404 pastis-framework-1.0.6/engines/pastis-aflpp/pastisaflpp/
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-aflpp/pastisaflpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-aflpp/pastisaflpp/aflpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12716 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-aflpp/pastisaflpp/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-aflpp/pastisaflpp/replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-aflpp/pastisaflpp/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.771404 pastis-framework-1.0.6/engines/pastis-honggfuzz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.771404 pastis-framework-1.0.6/engines/pastis-honggfuzz/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4645 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-honggfuzz/bin/pastis-honggfuzz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.771404 pastis-framework-1.0.6/engines/pastis-honggfuzz/broker-addon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.771404 pastis-framework-1.0.6/engines/pastis-honggfuzz/broker-addon/hfbroker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-honggfuzz/broker-addon/hfbroker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.771404 pastis-framework-1.0.6/engines/pastis-honggfuzz/pastishf/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-honggfuzz/pastishf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-honggfuzz/pastishf/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-honggfuzz/pastishf/honggfuzz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-honggfuzz/pastishf/replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-honggfuzz/pastishf/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.771404 pastis-framework-1.0.6/engines/pastis-triton/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.771404 pastis-framework-1.0.6/engines/pastis-triton/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10128 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-triton/bin/pastis-triton
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.771404 pastis-framework-1.0.6/engines/pastis-triton/broker-addon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.771404 pastis-framework-1.0.6/engines/pastis-triton/broker-addon/pastisttbroker/
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-triton/broker-addon/pastisttbroker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.771404 pastis-framework-1.0.6/engines/pastis-triton/pastisdse/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-triton/pastisdse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41039 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/engines/pastis-triton/pastisdse/pastisdse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.775405 pastis-framework-1.0.6/libpastis/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/libpastis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21929 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/libpastis/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/libpastis/enginedesc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/libpastis/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.775405 pastis-framework-1.0.6/libpastis/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/libpastis/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/libpastis/proto/message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/libpastis/sast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/libpastis/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/libpastis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.775405 pastis-framework-1.0.6/pastis_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-30 15:22:05.000000 pastis-framework-1.0.6/pastis_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-30 15:22:05.000000 pastis-framework-1.0.6/pastis_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 15:22:05.000000 pastis-framework-1.0.6/pastis_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-30 15:22:05.000000 pastis-framework-1.0.6/pastis_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-30 15:22:05.000000 pastis-framework-1.0.6/pastis_framework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.775405 pastis-framework-1.0.6/pastisbenchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/pastisbenchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/pastisbenchmark/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18707 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/pastisbenchmark/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/pastisbenchmark/replayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14349 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/pastisbenchmark/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:05.775405 pastis-framework-1.0.6/pastisbroker/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/pastisbroker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36053 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/pastisbroker/broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/pastisbroker/client.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10706 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/pastisbroker/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/pastisbroker/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/pastisbroker/stat_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/pastisbroker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/pastisbroker/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 15:22:05.775405 pastis-framework-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-07-30 15:22:03.000000 pastis-framework-1.0.6/setup.py
```

### Comparing `pastis-framework-1.0.5/LICENSE` & `pastis-framework-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/PKG-INFO` & `pastis-framework-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pastis-framework
-Version: 1.0.5
+Version: 1.0.6
 Summary: PASTIS framework for collaborative fuzzing
 Home-page: https://github.com/quarkslab/pastis
 Author: Quarkslab
 License: AGPL-3.0
 Project-URL: Documentation, https://quarkslab.github.io/pastis/
 Project-URL: Bug Tracker, https://github.com/quarkslab/pastis/issues
 Project-URL: Source, https://github.com/quarkslab/pastis
```

### Comparing `pastis-framework-1.0.5/README.md` & `pastis-framework-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/bin/pastis-benchmark` & `pastis-framework-1.0.6/bin/pastis-benchmark`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/bin/pastis-broker` & `pastis-framework-1.0.6/bin/pastis-broker`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/bin/pastisd` & `pastis-framework-1.0.6/bin/pastisd`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/engines/pastis-aflpp/bin/pastis-aflpp` & `pastis-framework-1.0.6/engines/pastis-aflpp/bin/pastis-aflpp`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/engines/pastis-aflpp/broker-addon/aflppbroker/__init__.py` & `pastis-framework-1.0.6/engines/pastis-aflpp/broker-addon/aflppbroker/__init__.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/engines/pastis-aflpp/pastisaflpp/__init__.py` & `pastis-framework-1.0.6/engines/pastis-aflpp/pastisaflpp/__init__.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/engines/pastis-aflpp/pastisaflpp/aflpp.py` & `pastis-framework-1.0.6/engines/pastis-aflpp/pastisaflpp/aflpp.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/engines/pastis-aflpp/pastisaflpp/driver.py` & `pastis-framework-1.0.6/engines/pastis-aflpp/pastisaflpp/driver.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/engines/pastis-aflpp/pastisaflpp/replay.py` & `pastis-framework-1.0.6/engines/pastis-aflpp/pastisaflpp/replay.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/engines/pastis-aflpp/pastisaflpp/workspace.py` & `pastis-framework-1.0.6/engines/pastis-aflpp/pastisaflpp/workspace.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/engines/pastis-honggfuzz/bin/pastis-honggfuzz` & `pastis-framework-1.0.6/engines/pastis-honggfuzz/bin/pastis-honggfuzz`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/engines/pastis-honggfuzz/broker-addon/hfbroker/__init__.py` & `pastis-framework-1.0.6/engines/pastis-honggfuzz/broker-addon/hfbroker/__init__.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/engines/pastis-honggfuzz/pastishf/__init__.py` & `pastis-framework-1.0.6/engines/pastis-honggfuzz/pastishf/__init__.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/engines/pastis-honggfuzz/pastishf/driver.py` & `pastis-framework-1.0.6/engines/pastis-honggfuzz/pastishf/driver.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/engines/pastis-honggfuzz/pastishf/honggfuzz.py` & `pastis-framework-1.0.6/engines/pastis-honggfuzz/pastishf/honggfuzz.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/engines/pastis-honggfuzz/pastishf/replay.py` & `pastis-framework-1.0.6/engines/pastis-honggfuzz/pastishf/replay.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/engines/pastis-honggfuzz/pastishf/workspace.py` & `pastis-framework-1.0.6/engines/pastis-honggfuzz/pastishf/workspace.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/engines/pastis-triton/bin/pastis-triton` & `pastis-framework-1.0.6/engines/pastis-triton/bin/pastis-triton`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/engines/pastis-triton/broker-addon/pastisttbroker/__init__.py` & `pastis-framework-1.0.6/engines/pastis-triton/broker-addon/pastisttbroker/__init__.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/engines/pastis-triton/pastisdse/pastisdse.py` & `pastis-framework-1.0.6/engines/pastis-triton/pastisdse/pastisdse.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/libpastis/agent.py` & `pastis-framework-1.0.6/libpastis/agent.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/libpastis/enginedesc.py` & `pastis-framework-1.0.6/libpastis/enginedesc.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/libpastis/package.py` & `pastis-framework-1.0.6/libpastis/package.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/libpastis/proto/message_pb2.py` & `pastis-framework-1.0.6/libpastis/proto/message_pb2.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/libpastis/sast.py` & `pastis-framework-1.0.6/libpastis/sast.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/libpastis/types.py` & `pastis-framework-1.0.6/libpastis/types.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/libpastis/utils.py` & `pastis-framework-1.0.6/libpastis/utils.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/pastis_framework.egg-info/PKG-INFO` & `pastis-framework-1.0.6/pastis_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pastis-framework
-Version: 1.0.5
+Version: 1.0.6
 Summary: PASTIS framework for collaborative fuzzing
 Home-page: https://github.com/quarkslab/pastis
 Author: Quarkslab
 License: AGPL-3.0
 Project-URL: Documentation, https://quarkslab.github.io/pastis/
 Project-URL: Bug Tracker, https://github.com/quarkslab/pastis/issues
 Project-URL: Source, https://github.com/quarkslab/pastis
```

### Comparing `pastis-framework-1.0.5/pastis_framework.egg-info/SOURCES.txt` & `pastis-framework-1.0.6/pastis_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/pastisbenchmark/models.py` & `pastis-framework-1.0.6/pastisbenchmark/models.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/pastisbenchmark/plotter.py` & `pastis-framework-1.0.6/pastisbenchmark/plotter.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/pastisbenchmark/replayer.py` & `pastis-framework-1.0.6/pastisbenchmark/replayer.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/pastisbenchmark/results.py` & `pastis-framework-1.0.6/pastisbenchmark/results.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/pastisbroker/broker.py` & `pastis-framework-1.0.6/pastisbroker/broker.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,28 +222,28 @@
         # Show log message and save seed to file
         self.statmanager.update_seed_stat(cli, typ)  # Add info only if new
         cli.log(LogLevel.INFO, f"seed {h} [{self._colored_seed_type(typ)}][{self._colored_seed_newness(is_new)}]")
         cli.add_own_seed(seed)  # Add seed in client's seed
         fname = self.write_seed(typ, cli.strid, seed) # Write seed to file
 
         if is_new:
-            self._seed_pool[seed] = typ  # Save it in the local pool
-
             if self._coverage_manager:
                 sp = fname.split("_")
                 covi = ClientInput(seed, "", f"{sp[0]}_{sp[1]}", sp[2], h, fname, typ, cli.netid, cli.strid, "GRANTED", "", -1, [])
                 self._coverage_manager.push_input(covi)
 
             if not self.filter_inputs:  # If seed are not filtered send it right away
                 self.seed_granted(cli.netid, typ, seed)
         else:
             logging.debug(f"receive duplicate seed {h} by {cli.strid}")
 
-
     def seed_granted(self, cli_id: bytes, typ: SeedType, seed: bytes):
+        # Save it in the local pool
+        self._seed_pool[seed] = typ
+
         # Iterate on all clients and send it to whomever never received it
         if self.broker_mode == BrokingMode.FULL:
             self.send_seed_to_all_others(cli_id, typ, seed)
 
         if self.is_proxied:  # Forward it to the proxy
             self._proxy.send_seed(typ, seed)
```

### Comparing `pastis-framework-1.0.5/pastisbroker/client.py` & `pastis-framework-1.0.6/pastisbroker/client.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/pastisbroker/coverage.py` & `pastis-framework-1.0.6/pastisbroker/coverage.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/pastisbroker/stat_manager.py` & `pastis-framework-1.0.6/pastisbroker/stat_manager.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/pastisbroker/utils.py` & `pastis-framework-1.0.6/pastisbroker/utils.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/pastisbroker/workspace.py` & `pastis-framework-1.0.6/pastisbroker/workspace.py`

 * *Files identical despite different names*

### Comparing `pastis-framework-1.0.5/setup.py` & `pastis-framework-1.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open("README.md") as f:
     lines = f.readlines()
     README = "\n".join(lines[4:7]+lines[51:])
 
 
 setup(
     name="pastis-framework",
-    version="1.0.5",
+    version="1.0.6",
     description="PASTIS framework for collaborative fuzzing",
     long_description=README,
     long_description_content_type='text/markdown',
     packages=[
         "libpastis",
         "libpastis.proto",
         "pastisbroker",
```

