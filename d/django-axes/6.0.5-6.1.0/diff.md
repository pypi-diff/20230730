# Comparing `tmp/django-axes-6.0.5.tar.gz` & `tmp/django-axes-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-axes-6.0.5.tar", last modified: Fri Jun 30 21:07:57 2023, max compression
+gzip compressed data, was "django-axes-6.1.0.tar", last modified: Sun Jul 30 16:04:42 2023, max compression
```

## Comparing `django-axes-6.0.5.tar` & `django-axes-6.1.0.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.525846 django-axes-6.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.509846 django-axes-6.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.513846 django-axes-6.0.5/.github/ISSUE_TEMPLATES/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-30 21:07:43.000000 django-axes-6.0.5/.github/ISSUE_TEMPLATES/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-30 21:07:43.000000 django-axes-6.0.5/.github/ISSUE_TEMPLATES/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-30 21:07:43.000000 django-axes-6.0.5/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-30 21:07:43.000000 django-axes-6.0.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.513846 django-axes-6.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-30 21:07:43.000000 django-axes-6.0.5/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-30 21:07:43.000000 django-axes-6.0.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-30 21:07:43.000000 django-axes-6.0.5/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-30 21:07:43.000000 django-axes-6.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-30 21:07:43.000000 django-axes-6.0.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-30 21:07:43.000000 django-axes-6.0.5/.prospector.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    32723 2023-06-30 21:07:43.000000 django-axes-6.0.5/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-30 21:07:43.000000 django-axes-6.0.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-30 21:07:43.000000 django-axes-6.0.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-30 21:07:43.000000 django-axes-6.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    36937 2023-06-30 21:07:57.521846 django-axes-6.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-30 21:07:43.000000 django-axes-6.0.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.513846 django-axes-6.0.5/axes/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/attempts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.513846 django-axes-6.0.5/axes/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/handlers/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    13006 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/handlers/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/handlers/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/handlers/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/handlers/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    21297 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.509846 django-axes-6.0.5/axes/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.509846 django-axes-6.0.5/axes/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.513846 django-axes-6.0.5/axes/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.509846 django-axes-6.0.5/axes/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.513846 django-axes-6.0.5/axes/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.509846 django-axes-6.0.5/axes/locale/id/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.513846 django-axes-6.0.5/axes/locale/id/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/locale/id/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/locale/id/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.509846 django-axes-6.0.5/axes/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.513846 django-axes-6.0.5/axes/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.509846 django-axes-6.0.5/axes/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.517846 django-axes-6.0.5/axes/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.509846 django-axes-6.0.5/axes/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.517846 django-axes-6.0.5/axes/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.517846 django-axes-6.0.5/axes/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.517846 django-axes-6.0.5/axes/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/management/commands/axes_list_attempts.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/management/commands/axes_reset.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/management/commands/axes_reset_failure_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/management/commands/axes_reset_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/management/commands/axes_reset_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/management/commands/axes_reset_username.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.517846 django-axes-6.0.5/axes/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/migrations/0002_auto_20151217_2044.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/migrations/0003_auto_20160322_0929.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/migrations/0004_auto_20181024_1538.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/migrations/0005_remove_accessattempt_trusted.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/migrations/0006_remove_accesslog_trusted.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/migrations/0007_alter_accessattempt_unique_together.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/migrations/0008_accessfailurelog.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-30 21:07:43.000000 django-axes-6.0.5/axes/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-30 21:07:43.000000 django-axes-6.0.5/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.517846 django-axes-6.0.5/django_axes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36937 2023-06-30 21:07:57.000000 django-axes-6.0.5/django_axes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-06-30 21:07:57.000000 django-axes-6.0.5/django_axes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 21:07:57.000000 django-axes-6.0.5/django_axes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 21:07:57.000000 django-axes-6.0.5/django_axes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-30 21:07:57.000000 django-axes-6.0.5/django_axes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-30 21:07:57.000000 django-axes-6.0.5/django_axes.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.521846 django-axes-6.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-30 21:07:43.000000 django-axes-6.0.5/docs/10_changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-30 21:07:43.000000 django-axes-6.0.5/docs/1_requirements.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-06-30 21:07:43.000000 django-axes-6.0.5/docs/2_installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-30 21:07:43.000000 django-axes-6.0.5/docs/3_usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)    64873 2023-06-30 21:07:43.000000 django-axes-6.0.5/docs/4_configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-06-30 21:07:43.000000 django-axes-6.0.5/docs/5_customization.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-06-30 21:07:43.000000 django-axes-6.0.5/docs/6_integration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-30 21:07:43.000000 django-axes-6.0.5/docs/7_architecture.rst
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-30 21:07:43.000000 django-axes-6.0.5/docs/8_reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-30 21:07:43.000000 django-axes-6.0.5/docs/9_contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-06-30 21:07:44.000000 django-axes-6.0.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-06-30 21:07:44.000000 django-axes-6.0.5/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.521846 django-axes-6.0.5/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)   133029 2023-06-30 21:07:44.000000 django-axes-6.0.5/docs/images/flow.png
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-30 21:07:44.000000 django-axes-6.0.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-30 21:07:44.000000 django-axes-6.0.5/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-30 21:07:44.000000 django-axes-6.0.5/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-30 21:07:44.000000 django-axes-6.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-30 21:07:44.000000 django-axes-6.0.5/requirements-qa.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-30 21:07:44.000000 django-axes-6.0.5/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-30 21:07:44.000000 django-axes-6.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 21:07:57.525846 django-axes-6.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-30 21:07:44.000000 django-axes-6.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:57.521846 django-axes-6.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/test_attempts.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/test_failures.py
--rw-r--r--   0 runner    (1001) docker     (123)    22313 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    39363 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    38226 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/test_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/test_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-30 21:07:44.000000 django-axes-6.0.5/tests/urls_empty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:04:42.214688 django-axes-6.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:04:42.194687 django-axes-6.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:04:42.194687 django-axes-6.1.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-30 16:04:25.000000 django-axes-6.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-30 16:04:25.000000 django-axes-6.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-30 16:04:25.000000 django-axes-6.1.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-30 16:04:25.000000 django-axes-6.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:04:42.194687 django-axes-6.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-30 16:04:25.000000 django-axes-6.1.0/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-30 16:04:25.000000 django-axes-6.1.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-30 16:04:25.000000 django-axes-6.1.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-30 16:04:25.000000 django-axes-6.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-30 16:04:25.000000 django-axes-6.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-30 16:04:25.000000 django-axes-6.1.0/.prospector.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    33301 2023-07-30 16:04:25.000000 django-axes-6.1.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-30 16:04:25.000000 django-axes-6.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-30 16:04:25.000000 django-axes-6.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-30 16:04:25.000000 django-axes-6.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    37515 2023-07-30 16:04:42.206688 django-axes-6.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-30 16:04:25.000000 django-axes-6.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:04:42.194687 django-axes-6.1.0/axes/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/attempts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:04:42.198688 django-axes-6.1.0/axes/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/handlers/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13006 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/handlers/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/handlers/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/handlers/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/handlers/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21310 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:04:42.190688 django-axes-6.1.0/axes/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:04:42.190688 django-axes-6.1.0/axes/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:04:42.198688 django-axes-6.1.0/axes/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:04:42.190688 django-axes-6.1.0/axes/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:04:42.198688 django-axes-6.1.0/axes/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:04:42.190688 django-axes-6.1.0/axes/locale/id/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:04:42.198688 django-axes-6.1.0/axes/locale/id/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:04:42.190688 django-axes-6.1.0/axes/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:04:42.198688 django-axes-6.1.0/axes/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:04:42.190688 django-axes-6.1.0/axes/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:04:42.198688 django-axes-6.1.0/axes/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:04:42.190688 django-axes-6.1.0/axes/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:04:42.198688 django-axes-6.1.0/axes/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:04:42.198688 django-axes-6.1.0/axes/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:04:42.198688 django-axes-6.1.0/axes/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/management/commands/axes_list_attempts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/management/commands/axes_reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/management/commands/axes_reset_failure_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/management/commands/axes_reset_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/management/commands/axes_reset_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/management/commands/axes_reset_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:04:42.202688 django-axes-6.1.0/axes/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/migrations/0002_auto_20151217_2044.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/migrations/0003_auto_20160322_0929.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/migrations/0004_auto_20181024_1538.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/migrations/0005_remove_accessattempt_trusted.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/migrations/0006_remove_accesslog_trusted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/migrations/0007_alter_accessattempt_unique_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/migrations/0008_accessfailurelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-30 16:04:25.000000 django-axes-6.1.0/axes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-30 16:04:25.000000 django-axes-6.1.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:04:42.202688 django-axes-6.1.0/django_axes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    37515 2023-07-30 16:04:42.000000 django-axes-6.1.0/django_axes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-30 16:04:42.000000 django-axes-6.1.0/django_axes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 16:04:42.000000 django-axes-6.1.0/django_axes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 16:04:42.000000 django-axes-6.1.0/django_axes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-30 16:04:42.000000 django-axes-6.1.0/django_axes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-30 16:04:42.000000 django-axes-6.1.0/django_axes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:04:42.202688 django-axes-6.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-30 16:04:25.000000 django-axes-6.1.0/docs/10_changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-30 16:04:25.000000 django-axes-6.1.0/docs/1_requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-07-30 16:04:25.000000 django-axes-6.1.0/docs/2_installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-07-30 16:04:25.000000 django-axes-6.1.0/docs/3_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    64873 2023-07-30 16:04:25.000000 django-axes-6.1.0/docs/4_configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-07-30 16:04:25.000000 django-axes-6.1.0/docs/5_customization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-07-30 16:04:25.000000 django-axes-6.1.0/docs/6_integration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-07-30 16:04:25.000000 django-axes-6.1.0/docs/7_architecture.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-30 16:04:25.000000 django-axes-6.1.0/docs/8_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-30 16:04:25.000000 django-axes-6.1.0/docs/9_contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-07-30 16:04:25.000000 django-axes-6.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-07-30 16:04:25.000000 django-axes-6.1.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:04:42.202688 django-axes-6.1.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   133029 2023-07-30 16:04:25.000000 django-axes-6.1.0/docs/images/flow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-30 16:04:25.000000 django-axes-6.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-30 16:04:25.000000 django-axes-6.1.0/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-30 16:04:25.000000 django-axes-6.1.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-30 16:04:25.000000 django-axes-6.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-30 16:04:25.000000 django-axes-6.1.0/requirements-qa.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-30 16:04:25.000000 django-axes-6.1.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-30 16:04:25.000000 django-axes-6.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 16:04:42.214688 django-axes-6.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-30 16:04:25.000000 django-axes-6.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:04:42.206688 django-axes-6.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 16:04:25.000000 django-axes-6.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-07-30 16:04:25.000000 django-axes-6.1.0/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-30 16:04:25.000000 django-axes-6.1.0/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-30 16:04:25.000000 django-axes-6.1.0/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-07-30 16:04:25.000000 django-axes-6.1.0/tests/test_attempts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-30 16:04:25.000000 django-axes-6.1.0/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-30 16:04:25.000000 django-axes-6.1.0/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-30 16:04:25.000000 django-axes-6.1.0/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-30 16:04:25.000000 django-axes-6.1.0/tests/test_failures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22313 2023-07-30 16:04:25.000000 django-axes-6.1.0/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39534 2023-07-30 16:04:25.000000 django-axes-6.1.0/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-07-30 16:04:25.000000 django-axes-6.1.0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38226 2023-07-30 16:04:25.000000 django-axes-6.1.0/tests/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-07-30 16:04:25.000000 django-axes-6.1.0/tests/test_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-30 16:04:25.000000 django-axes-6.1.0/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-30 16:04:25.000000 django-axes-6.1.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-30 16:04:25.000000 django-axes-6.1.0/tests/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-30 16:04:25.000000 django-axes-6.1.0/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-30 16:04:25.000000 django-axes-6.1.0/tests/urls_empty.py
```

### Comparing `django-axes-6.0.5/.github/ISSUE_TEMPLATES/bug_report.md` & `django-axes-6.1.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ---
 name: Bug report
 about: Create a report to help us improve django-axes
 title: 'BUG: Short description of the problem'
 labels: 'bug'
 assignees: ''
+
 ---
 
 **Describe the bug**
 A clear and concise description of what the bug is.
 
 **To Reproduce**
 Steps to reproduce the behavior:
```

### Comparing `django-axes-6.0.5/.github/ISSUE_TEMPLATES/feature_request.md` & `django-axes-6.1.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ---
 name: Feature request
 about: Suggest an idea for django-axes
 title: 'FEATURE REQUEST: Short description of requested feature'
 labels: 'feature request'
 assignees: ''
+
 ---
 
 **Is your feature request related to a problem? Please describe.**
 A clear and concise description of what the problem is. Ex. I'm always frustrated when [...]
 
 **Describe the solution you'd like**
 A clear and concise description of what you want to happen.
```

### Comparing `django-axes-6.0.5/.github/PULL_REQUEST_TEMPLATE.md` & `django-axes-6.1.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/.github/workflows/codeql.yml` & `django-axes-6.1.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/.github/workflows/release.yml` & `django-axes-6.1.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/.github/workflows/test.yml` & `django-axes-6.1.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/CHANGES.rst` & `django-axes-6.1.0/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 
 Changes
 =======
 
 
+6.1.0 (2023-07-30)
+------------------
+
+- Set ``AXES_SENSITIVE_PARAMETERS`` default value to ``["username", "ip_address"]`` in addition to the ``AXES_PASSWORD_FORM_FIELD`` configuration flag.
+  This masks the username and IP address fields by default in the logs when writing information about login attempts to the application logs.
+  Reverting to old configuration default of ``[]`` can be done by setting ``AXES_SENSITIVE_PARAMETERS = []`` in the Django project settings file.
+  [GitRon]
+- Improve documentation on GDPR and privacy notes and configuration flags.
+  [GitRon]
+
+
 6.0.5 (2023-07-01)
 ------------------
 
 - Add Indonesion translation.
   [kiraware]
```

### Comparing `django-axes-6.0.5/CODE_OF_CONDUCT.md` & `django-axes-6.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/CONTRIBUTING.rst` & `django-axes-6.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/LICENSE` & `django-axes-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/PKG-INFO` & `django-axes-6.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-axes
-Version: 6.0.5
+Version: 6.1.0
 Summary: Keep track of failed login attempts in Django-powered sites.
 Home-page: https://github.com/jazzband/django-axes
 Author: Josh VanderLinden, Philip Neustrom, Michael Blume, Alex Clark, Camilo Nova, Aleksi Hakli
 Author-email: security@jazzband.co
 Maintainer: Jazzband
 Maintainer-email: security@jazzband.co
 License: MIT
@@ -123,14 +123,25 @@
 See `CONTRIBUTING <CONTRIBUTING.rst>`__.
 
 
 Changes
 =======
 
 
+6.1.0 (2023-07-30)
+------------------
+
+- Set ``AXES_SENSITIVE_PARAMETERS`` default value to ``["username", "ip_address"]`` in addition to the ``AXES_PASSWORD_FORM_FIELD`` configuration flag.
+  This masks the username and IP address fields by default in the logs when writing information about login attempts to the application logs.
+  Reverting to old configuration default of ``[]`` can be done by setting ``AXES_SENSITIVE_PARAMETERS = []`` in the Django project settings file.
+  [GitRon]
+- Improve documentation on GDPR and privacy notes and configuration flags.
+  [GitRon]
+
+
 6.0.5 (2023-07-01)
 ------------------
 
 - Add Indonesion translation.
   [kiraware]
```

### Comparing `django-axes-6.0.5/README.rst` & `django-axes-6.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/admin.py` & `django-axes-6.1.0/axes/admin.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/apps.py` & `django-axes-6.1.0/axes/apps.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/attempts.py` & `django-axes-6.1.0/axes/attempts.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/backends.py` & `django-axes-6.1.0/axes/backends.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/checks.py` & `django-axes-6.1.0/axes/checks.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/conf.py` & `django-axes-6.1.0/axes/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 # set CORS allowed origins when calling authentication over ajax
 settings.AXES_ALLOWED_CORS_ORIGINS = getattr(settings, "AXES_ALLOWED_CORS_ORIGINS", "*")
 
 # set the list of sensitive parameters to cleanse from get/post data before logging
 settings.AXES_SENSITIVE_PARAMETERS = getattr(
     settings,
     "AXES_SENSITIVE_PARAMETERS",
-    [],
+    ["username", "ip_address"],
 )
 
 # set the callable for the readable string that can be used in
 # e.g. logging to distinguish client requests
 settings.AXES_CLIENT_STR_CALLABLE = getattr(settings, "AXES_CLIENT_STR_CALLABLE", None)
 
 # set the HTTP response code given by too many requests
```

### Comparing `django-axes-6.0.5/axes/decorators.py` & `django-axes-6.1.0/axes/decorators.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/handlers/base.py` & `django-axes-6.1.0/axes/handlers/base.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/handlers/cache.py` & `django-axes-6.1.0/axes/handlers/cache.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/handlers/database.py` & `django-axes-6.1.0/axes/handlers/database.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/handlers/dummy.py` & `django-axes-6.1.0/axes/handlers/dummy.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/handlers/proxy.py` & `django-axes-6.1.0/axes/handlers/proxy.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/handlers/test.py` & `django-axes-6.1.0/axes/handlers/test.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/helpers.py` & `django-axes-6.1.0/axes/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 def get_cache_timeout() -> Optional[int]:
     """
     Return the cache timeout interpreted from settings.AXES_COOLOFF_TIME.
 
     The cache timeout can be either None if not configured or integer of seconds if configured.
 
-    Notice that the settings.AXES_COOLOFF_TIME can be None, timedelta, integer, callable, or str path,
+    Notice that the settings.AXES_COOLOFF_TIME can be None, timedelta, float, integer, callable, or str path,
     and this function offers a unified _integer or None_ representation of that configuration
     for use with the Django cache backends.
     """
 
     cool_off = get_cool_off()
     if cool_off is None:
         return None
@@ -50,15 +50,15 @@
 
 def get_cool_off() -> Optional[timedelta]:
     """
     Return the login cool off time interpreted from settings.AXES_COOLOFF_TIME.
 
     The return value is either None or timedelta.
 
-    Notice that the settings.AXES_COOLOFF_TIME is either None, timedelta, or integer of hours,
+    Notice that the settings.AXES_COOLOFF_TIME is either None, timedelta, or integer/float of hours,
     and this function offers a unified _timedelta or None_ representation of that configuration
     for use with the Axes internal implementations.
 
     :exception TypeError: if settings.AXES_COOLOFF_TIME is of wrong type.
     """
 
     cool_off = settings.AXES_COOLOFF_TIME
```

### Comparing `django-axes-6.0.5/axes/locale/ar/LC_MESSAGES/django.mo` & `django-axes-6.1.0/axes/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/locale/ar/LC_MESSAGES/django.po` & `django-axes-6.1.0/axes/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/locale/de/LC_MESSAGES/django.mo` & `django-axes-6.1.0/axes/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/locale/de/LC_MESSAGES/django.po` & `django-axes-6.1.0/axes/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/locale/id/LC_MESSAGES/django.mo` & `django-axes-6.1.0/axes/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/locale/id/LC_MESSAGES/django.po` & `django-axes-6.1.0/axes/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/locale/pl/LC_MESSAGES/django.mo` & `django-axes-6.1.0/axes/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/locale/pl/LC_MESSAGES/django.po` & `django-axes-6.1.0/axes/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/locale/ru/LC_MESSAGES/django.mo` & `django-axes-6.1.0/axes/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/locale/ru/LC_MESSAGES/django.po` & `django-axes-6.1.0/axes/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/locale/tr/LC_MESSAGES/django.mo` & `django-axes-6.1.0/axes/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/locale/tr/LC_MESSAGES/django.po` & `django-axes-6.1.0/axes/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/management/commands/axes_reset_failure_logs.py` & `django-axes-6.1.0/axes/management/commands/axes_reset_failure_logs.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/management/commands/axes_reset_ip.py` & `django-axes-6.1.0/axes/management/commands/axes_reset_ip.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/management/commands/axes_reset_logs.py` & `django-axes-6.1.0/axes/management/commands/axes_reset_logs.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/management/commands/axes_reset_username.py` & `django-axes-6.1.0/axes/management/commands/axes_reset_username.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/middleware.py` & `django-axes-6.1.0/axes/middleware.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/migrations/0001_initial.py` & `django-axes-6.1.0/axes/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/migrations/0002_auto_20151217_2044.py` & `django-axes-6.1.0/axes/migrations/0002_auto_20151217_2044.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/migrations/0003_auto_20160322_0929.py` & `django-axes-6.1.0/axes/migrations/0003_auto_20160322_0929.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/migrations/0004_auto_20181024_1538.py` & `django-axes-6.1.0/axes/migrations/0004_auto_20181024_1538.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/migrations/0007_alter_accessattempt_unique_together.py` & `django-axes-6.1.0/axes/migrations/0007_alter_accessattempt_unique_together.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/migrations/0008_accessfailurelog.py` & `django-axes-6.1.0/axes/migrations/0008_accessfailurelog.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/models.py` & `django-axes-6.1.0/axes/models.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/signals.py` & `django-axes-6.1.0/axes/signals.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/axes/utils.py` & `django-axes-6.1.0/axes/utils.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/django_axes.egg-info/PKG-INFO` & `django-axes-6.1.0/django_axes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-axes
-Version: 6.0.5
+Version: 6.1.0
 Summary: Keep track of failed login attempts in Django-powered sites.
 Home-page: https://github.com/jazzband/django-axes
 Author: Josh VanderLinden, Philip Neustrom, Michael Blume, Alex Clark, Camilo Nova, Aleksi Hakli
 Author-email: security@jazzband.co
 Maintainer: Jazzband
 Maintainer-email: security@jazzband.co
 License: MIT
@@ -123,14 +123,25 @@
 See `CONTRIBUTING <CONTRIBUTING.rst>`__.
 
 
 Changes
 =======
 
 
+6.1.0 (2023-07-30)
+------------------
+
+- Set ``AXES_SENSITIVE_PARAMETERS`` default value to ``["username", "ip_address"]`` in addition to the ``AXES_PASSWORD_FORM_FIELD`` configuration flag.
+  This masks the username and IP address fields by default in the logs when writing information about login attempts to the application logs.
+  Reverting to old configuration default of ``[]`` can be done by setting ``AXES_SENSITIVE_PARAMETERS = []`` in the Django project settings file.
+  [GitRon]
+- Improve documentation on GDPR and privacy notes and configuration flags.
+  [GitRon]
+
+
 6.0.5 (2023-07-01)
 ------------------
 
 - Add Indonesion translation.
   [kiraware]
```

### Comparing `django-axes-6.0.5/django_axes.egg-info/SOURCES.txt` & `django-axes-6.1.0/django_axes.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 pyproject.toml
 requirements-qa.txt
 requirements-test.txt
 requirements.txt
 setup.py
 .github/PULL_REQUEST_TEMPLATE.md
 .github/dependabot.yml
-.github/ISSUE_TEMPLATES/bug_report.md
-.github/ISSUE_TEMPLATES/feature_request.md
+.github/ISSUE_TEMPLATE/bug_report.md
+.github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/codeql.yml
 .github/workflows/release.yml
 .github/workflows/test.yml
 axes/__init__.py
 axes/admin.py
 axes/apps.py
 axes/attempts.py
```

### Comparing `django-axes-6.0.5/docs/1_requirements.rst` & `django-axes-6.1.0/docs/1_requirements.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/docs/2_installation.rst` & `django-axes-6.1.0/docs/2_installation.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/docs/3_usage.rst` & `django-axes-6.1.0/docs/3_usage.rst`

 * *Files 14% similar despite different names*

```diff
@@ -103,7 +103,28 @@
 - ``reset(ip=ip)`` will clear lockouts and records for the given IP address.
 - ``reset(username=username)`` will clear lockouts and records for the given username.
 
 .. note::
    Please note that if you give both ``username`` and ``ip`` arguments to ``reset``
    that attempts that have both the set IP and username are reset.
    The effective behaviour of ``reset`` is to ``and`` the terms instead of ``or`` ing them.
+
+
+
+Data privacy and GDPR
+^^^^^^^^^^^^^^^^^^^^^
+
+Most European countries have quite strict laws regarding data protection and privacy. It's highly recommended and good 
+practice to treat your sensitive user data with care. The general rule here is that you shouldn't store what you don't need.
+
+When dealing with brute-force protection, the IP address and the username (often the email address) are most crucial.
+Given that you can perfectly use `django-axes` without locking the user out by IP but by username, it does make sense to
+avoid storing the IP address at all. You can not lose what you don't have.
+
+You can adjust the AXES settings as follows::
+
+    # Block by Username only (i.e.: Same user different IP is still blocked, but different user same IP is not)
+    AXES_LOCKOUT_PARAMETERS = ["username"]
+
+    # Disable logging the IP-Address of failed login attempts by returning None for attempts to get the IP
+    # Ignore assigning a lambda function to a variable for brevity
+    AXES_CLIENT_IP_CALLABLE = lambda x: None  # noqa: E731
```

### Comparing `django-axes-6.0.5/docs/4_configuration.rst` & `django-axes-6.1.0/docs/4_configuration.rst`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 +------------------------------------------------------+----------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
 | AXES_LOCKOUT_CALLABLE                                | None                                         | A callable or a string path to callable that takes two arguments returns a response. For example: ``def generate_lockout_response(request: HttpRequest, credentials: dict) -> HttpResponse: ...``. This can be any callable similarly to ``AXES_USERNAME_CALLABLE``. If not callable is defined, then the default implementation in ``axes.helpers.get_lockout_response`` is used for determining the correct lockout response that is sent to the requesting client.                                                                                                                                                                                                                                                                     |
 +------------------------------------------------------+----------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
 | AXES_CLIENT_IP_CALLABLE                              | None                                         | A callable or a string path to callable that takes two arguments returns a response. For example: ``def get_ip(request: HttpRequest) -> str: ...``. This can be any callable similarly to ``AXES_USERNAME_CALLABLE``. If not callable is defined, then the default implementation in ``axes.helpers.get_client_ip_address`` is used.                                                                                                                                                                                                                                                                                                                                                                                                      |
 +------------------------------------------------------+----------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
 | AXES_PASSWORD_FORM_FIELD                             | 'password'                                   | The name of the form or credentials field that contains your users password.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
 +------------------------------------------------------+----------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
-| AXES_SENSITIVE_PARAMETERS                            | []                                           | Configures POST and GET parameter values (in addition to the value of ``AXES_PASSWORD_FORM_FIELD``) to mask in login attempt logging.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
+| AXES_SENSITIVE_PARAMETERS                            | ["username", "ip_address"]                   | Configures POST and GET parameter values (in addition to the value of ``AXES_PASSWORD_FORM_FIELD``) to mask in login attempt logging. Defaults enable privacy-by-design.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
 +------------------------------------------------------+----------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
 | AXES_NEVER_LOCKOUT_GET                               | False                                        | If ``True``, Axes will never lock out HTTP GET requests.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
 +------------------------------------------------------+----------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
 | AXES_NEVER_LOCKOUT_WHITELIST                         | False                                        |  If ``True``, users can always login from whitelisted IP addresses.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
 +------------------------------------------------------+----------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
 | AXES_IP_BLACKLIST                                    | None                                         | An iterable of IPs to be blacklisted. Takes precedence over whitelists. For example: ``AXES_IP_BLACKLIST = ['0.0.0.0']``.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
 +------------------------------------------------------+----------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
```

### Comparing `django-axes-6.0.5/docs/5_customization.rst` & `django-axes-6.1.0/docs/5_customization.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/docs/6_integration.rst` & `django-axes-6.1.0/docs/6_integration.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/docs/7_architecture.rst` & `django-axes-6.1.0/docs/7_architecture.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/docs/Makefile` & `django-axes-6.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/docs/conf.py` & `django-axes-6.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/docs/images/flow.png` & `django-axes-6.1.0/docs/images/flow.png`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/pyproject.toml` & `django-axes-6.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/setup.py` & `django-axes-6.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/tests/base.py` & `django-axes-6.1.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/tests/settings.py` & `django-axes-6.1.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/tests/test_admin.py` & `django-axes-6.1.0/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/tests/test_attempts.py` & `django-axes-6.1.0/tests/test_attempts.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/tests/test_backends.py` & `django-axes-6.1.0/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/tests/test_checks.py` & `django-axes-6.1.0/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/tests/test_decorators.py` & `django-axes-6.1.0/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/tests/test_failures.py` & `django-axes-6.1.0/tests/test_failures.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/tests/test_handlers.py` & `django-axes-6.1.0/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/tests/test_helpers.py` & `django-axes-6.1.0/tests/test_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,15 @@
         }
 
         for delta, iso_duration in expected.items():
             with self.subTest(iso_duration):
                 self.assertEqual(get_cool_off_iso8601(delta), iso_duration)
 
 
+@override_settings(AXES_SENSITIVE_PARAMETERS=[])
 class ClientStringTestCase(AxesTestCase):
     @staticmethod
     def get_expected_client_str(*args, **kwargs):
         client_str_template = '{{username: "{0}", ip_address: "{1}", user_agent: "{2}", path_info: "{3}"}}'
         return client_str_template.format(*args, **kwargs)
 
     @override_settings(AXES_VERBOSE=True)
@@ -924,23 +925,23 @@
         self.assertIsNone(get_cool_off())
 
     @override_settings(AXES_COOLOFF_TIME=2)
     def test_get_cool_off_int(self):
         self.assertEqual(get_cool_off(), timedelta(hours=2))
 
     @override_settings(AXES_COOLOFF_TIME=2.0)
-    def test_get_cool_off_int(self):
+    def test_get_cool_off_float(self):
         self.assertEqual(get_cool_off(), timedelta(minutes=120))
 
     @override_settings(AXES_COOLOFF_TIME=0.25)
-    def test_get_cool_off_int(self):
+    def test_get_cool_off_float_lt_0(self):
         self.assertEqual(get_cool_off(), timedelta(minutes=15))
 
     @override_settings(AXES_COOLOFF_TIME=1.7)
-    def test_get_cool_off_int(self):
+    def test_get_cool_off_float_gt_0(self):
         self.assertEqual(get_cool_off(), timedelta(seconds=6120))
 
     @override_settings(AXES_COOLOFF_TIME=lambda: timedelta(seconds=30))
     def test_get_cool_off_callable(self):
         self.assertEqual(get_cool_off(), timedelta(seconds=30))
 
     @override_settings(AXES_COOLOFF_TIME="tests.test_helpers.mock_get_cool_off_str")
@@ -1016,14 +1017,15 @@
     def setUp(self):
         self.parameters = {
             "username": "test_user",
             "password": "test_password",
             "other_sensitive_data": "sensitive",
         }
 
+    @override_settings(AXES_SENSITIVE_PARAMETERS=[])
     def test_cleanse_parameters(self):
         cleansed = cleanse_parameters(self.parameters)
         self.assertEqual("test_user", cleansed["username"])
         self.assertEqual("********************", cleansed["password"])
         self.assertEqual("sensitive", cleansed["other_sensitive_data"])
 
     @override_settings(AXES_SENSITIVE_PARAMETERS=["other_sensitive_data"])
@@ -1037,13 +1039,14 @@
     @override_settings(AXES_PASSWORD_FORM_FIELD="username")
     def test_cleanse_parameters_override_both(self):
         cleansed = cleanse_parameters(self.parameters)
         self.assertEqual("********************", cleansed["username"])
         self.assertEqual("********************", cleansed["password"])
         self.assertEqual("********************", cleansed["other_sensitive_data"])
 
+    @override_settings(AXES_SENSITIVE_PARAMETERS=[])
     @override_settings(AXES_PASSWORD_FORM_FIELD=None)
     def test_cleanse_parameters_override_empty(self):
         cleansed = cleanse_parameters(self.parameters)
         self.assertEqual("test_user", cleansed["username"])
         self.assertEqual("********************", cleansed["password"])
         self.assertEqual("sensitive", cleansed["other_sensitive_data"])
```

### Comparing `django-axes-6.0.5/tests/test_logging.py` & `django-axes-6.1.0/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/tests/test_login.py` & `django-axes-6.1.0/tests/test_login.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/tests/test_management.py` & `django-axes-6.1.0/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/tests/test_middleware.py` & `django-axes-6.1.0/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.5/tests/test_models.py` & `django-axes-6.1.0/tests/test_models.py`

 * *Files identical despite different names*

