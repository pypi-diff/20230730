# Comparing `tmp/scrapli_cfg-2023.1.30.tar.gz` & `tmp/scrapli_cfg-2023.7.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapli_cfg-2023.1.30.tar", last modified: Sat Jan 28 19:37:46 2023, max compression
+gzip compressed data, was "scrapli_cfg-2023.7.30.tar", last modified: Sun Jul 30 17:18:16 2023, max compression
```

## Comparing `scrapli_cfg-2023.1.30.tar` & `scrapli_cfg-2023.7.30.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 19:37:46.007292 scrapli_cfg-2023.1.30/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-01-28 19:37:46.007292 scrapli_cfg-2023.1.30/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/requirements-asyncssh.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/requirements-paramiko.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/requirements-ssh2.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 19:37:45.995292 scrapli_cfg-2023.1.30/scrapli_cfg/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 19:37:45.995292 scrapli_cfg-2023.1.30/scrapli_cfg/platform/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/platform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 19:37:45.999292 scrapli_cfg-2023.1.30/scrapli_cfg/platform/base/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/platform/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10387 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/platform/base/async_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)    18882 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/platform/base/base_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/platform/base/sync_platform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 19:37:45.999292 scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 19:37:45.999292 scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/arista_eos/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/arista_eos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11057 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/arista_eos/async_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/arista_eos/base_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/arista_eos/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)    10870 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/arista_eos/sync_platform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 19:37:46.003292 scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/cisco_iosxe/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/cisco_iosxe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12759 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/cisco_iosxe/async_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/cisco_iosxe/base_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/cisco_iosxe/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/cisco_iosxe/sync_platform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 19:37:46.003292 scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/cisco_iosxr/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/cisco_iosxr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/cisco_iosxr/async_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/cisco_iosxr/base_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/cisco_iosxr/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/cisco_iosxr/sync_platform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 19:37:46.003292 scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/cisco_nxos/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/cisco_nxos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/cisco_nxos/async_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/cisco_nxos/base_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/cisco_nxos/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/cisco_nxos/sync_platform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 19:37:46.007292 scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/juniper_junos/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/juniper_junos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/juniper_junos/async_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/juniper_junos/base_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/juniper_junos/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/juniper_junos/sync_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-01-28 19:37:28.000000 scrapli_cfg-2023.1.30/scrapli_cfg/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 19:37:45.995292 scrapli_cfg-2023.1.30/scrapli_cfg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-01-28 19:37:45.000000 scrapli_cfg-2023.1.30/scrapli_cfg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-01-28 19:37:45.000000 scrapli_cfg-2023.1.30/scrapli_cfg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-28 19:37:45.000000 scrapli_cfg-2023.1.30/scrapli_cfg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-01-28 19:37:45.000000 scrapli_cfg-2023.1.30/scrapli_cfg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-28 19:37:45.000000 scrapli_cfg-2023.1.30/scrapli_cfg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-01-28 19:37:46.007292 scrapli_cfg-2023.1.30/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:18:16.707470 scrapli_cfg-2023.7.30/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-30 17:18:16.707470 scrapli_cfg-2023.7.30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/requirements-asyncssh.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/requirements-paramiko.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/requirements-ssh2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:18:16.699469 scrapli_cfg-2023.7.30/scrapli_cfg/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:18:16.699469 scrapli_cfg-2023.7.30/scrapli_cfg/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/platform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:18:16.699469 scrapli_cfg-2023.7.30/scrapli_cfg/platform/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/platform/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10387 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/platform/base/async_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18882 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/platform/base/base_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/platform/base/sync_platform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:18:16.699469 scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:18:16.699469 scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/arista_eos/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/arista_eos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11057 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/arista_eos/async_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/arista_eos/base_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/arista_eos/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10870 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/arista_eos/sync_platform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:18:16.703469 scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/cisco_iosxe/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/cisco_iosxe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12759 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/cisco_iosxe/async_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/cisco_iosxe/base_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/cisco_iosxe/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/cisco_iosxe/sync_platform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:18:16.703469 scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/cisco_iosxr/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/cisco_iosxr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/cisco_iosxr/async_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/cisco_iosxr/base_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/cisco_iosxr/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/cisco_iosxr/sync_platform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:18:16.703469 scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/cisco_nxos/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/cisco_nxos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/cisco_nxos/async_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/cisco_nxos/base_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/cisco_nxos/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/cisco_nxos/sync_platform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:18:16.707470 scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/juniper_junos/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/juniper_junos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/juniper_junos/async_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/juniper_junos/base_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/juniper_junos/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/juniper_junos/sync_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-07-30 17:17:59.000000 scrapli_cfg-2023.7.30/scrapli_cfg/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:18:16.699469 scrapli_cfg-2023.7.30/scrapli_cfg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-30 17:18:16.000000 scrapli_cfg-2023.7.30/scrapli_cfg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-30 17:18:16.000000 scrapli_cfg-2023.7.30/scrapli_cfg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 17:18:16.000000 scrapli_cfg-2023.7.30/scrapli_cfg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-30 17:18:16.000000 scrapli_cfg-2023.7.30/scrapli_cfg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-30 17:18:16.000000 scrapli_cfg-2023.7.30/scrapli_cfg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-30 17:18:16.707470 scrapli_cfg-2023.7.30/setup.cfg
```

### Comparing `scrapli_cfg-2023.1.30/LICENSE` & `scrapli_cfg-2023.7.30/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapli_cfg-2023.1.30/PKG-INFO` & `scrapli_cfg-2023.7.30/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapli_cfg
-Version: 2023.1.30
+Version: 2023.7.30
 Summary: Network device configuration management with scrapli
 Author-email: Carl Montanari <carl.r.montanari@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Carl Montanari
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,18 +21,18 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.com/scrapli/scrapli_cfg
 Project-URL: Changelog, https://scrapli.github.io/scrapli_cfg/changelog/
 Project-URL: Docs, https://scrapli.github.io/scrapli_cfg/
-Keywords: ssh,telnet,netconf,automation,network,cisco,iosxr,iosxe,nxos,arista,eos,juniper,junos
+Project-URL: Homepage, https://github.com/scrapli/scrapli_cfg
+Keywords: arista,automation,cisco,eos,iosxe,iosxr,juniper,junos,netconf,network,nxos,ssh,telnet
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scrapli_cfg Version: 2023.1.30 Summary: Network
+Metadata-Version: 2.1 Name: scrapli_cfg Version: 2023.7.30 Summary: Network
 device configuration management with scrapli Author-email: Carl Montanari
 r.montanari@gmail.com> License: MIT License Copyright (c) 2021 Carl Montanari
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
@@ -10,18 +10,19 @@
 permission notice shall be included in all copies or substantial portions of
 the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
 EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
 OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://github.com/scrapli/
-scrapli_cfg Project-URL: Changelog, https://scrapli.github.io/scrapli_cfg/
-changelog/ Project-URL: Docs, https://scrapli.github.io/scrapli_cfg/ Keywords:
-ssh,telnet,netconf,automation,network,cisco,iosxr,iosxe,nxos,arista,eos,juniper,junos
+DEALINGS IN THE SOFTWARE. Project-URL: Changelog, https://scrapli.github.io/
+scrapli_cfg/changelog/ Project-URL: Docs, https://scrapli.github.io/
+scrapli_cfg/ Project-URL: Homepage, https://github.com/scrapli/scrapli_cfg
+Keywords:
+arista,automation,cisco,eos,iosxe,iosxr,juniper,junos,netconf,network,nxos,ssh,telnet
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: POSIX :: Linux Classifier: Operating System :: MacOS Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Topic :: Software Development ::
```

### Comparing `scrapli_cfg-2023.1.30/README.md` & `scrapli_cfg-2023.7.30/README.md`

 * *Files identical despite different names*

### Comparing `scrapli_cfg-2023.1.30/pyproject.toml` & `scrapli_cfg-2023.7.30/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,58 +1,60 @@
 [build-system]
-requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
+requires = [
+  "setuptools",
+  "wheel",
+]
 
 [project]
 name = "scrapli_cfg"
-dynamic = [
-    "version",
-    "dependencies",
-    "optional-dependencies",
-]
 description = "Network device configuration management with scrapli"
 readme = "README.md"
+keywords = [
+  "arista",
+  "automation",
+  "cisco",
+  "eos",
+  "iosxe",
+  "iosxr",
+  "juniper",
+  "junos",
+  "netconf",
+  "network",
+  "nxos",
+  "ssh",
+  "telnet",
+]
 license = { file = "LICENSE" }
-requires-python = ">=3.7"
 authors = [
     { name = "Carl Montanari", email = "carl.r.montanari@gmail.com" },
 ]
+requires-python = ">=3.7"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-keywords = [
-    "ssh",
-    "telnet",
-    "netconf",
-    "automation",
-    "network",
-    "cisco",
-    "iosxr",
-    "iosxe",
-    "nxos",
-    "arista",
-    "eos",
-    "juniper",
-    "junos",
+dynamic = [
+  "dependencies",
+  "optional-dependencies",
+  "version",
 ]
-
 [project.urls]
-Homepage = "https://github.com/scrapli/scrapli_cfg"
 Changelog = "https://scrapli.github.io/scrapli_cfg/changelog/"
 Docs = "https://scrapli.github.io/scrapli_cfg/"
+Homepage = "https://github.com/scrapli/scrapli_cfg"
 
 [tool.setuptools.dynamic]
 version = { attr = "scrapli_cfg.__version__" }
 dependencies = { file = "requirements.txt" }
 optional-dependencies.dev = { file = [
     "requirements-dev.txt",
     "requirements-paramiko.txt",
@@ -65,29 +67,46 @@
 optional-dependencies.asyncssh = { file = "requirements-asyncssh.txt" }
 
 [tool.setuptools.package-data]
 scrapli_cfg = [
     "py.typed"
 ]
 
+[tool.black]
+line-length = 100
+target-version = [
+    "py311",
+]
+
+[tool.isort]
+profile = "black"
+line_length = 100
+multi_line_output = 3
+include_trailing_comma = true
+known_first_party = "scrapli"
+known_third_party = "asyncssh,pytest"
+[tool.pytest.ini_options]
+asyncio_mode = "auto"
+
 [tool.coverage.run]
 source = [
     "scrapli_cfg/"
 ]
 
 [tool.coverage.report]
 sort = "cover"
 
-[tool.black]
-line-length = 100
-target-version = [
-    "py311",
-]
-[tool.pytest.ini_options]
-asyncio_mode = "auto"
+[tool.mypy]
+python_version = "3.10"
+pretty = true
+ignore_missing_imports = true
+warn_redundant_casts = true
+warn_unused_configs = true
+strict_optional = true
+
 
 [tool.pylama]
 linters = "mccabe,pycodestyle,pylint"
 skip = ".nox/*,.private/*,build/*,docs/*,private/*,site/*,tests/*,venv/*"
 
 [tool.pylama.pycodestyle]
 max_line_length = 100
@@ -104,24 +123,7 @@
 # D212: Multi-line docstring summary should start at the first line
 # D400: First line should end with a period
 # D406: Section name should end with a newline
 # D407: Missing dashed underline after section
 # D408: Section underline should be in the line following the sections name
 # D409: Section underline should match the length of its name
 # D415: first line should end with a period, question mark, or exclamation point
-
-[tool.isort]
-profile = "black"
-line_length = 100
-multi_line_output = 3
-include_trailing_comma = true
-known_first_party = "scrapli"
-known_third_party = "asyncssh,pytest"
-
-[tool.mypy]
-python_version = "3.10"
-pretty = true
-ignore_missing_imports = true
-warn_redundant_casts = true
-warn_unused_configs = true
-strict_optional = true
-
```

### Comparing `scrapli_cfg-2023.1.30/scrapli_cfg/diff.py` & `scrapli_cfg-2023.7.30/scrapli_cfg/diff.py`

 * *Files identical despite different names*

### Comparing `scrapli_cfg-2023.1.30/scrapli_cfg/exceptions.py` & `scrapli_cfg-2023.7.30/scrapli_cfg/exceptions.py`

 * *Files identical despite different names*

### Comparing `scrapli_cfg-2023.1.30/scrapli_cfg/factory.py` & `scrapli_cfg-2023.7.30/scrapli_cfg/factory.py`

 * *Files identical despite different names*

### Comparing `scrapli_cfg-2023.1.30/scrapli_cfg/logging.py` & `scrapli_cfg-2023.7.30/scrapli_cfg/logging.py`

 * *Files identical despite different names*

### Comparing `scrapli_cfg-2023.1.30/scrapli_cfg/platform/base/async_platform.py` & `scrapli_cfg-2023.7.30/scrapli_cfg/platform/base/async_platform.py`

 * *Files identical despite different names*

### Comparing `scrapli_cfg-2023.1.30/scrapli_cfg/platform/base/base_platform.py` & `scrapli_cfg-2023.7.30/scrapli_cfg/platform/base/base_platform.py`

 * *Files identical despite different names*

### Comparing `scrapli_cfg-2023.1.30/scrapli_cfg/platform/base/sync_platform.py` & `scrapli_cfg-2023.7.30/scrapli_cfg/platform/base/sync_platform.py`

 * *Files identical despite different names*

### Comparing `scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/arista_eos/async_platform.py` & `scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/arista_eos/async_platform.py`

 * *Files identical despite different names*

### Comparing `scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/arista_eos/base_platform.py` & `scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/arista_eos/base_platform.py`

 * *Files identical despite different names*

### Comparing `scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/arista_eos/patterns.py` & `scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/arista_eos/patterns.py`

 * *Files identical despite different names*

### Comparing `scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/arista_eos/sync_platform.py` & `scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/arista_eos/sync_platform.py`

 * *Files identical despite different names*

### Comparing `scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/cisco_iosxe/async_platform.py` & `scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/cisco_iosxe/async_platform.py`

 * *Files identical despite different names*

### Comparing `scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/cisco_iosxe/base_platform.py` & `scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/cisco_iosxe/base_platform.py`

 * *Files identical despite different names*

### Comparing `scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/cisco_iosxe/sync_platform.py` & `scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/cisco_iosxe/sync_platform.py`

 * *Files identical despite different names*

### Comparing `scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/cisco_iosxr/async_platform.py` & `scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/cisco_iosxr/async_platform.py`

 * *Files identical despite different names*

### Comparing `scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/cisco_iosxr/base_platform.py` & `scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/cisco_iosxr/base_platform.py`

 * *Files identical despite different names*

### Comparing `scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/cisco_iosxr/patterns.py` & `scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/cisco_iosxr/patterns.py`

 * *Files identical despite different names*

### Comparing `scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/cisco_iosxr/sync_platform.py` & `scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/cisco_iosxr/sync_platform.py`

 * *Files identical despite different names*

### Comparing `scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/cisco_nxos/async_platform.py` & `scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/cisco_nxos/async_platform.py`

 * *Files identical despite different names*

### Comparing `scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/cisco_nxos/base_platform.py` & `scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/cisco_nxos/base_platform.py`

 * *Files identical despite different names*

### Comparing `scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/cisco_nxos/patterns.py` & `scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/cisco_nxos/patterns.py`

 * *Files identical despite different names*

### Comparing `scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/cisco_nxos/sync_platform.py` & `scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/cisco_nxos/sync_platform.py`

 * *Files identical despite different names*

### Comparing `scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/juniper_junos/async_platform.py` & `scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/juniper_junos/async_platform.py`

 * *Files identical despite different names*

### Comparing `scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/juniper_junos/base_platform.py` & `scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/juniper_junos/base_platform.py`

 * *Files identical despite different names*

### Comparing `scrapli_cfg-2023.1.30/scrapli_cfg/platform/core/juniper_junos/sync_platform.py` & `scrapli_cfg-2023.7.30/scrapli_cfg/platform/core/juniper_junos/sync_platform.py`

 * *Files identical despite different names*

### Comparing `scrapli_cfg-2023.1.30/scrapli_cfg/response.py` & `scrapli_cfg-2023.7.30/scrapli_cfg/response.py`

 * *Files identical despite different names*

### Comparing `scrapli_cfg-2023.1.30/scrapli_cfg.egg-info/PKG-INFO` & `scrapli_cfg-2023.7.30/scrapli_cfg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapli-cfg
-Version: 2023.1.30
+Version: 2023.7.30
 Summary: Network device configuration management with scrapli
 Author-email: Carl Montanari <carl.r.montanari@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Carl Montanari
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,18 +21,18 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.com/scrapli/scrapli_cfg
 Project-URL: Changelog, https://scrapli.github.io/scrapli_cfg/changelog/
 Project-URL: Docs, https://scrapli.github.io/scrapli_cfg/
-Keywords: ssh,telnet,netconf,automation,network,cisco,iosxr,iosxe,nxos,arista,eos,juniper,junos
+Project-URL: Homepage, https://github.com/scrapli/scrapli_cfg
+Keywords: arista,automation,cisco,eos,iosxe,iosxr,juniper,junos,netconf,network,nxos,ssh,telnet
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scrapli-cfg Version: 2023.1.30 Summary: Network
+Metadata-Version: 2.1 Name: scrapli-cfg Version: 2023.7.30 Summary: Network
 device configuration management with scrapli Author-email: Carl Montanari
 r.montanari@gmail.com> License: MIT License Copyright (c) 2021 Carl Montanari
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
@@ -10,18 +10,19 @@
 permission notice shall be included in all copies or substantial portions of
 the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
 EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
 OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://github.com/scrapli/
-scrapli_cfg Project-URL: Changelog, https://scrapli.github.io/scrapli_cfg/
-changelog/ Project-URL: Docs, https://scrapli.github.io/scrapli_cfg/ Keywords:
-ssh,telnet,netconf,automation,network,cisco,iosxr,iosxe,nxos,arista,eos,juniper,junos
+DEALINGS IN THE SOFTWARE. Project-URL: Changelog, https://scrapli.github.io/
+scrapli_cfg/changelog/ Project-URL: Docs, https://scrapli.github.io/
+scrapli_cfg/ Project-URL: Homepage, https://github.com/scrapli/scrapli_cfg
+Keywords:
+arista,automation,cisco,eos,iosxe,iosxr,juniper,junos,netconf,network,nxos,ssh,telnet
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: POSIX :: Linux Classifier: Operating System :: MacOS Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Topic :: Software Development ::
```

### Comparing `scrapli_cfg-2023.1.30/scrapli_cfg.egg-info/SOURCES.txt` & `scrapli_cfg-2023.7.30/scrapli_cfg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scrapli_cfg-2023.1.30/scrapli_cfg.egg-info/requires.txt` & `scrapli_cfg-2023.7.30/scrapli_cfg.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 scrapli>=2022.01.30a2
 
 [asyncssh]
 asyncssh<3.0.0,>=2.2.1
 
 [dev]
-black==22.12.0
+black<24.0.0,>=23.3.0
 darglint<2.0.0,>=1.8.1
 isort<6.0.0,>=5.10.1
-mypy==0.991
-nox==2022.11.21
+mypy==1.4.1
+nox==2023.4.22
 pycodestyle<3.0.0,>=2.8.0
 pydocstyle<7.0.0,>=6.1.1
 pyfakefs<6.0.0,>=5.0.0
 pylama<9.0.0,>=8.4.0
-pylint==2.15.10
+pylint==2.17.5
 pytest-asyncio<1.0.0,>=0.17.0
 pytest-cov<5.0.0,>=3.0.0
 pytest<8.0.0,>=7.0.0
 scrapli-replay==2022.7.30
 toml<1.0.0,>=0.10.2
-paramiko<3.0.0,>=2.6.0
-ssh2-python<2.0.0,>=0.23.0
+paramiko<4.0.0,>=2.6.0
 asyncssh<3.0.0,>=2.2.1
 
+[dev:python_version < "3.12"]
+ssh2-python<2.0.0,>=0.23.0
+
 [docs]
 mdx-gh-links<1.0,>=0.2
 mkdocs<2.0.0,>=1.2.3
 mkdocs-gen-files<1.0.0,>=0.4.0
 mkdocs-literate-nav<1.0.0,>=0.5.0
 mkdocs-material<10.0.0,>=8.1.6
 mkdocs-material-extensions<2.0.0,>=1.0.3
 mkdocs-section-index<1.0.0,>=0.3.4
 mkdocstrings[python]<1.0.0,>=0.19.0
 
 [paramiko]
-paramiko<3.0.0,>=2.6.0
+paramiko<4.0.0,>=2.6.0
 
 [ssh2]
+
+[ssh2:python_version < "3.12"]
 ssh2-python<2.0.0,>=0.23.0
```

