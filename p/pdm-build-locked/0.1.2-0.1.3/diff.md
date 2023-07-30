# Comparing `tmp/pdm_build_locked-0.1.2.tar.gz` & `tmp/pdm_build_locked-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_build_locked-0.1.2.tar", last modified: Wed Jul 26 05:36:53 2023, max compression
+gzip compressed data, was "pdm_build_locked-0.1.3.tar", last modified: Sun Jul 30 13:35:17 2023, max compression
```

## Comparing `pdm_build_locked-0.1.2.tar` & `pdm_build_locked-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1064 2023-07-26 05:36:34.602619 pdm_build_locked-0.1.2/LICENSE
--rw-r--r--   0        0        0     1017 2023-07-26 05:36:34.602619 pdm_build_locked-0.1.2/README.rst
--rw-r--r--   0        0        0     2052 2023-07-26 05:36:53.770502 pdm_build_locked-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      515 2023-07-26 05:36:34.602619 pdm_build_locked-0.1.2/src/pdm_build_locked/__init__.py
--rw-r--r--   0        0        0     6916 2023-07-26 05:36:34.602619 pdm_build_locked-0.1.2/src/pdm_build_locked/command.py
--rw-r--r--   0        0        0        0 2023-07-26 05:36:34.602619 pdm_build_locked-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0     2176 2023-07-26 05:36:34.602619 pdm_build_locked-0.1.2/tests/conftest.py
--rw-r--r--   0        0        0      200 2023-07-26 05:36:34.602619 pdm_build_locked-0.1.2/tests/data/invalid/pyproject.toml
--rw-r--r--   0        0        0   117717 2023-07-26 05:36:34.606619 pdm_build_locked-0.1.2/tests/data/large/pdm.lock
--rw-r--r--   0        0        0     1896 2023-07-26 05:36:34.606619 pdm_build_locked-0.1.2/tests/data/large/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-26 05:36:34.606619 pdm_build_locked-0.1.2/tests/data/large/src/large/__init__.py
--rw-r--r--   0        0        0      221 2023-07-26 05:36:34.606619 pdm_build_locked-0.1.2/tests/data/simple-optional/pyproject.toml
--rw-r--r--   0        0        0      108 2023-07-26 05:36:34.606619 pdm_build_locked-0.1.2/tests/data/simple/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-26 05:36:34.606619 pdm_build_locked-0.1.2/tests/unit/__init__.py
--rw-r--r--   0        0        0     7138 2023-07-26 05:36:34.606619 pdm_build_locked-0.1.2/tests/unit/test_build_locked.py
--rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 pdm_build_locked-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-30 13:34:58.923403 pdm_build_locked-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1017 2023-07-30 13:34:58.923403 pdm_build_locked-0.1.3/README.rst
+-rw-r--r--   0        0        0     2052 2023-07-30 13:35:17.375301 pdm_build_locked-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      515 2023-07-30 13:34:58.923403 pdm_build_locked-0.1.3/src/pdm_build_locked/__init__.py
+-rw-r--r--   0        0        0     6963 2023-07-30 13:34:58.923403 pdm_build_locked-0.1.3/src/pdm_build_locked/command.py
+-rw-r--r--   0        0        0        0 2023-07-30 13:34:58.927404 pdm_build_locked-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     2176 2023-07-30 13:34:58.927404 pdm_build_locked-0.1.3/tests/conftest.py
+-rw-r--r--   0        0        0      200 2023-07-30 13:34:58.927404 pdm_build_locked-0.1.3/tests/data/invalid/pyproject.toml
+-rw-r--r--   0        0        0   117717 2023-07-30 13:34:58.927404 pdm_build_locked-0.1.3/tests/data/large/pdm.lock
+-rw-r--r--   0        0        0     1896 2023-07-30 13:34:58.927404 pdm_build_locked-0.1.3/tests/data/large/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-30 13:34:58.927404 pdm_build_locked-0.1.3/tests/data/large/src/large/__init__.py
+-rw-r--r--   0        0        0      221 2023-07-30 13:34:58.927404 pdm_build_locked-0.1.3/tests/data/simple-optional/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-07-30 13:34:58.927404 pdm_build_locked-0.1.3/tests/data/simple/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-30 13:34:58.927404 pdm_build_locked-0.1.3/tests/unit/__init__.py
+-rw-r--r--   0        0        0     7138 2023-07-30 13:34:58.927404 pdm_build_locked-0.1.3/tests/unit/test_build_locked.py
+-rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 pdm_build_locked-0.1.3/PKG-INFO
```

### Comparing `pdm_build_locked-0.1.2/LICENSE` & `pdm_build_locked-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_build_locked-0.1.2/README.rst` & `pdm_build_locked-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `pdm_build_locked-0.1.2/pyproject.toml` & `pdm_build_locked-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "Programming Language :: Python :: 3.11",
 ]
 authors = [
     { name = "sigma67", email = "sigma67.github@gmail.com" },
 ]
 dependencies = []
 requires-python = ">=3.8"
-version = "0.1.2"
+version = "0.1.3"
 
 [project.entry-points.pdm]
 pdm-build-locked = "pdm_build_locked:plugin"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `pdm_build_locked-0.1.2/src/pdm_build_locked/__init__.py` & `pdm_build_locked-0.1.3/src/pdm_build_locked/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_build_locked-0.1.2/src/pdm_build_locked/command.py` & `pdm_build_locked-0.1.3/src/pdm_build_locked/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,20 +150,20 @@
             Set of locked packages
         """
         requirements: Dict[str, Requirement] = project.get_dependencies(group)
 
         # taken from pdm.actions.resolve_candidates_from_lockfile and adjusted so
         # that environment markers are not evaluated
         # -- we want to publish all requirements with markers
-        provider = project.get_provider(ignore_compatibility=True)
+        provider = project.get_provider(strategy="reuse", ignore_compatibility=True)
         resolver = project.core.resolver_class(provider, BaseReporter())  # type: ignore
         reqs = list(requirements.values())
         candidates, *_ = resolve(resolver, reqs, project.environment.python_requires)
 
-        return [str(c.req) for c in candidates.values()]
+        return [str(c.req.as_pinned_version(c.version)) for c in candidates.values()]
 
     @staticmethod
     def _git_ignore_pyproject(project: Project, ignore: bool = True) -> None:
         """
         set the git index status of pyproject.toml if the project uses scm-based versioning
         Note: currently only git is supported - will crash if git repo is not present
```

### Comparing `pdm_build_locked-0.1.2/tests/conftest.py` & `pdm_build_locked-0.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm_build_locked-0.1.2/tests/data/large/pdm.lock` & `pdm_build_locked-0.1.3/tests/data/large/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm_build_locked-0.1.2/tests/data/large/pyproject.toml` & `pdm_build_locked-0.1.3/tests/data/large/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_build_locked-0.1.2/tests/unit/test_build_locked.py` & `pdm_build_locked-0.1.3/tests/unit/test_build_locked.py`

 * *Files identical despite different names*

### Comparing `pdm_build_locked-0.1.2/PKG-INFO` & `pdm_build_locked-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-build-locked
-Version: 0.1.2
+Version: 0.1.3
 Summary: \
                 pdm-build-locked is a pdm plugin to add locked packages as additional optional dependency groups
                 to the distribution metadata
             
 Keywords: pdm plugin
 Author-Email: sigma67 <sigma67.github@gmail.com>
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

