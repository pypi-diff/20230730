# Comparing `tmp/netbox-config-diff-1.0.0.tar.gz` & `tmp/netbox-config-diff-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-config-diff-1.0.0.tar", last modified: Sun Jul 23 13:06:28 2023, max compression
+gzip compressed data, was "netbox-config-diff-1.1.0.tar", last modified: Sun Jul 30 13:50:33 2023, max compression
```

## Comparing `netbox-config-diff-1.0.0.tar` & `netbox-config-diff-1.1.0.tar`

### file list

```diff
@@ -1,68 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:06:28.954193 netbox-config-diff-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16661 2023-07-23 13:06:28.954193 netbox-config-diff-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:06:28.938193 netbox-config-diff-1.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:06:28.938193 netbox-config-diff-1.0.0/docs/media/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:06:28.942193 netbox-config-diff-1.0.0/docs/media/screenshots/
--rw-r--r--   0 runner    (1001) docker     (123)    31744 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/docs/media/screenshots/compliance-diff.png
--rw-r--r--   0 runner    (1001) docker     (123)    48801 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/docs/media/screenshots/compliance-error.png
--rw-r--r--   0 runner    (1001) docker     (123)    23740 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/docs/media/screenshots/compliance-list.png
--rw-r--r--   0 runner    (1001) docker     (123)    17602 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/docs/media/screenshots/compliance-ok.png
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/docs/media/screenshots/navbar.png
--rw-r--r--   0 runner    (1001) docker     (123)    28028 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/docs/media/screenshots/platformsetting.png
--rw-r--r--   0 runner    (1001) docker     (123)    14783 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/docs/media/screenshots/script-list.png
--rw-r--r--   0 runner    (1001) docker     (123)    37552 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/docs/media/screenshots/script.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:06:28.946193 netbox-config-diff-1.0.0/netbox_config_diff/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/netbox_config_diff/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:06:28.946193 netbox-config-diff-1.0.0/netbox_config_diff/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/netbox_config_diff/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/netbox_config_diff/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/netbox_config_diff/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/netbox_config_diff/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/netbox_config_diff/choices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:06:28.946193 netbox-config-diff-1.0.0/netbox_config_diff/compliance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/netbox_config_diff/compliance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/netbox_config_diff/compliance/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/netbox_config_diff/compliance/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/netbox_config_diff/compliance/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/netbox_config_diff/filtersets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/netbox_config_diff/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/netbox_config_diff/graphql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:06:28.950193 netbox-config-diff-1.0.0/netbox_config_diff/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/netbox_config_diff/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/netbox_config_diff/migrations/0002_add_script.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/netbox_config_diff/migrations/0003_configcompliance_actual_config_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/netbox_config_diff/migrations/0004_update_script.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/netbox_config_diff/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/netbox_config_diff/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/netbox_config_diff/navigation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:06:28.950193 netbox-config-diff-1.0.0/netbox_config_diff/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/netbox_config_diff/scripts/config_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/netbox_config_diff/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:06:28.942193 netbox-config-diff-1.0.0/netbox_config_diff/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:06:28.950193 netbox-config-diff-1.0.0/netbox_config_diff/static/netbox_config_diff/
--rw-r--r--   0 runner    (1001) docker     (123)  1000358 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/netbox_config_diff/static/netbox_config_diff/diff2html-ui.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/netbox_config_diff/static/netbox_config_diff/diff2html.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/netbox_config_diff/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:06:28.942193 netbox-config-diff-1.0.0/netbox_config_diff/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:06:28.950193 netbox-config-diff-1.0.0/netbox_config_diff/templates/netbox_config_diff/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:06:28.950193 netbox-config-diff-1.0.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/config.html
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/netbox_config_diff/templates/netbox_config_diff/configcompliance.html
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/netbox_config_diff/templates/netbox_config_diff/platformsetting.html
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/netbox_config_diff/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/netbox_config_diff/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:06:28.946193 netbox-config-diff-1.0.0/netbox_config_diff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16661 2023-07-23 13:06:28.000000 netbox-config-diff-1.0.0/netbox_config_diff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-23 13:06:28.000000 netbox-config-diff-1.0.0/netbox_config_diff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 13:06:28.000000 netbox-config-diff-1.0.0/netbox_config_diff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-23 13:06:28.000000 netbox-config-diff-1.0.0/netbox_config_diff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-23 13:06:28.000000 netbox-config-diff-1.0.0/netbox_config_diff.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 13:06:28.950193 netbox-config-diff-1.0.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-23 13:05:58.000000 netbox-config-diff-1.0.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 13:06:28.954193 netbox-config-diff-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:50:33.703383 netbox-config-diff-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17603 2023-07-30 13:50:33.703383 netbox-config-diff-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:50:33.691383 netbox-config-diff-1.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:50:33.691383 netbox-config-diff-1.1.0/docs/media/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:50:33.695383 netbox-config-diff-1.1.0/docs/media/screenshots/
+-rw-r--r--   0 runner    (1001) docker     (123)    31744 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/docs/media/screenshots/compliance-diff.png
+-rw-r--r--   0 runner    (1001) docker     (123)    48801 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/docs/media/screenshots/compliance-error.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23740 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/docs/media/screenshots/compliance-list.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27108 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/docs/media/screenshots/compliance-missing-extra.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17602 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/docs/media/screenshots/compliance-ok.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/docs/media/screenshots/navbar.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28028 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/docs/media/screenshots/platformsetting.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14783 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/docs/media/screenshots/script-list.png
+-rw-r--r--   0 runner    (1001) docker     (123)    37552 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/docs/media/screenshots/script.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:50:33.699383 netbox-config-diff-1.1.0/netbox_config_diff/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/netbox_config_diff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:50:33.699383 netbox-config-diff-1.1.0/netbox_config_diff/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/netbox_config_diff/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/netbox_config_diff/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/netbox_config_diff/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/netbox_config_diff/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/netbox_config_diff/choices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:50:33.699383 netbox-config-diff-1.1.0/netbox_config_diff/compliance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/netbox_config_diff/compliance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/netbox_config_diff/compliance/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/netbox_config_diff/compliance/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/netbox_config_diff/compliance/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/netbox_config_diff/filtersets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/netbox_config_diff/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/netbox_config_diff/graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:50:33.699383 netbox-config-diff-1.1.0/netbox_config_diff/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/netbox_config_diff/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/netbox_config_diff/migrations/0002_add_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/netbox_config_diff/migrations/0003_configcompliance_actual_config_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/netbox_config_diff/migrations/0004_update_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/netbox_config_diff/migrations/0005_configcompliance_extra_missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/netbox_config_diff/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/netbox_config_diff/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/netbox_config_diff/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:50:33.699383 netbox-config-diff-1.1.0/netbox_config_diff/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/netbox_config_diff/scripts/config_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/netbox_config_diff/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:50:33.695383 netbox-config-diff-1.1.0/netbox_config_diff/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:50:33.699383 netbox-config-diff-1.1.0/netbox_config_diff/static/netbox_config_diff/
+-rw-r--r--   0 runner    (1001) docker     (123)  1000358 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/netbox_config_diff/static/netbox_config_diff/diff2html-ui.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/netbox_config_diff/static/netbox_config_diff/diff2html.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/netbox_config_diff/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:50:33.695383 netbox-config-diff-1.1.0/netbox_config_diff/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:50:33.703383 netbox-config-diff-1.1.0/netbox_config_diff/templates/netbox_config_diff/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:50:33.703383 netbox-config-diff-1.1.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/config.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/missing_extra.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/netbox_config_diff/templates/netbox_config_diff/configcompliance.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/netbox_config_diff/templates/netbox_config_diff/platformsetting.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/netbox_config_diff/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/netbox_config_diff/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:50:33.699383 netbox-config-diff-1.1.0/netbox_config_diff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17603 2023-07-30 13:50:33.000000 netbox-config-diff-1.1.0/netbox_config_diff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-30 13:50:33.000000 netbox-config-diff-1.1.0/netbox_config_diff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 13:50:33.000000 netbox-config-diff-1.1.0/netbox_config_diff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-30 13:50:33.000000 netbox-config-diff-1.1.0/netbox_config_diff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-30 13:50:33.000000 netbox-config-diff-1.1.0/netbox_config_diff.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:50:33.703383 netbox-config-diff-1.1.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-30 13:50:17.000000 netbox-config-diff-1.1.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 13:50:33.703383 netbox-config-diff-1.1.0/setup.cfg
```

### Comparing `netbox-config-diff-1.0.0/LICENSE` & `netbox-config-diff-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-1.0.0/PKG-INFO` & `netbox-config-diff-1.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-config-diff
-Version: 1.0.0
+Version: 1.1.0
 Summary: Find diff between the intended device configuration and actual.
 Author: Artem Kotik
 Author-email: miaow2@yandex.ru
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -214,14 +214,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
+[![NetBox version](https://img.shields.io/badge/NetBox-3.5-blue.svg)](https://github.com/netbox-community/netbox)
+[![Supported Versions](https://img.shields.io/pypi/pyversions/netbox-config-diff.svg)](https://pypi.org/project/netbox-config-diff/)
+[![PyPI version](https://badge.fury.io/py/netbox-config-diff.svg)](https://badge.fury.io/py/netbox-config-diff)
+[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+[![CI](https://github.com/miaow2/netbox-config-diff/actions/workflows/commit.yaml/badge.svg?branch=develop)](https://github.com/miaow2/netbox-config-diff/actions)
+
 # NetBox Config Diff Plugin
 
 NetBox plugin for Config Diff.
 
 * Free software: Apache-2.0
 * Documentation: https://miaow2.github.io/netbox-config-diff/
 
@@ -230,15 +238,15 @@
 
 With this plugin you can find diff between the rendered configuration for a device to its actual configuration, retrieved from the device itself, or stored in DataSource.
 Read about [DataSources](https://demo.netbox.dev/static/docs/models/core/datasource/) for further details.
 
 Device configuration renders natively in NetBox. This [feature](https://demo.netbox.dev/static/docs/features/configuration-rendering/) was introduced in 3.5 version.
  NetBox Labs [blog](https://demo.netbox.dev/static/docs/features/configuration-rendering/) post about it.
 
-Plugin supports a wide list of vendors (Cisco, Juniper, Huawei, MicroTik etc.) with the help of Scrapli. Read [Scrapli](https://github.com/carlmontanari/scrapli/tree/main/scrapli/driver/core) and [scrapli-community](https://github.com/scrapli/scrapli_community/tree/main/scrapli_community) documentations to find full list of vendors.
+Plugin supports a wide list of vendors (Cisco, Juniper, Huawei, MicroTik etc.) with the help of Scrapli. Read [Scrapli](https://carlmontanari.github.io/scrapli/user_guide/project_details/#supported-platforms) and [scrapli-community](https://scrapli.github.io/scrapli_community/user_guide/project_details/#supported-platforms) documentations to find full list of vendors.
 <!--about-end-->
 
 ## Compatibility
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
 |     3.5        |    =>0.1.0     |
```

### Comparing `netbox-config-diff-1.0.0/docs/media/screenshots/compliance-diff.png` & `netbox-config-diff-1.1.0/docs/media/screenshots/compliance-diff.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-1.0.0/docs/media/screenshots/compliance-error.png` & `netbox-config-diff-1.1.0/docs/media/screenshots/compliance-error.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-1.0.0/docs/media/screenshots/compliance-list.png` & `netbox-config-diff-1.1.0/docs/media/screenshots/compliance-list.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-1.0.0/docs/media/screenshots/compliance-ok.png` & `netbox-config-diff-1.1.0/docs/media/screenshots/compliance-ok.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-1.0.0/docs/media/screenshots/navbar.png` & `netbox-config-diff-1.1.0/docs/media/screenshots/navbar.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-1.0.0/docs/media/screenshots/platformsetting.png` & `netbox-config-diff-1.1.0/docs/media/screenshots/platformsetting.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-1.0.0/docs/media/screenshots/script-list.png` & `netbox-config-diff-1.1.0/docs/media/screenshots/script-list.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-1.0.0/docs/media/screenshots/script.png` & `netbox-config-diff-1.1.0/docs/media/screenshots/script.png`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-1.0.0/netbox_config_diff/__init__.py` & `netbox-config-diff-1.1.0/netbox_config_diff/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from extras.plugins import PluginConfig
 
 __author__ = "Artem Kotik"
 __email__ = "miaow2@yandex.ru"
-__version__ = "1.0.0"
+__version__ = "1.1.0"
 
 
 class ConfigDiffConfig(PluginConfig):
     name = "netbox_config_diff"
     verbose_name = "NetBox Config Diff Plugin"
     description = "Find diff between the intended device configuration and actual."
     author = __author__
-    email = __email__
+    author_email = __email__
     version = __version__
     base_url = "config-diff"
     required_settings = ["USERNAME", "PASSWORD"]
     min_version = "3.5.0"
 
 
 config = ConfigDiffConfig
```

### Comparing `netbox-config-diff-1.0.0/netbox_config_diff/api/serializers.py` & `netbox-config-diff-1.1.0/netbox_config_diff/api/serializers.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,14 +20,16 @@
             "display",
             "device",
             "status",
             "error",
             "diff",
             "rendered_config",
             "actual_config",
+            "missing",
+            "extra",
             "created",
             "last_updated",
         )
 
 
 class PlatformSettingSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(view_name="plugins-api:netbox_config_diff-api:platformsetting-detail")
```

### Comparing `netbox-config-diff-1.0.0/netbox_config_diff/api/views.py` & `netbox-config-diff-1.1.0/netbox_config_diff/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-1.0.0/netbox_config_diff/compliance/base.py` & `netbox-config-diff-1.1.0/netbox_config_diff/compliance/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from core.choices import DataSourceStatusChoices
 from core.models import DataFile, DataSource
 from dcim.choices import DeviceStatusChoices
 from dcim.models import Device, Site
 from django.core.exceptions import ObjectDoesNotExist
 from django.db.models import Q
 from extras.plugins import get_plugin_config
-from extras.querysets import ConfigContextQuerySet
 from extras.scripts import MultiObjectVar, ObjectVar
 from jinja2.exceptions import TemplateError
+from netutils.config.compliance import diff_network_config
 from utilities.exceptions import AbortScript
 
 from netbox_config_diff.models import ConfigCompliance
 
 from .models import DeviceDataClass
-from .utils import exclude_lines, get_unified_diff
+from .utils import PLATFORM_MAPPING, exclude_lines, get_unified_diff
 
 
 class ConfigDiffBase:
     site = ObjectVar(
         model=Site,
         required=False,
         description="Run compliance for devices (with status Active, primary IP and platform) in this site",
@@ -48,15 +48,15 @@
     def run_script(self, data: dict) -> None:
         devices = self.validate_data(data)
         devices = list(self.get_devices_with_rendered_configs(devices))
         self.get_actual_configs(devices)
         self.get_diff(devices)
         self.update_in_db(devices)
 
-    def validate_data(self, data: dict) -> Iterable[ConfigContextQuerySet]:
+    def validate_data(self, data: dict) -> Iterable[Device]:
         if not data["site"] and not data["devices"]:
             raise AbortScript("Define site or devices")
         if data.get("data_source") and data["data_source"].status != DataSourceStatusChoices.COMPLETED:
             raise AbortScript("Define synced DataSource")
 
         self.data = data
         if data["devices"]:
@@ -97,15 +97,15 @@
         if device.error:
             self.log_failure(f"{device.name} errored")
         elif device.diff:
             self.log_warning(f"{device.name} has diff between intented and actual configurations")
         else:
             self.log_success(f"{device.name} no diff")
 
-    def get_devices_with_rendered_configs(self, devices: Iterable[ConfigContextQuerySet]) -> Iterator[DeviceDataClass]:
+    def get_devices_with_rendered_configs(self, devices: Iterable[Device]) -> Iterator[DeviceDataClass]:
         username = get_plugin_config("netbox_config_diff", "USERNAME")
         password = get_plugin_config("netbox_config_diff", "PASSWORD")
         for device in devices:
             rendered_config = None
             error = None
             context_data = device.get_config_context()
             context_data.update({"device": device})
@@ -147,10 +147,16 @@
             loop = asyncio.get_event_loop()
             loop.run_until_complete(asyncio.gather(*(d.get_actual_config() for d in devices)))
 
     def get_diff(self, devices: list[DeviceDataClass]) -> None:
         for device in devices:
             if device.error is not None:
                 continue
-            device.diff = get_unified_diff(
-                device.rendered_config, exclude_lines(device.actual_config, device.exclude_regex), device.name
-            )
+            cleaned_config = exclude_lines(device.actual_config, device.exclude_regex)
+            device.diff = get_unified_diff(device.rendered_config, cleaned_config, device.name)
+            if device.platform in PLATFORM_MAPPING:
+                device.missing = diff_network_config(
+                    device.rendered_config, cleaned_config, PLATFORM_MAPPING[device.platform]
+                )
+                device.extra = diff_network_config(
+                    cleaned_config, device.rendered_config, PLATFORM_MAPPING[device.platform]
+                )
```

### Comparing `netbox-config-diff-1.0.0/netbox_config_diff/filtersets.py` & `netbox-config-diff-1.1.0/netbox_config_diff/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-1.0.0/netbox_config_diff/forms.py` & `netbox-config-diff-1.1.0/netbox_config_diff/forms.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-1.0.0/netbox_config_diff/graphql.py` & `netbox-config-diff-1.1.0/netbox_config_diff/graphql.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-1.0.0/netbox_config_diff/migrations/0001_initial.py` & `netbox-config-diff-1.1.0/netbox_config_diff/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-1.0.0/netbox_config_diff/migrations/0002_add_script.py` & `netbox-config-diff-1.1.0/netbox_config_diff/migrations/0002_add_script.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-1.0.0/netbox_config_diff/migrations/0003_configcompliance_actual_config_and_more.py` & `netbox-config-diff-1.1.0/netbox_config_diff/migrations/0003_configcompliance_actual_config_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-1.0.0/netbox_config_diff/migrations/0004_update_script.py` & `netbox-config-diff-1.1.0/netbox_config_diff/migrations/0004_update_script.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-1.0.0/netbox_config_diff/models.py` & `netbox-config-diff-1.1.0/netbox_config_diff/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,20 @@
     )
     actual_config = models.TextField(
         blank=True,
     )
     rendered_config = models.TextField(
         blank=True,
     )
+    missing = models.TextField(
+        blank=True,
+    )
+    extra = models.TextField(
+        blank=True,
+    )
 
     objects = RestrictedQuerySet.as_manager()
 
     class Meta:
         ordering = ("device",)
 
     def __str__(self):
@@ -63,16 +69,16 @@
         on_delete=models.CASCADE,
         related_name="platform_setting",
     )
     driver = models.CharField(
         max_length=25,
         help_text=_(
             "Scrapli driver for platfrom, you can find them in "
-            "<a href='https://github.com/carlmontanari/scrapli'>Scrapli</a> and "
-            "<a href='https://github.com/scrapli/scrapli_community'>Scrapli community</a> documentation."
+            "<a href='https://carlmontanari.github.io/scrapli/user_guide/project_details/#supported-platforms'>Scrapli</a> and "  # noqa
+            "<a href='https://scrapli.github.io/scrapli_community/user_guide/project_details/#supported-platforms'>Scrapli community</a> documentation."  # noqa
         ),
     )
     command = models.CharField(
         max_length=50,
         help_text=_("Command for getting config from device."),
     )
     exclude_regex = models.TextField(
```

### Comparing `netbox-config-diff-1.0.0/netbox_config_diff/navigation.py` & `netbox-config-diff-1.1.0/netbox_config_diff/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-1.0.0/netbox_config_diff/static/netbox_config_diff/diff2html-ui.min.js` & `netbox-config-diff-1.1.0/netbox_config_diff/static/netbox_config_diff/diff2html-ui.min.js`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-1.0.0/netbox_config_diff/static/netbox_config_diff/diff2html.min.css` & `netbox-config-diff-1.1.0/netbox_config_diff/static/netbox_config_diff/diff2html.min.css`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-1.0.0/netbox_config_diff/tables.py` & `netbox-config-diff-1.1.0/netbox_config_diff/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-1.0.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/config.html` & `netbox-config-diff-1.1.0/netbox_config_diff/templates/netbox_config_diff/configcompliance/config.html`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-1.0.0/netbox_config_diff/templates/netbox_config_diff/configcompliance.html` & `netbox-config-diff-1.1.0/netbox_config_diff/templates/netbox_config_diff/configcompliance.html`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-1.0.0/netbox_config_diff/templates/netbox_config_diff/platformsetting.html` & `netbox-config-diff-1.1.0/netbox_config_diff/templates/netbox_config_diff/platformsetting.html`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-1.0.0/netbox_config_diff/urls.py` & `netbox-config-diff-1.1.0/netbox_config_diff/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-config-diff-1.0.0/netbox_config_diff/views.py` & `netbox-config-diff-1.1.0/netbox_config_diff/views.py`

 * *Files 24% similar despite different names*

```diff
@@ -71,14 +71,50 @@
     template_header = "Actual Config"
     tab = ViewTab(
         label=_(template_header),
         weight=510,
     )
 
 
+@register_model_view(ConfigCompliance, "missing-extra")
+class ConfigComplianceMissingExtraConfigView(generic.ObjectView):
+    queryset = ConfigCompliance.objects.all()
+    template_name = "netbox_config_diff/configcompliance/missing_extra.html"
+    tab = ViewTab(
+        label=_("Missing/Extra"),
+        weight=520,
+    )
+
+    def export_parts(self, name, lines, suffix):
+        response = HttpResponse(lines, content_type="text")
+        filename = f"{name}_{suffix}.txt"
+        response["Content-Disposition"] = f'attachment; filename="{filename}"'
+        return response
+
+    def get(self, request, **kwargs):
+        instance = self.get_object(**kwargs)
+        context = self.get_extra_context(request, instance)
+
+        if request.GET.get("export_missing"):
+            return self.export_parts(instance.device.name, instance.missing, "missing")
+
+        if request.GET.get("export_extra"):
+            return self.export_parts(instance.device.name, instance.extra, "extra")
+
+        return render(
+            request,
+            self.get_template_name(),
+            {
+                "object": instance,
+                "tab": self.tab,
+                **context,
+            },
+        )
+
+
 class ConfigComplianceListView(generic.ObjectListView):
     queryset = ConfigCompliance.objects.prefetch_related("device")
     filterset = ConfigComplianceFilterSet
     filterset_form = ConfigComplianceFilterForm
     table = ConfigComplianceTable
```

### Comparing `netbox-config-diff-1.0.0/netbox_config_diff.egg-info/PKG-INFO` & `netbox-config-diff-1.1.0/netbox_config_diff.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-config-diff
-Version: 1.0.0
+Version: 1.1.0
 Summary: Find diff between the intended device configuration and actual.
 Author: Artem Kotik
 Author-email: miaow2@yandex.ru
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -214,14 +214,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
+[![NetBox version](https://img.shields.io/badge/NetBox-3.5-blue.svg)](https://github.com/netbox-community/netbox)
+[![Supported Versions](https://img.shields.io/pypi/pyversions/netbox-config-diff.svg)](https://pypi.org/project/netbox-config-diff/)
+[![PyPI version](https://badge.fury.io/py/netbox-config-diff.svg)](https://badge.fury.io/py/netbox-config-diff)
+[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+[![CI](https://github.com/miaow2/netbox-config-diff/actions/workflows/commit.yaml/badge.svg?branch=develop)](https://github.com/miaow2/netbox-config-diff/actions)
+
 # NetBox Config Diff Plugin
 
 NetBox plugin for Config Diff.
 
 * Free software: Apache-2.0
 * Documentation: https://miaow2.github.io/netbox-config-diff/
 
@@ -230,15 +238,15 @@
 
 With this plugin you can find diff between the rendered configuration for a device to its actual configuration, retrieved from the device itself, or stored in DataSource.
 Read about [DataSources](https://demo.netbox.dev/static/docs/models/core/datasource/) for further details.
 
 Device configuration renders natively in NetBox. This [feature](https://demo.netbox.dev/static/docs/features/configuration-rendering/) was introduced in 3.5 version.
  NetBox Labs [blog](https://demo.netbox.dev/static/docs/features/configuration-rendering/) post about it.
 
-Plugin supports a wide list of vendors (Cisco, Juniper, Huawei, MicroTik etc.) with the help of Scrapli. Read [Scrapli](https://github.com/carlmontanari/scrapli/tree/main/scrapli/driver/core) and [scrapli-community](https://github.com/scrapli/scrapli_community/tree/main/scrapli_community) documentations to find full list of vendors.
+Plugin supports a wide list of vendors (Cisco, Juniper, Huawei, MicroTik etc.) with the help of Scrapli. Read [Scrapli](https://carlmontanari.github.io/scrapli/user_guide/project_details/#supported-platforms) and [scrapli-community](https://scrapli.github.io/scrapli_community/user_guide/project_details/#supported-platforms) documentations to find full list of vendors.
 <!--about-end-->
 
 ## Compatibility
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
 |     3.5        |    =>0.1.0     |
```

### Comparing `netbox-config-diff-1.0.0/netbox_config_diff.egg-info/SOURCES.txt` & `netbox-config-diff-1.1.0/netbox_config_diff.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 docs/media/screenshots/compliance-diff.png
 docs/media/screenshots/compliance-error.png
 docs/media/screenshots/compliance-list.png
+docs/media/screenshots/compliance-missing-extra.png
 docs/media/screenshots/compliance-ok.png
 docs/media/screenshots/navbar.png
 docs/media/screenshots/platformsetting.png
 docs/media/screenshots/script-list.png
 docs/media/screenshots/script.png
 netbox_config_diff/__init__.py
 netbox_config_diff/choices.py
@@ -34,17 +35,19 @@
 netbox_config_diff/compliance/base.py
 netbox_config_diff/compliance/models.py
 netbox_config_diff/compliance/utils.py
 netbox_config_diff/migrations/0001_initial.py
 netbox_config_diff/migrations/0002_add_script.py
 netbox_config_diff/migrations/0003_configcompliance_actual_config_and_more.py
 netbox_config_diff/migrations/0004_update_script.py
+netbox_config_diff/migrations/0005_configcompliance_extra_missing.py
 netbox_config_diff/migrations/__init__.py
 netbox_config_diff/scripts/config_diff.py
 netbox_config_diff/static/netbox_config_diff/diff2html-ui.min.js
 netbox_config_diff/static/netbox_config_diff/diff2html.min.css
 netbox_config_diff/templates/netbox_config_diff/configcompliance.html
 netbox_config_diff/templates/netbox_config_diff/platformsetting.html
 netbox_config_diff/templates/netbox_config_diff/configcompliance/base.html
 netbox_config_diff/templates/netbox_config_diff/configcompliance/config.html
+netbox_config_diff/templates/netbox_config_diff/configcompliance/missing_extra.html
 requirements/base.txt
 requirements/dev.txt
```

### Comparing `netbox-config-diff-1.0.0/pyproject.toml` & `netbox-config-diff-1.1.0/pyproject.toml`

 * *Files identical despite different names*

