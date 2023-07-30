# Comparing `tmp/nornir_scrapli-2023.1.30.post1.tar.gz` & `tmp/nornir_scrapli-2023.7.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nornir_scrapli-2023.1.30.post1.tar", last modified: Thu Feb  2 13:43:51 2023, max compression
+gzip compressed data, was "nornir_scrapli-2023.7.30.tar", last modified: Sun Jul 30 17:20:55 2023, max compression
```

## Comparing `nornir_scrapli-2023.1.30.post1.tar` & `nornir_scrapli-2023.7.30.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 13:43:51.010497 nornir_scrapli-2023.1.30.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-02-02 13:43:51.010497 nornir_scrapli-2023.1.30.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 13:43:51.006497 nornir_scrapli-2023.1.30.post1/nornir_scrapli/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9889 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 13:43:51.006497 nornir_scrapli-2023.1.30.post1/nornir_scrapli/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/functions/print_structured_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 13:43:51.006497 nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 13:43:51.006497 nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/cfg/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/cfg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/cfg/abort_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/cfg/commit_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/cfg/diff_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/cfg/get_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/cfg/get_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/cfg/load_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 13:43:51.006497 nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/core/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/core/get_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/core/send_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/core/send_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/core/send_commands_from_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/core/send_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/core/send_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/core/send_configs_from_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/core/send_interactive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 13:43:51.010497 nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/netconf/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/netconf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/netconf/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/netconf/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/netconf/delete_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/netconf/discard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/netconf/edit_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/netconf/get.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/netconf/get_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/netconf/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/netconf/rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/netconf/unlock.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/netconf/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 13:43:51.006497 nornir_scrapli-2023.1.30.post1/nornir_scrapli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-02-02 13:43:50.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-02-02 13:43:51.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 13:43:50.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-02-02 13:43:50.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-02-02 13:43:50.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-02 13:43:50.000000 nornir_scrapli-2023.1.30.post1/nornir_scrapli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/requirements-genie.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-02-02 13:43:23.000000 nornir_scrapli-2023.1.30.post1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-02-02 13:43:51.010497 nornir_scrapli-2023.1.30.post1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:20:55.280997 nornir_scrapli-2023.7.30/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-07-30 17:20:55.280997 nornir_scrapli-2023.7.30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:20:55.276997 nornir_scrapli-2023.7.30/nornir_scrapli/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9889 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:20:55.276997 nornir_scrapli-2023.7.30/nornir_scrapli/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/functions/print_structured_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:20:55.276997 nornir_scrapli-2023.7.30/nornir_scrapli/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:20:55.276997 nornir_scrapli-2023.7.30/nornir_scrapli/tasks/cfg/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/tasks/cfg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/tasks/cfg/abort_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/tasks/cfg/commit_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/tasks/cfg/diff_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/tasks/cfg/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/tasks/cfg/get_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/tasks/cfg/load_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:20:55.280997 nornir_scrapli-2023.7.30/nornir_scrapli/tasks/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/tasks/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/tasks/core/get_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/tasks/core/send_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/tasks/core/send_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/tasks/core/send_commands_from_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/tasks/core/send_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/tasks/core/send_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/tasks/core/send_configs_from_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/tasks/core/send_interactive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:20:55.280997 nornir_scrapli-2023.7.30/nornir_scrapli/tasks/netconf/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/tasks/netconf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/tasks/netconf/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/tasks/netconf/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/tasks/netconf/delete_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/tasks/netconf/discard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/tasks/netconf/edit_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/tasks/netconf/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/tasks/netconf/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/tasks/netconf/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/tasks/netconf/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/tasks/netconf/unlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/nornir_scrapli/tasks/netconf/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:20:55.276997 nornir_scrapli-2023.7.30/nornir_scrapli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-07-30 17:20:55.000000 nornir_scrapli-2023.7.30/nornir_scrapli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-30 17:20:55.000000 nornir_scrapli-2023.7.30/nornir_scrapli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 17:20:55.000000 nornir_scrapli-2023.7.30/nornir_scrapli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-30 17:20:55.000000 nornir_scrapli-2023.7.30/nornir_scrapli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-30 17:20:55.000000 nornir_scrapli-2023.7.30/nornir_scrapli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-30 17:20:55.000000 nornir_scrapli-2023.7.30/nornir_scrapli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/requirements-genie.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-30 17:20:36.000000 nornir_scrapli-2023.7.30/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-30 17:20:55.280997 nornir_scrapli-2023.7.30/setup.cfg
```

### Comparing `nornir_scrapli-2023.1.30.post1/LICENSE` & `nornir_scrapli-2023.7.30/LICENSE`

 * *Files identical despite different names*

### Comparing `nornir_scrapli-2023.1.30.post1/PKG-INFO` & `nornir_scrapli-2023.7.30/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nornir_scrapli
-Version: 2023.1.30.post1
+Version: 2023.7.30
 Summary: Scrapli's plugin for Nornir
 Author-email: Carl Montanari <carl.r.montanari@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Carl Montanari
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,15 +23,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/scrapli/nornir_scrapli
 Project-URL: Docs, https://scrapli.github.io/nornir_scrapli/
-Keywords: ssh,telnet,netconf,automation,network,cisco,iosxr,iosxe,nxos,arista,eos,juniper,junos
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
-Metadata-Version: 2.1 Name: nornir_scrapli Version: 2023.1.30.post1 Summary:
+Metadata-Version: 2.1 Name: nornir_scrapli Version: 2023.7.30 Summary:
 Scrapli's plugin for Nornir Author-email: Carl Montanari
 r.montanari@gmail.com> License: MIT License Copyright (c) 2021 Carl Montanari
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
@@ -13,15 +13,15 @@
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
 EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
 OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://github.com/scrapli/
 nornir_scrapli Project-URL: Docs, https://scrapli.github.io/nornir_scrapli/
 Keywords:
-ssh,telnet,netconf,automation,network,cisco,iosxr,iosxe,nxos,arista,eos,juniper,junos
+arista,automation,cisco,eos,iosxe,iosxr,juniper,junos,netconf,network,nxos,ssh,telnet
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: POSIX :: Linux Classifier: Operating System :: MacOS Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Topic :: Software Development ::
```

### Comparing `nornir_scrapli-2023.1.30.post1/README.md` & `nornir_scrapli-2023.7.30/README.md`

 * *Files identical despite different names*

### Comparing `nornir_scrapli-2023.1.30.post1/nornir_scrapli/connection.py` & `nornir_scrapli-2023.7.30/nornir_scrapli/connection.py`

 * *Files identical despite different names*

### Comparing `nornir_scrapli-2023.1.30.post1/nornir_scrapli/functions/print_structured_result.py` & `nornir_scrapli-2023.7.30/nornir_scrapli/functions/print_structured_result.py`

 * *Files identical despite different names*

### Comparing `nornir_scrapli-2023.1.30.post1/nornir_scrapli/helper.py` & `nornir_scrapli-2023.7.30/nornir_scrapli/helper.py`

 * *Files identical despite different names*

### Comparing `nornir_scrapli-2023.1.30.post1/nornir_scrapli/result.py` & `nornir_scrapli-2023.7.30/nornir_scrapli/result.py`

 * *Files identical despite different names*

### Comparing `nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/__init__.py` & `nornir_scrapli-2023.7.30/nornir_scrapli/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/cfg/abort_config.py` & `nornir_scrapli-2023.7.30/nornir_scrapli/tasks/cfg/abort_config.py`

 * *Files identical despite different names*

### Comparing `nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/cfg/commit_config.py` & `nornir_scrapli-2023.7.30/nornir_scrapli/tasks/cfg/commit_config.py`

 * *Files identical despite different names*

### Comparing `nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/cfg/diff_config.py` & `nornir_scrapli-2023.7.30/nornir_scrapli/tasks/cfg/diff_config.py`

 * *Files identical despite different names*

### Comparing `nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/cfg/get_config.py` & `nornir_scrapli-2023.7.30/nornir_scrapli/tasks/cfg/get_config.py`

 * *Files identical despite different names*

### Comparing `nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/cfg/get_version.py` & `nornir_scrapli-2023.7.30/nornir_scrapli/tasks/cfg/get_version.py`

 * *Files identical despite different names*

### Comparing `nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/cfg/load_config.py` & `nornir_scrapli-2023.7.30/nornir_scrapli/tasks/cfg/load_config.py`

 * *Files identical despite different names*

### Comparing `nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/core/get_prompt.py` & `nornir_scrapli-2023.7.30/nornir_scrapli/tasks/core/get_prompt.py`

 * *Files identical despite different names*

### Comparing `nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/core/send_command.py` & `nornir_scrapli-2023.7.30/nornir_scrapli/tasks/core/send_command.py`

 * *Files identical despite different names*

### Comparing `nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/core/send_commands.py` & `nornir_scrapli-2023.7.30/nornir_scrapli/tasks/core/send_commands.py`

 * *Files identical despite different names*

### Comparing `nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/core/send_commands_from_file.py` & `nornir_scrapli-2023.7.30/nornir_scrapli/tasks/core/send_commands_from_file.py`

 * *Files identical despite different names*

### Comparing `nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/core/send_config.py` & `nornir_scrapli-2023.7.30/nornir_scrapli/tasks/core/send_config.py`

 * *Files identical despite different names*

### Comparing `nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/core/send_configs.py` & `nornir_scrapli-2023.7.30/nornir_scrapli/tasks/core/send_configs.py`

 * *Files identical despite different names*

### Comparing `nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/core/send_configs_from_file.py` & `nornir_scrapli-2023.7.30/nornir_scrapli/tasks/core/send_configs_from_file.py`

 * *Files identical despite different names*

### Comparing `nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/core/send_interactive.py` & `nornir_scrapli-2023.7.30/nornir_scrapli/tasks/core/send_interactive.py`

 * *Files identical despite different names*

### Comparing `nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/netconf/capabilities.py` & `nornir_scrapli-2023.7.30/nornir_scrapli/tasks/netconf/capabilities.py`

 * *Files identical despite different names*

### Comparing `nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/netconf/commit.py` & `nornir_scrapli-2023.7.30/nornir_scrapli/tasks/netconf/commit.py`

 * *Files identical despite different names*

### Comparing `nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/netconf/delete_config.py` & `nornir_scrapli-2023.7.30/nornir_scrapli/tasks/netconf/delete_config.py`

 * *Files identical despite different names*

### Comparing `nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/netconf/discard.py` & `nornir_scrapli-2023.7.30/nornir_scrapli/tasks/netconf/discard.py`

 * *Files identical despite different names*

### Comparing `nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/netconf/edit_config.py` & `nornir_scrapli-2023.7.30/nornir_scrapli/tasks/netconf/edit_config.py`

 * *Files identical despite different names*

### Comparing `nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/netconf/get.py` & `nornir_scrapli-2023.7.30/nornir_scrapli/tasks/netconf/get.py`

 * *Files identical despite different names*

### Comparing `nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/netconf/get_config.py` & `nornir_scrapli-2023.7.30/nornir_scrapli/tasks/netconf/get_config.py`

 * *Files identical despite different names*

### Comparing `nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/netconf/lock.py` & `nornir_scrapli-2023.7.30/nornir_scrapli/tasks/netconf/lock.py`

 * *Files identical despite different names*

### Comparing `nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/netconf/rpc.py` & `nornir_scrapli-2023.7.30/nornir_scrapli/tasks/netconf/rpc.py`

 * *Files identical despite different names*

### Comparing `nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/netconf/unlock.py` & `nornir_scrapli-2023.7.30/nornir_scrapli/tasks/netconf/unlock.py`

 * *Files identical despite different names*

### Comparing `nornir_scrapli-2023.1.30.post1/nornir_scrapli/tasks/netconf/validate.py` & `nornir_scrapli-2023.7.30/nornir_scrapli/tasks/netconf/validate.py`

 * *Files identical despite different names*

### Comparing `nornir_scrapli-2023.1.30.post1/nornir_scrapli.egg-info/PKG-INFO` & `nornir_scrapli-2023.7.30/nornir_scrapli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nornir-scrapli
-Version: 2023.1.30.post1
+Version: 2023.7.30
 Summary: Scrapli's plugin for Nornir
 Author-email: Carl Montanari <carl.r.montanari@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Carl Montanari
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,15 +23,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/scrapli/nornir_scrapli
 Project-URL: Docs, https://scrapli.github.io/nornir_scrapli/
-Keywords: ssh,telnet,netconf,automation,network,cisco,iosxr,iosxe,nxos,arista,eos,juniper,junos
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
-Metadata-Version: 2.1 Name: nornir-scrapli Version: 2023.1.30.post1 Summary:
+Metadata-Version: 2.1 Name: nornir-scrapli Version: 2023.7.30 Summary:
 Scrapli's plugin for Nornir Author-email: Carl Montanari
 r.montanari@gmail.com> License: MIT License Copyright (c) 2021 Carl Montanari
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
@@ -13,15 +13,15 @@
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
 EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
 OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://github.com/scrapli/
 nornir_scrapli Project-URL: Docs, https://scrapli.github.io/nornir_scrapli/
 Keywords:
-ssh,telnet,netconf,automation,network,cisco,iosxr,iosxe,nxos,arista,eos,juniper,junos
+arista,automation,cisco,eos,iosxe,iosxr,juniper,junos,netconf,network,nxos,ssh,telnet
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: POSIX :: Linux Classifier: Operating System :: MacOS Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Topic :: Software Development ::
```

### Comparing `nornir_scrapli-2023.1.30.post1/nornir_scrapli.egg-info/SOURCES.txt` & `nornir_scrapli-2023.7.30/nornir_scrapli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nornir_scrapli-2023.1.30.post1/nornir_scrapli.egg-info/requires.txt` & `nornir_scrapli-2023.7.30/nornir_scrapli.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 scrapli>=2022.01.30
 scrapli_cfg>=2022.01.30
 scrapli_community>=2021.01.30
 scrapli_netconf>=2022.01.30
 textfsm>=1.1.0
 
 [dev]
-black==22.12.0
+black<24.0.0,>=23.3.0
 darglint<2.0.0,>=1.8.1
 isort<6.0.0,>=5.10.1
-mypy==0.991
-nox==2022.11.21
+mypy<2.0.0,>1.0.0
+nox==2023.4.22
 pycodestyle<3.0.0,>=2.8.0
 pydocstyle<7.0.0,>=6.1.1
 pylama<9.0.0,>=8.4.0
-pylint==2.15.10
+pylint==2.17.5
 pytest-cov<5.0.0,>=3.0.0
 pytest<8.0.0,>=7.0.0
 toml<1.0.0,>=0.10.2
 
 [dev:sys_platform != "win32" and python_version < "3.11"]
 genie>=20.2
 pyats>=20.2
```

### Comparing `nornir_scrapli-2023.1.30.post1/pyproject.toml` & `nornir_scrapli-2023.7.30/pyproject.toml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -26,27 +26,27 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 keywords = [
-    "ssh",
-    "telnet",
-    "netconf",
+    "arista",
     "automation",
-    "network",
     "cisco",
-    "iosxr",
-    "iosxe",
-    "nxos",
-    "arista",
     "eos",
+    "iosxe",
+    "iosxr",
     "juniper",
     "junos",
+    "netconf",
+    "network",
+    "nxos",
+    "ssh",
+    "telnet",
 ]
 
 [project.urls]
 Homepage = "https://github.com/scrapli/nornir_scrapli"
 Docs = "https://scrapli.github.io/nornir_scrapli/"
 
 [project.entry-points."nornir.plugins.connections"]
```

