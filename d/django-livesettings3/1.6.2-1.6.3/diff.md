# Comparing `tmp/django-livesettings3-1.6.2.tar.gz` & `tmp/django-livesettings3-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-livesettings3-1.6.2.tar", last modified: Sun Jul 30 00:57:25 2023, max compression
+gzip compressed data, was "django-livesettings3-1.6.3.tar", last modified: Sun Jul 30 01:36:24 2023, max compression
```

## Comparing `django-livesettings3-1.6.2.tar` & `django-livesettings3-1.6.3.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.483907 django-livesettings3-1.6.2/
--rw-r--r--   0 evgeny     (501) staff       (20)       88 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/AUTHORS
--rw-r--r--   0 evgeny     (501) staff       (20)     1498 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/LICENSE
--rw-r--r--   0 evgeny     (501) staff       (20)       93 2023-07-30 00:53:02.000000 django-livesettings3-1.6.2/MANIFEST.in
--rw-r--r--   0 evgeny     (501) staff       (20)     1000 2023-07-30 00:57:25.484062 django-livesettings3-1.6.2/PKG-INFO
--rw-r--r--   0 evgeny     (501) staff       (20)     5910 2023-07-30 00:52:14.000000 django-livesettings3-1.6.2/README.md
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.444952 django-livesettings3-1.6.2/django_livesettings3.egg-info/
--rw-r--r--   0 evgeny     (501) staff       (20)     1000 2023-07-30 00:57:25.000000 django-livesettings3-1.6.2/django_livesettings3.egg-info/PKG-INFO
--rw-r--r--   0 evgeny     (501) staff       (20)     3588 2023-07-30 00:57:25.000000 django-livesettings3-1.6.2/django_livesettings3.egg-info/SOURCES.txt
--rw-r--r--   0 evgeny     (501) staff       (20)        1 2023-07-30 00:57:25.000000 django-livesettings3-1.6.2/django_livesettings3.egg-info/dependency_links.txt
--rw-r--r--   0 evgeny     (501) staff       (20)        1 2023-07-24 21:10:38.000000 django-livesettings3-1.6.2/django_livesettings3.egg-info/not-zip-safe
--rw-r--r--   0 evgeny     (501) staff       (20)       34 2023-07-30 00:57:25.000000 django-livesettings3-1.6.2/django_livesettings3.egg-info/requires.txt
--rw-r--r--   0 evgeny     (501) staff       (20)       13 2023-07-30 00:57:25.000000 django-livesettings3-1.6.2/django_livesettings3.egg-info/top_level.txt
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.454913 django-livesettings3-1.6.2/livesettings/
--rw-r--r--   0 evgeny     (501) staff       (20)      394 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/__init__.py
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.460634 django-livesettings3-1.6.2/livesettings/__pycache__/
--rw-r--r--   0 evgeny     (501) staff       (20)      565 2023-07-21 17:27:35.000000 django-livesettings3-1.6.2/livesettings/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 evgeny     (501) staff       (20)     1898 2023-07-30 00:55:57.000000 django-livesettings3-1.6.2/livesettings/__pycache__/forms.cpython-39.pyc
--rw-r--r--   0 evgeny     (501) staff       (20)     8564 2023-07-21 17:27:35.000000 django-livesettings3-1.6.2/livesettings/__pycache__/functions.cpython-39.pyc
--rw-r--r--   0 evgeny     (501) staff       (20)     7610 2023-07-21 17:27:35.000000 django-livesettings3-1.6.2/livesettings/__pycache__/models.cpython-39.pyc
--rw-r--r--   0 evgeny     (501) staff       (20)     1922 2023-07-21 17:27:35.000000 django-livesettings3-1.6.2/livesettings/__pycache__/overrides.cpython-39.pyc
--rw-r--r--   0 evgeny     (501) staff       (20)      256 2023-07-21 17:27:35.000000 django-livesettings3-1.6.2/livesettings/__pycache__/signals.cpython-39.pyc
--rw-r--r--   0 evgeny     (501) staff       (20)      639 2023-07-30 00:55:59.000000 django-livesettings3-1.6.2/livesettings/__pycache__/test_urls.cpython-39.pyc
--rw-r--r--   0 evgeny     (501) staff       (20)    28533 2023-07-30 00:55:58.000000 django-livesettings3-1.6.2/livesettings/__pycache__/tests.cpython-39.pyc
--rw-r--r--   0 evgeny     (501) staff       (20)      549 2023-07-30 00:55:58.000000 django-livesettings3-1.6.2/livesettings/__pycache__/urls.cpython-39.pyc
--rw-r--r--   0 evgeny     (501) staff       (20)     2557 2023-07-21 17:27:35.000000 django-livesettings3-1.6.2/livesettings/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0 evgeny     (501) staff       (20)    36310 2023-07-30 00:55:57.000000 django-livesettings3-1.6.2/livesettings/__pycache__/values.cpython-39.pyc
--rw-r--r--   0 evgeny     (501) staff       (20)     3341 2023-07-30 00:55:58.000000 django-livesettings3-1.6.2/livesettings/__pycache__/views.cpython-39.pyc
--rw-r--r--   0 evgeny     (501) staff       (20)     2359 2023-07-30 00:55:57.000000 django-livesettings3-1.6.2/livesettings/__pycache__/widgets.cpython-39.pyc
--rw-r--r--   0 evgeny     (501) staff       (20)     1994 2023-07-30 00:52:20.000000 django-livesettings3-1.6.2/livesettings/forms.py
--rw-r--r--   0 evgeny     (501) staff       (20)     7684 2023-07-14 19:51:10.000000 django-livesettings3-1.6.2/livesettings/functions.py
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.431501 django-livesettings3-1.6.2/livesettings/locale/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.427502 django-livesettings3-1.6.2/livesettings/locale/de/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.462057 django-livesettings3-1.6.2/livesettings/locale/de/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)      706 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 evgeny     (501) staff       (20)     2982 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.427848 django-livesettings3-1.6.2/livesettings/locale/en/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.463213 django-livesettings3-1.6.2/livesettings/locale/en/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)      367 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 evgeny     (501) staff       (20)     2878 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.428189 django-livesettings3-1.6.2/livesettings/locale/es/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.463745 django-livesettings3-1.6.2/livesettings/locale/es/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)        0 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.428532 django-livesettings3-1.6.2/livesettings/locale/fr/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.464662 django-livesettings3-1.6.2/livesettings/locale/fr/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)     1621 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 evgeny     (501) staff       (20)     3618 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.428878 django-livesettings3-1.6.2/livesettings/locale/he/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.465756 django-livesettings3-1.6.2/livesettings/locale/he/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)     1655 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/he/LC_MESSAGES/django.mo
--rw-r--r--   0 evgeny     (501) staff       (20)     2837 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/he/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.429187 django-livesettings3-1.6.2/livesettings/locale/it/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.466984 django-livesettings3-1.6.2/livesettings/locale/it/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)     1582 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 evgeny     (501) staff       (20)     3117 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.429534 django-livesettings3-1.6.2/livesettings/locale/ko/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.468167 django-livesettings3-1.6.2/livesettings/locale/ko/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)     1128 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/ko/LC_MESSAGES/django.mo
--rw-r--r--   0 evgeny     (501) staff       (20)     3110 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/ko/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.429927 django-livesettings3-1.6.2/livesettings/locale/pl/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.469210 django-livesettings3-1.6.2/livesettings/locale/pl/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)     1470 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 evgeny     (501) staff       (20)     2637 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.430259 django-livesettings3-1.6.2/livesettings/locale/pt_BR/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.470345 django-livesettings3-1.6.2/livesettings/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)     1208 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 evgeny     (501) staff       (20)     2645 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.430734 django-livesettings3-1.6.2/livesettings/locale/ru/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.471427 django-livesettings3-1.6.2/livesettings/locale/ru/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)     1178 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 evgeny     (501) staff       (20)     2470 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.431227 django-livesettings3-1.6.2/livesettings/locale/sv/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.472530 django-livesettings3-1.6.2/livesettings/locale/sv/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)     1481 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0 evgeny     (501) staff       (20)     2598 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.431676 django-livesettings3-1.6.2/livesettings/locale/tr/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.473571 django-livesettings3-1.6.2/livesettings/locale/tr/LC_MESSAGES/
--rw-r--r--   0 evgeny     (501) staff       (20)     1242 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 evgeny     (501) staff       (20)     3243 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.474562 django-livesettings3-1.6.2/livesettings/migrations/
--rw-r--r--   0 evgeny     (501) staff       (20)     1684 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/migrations/0001_initial.py
--rw-r--r--   0 evgeny     (501) staff       (20)        0 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/migrations/__init__.py
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.475335 django-livesettings3-1.6.2/livesettings/migrations/__pycache__/
--rw-r--r--   0 evgeny     (501) staff       (20)     1225 2023-07-21 17:28:00.000000 django-livesettings3-1.6.2/livesettings/migrations/__pycache__/0001_initial.cpython-39.pyc
--rw-r--r--   0 evgeny     (501) staff       (20)      174 2023-07-21 17:28:00.000000 django-livesettings3-1.6.2/livesettings/migrations/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 evgeny     (501) staff       (20)     7142 2023-07-14 19:51:10.000000 django-livesettings3-1.6.2/livesettings/models.py
--rw-r--r--   0 evgeny     (501) staff       (20)     1846 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/overrides.py
--rw-r--r--   0 evgeny     (501) staff       (20)       79 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/signals.py
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.432833 django-livesettings3-1.6.2/livesettings/static/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.433050 django-livesettings3-1.6.2/livesettings/static/livesettings/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.475758 django-livesettings3-1.6.2/livesettings/static/livesettings/js/
--rw-r--r--   0 evgeny     (501) staff       (20)    36012 2023-07-30 00:52:20.000000 django-livesettings3-1.6.2/livesettings/static/livesettings/js/string_array_widget.js
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.476683 django-livesettings3-1.6.2/livesettings/svelte/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.477655 django-livesettings3-1.6.2/livesettings/svelte/StringArrayWidget/
--rw-r--r--   0 evgeny     (501) staff       (20)     1857 2023-07-30 00:52:20.000000 django-livesettings3-1.6.2/livesettings/svelte/StringArrayWidget/StringArrayItem.svelte
--rw-r--r--   0 evgeny     (501) staff       (20)     3407 2023-07-30 00:52:20.000000 django-livesettings3-1.6.2/livesettings/svelte/StringArrayWidget/index.svelte
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.478078 django-livesettings3-1.6.2/livesettings/svelte/components/
--rw-r--r--   0 evgeny     (501) staff       (20)      379 2023-07-30 00:52:20.000000 django-livesettings3-1.6.2/livesettings/svelte/components/Dots.svelte
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.478874 django-livesettings3-1.6.2/livesettings/svelte/icons/
--rw-r--r--   0 evgeny     (501) staff       (20)      419 2023-07-30 00:52:20.000000 django-livesettings3-1.6.2/livesettings/svelte/icons/Cross.svelte
--rw-r--r--   0 evgeny     (501) staff       (20)      670 2023-07-30 00:52:20.000000 django-livesettings3-1.6.2/livesettings/svelte/icons/DragHandleDots.svelte
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.479328 django-livesettings3-1.6.2/livesettings/svelte/lib/
--rw-r--r--   0 evgeny     (501) staff       (20)       47 2023-07-30 00:52:20.000000 django-livesettings3-1.6.2/livesettings/svelte/lib/actions.js
--rw-r--r--   0 evgeny     (501) staff       (20)      393 2023-07-30 00:52:20.000000 django-livesettings3-1.6.2/livesettings/svelte/package.json
--rw-r--r--   0 evgeny     (501) staff       (20)      562 2023-07-30 00:52:20.000000 django-livesettings3-1.6.2/livesettings/svelte/rollup.config.mjs
--rw-r--r--   0 evgeny     (501) staff       (20)    21536 2023-07-30 00:52:20.000000 django-livesettings3-1.6.2/livesettings/svelte/yarn.lock
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.437808 django-livesettings3-1.6.2/livesettings/templates/
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.481913 django-livesettings3-1.6.2/livesettings/templates/livesettings/
--rw-r--r--   0 evgeny     (501) staff       (20)      437 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/templates/livesettings/_admin_site_views.html
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.482241 django-livesettings3-1.6.2/livesettings/templates/livesettings/form_widgets/
--rw-r--r--   0 evgeny     (501) staff       (20)      636 2023-07-30 00:52:20.000000 django-livesettings3-1.6.2/livesettings/templates/livesettings/form_widgets/string_array_widget.html
--rw-r--r--   0 evgeny     (501) staff       (20)     4901 2023-07-30 00:52:20.000000 django-livesettings3-1.6.2/livesettings/templates/livesettings/group_settings.html
--rw-r--r--   0 evgeny     (501) staff       (20)     3154 2023-07-20 23:55:47.000000 django-livesettings3-1.6.2/livesettings/templates/livesettings/group_settings.html.orig
--rw-r--r--   0 evgeny     (501) staff       (20)      878 2023-07-30 00:52:14.000000 django-livesettings3-1.6.2/livesettings/templates/livesettings/groups_navbar.html
--rw-r--r--   0 evgeny     (501) staff       (20)     6925 2023-07-30 00:52:20.000000 django-livesettings3-1.6.2/livesettings/templates/livesettings/site_settings.html
--rw-r--r--   0 evgeny     (501) staff       (20)       41 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/templates/livesettings/text.txt
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.482747 django-livesettings3-1.6.2/livesettings/templatetags/
--rw-r--r--   0 evgeny     (501) staff       (20)        0 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/templatetags/__init__.py
-drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 00:57:25.483595 django-livesettings3-1.6.2/livesettings/templatetags/__pycache__/
--rw-r--r--   0 evgeny     (501) staff       (20)      176 2023-07-21 17:28:00.000000 django-livesettings3-1.6.2/livesettings/templatetags/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 evgeny     (501) staff       (20)     2098 2023-07-21 17:28:00.000000 django-livesettings3-1.6.2/livesettings/templatetags/__pycache__/config_tags.cpython-39.pyc
--rw-r--r--   0 evgeny     (501) staff       (20)     2142 2023-07-14 19:51:10.000000 django-livesettings3-1.6.2/livesettings/templatetags/config_tags.py
--rw-r--r--   0 evgeny     (501) staff       (20)      447 2023-07-30 00:52:14.000000 django-livesettings3-1.6.2/livesettings/test_urls.py
--rw-r--r--   0 evgeny     (501) staff       (20)    29460 2023-07-30 00:52:14.000000 django-livesettings3-1.6.2/livesettings/tests.py
--rw-r--r--   0 evgeny     (501) staff       (20)      392 2023-07-30 00:52:14.000000 django-livesettings3-1.6.2/livesettings/urls.py
--rw-r--r--   0 evgeny     (501) staff       (20)     2131 2022-02-10 21:13:39.000000 django-livesettings3-1.6.2/livesettings/utils.py
--rw-r--r--   0 evgeny     (501) staff       (20)    35615 2023-07-30 00:52:20.000000 django-livesettings3-1.6.2/livesettings/values.py
--rw-r--r--   0 evgeny     (501) staff       (20)    33758 2023-07-19 23:59:41.000000 django-livesettings3-1.6.2/livesettings/values.py.orig
--rw-r--r--   0 evgeny     (501) staff       (20)     4706 2023-07-30 00:52:14.000000 django-livesettings3-1.6.2/livesettings/views.py
--rw-r--r--   0 evgeny     (501) staff       (20)     1782 2023-07-30 00:52:20.000000 django-livesettings3-1.6.2/livesettings/widgets.py
--rw-r--r--   0 evgeny     (501) staff       (20)     1135 2023-07-19 23:59:41.000000 django-livesettings3-1.6.2/livesettings/widgets.py.orig
--rw-r--r--   0 evgeny     (501) staff       (20)       79 2023-07-30 00:57:25.484519 django-livesettings3-1.6.2/setup.cfg
--rw-r--r--   0 evgeny     (501) staff       (20)     1297 2023-07-30 00:53:29.000000 django-livesettings3-1.6.2/setup.py
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.690402 django-livesettings3-1.6.3/
+-rw-r--r--   0 evgeny     (501) staff       (20)       88 2022-02-10 21:13:39.000000 django-livesettings3-1.6.3/AUTHORS
+-rw-r--r--   0 evgeny     (501) staff       (20)     1498 2022-02-10 21:13:39.000000 django-livesettings3-1.6.3/LICENSE
+-rw-r--r--   0 evgeny     (501) staff       (20)       93 2023-07-30 00:53:02.000000 django-livesettings3-1.6.3/MANIFEST.in
+-rw-r--r--   0 evgeny     (501) staff       (20)     1000 2023-07-30 01:36:24.690551 django-livesettings3-1.6.3/PKG-INFO
+-rw-r--r--   0 evgeny     (501) staff       (20)     5910 2023-07-30 00:52:14.000000 django-livesettings3-1.6.3/README.md
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.637298 django-livesettings3-1.6.3/django_livesettings3.egg-info/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1000 2023-07-30 01:36:24.000000 django-livesettings3-1.6.3/django_livesettings3.egg-info/PKG-INFO
+-rw-r--r--   0 evgeny     (501) staff       (20)     3588 2023-07-30 01:36:24.000000 django-livesettings3-1.6.3/django_livesettings3.egg-info/SOURCES.txt
+-rw-r--r--   0 evgeny     (501) staff       (20)        1 2023-07-30 01:36:24.000000 django-livesettings3-1.6.3/django_livesettings3.egg-info/dependency_links.txt
+-rw-r--r--   0 evgeny     (501) staff       (20)        1 2023-07-24 21:10:38.000000 django-livesettings3-1.6.3/django_livesettings3.egg-info/not-zip-safe
+-rw-r--r--   0 evgeny     (501) staff       (20)       34 2023-07-30 01:36:24.000000 django-livesettings3-1.6.3/django_livesettings3.egg-info/requires.txt
+-rw-r--r--   0 evgeny     (501) staff       (20)       13 2023-07-30 01:36:24.000000 django-livesettings3-1.6.3/django_livesettings3.egg-info/top_level.txt
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.649029 django-livesettings3-1.6.3/livesettings/
+-rw-r--r--   0 evgeny     (501) staff       (20)      394 2022-02-10 21:13:39.000000 django-livesettings3-1.6.3/livesettings/__init__.py
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.657592 django-livesettings3-1.6.3/livesettings/__pycache__/
+-rw-r--r--   0 evgeny     (501) staff       (20)      565 2023-07-21 17:27:35.000000 django-livesettings3-1.6.3/livesettings/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 evgeny     (501) staff       (20)     1898 2023-07-30 00:55:57.000000 django-livesettings3-1.6.3/livesettings/__pycache__/forms.cpython-39.pyc
+-rw-r--r--   0 evgeny     (501) staff       (20)     8564 2023-07-21 17:27:35.000000 django-livesettings3-1.6.3/livesettings/__pycache__/functions.cpython-39.pyc
+-rw-r--r--   0 evgeny     (501) staff       (20)     7610 2023-07-21 17:27:35.000000 django-livesettings3-1.6.3/livesettings/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0 evgeny     (501) staff       (20)     1922 2023-07-21 17:27:35.000000 django-livesettings3-1.6.3/livesettings/__pycache__/overrides.cpython-39.pyc
+-rw-r--r--   0 evgeny     (501) staff       (20)      256 2023-07-21 17:27:35.000000 django-livesettings3-1.6.3/livesettings/__pycache__/signals.cpython-39.pyc
+-rw-r--r--   0 evgeny     (501) staff       (20)      639 2023-07-30 00:55:59.000000 django-livesettings3-1.6.3/livesettings/__pycache__/test_urls.cpython-39.pyc
+-rw-r--r--   0 evgeny     (501) staff       (20)    28533 2023-07-30 00:55:58.000000 django-livesettings3-1.6.3/livesettings/__pycache__/tests.cpython-39.pyc
+-rw-r--r--   0 evgeny     (501) staff       (20)      549 2023-07-30 00:55:58.000000 django-livesettings3-1.6.3/livesettings/__pycache__/urls.cpython-39.pyc
+-rw-r--r--   0 evgeny     (501) staff       (20)     2557 2023-07-21 17:27:35.000000 django-livesettings3-1.6.3/livesettings/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0 evgeny     (501) staff       (20)    36310 2023-07-30 00:55:57.000000 django-livesettings3-1.6.3/livesettings/__pycache__/values.cpython-39.pyc
+-rw-r--r--   0 evgeny     (501) staff       (20)     3341 2023-07-30 00:55:58.000000 django-livesettings3-1.6.3/livesettings/__pycache__/views.cpython-39.pyc
+-rw-r--r--   0 evgeny     (501) staff       (20)     2359 2023-07-30 00:55:57.000000 django-livesettings3-1.6.3/livesettings/__pycache__/widgets.cpython-39.pyc
+-rw-r--r--   0 evgeny     (501) staff       (20)     1994 2023-07-30 00:52:20.000000 django-livesettings3-1.6.3/livesettings/forms.py
+-rw-r--r--   0 evgeny     (501) staff       (20)     7684 2023-07-14 19:51:10.000000 django-livesettings3-1.6.3/livesettings/functions.py
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.624985 django-livesettings3-1.6.3/livesettings/locale/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.620386 django-livesettings3-1.6.3/livesettings/locale/de/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.659093 django-livesettings3-1.6.3/livesettings/locale/de/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)      706 2022-02-10 21:13:39.000000 django-livesettings3-1.6.3/livesettings/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 evgeny     (501) staff       (20)     2982 2022-02-10 21:13:39.000000 django-livesettings3-1.6.3/livesettings/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.620741 django-livesettings3-1.6.3/livesettings/locale/en/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.660657 django-livesettings3-1.6.3/livesettings/locale/en/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)      367 2022-02-10 21:13:39.000000 django-livesettings3-1.6.3/livesettings/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 evgeny     (501) staff       (20)     2878 2022-02-10 21:13:39.000000 django-livesettings3-1.6.3/livesettings/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.621116 django-livesettings3-1.6.3/livesettings/locale/es/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.661342 django-livesettings3-1.6.3/livesettings/locale/es/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)        0 2022-02-10 21:13:39.000000 django-livesettings3-1.6.3/livesettings/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.621485 django-livesettings3-1.6.3/livesettings/locale/fr/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.662303 django-livesettings3-1.6.3/livesettings/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1621 2022-02-10 21:13:39.000000 django-livesettings3-1.6.3/livesettings/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 evgeny     (501) staff       (20)     3618 2022-02-10 21:13:39.000000 django-livesettings3-1.6.3/livesettings/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.621837 django-livesettings3-1.6.3/livesettings/locale/he/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.663677 django-livesettings3-1.6.3/livesettings/locale/he/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1655 2022-02-10 21:13:39.000000 django-livesettings3-1.6.3/livesettings/locale/he/LC_MESSAGES/django.mo
+-rw-r--r--   0 evgeny     (501) staff       (20)     2837 2022-02-10 21:13:39.000000 django-livesettings3-1.6.3/livesettings/locale/he/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.622195 django-livesettings3-1.6.3/livesettings/locale/it/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.665172 django-livesettings3-1.6.3/livesettings/locale/it/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1582 2022-02-10 21:13:39.000000 django-livesettings3-1.6.3/livesettings/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 evgeny     (501) staff       (20)     3117 2022-02-10 21:13:39.000000 django-livesettings3-1.6.3/livesettings/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.622558 django-livesettings3-1.6.3/livesettings/locale/ko/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.666355 django-livesettings3-1.6.3/livesettings/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1128 2022-02-10 21:13:39.000000 django-livesettings3-1.6.3/livesettings/locale/ko/LC_MESSAGES/django.mo
+-rw-r--r--   0 evgeny     (501) staff       (20)     3110 2022-02-10 21:13:39.000000 django-livesettings3-1.6.3/livesettings/locale/ko/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.622955 django-livesettings3-1.6.3/livesettings/locale/pl/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.667616 django-livesettings3-1.6.3/livesettings/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1470 2022-02-10 21:13:39.000000 django-livesettings3-1.6.3/livesettings/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 evgeny     (501) staff       (20)     2637 2022-02-10 21:13:39.000000 django-livesettings3-1.6.3/livesettings/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.623486 django-livesettings3-1.6.3/livesettings/locale/pt_BR/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.668837 django-livesettings3-1.6.3/livesettings/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1208 2022-02-10 21:13:39.000000 django-livesettings3-1.6.3/livesettings/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 evgeny     (501) staff       (20)     2645 2022-02-10 21:13:39.000000 django-livesettings3-1.6.3/livesettings/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.624051 django-livesettings3-1.6.3/livesettings/locale/ru/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.669981 django-livesettings3-1.6.3/livesettings/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1178 2022-02-10 21:13:39.000000 django-livesettings3-1.6.3/livesettings/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 evgeny     (501) staff       (20)     2470 2022-02-10 21:13:39.000000 django-livesettings3-1.6.3/livesettings/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.624671 django-livesettings3-1.6.3/livesettings/locale/sv/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.671048 django-livesettings3-1.6.3/livesettings/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1481 2022-02-10 21:13:39.000000 django-livesettings3-1.6.3/livesettings/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0 evgeny     (501) staff       (20)     2598 2022-02-10 21:13:39.000000 django-livesettings3-1.6.3/livesettings/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.625229 django-livesettings3-1.6.3/livesettings/locale/tr/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.672248 django-livesettings3-1.6.3/livesettings/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1242 2022-02-10 21:13:39.000000 django-livesettings3-1.6.3/livesettings/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 evgeny     (501) staff       (20)     3243 2022-02-10 21:13:39.000000 django-livesettings3-1.6.3/livesettings/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.673413 django-livesettings3-1.6.3/livesettings/migrations/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1684 2022-02-10 21:13:39.000000 django-livesettings3-1.6.3/livesettings/migrations/0001_initial.py
+-rw-r--r--   0 evgeny     (501) staff       (20)        0 2022-02-10 21:13:39.000000 django-livesettings3-1.6.3/livesettings/migrations/__init__.py
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.674799 django-livesettings3-1.6.3/livesettings/migrations/__pycache__/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1225 2023-07-21 17:28:00.000000 django-livesettings3-1.6.3/livesettings/migrations/__pycache__/0001_initial.cpython-39.pyc
+-rw-r--r--   0 evgeny     (501) staff       (20)      174 2023-07-21 17:28:00.000000 django-livesettings3-1.6.3/livesettings/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 evgeny     (501) staff       (20)     7142 2023-07-14 19:51:10.000000 django-livesettings3-1.6.3/livesettings/models.py
+-rw-r--r--   0 evgeny     (501) staff       (20)     1846 2022-02-10 21:13:39.000000 django-livesettings3-1.6.3/livesettings/overrides.py
+-rw-r--r--   0 evgeny     (501) staff       (20)       79 2022-02-10 21:13:39.000000 django-livesettings3-1.6.3/livesettings/signals.py
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.626392 django-livesettings3-1.6.3/livesettings/static/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.626620 django-livesettings3-1.6.3/livesettings/static/livesettings/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.675630 django-livesettings3-1.6.3/livesettings/static/livesettings/js/
+-rw-r--r--   0 evgeny     (501) staff       (20)    36012 2023-07-30 00:52:20.000000 django-livesettings3-1.6.3/livesettings/static/livesettings/js/string_array_widget.js
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.678353 django-livesettings3-1.6.3/livesettings/svelte/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.679765 django-livesettings3-1.6.3/livesettings/svelte/StringArrayWidget/
+-rw-r--r--   0 evgeny     (501) staff       (20)     1857 2023-07-30 00:52:20.000000 django-livesettings3-1.6.3/livesettings/svelte/StringArrayWidget/StringArrayItem.svelte
+-rw-r--r--   0 evgeny     (501) staff       (20)     3407 2023-07-30 00:52:20.000000 django-livesettings3-1.6.3/livesettings/svelte/StringArrayWidget/index.svelte
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.680296 django-livesettings3-1.6.3/livesettings/svelte/components/
+-rw-r--r--   0 evgeny     (501) staff       (20)      379 2023-07-30 00:52:20.000000 django-livesettings3-1.6.3/livesettings/svelte/components/Dots.svelte
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.681429 django-livesettings3-1.6.3/livesettings/svelte/icons/
+-rw-r--r--   0 evgeny     (501) staff       (20)      419 2023-07-30 00:52:20.000000 django-livesettings3-1.6.3/livesettings/svelte/icons/Cross.svelte
+-rw-r--r--   0 evgeny     (501) staff       (20)      670 2023-07-30 00:52:20.000000 django-livesettings3-1.6.3/livesettings/svelte/icons/DragHandleDots.svelte
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.682117 django-livesettings3-1.6.3/livesettings/svelte/lib/
+-rw-r--r--   0 evgeny     (501) staff       (20)       47 2023-07-30 00:52:20.000000 django-livesettings3-1.6.3/livesettings/svelte/lib/actions.js
+-rw-r--r--   0 evgeny     (501) staff       (20)      393 2023-07-30 00:52:20.000000 django-livesettings3-1.6.3/livesettings/svelte/package.json
+-rw-r--r--   0 evgeny     (501) staff       (20)      562 2023-07-30 00:52:20.000000 django-livesettings3-1.6.3/livesettings/svelte/rollup.config.mjs
+-rw-r--r--   0 evgeny     (501) staff       (20)    21536 2023-07-30 00:52:20.000000 django-livesettings3-1.6.3/livesettings/svelte/yarn.lock
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.629088 django-livesettings3-1.6.3/livesettings/templates/
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.686351 django-livesettings3-1.6.3/livesettings/templates/livesettings/
+-rw-r--r--   0 evgeny     (501) staff       (20)      437 2022-02-10 21:13:39.000000 django-livesettings3-1.6.3/livesettings/templates/livesettings/_admin_site_views.html
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.686962 django-livesettings3-1.6.3/livesettings/templates/livesettings/form_widgets/
+-rw-r--r--   0 evgeny     (501) staff       (20)      636 2023-07-30 00:52:20.000000 django-livesettings3-1.6.3/livesettings/templates/livesettings/form_widgets/string_array_widget.html
+-rw-r--r--   0 evgeny     (501) staff       (20)     4901 2023-07-30 00:52:20.000000 django-livesettings3-1.6.3/livesettings/templates/livesettings/group_settings.html
+-rw-r--r--   0 evgeny     (501) staff       (20)     3154 2023-07-20 23:55:47.000000 django-livesettings3-1.6.3/livesettings/templates/livesettings/group_settings.html.orig
+-rw-r--r--   0 evgeny     (501) staff       (20)      878 2023-07-30 00:52:14.000000 django-livesettings3-1.6.3/livesettings/templates/livesettings/groups_navbar.html
+-rw-r--r--   0 evgeny     (501) staff       (20)     6925 2023-07-30 00:52:20.000000 django-livesettings3-1.6.3/livesettings/templates/livesettings/site_settings.html
+-rw-r--r--   0 evgeny     (501) staff       (20)       41 2022-02-10 21:13:39.000000 django-livesettings3-1.6.3/livesettings/templates/livesettings/text.txt
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.688040 django-livesettings3-1.6.3/livesettings/templatetags/
+-rw-r--r--   0 evgeny     (501) staff       (20)        0 2022-02-10 21:13:39.000000 django-livesettings3-1.6.3/livesettings/templatetags/__init__.py
+drwxr-xr-x   0 evgeny     (501) staff       (20)        0 2023-07-30 01:36:24.689711 django-livesettings3-1.6.3/livesettings/templatetags/__pycache__/
+-rw-r--r--   0 evgeny     (501) staff       (20)      176 2023-07-21 17:28:00.000000 django-livesettings3-1.6.3/livesettings/templatetags/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 evgeny     (501) staff       (20)     2098 2023-07-21 17:28:00.000000 django-livesettings3-1.6.3/livesettings/templatetags/__pycache__/config_tags.cpython-39.pyc
+-rw-r--r--   0 evgeny     (501) staff       (20)     2142 2023-07-14 19:51:10.000000 django-livesettings3-1.6.3/livesettings/templatetags/config_tags.py
+-rw-r--r--   0 evgeny     (501) staff       (20)      447 2023-07-30 00:52:14.000000 django-livesettings3-1.6.3/livesettings/test_urls.py
+-rw-r--r--   0 evgeny     (501) staff       (20)    29460 2023-07-30 00:52:14.000000 django-livesettings3-1.6.3/livesettings/tests.py
+-rw-r--r--   0 evgeny     (501) staff       (20)      392 2023-07-30 00:52:14.000000 django-livesettings3-1.6.3/livesettings/urls.py
+-rw-r--r--   0 evgeny     (501) staff       (20)     2131 2022-02-10 21:13:39.000000 django-livesettings3-1.6.3/livesettings/utils.py
+-rw-r--r--   0 evgeny     (501) staff       (20)    35556 2023-07-30 01:33:57.000000 django-livesettings3-1.6.3/livesettings/values.py
+-rw-r--r--   0 evgeny     (501) staff       (20)    33758 2023-07-19 23:59:41.000000 django-livesettings3-1.6.3/livesettings/values.py.orig
+-rw-r--r--   0 evgeny     (501) staff       (20)     4706 2023-07-30 00:52:14.000000 django-livesettings3-1.6.3/livesettings/views.py
+-rw-r--r--   0 evgeny     (501) staff       (20)     1782 2023-07-30 00:52:20.000000 django-livesettings3-1.6.3/livesettings/widgets.py
+-rw-r--r--   0 evgeny     (501) staff       (20)     1135 2023-07-19 23:59:41.000000 django-livesettings3-1.6.3/livesettings/widgets.py.orig
+-rw-r--r--   0 evgeny     (501) staff       (20)       79 2023-07-30 01:36:24.691203 django-livesettings3-1.6.3/setup.cfg
+-rw-r--r--   0 evgeny     (501) staff       (20)     1297 2023-07-30 01:35:02.000000 django-livesettings3-1.6.3/setup.py
```

### Comparing `django-livesettings3-1.6.2/LICENSE` & `django-livesettings3-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/PKG-INFO` & `django-livesettings3-1.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-livesettings3
-Version: 1.6.2
+Version: 1.6.3
 Summary: Python 3 port of django-livesettings
 Home-page: https://github.com/kunaldeo/django-livesettings3/
 Author: Kunal Deo
 Author-email: kunaldeo@gmail.com
 License: New BSD License
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-livesettings3-1.6.2/README.md` & `django-livesettings3-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/django_livesettings3.egg-info/PKG-INFO` & `django-livesettings3-1.6.3/django_livesettings3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-livesettings3
-Version: 1.6.2
+Version: 1.6.3
 Summary: Python 3 port of django-livesettings
 Home-page: https://github.com/kunaldeo/django-livesettings3/
 Author: Kunal Deo
 Author-email: kunaldeo@gmail.com
 License: New BSD License
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-livesettings3-1.6.2/django_livesettings3.egg-info/SOURCES.txt` & `django-livesettings3-1.6.3/django_livesettings3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/__pycache__/__init__.cpython-39.pyc` & `django-livesettings3-1.6.3/livesettings/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/__pycache__/forms.cpython-39.pyc` & `django-livesettings3-1.6.3/livesettings/__pycache__/forms.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/__pycache__/functions.cpython-39.pyc` & `django-livesettings3-1.6.3/livesettings/__pycache__/functions.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/__pycache__/models.cpython-39.pyc` & `django-livesettings3-1.6.3/livesettings/__pycache__/models.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/__pycache__/overrides.cpython-39.pyc` & `django-livesettings3-1.6.3/livesettings/__pycache__/overrides.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/__pycache__/test_urls.cpython-39.pyc` & `django-livesettings3-1.6.3/livesettings/__pycache__/test_urls.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/__pycache__/tests.cpython-39.pyc` & `django-livesettings3-1.6.3/livesettings/__pycache__/tests.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/__pycache__/urls.cpython-39.pyc` & `django-livesettings3-1.6.3/livesettings/__pycache__/urls.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/__pycache__/utils.cpython-39.pyc` & `django-livesettings3-1.6.3/livesettings/__pycache__/utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/__pycache__/values.cpython-39.pyc` & `django-livesettings3-1.6.3/livesettings/__pycache__/values.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/__pycache__/views.cpython-39.pyc` & `django-livesettings3-1.6.3/livesettings/__pycache__/views.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/__pycache__/widgets.cpython-39.pyc` & `django-livesettings3-1.6.3/livesettings/__pycache__/widgets.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/forms.py` & `django-livesettings3-1.6.3/livesettings/forms.py`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/functions.py` & `django-livesettings3-1.6.3/livesettings/functions.py`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/locale/de/LC_MESSAGES/django.mo` & `django-livesettings3-1.6.3/livesettings/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/locale/de/LC_MESSAGES/django.po` & `django-livesettings3-1.6.3/livesettings/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/locale/en/LC_MESSAGES/django.po` & `django-livesettings3-1.6.3/livesettings/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/locale/fr/LC_MESSAGES/django.mo` & `django-livesettings3-1.6.3/livesettings/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/locale/fr/LC_MESSAGES/django.po` & `django-livesettings3-1.6.3/livesettings/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/locale/he/LC_MESSAGES/django.mo` & `django-livesettings3-1.6.3/livesettings/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/locale/he/LC_MESSAGES/django.po` & `django-livesettings3-1.6.3/livesettings/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/locale/it/LC_MESSAGES/django.mo` & `django-livesettings3-1.6.3/livesettings/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/locale/it/LC_MESSAGES/django.po` & `django-livesettings3-1.6.3/livesettings/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/locale/ko/LC_MESSAGES/django.mo` & `django-livesettings3-1.6.3/livesettings/locale/ko/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/locale/ko/LC_MESSAGES/django.po` & `django-livesettings3-1.6.3/livesettings/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/locale/pl/LC_MESSAGES/django.mo` & `django-livesettings3-1.6.3/livesettings/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/locale/pl/LC_MESSAGES/django.po` & `django-livesettings3-1.6.3/livesettings/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/locale/pt_BR/LC_MESSAGES/django.mo` & `django-livesettings3-1.6.3/livesettings/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/locale/pt_BR/LC_MESSAGES/django.po` & `django-livesettings3-1.6.3/livesettings/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/locale/ru/LC_MESSAGES/django.mo` & `django-livesettings3-1.6.3/livesettings/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/locale/ru/LC_MESSAGES/django.po` & `django-livesettings3-1.6.3/livesettings/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/locale/sv/LC_MESSAGES/django.mo` & `django-livesettings3-1.6.3/livesettings/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/locale/sv/LC_MESSAGES/django.po` & `django-livesettings3-1.6.3/livesettings/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/locale/tr/LC_MESSAGES/django.mo` & `django-livesettings3-1.6.3/livesettings/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/locale/tr/LC_MESSAGES/django.po` & `django-livesettings3-1.6.3/livesettings/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/migrations/0001_initial.py` & `django-livesettings3-1.6.3/livesettings/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/migrations/__pycache__/0001_initial.cpython-39.pyc` & `django-livesettings3-1.6.3/livesettings/migrations/__pycache__/0001_initial.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/models.py` & `django-livesettings3-1.6.3/livesettings/models.py`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/overrides.py` & `django-livesettings3-1.6.3/livesettings/overrides.py`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/static/livesettings/js/string_array_widget.js` & `django-livesettings3-1.6.3/livesettings/static/livesettings/js/string_array_widget.js`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/svelte/StringArrayWidget/StringArrayItem.svelte` & `django-livesettings3-1.6.3/livesettings/svelte/StringArrayWidget/StringArrayItem.svelte`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/svelte/StringArrayWidget/index.svelte` & `django-livesettings3-1.6.3/livesettings/svelte/StringArrayWidget/index.svelte`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/svelte/icons/DragHandleDots.svelte` & `django-livesettings3-1.6.3/livesettings/svelte/icons/DragHandleDots.svelte`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/svelte/rollup.config.mjs` & `django-livesettings3-1.6.3/livesettings/svelte/rollup.config.mjs`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/svelte/yarn.lock` & `django-livesettings3-1.6.3/livesettings/svelte/yarn.lock`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/templates/livesettings/form_widgets/string_array_widget.html` & `django-livesettings3-1.6.3/livesettings/templates/livesettings/form_widgets/string_array_widget.html`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/templates/livesettings/group_settings.html` & `django-livesettings3-1.6.3/livesettings/templates/livesettings/group_settings.html`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/templates/livesettings/group_settings.html.orig` & `django-livesettings3-1.6.3/livesettings/templates/livesettings/group_settings.html.orig`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/templates/livesettings/groups_navbar.html` & `django-livesettings3-1.6.3/livesettings/templates/livesettings/groups_navbar.html`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/templates/livesettings/site_settings.html` & `django-livesettings3-1.6.3/livesettings/templates/livesettings/site_settings.html`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/templatetags/__pycache__/config_tags.cpython-39.pyc` & `django-livesettings3-1.6.3/livesettings/templatetags/__pycache__/config_tags.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/templatetags/config_tags.py` & `django-livesettings3-1.6.3/livesettings/templatetags/config_tags.py`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/tests.py` & `django-livesettings3-1.6.3/livesettings/tests.py`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/utils.py` & `django-livesettings3-1.6.3/livesettings/utils.py`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/values.py` & `django-livesettings3-1.6.3/livesettings/values.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 try:
     import json
 except ImportError:
     from django.utils import simplejson as json
 
 from django import forms
 from django.conf import settings as djangosettings
-from django.contrib.postgres.forms import SimpleArrayField
 from django.core.exceptions import ImproperlyConfigured
 from django.core.files import storage
 from django.db import connection, DatabaseError
 from django.utils.encoding import smart_str
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext, gettext_lazy as _
 from django.utils.translation import get_language as _get_language
```

### Comparing `django-livesettings3-1.6.2/livesettings/values.py.orig` & `django-livesettings3-1.6.3/livesettings/values.py.orig`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/views.py` & `django-livesettings3-1.6.3/livesettings/views.py`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/widgets.py` & `django-livesettings3-1.6.3/livesettings/widgets.py`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/livesettings/widgets.py.orig` & `django-livesettings3-1.6.3/livesettings/widgets.py.orig`

 * *Files identical despite different names*

### Comparing `django-livesettings3-1.6.2/setup.py` & `django-livesettings3-1.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django-livesettings3',
-    version='1.6.2',
+    version='1.6.3',
     description="Python 3 port of django-livesettings",
     long_description="""Python 3 version of django live settings. It provides the ability to configure settings via an admin interface, rather than by editing "settings.py". Documentation avaiable at Github.""",
     author='Kunal Deo',
     author_email='kunaldeo@gmail.com',
     url='https://github.com/kunaldeo/django-livesettings3/',
     license='New BSD License',
     platforms=['any'],
```

