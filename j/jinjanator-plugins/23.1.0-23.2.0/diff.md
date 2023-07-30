# Comparing `tmp/jinjanator_plugins-23.1.0.tar.gz` & `tmp/jinjanator_plugins-23.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Jul 24 17:45:52 2023, max compression
+gzip compressed data, last modified: Sun Jul 30 10:29:42 2023, max compression
```

## Comparing `jinjanator_plugins-23.1.0.tar` & `jinjanator_plugins-23.2.0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0     1010 2023-07-24 17:45:52.000000 jinjanator_plugins-23.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     9134 2023-07-24 17:45:52.000000 jinjanator_plugins-23.1.0/README.md
--rw-r--r--   0        0        0     1121 2023-07-24 17:45:52.000000 jinjanator_plugins-23.1.0/plugin_example/jinjanator_plugin_example.py
--rw-r--r--   0        0        0      599 2023-07-24 17:45:52.000000 jinjanator_plugins-23.1.0/plugin_example/pyproject.toml
--rw-r--r--   0        0        0     1571 2023-07-24 17:45:52.000000 jinjanator_plugins-23.1.0/plugin_example/tests/test_plugin.py
--rw-r--r--   0        0        0     2456 2023-07-24 17:45:52.000000 jinjanator_plugins-23.1.0/src/jinjanator_plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-07-24 17:45:52.000000 jinjanator_plugins-23.1.0/src/jinjanator_plugins/py.typed
--rw-r--r--   0        0        0       32 2023-07-24 17:45:52.000000 jinjanator_plugins-23.1.0/.gitignore
--rw-r--r--   0        0        0    35149 2023-07-24 17:45:52.000000 jinjanator_plugins-23.1.0/LICENSE
--rw-r--r--   0        0        0     6344 2023-07-24 17:45:52.000000 jinjanator_plugins-23.1.0/pyproject.toml
--rw-r--r--   0        0        0     8018 2023-07-24 17:45:52.000000 jinjanator_plugins-23.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1483 2023-07-30 10:29:42.000000 jinjanator_plugins-23.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     9133 2023-07-30 10:29:42.000000 jinjanator_plugins-23.2.0/README.md
+-rw-r--r--   0        0        0     1872 2023-07-30 10:29:42.000000 jinjanator_plugins-23.2.0/plugin_example/jinjanator_plugin_example.py
+-rw-r--r--   0        0        0      599 2023-07-30 10:29:42.000000 jinjanator_plugins-23.2.0/plugin_example/pyproject.toml
+-rw-r--r--   0        0        0     1144 2023-07-30 10:29:42.000000 jinjanator_plugins-23.2.0/plugin_example/tests/test_plugin.py
+-rw-r--r--   0        0        0     1296 2023-07-30 10:29:42.000000 jinjanator_plugins-23.2.0/plugin_example/tests/test_plugin_discovery.py
+-rw-r--r--   0        0        0     1321 2023-07-30 10:29:42.000000 jinjanator_plugins-23.2.0/plugin_example/tests/test_plugin_discovery_entrypoint.py
+-rw-r--r--   0        0        0     3066 2023-07-30 10:29:42.000000 jinjanator_plugins-23.2.0/src/jinjanator_plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 10:29:42.000000 jinjanator_plugins-23.2.0/src/jinjanator_plugins/py.typed
+-rw-r--r--   0        0        0       32 2023-07-30 10:29:42.000000 jinjanator_plugins-23.2.0/.gitignore
+-rw-r--r--   0        0        0    11357 2023-07-30 10:29:42.000000 jinjanator_plugins-23.2.0/LICENSE
+-rw-r--r--   0        0        0     6352 2023-07-30 10:29:42.000000 jinjanator_plugins-23.2.0/pyproject.toml
+-rw-r--r--   0        0        0     8595 2023-07-30 10:29:42.000000 jinjanator_plugins-23.2.0/PKG-INFO
```

### Comparing `jinjanator_plugins-23.1.0/README.md` & `jinjanator_plugins-23.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 This repo contains `jinjanator-plugins`, a set of types and decorators
 which can be used to implement plugins for the
 [Jinjanator](https://github.com/kpfleming/jinjanator) tool.
 
 Open Source software: [Apache License 2.0](https://spdx.org/licenses/Apache-2.0.html)
 
 ## &nbsp;
-
 <!-- fancy-readme start -->
 
 Jinjanator can be extended through the use of plugins; these are
 Python packages installed into the same environment as the tool
 itself, which use special markers to 'hook' into various
 features. There is a minimal example in the
 [plugin_example](plugin_example) directory which demonstrates three of
```

### Comparing `jinjanator_plugins-23.1.0/plugin_example/pyproject.toml` & `jinjanator_plugins-23.2.0/plugin_example/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jinjanator_plugins-23.1.0/src/jinjanator_plugins/__init__.py` & `jinjanator_plugins-23.2.0/src/jinjanator_plugins/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,27 +22,45 @@
 
 @define(kw_only=True)
 class Format:
     parser: Callable[[str, list[str] | None], Mapping[str, Any]]
     suffixes: list[str]
 
 
+class FormatOptionUnknownError(Exception):
+    pass
+
+
+class FormatOptionUnsupportedError(Exception):
+    pass
+
+
+class FormatOptionValueError(Exception):
+    pass
+
+
 F = TypeVar("F", bound=Callable[..., Any])
 hookspec = cast(Callable[[F], F], pluggy.HookspecMarker("jinjanator"))
 
+Identity: TypeAlias = str
 Formats: TypeAlias = Mapping[str, Format]
 Filters: TypeAlias = Mapping[str, Callable[..., Any]]
 Globals: TypeAlias = Mapping[str, Callable[..., Any]]
 Tests: TypeAlias = Mapping[str, Callable[..., Any]]
 
+PluginIdentityHook: TypeAlias = Callable[[], Identity]
 PluginFormatsHook: TypeAlias = Callable[[], Formats]
 PluginFiltersHook: TypeAlias = Callable[[], Filters]
 PluginTestsHook: TypeAlias = Callable[[], Tests]
 PluginGlobalsHook: TypeAlias = Callable[[], Globals]
 
+plugin_identity_hook = cast(
+    Callable[[PluginIdentityHook], PluginIdentityHook],
+    pluggy.HookimplMarker("jinjanator"),
+)
 plugin_formats_hook = cast(
     Callable[[PluginFormatsHook], PluginFormatsHook],
     pluggy.HookimplMarker("jinjanator"),
 )
 plugin_filters_hook = cast(
     Callable[[PluginFiltersHook], PluginFiltersHook],
     pluggy.HookimplMarker("jinjanator"),
@@ -56,14 +74,19 @@
     pluggy.HookimplMarker("jinjanator"),
 )
 
 
 class PluginHooks(Protocol):
     @staticmethod
     @hookspec
+    def plugin_identities() -> Identity:
+        """Returns identity as string"""
+
+    @staticmethod
+    @hookspec
     def plugin_formats() -> Formats:
         """Returns dict of formats"""
 
     @staticmethod
     @hookspec
     def plugin_filters() -> Filters:
         """Returns dict of filter functions"""
@@ -77,14 +100,18 @@
     @hookspec
     def plugin_tests() -> Tests:
         """Returns dict of test functions"""
 
 
 class PluginHookCallers(Protocol):
     @staticmethod
+    def plugin_identities() -> Sequence[Identity]:
+        """Returns list of strings of identities"""
+
+    @staticmethod
     def plugin_formats() -> Sequence[Formats]:
         """Returns list of dicts of formats"""
 
     @staticmethod
     def plugin_filters() -> Sequence[Filters]:
         """Returns list of dicts of filter functions"""
```

### Comparing `jinjanator_plugins-23.1.0/pyproject.toml` & `jinjanator_plugins-23.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -37,24 +37,25 @@
   "pluggy",
 ]
 [project.urls]
 "Bug Tracker" = "https://github.com/kpfleming/jinjanator-plugins/issues"
 "Homepage" = "https://github.com/kpfleming/jinjanator-plugins"
 
 [tool.hatch.envs.changelog]
+skip-install = true
 dependencies = [
   "towncrier",
 ]
 
 [tool.hatch.envs.changelog.scripts]
 draft = [
   "towncrier build --version main --draft",
 ]
 release = [
-  "towncrier build --version {args}",
+  "towncrier build --yes --version {args}",
 ]
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.build]
 exclude = [
@@ -100,15 +101,14 @@
      "mypy plugin_example/*.py",
      "shellcheck workflow-support/*.sh",
 ]
 
 [tool.hatch.envs.ci]
 dependencies = [
     "coverage[toml]",
-    "jinjanator",
     "pytest",
     "pytest-cov",
     "pytest-icdiff",
 ]
 
 [[tool.hatch.envs.ci.matrix]]
 python = [
```

### Comparing `jinjanator_plugins-23.1.0/PKG-INFO` & `jinjanator_plugins-23.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinjanator-plugins
-Version: 23.1.0
+Version: 23.2.0
 Summary: Package which provides the plugin API for the Jinjanator tool
 Project-URL: Bug Tracker, https://github.com/kpfleming/jinjanator-plugins/issues
 Project-URL: Homepage, https://github.com/kpfleming/jinjanator-plugins
 Author-email: "Kevin P. Fleming" <jinjanator@kevin.km6g.us>
 License: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
@@ -248,13 +248,27 @@
 during format auto-detection.
 
 Note that the function *must* be named `plugin_formats`; it is the
 second part of the 'magic' mechanism mentioned above.
 ## Release Information
 
 
-## [23.1.0](https://github.com/kpfleming/jinjanator/tree/23.1.0) - 2023-07-24
+## [23.2.0](https://github.com/kpfleming/jinjanator-plugins/tree/23.2.0) - 2023-07-30
 
-Initial release!
+### Additions
+
+- Added hook for plugins to report their identities.
+  [[#1](https://github.com/kpfleming/jinjanator-plugins/issues/1)](https://github.com/kpfleming/jinjanator-plugins/issues/1)
+- Added three exceptions which Format plugins can raise to indicate problems with options provided to them.
+  [[#2](https://github.com/kpfleming/jinjanator-plugins/issues/2)](https://github.com/kpfleming/jinjanator-plugins/issues/2)
+
+
+### Changes
 
+- Converted tests to proper unit tests.
+
+
+## [23.1.0](https://github.com/kpfleming/jinjanator-plugins/tree/23.1.0) - 2023-07-24
+
+Initial release!
 ---
 [→ Full Changelog](https://github.com/kpfleming/jinjanator-plugins/blob/main/CHANGELOG.md)
```

