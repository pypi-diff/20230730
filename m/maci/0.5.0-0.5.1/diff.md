# Comparing `tmp/maci-0.5.0.tar.gz` & `tmp/maci-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maci-0.5.0.tar", last modified: Fri Jul 14 03:31:16 2023, max compression
+gzip compressed data, was "maci-0.5.1.tar", last modified: Sun Jul 30 03:28:50 2023, max compression
```

## Comparing `maci-0.5.0.tar` & `maci-0.5.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:31:16.296071 maci-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-07-14 03:31:06.000000 maci-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-07-14 03:31:16.296071 maci-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-07-14 03:31:16.000000 maci-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:31:16.288071 maci-0.5.0/maci/
--rw-r--r--   0 runner    (1001) docker     (122)     3371 2023-07-14 03:31:16.000000 maci-0.5.0/maci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    22867 2023-07-14 03:31:16.000000 maci-0.5.0/maci/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:31:16.292071 maci-0.5.0/maci/_hash/
--rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_hash/comparefilehash.py
--rw-r--r--   0 runner    (1001) docker     (122)     3868 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_hash/createfilehash.py
--rw-r--r--   0 runner    (1001) docker     (122)     3454 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_hash/createhash.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:31:16.292071 maci-0.5.0/maci/_ini/
--rw-r--r--   0 runner    (1001) docker     (122)     2156 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_ini/inibuildauto.py
--rw-r--r--   0 runner    (1001) docker     (122)      902 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_ini/inibuildmanual.py
--rw-r--r--   0 runner    (1001) docker     (122)     2030 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_ini/inidump.py
--rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_ini/iniload.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:31:16.292071 maci-0.5.0/maci/_json/
--rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_json/jsondump.py
--rw-r--r--   0 runner    (1001) docker     (122)     1481 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_json/jsondumpstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     1685 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_json/jsonload.py
--rw-r--r--   0 runner    (1001) docker     (122)     1236 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_json/jsonloadstr.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:31:16.292071 maci-0.5.0/maci/_native/
--rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_native/build.py
--rw-r--r--   0 runner    (1001) docker     (122)     2272 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_native/cleanformat.py
--rw-r--r--   0 runner    (1001) docker     (122)     6878 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_native/dump.py
--rw-r--r--   0 runner    (1001) docker     (122)     4376 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_native/dumpraw.py
--rw-r--r--   0 runner    (1001) docker     (122)     6174 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_native/dumpstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     3615 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_native/load.py
--rw-r--r--   0 runner    (1001) docker     (122)     2815 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_native/loadattrs.py
--rw-r--r--   0 runner    (1001) docker     (122)     4126 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_native/loaddict.py
--rw-r--r--   0 runner    (1001) docker     (122)     2046 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_native/loadraw.py
--rw-r--r--   0 runner    (1001) docker     (122)     2591 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_native/loadstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     3502 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_native/loadstrdict.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:31:16.296071 maci-0.5.0/maci/_toml/
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_toml/tomldump.py
--rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_toml/tomldumpstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     1283 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_toml/tomlload.py
--rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_toml/tomlloadstr.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:31:16.296071 maci-0.5.0/maci/_xml/
--rw-r--r--   0 runner    (1001) docker     (122)      888 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_xml/xmlbuildmanual.py
--rw-r--r--   0 runner    (1001) docker     (122)     2406 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_xml/xmldump.py
--rw-r--r--   0 runner    (1001) docker     (122)     1466 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_xml/xmldumpstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     2015 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_xml/xmlload.py
--rw-r--r--   0 runner    (1001) docker     (122)     1347 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_xml/xmlloadstr.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:31:16.296071 maci-0.5.0/maci/_yaml/
--rw-r--r--   0 runner    (1001) docker     (122)     2107 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_yaml/yamldump.py
--rw-r--r--   0 runner    (1001) docker     (122)     1124 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_yaml/yamldumpstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_yaml/yamlload.py
--rw-r--r--   0 runner    (1001) docker     (122)     1277 2023-07-14 03:31:16.000000 maci-0.5.0/maci/_yaml/yamlloadstr.py
--rw-r--r--   0 runner    (1001) docker     (122)    75021 2023-07-14 03:31:16.000000 maci-0.5.0/maci/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     7977 2023-07-14 03:31:16.000000 maci-0.5.0/maci/data.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-07-14 03:31:16.000000 maci-0.5.0/maci/error.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:31:16.288071 maci-0.5.0/maci/ext/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:31:16.296071 maci-0.5.0/maci/ext/defusedxml/
--rw-r--r--   0 runner    (1001) docker     (122)     2408 2023-07-14 03:31:16.000000 maci-0.5.0/maci/ext/defusedxml/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-07-14 03:31:16.000000 maci-0.5.0/maci/hint.py
--rw-r--r--   0 runner    (1001) docker     (122)      880 2023-07-14 03:31:16.000000 maci-0.5.0/maci/hint.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 03:31:16.000000 maci-0.5.0/maci/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:31:16.292071 maci-0.5.0/maci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-07-14 03:31:16.000000 maci-0.5.0/maci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1199 2023-07-14 03:31:16.000000 maci-0.5.0/maci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-14 03:31:16.000000 maci-0.5.0/maci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-14 03:31:16.000000 maci-0.5.0/maci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-14 03:31:16.000000 maci-0.5.0/maci.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1344 2023-07-14 03:31:16.296071 maci-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      154 2023-07-14 03:31:06.000000 maci-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 03:28:50.846597 maci-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-07-30 03:28:38.000000 maci-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-07-30 03:28:50.846597 maci-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-07-30 03:28:50.000000 maci-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 03:28:50.842597 maci-0.5.1/maci/
+-rw-r--r--   0 runner    (1001) docker     (122)     3371 2023-07-30 03:28:50.000000 maci-0.5.1/maci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22867 2023-07-30 03:28:50.000000 maci-0.5.1/maci/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 03:28:50.842597 maci-0.5.1/maci/_hash/
+-rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_hash/comparefilehash.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3868 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_hash/createfilehash.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3454 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_hash/createhash.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 03:28:50.842597 maci-0.5.1/maci/_ini/
+-rw-r--r--   0 runner    (1001) docker     (122)     2156 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_ini/inibuildauto.py
+-rw-r--r--   0 runner    (1001) docker     (122)      902 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_ini/inibuildmanual.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2030 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_ini/inidump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_ini/iniload.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 03:28:50.846597 maci-0.5.1/maci/_json/
+-rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_json/jsondump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1481 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_json/jsondumpstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1685 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_json/jsonload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1236 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_json/jsonloadstr.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 03:28:50.846597 maci-0.5.1/maci/_native/
+-rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_native/build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2272 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_native/cleanformat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6878 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_native/dump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4376 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_native/dumpraw.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6174 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_native/dumpstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3615 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_native/load.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2815 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_native/loadattrs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4126 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_native/loaddict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2046 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_native/loadraw.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2591 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_native/loadstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3502 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_native/loadstrdict.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 03:28:50.846597 maci-0.5.1/maci/_toml/
+-rw-r--r--   0 runner    (1001) docker     (122)     2160 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_toml/tomldump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_toml/tomldumpstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1283 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_toml/tomlload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_toml/tomlloadstr.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 03:28:50.846597 maci-0.5.1/maci/_xml/
+-rw-r--r--   0 runner    (1001) docker     (122)      888 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_xml/xmlbuildmanual.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2406 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_xml/xmldump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1466 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_xml/xmldumpstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2015 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_xml/xmlload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1347 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_xml/xmlloadstr.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 03:28:50.846597 maci-0.5.1/maci/_yaml/
+-rw-r--r--   0 runner    (1001) docker     (122)     2107 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_yaml/yamldump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1124 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_yaml/yamldumpstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_yaml/yamlload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1277 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_yaml/yamlloadstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    75585 2023-07-30 03:28:50.000000 maci-0.5.1/maci/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7977 2023-07-30 03:28:50.000000 maci-0.5.1/maci/data.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-07-30 03:28:50.000000 maci-0.5.1/maci/error.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 03:28:50.842597 maci-0.5.1/maci/ext/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 03:28:50.846597 maci-0.5.1/maci/ext/defusedxml/
+-rw-r--r--   0 runner    (1001) docker     (122)     2408 2023-07-30 03:28:50.000000 maci-0.5.1/maci/ext/defusedxml/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-07-30 03:28:50.000000 maci-0.5.1/maci/hint.py
+-rw-r--r--   0 runner    (1001) docker     (122)      880 2023-07-30 03:28:50.000000 maci-0.5.1/maci/hint.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 03:28:50.000000 maci-0.5.1/maci/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 03:28:50.842597 maci-0.5.1/maci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-07-30 03:28:50.000000 maci-0.5.1/maci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1199 2023-07-30 03:28:50.000000 maci-0.5.1/maci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-30 03:28:50.000000 maci-0.5.1/maci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-30 03:28:50.000000 maci-0.5.1/maci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-30 03:28:50.000000 maci-0.5.1/maci.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1344 2023-07-30 03:28:50.846597 maci-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      154 2023-07-30 03:28:38.000000 maci-0.5.1/setup.py
```

### Comparing `maci-0.5.0/PKG-INFO` & `maci-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maci
-Version: 0.5.0
+Version: 0.5.1
 Summary: The easy to use library for your data, configuration, and save files
 Author: aaronater10
 Author-email: dev_admin@dunnts.com
 License: MIT
 Project-URL: Docs, https://docs.macilib.org
 Project-URL: Code, https://github.com/aaronater10/maci
 Project-URL: Bugs, https://github.com/aaronater10/maci/issues
@@ -23,15 +23,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # maci
 The easy to use library for your data, configuration, and save files
 
-##### Latest Version: 0.5.0
+##### Latest Version: 0.5.1
 
 #
 
 Import or Export **custom**, or **industry-common**, data, config, and save files easily for your python program or script!
 
 **Use python data types for your data** (literally use python data types as stored values importing them securely vs just importing a .py file) **in any text file**.
```

### Comparing `maci-0.5.0/README.md` & `maci-0.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # maci
 The easy to use library for your data, configuration, and save files
 
-##### Latest Version: 0.5.0
+##### Latest Version: 0.5.1
 
 #
 
 Import or Export **custom**, or **industry-common**, data, config, and save files easily for your python program or script!
 
 **Use python data types for your data** (literally use python data types as stored values importing them securely vs just importing a .py file) **in any text file**.
```

### Comparing `maci-0.5.0/maci/__init__.py` & `maci-0.5.1/maci/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 maci - by aaronater10
 
 A Pythonic Configuration Language & Thin Wrapper Library
 
-Version 0.5.0
+Version 0.5.1
 
 Tutorials and docs: https://docs.macilib.org
 
 Source: https://github.com/aaronater10/maci
 """
-__version__ = '0.5.0'
+__version__ = '0.5.1'
 
 #########################################################################################################
 # Imports
 
 # Exceptions
 from . import error
```

### Comparing `maci-0.5.0/maci/__init__.pyi` & `maci-0.5.1/maci/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # stub file to document public api functions, errors, object types, and doc string comments
 """
 maci - by aaronater10
 
 A Pythonic Configuration Language & Thin Wrapper Library
 
-Version 0.5.0
+Version 0.5.1
 
 Tutorials and docs: https://docs.macilib.org
 
 Source: https://github.com/aaronater10/maci
 """
 #########################################################################################################
 # Imports
```

### Comparing `maci-0.5.0/maci/_hash/comparefilehash.py` & `maci-0.5.1/maci/_hash/comparefilehash.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/_hash/createfilehash.py` & `maci-0.5.1/maci/_hash/createfilehash.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/_hash/createhash.py` & `maci-0.5.1/maci/_hash/createhash.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/_ini/inibuildauto.py` & `maci-0.5.1/maci/_ini/inibuildauto.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/_ini/inibuildmanual.py` & `maci-0.5.1/maci/_ini/inibuildmanual.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/_ini/inidump.py` & `maci-0.5.1/maci/_ini/inidump.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/_ini/iniload.py` & `maci-0.5.1/maci/_ini/iniload.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/_json/jsondump.py` & `maci-0.5.1/maci/_json/jsondump.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/_json/jsondumpstr.py` & `maci-0.5.1/maci/_json/jsondumpstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/_json/jsonload.py` & `maci-0.5.1/maci/_json/jsonload.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/_json/jsonloadstr.py` & `maci-0.5.1/maci/_json/jsonloadstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/_native/build.py` & `maci-0.5.1/maci/_native/build.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/_native/cleanformat.py` & `maci-0.5.1/maci/_native/cleanformat.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/_native/dump.py` & `maci-0.5.1/maci/_native/dump.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/_native/dumpraw.py` & `maci-0.5.1/maci/_native/dumpraw.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/_native/dumpstr.py` & `maci-0.5.1/maci/_native/dumpstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/_native/load.py` & `maci-0.5.1/maci/_native/load.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/_native/loadattrs.py` & `maci-0.5.1/maci/_native/loadattrs.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/_native/loaddict.py` & `maci-0.5.1/maci/_native/loaddict.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/_native/loadraw.py` & `maci-0.5.1/maci/_native/loadraw.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/_native/loadstr.py` & `maci-0.5.1/maci/_native/loadstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/_native/loadstrdict.py` & `maci-0.5.1/maci/_native/loadstrdict.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/_toml/tomldump.py` & `maci-0.5.1/maci/_toml/tomldump.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,9 +44,9 @@
 
     try:
         # Dump data to toml file
         file_data: _Any  # ignore type checker
         with open(filename, write_mode) as file_data:
             _tomli_w.dump(data, file_data, multiline_strings=multi_line_str)
             if write_mode == 'ab': _dumpraw(filename, '', append=True)
-    except TypeError as err_msg: raise TomlDump(err_msg, f'\nGot: {repr(filename)} \nGot: {repr(data)}')
+    except TypeError as err_msg: raise TomlDump(err_msg, f'\nFile: {repr(filename)} \nGot: {repr(data)}')
     except (FileNotFoundError, OSError) as err_msg: raise TomlDump(err_msg, f'\nGot: {repr(filename)}')
```

### Comparing `maci-0.5.0/maci/_toml/tomldumpstr.py` & `maci-0.5.1/maci/_toml/tomldumpstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/_toml/tomlload.py` & `maci-0.5.1/maci/_toml/tomlload.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/_toml/tomlloadstr.py` & `maci-0.5.1/maci/_toml/tomlloadstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/_xml/xmlbuildmanual.py` & `maci-0.5.1/maci/_xml/xmlbuildmanual.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/_xml/xmldump.py` & `maci-0.5.1/maci/_xml/xmldump.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/_xml/xmldumpstr.py` & `maci-0.5.1/maci/_xml/xmldumpstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/_xml/xmlload.py` & `maci-0.5.1/maci/_xml/xmlload.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/_xml/xmlloadstr.py` & `maci-0.5.1/maci/_xml/xmlloadstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/_yaml/yamldump.py` & `maci-0.5.1/maci/_yaml/yamldump.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/_yaml/yamldumpstr.py` & `maci-0.5.1/maci/_yaml/yamldumpstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/_yaml/yamlload.py` & `maci-0.5.1/maci/_yaml/yamlload.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/_yaml/yamlloadstr.py` & `maci-0.5.1/maci/_yaml/yamlloadstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/data.py` & `maci-0.5.1/maci/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,21 +224,21 @@
         # Data Build Setup and Switches        
         __is_building_data_sw = False
         __body_build_data_sw = False
         __end_data_build_sw = False
         __build_data = ''
 
         # Markers
-        __start_markers = {'[', '{', '(', "'''", '"""'}
+        __start_markers = {'[', '{', '(', "'''", '"""', "r'''", 'r"""'}
         __end_markers = {']', '}', ')', "'''", '"""'}
         __end_multistr_markers = {"'''", '"""'}
         __end_markers_build = __end_markers
         __skip_markers = ('', ' ', '#', '\n')
         __eof_marker = file_data[-1]
-        __ignore_multistr_markers = ("'''", '"""')
+        __ignore_multistr_markers = ("'''", '"""', "r'''", 'r"""')
         __ignore_multistr_marker = ''
 
         # Assignment Glyphs - Set by Another Class and is a NamedTuple
         __assignment_glyphs = _Glyphs()
 
         # Glyph Checks for Internal Mechs
         _assignment_glyphs_for_any_checks = set(__assignment_glyphs)
@@ -370,14 +370,16 @@
                     
                     # Set First Value
                     __build_data = __value_token
 
                     # Swap ignore type if multi-str. If triple-singles, then ignore triple-doubles and vice-versa
                     if __ignore_multistr_markers[0] == __value_token: __ignore_multistr_marker = __ignore_multistr_markers[1]
                     if __ignore_multistr_markers[1] == __value_token: __ignore_multistr_marker = __ignore_multistr_markers[0]
+                    if __ignore_multistr_markers[2] == __value_token: __ignore_multistr_marker = __ignore_multistr_markers[1]
+                    if __ignore_multistr_markers[3] == __value_token: __ignore_multistr_marker = __ignore_multistr_markers[0]
 
                     # Turn ON/UPDATE Data Build Switches
                     __is_building_data_sw = True
                     __body_build_data_sw = True
                     __end_data_build_sw = True
                     if __value_token in __end_multistr_markers: # pragma: no branch
                         __end_markers_build = __end_multistr_markers
@@ -395,15 +397,15 @@
                         if __current_assignment_glyph in _assignment_glyphs_for_lock_checks:
                             self.__assignment_locked_attribs.add(__var_token)
 
                         # Check if Attr is Hard Locked from Re-Assignment
                         if __current_assignment_glyph in _assignment_glyphs_for_hard_lock_checks:
                             self.__assignment_hard_locked_attribs.add(__var_token)
 
-                    except SyntaxError: raise Load(py_syntax_err_msg, f'\nFile: {repr(filename)} \nLine: {line_num} \nAttr: {__var_token}')
+                    except (ValueError, SyntaxError): raise Load(py_syntax_err_msg, f'\nFile: {repr(filename)} \nLine: {line_num} \nAttr: {__var_token}')
 
                     # Turn OFF/UPDATE Data Build Switches
                     __is_building_data_sw = False
                     __body_build_data_sw = False
                     __end_data_build_sw = False
                     __build_data = ''
                     __end_markers_build = __end_markers
@@ -647,22 +649,26 @@
         to the concept of a pointer.
         """
         # Error Checks
         __err_msg_attr_name_str = "Only str is allowed for 'child_attr'"
         __err_msg_reference_name_str = "Only str is allowed for 'parent_attr'"
         __err_msg_attr_name_exist = f"Attribute name '{child_attr}' does not exist! Must be created first to assign to parent attribute"
         __err_msg_reference_name_exist = f"Attribute name '{parent_attr}' does not exist! Cannot assign value to child attribute"
+        __err_msg_map_to_itself = f"Mapping to same name! Attribute name cannot be mapped to itself"
 
         if not isinstance(child_attr, str): raise GeneralError(__err_msg_attr_name_str, f'\nAttr: {repr(child_attr)}')
         if not isinstance(parent_attr, str): raise GeneralError(__err_msg_reference_name_str, f'\nAttr: {repr(parent_attr)}')
 
         # Look up if Attr or Reference Name Exists
         if not child_attr in self.__dict__: raise GeneralError(__err_msg_attr_name_exist, f'\nAttr: {repr(child_attr)}')
         if not parent_attr in self.__dict__: raise GeneralError(__err_msg_reference_name_exist, f'\nAttr: {repr(parent_attr)}')
 
+        # Verify Attr Names not Referencing Itself
+        if child_attr == parent_attr: raise GeneralError(__err_msg_map_to_itself, f'\nAttr: {repr(child_attr)}')
+
         # Set Value to Reference Value
         setattr(self, child_attr, getattr(self, parent_attr))
     
         # Assign Attr Name to Reference Name in Reference Maps
         self.__assigned_src_reference_attr_map[child_attr] = parent_attr
         self.__assigned_dst_reference_attr_map.setdefault(parent_attr, {}).setdefault(child_attr, parent_attr)
```

### Comparing `maci-0.5.0/maci/data.pyi` & `maci-0.5.1/maci/data.pyi`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/error.py` & `maci-0.5.1/maci/error.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/ext/defusedxml/LICENSE.txt` & `maci-0.5.1/maci/ext/defusedxml/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/hint.py` & `maci-0.5.1/maci/hint.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci/hint.pyi` & `maci-0.5.1/maci/hint.pyi`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/maci.egg-info/PKG-INFO` & `maci-0.5.1/maci.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maci
-Version: 0.5.0
+Version: 0.5.1
 Summary: The easy to use library for your data, configuration, and save files
 Author: aaronater10
 Author-email: dev_admin@dunnts.com
 License: MIT
 Project-URL: Docs, https://docs.macilib.org
 Project-URL: Code, https://github.com/aaronater10/maci
 Project-URL: Bugs, https://github.com/aaronater10/maci/issues
@@ -23,15 +23,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # maci
 The easy to use library for your data, configuration, and save files
 
-##### Latest Version: 0.5.0
+##### Latest Version: 0.5.1
 
 #
 
 Import or Export **custom**, or **industry-common**, data, config, and save files easily for your python program or script!
 
 **Use python data types for your data** (literally use python data types as stored values importing them securely vs just importing a .py file) **in any text file**.
```

### Comparing `maci-0.5.0/maci.egg-info/SOURCES.txt` & `maci-0.5.1/maci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maci-0.5.0/setup.cfg` & `maci-0.5.1/setup.cfg`

 * *Files identical despite different names*

