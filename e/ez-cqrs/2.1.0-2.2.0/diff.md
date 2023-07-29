# Comparing `tmp/ez_cqrs-2.1.0.tar.gz` & `tmp/ez_cqrs-2.2.0.tar.gz`

## Comparing `ez_cqrs-2.1.0.tar` & `ez_cqrs-2.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/.tool-versions
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/mkdocs.yml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/.vscode/settings.json
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/ez_cqrs/__init__.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/ez_cqrs/acid_exec.py
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/ez_cqrs/components.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/ez_cqrs/error.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/ez_cqrs/handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/ez_cqrs/py.typed
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/ez_cqrs/framework/__init__.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/ez_cqrs/framework/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/ez_cqrs/utilities/__init__.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/ez_cqrs/utilities/cli.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/requirements/core.txt
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/requirements/dev.txt
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/scripts/new_release.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/tests/__init__.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/tests/conftest.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/tests/test_acid_exec.py
--rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/tests/test_framework.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/LICENSE
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/README.md
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 ez_cqrs-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/.tool-versions
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/mkdocs.yml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/.vscode/settings.json
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/ez_cqrs/__init__.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/ez_cqrs/acid_exec.py
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/ez_cqrs/components.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/ez_cqrs/error.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/ez_cqrs/handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/ez_cqrs/py.typed
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/ez_cqrs/framework/__init__.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/ez_cqrs/framework/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/ez_cqrs/utilities/__init__.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/ez_cqrs/utilities/cli.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/requirements/core.txt
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/requirements/dev.txt
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/scripts/new_release.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/tests/test_acid_exec.py
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/tests/test_framework.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/LICENSE
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/README.md
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 ez_cqrs-2.2.0/PKG-INFO
```

### Comparing `ez_cqrs-2.1.0/.github/workflows/release.yml` & `ez_cqrs-2.2.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.1.0/.github/workflows/test.yml` & `ez_cqrs-2.2.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.1.0/.vscode/settings.json` & `ez_cqrs-2.2.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.1.0/ez_cqrs/acid_exec.py` & `ez_cqrs-2.2.0/ez_cqrs/acid_exec.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.1.0/ez_cqrs/components.py` & `ez_cqrs-2.2.0/ez_cqrs/components.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.1.0/ez_cqrs/error.py` & `ez_cqrs-2.2.0/ez_cqrs/error.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.1.0/ez_cqrs/handler.py` & `ez_cqrs-2.2.0/ez_cqrs/handler.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.1.0/ez_cqrs/framework/__init__.py` & `ez_cqrs-2.2.0/ez_cqrs/framework/__init__.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.1.0/ez_cqrs/framework/testing.py` & `ez_cqrs-2.2.0/ez_cqrs/framework/testing.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,12 +61,12 @@
             app_database=self.app_database,
             event_registry=event_registry,
         )
         if not isinstance(use_case_result, Ok):
             error = use_case_result.err()
             if not isinstance(error, DomainError):
                 msg = f"Encounter error is {error}"
-                raise RuntimeError(msg)
+                raise TypeError(msg)
 
         return all(
             [use_case_result == expected_result, event_registry == expected_events],
         )
```

### Comparing `ez_cqrs-2.1.0/ez_cqrs/utilities/cli.py` & `ez_cqrs-2.2.0/ez_cqrs/utilities/cli.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.1.0/requirements/dev.txt` & `ez_cqrs-2.2.0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.1.0/scripts/new_release.py` & `ez_cqrs-2.2.0/scripts/new_release.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.1.0/tests/conftest.py` & `ez_cqrs-2.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.1.0/tests/test_acid_exec.py` & `ez_cqrs-2.2.0/tests/test_acid_exec.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.1.0/tests/test_framework.py` & `ez_cqrs-2.2.0/tests/test_framework.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.1.0/.gitignore` & `ez_cqrs-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.1.0/LICENSE` & `ez_cqrs-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ez_cqrs-2.1.0/pyproject.toml` & `ez_cqrs-2.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ez_cqrs"
-version = "2.1.0"
+version = "2.2.0"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 authors = [
```

### Comparing `ez_cqrs-2.1.0/PKG-INFO` & `ez_cqrs-2.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez_cqrs
-Version: 2.1.0
+Version: 2.2.0
 Project-URL: Documentation, https://github.com/Tomperez98/ez-cqrs#readme
 Project-URL: Issues, https://github.com/Tomperez98/ez-cqrs/issues
 Project-URL: Source, https://github.com/Tomperez98/ez-cqrs
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

