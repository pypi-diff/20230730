# Comparing `tmp/django_tailwind_cli-2.0.2.tar.gz` & `tmp/django_tailwind_cli-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tailwind_cli-2.0.2.tar", max compression
+gzip compressed data, was "django_tailwind_cli-2.0.3.tar", max compression
```

## Comparing `django_tailwind_cli-2.0.2.tar` & `django_tailwind_cli-2.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1071 2023-07-29 18:26:46.365417 django_tailwind_cli-2.0.2/LICENSE
--rw-r--r--   0        0        0     2776 2023-07-29 18:26:46.369417 django_tailwind_cli-2.0.2/README.md
--rw-r--r--   0        0        0     2559 2023-07-29 18:26:46.369417 django_tailwind_cli-2.0.2/pyproject.toml
--rw-r--r--   0        0        0       78 2023-07-29 18:26:46.369417 django_tailwind_cli-2.0.2/src/django_tailwind_cli/__init__.py
--rw-r--r--   0        0        0      168 2023-07-29 18:26:46.369417 django_tailwind_cli-2.0.2/src/django_tailwind_cli/apps.py
--rw-r--r--   0        0        0        0 2023-07-29 18:26:46.369417 django_tailwind_cli-2.0.2/src/django_tailwind_cli/management/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 18:26:46.369417 django_tailwind_cli-2.0.2/src/django_tailwind_cli/management/commands/__init__.py
--rw-r--r--   0        0        0     7592 2023-07-29 18:26:46.369417 django_tailwind_cli-2.0.2/src/django_tailwind_cli/management/commands/tailwind.py
--rw-r--r--   0        0        0        0 2023-07-29 18:26:46.369417 django_tailwind_cli-2.0.2/src/django_tailwind_cli/py.typed
--rw-r--r--   0        0        0       79 2023-07-29 18:26:46.369417 django_tailwind_cli-2.0.2/src/django_tailwind_cli/styles.css
--rw-r--r--   0        0        0      436 2023-07-29 18:26:46.369417 django_tailwind_cli-2.0.2/src/django_tailwind_cli/tailwind.config.js
--rw-r--r--   0        0        0      518 2023-07-29 18:26:46.369417 django_tailwind_cli-2.0.2/src/django_tailwind_cli/templates/tailwind_cli/base.html
--rw-r--r--   0        0        0      257 2023-07-29 18:26:46.369417 django_tailwind_cli-2.0.2/src/django_tailwind_cli/templates/tailwind_cli/tailwind_css.html
--rw-r--r--   0        0        0        0 2023-07-29 18:26:46.369417 django_tailwind_cli-2.0.2/src/django_tailwind_cli/templatetags/__init__.py
--rw-r--r--   0        0        0      420 2023-07-29 18:26:46.369417 django_tailwind_cli-2.0.2/src/django_tailwind_cli/templatetags/tailwind_cli.py
--rw-r--r--   0        0        0     3016 2023-07-29 18:26:46.369417 django_tailwind_cli-2.0.2/src/django_tailwind_cli/utils.py
--rw-r--r--   0        0        0     4015 1970-01-01 00:00:00.000000 django_tailwind_cli-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-30 07:32:30.507146 django_tailwind_cli-2.0.3/LICENSE
+-rw-r--r--   0        0        0     2776 2023-07-30 07:32:30.507146 django_tailwind_cli-2.0.3/README.md
+-rw-r--r--   0        0        0     2432 2023-07-30 07:32:30.507146 django_tailwind_cli-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-07-30 07:32:30.511147 django_tailwind_cli-2.0.3/src/django_tailwind_cli/__init__.py
+-rw-r--r--   0        0        0      168 2023-07-30 07:32:30.511147 django_tailwind_cli-2.0.3/src/django_tailwind_cli/apps.py
+-rw-r--r--   0        0        0        0 2023-07-30 07:32:30.511147 django_tailwind_cli-2.0.3/src/django_tailwind_cli/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 07:32:30.511147 django_tailwind_cli-2.0.3/src/django_tailwind_cli/management/commands/__init__.py
+-rw-r--r--   0        0        0     7598 2023-07-30 07:32:30.511147 django_tailwind_cli-2.0.3/src/django_tailwind_cli/management/commands/tailwind.py
+-rw-r--r--   0        0        0        0 2023-07-30 07:32:30.511147 django_tailwind_cli-2.0.3/src/django_tailwind_cli/py.typed
+-rw-r--r--   0        0        0       79 2023-07-30 07:32:30.511147 django_tailwind_cli-2.0.3/src/django_tailwind_cli/styles.css
+-rw-r--r--   0        0        0      436 2023-07-30 07:32:30.511147 django_tailwind_cli-2.0.3/src/django_tailwind_cli/tailwind.config.js
+-rw-r--r--   0        0        0      518 2023-07-30 07:32:30.511147 django_tailwind_cli-2.0.3/src/django_tailwind_cli/templates/tailwind_cli/base.html
+-rw-r--r--   0        0        0      257 2023-07-30 07:32:30.511147 django_tailwind_cli-2.0.3/src/django_tailwind_cli/templates/tailwind_cli/tailwind_css.html
+-rw-r--r--   0        0        0        0 2023-07-30 07:32:30.511147 django_tailwind_cli-2.0.3/src/django_tailwind_cli/templatetags/__init__.py
+-rw-r--r--   0        0        0      420 2023-07-30 07:32:30.511147 django_tailwind_cli-2.0.3/src/django_tailwind_cli/templatetags/tailwind_cli.py
+-rw-r--r--   0        0        0     3023 2023-07-30 07:32:30.511147 django_tailwind_cli-2.0.3/src/django_tailwind_cli/utils.py
+-rw-r--r--   0        0        0     4079 1970-01-01 00:00:00.000000 django_tailwind_cli-2.0.3/PKG-INFO
```

### Comparing `django_tailwind_cli-2.0.2/LICENSE` & `django_tailwind_cli-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.0.2/README.md` & `django_tailwind_cli-2.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -67,12 +67,12 @@
 
 ## Documentation
 
 The documentation can be found at [https://django-tailwind-cli.andrich.me/](https://django-tailwind-cli.andrich.me/)
 
 ## Requirements
 
-Python 3.9 or newer with Django >= 3.2.
+Python 3.8 or newer with Django >= 3.2.
 
 ## License
 
 This software is licensed under [MIT license](https://github.com/oliverandrich/django-tailwind-cli/blob/main/LICENSE).
```

#### html2text {}

```diff
@@ -27,10 +27,10 @@
 production grade CSS file for your project. - To start a debug server along
 with the Tailwind CLI in watch mode in a single session. - Necessary
 configuration to adapt the library to your project, when the defaults don't fit
 you. - A template tag to include the Tailwind CSS file in your project. - A
 base template for your project. - A sane tailwind.config.js that activates all
 the official plugins and includes a simple HTMX plugin. ## Documentation The
 documentation can be found at [https://django-tailwind-cli.andrich.me/](https:/
-/django-tailwind-cli.andrich.me/) ## Requirements Python 3.9 or newer with
+/django-tailwind-cli.andrich.me/) ## Requirements Python 3.8 or newer with
 Django >= 3.2. ## License This software is licensed under [MIT license](https:/
 /github.com/oliverandrich/django-tailwind-cli/blob/main/LICENSE).
```

### Comparing `django_tailwind_cli-2.0.2/pyproject.toml` & `django_tailwind_cli-2.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,70 +1,66 @@
 [tool.poetry]
 name = "django-tailwind-cli"
-version = "2.0.2"
+version = "2.0.3"
 description = "Django and Tailwind integration based on the prebuilt Tailwind CSS CLI."
 license = "MIT"
 authors = ["Oliver Andrich <oliver@andrich.me>"]
 readme = "README.md"
 homepage = "https://oliverandrich.github.io/django-tailwind-cli/"
 repository = "https://github.com/oliverandrich/django-tailwind-cli"
 keywords = ["django", "tailwind", "css"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries",
     "Topic :: Utilities",
     "Environment :: Web Environment",
     "Framework :: Django :: 3.2",
-    "Framework :: Django :: 4.0",
     "Framework :: Django :: 4.1",
     "Framework :: Django :: 4.2",
 ]
 packages = [{ include = "django_tailwind_cli", from = "src" }]
 
 [tool.poetry.urls]
 "Mastodon" = "https://2pxnl.de/@oliver"
 
 [tool.poetry.dependencies]
-python = ">=3.9,<4"
-django = ">=3.2,<5"
+python = ">=3.8,<4"
+django = ">=4.2,<4.3"
 certifi = "*"
 
 [tool.poetry.group.dev.dependencies]
 django-types = "^0.17.0"
 mkdocs-material = "^9.1.5"
 tox = "^4.6.4"
 tox-gh-actions = "^3.1.3"
+django-rich = "^1.7.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
-target-version = ["py39"]
+target-version = ["py38"]
 line-length = 120
 
 [tool.pyright]
 venvPath = "."
 venv = ".venv"
 typeCheckingMode = "strict"
 
-[tool.pytest.ini_options]
-pythonpath = [".", "src"]
-addopts = "--strict-config --strict-markers --ds=tests.settings"
-django_find_project = false
-filterwarnings = ["ignore::DeprecationWarning"]
-
 [tool.coverage.run]
-omit = ["*/tests/*", "conftest.py"]
+omit = ["*/tests/*"]
 
 [tool.ruff]
 select = ["A", "B", "C4", "D", "E", "F", "I", "DJ", "INP", "TID", "UP", "YTT"]
 ignore = ["D202", "D203", "D212"]
 fixable = ["A", "B", "C4", "D", "E", "F", "I", "TID", "UP"]
 unfixable = []
 exclude = [
@@ -84,15 +80,15 @@
     "dist",
     "migrations",
     "node_modules",
     "static",
 ]
 line-length = 120
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
-target-version = "py39"
+target-version = "py38"
 
 [tool.ruff.mccabe]
 max-complexity = 10
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["D104"]
 "apps.py" = ["D100", "D101"]
```

### Comparing `django_tailwind_cli-2.0.2/src/django_tailwind_cli/management/commands/tailwind.py` & `django_tailwind_cli-2.0.3/src/django_tailwind_cli/management/commands/tailwind.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import shutil
 import ssl
 import subprocess
 import sys
 import urllib.request
 from multiprocessing import Process
-from typing import Any
+from typing import Any, List
 
 import certifi
 from django.conf import settings
 from django.core.management.base import BaseCommand, CommandError
 
 from django_tailwind_cli.utils import Config
 
@@ -113,15 +113,15 @@
             debugserver_process.start()
             watch_process.join()
             debugserver_process.join()
         except KeyboardInterrupt:
             watch_process.terminate()
             debugserver_process.terminate()
 
-    def get_build_cmd(self) -> list[str]:
+    def get_build_cmd(self) -> List[str]:
         """Get the command to build the CSS."""
         if self.config.src_css is None:
             return [
                 str(self.config.get_full_cli_path()),
                 "--output",
                 str(self.config.get_full_dist_css_path()),
                 "--minify",
@@ -132,15 +132,15 @@
                 "--input",
                 str(self.config.get_full_src_css_path()),
                 "--output",
                 str(self.config.get_full_dist_css_path()),
                 "--minify",
             ]
 
-    def get_watch_cmd(self) -> list[str]:
+    def get_watch_cmd(self) -> List[str]:
         """Get the command to watch the CSS."""
         if self.config.src_css is None:
             return [
                 str(self.config.get_full_cli_path()),
                 "--output",
                 str(self.config.get_full_dist_css_path()),
                 "--watch",
```

### Comparing `django_tailwind_cli-2.0.2/src/django_tailwind_cli/templates/tailwind_cli/base.html` & `django_tailwind_cli-2.0.3/src/django_tailwind_cli/templates/tailwind_cli/base.html`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.0.2/src/django_tailwind_cli/utils.py` & `django_tailwind_cli-2.0.3/src/django_tailwind_cli/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 This module contains utility functions to read the configuration, download the CLI and determine
 the various paths.
 """
 
 import platform
 from pathlib import Path
-from typing import Union
+from typing import Tuple, Union
 
 from django.conf import settings
 
 
 class Config:
     """Configuration for the Tailwind CSS CLI."""
 
@@ -24,15 +24,15 @@
         self.config_file: str = getattr(settings, "TAILWIND_CLI_CONFIG_FILE", "tailwind.config.js")
 
     def validate_settings(self) -> None:
         """Validate the settings."""
         if settings.STATICFILES_DIRS is None or len(settings.STATICFILES_DIRS) == 0:
             raise ValueError("STATICFILES_DIRS is empty. Please add a path to your static files.")
 
-    def get_system_and_machine(self) -> tuple[str, str]:
+    def get_system_and_machine(self) -> Tuple[str, str]:
         """Get the system and machine name."""
         system = platform.system().lower()
         if system == "darwin":  # pragma: no cover
             system = "macos"
 
         machine = platform.machine().lower()
         if machine == "x86_64":  # pragma: no cover
```

### Comparing `django_tailwind_cli-2.0.2/PKG-INFO` & `django_tailwind_cli-2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: django-tailwind-cli
-Version: 2.0.2
+Version: 2.0.3
 Summary: Django and Tailwind integration based on the prebuilt Tailwind CSS CLI.
 Home-page: https://oliverandrich.github.io/django-tailwind-cli/
 License: MIT
 Keywords: django,tailwind,css
 Author: Oliver Andrich
 Author-email: oliver@andrich.me
-Requires-Python: >=3.9,<4
+Requires-Python: >=3.8,<4
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Dist: certifi
-Requires-Dist: django (>=3.2,<5)
+Requires-Dist: django (>=4.2,<4.3)
 Project-URL: Mastodon, https://2pxnl.de/@oliver
 Project-URL: Repository, https://github.com/oliverandrich/django-tailwind-cli
 Description-Content-Type: text/markdown
 
 # django-tailwind-cli
 
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/oliverandrich/django-tailwind-cli/test.yml?style=flat-square)
@@ -98,13 +99,13 @@
 
 ## Documentation
 
 The documentation can be found at [https://django-tailwind-cli.andrich.me/](https://django-tailwind-cli.andrich.me/)
 
 ## Requirements
 
-Python 3.9 or newer with Django >= 3.2.
+Python 3.8 or newer with Django >= 3.2.
 
 ## License
 
 This software is licensed under [MIT license](https://github.com/oliverandrich/django-tailwind-cli/blob/main/LICENSE).
```

#### html2text {}

```diff
@@ -1,37 +1,38 @@
-Metadata-Version: 2.1 Name: django-tailwind-cli Version: 2.0.2 Summary: Django
+Metadata-Version: 2.1 Name: django-tailwind-cli Version: 2.0.3 Summary: Django
 and Tailwind integration based on the prebuilt Tailwind CSS CLI. Home-page:
 https://oliverandrich.github.io/django-tailwind-cli/ License: MIT Keywords:
 django,tailwind,css Author: Oliver Andrich Author-email: oliver@andrich.me
-Requires-Python: >=3.9,<4 Classifier: Development Status :: 5 - Production/
+Requires-Python: >=3.8,<4 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Environment :: Web Environment Classifier: Framework ::
-Django :: 3.2 Classifier: Framework :: Django :: 4.0 Classifier: Framework ::
-Django :: 4.1 Classifier: Framework :: Django :: 4.2 Classifier: Intended
-Audience :: Developers Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Utilities Requires-Dist: certifi Requires-Dist: django
-(>=3.2,<5) Project-URL: Mastodon, https://2pxnl.de/@oliver Project-URL:
-Repository, https://github.com/oliverandrich/django-tailwind-cli Description-
-Content-Type: text/markdown # django-tailwind-cli ![GitHub Workflow Status]
-(https://img.shields.io/github/actions/workflow/status/oliverandrich/django-
-tailwind-cli/test.yml?style=flat-square) [![PyPI](https://img.shields.io/pypi/
-v/django-tailwind-cli.svg?style=flat-square)](https://pypi.org/project/django-
-tailwind-cli/) [![Code style: black](https://img.shields.io/badge/code%20style-
-black-000000.svg?style=flat-square)](https://github.com/psf/black) ![GitHub]
-(https://img.shields.io/github/license/oliverandrich/django-tailwind-
-cli?style=flat-square) [![poetry-managed](https://img.shields.io/badge/poetry-
-managed-blue?style=flat-square)](https://python-poetry.org) This library
-provides an integration of [Tailwind CSS](https://tailwindcss.com) for Django
-that is using on the precompiled versions of the [Tailwind CSS CLI](https://
-tailwindcss.com/blog/standalone-cli). The goal of this library is to provided
-the simplest possible Tailwind integration for your Django project. It took its
-inspiration from the [Tailwind integration for Phoenix](https://github.com/
+Django :: 3.2 Classifier: Framework :: Django :: 4.1 Classifier: Framework ::
+Django :: 4.2 Classifier: Intended Audience :: Developers Classifier: License
+:: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
+Utilities Requires-Dist: certifi Requires-Dist: django (>=4.2,<4.3) Project-
+URL: Mastodon, https://2pxnl.de/@oliver Project-URL: Repository, https://
+github.com/oliverandrich/django-tailwind-cli Description-Content-Type: text/
+markdown # django-tailwind-cli ![GitHub Workflow Status](https://
+img.shields.io/github/actions/workflow/status/oliverandrich/django-tailwind-
+cli/test.yml?style=flat-square) [![PyPI](https://img.shields.io/pypi/v/django-
+tailwind-cli.svg?style=flat-square)](https://pypi.org/project/django-tailwind-
+cli/) [![Code style: black](https://img.shields.io/badge/code%20style-black-
+000000.svg?style=flat-square)](https://github.com/psf/black) ![GitHub](https://
+img.shields.io/github/license/oliverandrich/django-tailwind-cli?style=flat-
+square) [![poetry-managed](https://img.shields.io/badge/poetry-managed-
+blue?style=flat-square)](https://python-poetry.org) This library provides an
+integration of [Tailwind CSS](https://tailwindcss.com) for Django that is using
+on the precompiled versions of the [Tailwind CSS CLI](https://tailwindcss.com/
+blog/standalone-cli). The goal of this library is to provided the simplest
+possible Tailwind integration for your Django project. It took its inspiration
+from the [Tailwind integration for Phoenix](https://github.com/
 phoenixframework/tailwind) which completely skips the neccesity of a node
 installation. ## Installation 1. Install the library. ```shell python -m pip
 install django-tailwind-cli ``` 2. Add `django_tailwind_cli` to
 `INSTALLED_APPS` in `settings.py`. ```python INSTALLED_APPS = [ # other Django
 apps "django_tailwind_cli", ] ``` 3. Configure the `STATICFILES_DIRS` parameter
 in your `settings.py` if not already configured. ```python STATICFILES_DIRS =
 [BASE_DIR / "assets"] ``` 4. Add template code. ```htmldjango {% load
@@ -43,10 +44,10 @@
 production grade CSS file for your project. - To start a debug server along
 with the Tailwind CLI in watch mode in a single session. - Necessary
 configuration to adapt the library to your project, when the defaults don't fit
 you. - A template tag to include the Tailwind CSS file in your project. - A
 base template for your project. - A sane tailwind.config.js that activates all
 the official plugins and includes a simple HTMX plugin. ## Documentation The
 documentation can be found at [https://django-tailwind-cli.andrich.me/](https:/
-/django-tailwind-cli.andrich.me/) ## Requirements Python 3.9 or newer with
+/django-tailwind-cli.andrich.me/) ## Requirements Python 3.8 or newer with
 Django >= 3.2. ## License This software is licensed under [MIT license](https:/
 /github.com/oliverandrich/django-tailwind-cli/blob/main/LICENSE).
```

