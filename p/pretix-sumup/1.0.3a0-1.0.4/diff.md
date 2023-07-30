# Comparing `tmp/pretix-sumup-1.0.3a0.tar.gz` & `tmp/pretix-sumup-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-sumup-1.0.3a0.tar", last modified: Sun Jul 30 10:01:16 2023, max compression
+gzip compressed data, was "pretix-sumup-1.0.4.tar", last modified: Sun Jul 30 14:50:25 2023, max compression
```

## Comparing `pretix-sumup-1.0.3a0.tar` & `pretix-sumup-1.0.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:01:16.788729 pretix-sumup-1.0.3a0/
--rw-r--r--   0 runner    (1001) docker     (123)    33886 2023-07-30 09:59:54.000000 pretix-sumup-1.0.3a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-30 09:59:54.000000 pretix-sumup-1.0.3a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    41113 2023-07-30 10:01:16.788729 pretix-sumup-1.0.3a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-30 09:59:54.000000 pretix-sumup-1.0.3a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:01:16.784729 pretix-sumup-1.0.3a0/pretix_sumup/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-30 09:59:54.000000 pretix-sumup-1.0.3a0/pretix_sumup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-30 09:59:54.000000 pretix-sumup-1.0.3a0/pretix_sumup/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:01:16.784729 pretix-sumup-1.0.3a0/pretix_sumup/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:01:16.780729 pretix-sumup-1.0.3a0/pretix_sumup/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:01:16.784729 pretix-sumup-1.0.3a0/pretix_sumup/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-30 09:59:54.000000 pretix-sumup-1.0.3a0/pretix_sumup/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:01:16.784729 pretix-sumup-1.0.3a0/pretix_sumup/locale/de_Informal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 09:59:54.000000 pretix-sumup-1.0.3a0/pretix_sumup/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:01:16.784729 pretix-sumup-1.0.3a0/pretix_sumup/locale/de_Informal/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-30 09:59:54.000000 pretix-sumup-1.0.3a0/pretix_sumup/locale/de_Informal/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-30 09:59:54.000000 pretix-sumup-1.0.3a0/pretix_sumup/locale/django.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:01:16.780729 pretix-sumup-1.0.3a0/pretix_sumup/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:01:16.784729 pretix-sumup-1.0.3a0/pretix_sumup/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-30 09:59:54.000000 pretix-sumup-1.0.3a0/pretix_sumup/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:01:16.780729 pretix-sumup-1.0.3a0/pretix_sumup/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:01:16.784729 pretix-sumup-1.0.3a0/pretix_sumup/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-30 09:59:54.000000 pretix-sumup-1.0.3a0/pretix_sumup/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:01:16.780729 pretix-sumup-1.0.3a0/pretix_sumup/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:01:16.784729 pretix-sumup-1.0.3a0/pretix_sumup/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-30 09:59:54.000000 pretix-sumup-1.0.3a0/pretix_sumup/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)    10386 2023-07-30 09:59:54.000000 pretix-sumup-1.0.3a0/pretix_sumup/payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-30 09:59:54.000000 pretix-sumup-1.0.3a0/pretix_sumup/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:01:16.780729 pretix-sumup-1.0.3a0/pretix_sumup/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:01:16.784729 pretix-sumup-1.0.3a0/pretix_sumup/static/pretix_sumup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 09:59:54.000000 pretix-sumup-1.0.3a0/pretix_sumup/static/pretix_sumup/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-07-30 09:59:54.000000 pretix-sumup-1.0.3a0/pretix_sumup/static/pretix_sumup/sumup-logo-black.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:01:16.780729 pretix-sumup-1.0.3a0/pretix_sumup/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:01:16.788729 pretix-sumup-1.0.3a0/pretix_sumup/templates/pretix_sumup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 09:59:54.000000 pretix-sumup-1.0.3a0/pretix_sumup/templates/pretix_sumup/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-30 09:59:54.000000 pretix-sumup-1.0.3a0/pretix_sumup/templates/pretix_sumup/checkout_confirm_render.html
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-30 09:59:54.000000 pretix-sumup-1.0.3a0/pretix_sumup/templates/pretix_sumup/checkout_payment_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-30 09:59:54.000000 pretix-sumup-1.0.3a0/pretix_sumup/templates/pretix_sumup/control.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:01:16.788729 pretix-sumup-1.0.3a0/pretix_sumup/templates/pretix_sumup/email/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-30 09:59:54.000000 pretix-sumup-1.0.3a0/pretix_sumup/templates/pretix_sumup/email/order_pending.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-30 09:59:54.000000 pretix-sumup-1.0.3a0/pretix_sumup/templates/pretix_sumup/not_available.html
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-30 09:59:54.000000 pretix-sumup-1.0.3a0/pretix_sumup/templates/pretix_sumup/pending.html
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-30 09:59:54.000000 pretix-sumup-1.0.3a0/pretix_sumup/templates/pretix_sumup/prepare.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:01:16.784729 pretix-sumup-1.0.3a0/pretix_sumup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41113 2023-07-30 10:01:16.000000 pretix-sumup-1.0.3a0/pretix_sumup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-30 10:01:16.000000 pretix-sumup-1.0.3a0/pretix_sumup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 10:01:16.000000 pretix-sumup-1.0.3a0/pretix_sumup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-30 10:01:16.000000 pretix-sumup-1.0.3a0/pretix_sumup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-30 10:01:16.000000 pretix-sumup-1.0.3a0/pretix_sumup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-30 09:59:54.000000 pretix-sumup-1.0.3a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-30 10:01:16.788729 pretix-sumup-1.0.3a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-30 09:59:54.000000 pretix-sumup-1.0.3a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 10:01:16.788729 pretix-sumup-1.0.3a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-30 09:59:54.000000 pretix-sumup-1.0.3a0/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:50:25.726373 pretix-sumup-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    33886 2023-07-30 14:48:57.000000 pretix-sumup-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-30 14:48:57.000000 pretix-sumup-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    41111 2023-07-30 14:50:25.726373 pretix-sumup-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-30 14:48:57.000000 pretix-sumup-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:50:25.722372 pretix-sumup-1.0.4/pretix_sumup/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-30 14:48:57.000000 pretix-sumup-1.0.4/pretix_sumup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-30 14:48:57.000000 pretix-sumup-1.0.4/pretix_sumup/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:50:25.722372 pretix-sumup-1.0.4/pretix_sumup/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:50:25.722372 pretix-sumup-1.0.4/pretix_sumup/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:50:25.722372 pretix-sumup-1.0.4/pretix_sumup/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-30 14:48:57.000000 pretix-sumup-1.0.4/pretix_sumup/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:50:25.726373 pretix-sumup-1.0.4/pretix_sumup/locale/de_Informal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:48:57.000000 pretix-sumup-1.0.4/pretix_sumup/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:50:25.726373 pretix-sumup-1.0.4/pretix_sumup/locale/de_Informal/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-30 14:48:57.000000 pretix-sumup-1.0.4/pretix_sumup/locale/de_Informal/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-30 14:48:57.000000 pretix-sumup-1.0.4/pretix_sumup/locale/django.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:50:25.722372 pretix-sumup-1.0.4/pretix_sumup/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:50:25.726373 pretix-sumup-1.0.4/pretix_sumup/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-30 14:48:57.000000 pretix-sumup-1.0.4/pretix_sumup/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:50:25.722372 pretix-sumup-1.0.4/pretix_sumup/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:50:25.726373 pretix-sumup-1.0.4/pretix_sumup/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-30 14:48:57.000000 pretix-sumup-1.0.4/pretix_sumup/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:50:25.722372 pretix-sumup-1.0.4/pretix_sumup/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:50:25.726373 pretix-sumup-1.0.4/pretix_sumup/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-30 14:48:57.000000 pretix-sumup-1.0.4/pretix_sumup/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)    10386 2023-07-30 14:48:57.000000 pretix-sumup-1.0.4/pretix_sumup/payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-30 14:48:57.000000 pretix-sumup-1.0.4/pretix_sumup/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:50:25.722372 pretix-sumup-1.0.4/pretix_sumup/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:50:25.726373 pretix-sumup-1.0.4/pretix_sumup/static/pretix_sumup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:48:57.000000 pretix-sumup-1.0.4/pretix_sumup/static/pretix_sumup/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-07-30 14:48:57.000000 pretix-sumup-1.0.4/pretix_sumup/static/pretix_sumup/sumup-logo-black.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:50:25.722372 pretix-sumup-1.0.4/pretix_sumup/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:50:25.726373 pretix-sumup-1.0.4/pretix_sumup/templates/pretix_sumup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:48:57.000000 pretix-sumup-1.0.4/pretix_sumup/templates/pretix_sumup/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-30 14:48:57.000000 pretix-sumup-1.0.4/pretix_sumup/templates/pretix_sumup/checkout_confirm_render.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-30 14:48:57.000000 pretix-sumup-1.0.4/pretix_sumup/templates/pretix_sumup/checkout_payment_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-30 14:48:57.000000 pretix-sumup-1.0.4/pretix_sumup/templates/pretix_sumup/control.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:50:25.726373 pretix-sumup-1.0.4/pretix_sumup/templates/pretix_sumup/email/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-30 14:48:57.000000 pretix-sumup-1.0.4/pretix_sumup/templates/pretix_sumup/email/order_pending.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-30 14:48:57.000000 pretix-sumup-1.0.4/pretix_sumup/templates/pretix_sumup/not_available.html
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-30 14:48:57.000000 pretix-sumup-1.0.4/pretix_sumup/templates/pretix_sumup/pending.html
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-30 14:48:57.000000 pretix-sumup-1.0.4/pretix_sumup/templates/pretix_sumup/prepare.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:50:25.722372 pretix-sumup-1.0.4/pretix_sumup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41111 2023-07-30 14:50:25.000000 pretix-sumup-1.0.4/pretix_sumup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-30 14:50:25.000000 pretix-sumup-1.0.4/pretix_sumup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 14:50:25.000000 pretix-sumup-1.0.4/pretix_sumup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-30 14:50:25.000000 pretix-sumup-1.0.4/pretix_sumup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-30 14:50:25.000000 pretix-sumup-1.0.4/pretix_sumup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-30 14:48:57.000000 pretix-sumup-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-30 14:50:25.726373 pretix-sumup-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-30 14:48:57.000000 pretix-sumup-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:50:25.726373 pretix-sumup-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-30 14:48:57.000000 pretix-sumup-1.0.4/tests/test_main.py
```

### Comparing `pretix-sumup-1.0.3a0/LICENSE` & `pretix-sumup-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.3a0/PKG-INFO` & `pretix-sumup-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-sumup
-Version: 1.0.3a0
+Version: 1.0.4
 Summary: Sumup plugin
 Author-email: Ronan Le Meillat <ronan@highcanfly.club>
 Maintainer-email: Ronan Le Meillat <ronan@highcanfly.club>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
         Version 3, 19 November 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `pretix-sumup-1.0.3a0/README.md` & `pretix-sumup-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.3a0/pretix_sumup/apps.py` & `pretix-sumup-1.0.4/pretix_sumup/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.3a0/pretix_sumup/locale/de/LC_MESSAGES/django.po` & `pretix-sumup-1.0.4/pretix_sumup/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.3a0/pretix_sumup/locale/de_Informal/LC_MESSAGES/django.po` & `pretix-sumup-1.0.4/pretix_sumup/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.3a0/pretix_sumup/locale/django.pot` & `pretix-sumup-1.0.4/pretix_sumup/locale/django.pot`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.3a0/pretix_sumup/locale/es/LC_MESSAGES/django.po` & `pretix-sumup-1.0.4/pretix_sumup/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.3a0/pretix_sumup/locale/fr/LC_MESSAGES/django.po` & `pretix-sumup-1.0.4/pretix_sumup/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.3a0/pretix_sumup/locale/it/LC_MESSAGES/django.po` & `pretix-sumup-1.0.4/pretix_sumup/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.3a0/pretix_sumup/payment.py` & `pretix-sumup-1.0.4/pretix_sumup/payment.py`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.3a0/pretix_sumup/signals.py` & `pretix-sumup-1.0.4/pretix_sumup/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.3a0/pretix_sumup/static/pretix_sumup/sumup-logo-black.svg` & `pretix-sumup-1.0.4/pretix_sumup/static/pretix_sumup/sumup-logo-black.svg`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.3a0/pretix_sumup/templates/pretix_sumup/checkout_payment_form.html` & `pretix-sumup-1.0.4/pretix_sumup/templates/pretix_sumup/checkout_payment_form.html`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.3a0/pretix_sumup/templates/pretix_sumup/control.html` & `pretix-sumup-1.0.4/pretix_sumup/templates/pretix_sumup/control.html`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.3a0/pretix_sumup.egg-info/PKG-INFO` & `pretix-sumup-1.0.4/pretix_sumup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-sumup
-Version: 1.0.3a0
+Version: 1.0.4
 Summary: Sumup plugin
 Author-email: Ronan Le Meillat <ronan@highcanfly.club>
 Maintainer-email: Ronan Le Meillat <ronan@highcanfly.club>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
         Version 3, 19 November 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `pretix-sumup-1.0.3a0/pretix_sumup.egg-info/SOURCES.txt` & `pretix-sumup-1.0.4/pretix_sumup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.3a0/pyproject.toml` & `pretix-sumup-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pretix-sumup-1.0.3a0/setup.cfg` & `pretix-sumup-1.0.4/setup.cfg`

 * *Files identical despite different names*

