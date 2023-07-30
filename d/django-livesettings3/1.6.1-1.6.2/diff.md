# Comparing `tmp/django-livesettings3-1.6.1.tar.gz` & `tmp/django-livesettings3-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-livesettings3-1.6.1.tar", last modified: Thu Jul 20 01:18:06 2023, max compression
+gzip compressed data, was "django-livesettings3-1.6.2.tar", last modified: Sun Jul 30 00:57:25 2023, max compression
```

## Comparing `django-livesettings3-1.6.1.tar` & `django-livesettings3-1.6.2.tar`

### file list

```diff
@@ -1,89 +1,133 @@
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.893473 django-livesettings3-1.6.1/
--rw-r--r--   0 evgeny     (501) staff       (20)       88 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/AUTHORS
--rw-r--r--   0 evgeny     (501) staff       (20)     1498 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/LICENSE
--rw-r--r--   0 evgeny     (501) staff       (20)       93 2023-07-20 01:14:43.000000 django-livesettings3-1.6.1/MANIFEST.in
--rw-r--r--   0 evgeny     (501) staff       (20)     1000 2023-07-20 01:18:06.893626 django-livesettings3-1.6.1/PKG-INFO
--rw-r--r--   0 evgeny     (501) staff       (20)     5906 2023-07-19 23:59:41.000000 django-livesettings3-1.6.1/README.md
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.865051 django-livesettings3-1.6.1/django_livesettings3.egg-info/
--rw-r--r--   0 evgeny     (501) staff       (20)     1000 2023-07-20 01:18:06.000000 django-livesettings3-1.6.1/django_livesettings3.egg-info/PKG-INFO
--rw-r--r--   0 evgeny     (501) staff       (20)     2047 2023-07-20 01:18:06.000000 django-livesettings3-1.6.1/django_livesettings3.egg-info/SOURCES.txt
--rw-r--r--   0 evgeny     (501) staff       (20)        1 2023-07-20 01:18:06.000000 django-livesettings3-1.6.1/django_livesettings3.egg-info/dependency_links.txt
--rw-r--r--   0 evgeny     (501) staff       (20)       34 2023-07-20 01:18:06.000000 django-livesettings3-1.6.1/django_livesettings3.egg-info/requires.txt
--rw-r--r--   0 evgeny     (501) staff       (20)       13 2023-07-20 01:18:06.000000 django-livesettings3-1.6.1/django_livesettings3.egg-info/top_level.txt
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.873976 django-livesettings3-1.6.1/livesettings/
--rw-r--r--   0 evgeny     (501) staff       (20)      394 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/__init__.py
--rw-r--r--   0 evgeny     (501) staff       (20)     1922 2023-07-14 19:51:10.000000 django-livesettings3-1.6.1/livesettings/forms.py
--rw-r--r--   0 evgeny     (501) staff       (20)     7684 2023-07-14 19:51:10.000000 django-livesettings3-1.6.1/livesettings/functions.py
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.859092 django-livesettings3-1.6.1/livesettings/locale/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.854882 django-livesettings3-1.6.1/livesettings/locale/de/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.874972 django-livesettings3-1.6.1/livesettings/locale/de/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)      706 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 evgeny     (501) staff       (20)     2982 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.855238 django-livesettings3-1.6.1/livesettings/locale/en/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.876140 django-livesettings3-1.6.1/livesettings/locale/en/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)      367 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 evgeny     (501) staff       (20)     2878 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.855588 django-livesettings3-1.6.1/livesettings/locale/es/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.876586 django-livesettings3-1.6.1/livesettings/locale/es/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)        0 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.855936 django-livesettings3-1.6.1/livesettings/locale/fr/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.877364 django-livesettings3-1.6.1/livesettings/locale/fr/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)     1621 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 evgeny     (501) staff       (20)     3618 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.856382 django-livesettings3-1.6.1/livesettings/locale/he/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.878250 django-livesettings3-1.6.1/livesettings/locale/he/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)     1655 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/he/LC_MESSAGES/django.mo
--rw-r--r--   0 evgeny     (501) staff       (20)     2837 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/he/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.856786 django-livesettings3-1.6.1/livesettings/locale/it/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.879166 django-livesettings3-1.6.1/livesettings/locale/it/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)     1582 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 evgeny     (501) staff       (20)     3117 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.857232 django-livesettings3-1.6.1/livesettings/locale/ko/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.880015 django-livesettings3-1.6.1/livesettings/locale/ko/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)     1128 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/ko/LC_MESSAGES/django.mo
--rw-r--r--   0 evgeny     (501) staff       (20)     3110 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/ko/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.857629 django-livesettings3-1.6.1/livesettings/locale/pl/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.881208 django-livesettings3-1.6.1/livesettings/locale/pl/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)     1470 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 evgeny     (501) staff       (20)     2637 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.858003 django-livesettings3-1.6.1/livesettings/locale/pt_BR/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.882661 django-livesettings3-1.6.1/livesettings/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)     1208 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 evgeny     (501) staff       (20)     2645 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.858373 django-livesettings3-1.6.1/livesettings/locale/ru/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.884125 django-livesettings3-1.6.1/livesettings/locale/ru/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)     1178 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 evgeny     (501) staff       (20)     2470 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.858743 django-livesettings3-1.6.1/livesettings/locale/sv/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.885533 django-livesettings3-1.6.1/livesettings/locale/sv/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)     1481 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0 evgeny     (501) staff       (20)     2598 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.859254 django-livesettings3-1.6.1/livesettings/locale/tr/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.886945 django-livesettings3-1.6.1/livesettings/locale/tr/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)     1242 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 evgeny     (501) staff       (20)     3243 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.888294 django-livesettings3-1.6.1/livesettings/migrations/
--rw-r--r--   0 evgeny     (501) staff       (20)     1684 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/migrations/0001_initial.py
--rw-r--r--   0 evgeny     (501) staff       (20)        0 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/migrations/__init__.py
--rw-r--r--   0 evgeny     (501) staff       (20)     7142 2023-07-14 19:51:10.000000 django-livesettings3-1.6.1/livesettings/models.py
--rw-r--r--   0 evgeny     (501) staff       (20)     1846 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/overrides.py
--rw-r--r--   0 evgeny     (501) staff       (20)       79 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/signals.py
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.859873 django-livesettings3-1.6.1/livesettings/templates/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.892094 django-livesettings3-1.6.1/livesettings/templates/livesettings/
--rw-r--r--   0 evgeny     (501) staff       (20)      437 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/templates/livesettings/_admin_site_views.html
--rw-r--r--   0 evgeny     (501) staff       (20)     4781 2023-07-19 23:59:41.000000 django-livesettings3-1.6.1/livesettings/templates/livesettings/group_settings.html
--rw-r--r--   0 evgeny     (501) staff       (20)      878 2023-07-17 19:18:52.000000 django-livesettings3-1.6.1/livesettings/templates/livesettings/groups_navbar.html
--rw-r--r--   0 evgeny     (501) staff       (20)     6159 2023-07-16 21:37:36.000000 django-livesettings3-1.6.1/livesettings/templates/livesettings/site_settings.html
--rw-r--r--   0 evgeny     (501) staff       (20)       41 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/templates/livesettings/text.txt
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-20 01:18:06.893022 django-livesettings3-1.6.1/livesettings/templatetags/
--rw-r--r--   0 evgeny     (501) staff       (20)        0 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/templatetags/__init__.py
--rw-r--r--   0 evgeny     (501) staff       (20)     2142 2023-07-14 19:51:10.000000 django-livesettings3-1.6.1/livesettings/templatetags/config_tags.py
--rw-r--r--   0 evgeny     (501) staff       (20)      447 2023-07-16 19:44:06.000000 django-livesettings3-1.6.1/livesettings/test_urls.py
--rw-r--r--   0 evgeny     (501) staff       (20)    29460 2023-07-17 19:11:51.000000 django-livesettings3-1.6.1/livesettings/tests.py
--rw-r--r--   0 evgeny     (501) staff       (20)      392 2023-07-15 19:16:27.000000 django-livesettings3-1.6.1/livesettings/urls.py
--rw-r--r--   0 evgeny     (501) staff       (20)     2131 2022-02-10 21:13:39.000000 django-livesettings3-1.6.1/livesettings/utils.py
--rw-r--r--   0 evgeny     (501) staff       (20)    33758 2023-07-19 23:59:41.000000 django-livesettings3-1.6.1/livesettings/values.py
--rw-r--r--   0 evgeny     (501) staff       (20)     4706 2023-07-17 19:19:33.000000 django-livesettings3-1.6.1/livesettings/views.py
--rw-r--r--   0 evgeny     (501) staff       (20)     1135 2023-07-19 23:59:41.000000 django-livesettings3-1.6.1/livesettings/widgets.py
--rw-r--r--   0 evgeny     (501) staff       (20)       79 2023-07-20 01:18:06.894150 django-livesettings3-1.6.1/setup.cfg
--rw-r--r--   0 evgeny     (501) staff       (20)     1277 2023-07-20 01:16:11.000000 django-livesettings3-1.6.1/setup.py
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.483907 django-livesettings3-1.6.2/
+-rw-r--r--   0 evgeny     (501) staff       (20)       88 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/AUTHORS
+-rw-r--r--   0 evgeny     (501) staff       (20)     1498 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/LICENSE
+-rw-r--r--   0 evgeny     (501) staff       (20)       93 2023-07-30 00:53:02.000000 django-livesettings3-1.6.2/MANIFEST.in
+-rw-r--r--   0 evgeny     (501) staff       (20)     1000 2023-07-30 00:57:25.484062 django-livesettings3-1.6.2/PKG-INFO
+-rw-r--r--   0 evgeny     (501) staff       (20)     5910 2023-07-30 00:52:14.000000 django-livesettings3-1.6.2/README.md
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.444952 django-livesettings3-1.6.2/django_livesettings3.egg-info/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1000 2023-07-30 00:57:25.000000 django-livesettings3-1.6.2/django_livesettings3.egg-info/PKG-INFO
+-rw-r--r--   0 evgeny     (501) staff       (20)     3588 2023-07-30 00:57:25.000000 django-livesettings3-1.6.2/django_livesettings3.egg-info/SOURCES.txt
+-rw-r--r--   0 evgeny     (501) staff       (20)        1 2023-07-30 00:57:25.000000 django-livesettings3-1.6.2/django_livesettings3.egg-info/dependency_links.txt
+-rw-r--r--   0 evgeny     (501) staff       (20)        1 2023-07-24 21:10:38.000000 django-livesettings3-1.6.2/django_livesettings3.egg-info/not-zip-safe
+-rw-r--r--   0 evgeny     (501) staff       (20)       34 2023-07-30 00:57:25.000000 django-livesettings3-1.6.2/django_livesettings3.egg-info/requires.txt
+-rw-r--r--   0 evgeny     (501) staff       (20)       13 2023-07-30 00:57:25.000000 django-livesettings3-1.6.2/django_livesettings3.egg-info/top_level.txt
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.454913 django-livesettings3-1.6.2/livesettings/
+-rw-r--r--   0 evgeny     (501) staff       (20)      394 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/__init__.py
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.460634 django-livesettings3-1.6.2/livesettings/__pycache__/
+-rw-r--r--   0 evgeny     (501) staff       (20)      565 2023-07-21 17:27:35.000000 django-livesettings3-1.6.2/livesettings/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 evgeny     (501) staff       (20)     1898 2023-07-30 00:55:57.000000 django-livesettings3-1.6.2/livesettings/__pycache__/forms.cpython-39.pyc
+-rw-r--r--   0 evgeny     (501) staff       (20)     8564 2023-07-21 17:27:35.000000 django-livesettings3-1.6.2/livesettings/__pycache__/functions.cpython-39.pyc
+-rw-r--r--   0 evgeny     (501) staff       (20)     7610 2023-07-21 17:27:35.000000 django-livesettings3-1.6.2/livesettings/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0 evgeny     (501) staff       (20)     1922 2023-07-21 17:27:35.000000 django-livesettings3-1.6.2/livesettings/__pycache__/overrides.cpython-39.pyc
+-rw-r--r--   0 evgeny     (501) staff       (20)      256 2023-07-21 17:27:35.000000 django-livesettings3-1.6.2/livesettings/__pycache__/signals.cpython-39.pyc
+-rw-r--r--   0 evgeny     (501) staff       (20)      639 2023-07-30 00:55:59.000000 django-livesettings3-1.6.2/livesettings/__pycache__/test_urls.cpython-39.pyc
+-rw-r--r--   0 evgeny     (501) staff       (20)    28533 2023-07-30 00:55:58.000000 django-livesettings3-1.6.2/livesettings/__pycache__/tests.cpython-39.pyc
+-rw-r--r--   0 evgeny     (501) staff       (20)      549 2023-07-30 00:55:58.000000 django-livesettings3-1.6.2/livesettings/__pycache__/urls.cpython-39.pyc
+-rw-r--r--   0 evgeny     (501) staff       (20)     2557 2023-07-21 17:27:35.000000 django-livesettings3-1.6.2/livesettings/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0 evgeny     (501) staff       (20)    36310 2023-07-30 00:55:57.000000 django-livesettings3-1.6.2/livesettings/__pycache__/values.cpython-39.pyc
+-rw-r--r--   0 evgeny     (501) staff       (20)     3341 2023-07-30 00:55:58.000000 django-livesettings3-1.6.2/livesettings/__pycache__/views.cpython-39.pyc
+-rw-r--r--   0 evgeny     (501) staff       (20)     2359 2023-07-30 00:55:57.000000 django-livesettings3-1.6.2/livesettings/__pycache__/widgets.cpython-39.pyc
+-rw-r--r--   0 evgeny     (501) staff       (20)     1994 2023-07-30 00:52:20.000000 django-livesettings3-1.6.2/livesettings/forms.py
+-rw-r--r--   0 evgeny     (501) staff       (20)     7684 2023-07-14 19:51:10.000000 django-livesettings3-1.6.2/livesettings/functions.py
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.431501 django-livesettings3-1.6.2/livesettings/locale/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.427502 django-livesettings3-1.6.2/livesettings/locale/de/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.462057 django-livesettings3-1.6.2/livesettings/locale/de/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)      706 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 evgeny     (501) staff       (20)     2982 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.427848 django-livesettings3-1.6.2/livesettings/locale/en/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.463213 django-livesettings3-1.6.2/livesettings/locale/en/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)      367 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 evgeny     (501) staff       (20)     2878 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.428189 django-livesettings3-1.6.2/livesettings/locale/es/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.463745 django-livesettings3-1.6.2/livesettings/locale/es/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)        0 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.428532 django-livesettings3-1.6.2/livesettings/locale/fr/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.464662 django-livesettings3-1.6.2/livesettings/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1621 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 evgeny     (501) staff       (20)     3618 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.428878 django-livesettings3-1.6.2/livesettings/locale/he/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.465756 django-livesettings3-1.6.2/livesettings/locale/he/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1655 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/he/LC_MESSAGES/django.mo
+-rw-r--r--   0 evgeny     (501) staff       (20)     2837 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/he/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.429187 django-livesettings3-1.6.2/livesettings/locale/it/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.466984 django-livesettings3-1.6.2/livesettings/locale/it/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1582 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 evgeny     (501) staff       (20)     3117 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.429534 django-livesettings3-1.6.2/livesettings/locale/ko/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.468167 django-livesettings3-1.6.2/livesettings/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1128 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/ko/LC_MESSAGES/django.mo
+-rw-r--r--   0 evgeny     (501) staff       (20)     3110 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/ko/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.429927 django-livesettings3-1.6.2/livesettings/locale/pl/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.469210 django-livesettings3-1.6.2/livesettings/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1470 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 evgeny     (501) staff       (20)     2637 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.430259 django-livesettings3-1.6.2/livesettings/locale/pt_BR/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.470345 django-livesettings3-1.6.2/livesettings/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1208 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 evgeny     (501) staff       (20)     2645 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.430734 django-livesettings3-1.6.2/livesettings/locale/ru/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.471427 django-livesettings3-1.6.2/livesettings/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1178 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 evgeny     (501) staff       (20)     2470 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.431227 django-livesettings3-1.6.2/livesettings/locale/sv/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.472530 django-livesettings3-1.6.2/livesettings/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1481 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0 evgeny     (501) staff       (20)     2598 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.431676 django-livesettings3-1.6.2/livesettings/locale/tr/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.473571 django-livesettings3-1.6.2/livesettings/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1242 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 evgeny     (501) staff       (20)     3243 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.474562 django-livesettings3-1.6.2/livesettings/migrations/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1684 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/migrations/0001_initial.py
+-rw-r--r--   0 evgeny     (501) staff       (20)        0 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/migrations/__init__.py
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.475335 django-livesettings3-1.6.2/livesettings/migrations/__pycache__/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1225 2023-07-21 17:28:00.000000 django-livesettings3-1.6.2/livesettings/migrations/__pycache__/0001_initial.cpython-39.pyc
+-rw-r--r--   0 evgeny     (501) staff       (20)      174 2023-07-21 17:28:00.000000 django-livesettings3-1.6.2/livesettings/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 evgeny     (501) staff       (20)     7142 2023-07-14 19:51:10.000000 django-livesettings3-1.6.2/livesettings/models.py
+-rw-r--r--   0 evgeny     (501) staff       (20)     1846 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/overrides.py
+-rw-r--r--   0 evgeny     (501) staff       (20)       79 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/signals.py
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.432833 django-livesettings3-1.6.2/livesettings/static/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.433050 django-livesettings3-1.6.2/livesettings/static/livesettings/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.475758 django-livesettings3-1.6.2/livesettings/static/livesettings/js/
+-rw-r--r--   0 evgeny     (501) staff       (20)    36012 2023-07-30 00:52:20.000000 django-livesettings3-1.6.2/livesettings/static/livesettings/js/string_array_widget.js
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.476683 django-livesettings3-1.6.2/livesettings/svelte/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.477655 django-livesettings3-1.6.2/livesettings/svelte/StringArrayWidget/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1857 2023-07-30 00:52:20.000000 django-livesettings3-1.6.2/livesettings/svelte/StringArrayWidget/StringArrayItem.svelte
+-rw-r--r--   0 evgeny     (501) staff       (20)     3407 2023-07-30 00:52:20.000000 django-livesettings3-1.6.2/livesettings/svelte/StringArrayWidget/index.svelte
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.478078 django-livesettings3-1.6.2/livesettings/svelte/components/
+-rw-r--r--   0 evgeny     (501) staff       (20)      379 2023-07-30 00:52:20.000000 django-livesettings3-1.6.2/livesettings/svelte/components/Dots.svelte
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.478874 django-livesettings3-1.6.2/livesettings/svelte/icons/
+-rw-r--r--   0 evgeny     (501) staff       (20)      419 2023-07-30 00:52:20.000000 django-livesettings3-1.6.2/livesettings/svelte/icons/Cross.svelte
+-rw-r--r--   0 evgeny     (501) staff       (20)      670 2023-07-30 00:52:20.000000 django-livesettings3-1.6.2/livesettings/svelte/icons/DragHandleDots.svelte
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.479328 django-livesettings3-1.6.2/livesettings/svelte/lib/
+-rw-r--r--   0 evgeny     (501) staff       (20)       47 2023-07-30 00:52:20.000000 django-livesettings3-1.6.2/livesettings/svelte/lib/actions.js
+-rw-r--r--   0 evgeny     (501) staff       (20)      393 2023-07-30 00:52:20.000000 django-livesettings3-1.6.2/livesettings/svelte/package.json
+-rw-r--r--   0 evgeny     (501) staff       (20)      562 2023-07-30 00:52:20.000000 django-livesettings3-1.6.2/livesettings/svelte/rollup.config.mjs
+-rw-r--r--   0 evgeny     (501) staff       (20)    21536 2023-07-30 00:52:20.000000 django-livesettings3-1.6.2/livesettings/svelte/yarn.lock
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.437808 django-livesettings3-1.6.2/livesettings/templates/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.481913 django-livesettings3-1.6.2/livesettings/templates/livesettings/
+-rw-r--r--   0 evgeny     (501) staff       (20)      437 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/templates/livesettings/_admin_site_views.html
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.482241 django-livesettings3-1.6.2/livesettings/templates/livesettings/form_widgets/
+-rw-r--r--   0 evgeny     (501) staff       (20)      636 2023-07-30 00:52:20.000000 django-livesettings3-1.6.2/livesettings/templates/livesettings/form_widgets/string_array_widget.html
+-rw-r--r--   0 evgeny     (501) staff       (20)     4901 2023-07-30 00:52:20.000000 django-livesettings3-1.6.2/livesettings/templates/livesettings/group_settings.html
+-rw-r--r--   0 evgeny     (501) staff       (20)     3154 2023-07-20 23:55:47.000000 django-livesettings3-1.6.2/livesettings/templates/livesettings/group_settings.html.orig
+-rw-r--r--   0 evgeny     (501) staff       (20)      878 2023-07-30 00:52:14.000000 django-livesettings3-1.6.2/livesettings/templates/livesettings/groups_navbar.html
+-rw-r--r--   0 evgeny     (501) staff       (20)     6925 2023-07-30 00:52:20.000000 django-livesettings3-1.6.2/livesettings/templates/livesettings/site_settings.html
+-rw-r--r--   0 evgeny     (501) staff       (20)       41 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/templates/livesettings/text.txt
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.482747 django-livesettings3-1.6.2/livesettings/templatetags/
+-rw-r--r--   0 evgeny     (501) staff       (20)        0 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/templatetags/__init__.py
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.483595 django-livesettings3-1.6.2/livesettings/templatetags/__pycache__/
+-rw-r--r--   0 evgeny     (501) staff       (20)      176 2023-07-21 17:28:00.000000 django-livesettings3-1.6.2/livesettings/templatetags/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 evgeny     (501) staff       (20)     2098 2023-07-21 17:28:00.000000 django-livesettings3-1.6.2/livesettings/templatetags/__pycache__/config_tags.cpython-39.pyc
+-rw-r--r--   0 evgeny     (501) staff       (20)     2142 2023-07-14 19:51:10.000000 django-livesettings3-1.6.2/livesettings/templatetags/config_tags.py
+-rw-r--r--   0 evgeny     (501) staff       (20)      447 2023-07-30 00:52:14.000000 django-livesettings3-1.6.2/livesettings/test_urls.py
+-rw-r--r--   0 evgeny     (501) staff       (20)    29460 2023-07-30 00:52:14.000000 django-livesettings3-1.6.2/livesettings/tests.py
+-rw-r--r--   0 evgeny     (501) staff       (20)      392 2023-07-30 00:52:14.000000 django-livesettings3-1.6.2/livesettings/urls.py
+-rw-r--r--   0 evgeny     (501) staff       (20)     2131 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/utils.py
+-rw-r--r--   0 evgeny     (501) staff       (20)    35615 2023-07-30 00:52:20.000000 django-livesettings3-1.6.2/livesettings/values.py
+-rw-r--r--   0 evgeny     (501) staff       (20)    33758 2023-07-19 23:59:41.000000 django-livesettings3-1.6.2/livesettings/values.py.orig
+-rw-r--r--   0 evgeny     (501) staff       (20)     4706 2023-07-30 00:52:14.000000 django-livesettings3-1.6.2/livesettings/views.py
+-rw-r--r--   0 evgeny     (501) staff       (20)     1782 2023-07-30 00:52:20.000000 django-livesettings3-1.6.2/livesettings/widgets.py
+-rw-r--r--   0 evgeny     (501) staff       (20)     1135 2023-07-19 23:59:41.000000 django-livesettings3-1.6.2/livesettings/widgets.py.orig
+-rw-r--r--   0 evgeny     (501) staff       (20)       79 2023-07-30 00:57:25.484519 django-livesettings3-1.6.2/setup.cfg
+-rw-r--r--   0 evgeny     (501) staff       (20)     1297 2023-07-30 00:53:29.000000 django-livesettings3-1.6.2/setup.py
```

### Comparing `django-livesettings3-1.6.1/LICENSE` & `django-livesettings3-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.1/PKG-INFO` & `django-livesettings3-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-livesettings3
-Version: 1.6.1
+Version: 1.6.2
 Summary: Python 3 port of django-livesettings
 Home-page: https://github.com/kunaldeo/django-livesettings3/
 Author: Kunal Deo
 Author-email: kunaldeo@gmail.com
 License: New BSD License
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-livesettings3-1.6.1/README.md` & `django-livesettings3-1.6.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 django-livesettings3
 =====
 [![Build Status](https://travis-ci.org/kunaldeo/django-livesettings3.svg?branch=master)](https://travis-ci.org/kunaldeo/django-livesettings3) [![PyPI version](https://badge.fury.io/py/django-livesettings3.svg)](https://badge.fury.io/py/django-livesettings3) [![codecov.io](https://codecov.io/github/kunaldeo/django-livesettings3/coverage.svg?branch=master)](https://codecov.io/github/kunaldeo/django-livesettings3?branch=master)
 
-This is a Python 3 Port of django-livesettings that has been tested with Python 3.6.X and Django 2.X.
+This is a Python 3 Port of django-livesettings that has been tested with Python 3.X and Django up to 4.X.
 
 **django-livesettings3** provides the ability to configure settings via an admin interface, rather than by editing settings.py. In addition, livesettings allows you to set sane defaults so that your site can be perfectly functional without any changes. Livesettings uses caching to make sure this has minimal impact on your site’s performance. Finally, if you wish to lock down your site and disable the settings, you can export your livesettings and store them in your settings.py. This allows you have flexibility in deciding how various users interact with your app.
 
 ## Requirements
 - Python 3.6+
 - Django 1.8+
 - [django-keyedcache3](https://github.com/kunaldeo/django-keyedcache3)
```

### Comparing `django-livesettings3-1.6.1/django_livesettings3.egg-info/PKG-INFO` & `django-livesettings3-1.6.2/django_livesettings3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-livesettings3
-Version: 1.6.1
+Version: 1.6.2
 Summary: Python 3 port of django-livesettings
 Home-page: https://github.com/kunaldeo/django-livesettings3/
 Author: Kunal Deo
 Author-email: kunaldeo@gmail.com
 License: New BSD License
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-livesettings3-1.6.1/livesettings/forms.py` & `django-livesettings3-1.6.2/livesettings/forms.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,15 +41,17 @@
         self.groups = groups
 
 
 class LocalizedChoiceField(forms.ChoiceField):
     def __init__(self, *args, **kwargs):
         #self.language_code = kwargs.pop('language_code',
         #                                django_settings.LANGUAGE_CODE)
+        kwargs.pop('default', None)
         super(LocalizedChoiceField, self).__init__(*args, **kwargs)
 
 
 class LocalizedMultipleChoiceField(forms.MultipleChoiceField):
     def __init__(self, *args, **kwargs):
         #self.language_code = kwargs.pop('language_code',
         #                                django_settings.LANGUAGE_CODE)
+        kwargs.pop('default', None)
         super(LocalizedMultipleChoiceField, self).__init__(*args, **kwargs)
```

### Comparing `django-livesettings3-1.6.1/livesettings/functions.py` & `django-livesettings3-1.6.2/livesettings/functions.py`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.1/livesettings/locale/de/LC_MESSAGES/django.mo` & `django-livesettings3-1.6.2/livesettings/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.1/livesettings/locale/de/LC_MESSAGES/django.po` & `django-livesettings3-1.6.2/livesettings/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.1/livesettings/locale/en/LC_MESSAGES/django.po` & `django-livesettings3-1.6.2/livesettings/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.1/livesettings/locale/fr/LC_MESSAGES/django.mo` & `django-livesettings3-1.6.2/livesettings/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.1/livesettings/locale/fr/LC_MESSAGES/django.po` & `django-livesettings3-1.6.2/livesettings/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.1/livesettings/locale/he/LC_MESSAGES/django.mo` & `django-livesettings3-1.6.2/livesettings/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.1/livesettings/locale/he/LC_MESSAGES/django.po` & `django-livesettings3-1.6.2/livesettings/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.1/livesettings/locale/it/LC_MESSAGES/django.mo` & `django-livesettings3-1.6.2/livesettings/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.1/livesettings/locale/it/LC_MESSAGES/django.po` & `django-livesettings3-1.6.2/livesettings/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.1/livesettings/locale/ko/LC_MESSAGES/django.mo` & `django-livesettings3-1.6.2/livesettings/locale/ko/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.1/livesettings/locale/ko/LC_MESSAGES/django.po` & `django-livesettings3-1.6.2/livesettings/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.1/livesettings/locale/pl/LC_MESSAGES/django.mo` & `django-livesettings3-1.6.2/livesettings/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.1/livesettings/locale/pl/LC_MESSAGES/django.po` & `django-livesettings3-1.6.2/livesettings/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.1/livesettings/locale/pt_BR/LC_MESSAGES/django.mo` & `django-livesettings3-1.6.2/livesettings/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.1/livesettings/locale/pt_BR/LC_MESSAGES/django.po` & `django-livesettings3-1.6.2/livesettings/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.1/livesettings/locale/ru/LC_MESSAGES/django.mo` & `django-livesettings3-1.6.2/livesettings/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.1/livesettings/locale/ru/LC_MESSAGES/django.po` & `django-livesettings3-1.6.2/livesettings/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.1/livesettings/locale/sv/LC_MESSAGES/django.mo` & `django-livesettings3-1.6.2/livesettings/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.1/livesettings/locale/sv/LC_MESSAGES/django.po` & `django-livesettings3-1.6.2/livesettings/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.1/livesettings/locale/tr/LC_MESSAGES/django.mo` & `django-livesettings3-1.6.2/livesettings/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.1/livesettings/locale/tr/LC_MESSAGES/django.po` & `django-livesettings3-1.6.2/livesettings/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.1/livesettings/migrations/0001_initial.py` & `django-livesettings3-1.6.2/livesettings/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.1/livesettings/models.py` & `django-livesettings3-1.6.2/livesettings/models.py`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.1/livesettings/overrides.py` & `django-livesettings3-1.6.2/livesettings/overrides.py`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.1/livesettings/templates/livesettings/group_settings.html` & `django-livesettings3-1.6.2/livesettings/templates/livesettings/group_settings.html`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,18 @@
         }
         #livesettings-values-column p.help:last-child {
             margin: 0;
         }
     </style>
 {% endblock %}
 
+{% block extrahead %}
+    <script src="{% static "livesettings/js/string_array_widget.js" %}"></script>
+{% endblock %}
+
 {% block coltype %}colMS{% endblock %}
 {% block bodyclass %}dashboard{% endblock %}
 
 {% block branding %}
 <h1 id="site-name"><a href="{% url 'satchmo_site_settings' %}">{{ site_header|default:_('Django administration') }}</a></h1>
 {% if user.is_anonymous %}
   {% include "admin/color_theme_toggle.html" %}
```

#### html2text {}

```diff
@@ -1,10 +1,12 @@
 {% extends "admin/base_site.html" %} {% load i18n config_tags %} {% load static
 %} {% block extrastyle %} {{ block.super }}
- {% endblock %} {% block coltype %}colMS{% endblock %} {% block bodyclass
+ {% endblock %} {% block extrahead %}
+s/string_array_widget.js" %}">
+{% endblock %} {% block coltype %}colMS{% endblock %} {% block bodyclass
 %}dashboard{% endblock %} {% block branding %}
 ****** {{_site_header|default:_('Django_administration')_}} ******
 {% if user.is_anonymous %} {% include "admin/color_theme_toggle.html" %} {%
 endif %} {% endblock %} {% block userlinks %}{%_trans_'Documentation'_%} / {%
 trans_'Change_password'_%} / {%_trans_'Log_out'_%}{% endblock %} {% block
 breadcrumbs %} {% if not is_popup %} {% if has_multiple_groups %}
 {%_trans_"Settings"_%} › {{ settings_group.super_group.name }} › {
```

### Comparing `django-livesettings3-1.6.1/livesettings/templates/livesettings/groups_navbar.html` & `django-livesettings3-1.6.2/livesettings/templates/livesettings/groups_navbar.html`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.1/livesettings/templates/livesettings/site_settings.html` & `django-livesettings3-1.6.2/livesettings/templates/livesettings/site_settings.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,385 +1,433 @@
 00000000: 7b25 2065 7874 656e 6473 2022 6164 6d69  {% extends "admi
 00000010: 6e2f 6261 7365 5f73 6974 652e 6874 6d6c  n/base_site.html
 00000020: 2220 257d 0a7b 2520 6c6f 6164 2069 3138  " %}.{% load i18
 00000030: 6e20 7374 6174 6963 2063 6f6e 6669 675f  n static config_
 00000040: 7461 6773 2025 7d0a 0a7b 2520 626c 6f63  tags %}..{% bloc
 00000050: 6b20 6578 7472 6168 6561 6420 257d 7b7b  k extrahead %}{{
 00000060: 2062 6c6f 636b 2e73 7570 6572 207d 7d0a   block.super }}.
-00000070: 2020 2020 3c73 6372 6970 7420 7479 7065      <script type
-00000080: 3d22 7465 7874 2f6a 6176 6173 6372 6970  ="text/javascrip
-00000090: 7422 2073 7263 3d22 7b25 2075 726c 2027  t" src="{% url '
-000000a0: 6164 6d69 6e3a 6a73 6931 386e 2720 257d  admin:jsi18n' %}
-000000b0: 223e 3c2f 7363 7269 7074 3e0a 2020 2020  "></script>.    
-000000c0: 3c73 6372 6970 7420 7479 7065 3d22 7465  <script type="te
-000000d0: 7874 2f6a 6176 6173 6372 6970 7422 2073  xt/javascript" s
-000000e0: 7263 3d22 7b25 2073 7461 7469 6320 2261  rc="{% static "a
-000000f0: 646d 696e 2f6a 732f 636f 7265 2e6a 7322  dmin/js/core.js"
-00000100: 2025 7d22 3e3c 2f73 6372 6970 743e 0a20   %}"></script>. 
-00000110: 2020 203c 7363 7269 7074 2074 7970 653d     <script type=
-00000120: 2274 6578 742f 6a61 7661 7363 7269 7074  "text/javascript
-00000130: 2220 7372 633d 227b 2520 7374 6174 6963  " src="{% static
-00000140: 2022 6164 6d69 6e2f 6a73 2f76 656e 646f   "admin/js/vendo
-00000150: 722f 6a71 7565 7279 2f6a 7175 6572 792e  r/jquery/jquery.
-00000160: 6d69 6e2e 6a73 2220 257d 223e 3c2f 7363  min.js" %}"></sc
-00000170: 7269 7074 3e0a 2020 2020 3c73 6372 6970  ript>.    <scrip
-00000180: 7420 7479 7065 3d22 7465 7874 2f6a 6176  t type="text/jav
-00000190: 6173 6372 6970 7422 2073 7263 3d22 7b25  ascript" src="{%
-000001a0: 2073 7461 7469 6320 2261 646d 696e 2f6a   static "admin/j
-000001b0: 732f 6a71 7565 7279 2e69 6e69 742e 6a73  s/jquery.init.js
-000001c0: 2220 257d 223e 3c2f 7363 7269 7074 3e0a  " %}"></script>.
-000001d0: 2020 2020 3c73 6372 6970 7420 7479 7065      <script type
-000001e0: 3d22 7465 7874 2f6a 6176 6173 6372 6970  ="text/javascrip
-000001f0: 7422 2073 7263 3d22 7b25 2073 7461 7469  t" src="{% stati
-00000200: 6320 2261 646d 696e 2f6a 732f 636f 6c6c  c "admin/js/coll
-00000210: 6170 7365 2e6a 7322 2025 7d22 3e3c 2f73  apse.js" %}"></s
-00000220: 6372 6970 743e 0a20 2020 203c 7363 7269  cript>.    <scri
-00000230: 7074 2074 7970 653d 2274 6578 742f 6a61  pt type="text/ja
-00000240: 7661 7363 7269 7074 223e 0a20 2020 2020  vascript">.     
-00000250: 2020 2076 6172 2024 203d 2064 6a61 6e67     var $ = djang
-00000260: 6f2e 6a51 7565 7279 2c0a 2020 2020 2020  o.jQuery,.      
-00000270: 2020 2020 2020 2020 2020 756e 636f 6c6c            uncoll
-00000280: 6170 7365 203d 2066 756e 6374 696f 6e20  apse = function 
-00000290: 2829 207b 0a20 2020 2020 2020 2020 2020  () {.           
-000002a0: 2020 2020 2020 2020 2024 2822 6669 656c           $("fiel
-000002b0: 6473 6574 2e63 6f6c 6c61 7073 6520 612e  dset.collapse a.
-000002c0: 636f 6c6c 6170 7365 2d74 6f67 676c 6522  collapse-toggle"
-000002d0: 292e 6561 6368 2866 756e 6374 696f 6e20  ).each(function 
-000002e0: 2829 207b 0a20 2020 2020 2020 2020 2020  () {.           
-000002f0: 2020 2020 2020 2020 2020 2020 2076 6172               var
-00000300: 2065 6c74 203d 2024 2874 6869 7329 3b0a   elt = $(this);.
-00000310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000320: 2020 2020 2020 2020 6966 2028 656c 742e          if (elt.
-00000330: 7465 7874 2829 203d 3d20 6765 7474 6578  text() == gettex
-00000340: 7428 2753 686f 7727 2929 207b 0a20 2020  t('Show')) {.   
-00000350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000360: 2020 2020 2020 2020 2065 6c74 2e63 6c69           elt.cli
-00000370: 636b 2829 3b0a 2020 2020 2020 2020 2020  ck();.          
-00000380: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
-00000390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000003a0: 2020 2020 7d29 3b0a 2020 2020 2020 2020      });.        
-000003b0: 2020 2020 2020 2020 2020 2020 2428 2766              $('f
-000003c0: 6965 6c64 7365 7427 292e 7265 6d6f 7665  ieldset').remove
-000003d0: 436c 6173 7328 2763 6f6c 6c61 7073 6564  Class('collapsed
-000003e0: 2729 3b0a 2020 2020 2020 2020 2020 2020  ');.            
-000003f0: 2020 2020 2020 2020 7265 7475 726e 2066          return f
-00000400: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
-00000410: 2020 2020 207d 3b0a 2020 2020 3c2f 7363       };.    </sc
-00000420: 7269 7074 3e0a 7b25 2065 6e64 626c 6f63  ript>.{% endbloc
-00000430: 6b20 257d 0a0a 7b25 2062 6c6f 636b 2065  k %}..{% block e
-00000440: 7874 7261 7374 796c 6520 257d 0a20 2020  xtrastyle %}.   
-00000450: 207b 7b20 626c 6f63 6b2e 7375 7065 7220   {{ block.super 
-00000460: 7d7d 0a20 2020 203c 6c69 6e6b 2072 656c  }}.    <link rel
-00000470: 3d22 7374 796c 6573 6865 6574 2220 7479  ="stylesheet" ty
-00000480: 7065 3d22 7465 7874 2f63 7373 2220 6872  pe="text/css" hr
-00000490: 6566 3d22 7b25 2073 7461 7469 6320 2261  ef="{% static "a
-000004a0: 646d 696e 2f63 7373 2f66 6f72 6d73 2e63  dmin/css/forms.c
-000004b0: 7373 2220 257d 222f 3e0a 2020 2020 3c73  ss" %}"/>.    <s
-000004c0: 7479 6c65 2074 7970 653d 2274 6578 742f  tyle type="text/
-000004d0: 6373 7322 3e0a 2020 2020 2020 2020 756c  css">.        ul
-000004e0: 2e66 6965 6c64 7265 6620 7b0a 2020 2020  .fieldref {.    
-000004f0: 2020 2020 2020 2020 6d61 7267 696e 3a20          margin: 
-00000500: 303b 0a20 2020 2020 2020 2020 2020 2070  0;.            p
-00000510: 6164 6469 6e67 3a20 303b 0a20 2020 2020  adding: 0;.     
-00000520: 2020 2020 2020 2066 6f6e 742d 7369 7a65         font-size
-00000530: 3a20 3970 783b 0a20 2020 2020 2020 207d  : 9px;.        }
-00000540: 0a0a 2020 2020 2020 2020 756c 2e66 6965  ..        ul.fie
-00000550: 6c64 7265 6620 6c69 207b 0a20 2020 2020  ldref li {.     
-00000560: 2020 2020 2020 2066 6c6f 6174 3a20 6c65         float: le
-00000570: 6674 3b0a 2020 2020 2020 2020 2020 2020  ft;.            
-00000580: 6d61 7267 696e 3a20 3020 3130 7078 2030  margin: 0 10px 0
-00000590: 2030 3b0a 2020 2020 2020 2020 2020 2020   0;.            
-000005a0: 6c69 7374 2d73 7479 6c65 3a20 6e6f 6e65  list-style: none
-000005b0: 3b0a 2020 2020 2020 2020 7d0a 0a20 2020  ;.        }..   
-000005c0: 2020 2020 2066 6965 6c64 7365 742e 636f       fieldset.co
-000005d0: 6c6c 6170 7365 6420 6832 207b 0a20 2020  llapsed h2 {.   
-000005e0: 2020 2020 2020 2020 2064 6973 706c 6179           display
-000005f0: 3a20 626c 6f63 6b20 2169 6d70 6f72 7461  : block !importa
-00000600: 6e74 3b0a 2020 2020 2020 2020 7d0a 0a20  nt;.        }.. 
-00000610: 2020 2020 2020 2066 6965 6c64 7365 742e         fieldset.
-00000620: 636f 6c6c 6170 7365 6420 6832 2061 207b  collapsed h2 a {
-00000630: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
-00000640: 706c 6179 3a20 696e 6c69 6e65 2021 696d  play: inline !im
-00000650: 706f 7274 616e 743b 0a20 2020 2020 2020  portant;.       
-00000660: 207d 0a0a 2020 2020 2020 2020 6469 762e   }..        div.
-00000670: 6669 656c 6463 6f6e 7461 696e 6572 207b  fieldcontainer {
-00000680: 0a20 2020 2020 2020 2020 2020 2066 6c6f  .            flo
-00000690: 6174 3a20 6c65 6674 3b0a 2020 2020 2020  at: left;.      
-000006a0: 2020 2020 2020 6d61 7267 696e 2d72 6967        margin-rig
-000006b0: 6874 3a20 303b 0a20 2020 2020 2020 207d  ht: 0;.        }
-000006c0: 0a20 2020 203c 2f73 7479 6c65 3e0a 7b25  .    </style>.{%
-000006d0: 2065 6e64 626c 6f63 6b20 257d 0a0a 7b25   endblock %}..{%
-000006e0: 2062 6c6f 636b 2063 6f6c 7479 7065 2025   block coltype %
-000006f0: 7d63 6f6c 4d53 7b25 2065 6e64 626c 6f63  }colMS{% endbloc
-00000700: 6b20 257d 0a0a 7b25 2062 6c6f 636b 2062  k %}..{% block b
-00000710: 6f64 7963 6c61 7373 2025 7d64 6173 6862  odyclass %}dashb
-00000720: 6f61 7264 7b25 2065 6e64 626c 6f63 6b20  oard{% endblock 
-00000730: 257d 0a0a 7b25 2062 6c6f 636b 2075 7365  %}..{% block use
-00000740: 726c 696e 6b73 2025 7d3c 6120 6872 6566  rlinks %}<a href
-00000750: 3d22 7b25 2075 726c 2027 6164 6d69 6e3a  ="{% url 'admin:
-00000760: 696e 6465 7827 2025 7d64 6f63 2f22 3e7b  index' %}doc/">{
-00000770: 2520 7472 616e 7320 2744 6f63 756d 656e  % trans 'Documen
-00000780: 7461 7469 6f6e 2720 257d 3c2f 613e 202f  tation' %}</a> /
-00000790: 0a20 2020 203c 6120 6872 6566 3d22 7b25  .    <a href="{%
-000007a0: 2075 726c 2027 6164 6d69 6e3a 696e 6465   url 'admin:inde
-000007b0: 7827 2025 7d70 6173 7377 6f72 645f 6368  x' %}password_ch
-000007c0: 616e 6765 2f22 3e7b 2520 7472 616e 7320  ange/">{% trans 
-000007d0: 2743 6861 6e67 6520 7061 7373 776f 7264  'Change password
-000007e0: 2720 257d 3c2f 613e 202f 0a20 2020 203c  ' %}</a> /.    <
-000007f0: 6120 6872 6566 3d22 7b25 2075 726c 2027  a href="{% url '
-00000800: 6164 6d69 6e3a 696e 6465 7827 2025 7d6c  admin:index' %}l
-00000810: 6f67 6f75 742f 223e 7b25 2074 7261 6e73  ogout/">{% trans
-00000820: 2027 4c6f 6720 6f75 7427 2025 7d3c 2f61   'Log out' %}</a
-00000830: 3e7b 2520 656e 6462 6c6f 636b 2025 7d0a  >{% endblock %}.
-00000840: 0a7b 2520 626c 6f63 6b20 6272 6561 6463  .{% block breadc
-00000850: 7275 6d62 7320 257d 7b25 2069 6620 6e6f  rumbs %}{% if no
-00000860: 7420 6973 5f70 6f70 7570 2025 7d0a 2020  t is_popup %}.  
-00000870: 2020 3c64 6976 2063 6c61 7373 3d22 6272    <div class="br
-00000880: 6561 6463 7275 6d62 7322 3e0a 2020 2020  eadcrumbs">.    
-00000890: 2020 2020 3c61 2068 7265 663d 227b 2520      <a href="{% 
-000008a0: 7572 6c20 2761 646d 696e 3a69 6e64 6578  url 'admin:index
-000008b0: 2720 257d 223e 7b25 2074 7261 6e73 2022  ' %}">{% trans "
-000008c0: 486f 6d65 2220 257d 3c2f 613e 2026 7273  Home" %}</a> &rs
-000008d0: 6171 756f 3b0a 2020 2020 2020 2020 7b25  aquo;.        {%
-000008e0: 2074 7261 6e73 2022 4564 6974 2053 6974   trans "Edit Sit
-000008f0: 6520 5365 7474 696e 6773 2220 257d 0a20  e Settings" %}. 
-00000900: 2020 203c 2f64 6976 3e0a 7b25 2065 6e64     </div>.{% end
-00000910: 6966 2025 7d7b 2520 656e 6462 6c6f 636b  if %}{% endblock
-00000920: 2025 7d0a 0a7b 2520 626c 6f63 6b20 6d65   %}..{% block me
-00000930: 7373 6167 6573 2025 7d0a 2020 2020 7b25  ssages %}.    {%
-00000940: 2069 6620 6d65 7373 6167 6573 2025 7d0a   if messages %}.
-00000950: 2020 2020 2020 2020 3c75 6c20 636c 6173          <ul clas
-00000960: 733d 226d 6573 7361 6765 6c69 7374 223e  s="messagelist">
-00000970: 7b25 2066 6f72 206d 6573 7361 6765 2069  {% for message i
-00000980: 6e20 6d65 7373 6167 6573 2025 7d0a 2020  n messages %}.  
-00000990: 2020 2020 2020 2020 2020 3c6c 697b 2520            <li{% 
-000009a0: 6966 206d 6573 7361 6765 2e74 6167 7320  if message.tags 
-000009b0: 257d 2063 6c61 7373 3d22 7b7b 206d 6573  %} class="{{ mes
-000009c0: 7361 6765 2e74 6167 7320 7d7d 227b 2520  sage.tags }}"{% 
-000009d0: 656e 6469 6620 257d 3e7b 7b20 6d65 7373  endif %}>{{ mess
-000009e0: 6167 6520 7d7d 3c2f 6c69 3e0a 2020 2020  age }}</li>.    
-000009f0: 2020 2020 7b25 2065 6e64 666f 7220 257d      {% endfor %}
-00000a00: 3c2f 756c 3e0a 2020 2020 7b25 2065 6e64  </ul>.    {% end
-00000a10: 6966 2025 7d0a 7b25 2065 6e64 626c 6f63  if %}.{% endbloc
-00000a20: 6b20 6d65 7373 6167 6573 2025 7d0a 0a7b  k messages %}..{
-00000a30: 2520 626c 6f63 6b20 636f 6e74 656e 7420  % block content 
-00000a40: 257d 0a20 2020 203c 7370 616e 2073 7479  %}.    <span sty
-00000a50: 6c65 3d22 636c 6561 723a 2062 6f74 683b  le="clear: both;
-00000a60: 223e 3c2f 7370 616e 3e0a 2020 2020 3c64  "></span>.    <d
-00000a70: 6976 2069 643d 2263 6f6e 7465 6e74 2d6d  iv id="content-m
-00000a80: 6169 6e22 3e0a 2020 2020 2020 2020 7b25  ain">.        {%
-00000a90: 2069 6620 6e6f 7420 7573 655f 6462 2025   if not use_db %
-00000aa0: 7d0a 2020 2020 2020 2020 2020 2020 3c70  }.            <p
-00000ab0: 3e7b 2520 7472 616e 7320 224c 6976 6573  >{% trans "Lives
-00000ac0: 6574 7469 6e67 7320 6172 6520 6469 7361  ettings are disa
-00000ad0: 626c 6564 2066 6f72 2074 6869 7320 7369  bled for this si
-00000ae0: 7465 2e22 2025 7d3c 2f70 3e0a 2020 2020  te." %}</p>.    
-00000af0: 2020 2020 2020 2020 3c70 3e7b 2520 7472          <p>{% tr
-00000b00: 616e 7320 2241 6c6c 2063 6f6e 6669 6775  ans "All configu
-00000b10: 7261 7469 6f6e 206f 7074 696f 6e73 206d  ration options m
-00000b20: 7573 7420 6265 2065 6469 7465 6420 696e  ust be edited in
-00000b30: 2074 6865 2073 6974 6520 7365 7474 696e   the site settin
-00000b40: 6773 2e70 7920 6669 6c65 2220 257d 3c2f  gs.py file" %}</
-00000b50: 703e 0a20 2020 2020 2020 2020 2020 203c  p>.            <
-00000b60: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
-00000b70: 2020 7b25 2061 646d 696e 5f73 6974 655f    {% admin_site_
-00000b80: 7669 6577 7320 2773 6174 6368 6d6f 5f73  views 'satchmo_s
-00000b90: 6974 655f 7365 7474 696e 6773 2720 257d  ite_settings' %}
-00000ba0: 0a20 2020 2020 2020 207b 2520 656c 7365  .        {% else
-00000bb0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-00000bc0: 7b25 2069 6620 666f 726d 2e65 7272 6f72  {% if form.error
-00000bd0: 7320 257d 0a20 2020 2020 2020 2020 2020  s %}.           
-00000be0: 2020 2020 203c 7020 636c 6173 733d 2265       <p class="e
-00000bf0: 7272 6f72 6e6f 7465 223e 0a20 2020 2020  rrornote">.     
-00000c00: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00000c10: 2520 626c 6f63 6b74 7261 6e73 2063 6f75  % blocktrans cou
-00000c20: 6e74 2066 6f72 6d2e 6572 726f 7273 7c6c  nt form.errors|l
-00000c30: 656e 6774 6820 6173 2063 6f75 6e74 6572  ength as counter
-00000c40: 2025 7d50 6c65 6173 6520 636f 7272 6563   %}Please correc
-00000c50: 7420 7468 6520 6572 726f 7220 6265 6c6f  t the error belo
-00000c60: 772e 7b25 2070 6c75 7261 6c20 257d 0a20  w.{% plural %}. 
-00000c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c80: 2020 2020 2020 2050 6c65 6173 6520 636f         Please co
-00000c90: 7272 6563 7420 7468 6520 6572 726f 7273  rrect the errors
-00000ca0: 2062 656c 6f77 2e7b 2520 656e 6462 6c6f   below.{% endblo
-00000cb0: 636b 7472 616e 7320 257d 0a20 2020 2020  cktrans %}.     
-00000cc0: 2020 2020 2020 2020 2020 203c 2f70 3e0a             </p>.
-00000cd0: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
-00000ce0: 6e64 6966 2025 7d0a 2020 2020 2020 2020  ndif %}.        
-00000cf0: 2020 2020 7b25 2069 6620 666f 726d 2e66      {% if form.f
-00000d00: 6965 6c64 7320 257d 0a20 2020 2020 2020  ields %}.       
-00000d10: 2020 2020 2020 2020 203c 666f 726d 206d           <form m
-00000d20: 6574 686f 643d 2270 6f73 7422 2069 643d  ethod="post" id=
-00000d30: 2273 6574 7469 6e67 7366 6f72 6d22 2065  "settingsform" e
-00000d40: 6e63 7479 7065 3d22 6d75 6c74 6970 6172  nctype="multipar
-00000d50: 742f 666f 726d 2d64 6174 6122 3e7b 2520  t/form-data">{% 
-00000d60: 6373 7266 5f74 6f6b 656e 2025 7d0a 2020  csrf_token %}.  
-00000d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d80: 2020 7b25 2066 6f72 2066 6965 6c64 2069    {% for field i
-00000d90: 6e20 666f 726d 2025 7d0a 2020 2020 2020  n form %}.      
-00000da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000db0: 2020 7b25 2069 6620 6669 656c 642e 6973    {% if field.is
-00000dc0: 5f68 6964 6465 6e20 257d 0a20 2020 2020  _hidden %}.     
-00000dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000de0: 2020 2020 2020 203c 7472 2073 7479 6c65         <tr style
-00000df0: 3d22 6469 7370 6c61 793a 206e 6f6e 653b  ="display: none;
-00000e00: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00000e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e20: 2020 203c 7464 3e7b 7b20 6669 656c 6420     <td>{{ field 
-00000e30: 7d7d 3c2f 7464 3e0a 2020 2020 2020 2020  }}</td>.        
-00000e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e50: 2020 2020 3c2f 7472 3e0a 2020 2020 2020      </tr>.      
-00000e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e70: 2020 7b25 2065 6c73 6520 257d 0a20 2020    {% else %}.   
-00000e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e90: 2020 2020 2020 2020 207b 2520 6966 6368           {% ifch
-00000ea0: 616e 6765 6420 6669 656c 642e 6669 656c  anged field.fiel
-00000eb0: 642e 6772 6f75 7020 257d 7b25 2077 6974  d.group %}{% wit
-00000ec0: 6820 6669 656c 642e 6669 656c 642e 6772  h field.field.gr
-00000ed0: 6f75 7020 6173 2067 726f 7570 2025 7d0a  oup as group %}.
-00000ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f00: 7b25 2069 6620 6e6f 7420 666f 726c 6f6f  {% if not forloo
-00000f10: 702e 6669 7273 7420 257d 0a20 2020 2020  p.first %}.     
-00000f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f30: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000f40: 2f74 6162 6c65 3e0a 2020 2020 2020 2020  /table>.        
-00000f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f60: 2020 2020 2020 2020 2020 2020 3c2f 6669              </fi
-00000f70: 656c 6473 6574 3e0a 2020 2020 2020 2020  eldset>.        
-00000f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f90: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
-00000fa0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-00000fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fc0: 2020 2020 3c66 6965 6c64 7365 7420 636c      <fieldset cl
-00000fd0: 6173 733d 226d 6f64 756c 6520 636f 6c6c  ass="module coll
-00000fe0: 6170 7365 223e 0a20 2020 2020 2020 2020  apse">.         
-00000ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001000: 2020 2020 2020 203c 6832 2069 643d 227b         <h2 id="{
-00001010: 7b20 6772 6f75 702e 6b65 7920 7d7d 223e  { group.key }}">
-00001020: 7b7b 2067 726f 7570 2e6e 616d 6520 7d7d  {{ group.name }}
-00001030: 3c2f 6832 3e0a 2020 2020 2020 2020 2020  </h2>.          
-00001040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001050: 2020 2020 2020 3c74 6162 6c65 2073 756d        <table sum
-00001060: 6d61 7279 3d22 7b25 2062 6c6f 636b 7472  mary="{% blocktr
-00001070: 616e 7320 7769 7468 2067 726f 7570 2e6e  ans with group.n
-00001080: 616d 6520 6173 206e 616d 6520 257d 4772  ame as name %}Gr
-00001090: 6f75 7020 7365 7474 696e 6773 3a20 7b7b  oup settings: {{
-000010a0: 206e 616d 6520 7d7d 7b25 2065 6e64 626c   name }}{% endbl
-000010b0: 6f63 6b74 7261 6e73 2025 7d22 0a20 2020  ocktrans %}".   
-000010c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010e0: 2020 2020 7374 796c 653d 2277 6964 7468      style="width
-000010f0: 3a20 3130 3025 223e 0a20 2020 2020 2020  : 100%">.       
-00001100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001110: 2020 2020 207b 2520 656e 6477 6974 6820       {% endwith 
-00001120: 257d 7b25 2065 6e64 6966 6368 616e 6765  %}{% endifchange
-00001130: 6420 257d 0a20 2020 2020 2020 2020 2020  d %}.           
-00001140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001150: 207b 2520 6966 2066 6965 6c64 2e65 7272   {% if field.err
-00001160: 6f72 7320 257d 0a20 2020 2020 2020 2020  ors %}.         
+00000070: 2020 2020 3c73 6372 6970 7420 7372 633d      <script src=
+00000080: 227b 2520 7374 6174 6963 2022 6c69 7665  "{% static "live
+00000090: 7365 7474 696e 6773 2f6a 732f 7374 7269  settings/js/stri
+000000a0: 6e67 5f61 7272 6179 5f77 6964 6765 742e  ng_array_widget.
+000000b0: 6a73 2220 257d 223e 3c2f 7363 7269 7074  js" %}"></script
+000000c0: 3e0a 2020 2020 3c73 6372 6970 7420 7479  >.    <script ty
+000000d0: 7065 3d22 7465 7874 2f6a 6176 6173 6372  pe="text/javascr
+000000e0: 6970 7422 2073 7263 3d22 7b25 2075 726c  ipt" src="{% url
+000000f0: 2027 6164 6d69 6e3a 6a73 6931 386e 2720   'admin:jsi18n' 
+00000100: 257d 223e 3c2f 7363 7269 7074 3e0a 2020  %}"></script>.  
+00000110: 2020 3c73 6372 6970 7420 7479 7065 3d22    <script type="
+00000120: 7465 7874 2f6a 6176 6173 6372 6970 7422  text/javascript"
+00000130: 2073 7263 3d22 7b25 2073 7461 7469 6320   src="{% static 
+00000140: 2261 646d 696e 2f6a 732f 636f 7265 2e6a  "admin/js/core.j
+00000150: 7322 2025 7d22 3e3c 2f73 6372 6970 743e  s" %}"></script>
+00000160: 0a20 2020 203c 7363 7269 7074 2074 7970  .    <script typ
+00000170: 653d 2274 6578 742f 6a61 7661 7363 7269  e="text/javascri
+00000180: 7074 2220 7372 633d 227b 2520 7374 6174  pt" src="{% stat
+00000190: 6963 2022 6164 6d69 6e2f 6a73 2f76 656e  ic "admin/js/ven
+000001a0: 646f 722f 6a71 7565 7279 2f6a 7175 6572  dor/jquery/jquer
+000001b0: 792e 6d69 6e2e 6a73 2220 257d 223e 3c2f  y.min.js" %}"></
+000001c0: 7363 7269 7074 3e0a 2020 2020 3c73 6372  script>.    <scr
+000001d0: 6970 7420 7479 7065 3d22 7465 7874 2f6a  ipt type="text/j
+000001e0: 6176 6173 6372 6970 7422 2073 7263 3d22  avascript" src="
+000001f0: 7b25 2073 7461 7469 6320 2261 646d 696e  {% static "admin
+00000200: 2f6a 732f 6a71 7565 7279 2e69 6e69 742e  /js/jquery.init.
+00000210: 6a73 2220 257d 223e 3c2f 7363 7269 7074  js" %}"></script
+00000220: 3e0a 2020 2020 3c73 6372 6970 7420 7479  >.    <script ty
+00000230: 7065 3d22 7465 7874 2f6a 6176 6173 6372  pe="text/javascr
+00000240: 6970 7422 2073 7263 3d22 7b25 2073 7461  ipt" src="{% sta
+00000250: 7469 6320 2261 646d 696e 2f6a 732f 636f  tic "admin/js/co
+00000260: 6c6c 6170 7365 2e6a 7322 2025 7d22 3e3c  llapse.js" %}"><
+00000270: 2f73 6372 6970 743e 0a20 2020 203c 7363  /script>.    <sc
+00000280: 7269 7074 2074 7970 653d 2274 6578 742f  ript type="text/
+00000290: 6a61 7661 7363 7269 7074 223e 0a20 2020  javascript">.   
+000002a0: 2020 2020 2076 6172 2024 203d 2064 6a61       var $ = dja
+000002b0: 6e67 6f2e 6a51 7565 7279 3b0a 0a20 2020  ngo.jQuery;..   
+000002c0: 2020 2020 2066 756e 6374 696f 6e20 746f       function to
+000002d0: 6767 6c65 436f 6c6c 6170 7365 416c 6c28  ggleCollapseAll(
+000002e0: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
+000002f0: 7661 7220 616c 6c53 6574 7320 3d20 2428  var allSets = $(
+00000300: 2266 6965 6c64 7365 742e 636f 6c6c 6170  "fieldset.collap
+00000310: 7365 2229 3b0a 2020 2020 2020 2020 2020  se");.          
+00000320: 2020 7661 7220 636f 6c6c 6170 7365 6453    var collapsedS
+00000330: 6574 7320 3d20 2428 2266 6965 6c64 7365  ets = $("fieldse
+00000340: 742e 636f 6c6c 6170 7365 2e63 6f6c 6c61  t.collapse.colla
+00000350: 7073 6564 2229 3b0a 2020 2020 2020 2020  psed");.        
+00000360: 2020 2020 6966 2028 616c 6c53 6574 732e      if (allSets.
+00000370: 6c65 6e67 7468 202d 2063 6f6c 6c61 7073  length - collaps
+00000380: 6564 5365 7473 2e6c 656e 6774 6820 3e20  edSets.length > 
+00000390: 636f 6c6c 6170 7365 6453 6574 732e 6c65  collapsedSets.le
+000003a0: 6e67 7468 2920 7b0a 2020 2020 2020 2020  ngth) {.        
+000003b0: 2020 2020 2020 2020 616c 6c53 6574 732e          allSets.
+000003c0: 6164 6443 6c61 7373 2822 636f 6c6c 6170  addClass("collap
+000003d0: 7365 6422 293b 0a20 2020 2020 2020 2020  sed");.         
+000003e0: 2020 207d 2065 6c73 6520 7b0a 2020 2020     } else {.    
+000003f0: 2020 2020 2020 2020 2020 2020 616c 6c53              allS
+00000400: 6574 732e 7265 6d6f 7665 436c 6173 7328  ets.removeClass(
+00000410: 2263 6f6c 6c61 7073 6564 2229 3b0a 2020  "collapsed");.  
+00000420: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00000430: 2020 2020 2020 2020 7265 7475 726e 2066          return f
+00000440: 616c 7365 3b0a 2020 2020 2020 2020 7d0a  alse;.        }.
+00000450: 0a20 2020 2020 2020 2066 756e 6374 696f  .        functio
+00000460: 6e20 746f 6767 6c65 436f 6c6c 6170 7365  n toggleCollapse
+00000470: 2865 6c65 6d29 207b 0a20 2020 2020 2020  (elem) {.       
+00000480: 2020 2020 2076 6172 2066 6965 6c64 7365       var fieldse
+00000490: 7420 3d20 2428 656c 656d 292e 636c 6f73  t = $(elem).clos
+000004a0: 6573 7428 2766 6965 6c64 7365 7427 293b  est('fieldset');
+000004b0: 0a20 2020 2020 2020 2020 2020 2066 6965  .            fie
+000004c0: 6c64 7365 742e 746f 6767 6c65 436c 6173  ldset.toggleClas
+000004d0: 7328 2763 6f6c 6c61 7073 6564 2729 3b0a  s('collapsed');.
+000004e0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000004f0: 726e 2066 616c 7365 3b0a 2020 2020 2020  rn false;.      
+00000500: 2020 7d0a 2020 2020 3c2f 7363 7269 7074    }.    </script
+00000510: 3e0a 7b25 2065 6e64 626c 6f63 6b20 257d  >.{% endblock %}
+00000520: 0a0a 7b25 2062 6c6f 636b 2065 7874 7261  ..{% block extra
+00000530: 7374 796c 6520 257d 0a20 2020 207b 7b20  style %}.    {{ 
+00000540: 626c 6f63 6b2e 7375 7065 7220 7d7d 0a20  block.super }}. 
+00000550: 2020 203c 6c69 6e6b 2072 656c 3d22 7374     <link rel="st
+00000560: 796c 6573 6865 6574 2220 7479 7065 3d22  ylesheet" type="
+00000570: 7465 7874 2f63 7373 2220 6872 6566 3d22  text/css" href="
+00000580: 7b25 2073 7461 7469 6320 2261 646d 696e  {% static "admin
+00000590: 2f63 7373 2f66 6f72 6d73 2e63 7373 2220  /css/forms.css" 
+000005a0: 257d 222f 3e0a 2020 2020 3c73 7479 6c65  %}"/>.    <style
+000005b0: 2074 7970 653d 2274 6578 742f 6373 7322   type="text/css"
+000005c0: 3e0a 2020 2020 2020 2020 756c 2e66 6965  >.        ul.fie
+000005d0: 6c64 7265 6620 7b0a 2020 2020 2020 2020  ldref {.        
+000005e0: 2020 2020 6d61 7267 696e 3a20 303b 0a20      margin: 0;. 
+000005f0: 2020 2020 2020 2020 2020 2070 6164 6469             paddi
+00000600: 6e67 3a20 303b 0a20 2020 2020 2020 2020  ng: 0;.         
+00000610: 2020 2066 6f6e 742d 7369 7a65 3a20 3970     font-size: 9p
+00000620: 783b 0a20 2020 2020 2020 207d 0a0a 2020  x;.        }..  
+00000630: 2020 2020 2020 756c 2e66 6965 6c64 7265        ul.fieldre
+00000640: 6620 6c69 207b 0a20 2020 2020 2020 2020  f li {.         
+00000650: 2020 2066 6c6f 6174 3a20 6c65 6674 3b0a     float: left;.
+00000660: 2020 2020 2020 2020 2020 2020 6d61 7267              marg
+00000670: 696e 3a20 3020 3130 7078 2030 2030 3b0a  in: 0 10px 0 0;.
+00000680: 2020 2020 2020 2020 2020 2020 6c69 7374              list
+00000690: 2d73 7479 6c65 3a20 6e6f 6e65 3b0a 2020  -style: none;.  
+000006a0: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
+000006b0: 2066 6965 6c64 7365 742e 636f 6c6c 6170   fieldset.collap
+000006c0: 7365 2068 322c 0a20 2020 2020 2020 2066  se h2,.        f
+000006d0: 6965 6c64 7365 742e 636f 6c6c 6170 7365  ieldset.collapse
+000006e0: 2e63 6f6c 6c61 7073 6564 2068 3220 7b0a  .collapsed h2 {.
+000006f0: 2020 2020 2020 2020 2020 2020 6469 7370              disp
+00000700: 6c61 793a 2066 6c65 7820 2169 6d70 6f72  lay: flex !impor
+00000710: 7461 6e74 3b0a 2020 2020 2020 2020 7d0a  tant;.        }.
+00000720: 0a20 2020 2020 2020 2066 6965 6c64 7365  .        fieldse
+00000730: 742e 636f 6c6c 6170 7365 6420 6832 203e  t.collapsed h2 >
+00000740: 202a 207b 0a20 2020 2020 2020 2020 2020   * {.           
+00000750: 2064 6973 706c 6179 3a20 626c 6f63 6b20   display: block 
+00000760: 2169 6d70 6f72 7461 6e74 0a20 2020 2020  !important.     
+00000770: 2020 207d 0a0a 2020 2020 2020 2020 6669     }..        fi
+00000780: 656c 6473 6574 2068 3220 7b0a 2020 2020  eldset h2 {.    
+00000790: 2020 2020 2020 2020 6a75 7374 6966 792d          justify-
+000007a0: 636f 6e74 656e 743a 2073 7061 6365 2d62  content: space-b
+000007b0: 6574 7765 656e 3b0a 2020 2020 2020 2020  etween;.        
+000007c0: 2020 2020 7769 6474 683a 2031 3030 253b      width: 100%;
+000007d0: 0a20 2020 2020 2020 2020 2020 2062 6f78  .            box
+000007e0: 2d73 697a 696e 673a 2062 6f72 6465 722d  -sizing: border-
+000007f0: 626f 783b 0a20 2020 2020 2020 207d 0a0a  box;.        }..
+00000800: 2020 2020 2020 2020 6669 656c 6473 6574          fieldset
+00000810: 2068 3220 6120 7b0a 2020 2020 2020 2020   h2 a {.        
+00000820: 2020 2020 636f 6c6f 723a 2076 6172 282d      color: var(-
+00000830: 2d61 6363 656e 7429 3b0a 2020 2020 2020  -accent);.      
+00000840: 2020 2020 2020 6375 7273 6f72 3a20 706f        cursor: po
+00000850: 696e 7465 723b 0a20 2020 2020 2020 207d  inter;.        }
+00000860: 0a0a 2020 2020 2020 2020 6469 762e 6669  ..        div.fi
+00000870: 656c 6463 6f6e 7461 696e 6572 207b 0a20  eldcontainer {. 
+00000880: 2020 2020 2020 2020 2020 2066 6c6f 6174             float
+00000890: 3a20 6c65 6674 3b0a 2020 2020 2020 2020  : left;.        
+000008a0: 2020 2020 6d61 7267 696e 2d72 6967 6874      margin-right
+000008b0: 3a20 303b 0a20 2020 2020 2020 207d 0a0a  : 0;.        }..
+000008c0: 2020 2020 2020 2020 2e74 6f67 676c 652d          .toggle-
+000008d0: 636f 6c6c 6170 7365 2d61 6c6c 207b 0a20  collapse-all {. 
+000008e0: 2020 2020 2020 2020 2020 2074 6578 742d             text-
+000008f0: 616c 6967 6e3a 2072 6967 6874 3b0a 2020  align: right;.  
+00000900: 2020 2020 2020 2020 2020 7472 616e 7366            transf
+00000910: 6f72 6d3a 2074 7261 6e73 6c61 7465 5928  orm: translateY(
+00000920: 2d32 2e36 3572 656d 293b 0a20 2020 2020  -2.65rem);.     
+00000930: 2020 2020 2020 2068 6569 6768 743a 2030         height: 0
+00000940: 3b0a 2020 2020 2020 2020 7d0a 2020 2020  ;.        }.    
+00000950: 3c2f 7374 796c 653e 0a7b 2520 656e 6462  </style>.{% endb
+00000960: 6c6f 636b 2025 7d0a 0a7b 2520 626c 6f63  lock %}..{% bloc
+00000970: 6b20 636f 6c74 7970 6520 257d 636f 6c4d  k coltype %}colM
+00000980: 537b 2520 656e 6462 6c6f 636b 2025 7d0a  S{% endblock %}.
+00000990: 0a7b 2520 626c 6f63 6b20 626f 6479 636c  .{% block bodycl
+000009a0: 6173 7320 257d 6461 7368 626f 6172 647b  ass %}dashboard{
+000009b0: 2520 656e 6462 6c6f 636b 2025 7d0a 0a7b  % endblock %}..{
+000009c0: 2520 626c 6f63 6b20 7573 6572 6c69 6e6b  % block userlink
+000009d0: 7320 257d 3c61 2068 7265 663d 227b 2520  s %}<a href="{% 
+000009e0: 7572 6c20 2761 646d 696e 3a69 6e64 6578  url 'admin:index
+000009f0: 2720 257d 646f 632f 223e 7b25 2074 7261  ' %}doc/">{% tra
+00000a00: 6e73 2027 446f 6375 6d65 6e74 6174 696f  ns 'Documentatio
+00000a10: 6e27 2025 7d3c 2f61 3e20 2f0a 2020 2020  n' %}</a> /.    
+00000a20: 3c61 2068 7265 663d 227b 2520 7572 6c20  <a href="{% url 
+00000a30: 2761 646d 696e 3a69 6e64 6578 2720 257d  'admin:index' %}
+00000a40: 7061 7373 776f 7264 5f63 6861 6e67 652f  password_change/
+00000a50: 223e 7b25 2074 7261 6e73 2027 4368 616e  ">{% trans 'Chan
+00000a60: 6765 2070 6173 7377 6f72 6427 2025 7d3c  ge password' %}<
+00000a70: 2f61 3e20 2f0a 2020 2020 3c61 2068 7265  /a> /.    <a hre
+00000a80: 663d 227b 2520 7572 6c20 2761 646d 696e  f="{% url 'admin
+00000a90: 3a69 6e64 6578 2720 257d 6c6f 676f 7574  :index' %}logout
+00000aa0: 2f22 3e7b 2520 7472 616e 7320 274c 6f67  /">{% trans 'Log
+00000ab0: 206f 7574 2720 257d 3c2f 613e 7b25 2065   out' %}</a>{% e
+00000ac0: 6e64 626c 6f63 6b20 257d 0a0a 7b25 2062  ndblock %}..{% b
+00000ad0: 6c6f 636b 2062 7265 6164 6372 756d 6273  lock breadcrumbs
+00000ae0: 2025 7d7b 2520 6966 206e 6f74 2069 735f   %}{% if not is_
+00000af0: 706f 7075 7020 257d 0a20 2020 203c 6469  popup %}.    <di
+00000b00: 7620 636c 6173 733d 2262 7265 6164 6372  v class="breadcr
+00000b10: 756d 6273 223e 0a20 2020 2020 2020 203c  umbs">.        <
+00000b20: 6120 6872 6566 3d22 7b25 2075 726c 2027  a href="{% url '
+00000b30: 6164 6d69 6e3a 696e 6465 7827 2025 7d22  admin:index' %}"
+00000b40: 3e7b 2520 7472 616e 7320 2248 6f6d 6522  >{% trans "Home"
+00000b50: 2025 7d3c 2f61 3e20 2672 7361 7175 6f3b   %}</a> &rsaquo;
+00000b60: 0a20 2020 2020 2020 207b 2520 7472 616e  .        {% tran
+00000b70: 7320 2245 6469 7420 5369 7465 2053 6574  s "Edit Site Set
+00000b80: 7469 6e67 7322 2025 7d0a 2020 2020 3c2f  tings" %}.    </
+00000b90: 6469 763e 0a7b 2520 656e 6469 6620 257d  div>.{% endif %}
+00000ba0: 7b25 2065 6e64 626c 6f63 6b20 257d 0a0a  {% endblock %}..
+00000bb0: 7b25 2062 6c6f 636b 206d 6573 7361 6765  {% block message
+00000bc0: 7320 257d 0a20 2020 207b 2520 6966 206d  s %}.    {% if m
+00000bd0: 6573 7361 6765 7320 257d 0a20 2020 2020  essages %}.     
+00000be0: 2020 203c 756c 2063 6c61 7373 3d22 6d65     <ul class="me
+00000bf0: 7373 6167 656c 6973 7422 3e7b 2520 666f  ssagelist">{% fo
+00000c00: 7220 6d65 7373 6167 6520 696e 206d 6573  r message in mes
+00000c10: 7361 6765 7320 257d 0a20 2020 2020 2020  sages %}.       
+00000c20: 2020 2020 203c 6c69 7b25 2069 6620 6d65       <li{% if me
+00000c30: 7373 6167 652e 7461 6773 2025 7d20 636c  ssage.tags %} cl
+00000c40: 6173 733d 227b 7b20 6d65 7373 6167 652e  ass="{{ message.
+00000c50: 7461 6773 207d 7d22 7b25 2065 6e64 6966  tags }}"{% endif
+00000c60: 2025 7d3e 7b7b 206d 6573 7361 6765 207d   %}>{{ message }
+00000c70: 7d3c 2f6c 693e 0a20 2020 2020 2020 207b  }</li>.        {
+00000c80: 2520 656e 6466 6f72 2025 7d3c 2f75 6c3e  % endfor %}</ul>
+00000c90: 0a20 2020 207b 2520 656e 6469 6620 257d  .    {% endif %}
+00000ca0: 0a7b 2520 656e 6462 6c6f 636b 206d 6573  .{% endblock mes
+00000cb0: 7361 6765 7320 257d 0a0a 7b25 2062 6c6f  sages %}..{% blo
+00000cc0: 636b 2063 6f6e 7465 6e74 2025 7d0a 2020  ck content %}.  
+00000cd0: 2020 3c73 7061 6e20 7374 796c 653d 2263    <span style="c
+00000ce0: 6c65 6172 3a20 626f 7468 3b22 3e3c 2f73  lear: both;"></s
+00000cf0: 7061 6e3e 0a20 2020 203c 6469 7620 6964  pan>.    <div id
+00000d00: 3d22 636f 6e74 656e 742d 6d61 696e 223e  ="content-main">
+00000d10: 0a20 2020 2020 2020 203c 7020 636c 6173  .        <p clas
+00000d20: 733d 2274 6f67 676c 652d 636f 6c6c 6170  s="toggle-collap
+00000d30: 7365 2d61 6c6c 223e 3c61 206f 6e63 6c69  se-all"><a oncli
+00000d40: 636b 3d22 6a61 7661 7363 7269 7074 3a72  ck="javascript:r
+00000d50: 6574 7572 6e20 746f 6767 6c65 436f 6c6c  eturn toggleColl
+00000d60: 6170 7365 416c 6c28 293b 2220 6872 6566  apseAll();" href
+00000d70: 3d22 2322 3e7b 2520 7472 616e 7320 2773  ="#">{% trans 's
+00000d80: 686f 772f 6869 6465 2061 6c6c 2720 257d  how/hide all' %}
+00000d90: 3c2f 613e 3c2f 703e 0a20 2020 2020 2020  </a></p>.       
+00000da0: 207b 2520 6966 206e 6f74 2075 7365 5f64   {% if not use_d
+00000db0: 6220 257d 0a20 2020 2020 2020 2020 2020  b %}.           
+00000dc0: 203c 703e 7b25 2074 7261 6e73 2022 4c69   <p>{% trans "Li
+00000dd0: 7665 7365 7474 696e 6773 2061 7265 2064  vesettings are d
+00000de0: 6973 6162 6c65 6420 666f 7220 7468 6973  isabled for this
+00000df0: 2073 6974 652e 2220 257d 3c2f 703e 0a20   site." %}</p>. 
+00000e00: 2020 2020 2020 2020 2020 203c 703e 7b25             <p>{%
+00000e10: 2074 7261 6e73 2022 416c 6c20 636f 6e66   trans "All conf
+00000e20: 6967 7572 6174 696f 6e20 6f70 7469 6f6e  iguration option
+00000e30: 7320 6d75 7374 2062 6520 6564 6974 6564  s must be edited
+00000e40: 2069 6e20 7468 6520 7369 7465 2073 6574   in the site set
+00000e50: 7469 6e67 732e 7079 2066 696c 6522 2025  tings.py file" %
+00000e60: 7d3c 2f70 3e0a 2020 2020 2020 2020 2020  }</p>.          
+00000e70: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
+00000e80: 2020 2020 207b 2520 6164 6d69 6e5f 7369       {% admin_si
+00000e90: 7465 5f76 6965 7773 2027 7361 7463 686d  te_views 'satchm
+00000ea0: 6f5f 7369 7465 5f73 6574 7469 6e67 7327  o_site_settings'
+00000eb0: 2025 7d0a 2020 2020 2020 2020 7b25 2065   %}.        {% e
+00000ec0: 6c73 6520 257d 0a20 2020 2020 2020 2020  lse %}.         
+00000ed0: 2020 207b 2520 6966 2066 6f72 6d2e 6572     {% if form.er
+00000ee0: 726f 7273 2025 7d0a 2020 2020 2020 2020  rors %}.        
+00000ef0: 2020 2020 2020 2020 3c70 2063 6c61 7373          <p class
+00000f00: 3d22 6572 726f 726e 6f74 6522 3e0a 2020  ="errornote">.  
+00000f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f20: 2020 7b25 2062 6c6f 636b 7472 616e 7320    {% blocktrans 
+00000f30: 636f 756e 7420 666f 726d 2e65 7272 6f72  count form.error
+00000f40: 737c 6c65 6e67 7468 2061 7320 636f 756e  s|length as coun
+00000f50: 7465 7220 257d 506c 6561 7365 2063 6f72  ter %}Please cor
+00000f60: 7265 6374 2074 6865 2065 7272 6f72 2062  rect the error b
+00000f70: 656c 6f77 2e7b 2520 706c 7572 616c 2025  elow.{% plural %
+00000f80: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00000f90: 2020 2020 2020 2020 2020 506c 6561 7365            Please
+00000fa0: 2063 6f72 7265 6374 2074 6865 2065 7272   correct the err
+00000fb0: 6f72 7320 6265 6c6f 772e 7b25 2065 6e64  ors below.{% end
+00000fc0: 626c 6f63 6b74 7261 6e73 2025 7d0a 2020  blocktrans %}.  
+00000fd0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00000fe0: 703e 0a20 2020 2020 2020 2020 2020 207b  p>.            {
+00000ff0: 2520 656e 6469 6620 257d 0a20 2020 2020  % endif %}.     
+00001000: 2020 2020 2020 207b 2520 6966 2066 6f72         {% if for
+00001010: 6d2e 6669 656c 6473 2025 7d0a 2020 2020  m.fields %}.    
+00001020: 2020 2020 2020 2020 2020 2020 3c66 6f72              <for
+00001030: 6d20 6d65 7468 6f64 3d22 706f 7374 2220  m method="post" 
+00001040: 6964 3d22 7365 7474 696e 6773 666f 726d  id="settingsform
+00001050: 2220 656e 6374 7970 653d 226d 756c 7469  " enctype="multi
+00001060: 7061 7274 2f66 6f72 6d2d 6461 7461 223e  part/form-data">
+00001070: 7b25 2063 7372 665f 746f 6b65 6e20 257d  {% csrf_token %}
+00001080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001090: 2020 2020 207b 2520 666f 7220 6669 656c       {% for fiel
+000010a0: 6420 696e 2066 6f72 6d20 257d 0a20 2020  d in form %}.   
+000010b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010c0: 2020 2020 207b 2520 6966 2066 6965 6c64       {% if field
+000010d0: 2e69 735f 6869 6464 656e 2025 7d0a 2020  .is_hidden %}.  
+000010e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010f0: 2020 2020 2020 2020 2020 3c74 7220 7374            <tr st
+00001100: 796c 653d 2264 6973 706c 6179 3a20 6e6f  yle="display: no
+00001110: 6e65 3b22 3e0a 2020 2020 2020 2020 2020  ne;">.          
+00001120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001130: 2020 2020 2020 3c74 643e 7b7b 2066 6965        <td>{{ fie
+00001140: 6c64 207d 7d3c 2f74 643e 0a20 2020 2020  ld }}</td>.     
+00001150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001160: 2020 2020 2020 203c 2f74 723e 0a20 2020         </tr>.   
 00001170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001180: 2020 2020 2020 203c 7472 2063 6c61 7373         <tr class
-00001190: 3d22 6572 726f 7222 3e0a 2020 2020 2020  ="error">.      
-000011a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011b0: 2020 2020 2020 2020 2020 2020 2020 3c74                <t
-000011c0: 6420 636f 6c73 7061 6e3d 2232 223e 7b7b  d colspan="2">{{
-000011d0: 2066 6965 6c64 2e65 7272 6f72 7320 7d7d   field.errors }}
-000011e0: 3c2f 7464 3e0a 2020 2020 2020 2020 2020  </td>.          
-000011f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001200: 2020 2020 2020 3c2f 7472 3e0a 2020 2020        </tr>.    
-00001210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001220: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
-00001230: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00001180: 2020 2020 207b 2520 656c 7365 2025 7d0a       {% else %}.
+00001190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011a0: 2020 2020 2020 2020 2020 2020 7b25 2069              {% i
+000011b0: 6663 6861 6e67 6564 2066 6965 6c64 2e66  fchanged field.f
+000011c0: 6965 6c64 2e67 726f 7570 2025 7d7b 2520  ield.group %}{% 
+000011d0: 7769 7468 2066 6965 6c64 2e66 6965 6c64  with field.field
+000011e0: 2e67 726f 7570 2061 7320 6772 6f75 7020  .group as group 
+000011f0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+00001200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001210: 2020 207b 2520 6966 206e 6f74 2066 6f72     {% if not for
+00001220: 6c6f 6f70 2e66 6972 7374 2025 7d0a 2020  loop.first %}.  
+00001230: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001250: 3c74 727b 2520 6966 2066 6965 6c64 2e65  <tr{% if field.e
-00001260: 7272 6f72 7320 257d 2063 6c61 7373 3d22  rrors %} class="
-00001270: 6572 726f 7222 7b25 2065 6e64 6966 2025  error"{% endif %
-00001280: 7d3e 0a20 2020 2020 2020 2020 2020 2020  }>.             
+00001250: 2020 3c2f 7461 626c 653e 0a20 2020 2020    </table>.     
+00001260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001270: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00001280: 2f66 6965 6c64 7365 743e 0a20 2020 2020  /fieldset>.     
 00001290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012a0: 2020 203c 7464 2073 7479 6c65 3d22 7769     <td style="wi
-000012b0: 6474 683a 2035 3025 3b22 3e0a 2020 2020  dth: 50%;">.    
+000012a0: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
+000012b0: 6469 6620 257d 0a20 2020 2020 2020 2020  dif %}.         
 000012c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012e0: 7b7b 2066 6965 6c64 2e6c 6162 656c 5f74  {{ field.label_t
-000012f0: 6167 207d 7d0a 2020 2020 2020 2020 2020  ag }}.          
-00001300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001310: 2020 2020 2020 2020 2020 7b25 2069 6620            {% if 
-00001320: 6669 656c 642e 6865 6c70 5f74 6578 7420  field.help_text 
-00001330: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-00001340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001350: 2020 2020 2020 2020 2020 203c 7020 636c             <p cl
-00001360: 6173 733d 2268 656c 7022 3e7b 7b20 6669  ass="help">{{ fi
-00001370: 656c 642e 6865 6c70 5f74 6578 747c 6272  eld.help_text|br
-00001380: 6561 6b5f 6174 3a34 307c 7361 6665 207d  eak_at:40|safe }
-00001390: 7d3c 2f70 3e0a 2020 2020 2020 2020 2020  }</p>.          
-000013a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013b0: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
-000013c0: 6966 2025 7d0a 2020 2020 2020 2020 2020  if %}.          
-000013d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013e0: 2020 2020 2020 2020 2020 7b25 2069 6620            {% if 
-000013f0: 6669 656c 642e 6669 656c 642e 6465 6661  field.field.defa
-00001400: 756c 745f 7465 7874 2025 7d0a 2020 2020  ult_text %}.    
-00001410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001430: 2020 2020 3c70 2063 6c61 7373 3d22 6865      <p class="he
-00001440: 6c70 223e 7b7b 2066 6965 6c64 2e66 6965  lp">{{ field.fie
-00001450: 6c64 2e64 6566 6175 6c74 5f74 6578 747c  ld.default_text|
-00001460: 6272 6561 6b5f 6174 3a34 3020 7d7d 3c2f  break_at:40 }}</
-00001470: 703e 0a20 2020 2020 2020 2020 2020 2020  p>.             
-00001480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001490: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
-000014a0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+000012d0: 2020 2020 2020 203c 6669 656c 6473 6574         <fieldset
+000012e0: 2063 6c61 7373 3d22 6d6f 6475 6c65 2063   class="module c
+000012f0: 6f6c 6c61 7073 6520 636f 6c6c 6170 7365  ollapse collapse
+00001300: 6422 3e0a 2020 2020 2020 2020 2020 2020  d">.            
+00001310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001320: 2020 2020 2020 2020 3c68 3220 6964 3d22          <h2 id="
+00001330: 7b7b 2067 726f 7570 2e6b 6579 207d 7d22  {{ group.key }}"
+00001340: 3e3c 7370 616e 3e7b 7b20 6772 6f75 702e  ><span>{{ group.
+00001350: 6e61 6d65 207d 7d3c 2f73 7061 6e3e 3c61  name }}</span><a
+00001360: 206f 6e63 6c69 636b 3d22 6a61 7661 7363   onclick="javasc
+00001370: 7269 7074 3a20 7265 7475 726e 2074 6f67  ript: return tog
+00001380: 676c 6543 6f6c 6c61 7073 6528 7468 6973  gleCollapse(this
+00001390: 2922 3e73 686f 772f 6869 6465 3c2f 613e  )">show/hide</a>
+000013a0: 3c2f 6832 3e0a 2020 2020 2020 2020 2020  </h2>.          
+000013b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013c0: 2020 2020 2020 3c74 6162 6c65 2073 756d        <table sum
+000013d0: 6d61 7279 3d22 7b25 2062 6c6f 636b 7472  mary="{% blocktr
+000013e0: 616e 7320 7769 7468 2067 726f 7570 2e6e  ans with group.n
+000013f0: 616d 6520 6173 206e 616d 6520 257d 4772  ame as name %}Gr
+00001400: 6f75 7020 7365 7474 696e 6773 3a20 7b7b  oup settings: {{
+00001410: 206e 616d 6520 7d7d 7b25 2065 6e64 626c   name }}{% endbl
+00001420: 6f63 6b74 7261 6e73 2025 7d22 0a20 2020  ocktrans %}".   
+00001430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001450: 2020 2020 7374 796c 653d 2277 6964 7468      style="width
+00001460: 3a20 3130 3025 223e 0a20 2020 2020 2020  : 100%">.       
+00001470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001480: 2020 2020 207b 2520 656e 6477 6974 6820       {% endwith 
+00001490: 257d 7b25 2065 6e64 6966 6368 616e 6765  %}{% endifchange
+000014a0: 6420 257d 0a20 2020 2020 2020 2020 2020  d %}.           
 000014b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014c0: 2020 203c 2f74 643e 0a20 2020 2020 2020     </td>.       
-000014d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014e0: 2020 2020 2020 2020 203c 7464 3e7b 7b20           <td>{{ 
-000014f0: 6669 656c 6420 7d7d 3c2f 7464 3e0a 2020  field }}</td>.  
-00001500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001510: 2020 2020 2020 2020 2020 3c2f 7472 3e0a            </tr>.
-00001520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001530: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
-00001540: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-00001550: 2020 2020 2020 2020 7b25 2065 6e64 666f          {% endfo
-00001560: 7220 257d 0a20 2020 2020 2020 2020 2020  r %}.           
-00001570: 2020 2020 2020 2020 203c 2f74 6162 6c65           </table
-00001580: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00001590: 2020 2020 2020 3c2f 6669 656c 6473 6574        </fieldset
-000015a0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000015b0: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
-000015c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015d0: 207b 2520 6164 6d69 6e5f 7369 7465 5f76   {% admin_site_v
-000015e0: 6965 7773 2027 7361 7463 686d 6f5f 7369  iews 'satchmo_si
-000015f0: 7465 5f73 6574 7469 6e67 7327 2025 7d0a  te_settings' %}.
+000014c0: 207b 2520 6966 2066 6965 6c64 2e65 7272   {% if field.err
+000014d0: 6f72 7320 257d 0a20 2020 2020 2020 2020  ors %}.         
+000014e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014f0: 2020 2020 2020 203c 7472 2063 6c61 7373         <tr class
+00001500: 3d22 6572 726f 7222 3e0a 2020 2020 2020  ="error">.      
+00001510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001520: 2020 2020 2020 2020 2020 2020 2020 3c74                <t
+00001530: 6420 636f 6c73 7061 6e3d 2232 223e 7b7b  d colspan="2">{{
+00001540: 2066 6965 6c64 2e65 7272 6f72 7320 7d7d   field.errors }}
+00001550: 3c2f 7464 3e0a 2020 2020 2020 2020 2020  </td>.          
+00001560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001570: 2020 2020 2020 3c2f 7472 3e0a 2020 2020        </tr>.    
+00001580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001590: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
+000015a0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+000015b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015c0: 3c74 727b 2520 6966 2066 6965 6c64 2e65  <tr{% if field.e
+000015d0: 7272 6f72 7320 257d 2063 6c61 7373 3d22  rrors %} class="
+000015e0: 6572 726f 7222 7b25 2065 6e64 6966 2025  error"{% endif %
+000015f0: 7d3e 0a20 2020 2020 2020 2020 2020 2020  }>.             
 00001600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001610: 2020 2020 3c62 7220 636c 6173 733d 2263      <br class="c
-00001620: 6c65 6172 3a62 6f74 683b 222f 3e0a 2020  lear:both;"/>.  
+00001610: 2020 203c 7464 2073 7479 6c65 3d22 7769     <td style="wi
+00001620: 6474 683a 2035 3025 3b22 3e0a 2020 2020  dth: 50%;">.    
 00001630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001640: 2020 3c69 6e70 7574 2074 7970 653d 2273    <input type="s
-00001650: 7562 6d69 7422 2076 616c 7565 3d22 7b25  ubmit" value="{%
-00001660: 2074 7261 6e73 2027 5570 6461 7465 2053   trans 'Update S
-00001670: 6574 7469 6e67 7327 2025 7d22 2f3e 0a20  ettings' %}"/>. 
-00001680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001690: 2020 203c 703e 3c61 206f 6e63 6c69 636b     <p><a onclick
-000016a0: 3d22 6a61 7661 7363 7269 7074 3a72 6574  ="javascript:ret
-000016b0: 7572 6e20 756e 636f 6c6c 6170 7365 2829  urn uncollapse()
-000016c0: 3b22 2068 7265 663d 2223 223e 7b25 2074  ;" href="#">{% t
-000016d0: 7261 6e73 2027 556e 636f 6c6c 6170 7365  rans 'Uncollapse
-000016e0: 2061 6c6c 2720 257d 3c2f 613e 3c2f 703e   all' %}</a></p>
-000016f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001700: 2020 2020 203c 703e 3c61 2068 7265 663d       <p><a href=
-00001710: 227b 2520 7572 6c20 2773 6574 7469 6e67  "{% url 'setting
-00001720: 735f 6578 706f 7274 2720 257d 223e 7b25  s_export' %}">{%
-00001730: 2074 7261 6e73 2027 4578 706f 7274 2720   trans 'Export' 
-00001740: 257d 3c2f 613e 3c2f 703e 0a20 2020 2020  %}</a></p>.     
-00001750: 2020 2020 2020 2020 2020 203c 2f66 6f72             </for
-00001760: 6d3e 0a20 2020 2020 2020 2020 2020 207b  m>.            {
-00001770: 2520 656c 7365 2025 7d0a 2020 2020 2020  % else %}.      
-00001780: 2020 2020 2020 2020 2020 3c70 3e7b 2520            <p>{% 
-00001790: 7472 616e 7320 2259 6f75 2064 6f6e 2774  trans "You don't
-000017a0: 2068 6176 6520 7065 726d 6973 7369 6f6e   have permission
-000017b0: 2074 6f20 6564 6974 2076 616c 7565 732e   to edit values.
-000017c0: 2220 257d 3c2f 703e 0a20 2020 2020 2020  " %}</p>.       
-000017d0: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
-000017e0: 0a20 2020 2020 2020 207b 2520 656e 6469  .        {% endi
-000017f0: 6620 257d 0a20 2020 203c 2f64 6976 3e0a  f %}.    </div>.
-00001800: 7b25 2065 6e64 626c 6f63 6b20 257d 0a    {% endblock %}.
+00001640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001650: 7b7b 2066 6965 6c64 2e6c 6162 656c 5f74  {{ field.label_t
+00001660: 6167 207d 7d0a 2020 2020 2020 2020 2020  ag }}.          
+00001670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001680: 2020 2020 2020 2020 2020 7b25 2069 6620            {% if 
+00001690: 6669 656c 642e 6865 6c70 5f74 6578 7420  field.help_text 
+000016a0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+000016b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016c0: 2020 2020 2020 2020 2020 203c 7020 636c             <p cl
+000016d0: 6173 733d 2268 656c 7022 3e7b 7b20 6669  ass="help">{{ fi
+000016e0: 656c 642e 6865 6c70 5f74 6578 747c 6272  eld.help_text|br
+000016f0: 6561 6b5f 6174 3a34 307c 7361 6665 207d  eak_at:40|safe }
+00001700: 7d3c 2f70 3e0a 2020 2020 2020 2020 2020  }</p>.          
+00001710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001720: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
+00001730: 6966 2025 7d0a 2020 2020 2020 2020 2020  if %}.          
+00001740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001750: 2020 2020 2020 2020 2020 7b25 2069 6620            {% if 
+00001760: 6669 656c 642e 6669 656c 642e 6465 6661  field.field.defa
+00001770: 756c 745f 7465 7874 2025 7d0a 2020 2020  ult_text %}.    
+00001780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017a0: 2020 2020 3c70 2063 6c61 7373 3d22 6865      <p class="he
+000017b0: 6c70 223e 7b7b 2066 6965 6c64 2e66 6965  lp">{{ field.fie
+000017c0: 6c64 2e64 6566 6175 6c74 5f74 6578 747c  ld.default_text|
+000017d0: 6272 6561 6b5f 6174 3a34 3020 7d7d 3c2f  break_at:40 }}</
+000017e0: 703e 0a20 2020 2020 2020 2020 2020 2020  p>.             
+000017f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001800: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
+00001810: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+00001820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001830: 2020 203c 2f74 643e 0a20 2020 2020 2020     </td>.       
+00001840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001850: 2020 2020 2020 2020 203c 7464 3e7b 7b20           <td>{{ 
+00001860: 6669 656c 6420 7d7d 3c2f 7464 3e0a 2020  field }}</td>.  
+00001870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001880: 2020 2020 2020 2020 2020 3c2f 7472 3e0a            </tr>.
+00001890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018a0: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
+000018b0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+000018c0: 2020 2020 2020 2020 7b25 2065 6e64 666f          {% endfo
+000018d0: 7220 257d 0a20 2020 2020 2020 2020 2020  r %}.           
+000018e0: 2020 2020 2020 2020 203c 2f74 6162 6c65           </table
+000018f0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00001900: 2020 2020 2020 3c2f 6669 656c 6473 6574        </fieldset
+00001910: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00001920: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
+00001930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001940: 207b 2520 6164 6d69 6e5f 7369 7465 5f76   {% admin_site_v
+00001950: 6965 7773 2027 7361 7463 686d 6f5f 7369  iews 'satchmo_si
+00001960: 7465 5f73 6574 7469 6e67 7327 2025 7d0a  te_settings' %}.
+00001970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001980: 2020 2020 3c62 7220 636c 6173 733d 2263      <br class="c
+00001990: 6c65 6172 3a62 6f74 683b 222f 3e0a 2020  lear:both;"/>.  
+000019a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019b0: 2020 3c69 6e70 7574 2074 7970 653d 2273    <input type="s
+000019c0: 7562 6d69 7422 2076 616c 7565 3d22 7b25  ubmit" value="{%
+000019d0: 2074 7261 6e73 2027 5570 6461 7465 2053   trans 'Update S
+000019e0: 6574 7469 6e67 7327 2025 7d22 2f3e 0a20  ettings' %}"/>. 
+000019f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a00: 2020 203c 703e 3c61 2068 7265 663d 227b     <p><a href="{
+00001a10: 2520 7572 6c20 2773 6574 7469 6e67 735f  % url 'settings_
+00001a20: 6578 706f 7274 2720 257d 223e 7b25 2074  export' %}">{% t
+00001a30: 7261 6e73 2027 4578 706f 7274 2720 257d  rans 'Export' %}
+00001a40: 3c2f 613e 3c2f 703e 0a20 2020 2020 2020  </a></p>.       
+00001a50: 2020 2020 2020 2020 203c 2f66 6f72 6d3e           </form>
+00001a60: 0a20 2020 2020 2020 2020 2020 207b 2520  .            {% 
+00001a70: 656c 7365 2025 7d0a 2020 2020 2020 2020  else %}.        
+00001a80: 2020 2020 2020 2020 3c70 3e7b 2520 7472          <p>{% tr
+00001a90: 616e 7320 2259 6f75 2064 6f6e 2774 2068  ans "You don't h
+00001aa0: 6176 6520 7065 726d 6973 7369 6f6e 2074  ave permission t
+00001ab0: 6f20 6564 6974 2076 616c 7565 732e 2220  o edit values." 
+00001ac0: 257d 3c2f 703e 0a20 2020 2020 2020 2020  %}</p>.         
+00001ad0: 2020 207b 2520 656e 6469 6620 257d 0a20     {% endif %}. 
+00001ae0: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
+00001af0: 257d 0a20 2020 203c 2f64 6976 3e0a 7b25  %}.    </div>.{%
+00001b00: 2065 6e64 626c 6f63 6b20 257d 0a          endblock %}.
```

### Comparing `django-livesettings3-1.6.1/livesettings/templatetags/config_tags.py` & `django-livesettings3-1.6.2/livesettings/templatetags/config_tags.py`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.1/livesettings/tests.py` & `django-livesettings3-1.6.2/livesettings/tests.py`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.1/livesettings/utils.py` & `django-livesettings3-1.6.2/livesettings/utils.py`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.1/livesettings/values.py` & `django-livesettings3-1.6.2/livesettings/values.py.orig`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.1/livesettings/views.py` & `django-livesettings3-1.6.2/livesettings/views.py`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.1/livesettings/widgets.py` & `django-livesettings3-1.6.2/livesettings/widgets.py.orig`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.1/setup.py` & `django-livesettings3-1.6.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django-livesettings3',
-    version='1.6.1',
+    version='1.6.2',
     description="Python 3 port of django-livesettings",
     long_description="""Python 3 version of django live settings. It provides the ability to configure settings via an admin interface, rather than by editing "settings.py". Documentation avaiable at Github.""",
     author='Kunal Deo',
     author_email='kunaldeo@gmail.com',
     url='https://github.com/kunaldeo/django-livesettings3/',
     license='New BSD License',
     platforms=['any'],
@@ -20,8 +20,9 @@
                  'Programming Language :: Python :: 3.8',
                  'Programming Language :: Python :: 3.9',
                  'Programming Language :: Python :: 3.10',
                  'Framework :: Django'],
     packages=find_packages(),
     install_requires=['django>=1.8,<5', 'django-keyedcache3'],
     include_package_data=True,
+    zip_safe=False,
 )
```

