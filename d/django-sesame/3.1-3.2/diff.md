# Comparing `tmp/django-sesame-3.1.tar.gz` & `tmp/django_sesame-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sesame-3.1.tar", max compression
+gzip compressed data, was "django_sesame-3.2.tar", max compression
```

## Comparing `django-sesame-3.1.tar` & `django_sesame-3.2.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1529 2022-05-06 06:25:59.195308 django-sesame-3.1/LICENSE
--rw-r--r--   0        0        0     4569 2022-07-11 21:16:40.633841 django-sesame-3.1/README.rst
--rw-r--r--   0        0        0     1336 2022-07-28 06:25:23.197142 django-sesame-3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-02-19 07:12:12.189730 django-sesame-3.1/src/sesame/__init__.py
--rw-r--r--   0        0        0     2291 2022-07-28 06:22:47.761232 django-sesame-3.1/src/sesame/backends.py
--rw-r--r--   0        0        0     3413 2022-07-11 21:16:40.638023 django-sesame-3.1/src/sesame/decorators.py
--rw-r--r--   0        0        0     4206 2022-07-11 21:16:40.638178 django-sesame-3.1/src/sesame/middleware.py
--rw-r--r--   0        0        0     4586 2022-07-27 06:55:07.944630 django-sesame-3.1/src/sesame/packers.py
--rw-r--r--   0        0        0     3374 2022-07-28 06:19:39.648503 django-sesame-3.1/src/sesame/settings.py
--rw-r--r--   0        0        0      816 2022-07-28 06:22:47.783249 django-sesame-3.1/src/sesame/tokens.py
--rw-r--r--   0        0        0     4317 2022-07-28 06:22:47.761447 django-sesame-3.1/src/sesame/tokens_v1.py
--rw-r--r--   0        0        0     8161 2022-07-28 06:22:47.761169 django-sesame-3.1/src/sesame/tokens_v2.py
--rw-r--r--   0        0        0     3363 2022-07-11 21:16:40.638848 django-sesame-3.1/src/sesame/utils.py
--rw-r--r--   0        0        0     3676 2022-07-11 21:16:40.639017 django-sesame-3.1/src/sesame/views.py
--rw-r--r--   0        0        0     5574 2022-07-28 06:25:55.296407 django-sesame-3.1/setup.py
--rw-r--r--   0        0        0     5793 2022-07-28 06:25:55.296851 django-sesame-3.1/PKG-INFO
+-rw-r--r--   0        0        0     1529 2022-05-06 06:25:59.195308 django_sesame-3.2/LICENSE
+-rw-r--r--   0        0        0     4586 2023-05-05 06:34:05.875467 django_sesame-3.2/README.rst
+-rw-r--r--   0        0        0     1415 2023-07-30 07:31:11.796156 django_sesame-3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-02-19 07:12:12.189730 django_sesame-3.2/src/sesame/__init__.py
+-rw-r--r--   0        0        0     2291 2022-07-28 06:22:47.761232 django_sesame-3.2/src/sesame/backends.py
+-rw-r--r--   0        0        0     3413 2022-07-11 21:16:40.638023 django_sesame-3.2/src/sesame/decorators.py
+-rw-r--r--   0        0        0     4206 2022-07-11 21:16:40.638178 django_sesame-3.2/src/sesame/middleware.py
+-rw-r--r--   0        0        0     4586 2023-07-30 07:21:51.017023 django_sesame-3.2/src/sesame/packers.py
+-rw-r--r--   0        0        0     4414 2023-07-30 07:30:40.118731 django_sesame-3.2/src/sesame/settings.py
+-rw-r--r--   0        0        0      816 2022-07-28 06:22:47.783249 django_sesame-3.2/src/sesame/tokens.py
+-rw-r--r--   0        0        0     4507 2023-07-30 07:21:51.017645 django_sesame-3.2/src/sesame/tokens_v1.py
+-rw-r--r--   0        0        0     8352 2023-07-24 06:31:02.016884 django_sesame-3.2/src/sesame/tokens_v2.py
+-rw-r--r--   0        0        0     3363 2022-07-11 21:16:40.638848 django_sesame-3.2/src/sesame/utils.py
+-rw-r--r--   0        0        0     3676 2022-07-11 21:16:40.639017 django_sesame-3.2/src/sesame/views.py
+-rw-r--r--   0        0        0     5940 1970-01-01 00:00:00.000000 django_sesame-3.2/PKG-INFO
```

### Comparing `django-sesame-3.1/LICENSE` & `django_sesame-3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-sesame-3.1/README.rst` & `django_sesame-3.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 __ https://django-sesame.readthedocs.io/en/stable/
 
 Requirements
 ------------
 
 django-sesame is tested with:
 
-- Django 3.2 (LTS) and 4.0;
+- Django 3.2 (LTS), 4.0, 4.1, and 4.2 (LTS);
 - Python ≥ 3.6.
 
 It requires ``django.contrib.auth``.
 
 Getting started
 ---------------
```

### Comparing `django-sesame-3.1/pyproject.toml` & `django_sesame-3.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 source = ["sesame", "tests"]
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry]
 name = "django-sesame"
-version = "3.1"
+version = "3.2"
 description = """\
     Frictionless authentication with "Magic Links" \
     for your Django project."""
 license = "BSD-3-Clause"
 authors = ["Aymeric Augustin <aymeric.augustin@m4x.org>"]
 readme = "README.rst"
 repository = "https://github.com/aaugustin/django-sesame"
@@ -23,32 +23,35 @@
 keywords = ["authentication", "token-based-authentication"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Framework :: Django",
     "Framework :: Django :: 3.2",
     "Framework :: Django :: 4.0",
+    "Framework :: Django :: 4.1",
+    "Framework :: Django :: 4.2",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
 ]
 packages = [
     { include = "sesame", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 django = ">=3.2"
 python = ">=3.6.2"
-ua-parser = { version = ">=0.10", optional = true }
+ua-parser = { version = ">=0.15", optional = true }
 
 [tool.poetry.dev-dependencies]
 black = "*"
 coverage = "*"
 flake8 = "*"
 furo = "*"
 isort = "*"
 sphinx = "*"
 sphinx-autobuild = "*"
 sphinx-copybutton = "*"
 sphinxcontrib-spelling = { version = "*", optional = true }
+toml = "*"
 
 [tool.poetry.extras]
 ua = ["ua-parser"]
```

### Comparing `django-sesame-3.1/src/sesame/backends.py` & `django_sesame-3.2/src/sesame/backends.py`

 * *Files identical despite different names*

### Comparing `django-sesame-3.1/src/sesame/decorators.py` & `django_sesame-3.2/src/sesame/decorators.py`

 * *Files identical despite different names*

### Comparing `django-sesame-3.1/src/sesame/middleware.py` & `django_sesame-3.2/src/sesame/middleware.py`

 * *Files identical despite different names*

### Comparing `django-sesame-3.1/src/sesame/packers.py` & `django_sesame-3.2/src/sesame/packers.py`

 * *Files identical despite different names*

### Comparing `django-sesame-3.1/src/sesame/settings.py` & `django_sesame-3.2/src/sesame/settings.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 import datetime
 import hashlib
 import importlib
 import sys
 
 from django.conf import settings
-from django.core.exceptions import ImproperlyConfigured
+from django.contrib.auth import get_user_model
+from django.core.exceptions import FieldDoesNotExist, ImproperlyConfigured
+from django.core.signals import setting_changed
+from django.dispatch import receiver
 
 DEFAULTS = {
     # Generating URLs
     "TOKEN_NAME": "sesame",
     # Tokens lifecycle
     "MAX_AGE": None,
     "ONE_TIME": False,
     "INVALIDATE_ON_PASSWORD_CHANGE": True,
+    "INVALIDATE_ON_EMAIL_CHANGE": False,
     # Custom primary keys
     "PACKER": None,
     "PRIMARY_KEY_FIELD": "pk",
     # Tokens
     "TOKENS": ["sesame.tokens_v2", "sesame.tokens_v1"],
     # Tokens v2
     "KEY": "",
@@ -101,9 +105,36 @@
     global MAX_AGE, INVALIDATE_ON_PASSWORD_CHANGE
     if MAX_AGE is None and not INVALIDATE_ON_PASSWORD_CHANGE:
         raise ImproperlyConfigured(
             "insecure configuration: set SESAME_MAX_AGE to a low value "
             "or set SESAME_INVALIDATE_ON_PASSWORD_CHANGE to True"
         )
 
+    global INVALIDATE_ON_EMAIL_CHANGE
+    User = get_user_model()
+    try:
+        User._meta.get_field(User.get_email_field_name())
+    except FieldDoesNotExist:
+        raise ImproperlyConfigured(
+            "invalid configuration: set User.EMAIL_FIELD correctly "
+            "or set SESAME_INVALIDATE_ON_EMAIL_CHANGE to False"
+        )
+
 
 check()
+
+
+@receiver(setting_changed)
+def reload(*, setting, **kwargs):
+    if setting.startswith("SECRET_KEY") or setting.startswith("SESAME_"):
+        load()
+
+    if setting in ["AUTH_USER_MODEL", "SESAME_PACKER", "SESAME_PRIMARY_KEY_FIELD"]:
+        from . import packers
+
+        packers.packer = packers.get_packer()
+
+    if setting in ["SESAME_SALT", "SESAME_MAX_AGE"]:
+        from . import tokens_v1
+
+        tokens_v1.signer = tokens_v1.get_signer()
+        tokens_v1.token_re = tokens_v1.get_token_re()
```

### Comparing `django-sesame-3.1/src/sesame/tokens.py` & `django_sesame-3.2/src/sesame/tokens.py`

 * *Files identical despite different names*

### Comparing `django-sesame-3.1/src/sesame/tokens_v1.py` & `django_sesame-3.2/src/sesame/tokens_v1.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,26 +10,31 @@
 __all__ = ["create_token", "detect_token", "parse_token"]
 
 logger = logging.getLogger("sesame")
 
 
 def get_revocation_key(user):
     """
-    When the value returned by this method changes, this revocates tokens.
+    When the value returned by this method changes, this revokes tokens.
 
     It is derived from the hashed password so that changing the password
     revokes tokens.
 
+    It may be derived from the email so that changing the email revokes tokens
+    too.
+
     For one-time tokens, it also contains the last login datetime so that
     logging in revokes existing tokens.
 
     """
     data = ""
     if settings.INVALIDATE_ON_PASSWORD_CHANGE:
         data += user.password
+    if settings.INVALIDATE_ON_EMAIL_CHANGE:
+        data += getattr(user, user.get_email_field_name())
     if settings.ONE_TIME:
         data += str(user.last_login)
     # The password is expected to be a secure hash but we hash it again
     # for additional safety. We default to MD5 to minimize the length of
     # the token. (Remember, if an attacker obtains the URL, he can already
     # log in. This isn't high security.)
     return crypto.pbkdf2(
```

### Comparing `django-sesame-3.1/src/sesame/tokens_v2.py` & `django_sesame-3.2/src/sesame/tokens_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,19 +53,22 @@
     "md5": 32,  # hex, not base64
     "crypt": 11,  # salt (2) + hash (11)
 }
 
 
 def get_revocation_key(user):
     """
-    When the value returned by this method changes, this revocates tokens.
+    When the value returned by this method changes, this revokes tokens.
 
     It is derived from the hashed password so that changing the password
     revokes tokens.
 
+    It may be derived from the email so that changing the email revokes tokens
+    too.
+
     For one-time tokens, it also contains the last login datetime so that
     logging in revokes existing tokens.
 
     """
     data = ""
 
     # Tokens generated by django-sesame are more likely to leak than hashed
@@ -96,14 +99,17 @@
         try:
             hash_size = HASH_SIZES[algorithm]
         except KeyError:
             data += user.password
         else:
             data += user.password[-hash_size:]
 
+    if settings.INVALIDATE_ON_EMAIL_CHANGE:
+        data += getattr(user, user.get_email_field_name())
+
     if settings.ONE_TIME and user.last_login is not None:
         data += user.last_login.isoformat()
 
     return data.encode()
 
 
 def sign(data, key, size):
```

### Comparing `django-sesame-3.1/src/sesame/utils.py` & `django_sesame-3.2/src/sesame/utils.py`

 * *Files identical despite different names*

### Comparing `django-sesame-3.1/src/sesame/views.py` & `django_sesame-3.2/src/sesame/views.py`

 * *Files identical despite different names*

### Comparing `django-sesame-3.1/PKG-INFO` & `django_sesame-3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: django-sesame
-Version: 3.1
+Version: 3.2
 Summary: Frictionless authentication with "Magic Links" for your Django project.
 Home-page: https://github.com/aaugustin/django-sesame
 License: BSD-3-Clause
 Keywords: authentication,token-based-authentication
 Author: Aymeric Augustin
 Author-email: aymeric.augustin@m4x.org
 Requires-Python: >=3.6.2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: ua
 Requires-Dist: django (>=3.2)
-Requires-Dist: ua-parser (>=0.10); extra == "ua"
+Requires-Dist: ua-parser (>=0.15) ; extra == "ua"
 Project-URL: Documentation, https://django-sesame.readthedocs.io/
 Project-URL: Repository, https://github.com/aaugustin/django-sesame
 Description-Content-Type: text/x-rst
 
 .. image:: logo/horizontal.svg
    :width: 400px
    :alt: django-sesame
@@ -54,15 +57,15 @@
 __ https://django-sesame.readthedocs.io/en/stable/
 
 Requirements
 ------------
 
 django-sesame is tested with:
 
-- Django 3.2 (LTS) and 4.0;
+- Django 3.2 (LTS), 4.0, 4.1, and 4.2 (LTS);
 - Python ≥ 3.6.
 
 It requires ``django.contrib.auth``.
 
 Getting started
 ---------------
```

