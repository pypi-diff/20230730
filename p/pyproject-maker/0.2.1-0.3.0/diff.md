# Comparing `tmp/pyproject_maker-0.2.1.tar.gz` & `tmp/pyproject_maker-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject_maker-0.2.1.tar", max compression
+gzip compressed data, was "pyproject_maker-0.3.0.tar", max compression
```

## Comparing `pyproject_maker-0.2.1.tar` & `pyproject_maker-0.3.0.tar`

### file list

```diff
@@ -1,32 +1,35 @@
--rw-r--r--   0        0        0     1069 2023-06-30 11:14:30.586362 pyproject_maker-0.2.1/LICENSE.txt
--rw-r--r--   0        0        0     5535 2023-07-26 16:09:17.375115 pyproject_maker-0.2.1/README.md
--rw-r--r--   0        0        0      196 2023-06-30 11:14:30.586362 pyproject_maker-0.2.1/py_maker/__init__.py
--rw-r--r--   0        0        0      332 2023-07-03 19:19:37.274781 pyproject_maker-0.2.1/py_maker/commands/new.py
--rw-r--r--   0        0        0     1170 2023-07-25 18:49:52.756669 pyproject_maker-0.2.1/py_maker/constants.py
--rw-r--r--   0        0        0      555 2023-07-26 09:30:08.132829 pyproject_maker-0.2.1/py_maker/licenses/Apache2.jinja
--rw-r--r--   0        0        0     1273 2023-07-26 09:30:08.132829 pyproject_maker-0.2.1/py_maker/licenses/BSD2.jinja
--rw-r--r--   0        0        0     1466 2023-07-26 09:30:08.132829 pyproject_maker-0.2.1/py_maker/licenses/BSD3.jinja
--rw-r--r--   0        0        0    16380 2023-07-26 09:30:08.136829 pyproject_maker-0.2.1/py_maker/licenses/CDDL.jinja
--rw-r--r--   0        0        0    14197 2023-07-26 09:30:08.136829 pyproject_maker-0.2.1/py_maker/licenses/EPL2.jinja
--rw-r--r--   0        0        0    18092 2023-07-26 09:30:08.136829 pyproject_maker-0.2.1/py_maker/licenses/GPL2.jinja
--rw-r--r--   0        0        0    35149 2023-07-26 09:30:08.136829 pyproject_maker-0.2.1/py_maker/licenses/GPL3.jinja
--rw-r--r--   0        0        0     7652 2023-07-26 09:30:08.136829 pyproject_maker-0.2.1/py_maker/licenses/LGPL.jinja
--rw-r--r--   0        0        0     1079 2023-07-26 09:30:08.136829 pyproject_maker-0.2.1/py_maker/licenses/MIT.jinja
--rw-r--r--   0        0        0    16725 2023-07-26 09:30:08.136829 pyproject_maker-0.2.1/py_maker/licenses/MPL2.jinja
--rw-r--r--   0        0        0        0 2023-07-26 09:30:08.136829 pyproject_maker-0.2.1/py_maker/licenses/__init__.py
--rw-r--r--   0        0        0      303 2023-07-04 18:51:00.941921 pyproject_maker-0.2.1/py_maker/main.py
--rw-r--r--   0        0        0     2163 2023-07-26 09:30:08.136829 pyproject_maker-0.2.1/py_maker/prompt.py
--rw-r--r--   0        0        0    11252 2023-07-26 09:30:08.136829 pyproject_maker-0.2.1/py_maker/pymaker.py
--rw-r--r--   0        0        0      502 2023-07-06 19:54:51.102633 pyproject_maker-0.2.1/py_maker/schema.py
--rw-r--r--   0        0        0     4436 2023-07-04 16:47:59.617003 pyproject_maker-0.2.1/py_maker/template/.gitignore
--rw-r--r--   0        0        0       39 2023-07-04 16:47:59.617003 pyproject_maker-0.2.1/py_maker/template/.markdownlint.json
--rw-r--r--   0        0        0     1712 2023-07-04 16:47:59.617003 pyproject_maker-0.2.1/py_maker/template/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2675 2023-07-25 18:46:19.549277 pyproject_maker-0.2.1/py_maker/template/README.md.jinja
--rw-r--r--   0        0        0        0 2023-07-04 20:20:53.136537 pyproject_maker-0.2.1/py_maker/template/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 19:19:37.278781 pyproject_maker-0.2.1/py_maker/template/app/__init__.py
--rw-r--r--   0        0        0      626 2023-07-25 18:31:48.063758 pyproject_maker-0.2.1/py_maker/template/app/main.py.jinja
--rw-r--r--   0        0        0     2348 2023-07-26 15:08:39.015504 pyproject_maker-0.2.1/py_maker/template/pyproject.toml.jinja
--rw-r--r--   0        0        0        0 2023-07-04 16:47:59.617003 pyproject_maker-0.2.1/py_maker/template/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-07-25 20:30:14.846327 pyproject_maker-0.2.1/py_maker/tests/__init__.py
--rw-r--r--   0        0        0     3336 2023-07-26 16:12:08.190765 pyproject_maker-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6950 1970-01-01 00:00:00.000000 pyproject_maker-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-30 11:14:30.586362 pyproject_maker-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     6148 2023-07-28 10:24:28.805906 pyproject_maker-0.3.0/README.md
+-rw-r--r--   0        0        0      196 2023-06-30 11:14:30.586362 pyproject_maker-0.3.0/py_maker/__init__.py
+-rw-r--r--   0        0        0      520 2023-07-30 17:47:04.258923 pyproject_maker-0.3.0/py_maker/commands/config.py
+-rw-r--r--   0        0        0      352 2023-07-30 17:47:04.258923 pyproject_maker-0.3.0/py_maker/commands/new.py
+-rw-r--r--   0        0        0     3877 2023-07-30 17:47:04.258923 pyproject_maker-0.3.0/py_maker/config/settings.py
+-rw-r--r--   0        0        0     1170 2023-07-25 18:49:52.756669 pyproject_maker-0.3.0/py_maker/constants.py
+-rw-r--r--   0        0        0     1339 2023-07-30 17:47:04.258923 pyproject_maker-0.3.0/py_maker/helpers.py
+-rw-r--r--   0        0        0      555 2023-07-26 09:30:08.132829 pyproject_maker-0.3.0/py_maker/licenses/Apache2.jinja
+-rw-r--r--   0        0        0     1273 2023-07-26 09:30:08.132829 pyproject_maker-0.3.0/py_maker/licenses/BSD2.jinja
+-rw-r--r--   0        0        0     1466 2023-07-26 09:30:08.132829 pyproject_maker-0.3.0/py_maker/licenses/BSD3.jinja
+-rw-r--r--   0        0        0    16380 2023-07-26 09:30:08.136829 pyproject_maker-0.3.0/py_maker/licenses/CDDL.jinja
+-rw-r--r--   0        0        0    14197 2023-07-26 09:30:08.136829 pyproject_maker-0.3.0/py_maker/licenses/EPL2.jinja
+-rw-r--r--   0        0        0    18092 2023-07-26 09:30:08.136829 pyproject_maker-0.3.0/py_maker/licenses/GPL2.jinja
+-rw-r--r--   0        0        0    35149 2023-07-26 09:30:08.136829 pyproject_maker-0.3.0/py_maker/licenses/GPL3.jinja
+-rw-r--r--   0        0        0     7652 2023-07-26 09:30:08.136829 pyproject_maker-0.3.0/py_maker/licenses/LGPL.jinja
+-rw-r--r--   0        0        0     1079 2023-07-26 09:30:08.136829 pyproject_maker-0.3.0/py_maker/licenses/MIT.jinja
+-rw-r--r--   0        0        0    16725 2023-07-26 09:30:08.136829 pyproject_maker-0.3.0/py_maker/licenses/MPL2.jinja
+-rw-r--r--   0        0        0        0 2023-07-26 09:30:08.136829 pyproject_maker-0.3.0/py_maker/licenses/__init__.py
+-rw-r--r--   0        0        0      437 2023-07-30 17:47:04.258923 pyproject_maker-0.3.0/py_maker/main.py
+-rw-r--r--   0        0        0      102 2023-07-30 17:47:04.258923 pyproject_maker-0.3.0/py_maker/prompt/__init__.py
+-rw-r--r--   0        0        0     2163 2023-07-30 17:47:04.258923 pyproject_maker-0.3.0/py_maker/prompt/prompt.py
+-rw-r--r--   0        0        0    10473 2023-07-30 17:47:04.258923 pyproject_maker-0.3.0/py_maker/pymaker.py
+-rw-r--r--   0        0        0      569 2023-07-28 11:21:56.359351 pyproject_maker-0.3.0/py_maker/schema.py
+-rw-r--r--   0        0        0     4436 2023-07-04 16:47:59.617003 pyproject_maker-0.3.0/py_maker/template/.gitignore
+-rw-r--r--   0        0        0       39 2023-07-04 16:47:59.617003 pyproject_maker-0.3.0/py_maker/template/.markdownlint.json
+-rw-r--r--   0        0        0     1712 2023-07-04 16:47:59.617003 pyproject_maker-0.3.0/py_maker/template/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2675 2023-07-28 10:06:10.086338 pyproject_maker-0.3.0/py_maker/template/README.md.jinja
+-rw-r--r--   0        0        0        0 2023-07-04 20:20:53.136537 pyproject_maker-0.3.0/py_maker/template/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 19:19:37.278781 pyproject_maker-0.3.0/py_maker/template/app/__init__.py
+-rw-r--r--   0        0        0      662 2023-07-28 10:06:10.086338 pyproject_maker-0.3.0/py_maker/template/app/main.py.jinja
+-rw-r--r--   0        0        0     2385 2023-07-28 10:06:10.086338 pyproject_maker-0.3.0/py_maker/template/pyproject.toml.jinja
+-rw-r--r--   0        0        0        0 2023-07-04 16:47:59.617003 pyproject_maker-0.3.0/py_maker/template/tests/__init__.py
+-rw-r--r--   0        0        0     3427 2023-07-30 17:47:04.258923 pyproject_maker-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7548 1970-01-01 00:00:00.000000 pyproject_maker-0.3.0/PKG-INFO
```

### Comparing `pyproject_maker-0.2.1/LICENSE.txt` & `pyproject_maker-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyproject_maker-0.2.1/README.md` & `pyproject_maker-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 # Python Project Generation Tool <!-- omit in toc -->
 
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/7c86940f816b455ab171dc8126476849)](https://app.codacy.com/gh/seapagan/py-maker/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![PyPI version](https://badge.fury.io/py/pyproject-maker.svg)](https://badge.fury.io/py/pyproject-maker)
+[![Codacy
+Badge](https://app.codacy.com/project/badge/Grade/7c86940f816b455ab171dc8126476849)](https://app.codacy.com/gh/seapagan/py-maker/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![CodeQL](https://github.com/seapagan/py-maker/actions/workflows/codeql.yml/badge.svg)](https://github.com/seapagan/py-maker/actions/workflows/codeql.yml)
+[![pages-build-deployment](https://github.com/seapagan/py-maker/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/seapagan/py-maker/actions/workflows/pages/pages-build-deployment)
+![PyPI - License](https://img.shields.io/pypi/l/pyproject-maker)
+![PyPI - Downloads](https://img.shields.io/pypi/dw/pyproject-maker?logo=pypi)
 
 This is a command line tool to help you create new Python projects.  It will
 create a new directory for your project, initialise a git repository, create a
 virtual environment, and install some basic dependencies.
 
 More functionality will be added very shortly and the code will be refactored
 and cleaned up.
```

### Comparing `pyproject_maker-0.2.1/py_maker/constants.py` & `pyproject_maker-0.3.0/py_maker/constants.py`

 * *Files identical despite different names*

### Comparing `pyproject_maker-0.2.1/py_maker/licenses/Apache2.jinja` & `pyproject_maker-0.3.0/py_maker/licenses/Apache2.jinja`

 * *Files identical despite different names*

### Comparing `pyproject_maker-0.2.1/py_maker/licenses/BSD2.jinja` & `pyproject_maker-0.3.0/py_maker/licenses/BSD2.jinja`

 * *Files identical despite different names*

### Comparing `pyproject_maker-0.2.1/py_maker/licenses/BSD3.jinja` & `pyproject_maker-0.3.0/py_maker/licenses/BSD3.jinja`

 * *Files identical despite different names*

### Comparing `pyproject_maker-0.2.1/py_maker/licenses/CDDL.jinja` & `pyproject_maker-0.3.0/py_maker/licenses/CDDL.jinja`

 * *Files identical despite different names*

### Comparing `pyproject_maker-0.2.1/py_maker/licenses/EPL2.jinja` & `pyproject_maker-0.3.0/py_maker/licenses/EPL2.jinja`

 * *Files identical despite different names*

### Comparing `pyproject_maker-0.2.1/py_maker/licenses/GPL2.jinja` & `pyproject_maker-0.3.0/py_maker/licenses/GPL2.jinja`

 * *Files identical despite different names*

### Comparing `pyproject_maker-0.2.1/py_maker/licenses/GPL3.jinja` & `pyproject_maker-0.3.0/py_maker/licenses/GPL3.jinja`

 * *Files identical despite different names*

### Comparing `pyproject_maker-0.2.1/py_maker/licenses/LGPL.jinja` & `pyproject_maker-0.3.0/py_maker/licenses/LGPL.jinja`

 * *Files identical despite different names*

### Comparing `pyproject_maker-0.2.1/py_maker/licenses/MIT.jinja` & `pyproject_maker-0.3.0/py_maker/licenses/MIT.jinja`

 * *Files identical despite different names*

### Comparing `pyproject_maker-0.2.1/py_maker/licenses/MPL2.jinja` & `pyproject_maker-0.3.0/py_maker/licenses/MPL2.jinja`

 * *Files identical despite different names*

### Comparing `pyproject_maker-0.2.1/py_maker/prompt.py` & `pyproject_maker-0.3.0/py_maker/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `pyproject_maker-0.2.1/py_maker/pymaker.py` & `pyproject_maker-0.3.0/py_maker/pymaker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 """Class to encapsulate the application."""
 import importlib.resources as pkg_resources
 import os
 import re
 import shutil
 import sys
-from datetime import datetime
 from pathlib import Path, PurePath
 from typing import Union
 
-import rtoml
-from git.config import GitConfigParser
 from git.exc import GitError
 from git.repo import Repo
 from jinja2 import Environment, FileSystemLoader
 from rich import print  # pylint: disable=W0622
 
 from py_maker import template
+from py_maker.config.settings import Settings
 from py_maker.constants import ExitErrors, license_names
+from py_maker.helpers import get_current_year, header
 from py_maker.prompt import Confirm, Prompt
 from py_maker.schema import ProjectValues
 
 
 class PyMaker:
     """PyMaker class."""
 
     def __init__(self, location: str) -> None:
         """Initialize the PyMaker class."""
         self.choices: ProjectValues = ProjectValues()
         self.location: str = location
 
-        self.header()
+        header()
+
+        self.settings = Settings()
 
         if len(Path(self.location).parts) > 1:
             print(
                 "[red]  -> Error: Location must be a single directory name, "
                 "and is relative to the current direcotry.\n"
             )
             sys.exit(ExitErrors.LOCATION_ERROR)
@@ -59,34 +60,14 @@
 
         return Confirm.ask("\nIs this correct?", default=True)
 
     def get_title(self, key: str) -> str:
         """Get the title for the application."""
         return re.sub("[_-]", " ", key).title() if key != "." else ""
 
-    @staticmethod
-    def header() -> None:
-        """Print a header for the application."""
-        print("[bold]PyMaker[/bold] - Generate a Python project skeleton.\n")
-
-    @staticmethod
-    def get_author_and_email_from_git() -> tuple[str, str]:
-        """Get the author name and email from git."""
-        config = GitConfigParser()
-
-        return (
-            str(config.get_value("user", "name", None)),
-            str(config.get_value("user", "email", None)),
-        )
-
-    @staticmethod
-    def get_current_year() -> str:
-        """Get the current year."""
-        return str(datetime.now().year)
-
     # ------------------------------------------------------------------------ #
     #                   create the project skeleton folders.                   #
     # ------------------------------------------------------------------------ #
     def create_folders(self) -> None:
         """Create the root folder for the project."""
         try:
             print("--> Creating project folder ... ", end="")
@@ -128,14 +109,17 @@
         ]
 
         try:
             # ---------------------- copy all the files ---------------------- #
             jinja_env = Environment(
                 loader=FileSystemLoader(str(template_dir)),
                 autoescape=True,
+                trim_blocks=True,
+                lstrip_blocks=True,
+                keep_trailing_newline=True,
             )
             for item in file_list:
                 with pkg_resources.as_file(template_dir / item) as src:
                     if src.is_dir():
                         Path(self.choices.project_dir / item).mkdir()
                     elif src.suffix == ".jinja":
                         jinja_template = jinja_env.get_template(str(item))
@@ -152,47 +136,37 @@
                         dst = self.choices.project_dir / item
                         dst.write_text(src.read_text(encoding="UTF-8"))
 
             # ---------------- generate the license file next. ------------- #
             license_env = Environment(
                 loader=FileSystemLoader(str(template_dir / "../licenses")),
                 autoescape=True,
+                keep_trailing_newline=True,
             )
             license_template = license_env.get_template(
                 f"{self.choices.license}.jinja"
             )
             dst = self.choices.project_dir / "LICENSE.txt"
             dst.write_text(
                 license_template.render(
-                    author=self.choices.author, year=self.get_current_year()
+                    author=self.choices.author, year=get_current_year()
                 )
             )
 
             # ---------- rename or delete the 'app' dir if required ---------- #
             if self.choices.package_name != "-":
                 Path(self.choices.project_dir / "app").rename(
                     self.choices.project_dir / self.choices.package_name
                 )
             else:
                 # move the main.py into the root project folder and delete app
                 Path(self.choices.project_dir / "app" / "main.py").rename(
                     Path(self.choices.project_dir / "main.py")
                 )
                 shutil.rmtree(self.choices.project_dir / "app")
-                # remove script setting from pyproject.toml
-                toml_file = rtoml.load(
-                    Path(self.choices.project_dir) / "pyproject.toml"
-                )
-                for key in ["packages", "urls", "scripts"]:
-                    del toml_file["tool"]["poetry"][key]
-                rtoml.dump(
-                    toml_file,
-                    Path(self.choices.project_dir) / "pyproject.toml",
-                    pretty=True,
-                )
         except OSError as exc:
             print(f"\n[red]  -> {exc}")
             sys.exit(ExitErrors.OS_ERROR)
 
     # ------------------------------------------------------------------------ #
     #                create the git repository for the project.                #
     # ------------------------------------------------------------------------ #
@@ -213,15 +187,15 @@
     # ------------------------------------------------------------------------ #
     def post_process(self) -> None:
         """Display steps to be carried out after the project is created.
 
         Currently just prints messages on what to do next.
         """
         output = f"""
-[green]--> Project created successfully.[/green]
+--> [green]Project created successfully.[/green]
 
 [bold]Next steps:[/bold]
 
     1) Change to the project directory:
     2) Install the dependencies (creates a virtual environment):
         'poetry install'
     3) Activate the virtual environment:
@@ -253,39 +227,44 @@
             sys.exit(ExitErrors.FOLDER_NOT_EMPTY)
 
         print(
             "[green]Creating a new project at[/green] "
             f"{self.choices.project_dir}\n"
         )
 
-        git_author, git_email = self.get_author_and_email_from_git()
-
         self.choices.name = Prompt.ask(
             "Name of the Application?",
             default=self.get_title(PurePath(self.choices.project_dir).name),
         )
         pk_name = self.sanitize(self.location)
         self.choices.package_name = Prompt.ask(
             "Package Name? (Use '-' for standalone script)",
             default=pk_name
             if pk_name != "."
             else self.sanitize(self.choices.project_dir.name),
         )
         self.choices.description = Prompt.ask(
             "Description of the Application?",
         )
-        self.choices.author = Prompt.ask("Author Name?", default=git_author)
+        self.choices.author = Prompt.ask(
+            "Author Name?", default=self.settings.author_name
+        )
 
-        self.choices.email = Prompt.ask("Author Email?", default=git_email)
+        self.choices.email = Prompt.ask(
+            "Author Email?", default=self.settings.author_email
+        )
         self.choices.license = Prompt.ask(
             "Application License?",
             choices=license_names,
-            default="MIT",
+            default=self.settings.default_license,
         )
 
+        if self.choices.package_name == "-":
+            self.choices.standalone = True
+
         if not self.confirm_values():
             # User chose not to continue
             print("\n[red]Aborting![/red]")
             sys.exit(ExitErrors.USER_ABORT)
 
         print()
```

### Comparing `pyproject_maker-0.2.1/py_maker/template/.gitignore` & `pyproject_maker-0.3.0/py_maker/template/.gitignore`

 * *Files identical despite different names*

### Comparing `pyproject_maker-0.2.1/py_maker/template/.pre-commit-config.yaml` & `pyproject_maker-0.3.0/py_maker/template/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyproject_maker-0.2.1/py_maker/template/README.md.jinja` & `pyproject_maker-0.3.0/py_maker/template/README.md.jinja`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 These are run (from within the virtual environment) using the `poe` command and
 then the script name, for example:
 
 ```console
 $ poe pre
 ```
 
-You can define your own, but there are 5 specific ones provided with the script.
+You can define your own, but there are 7 specific ones provided with the script.
 
 - `pre` : Run `pre-commit run --all-files`
 - `pylint`: Run Pylint on all Python files in the project.
 - `mypy` = Run MyPy type-checker on all Python files in the project.
 - `flake8` = Run Flake8 linter on all Python files in the project.
 - `black` = Run Black code formatter on all Python files in the project.
 - `try` = Run Tryceratops linter on all Python files in the project.
```

### Comparing `pyproject_maker-0.2.1/py_maker/template/app/main.py.jinja` & `pyproject_maker-0.3.0/py_maker/template/app/main.py.jinja`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Entry point for the main application loop.
 
 You can customize this file to your liking, or indeed empty it entirely and
 start from scratch.
+{% if not standalone %}
 Note that if you remove the 'App' class entirely, you will need to remove the
 `[tool.poetry.scripts]` section from pyproject.toml as well (if it exist).
+{% endif %}
 """
 
 
 class App:  # pylint: disable=too-few-public-methods
     """Main application class."""
 
     def __init__(self) -> None:
```

### Comparing `pyproject_maker-0.2.1/py_maker/template/pyproject.toml.jinja` & `pyproject_maker-0.3.0/py_maker/template/pyproject.toml.jinja`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [tool.poetry]
-name = "{{ name }}"
+name = "{{ slug }}"
 version = "0.1.0"
 description = "{{ description }}."
 authors = ["{{ author }} <{{ email }}>"]
 readme = "README.md"
 license = "{{ license }}"
 
+{% if not standalone %}
 packages = [{ include = "{{ package_name }}" }]
 
 [tool.poetry.urls]
 # customize the below URLs to point to your own GitHub repo. These will be
 # shown on [Pypi.org](https://pypi.org/) if you are creating a public package.
-#"Pull Requests" = "https://github.com/seapagan/py-maker/pulls"
-#"Bug Tracker" = "https://github.com/seapagan/py-maker/issues"
-
+"Pull Requests" = "https://github.com/seapagan/{{ slug }}/pulls"
+"Bug Tracker" = "https://github.com/seapagan/{{ slug }}/issues"
 [tool.poetry.scripts]
 # rename "{{ slug }}" below to change the executable name. You can also
 # add more scripts if your package offers multiple commands.
 {{ slug }} = "{{ package_name }}.main:app"
+{% endif %}
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyproject_maker-0.2.1/pyproject.toml` & `pyproject_maker-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "pyproject-maker"
-version = "0.2.1"
+version = "0.3.0"
 description = "A command line app to create a Python project skeleton."
 authors = ["Grant Ramsay <seapagan@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 
 repository = "https://github.com/seapagan/py-maker"
-homepage = "https://seapagan.github.io/seapagan/py-maker"
+homepage = "https://py-maker.seapagan.net"
 
 classifiers = [
   "Development Status :: 4 - Beta",
   "Environment :: Console",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
@@ -36,15 +36,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 typer = { extras = ["all"], version = "^0.9.0" }
 jinja2 = "^3.1.2"
 gitpython = "^3.1.32"
 tomli = "^2.0.1"
-pydantic = "^2.0"
+pydantic = "^2.1"
 rich = "^13.4.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 # Configure dev dependencies
@@ -83,14 +83,16 @@
 # documentation
 mkdocs = "^1.4.3"
 mkdocs-material = "^9.1.19"
 mkdocstrings = "^0.22.0"
 mkdocs-git-revision-date-localized-plugin = "^1.2.0"
 mkdocs-latest-git-tag-plugin = "^0.1.2"
 mkdocs-minify-plugin = "^0.7.0"
+pymdown-extensions = "^10.1"
+pygments = "^2.15.1"
 
 [tool.poe.tasks]
 # setup PoeThePoet tasks
 pre = "pre-commit run --all-files"
 pylint = "pylint **/*.py"
 mypy = "mypy **/*.py"
 flake8 = "flake8 **/*.py"
@@ -137,7 +139,11 @@
 skips = ['*_test.py', '*/test_*.py']
 
 [tool.pydocstyle]
 add-ignore = ["D104"]
 
 [tool.pytest.ini_options]
 filterwarnings = []
+
+[tool.coverage.run]
+# source = []
+omit = ["*/tests/*"]
```

### Comparing `pyproject_maker-0.2.1/PKG-INFO` & `pyproject_maker-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pyproject-maker
-Version: 0.2.1
+Version: 0.3.0
 Summary: A command line app to create a Python project skeleton.
-Home-page: https://seapagan.github.io/seapagan/py-maker
+Home-page: https://py-maker.seapagan.net
 License: MIT
 Author: Grant Ramsay
 Author-email: seapagan@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -19,26 +19,32 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Utilities
 Requires-Dist: gitpython (>=3.1.32,<4.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: pydantic (>=2.0,<3.0)
+Requires-Dist: pydantic (>=2.1,<3.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Project-URL: Bug Tracker, https://github.com/seapagan/py-maker/issues
 Project-URL: Pull Requests, https://github.com/seapagan/py-maker/pulls
 Project-URL: Repository, https://github.com/seapagan/py-maker
 Description-Content-Type: text/markdown
 
 # Python Project Generation Tool <!-- omit in toc -->
 
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/7c86940f816b455ab171dc8126476849)](https://app.codacy.com/gh/seapagan/py-maker/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![PyPI version](https://badge.fury.io/py/pyproject-maker.svg)](https://badge.fury.io/py/pyproject-maker)
+[![Codacy
+Badge](https://app.codacy.com/project/badge/Grade/7c86940f816b455ab171dc8126476849)](https://app.codacy.com/gh/seapagan/py-maker/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![CodeQL](https://github.com/seapagan/py-maker/actions/workflows/codeql.yml/badge.svg)](https://github.com/seapagan/py-maker/actions/workflows/codeql.yml)
+[![pages-build-deployment](https://github.com/seapagan/py-maker/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/seapagan/py-maker/actions/workflows/pages/pages-build-deployment)
+![PyPI - License](https://img.shields.io/pypi/l/pyproject-maker)
+![PyPI - Downloads](https://img.shields.io/pypi/dw/pyproject-maker?logo=pypi)
 
 This is a command line tool to help you create new Python projects.  It will
 create a new directory for your project, initialise a git repository, create a
 virtual environment, and install some basic dependencies.
 
 More functionality will be added very shortly and the code will be refactored
 and cleaned up.
```

