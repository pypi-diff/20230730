# Comparing `tmp/rubrical-0.2.2.tar.gz` & `tmp/rubrical-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubrical-0.2.2.tar", max compression
+gzip compressed data, was "rubrical-0.3.0.tar", max compression
```

## Comparing `rubrical-0.2.2.tar` & `rubrical-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    15976 2023-06-27 15:14:04.314099 rubrical-0.2.2/LICENSE
--rw-r--r--   0        0        0     2782 2023-06-27 15:14:04.314099 rubrical-0.2.2/README.md
--rw-r--r--   0        0        0     1843 2023-06-27 15:14:24.855625 rubrical-0.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-27 15:14:04.314099 rubrical-0.2.2/rubrical/__init__.py
--rw-r--r--   0        0        0      784 2023-06-27 15:14:04.314099 rubrical-0.2.2/rubrical/comparisons/__init__.py
--rw-r--r--   0        0        0     2255 2023-06-27 15:14:04.314099 rubrical-0.2.2/rubrical/comparisons/semversion.py
--rw-r--r--   0        0        0      519 2023-06-27 15:14:04.314099 rubrical-0.2.2/rubrical/comparisons/string.py
--rw-r--r--   0        0        0      295 2023-06-27 15:14:04.314099 rubrical-0.2.2/rubrical/comparisons/utils.py
--rw-r--r--   0        0        0      568 2023-06-27 15:14:04.314099 rubrical-0.2.2/rubrical/enum.py
--rw-r--r--   0        0        0     2623 2023-06-27 15:14:04.318100 rubrical-0.2.2/rubrical/main.py
--rw-r--r--   0        0        0        0 2023-06-27 15:14:04.318100 rubrical-0.2.2/rubrical/package_managers/__init__.py
--rw-r--r--   0        0        0     2519 2023-06-27 15:14:04.318100 rubrical-0.2.2/rubrical/package_managers/base_package_manager.py
--rw-r--r--   0        0        0     1242 2023-06-27 15:14:04.318100 rubrical-0.2.2/rubrical/package_managers/go.py
--rw-r--r--   0        0        0     1504 2023-06-27 15:14:04.318100 rubrical-0.2.2/rubrical/package_managers/jsonnet.py
--rw-r--r--   0        0        0     4102 2023-06-27 15:14:04.318100 rubrical-0.2.2/rubrical/package_managers/nodejs.py
--rw-r--r--   0        0        0     1933 2023-06-27 15:14:04.318100 rubrical-0.2.2/rubrical/package_managers/python.py
--rw-r--r--   0        0        0      271 2023-06-27 15:14:04.318100 rubrical-0.2.2/rubrical/package_managers/utilities/git.py
--rw-r--r--   0        0        0     2352 2023-06-27 15:14:04.318100 rubrical-0.2.2/rubrical/reporters/gh.py
--rw-r--r--   0        0        0     1476 2023-06-27 15:14:04.318100 rubrical-0.2.2/rubrical/reporters/terminal.py
--rw-r--r--   0        0        0     4265 2023-06-27 15:14:04.318100 rubrical-0.2.2/rubrical/rubrical.py
--rw-r--r--   0        0        0      467 2023-06-27 15:14:04.318100 rubrical-0.2.2/rubrical/schemas/configuration.py
--rw-r--r--   0        0        0      251 2023-06-27 15:14:04.318100 rubrical-0.2.2/rubrical/schemas/package.py
--rw-r--r--   0        0        0      235 2023-06-27 15:14:04.318100 rubrical-0.2.2/rubrical/schemas/results.py
--rw-r--r--   0        0        0      633 2023-06-27 15:14:04.318100 rubrical-0.2.2/rubrical/utilities/console.py
--rw-r--r--   0        0        0     3753 1970-01-01 00:00:00.000000 rubrical-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    15976 2023-07-30 10:56:33.962203 rubrical-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2780 2023-07-30 10:56:33.962203 rubrical-0.3.0/README.md
+-rw-r--r--   0        0        0     1870 2023-07-30 10:56:57.420529 rubrical-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-30 10:56:33.962203 rubrical-0.3.0/rubrical/__init__.py
+-rw-r--r--   0        0        0      784 2023-07-30 10:56:33.962203 rubrical-0.3.0/rubrical/comparisons/__init__.py
+-rw-r--r--   0        0        0     2255 2023-07-30 10:56:33.962203 rubrical-0.3.0/rubrical/comparisons/semversion.py
+-rw-r--r--   0        0        0      519 2023-07-30 10:56:33.962203 rubrical-0.3.0/rubrical/comparisons/string.py
+-rw-r--r--   0        0        0      295 2023-07-30 10:56:33.962203 rubrical-0.3.0/rubrical/comparisons/utils.py
+-rw-r--r--   0        0        0      568 2023-07-30 10:56:33.962203 rubrical-0.3.0/rubrical/enum.py
+-rw-r--r--   0        0        0     2623 2023-07-30 10:56:33.962203 rubrical-0.3.0/rubrical/main.py
+-rw-r--r--   0        0        0        0 2023-07-30 10:56:33.962203 rubrical-0.3.0/rubrical/package_managers/__init__.py
+-rw-r--r--   0        0        0     2528 2023-07-30 10:56:33.962203 rubrical-0.3.0/rubrical/package_managers/base_package_manager.py
+-rw-r--r--   0        0        0     1242 2023-07-30 10:56:33.962203 rubrical-0.3.0/rubrical/package_managers/go.py
+-rw-r--r--   0        0        0     1504 2023-07-30 10:56:33.962203 rubrical-0.3.0/rubrical/package_managers/jsonnet.py
+-rw-r--r--   0        0        0     4102 2023-07-30 10:56:33.962203 rubrical-0.3.0/rubrical/package_managers/nodejs.py
+-rw-r--r--   0        0        0     2901 2023-07-30 10:56:33.962203 rubrical-0.3.0/rubrical/package_managers/python.py
+-rw-r--r--   0        0        0      271 2023-07-30 10:56:33.962203 rubrical-0.3.0/rubrical/package_managers/utilities/git.py
+-rw-r--r--   0        0        0     2387 2023-07-30 10:56:33.962203 rubrical-0.3.0/rubrical/reporters/gh.py
+-rw-r--r--   0        0        0     1508 2023-07-30 10:56:33.962203 rubrical-0.3.0/rubrical/reporters/terminal.py
+-rw-r--r--   0        0        0     4265 2023-07-30 10:56:33.962203 rubrical-0.3.0/rubrical/rubrical.py
+-rw-r--r--   0        0        0      467 2023-07-30 10:56:33.962203 rubrical-0.3.0/rubrical/schemas/configuration.py
+-rw-r--r--   0        0        0      251 2023-07-30 10:56:33.962203 rubrical-0.3.0/rubrical/schemas/package.py
+-rw-r--r--   0        0        0      235 2023-07-30 10:56:33.962203 rubrical-0.3.0/rubrical/schemas/results.py
+-rw-r--r--   0        0        0      633 2023-07-30 10:56:33.962203 rubrical-0.3.0/rubrical/utilities/console.py
+-rw-r--r--   0        0        0     3800 1970-01-01 00:00:00.000000 rubrical-0.3.0/PKG-INFO
```

### Comparing `rubrical-0.2.2/LICENSE` & `rubrical-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.2/README.md` & `rubrical-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -54,16 +54,16 @@
 
 ```yaml
 version: 1
 package_managers:
   - name: jsonnet
     packages:
       - name: "xunleii/vector_jsonnet" # Name of the dependency
-        block: v0.1.0  # If dependency is older than this, error.
-        warn: v0.1.2  # If dependency is older than this, warn.
+        block: v0.1.0  # If dependency is less than this, error.
+        warn: v0.1.2  # If dependency is less than this, warn.
   - name: python
     packages:
       - name: Mopidy-Dirble
         block: v1.2.1
         warn: v1.2.2
   - name: go
     packages:
```

### Comparing `rubrical-0.2.2/pyproject.toml` & `rubrical-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 [tool.isort]
 profile = "black"
 
 [tool.setuptools_scm]
 
 [tool.poetry]
 name = "rubrical"
-version = "0.2.2"
+version = "0.3.0"
 description = "A CLI to encourage (😅) people to update their dependencies!"
 authors = ["Ivan Lee <ivanklee86@gmail.com>"]
 license = "MPL-2.0"
 homepage = "https://github.com/ivanklee86/rubrical"
 repository = "https://github.com/ivanklee86/rubrical"
 readme = "README.md"
 classifiers=[
@@ -44,20 +44,21 @@
 
 [tool.poetry.scripts]
 rubrical = "rubrical.main:app"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 typer = {extras = ["all"], version = "^0.9.0"}
-pydantic = "^1.10.4"
+pydantic = "^2.0.3"
 semver = "^3.0.0"
 pygithub = "^1.58.0"
-python-benedict = {extras = ["all"], version = "^0.31.0"}
+python-benedict = {extras = ["all"], version = "^0.32.0"}
 pyyaml = "^6.0"
 requirements-parser = "^0.5.0"
+pyproject-parser = "^0.9.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.0.0"
 mypy = "^1.0"
 pytest = "^7.2.0"
 pylint = "^2.15.7"
 pytest-cov = "^4.0.0"
@@ -65,15 +66,15 @@
 pytest-html = "^3.2.0"
 pytest-mock = "^3.10.0"
 pytest-xdist = "^3.0.2"
 setuptools-scm = "^7.0.5"
 twine = "^4.0.2"
 pre-commit = "^3.0.0"
 isort = "^5.10.1"
-ruff = "^0.0.275"
+ruff = "^0.0.278"
 python-dotenv = "^1.0.0"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
```

### Comparing `rubrical-0.2.2/rubrical/comparisons/__init__.py` & `rubrical-0.3.0/rubrical/comparisons/__init__.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.2/rubrical/comparisons/semversion.py` & `rubrical-0.3.0/rubrical/comparisons/semversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,19 +44,19 @@
                 break
         if len(parsed_version) < 3:
             parsed_version += ["999999"] * (3 - len(parsed_version))
         package_semver = ".".join(parsed_version)
 
     if not result:
         try:
-            warn_signal = SemverComparison.GT.value != semver.compare(
+            warn_signal = SemverComparison.LT.value == semver.compare(
                 package_semver,
                 __semver_conversion(package_requirement.warn),
             )
-            block_signal = SemverComparison.GT.value != semver.compare(
+            block_signal = SemverComparison.LT.value == semver.compare(
                 package_semver,
                 __semver_conversion(package_requirement.block),
             )
         except ValueError:
             warn_signal = False
             block_signal = False
```

### Comparing `rubrical-0.2.2/rubrical/comparisons/string.py` & `rubrical-0.3.0/rubrical/comparisons/string.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.2/rubrical/enum.py` & `rubrical-0.3.0/rubrical/enum.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.2/rubrical/main.py` & `rubrical-0.3.0/rubrical/main.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.2/rubrical/package_managers/base_package_manager.py` & `rubrical-0.3.0/rubrical/package_managers/base_package_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,10 +61,10 @@
                     for symbol_char in symbol:
                         sanitized_version = sanitized_version.replace(symbol_char, "")
 
         return (specficiation, sanitized_version)
 
     @abc.abstractmethod
     def parse_package_manager_file(
-        self, package_file_filename: str, package_file: str
+        self, package_file_filename: str, package_file_contents: str
     ) -> None:
         pass
```

### Comparing `rubrical-0.2.2/rubrical/package_managers/go.py` & `rubrical-0.3.0/rubrical/package_managers/go.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.2/rubrical/package_managers/jsonnet.py` & `rubrical-0.3.0/rubrical/package_managers/jsonnet.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.2/rubrical/package_managers/nodejs.py` & `rubrical-0.3.0/rubrical/package_managers/nodejs.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.2/rubrical/package_managers/python.py` & `rubrical-0.3.0/rubrical/package_managers/python.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+import pyproject_parser
 import requirements
+import tomllib
+from requirements.requirement import Requirement
 
 from rubrical.enum import DependencySpecifications, SupportedPackageManagers
 from rubrical.package_managers.base_package_manager import BasePackageManager
 from rubrical.schemas.package import Package
 
 
 class Python(BasePackageManager):
-    target_files = ["requirements.txt"]
+    target_files = ["requirements.txt", "pyproject.toml"]
 
     def __init__(self) -> None:
         super().__init__()
 
         self.name = SupportedPackageManagers.PYTHON.value
 
         self.specification_symbols = self.specification_symbols | {
@@ -25,29 +28,47 @@
                     Package(
                         name=requirement.name,
                         version=spec[1],
                         specifier=DependencySpecifications(key),
                     ),
                 )
 
+    def _parse_requirement(self, req: Requirement, package_file_filename: str):
+        if req.specifier:
+            # Handle cases for single specifiers.
+            if len(req.specs) == 1:
+                [spec] = req.specs
+                self._set_package(package_file_filename, req, spec)
+            elif len(req.specs) > 1:
+                [spec] = [
+                    x
+                    for x in req.specs
+                    if x[0]
+                    in self.specification_symbols["GT"]
+                    + self.specification_symbols["GTE"]
+                ]
+                self._set_package(package_file_filename, req, spec)
+            else:
+                pass
+
     def parse_package_manager_file(
         self, package_file_filename: str, package_file_contents: str
     ) -> None:
         self.packages[package_file_filename] = []
 
-        for req in requirements.parse(package_file_contents):
-            if req.specifier:
-                # Handle cases for single specifiers.
-                if len(req.specs) == 1:
-                    [spec] = req.specs
-                    self._set_package(package_file_filename, req, spec)
-                elif len(req.specs) > 1:
-                    [spec] = [
-                        x
-                        for x in req.specs
-                        if x[0]
-                        in self.specification_symbols["GT"]
-                        + self.specification_symbols["GTE"]
-                    ]
-                    self._set_package(package_file_filename, req, spec)
-                else:
-                    pass
+        if "requirements.txt" in package_file_filename:
+            for req in requirements.parse(package_file_contents):
+                self._parse_requirement(
+                    req=req, package_file_filename=package_file_filename
+                )
+
+        elif "pyproject.toml" in package_file_filename:
+            pyproject_contents = tomllib.loads(package_file_contents)
+            parser = pyproject_parser.PyProject()
+            contents = parser.from_dict(pyproject_contents)
+
+            # Is not a Poetry file.
+            if contents.project and "dependencies" in contents.project.keys():
+                for pyproject_req in contents.project["dependencies"]:
+                    # Hacky hack to use same parser as requirements.txt
+                    for fake_req in requirements.parse(str(pyproject_req)):
+                        self._parse_requirement(fake_req, package_file_filename)
```

### Comparing `rubrical-0.2.2/rubrical/reporters/gh.py` & `rubrical-0.3.0/rubrical/reporters/gh.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,17 +23,17 @@
         ]
         if not_ok_results:
             test += "| File | Dependency | Result |\n"
             test += "|------|------------|--------|\n"
 
             for result in not_ok_results:
                 if result.check == PackageCheck.BLOCK:
-                    test += f"| {result.file} | {result.name} | ❌ {result.version_package} <= {result.version_block}, update to > {result.version_warn} |\n"
+                    test += f"| {result.file} | {result.name} | ❌ {result.version_package} < {result.version_block}, update to >= {result.version_warn} |\n"
                 elif result.check == PackageCheck.WARN:
-                    test += f"| {result.file} | {result.name} | ⚠️ {result.version_package} <= {result.version_warn} |\n"
+                    test += f"| {result.file} | {result.name} | ⚠️ {result.version_package} < {result.version_warn}, update to >= {result.version_warn} |\n"
         else:
             test += "🟢 All dependencies up to date!"
 
     return test
 
 
 def report_github(
```

### Comparing `rubrical-0.2.2/rubrical/reporters/terminal.py` & `rubrical-0.3.0/rubrical/reporters/terminal.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,18 +20,18 @@
         rconsole = Console()
 
         table = Table("File", "Dependency", "Result")
 
         # Only report unsuccessful checks.
         for result in [x for x in check_results if x.check != PackageCheck.OK]:
             if result.check == PackageCheck.BLOCK:
-                result_text = f"❌ {result.version_package} <= {result.version_block}, update to > {result.version_warn}"
+                result_text = f"❌ {result.version_package} < {result.version_block}, update to >= {result.version_warn}"
             elif result.check == PackageCheck.WARN:
                 # Terminal is cranky about the emoji, needs two spaces.
-                result_text = f"⚠️  {result.version_package} <= {result.version_warn}"
+                result_text = f"🚧 {result.version_package} < {result.version_warn}, update to >= {result.version_warn}"
 
             table.add_row(result.file, result.name, result_text)
 
         rconsole.print(table)
     else:
         console.print_message(
             f"[bold][spring_green1]{package_manager_name}[/spring_green1][/bold] checks completed with no warnings or blocks!"
```

### Comparing `rubrical-0.2.2/rubrical/rubrical.py` & `rubrical-0.3.0/rubrical/rubrical.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.2/rubrical/utilities/console.py` & `rubrical-0.3.0/rubrical/utilities/console.py`

 * *Files identical despite different names*

### Comparing `rubrical-0.2.2/PKG-INFO` & `rubrical-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: rubrical
-Version: 0.2.2
+Version: 0.3.0
 Summary: A CLI to encourage (😅) people to update their dependencies!
 Home-page: https://github.com/ivanklee86/rubrical
 License: MPL-2.0
 Author: Ivan Lee
 Author-email: ivanklee86@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Build Tools
-Requires-Dist: pydantic (>=1.10.4,<2.0.0)
+Requires-Dist: pydantic (>=2.0.3,<3.0.0)
 Requires-Dist: pygithub (>=1.58.0,<2.0.0)
-Requires-Dist: python-benedict[all] (>=0.31.0,<0.32.0)
+Requires-Dist: pyproject-parser (>=0.9.1,<0.10.0)
+Requires-Dist: python-benedict[all] (>=0.32.0,<0.33.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requirements-parser (>=0.5.0,<0.6.0)
 Requires-Dist: semver (>=3.0.0,<4.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/ivanklee86/rubrical
 Description-Content-Type: text/markdown
 
@@ -79,16 +80,16 @@
 
 ```yaml
 version: 1
 package_managers:
   - name: jsonnet
     packages:
       - name: "xunleii/vector_jsonnet" # Name of the dependency
-        block: v0.1.0  # If dependency is older than this, error.
-        warn: v0.1.2  # If dependency is older than this, warn.
+        block: v0.1.0  # If dependency is less than this, error.
+        warn: v0.1.2  # If dependency is less than this, warn.
   - name: python
     packages:
       - name: Mopidy-Dirble
         block: v1.2.1
         warn: v1.2.2
   - name: go
     packages:
```

