# Comparing `tmp/django_base_template-1.0.0.tar.gz` & `tmp/django_base_template-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_base_template-1.0.0.tar", last modified: Sat Jul 29 12:08:47 2023, max compression
+gzip compressed data, was "django_base_template-1.0.3.tar", last modified: Sun Jul 30 15:53:33 2023, max compression
```

## Comparing `django_base_template-1.0.0.tar` & `django_base_template-1.0.3.tar`

### file list

```diff
@@ -1,170 +1,171 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.248321 django_base_template-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.196317 django_base_template-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.208318 django_base_template-1.0.0/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-07-29 12:08:37.000000 django_base_template-1.0.0/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.208318 django_base_template-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-29 12:08:37.000000 django_base_template-1.0.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-29 12:08:37.000000 django_base_template-1.0.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-29 12:08:37.000000 django_base_template-1.0.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.212318 django_base_template-1.0.0/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-29 12:08:37.000000 django_base_template-1.0.0/.idea/base_template.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.212318 django_base_template-1.0.0/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-29 12:08:37.000000 django_base_template-1.0.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-29 12:08:37.000000 django_base_template-1.0.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-29 12:08:37.000000 django_base_template-1.0.0/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-29 12:08:37.000000 django_base_template-1.0.0/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)    22190 2023-07-29 12:08:37.000000 django_base_template-1.0.0/.idea/workspace.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-29 12:08:37.000000 django_base_template-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-29 12:08:37.000000 django_base_template-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-29 12:08:47.252321 django_base_template-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:37.000000 django_base_template-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:37.000000 django_base_template-1.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.212318 django_base_template-1.0.0/base_template/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:37.000000 django_base_template-1.0.0/base_template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.216318 django_base_template-1.0.0/base_template/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-29 12:08:37.000000 django_base_template-1.0.0/base_template/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-07-29 12:08:37.000000 django_base_template-1.0.0/base_template/__pycache__/settings.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-29 12:08:37.000000 django_base_template-1.0.0/base_template/__pycache__/sidebars.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-29 12:08:37.000000 django_base_template-1.0.0/base_template/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-29 12:08:37.000000 django_base_template-1.0.0/base_template/__pycache__/wsgi.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-29 12:08:37.000000 django_base_template-1.0.0/base_template/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-29 12:08:37.000000 django_base_template-1.0.0/base_template/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-29 12:08:37.000000 django_base_template-1.0.0/base_template/sidebars.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-29 12:08:37.000000 django_base_template-1.0.0/base_template/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-29 12:08:37.000000 django_base_template-1.0.0/base_template/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (123)   118784 2023-07-29 12:08:37.000000 django_base_template-1.0.0/db.sqlite3
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.216318 django_base_template-1.0.0/example/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:37.000000 django_base_template-1.0.0/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-07-29 12:08:37.000000 django_base_template-1.0.0/example/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.216318 django_base_template-1.0.0/example/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:37.000000 django_base_template-1.0.0/example/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-29 12:08:37.000000 django_base_template-1.0.0/example/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.200317 django_base_template-1.0.0/example/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.216318 django_base_template-1.0.0/example/templates/example/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-29 12:08:37.000000 django_base_template-1.0.0/example/templates/example/actions.html
--rw-r--r--   0 runner    (1001) docker     (123)    22939 2023-07-29 12:08:37.000000 django_base_template-1.0.0/example/templates/example/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-29 12:08:37.000000 django_base_template-1.0.0/example/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-29 12:08:37.000000 django_base_template-1.0.0/example/views.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      669 2023-07-29 12:08:37.000000 django_base_template-1.0.0/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-29 12:08:37.000000 django_base_template-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-29 12:08:47.252321 django_base_template-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 12:08:37.000000 django_base_template-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.204318 django_base_template-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.220319 django_base_template-1.0.0/src/base_template/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.220319 django_base_template-1.0.0/src/base_template/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/__pycache__/apps.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/__pycache__/context_processors.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/__pycache__/settings.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/context_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.200317 django_base_template-1.0.0/src/base_template/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.200317 django_base_template-1.0.0/src/base_template/static/base_template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.220319 django_base_template-1.0.0/src/base_template/static/base_template/css/
--rw-r--r--   0 runner    (1001) docker     (123)  1568007 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/css/style.bundle.css
--rw-r--r--   0 runner    (1001) docker     (123)  1420069 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/css/style.bundle.rtl.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.224319 django_base_template-1.0.0/src/base_template/static/base_template/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/images/icon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/images/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/images/logo-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/images/logo-white.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/images/smartphone-2-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/images/smartphone-2.svg
--rw-r--r--   0 runner    (1001) docker     (123)    68122 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/images/user.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.224319 django_base_template-1.0.0/src/base_template/static/base_template/js/
--rw-r--r--   0 runner    (1001) docker     (123)   238093 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/js/scripts.bundle.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.200317 django_base_template-1.0.0/src/base_template/static/base_template/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.228320 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.200317 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.232320 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/@fortawesome/
--rw-r--r--   0 runner    (1001) docker     (123)   187208 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   108020 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    63952 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    24948 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   394628 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   150124 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-v4compatibility.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-v4compatibility.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.232320 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/bootstrap-icons/
--rw-r--r--   0 runner    (1001) docker     (123)   164360 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/bootstrap-icons/bootstrap-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)   121340 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/bootstrap-icons/bootstrap-icons.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.240320 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/keenicons/
--rw-r--r--   0 runner    (1001) docker     (123)   187664 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-duotone.eot
--rw-r--r--   0 runner    (1001) docker     (123)   690267 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-duotone.svg
--rw-r--r--   0 runner    (1001) docker     (123)   187500 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-duotone.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   187576 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-duotone.woff
--rw-r--r--   0 runner    (1001) docker     (123)   246928 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-outline.eot
--rw-r--r--   0 runner    (1001) docker     (123)  1058682 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-outline.svg
--rw-r--r--   0 runner    (1001) docker     (123)   246764 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-outline.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   246840 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-outline.woff
--rw-r--r--   0 runner    (1001) docker     (123)   165296 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-solid.eot
--rw-r--r--   0 runner    (1001) docker     (123)   695434 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-solid.svg
--rw-r--r--   0 runner    (1001) docker     (123)   165132 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-solid.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   165208 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-solid.woff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.248321 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/line-awesome/
--rw-r--r--   0 runner    (1001) docker     (123)   156260 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-brands-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)   927335 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-brands-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)   156072 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    98673 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-brands-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    84772 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    33916 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-regular-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)   113535 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-regular-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)    33724 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    15489 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   226312 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-solid-900.eot
--rw-r--r--   0 runner    (1001) docker     (123)   923151 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-solid-900.svg
--rw-r--r--   0 runner    (1001) docker     (123)   226128 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   125421 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (123)    96752 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   873384 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/plugins.bundle.css
--rw-r--r--   0 runner    (1001) docker     (123)  3695326 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/plugins.bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)   873384 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/plugins.bundle.rtl.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.204318 django_base_template-1.0.0/src/base_template/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.248321 django_base_template-1.0.0/src/base_template/templates/base_template/
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/templates/base_template/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.248321 django_base_template-1.0.0/src/base_template/templates/base_template/layout/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/templates/base_template/layout/_localization.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.204318 django_base_template-1.0.0/src/base_template/templates/base_template/layout/partials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.248321 django_base_template-1.0.0/src/base_template/templates/base_template/layout/partials/footer/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/templates/base_template/layout/partials/footer/__footer_links.html
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/templates/base_template/layout/partials/footer/_footer.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.248321 django_base_template-1.0.0/src/base_template/templates/base_template/layout/partials/header/
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/templates/base_template/layout/partials/header/_header.html
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/templates/base_template/layout/partials/header/_left_menus.html
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/templates/base_template/layout/partials/header/_navbar.html
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/templates/base_template/layout/partials/header/_right_menus.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.248321 django_base_template-1.0.0/src/base_template/templates/base_template/layout/partials/sidebar/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/templates/base_template/layout/partials/sidebar/_footer.html
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/templates/base_template/layout/partials/sidebar/_logo.html
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/templates/base_template/layout/partials/sidebar/_menu.html
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/templates/base_template/layout/partials/sidebar/_sidebar.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.248321 django_base_template-1.0.0/src/base_template/templates/base_template/layout/partials/toolbar/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/templates/base_template/layout/partials/toolbar/_page-title.html
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/templates/base_template/layout/partials/toolbar/_toolbar.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.248321 django_base_template-1.0.0/src/base_template/templates/base_template/partials/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/templates/base_template/partials/_scrolltop.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.248321 django_base_template-1.0.0/src/base_template/templates/base_template/partials/menus/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/templates/base_template/partials/menus/__langauage_menu.html
--rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/templates/base_template/partials/menus/_sample_right_menu.html
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/templates/base_template/partials/menus/_user-account-menu.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.248321 django_base_template-1.0.0/src/base_template/templates/base_template/partials/theme-mode/
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/templates/base_template/partials/theme-mode/__menu.html
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/templates/base_template/partials/theme-mode/_init.html
--rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/templates/base_template/partials/theme-mode/_main.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.248321 django_base_template-1.0.0/src/base_template/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/templatetags/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.248321 django_base_template-1.0.0/src/base_template/templatetags/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/templatetags/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/templatetags/__pycache__/base_template.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/templatetags/base_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-29 12:08:37.000000 django_base_template-1.0.0/src/base_template/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:08:47.248321 django_base_template-1.0.0/src/django_base_template.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-29 12:08:47.000000 django_base_template-1.0.0/src/django_base_template.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-07-29 12:08:47.000000 django_base_template-1.0.0/src/django_base_template.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 12:08:47.000000 django_base_template-1.0.0/src/django_base_template.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-29 12:08:47.000000 django_base_template-1.0.0/src/django_base_template.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.664442 django_base_template-1.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.628442 django_base_template-1.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.632442 django_base_template-1.0.3/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-07-30 15:53:25.000000 django_base_template-1.0.3/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.632442 django_base_template-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-30 15:53:25.000000 django_base_template-1.0.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-30 15:53:25.000000 django_base_template-1.0.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-30 15:53:25.000000 django_base_template-1.0.3/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.632442 django_base_template-1.0.3/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-30 15:53:25.000000 django_base_template-1.0.3/.idea/base_template.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.632442 django_base_template-1.0.3/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-30 15:53:25.000000 django_base_template-1.0.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-30 15:53:25.000000 django_base_template-1.0.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-30 15:53:25.000000 django_base_template-1.0.3/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-30 15:53:25.000000 django_base_template-1.0.3/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-07-30 15:53:25.000000 django_base_template-1.0.3/.idea/workspace.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-30 15:53:25.000000 django_base_template-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-30 15:53:25.000000 django_base_template-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-30 15:53:33.664442 django_base_template-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:25.000000 django_base_template-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:25.000000 django_base_template-1.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.632442 django_base_template-1.0.3/base_template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:25.000000 django_base_template-1.0.3/base_template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.636442 django_base_template-1.0.3/base_template/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-30 15:53:25.000000 django_base_template-1.0.3/base_template/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-07-30 15:53:25.000000 django_base_template-1.0.3/base_template/__pycache__/settings.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-30 15:53:25.000000 django_base_template-1.0.3/base_template/__pycache__/sidebars.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-30 15:53:25.000000 django_base_template-1.0.3/base_template/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-30 15:53:25.000000 django_base_template-1.0.3/base_template/__pycache__/wsgi.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-30 15:53:25.000000 django_base_template-1.0.3/base_template/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-30 15:53:25.000000 django_base_template-1.0.3/base_template/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-30 15:53:25.000000 django_base_template-1.0.3/base_template/sidebars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-30 15:53:25.000000 django_base_template-1.0.3/base_template/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-30 15:53:25.000000 django_base_template-1.0.3/base_template/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118784 2023-07-30 15:53:25.000000 django_base_template-1.0.3/db.sqlite3
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.636442 django_base_template-1.0.3/example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:25.000000 django_base_template-1.0.3/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-07-30 15:53:25.000000 django_base_template-1.0.3/example/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.636442 django_base_template-1.0.3/example/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:25.000000 django_base_template-1.0.3/example/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-30 15:53:25.000000 django_base_template-1.0.3/example/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.628442 django_base_template-1.0.3/example/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.636442 django_base_template-1.0.3/example/templates/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-30 15:53:25.000000 django_base_template-1.0.3/example/templates/example/actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)    22939 2023-07-30 15:53:25.000000 django_base_template-1.0.3/example/templates/example/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-30 15:53:25.000000 django_base_template-1.0.3/example/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-30 15:53:25.000000 django_base_template-1.0.3/example/views.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      669 2023-07-30 15:53:25.000000 django_base_template-1.0.3/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-30 15:53:25.000000 django_base_template-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-30 15:53:33.664442 django_base_template-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 15:53:25.000000 django_base_template-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.632442 django_base_template-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.636442 django_base_template-1.0.3/src/base_template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.636442 django_base_template-1.0.3/src/base_template/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/__pycache__/apps.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/__pycache__/context_processors.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/__pycache__/settings.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/context_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.628442 django_base_template-1.0.3/src/base_template/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.628442 django_base_template-1.0.3/src/base_template/static/base_template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.636442 django_base_template-1.0.3/src/base_template/static/base_template/css/
+-rw-r--r--   0 runner    (1001) docker     (123)  1568007 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/css/style.bundle.css
+-rw-r--r--   0 runner    (1001) docker     (123)  1420069 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/css/style.bundle.rtl.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.640442 django_base_template-1.0.3/src/base_template/static/base_template/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/images/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/images/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/images/logo-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/images/logo-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/images/smartphone-2-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/images/smartphone-2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    68122 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/images/user.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.640442 django_base_template-1.0.3/src/base_template/static/base_template/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   238093 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/js/scripts.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/js/utils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.628442 django_base_template-1.0.3/src/base_template/static/base_template/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.644442 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.628442 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.648442 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/@fortawesome/
+-rw-r--r--   0 runner    (1001) docker     (123)   187208 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   108020 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    63952 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    24948 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   394628 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   150124 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-v4compatibility.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-v4compatibility.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.648442 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/bootstrap-icons/
+-rw-r--r--   0 runner    (1001) docker     (123)   164360 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/bootstrap-icons/bootstrap-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   121340 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/bootstrap-icons/bootstrap-icons.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.656442 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/keenicons/
+-rw-r--r--   0 runner    (1001) docker     (123)   187664 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-duotone.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   690267 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-duotone.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   187500 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-duotone.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   187576 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-duotone.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   246928 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-outline.eot
+-rw-r--r--   0 runner    (1001) docker     (123)  1058682 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-outline.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   246764 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-outline.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   246840 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-outline.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   165296 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-solid.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   695434 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-solid.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   165132 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-solid.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   165208 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-solid.woff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.660442 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/line-awesome/
+-rw-r--r--   0 runner    (1001) docker     (123)   156260 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-brands-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   927335 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-brands-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   156072 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    98673 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    84772 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    33916 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   113535 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    33724 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    15489 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   226312 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   923151 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   226128 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   125421 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    96752 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   873384 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/plugins.bundle.css
+-rw-r--r--   0 runner    (1001) docker     (123)  3695326 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/plugins.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   873384 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/plugins.bundle.rtl.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.632442 django_base_template-1.0.3/src/base_template/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.660442 django_base_template-1.0.3/src/base_template/templates/base_template/
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/templates/base_template/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.660442 django_base_template-1.0.3/src/base_template/templates/base_template/layout/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/templates/base_template/layout/_localization.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.632442 django_base_template-1.0.3/src/base_template/templates/base_template/layout/partials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.660442 django_base_template-1.0.3/src/base_template/templates/base_template/layout/partials/footer/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/templates/base_template/layout/partials/footer/__footer_links.html
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/templates/base_template/layout/partials/footer/_footer.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.660442 django_base_template-1.0.3/src/base_template/templates/base_template/layout/partials/header/
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/templates/base_template/layout/partials/header/_header.html
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/templates/base_template/layout/partials/header/_left_menus.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/templates/base_template/layout/partials/header/_navbar.html
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/templates/base_template/layout/partials/header/_right_menus.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.660442 django_base_template-1.0.3/src/base_template/templates/base_template/layout/partials/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/templates/base_template/layout/partials/sidebar/_footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/templates/base_template/layout/partials/sidebar/_logo.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/templates/base_template/layout/partials/sidebar/_menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/templates/base_template/layout/partials/sidebar/_sidebar.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.660442 django_base_template-1.0.3/src/base_template/templates/base_template/layout/partials/toolbar/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/templates/base_template/layout/partials/toolbar/_page-title.html
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/templates/base_template/layout/partials/toolbar/_toolbar.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.660442 django_base_template-1.0.3/src/base_template/templates/base_template/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/templates/base_template/partials/_scrolltop.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.660442 django_base_template-1.0.3/src/base_template/templates/base_template/partials/menus/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/templates/base_template/partials/menus/__langauage_menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/templates/base_template/partials/menus/_sample_right_menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/templates/base_template/partials/menus/_user-account-menu.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.664442 django_base_template-1.0.3/src/base_template/templates/base_template/partials/theme-mode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/templates/base_template/partials/theme-mode/__menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/templates/base_template/partials/theme-mode/_init.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/templates/base_template/partials/theme-mode/_main.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.664442 django_base_template-1.0.3/src/base_template/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/templatetags/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.664442 django_base_template-1.0.3/src/base_template/templatetags/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/templatetags/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/templatetags/__pycache__/base_template.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/templatetags/base_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-07-30 15:53:25.000000 django_base_template-1.0.3/src/base_template/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:53:33.664442 django_base_template-1.0.3/src/django_base_template.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-30 15:53:33.000000 django_base_template-1.0.3/src/django_base_template.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-07-30 15:53:33.000000 django_base_template-1.0.3/src/django_base_template.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 15:53:33.000000 django_base_template-1.0.3/src/django_base_template.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-30 15:53:33.000000 django_base_template-1.0.3/src/django_base_template.egg-info/top_level.txt
```

### Comparing `django_base_template-1.0.0/.github/scripts/release.py` & `django_base_template-1.0.3/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/.gitignore` & `django_base_template-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/.idea/inspectionProfiles/Project_Default.xml` & `django_base_template-1.0.3/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/LICENSE` & `django_base_template-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/PKG-INFO` & `django_base_template-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_base_template
-Version: 1.0.0
+Version: 1.0.3
 Summary: Django package provides easy configuration admin template
 Author: Sohype Khaled
 Author-email: sohype.mop@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

### Comparing `django_base_template-1.0.0/base_template/__pycache__/settings.cpython-38.pyc` & `django_base_template-1.0.3/base_template/__pycache__/settings.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/base_template/__pycache__/wsgi.cpython-38.pyc` & `django_base_template-1.0.3/base_template/__pycache__/wsgi.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/base_template/settings.py` & `django_base_template-1.0.3/base_template/settings.py`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/db.sqlite3` & `django_base_template-1.0.3/db.sqlite3`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/example/apps.py` & `django_base_template-1.0.3/example/apps.py`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/example/templates/example/index.html` & `django_base_template-1.0.3/example/templates/example/index.html`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/example/views.py` & `django_base_template-1.0.3/example/views.py`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/manage.py` & `django_base_template-1.0.3/manage.py`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/setup.cfg` & `django_base_template-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/__pycache__/context_processors.cpython-38.pyc` & `django_base_template-1.0.3/src/base_template/__pycache__/context_processors.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/__pycache__/settings.cpython-38.pyc` & `django_base_template-1.0.3/src/base_template/__pycache__/settings.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/__pycache__/utils.cpython-38.pyc` & `django_base_template-1.0.3/src/base_template/__pycache__/utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/context_processors.py` & `django_base_template-1.0.3/src/base_template/context_processors.py`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/settings.py` & `django_base_template-1.0.3/src/base_template/settings.py`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/css/style.bundle.css` & `django_base_template-1.0.3/src/base_template/static/base_template/css/style.bundle.css`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/css/style.bundle.rtl.css` & `django_base_template-1.0.3/src/base_template/static/base_template/css/style.bundle.rtl.css`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/images/icon.ico` & `django_base_template-1.0.3/src/base_template/static/base_template/images/icon.ico`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/images/icon.svg` & `django_base_template-1.0.3/src/base_template/static/base_template/images/icon.svg`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/images/logo-dark.svg` & `django_base_template-1.0.3/src/base_template/static/base_template/images/logo-dark.svg`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/images/logo-white.svg` & `django_base_template-1.0.3/src/base_template/static/base_template/images/logo-white.svg`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/images/logo.png` & `django_base_template-1.0.3/src/base_template/static/base_template/images/logo.png`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/images/smartphone-2-dark.svg` & `django_base_template-1.0.3/src/base_template/static/base_template/images/smartphone-2-dark.svg`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/images/smartphone-2.svg` & `django_base_template-1.0.3/src/base_template/static/base_template/images/smartphone-2.svg`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/images/user.jpg` & `django_base_template-1.0.3/src/base_template/static/base_template/images/user.jpg`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/js/scripts.bundle.js` & `django_base_template-1.0.3/src/base_template/static/base_template/js/scripts.bundle.js`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-brands-400.ttf` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-brands-400.woff2` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-regular-400.ttf` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-regular-400.woff2` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-solid-900.ttf` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-solid-900.woff2` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-v4compatibility.ttf` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-v4compatibility.woff2` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/bootstrap-icons/bootstrap-icons.woff` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/bootstrap-icons/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/bootstrap-icons/bootstrap-icons.woff2` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/bootstrap-icons/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-duotone.eot` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-duotone.eot`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-duotone.svg` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-duotone.svg`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-duotone.ttf` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-duotone.ttf`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-duotone.woff` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-duotone.woff`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-outline.eot` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-outline.eot`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-outline.svg` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-outline.svg`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-outline.ttf` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-outline.ttf`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-outline.woff` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-outline.woff`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-solid.eot` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-solid.eot`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-solid.svg` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-solid.svg`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-solid.ttf` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-solid.ttf`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-solid.woff` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/keenicons/keenicons-solid.woff`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-brands-400.eot` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-brands-400.eot`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-brands-400.svg` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-brands-400.svg`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-brands-400.ttf` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-brands-400.woff` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-brands-400.woff`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-brands-400.woff2` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-regular-400.eot` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-regular-400.eot`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-regular-400.svg` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-regular-400.svg`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-regular-400.ttf` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-regular-400.woff` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-regular-400.woff`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-regular-400.woff2` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-solid-900.eot` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-solid-900.eot`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-solid-900.svg` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-solid-900.svg`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-solid-900.ttf` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-solid-900.woff` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-solid-900.woff`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-solid-900.woff2` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/fonts/line-awesome/la-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/plugins.bundle.css` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/plugins.bundle.css`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/plugins.bundle.js` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/plugins.bundle.js`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/static/base_template/plugins/global/plugins.bundle.rtl.css` & `django_base_template-1.0.3/src/base_template/static/base_template/plugins/global/plugins.bundle.rtl.css`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/templates/base_template/base.html` & `django_base_template-1.0.3/src/base_template/templates/base_template/base.html`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/templates/base_template/layout/partials/footer/_footer.html` & `django_base_template-1.0.3/src/base_template/templates/base_template/layout/partials/footer/_footer.html`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/templates/base_template/layout/partials/header/_header.html` & `django_base_template-1.0.3/src/base_template/templates/base_template/layout/partials/header/_header.html`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/templates/base_template/layout/partials/header/_left_menus.html` & `django_base_template-1.0.3/src/base_template/templates/base_template/layout/partials/header/_left_menus.html`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/templates/base_template/layout/partials/header/_navbar.html` & `django_base_template-1.0.3/src/base_template/templates/base_template/layout/partials/header/_navbar.html`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/templates/base_template/layout/partials/sidebar/_footer.html` & `django_base_template-1.0.3/src/base_template/templates/base_template/layout/partials/sidebar/_footer.html`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/templates/base_template/layout/partials/sidebar/_logo.html` & `django_base_template-1.0.3/src/base_template/templates/base_template/layout/partials/sidebar/_logo.html`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/templates/base_template/layout/partials/sidebar/_menu.html` & `django_base_template-1.0.3/src/base_template/templates/base_template/layout/partials/sidebar/_menu.html`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/templates/base_template/layout/partials/sidebar/_sidebar.html` & `django_base_template-1.0.3/src/base_template/templates/base_template/layout/partials/sidebar/_sidebar.html`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/templates/base_template/layout/partials/toolbar/_page-title.html` & `django_base_template-1.0.3/src/base_template/templates/base_template/layout/partials/toolbar/_page-title.html`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/templates/base_template/partials/menus/__langauage_menu.html` & `django_base_template-1.0.3/src/base_template/templates/base_template/partials/menus/__langauage_menu.html`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/templates/base_template/partials/menus/_sample_right_menu.html` & `django_base_template-1.0.3/src/base_template/templates/base_template/partials/menus/_sample_right_menu.html`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/templates/base_template/partials/menus/_user-account-menu.html` & `django_base_template-1.0.3/src/base_template/templates/base_template/partials/menus/_user-account-menu.html`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/templates/base_template/partials/theme-mode/__menu.html` & `django_base_template-1.0.3/src/base_template/templates/base_template/partials/theme-mode/__menu.html`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/templates/base_template/partials/theme-mode/_init.html` & `django_base_template-1.0.3/src/base_template/templates/base_template/partials/theme-mode/_init.html`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/templates/base_template/partials/theme-mode/_main.html` & `django_base_template-1.0.3/src/base_template/templates/base_template/partials/theme-mode/_main.html`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/templatetags/__pycache__/base_template.cpython-38.pyc` & `django_base_template-1.0.3/src/base_template/templatetags/__pycache__/base_template.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django_base_template-1.0.0/src/base_template/utils.py` & `django_base_template-1.0.3/src/base_template/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,16 @@
         {
             "rel": "stylesheet",
             "href": "https://fonts.googleapis.com/css?family=Inter:300,400,500,600,700"
         }
     ]
     js = [
         static("base_template/plugins/global/plugins.bundle.js"),
-        static("base_template/js/scripts.bundle.js")
+        static("base_template/js/scripts.bundle.js"),
+        static("base_template/js/utils.js")
     ]
     if get_settings_value("BASE_TEMPLATE_MULTIPLE_LANGUAGES", False):
         from django.urls import reverse
         js.insert(0, reverse("javascript-catalog"))
     if get_language() in settings.LANGUAGES_BIDI:
         css.append({
             "rel": "stylesheet",
```

### Comparing `django_base_template-1.0.0/src/django_base_template.egg-info/PKG-INFO` & `django_base_template-1.0.3/src/django_base_template.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-base-template
-Version: 1.0.0
+Version: 1.0.3
 Summary: Django package provides easy configuration admin template
 Author: Sohype Khaled
 Author-email: sohype.mop@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

### Comparing `django_base_template-1.0.0/src/django_base_template.egg-info/SOURCES.txt` & `django_base_template-1.0.3/src/django_base_template.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 src/base_template/static/base_template/images/logo-dark.svg
 src/base_template/static/base_template/images/logo-white.svg
 src/base_template/static/base_template/images/logo.png
 src/base_template/static/base_template/images/smartphone-2-dark.svg
 src/base_template/static/base_template/images/smartphone-2.svg
 src/base_template/static/base_template/images/user.jpg
 src/base_template/static/base_template/js/scripts.bundle.js
+src/base_template/static/base_template/js/utils.js
 src/base_template/static/base_template/plugins/global/plugins.bundle.css
 src/base_template/static/base_template/plugins/global/plugins.bundle.js
 src/base_template/static/base_template/plugins/global/plugins.bundle.rtl.css
 src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-brands-400.ttf
 src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-brands-400.woff2
 src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-regular-400.ttf
 src/base_template/static/base_template/plugins/global/fonts/@fortawesome/fa-regular-400.woff2
```

