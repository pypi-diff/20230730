# Comparing `tmp/aa_sov_timer-1.8.0.tar.gz` & `tmp/aa_sov_timer-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_sov_timer-1.8.0.tar", last modified: Thu Apr 13 20:51:16 2023, max compression
+gzip compressed data, was "aa_sov_timer-1.9.0.tar", last modified: Sun Apr 16 17:59:19 2023, max compression
```

## Comparing `aa_sov_timer-1.8.0.tar` & `aa_sov_timer-1.9.0.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.745905 aa_sov_timer-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-04-13 20:51:16.745905 aa_sov_timer-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.733904 aa_sov_timer-1.8.0/aa_sov_timer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-04-13 20:51:16.000000 aa_sov_timer-1.8.0/aa_sov_timer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-13 20:51:16.000000 aa_sov_timer-1.8.0/aa_sov_timer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:51:16.000000 aa_sov_timer-1.8.0/aa_sov_timer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:51:16.000000 aa_sov_timer-1.8.0/aa_sov_timer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-13 20:51:16.000000 aa_sov_timer-1.8.0/aa_sov_timer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 20:51:16.000000 aa_sov_timer-1.8.0/aa_sov_timer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-13 20:51:16.745905 aa_sov_timer-1.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.733904 aa_sov_timer-1.8.0/sovtimer/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.725904 aa_sov_timer-1.8.0/sovtimer/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.725904 aa_sov_timer-1.8.0/sovtimer/docs/changelog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.733904 aa_sov_timer-1.8.0/sovtimer/docs/changelog/0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    19485 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/docs/changelog/0.6.0/128572686-b01869c4-005e-4141-a28f-7bd286c301f0.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.733904 aa_sov_timer-1.8.0/sovtimer/docs/presentation/
--rw-r--r--   0 runner    (1001) docker     (123)   166569 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/docs/presentation/aa-sov-timer-dark-mode.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   159628 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/docs/presentation/aa-sov-timer-light-mode.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.733904 aa_sov_timer-1.8.0/sovtimer/locale/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/locale/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.725904 aa_sov_timer-1.8.0/sovtimer/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.737904 aa_sov_timer-1.8.0/sovtimer/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.725904 aa_sov_timer-1.8.0/sovtimer/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.737904 aa_sov_timer-1.8.0/sovtimer/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.725904 aa_sov_timer-1.8.0/sovtimer/locale/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.737904 aa_sov_timer-1.8.0/sovtimer/locale/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/locale/fr_FR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.725904 aa_sov_timer-1.8.0/sovtimer/locale/it_IT/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.737904 aa_sov_timer-1.8.0/sovtimer/locale/it_IT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/locale/it_IT/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.725904 aa_sov_timer-1.8.0/sovtimer/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.737904 aa_sov_timer-1.8.0/sovtimer/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.725904 aa_sov_timer-1.8.0/sovtimer/locale/ko_KR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.737904 aa_sov_timer-1.8.0/sovtimer/locale/ko_KR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/locale/ko_KR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.725904 aa_sov_timer-1.8.0/sovtimer/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.737904 aa_sov_timer-1.8.0/sovtimer/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.725904 aa_sov_timer-1.8.0/sovtimer/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.737904 aa_sov_timer-1.8.0/sovtimer/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.725904 aa_sov_timer-1.8.0/sovtimer/management/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.737904 aa_sov_timer-1.8.0/sovtimer/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/management/commands/sovtimer_load_initial_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.737904 aa_sov_timer-1.8.0/sovtimer/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/migrations/0002_aasovtimercampaigns_aasovtimerstructures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/migrations/0003_auto_20201113_1033.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/migrations/0004_auto_20201113_1856.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/migrations/0005_auto_20201114_0720.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/migrations/0006_rename_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/migrations/0007_cleanup_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/migrations/0008_fix_campaign_attackers_score.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/providers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.725904 aa_sov_timer-1.8.0/sovtimer/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.729904 aa_sov_timer-1.8.0/sovtimer/static/sovtimer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.741904 aa_sov_timer-1.8.0/sovtimer/static/sovtimer/css/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/static/sovtimer/css/aa-bootstrap-fix.css
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/static/sovtimer/css/aa-bootstrap-fix.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/static/sovtimer/css/aa-sov-timer.css
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/static/sovtimer/css/aa-sov-timer.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.729904 aa_sov_timer-1.8.0/sovtimer/static/sovtimer/font/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.729904 aa_sov_timer-1.8.0/sovtimer/static/sovtimer/font/materialicons/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.741904 aa_sov_timer-1.8.0/sovtimer/static/sovtimer/font/materialicons/v103/
--rw-r--r--   0 runner    (1001) docker     (123)    33122 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/static/sovtimer/font/materialicons/v103/MaterialIcons-Regular.codepoints
--rw-r--r--   0 runner    (1001) docker     (123)   285724 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/static/sovtimer/font/materialicons/v103/MaterialIcons-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   110560 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/static/sovtimer/font/materialicons/v103/MaterialIcons-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/static/sovtimer/font/materialicons/v103/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.741904 aa_sov_timer-1.8.0/sovtimer/static/sovtimer/images/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/static/sovtimer/images/zkillboard.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.741904 aa_sov_timer-1.8.0/sovtimer/static/sovtimer/js/
--rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/static/sovtimer/js/aa-sov-timer.js
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/static/sovtimer/js/aa-sov-timer.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.729904 aa_sov_timer-1.8.0/sovtimer/static/sovtimer/libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.729904 aa_sov_timer-1.8.0/sovtimer/static/sovtimer/libs/datatables/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.741904 aa_sov_timer-1.8.0/sovtimer/static/sovtimer/libs/datatables/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/static/sovtimer/libs/datatables/plugins/datetime.js
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/static/sovtimer/libs/datatables/plugins/datetime.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.729904 aa_sov_timer-1.8.0/sovtimer/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.741904 aa_sov_timer-1.8.0/sovtimer/templates/sovtimer/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/templates/sovtimer/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.745905 aa_sov_timer-1.8.0/sovtimer/templates/sovtimer/bundles/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/templates/sovtimer/bundles/aa-sov-timer-css.html
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/templates/sovtimer/bundles/aa-sov-timer-js.html
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/templates/sovtimer/bundles/datatables-datetime-js.html
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/templates/sovtimer/dashboard.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.729904 aa_sov_timer-1.8.0/sovtimer/templates/sovtimer/partials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.745905 aa_sov_timer-1.8.0/sovtimer/templates/sovtimer/partials/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/templates/sovtimer/partials/dashboard/table.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.745905 aa_sov_timer-1.8.0/sovtimer/templates/sovtimer/partials/header/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/templates/sovtimer/partials/header/h1.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.745905 aa_sov_timer-1.8.0/sovtimer/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/templatetags/sovtimer_versioned_static.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.745905 aa_sov_timer-1.8.0/sovtimer/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:51:16.745905 aa_sov_timer-1.8.0/sovtimer/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/tests/fixtures/allianceauth.json
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/tests/fixtures/load_allianceauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/tests/fixtures/load_sovtimer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/tests/fixtures/sovtimer.json
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/tests/fixtures/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/tests/test_ajax_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/tests/test_templatetags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-04-13 20:50:54.000000 aa_sov_timer-1.8.0/sovtimer/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.023719 aa_sov_timer-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-04-16 17:59:19.023719 aa_sov_timer-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.011719 aa_sov_timer-1.9.0/aa_sov_timer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-04-16 17:59:18.000000 aa_sov_timer-1.9.0/aa_sov_timer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-16 17:59:19.000000 aa_sov_timer-1.9.0/aa_sov_timer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 17:59:18.000000 aa_sov_timer-1.9.0/aa_sov_timer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 17:59:18.000000 aa_sov_timer-1.9.0/aa_sov_timer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-16 17:59:18.000000 aa_sov_timer-1.9.0/aa_sov_timer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-16 17:59:18.000000 aa_sov_timer-1.9.0/aa_sov_timer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-16 17:59:19.023719 aa_sov_timer-1.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.011719 aa_sov_timer-1.9.0/sovtimer/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/auth_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.003719 aa_sov_timer-1.9.0/sovtimer/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.003719 aa_sov_timer-1.9.0/sovtimer/docs/changelog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.011719 aa_sov_timer-1.9.0/sovtimer/docs/changelog/0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    19485 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/docs/changelog/0.6.0/128572686-b01869c4-005e-4141-a28f-7bd286c301f0.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.011719 aa_sov_timer-1.9.0/sovtimer/docs/presentation/
+-rw-r--r--   0 runner    (1001) docker     (123)   166569 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/docs/presentation/aa-sov-timer-dark-mode.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   159628 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/docs/presentation/aa-sov-timer-light-mode.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.011719 aa_sov_timer-1.9.0/sovtimer/locale/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/locale/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.007719 aa_sov_timer-1.9.0/sovtimer/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.015719 aa_sov_timer-1.9.0/sovtimer/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.007719 aa_sov_timer-1.9.0/sovtimer/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.015719 aa_sov_timer-1.9.0/sovtimer/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.007719 aa_sov_timer-1.9.0/sovtimer/locale/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.015719 aa_sov_timer-1.9.0/sovtimer/locale/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/locale/fr_FR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.007719 aa_sov_timer-1.9.0/sovtimer/locale/it_IT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.015719 aa_sov_timer-1.9.0/sovtimer/locale/it_IT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/locale/it_IT/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.007719 aa_sov_timer-1.9.0/sovtimer/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.015719 aa_sov_timer-1.9.0/sovtimer/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.007719 aa_sov_timer-1.9.0/sovtimer/locale/ko_KR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.015719 aa_sov_timer-1.9.0/sovtimer/locale/ko_KR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/locale/ko_KR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.007719 aa_sov_timer-1.9.0/sovtimer/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.015719 aa_sov_timer-1.9.0/sovtimer/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.007719 aa_sov_timer-1.9.0/sovtimer/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.015719 aa_sov_timer-1.9.0/sovtimer/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.007719 aa_sov_timer-1.9.0/sovtimer/management/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.015719 aa_sov_timer-1.9.0/sovtimer/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/management/commands/sovtimer_load_initial_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.015719 aa_sov_timer-1.9.0/sovtimer/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/migrations/0002_aasovtimercampaigns_aasovtimerstructures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/migrations/0003_auto_20201113_1033.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/migrations/0004_auto_20201113_1856.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/migrations/0005_auto_20201114_0720.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/migrations/0006_rename_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/migrations/0007_cleanup_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/migrations/0008_fix_campaign_attackers_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/providers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.007719 aa_sov_timer-1.9.0/sovtimer/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.007719 aa_sov_timer-1.9.0/sovtimer/static/sovtimer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.015719 aa_sov_timer-1.9.0/sovtimer/static/sovtimer/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/static/sovtimer/css/aa-bootstrap-fix.css
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/static/sovtimer/css/aa-bootstrap-fix.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/static/sovtimer/css/aa-sov-timer.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/static/sovtimer/css/aa-sov-timer.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.007719 aa_sov_timer-1.9.0/sovtimer/static/sovtimer/font/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.007719 aa_sov_timer-1.9.0/sovtimer/static/sovtimer/font/materialicons/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.019719 aa_sov_timer-1.9.0/sovtimer/static/sovtimer/font/materialicons/v103/
+-rw-r--r--   0 runner    (1001) docker     (123)    33122 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/static/sovtimer/font/materialicons/v103/MaterialIcons-Regular.codepoints
+-rw-r--r--   0 runner    (1001) docker     (123)   285724 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/static/sovtimer/font/materialicons/v103/MaterialIcons-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   110560 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/static/sovtimer/font/materialicons/v103/MaterialIcons-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/static/sovtimer/font/materialicons/v103/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.019719 aa_sov_timer-1.9.0/sovtimer/static/sovtimer/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/static/sovtimer/images/zkillboard.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.019719 aa_sov_timer-1.9.0/sovtimer/static/sovtimer/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/static/sovtimer/js/aa-sov-timer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/static/sovtimer/js/aa-sov-timer.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.007719 aa_sov_timer-1.9.0/sovtimer/static/sovtimer/libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.007719 aa_sov_timer-1.9.0/sovtimer/static/sovtimer/libs/datatables/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.019719 aa_sov_timer-1.9.0/sovtimer/static/sovtimer/libs/datatables/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/static/sovtimer/libs/datatables/plugins/datetime.js
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/static/sovtimer/libs/datatables/plugins/datetime.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.007719 aa_sov_timer-1.9.0/sovtimer/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.019719 aa_sov_timer-1.9.0/sovtimer/templates/sovtimer/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/templates/sovtimer/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.019719 aa_sov_timer-1.9.0/sovtimer/templates/sovtimer/bundles/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/templates/sovtimer/bundles/aa-sov-timer-css.html
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/templates/sovtimer/bundles/aa-sov-timer-js.html
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/templates/sovtimer/bundles/datatables-datetime-js.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/templates/sovtimer/dashboard.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.011719 aa_sov_timer-1.9.0/sovtimer/templates/sovtimer/partials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.019719 aa_sov_timer-1.9.0/sovtimer/templates/sovtimer/partials/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/templates/sovtimer/partials/dashboard/table.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.019719 aa_sov_timer-1.9.0/sovtimer/templates/sovtimer/partials/header/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/templates/sovtimer/partials/header/h1.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.019719 aa_sov_timer-1.9.0/sovtimer/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/templatetags/sovtimer_versioned_static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.023719 aa_sov_timer-1.9.0/sovtimer/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:59:19.023719 aa_sov_timer-1.9.0/sovtimer/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/tests/fixtures/allianceauth.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/tests/fixtures/load_allianceauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/tests/fixtures/load_sovtimer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/tests/fixtures/sovtimer.json
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/tests/fixtures/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/tests/test_ajax_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/tests/test_templatetags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-04-16 17:59:00.000000 aa_sov_timer-1.9.0/sovtimer/views.py
```

### Comparing `aa_sov_timer-1.8.0/LICENSE` & `aa_sov_timer-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/PKG-INFO` & `aa_sov_timer-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa_sov_timer
-Version: 1.8.0
+Version: 1.9.0
 Summary: Sov Campaign Timer for Alliance Auth
 Home-page: https://github.com/ppfeufer/aa-sov-timer
 Author: Peter Pfeufer
 Author-email: develop@ppfeufer.de
 Maintainer: Peter Pfeufer
 Maintainer-email: develop@ppfeufer.de
 License: GPL-3.0
```

### Comparing `aa_sov_timer-1.8.0/README.md` & `aa_sov_timer-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/aa_sov_timer.egg-info/PKG-INFO` & `aa_sov_timer-1.9.0/aa_sov_timer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-sov-timer
-Version: 1.8.0
+Version: 1.9.0
 Summary: Sov Campaign Timer for Alliance Auth
 Home-page: https://github.com/ppfeufer/aa-sov-timer
 Author: Peter Pfeufer
 Author-email: develop@ppfeufer.de
 Maintainer: Peter Pfeufer
 Maintainer-email: develop@ppfeufer.de
 License: GPL-3.0
```

### Comparing `aa_sov_timer-1.8.0/aa_sov_timer.egg-info/SOURCES.txt` & `aa_sov_timer-1.9.0/aa_sov_timer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/setup.cfg` & `aa_sov_timer-1.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/auth_hooks.py` & `aa_sov_timer-1.9.0/sovtimer/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/docs/changelog/0.6.0/128572686-b01869c4-005e-4141-a28f-7bd286c301f0.png` & `aa_sov_timer-1.9.0/sovtimer/docs/changelog/0.6.0/128572686-b01869c4-005e-4141-a28f-7bd286c301f0.png`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/docs/presentation/aa-sov-timer-dark-mode.jpg` & `aa_sov_timer-1.9.0/sovtimer/docs/presentation/aa-sov-timer-dark-mode.jpg`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/docs/presentation/aa-sov-timer-light-mode.jpg` & `aa_sov_timer-1.9.0/sovtimer/docs/presentation/aa-sov-timer-light-mode.jpg`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/locale/de/LC_MESSAGES/django.mo` & `aa_sov_timer-1.9.0/sovtimer/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/locale/de/LC_MESSAGES/django.po` & `aa_sov_timer-1.9.0/sovtimer/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/locale/es/LC_MESSAGES/django.po` & `aa_sov_timer-1.9.0/sovtimer/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/locale/fr_FR/LC_MESSAGES/django.po` & `aa_sov_timer-1.9.0/sovtimer/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/locale/it_IT/LC_MESSAGES/django.po` & `aa_sov_timer-1.9.0/sovtimer/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/locale/ja/LC_MESSAGES/django.po` & `aa_sov_timer-1.9.0/sovtimer/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/locale/ko_KR/LC_MESSAGES/django.po` & `aa_sov_timer-1.9.0/sovtimer/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/locale/ru/LC_MESSAGES/django.po` & `aa_sov_timer-1.9.0/sovtimer/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
+#, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-04-12 09:23+0200\n"
-"PO-Revision-Date: 2023-04-13 10:41+0000\n"
-"Last-Translator: \"H. Peter Pfeufer\" <info@ppfeufer.de>\n"
-"Language-Team: Russian <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-sov-timer/ru/>\n"
-"Language: ru\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || ("
-"n%100>=11 && n%100<=14)? 2 : 3);\n"
-"X-Generator: Weblate 4.16.4\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: models.py:103
 msgid "IHub Defense"
 msgstr ""
 
 #: models.py:104
 msgid "TCU Defense"
@@ -35,15 +33,15 @@
 #: templates/sovtimer/dashboard.html:6
 msgid "Sovereignty Timers"
 msgstr ""
 
 #: templates/sovtimer/dashboard.html:20
 #: templates/sovtimer/partials/dashboard/table.html:24
 msgid "System"
-msgstr "Система"
+msgstr ""
 
 #: templates/sovtimer/dashboard.html:21
 #: templates/sovtimer/partials/dashboard/table.html:25
 msgid "Constellation"
 msgstr ""
 
 #: templates/sovtimer/dashboard.html:22
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aa_sov_timer-1.8.0/sovtimer/management/commands/sovtimer_load_initial_data.py` & `aa_sov_timer-1.9.0/sovtimer/management/commands/sovtimer_load_initial_data.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/migrations/0001_initial.py` & `aa_sov_timer-1.9.0/sovtimer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/migrations/0002_aasovtimercampaigns_aasovtimerstructures.py` & `aa_sov_timer-1.9.0/sovtimer/migrations/0002_aasovtimercampaigns_aasovtimerstructures.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/migrations/0003_auto_20201113_1033.py` & `aa_sov_timer-1.9.0/sovtimer/migrations/0003_auto_20201113_1033.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/migrations/0004_auto_20201113_1856.py` & `aa_sov_timer-1.9.0/sovtimer/migrations/0004_auto_20201113_1856.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/migrations/0005_auto_20201114_0720.py` & `aa_sov_timer-1.9.0/sovtimer/migrations/0005_auto_20201114_0720.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/migrations/0006_rename_models.py` & `aa_sov_timer-1.9.0/sovtimer/migrations/0006_rename_models.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/migrations/0007_cleanup_models.py` & `aa_sov_timer-1.9.0/sovtimer/migrations/0007_cleanup_models.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/models.py` & `aa_sov_timer-1.9.0/sovtimer/models.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/static/sovtimer/css/aa-sov-timer.css` & `aa_sov_timer-1.9.0/sovtimer/static/sovtimer/css/aa-sov-timer.css`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/static/sovtimer/css/aa-sov-timer.min.css` & `aa_sov_timer-1.9.0/sovtimer/static/sovtimer/css/aa-sov-timer.min.css`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/static/sovtimer/font/materialicons/v103/MaterialIcons-Regular.codepoints` & `aa_sov_timer-1.9.0/sovtimer/static/sovtimer/font/materialicons/v103/MaterialIcons-Regular.codepoints`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/static/sovtimer/font/materialicons/v103/MaterialIcons-Regular.ttf` & `aa_sov_timer-1.9.0/sovtimer/static/sovtimer/font/materialicons/v103/MaterialIcons-Regular.ttf`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/static/sovtimer/font/materialicons/v103/MaterialIcons-Regular.woff2` & `aa_sov_timer-1.9.0/sovtimer/static/sovtimer/font/materialicons/v103/MaterialIcons-Regular.woff2`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/static/sovtimer/font/materialicons/v103/README.md` & `aa_sov_timer-1.9.0/sovtimer/static/sovtimer/font/materialicons/v103/README.md`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/static/sovtimer/js/aa-sov-timer.js` & `aa_sov_timer-1.9.0/sovtimer/static/sovtimer/js/aa-sov-timer.js`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/static/sovtimer/js/aa-sov-timer.min.js` & `aa_sov_timer-1.9.0/sovtimer/static/sovtimer/js/aa-sov-timer.min.js`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/static/sovtimer/libs/datatables/plugins/datetime.js` & `aa_sov_timer-1.9.0/sovtimer/static/sovtimer/libs/datatables/plugins/datetime.js`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/static/sovtimer/libs/datatables/plugins/datetime.min.js` & `aa_sov_timer-1.9.0/sovtimer/static/sovtimer/libs/datatables/plugins/datetime.min.js`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/tasks.py` & `aa_sov_timer-1.9.0/sovtimer/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/templates/sovtimer/dashboard.html` & `aa_sov_timer-1.9.0/sovtimer/templates/sovtimer/dashboard.html`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/templates/sovtimer/partials/dashboard/table.html` & `aa_sov_timer-1.9.0/sovtimer/templates/sovtimer/partials/dashboard/table.html`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/templatetags/sovtimer_versioned_static.py` & `aa_sov_timer-1.9.0/sovtimer/templatetags/sovtimer_versioned_static.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/tests/fixtures/allianceauth.json` & `aa_sov_timer-1.9.0/sovtimer/tests/fixtures/allianceauth.json`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/tests/fixtures/load_allianceauth.py` & `aa_sov_timer-1.9.0/sovtimer/tests/fixtures/load_allianceauth.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/tests/fixtures/load_sovtimer.py` & `aa_sov_timer-1.9.0/sovtimer/tests/fixtures/load_sovtimer.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/tests/fixtures/sovtimer.json` & `aa_sov_timer-1.9.0/sovtimer/tests/fixtures/sovtimer.json`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/tests/test_ajax_calls.py` & `aa_sov_timer-1.9.0/sovtimer/tests/test_ajax_calls.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/tests/test_integration.py` & `aa_sov_timer-1.9.0/sovtimer/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/tests/test_templatetags.py` & `aa_sov_timer-1.9.0/sovtimer/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/tests/utils.py` & `aa_sov_timer-1.9.0/sovtimer/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-1.8.0/sovtimer/views.py` & `aa_sov_timer-1.9.0/sovtimer/views.py`

 * *Files identical despite different names*

