# Comparing `tmp/django_tailwind_cli-2.0.5.tar.gz` & `tmp/django_tailwind_cli-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tailwind_cli-2.0.5.tar", max compression
+gzip compressed data, was "django_tailwind_cli-2.0.6.tar", max compression
```

## Comparing `django_tailwind_cli-2.0.5.tar` & `django_tailwind_cli-2.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1071 2023-07-30 08:10:40.813220 django_tailwind_cli-2.0.5/LICENSE
--rw-r--r--   0        0        0     2776 2023-07-30 08:10:40.813220 django_tailwind_cli-2.0.5/README.md
--rw-r--r--   0        0        0     2432 2023-07-30 08:10:40.817221 django_tailwind_cli-2.0.5/pyproject.toml
--rw-r--r--   0        0        0       78 2023-07-30 08:10:40.817221 django_tailwind_cli-2.0.5/src/django_tailwind_cli/__init__.py
--rw-r--r--   0        0        0      168 2023-07-30 08:10:40.817221 django_tailwind_cli-2.0.5/src/django_tailwind_cli/apps.py
--rw-r--r--   0        0        0        0 2023-07-30 08:10:40.817221 django_tailwind_cli-2.0.5/src/django_tailwind_cli/management/__init__.py
--rw-r--r--   0        0        0        0 2023-07-30 08:10:40.817221 django_tailwind_cli-2.0.5/src/django_tailwind_cli/management/commands/__init__.py
--rw-r--r--   0        0        0     7598 2023-07-30 08:10:40.817221 django_tailwind_cli-2.0.5/src/django_tailwind_cli/management/commands/tailwind.py
--rw-r--r--   0        0        0        0 2023-07-30 08:10:40.817221 django_tailwind_cli-2.0.5/src/django_tailwind_cli/py.typed
--rw-r--r--   0        0        0       79 2023-07-30 08:10:40.817221 django_tailwind_cli-2.0.5/src/django_tailwind_cli/styles.css
--rw-r--r--   0        0        0      436 2023-07-30 08:10:40.817221 django_tailwind_cli-2.0.5/src/django_tailwind_cli/tailwind.config.js
--rw-r--r--   0        0        0      518 2023-07-30 08:10:40.817221 django_tailwind_cli-2.0.5/src/django_tailwind_cli/templates/tailwind_cli/base.html
--rw-r--r--   0        0        0      257 2023-07-30 08:10:40.817221 django_tailwind_cli-2.0.5/src/django_tailwind_cli/templates/tailwind_cli/tailwind_css.html
--rw-r--r--   0        0        0        0 2023-07-30 08:10:40.817221 django_tailwind_cli-2.0.5/src/django_tailwind_cli/templatetags/__init__.py
--rw-r--r--   0        0        0      420 2023-07-30 08:10:40.817221 django_tailwind_cli-2.0.5/src/django_tailwind_cli/templatetags/tailwind_cli.py
--rw-r--r--   0        0        0     3034 2023-07-30 08:10:40.817221 django_tailwind_cli-2.0.5/src/django_tailwind_cli/utils.py
--rw-r--r--   0        0        0     4079 1970-01-01 00:00:00.000000 django_tailwind_cli-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-30 15:29:21.606368 django_tailwind_cli-2.0.6/LICENSE
+-rw-r--r--   0        0        0     2776 2023-07-30 15:29:21.606368 django_tailwind_cli-2.0.6/README.md
+-rw-r--r--   0        0        0     2432 2023-07-30 15:29:21.606368 django_tailwind_cli-2.0.6/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-07-30 15:29:21.606368 django_tailwind_cli-2.0.6/src/django_tailwind_cli/__init__.py
+-rw-r--r--   0        0        0      168 2023-07-30 15:29:21.606368 django_tailwind_cli-2.0.6/src/django_tailwind_cli/apps.py
+-rw-r--r--   0        0        0        0 2023-07-30 15:29:21.606368 django_tailwind_cli-2.0.6/src/django_tailwind_cli/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 15:29:21.606368 django_tailwind_cli-2.0.6/src/django_tailwind_cli/management/commands/__init__.py
+-rw-r--r--   0        0        0     7645 2023-07-30 15:29:21.606368 django_tailwind_cli-2.0.6/src/django_tailwind_cli/management/commands/tailwind.py
+-rw-r--r--   0        0        0        0 2023-07-30 15:29:21.606368 django_tailwind_cli-2.0.6/src/django_tailwind_cli/py.typed
+-rw-r--r--   0        0        0       79 2023-07-30 15:29:21.606368 django_tailwind_cli-2.0.6/src/django_tailwind_cli/styles.css
+-rw-r--r--   0        0        0      436 2023-07-30 15:29:21.606368 django_tailwind_cli-2.0.6/src/django_tailwind_cli/tailwind.config.js
+-rw-r--r--   0        0        0      518 2023-07-30 15:29:21.606368 django_tailwind_cli-2.0.6/src/django_tailwind_cli/templates/tailwind_cli/base.html
+-rw-r--r--   0        0        0      257 2023-07-30 15:29:21.606368 django_tailwind_cli-2.0.6/src/django_tailwind_cli/templates/tailwind_cli/tailwind_css.html
+-rw-r--r--   0        0        0        0 2023-07-30 15:29:21.606368 django_tailwind_cli-2.0.6/src/django_tailwind_cli/templatetags/__init__.py
+-rw-r--r--   0        0        0      420 2023-07-30 15:29:21.606368 django_tailwind_cli-2.0.6/src/django_tailwind_cli/templatetags/tailwind_cli.py
+-rw-r--r--   0        0        0     3034 2023-07-30 15:29:21.606368 django_tailwind_cli-2.0.6/src/django_tailwind_cli/utils.py
+-rw-r--r--   0        0        0     4079 1970-01-01 00:00:00.000000 django_tailwind_cli-2.0.6/PKG-INFO
```

### Comparing `django_tailwind_cli-2.0.5/LICENSE` & `django_tailwind_cli-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.0.5/README.md` & `django_tailwind_cli-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.0.5/pyproject.toml` & `django_tailwind_cli-2.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-tailwind-cli"
-version = "2.0.5"
+version = "2.0.6"
 description = "Django and Tailwind integration based on the prebuilt Tailwind CSS CLI."
 license = "MIT"
 authors = ["Oliver Andrich <oliver@andrich.me>"]
 readme = "README.md"
 homepage = "https://oliverandrich.github.io/django-tailwind-cli/"
 repository = "https://github.com/oliverandrich/django-tailwind-cli"
 keywords = ["django", "tailwind", "css"]
```

### Comparing `django_tailwind_cli-2.0.5/src/django_tailwind_cli/management/commands/tailwind.py` & `django_tailwind_cli-2.0.6/src/django_tailwind_cli/management/commands/tailwind.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,14 +178,16 @@
         if not tailwind_config_file.exists():
             self.stdout.write(self.style.ERROR("Tailwind CSS config not found."))
             tailwind_config_file.write_text(DEFAULT_TAILWIND_CONFIG)
             self.stdout.write(self.style.SUCCESS(f"Created Tailwind CSS config at '{tailwind_config_file}'"))
 
 
 DEFAULT_TAILWIND_CONFIG = """/** @type {import('tailwindcss').Config} */
+const plugin = require("tailwindcss/plugin");
+
 module.exports = {
   content: [
     './templates/**/*.html',
     '**/templates/**/*.html',
   ],
   theme: {
     extend: {},
```

### Comparing `django_tailwind_cli-2.0.5/src/django_tailwind_cli/templates/tailwind_cli/base.html` & `django_tailwind_cli-2.0.6/src/django_tailwind_cli/templates/tailwind_cli/base.html`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.0.5/src/django_tailwind_cli/utils.py` & `django_tailwind_cli-2.0.6/src/django_tailwind_cli/utils.py`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.0.5/PKG-INFO` & `django_tailwind_cli-2.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tailwind-cli
-Version: 2.0.5
+Version: 2.0.6
 Summary: Django and Tailwind integration based on the prebuilt Tailwind CSS CLI.
 Home-page: https://oliverandrich.github.io/django-tailwind-cli/
 License: MIT
 Keywords: django,tailwind,css
 Author: Oliver Andrich
 Author-email: oliver@andrich.me
 Requires-Python: >=3.8,<4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-tailwind-cli Version: 2.0.5 Summary: Django
+Metadata-Version: 2.1 Name: django-tailwind-cli Version: 2.0.6 Summary: Django
 and Tailwind integration based on the prebuilt Tailwind CSS CLI. Home-page:
 https://oliverandrich.github.io/django-tailwind-cli/ License: MIT Keywords:
 django,tailwind,css Author: Oliver Andrich Author-email: oliver@andrich.me
 Requires-Python: >=3.8,<4 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Environment :: Web Environment Classifier: Framework ::
 Django :: 3.2 Classifier: Framework :: Django :: 4.1 Classifier: Framework ::
 Django :: 4.2 Classifier: Intended Audience :: Developers Classifier: License
```

