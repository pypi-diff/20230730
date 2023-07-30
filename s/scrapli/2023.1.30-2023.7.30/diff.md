# Comparing `tmp/scrapli-2023.1.30.tar.gz` & `tmp/scrapli-2023.7.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapli-2023.1.30.tar", last modified: Sat Jan 28 18:50:03 2023, max compression
+gzip compressed data, was "scrapli-2023.7.30.tar", last modified: Sun Jul 30 16:54:47 2023, max compression
```

## Comparing `scrapli-2023.1.30.tar` & `scrapli-2023.7.30.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 18:50:03.670698 scrapli-2023.1.30/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-01-28 18:49:48.000000 scrapli-2023.1.30/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-28 18:49:48.000000 scrapli-2023.1.30/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-01-28 18:50:03.670698 scrapli-2023.1.30/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-01-28 18:49:48.000000 scrapli-2023.1.30/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-01-28 18:49:48.000000 scrapli-2023.1.30/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-28 18:49:48.000000 scrapli-2023.1.30/requirements-asyncssh.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-01-28 18:49:48.000000 scrapli-2023.1.30/requirements-community.txt
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-01-28 18:49:48.000000 scrapli-2023.1.30/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-01-28 18:49:48.000000 scrapli-2023.1.30/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-01-28 18:49:48.000000 scrapli-2023.1.30/requirements-genie.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-28 18:49:48.000000 scrapli-2023.1.30/requirements-paramiko.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-28 18:49:48.000000 scrapli-2023.1.30/requirements-ssh2.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-28 18:49:48.000000 scrapli-2023.1.30/requirements-textfsm.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-28 18:49:48.000000 scrapli-2023.1.30/requirements-ttp.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-28 18:49:48.000000 scrapli-2023.1.30/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 18:50:03.662698 scrapli-2023.1.30/scrapli/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 18:50:03.662698 scrapli-2023.1.30/scrapli/channel/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22370 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/channel/async_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    19530 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/channel/base_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    21774 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/channel/sync_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    10089 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 18:50:03.662698 scrapli-2023.1.30/scrapli/driver/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/driver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 18:50:03.666698 scrapli-2023.1.30/scrapli/driver/base/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/driver/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/driver/base/async_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    33133 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/driver/base/base_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/driver/base/sync_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 18:50:03.666698 scrapli-2023.1.30/scrapli/driver/core/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/driver/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 18:50:03.666698 scrapli-2023.1.30/scrapli/driver/core/arista_eos/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/driver/core/arista_eos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/driver/core/arista_eos/async_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/driver/core/arista_eos/base_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/driver/core/arista_eos/sync_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 18:50:03.666698 scrapli-2023.1.30/scrapli/driver/core/cisco_iosxe/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/driver/core/cisco_iosxe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/driver/core/cisco_iosxe/async_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/driver/core/cisco_iosxe/base_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/driver/core/cisco_iosxe/sync_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 18:50:03.666698 scrapli-2023.1.30/scrapli/driver/core/cisco_iosxr/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/driver/core/cisco_iosxr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/driver/core/cisco_iosxr/async_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/driver/core/cisco_iosxr/base_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/driver/core/cisco_iosxr/sync_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 18:50:03.666698 scrapli-2023.1.30/scrapli/driver/core/cisco_nxos/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/driver/core/cisco_nxos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/driver/core/cisco_nxos/async_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/driver/core/cisco_nxos/base_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/driver/core/cisco_nxos/sync_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 18:50:03.666698 scrapli-2023.1.30/scrapli/driver/core/juniper_junos/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/driver/core/juniper_junos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/driver/core/juniper_junos/async_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/driver/core/juniper_junos/base_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/driver/core/juniper_junos/sync_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 18:50:03.666698 scrapli-2023.1.30/scrapli/driver/generic/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/driver/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24022 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/driver/generic/async_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    11719 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/driver/generic/base_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    23762 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/driver/generic/sync_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 18:50:03.666698 scrapli-2023.1.30/scrapli/driver/network/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/driver/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26187 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/driver/network/async_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    21165 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/driver/network/base_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    25989 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/driver/network/sync_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    36079 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9801 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/response.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    17910 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/ssh_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 18:50:03.666698 scrapli-2023.1.30/scrapli/transport/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/transport/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 18:50:03.670698 scrapli-2023.1.30/scrapli/transport/base/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/transport/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/transport/base/async_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/transport/base/base_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/transport/base/base_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/transport/base/sync_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/transport/base/telnet_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 18:50:03.670698 scrapli-2023.1.30/scrapli/transport/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/transport/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 18:50:03.670698 scrapli-2023.1.30/scrapli/transport/plugins/asyncssh/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/transport/plugins/asyncssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10282 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/transport/plugins/asyncssh/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 18:50:03.670698 scrapli-2023.1.30/scrapli/transport/plugins/asynctelnet/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/transport/plugins/asynctelnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/transport/plugins/asynctelnet/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 18:50:03.670698 scrapli-2023.1.30/scrapli/transport/plugins/paramiko/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/transport/plugins/paramiko/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/transport/plugins/paramiko/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 18:50:03.670698 scrapli-2023.1.30/scrapli/transport/plugins/ssh2/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/transport/plugins/ssh2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/transport/plugins/ssh2/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 18:50:03.670698 scrapli-2023.1.30/scrapli/transport/plugins/system/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/transport/plugins/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24131 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/transport/plugins/system/ptyprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/transport/plugins/system/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 18:50:03.670698 scrapli-2023.1.30/scrapli/transport/plugins/telnet/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/transport/plugins/telnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-01-28 18:49:48.000000 scrapli-2023.1.30/scrapli/transport/plugins/telnet/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 18:50:03.662698 scrapli-2023.1.30/scrapli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-01-28 18:50:03.000000 scrapli-2023.1.30/scrapli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-01-28 18:50:03.000000 scrapli-2023.1.30/scrapli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-28 18:50:03.000000 scrapli-2023.1.30/scrapli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-01-28 18:50:03.000000 scrapli-2023.1.30/scrapli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-28 18:50:03.000000 scrapli-2023.1.30/scrapli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-01-28 18:50:03.670698 scrapli-2023.1.30/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:54:47.121202 scrapli-2023.7.30/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-30 16:54:29.000000 scrapli-2023.7.30/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-30 16:54:29.000000 scrapli-2023.7.30/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-07-30 16:54:47.121202 scrapli-2023.7.30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-30 16:54:29.000000 scrapli-2023.7.30/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-07-30 16:54:29.000000 scrapli-2023.7.30/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-30 16:54:29.000000 scrapli-2023.7.30/requirements-asyncssh.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-30 16:54:29.000000 scrapli-2023.7.30/requirements-community.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-30 16:54:29.000000 scrapli-2023.7.30/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-30 16:54:29.000000 scrapli-2023.7.30/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-30 16:54:29.000000 scrapli-2023.7.30/requirements-genie.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-30 16:54:29.000000 scrapli-2023.7.30/requirements-paramiko.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-30 16:54:29.000000 scrapli-2023.7.30/requirements-ssh2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-30 16:54:29.000000 scrapli-2023.7.30/requirements-textfsm.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-30 16:54:29.000000 scrapli-2023.7.30/requirements-ttp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 16:54:29.000000 scrapli-2023.7.30/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:54:47.109202 scrapli-2023.7.30/scrapli/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:54:47.109202 scrapli-2023.7.30/scrapli/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22370 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/channel/async_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21066 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/channel/base_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22353 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/channel/sync_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10421 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:54:47.109202 scrapli-2023.7.30/scrapli/driver/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/driver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:54:47.109202 scrapli-2023.7.30/scrapli/driver/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/driver/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/driver/base/async_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33907 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/driver/base/base_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/driver/base/sync_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:54:47.109202 scrapli-2023.7.30/scrapli/driver/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/driver/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:54:47.109202 scrapli-2023.7.30/scrapli/driver/core/arista_eos/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/driver/core/arista_eos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/driver/core/arista_eos/async_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/driver/core/arista_eos/base_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/driver/core/arista_eos/sync_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:54:47.113202 scrapli-2023.7.30/scrapli/driver/core/cisco_iosxe/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/driver/core/cisco_iosxe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/driver/core/cisco_iosxe/async_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/driver/core/cisco_iosxe/base_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/driver/core/cisco_iosxe/sync_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:54:47.113202 scrapli-2023.7.30/scrapli/driver/core/cisco_iosxr/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/driver/core/cisco_iosxr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/driver/core/cisco_iosxr/async_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/driver/core/cisco_iosxr/base_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/driver/core/cisco_iosxr/sync_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:54:47.113202 scrapli-2023.7.30/scrapli/driver/core/cisco_nxos/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/driver/core/cisco_nxos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/driver/core/cisco_nxos/async_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/driver/core/cisco_nxos/base_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/driver/core/cisco_nxos/sync_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:54:47.113202 scrapli-2023.7.30/scrapli/driver/core/juniper_junos/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/driver/core/juniper_junos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/driver/core/juniper_junos/async_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/driver/core/juniper_junos/base_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/driver/core/juniper_junos/sync_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:54:47.113202 scrapli-2023.7.30/scrapli/driver/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/driver/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24334 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/driver/generic/async_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11719 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/driver/generic/base_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24074 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/driver/generic/sync_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:54:47.113202 scrapli-2023.7.30/scrapli/driver/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/driver/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26499 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/driver/network/async_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21165 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/driver/network/base_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26301 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/driver/network/sync_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36079 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9801 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17910 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/ssh_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:54:47.113202 scrapli-2023.7.30/scrapli/transport/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/transport/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:54:47.113202 scrapli-2023.7.30/scrapli/transport/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/transport/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/transport/base/async_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/transport/base/base_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/transport/base/base_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/transport/base/sync_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/transport/base/telnet_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:54:47.113202 scrapli-2023.7.30/scrapli/transport/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/transport/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:54:47.117202 scrapli-2023.7.30/scrapli/transport/plugins/asyncssh/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/transport/plugins/asyncssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/transport/plugins/asyncssh/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:54:47.117202 scrapli-2023.7.30/scrapli/transport/plugins/asynctelnet/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/transport/plugins/asynctelnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/transport/plugins/asynctelnet/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:54:47.117202 scrapli-2023.7.30/scrapli/transport/plugins/paramiko/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/transport/plugins/paramiko/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/transport/plugins/paramiko/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:54:47.117202 scrapli-2023.7.30/scrapli/transport/plugins/ssh2/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/transport/plugins/ssh2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/transport/plugins/ssh2/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:54:47.117202 scrapli-2023.7.30/scrapli/transport/plugins/system/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/transport/plugins/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24131 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/transport/plugins/system/ptyprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/transport/plugins/system/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:54:47.121202 scrapli-2023.7.30/scrapli/transport/plugins/telnet/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/transport/plugins/telnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-07-30 16:54:29.000000 scrapli-2023.7.30/scrapli/transport/plugins/telnet/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:54:47.109202 scrapli-2023.7.30/scrapli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-07-30 16:54:47.000000 scrapli-2023.7.30/scrapli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-30 16:54:47.000000 scrapli-2023.7.30/scrapli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 16:54:47.000000 scrapli-2023.7.30/scrapli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-30 16:54:47.000000 scrapli-2023.7.30/scrapli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-30 16:54:47.000000 scrapli-2023.7.30/scrapli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-30 16:54:47.121202 scrapli-2023.7.30/setup.cfg
```

### Comparing `scrapli-2023.1.30/LICENSE` & `scrapli-2023.7.30/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapli-2023.1.30/PKG-INFO` & `scrapli-2023.7.30/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapli
-Version: 2023.1.30
+Version: 2023.7.30
 Summary: Fast, flexible, sync/async, Python 3.7+ screen scraping client specifically for network devices
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
         
-Project-URL: Homepage, https://github.com/carlmontanari/scrapli
 Project-URL: Changelog, https://carlmontanari.github.io/scrapli/changelog
 Project-URL: Docs, https://carlmontanari.github.io/scrapli/
-Keywords: ssh,telnet,netconf,automation,network,cisco,iosxr,iosxe,nxos,arista,eos,juniper,junos
+Project-URL: Homepage, https://github.com/carlmontanari/scrapli
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
-Metadata-Version: 2.1 Name: scrapli Version: 2023.1.30 Summary: Fast, flexible,
+Metadata-Version: 2.1 Name: scrapli Version: 2023.7.30 Summary: Fast, flexible,
 sync/async, Python 3.7+ screen scraping client specifically for network devices
 Author-email: Carl Montanari
 r.montanari@gmail.com> License: MIT License Copyright (c) 2021 Carl Montanari
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
@@ -11,19 +11,19 @@
 permission notice shall be included in all copies or substantial portions of
 the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
 EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
 OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://github.com/
-carlmontanari/scrapli Project-URL: Changelog, https://carlmontanari.github.io/
-scrapli/changelog Project-URL: Docs, https://carlmontanari.github.io/scrapli/
-Keywords:
-ssh,telnet,netconf,automation,network,cisco,iosxr,iosxe,nxos,arista,eos,juniper,junos
+DEALINGS IN THE SOFTWARE. Project-URL: Changelog, https://
+carlmontanari.github.io/scrapli/changelog Project-URL: Docs, https://
+carlmontanari.github.io/scrapli/ Project-URL: Homepage, https://github.com/
+carlmontanari/scrapli Keywords:
+arista,automation,cisco,eos,iosxe,iosxr,juniper,junos,netconf,network,nxos,ssh,telnet
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: POSIX :: Linux Classifier: Operating System :: MacOS Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Topic :: Software Development ::
```

### Comparing `scrapli-2023.1.30/README.md` & `scrapli-2023.7.30/README.md`

 * *Files identical despite different names*

### Comparing `scrapli-2023.1.30/pyproject.toml` & `scrapli-2023.7.30/pyproject.toml`

 * *Files 2% similar despite different names*

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
 name = "scrapli"
-dynamic = [
-    "version",
-    "dependencies",
-    "optional-dependencies",
-]
 description = "Fast, flexible, sync/async, Python 3.7+ screen scraping client specifically for network devices"
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
-Homepage = "https://github.com/carlmontanari/scrapli"
 Changelog = "https://carlmontanari.github.io/scrapli/changelog"
 Docs = "https://carlmontanari.github.io/scrapli/"
+Homepage = "https://github.com/carlmontanari/scrapli"
 
 [tool.setuptools.dynamic]
 version = { attr = "scrapli.__version__" }
 dependencies = { file = "requirements.txt" }
 optional-dependencies.dev = { file = [
     "requirements-dev.txt",
     "requirements-textfsm.txt",
@@ -73,33 +75,53 @@
 optional-dependencies.community = { file = "requirements-community.txt" }
 
 [tool.setuptools.package-data]
 scrapli = [
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
     "scrapli/"
 ]
 omit = [
     "scrapli/transport/plugins/system/ptyprocess.py"
 ]
 
 [tool.coverage.report]
 sort = "cover"
 omit = ["scrapli/transport/plugins/system/ptyprocess.py"]
 
-[tool.black]
-line-length = 100
-target-version = [
-    "py311",
-]
-[tool.pytest.ini_options]
-asyncio_mode = "auto"
+[tool.mypy]
+python_version = "3.11"
+pretty = true
+ignore_missing_imports = true
+warn_redundant_casts = true
+warn_unused_configs = true
+strict_optional = true
+
+[[tool.mypy.overrides]]
+module = "scrapli.transport.plugins.system.ptyprocess"
+ignore_errors = true
 
 [tool.pylama]
 linters = "mccabe,pycodestyle,pylint"
 skip = ".nox/*,.private/*,build/*,docs/*,private/*,scrapli/transport/plugins/system/ptyprocess.py,site/*,tests/*,venv/*"
 
 [tool.pylama.pycodestyle]
 max_line_length = 100
@@ -116,27 +138,7 @@
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
-python_version = "3.11"
-pretty = true
-ignore_missing_imports = true
-warn_redundant_casts = true
-warn_unused_configs = true
-strict_optional = true
-
-[[tool.mypy.overrides]]
-module = "scrapli.transport.plugins.system.ptyprocess"
-ignore_errors = true
```

### Comparing `scrapli-2023.1.30/scrapli/channel/async_channel.py` & `scrapli-2023.7.30/scrapli/channel/async_channel.py`

 * *Files identical despite different names*

### Comparing `scrapli-2023.1.30/scrapli/channel/base_channel.py` & `scrapli-2023.7.30/scrapli/channel/base_channel.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,18 +11,24 @@
 from scrapli.transport.base import AsyncTransport, Transport
 
 ANSI_ESCAPE_PATTERN = re.compile(rb"\x1b(\[.*?[@-~]|\].*?(\x07|\x1b\\)|E)")
 
 
 @dataclass()
 class BaseChannelArgs:
-    """
+    r"""
     Dataclass for all base Channel arguments
 
     Args:
+        auth_telnet_login_pattern: the pattern to use to find the telnet login/username prompt,
+            defaults to `r"^(.*username:)|(.*login:)\s?$"`
+        auth_password_pattern: the pattern to use to find the password prompt during in channel
+            authentication, defaults to `r"(.*@.*)?password:\s?$"`
+        auth_passphrase_pattern: the pattern used to find the ssh key passphrase prompt during
+            in channel authentication, defaults to: `r"enter passphrase for key"`
         comms_prompt_pattern: comms_prompt_pattern to assign to the channel; should generally be
             created/passed from the driver class
         comms_return_char: comms_return_char to assign to the channel, see above
         comms_prompt_search_depth: depth of the buffer to search in for searching for the prompt
             in "read_until_prompt"; smaller number here will generally be faster, though may be less
             reliable; default value is 1000
         timeout_ops: timeout_ops to assign to the channel, see above
@@ -37,14 +43,17 @@
         None
 
     Raises:
         N/A
 
     """
 
+    auth_telnet_login_pattern: str = r"^(.*username:)|(.*login:)\s?$"
+    auth_password_pattern: str = r"(.*@.*)?password:\s?$"
+    auth_passphrase_pattern: str = r"enter passphrase for key"
     comms_prompt_pattern: str = r"^[a-z0-9.\-@()/:]{1,32}[#>$]$"
     comms_return_char: str = "\n"
     comms_prompt_search_depth: int = 1000
     timeout_ops: float = 30.0
     channel_log: Union[str, bool, BytesIO] = False
     channel_log_mode: str = "write"
     channel_lock: bool = False
@@ -59,14 +68,23 @@
         Returns:
             None
 
         Raises:
             ScrapliValueError: if invalid channel_log_mode provided
 
         """
+        if self.auth_telnet_login_pattern == "":
+            self.auth_telnet_login_pattern = r"^(.*username:)|(.*login:)\s?$"
+
+        if self.auth_password_pattern == "":
+            self.auth_password_pattern = r"(.*@.*)?password:\s?$"
+
+        if self.auth_passphrase_pattern == "":
+            self.auth_passphrase_pattern = r"enter passphrase for key"
+
         if self.channel_log_mode.lower() not in (
             "write",
             "append",
         ):
             raise ScrapliValueError(
                 f"provided channel_log_mode '{self.channel_log_mode}' is not valid, mode must be "
                 f"one of: 'write', 'append'"
@@ -106,18 +124,14 @@
             host=self.transport._base_transport_args.host,
             port=self.transport._base_transport_args.port,
             uid=self.transport._base_transport_args.logging_uid,
         )
 
         self.channel_log: Optional[BinaryIO] = None
 
-        self._auth_telnet_login_pattern = r"^(.*username:)|(.*login:)\s?$"
-        self._auth_password_pattern = r"(.*@.*)?password:\s?$"
-        self._auth_passphrase_pattern = r"enter passphrase for key"
-
     @property
     def auth_telnet_login_pattern(self) -> Pattern[bytes]:
         """
         Getter for `auth_telnet_login_pattern` attribute
 
         Args:
             N/A
@@ -125,15 +139,17 @@
         Returns:
             Pattern: compiled pattern of the set auth_telnet_login_pattern value
 
         Raises:
             N/A
 
         """
-        return re.compile(self._auth_telnet_login_pattern.encode(), flags=re.I | re.M)
+        return re.compile(
+            self._base_channel_args.auth_telnet_login_pattern.encode(), flags=re.I | re.M
+        )
 
     @auth_telnet_login_pattern.setter
     def auth_telnet_login_pattern(self, value: str) -> None:
         """
         Setter for `auth_telnet_login_pattern` attribute
 
         Args:
@@ -148,15 +164,15 @@
 
         """
         self.logger.debug(f"setting 'auth_telnet_login_pattern' value to '{value}'")
 
         if not isinstance(value, str):
             raise ScrapliTypeError
 
-        self._auth_telnet_login_pattern = value
+        self._base_channel_args.auth_telnet_login_pattern = value
 
     @property
     def auth_password_pattern(self) -> Pattern[bytes]:
         """
         Getter for `auth_password_pattern` attribute
 
         Args:
@@ -165,15 +181,15 @@
         Returns:
             Pattern: compiled pattern of the set auth_password_pattern value
 
         Raises:
             N/A
 
         """
-        return re.compile(self._auth_password_pattern.encode(), flags=re.I | re.M)
+        return re.compile(self._base_channel_args.auth_password_pattern.encode(), flags=re.I | re.M)
 
     @auth_password_pattern.setter
     def auth_password_pattern(self, value: str) -> None:
         """
         Setter for `auth_password_pattern` attribute
 
         Args:
@@ -188,15 +204,15 @@
 
         """
         self.logger.debug(f"setting 'auth_password_pattern' value to '{value}'")
 
         if not isinstance(value, str):
             raise ScrapliTypeError
 
-        self._auth_password_pattern = value
+        self._base_channel_args.auth_password_pattern = value
 
     @property
     def auth_passphrase_pattern(self) -> Pattern[bytes]:
         """
         Getter for `auth_passphrase_pattern` attribute
 
         Args:
@@ -205,15 +221,17 @@
         Returns:
             Pattern: compiled pattern of the set auth_passphrase_pattern value
 
         Raises:
             N/A
 
         """
-        return re.compile(self._auth_passphrase_pattern.encode(), flags=re.I | re.M)
+        return re.compile(
+            self._base_channel_args.auth_passphrase_pattern.encode(), flags=re.I | re.M
+        )
 
     @auth_passphrase_pattern.setter
     def auth_passphrase_pattern(self, value: str) -> None:
         """
         Setter for `auth_passphrase_pattern` attribute
 
         Args:
@@ -228,15 +246,15 @@
 
         """
         self.logger.debug(f"setting '_auth_passphrase_pattern' value to '{value}'")
 
         if not isinstance(value, str):
             raise ScrapliTypeError
 
-        self._auth_passphrase_pattern = value
+        self._base_channel_args.auth_passphrase_pattern = value
 
     def open(self) -> None:
         """
         Channel open method
 
         Args:
             N/A
@@ -392,14 +410,23 @@
         msg = ""
         if b"host key verification failed" in output.lower():
             msg = "Host key verification failed"
         elif b"operation timed out" in output.lower() or b"connection timed out" in output.lower():
             msg = "Timed out connecting to host"
         elif b"no route to host" in output.lower():
             msg = "No route to host"
+        elif b"no matching host key" in output.lower():
+            msg = "No matching host key type found for host"
+            key_exchange_pattern = re.compile(
+                pattern=rb"their offer: ([a-z0-9\-,]*)", flags=re.M | re.I
+            )
+            offered_key_exchanges_match = re.search(pattern=key_exchange_pattern, string=output)
+            if offered_key_exchanges_match:
+                offered_key_exchanges = offered_key_exchanges_match.group(1).decode()
+                msg += f", their offer: {offered_key_exchanges}"
         elif b"no matching key exchange" in output.lower():
             msg = "No matching key exchange found for host"
             key_exchange_pattern = re.compile(
                 pattern=rb"their offer: ([a-z0-9\-,]*)", flags=re.M | re.I
             )
             offered_key_exchanges_match = re.search(pattern=key_exchange_pattern, string=output)
             if offered_key_exchanges_match:
```

### Comparing `scrapli-2023.1.30/scrapli/channel/sync_channel.py` & `scrapli-2023.7.30/scrapli/channel/sync_channel.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from datetime import datetime
 from io import BytesIO
 from threading import Lock
 from typing import Iterator, List, Optional, Tuple
 
 from scrapli.channel.base_channel import BaseChannel, BaseChannelArgs
 from scrapli.decorators import timeout_wrapper
-from scrapli.exceptions import ScrapliAuthenticationFailed, ScrapliTimeout
+from scrapli.exceptions import ScrapliAuthenticationFailed, ScrapliConnectionError, ScrapliTimeout
 from scrapli.transport.base import Transport
 
 
 class Channel(BaseChannel):
     def __init__(
         self,
         transport: Transport,
@@ -318,15 +318,17 @@
                 if re.search(
                     pattern=prompt_pattern,
                     string=authenticate_buf,
                 ):
                     return
 
     @timeout_wrapper
-    def channel_authenticate_telnet(self, auth_username: str = "", auth_password: str = "") -> None:
+    def channel_authenticate_telnet(  # noqa: c901
+        self, auth_username: str = "", auth_password: str = ""
+    ) -> None:
         """
         Handle Telnet Authentication
 
         Args:
             auth_username: username to use for telnet authentication
             auth_password: password to use for telnet authentication
 
@@ -352,15 +354,24 @@
             return_interval,
         ) = self._pre_channel_authenticate_telnet()
 
         return_attempts = 1
 
         with self._channel_lock():
             while True:
-                buf = self.read()
+                try:
+                    buf = self.read()
+                except ScrapliConnectionError:
+                    # telnet transport socket can send us an EOF which gets raised as a connection
+                    # error, if we see that we can try to send a return and go back to the top...
+                    # this first cropped up with telnet on asa devices in:
+                    # https://github.com/carlmontanari/scrapli/issues/278
+                    self.send_return()
+                    return_attempts += 1
+                    continue
 
                 if not buf:
                     current_iteration_time = datetime.now().timestamp()
                     if (current_iteration_time - auth_start_time) > (
                         return_interval * return_attempts
                     ):
                         self.send_return()
```

### Comparing `scrapli-2023.1.30/scrapli/decorators.py` & `scrapli-2023.7.30/scrapli/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import threading
 from concurrent.futures import ThreadPoolExecutor, wait
 from functools import partial, update_wrapper
 from logging import Logger, LoggerAdapter
 from typing import TYPE_CHECKING, Any, Callable, Tuple
 
 from scrapli.exceptions import ScrapliTimeout
+from scrapli.settings import Settings
 
 if TYPE_CHECKING:
     from scrapli.driver import AsyncGenericDriver, GenericDriver  # pragma:  no cover
     from scrapli.transport.base.base_transport import BaseTransport  # pragma:  no cover
 
 if TYPE_CHECKING:
     LoggerAdapterT = LoggerAdapter[Logger]  # pragma:  no cover  # pylint:disable=E1136
@@ -125,16 +126,22 @@
     Returns:
         None
 
     Raises:
         ScrapliTimeout: always, if we hit this method we have already timed out!
 
     """
-    logger.critical("operation timed out, closing connection")
-    transport.close()
+    if Settings.NO_TERMINATE_ON_TIMEOUT:
+        logger.critical(
+            "operation timed out, NO_TERMINATE_ON_TIMEOUT is true, not closing connection"
+        )
+    else:
+        logger.critical("operation timed out, closing connection")
+        transport.close()
+
     raise ScrapliTimeout(message)
 
 
 def _get_transport_logger_timeout(
     cls: Any,
 ) -> Tuple["BaseTransport", LoggerAdapterT, float]:
     """
@@ -275,16 +282,18 @@
             else:
                 driver_logger.info(
                     "modifying driver timeout for current operation, temporary timeout_ops "
                     f"value: '{timeout_ops_kwarg}'"
                 )
                 base_timeout_ops = driver_instance.timeout_ops
                 driver_instance.timeout_ops = kwargs["timeout_ops"]
-                result = await wrapped_func(*args, **kwargs)
-                driver_instance.timeout_ops = base_timeout_ops
+                try:
+                    result = await wrapped_func(*args, **kwargs)
+                finally:
+                    driver_instance.timeout_ops = base_timeout_ops
             return result
 
     else:
         # ignoring type error:
         # "All conditional function variants must have identical signatures"
         # one is sync one is async so never going to be identical here!
         def decorate(*args: Any, **kwargs: Any) -> Any:  # type: ignore
@@ -298,15 +307,17 @@
             else:
                 driver_logger.info(
                     "modifying driver timeout for current operation, temporary timeout_ops "
                     f"value: '{timeout_ops_kwarg}'"
                 )
                 base_timeout_ops = driver_instance.timeout_ops
                 driver_instance.timeout_ops = kwargs["timeout_ops"]
-                result = wrapped_func(*args, **kwargs)
-                driver_instance.timeout_ops = base_timeout_ops
+                try:
+                    result = wrapped_func(*args, **kwargs)
+                finally:
+                    driver_instance.timeout_ops = base_timeout_ops
             return result
 
     # ensures that the wrapped function is updated w/ the original functions docs/etc. --
     # necessary for introspection for the auto gen docs to work!
     update_wrapper(wrapper=decorate, wrapped=wrapped_func)
     return decorate
```

### Comparing `scrapli-2023.1.30/scrapli/driver/base/async_driver.py` & `scrapli-2023.7.30/scrapli/driver/base/async_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,17 @@
             )
 
         self.channel = AsyncChannel(
             transport=self.transport,
             base_channel_args=self._base_channel_args,
         )
 
+        if self.on_init:
+            self.on_init(self)
+
     async def __aenter__(self: _T) -> _T:
         """
         Enter method for context manager
 
         Args:
             N/A
```

### Comparing `scrapli-2023.1.30/scrapli/driver/base/base_driver.py` & `scrapli-2023.7.30/scrapli/driver/base/base_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,17 @@
         port: Optional[int] = None,
         auth_username: str = "",
         auth_password: str = "",
         auth_private_key: str = "",
         auth_private_key_passphrase: str = "",
         auth_strict_key: bool = True,
         auth_bypass: bool = False,
+        auth_telnet_login_pattern: str = "",
+        auth_password_pattern: str = "",
+        auth_passphrase_pattern: str = "",
         timeout_socket: float = 15.0,
         timeout_transport: float = 30.0,
         timeout_ops: float = 30.0,
         comms_prompt_pattern: str = r"^[a-z0-9.\-@()/:]{1,48}[#>$]\s*$",
         comms_return_char: str = "\n",
         ssh_config_file: Union[str, bool] = False,
         ssh_known_hosts_file: Union[str, bool] = False,
@@ -58,14 +61,20 @@
             auth_username: username for authentication
             auth_private_key: path to private key for authentication
             auth_private_key_passphrase: passphrase for decrypting ssh key if necessary
             auth_password: password for authentication
             auth_strict_key: strict host checking or not
             auth_bypass: bypass "in channel" authentication -- only supported with telnet,
                 asynctelnet, and system transport plugins
+            auth_telnet_login_pattern: the pattern to use to find the telnet login/username prompt,
+                defaults to `r"^(.*username:)|(.*login:)\s?$"`
+            auth_password_pattern: the pattern to use to find the password prompt during in channel
+                authentication, defaults to `r"(.*@.*)?password:\s?$"`
+            auth_passphrase_pattern: the pattern used to find the ssh key passphrase prompt during
+                in channel authentication, defaults to: `r"enter passphrase for key"`
             timeout_socket: timeout for establishing socket/initial connection in seconds
             timeout_transport: timeout for ssh|telnet transport in seconds
             timeout_ops: timeout for ssh channel operations
             comms_prompt_pattern: raw string regex pattern -- preferably use `^` and `$` anchors!
                 this is the single most important attribute here! if this does not match a prompt,
                 scrapli will not work!
                 IMPORTANT: regex search uses multi-line + case insensitive flags. multi-line allows
@@ -131,14 +140,17 @@
                 port = 23
 
         self.logger = get_instance_logger(
             instance_name="scrapli.driver", host=host, port=port, uid=logging_uid
         )
 
         self._base_channel_args = BaseChannelArgs(
+            auth_telnet_login_pattern=auth_telnet_login_pattern,
+            auth_password_pattern=auth_password_pattern,
+            auth_passphrase_pattern=auth_passphrase_pattern,
             comms_prompt_pattern=comms_prompt_pattern,
             comms_return_char=comms_return_char,
             timeout_ops=timeout_ops,
             channel_log=channel_log,
             channel_log_mode=channel_log_mode,
             channel_lock=channel_lock,
         )
@@ -185,17 +197,14 @@
         transport_class, self._plugin_transport_args = self._transport_factory()
 
         self.transport = transport_class(
             base_transport_args=self._base_transport_args,
             plugin_transport_args=self._plugin_transport_args,
         )
 
-        if self.on_init:
-            self.on_init(self)
-
     def __str__(self) -> str:
         """
         Magic str method for Scrape
 
         Args:
             N/A
```

### Comparing `scrapli-2023.1.30/scrapli/driver/base/sync_driver.py` & `scrapli-2023.7.30/scrapli/driver/base/sync_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,19 @@
             )
 
         self.channel = Channel(
             transport=self.transport,
             base_channel_args=self._base_channel_args,
         )
 
+        # ensure the "on_init" func is called in the actual driver (sync/async rather than the base
+        # class) since we want to wait until after the channel is setup!
+        if self.on_init:
+            self.on_init(self)
+
     def __enter__(self: _T) -> _T:
         """
         Enter method for context manager
 
         Args:
             N/A
```

### Comparing `scrapli-2023.1.30/scrapli/driver/core/__init__.py` & `scrapli-2023.7.30/scrapli/driver/core/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapli-2023.1.30/scrapli/driver/core/arista_eos/async_driver.py` & `scrapli-2023.7.30/scrapli/driver/core/arista_eos/async_driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,17 @@
         port: Optional[int] = None,
         auth_username: str = "",
         auth_password: str = "",
         auth_private_key: str = "",
         auth_private_key_passphrase: str = "",
         auth_strict_key: bool = True,
         auth_bypass: bool = False,
+        auth_telnet_login_pattern: str = "",
+        auth_password_pattern: str = "",
+        auth_passphrase_pattern: str = "",
         timeout_socket: float = 15.0,
         timeout_transport: float = 30.0,
         timeout_ops: float = 30.0,
         comms_return_char: str = "\n",
         ssh_config_file: Union[str, bool] = False,
         ssh_known_hosts_file: Union[str, bool] = False,
         on_init: Optional[Callable[..., Any]] = None,
@@ -132,14 +135,17 @@
             port=port,
             auth_username=auth_username,
             auth_password=auth_password,
             auth_private_key=auth_private_key,
             auth_private_key_passphrase=auth_private_key_passphrase,
             auth_strict_key=auth_strict_key,
             auth_bypass=auth_bypass,
+            auth_telnet_login_pattern=auth_telnet_login_pattern,
+            auth_password_pattern=auth_password_pattern,
+            auth_passphrase_pattern=auth_passphrase_pattern,
             timeout_socket=timeout_socket,
             timeout_transport=timeout_transport,
             timeout_ops=timeout_ops,
             comms_return_char=comms_return_char,
             ssh_config_file=ssh_config_file,
             ssh_known_hosts_file=ssh_known_hosts_file,
             on_init=on_init,
```

### Comparing `scrapli-2023.1.30/scrapli/driver/core/arista_eos/base_driver.py` & `scrapli-2023.7.30/scrapli/driver/core/arista_eos/base_driver.py`

 * *Files identical despite different names*

### Comparing `scrapli-2023.1.30/scrapli/driver/core/arista_eos/sync_driver.py` & `scrapli-2023.7.30/scrapli/driver/core/arista_eos/sync_driver.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,17 @@
         port: Optional[int] = None,
         auth_username: str = "",
         auth_password: str = "",
         auth_private_key: str = "",
         auth_private_key_passphrase: str = "",
         auth_strict_key: bool = True,
         auth_bypass: bool = False,
+        auth_telnet_login_pattern: str = "",
+        auth_password_pattern: str = "",
+        auth_passphrase_pattern: str = "",
         timeout_socket: float = 15.0,
         timeout_transport: float = 30.0,
         timeout_ops: float = 30.0,
         comms_return_char: str = "\n",
         ssh_config_file: Union[str, bool] = False,
         ssh_known_hosts_file: Union[str, bool] = False,
         on_init: Optional[Callable[..., Any]] = None,
@@ -132,14 +135,17 @@
             port=port,
             auth_username=auth_username,
             auth_password=auth_password,
             auth_private_key=auth_private_key,
             auth_private_key_passphrase=auth_private_key_passphrase,
             auth_strict_key=auth_strict_key,
             auth_bypass=auth_bypass,
+            auth_telnet_login_pattern=auth_telnet_login_pattern,
+            auth_password_pattern=auth_password_pattern,
+            auth_passphrase_pattern=auth_passphrase_pattern,
             timeout_socket=timeout_socket,
             timeout_transport=timeout_transport,
             timeout_ops=timeout_ops,
             comms_return_char=comms_return_char,
             ssh_config_file=ssh_config_file,
             ssh_known_hosts_file=ssh_known_hosts_file,
             on_init=on_init,
```

### Comparing `scrapli-2023.1.30/scrapli/driver/core/cisco_iosxe/async_driver.py` & `scrapli-2023.7.30/scrapli/driver/core/cisco_iosxe/async_driver.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,14 +55,17 @@
         port: Optional[int] = None,
         auth_username: str = "",
         auth_password: str = "",
         auth_private_key: str = "",
         auth_private_key_passphrase: str = "",
         auth_strict_key: bool = True,
         auth_bypass: bool = False,
+        auth_telnet_login_pattern: str = "",
+        auth_password_pattern: str = "",
+        auth_passphrase_pattern: str = "",
         timeout_socket: float = 15.0,
         timeout_transport: float = 30.0,
         timeout_ops: float = 30.0,
         comms_return_char: str = "\n",
         ssh_config_file: Union[str, bool] = False,
         ssh_known_hosts_file: Union[str, bool] = False,
         on_init: Optional[Callable[..., Any]] = None,
@@ -129,14 +132,17 @@
             port=port,
             auth_username=auth_username,
             auth_password=auth_password,
             auth_private_key=auth_private_key,
             auth_private_key_passphrase=auth_private_key_passphrase,
             auth_strict_key=auth_strict_key,
             auth_bypass=auth_bypass,
+            auth_telnet_login_pattern=auth_telnet_login_pattern,
+            auth_password_pattern=auth_password_pattern,
+            auth_passphrase_pattern=auth_passphrase_pattern,
             timeout_socket=timeout_socket,
             timeout_transport=timeout_transport,
             timeout_ops=timeout_ops,
             comms_return_char=comms_return_char,
             ssh_config_file=ssh_config_file,
             ssh_known_hosts_file=ssh_known_hosts_file,
             on_init=on_init,
```

### Comparing `scrapli-2023.1.30/scrapli/driver/core/cisco_iosxe/base_driver.py` & `scrapli-2023.7.30/scrapli/driver/core/cisco_iosxe/base_driver.py`

 * *Files identical despite different names*

### Comparing `scrapli-2023.1.30/scrapli/driver/core/cisco_iosxe/sync_driver.py` & `scrapli-2023.7.30/scrapli/driver/core/cisco_iosxe/sync_driver.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,17 @@
         port: Optional[int] = None,
         auth_username: str = "",
         auth_password: str = "",
         auth_private_key: str = "",
         auth_private_key_passphrase: str = "",
         auth_strict_key: bool = True,
         auth_bypass: bool = False,
+        auth_telnet_login_pattern: str = "",
+        auth_password_pattern: str = "",
+        auth_passphrase_pattern: str = "",
         timeout_socket: float = 15.0,
         timeout_transport: float = 30.0,
         timeout_ops: float = 30.0,
         comms_return_char: str = "\n",
         ssh_config_file: Union[str, bool] = False,
         ssh_known_hosts_file: Union[str, bool] = False,
         on_init: Optional[Callable[..., Any]] = None,
@@ -129,14 +132,17 @@
             port=port,
             auth_username=auth_username,
             auth_password=auth_password,
             auth_private_key=auth_private_key,
             auth_private_key_passphrase=auth_private_key_passphrase,
             auth_strict_key=auth_strict_key,
             auth_bypass=auth_bypass,
+            auth_telnet_login_pattern=auth_telnet_login_pattern,
+            auth_password_pattern=auth_password_pattern,
+            auth_passphrase_pattern=auth_passphrase_pattern,
             timeout_socket=timeout_socket,
             timeout_transport=timeout_transport,
             timeout_ops=timeout_ops,
             comms_return_char=comms_return_char,
             ssh_config_file=ssh_config_file,
             ssh_known_hosts_file=ssh_known_hosts_file,
             on_init=on_init,
```

### Comparing `scrapli-2023.1.30/scrapli/driver/core/cisco_iosxr/async_driver.py` & `scrapli-2023.7.30/scrapli/driver/core/cisco_iosxr/async_driver.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,14 +54,17 @@
         port: Optional[int] = None,
         auth_username: str = "",
         auth_password: str = "",
         auth_private_key: str = "",
         auth_private_key_passphrase: str = "",
         auth_strict_key: bool = True,
         auth_bypass: bool = False,
+        auth_telnet_login_pattern: str = "",
+        auth_password_pattern: str = "",
+        auth_passphrase_pattern: str = "",
         timeout_socket: float = 15.0,
         timeout_transport: float = 30.0,
         timeout_ops: float = 30.0,
         comms_return_char: str = "\n",
         ssh_config_file: Union[str, bool] = False,
         ssh_known_hosts_file: Union[str, bool] = False,
         on_init: Optional[Callable[..., Any]] = None,
@@ -128,14 +131,17 @@
             port=port,
             auth_username=auth_username,
             auth_password=auth_password,
             auth_private_key=auth_private_key,
             auth_private_key_passphrase=auth_private_key_passphrase,
             auth_strict_key=auth_strict_key,
             auth_bypass=auth_bypass,
+            auth_telnet_login_pattern=auth_telnet_login_pattern,
+            auth_password_pattern=auth_password_pattern,
+            auth_passphrase_pattern=auth_passphrase_pattern,
             timeout_socket=timeout_socket,
             timeout_transport=timeout_transport,
             timeout_ops=timeout_ops,
             comms_return_char=comms_return_char,
             ssh_config_file=ssh_config_file,
             ssh_known_hosts_file=ssh_known_hosts_file,
             on_init=on_init,
```

### Comparing `scrapli-2023.1.30/scrapli/driver/core/cisco_iosxr/base_driver.py` & `scrapli-2023.7.30/scrapli/driver/core/cisco_iosxr/base_driver.py`

 * *Files identical despite different names*

### Comparing `scrapli-2023.1.30/scrapli/driver/core/cisco_iosxr/sync_driver.py` & `scrapli-2023.7.30/scrapli/driver/core/cisco_nxos/sync_driver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,70 +1,71 @@
-"""scrapli.driver.core.cisco_iosxr.sync_driver"""
+"""scrapli.driver.core.cisco_nxos.sync_driver"""
 from copy import deepcopy
 from io import BytesIO
 from typing import Any, Callable, Dict, List, Optional, Union
 
 from scrapli.driver import NetworkDriver
-from scrapli.driver.core.cisco_iosxr.base_driver import FAILED_WHEN_CONTAINS, PRIVS
+from scrapli.driver.core.cisco_nxos.base_driver import FAILED_WHEN_CONTAINS, PRIVS, NXOSDriverBase
 from scrapli.driver.network.base_driver import PrivilegeLevel
 
 
-def iosxr_on_open(conn: NetworkDriver) -> None:
+def nxos_on_open(conn: NetworkDriver) -> None:
     """
-    IOSXRDriver default on_open callable
+    NXOSDriver default on_open callable
 
     Args:
         conn: NetworkDriver object
 
     Returns:
         None
 
     Raises:
         N/A
 
     """
     conn.acquire_priv(desired_priv=conn.default_desired_privilege_level)
     conn.send_command(command="terminal length 0")
-    conn.send_command(command="terminal width 512")
+    conn.send_command(command="terminal width 511")
 
 
-def iosxr_on_close(conn: NetworkDriver) -> None:
+def nxos_on_close(conn: NetworkDriver) -> None:
     """
-    IOSXRDriver default on_close callable
+    NXOSDriver default on_close callable
 
     Args:
         conn: NetworkDriver object
 
     Returns:
         None
 
     Raises:
         N/A
 
     """
-    # write exit directly to the transport as channel would fail to find the prompt after sending
-    # the exit command!
     conn.acquire_priv(desired_priv=conn.default_desired_privilege_level)
     conn.channel.write(channel_input="exit")
     conn.channel.send_return()
 
 
-class IOSXRDriver(NetworkDriver):
+class NXOSDriver(NetworkDriver, NXOSDriverBase):
     def __init__(
         self,
         host: str,
         privilege_levels: Optional[Dict[str, PrivilegeLevel]] = None,
         default_desired_privilege_level: str = "privilege_exec",
         port: Optional[int] = None,
         auth_username: str = "",
         auth_password: str = "",
         auth_private_key: str = "",
         auth_private_key_passphrase: str = "",
         auth_strict_key: bool = True,
         auth_bypass: bool = False,
+        auth_telnet_login_pattern: str = "",
+        auth_password_pattern: str = "",
+        auth_passphrase_pattern: str = "",
         timeout_socket: float = 15.0,
         timeout_transport: float = 30.0,
         timeout_ops: float = 30.0,
         comms_return_char: str = "\n",
         ssh_config_file: Union[str, bool] = False,
         ssh_known_hosts_file: Union[str, bool] = False,
         on_init: Optional[Callable[..., Any]] = None,
@@ -74,26 +75,26 @@
         transport_options: Optional[Dict[str, Any]] = None,
         channel_log: Union[str, bool, BytesIO] = False,
         channel_log_mode: str = "write",
         channel_lock: bool = False,
         logging_uid: str = "",
         auth_secondary: str = "",
         failed_when_contains: Optional[List[str]] = None,
-        textfsm_platform: str = "cisco_xr",
-        genie_platform: str = "iosxr",
+        textfsm_platform: str = "cisco_nxos",
+        genie_platform: str = "nxos",
     ):
         """
-        IOSXRDriver Object
+        NXOSDriver Object
 
         Please see `scrapli.driver.base.base_driver.Driver` for all "base driver" arguments!
 
         # noqa: DAR101
 
         Args:
-            privilege_levels: optional user provided privilege levels, if left None will default to
+             privilege_levels: optional user provided privilege levels, if left None will default to
                 scrapli standard privilege levels
             default_desired_privilege_level: string of name of default desired priv, this is the
                 priv level that is generally used to disable paging/set terminal width and things
                 like that upon first login, and is also the priv level scrapli will try to acquire
                 for normal "command" operations (`send_command`, `send_commands`)
             auth_secondary: password to use for secondary authentication (enable)
             on_open: callable that accepts the class instance as its only argument. this callable,
@@ -111,34 +112,40 @@
         Returns:
             None
 
         Raises:
             N/A
 
         """
+        # somewhere/somehow the mixin is causing mypy to be upset about comms_prompt_pattern...
+        self.comms_prompt_pattern: str
+
         if privilege_levels is None:
             privilege_levels = deepcopy(PRIVS)
 
         if on_open is None:
-            on_open = iosxr_on_open
+            on_open = nxos_on_open
         if on_close is None:
-            on_close = iosxr_on_close
+            on_close = nxos_on_close
 
         if failed_when_contains is None:
             failed_when_contains = FAILED_WHEN_CONTAINS.copy()
 
         super().__init__(
             host=host,
             port=port,
             auth_username=auth_username,
             auth_password=auth_password,
             auth_private_key=auth_private_key,
             auth_private_key_passphrase=auth_private_key_passphrase,
             auth_strict_key=auth_strict_key,
             auth_bypass=auth_bypass,
+            auth_telnet_login_pattern=auth_telnet_login_pattern,
+            auth_password_pattern=auth_password_pattern,
+            auth_passphrase_pattern=auth_passphrase_pattern,
             timeout_socket=timeout_socket,
             timeout_transport=timeout_transport,
             timeout_ops=timeout_ops,
             comms_return_char=comms_return_char,
             ssh_config_file=ssh_config_file,
             ssh_known_hosts_file=ssh_known_hosts_file,
             on_init=on_init,
@@ -156,21 +163,40 @@
             failed_when_contains=failed_when_contains,
             textfsm_platform=textfsm_platform,
             genie_platform=genie_platform,
         )
 
     def _abort_config(self) -> None:
         """
-        Abort IOSXR configuration session
+        Abort NXOS configuration session (if using a config session!)
 
         Args:
             N/A
 
         Returns:
             None
 
         Raises:
             N/A
 
         """
-        self.channel.send_input(channel_input="abort")
-        self._current_priv_level = self.privilege_levels["privilege_exec"]
+        # nxos pattern for config sessions should *always* have `config-s`
+        if "config\\-s" in self._current_priv_level.pattern:
+            self.channel.send_input(channel_input="abort")
+            self._current_priv_level = self.privilege_levels["privilege_exec"]
+
+    def register_configuration_session(self, session_name: str) -> None:
+        """
+        NXOS specific implementation of register_configuration_session
+
+        Args:
+            session_name: name of session to register
+
+        Returns:
+            None
+
+        Raises:
+            N/A
+
+        """
+        self._create_configuration_session(session_name=session_name)
+        self.update_privilege_levels()
```

### Comparing `scrapli-2023.1.30/scrapli/driver/core/cisco_nxos/async_driver.py` & `scrapli-2023.7.30/scrapli/driver/core/cisco_nxos/async_driver.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,14 +55,17 @@
         port: Optional[int] = None,
         auth_username: str = "",
         auth_password: str = "",
         auth_private_key: str = "",
         auth_private_key_passphrase: str = "",
         auth_strict_key: bool = True,
         auth_bypass: bool = False,
+        auth_telnet_login_pattern: str = "",
+        auth_password_pattern: str = "",
+        auth_passphrase_pattern: str = "",
         timeout_socket: float = 15.0,
         timeout_transport: float = 30.0,
         timeout_ops: float = 30.0,
         comms_return_char: str = "\n",
         ssh_config_file: Union[str, bool] = False,
         ssh_known_hosts_file: Union[str, bool] = False,
         on_init: Optional[Callable[..., Any]] = None,
@@ -132,14 +135,17 @@
             port=port,
             auth_username=auth_username,
             auth_password=auth_password,
             auth_private_key=auth_private_key,
             auth_private_key_passphrase=auth_private_key_passphrase,
             auth_strict_key=auth_strict_key,
             auth_bypass=auth_bypass,
+            auth_telnet_login_pattern=auth_telnet_login_pattern,
+            auth_password_pattern=auth_password_pattern,
+            auth_passphrase_pattern=auth_passphrase_pattern,
             timeout_socket=timeout_socket,
             timeout_transport=timeout_transport,
             timeout_ops=timeout_ops,
             comms_return_char=comms_return_char,
             ssh_config_file=ssh_config_file,
             ssh_known_hosts_file=ssh_known_hosts_file,
             on_init=on_init,
```

### Comparing `scrapli-2023.1.30/scrapli/driver/core/cisco_nxos/base_driver.py` & `scrapli-2023.7.30/scrapli/driver/core/cisco_nxos/base_driver.py`

 * *Files identical despite different names*

### Comparing `scrapli-2023.1.30/scrapli/driver/core/cisco_nxos/sync_driver.py` & `scrapli-2023.7.30/scrapli/driver/core/juniper_junos/async_driver.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,68 +1,72 @@
-"""scrapli.driver.core.cisco_nxos.sync_driver"""
+"""scrapli.driver.core.juniper_junos.async_driver"""
 from copy import deepcopy
 from io import BytesIO
 from typing import Any, Callable, Dict, List, Optional, Union
 
-from scrapli.driver import NetworkDriver
-from scrapli.driver.core.cisco_nxos.base_driver import FAILED_WHEN_CONTAINS, PRIVS, NXOSDriverBase
+from scrapli.driver import AsyncNetworkDriver
+from scrapli.driver.core.juniper_junos.base_driver import FAILED_WHEN_CONTAINS, PRIVS
 from scrapli.driver.network.base_driver import PrivilegeLevel
 
 
-def nxos_on_open(conn: NetworkDriver) -> None:
+async def junos_on_open(conn: AsyncNetworkDriver) -> None:
     """
-    NXOSDriver default on_open callable
+    JunosDriver default on_open callable
 
     Args:
         conn: NetworkDriver object
 
     Returns:
         None
 
     Raises:
         N/A
 
     """
-    conn.acquire_priv(desired_priv=conn.default_desired_privilege_level)
-    conn.send_command(command="terminal length 0")
-    conn.send_command(command="terminal width 511")
+    await conn.acquire_priv(desired_priv=conn.default_desired_privilege_level)
+    await conn.send_command(command="set cli screen-length 0")
+    await conn.send_command(command="set cli screen-width 511")
+    await conn.send_command(command="set cli complete-on-space off")
 
 
-def nxos_on_close(conn: NetworkDriver) -> None:
+async def junos_on_close(conn: AsyncNetworkDriver) -> None:
     """
-    NXOSDriver default on_close callable
+    JunosDriver default on_close callable
 
     Args:
         conn: NetworkDriver object
 
     Returns:
         None
 
     Raises:
         N/A
 
     """
-    conn.acquire_priv(desired_priv=conn.default_desired_privilege_level)
+    await conn.acquire_priv(desired_priv=conn.default_desired_privilege_level)
     conn.channel.write(channel_input="exit")
     conn.channel.send_return()
 
 
-class NXOSDriver(NetworkDriver, NXOSDriverBase):
+class AsyncJunosDriver(AsyncNetworkDriver):
     def __init__(
         self,
         host: str,
         privilege_levels: Optional[Dict[str, PrivilegeLevel]] = None,
-        default_desired_privilege_level: str = "privilege_exec",
+        default_desired_privilege_level: str = "exec",
         port: Optional[int] = None,
         auth_username: str = "",
         auth_password: str = "",
         auth_private_key: str = "",
         auth_private_key_passphrase: str = "",
         auth_strict_key: bool = True,
         auth_bypass: bool = False,
+        auth_telnet_login_pattern: str = "",
+        auth_password_pattern: str = "",
+        auth_passphrase_pattern: str = "",
         timeout_socket: float = 15.0,
         timeout_transport: float = 30.0,
         timeout_ops: float = 30.0,
         comms_return_char: str = "\n",
         ssh_config_file: Union[str, bool] = False,
         ssh_known_hosts_file: Union[str, bool] = False,
         on_init: Optional[Callable[..., Any]] = None,
@@ -72,19 +76,19 @@
         transport_options: Optional[Dict[str, Any]] = None,
         channel_log: Union[str, bool, BytesIO] = False,
         channel_log_mode: str = "write",
         channel_lock: bool = False,
         logging_uid: str = "",
         auth_secondary: str = "",
         failed_when_contains: Optional[List[str]] = None,
-        textfsm_platform: str = "cisco_nxos",
-        genie_platform: str = "nxos",
+        textfsm_platform: str = "juniper_junos",
+        genie_platform: str = "",
     ):
         """
-        NXOSDriver Object
+        JunosDriver Object
 
         Please see `scrapli.driver.base.base_driver.Driver` for all "base driver" arguments!
 
         # noqa: DAR101
 
         Args:
              privilege_levels: optional user provided privilege levels, if left None will default to
@@ -109,37 +113,37 @@
         Returns:
             None
 
         Raises:
             N/A
 
         """
-        # somewhere/somehow the mixin is causing mypy to be upset about comms_prompt_pattern...
-        self.comms_prompt_pattern: str
-
         if privilege_levels is None:
             privilege_levels = deepcopy(PRIVS)
 
         if on_open is None:
-            on_open = nxos_on_open
+            on_open = junos_on_open
         if on_close is None:
-            on_close = nxos_on_close
+            on_close = junos_on_close
 
         if failed_when_contains is None:
             failed_when_contains = FAILED_WHEN_CONTAINS.copy()
 
         super().__init__(
             host=host,
             port=port,
             auth_username=auth_username,
             auth_password=auth_password,
             auth_private_key=auth_private_key,
             auth_private_key_passphrase=auth_private_key_passphrase,
             auth_strict_key=auth_strict_key,
             auth_bypass=auth_bypass,
+            auth_telnet_login_pattern=auth_telnet_login_pattern,
+            auth_password_pattern=auth_password_pattern,
+            auth_passphrase_pattern=auth_passphrase_pattern,
             timeout_socket=timeout_socket,
             timeout_transport=timeout_transport,
             timeout_ops=timeout_ops,
             comms_return_char=comms_return_char,
             ssh_config_file=ssh_config_file,
             ssh_known_hosts_file=ssh_known_hosts_file,
             on_init=on_init,
@@ -155,42 +159,23 @@
             default_desired_privilege_level=default_desired_privilege_level,
             auth_secondary=auth_secondary,
             failed_when_contains=failed_when_contains,
             textfsm_platform=textfsm_platform,
             genie_platform=genie_platform,
         )
 
-    def _abort_config(self) -> None:
+    async def _abort_config(self) -> None:
         """
-        Abort NXOS configuration session (if using a config session!)
+        Abort Junos configuration session
 
         Args:
             N/A
 
         Returns:
             None
 
         Raises:
             N/A
 
         """
-        # nxos pattern for config sessions should *always* have `config-s`
-        if "config\\-s" in self._current_priv_level.pattern:
-            self.channel.send_input(channel_input="abort")
-            self._current_priv_level = self.privilege_levels["privilege_exec"]
-
-    def register_configuration_session(self, session_name: str) -> None:
-        """
-        NXOS specific implementation of register_configuration_session
-
-        Args:
-            session_name: name of session to register
-
-        Returns:
-            None
-
-        Raises:
-            N/A
-
-        """
-        self._create_configuration_session(session_name=session_name)
-        self.update_privilege_levels()
+        await self.send_configs(["rollback 0", "exit"])
+        self._current_priv_level = self.privilege_levels["exec"]
```

### Comparing `scrapli-2023.1.30/scrapli/driver/core/juniper_junos/async_driver.py` & `scrapli-2023.7.30/scrapli/driver/core/juniper_junos/sync_driver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,69 +1,72 @@
-"""scrapli.driver.core.juniper_junos.async_driver"""
+"""scrapli.driver.core.juniper_junos.driver"""
 from copy import deepcopy
 from io import BytesIO
 from typing import Any, Callable, Dict, List, Optional, Union
 
-from scrapli.driver import AsyncNetworkDriver
+from scrapli.driver import NetworkDriver
 from scrapli.driver.core.juniper_junos.base_driver import FAILED_WHEN_CONTAINS, PRIVS
 from scrapli.driver.network.base_driver import PrivilegeLevel
 
 
-async def junos_on_open(conn: AsyncNetworkDriver) -> None:
+def junos_on_open(conn: NetworkDriver) -> None:
     """
     JunosDriver default on_open callable
 
     Args:
         conn: NetworkDriver object
 
     Returns:
         None
 
     Raises:
         N/A
 
     """
-    await conn.acquire_priv(desired_priv=conn.default_desired_privilege_level)
-    await conn.send_command(command="set cli screen-length 0")
-    await conn.send_command(command="set cli screen-width 511")
-    await conn.send_command(command="set cli complete-on-space off")
+    conn.acquire_priv(desired_priv=conn.default_desired_privilege_level)
+    conn.send_command(command="set cli screen-length 0")
+    conn.send_command(command="set cli screen-width 511")
+    conn.send_command(command="set cli complete-on-space off")
 
 
-async def junos_on_close(conn: AsyncNetworkDriver) -> None:
+def junos_on_close(conn: NetworkDriver) -> None:
     """
     JunosDriver default on_close callable
 
     Args:
         conn: NetworkDriver object
 
     Returns:
         None
 
     Raises:
         N/A
 
     """
-    await conn.acquire_priv(desired_priv=conn.default_desired_privilege_level)
+    conn.acquire_priv(desired_priv=conn.default_desired_privilege_level)
     conn.channel.write(channel_input="exit")
     conn.channel.send_return()
 
 
-class AsyncJunosDriver(AsyncNetworkDriver):
+class JunosDriver(NetworkDriver):
     def __init__(
         self,
         host: str,
         privilege_levels: Optional[Dict[str, PrivilegeLevel]] = None,
         default_desired_privilege_level: str = "exec",
         port: Optional[int] = None,
         auth_username: str = "",
         auth_password: str = "",
         auth_private_key: str = "",
         auth_private_key_passphrase: str = "",
         auth_strict_key: bool = True,
         auth_bypass: bool = False,
+        auth_telnet_login_pattern: str = "",
+        auth_password_pattern: str = "",
+        auth_passphrase_pattern: str = "",
         timeout_socket: float = 15.0,
         timeout_transport: float = 30.0,
         timeout_ops: float = 30.0,
         comms_return_char: str = "\n",
         ssh_config_file: Union[str, bool] = False,
         ssh_known_hosts_file: Union[str, bool] = False,
         on_init: Optional[Callable[..., Any]] = None,
@@ -74,15 +77,15 @@
         channel_log: Union[str, bool, BytesIO] = False,
         channel_log_mode: str = "write",
         channel_lock: bool = False,
         logging_uid: str = "",
         auth_secondary: str = "",
         failed_when_contains: Optional[List[str]] = None,
         textfsm_platform: str = "juniper_junos",
-        genie_platform: str = "",
+        genie_platform: str = "junos",
     ):
         """
         JunosDriver Object
 
         Please see `scrapli.driver.base.base_driver.Driver` for all "base driver" arguments!
 
         # noqa: DAR101
@@ -100,15 +103,15 @@
                 cases for this callable would be to disable paging or accept any kind of banner
                 message that prompts a user upon connection
             on_close: callable that accepts the class instance as its only argument. this callable,
                 if provided, is executed immediately prior to closing the underlying transport.
                 Common use cases for this callable would be to save configurations prior to exiting,
                 or to logout properly to free up vtys or similar.
             textfsm_platform: string name of textfsm parser platform
-            genie_platform: string name of cisco genie parser platform
+            genie_platform: string name of cisco genie parser platform.  Default: junos
             failed_when_contains: List of strings that indicate a command/config has failed
 
         Returns:
             None
 
         Raises:
             N/A
@@ -130,14 +133,17 @@
             port=port,
             auth_username=auth_username,
             auth_password=auth_password,
             auth_private_key=auth_private_key,
             auth_private_key_passphrase=auth_private_key_passphrase,
             auth_strict_key=auth_strict_key,
             auth_bypass=auth_bypass,
+            auth_telnet_login_pattern=auth_telnet_login_pattern,
+            auth_password_pattern=auth_password_pattern,
+            auth_passphrase_pattern=auth_passphrase_pattern,
             timeout_socket=timeout_socket,
             timeout_transport=timeout_transport,
             timeout_ops=timeout_ops,
             comms_return_char=comms_return_char,
             ssh_config_file=ssh_config_file,
             ssh_known_hosts_file=ssh_known_hosts_file,
             on_init=on_init,
@@ -153,23 +159,23 @@
             default_desired_privilege_level=default_desired_privilege_level,
             auth_secondary=auth_secondary,
             failed_when_contains=failed_when_contains,
             textfsm_platform=textfsm_platform,
             genie_platform=genie_platform,
         )
 
-    async def _abort_config(self) -> None:
+    def _abort_config(self) -> None:
         """
         Abort Junos configuration session
 
         Args:
             N/A
 
         Returns:
             None
 
         Raises:
             N/A
 
         """
-        await self.send_configs(["rollback 0", "exit"])
+        self.send_configs(["rollback 0", "exit"])
         self._current_priv_level = self.privilege_levels["exec"]
```

### Comparing `scrapli-2023.1.30/scrapli/driver/core/juniper_junos/base_driver.py` & `scrapli-2023.7.30/scrapli/driver/core/juniper_junos/base_driver.py`

 * *Files identical despite different names*

### Comparing `scrapli-2023.1.30/scrapli/driver/core/juniper_junos/sync_driver.py` & `scrapli-2023.7.30/scrapli/driver/core/cisco_iosxr/sync_driver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,69 +1,73 @@
-"""scrapli.driver.core.juniper_junos.driver"""
+"""scrapli.driver.core.cisco_iosxr.sync_driver"""
 from copy import deepcopy
 from io import BytesIO
 from typing import Any, Callable, Dict, List, Optional, Union
 
 from scrapli.driver import NetworkDriver
-from scrapli.driver.core.juniper_junos.base_driver import FAILED_WHEN_CONTAINS, PRIVS
+from scrapli.driver.core.cisco_iosxr.base_driver import FAILED_WHEN_CONTAINS, PRIVS
 from scrapli.driver.network.base_driver import PrivilegeLevel
 
 
-def junos_on_open(conn: NetworkDriver) -> None:
+def iosxr_on_open(conn: NetworkDriver) -> None:
     """
-    JunosDriver default on_open callable
+    IOSXRDriver default on_open callable
 
     Args:
         conn: NetworkDriver object
 
     Returns:
         None
 
     Raises:
         N/A
 
     """
     conn.acquire_priv(desired_priv=conn.default_desired_privilege_level)
-    conn.send_command(command="set cli screen-length 0")
-    conn.send_command(command="set cli screen-width 511")
-    conn.send_command(command="set cli complete-on-space off")
+    conn.send_command(command="terminal length 0")
+    conn.send_command(command="terminal width 512")
 
 
-def junos_on_close(conn: NetworkDriver) -> None:
+def iosxr_on_close(conn: NetworkDriver) -> None:
     """
-    JunosDriver default on_close callable
+    IOSXRDriver default on_close callable
 
     Args:
         conn: NetworkDriver object
 
     Returns:
         None
 
     Raises:
         N/A
 
     """
+    # write exit directly to the transport as channel would fail to find the prompt after sending
+    # the exit command!
     conn.acquire_priv(desired_priv=conn.default_desired_privilege_level)
     conn.channel.write(channel_input="exit")
     conn.channel.send_return()
 
 
-class JunosDriver(NetworkDriver):
+class IOSXRDriver(NetworkDriver):
     def __init__(
         self,
         host: str,
         privilege_levels: Optional[Dict[str, PrivilegeLevel]] = None,
-        default_desired_privilege_level: str = "exec",
+        default_desired_privilege_level: str = "privilege_exec",
         port: Optional[int] = None,
         auth_username: str = "",
         auth_password: str = "",
         auth_private_key: str = "",
         auth_private_key_passphrase: str = "",
         auth_strict_key: bool = True,
         auth_bypass: bool = False,
+        auth_telnet_login_pattern: str = "",
+        auth_password_pattern: str = "",
+        auth_passphrase_pattern: str = "",
         timeout_socket: float = 15.0,
         timeout_transport: float = 30.0,
         timeout_ops: float = 30.0,
         comms_return_char: str = "\n",
         ssh_config_file: Union[str, bool] = False,
         ssh_known_hosts_file: Union[str, bool] = False,
         on_init: Optional[Callable[..., Any]] = None,
@@ -73,26 +77,26 @@
         transport_options: Optional[Dict[str, Any]] = None,
         channel_log: Union[str, bool, BytesIO] = False,
         channel_log_mode: str = "write",
         channel_lock: bool = False,
         logging_uid: str = "",
         auth_secondary: str = "",
         failed_when_contains: Optional[List[str]] = None,
-        textfsm_platform: str = "juniper_junos",
-        genie_platform: str = "junos",
+        textfsm_platform: str = "cisco_xr",
+        genie_platform: str = "iosxr",
     ):
         """
-        JunosDriver Object
+        IOSXRDriver Object
 
         Please see `scrapli.driver.base.base_driver.Driver` for all "base driver" arguments!
 
         # noqa: DAR101
 
         Args:
-             privilege_levels: optional user provided privilege levels, if left None will default to
+            privilege_levels: optional user provided privilege levels, if left None will default to
                 scrapli standard privilege levels
             default_desired_privilege_level: string of name of default desired priv, this is the
                 priv level that is generally used to disable paging/set terminal width and things
                 like that upon first login, and is also the priv level scrapli will try to acquire
                 for normal "command" operations (`send_command`, `send_commands`)
             auth_secondary: password to use for secondary authentication (enable)
             on_open: callable that accepts the class instance as its only argument. this callable,
@@ -100,44 +104,47 @@
                 cases for this callable would be to disable paging or accept any kind of banner
                 message that prompts a user upon connection
             on_close: callable that accepts the class instance as its only argument. this callable,
                 if provided, is executed immediately prior to closing the underlying transport.
                 Common use cases for this callable would be to save configurations prior to exiting,
                 or to logout properly to free up vtys or similar.
             textfsm_platform: string name of textfsm parser platform
-            genie_platform: string name of cisco genie parser platform.  Default: junos
+            genie_platform: string name of cisco genie parser platform
             failed_when_contains: List of strings that indicate a command/config has failed
 
         Returns:
             None
 
         Raises:
             N/A
 
         """
         if privilege_levels is None:
             privilege_levels = deepcopy(PRIVS)
 
         if on_open is None:
-            on_open = junos_on_open
+            on_open = iosxr_on_open
         if on_close is None:
-            on_close = junos_on_close
+            on_close = iosxr_on_close
 
         if failed_when_contains is None:
             failed_when_contains = FAILED_WHEN_CONTAINS.copy()
 
         super().__init__(
             host=host,
             port=port,
             auth_username=auth_username,
             auth_password=auth_password,
             auth_private_key=auth_private_key,
             auth_private_key_passphrase=auth_private_key_passphrase,
             auth_strict_key=auth_strict_key,
             auth_bypass=auth_bypass,
+            auth_telnet_login_pattern=auth_telnet_login_pattern,
+            auth_password_pattern=auth_password_pattern,
+            auth_passphrase_pattern=auth_passphrase_pattern,
             timeout_socket=timeout_socket,
             timeout_transport=timeout_transport,
             timeout_ops=timeout_ops,
             comms_return_char=comms_return_char,
             ssh_config_file=ssh_config_file,
             ssh_known_hosts_file=ssh_known_hosts_file,
             on_init=on_init,
@@ -155,21 +162,21 @@
             failed_when_contains=failed_when_contains,
             textfsm_platform=textfsm_platform,
             genie_platform=genie_platform,
         )
 
     def _abort_config(self) -> None:
         """
-        Abort Junos configuration session
+        Abort IOSXR configuration session
 
         Args:
             N/A
 
         Returns:
             None
 
         Raises:
             N/A
 
         """
-        self.send_configs(["rollback 0", "exit"])
-        self._current_priv_level = self.privilege_levels["exec"]
+        self.channel.send_input(channel_input="abort")
+        self._current_priv_level = self.privilege_levels["privilege_exec"]
```

### Comparing `scrapli-2023.1.30/scrapli/driver/generic/async_driver.py` & `scrapli-2023.7.30/scrapli/driver/generic/sync_driver.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,39 @@
-"""scrapli.driver.generic.async_driver"""
-import asyncio
+"""scrapli.driver.generic.sync_driver"""
+import time
 from io import BytesIO
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Union
 
 from scrapli.decorators import timeout_modifier
-from scrapli.driver import AsyncDriver
+from scrapli.driver import Driver
 from scrapli.driver.generic.base_driver import BaseGenericDriver
 from scrapli.exceptions import ScrapliTimeout, ScrapliValueError
 from scrapli.response import MultiResponse, Response
 
 if TYPE_CHECKING:
     from scrapli.driver.generic.base_driver import (  # pragma:  no cover
         ReadCallback,
         ReadCallbackReturnable,
     )
 
 
-class AsyncGenericDriver(AsyncDriver, BaseGenericDriver):
+class GenericDriver(Driver, BaseGenericDriver):
     def __init__(
         self,
         host: str,
         port: Optional[int] = None,
         auth_username: str = "",
         auth_password: str = "",
         auth_private_key: str = "",
         auth_private_key_passphrase: str = "",
         auth_strict_key: bool = True,
         auth_bypass: bool = False,
+        auth_telnet_login_pattern: str = "",
+        auth_password_pattern: str = "",
+        auth_passphrase_pattern: str = "",
         timeout_socket: float = 15.0,
         timeout_transport: float = 30.0,
         timeout_ops: float = 30.0,
         comms_prompt_pattern: str = r"^\S{0,48}[#>$~@:\]]\s*$",
         comms_return_char: str = "\n",
         ssh_config_file: Union[str, bool] = False,
         ssh_known_hosts_file: Union[str, bool] = False,
@@ -49,14 +52,17 @@
             port=port,
             auth_username=auth_username,
             auth_password=auth_password,
             auth_private_key=auth_private_key,
             auth_private_key_passphrase=auth_private_key_passphrase,
             auth_strict_key=auth_strict_key,
             auth_bypass=auth_bypass,
+            auth_telnet_login_pattern=auth_telnet_login_pattern,
+            auth_password_pattern=auth_password_pattern,
+            auth_passphrase_pattern=auth_passphrase_pattern,
             timeout_socket=timeout_socket,
             timeout_transport=timeout_transport,
             timeout_ops=timeout_ops,
             comms_prompt_pattern=comms_prompt_pattern,
             comms_return_char=comms_return_char,
             ssh_config_file=ssh_config_file,
             ssh_known_hosts_file=ssh_known_hosts_file,
@@ -67,33 +73,34 @@
             transport_options=transport_options,
             channel_log=channel_log,
             channel_log_mode=channel_log_mode,
             channel_lock=channel_lock,
             logging_uid=logging_uid,
         )
 
-    async def get_prompt(self) -> str:
+    def get_prompt(self) -> str:
         """
         Convenience method to fetch prompt from the underlying Channel object
 
         Args:
             N/A
 
         Returns:
             str: string of the current prompt
 
         Raises:
             N/A
 
         """
-        prompt: str = await self.channel.get_prompt()
+        # assigned/typed here as decorator indicates return of Any
+        prompt: str = self.channel.get_prompt()
         return prompt
 
     @timeout_modifier
-    async def _send_command(
+    def _send_command(
         self,
         command: str,
         strip_prompt: bool = True,
         failed_when_contains: Optional[Union[str, List[str]]] = None,
         eager: bool = False,
         timeout_ops: Optional[float] = None,
     ) -> Response:
@@ -130,22 +137,22 @@
             raise ScrapliValueError("driver _base_transport_args not set for some reason")
 
         response = self._pre_send_command(
             host=self._base_transport_args.host,
             command=command,
             failed_when_contains=failed_when_contains,
         )
-        raw_response, processed_response = await self.channel.send_input(
+        raw_response, processed_response = self.channel.send_input(
             channel_input=command, strip_prompt=strip_prompt, eager=eager
         )
         return self._post_send_command(
             raw_response=raw_response, processed_response=processed_response, response=response
         )
 
-    async def send_command(
+    def send_command(
         self,
         command: str,
         *,
         strip_prompt: bool = True,
         failed_when_contains: Optional[Union[str, List[str]]] = None,
         timeout_ops: Optional[float] = None,
     ) -> Response:
@@ -163,23 +170,23 @@
         Returns:
             Response: Scrapli Response object
 
         Raises:
             N/A
 
         """
-        response: Response = await self._send_command(
+        response: Response = self._send_command(
             command=command,
             strip_prompt=strip_prompt,
             failed_when_contains=failed_when_contains,
             timeout_ops=timeout_ops,
         )
         return response
 
-    async def send_commands(
+    def send_commands(
         self,
         commands: List[str],
         *,
         strip_prompt: bool = True,
         failed_when_contains: Optional[Union[str, List[str]]] = None,
         stop_on_failed: bool = False,
         eager: bool = False,
@@ -207,41 +214,41 @@
 
         Raises:
             N/A
 
         """
         responses = self._pre_send_commands(commands=commands)
         for command in commands[:-1]:
-            response = await self._send_command(
+            response = self._send_command(
                 command=command,
                 strip_prompt=strip_prompt,
                 failed_when_contains=failed_when_contains,
                 timeout_ops=timeout_ops,
                 eager=eager,
             )
             responses.append(response)
             if stop_on_failed and response.failed is True:
                 # should we find the prompt here w/ get_prompt?? or just let subsequent operations
                 # deal w/ finding that? future us problem? :)
                 break
         else:
             # if we did *not* break (i.e. no failure and/or no stop_on_failed) send the last command
             # with eager = False -- this way we *always* find the prompt at the end of the commands
-            response = await self._send_command(
+            response = self._send_command(
                 command=commands[-1],
                 strip_prompt=strip_prompt,
                 failed_when_contains=failed_when_contains,
                 timeout_ops=timeout_ops,
                 eager=False,
             )
             responses.append(response)
 
         return responses
 
-    async def send_commands_from_file(
+    def send_commands_from_file(
         self,
         file: str,
         *,
         strip_prompt: bool = True,
         failed_when_contains: Optional[Union[str, List[str]]] = None,
         stop_on_failed: bool = False,
         eager: bool = False,
@@ -269,25 +276,25 @@
 
         Raises:
             N/A
 
         """
         commands = self._pre_send_from_file(file=file, caller="send_commands_from_file")
 
-        return await self.send_commands(
+        return self.send_commands(
             commands=commands,
             strip_prompt=strip_prompt,
             failed_when_contains=failed_when_contains,
             stop_on_failed=stop_on_failed,
             eager=eager,
             timeout_ops=timeout_ops,
         )
 
     @timeout_modifier
-    async def send_and_read(
+    def send_and_read(
         self,
         channel_input: str,
         *,
         expected_outputs: Optional[List[str]] = None,
         strip_prompt: bool = True,
         failed_when_contains: Optional[Union[str, List[str]]] = None,
         timeout_ops: Optional[float] = None,
@@ -328,26 +335,26 @@
             raise ScrapliValueError("driver _base_transport_args not set for some reason")
 
         response = self._pre_send_command(
             host=self._base_transport_args.host,
             command=channel_input,
             failed_when_contains=failed_when_contains,
         )
-        raw_response, processed_response = await self.channel.send_input_and_read(
+        raw_response, processed_response = self.channel.send_input_and_read(
             channel_input=channel_input,
             strip_prompt=strip_prompt,
             expected_outputs=expected_outputs,
             read_duration=read_duration,
         )
         return self._post_send_command(
             raw_response=raw_response, processed_response=processed_response, response=response
         )
 
     @timeout_modifier
-    async def send_interactive(
+    def send_interactive(
         self,
         interact_events: Union[List[Tuple[str, str]], List[Tuple[str, str, bool]]],
         *,
         failed_when_contains: Optional[Union[str, List[str]]] = None,
         privilege_level: str = "",
         timeout_ops: Optional[float] = None,
         interaction_complete_patterns: Optional[List[str]] = None,
@@ -430,23 +437,23 @@
             raise ScrapliValueError("driver _base_transport_args not set for some reason")
 
         response = self._pre_send_interactive(
             host=self._base_transport_args.host,
             interact_events=interact_events,
             failed_when_contains=failed_when_contains,
         )
-        raw_response, processed_response = await self.channel.send_inputs_interact(
+        raw_response, processed_response = self.channel.send_inputs_interact(
             interact_events=interact_events,
             interaction_complete_patterns=interaction_complete_patterns,
         )
         return self._post_send_command(
             raw_response=raw_response, processed_response=processed_response, response=response
         )
 
-    async def read_callback(  # noqa: C901
+    def read_callback(
         self,
         callbacks: List["ReadCallback"],
         initial_input: Optional[str] = None,
         read_output: bytes = b"",
         read_delay: float = 0.1,
         read_timeout: float = -1.0,
     ) -> "ReadCallbackReturnable":
@@ -520,27 +527,27 @@
         Raises:
             ScrapliTimeout: if the read operation times out (base don the read_timeout value) during
                 the read callback check.
 
         """
         if initial_input is not None:
             self.channel.write(channel_input=f"{initial_input}{self.comms_return_char}")
-            return await self.read_callback(callbacks=callbacks, initial_input=None)
+            return self.read_callback(callbacks=callbacks, initial_input=None)
 
         original_transport_timeout = self.timeout_transport
 
         # if the read_timeout value is -1.0 or just less than 0, that indicates we should use
         # the "normal" transport timeout and not modify anything
         self.timeout_transport = read_timeout if read_timeout >= 0 else self.timeout_transport
 
         _read_delay = 0.1 if read_delay <= 0 else read_delay
 
         while True:
             try:
-                read_output += await self.channel.read()
+                read_output += self.channel.read()
             except ScrapliTimeout as exc:
                 self.timeout_transport = original_transport_timeout
 
                 raise ScrapliTimeout("timeout during read in read_callback operation") from exc
 
             for callback in callbacks:
                 _run_callback = callback.check(read_output=read_output)
@@ -557,28 +564,25 @@
                     continue
 
                 if _run_callback is True:
                     self.logger.info(f"callback {callback.name} matched, executing")
 
                     self.timeout_transport = original_transport_timeout
 
-                    coro = callback.run(driver=self)
-                    if coro is not None:
-                        # should always be a coroutine in this case, this appeases mypy
-                        await coro
+                    callback.run(driver=self)
 
                     if callback.complete:
                         self.logger.debug("callback complete is true, done with read_callback")
                         return None
 
                     if callback.reset_output:
                         read_output = b""
 
-                    return await self.read_callback(
+                    return self.read_callback(
                         callbacks=callbacks,
                         initial_input=None,
                         read_output=read_output,
                         read_delay=callback.next_delay,
                         read_timeout=callback.next_timeout,
                     )
 
-            await asyncio.sleep(_read_delay)
+            time.sleep(_read_delay)
```

### Comparing `scrapli-2023.1.30/scrapli/driver/generic/base_driver.py` & `scrapli-2023.7.30/scrapli/driver/generic/base_driver.py`

 * *Files identical despite different names*

### Comparing `scrapli-2023.1.30/scrapli/driver/generic/sync_driver.py` & `scrapli-2023.7.30/scrapli/driver/generic/async_driver.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,39 @@
-"""scrapli.driver.generic.sync_driver"""
-import time
+"""scrapli.driver.generic.async_driver"""
+import asyncio
 from io import BytesIO
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Union
 
 from scrapli.decorators import timeout_modifier
-from scrapli.driver import Driver
+from scrapli.driver import AsyncDriver
 from scrapli.driver.generic.base_driver import BaseGenericDriver
 from scrapli.exceptions import ScrapliTimeout, ScrapliValueError
 from scrapli.response import MultiResponse, Response
 
 if TYPE_CHECKING:
     from scrapli.driver.generic.base_driver import (  # pragma:  no cover
         ReadCallback,
         ReadCallbackReturnable,
     )
 
 
-class GenericDriver(Driver, BaseGenericDriver):
+class AsyncGenericDriver(AsyncDriver, BaseGenericDriver):
     def __init__(
         self,
         host: str,
         port: Optional[int] = None,
         auth_username: str = "",
         auth_password: str = "",
         auth_private_key: str = "",
         auth_private_key_passphrase: str = "",
         auth_strict_key: bool = True,
         auth_bypass: bool = False,
+        auth_telnet_login_pattern: str = "",
+        auth_password_pattern: str = "",
+        auth_passphrase_pattern: str = "",
         timeout_socket: float = 15.0,
         timeout_transport: float = 30.0,
         timeout_ops: float = 30.0,
         comms_prompt_pattern: str = r"^\S{0,48}[#>$~@:\]]\s*$",
         comms_return_char: str = "\n",
         ssh_config_file: Union[str, bool] = False,
         ssh_known_hosts_file: Union[str, bool] = False,
@@ -49,14 +52,17 @@
             port=port,
             auth_username=auth_username,
             auth_password=auth_password,
             auth_private_key=auth_private_key,
             auth_private_key_passphrase=auth_private_key_passphrase,
             auth_strict_key=auth_strict_key,
             auth_bypass=auth_bypass,
+            auth_telnet_login_pattern=auth_telnet_login_pattern,
+            auth_password_pattern=auth_password_pattern,
+            auth_passphrase_pattern=auth_passphrase_pattern,
             timeout_socket=timeout_socket,
             timeout_transport=timeout_transport,
             timeout_ops=timeout_ops,
             comms_prompt_pattern=comms_prompt_pattern,
             comms_return_char=comms_return_char,
             ssh_config_file=ssh_config_file,
             ssh_known_hosts_file=ssh_known_hosts_file,
@@ -67,34 +73,33 @@
             transport_options=transport_options,
             channel_log=channel_log,
             channel_log_mode=channel_log_mode,
             channel_lock=channel_lock,
             logging_uid=logging_uid,
         )
 
-    def get_prompt(self) -> str:
+    async def get_prompt(self) -> str:
         """
         Convenience method to fetch prompt from the underlying Channel object
 
         Args:
             N/A
 
         Returns:
             str: string of the current prompt
 
         Raises:
             N/A
 
         """
-        # assigned/typed here as decorator indicates return of Any
-        prompt: str = self.channel.get_prompt()
+        prompt: str = await self.channel.get_prompt()
         return prompt
 
     @timeout_modifier
-    def _send_command(
+    async def _send_command(
         self,
         command: str,
         strip_prompt: bool = True,
         failed_when_contains: Optional[Union[str, List[str]]] = None,
         eager: bool = False,
         timeout_ops: Optional[float] = None,
     ) -> Response:
@@ -131,22 +136,22 @@
             raise ScrapliValueError("driver _base_transport_args not set for some reason")
 
         response = self._pre_send_command(
             host=self._base_transport_args.host,
             command=command,
             failed_when_contains=failed_when_contains,
         )
-        raw_response, processed_response = self.channel.send_input(
+        raw_response, processed_response = await self.channel.send_input(
             channel_input=command, strip_prompt=strip_prompt, eager=eager
         )
         return self._post_send_command(
             raw_response=raw_response, processed_response=processed_response, response=response
         )
 
-    def send_command(
+    async def send_command(
         self,
         command: str,
         *,
         strip_prompt: bool = True,
         failed_when_contains: Optional[Union[str, List[str]]] = None,
         timeout_ops: Optional[float] = None,
     ) -> Response:
@@ -164,23 +169,23 @@
         Returns:
             Response: Scrapli Response object
 
         Raises:
             N/A
 
         """
-        response: Response = self._send_command(
+        response: Response = await self._send_command(
             command=command,
             strip_prompt=strip_prompt,
             failed_when_contains=failed_when_contains,
             timeout_ops=timeout_ops,
         )
         return response
 
-    def send_commands(
+    async def send_commands(
         self,
         commands: List[str],
         *,
         strip_prompt: bool = True,
         failed_when_contains: Optional[Union[str, List[str]]] = None,
         stop_on_failed: bool = False,
         eager: bool = False,
@@ -208,41 +213,41 @@
 
         Raises:
             N/A
 
         """
         responses = self._pre_send_commands(commands=commands)
         for command in commands[:-1]:
-            response = self._send_command(
+            response = await self._send_command(
                 command=command,
                 strip_prompt=strip_prompt,
                 failed_when_contains=failed_when_contains,
                 timeout_ops=timeout_ops,
                 eager=eager,
             )
             responses.append(response)
             if stop_on_failed and response.failed is True:
                 # should we find the prompt here w/ get_prompt?? or just let subsequent operations
                 # deal w/ finding that? future us problem? :)
                 break
         else:
             # if we did *not* break (i.e. no failure and/or no stop_on_failed) send the last command
             # with eager = False -- this way we *always* find the prompt at the end of the commands
-            response = self._send_command(
+            response = await self._send_command(
                 command=commands[-1],
                 strip_prompt=strip_prompt,
                 failed_when_contains=failed_when_contains,
                 timeout_ops=timeout_ops,
                 eager=False,
             )
             responses.append(response)
 
         return responses
 
-    def send_commands_from_file(
+    async def send_commands_from_file(
         self,
         file: str,
         *,
         strip_prompt: bool = True,
         failed_when_contains: Optional[Union[str, List[str]]] = None,
         stop_on_failed: bool = False,
         eager: bool = False,
@@ -270,25 +275,25 @@
 
         Raises:
             N/A
 
         """
         commands = self._pre_send_from_file(file=file, caller="send_commands_from_file")
 
-        return self.send_commands(
+        return await self.send_commands(
             commands=commands,
             strip_prompt=strip_prompt,
             failed_when_contains=failed_when_contains,
             stop_on_failed=stop_on_failed,
             eager=eager,
             timeout_ops=timeout_ops,
         )
 
     @timeout_modifier
-    def send_and_read(
+    async def send_and_read(
         self,
         channel_input: str,
         *,
         expected_outputs: Optional[List[str]] = None,
         strip_prompt: bool = True,
         failed_when_contains: Optional[Union[str, List[str]]] = None,
         timeout_ops: Optional[float] = None,
@@ -329,26 +334,26 @@
             raise ScrapliValueError("driver _base_transport_args not set for some reason")
 
         response = self._pre_send_command(
             host=self._base_transport_args.host,
             command=channel_input,
             failed_when_contains=failed_when_contains,
         )
-        raw_response, processed_response = self.channel.send_input_and_read(
+        raw_response, processed_response = await self.channel.send_input_and_read(
             channel_input=channel_input,
             strip_prompt=strip_prompt,
             expected_outputs=expected_outputs,
             read_duration=read_duration,
         )
         return self._post_send_command(
             raw_response=raw_response, processed_response=processed_response, response=response
         )
 
     @timeout_modifier
-    def send_interactive(
+    async def send_interactive(
         self,
         interact_events: Union[List[Tuple[str, str]], List[Tuple[str, str, bool]]],
         *,
         failed_when_contains: Optional[Union[str, List[str]]] = None,
         privilege_level: str = "",
         timeout_ops: Optional[float] = None,
         interaction_complete_patterns: Optional[List[str]] = None,
@@ -431,23 +436,23 @@
             raise ScrapliValueError("driver _base_transport_args not set for some reason")
 
         response = self._pre_send_interactive(
             host=self._base_transport_args.host,
             interact_events=interact_events,
             failed_when_contains=failed_when_contains,
         )
-        raw_response, processed_response = self.channel.send_inputs_interact(
+        raw_response, processed_response = await self.channel.send_inputs_interact(
             interact_events=interact_events,
             interaction_complete_patterns=interaction_complete_patterns,
         )
         return self._post_send_command(
             raw_response=raw_response, processed_response=processed_response, response=response
         )
 
-    def read_callback(
+    async def read_callback(  # noqa: C901
         self,
         callbacks: List["ReadCallback"],
         initial_input: Optional[str] = None,
         read_output: bytes = b"",
         read_delay: float = 0.1,
         read_timeout: float = -1.0,
     ) -> "ReadCallbackReturnable":
@@ -521,27 +526,27 @@
         Raises:
             ScrapliTimeout: if the read operation times out (base don the read_timeout value) during
                 the read callback check.
 
         """
         if initial_input is not None:
             self.channel.write(channel_input=f"{initial_input}{self.comms_return_char}")
-            return self.read_callback(callbacks=callbacks, initial_input=None)
+            return await self.read_callback(callbacks=callbacks, initial_input=None)
 
         original_transport_timeout = self.timeout_transport
 
         # if the read_timeout value is -1.0 or just less than 0, that indicates we should use
         # the "normal" transport timeout and not modify anything
         self.timeout_transport = read_timeout if read_timeout >= 0 else self.timeout_transport
 
         _read_delay = 0.1 if read_delay <= 0 else read_delay
 
         while True:
             try:
-                read_output += self.channel.read()
+                read_output += await self.channel.read()
             except ScrapliTimeout as exc:
                 self.timeout_transport = original_transport_timeout
 
                 raise ScrapliTimeout("timeout during read in read_callback operation") from exc
 
             for callback in callbacks:
                 _run_callback = callback.check(read_output=read_output)
@@ -558,25 +563,28 @@
                     continue
 
                 if _run_callback is True:
                     self.logger.info(f"callback {callback.name} matched, executing")
 
                     self.timeout_transport = original_transport_timeout
 
-                    callback.run(driver=self)
+                    coro = callback.run(driver=self)
+                    if coro is not None:
+                        # should always be a coroutine in this case, this appeases mypy
+                        await coro
 
                     if callback.complete:
                         self.logger.debug("callback complete is true, done with read_callback")
                         return None
 
                     if callback.reset_output:
                         read_output = b""
 
-                    return self.read_callback(
+                    return await self.read_callback(
                         callbacks=callbacks,
                         initial_input=None,
                         read_output=read_output,
                         read_delay=callback.next_delay,
                         read_timeout=callback.next_timeout,
                     )
 
-            time.sleep(_read_delay)
+            await asyncio.sleep(_read_delay)
```

### Comparing `scrapli-2023.1.30/scrapli/driver/network/async_driver.py` & `scrapli-2023.7.30/scrapli/driver/network/async_driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,17 @@
         port: Optional[int] = None,
         auth_username: str = "",
         auth_password: str = "",
         auth_private_key: str = "",
         auth_private_key_passphrase: str = "",
         auth_strict_key: bool = True,
         auth_bypass: bool = False,
+        auth_telnet_login_pattern: str = "",
+        auth_password_pattern: str = "",
+        auth_passphrase_pattern: str = "",
         timeout_socket: float = 15.0,
         timeout_transport: float = 30.0,
         timeout_ops: float = 30.0,
         comms_return_char: str = "\n",
         ssh_config_file: Union[str, bool] = False,
         ssh_known_hosts_file: Union[str, bool] = False,
         on_init: Optional[Callable[..., Any]] = None,
@@ -50,14 +53,17 @@
             port=port,
             auth_username=auth_username,
             auth_password=auth_password,
             auth_private_key=auth_private_key,
             auth_private_key_passphrase=auth_private_key_passphrase,
             auth_strict_key=auth_strict_key,
             auth_bypass=auth_bypass,
+            auth_telnet_login_pattern=auth_telnet_login_pattern,
+            auth_password_pattern=auth_password_pattern,
+            auth_passphrase_pattern=auth_passphrase_pattern,
             timeout_socket=timeout_socket,
             timeout_transport=timeout_transport,
             timeout_ops=timeout_ops,
             comms_return_char=comms_return_char,
             ssh_config_file=ssh_config_file,
             ssh_known_hosts_file=ssh_known_hosts_file,
             on_init=on_init,
```

### Comparing `scrapli-2023.1.30/scrapli/driver/network/base_driver.py` & `scrapli-2023.7.30/scrapli/driver/network/base_driver.py`

 * *Files identical despite different names*

### Comparing `scrapli-2023.1.30/scrapli/driver/network/sync_driver.py` & `scrapli-2023.7.30/scrapli/driver/network/sync_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,17 @@
         port: Optional[int] = None,
         auth_username: str = "",
         auth_password: str = "",
         auth_private_key: str = "",
         auth_private_key_passphrase: str = "",
         auth_strict_key: bool = True,
         auth_bypass: bool = False,
+        auth_telnet_login_pattern: str = "",
+        auth_password_pattern: str = "",
+        auth_passphrase_pattern: str = "",
         timeout_socket: float = 15.0,
         timeout_transport: float = 30.0,
         timeout_ops: float = 30.0,
         comms_return_char: str = "\n",
         ssh_config_file: Union[str, bool] = False,
         ssh_known_hosts_file: Union[str, bool] = False,
         on_init: Optional[Callable[..., Any]] = None,
@@ -50,14 +53,17 @@
             port=port,
             auth_username=auth_username,
             auth_password=auth_password,
             auth_private_key=auth_private_key,
             auth_private_key_passphrase=auth_private_key_passphrase,
             auth_strict_key=auth_strict_key,
             auth_bypass=auth_bypass,
+            auth_telnet_login_pattern=auth_telnet_login_pattern,
+            auth_password_pattern=auth_password_pattern,
+            auth_passphrase_pattern=auth_passphrase_pattern,
             timeout_socket=timeout_socket,
             timeout_transport=timeout_transport,
             timeout_ops=timeout_ops,
             comms_return_char=comms_return_char,
             ssh_config_file=ssh_config_file,
             ssh_known_hosts_file=ssh_known_hosts_file,
             on_init=on_init,
```

### Comparing `scrapli-2023.1.30/scrapli/exceptions.py` & `scrapli-2023.7.30/scrapli/exceptions.py`

 * *Files identical despite different names*

### Comparing `scrapli-2023.1.30/scrapli/factory.py` & `scrapli-2023.7.30/scrapli/factory.py`

 * *Files identical despite different names*

### Comparing `scrapli-2023.1.30/scrapli/helper.py` & `scrapli-2023.7.30/scrapli/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import urllib.request
 from io import BytesIO, TextIOWrapper
 from pathlib import Path
 from shutil import get_terminal_size
 from typing import Any, Dict, List, Optional, TextIO, Union
 from warnings import warn
 
-import pkg_resources  # pylint: disable=C0411
+import pkg_resources
 
 from scrapli.exceptions import ScrapliValueError
 from scrapli.logging import logger
 from scrapli.settings import Settings
 
 
 def _textfsm_get_template(platform: str, command: str) -> Optional[TextIO]:
```

### Comparing `scrapli-2023.1.30/scrapli/logging.py` & `scrapli-2023.7.30/scrapli/logging.py`

 * *Files identical despite different names*

### Comparing `scrapli-2023.1.30/scrapli/response.py` & `scrapli-2023.7.30/scrapli/response.py`

 * *Files identical despite different names*

### Comparing `scrapli-2023.1.30/scrapli/ssh_config.py` & `scrapli-2023.7.30/scrapli/ssh_config.py`

 * *Files identical despite different names*

### Comparing `scrapli-2023.1.30/scrapli/transport/base/async_transport.py` & `scrapli-2023.7.30/scrapli/transport/base/async_transport.py`

 * *Files identical despite different names*

### Comparing `scrapli-2023.1.30/scrapli/transport/base/base_socket.py` & `scrapli-2023.7.30/scrapli/transport/base/base_socket.py`

 * *Files identical despite different names*

### Comparing `scrapli-2023.1.30/scrapli/transport/base/base_transport.py` & `scrapli-2023.7.30/scrapli/transport/base/base_transport.py`

 * *Files identical despite different names*

### Comparing `scrapli-2023.1.30/scrapli/transport/base/sync_transport.py` & `scrapli-2023.7.30/scrapli/transport/base/sync_transport.py`

 * *Files identical despite different names*

### Comparing `scrapli-2023.1.30/scrapli/transport/plugins/asyncssh/transport.py` & `scrapli-2023.7.30/scrapli/transport/plugins/asyncssh/transport.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,14 @@
 
         self._post_open_closing_log(closing=False)
 
     def close(self) -> None:
         self._pre_open_closing_log(closing=True)
 
         if self.session:
-
             with suppress(BrokenPipeError):
                 # this may raise a BrokenPipeError because seems it is possible for the connection
                 # transport is_closing() to be true already in some cases... since we are closing
                 # the connection anyway we will just ignore this note that this seemed to only
                 # happen in github actions on ubuntu-latest w/ py3.8... hence the suppress!
                 self.session.close()
```

### Comparing `scrapli-2023.1.30/scrapli/transport/plugins/asynctelnet/transport.py` & `scrapli-2023.7.30/scrapli/transport/plugins/asynctelnet/transport.py`

 * *Files identical despite different names*

### Comparing `scrapli-2023.1.30/scrapli/transport/plugins/paramiko/transport.py` & `scrapli-2023.7.30/scrapli/transport/plugins/paramiko/transport.py`

 * *Files identical despite different names*

### Comparing `scrapli-2023.1.30/scrapli/transport/plugins/ssh2/transport.py` & `scrapli-2023.7.30/scrapli/transport/plugins/ssh2/transport.py`

 * *Files identical despite different names*

### Comparing `scrapli-2023.1.30/scrapli/transport/plugins/system/ptyprocess.py` & `scrapli-2023.7.30/scrapli/transport/plugins/system/ptyprocess.py`

 * *Files identical despite different names*

### Comparing `scrapli-2023.1.30/scrapli/transport/plugins/system/transport.py` & `scrapli-2023.7.30/scrapli/transport/plugins/system/transport.py`

 * *Files identical despite different names*

### Comparing `scrapli-2023.1.30/scrapli/transport/plugins/telnet/transport.py` & `scrapli-2023.7.30/scrapli/transport/plugins/telnet/transport.py`

 * *Files identical despite different names*

### Comparing `scrapli-2023.1.30/scrapli.egg-info/PKG-INFO` & `scrapli-2023.7.30/scrapli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapli
-Version: 2023.1.30
+Version: 2023.7.30
 Summary: Fast, flexible, sync/async, Python 3.7+ screen scraping client specifically for network devices
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
         
-Project-URL: Homepage, https://github.com/carlmontanari/scrapli
 Project-URL: Changelog, https://carlmontanari.github.io/scrapli/changelog
 Project-URL: Docs, https://carlmontanari.github.io/scrapli/
-Keywords: ssh,telnet,netconf,automation,network,cisco,iosxr,iosxe,nxos,arista,eos,juniper,junos
+Project-URL: Homepage, https://github.com/carlmontanari/scrapli
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
-Metadata-Version: 2.1 Name: scrapli Version: 2023.1.30 Summary: Fast, flexible,
+Metadata-Version: 2.1 Name: scrapli Version: 2023.7.30 Summary: Fast, flexible,
 sync/async, Python 3.7+ screen scraping client specifically for network devices
 Author-email: Carl Montanari
 r.montanari@gmail.com> License: MIT License Copyright (c) 2021 Carl Montanari
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
@@ -11,19 +11,19 @@
 permission notice shall be included in all copies or substantial portions of
 the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
 EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
 OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://github.com/
-carlmontanari/scrapli Project-URL: Changelog, https://carlmontanari.github.io/
-scrapli/changelog Project-URL: Docs, https://carlmontanari.github.io/scrapli/
-Keywords:
-ssh,telnet,netconf,automation,network,cisco,iosxr,iosxe,nxos,arista,eos,juniper,junos
+DEALINGS IN THE SOFTWARE. Project-URL: Changelog, https://
+carlmontanari.github.io/scrapli/changelog Project-URL: Docs, https://
+carlmontanari.github.io/scrapli/ Project-URL: Homepage, https://github.com/
+carlmontanari/scrapli Keywords:
+arista,automation,cisco,eos,iosxe,iosxr,juniper,junos,netconf,network,nxos,ssh,telnet
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: POSIX :: Linux Classifier: Operating System :: MacOS Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Topic :: Software Development ::
```

### Comparing `scrapli-2023.1.30/scrapli.egg-info/SOURCES.txt` & `scrapli-2023.7.30/scrapli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

