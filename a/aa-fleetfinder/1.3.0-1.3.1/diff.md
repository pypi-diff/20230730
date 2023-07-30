# Comparing `tmp/aa_fleetfinder-1.3.0.tar.gz` & `tmp/aa_fleetfinder-1.3.1.tar.gz`

## Comparing `aa_fleetfinder-1.3.0.tar` & `aa_fleetfinder-1.3.1.tar`

### file list

```diff
@@ -1,58 +1,62 @@
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/__init__.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/apps.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/auth_hooks.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/constants.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/models.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/providers.py
--rw-r--r--   0        0        0    10529 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/tasks.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/urls.py
--rw-r--r--   0        0        0     9144 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/views.py
--rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/locale/django.pot
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5754 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     6564 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5209 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/migrations/0001_initial.py
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/migrations/0002_esi_error_handling_and_verbose_names.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/migrations/__init__.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/static/fleetfinder/css/aa-bootstrap-fix.css
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/static/fleetfinder/css/aa-bootstrap-fix.min.css
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/static/fleetfinder/css/fleetfinder.css
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/static/fleetfinder/css/fleetfinder.min.css
--rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/datetime.js
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/datetime.min.js
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/static/fleetfinder/libs/multi-select/0.9.12/css/multi-select.min.css
--rw-r--r--   0        0        0     6241 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/css/slimselect.min.css
--rw-r--r--   0        0        0    35554 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/js/slimselect.min.js
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/base.html
--rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/create-fleet.html
--rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/dashboard.html
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/edit-fleet.html
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/fleet-details.html
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/join-fleet.html
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/bundles/css/fleetfinder-css.html
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/bundles/css/multi-select-css.html
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/bundles/css/slim-select-css.html
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/bundles/js/datetime-js.html
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/bundles/js/slim-select-js.html
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/partials/header/header-navigation.html
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/templatetags/__init__.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/templatetags/fleetfinder_versioned_static.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/tests/__init__.py
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/tests/test_access.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/tests/test_auth_hooks.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/tests/test_templatetags.py
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/fleetfinder/tests/utils.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/LICENSE
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/README.md
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/__init__.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/apps.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/auth_hooks.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/constants.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/models.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/providers.py
+-rw-r--r--   0        0        0    10529 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/tasks.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/urls.py
+-rw-r--r--   0        0        0     9144 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/docs/screenshots/weblate/.gitkeep
+-rw-r--r--   0        0        0    31860 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/docs/screenshots/weblate/aa-fleetfinder-available-fleets-overview.jpg
+-rw-r--r--   0        0        0    57101 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/docs/screenshots/weblate/aa-fleetfinder-create-fleet-form.jpg
+-rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/locale/django.pot
+-rw-r--r--   0        0        0     3826 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     6376 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4953 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7237 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5971 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4953 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/migrations/0001_initial.py
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/migrations/0002_esi_error_handling_and_verbose_names.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/migrations/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/static/fleetfinder/css/aa-bootstrap-fix.css
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/static/fleetfinder/css/aa-bootstrap-fix.min.css
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/static/fleetfinder/css/fleetfinder.css
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/static/fleetfinder/css/fleetfinder.min.css
+-rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/datetime.js
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/datetime.min.js
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/static/fleetfinder/libs/multi-select/0.9.12/css/multi-select.min.css
+-rw-r--r--   0        0        0     6241 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/css/slimselect.min.css
+-rw-r--r--   0        0        0    35554 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/js/slimselect.min.js
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/templates/fleetfinder/base.html
+-rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/templates/fleetfinder/create-fleet.html
+-rw-r--r--   0        0        0     4546 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/templates/fleetfinder/dashboard.html
+-rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/templates/fleetfinder/edit-fleet.html
+-rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/templates/fleetfinder/fleet-details.html
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/templates/fleetfinder/join-fleet.html
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/templates/fleetfinder/bundles/css/fleetfinder-css.html
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/templates/fleetfinder/bundles/css/multi-select-css.html
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/templates/fleetfinder/bundles/css/slim-select-css.html
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/templates/fleetfinder/bundles/js/datetime-js.html
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/templates/fleetfinder/bundles/js/slim-select-js.html
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/templates/fleetfinder/partials/footer/app-translation-footer.html
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/templates/fleetfinder/partials/header/header-navigation.html
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/templatetags/__init__.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/templatetags/fleetfinder_versioned_static.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/tests/__init__.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/tests/test_access.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/tests/test_templatetags.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/fleetfinder/tests/utils.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/LICENSE
+-rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/README.md
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5807 2020-02-02 00:00:00.000000 aa_fleetfinder-1.3.1/PKG-INFO
```

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/auth_hooks.py` & `aa_fleetfinder-1.3.1/fleetfinder/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/models.py` & `aa_fleetfinder-1.3.1/fleetfinder/models.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/tasks.py` & `aa_fleetfinder-1.3.1/fleetfinder/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/urls.py` & `aa_fleetfinder-1.3.1/fleetfinder/urls.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/views.py` & `aa_fleetfinder-1.3.1/fleetfinder/views.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/locale/django.pot` & `aa_fleetfinder-1.3.1/fleetfinder/locale/django.pot`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 15:41+0200\n"
+"POT-Creation-Date: 2023-07-27 23:27+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -40,28 +40,28 @@
 msgid "FC is no longer the fleet boss."
 msgstr ""
 
 #: models.py:48
 msgid "FC switched to another fleet."
 msgstr ""
 
-#: models.py:51 templates/fleetfinder/create-fleet.html:25
+#: models.py:51 templates/fleetfinder/create-fleet.html:27
 #: templates/fleetfinder/edit-fleet.html:27
 msgid "Fleet Name"
 msgstr ""
 
 #: models.py:59 templates/fleetfinder/dashboard.html:17
 msgid "Fleet Commander"
 msgstr ""
 
 #: models.py:61
 msgid "Creation date and time"
 msgstr ""
 
-#: models.py:62 templates/fleetfinder/create-fleet.html:59
+#: models.py:62 templates/fleetfinder/create-fleet.html:62
 #: templates/fleetfinder/edit-fleet.html:58
 msgid "Fleet MOTD"
 msgstr ""
 
 #: models.py:63
 msgid "Free move"
 msgstr ""
@@ -79,37 +79,37 @@
 msgstr ""
 
 #: models.py:84
 msgid "ESI error count"
 msgstr ""
 
 #: templates/fleetfinder/create-fleet.html:5
-#: templates/fleetfinder/create-fleet.html:10
+#: templates/fleetfinder/create-fleet.html:11
 #: templates/fleetfinder/partials/header/header-navigation.html:18
 msgid "Create Fleet"
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:34
+#: templates/fleetfinder/create-fleet.html:36
 #: templates/fleetfinder/edit-fleet.html:36
 msgid "Select Groups"
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:36
+#: templates/fleetfinder/create-fleet.html:39
 #: templates/fleetfinder/edit-fleet.html:39
 msgid ""
 "Only selected groups will have access to the fleet. If no groups are "
-"selected the fleet will be available to all of the authed groups."
+"selected the fleet will be available to all who have access to this module."
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:69
+#: templates/fleetfinder/create-fleet.html:72
 #: templates/fleetfinder/edit-fleet.html:68
 msgid "Enable Free Move"
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:71
+#: templates/fleetfinder/create-fleet.html:74
 #: templates/fleetfinder/edit-fleet.html:70
 msgid "Submit"
 msgstr ""
 
 #: templates/fleetfinder/dashboard.html:9
 #: templates/fleetfinder/partials/header/header-navigation.html:13
 msgid "Available Fleets"
@@ -178,15 +178,28 @@
 msgstr ""
 
 #: templates/fleetfinder/join-fleet.html:21
 msgid "Select the characters to invite"
 msgstr ""
 
 #: templates/fleetfinder/join-fleet.html:29
-msgid "Send fleet invite(s)"
+msgid "Send fleet invites"
+msgstr ""
+
+#: templates/fleetfinder/partials/footer/app-translation-footer.html:4
+msgid "Join our team of translators!"
+msgstr ""
+
+#: templates/fleetfinder/partials/footer/app-translation-footer.html:7
+#, python-format
+msgid ""
+"\n"
+"            Do you want to help translate this app into your language or "
+"improve the existing translation? - %(weblate_link)s\n"
+"        "
 msgstr ""
 
 #: templates/fleetfinder/partials/header/header-navigation.html:7
 msgid "Toggle navigation"
 msgstr ""
 
 #: views.py:92
```

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/locale/de/LC_MESSAGES/django.mo` & `aa_fleetfinder-1.3.1/fleetfinder/locale/de/LC_MESSAGES/django.mo`

 * *Files 23% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,26 @@
 "Language-Team: German <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-fleetfinder/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.18.1\n"
+"X-Generator: Weblate 4.18.2\n"
+
+msgid ""
+"\n"
+"            Do you want to help translate this app into your language or "
+"improve the existing translation? - %(weblate_link)s\n"
+"        "
+msgstr ""
+"\n"
+"            Du möchtest helfen diese App in Deine Sprache zu übersetzen oder "
+"die bestehende Übersetzung verbessern? - %(weblate_link)s\n"
+"        "
 
 msgid ""
 "<h4>Error!</h4><p>ESI returned the following error: {esi_error_message}</p>"
 msgstr ""
 "<h4>Fehler!</h4><p>ESI hat den folgenden Fehler zurückgegeben: "
 "{esi_error_message}</p>"
 
@@ -96,44 +107,48 @@
 
 msgid "Join"
 msgstr "Beitreten"
 
 msgid "Join Fleet"
 msgstr "Flotte beitreten"
 
+msgid "Join our team of translators!"
+msgstr "Tritt unserm Team von Übersetzern bei!"
+
 msgid "Last ESI error"
 msgstr "Letzter ESI Fehler"
 
 msgid "Last ESI error time"
 msgstr "Zeitpunkt des letzten ESI Fehlers"
 
 msgid "Name"
 msgstr "Name"
 
 msgid ""
 "Only selected groups will have access to the fleet. If no groups are "
-"selected the fleet will be available to all of the authed groups."
+"selected the fleet will be available to all who have access to this module."
 msgstr ""
 "Nur die ausgewählten Gruppen haben Zugriff zu dieser Flotte. Wenn keine "
-"Gruppen ausgewählt sind ist die Flotte für alle verfügbar."
+"Gruppen ausgewählt sind, ist die Flotte für alle die Zugriff auf dieses "
+"Modul haben verfügbar."
 
 msgid "Quantity"
 msgstr "Anzahl"
 
 msgid "Registered fleet seems to be no longer available."
 msgstr "Die registrierte Flotte scheint nicht mehr verfügbar zu sein."
 
 msgid "Select Groups"
 msgstr "Gruppenauswahl"
 
 msgid "Select the characters to invite"
 msgstr "Wähle einzuladende Charaktere"
 
-msgid "Send fleet invite(s)"
-msgstr "Flotteneinladung(en) senden"
+msgid "Send fleet invites"
+msgstr "Flotteneinladungen senden"
 
 msgid "Ship Name"
 msgstr "Schiffsname"
 
 msgid "Ship type"
 msgstr "Schiffstyp"
```

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/locale/de/LC_MESSAGES/django.po` & `aa_fleetfinder-1.3.1/fleetfinder/locale/de/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 15:41+0200\n"
-"PO-Revision-Date: 2023-06-29 14:19+0000\n"
+"POT-Creation-Date: 2023-07-27 23:27+0200\n"
+"PO-Revision-Date: 2023-07-28 22:39+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
 "Language-Team: German <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-fleetfinder/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.18.1\n"
+"X-Generator: Weblate 4.18.2\n"
 
 #: __init__.py:12 templates/fleetfinder/base.html:5
 msgid "Fleet Finder"
 msgstr "Flottenfinder"
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: apps.py:21
@@ -43,28 +43,28 @@
 msgid "FC is no longer the fleet boss."
 msgstr "Der FC ist nicht länger Flottenchef."
 
 #: models.py:48
 msgid "FC switched to another fleet."
 msgstr "Der FC wechselte zu einer anderen Flotte."
 
-#: models.py:51 templates/fleetfinder/create-fleet.html:25
+#: models.py:51 templates/fleetfinder/create-fleet.html:27
 #: templates/fleetfinder/edit-fleet.html:27
 msgid "Fleet Name"
 msgstr "Flottenname"
 
 #: models.py:59 templates/fleetfinder/dashboard.html:17
 msgid "Fleet Commander"
 msgstr "Flottenkommandant"
 
 #: models.py:61
 msgid "Creation date and time"
 msgstr "Erstellungsdatum und -uhrzeit"
 
-#: models.py:62 templates/fleetfinder/create-fleet.html:59
+#: models.py:62 templates/fleetfinder/create-fleet.html:62
 #: templates/fleetfinder/edit-fleet.html:58
 msgid "Fleet MOTD"
 msgstr "Flotten MOTD"
 
 #: models.py:63
 msgid "Free move"
 msgstr "Freie Bewegung"
@@ -82,39 +82,40 @@
 msgstr "Zeitpunkt des letzten ESI Fehlers"
 
 #: models.py:84
 msgid "ESI error count"
 msgstr "Anzahl der ESI Fehler"
 
 #: templates/fleetfinder/create-fleet.html:5
-#: templates/fleetfinder/create-fleet.html:10
+#: templates/fleetfinder/create-fleet.html:11
 #: templates/fleetfinder/partials/header/header-navigation.html:18
 msgid "Create Fleet"
 msgstr "Flotte erstellen"
 
-#: templates/fleetfinder/create-fleet.html:34
+#: templates/fleetfinder/create-fleet.html:36
 #: templates/fleetfinder/edit-fleet.html:36
 msgid "Select Groups"
 msgstr "Gruppenauswahl"
 
-#: templates/fleetfinder/create-fleet.html:36
+#: templates/fleetfinder/create-fleet.html:39
 #: templates/fleetfinder/edit-fleet.html:39
 msgid ""
 "Only selected groups will have access to the fleet. If no groups are "
-"selected the fleet will be available to all of the authed groups."
+"selected the fleet will be available to all who have access to this module."
 msgstr ""
 "Nur die ausgewählten Gruppen haben Zugriff zu dieser Flotte. Wenn keine "
-"Gruppen ausgewählt sind ist die Flotte für alle verfügbar."
+"Gruppen ausgewählt sind, ist die Flotte für alle die Zugriff auf dieses "
+"Modul haben verfügbar."
 
-#: templates/fleetfinder/create-fleet.html:69
+#: templates/fleetfinder/create-fleet.html:72
 #: templates/fleetfinder/edit-fleet.html:68
 msgid "Enable Free Move"
 msgstr "Freie Bewegung aktivieren"
 
-#: templates/fleetfinder/create-fleet.html:71
+#: templates/fleetfinder/create-fleet.html:74
 #: templates/fleetfinder/edit-fleet.html:70
 msgid "Submit"
 msgstr "Absenden"
 
 #: templates/fleetfinder/dashboard.html:9
 #: templates/fleetfinder/partials/header/header-navigation.html:13
 msgid "Available Fleets"
@@ -183,16 +184,33 @@
 msgstr "Flotteneinladung"
 
 #: templates/fleetfinder/join-fleet.html:21
 msgid "Select the characters to invite"
 msgstr "Wähle einzuladende Charaktere"
 
 #: templates/fleetfinder/join-fleet.html:29
-msgid "Send fleet invite(s)"
-msgstr "Flotteneinladung(en) senden"
+msgid "Send fleet invites"
+msgstr "Flotteneinladungen senden"
+
+#: templates/fleetfinder/partials/footer/app-translation-footer.html:4
+msgid "Join our team of translators!"
+msgstr "Tritt unserm Team von Übersetzern bei!"
+
+#: templates/fleetfinder/partials/footer/app-translation-footer.html:7
+#, python-format
+msgid ""
+"\n"
+"            Do you want to help translate this app into your language or "
+"improve the existing translation? - %(weblate_link)s\n"
+"        "
+msgstr ""
+"\n"
+"            Du möchtest helfen diese App in Deine Sprache zu übersetzen oder "
+"die bestehende Übersetzung verbessern? - %(weblate_link)s\n"
+"        "
 
 #: templates/fleetfinder/partials/header/header-navigation.html:7
 msgid "Toggle navigation"
 msgstr "Navigation umschalten"
 
 #: views.py:92
 msgid "View Fleet Details"
```

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/locale/es/LC_MESSAGES/django.po` & `aa_fleetfinder-1.3.1/fleetfinder/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files 9% similar despite different names*

```diff
@@ -4,23 +4,22 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 15:41+0200\n"
+"POT-Creation-Date: 2023-07-27 23:27+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: __init__.py:12 templates/fleetfinder/base.html:5
 msgid "Fleet Finder"
 msgstr ""
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: apps.py:21
@@ -41,28 +40,28 @@
 msgid "FC is no longer the fleet boss."
 msgstr ""
 
 #: models.py:48
 msgid "FC switched to another fleet."
 msgstr ""
 
-#: models.py:51 templates/fleetfinder/create-fleet.html:25
+#: models.py:51 templates/fleetfinder/create-fleet.html:27
 #: templates/fleetfinder/edit-fleet.html:27
 msgid "Fleet Name"
 msgstr ""
 
 #: models.py:59 templates/fleetfinder/dashboard.html:17
 msgid "Fleet Commander"
 msgstr ""
 
 #: models.py:61
 msgid "Creation date and time"
 msgstr ""
 
-#: models.py:62 templates/fleetfinder/create-fleet.html:59
+#: models.py:62 templates/fleetfinder/create-fleet.html:62
 #: templates/fleetfinder/edit-fleet.html:58
 msgid "Fleet MOTD"
 msgstr ""
 
 #: models.py:63
 msgid "Free move"
 msgstr ""
@@ -80,37 +79,37 @@
 msgstr ""
 
 #: models.py:84
 msgid "ESI error count"
 msgstr ""
 
 #: templates/fleetfinder/create-fleet.html:5
-#: templates/fleetfinder/create-fleet.html:10
+#: templates/fleetfinder/create-fleet.html:11
 #: templates/fleetfinder/partials/header/header-navigation.html:18
 msgid "Create Fleet"
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:34
+#: templates/fleetfinder/create-fleet.html:36
 #: templates/fleetfinder/edit-fleet.html:36
 msgid "Select Groups"
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:36
+#: templates/fleetfinder/create-fleet.html:39
 #: templates/fleetfinder/edit-fleet.html:39
 msgid ""
 "Only selected groups will have access to the fleet. If no groups are "
-"selected the fleet will be available to all of the authed groups."
+"selected the fleet will be available to all who have access to this module."
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:69
+#: templates/fleetfinder/create-fleet.html:72
 #: templates/fleetfinder/edit-fleet.html:68
 msgid "Enable Free Move"
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:71
+#: templates/fleetfinder/create-fleet.html:74
 #: templates/fleetfinder/edit-fleet.html:70
 msgid "Submit"
 msgstr ""
 
 #: templates/fleetfinder/dashboard.html:9
 #: templates/fleetfinder/partials/header/header-navigation.html:13
 msgid "Available Fleets"
@@ -179,15 +178,28 @@
 msgstr ""
 
 #: templates/fleetfinder/join-fleet.html:21
 msgid "Select the characters to invite"
 msgstr ""
 
 #: templates/fleetfinder/join-fleet.html:29
-msgid "Send fleet invite(s)"
+msgid "Send fleet invites"
+msgstr ""
+
+#: templates/fleetfinder/partials/footer/app-translation-footer.html:4
+msgid "Join our team of translators!"
+msgstr ""
+
+#: templates/fleetfinder/partials/footer/app-translation-footer.html:7
+#, python-format
+msgid ""
+"\n"
+"            Do you want to help translate this app into your language or "
+"improve the existing translation? - %(weblate_link)s\n"
+"        "
 msgstr ""
 
 #: templates/fleetfinder/partials/header/header-navigation.html:7
 msgid "Toggle navigation"
 msgstr ""
 
 #: views.py:92
```

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/locale/fr_FR/LC_MESSAGES/django.po` & `aa_fleetfinder-1.3.1/fleetfinder/locale/it_IT/LC_MESSAGES/django.po`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 15:41+0200\n"
+"POT-Creation-Date: 2023-07-27 23:27+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -40,28 +40,28 @@
 msgid "FC is no longer the fleet boss."
 msgstr ""
 
 #: models.py:48
 msgid "FC switched to another fleet."
 msgstr ""
 
-#: models.py:51 templates/fleetfinder/create-fleet.html:25
+#: models.py:51 templates/fleetfinder/create-fleet.html:27
 #: templates/fleetfinder/edit-fleet.html:27
 msgid "Fleet Name"
 msgstr ""
 
 #: models.py:59 templates/fleetfinder/dashboard.html:17
 msgid "Fleet Commander"
 msgstr ""
 
 #: models.py:61
 msgid "Creation date and time"
 msgstr ""
 
-#: models.py:62 templates/fleetfinder/create-fleet.html:59
+#: models.py:62 templates/fleetfinder/create-fleet.html:62
 #: templates/fleetfinder/edit-fleet.html:58
 msgid "Fleet MOTD"
 msgstr ""
 
 #: models.py:63
 msgid "Free move"
 msgstr ""
@@ -79,37 +79,37 @@
 msgstr ""
 
 #: models.py:84
 msgid "ESI error count"
 msgstr ""
 
 #: templates/fleetfinder/create-fleet.html:5
-#: templates/fleetfinder/create-fleet.html:10
+#: templates/fleetfinder/create-fleet.html:11
 #: templates/fleetfinder/partials/header/header-navigation.html:18
 msgid "Create Fleet"
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:34
+#: templates/fleetfinder/create-fleet.html:36
 #: templates/fleetfinder/edit-fleet.html:36
 msgid "Select Groups"
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:36
+#: templates/fleetfinder/create-fleet.html:39
 #: templates/fleetfinder/edit-fleet.html:39
 msgid ""
 "Only selected groups will have access to the fleet. If no groups are "
-"selected the fleet will be available to all of the authed groups."
+"selected the fleet will be available to all who have access to this module."
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:69
+#: templates/fleetfinder/create-fleet.html:72
 #: templates/fleetfinder/edit-fleet.html:68
 msgid "Enable Free Move"
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:71
+#: templates/fleetfinder/create-fleet.html:74
 #: templates/fleetfinder/edit-fleet.html:70
 msgid "Submit"
 msgstr ""
 
 #: templates/fleetfinder/dashboard.html:9
 #: templates/fleetfinder/partials/header/header-navigation.html:13
 msgid "Available Fleets"
@@ -178,15 +178,28 @@
 msgstr ""
 
 #: templates/fleetfinder/join-fleet.html:21
 msgid "Select the characters to invite"
 msgstr ""
 
 #: templates/fleetfinder/join-fleet.html:29
-msgid "Send fleet invite(s)"
+msgid "Send fleet invites"
+msgstr ""
+
+#: templates/fleetfinder/partials/footer/app-translation-footer.html:4
+msgid "Join our team of translators!"
+msgstr ""
+
+#: templates/fleetfinder/partials/footer/app-translation-footer.html:7
+#, python-format
+msgid ""
+"\n"
+"            Do you want to help translate this app into your language or "
+"improve the existing translation? - %(weblate_link)s\n"
+"        "
 msgstr ""
 
 #: templates/fleetfinder/partials/header/header-navigation.html:7
 msgid "Toggle navigation"
 msgstr ""
 
 #: views.py:92
```

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/locale/it_IT/LC_MESSAGES/django.po` & `aa_fleetfinder-1.3.1/fleetfinder/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 15:41+0200\n"
+"POT-Creation-Date: 2023-07-27 23:27+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -40,28 +40,28 @@
 msgid "FC is no longer the fleet boss."
 msgstr ""
 
 #: models.py:48
 msgid "FC switched to another fleet."
 msgstr ""
 
-#: models.py:51 templates/fleetfinder/create-fleet.html:25
+#: models.py:51 templates/fleetfinder/create-fleet.html:27
 #: templates/fleetfinder/edit-fleet.html:27
 msgid "Fleet Name"
 msgstr ""
 
 #: models.py:59 templates/fleetfinder/dashboard.html:17
 msgid "Fleet Commander"
 msgstr ""
 
 #: models.py:61
 msgid "Creation date and time"
 msgstr ""
 
-#: models.py:62 templates/fleetfinder/create-fleet.html:59
+#: models.py:62 templates/fleetfinder/create-fleet.html:62
 #: templates/fleetfinder/edit-fleet.html:58
 msgid "Fleet MOTD"
 msgstr ""
 
 #: models.py:63
 msgid "Free move"
 msgstr ""
@@ -79,37 +79,37 @@
 msgstr ""
 
 #: models.py:84
 msgid "ESI error count"
 msgstr ""
 
 #: templates/fleetfinder/create-fleet.html:5
-#: templates/fleetfinder/create-fleet.html:10
+#: templates/fleetfinder/create-fleet.html:11
 #: templates/fleetfinder/partials/header/header-navigation.html:18
 msgid "Create Fleet"
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:34
+#: templates/fleetfinder/create-fleet.html:36
 #: templates/fleetfinder/edit-fleet.html:36
 msgid "Select Groups"
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:36
+#: templates/fleetfinder/create-fleet.html:39
 #: templates/fleetfinder/edit-fleet.html:39
 msgid ""
 "Only selected groups will have access to the fleet. If no groups are "
-"selected the fleet will be available to all of the authed groups."
+"selected the fleet will be available to all who have access to this module."
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:69
+#: templates/fleetfinder/create-fleet.html:72
 #: templates/fleetfinder/edit-fleet.html:68
 msgid "Enable Free Move"
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:71
+#: templates/fleetfinder/create-fleet.html:74
 #: templates/fleetfinder/edit-fleet.html:70
 msgid "Submit"
 msgstr ""
 
 #: templates/fleetfinder/dashboard.html:9
 #: templates/fleetfinder/partials/header/header-navigation.html:13
 msgid "Available Fleets"
@@ -178,15 +178,28 @@
 msgstr ""
 
 #: templates/fleetfinder/join-fleet.html:21
 msgid "Select the characters to invite"
 msgstr ""
 
 #: templates/fleetfinder/join-fleet.html:29
-msgid "Send fleet invite(s)"
+msgid "Send fleet invites"
+msgstr ""
+
+#: templates/fleetfinder/partials/footer/app-translation-footer.html:4
+msgid "Join our team of translators!"
+msgstr ""
+
+#: templates/fleetfinder/partials/footer/app-translation-footer.html:7
+#, python-format
+msgid ""
+"\n"
+"            Do you want to help translate this app into your language or "
+"improve the existing translation? - %(weblate_link)s\n"
+"        "
 msgstr ""
 
 #: templates/fleetfinder/partials/header/header-navigation.html:7
 msgid "Toggle navigation"
 msgstr ""
 
 #: views.py:92
```

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/locale/ja/LC_MESSAGES/django.po` & `aa_fleetfinder-1.3.1/fleetfinder/locale/es/LC_MESSAGES/django.po`

 * *Files 22% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 15:41+0200\n"
+"POT-Creation-Date: 2023-07-27 23:27+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: __init__.py:12 templates/fleetfinder/base.html:5
 msgid "Fleet Finder"
 msgstr ""
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: apps.py:21
@@ -41,28 +41,28 @@
 msgid "FC is no longer the fleet boss."
 msgstr ""
 
 #: models.py:48
 msgid "FC switched to another fleet."
 msgstr ""
 
-#: models.py:51 templates/fleetfinder/create-fleet.html:25
+#: models.py:51 templates/fleetfinder/create-fleet.html:27
 #: templates/fleetfinder/edit-fleet.html:27
 msgid "Fleet Name"
 msgstr ""
 
 #: models.py:59 templates/fleetfinder/dashboard.html:17
 msgid "Fleet Commander"
 msgstr ""
 
 #: models.py:61
 msgid "Creation date and time"
 msgstr ""
 
-#: models.py:62 templates/fleetfinder/create-fleet.html:59
+#: models.py:62 templates/fleetfinder/create-fleet.html:62
 #: templates/fleetfinder/edit-fleet.html:58
 msgid "Fleet MOTD"
 msgstr ""
 
 #: models.py:63
 msgid "Free move"
 msgstr ""
@@ -80,37 +80,37 @@
 msgstr ""
 
 #: models.py:84
 msgid "ESI error count"
 msgstr ""
 
 #: templates/fleetfinder/create-fleet.html:5
-#: templates/fleetfinder/create-fleet.html:10
+#: templates/fleetfinder/create-fleet.html:11
 #: templates/fleetfinder/partials/header/header-navigation.html:18
 msgid "Create Fleet"
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:34
+#: templates/fleetfinder/create-fleet.html:36
 #: templates/fleetfinder/edit-fleet.html:36
 msgid "Select Groups"
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:36
+#: templates/fleetfinder/create-fleet.html:39
 #: templates/fleetfinder/edit-fleet.html:39
 msgid ""
 "Only selected groups will have access to the fleet. If no groups are "
-"selected the fleet will be available to all of the authed groups."
+"selected the fleet will be available to all who have access to this module."
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:69
+#: templates/fleetfinder/create-fleet.html:72
 #: templates/fleetfinder/edit-fleet.html:68
 msgid "Enable Free Move"
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:71
+#: templates/fleetfinder/create-fleet.html:74
 #: templates/fleetfinder/edit-fleet.html:70
 msgid "Submit"
 msgstr ""
 
 #: templates/fleetfinder/dashboard.html:9
 #: templates/fleetfinder/partials/header/header-navigation.html:13
 msgid "Available Fleets"
@@ -179,15 +179,28 @@
 msgstr ""
 
 #: templates/fleetfinder/join-fleet.html:21
 msgid "Select the characters to invite"
 msgstr ""
 
 #: templates/fleetfinder/join-fleet.html:29
-msgid "Send fleet invite(s)"
+msgid "Send fleet invites"
+msgstr ""
+
+#: templates/fleetfinder/partials/footer/app-translation-footer.html:4
+msgid "Join our team of translators!"
+msgstr ""
+
+#: templates/fleetfinder/partials/footer/app-translation-footer.html:7
+#, python-format
+msgid ""
+"\n"
+"            Do you want to help translate this app into your language or "
+"improve the existing translation? - %(weblate_link)s\n"
+"        "
 msgstr ""
 
 #: templates/fleetfinder/partials/header/header-navigation.html:7
 msgid "Toggle navigation"
 msgstr ""
 
 #: views.py:92
```

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/locale/ko_KR/LC_MESSAGES/django.po` & `aa_fleetfinder-1.3.1/fleetfinder/locale/ja/LC_MESSAGES/django.po`

 * *Files 22% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 15:41+0200\n"
+"POT-Creation-Date: 2023-07-27 23:27+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: __init__.py:12 templates/fleetfinder/base.html:5
 msgid "Fleet Finder"
 msgstr ""
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: apps.py:21
@@ -40,28 +41,28 @@
 msgid "FC is no longer the fleet boss."
 msgstr ""
 
 #: models.py:48
 msgid "FC switched to another fleet."
 msgstr ""
 
-#: models.py:51 templates/fleetfinder/create-fleet.html:25
+#: models.py:51 templates/fleetfinder/create-fleet.html:27
 #: templates/fleetfinder/edit-fleet.html:27
 msgid "Fleet Name"
 msgstr ""
 
 #: models.py:59 templates/fleetfinder/dashboard.html:17
 msgid "Fleet Commander"
 msgstr ""
 
 #: models.py:61
 msgid "Creation date and time"
 msgstr ""
 
-#: models.py:62 templates/fleetfinder/create-fleet.html:59
+#: models.py:62 templates/fleetfinder/create-fleet.html:62
 #: templates/fleetfinder/edit-fleet.html:58
 msgid "Fleet MOTD"
 msgstr ""
 
 #: models.py:63
 msgid "Free move"
 msgstr ""
@@ -79,37 +80,37 @@
 msgstr ""
 
 #: models.py:84
 msgid "ESI error count"
 msgstr ""
 
 #: templates/fleetfinder/create-fleet.html:5
-#: templates/fleetfinder/create-fleet.html:10
+#: templates/fleetfinder/create-fleet.html:11
 #: templates/fleetfinder/partials/header/header-navigation.html:18
 msgid "Create Fleet"
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:34
+#: templates/fleetfinder/create-fleet.html:36
 #: templates/fleetfinder/edit-fleet.html:36
 msgid "Select Groups"
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:36
+#: templates/fleetfinder/create-fleet.html:39
 #: templates/fleetfinder/edit-fleet.html:39
 msgid ""
 "Only selected groups will have access to the fleet. If no groups are "
-"selected the fleet will be available to all of the authed groups."
+"selected the fleet will be available to all who have access to this module."
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:69
+#: templates/fleetfinder/create-fleet.html:72
 #: templates/fleetfinder/edit-fleet.html:68
 msgid "Enable Free Move"
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:71
+#: templates/fleetfinder/create-fleet.html:74
 #: templates/fleetfinder/edit-fleet.html:70
 msgid "Submit"
 msgstr ""
 
 #: templates/fleetfinder/dashboard.html:9
 #: templates/fleetfinder/partials/header/header-navigation.html:13
 msgid "Available Fleets"
@@ -178,15 +179,28 @@
 msgstr ""
 
 #: templates/fleetfinder/join-fleet.html:21
 msgid "Select the characters to invite"
 msgstr ""
 
 #: templates/fleetfinder/join-fleet.html:29
-msgid "Send fleet invite(s)"
+msgid "Send fleet invites"
+msgstr ""
+
+#: templates/fleetfinder/partials/footer/app-translation-footer.html:4
+msgid "Join our team of translators!"
+msgstr ""
+
+#: templates/fleetfinder/partials/footer/app-translation-footer.html:7
+#, python-format
+msgid ""
+"\n"
+"            Do you want to help translate this app into your language or "
+"improve the existing translation? - %(weblate_link)s\n"
+"        "
 msgstr ""
 
 #: templates/fleetfinder/partials/header/header-navigation.html:7
 msgid "Toggle navigation"
 msgstr ""
 
 #: views.py:92
```

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/locale/ru/LC_MESSAGES/django.mo` & `aa_fleetfinder-1.3.1/fleetfinder/locale/ru/LC_MESSAGES/django.mo`

 * *Files 23% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,26 @@
 "apps/aa-fleetfinder/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 4.18.1\n"
+"X-Generator: Weblate 4.18.2\n"
+
+msgid ""
+"\n"
+"            Do you want to help translate this app into your language or "
+"improve the existing translation? - %(weblate_link)s\n"
+"        "
+msgstr ""
+"\n"
+"            Вы хотите помочь перевести это приложение на ваш язык или "
+"улучшить текущий перевод? - %(weblate_link)s\n"
+"        "
 
 msgid ""
 "<h4>Error!</h4><p>ESI returned the following error: {esi_error_message}</p>"
 msgstr ""
 "<h4>Ошибка!</h4><p>ESI вернул следующую ошибку: {esi_error_message}</p>"
 
 msgid "Available Fleets"
@@ -94,44 +105,47 @@
 
 msgid "Join"
 msgstr "Присоединиться"
 
 msgid "Join Fleet"
 msgstr "Присоединиться к флоту"
 
+msgid "Join our team of translators!"
+msgstr "Присоединяйтесь к нашей команде переводчиков!"
+
 msgid "Last ESI error"
 msgstr "Последняя ESI ошибка"
 
 msgid "Last ESI error time"
 msgstr "Время последней ESI ошибки"
 
 msgid "Name"
 msgstr "Название"
 
 msgid ""
 "Only selected groups will have access to the fleet. If no groups are "
-"selected the fleet will be available to all of the authed groups."
+"selected the fleet will be available to all who have access to this module."
 msgstr ""
 "Только выбранные группы будут иметь доступ к флоту. Если группы не выбраны, "
-"флот будет доступен всем авторизованным группам."
+"флот будет доступен всем пользователям модуля."
 
 msgid "Quantity"
 msgstr "Количество"
 
 msgid "Registered fleet seems to be no longer available."
 msgstr "Похоже, зарегистрированный флот больше недоступен."
 
 msgid "Select Groups"
 msgstr "Выбор групп"
 
 msgid "Select the characters to invite"
 msgstr "Выберите пилота для приглашения"
 
-msgid "Send fleet invite(s)"
-msgstr "Отправить приглашение(я)"
+msgid "Send fleet invites"
+msgstr "Отправить приглашения"
 
 msgid "Ship Name"
 msgstr "Название корабля"
 
 msgid "Ship type"
 msgstr "Тип корабля"
```

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/locale/ru/LC_MESSAGES/django.po` & `aa_fleetfinder-1.3.1/fleetfinder/locale/ru/LC_MESSAGES/django.po`

 * *Files 12% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 # This file is distributed under the same license as the PACKAGE package.
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
 # Nikolay <nick.postnikov@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 15:41+0200\n"
-"PO-Revision-Date: 2023-06-29 14:19+0000\n"
+"POT-Creation-Date: 2023-07-27 23:27+0200\n"
+"PO-Revision-Date: 2023-07-29 23:45+0000\n"
 "Last-Translator: Nikolay <nick.postnikov@gmail.com>\n"
 "Language-Team: Russian <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-fleetfinder/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 4.18.1\n"
+"X-Generator: Weblate 4.18.2\n"
 
 #: __init__.py:12 templates/fleetfinder/base.html:5
 msgid "Fleet Finder"
 msgstr "Поиск флота"
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: apps.py:21
@@ -43,28 +43,28 @@
 msgid "FC is no longer the fleet boss."
 msgstr "ФК больше не руководитель флота."
 
 #: models.py:48
 msgid "FC switched to another fleet."
 msgstr "ФК перешел в другой флот."
 
-#: models.py:51 templates/fleetfinder/create-fleet.html:25
+#: models.py:51 templates/fleetfinder/create-fleet.html:27
 #: templates/fleetfinder/edit-fleet.html:27
 msgid "Fleet Name"
 msgstr "Название флота"
 
 #: models.py:59 templates/fleetfinder/dashboard.html:17
 msgid "Fleet Commander"
 msgstr "Командир флота"
 
 #: models.py:61
 msgid "Creation date and time"
 msgstr "Дата и время создания"
 
-#: models.py:62 templates/fleetfinder/create-fleet.html:59
+#: models.py:62 templates/fleetfinder/create-fleet.html:62
 #: templates/fleetfinder/edit-fleet.html:58
 msgid "Fleet MOTD"
 msgstr "MOTD флота"
 
 #: models.py:63
 msgid "Free move"
 msgstr "Свободное перемещение"
@@ -82,39 +82,39 @@
 msgstr "Время последней ESI ошибки"
 
 #: models.py:84
 msgid "ESI error count"
 msgstr "Счетчик ESI ошибок"
 
 #: templates/fleetfinder/create-fleet.html:5
-#: templates/fleetfinder/create-fleet.html:10
+#: templates/fleetfinder/create-fleet.html:11
 #: templates/fleetfinder/partials/header/header-navigation.html:18
 msgid "Create Fleet"
 msgstr "Создание флота"
 
-#: templates/fleetfinder/create-fleet.html:34
+#: templates/fleetfinder/create-fleet.html:36
 #: templates/fleetfinder/edit-fleet.html:36
 msgid "Select Groups"
 msgstr "Выбор групп"
 
-#: templates/fleetfinder/create-fleet.html:36
+#: templates/fleetfinder/create-fleet.html:39
 #: templates/fleetfinder/edit-fleet.html:39
 msgid ""
 "Only selected groups will have access to the fleet. If no groups are "
-"selected the fleet will be available to all of the authed groups."
+"selected the fleet will be available to all who have access to this module."
 msgstr ""
 "Только выбранные группы будут иметь доступ к флоту. Если группы не выбраны, "
-"флот будет доступен всем авторизованным группам."
+"флот будет доступен всем пользователям модуля."
 
-#: templates/fleetfinder/create-fleet.html:69
+#: templates/fleetfinder/create-fleet.html:72
 #: templates/fleetfinder/edit-fleet.html:68
 msgid "Enable Free Move"
 msgstr "Разрешить Free Move"
 
-#: templates/fleetfinder/create-fleet.html:71
+#: templates/fleetfinder/create-fleet.html:74
 #: templates/fleetfinder/edit-fleet.html:70
 msgid "Submit"
 msgstr "Отправить"
 
 #: templates/fleetfinder/dashboard.html:9
 #: templates/fleetfinder/partials/header/header-navigation.html:13
 msgid "Available Fleets"
@@ -183,16 +183,33 @@
 msgstr "Приглашение во флот"
 
 #: templates/fleetfinder/join-fleet.html:21
 msgid "Select the characters to invite"
 msgstr "Выберите пилота для приглашения"
 
 #: templates/fleetfinder/join-fleet.html:29
-msgid "Send fleet invite(s)"
-msgstr "Отправить приглашение(я)"
+msgid "Send fleet invites"
+msgstr "Отправить приглашения"
+
+#: templates/fleetfinder/partials/footer/app-translation-footer.html:4
+msgid "Join our team of translators!"
+msgstr "Присоединяйтесь к нашей команде переводчиков!"
+
+#: templates/fleetfinder/partials/footer/app-translation-footer.html:7
+#, python-format
+msgid ""
+"\n"
+"            Do you want to help translate this app into your language or "
+"improve the existing translation? - %(weblate_link)s\n"
+"        "
+msgstr ""
+"\n"
+"            Вы хотите помочь перевести это приложение на ваш язык или "
+"улучшить текущий перевод? - %(weblate_link)s\n"
+"        "
 
 #: templates/fleetfinder/partials/header/header-navigation.html:7
 msgid "Toggle navigation"
 msgstr "Переключить навигацию"
 
 #: views.py:92
 msgid "View Fleet Details"
@@ -202,8 +219,9 @@
 msgid "Edit Fleet Advert"
 msgstr "Редактировать оповещение"
 
 #: views.py:243
 #, python-brace-format
 msgid ""
 "<h4>Error!</h4><p>ESI returned the following error: {esi_error_message}</p>"
-msgstr "<h4>Ошибка!</h4><p>ESI вернул следующую ошибку: {esi_error_message}</p>"
+msgstr ""
+"<h4>Ошибка!</h4><p>ESI вернул следующую ошибку: {esi_error_message}</p>"
```

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/locale/uk/LC_MESSAGES/django.po` & `aa_fleetfinder-1.3.1/fleetfinder/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# "Andrii M." <elfleg0las88@gmail.com>, 2023.
-# Peter Pfeufer <info@ppfeufer.de>, 2023.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
+#, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-28 15:41+0200\n"
-"PO-Revision-Date: 2023-06-29 14:19+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-fleetfinder/uk/>\n"
-"Language: uk\n"
+"POT-Creation-Date: 2023-07-27 23:27+0200\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
-"n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 4.18.1\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: __init__.py:12 templates/fleetfinder/base.html:5
 msgid "Fleet Finder"
-msgstr "Пошук флоту"
+msgstr ""
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: apps.py:21
 #, python-brace-format
 msgid "Fleet Finder v{__version__}"
-msgstr "Пошук флоту v{__version__}"
+msgstr ""
 
 #: models.py:44
 msgid ""
 "FC is not in the registered fleet anymore or fleet is no longer available."
 msgstr ""
 
 #: models.py:46
@@ -43,37 +41,35 @@
 msgid "FC is no longer the fleet boss."
 msgstr ""
 
 #: models.py:48
 msgid "FC switched to another fleet."
 msgstr ""
 
-#: models.py:51 templates/fleetfinder/create-fleet.html:25
+#: models.py:51 templates/fleetfinder/create-fleet.html:27
 #: templates/fleetfinder/edit-fleet.html:27
 msgid "Fleet Name"
-msgstr "Назва флоту"
+msgstr ""
 
 #: models.py:59 templates/fleetfinder/dashboard.html:17
 msgid "Fleet Commander"
-msgstr "Командувач флотом"
+msgstr ""
 
 #: models.py:61
 msgid "Creation date and time"
 msgstr ""
 
-#: models.py:62 templates/fleetfinder/create-fleet.html:59
+#: models.py:62 templates/fleetfinder/create-fleet.html:62
 #: templates/fleetfinder/edit-fleet.html:58
 msgid "Fleet MOTD"
-msgstr "\"Шапка\" флоту"
+msgstr ""
 
 #: models.py:63
-#, fuzzy
-#| msgid "Enable Free Move"
 msgid "Free move"
-msgstr "Дозволити вільне переміщення"
+msgstr ""
 
 #: models.py:69
 msgid "Group restrictions"
 msgstr ""
 
 #: models.py:77
 msgid "Last ESI error"
@@ -84,50 +80,50 @@
 msgstr ""
 
 #: models.py:84
 msgid "ESI error count"
 msgstr ""
 
 #: templates/fleetfinder/create-fleet.html:5
-#: templates/fleetfinder/create-fleet.html:10
+#: templates/fleetfinder/create-fleet.html:11
 #: templates/fleetfinder/partials/header/header-navigation.html:18
 msgid "Create Fleet"
-msgstr "Створити флот"
+msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:34
+#: templates/fleetfinder/create-fleet.html:36
 #: templates/fleetfinder/edit-fleet.html:36
 msgid "Select Groups"
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:36
+#: templates/fleetfinder/create-fleet.html:39
 #: templates/fleetfinder/edit-fleet.html:39
 msgid ""
 "Only selected groups will have access to the fleet. If no groups are "
-"selected the fleet will be available to all of the authed groups."
+"selected the fleet will be available to all who have access to this module."
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:69
+#: templates/fleetfinder/create-fleet.html:72
 #: templates/fleetfinder/edit-fleet.html:68
 msgid "Enable Free Move"
-msgstr "Дозволити вільне переміщення"
+msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:71
+#: templates/fleetfinder/create-fleet.html:74
 #: templates/fleetfinder/edit-fleet.html:70
 msgid "Submit"
-msgstr "Відправити"
+msgstr ""
 
 #: templates/fleetfinder/dashboard.html:9
 #: templates/fleetfinder/partials/header/header-navigation.html:13
 msgid "Available Fleets"
-msgstr "Доступні флоти"
+msgstr ""
 
 #: templates/fleetfinder/dashboard.html:18
 #: templates/fleetfinder/fleet-details.html:44
 msgid "Name"
-msgstr "Назва"
+msgstr ""
 
 #: templates/fleetfinder/dashboard.html:19
 msgid "Created At"
 msgstr ""
 
 #: templates/fleetfinder/dashboard.html:20
 msgid "Join"
@@ -135,15 +131,15 @@
 
 #: templates/fleetfinder/dashboard.html:23
 msgid "Details"
 msgstr ""
 
 #: templates/fleetfinder/dashboard.html:24
 msgid "Edit"
-msgstr "Редагувати"
+msgstr ""
 
 #: templates/fleetfinder/edit-fleet.html:5
 #: templates/fleetfinder/edit-fleet.html:11
 msgid "Edit Fleet"
 msgstr ""
 
 #: templates/fleetfinder/fleet-details.html:5
@@ -168,30 +164,43 @@
 
 #: templates/fleetfinder/fleet-details.html:45
 msgid "Ship type"
 msgstr ""
 
 #: templates/fleetfinder/fleet-details.html:46
 msgid "System"
-msgstr "Система"
+msgstr ""
 
 #: templates/fleetfinder/join-fleet.html:5 views.py:79
 msgid "Join Fleet"
 msgstr ""
 
 #: templates/fleetfinder/join-fleet.html:11
 msgid "Fleet Invitation"
 msgstr ""
 
 #: templates/fleetfinder/join-fleet.html:21
 msgid "Select the characters to invite"
 msgstr ""
 
 #: templates/fleetfinder/join-fleet.html:29
-msgid "Send fleet invite(s)"
+msgid "Send fleet invites"
+msgstr ""
+
+#: templates/fleetfinder/partials/footer/app-translation-footer.html:4
+msgid "Join our team of translators!"
+msgstr ""
+
+#: templates/fleetfinder/partials/footer/app-translation-footer.html:7
+#, python-format
+msgid ""
+"\n"
+"            Do you want to help translate this app into your language or "
+"improve the existing translation? - %(weblate_link)s\n"
+"        "
 msgstr ""
 
 #: templates/fleetfinder/partials/header/header-navigation.html:7
 msgid "Toggle navigation"
 msgstr ""
 
 #: views.py:92
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/migrations/0001_initial.py` & `aa_fleetfinder-1.3.1/fleetfinder/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/migrations/0002_esi_error_handling_and_verbose_names.py` & `aa_fleetfinder-1.3.1/fleetfinder/migrations/0002_esi_error_handling_and_verbose_names.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/static/fleetfinder/css/fleetfinder.css` & `aa_fleetfinder-1.3.1/fleetfinder/static/fleetfinder/css/fleetfinder.css`

 * *Files 25% similar despite different names*

```diff
@@ -21,8 +21,19 @@
     .aa-fleetfinder .eve-type-icon {
         margin-right: 0.5rem;
     }
 
     .aa-fleetfinder .table-vertical-middle td {
         vertical-align: middle;
     }
+
+    .aa-fleetfinder-footer {
+        border-top: 1px solid rgb(236 240 241);
+        font-size: 85%;
+        margin-top: 1rem;
+        padding-top: 1rem;
+    }
+
+    .template-dark-mode .aa-fleetfinder-footer {
+        border-color: rgb(70 69 69);
+    }
 }
```

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/datetime.js` & `aa_fleetfinder-1.3.1/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/datetime.js`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/datetime.min.js` & `aa_fleetfinder-1.3.1/fleetfinder/static/fleetfinder/libs/datatables/plugins/datetime/datetime.min.js`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/static/fleetfinder/libs/multi-select/0.9.12/css/multi-select.min.css` & `aa_fleetfinder-1.3.1/fleetfinder/static/fleetfinder/libs/multi-select/0.9.12/css/multi-select.min.css`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/css/slimselect.min.css` & `aa_fleetfinder-1.3.1/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/css/slimselect.min.css`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/js/slimselect.min.js` & `aa_fleetfinder-1.3.1/fleetfinder/static/fleetfinder/libs/slim-select/1.26.0/js/slimselect.min.js`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/create-fleet.html` & `aa_fleetfinder-1.3.1/fleetfinder/templates/fleetfinder/create-fleet.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 {% extends "fleetfinder/base.html" %}
 
 {% load i18n %}
 
 {% block page_title %}{% translate "Create Fleet" %}{% endblock %}
 
-{% block fleetfinder_block %}
+{% block aa_fleetfinder_body %}
     <div class="panel panel-primary">
         <div class="panel-heading">
-            <div class="panel-title">{% translate "Create Fleet" %}</div>
+            <div class="panel-title">
+                {% translate "Create Fleet" %}
+            </div>
         </div>
 
         <div class="panel-body">
             <div class="row">
                 <div class="col-md-10 col-md-offset-1">
                     <form class="form-signin" role="form" action="{% url 'fleetfinder:save_fleet' %}" method="POST">
                         {% csrf_token %}
@@ -28,16 +30,17 @@
                             </div>
                         </div>
 
                         <div class="row">
                             <div class="col-sm-12">
                                 <div class="form-group">
                                     <label for="groups" style="margin-bottom: 0;">{% translate "Select Groups" %}</label>
+
                                     <span class="help-block text-small">
-                                        {% translate "Only selected groups will have access to the fleet. If no groups are selected the fleet will be available to all of the authed groups." %}
+                                        {% translate "Only selected groups will have access to the fleet. If no groups are selected the fleet will be available to all who have access to this module." %}
                                     </span>
 
                                     <select name="groups" id="groups" multiple>
                                         {% for group in auth_groups %}
                                             {% if groups %}
                                                 {% if group in groups %}
                                                     <option value="{{ group.group_id }}" selected>{{ group }}</option>
```

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/dashboard.html` & `aa_fleetfinder-1.3.1/fleetfinder/templates/fleetfinder/dashboard.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% extends "fleetfinder/base.html" %}
 
 {% load i18n %}
 
-{% block fleetfinder_block %}
+{% block aa_fleetfinder_body %}
     <div class="panel panel-default">
         <div class="panel-heading">
             <div class="panel-title">
                 {% translate "Available Fleets" %}
             </div>
         </div>
```

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/edit-fleet.html` & `aa_fleetfinder-1.3.1/fleetfinder/templates/fleetfinder/edit-fleet.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% extends "fleetfinder/base.html" %}
 
 {% load i18n %}
 
 {% block page_title %}{% translate "Edit Fleet" %}{% endblock %}
 
-{% block fleetfinder_block %}
+{% block aa_fleetfinder_body %}
     <div class="panel panel-primary">
         <div class="panel-heading">
             <div class="panel-title">
                 {% translate "Edit Fleet" %}
             </div>
         </div>
 
@@ -32,15 +32,15 @@
 
                         <div class="row">
                             <div class="col-sm-12">
                                 <div class="form-group">
                                     <label for="groups" style="margin-bottom: 0;">{% translate "Select Groups" %}</label>
 
                                     <span class="help-block text-small">
-                                        {% translate "Only selected groups will have access to the fleet. If no groups are selected the fleet will be available to all of the authed groups." %}
+                                        {% translate "Only selected groups will have access to the fleet. If no groups are selected the fleet will be available to all who have access to this module." %}
                                     </span>
 
                                     <select name="groups" id="groups" multiple>
                                         {% for group in auth_groups %}
                                             {% if group in fleet.groups.all %}
                                                 <option value="{{ group.group_id }}" selected>{{ group }}</option>
                                             {% else %}
```

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/fleet-details.html` & `aa_fleetfinder-1.3.1/fleetfinder/templates/fleetfinder/fleet-details.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% extends "fleetfinder/base.html" %}
 
 {% load i18n %}
 
 {% block page_title %}{% translate "Fleet Details" %}{% endblock %}
 
-{% block fleetfinder_block %}
+{% block aa_fleetfinder_body %}
     <div class="row">
         <div class="col-lg-6 col-lg-push-6">
             <div class="panel panel-primary">
                 <div class="panel-heading">
                     <div class="panel-title">
                         {% translate "Fleet Composition" %}
                     </div>
```

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/join-fleet.html` & `aa_fleetfinder-1.3.1/fleetfinder/templates/fleetfinder/join-fleet.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% extends "fleetfinder/base.html" %}
 
 {% load i18n %}
 
 {% block page_title %}{% translate "Join Fleet" %}{% endblock %}
 
-{% block fleetfinder_block %}
+{% block aa_fleetfinder_body %}
     <div class="panel panel-primary">
         <div class="panel-heading">
             <div class="panel-title">
                 {% translate "Fleet Invitation" %}
             </div>
         </div>
 
@@ -22,15 +22,15 @@
 
                         <select class="multiselect-ui" multiple="multiple" name="character_ids" id="character_ids">
                             {% for character in characters %}
                                 <option value="{{ character.character_id }}" >{{ character.character_name }}</option>
                             {% endfor %}
                         </select>
 
-                        <button class="btn btn-primary btn-block" style="margin-top: 10px;" type="submit">{% translate "Send fleet invite(s)" %}</button>
+                        <button class="btn btn-primary btn-block" style="margin-top: 10px;" type="submit">{% translate "Send fleet invites" %}</button>
                     </form>
                 </div>
             </div>
         </div>
     </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 {% extends "fleetfinder/base.html" %} {% load i18n %} {% block page_title %}{%
-translate "Join Fleet" %}{% endblock %} {% block fleetfinder_block %}
+translate "Join Fleet" %}{% endblock %} {% block aa_fleetfinder_body %}
 {% translate "Fleet Invitation" %}
 {% for character in characters %}
 {{ character.character_name }}
 {% endfor %}
- {% translate "Send fleet invite(s)" %}
+ {% translate "Send fleet invites" %}
 {% endblock %} {% block extra_css %} {% include "fleetfinder/bundles/css/multi-
 select-css.html" %} {% include "fleetfinder/bundles/css/slim-select-css.html"
 %} {% include "fleetfinder/bundles/css/fleetfinder-css.html" %} {% endblock %}
 {% block extra_javascript %} {% include "fleetfinder/bundles/js/slim-select-
 js.html" %}
  {% endblock %}
```

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/templates/fleetfinder/partials/header/header-navigation.html` & `aa_fleetfinder-1.3.1/fleetfinder/templates/fleetfinder/partials/header/header-navigation.html`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/templatetags/fleetfinder_versioned_static.py` & `aa_fleetfinder-1.3.1/fleetfinder/templatetags/fleetfinder_versioned_static.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/tests/test_access.py` & `aa_fleetfinder-1.3.1/fleetfinder/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/tests/test_auth_hooks.py` & `aa_fleetfinder-1.3.1/fleetfinder/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/tests/test_templatetags.py` & `aa_fleetfinder-1.3.1/fleetfinder/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.3.0/fleetfinder/tests/utils.py` & `aa_fleetfinder-1.3.1/fleetfinder/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.3.0/LICENSE` & `aa_fleetfinder-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-1.3.0/README.md` & `aa_fleetfinder-1.3.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 ---
 
 <!-- TOC -->
 * [AA Fleet Finder](#aa-fleet-finder)
   * [Installation](#installation)
     * [Step 1: Install the Package](#step-1-install-the-package)
     * [Step 2: Configure Alliance Auth](#step-2-configure-alliance-auth)
-    * [Step 3: Finalizing the Installation](#step-3-finalizing-the-installation)
+    * [Step 3: Add the Scheduled Task](#step-3-add-the-scheduled-task)
+    * [Step 4: Finalizing the Installation](#step-4-finalizing-the-installation)
     * [Step 4: Setup Permissions](#step-4-setup-permissions)
   * [Changelog](#changelog)
   * [Contributing](#contributing)
 <!-- TOC -->
 
 ---
 
@@ -48,15 +49,29 @@
 This is fairly simple, just add the following to the `INSTALLED_APPS` of your `local.py`
 
 Configure your AA settings (`local.py`) as follows:
 
 - Add `"fleetfinder",` to `INSTALLED_APPS`
 
 
-### Step 3: Finalizing the Installation
+### Step 3: Add the Scheduled Task
+
+To set up the scheduled task, add the following code to your `local.py`:
+
+```python
+# AA Fleetfinder - https://github.com/ppfeufer/aa-fleetfinder
+if "fleetfinder" in INSTALLED_APPS:
+    CELERYBEAT_SCHEDULE["fleetfinder_check_fleet_adverts"] = {
+        "task": "fleetfinder.tasks.check_fleet_adverts",
+        "schedule": crontab(minute="*/1"),
+    }
+```
+
+
+### Step 4: Finalizing the Installation
 
 Run static files collection and migrations
 
 ```shell
 python manage.py collectstatic
 python manage.py migrate
 ```
```

### Comparing `aa_fleetfinder-1.3.0/pyproject.toml` & `aa_fleetfinder-1.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aa-fleetfinder"
-version = "1.3.0"
+version = "1.3.1"
 description = "Fleet finder plugin for Alliance Auth"
 readme = "README.md"
 license = "GPL-3.0"
 requires-python = "~=3.8"
 authors = [
     { name = "Peter Pfeufer", email = "develop@ppfeufer.de" },
 ]
```

### Comparing `aa_fleetfinder-1.3.0/PKG-INFO` & `aa_fleetfinder-1.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-fleetfinder
-Version: 1.3.0
+Version: 1.3.1
 Summary: Fleet finder plugin for Alliance Auth
 Project-URL: Homepage, https://github.com/ppfeufer/aa-fleetfinder
 Project-URL: Documentation, https://github.com/ppfeufer/aa-fleetfinder/blob/master/README.md
 Project-URL: Source, https://github.com/ppfeufer/aa-fleetfinder.git
 Project-URL: Changelog, https://github.com/ppfeufer/aa-fleetfinder/blob/master/CHANGELOG.md
 Project-URL: Tracker, https://github.com/ppfeufer/aa-fleetfinder/issues
 Author-email: Peter Pfeufer <develop@ppfeufer.de>
@@ -51,15 +51,16 @@
 ---
 
 <!-- TOC -->
 * [AA Fleet Finder](#aa-fleet-finder)
   * [Installation](#installation)
     * [Step 1: Install the Package](#step-1-install-the-package)
     * [Step 2: Configure Alliance Auth](#step-2-configure-alliance-auth)
-    * [Step 3: Finalizing the Installation](#step-3-finalizing-the-installation)
+    * [Step 3: Add the Scheduled Task](#step-3-add-the-scheduled-task)
+    * [Step 4: Finalizing the Installation](#step-4-finalizing-the-installation)
     * [Step 4: Setup Permissions](#step-4-setup-permissions)
   * [Changelog](#changelog)
   * [Contributing](#contributing)
 <!-- TOC -->
 
 ---
 
@@ -80,15 +81,29 @@
 This is fairly simple, just add the following to the `INSTALLED_APPS` of your `local.py`
 
 Configure your AA settings (`local.py`) as follows:
 
 - Add `"fleetfinder",` to `INSTALLED_APPS`
 
 
-### Step 3: Finalizing the Installation
+### Step 3: Add the Scheduled Task
+
+To set up the scheduled task, add the following code to your `local.py`:
+
+```python
+# AA Fleetfinder - https://github.com/ppfeufer/aa-fleetfinder
+if "fleetfinder" in INSTALLED_APPS:
+    CELERYBEAT_SCHEDULE["fleetfinder_check_fleet_adverts"] = {
+        "task": "fleetfinder.tasks.check_fleet_adverts",
+        "schedule": crontab(minute="*/1"),
+    }
+```
+
+
+### Step 4: Finalizing the Installation
 
 Run static files collection and migrations
 
 ```shell
 python manage.py collectstatic
 python manage.py migrate
 ```
```

