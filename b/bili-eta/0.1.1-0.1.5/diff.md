# Comparing `tmp/bili_eta-0.1.1.tar.gz` & `tmp/bili_eta-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bili_eta-0.1.1.tar", max compression
+gzip compressed data, was "bili_eta-0.1.5.tar", max compression
```

## Comparing `bili_eta-0.1.1.tar` & `bili_eta-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.1.1/bili_eta/__init__.py
--rw-r--r--   0        0        0      155 2023-07-30 08:32:48.386313 bili_eta-0.1.1/bili_eta/__main__.py
--rw-r--r--   0        0        0      368 2023-07-30 08:33:05.781659 bili_eta-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      375 1970-01-01 00:00:00.000000 bili_eta-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.1.5/bili_eta/__init__.py
+-rw-r--r--   0        0        0      922 2023-07-30 12:21:42.009481 bili_eta-0.1.5/bili_eta/__main__.py
+-rw-r--r--   0        0        0      421 2023-07-30 12:15:27.190137 bili_eta-0.1.5/bili_eta/bot.py
+-rw-r--r--   0        0        0      562 2023-07-30 12:24:49.289436 bili_eta-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      644 1970-01-01 00:00:00.000000 bili_eta-0.1.5/PKG-INFO
```

