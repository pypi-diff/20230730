# Comparing `tmp/sync_pre_commit_lock-0.2.0.tar.gz` & `tmp/sync_pre_commit_lock-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sync_pre_commit_lock-0.2.0.tar", last modified: Wed Jul 26 20:02:31 2023, max compression
+gzip compressed data, was "sync_pre_commit_lock-0.2.1.tar", last modified: Sun Jul 30 19:36:12 2023, max compression
```

## Comparing `sync_pre_commit_lock-0.2.0.tar` & `sync_pre_commit_lock-0.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    35149 2023-07-26 20:02:16.730483 sync_pre_commit_lock-0.2.0/LICENSE
--rw-r--r--   0        0        0     5034 2023-07-26 20:02:16.730483 sync_pre_commit_lock-0.2.0/README.md
--rw-r--r--   0        0        0     3020 2023-07-26 20:02:31.614621 sync_pre_commit_lock-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      778 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/actions/__init__.py
--rw-r--r--   0        0        0     3232 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/actions/install_hooks.py
--rw-r--r--   0        0        0     5427 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/actions/sync_hooks.py
--rw-r--r--   0        0        0     2039 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/config.py
--rw-r--r--   0        0        0     1694 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/db.py
--rw-r--r--   0        0        0     3933 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/pdm_plugin.py
--rw-r--r--   0        0        0     4310 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/poetry_plugin.py
--rw-r--r--   0        0        0     4054 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/pre_commit_config.py
--rw-r--r--   0        0        0       93 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/py.typed
--rw-r--r--   0        0        0     1172 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/utils.py
--rw-r--r--   0        0        0       39 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0      405 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/fixtures/poetry_project/.pre-commit-config.yaml
--rw-r--r--   0        0        0     8012 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/fixtures/poetry_project/poetry.lock
--rw-r--r--   0        0        0      412 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/fixtures/poetry_project/pyproject.toml
--rw-r--r--   0        0        0      687 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/fixtures/sample_pre_commit_config/pre-commit-config-document-separator.yaml
--rw-r--r--   0        0        0      696 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/fixtures/sample_pre_commit_config/pre-commit-config-start-empty-lines.yaml
--rw-r--r--   0        0        0      493 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/fixtures/sample_pre_commit_config/pre-commit-config-with-local.yaml
--rw-r--r--   0        0        0      661 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/fixtures/sample_pre_commit_config/pre-commit-config.yaml
--rw-r--r--   0        0        0     1116 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/fixtures/sample_pre_commit_config/sample-django-stubs.yaml
--rw-r--r--   0        0        0     6401 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/test_actions/test_install_hooks.py
--rw-r--r--   0        0        0    13332 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/test_actions/test_sync_hooks.py
--rw-r--r--   0        0        0     2627 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/test_config.py
--rw-r--r--   0        0        0      273 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/test_db.py
--rw-r--r--   0        0        0     3225 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/test_pdm/test_pdm_plugin.py
--rw-r--r--   0        0        0     2093 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/test_pdm/test_pdm_sync_pre_commit_hook.py
--rw-r--r--   0        0        0     3192 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/test_poetry/test_poetry_plugin.py
--rw-r--r--   0        0        0     3071 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/test_pre_commit_config_file.py
--rw-r--r--   0        0        0     1323 2023-07-26 20:02:16.734483 sync_pre_commit_lock-0.2.0/tests/test_utils.py
--rw-r--r--   0        0        0    46881 1970-01-01 00:00:00.000000 sync_pre_commit_lock-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-30 19:35:57.765608 sync_pre_commit_lock-0.2.1/LICENSE
+-rw-r--r--   0        0        0     5034 2023-07-30 19:35:57.765608 sync_pre_commit_lock-0.2.1/README.md
+-rw-r--r--   0        0        0     3020 2023-07-30 19:36:12.813770 sync_pre_commit_lock-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      778 2023-07-30 19:35:57.765608 sync_pre_commit_lock-0.2.1/src/sync_pre_commit_lock/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 19:35:57.765608 sync_pre_commit_lock-0.2.1/src/sync_pre_commit_lock/actions/__init__.py
+-rw-r--r--   0        0        0     3232 2023-07-30 19:35:57.765608 sync_pre_commit_lock-0.2.1/src/sync_pre_commit_lock/actions/install_hooks.py
+-rw-r--r--   0        0        0     5427 2023-07-30 19:35:57.765608 sync_pre_commit_lock-0.2.1/src/sync_pre_commit_lock/actions/sync_hooks.py
+-rw-r--r--   0        0        0     2040 2023-07-30 19:35:57.765608 sync_pre_commit_lock-0.2.1/src/sync_pre_commit_lock/config.py
+-rw-r--r--   0        0        0     1694 2023-07-30 19:35:57.765608 sync_pre_commit_lock-0.2.1/src/sync_pre_commit_lock/db.py
+-rw-r--r--   0        0        0     3974 2023-07-30 19:35:57.765608 sync_pre_commit_lock-0.2.1/src/sync_pre_commit_lock/pdm_plugin.py
+-rw-r--r--   0        0        0     4310 2023-07-30 19:35:57.765608 sync_pre_commit_lock-0.2.1/src/sync_pre_commit_lock/poetry_plugin.py
+-rw-r--r--   0        0        0     4054 2023-07-30 19:35:57.765608 sync_pre_commit_lock-0.2.1/src/sync_pre_commit_lock/pre_commit_config.py
+-rw-r--r--   0        0        0       93 2023-07-30 19:35:57.765608 sync_pre_commit_lock-0.2.1/src/sync_pre_commit_lock/py.typed
+-rw-r--r--   0        0        0     1172 2023-07-30 19:35:57.765608 sync_pre_commit_lock-0.2.1/src/sync_pre_commit_lock/utils.py
+-rw-r--r--   0        0        0       39 2023-07-30 19:35:57.765608 sync_pre_commit_lock-0.2.1/tests/conftest.py
+-rw-r--r--   0        0        0      405 2023-07-30 19:35:57.765608 sync_pre_commit_lock-0.2.1/tests/fixtures/poetry_project/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     8012 2023-07-30 19:35:57.765608 sync_pre_commit_lock-0.2.1/tests/fixtures/poetry_project/poetry.lock
+-rw-r--r--   0        0        0      412 2023-07-30 19:35:57.765608 sync_pre_commit_lock-0.2.1/tests/fixtures/poetry_project/pyproject.toml
+-rw-r--r--   0        0        0      687 2023-07-30 19:35:57.765608 sync_pre_commit_lock-0.2.1/tests/fixtures/sample_pre_commit_config/pre-commit-config-document-separator.yaml
+-rw-r--r--   0        0        0      696 2023-07-30 19:35:57.765608 sync_pre_commit_lock-0.2.1/tests/fixtures/sample_pre_commit_config/pre-commit-config-start-empty-lines.yaml
+-rw-r--r--   0        0        0      493 2023-07-30 19:35:57.765608 sync_pre_commit_lock-0.2.1/tests/fixtures/sample_pre_commit_config/pre-commit-config-with-local.yaml
+-rw-r--r--   0        0        0      661 2023-07-30 19:35:57.765608 sync_pre_commit_lock-0.2.1/tests/fixtures/sample_pre_commit_config/pre-commit-config.yaml
+-rw-r--r--   0        0        0     1116 2023-07-30 19:35:57.765608 sync_pre_commit_lock-0.2.1/tests/fixtures/sample_pre_commit_config/sample-django-stubs.yaml
+-rw-r--r--   0        0        0     6401 2023-07-30 19:35:57.765608 sync_pre_commit_lock-0.2.1/tests/test_actions/test_install_hooks.py
+-rw-r--r--   0        0        0    13332 2023-07-30 19:35:57.765608 sync_pre_commit_lock-0.2.1/tests/test_actions/test_sync_hooks.py
+-rw-r--r--   0        0        0     2627 2023-07-30 19:35:57.765608 sync_pre_commit_lock-0.2.1/tests/test_config.py
+-rw-r--r--   0        0        0      273 2023-07-30 19:35:57.765608 sync_pre_commit_lock-0.2.1/tests/test_db.py
+-rw-r--r--   0        0        0     3225 2023-07-30 19:35:57.765608 sync_pre_commit_lock-0.2.1/tests/test_pdm/test_pdm_plugin.py
+-rw-r--r--   0        0        0     2093 2023-07-30 19:35:57.765608 sync_pre_commit_lock-0.2.1/tests/test_pdm/test_pdm_sync_pre_commit_hook.py
+-rw-r--r--   0        0        0     3192 2023-07-30 19:35:57.765608 sync_pre_commit_lock-0.2.1/tests/test_poetry/test_poetry_plugin.py
+-rw-r--r--   0        0        0     3071 2023-07-30 19:35:57.765608 sync_pre_commit_lock-0.2.1/tests/test_pre_commit_config_file.py
+-rw-r--r--   0        0        0     1323 2023-07-30 19:35:57.765608 sync_pre_commit_lock-0.2.1/tests/test_utils.py
+-rw-r--r--   0        0        0    46881 1970-01-01 00:00:00.000000 sync_pre_commit_lock-0.2.1/PKG-INFO
```

### Comparing `sync_pre_commit_lock-0.2.0/LICENSE` & `sync_pre_commit_lock-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.2.0/README.md` & `sync_pre_commit_lock-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.2.0/pyproject.toml` & `sync_pre_commit_lock-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "sync-pre-commit-lock"
-version = "0.2.0"
+version = "0.2.1"
 description = "PDM plugin to sync your pre-commit versions with your lockfile, and install them, all automatically."
 authors = [
     { name = "Gabriel Dugny", email = "sync-pre-commit-lock@dugny.me" },
 ]
 dependencies = [
     "tomli>=2.0.0; python_version < \"3.11\"",
     "strictyaml>=1.7.3",
@@ -128,8 +128,8 @@
     "@(abc\\.)?abstractmethod]",
     "except ImportError:",
     "# nocov",
 ]
 
 [tool.poetry]
 name = "sync-pre-commit-lock"
-version = "0.1.0"
+version = "0.2.1"
```

### Comparing `sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/__init__.py` & `sync_pre_commit_lock-0.2.1/src/sync_pre_commit_lock/__init__.py`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/actions/install_hooks.py` & `sync_pre_commit_lock-0.2.1/src/sync_pre_commit_lock/actions/install_hooks.py`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/actions/sync_hooks.py` & `sync_pre_commit_lock-0.2.1/src/sync_pre_commit_lock/actions/sync_hooks.py`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/config.py` & `sync_pre_commit_lock-0.2.1/src/sync_pre_commit_lock/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     disable_sync_from_lock: bool = field(default=False, metadata={"toml": "disable-sync-from-lock"})
     ignore: list[str] = field(default_factory=list, metadata={"toml": "ignore"})
     pre_commit_config_file: str = field(metadata={"toml": "pre-commit-config-file"}, default=".pre-commit-config.yaml")
     dependency_mapping: PackageRepoMapping = field(default_factory=dict, metadata={"toml": "dependency-mapping"})
 
 
 def load_config(path: Path | None = None) -> SyncPreCommitLockConfig:
-    # XXX We Should not hardcode this, and get the filename from PDM/Poetry/custom resolution
+    # XXX We should not hard-code this, and get the filename from PDM/Poetry/custom resolution
     path = path or Path("pyproject.toml")
     with path.open("rb") as file:
         config_dict = toml.load(file)
 
     tool_dict = config_dict.get("tool", {}).get("sync-pre-commit-lock", {})
     if not tool_dict or len(tool_dict) == 0:
         return SyncPreCommitLockConfig()
```

### Comparing `sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/db.py` & `sync_pre_commit_lock-0.2.1/src/sync_pre_commit_lock/db.py`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/pdm_plugin.py` & `sync_pre_commit_lock-0.2.1/src/sync_pre_commit_lock/pdm_plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,17 +85,17 @@
     action.execute()
 
 
 @post_lock.connect
 def on_pdm_lock_check_pre_commit(
     project: Project, *, resolution: dict[str, Candidate], dry_run: bool, **kwargs: Any
 ) -> None:
-    plugin_config: SyncPreCommitLockConfig = load_config()
-    printer = PDMPrinter(project.core.ui)
     project_root: Path = project.root
+    plugin_config: SyncPreCommitLockConfig = load_config(project_root / project.PYPROJECT_FILENAME)
+    printer = PDMPrinter(project.core.ui)
 
     file_path = project_root / plugin_config.pre_commit_config_file
     resolved_packages: dict[str, GenericLockedPackage] = {
         k: GenericLockedPackage(v.name, v.version) for k, v in resolution.items() if v.name and v.version
     }
     action = SyncPreCommitHooksVersion(
         printer=printer,
```

### Comparing `sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/poetry_plugin.py` & `sync_pre_commit_lock-0.2.1/src/sync_pre_commit_lock/poetry_plugin.py`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/pre_commit_config.py` & `sync_pre_commit_lock-0.2.1/src/sync_pre_commit_lock/pre_commit_config.py`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.2.0/src/sync_pre_commit_lock/utils.py` & `sync_pre_commit_lock-0.2.1/src/sync_pre_commit_lock/utils.py`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.2.0/tests/fixtures/poetry_project/poetry.lock` & `sync_pre_commit_lock-0.2.1/tests/fixtures/poetry_project/poetry.lock`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.2.0/tests/fixtures/sample_pre_commit_config/pre-commit-config-document-separator.yaml` & `sync_pre_commit_lock-0.2.1/tests/fixtures/sample_pre_commit_config/pre-commit-config-document-separator.yaml`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.2.0/tests/fixtures/sample_pre_commit_config/pre-commit-config-start-empty-lines.yaml` & `sync_pre_commit_lock-0.2.1/tests/fixtures/sample_pre_commit_config/pre-commit-config-start-empty-lines.yaml`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.2.0/tests/fixtures/sample_pre_commit_config/pre-commit-config.yaml` & `sync_pre_commit_lock-0.2.1/tests/fixtures/sample_pre_commit_config/pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.2.0/tests/fixtures/sample_pre_commit_config/sample-django-stubs.yaml` & `sync_pre_commit_lock-0.2.1/tests/fixtures/sample_pre_commit_config/sample-django-stubs.yaml`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.2.0/tests/test_actions/test_install_hooks.py` & `sync_pre_commit_lock-0.2.1/tests/test_actions/test_install_hooks.py`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.2.0/tests/test_actions/test_sync_hooks.py` & `sync_pre_commit_lock-0.2.1/tests/test_actions/test_sync_hooks.py`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.2.0/tests/test_config.py` & `sync_pre_commit_lock-0.2.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.2.0/tests/test_pdm/test_pdm_plugin.py` & `sync_pre_commit_lock-0.2.1/tests/test_pdm/test_pdm_plugin.py`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.2.0/tests/test_pdm/test_pdm_sync_pre_commit_hook.py` & `sync_pre_commit_lock-0.2.1/tests/test_pdm/test_pdm_sync_pre_commit_hook.py`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.2.0/tests/test_poetry/test_poetry_plugin.py` & `sync_pre_commit_lock-0.2.1/tests/test_poetry/test_poetry_plugin.py`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.2.0/tests/test_pre_commit_config_file.py` & `sync_pre_commit_lock-0.2.1/tests/test_pre_commit_config_file.py`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.2.0/tests/test_utils.py` & `sync_pre_commit_lock-0.2.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.2.0/PKG-INFO` & `sync_pre_commit_lock-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sync-pre-commit-lock
-Version: 0.2.0
+Version: 0.2.1
 Summary: PDM plugin to sync your pre-commit versions with your lockfile, and install them, all automatically.
 Author-Email: Gabriel Dugny <sync-pre-commit-lock@dugny.me>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

