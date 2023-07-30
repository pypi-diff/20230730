# Comparing `tmp/bili_eta-0.1.0.tar.gz` & `tmp/bili_eta-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bili_eta-0.1.0.tar", max compression
+gzip compressed data, was "bili_eta-0.1.1.tar", max compression
```

## Comparing `bili_eta-0.1.0.tar` & `bili_eta-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.1.0/bili_eta/__init__.py
--rw-r--r--   0        0        0      116 2023-07-30 08:28:36.477468 bili_eta-0.1.0/bili_eta/__main__.py
--rw-r--r--   0        0        0      368 2023-07-30 08:26:00.642469 bili_eta-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      375 1970-01-01 00:00:00.000000 bili_eta-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.1.1/bili_eta/__init__.py
+-rw-r--r--   0        0        0      155 2023-07-30 08:32:48.386313 bili_eta-0.1.1/bili_eta/__main__.py
+-rw-r--r--   0        0        0      368 2023-07-30 08:33:05.781659 bili_eta-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      375 1970-01-01 00:00:00.000000 bili_eta-0.1.1/PKG-INFO
```

