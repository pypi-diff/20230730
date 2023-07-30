# Comparing `tmp/galaxy-config-23.0.4.tar.gz` & `tmp/galaxy-config-23.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/config/dist/.tmp-q_l_cyss/galaxy-config-23.0.4.tar", last modified: Fri Jun 30 22:01:59 2023, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/config/dist/.tmp-rycvjzr1/galaxy-config-23.0.5.tar", last modified: Sun Jul 30 10:48:13 2023, max compression
```

## Comparing `galaxy-config-23.0.4.tar` & `galaxy-config-23.0.5.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:01:59.000000 galaxy-config-23.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-30 22:00:49.000000 galaxy-config-23.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-30 22:01:59.000000 galaxy-config-23.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:01:59.000000 galaxy-config-23.0.4/galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:01:59.000000 galaxy-config-23.0.4/galaxy/config/
--rw-r--r--   0 runner    (1001) docker     (123)    62353 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20123 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/config_manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:01:59.000000 galaxy-config-23.0.4/galaxy/config/sample/
--rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/sample/auth_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/sample/build_sites.yml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/sample/container_resolvers_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/sample/data_manager_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (123)   113255 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/sample/datatypes_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/sample/disposable_email_blocklist.conf.sample
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/sample/environment_modules_mapping.yml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/sample/error_report.yml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/sample/file_sources_conf.yml.sample
--rw-r--r--   0 runner    (1001) docker     (123)   124190 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/sample/galaxy.yml.sample
--rw-r--r--   0 runner    (1001) docker     (123)    53359 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/sample/job_conf.sample.yml
--rw-r--r--   0 runner    (1001) docker     (123)    79082 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/sample/job_conf.xml.sample_advanced
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/sample/job_conf.xml.sample_basic
--rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/sample/job_metrics_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/sample/job_resource_params_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/sample/lmod_modules_mapping.yml.sample
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/sample/local_conda_mapping.yml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/sample/object_store_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (123)    10056 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/sample/oidc_backends_config.xml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/sample/oidc_config.xml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/sample/reports.yml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/sample/themes_conf.yml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/sample/tool_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/sample/tool_data_table_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/sample/tool_destinations.yml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/sample/tool_recommendations_overwrite.yml.sample
--rw-r--r--   0 runner    (1001) docker     (123)    14874 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/sample/tool_shed.yml.sample
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/sample/tool_sheds_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/sample/trs_servers_conf.yml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/sample/user_preferences_extra_conf.yml.sample
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/sample/workflow_resource_mapper_conf.yml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/sample/workflow_resource_params_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/sample/workflow_schedulers_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:01:59.000000 galaxy-config-23.0.4/galaxy/config/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)   146525 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/schemas/config_schema.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/schemas/job_config_schema.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/schemas/reports_config_schema.yml
--rw-r--r--   0 runner    (1001) docker     (123)    21370 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/schemas/tool_shed_config_schema.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/script.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/config/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:01:59.000000 galaxy-config-23.0.4/galaxy_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-30 22:01:59.000000 galaxy-config-23.0.4/galaxy_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-30 22:01:59.000000 galaxy-config-23.0.4/galaxy_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 22:01:59.000000 galaxy-config-23.0.4/galaxy_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-30 22:01:59.000000 galaxy-config-23.0.4/galaxy_config.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-30 22:01:59.000000 galaxy-config-23.0.4/galaxy_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 22:01:59.000000 galaxy-config-23.0.4/galaxy_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-30 22:01:59.000000 galaxy-config-23.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-30 22:00:50.000000 galaxy-config-23.0.4/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:48:13.000000 galaxy-config-23.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-30 10:47:08.000000 galaxy-config-23.0.5/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-30 10:47:08.000000 galaxy-config-23.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-30 10:48:13.000000 galaxy-config-23.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-30 10:47:08.000000 galaxy-config-23.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-30 10:47:08.000000 galaxy-config-23.0.5/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:48:13.000000 galaxy-config-23.0.5/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-30 10:47:08.000000 galaxy-config-23.0.5/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:48:13.000000 galaxy-config-23.0.5/galaxy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)    62353 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20123 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/config_manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:48:13.000000 galaxy-config-23.0.5/galaxy/config/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/sample/auth_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/sample/build_sites.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/sample/container_resolvers_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/sample/data_manager_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)   113255 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/sample/datatypes_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/sample/disposable_email_blocklist.conf.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/sample/environment_modules_mapping.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/sample/error_report.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/sample/file_sources_conf.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)   124190 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/sample/galaxy.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)    53359 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/sample/job_conf.sample.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    79082 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/sample/job_conf.xml.sample_advanced
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/sample/job_conf.xml.sample_basic
+-rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/sample/job_metrics_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/sample/job_resource_params_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/sample/lmod_modules_mapping.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/sample/local_conda_mapping.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/sample/object_store_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)    10056 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/sample/oidc_backends_config.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/sample/oidc_config.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/sample/reports.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/sample/themes_conf.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/sample/tool_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/sample/tool_data_table_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/sample/tool_destinations.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/sample/tool_recommendations_overwrite.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)    14874 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/sample/tool_shed.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/sample/tool_sheds_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/sample/trs_servers_conf.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/sample/user_preferences_extra_conf.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/sample/workflow_resource_mapper_conf.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/sample/workflow_resource_params_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/sample/workflow_schedulers_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:48:13.000000 galaxy-config-23.0.5/galaxy/config/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)   146525 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/schemas/config_schema.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/schemas/job_config_schema.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/schemas/reports_config_schema.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    21370 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/schemas/tool_shed_config_schema.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-30 10:47:07.000000 galaxy-config-23.0.5/galaxy/config/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 10:47:08.000000 galaxy-config-23.0.5/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:48:13.000000 galaxy-config-23.0.5/galaxy_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-30 10:48:13.000000 galaxy-config-23.0.5/galaxy_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-30 10:48:13.000000 galaxy-config-23.0.5/galaxy_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 10:48:13.000000 galaxy-config-23.0.5/galaxy_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-30 10:48:13.000000 galaxy-config-23.0.5/galaxy_config.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-30 10:48:13.000000 galaxy-config-23.0.5/galaxy_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-30 10:48:13.000000 galaxy-config-23.0.5/galaxy_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-30 10:47:08.000000 galaxy-config-23.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-30 10:48:13.000000 galaxy-config-23.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-30 10:47:08.000000 galaxy-config-23.0.5/test-requirements.txt
```

### Comparing `galaxy-config-23.0.4/HISTORY.rst` & `galaxy-config-23.0.5/HISTORY.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.5 (2023-07-29)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Minor bug fix for default mail templates by `@neoformit <https://github.com/neoformit>`_ in `#16362 <https://github.com/galaxyproject/galaxy/pull/16362>`_
+
+-------------------
 23.0.4 (2023-06-30)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.3 (2023-06-26)
```

### Comparing `galaxy-config-23.0.4/LICENSE` & `galaxy-config-23.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/PKG-INFO` & `galaxy-config-23.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-config
-Version: 23.0.4
+Version: 23.0.5
 Summary: Galaxy configuration
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,14 +42,25 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.5 (2023-07-29)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Minor bug fix for default mail templates by `@neoformit <https://github.com/neoformit>`_ in `#16362 <https://github.com/galaxyproject/galaxy/pull/16362>`_
+
+-------------------
 23.0.4 (2023-06-30)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.3 (2023-06-26)
```

### Comparing `galaxy-config-23.0.4/galaxy/config/__init__.py` & `galaxy-config-23.0.5/galaxy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/config_manage.py` & `galaxy-config-23.0.5/galaxy/config/config_manage.py`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/sample/auth_conf.xml.sample` & `galaxy-config-23.0.5/galaxy/config/sample/auth_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/sample/build_sites.yml.sample` & `galaxy-config-23.0.5/galaxy/config/sample/build_sites.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/sample/container_resolvers_conf.xml.sample` & `galaxy-config-23.0.5/galaxy/config/sample/container_resolvers_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/sample/datatypes_conf.xml.sample` & `galaxy-config-23.0.5/galaxy/config/sample/datatypes_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/sample/environment_modules_mapping.yml.sample` & `galaxy-config-23.0.5/galaxy/config/sample/environment_modules_mapping.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/sample/error_report.yml.sample` & `galaxy-config-23.0.5/galaxy/config/sample/error_report.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/sample/file_sources_conf.yml.sample` & `galaxy-config-23.0.5/galaxy/config/sample/file_sources_conf.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/sample/galaxy.yml.sample` & `galaxy-config-23.0.5/galaxy/config/sample/galaxy.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/sample/job_conf.sample.yml` & `galaxy-config-23.0.5/galaxy/config/sample/job_conf.sample.yml`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/sample/job_conf.xml.sample_advanced` & `galaxy-config-23.0.5/galaxy/config/sample/job_conf.xml.sample_advanced`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/sample/job_metrics_conf.xml.sample` & `galaxy-config-23.0.5/galaxy/config/sample/job_metrics_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/sample/job_resource_params_conf.xml.sample` & `galaxy-config-23.0.5/galaxy/config/sample/job_resource_params_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/sample/lmod_modules_mapping.yml.sample` & `galaxy-config-23.0.5/galaxy/config/sample/lmod_modules_mapping.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/sample/object_store_conf.xml.sample` & `galaxy-config-23.0.5/galaxy/config/sample/object_store_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/sample/oidc_backends_config.xml.sample` & `galaxy-config-23.0.5/galaxy/config/sample/oidc_backends_config.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/sample/oidc_config.xml.sample` & `galaxy-config-23.0.5/galaxy/config/sample/oidc_config.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/sample/reports.yml.sample` & `galaxy-config-23.0.5/galaxy/config/sample/reports.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/sample/themes_conf.yml.sample` & `galaxy-config-23.0.5/galaxy/config/sample/themes_conf.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/sample/tool_conf.xml.sample` & `galaxy-config-23.0.5/galaxy/config/sample/tool_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/sample/tool_data_table_conf.xml.sample` & `galaxy-config-23.0.5/galaxy/config/sample/tool_data_table_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/sample/tool_destinations.yml.sample` & `galaxy-config-23.0.5/galaxy/config/sample/tool_destinations.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/sample/tool_recommendations_overwrite.yml.sample` & `galaxy-config-23.0.5/galaxy/config/sample/tool_recommendations_overwrite.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/sample/tool_shed.yml.sample` & `galaxy-config-23.0.5/galaxy/config/sample/tool_shed.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/sample/trs_servers_conf.yml.sample` & `galaxy-config-23.0.5/galaxy/config/sample/trs_servers_conf.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/sample/user_preferences_extra_conf.yml.sample` & `galaxy-config-23.0.5/galaxy/config/sample/user_preferences_extra_conf.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/sample/workflow_resource_params_conf.xml.sample` & `galaxy-config-23.0.5/galaxy/config/sample/workflow_resource_params_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/sample/workflow_schedulers_conf.xml.sample` & `galaxy-config-23.0.5/galaxy/config/sample/workflow_schedulers_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/schema.py` & `galaxy-config-23.0.5/galaxy/config/schema.py`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/schemas/config_schema.yml` & `galaxy-config-23.0.5/galaxy/config/schemas/config_schema.yml`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/schemas/job_config_schema.yml` & `galaxy-config-23.0.5/galaxy/config/schemas/job_config_schema.yml`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/schemas/reports_config_schema.yml` & `galaxy-config-23.0.5/galaxy/config/schemas/reports_config_schema.yml`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/schemas/tool_shed_config_schema.yml` & `galaxy-config-23.0.5/galaxy/config/schemas/tool_shed_config_schema.yml`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/script.py` & `galaxy-config-23.0.5/galaxy/config/script.py`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy/config/templates.py` & `galaxy-config-23.0.5/galaxy/config/templates.py`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/galaxy_config.egg-info/PKG-INFO` & `galaxy-config-23.0.5/galaxy_config.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-config
-Version: 23.0.4
+Version: 23.0.5
 Summary: Galaxy configuration
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,14 +42,25 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.5 (2023-07-29)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Minor bug fix for default mail templates by `@neoformit <https://github.com/neoformit>`_ in `#16362 <https://github.com/galaxyproject/galaxy/pull/16362>`_
+
+-------------------
 23.0.4 (2023-06-30)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.3 (2023-06-26)
```

### Comparing `galaxy-config-23.0.4/galaxy_config.egg-info/SOURCES.txt` & `galaxy-config-23.0.5/galaxy_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.4/setup.cfg` & `galaxy-config-23.0.5/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-config
 url = https://github.com/galaxyproject/galaxy
-version = 23.0.4
+version = 23.0.5
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-util
 	boltons
 	jinja2
```

