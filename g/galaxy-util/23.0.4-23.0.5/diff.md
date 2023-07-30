# Comparing `tmp/galaxy-util-23.0.4.tar.gz` & `tmp/galaxy-util-23.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/util/dist/.tmp-3g1lu66l/galaxy-util-23.0.4.tar", last modified: Fri Jun 30 22:01:26 2023, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/util/dist/.tmp-z7yhtutr/galaxy-util-23.0.5.tar", last modified: Sun Jul 30 10:47:42 2023, max compression
```

## Comparing `galaxy-util-23.0.4.tar` & `galaxy-util-23.0.5.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:01:26.000000 galaxy-util-23.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-30 22:00:49.000000 galaxy-util-23.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-30 22:01:26.000000 galaxy-util-23.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:01:26.000000 galaxy-util-23.0.4/galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:01:26.000000 galaxy-util-23.0.4/galaxy/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/exceptions/error_codes.json
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/exceptions/error_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:01:26.000000 galaxy-util-23.0.4/galaxy/util/
--rw-r--r--   0 runner    (1001) docker     (123)    61298 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/aliaspickler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/bool_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/bunch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/bytesize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    13411 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/compression_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:01:26.000000 galaxy-util-23.0.4/galaxy/util/custom_logging/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/custom_logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/custom_logging/fluent_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7819 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/dbkeys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/dictifiable.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/docutils_template.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/drs.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/facts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/filelock.py
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/form_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/hash_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/image_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/inflection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/jstree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/lazy_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/monitors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/odict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/oset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:01:26.000000 galaxy-util-23.0.4/galaxy/util/path/
--rw-r--r--   0 runner    (1001) docker     (123)    16902 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/path/ntpath.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/path/posixpath.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/permutations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/plugin_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7913 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/renamed_temporary_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/rules_dsl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/rules_dsl_spec.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/sanitize_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/script.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/simplegraph.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/sleeper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/sockets.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/specs.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/submodules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/template.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/themes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:01:26.000000 galaxy-util-23.0.4/galaxy/util/tool_shed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/tool_shed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13020 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/tool_shed/common_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/tool_shed/encoding_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/tool_shed/tool_shed_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/tool_shed/xml_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/tool_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/topsort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/ucsc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/unittest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:01:26.000000 galaxy-util-23.0.4/galaxy/util/unittest_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/unittest_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    11797 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/xml_macros.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/yaml_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/util/zipstream.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/galaxy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:01:26.000000 galaxy-util-23.0.4/galaxy_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-30 22:01:26.000000 galaxy-util-23.0.4/galaxy_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-30 22:01:26.000000 galaxy-util-23.0.4/galaxy_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 22:01:26.000000 galaxy-util-23.0.4/galaxy_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-30 22:01:26.000000 galaxy-util-23.0.4/galaxy_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 22:01:26.000000 galaxy-util-23.0.4/galaxy_util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-30 22:01:26.000000 galaxy-util-23.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-30 22:00:50.000000 galaxy-util-23.0.4/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:47:42.000000 galaxy-util-23.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-07-30 10:47:07.000000 galaxy-util-23.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-30 10:47:42.000000 galaxy-util-23.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:47:42.000000 galaxy-util-23.0.5/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:47:42.000000 galaxy-util-23.0.5/galaxy/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/exceptions/error_codes.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/exceptions/error_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:47:42.000000 galaxy-util-23.0.5/galaxy/util/
+-rw-r--r--   0 runner    (1001) docker     (123)    61298 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/aliaspickler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/bool_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/bunch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/bytesize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13411 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/compression_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:47:42.000000 galaxy-util-23.0.5/galaxy/util/custom_logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/custom_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/custom_logging/fluent_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7819 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/dbkeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/dictifiable.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/docutils_template.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/drs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/facts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/filelock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/form_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/hash_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/image_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/inflection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/jstree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/lazy_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/monitors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/odict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/oset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:47:42.000000 galaxy-util-23.0.5/galaxy/util/path/
+-rw-r--r--   0 runner    (1001) docker     (123)    16902 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/path/ntpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/path/posixpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/permutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/plugin_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7913 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/renamed_temporary_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/rules_dsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/rules_dsl_spec.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/sanitize_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/simplegraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/sleeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/submodules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/themes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:47:42.000000 galaxy-util-23.0.5/galaxy/util/tool_shed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/tool_shed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13020 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/tool_shed/common_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/tool_shed/encoding_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/tool_shed/tool_shed_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/tool_shed/xml_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/tool_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/topsort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/ucsc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/unittest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:47:42.000000 galaxy-util-23.0.5/galaxy/util/unittest_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/unittest_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11797 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/xml_macros.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/yaml_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/util/zipstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/galaxy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:47:42.000000 galaxy-util-23.0.5/galaxy_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-30 10:47:42.000000 galaxy-util-23.0.5/galaxy_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-30 10:47:42.000000 galaxy-util-23.0.5/galaxy_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 10:47:42.000000 galaxy-util-23.0.5/galaxy_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-30 10:47:42.000000 galaxy-util-23.0.5/galaxy_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-30 10:47:42.000000 galaxy-util-23.0.5/galaxy_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-30 10:47:42.000000 galaxy-util-23.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-30 10:47:08.000000 galaxy-util-23.0.5/test-requirements.txt
```

### Comparing `galaxy-util-23.0.4/HISTORY.rst` & `galaxy-util-23.0.5/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.5 (2023-07-29)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 23.0.4 (2023-06-30)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.3 (2023-06-26)
```

### Comparing `galaxy-util-23.0.4/LICENSE` & `galaxy-util-23.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/PKG-INFO` & `galaxy-util-23.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-util
-Version: 23.0.4
+Version: 23.0.5
 Summary: Galaxy generic utilities
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -44,14 +44,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.5 (2023-07-29)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 23.0.4 (2023-06-30)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.3 (2023-06-26)
```

### Comparing `galaxy-util-23.0.4/galaxy/exceptions/__init__.py` & `galaxy-util-23.0.5/galaxy/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/exceptions/error_codes.json` & `galaxy-util-23.0.5/galaxy/exceptions/error_codes.json`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/exceptions/error_codes.py` & `galaxy-util-23.0.5/galaxy/exceptions/error_codes.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/__init__.py` & `galaxy-util-23.0.5/galaxy/util/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/aliaspickler.py` & `galaxy-util-23.0.5/galaxy/util/aliaspickler.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/bool_expressions.py` & `galaxy-util-23.0.5/galaxy/util/bool_expressions.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/bunch.py` & `galaxy-util-23.0.5/galaxy/util/bunch.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/bytesize.py` & `galaxy-util-23.0.5/galaxy/util/bytesize.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/checkers.py` & `galaxy-util-23.0.5/galaxy/util/checkers.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/commands.py` & `galaxy-util-23.0.5/galaxy/util/commands.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/compression_utils.py` & `galaxy-util-23.0.5/galaxy/util/compression_utils.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/custom_logging/fluent_log.py` & `galaxy-util-23.0.5/galaxy/util/custom_logging/fluent_log.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/dbkeys.py` & `galaxy-util-23.0.5/galaxy/util/dbkeys.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/dictifiable.py` & `galaxy-util-23.0.5/galaxy/util/dictifiable.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/drs.py` & `galaxy-util-23.0.5/galaxy/util/drs.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/expressions.py` & `galaxy-util-23.0.5/galaxy/util/expressions.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/facts.py` & `galaxy-util-23.0.5/galaxy/util/facts.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/filelock.py` & `galaxy-util-23.0.5/galaxy/util/filelock.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/form_builder.py` & `galaxy-util-23.0.5/galaxy/util/form_builder.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/hash_util.py` & `galaxy-util-23.0.5/galaxy/util/hash_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/heartbeat.py` & `galaxy-util-23.0.5/galaxy/util/heartbeat.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/image_util.py` & `galaxy-util-23.0.5/galaxy/util/image_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/inflection.py` & `galaxy-util-23.0.5/galaxy/util/inflection.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/json.py` & `galaxy-util-23.0.5/galaxy/util/json.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/jstree.py` & `galaxy-util-23.0.5/galaxy/util/jstree.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/lazy_process.py` & `galaxy-util-23.0.5/galaxy/util/lazy_process.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/monitors.py` & `galaxy-util-23.0.5/galaxy/util/monitors.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/odict.py` & `galaxy-util-23.0.5/galaxy/util/odict.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/oset.py` & `galaxy-util-23.0.5/galaxy/util/oset.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/path/__init__.py` & `galaxy-util-23.0.5/galaxy/util/path/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/permutations.py` & `galaxy-util-23.0.5/galaxy/util/permutations.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/plugin_config.py` & `galaxy-util-23.0.5/galaxy/util/plugin_config.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/properties.py` & `galaxy-util-23.0.5/galaxy/util/properties.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/renamed_temporary_file.py` & `galaxy-util-23.0.5/galaxy/util/renamed_temporary_file.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/resources.py` & `galaxy-util-23.0.5/galaxy/util/resources.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/rules_dsl.py` & `galaxy-util-23.0.5/galaxy/util/rules_dsl.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/rules_dsl_spec.yml` & `galaxy-util-23.0.5/galaxy/util/rules_dsl_spec.yml`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/sanitize_html.py` & `galaxy-util-23.0.5/galaxy/util/sanitize_html.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/script.py` & `galaxy-util-23.0.5/galaxy/util/script.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/search.py` & `galaxy-util-23.0.5/galaxy/util/search.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/simplegraph.py` & `galaxy-util-23.0.5/galaxy/util/simplegraph.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/sleeper.py` & `galaxy-util-23.0.5/galaxy/util/sleeper.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/sockets.py` & `galaxy-util-23.0.5/galaxy/util/sockets.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/specs.py` & `galaxy-util-23.0.5/galaxy/util/specs.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/sqlite.py` & `galaxy-util-23.0.5/galaxy/util/sqlite.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/submodules.py` & `galaxy-util-23.0.5/galaxy/util/submodules.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/task.py` & `galaxy-util-23.0.5/galaxy/util/task.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/template.py` & `galaxy-util-23.0.5/galaxy/util/template.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/themes.py` & `galaxy-util-23.0.5/galaxy/util/themes.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/tool_shed/common_util.py` & `galaxy-util-23.0.5/galaxy/util/tool_shed/common_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/tool_shed/encoding_util.py` & `galaxy-util-23.0.5/galaxy/util/tool_shed/encoding_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/tool_shed/tool_shed_registry.py` & `galaxy-util-23.0.5/galaxy/util/tool_shed/tool_shed_registry.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/tool_shed/xml_util.py` & `galaxy-util-23.0.5/galaxy/util/tool_shed/xml_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/topsort.py` & `galaxy-util-23.0.5/galaxy/util/topsort.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/ucsc.py` & `galaxy-util-23.0.5/galaxy/util/ucsc.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/unittest.py` & `galaxy-util-23.0.5/galaxy/util/unittest.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/unittest_utils/__init__.py` & `galaxy-util-23.0.5/galaxy/util/unittest_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/validation.py` & `galaxy-util-23.0.5/galaxy/util/validation.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/watcher.py` & `galaxy-util-23.0.5/galaxy/util/watcher.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/xml_macros.py` & `galaxy-util-23.0.5/galaxy/util/xml_macros.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/yaml_util.py` & `galaxy-util-23.0.5/galaxy/util/yaml_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy/util/zipstream.py` & `galaxy-util-23.0.5/galaxy/util/zipstream.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/galaxy_util.egg-info/PKG-INFO` & `galaxy-util-23.0.5/galaxy_util.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-util
-Version: 23.0.4
+Version: 23.0.5
 Summary: Galaxy generic utilities
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -44,14 +44,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.5 (2023-07-29)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 23.0.4 (2023-06-30)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.3 (2023-06-26)
```

### Comparing `galaxy-util-23.0.4/galaxy_util.egg-info/SOURCES.txt` & `galaxy-util-23.0.5/galaxy_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-util-23.0.4/setup.cfg` & `galaxy-util-23.0.5/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-util
 url = https://github.com/galaxyproject/galaxy
-version = 23.0.4
+version = 23.0.5
 
 [options]
 include_package_data = True
 install_requires = 
 	bleach
 	boltons
 	docutils
```

