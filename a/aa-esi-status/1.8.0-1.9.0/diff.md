# Comparing `tmp/aa_esi_status-1.8.0.tar.gz` & `tmp/aa_esi_status-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_esi_status-1.8.0.tar", last modified: Thu Apr 13 16:12:22 2023, max compression
+gzip compressed data, was "aa_esi_status-1.9.0.tar", last modified: Sun Apr 16 16:25:10 2023, max compression
```

## Comparing `aa_esi_status-1.8.0.tar` & `aa_esi_status-1.9.0.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.945193 aa_esi_status-1.8.0/aa_esi_status.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-13 16:12:22.000000 aa_esi_status-1.8.0/aa_esi_status.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-13 16:12:22.000000 aa_esi_status-1.8.0/aa_esi_status.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 16:12:22.000000 aa_esi_status-1.8.0/aa_esi_status.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 16:12:22.000000 aa_esi_status-1.8.0/aa_esi_status.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-13 16:12:22.000000 aa_esi_status-1.8.0/aa_esi_status.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 16:12:22.000000 aa_esi_status-1.8.0/aa_esi_status.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.945193 aa_esi_status-1.8.0/esistatus/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.945193 aa_esi_status-1.8.0/esistatus/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   229003 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/docs/aa-esi-status.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.945193 aa_esi_status-1.8.0/esistatus/locale/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/locale/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.941193 aa_esi_status-1.8.0/esistatus/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/esistatus/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.941193 aa_esi_status-1.8.0/esistatus/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/esistatus/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.941193 aa_esi_status-1.8.0/esistatus/locale/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/esistatus/locale/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/locale/fr_FR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.941193 aa_esi_status-1.8.0/esistatus/locale/it_IT/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/esistatus/locale/it_IT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/locale/it_IT/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.941193 aa_esi_status-1.8.0/esistatus/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/esistatus/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.945193 aa_esi_status-1.8.0/esistatus/locale/ko_KR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/esistatus/locale/ko_KR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/locale/ko_KR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.945193 aa_esi_status-1.8.0/esistatus/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/esistatus/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.945193 aa_esi_status-1.8.0/esistatus/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/esistatus/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/esistatus/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.945193 aa_esi_status-1.8.0/esistatus/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.945193 aa_esi_status-1.8.0/esistatus/static/esistatus/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/esistatus/static/esistatus/css/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/static/esistatus/css/esistatus.css
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/static/esistatus/css/esistatus.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.945193 aa_esi_status-1.8.0/esistatus/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/esistatus/templates/esistatus/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/templates/esistatus/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/templates/esistatus/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/esistatus/templates/esistatus/partials/
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/templates/esistatus/partials/endpoints.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/esistatus/templates/esistatus/partials/header/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/templates/esistatus/partials/header/page-header.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/esistatus/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/templatetags/esistatus_versioned_static.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/esistatus/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/tests/test_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/tests/test_auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/tests/test_templatetags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/esistatus/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-13 16:12:05.000000 aa_esi_status-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-13 16:12:22.949193 aa_esi_status-1.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:10.787869 aa_esi_status-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-04-16 16:25:10.787869 aa_esi_status-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:10.783869 aa_esi_status-1.9.0/aa_esi_status.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-04-16 16:25:10.000000 aa_esi_status-1.9.0/aa_esi_status.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-16 16:25:10.000000 aa_esi_status-1.9.0/aa_esi_status.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 16:25:10.000000 aa_esi_status-1.9.0/aa_esi_status.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 16:25:10.000000 aa_esi_status-1.9.0/aa_esi_status.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-16 16:25:10.000000 aa_esi_status-1.9.0/aa_esi_status.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-16 16:25:10.000000 aa_esi_status-1.9.0/aa_esi_status.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:10.783869 aa_esi_status-1.9.0/esistatus/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/esistatus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/esistatus/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/esistatus/auth_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/esistatus/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:10.783869 aa_esi_status-1.9.0/esistatus/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   229003 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/esistatus/docs/aa-esi-status.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:10.783869 aa_esi_status-1.9.0/esistatus/locale/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/esistatus/locale/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:10.779869 aa_esi_status-1.9.0/esistatus/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:10.787869 aa_esi_status-1.9.0/esistatus/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/esistatus/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/esistatus/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:10.779869 aa_esi_status-1.9.0/esistatus/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:10.787869 aa_esi_status-1.9.0/esistatus/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/esistatus/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:10.779869 aa_esi_status-1.9.0/esistatus/locale/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:10.787869 aa_esi_status-1.9.0/esistatus/locale/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/esistatus/locale/fr_FR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:10.779869 aa_esi_status-1.9.0/esistatus/locale/it_IT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:10.787869 aa_esi_status-1.9.0/esistatus/locale/it_IT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/esistatus/locale/it_IT/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:10.779869 aa_esi_status-1.9.0/esistatus/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:10.787869 aa_esi_status-1.9.0/esistatus/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/esistatus/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:10.783869 aa_esi_status-1.9.0/esistatus/locale/ko_KR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:10.787869 aa_esi_status-1.9.0/esistatus/locale/ko_KR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/esistatus/locale/ko_KR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:10.783869 aa_esi_status-1.9.0/esistatus/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:10.787869 aa_esi_status-1.9.0/esistatus/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/esistatus/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/esistatus/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:10.783869 aa_esi_status-1.9.0/esistatus/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:10.787869 aa_esi_status-1.9.0/esistatus/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/esistatus/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:10.787869 aa_esi_status-1.9.0/esistatus/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/esistatus/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/esistatus/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/esistatus/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:10.783869 aa_esi_status-1.9.0/esistatus/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:10.783869 aa_esi_status-1.9.0/esistatus/static/esistatus/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:10.787869 aa_esi_status-1.9.0/esistatus/static/esistatus/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/esistatus/static/esistatus/css/esistatus.css
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/esistatus/static/esistatus/css/esistatus.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:10.783869 aa_esi_status-1.9.0/esistatus/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:10.787869 aa_esi_status-1.9.0/esistatus/templates/esistatus/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/esistatus/templates/esistatus/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/esistatus/templates/esistatus/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:10.787869 aa_esi_status-1.9.0/esistatus/templates/esistatus/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/esistatus/templates/esistatus/partials/endpoints.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:10.787869 aa_esi_status-1.9.0/esistatus/templates/esistatus/partials/header/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/esistatus/templates/esistatus/partials/header/page-header.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:10.787869 aa_esi_status-1.9.0/esistatus/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/esistatus/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/esistatus/templatetags/esistatus_versioned_static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:10.787869 aa_esi_status-1.9.0/esistatus/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/esistatus/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/esistatus/tests/test_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/esistatus/tests/test_auth_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/esistatus/tests/test_templatetags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/esistatus/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/esistatus/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/esistatus/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-16 16:24:53.000000 aa_esi_status-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-16 16:25:10.787869 aa_esi_status-1.9.0/setup.cfg
```

### Comparing `aa_esi_status-1.8.0/CHANGELOG.md` & `aa_esi_status-1.9.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 The format is based on [Keep a Changelog](http://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](http://semver.org/).
 
 
 ## [In Development] - Unreleased
 
 
+## [1.9.0] - 2023-04-16
+
+### Added
+
+- Russian translation
+
+
 ## [1.8.0] - 2023-04-13
 
 ### Added
 
 - German translation
 
 
@@ -183,15 +190,16 @@
 - Warning when ESI status couldn't be loaded, for what ever reason
 
 
 ## [0.1.0-alpha.2] - 2020-10-11
 
 ### Changed
 
-- Link to image in README updated since GitHub changed the default **master** branch to _main_. Fucking stupid change ...
+- Link to image in README updated since GitHub changed the default **master** branch
+  to _main_. Fucking stupid change ...
 
 
 ## [0.1.0-alpha.1] - 2020-10-11
 
 ### Added
 
 - initial version for testing purposes
```

### Comparing `aa_esi_status-1.8.0/LICENSE` & `aa_esi_status-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_esi_status-1.8.0/PKG-INFO` & `aa_esi_status-1.9.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa_esi_status
-Version: 1.8.0
+Version: 1.9.0
 Summary: A simple status monitor for ESI
 Home-page: https://github.com/ppfeufer/aa-esi-status
 Author: Peter Pfeufer
 Author-email: develop@ppfeufer.de
 Maintainer: Peter Pfeufer
 Maintainer-email: develop@ppfeufer.de
 License: GPL-3.0
@@ -44,76 +44,83 @@
 
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/N4N8CL1BY)
 
 App for Alliance Auth to show the current status of ESI and its end points.
 
 ![AA ESI Status](https://raw.githubusercontent.com/ppfeufer/aa-esi-status/main/esistatus/docs/aa-esi-status.jpg)
 
-## Contents
 
-- [Installation](#installation)
-- [Updating](#updating)
-- [Change Log](CHANGELOG.md)
+<!-- TOC -->
+* [AA ESI Status](#aa-esi-status)
+  * [Installation](#installation)
+    * [Step 1: Install the app](#step-1-install-the-app)
+    * [Step 2: Update your AA settings](#step-2-update-your-aa-settings)
+    * [Step 3: Finalizing the installation](#step-3-finalizing-the-installation)
+    * [Step 4: Setting up permissions](#step-4-setting-up-permissions)
+  * [Updating](#updating)
+<!-- TOC -->
 
 
 ## Installation
 
 **Important**: This app is a plugin for Alliance Auth. If you don't have
 Alliance Auth running already, please install it first before proceeding.
-(see the official [AA installation guide](https://allianceauth.readthedocs.io/en/latest/installation/allianceauth.html) for details)
+(See the official [AA installation guide](https://allianceauth.readthedocs.io/en/latest/installation/allianceauth.html) for details)
 
 
-### Step 1 - Install app
+### Step 1: Install the app
 
-Make sure you are in the virtual environment (venv) of your Alliance Auth installation.
+Make sure you're in the virtual environment (venv) of your Alliance Auth installation.
 Then install the latest version:
 
-```bash
+```shell
 pip install aa-esi-status
 ```
 
 
-### Step 2 - Update your AA settings
+### Step 2: Update your AA settings
 
 Configure your AA settings (`local.py`) as follows:
 
 - Add `'esistatus',` to `INSTALLED_APPS`
 
 
-### Step 3 - Finalize the installation
+### Step 3: Finalizing the installation
 
 Run migrations & copy static files
 
-```bash
+```shell
 python manage.py collectstatic
 python manage.py migrate
 ```
 
 Restart your supervisor services for AA
 
 
-### Step 4 - Setup permissions
+### Step 4: Setting up permissions
 
-Now you can setup permissions in Alliance Auth for your users.
-Add ``esistatus|esi status|Can access ths app`` to the states and/or groups you would
+Now you can set up permissions in Alliance Auth for your users.
+Add `esistatus|esi status|Can access this app` to the states and/or groups you would
 like to have access.
 
 
 ## Updating
 
-To update your existing installation of AA Time Zones first enable your virtual environment.
+To update your existing installation of AA Time Zones, first enable your virtual
+environment.
 
-Then run the following commands from your AA project directory (the one that contains `manage.py`).
+Then run the following commands from your AA project directory (the one that
+contains `manage.py`).
 
-```bash
+```shell
 pip install -U aa-esi-status
 ```
 
-```bash
+```shell
 python manage.py collectstatic
 ```
 
-```bash
+```shell
 python manage.py migrate
 ```
 
 Now restart your AA supervisor services.
```

### Comparing `aa_esi_status-1.8.0/README.md` & `aa_esi_status-1.9.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -13,76 +13,83 @@
 
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/N4N8CL1BY)
 
 App for Alliance Auth to show the current status of ESI and its end points.
 
 ![AA ESI Status](https://raw.githubusercontent.com/ppfeufer/aa-esi-status/main/esistatus/docs/aa-esi-status.jpg)
 
-## Contents
 
-- [Installation](#installation)
-- [Updating](#updating)
-- [Change Log](CHANGELOG.md)
+<!-- TOC -->
+* [AA ESI Status](#aa-esi-status)
+  * [Installation](#installation)
+    * [Step 1: Install the app](#step-1-install-the-app)
+    * [Step 2: Update your AA settings](#step-2-update-your-aa-settings)
+    * [Step 3: Finalizing the installation](#step-3-finalizing-the-installation)
+    * [Step 4: Setting up permissions](#step-4-setting-up-permissions)
+  * [Updating](#updating)
+<!-- TOC -->
 
 
 ## Installation
 
 **Important**: This app is a plugin for Alliance Auth. If you don't have
 Alliance Auth running already, please install it first before proceeding.
-(see the official [AA installation guide](https://allianceauth.readthedocs.io/en/latest/installation/allianceauth.html) for details)
+(See the official [AA installation guide](https://allianceauth.readthedocs.io/en/latest/installation/allianceauth.html) for details)
 
 
-### Step 1 - Install app
+### Step 1: Install the app
 
-Make sure you are in the virtual environment (venv) of your Alliance Auth installation.
+Make sure you're in the virtual environment (venv) of your Alliance Auth installation.
 Then install the latest version:
 
-```bash
+```shell
 pip install aa-esi-status
 ```
 
 
-### Step 2 - Update your AA settings
+### Step 2: Update your AA settings
 
 Configure your AA settings (`local.py`) as follows:
 
 - Add `'esistatus',` to `INSTALLED_APPS`
 
 
-### Step 3 - Finalize the installation
+### Step 3: Finalizing the installation
 
 Run migrations & copy static files
 
-```bash
+```shell
 python manage.py collectstatic
 python manage.py migrate
 ```
 
 Restart your supervisor services for AA
 
 
-### Step 4 - Setup permissions
+### Step 4: Setting up permissions
 
-Now you can setup permissions in Alliance Auth for your users.
-Add ``esistatus|esi status|Can access ths app`` to the states and/or groups you would
+Now you can set up permissions in Alliance Auth for your users.
+Add `esistatus|esi status|Can access this app` to the states and/or groups you would
 like to have access.
 
 
 ## Updating
 
-To update your existing installation of AA Time Zones first enable your virtual environment.
+To update your existing installation of AA Time Zones, first enable your virtual
+environment.
 
-Then run the following commands from your AA project directory (the one that contains `manage.py`).
+Then run the following commands from your AA project directory (the one that
+contains `manage.py`).
 
-```bash
+```shell
 pip install -U aa-esi-status
 ```
 
-```bash
+```shell
 python manage.py collectstatic
 ```
 
-```bash
+```shell
 python manage.py migrate
 ```
 
 Now restart your AA supervisor services.
```

### Comparing `aa_esi_status-1.8.0/aa_esi_status.egg-info/PKG-INFO` & `aa_esi_status-1.9.0/aa_esi_status.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-esi-status
-Version: 1.8.0
+Version: 1.9.0
 Summary: A simple status monitor for ESI
 Home-page: https://github.com/ppfeufer/aa-esi-status
 Author: Peter Pfeufer
 Author-email: develop@ppfeufer.de
 Maintainer: Peter Pfeufer
 Maintainer-email: develop@ppfeufer.de
 License: GPL-3.0
@@ -44,76 +44,83 @@
 
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/N4N8CL1BY)
 
 App for Alliance Auth to show the current status of ESI and its end points.
 
 ![AA ESI Status](https://raw.githubusercontent.com/ppfeufer/aa-esi-status/main/esistatus/docs/aa-esi-status.jpg)
 
-## Contents
 
-- [Installation](#installation)
-- [Updating](#updating)
-- [Change Log](CHANGELOG.md)
+<!-- TOC -->
+* [AA ESI Status](#aa-esi-status)
+  * [Installation](#installation)
+    * [Step 1: Install the app](#step-1-install-the-app)
+    * [Step 2: Update your AA settings](#step-2-update-your-aa-settings)
+    * [Step 3: Finalizing the installation](#step-3-finalizing-the-installation)
+    * [Step 4: Setting up permissions](#step-4-setting-up-permissions)
+  * [Updating](#updating)
+<!-- TOC -->
 
 
 ## Installation
 
 **Important**: This app is a plugin for Alliance Auth. If you don't have
 Alliance Auth running already, please install it first before proceeding.
-(see the official [AA installation guide](https://allianceauth.readthedocs.io/en/latest/installation/allianceauth.html) for details)
+(See the official [AA installation guide](https://allianceauth.readthedocs.io/en/latest/installation/allianceauth.html) for details)
 
 
-### Step 1 - Install app
+### Step 1: Install the app
 
-Make sure you are in the virtual environment (venv) of your Alliance Auth installation.
+Make sure you're in the virtual environment (venv) of your Alliance Auth installation.
 Then install the latest version:
 
-```bash
+```shell
 pip install aa-esi-status
 ```
 
 
-### Step 2 - Update your AA settings
+### Step 2: Update your AA settings
 
 Configure your AA settings (`local.py`) as follows:
 
 - Add `'esistatus',` to `INSTALLED_APPS`
 
 
-### Step 3 - Finalize the installation
+### Step 3: Finalizing the installation
 
 Run migrations & copy static files
 
-```bash
+```shell
 python manage.py collectstatic
 python manage.py migrate
 ```
 
 Restart your supervisor services for AA
 
 
-### Step 4 - Setup permissions
+### Step 4: Setting up permissions
 
-Now you can setup permissions in Alliance Auth for your users.
-Add ``esistatus|esi status|Can access ths app`` to the states and/or groups you would
+Now you can set up permissions in Alliance Auth for your users.
+Add `esistatus|esi status|Can access this app` to the states and/or groups you would
 like to have access.
 
 
 ## Updating
 
-To update your existing installation of AA Time Zones first enable your virtual environment.
+To update your existing installation of AA Time Zones, first enable your virtual
+environment.
 
-Then run the following commands from your AA project directory (the one that contains `manage.py`).
+Then run the following commands from your AA project directory (the one that
+contains `manage.py`).
 
-```bash
+```shell
 pip install -U aa-esi-status
 ```
 
-```bash
+```shell
 python manage.py collectstatic
 ```
 
-```bash
+```shell
 python manage.py migrate
 ```
 
 Now restart your AA supervisor services.
```

### Comparing `aa_esi_status-1.8.0/aa_esi_status.egg-info/SOURCES.txt` & `aa_esi_status-1.9.0/aa_esi_status.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 esistatus/locale/de/LC_MESSAGES/django.mo
 esistatus/locale/de/LC_MESSAGES/django.po
 esistatus/locale/es/LC_MESSAGES/django.po
 esistatus/locale/fr_FR/LC_MESSAGES/django.po
 esistatus/locale/it_IT/LC_MESSAGES/django.po
 esistatus/locale/ja/LC_MESSAGES/django.po
 esistatus/locale/ko_KR/LC_MESSAGES/django.po
+esistatus/locale/ru/LC_MESSAGES/django.mo
 esistatus/locale/ru/LC_MESSAGES/django.po
 esistatus/locale/zh_Hans/LC_MESSAGES/django.po
 esistatus/migrations/0001_initial.py
 esistatus/migrations/__init__.py
 esistatus/static/esistatus/css/esistatus.css
 esistatus/static/esistatus/css/esistatus.min.css
 esistatus/templates/esistatus/base.html
```

### Comparing `aa_esi_status-1.8.0/esistatus/auth_hooks.py` & `aa_esi_status-1.9.0/esistatus/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_esi_status-1.8.0/esistatus/docs/aa-esi-status.jpg` & `aa_esi_status-1.9.0/esistatus/docs/aa-esi-status.jpg`

 * *Files identical despite different names*

### Comparing `aa_esi_status-1.8.0/esistatus/locale/de/LC_MESSAGES/django.mo` & `aa_esi_status-1.9.0/esistatus/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_esi_status-1.8.0/esistatus/locale/de/LC_MESSAGES/django.po` & `aa_esi_status-1.9.0/esistatus/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_esi_status-1.8.0/esistatus/locale/es/LC_MESSAGES/django.po` & `aa_esi_status-1.9.0/esistatus/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_esi_status-1.8.0/esistatus/locale/fr_FR/LC_MESSAGES/django.po` & `aa_esi_status-1.9.0/esistatus/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_esi_status-1.8.0/esistatus/locale/it_IT/LC_MESSAGES/django.po` & `aa_esi_status-1.9.0/esistatus/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_esi_status-1.8.0/esistatus/locale/ja/LC_MESSAGES/django.po` & `aa_esi_status-1.9.0/esistatus/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_esi_status-1.8.0/esistatus/locale/ko_KR/LC_MESSAGES/django.po` & `aa_esi_status-1.9.0/esistatus/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_esi_status-1.8.0/esistatus/locale/ru/LC_MESSAGES/django.po` & `aa_esi_status-1.9.0/esistatus/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 26% similar despite different names*

```diff
@@ -12,17 +12,15 @@
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
-"(n%100>=11 && n%100<=14)? 2 : 3);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: templates/esistatus/base.html:5 templates/esistatus/base.html:9
 msgid "ESI Status"
 msgstr ""
 
 #: templates/esistatus/index.html:9
 msgid "Red Endpoints"
```

### Comparing `aa_esi_status-1.8.0/esistatus/migrations/0001_initial.py` & `aa_esi_status-1.9.0/esistatus/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_esi_status-1.8.0/esistatus/templates/esistatus/index.html` & `aa_esi_status-1.9.0/esistatus/templates/esistatus/index.html`

 * *Files identical despite different names*

### Comparing `aa_esi_status-1.8.0/esistatus/templates/esistatus/partials/endpoints.html` & `aa_esi_status-1.9.0/esistatus/templates/esistatus/partials/endpoints.html`

 * *Files identical despite different names*

### Comparing `aa_esi_status-1.8.0/esistatus/templatetags/esistatus_versioned_static.py` & `aa_esi_status-1.9.0/esistatus/templatetags/esistatus_versioned_static.py`

 * *Files identical despite different names*

### Comparing `aa_esi_status-1.8.0/esistatus/tests/test_access.py` & `aa_esi_status-1.9.0/esistatus/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `aa_esi_status-1.8.0/esistatus/tests/test_auth_hooks.py` & `aa_esi_status-1.9.0/esistatus/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_esi_status-1.8.0/esistatus/tests/test_templatetags.py` & `aa_esi_status-1.9.0/esistatus/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_esi_status-1.8.0/esistatus/tests/utils.py` & `aa_esi_status-1.9.0/esistatus/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_esi_status-1.8.0/esistatus/views.py` & `aa_esi_status-1.9.0/esistatus/views.py`

 * *Files identical despite different names*

### Comparing `aa_esi_status-1.8.0/setup.cfg` & `aa_esi_status-1.9.0/setup.cfg`

 * *Files identical despite different names*

