# Comparing `tmp/scrapli_netconf-2023.1.30.tar.gz` & `tmp/scrapli_netconf-2023.7.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapli_netconf-2023.1.30.tar", last modified: Sat Jan 28 19:26:20 2023, max compression
+gzip compressed data, was "scrapli_netconf-2023.7.30.tar", last modified: Sun Jul 30 17:04:55 2023, max compression
```

## Comparing `scrapli_netconf-2023.1.30.tar` & `scrapli_netconf-2023.7.30.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 19:26:20.139973 scrapli_netconf-2023.1.30/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-01-28 19:26:05.000000 scrapli_netconf-2023.1.30/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-28 19:26:05.000000 scrapli_netconf-2023.1.30/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-01-28 19:26:20.139973 scrapli_netconf-2023.1.30/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-01-28 19:26:05.000000 scrapli_netconf-2023.1.30/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-01-28 19:26:05.000000 scrapli_netconf-2023.1.30/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-28 19:26:05.000000 scrapli_netconf-2023.1.30/requirements-asyncssh.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-01-28 19:26:05.000000 scrapli_netconf-2023.1.30/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-01-28 19:26:05.000000 scrapli_netconf-2023.1.30/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-28 19:26:05.000000 scrapli_netconf-2023.1.30/requirements-paramiko.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-28 19:26:05.000000 scrapli_netconf-2023.1.30/requirements-ssh2.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-28 19:26:05.000000 scrapli_netconf-2023.1.30/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 19:26:20.135974 scrapli_netconf-2023.1.30/scrapli_netconf/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-01-28 19:26:05.000000 scrapli_netconf-2023.1.30/scrapli_netconf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 19:26:20.135974 scrapli_netconf-2023.1.30/scrapli_netconf/channel/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-01-28 19:26:05.000000 scrapli_netconf-2023.1.30/scrapli_netconf/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-01-28 19:26:05.000000 scrapli_netconf-2023.1.30/scrapli_netconf/channel/async_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-01-28 19:26:05.000000 scrapli_netconf-2023.1.30/scrapli_netconf/channel/base_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    12796 2023-01-28 19:26:05.000000 scrapli_netconf-2023.1.30/scrapli_netconf/channel/sync_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-01-28 19:26:05.000000 scrapli_netconf-2023.1.30/scrapli_netconf/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 19:26:20.139973 scrapli_netconf-2023.1.30/scrapli_netconf/driver/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-01-28 19:26:05.000000 scrapli_netconf-2023.1.30/scrapli_netconf/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-01-28 19:26:05.000000 scrapli_netconf-2023.1.30/scrapli_netconf/driver/async_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    40546 2023-01-28 19:26:05.000000 scrapli_netconf-2023.1.30/scrapli_netconf/driver/base_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    12015 2023-01-28 19:26:05.000000 scrapli_netconf-2023.1.30/scrapli_netconf/driver/sync_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-01-28 19:26:05.000000 scrapli_netconf-2023.1.30/scrapli_netconf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-01-28 19:26:05.000000 scrapli_netconf-2023.1.30/scrapli_netconf/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-28 19:26:05.000000 scrapli_netconf-2023.1.30/scrapli_netconf/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-01-28 19:26:05.000000 scrapli_netconf-2023.1.30/scrapli_netconf/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 19:26:20.139973 scrapli_netconf-2023.1.30/scrapli_netconf/transport/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-28 19:26:05.000000 scrapli_netconf-2023.1.30/scrapli_netconf/transport/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 19:26:20.139973 scrapli_netconf-2023.1.30/scrapli_netconf/transport/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-01-28 19:26:05.000000 scrapli_netconf-2023.1.30/scrapli_netconf/transport/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 19:26:20.139973 scrapli_netconf-2023.1.30/scrapli_netconf/transport/plugins/asyncssh/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-28 19:26:05.000000 scrapli_netconf-2023.1.30/scrapli_netconf/transport/plugins/asyncssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-01-28 19:26:05.000000 scrapli_netconf-2023.1.30/scrapli_netconf/transport/plugins/asyncssh/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 19:26:20.139973 scrapli_netconf-2023.1.30/scrapli_netconf/transport/plugins/paramiko/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-28 19:26:05.000000 scrapli_netconf-2023.1.30/scrapli_netconf/transport/plugins/paramiko/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-01-28 19:26:05.000000 scrapli_netconf-2023.1.30/scrapli_netconf/transport/plugins/paramiko/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 19:26:20.139973 scrapli_netconf-2023.1.30/scrapli_netconf/transport/plugins/ssh2/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-01-28 19:26:05.000000 scrapli_netconf-2023.1.30/scrapli_netconf/transport/plugins/ssh2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-01-28 19:26:05.000000 scrapli_netconf-2023.1.30/scrapli_netconf/transport/plugins/ssh2/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 19:26:20.139973 scrapli_netconf-2023.1.30/scrapli_netconf/transport/plugins/system/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-28 19:26:05.000000 scrapli_netconf-2023.1.30/scrapli_netconf/transport/plugins/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-01-28 19:26:05.000000 scrapli_netconf-2023.1.30/scrapli_netconf/transport/plugins/system/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 19:26:20.135974 scrapli_netconf-2023.1.30/scrapli_netconf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-01-28 19:26:20.000000 scrapli_netconf-2023.1.30/scrapli_netconf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-01-28 19:26:20.000000 scrapli_netconf-2023.1.30/scrapli_netconf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-28 19:26:20.000000 scrapli_netconf-2023.1.30/scrapli_netconf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-01-28 19:26:20.000000 scrapli_netconf-2023.1.30/scrapli_netconf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-28 19:26:20.000000 scrapli_netconf-2023.1.30/scrapli_netconf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-01-28 19:26:20.139973 scrapli_netconf-2023.1.30/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:04:55.404266 scrapli_netconf-2023.7.30/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-30 17:04:41.000000 scrapli_netconf-2023.7.30/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-30 17:04:41.000000 scrapli_netconf-2023.7.30/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-07-30 17:04:55.404266 scrapli_netconf-2023.7.30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-30 17:04:41.000000 scrapli_netconf-2023.7.30/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-30 17:04:41.000000 scrapli_netconf-2023.7.30/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-30 17:04:41.000000 scrapli_netconf-2023.7.30/requirements-asyncssh.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-30 17:04:41.000000 scrapli_netconf-2023.7.30/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-30 17:04:41.000000 scrapli_netconf-2023.7.30/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-30 17:04:41.000000 scrapli_netconf-2023.7.30/requirements-paramiko.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-30 17:04:41.000000 scrapli_netconf-2023.7.30/requirements-ssh2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-30 17:04:41.000000 scrapli_netconf-2023.7.30/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:04:55.404266 scrapli_netconf-2023.7.30/scrapli_netconf/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-30 17:04:41.000000 scrapli_netconf-2023.7.30/scrapli_netconf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:04:55.404266 scrapli_netconf-2023.7.30/scrapli_netconf/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-30 17:04:41.000000 scrapli_netconf-2023.7.30/scrapli_netconf/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-07-30 17:04:41.000000 scrapli_netconf-2023.7.30/scrapli_netconf/channel/async_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-07-30 17:04:41.000000 scrapli_netconf-2023.7.30/scrapli_netconf/channel/base_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12978 2023-07-30 17:04:41.000000 scrapli_netconf-2023.7.30/scrapli_netconf/channel/sync_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-30 17:04:41.000000 scrapli_netconf-2023.7.30/scrapli_netconf/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:04:55.404266 scrapli_netconf-2023.7.30/scrapli_netconf/driver/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-30 17:04:41.000000 scrapli_netconf-2023.7.30/scrapli_netconf/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-07-30 17:04:41.000000 scrapli_netconf-2023.7.30/scrapli_netconf/driver/async_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40546 2023-07-30 17:04:41.000000 scrapli_netconf-2023.7.30/scrapli_netconf/driver/base_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12015 2023-07-30 17:04:41.000000 scrapli_netconf-2023.7.30/scrapli_netconf/driver/sync_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-30 17:04:41.000000 scrapli_netconf-2023.7.30/scrapli_netconf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-30 17:04:41.000000 scrapli_netconf-2023.7.30/scrapli_netconf/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 17:04:41.000000 scrapli_netconf-2023.7.30/scrapli_netconf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13702 2023-07-30 17:04:41.000000 scrapli_netconf-2023.7.30/scrapli_netconf/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:04:55.404266 scrapli_netconf-2023.7.30/scrapli_netconf/transport/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-30 17:04:41.000000 scrapli_netconf-2023.7.30/scrapli_netconf/transport/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:04:55.404266 scrapli_netconf-2023.7.30/scrapli_netconf/transport/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-30 17:04:41.000000 scrapli_netconf-2023.7.30/scrapli_netconf/transport/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:04:55.404266 scrapli_netconf-2023.7.30/scrapli_netconf/transport/plugins/asyncssh/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-30 17:04:41.000000 scrapli_netconf-2023.7.30/scrapli_netconf/transport/plugins/asyncssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-30 17:04:41.000000 scrapli_netconf-2023.7.30/scrapli_netconf/transport/plugins/asyncssh/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:04:55.404266 scrapli_netconf-2023.7.30/scrapli_netconf/transport/plugins/paramiko/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-30 17:04:41.000000 scrapli_netconf-2023.7.30/scrapli_netconf/transport/plugins/paramiko/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-30 17:04:41.000000 scrapli_netconf-2023.7.30/scrapli_netconf/transport/plugins/paramiko/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:04:55.404266 scrapli_netconf-2023.7.30/scrapli_netconf/transport/plugins/ssh2/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-30 17:04:41.000000 scrapli_netconf-2023.7.30/scrapli_netconf/transport/plugins/ssh2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-30 17:04:41.000000 scrapli_netconf-2023.7.30/scrapli_netconf/transport/plugins/ssh2/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:04:55.404266 scrapli_netconf-2023.7.30/scrapli_netconf/transport/plugins/system/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-30 17:04:41.000000 scrapli_netconf-2023.7.30/scrapli_netconf/transport/plugins/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-07-30 17:04:41.000000 scrapli_netconf-2023.7.30/scrapli_netconf/transport/plugins/system/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:04:55.404266 scrapli_netconf-2023.7.30/scrapli_netconf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-07-30 17:04:55.000000 scrapli_netconf-2023.7.30/scrapli_netconf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-30 17:04:55.000000 scrapli_netconf-2023.7.30/scrapli_netconf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 17:04:55.000000 scrapli_netconf-2023.7.30/scrapli_netconf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-30 17:04:55.000000 scrapli_netconf-2023.7.30/scrapli_netconf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-30 17:04:55.000000 scrapli_netconf-2023.7.30/scrapli_netconf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-30 17:04:55.408267 scrapli_netconf-2023.7.30/setup.cfg
```

### Comparing `scrapli_netconf-2023.1.30/LICENSE` & `scrapli_netconf-2023.7.30/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapli_netconf-2023.1.30/PKG-INFO` & `scrapli_netconf-2023.7.30/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapli_netconf
-Version: 2023.1.30
+Version: 2023.7.30
 Summary: Fast, flexible, sync/async, Python 3.7+ NETCONF client built on scrapli
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
         
-Project-URL: Homepage, https://github.com/scrapli/scrapli_netconf
 Project-URL: Changelog, https://scrapli.github.io/scrapli_netconf/changelog/
 Project-URL: Docs, https://scrapli.github.io/scrapli_netconf/
-Keywords: ssh,telnet,netconf,automation,network,cisco,iosxr,iosxe,nxos,arista,eos,juniper,junos
+Project-URL: Homepage, https://github.com/scrapli/scrapli_netconf
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
-Metadata-Version: 2.1 Name: scrapli_netconf Version: 2023.1.30 Summary: Fast,
+Metadata-Version: 2.1 Name: scrapli_netconf Version: 2023.7.30 Summary: Fast,
 flexible, sync/async, Python 3.7+ NETCONF client built on scrapli Author-email:
 Carl Montanari
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
-DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://github.com/scrapli/
-scrapli_netconf Project-URL: Changelog, https://scrapli.github.io/
+DEALINGS IN THE SOFTWARE. Project-URL: Changelog, https://scrapli.github.io/
 scrapli_netconf/changelog/ Project-URL: Docs, https://scrapli.github.io/
-scrapli_netconf/ Keywords:
-ssh,telnet,netconf,automation,network,cisco,iosxr,iosxe,nxos,arista,eos,juniper,junos
+scrapli_netconf/ Project-URL: Homepage, https://github.com/scrapli/
+scrapli_netconf Keywords:
+arista,automation,cisco,eos,iosxe,iosxr,juniper,junos,netconf,network,nxos,ssh,telnet
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: POSIX :: Linux Classifier: Operating System :: MacOS Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Topic :: Software Development ::
```

### Comparing `scrapli_netconf-2023.1.30/README.md` & `scrapli_netconf-2023.7.30/README.md`

 * *Files identical despite different names*

### Comparing `scrapli_netconf-2023.1.30/pyproject.toml` & `scrapli_netconf-2023.7.30/pyproject.toml`

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
 name = "scrapli_netconf"
-dynamic = [
-    "version",
-    "dependencies",
-    "optional-dependencies",
-]
 description = "Fast, flexible, sync/async, Python 3.7+ NETCONF client built on scrapli"
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
-Homepage = "https://github.com/scrapli/scrapli_netconf"
 Changelog = "https://scrapli.github.io/scrapli_netconf/changelog/"
 Docs = "https://scrapli.github.io/scrapli_netconf/"
+Homepage = "https://github.com/scrapli/scrapli_netconf"
 
 [tool.setuptools.dynamic]
 version = { attr = "scrapli_netconf.__version__" }
 dependencies = { file = "requirements.txt" }
 optional-dependencies.dev = { file = [
     "requirements-dev.txt",
     "requirements-paramiko.txt",
@@ -65,29 +67,46 @@
 optional-dependencies.asyncssh = { file = "requirements-asyncssh.txt" }
 
 [tool.setuptools.package-data]
 scrapli_netconf = [
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
+known_third_party = "asyncssh,lxml,pytest"
+[tool.pytest.ini_options]
+asyncio_mode = "auto"
+
 [tool.coverage.run]
 source = [
     "scrapli_netconf/"
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
-known_third_party = "asyncssh,lxml,pytest"
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

### Comparing `scrapli_netconf-2023.1.30/scrapli_netconf/channel/async_channel.py` & `scrapli_netconf-2023.7.30/scrapli_netconf/channel/async_channel.py`

 * *Files identical despite different names*

### Comparing `scrapli_netconf-2023.1.30/scrapli_netconf/channel/base_channel.py` & `scrapli_netconf-2023.7.30/scrapli_netconf/channel/base_channel.py`

 * *Files identical despite different names*

### Comparing `scrapli_netconf-2023.1.30/scrapli_netconf/channel/sync_channel.py` & `scrapli_netconf-2023.7.30/scrapli_netconf/channel/sync_channel.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,26 +102,32 @@
                 buf = self.read()
 
                 authenticate_buf += buf.lower()
                 self._capabilities_buf += buf
 
                 self._ssh_message_handler(output=authenticate_buf)
 
-                if b"password" in authenticate_buf:
+                if re.search(
+                    pattern=self.auth_password_pattern,
+                    string=authenticate_buf,
+                ):
                     # clear the authentication buffer so we don't re-read the password prompt
                     authenticate_buf = b""
                     password_count += 1
                     if password_count > 2:
                         msg = "password prompt seen more than once, assuming auth failed"
                         self.logger.critical(msg)
                         raise ScrapliAuthenticationFailed(msg)
                     self.write(channel_input=auth_password, redacted=True)
                     self.send_return()
 
-                if b"enter passphrase for key" in authenticate_buf:
+                if re.search(
+                    pattern=self.auth_passphrase_pattern,
+                    string=authenticate_buf,
+                ):
                     # clear the authentication buffer so we don't re-read the passphrase prompt
                     authenticate_buf = b""
                     passphrase_count += 1
                     if passphrase_count > 2:
                         msg = "passphrase prompt seen more than once, assuming auth failed"
                         self.logger.critical(msg)
                         raise ScrapliAuthenticationFailed(msg)
```

### Comparing `scrapli_netconf-2023.1.30/scrapli_netconf/constants.py` & `scrapli_netconf-2023.7.30/scrapli_netconf/constants.py`

 * *Files identical despite different names*

### Comparing `scrapli_netconf-2023.1.30/scrapli_netconf/driver/async_driver.py` & `scrapli_netconf-2023.7.30/scrapli_netconf/driver/async_driver.py`

 * *Files identical despite different names*

### Comparing `scrapli_netconf-2023.1.30/scrapli_netconf/driver/base_driver.py` & `scrapli_netconf-2023.7.30/scrapli_netconf/driver/base_driver.py`

 * *Files identical despite different names*

### Comparing `scrapli_netconf-2023.1.30/scrapli_netconf/driver/sync_driver.py` & `scrapli_netconf-2023.7.30/scrapli_netconf/driver/sync_driver.py`

 * *Files identical despite different names*

### Comparing `scrapli_netconf-2023.1.30/scrapli_netconf/helper.py` & `scrapli_netconf-2023.7.30/scrapli_netconf/helper.py`

 * *Files identical despite different names*

### Comparing `scrapli_netconf-2023.1.30/scrapli_netconf/response.py` & `scrapli_netconf-2023.7.30/scrapli_netconf/response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """scrapli_netconf.response"""
 import logging
 import re
 from datetime import datetime
-from typing import Any, Dict, List, Optional, TextIO, Tuple, Union
+from typing import Any, Dict, List, Optional, TextIO, Union
 
 from lxml import etree
 from lxml.etree import Element
 
 from scrapli.exceptions import ScrapliCommandFailure
 from scrapli.response import Response
 from scrapli_netconf.constants import NetconfVersion
 from scrapli_netconf.helper import remove_namespaces
 
 LOG = logging.getLogger("response")
 
 # "chunk match" matches the "#123" netconf1.1 chunk size delimiters. We then simply slice out the
 # actual chunk from the received byte stream.
-CHUNK_MATCH_1_1 = re.compile(rb"^#(?P<size>\d+)\s*$", flags=re.M | re.I)
+CHUNK_MATCH_1_1 = re.compile(rb"(?P<size>\d+)\n(?P<content>.*?)^#", flags=re.M | re.S)
 
 # CONTROL_CHARS matches control chars we do not want to see in text output, such as \x07 (terminal
 # bell). See #127 for more details.
 CONTROL_CHARS = re.compile(rb"[\x00-\x1f\x7f-\x9f]")
 
 PARSER = etree.XMLParser(remove_blank_text=True, recover=True)
 
@@ -157,15 +157,15 @@
 
         if self.strip_namespaces:
             self.xml_result = remove_namespaces(self.xml_result)
             self.result = etree.tostring(self.xml_result, pretty_print=True).decode()
         else:
             self.result = etree.tostring(self.xml_result, pretty_print=True).decode()
 
-    def _validate_chunk_size_netconf_1_1(self, result: Tuple[int, bytes]) -> None:
+    def _validate_chunk_size_netconf_1_1(self, size: int, chunk: bytes) -> None:
         """
         Validate individual chunk size; handle parsing trailing new lines for chunk sizes
 
         It seems that some platforms behave slightly differently than others (looking at you IOSXE)
         in the way they count chunk sizes with respect to trailing whitespace. Per my reading of the
         RFC, the response for a netconf 1.1 response should look like this:
 
@@ -195,51 +195,50 @@
         newline counts -- we check the expected chunk length against the actual char count, the char
         count with all trailing whitespace stripped, and the count of the chunk + a *single*
         trailing newline character...
 
         FIN
 
         Args:
-            result: Tuple from re.findall parsing the full response object
+            size: the expected size of the chunk contents
+            chunk: the chunk contents
 
         Returns:
             N/A
 
         Raises:
             N/A
 
         """
-        expected_len, result_value = result
+        actual_size = len(chunk)
+        rstripped_size = len(chunk.rstrip())
 
-        actual_len = len(result_value)
-        rstripped_len = len(result_value.rstrip())
-
-        trailing_newline_count = actual_len - rstripped_len
+        trailing_newline_count = actual_size - rstripped_size
         if trailing_newline_count > 1:
             extraneous_trailing_newline_count = trailing_newline_count - 1
         else:
             extraneous_trailing_newline_count = 1
-        trimmed_newline_len = actual_len - extraneous_trailing_newline_count
+        trimmed_newline_len = actual_size - extraneous_trailing_newline_count
 
-        if rstripped_len == 0:
+        if rstripped_size == 0:
             # at least nokia tends to have itty bitty chunks of one element, and/or chunks that have
             # *only* whitespace and our regex ignores this, so if there was/is nothing in the result
             # section we can assume it was just whitespace and move on w/our lives
-            actual_len = expected_len
+            actual_size = size
 
-        if expected_len == actual_len:
+        if size == actual_size:
             return
-        if expected_len == rstripped_len:
+        if size == rstripped_size:
             return
-        if expected_len == trimmed_newline_len:
+        if size == trimmed_newline_len:
             return
 
         LOG.critical(
-            f"Return element length invalid, expected {expected_len} got {actual_len} for "
-            f"element: {repr(result_value)}"
+            f"Return element length invalid, expected {size} got {actual_size} for "
+            f"element: {repr(chunk)}"
         )
         self.failed = True
 
     def _record_response_netconf_1_1(self) -> None:
         """
         Record response for netconf version 1.1
 
@@ -249,36 +248,33 @@
         Returns:
             N/A
 
         Raises:
             N/A
 
         """
-        chunk_sizes = re.finditer(pattern=CHUNK_MATCH_1_1, string=self.raw_result)
+        chunk_matches = re.finditer(pattern=CHUNK_MATCH_1_1, string=self.raw_result)
 
-        result_sections: List[Tuple[int, bytes]] = []
+        chunks: List[bytes] = []
 
-        for chunk_match in chunk_sizes:
-            chunk_size = int(chunk_match.groupdict().get("size", 0))
-            chunk_end_pos = chunk_match.span()[1]
-            result_sections.append(
-                (chunk_size, self.raw_result[chunk_end_pos : chunk_end_pos + chunk_size])  # noqa
-            )
+        for chunk_match in chunk_matches:
+            size = int(chunk_match.groupdict().get("size", 0))
+            chunk = chunk_match.groupdict().get("content", "")
+
+            self._validate_chunk_size_netconf_1_1(size=size, chunk=chunk)
 
-        # validate all received data
-        for result in result_sections:
-            self._validate_chunk_size_netconf_1_1(result=result)
+            chunks.append(chunk[:-1])
 
         self.xml_result = etree.fromstring(
             b"\n".join(
                 [
                     # remove the message end characters and xml document header see:
                     # https://github.com/scrapli/scrapli_netconf/issues/1
-                    result[1].replace(b'<?xml version="1.0" encoding="UTF-8"?>', b"")
-                    for result in result_sections
+                    chunk.replace(b'<?xml version="1.0" encoding="UTF-8"?>', b"")
+                    for chunk in chunks
                 ]
             ),
             parser=PARSER,
         )
 
         if self.strip_namespaces:
             self.xml_result = remove_namespaces(self.xml_result)
```

### Comparing `scrapli_netconf-2023.1.30/scrapli_netconf/transport/plugins/asyncssh/transport.py` & `scrapli_netconf-2023.7.30/scrapli_netconf/transport/plugins/asyncssh/transport.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """scrapli_netconf.transport.plugins.asyncssh.transport"""
 import asyncio
+from typing import Any, Dict
 
 from asyncssh.connection import SSHClientConnection, connect
 from asyncssh.misc import ChannelOpenError, PermissionDenied
 
 from scrapli.exceptions import ScrapliAuthenticationFailed, ScrapliConnectionNotOpened
 from scrapli.transport.plugins.asyncssh.transport import AsyncsshTransport, PluginTransportArgs
 
@@ -34,36 +35,50 @@
                 f"Attempting to validate {self._base_transport_args.host} public key is in known "
                 f"hosts"
             )
             self._verify_key()
 
         # we already fetched host/port/user from the user input and/or the ssh config file, so we
         # want to use those explicitly. likewise we pass config file we already found. set known
-        # hosts and agent to None so we can not have an agent and deal w/ known hosts ourselves
-        common_args = {
+        # hosts and agent to None so we can not have an agent and deal w/ known hosts ourselves.
+        # to use ssh-agent either pass an empty tuple (to pick up ssh-agent socket from
+        # SSH_AUTH_SOCK), or pass an explicit path to ssh-agent socket should be provided as part
+        # of transport_options -- in either case these get merged into the dict *after* we set the
+        # default value of `None`, so users options override our defaults.
+
+        common_args: Dict[str, Any] = {
             "host": self._base_transport_args.host,
             "port": self._base_transport_args.port,
             "username": self.plugin_transport_args.auth_username,
             "known_hosts": None,
             "agent_path": None,
             "config": self.plugin_transport_args.ssh_config_file,
         }
 
+        # Allow passing `transport_options` to asyncssh
+        common_args.update(self._base_transport_args.transport_options.get("asyncssh", {}))
+
+        # Common authentication args
+        auth_args: Dict[str, Any] = {
+            "client_keys": self.plugin_transport_args.auth_private_key,
+            "password": self.plugin_transport_args.auth_password,
+            "preferred_auth": (
+                "publickey",
+                "keyboard-interactive",
+                "password",
+            ),
+        }
+
+        # The session args to use in connect() - to merge the dicts in
+        # the order to have transport options preference over predefined auth args
+        conn_args = {**auth_args, **common_args}
+
         try:
             self.session: SSHClientConnection = await asyncio.wait_for(
-                connect(
-                    client_keys=self.plugin_transport_args.auth_private_key,
-                    password=self.plugin_transport_args.auth_password,
-                    preferred_auth=(
-                        "publickey",
-                        "keyboard-interactive",
-                        "password",
-                    ),
-                    **common_args,
-                ),
+                connect(**conn_args),
                 timeout=self._base_transport_args.timeout_socket,
             )
         except PermissionDenied as exc:
             msg = "all authentication methods failed"
             self.logger.critical(msg)
             raise ScrapliAuthenticationFailed(msg) from exc
         except asyncio.TimeoutError as exc:
```

### Comparing `scrapli_netconf-2023.1.30/scrapli_netconf/transport/plugins/paramiko/transport.py` & `scrapli_netconf-2023.7.30/scrapli_netconf/transport/plugins/paramiko/transport.py`

 * *Files identical despite different names*

### Comparing `scrapli_netconf-2023.1.30/scrapli_netconf/transport/plugins/ssh2/transport.py` & `scrapli_netconf-2023.7.30/scrapli_netconf/transport/plugins/ssh2/transport.py`

 * *Files identical despite different names*

### Comparing `scrapli_netconf-2023.1.30/scrapli_netconf/transport/plugins/system/transport.py` & `scrapli_netconf-2023.7.30/scrapli_netconf/transport/plugins/system/transport.py`

 * *Files identical despite different names*

### Comparing `scrapli_netconf-2023.1.30/scrapli_netconf.egg-info/PKG-INFO` & `scrapli_netconf-2023.7.30/scrapli_netconf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapli-netconf
-Version: 2023.1.30
+Version: 2023.7.30
 Summary: Fast, flexible, sync/async, Python 3.7+ NETCONF client built on scrapli
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
         
-Project-URL: Homepage, https://github.com/scrapli/scrapli_netconf
 Project-URL: Changelog, https://scrapli.github.io/scrapli_netconf/changelog/
 Project-URL: Docs, https://scrapli.github.io/scrapli_netconf/
-Keywords: ssh,telnet,netconf,automation,network,cisco,iosxr,iosxe,nxos,arista,eos,juniper,junos
+Project-URL: Homepage, https://github.com/scrapli/scrapli_netconf
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
-Metadata-Version: 2.1 Name: scrapli-netconf Version: 2023.1.30 Summary: Fast,
+Metadata-Version: 2.1 Name: scrapli-netconf Version: 2023.7.30 Summary: Fast,
 flexible, sync/async, Python 3.7+ NETCONF client built on scrapli Author-email:
 Carl Montanari
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
-DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://github.com/scrapli/
-scrapli_netconf Project-URL: Changelog, https://scrapli.github.io/
+DEALINGS IN THE SOFTWARE. Project-URL: Changelog, https://scrapli.github.io/
 scrapli_netconf/changelog/ Project-URL: Docs, https://scrapli.github.io/
-scrapli_netconf/ Keywords:
-ssh,telnet,netconf,automation,network,cisco,iosxr,iosxe,nxos,arista,eos,juniper,junos
+scrapli_netconf/ Project-URL: Homepage, https://github.com/scrapli/
+scrapli_netconf Keywords:
+arista,automation,cisco,eos,iosxe,iosxr,juniper,junos,netconf,network,nxos,ssh,telnet
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: POSIX :: Linux Classifier: Operating System :: MacOS Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Topic :: Software Development ::
```

### Comparing `scrapli_netconf-2023.1.30/scrapli_netconf.egg-info/SOURCES.txt` & `scrapli_netconf-2023.7.30/scrapli_netconf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scrapli_netconf-2023.1.30/scrapli_netconf.egg-info/requires.txt` & `scrapli_netconf-2023.7.30/scrapli_netconf.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 lxml<5.0.0,>=4.5.1
 scrapli>=2022.07.30
 
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
 pylama<9.0.0,>=8.4.0
-pylint==2.15.10
+pylint==2.17.5
 pytest-asyncio<1.0.0,>=0.17.0
 pytest-cov<5.0.0,>=3.0.0
 pytest<8.0.0,>=7.0.0
 toml<1.0.0,>=0.10.2
 paramiko<3.0.0,>=2.6.0
-ssh2-python<2.0.0,>=0.23.0
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
 paramiko<3.0.0,>=2.6.0
 
 [ssh2]
+
+[ssh2:python_version < "3.12"]
 ssh2-python<2.0.0,>=0.23.0
```

