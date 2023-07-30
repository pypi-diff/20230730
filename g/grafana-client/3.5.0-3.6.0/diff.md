# Comparing `tmp/grafana-client-3.5.0.tar.gz` & `tmp/grafana-client-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grafana-client-3.5.0.tar", last modified: Wed Dec  7 22:29:37 2022, max compression
+gzip compressed data, was "grafana-client-3.6.0.tar", last modified: Sun Jul 30 19:56:55 2023, max compression
```

## Comparing `grafana-client-3.5.0.tar` & `grafana-client-3.6.0.tar`

### file list

```diff
@@ -1,88 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 22:29:37.788568 grafana-client-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    22380 2022-12-07 22:29:17.000000 grafana-client-3.5.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2022-12-07 22:29:17.000000 grafana-client-3.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      215 2022-12-07 22:29:17.000000 grafana-client-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11736 2022-12-07 22:29:37.788568 grafana-client-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8961 2022-12-07 22:29:17.000000 grafana-client-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      124 2022-12-07 22:29:17.000000 grafana-client-3.5.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 22:29:37.772568 grafana-client-3.5.0/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2022-12-07 22:29:17.000000 grafana-client-3.5.0/conda/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2022-12-07 22:29:17.000000 grafana-client-3.5.0/conda/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 22:29:37.772568 grafana-client-3.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2022-12-07 22:29:17.000000 grafana-client-3.5.0/docs/backlog.md
--rw-r--r--   0 runner    (1001) docker     (123)      814 2022-12-07 22:29:17.000000 grafana-client-3.5.0/docs/datasource-state.md
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2022-12-07 22:29:17.000000 grafana-client-3.5.0/docs/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 22:29:37.776568 grafana-client-3.5.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2022-12-07 22:29:17.000000 grafana-client-3.5.0/examples/datasource-health-check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2022-12-07 22:29:17.000000 grafana-client-3.5.0/examples/datasource-health-check.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2022-12-07 22:29:17.000000 grafana-client-3.5.0/examples/datasource-health-probe.py
--rw-r--r--   0 runner    (1001) docker     (123)     6798 2022-12-07 22:29:17.000000 grafana-client-3.5.0/examples/datasource-health-probe.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2022-12-07 22:29:17.000000 grafana-client-3.5.0/examples/datasource-smartquery.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2022-12-07 22:29:17.000000 grafana-client-3.5.0/examples/folders-dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2022-12-07 22:29:17.000000 grafana-client-3.5.0/examples/grafanalib-upload-dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2022-12-07 22:29:17.000000 grafana-client-3.5.0/examples/team.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 22:29:37.776568 grafana-client-3.5.0/grafana_client/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2022-12-07 22:29:17.000000 grafana-client-3.5.0/grafana_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2022-12-07 22:29:17.000000 grafana-client-3.5.0/grafana_client/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2022-12-07 22:29:17.000000 grafana-client-3.5.0/grafana_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 22:29:37.780568 grafana-client-3.5.0/grafana_client/elements/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2022-12-07 22:29:17.000000 grafana-client-3.5.0/grafana_client/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2022-12-07 22:29:17.000000 grafana-client-3.5.0/grafana_client/elements/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2022-12-07 22:29:17.000000 grafana-client-3.5.0/grafana_client/elements/alerting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2022-12-07 22:29:17.000000 grafana-client-3.5.0/grafana_client/elements/alertingprovisioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2022-12-07 22:29:17.000000 grafana-client-3.5.0/grafana_client/elements/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2022-12-07 22:29:17.000000 grafana-client-3.5.0/grafana_client/elements/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2022-12-07 22:29:17.000000 grafana-client-3.5.0/grafana_client/elements/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2022-12-07 22:29:17.000000 grafana-client-3.5.0/grafana_client/elements/dashboard_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)    25903 2022-12-07 22:29:17.000000 grafana-client-3.5.0/grafana_client/elements/datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2022-12-07 22:29:17.000000 grafana-client-3.5.0/grafana_client/elements/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2022-12-07 22:29:17.000000 grafana-client-3.5.0/grafana_client/elements/health.py
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2022-12-07 22:29:17.000000 grafana-client-3.5.0/grafana_client/elements/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     6913 2022-12-07 22:29:17.000000 grafana-client-3.5.0/grafana_client/elements/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2022-12-07 22:29:17.000000 grafana-client-3.5.0/grafana_client/elements/rbac.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2022-12-07 22:29:17.000000 grafana-client-3.5.0/grafana_client/elements/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2022-12-07 22:29:17.000000 grafana-client-3.5.0/grafana_client/elements/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2022-12-07 22:29:17.000000 grafana-client-3.5.0/grafana_client/elements/team.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2022-12-07 22:29:17.000000 grafana-client-3.5.0/grafana_client/elements/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     9610 2022-12-07 22:29:17.000000 grafana-client-3.5.0/grafana_client/knowledge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2022-12-07 22:29:17.000000 grafana-client-3.5.0/grafana_client/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2022-12-07 22:29:17.000000 grafana-client-3.5.0/grafana_client/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2022-12-07 22:29:37.000000 grafana-client-3.5.0/grafana_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 22:29:37.776568 grafana-client-3.5.0/grafana_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11736 2022-12-07 22:29:37.000000 grafana-client-3.5.0/grafana_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2022-12-07 22:29:37.000000 grafana-client-3.5.0/grafana_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-07 22:29:37.000000 grafana-client-3.5.0/grafana_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-07 22:29:37.000000 grafana-client-3.5.0/grafana_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      316 2022-12-07 22:29:37.000000 grafana-client-3.5.0/grafana_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2022-12-07 22:29:37.000000 grafana-client-3.5.0/grafana_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      920 2022-12-07 22:29:17.000000 grafana-client-3.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2022-12-07 22:29:37.788568 grafana-client-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      351 2022-12-07 22:29:17.000000 grafana-client-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 22:29:37.784568 grafana-client-3.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2022-12-07 22:29:17.000000 grafana-client-3.5.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 22:29:37.788568 grafana-client-3.5.0/test/elements/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-07 22:29:17.000000 grafana-client-3.5.0/test/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2022-12-07 22:29:17.000000 grafana-client-3.5.0/test/elements/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2022-12-07 22:29:17.000000 grafana-client-3.5.0/test/elements/test_alerting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2022-12-07 22:29:17.000000 grafana-client-3.5.0/test/elements/test_alertingprovisioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     7022 2022-12-07 22:29:17.000000 grafana-client-3.5.0/test/elements/test_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8709 2022-12-07 22:29:17.000000 grafana-client-3.5.0/test/elements/test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     7182 2022-12-07 22:29:17.000000 grafana-client-3.5.0/test/elements/test_dashboard_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13604 2022-12-07 22:29:17.000000 grafana-client-3.5.0/test/elements/test_datasource_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2022-12-07 22:29:17.000000 grafana-client-3.5.0/test/elements/test_datasource_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)    43142 2022-12-07 22:29:17.000000 grafana-client-3.5.0/test/elements/test_datasource_health.py
--rw-r--r--   0 runner    (1001) docker     (123)     9543 2022-12-07 22:29:17.000000 grafana-client-3.5.0/test/elements/test_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2022-12-07 22:29:17.000000 grafana-client-3.5.0/test/elements/test_health.py
--rw-r--r--   0 runner    (1001) docker     (123)    11641 2022-12-07 22:29:17.000000 grafana-client-3.5.0/test/elements/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     8009 2022-12-07 22:29:17.000000 grafana-client-3.5.0/test/elements/test_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2022-12-07 22:29:17.000000 grafana-client-3.5.0/test/elements/test_rbac.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2022-12-07 22:29:17.000000 grafana-client-3.5.0/test/elements/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2022-12-07 22:29:17.000000 grafana-client-3.5.0/test/elements/test_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)    11833 2022-12-07 22:29:17.000000 grafana-client-3.5.0/test/elements/test_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2022-12-07 22:29:17.000000 grafana-client-3.5.0/test/elements/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2022-12-07 22:29:17.000000 grafana-client-3.5.0/test/test_grafana_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2022-12-07 22:29:17.000000 grafana-client-3.5.0/test/test_grafana_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2022-12-07 22:29:17.000000 grafana-client-3.5.0/test/test_knowledge.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2022-12-07 22:29:17.000000 grafana-client-3.5.0/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2022-12-07 22:29:17.000000 grafana-client-3.5.0/test/test_package_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2022-12-07 22:29:17.000000 grafana-client-3.5.0/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:56:55.862365 grafana-client-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    22650 2023-07-30 19:56:42.000000 grafana-client-3.6.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-30 19:56:42.000000 grafana-client-3.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-30 19:56:42.000000 grafana-client-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-07-30 19:56:55.862365 grafana-client-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9134 2023-07-30 19:56:42.000000 grafana-client-3.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-30 19:56:42.000000 grafana-client-3.6.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:56:55.850365 grafana-client-3.6.0/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-30 19:56:42.000000 grafana-client-3.6.0/conda/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-30 19:56:42.000000 grafana-client-3.6.0/conda/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:56:55.854365 grafana-client-3.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-30 19:56:42.000000 grafana-client-3.6.0/docs/backlog.md
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-30 19:56:42.000000 grafana-client-3.6.0/docs/datasource-state.md
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-30 19:56:42.000000 grafana-client-3.6.0/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-30 19:56:42.000000 grafana-client-3.6.0/docs/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:56:55.854365 grafana-client-3.6.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-30 19:56:42.000000 grafana-client-3.6.0/examples/datasource-health-check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-30 19:56:42.000000 grafana-client-3.6.0/examples/datasource-health-check.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-07-30 19:56:42.000000 grafana-client-3.6.0/examples/datasource-health-probe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-07-30 19:56:42.000000 grafana-client-3.6.0/examples/datasource-health-probe.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-30 19:56:42.000000 grafana-client-3.6.0/examples/datasource-smartquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-30 19:56:42.000000 grafana-client-3.6.0/examples/folders-dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-30 19:56:42.000000 grafana-client-3.6.0/examples/grafana-tokenauth-healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-30 19:56:42.000000 grafana-client-3.6.0/examples/grafanalib-upload-dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-30 19:56:42.000000 grafana-client-3.6.0/examples/team.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:56:55.854365 grafana-client-3.6.0/grafana_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-30 19:56:42.000000 grafana-client-3.6.0/grafana_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-30 19:56:42.000000 grafana-client-3.6.0/grafana_client/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-07-30 19:56:42.000000 grafana-client-3.6.0/grafana_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:56:55.858365 grafana-client-3.6.0/grafana_client/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-30 19:56:42.000000 grafana-client-3.6.0/grafana_client/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-30 19:56:42.000000 grafana-client-3.6.0/grafana_client/elements/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-30 19:56:42.000000 grafana-client-3.6.0/grafana_client/elements/alerting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-07-30 19:56:42.000000 grafana-client-3.6.0/grafana_client/elements/alertingprovisioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-07-30 19:56:42.000000 grafana-client-3.6.0/grafana_client/elements/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-30 19:56:42.000000 grafana-client-3.6.0/grafana_client/elements/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-30 19:56:42.000000 grafana-client-3.6.0/grafana_client/elements/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-07-30 19:56:42.000000 grafana-client-3.6.0/grafana_client/elements/dashboard_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25902 2023-07-30 19:56:42.000000 grafana-client-3.6.0/grafana_client/elements/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-30 19:56:42.000000 grafana-client-3.6.0/grafana_client/elements/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-30 19:56:42.000000 grafana-client-3.6.0/grafana_client/elements/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-07-30 19:56:42.000000 grafana-client-3.6.0/grafana_client/elements/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-07-30 19:56:42.000000 grafana-client-3.6.0/grafana_client/elements/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-30 19:56:42.000000 grafana-client-3.6.0/grafana_client/elements/rbac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-30 19:56:42.000000 grafana-client-3.6.0/grafana_client/elements/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-30 19:56:42.000000 grafana-client-3.6.0/grafana_client/elements/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-07-30 19:56:42.000000 grafana-client-3.6.0/grafana_client/elements/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-07-30 19:56:42.000000 grafana-client-3.6.0/grafana_client/elements/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9610 2023-07-30 19:56:42.000000 grafana-client-3.6.0/grafana_client/knowledge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-30 19:56:42.000000 grafana-client-3.6.0/grafana_client/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-30 19:56:42.000000 grafana-client-3.6.0/grafana_client/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-30 19:56:55.000000 grafana-client-3.6.0/grafana_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:56:55.858365 grafana-client-3.6.0/grafana_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-07-30 19:56:55.000000 grafana-client-3.6.0/grafana_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-30 19:56:55.000000 grafana-client-3.6.0/grafana_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 19:56:55.000000 grafana-client-3.6.0/grafana_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 19:56:55.000000 grafana-client-3.6.0/grafana_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-30 19:56:55.000000 grafana-client-3.6.0/grafana_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-30 19:56:55.000000 grafana-client-3.6.0/grafana_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-30 19:56:42.000000 grafana-client-3.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-07-30 19:56:55.866366 grafana-client-3.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-30 19:56:42.000000 grafana-client-3.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:56:55.862365 grafana-client-3.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-30 19:56:42.000000 grafana-client-3.6.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:56:55.862365 grafana-client-3.6.0/test/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 19:56:42.000000 grafana-client-3.6.0/test/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-07-30 19:56:42.000000 grafana-client-3.6.0/test/elements/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-30 19:56:42.000000 grafana-client-3.6.0/test/elements/test_alerting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-07-30 19:56:42.000000 grafana-client-3.6.0/test/elements/test_alertingprovisioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-07-30 19:56:42.000000 grafana-client-3.6.0/test/elements/test_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8709 2023-07-30 19:56:42.000000 grafana-client-3.6.0/test/elements/test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-07-30 19:56:42.000000 grafana-client-3.6.0/test/elements/test_dashboard_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-07-30 19:56:42.000000 grafana-client-3.6.0/test/elements/test_datasource_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-07-30 19:56:42.000000 grafana-client-3.6.0/test/elements/test_datasource_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43142 2023-07-30 19:56:42.000000 grafana-client-3.6.0/test/elements/test_datasource_health.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-07-30 19:56:42.000000 grafana-client-3.6.0/test/elements/test_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-30 19:56:42.000000 grafana-client-3.6.0/test/elements/test_health.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11641 2023-07-30 19:56:42.000000 grafana-client-3.6.0/test/elements/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-07-30 19:56:42.000000 grafana-client-3.6.0/test/elements/test_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-07-30 19:56:42.000000 grafana-client-3.6.0/test/elements/test_rbac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-30 19:56:42.000000 grafana-client-3.6.0/test/elements/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-30 19:56:42.000000 grafana-client-3.6.0/test/elements/test_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11833 2023-07-30 19:56:42.000000 grafana-client-3.6.0/test/elements/test_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-07-30 19:56:42.000000 grafana-client-3.6.0/test/elements/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6875 2023-07-30 19:56:42.000000 grafana-client-3.6.0/test/test_grafana_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-07-30 19:56:42.000000 grafana-client-3.6.0/test/test_grafana_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-30 19:56:42.000000 grafana-client-3.6.0/test/test_knowledge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-30 19:56:42.000000 grafana-client-3.6.0/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-30 19:56:42.000000 grafana-client-3.6.0/test/test_package_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-30 19:56:42.000000 grafana-client-3.6.0/test/test_util.py
```

### Comparing `grafana-client-3.5.0/CHANGELOG.md` & `grafana-client-3.6.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 # CHANGELOG
 
 ## unreleased
 
 
+## 3.6.0 (2023-07-30)
+
+* Add missing argument `dashboard_uid` to `get_annotation` method.
+  Thanks, @nikita-b.
+* Add API method `get_alertrules_all`. Thanks, @harish422.
+* Improve usability and documentation for changing timeout settings.
+  Thanks, @bukem and @dheeg.
+
+
 ## 3.5.0 (2022-12-07)
 
 * Add support for a subset of the "RBAC" API. Thanks, @hamelg.
 
 
 ## 3.4.0 (2022-12-03)
```

### Comparing `grafana-client-3.5.0/LICENSE` & `grafana-client-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/PKG-INFO` & `grafana-client-3.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grafana-client
-Version: 3.5.0
+Version: 3.6.0
 Summary: A client library for accessing the Grafana HTTP API, written in Python
 Home-page: https://github.com/panodata/grafana-client
 Author: Andrew Prokhorenkov
 Author-email: andrew.prokhorenkov@gmail.com
 Maintainer: Andreas Motl
 Maintainer-email: andreas.motl@panodata.org
 License: MIT
@@ -192,14 +192,23 @@
 grafana = GrafanaApi.from_env()
 ```
 
 Please note that, on top of the specific examples above, the object obtained by
 `credential` can be an arbitrary `requests.auth.AuthBase` instance.
 
 
+## Timeout settings
+
+The default timeout value is five seconds, used for both connect and read timeout.
+
+The constructors of `GrafanaApi` and `GrafanaClient`, as well as the factory methods
+`from_url` and `from_env` accept the `timeout` argument, which can be obtained as a
+scalar `float` value, or as a tuple of `(<read timeout>, <connect timeout>)`.
+
+
 ## Proxy
 
 The underlying `requests` library honors the `HTTP_PROXY` and `HTTPS_PROXY`
 environment variables. Setting them before invoking an application using
 `grafana-client` has been confirmed to work. For example:
 ```
 export HTTP_PROXY=10.10.1.10:3128
@@ -294,66 +303,55 @@
 - [grafana-import-tool](https://github.com/peekjef72/grafana-import-tool)
 - [grafana-ldap-sync-script](https://github.com/NovatecConsulting/grafana-ldap-sync-script)
 - [grafana-snapshots-tool](https://github.com/peekjef72/grafana-snapshots-tool)
 - [grafana-wtf](https://github.com/panodata/grafana-wtf)
 - [nixops-grafana](https://github.com/tewfik-ghariani/nixops-grafana)
 
 
-## History
+## Project information
+
+### History
 
 The library was originally conceived by [Andrew Prokhorenkov] and contributors
 as [grafana_api]. Thank you very much for your efforts!
 
 At [future maintenance of `grafana_api`], we discussed the need for a fork
 because the repository stopped receiving updates since more than a year.
 While forking it, we renamed the package to `grafana-client` and slightly
 trimmed the module namespace.
 
 
-## Acknowledgements
+### Acknowledgements
 
 Thanks to the original authors and all [contributors] who helped to co-create
 and conceive this software in one way or another. You know who you are.
 
 
-## Contributing
+### Contributing
 
 Any kind of contribution and feedback are very much welcome! Just create an
 issue or submit a patch if you think we should include a new feature, or to 
 report or fix a bug.
 
 The issue tracker URL is: https://github.com/panodata/grafana-client/issues
 
 
-## Development
-
-In order to create a development sandbox, you may want to follow this list of
-commands. When you see the software tests succeed, you should be ready to start
-hacking.
-
-```shell
-git clone https://github.com/panodata/grafana-client
-cd grafana-client
-python3 -m venv .venv
-source .venv/bin/activate
-pip install --editable=.[test,develop]
+### Development
 
-# Run all tests.
-poe test
+In order to set up a development environment for `grafana-client`, please
+follow the [development documentation].
 
-# Run specific tests.
-python -m unittest -k preference -vvv
-```
 
-## License
+### License
 
 `grafana-client` is licensed under the terms of the MIT License, see [LICENSE] file.
 
 
 [Andrew Prokhorenkov]: https://github.com/m0nhawk/grafana_api
 [contributors]: https://github.com/panodata/grafana-client/graphs/contributors
+[development documentation]: https://github.com/panodata/grafana-client/blob/main/docs/development.md
 [examples folder]: https://github.com/panodata/grafana-client/tree/main/examples
 [future maintenance of `grafana_api`]: https://github.com/m0nhawk/grafana_api/issues/88
 [grafana_api]: https://github.com/m0nhawk/grafana_api
 [Grafana Admin API]: https://grafana.com/docs/grafana/latest/http_api/admin/
 [Grafana HTTP API reference]: https://grafana.com/docs/grafana/latest/http_api/
 [LICENSE]: https://github.com/panodata/grafana-client/blob/main/LICENSE
```

### Comparing `grafana-client-3.5.0/README.md` & `grafana-client-3.6.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -132,14 +132,23 @@
 grafana = GrafanaApi.from_env()
 ```
 
 Please note that, on top of the specific examples above, the object obtained by
 `credential` can be an arbitrary `requests.auth.AuthBase` instance.
 
 
+## Timeout settings
+
+The default timeout value is five seconds, used for both connect and read timeout.
+
+The constructors of `GrafanaApi` and `GrafanaClient`, as well as the factory methods
+`from_url` and `from_env` accept the `timeout` argument, which can be obtained as a
+scalar `float` value, or as a tuple of `(<read timeout>, <connect timeout>)`.
+
+
 ## Proxy
 
 The underlying `requests` library honors the `HTTP_PROXY` and `HTTPS_PROXY`
 environment variables. Setting them before invoking an application using
 `grafana-client` has been confirmed to work. For example:
 ```
 export HTTP_PROXY=10.10.1.10:3128
@@ -234,66 +243,55 @@
 - [grafana-import-tool](https://github.com/peekjef72/grafana-import-tool)
 - [grafana-ldap-sync-script](https://github.com/NovatecConsulting/grafana-ldap-sync-script)
 - [grafana-snapshots-tool](https://github.com/peekjef72/grafana-snapshots-tool)
 - [grafana-wtf](https://github.com/panodata/grafana-wtf)
 - [nixops-grafana](https://github.com/tewfik-ghariani/nixops-grafana)
 
 
-## History
+## Project information
+
+### History
 
 The library was originally conceived by [Andrew Prokhorenkov] and contributors
 as [grafana_api]. Thank you very much for your efforts!
 
 At [future maintenance of `grafana_api`], we discussed the need for a fork
 because the repository stopped receiving updates since more than a year.
 While forking it, we renamed the package to `grafana-client` and slightly
 trimmed the module namespace.
 
 
-## Acknowledgements
+### Acknowledgements
 
 Thanks to the original authors and all [contributors] who helped to co-create
 and conceive this software in one way or another. You know who you are.
 
 
-## Contributing
+### Contributing
 
 Any kind of contribution and feedback are very much welcome! Just create an
 issue or submit a patch if you think we should include a new feature, or to 
 report or fix a bug.
 
 The issue tracker URL is: https://github.com/panodata/grafana-client/issues
 
 
-## Development
-
-In order to create a development sandbox, you may want to follow this list of
-commands. When you see the software tests succeed, you should be ready to start
-hacking.
-
-```shell
-git clone https://github.com/panodata/grafana-client
-cd grafana-client
-python3 -m venv .venv
-source .venv/bin/activate
-pip install --editable=.[test,develop]
+### Development
 
-# Run all tests.
-poe test
+In order to set up a development environment for `grafana-client`, please
+follow the [development documentation].
 
-# Run specific tests.
-python -m unittest -k preference -vvv
-```
 
-## License
+### License
 
 `grafana-client` is licensed under the terms of the MIT License, see [LICENSE] file.
 
 
 [Andrew Prokhorenkov]: https://github.com/m0nhawk/grafana_api
 [contributors]: https://github.com/panodata/grafana-client/graphs/contributors
+[development documentation]: https://github.com/panodata/grafana-client/blob/main/docs/development.md
 [examples folder]: https://github.com/panodata/grafana-client/tree/main/examples
 [future maintenance of `grafana_api`]: https://github.com/m0nhawk/grafana_api/issues/88
 [grafana_api]: https://github.com/m0nhawk/grafana_api
 [Grafana Admin API]: https://grafana.com/docs/grafana/latest/http_api/admin/
 [Grafana HTTP API reference]: https://grafana.com/docs/grafana/latest/http_api/
 [LICENSE]: https://github.com/panodata/grafana-client/blob/main/LICENSE
```

### Comparing `grafana-client-3.5.0/conda/meta.yaml` & `grafana-client-3.6.0/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/docs/backlog.md` & `grafana-client-3.6.0/docs/backlog.md`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/docs/index.html` & `grafana-client-3.6.0/docs/index.html`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/examples/datasource-health-check.py` & `grafana-client-3.6.0/examples/datasource-health-check.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
         sys.exit(2)
 
     logger.info(f"Probing {len(datasources)} data sources")
 
     success = True
     statistics = {"ok": 0, "error": 0, "fatal": 0, "unknown": 0}
     for datasource in datasources:
-
         logger.info(f"Discovered datasource with uid={datasource['uid']} and type={datasource['type']}")
 
         # Invoke the health check.
         try:
             health_info = grafana.datasource.health_inquiry(datasource_uid=datasource["uid"])
             if health_info.success:
                 statistics["ok"] += 1
@@ -68,15 +67,14 @@
     logger.info(f"Statistics: {statistics}")
 
     if not success:
         sys.exit(1)
 
 
 if __name__ == "__main__":
-
     setup_logging(level=logging.DEBUG)
 
     # Connect to Grafana instance and run health check.
     grafana_client = GrafanaApi.from_env()
 
     try:
         grafana_client.connect()
```

### Comparing `grafana-client-3.5.0/examples/datasource-health-check.rst` & `grafana-client-3.6.0/examples/datasource-health-check.rst`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/examples/datasource-health-probe.py` & `grafana-client-3.6.0/examples/datasource-health-probe.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 
     # Create data source.
     datasource = datasource.asdict()
     try:
         logger.info(f"Creating data source '{datasource_name}'")
         datasource = grafana.datasource.create_datasource(datasource)["datasource"]
     except GrafanaClientError as ex:
-
         # When data source already exists, update data source.
         if ex.status_code == 409:
             logger.info(f"Data source already exists: {ex.response}. Updating.")
             datasource_existing = grafana.datasource.get_datasource_by_name(datasource_name=datasource_name)
             datasource = grafana.datasource.update_datasource(datasource_existing["id"], datasource)["datasource"]
         else:
             logger.error(
@@ -79,15 +78,14 @@
         name="probe-prometheus", type="prometheus", url="http://host.docker.internal:9090", access="server"
     )
     health_info = health_probe(grafana, datasource)
     return health_info
 
 
 def run(grafana: GrafanaApi, grafana_version: LooseVersion = None):
-
     # When called without options, invoke the Prometheus demo.
     if len(sys.argv) == 1:
         if grafana_version < VERSION_8:
             raise NotImplementedError(
                 f"Data source health check subsystem on Grafana version {grafana_version} not supported for Prometheus"
             )
         health_info = prometheus_demo(grafana)
@@ -119,15 +117,14 @@
     # Display the outcome and terminate program based on success state.
     print(json.dumps(health_info, indent=2))
     if not health_info["success"]:
         sys.exit(1)
 
 
 if __name__ == "__main__":
-
     setup_logging(level=logging.DEBUG)
 
     # Connect to Grafana instance and run health probe.
     grafana_client = GrafanaApi.from_env()
 
     try:
         grafana_client.connect()
```

### Comparing `grafana-client-3.5.0/examples/datasource-health-probe.rst` & `grafana-client-3.6.0/examples/datasource-health-probe.rst`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/examples/datasource-smartquery.py` & `grafana-client-3.6.0/examples/datasource-smartquery.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,14 @@
     )
 
     # Display the outcome in JSON format.
     print(json.dumps(response, indent=2))
 
 
 if __name__ == "__main__":
-
     setup_logging(level=logging.DEBUG)
 
     # Connect to Grafana instance and run health check.
     grafana_client = GrafanaApi.from_url("https://play.grafana.org/")
 
     try:
         grafana_client.connect()
```

### Comparing `grafana-client-3.5.0/examples/folders-dashboard.py` & `grafana-client-3.6.0/examples/folders-dashboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 import json
 import sys
 
 from grafana_client import GrafanaApi
 
 
 def main():
-
     # Connect to public Grafana instance of Grafana Labs fame.
     grafana = GrafanaApi(host="play.grafana.org")
 
     print("## All folders on play.grafana.org", file=sys.stderr)
     folders = grafana.folder.get_all_folders()
     print(json.dumps(folders, indent=2))
```

### Comparing `grafana-client-3.5.0/examples/grafanalib-upload-dashboard.py` & `grafana-client-3.6.0/examples/grafanalib-upload-dashboard.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/examples/team.py` & `grafana-client-3.6.0/examples/team.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 import json
 
 from grafana_client import GrafanaApi
 from grafana_client.client import GrafanaClientError
 
 
 def run_conversation(grafana: GrafanaApi):
-
     print("Grafana address")
     print(grafana.client.url)
 
     print("Health check")
     print(grafana.health.check())
 
     print("Create team")
@@ -54,15 +53,14 @@
 
 
 def jd(data):
     return json.dumps(data, indent=2)
 
 
 if __name__ == "__main__":
-
     # Connect to custom Grafana instance.
     grafana = GrafanaApi(
         auth=("admin", "admin"),
         host="localhost:3000",
     )
 
     # Connect to Grafana instance of Grafana Labs fame.
```

### Comparing `grafana-client-3.5.0/grafana_client/__init__.py` & `grafana-client-3.6.0/grafana_client/__init__.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/grafana_client/api.py` & `grafana-client-3.6.0/grafana_client/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Tuple, Union
 from urllib.parse import parse_qs, urlparse
 
 import requests
 import requests.auth
 from urllib3.exceptions import InsecureRequestWarning
 
-from .client import GrafanaClient
+from .client import DEFAULT_TIMEOUT, GrafanaClient
 from .elements import (
     Admin,
     Alerting,
     AlertingProvisioning,
     Annotations,
     Dashboard,
     DashboardVersions,
@@ -40,15 +40,15 @@
         self,
         auth=None,
         host="localhost",
         port=None,
         url_path_prefix="",
         protocol="http",
         verify=True,
-        timeout=5.0,
+        timeout=DEFAULT_TIMEOUT,
         user_agent: str = None,
     ):
         self.client = GrafanaClient(
             auth,
             host=host,
             port=port,
             url_path_prefix=url_path_prefix,
@@ -91,15 +91,20 @@
     def version(self):
         grafana_info = self.health.check()
         version = grafana_info["version"]
         logger.info(f"Inquired Grafana version: {version}")
         return version
 
     @classmethod
-    def from_url(cls, url: str = None, credential: Union[str, Tuple[str, str], requests.auth.AuthBase] = None):
+    def from_url(
+        cls,
+        url: str = None,
+        credential: Union[str, Tuple[str, str], requests.auth.AuthBase] = None,
+        timeout: Union[float, Tuple[float, float]] = DEFAULT_TIMEOUT,
+    ):
         """
         Factory method to create a `GrafanaApi` instance from a URL.
 
         Accepts an optional credential, which is either an authentication
         token, or a tuple of (username, password).
         """
 
@@ -125,18 +130,31 @@
         grafana = cls(
             credential,
             protocol=url.scheme,
             host=url.hostname,
             port=url.port,
             url_path_prefix=url.path.lstrip("/"),
             verify=verify,
+            timeout=timeout,
         )
         grafana.url = original_url
 
         return grafana
 
     @classmethod
-    def from_env(cls):
+    def from_env(cls, timeout: Union[float, Tuple[float, float]] = None):
         """
         Factory method to create a `GrafanaApi` instance from environment variables.
         """
-        return cls.from_url(url=os.environ.get("GRAFANA_URL"), credential=os.environ.get("GRAFANA_TOKEN"))
+        if timeout is None:
+            if "GRAFANA_TIMEOUT" in os.environ:
+                try:
+                    timeout = float(os.environ["GRAFANA_TIMEOUT"])
+                except Exception as ex:
+                    raise ValueError(
+                        f"Unable to parse invalid `float` value from " f"`GRAFANA_TIMEOUT` environment variable: {ex}"
+                    )
+        if timeout is None:
+            timeout = DEFAULT_TIMEOUT
+        return cls.from_url(
+            url=os.environ.get("GRAFANA_URL"), credential=os.environ.get("GRAFANA_TOKEN"), timeout=timeout
+        )
```

### Comparing `grafana-client-3.5.0/grafana_client/client.py` & `grafana-client-3.6.0/grafana_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import requests
 import requests.auth
 
+DEFAULT_TIMEOUT: float = 5.0
+
 
 class GrafanaException(Exception):
     def __init__(self, status_code, response, message):
         self.status_code = status_code
         self.response = response
         self.message = message
         # Backwards compatible with implementations that rely on just the message.
@@ -69,15 +71,15 @@
         self,
         auth,
         host="localhost",
         port=None,
         url_path_prefix="",
         protocol="http",
         verify=True,
-        timeout=5.0,
+        timeout=DEFAULT_TIMEOUT,
         user_agent: str = None,
     ):
         self.auth = auth
         self.verify = verify
         self.timeout = timeout
         self.url_host = host
         self.url_port = port
```

### Comparing `grafana-client-3.5.0/grafana_client/elements/__init__.py` & `grafana-client-3.6.0/grafana_client/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/grafana_client/elements/admin.py` & `grafana-client-3.6.0/grafana_client/elements/admin.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/grafana_client/elements/alerting.py` & `grafana-client-3.6.0/grafana_client/elements/alerting.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/grafana_client/elements/alertingprovisioning.py` & `grafana-client-3.6.0/grafana_client/elements/alertingprovisioning.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,23 @@
 
 
 class AlertingProvisioning(Base):
     def __init__(self, client):
         super(AlertingProvisioning, self).__init__(client)
         self.client = client
 
+    def get_alertrules_all(self):
+        """
+        Gets all alert rules
+        @return:
+        """
+        get_alertrules_all_path = "/v1/provisioning/alert-rules"
+        r = self.client.GET(get_alertrules_all_path)
+        return r
+
     def get_alertrule(self, alertrule_uid):
         """
 
         :param alertrule_uid:
         :return:
         """
         get_alertrule_path = "/v1/provisioning/alert-rules/%s" % alertrule_uid
```

### Comparing `grafana-client-3.5.0/grafana_client/elements/annotations.py` & `grafana-client-3.6.0/grafana_client/elements/annotations.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,28 +8,29 @@
 
     def get_annotation(
         self,
         time_from=None,
         time_to=None,
         alert_id=None,
         dashboard_id=None,
+        dashboard_uid=None,
         panel_id=None,
         user_id=None,
         ann_type=None,
         tags=None,
         limit=None,
     ):
-
         """
         https://grafana.com/docs/grafana/latest/http_api/annotations/#find-annotations
 
         :param time_from:
         :param time_to:
         :param alert_id:
         :param dashboard_id:
+        :param dashboard_uid:
         :param panel_id:
         :param user_id:
         :param ann_type: Annotation type. On of alert|annotation
         :param tags:
         :param limit:
         :return:
         """
@@ -44,14 +45,17 @@
 
         if alert_id:
             params.append("alertId=%s" % alert_id)
 
         if dashboard_id:
             params.append("dashboardId=%s" % dashboard_id)
 
+        if dashboard_uid:
+            params.append("dashboardUID=%s" % dashboard_uid)
+
         if panel_id:
             params.append("panelId=%s" % panel_id)
 
         if user_id:
             params.append("userId=%s" % user_id)
 
         if ann_type:
@@ -76,15 +80,14 @@
         dashboard_id=None,
         panel_id=None,
         time_from=None,
         time_to=None,
         tags=[],
         text=None,
     ):
-
         """
         https://grafana.com/docs/grafana/latest/http_api/annotations/#create-annotation
 
         :param dashboard_id:
         :param panel_id
         :param time_from:
         :param time_to:
@@ -179,15 +182,14 @@
         payload = {"time": time_from, "timeEnd": time_to, "tags": tags, "text": text}
 
         r = self.client.PATCH(annotations_path, json=payload)
 
         return r
 
     def delete_annotations_by_id(self, annotations_id=None):
-
         """
         https://grafana.com/docs/grafana/latest/http_api/annotations/#delete-annotation-by-id
 
         :param annotations_id:
         :return:
         """
         annotations_path = "/annotations/{}".format(annotations_id)
```

### Comparing `grafana-client-3.5.0/grafana_client/elements/dashboard.py` & `grafana-client-3.6.0/grafana_client/elements/dashboard.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/grafana_client/elements/dashboard_versions.py` & `grafana-client-3.6.0/grafana_client/elements/dashboard_versions.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/grafana_client/elements/datasource.py` & `grafana-client-3.6.0/grafana_client/elements/datasource.py`

 * *Files 0% similar despite different names*

```diff
@@ -630,15 +630,14 @@
 
     @staticmethod
     def parse_health_response_results(response: Dict) -> Tuple[bool, str]:
         success = False
         results = response["results"]
         if isinstance(results, dict):
             try:
-
                 # The `refId` currently used is always `test`, see `knowledge.py`.
                 # TODO: Change to `gcX`.
                 result = results["test"]
 
                 # Handle response in new DataFrame format.
                 # Data frames are available in Grafana 7.0+, and replaced the Time series and Table structures
                 # with a more generic data structure that can support a wider range of data types.
```

### Comparing `grafana-client-3.5.0/grafana_client/elements/folder.py` & `grafana-client-3.6.0/grafana_client/elements/folder.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/grafana_client/elements/notifications.py` & `grafana-client-3.6.0/grafana_client/elements/notifications.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/grafana_client/elements/organization.py` & `grafana-client-3.6.0/grafana_client/elements/organization.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/grafana_client/elements/rbac.py` & `grafana-client-3.6.0/grafana_client/elements/rbac.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/grafana_client/elements/search.py` & `grafana-client-3.6.0/grafana_client/elements/search.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/grafana_client/elements/snapshots.py` & `grafana-client-3.6.0/grafana_client/elements/snapshots.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/grafana_client/elements/team.py` & `grafana-client-3.6.0/grafana_client/elements/team.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/grafana_client/elements/user.py` & `grafana-client-3.6.0/grafana_client/elements/user.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/grafana_client/knowledge.py` & `grafana-client-3.6.0/grafana_client/knowledge.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/grafana_client/model.py` & `grafana-client-3.6.0/grafana_client/model.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/grafana_client/util.py` & `grafana-client-3.6.0/grafana_client/util.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/grafana_client.egg-info/PKG-INFO` & `grafana-client-3.6.0/grafana_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grafana-client
-Version: 3.5.0
+Version: 3.6.0
 Summary: A client library for accessing the Grafana HTTP API, written in Python
 Home-page: https://github.com/panodata/grafana-client
 Author: Andrew Prokhorenkov
 Author-email: andrew.prokhorenkov@gmail.com
 Maintainer: Andreas Motl
 Maintainer-email: andreas.motl@panodata.org
 License: MIT
@@ -192,14 +192,23 @@
 grafana = GrafanaApi.from_env()
 ```
 
 Please note that, on top of the specific examples above, the object obtained by
 `credential` can be an arbitrary `requests.auth.AuthBase` instance.
 
 
+## Timeout settings
+
+The default timeout value is five seconds, used for both connect and read timeout.
+
+The constructors of `GrafanaApi` and `GrafanaClient`, as well as the factory methods
+`from_url` and `from_env` accept the `timeout` argument, which can be obtained as a
+scalar `float` value, or as a tuple of `(<read timeout>, <connect timeout>)`.
+
+
 ## Proxy
 
 The underlying `requests` library honors the `HTTP_PROXY` and `HTTPS_PROXY`
 environment variables. Setting them before invoking an application using
 `grafana-client` has been confirmed to work. For example:
 ```
 export HTTP_PROXY=10.10.1.10:3128
@@ -294,66 +303,55 @@
 - [grafana-import-tool](https://github.com/peekjef72/grafana-import-tool)
 - [grafana-ldap-sync-script](https://github.com/NovatecConsulting/grafana-ldap-sync-script)
 - [grafana-snapshots-tool](https://github.com/peekjef72/grafana-snapshots-tool)
 - [grafana-wtf](https://github.com/panodata/grafana-wtf)
 - [nixops-grafana](https://github.com/tewfik-ghariani/nixops-grafana)
 
 
-## History
+## Project information
+
+### History
 
 The library was originally conceived by [Andrew Prokhorenkov] and contributors
 as [grafana_api]. Thank you very much for your efforts!
 
 At [future maintenance of `grafana_api`], we discussed the need for a fork
 because the repository stopped receiving updates since more than a year.
 While forking it, we renamed the package to `grafana-client` and slightly
 trimmed the module namespace.
 
 
-## Acknowledgements
+### Acknowledgements
 
 Thanks to the original authors and all [contributors] who helped to co-create
 and conceive this software in one way or another. You know who you are.
 
 
-## Contributing
+### Contributing
 
 Any kind of contribution and feedback are very much welcome! Just create an
 issue or submit a patch if you think we should include a new feature, or to 
 report or fix a bug.
 
 The issue tracker URL is: https://github.com/panodata/grafana-client/issues
 
 
-## Development
-
-In order to create a development sandbox, you may want to follow this list of
-commands. When you see the software tests succeed, you should be ready to start
-hacking.
-
-```shell
-git clone https://github.com/panodata/grafana-client
-cd grafana-client
-python3 -m venv .venv
-source .venv/bin/activate
-pip install --editable=.[test,develop]
+### Development
 
-# Run all tests.
-poe test
+In order to set up a development environment for `grafana-client`, please
+follow the [development documentation].
 
-# Run specific tests.
-python -m unittest -k preference -vvv
-```
 
-## License
+### License
 
 `grafana-client` is licensed under the terms of the MIT License, see [LICENSE] file.
 
 
 [Andrew Prokhorenkov]: https://github.com/m0nhawk/grafana_api
 [contributors]: https://github.com/panodata/grafana-client/graphs/contributors
+[development documentation]: https://github.com/panodata/grafana-client/blob/main/docs/development.md
 [examples folder]: https://github.com/panodata/grafana-client/tree/main/examples
 [future maintenance of `grafana_api`]: https://github.com/m0nhawk/grafana_api/issues/88
 [grafana_api]: https://github.com/m0nhawk/grafana_api
 [Grafana Admin API]: https://grafana.com/docs/grafana/latest/http_api/admin/
 [Grafana HTTP API reference]: https://grafana.com/docs/grafana/latest/http_api/
 [LICENSE]: https://github.com/panodata/grafana-client/blob/main/LICENSE
```

### Comparing `grafana-client-3.5.0/grafana_client.egg-info/SOURCES.txt` & `grafana-client-3.6.0/grafana_client.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 pyproject.toml
 setup.cfg
 setup.py
 conda/meta.yaml
 conda/setup.py
 docs/backlog.md
 docs/datasource-state.md
+docs/development.md
 docs/index.html
 examples/datasource-health-check.py
 examples/datasource-health-check.rst
 examples/datasource-health-probe.py
 examples/datasource-health-probe.rst
 examples/datasource-smartquery.py
 examples/folders-dashboard.py
+examples/grafana-tokenauth-healthcheck.py
 examples/grafanalib-upload-dashboard.py
 examples/team.py
 grafana_client/__init__.py
 grafana_client/api.py
 grafana_client/client.py
 grafana_client/knowledge.py
 grafana_client/model.py
```

### Comparing `grafana-client-3.5.0/pyproject.toml` & `grafana-client-3.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 # ===================
 
 [tool.poe.tasks]
 format = [
   {cmd="black ."},
   {cmd="isort ."},
 ]
-check-style = [
+lint = [
   {cmd="ruff ."},
   {cmd="black --check ."},
   {cmd="isort --check ."},
 ]
 test = [
   {cmd="python -m unittest -vvv"},
 ]
```

### Comparing `grafana-client-3.5.0/setup.cfg` & `grafana-client-3.6.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -72,24 +72,24 @@
 	dataclasses;python_version<='3.6'
 	importlib-metadata;python_version<='3.7'
 
 [options.extras_require]
 test = 
 	parameterized>=0.8,<1
 	codecov<3
-	coverage[toml]<7
+	coverage[toml]<8
 	unittest-xml-reporting<4
 	requests-mock<2
 develop = 
 	isort<6
-	black<23
+	black<24
 	build<1
 	poethepoet<1
 	pip-review<2  # Use `pip-review --local --interactive` to upgrade outdated packages.
-	ruff==0.0.158;python_version>='3.7'
+	ruff==0.0.280;python_version>='3.7'
 
 [options.packages.find]
 where = .
 exclude = test
 
 [bdist_wheel]
 universal = true
```

### Comparing `grafana-client-3.5.0/test/elements/test_admin.py` & `grafana-client-3.6.0/test/elements/test_admin.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/test/elements/test_alerting.py` & `grafana-client-3.6.0/test/elements/test_alerting.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/test/elements/test_alertingprovisioning.py` & `grafana-client-3.6.0/test/elements/test_alertingprovisioning.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,20 @@
 
 
 class AlertingProvisioningTestCase(unittest.TestCase):
     def setUp(self):
         self.grafana = GrafanaApi(("admin", "admin"), host="localhost", url_path_prefix="", protocol="http")
 
     @requests_mock.Mocker()
+    def test_get_alertrules_all(self, m):
+        m.get("http://localhost/api/v1/provisioning/alert-rules", json=[ALERTRULE])
+        response = self.grafana.alertingprovisioning.get_alertrules_all()
+        self.assertEqual(response[0]["uid"], "bUUGqLiVk")
+
+    @requests_mock.Mocker()
     def test_get_alertrule(self, m):
         m.get("http://localhost/api/v1/provisioning/alert-rules/bUUGqLiVk", json=ALERTRULE)
         response = self.grafana.alertingprovisioning.get_alertrule("bUUGqLiVk")
         self.assertEqual(response["uid"], "bUUGqLiVk")
 
     @requests_mock.Mocker()
     def test_delete_alertrule(self, m):
```

### Comparing `grafana-client-3.5.0/test/elements/test_annotations.py` & `grafana-client-3.6.0/test/elements/test_annotations.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,21 +15,22 @@
     def setUp(self):
         self.grafana = GrafanaApi(("admin", "admin"), host="localhost", url_path_prefix="", protocol="http")
 
     @requests_mock.Mocker()
     def test_annotations(self, m):
         m.get(
             "http://localhost/api/annotations?from=1563183710618&to=1563185212275"
-            "&alertId=11&dashboardId=111&panelId=22&userId=42&type=alert&tags=tags-test&limit=1",
+            "&alertId=11&dashboardId=111&dashboardUID=v1Mm5FPVz&panelId=22&userId=42&type=alert&tags=tags-test&limit=1",
             json=[
                 {
                     "id": 80,
                     "alertId": 11,
                     "alertName": "",
                     "dashboardId": 111,
+                    "dashboardUID": "v1Mm5FPVz",
                     "panelId": 22,
                     "userId": 42,
                     "type": "alert",
                     "newState": "",
                     "prevState": "",
                     "created": 1563280160455,
                     "updated": 1563280160455,
@@ -44,22 +45,24 @@
             ],
         )
         annotations = self.grafana.annotations.get_annotation(
             time_from=1563183710618,
             time_to=1563185212275,
             alert_id=11,
             dashboard_id=111,
+            dashboard_uid="v1Mm5FPVz",
             panel_id=22,
             user_id=42,
             ann_type="alert",
             tags=["tags-test"],
             limit=1,
         )
         self.assertEqual(annotations[0]["text"], "Annotation Description")
         self.assertEqual(annotations[0]["alertId"], 11)
+        self.assertEqual(annotations[0]["dashboardUID"], "v1Mm5FPVz")
         self.assertEqual(annotations[0]["dashboardId"], 111)
         self.assertEqual(annotations[0]["panelId"], 22)
         self.assertEqual(annotations[0]["userId"], 42)
         self.assertEqual(annotations[0]["type"], "alert")
         self.assertEqual(annotations[0]["tags"][0], "tags-test")
 
         self.assertEqual(len(annotations), 1)
```

### Comparing `grafana-client-3.5.0/test/elements/test_dashboard.py` & `grafana-client-3.6.0/test/elements/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/test/elements/test_dashboard_versions.py` & `grafana-client-3.6.0/test/elements/test_dashboard_versions.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/test/elements/test_datasource_base.py` & `grafana-client-3.6.0/test/elements/test_datasource_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,24 +322,22 @@
 
     def test_query_empty_expression_failure(self):
         datasource = PROMETHEUS_DATASOURCE.copy()
         self.assertRaises(ValueError, lambda: self.grafana.datasource.smartquery(datasource, expression=None))
 
     @patch("grafana_client.client.GrafanaClient.__getattr__")
     def test_query_client_error_failure(self, mock_get):
-
         mock_get.return_value = Mock()
         mock_get.return_value.side_effect = GrafanaClientError(status_code=400, response={}, message="Something failed")
 
         datasource = PROMETHEUS_DATASOURCE.copy()
         self.assertRaises(GrafanaClientError, lambda: self.grafana.datasource.smartquery(datasource, expression="1+1"))
 
     @patch("grafana_client.client.GrafanaClient.__getattr__")
     def test_query_server_error_failure(self, mock_get):
-
         mock_get.return_value = Mock()
         mock_get.return_value.side_effect = GrafanaServerError(
             status_code=500, response={}, message="Something serious failed"
         )
 
         datasource = PROMETHEUS_DATASOURCE.copy()
         self.assertRaises(GrafanaServerError, lambda: self.grafana.datasource.smartquery(datasource, expression="1+1"))
```

### Comparing `grafana-client-3.5.0/test/elements/test_datasource_fixtures.py` & `grafana-client-3.6.0/test/elements/test_datasource_fixtures.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/test/elements/test_datasource_health.py` & `grafana-client-3.6.0/test/elements/test_datasource_health.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/test/elements/test_folder.py` & `grafana-client-3.6.0/test/elements/test_folder.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/test/elements/test_health.py` & `grafana-client-3.6.0/test/elements/test_health.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/test/elements/test_notifications.py` & `grafana-client-3.6.0/test/elements/test_notifications.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/test/elements/test_organization.py` & `grafana-client-3.6.0/test/elements/test_organization.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/test/elements/test_rbac.py` & `grafana-client-3.6.0/test/elements/test_rbac.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/test/elements/test_search.py` & `grafana-client-3.6.0/test/elements/test_search.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/test/elements/test_snapshot.py` & `grafana-client-3.6.0/test/elements/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/test/elements/test_team.py` & `grafana-client-3.6.0/test/elements/test_team.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/test/elements/test_user.py` & `grafana-client-3.6.0/test/elements/test_user.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/test/test_grafana_api.py` & `grafana-client-3.6.0/test/test_grafana_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -62,14 +62,22 @@
         self.assertEqual(grafana.client.url_host, "daq.example.org")
         self.assertEqual(grafana.client.url_port, None)
         self.assertEqual(grafana.client.url_path_prefix, "grafana/")
         self.assertEqual(grafana.client.url_protocol, "https")
         self.assertEqual(grafana.client.verify, False)
         self.assertEqual(grafana.client.timeout, 5.0)
 
+    def test_from_url_with_timeout_value(self):
+        grafana = GrafanaApi.from_url(timeout=42.42)
+        self.assertEqual(grafana.client.timeout, 42.42)
+
+    def test_from_url_with_timeout_tuple(self):
+        grafana = GrafanaApi.from_url(timeout=(3.05, 27))
+        self.assertEqual(grafana.client.timeout, (3.05, 27))
+
     def test_from_env_default(self):
         grafana = GrafanaApi.from_env()
         self.assertIsInstance(grafana.client.auth, requests.auth.HTTPBasicAuth)
         self.assertEqual(grafana.client.auth.username, "admin")
         self.assertEqual(grafana.client.auth.password, "admin")
         self.assertEqual(grafana.client.url_host, "localhost")
         self.assertEqual(grafana.client.url_port, 3000)
@@ -110,7 +118,26 @@
         self.assertEqual(grafana.client.auth.password, "bar")
         self.assertEqual(grafana.client.url_host, "daq.example.org")
         self.assertEqual(grafana.client.url_port, None)
         self.assertEqual(grafana.client.url_path_prefix, "grafana/")
         self.assertEqual(grafana.client.url_protocol, "https")
         self.assertEqual(grafana.client.verify, False)
         self.assertEqual(grafana.client.timeout, 5.0)
+
+    @mock.patch.dict(os.environ, {"GRAFANA_TIMEOUT": "84.84"})
+    def test_from_env_with_timeout_from_env_valid(self):
+        grafana = GrafanaApi.from_env()
+        self.assertEqual(grafana.client.timeout, 84.84)
+
+    @mock.patch.dict(os.environ, {"GRAFANA_TIMEOUT": "foobar"})
+    def test_from_env_with_timeout_from_env_invalid(self):
+        with self.assertRaises(ValueError) as ctx:
+            GrafanaApi.from_env()
+        self.assertEqual(
+            str(ctx.exception),
+            "Unable to parse invalid `float` value from `GRAFANA_TIMEOUT` "
+            "environment variable: could not convert string to float: 'foobar'",
+        )
+
+    def test_from_env_with_timeout_tuple(self):
+        grafana = GrafanaApi.from_env(timeout=(3.05, 27))
+        self.assertEqual(grafana.client.timeout, (3.05, 27))
```

### Comparing `grafana-client-3.5.0/test/test_grafana_client.py` & `grafana-client-3.6.0/test/test_grafana_client.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/test/test_knowledge.py` & `grafana-client-3.6.0/test/test_knowledge.py`

 * *Files identical despite different names*

### Comparing `grafana-client-3.5.0/test/test_model.py` & `grafana-client-3.6.0/test/test_model.py`

 * *Files identical despite different names*

