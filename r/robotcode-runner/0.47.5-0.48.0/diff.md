# Comparing `tmp/robotcode_runner-0.47.5.tar.gz` & `tmp/robotcode_runner-0.48.0.tar.gz`

## Comparing `robotcode_runner-0.47.5.tar` & `robotcode_runner-0.48.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_runner-0.47.5/src/robotcode/runner/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_runner-0.47.5/src/robotcode/runner/__version__.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 robotcode_runner-0.47.5/src/robotcode/runner/hooks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_runner-0.47.5/src/robotcode/runner/py.typed
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 robotcode_runner-0.47.5/src/robotcode/runner/cli/__init__.py
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 robotcode_runner-0.47.5/src/robotcode/runner/cli/libdoc.py
--rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 robotcode_runner-0.47.5/src/robotcode/runner/cli/rebot.py
--rw-r--r--   0        0        0     6075 2020-02-02 00:00:00.000000 robotcode_runner-0.47.5/src/robotcode/runner/cli/robot.py
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 robotcode_runner-0.47.5/src/robotcode/runner/cli/testdoc.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 robotcode_runner-0.47.5/src/robotcode/runner/cli/discover/__init__.py
--rw-r--r--   0        0        0    23700 2020-02-02 00:00:00.000000 robotcode_runner-0.47.5/src/robotcode/runner/cli/discover/discover.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_runner-0.47.5/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_runner-0.47.5/LICENSE.txt
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_runner-0.47.5/README.md
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 robotcode_runner-0.47.5/pyproject.toml
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 robotcode_runner-0.47.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_runner-0.48.0/src/robotcode/runner/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_runner-0.48.0/src/robotcode/runner/__version__.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 robotcode_runner-0.48.0/src/robotcode/runner/hooks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_runner-0.48.0/src/robotcode/runner/py.typed
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 robotcode_runner-0.48.0/src/robotcode/runner/cli/__init__.py
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 robotcode_runner-0.48.0/src/robotcode/runner/cli/libdoc.py
+-rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 robotcode_runner-0.48.0/src/robotcode/runner/cli/rebot.py
+-rw-r--r--   0        0        0     6075 2020-02-02 00:00:00.000000 robotcode_runner-0.48.0/src/robotcode/runner/cli/robot.py
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 robotcode_runner-0.48.0/src/robotcode/runner/cli/testdoc.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 robotcode_runner-0.48.0/src/robotcode/runner/cli/discover/__init__.py
+-rw-r--r--   0        0        0    24078 2020-02-02 00:00:00.000000 robotcode_runner-0.48.0/src/robotcode/runner/cli/discover/discover.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_runner-0.48.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_runner-0.48.0/LICENSE.txt
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_runner-0.48.0/README.md
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 robotcode_runner-0.48.0/pyproject.toml
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 robotcode_runner-0.48.0/PKG-INFO
```

### Comparing `robotcode_runner-0.47.5/src/robotcode/runner/cli/libdoc.py` & `robotcode_runner-0.48.0/src/robotcode/runner/cli/libdoc.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.47.5/src/robotcode/runner/cli/rebot.py` & `robotcode_runner-0.48.0/src/robotcode/runner/cli/rebot.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.47.5/src/robotcode/runner/cli/robot.py` & `robotcode_runner-0.48.0/src/robotcode/runner/cli/robot.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.47.5/src/robotcode/runner/cli/testdoc.py` & `robotcode_runner-0.48.0/src/robotcode/runner/cli/testdoc.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.47.5/src/robotcode/runner/cli/discover/discover.py` & `robotcode_runner-0.48.0/src/robotcode/runner/cli/discover/discover.py`

 * *Files 5% similar despite different names*

```diff
@@ -131,23 +131,24 @@
                 LOGGER.error(str(e))
                 return ErroneousTestSuite(
                     error_message=str(e), name=TestSuite.name_from_source(structure.source), source=structure.source
                 ), TestDefaults(self.parent_defaults)
 
         SuiteStructureParser._build_suite_directory = build_suite_directory
 
-        old_validate_execution_mode = SuiteStructureParser._validate_execution_mode
+        if get_robot_version() < (6, 1, 1):
+            old_validate_execution_mode = SuiteStructureParser._validate_execution_mode
 
-        def _validate_execution_mode(self: SuiteStructureParser, suite: TestSuite) -> None:
-            try:
-                old_validate_execution_mode(self, suite)
-            except DataError as e:
-                LOGGER.error(f"Parsing '{suite.source}' failed: {e.message}")
+            def _validate_execution_mode(self: SuiteStructureParser, suite: TestSuite) -> None:
+                try:
+                    old_validate_execution_mode(self, suite)
+                except DataError as e:
+                    LOGGER.error(f"Parsing '{suite.source}' failed: {e.message}")
 
-        SuiteStructureParser._validate_execution_mode = _validate_execution_mode
+            SuiteStructureParser._validate_execution_mode = _validate_execution_mode
 
     old_get_file = FileReader._get_file
 
     def get_file(self: FileReader, source: Union[str, Path, IOBase], accept_text: bool) -> Any:
         path = self._get_path(source, accept_text)
         if path:
             if _stdin_data is not None and (data := _stdin_data.get(str(path))) is not None:
@@ -460,25 +461,36 @@
     suite, diagnostics = handle_options(app, by_longname, exclude_by_longname, robot_options_and_args)
 
     collector = Collector()
     suite.visit(collector)
 
     if collector.all.children:
         if app.config.output_format is None or app.config.output_format == OutputFormat.TEXT:
-            tests_or_tasks = "Tasks" if suite.rpa else "Tests"
+            tests_or_tasks = "Task" if suite.rpa else "Test"
 
             def print(item: TestItem, indent: int = 0) -> Iterable[str]:
-                yield (
-                    f"{'  ' * indent}"
-                    f"{item.type.capitalize() if item.type == 'suite' else tests_or_tasks.capitalize() }: "
-                    f"{item.name}{os.linesep}"
+                type = click.style(
+                    item.type.capitalize() if item.type == "suite" else tests_or_tasks.capitalize(), fg="green"
                 )
-                if item.children:
-                    for child in item.children:
-                        yield from print(child, indent + 2)
+
+                if item.type == "test":
+                    yield f"    {type}: {item.longname}{os.linesep}"
+                else:
+                    yield f"{type}: {item.longname}{os.linesep}"
+
+                for child in item.children or []:
+                    yield from print(child, indent + 2)
+
+                # type = click.style(
+                #     item.type.capitalize() if item.type == "suite" else tests_or_tasks.capitalize(), fg="green"
+                # )
+                # yield (f"{'  ' * indent}{type}: {item.name}{os.linesep}")
+                # if item.children:
+                #     for child in item.children:
+                #         yield from print(child, indent + 2)
 
                 if indent == 0:
                     yield os.linesep
                     yield f"Summary:{os.linesep}"
                     yield f"  Suites: {collector.statistics.suites}{os.linesep}"
                     yield f"  Suites with {tests_or_tasks}: {collector.statistics.suites_with_tests}{os.linesep}"
                     yield f"  {tests_or_tasks}: {collector.statistics.tests}{os.linesep}"
@@ -634,38 +646,18 @@
                 app.echo_via_pager(print(collector.tags))
 
         else:
             app.print_data(TagsResult(collector.tags), remove_defaults=True)
 
 
 @dataclass
-class RobotVersion:
-    major: int
-    minor: int
-    patch: Optional[int] = None
-    pre_id: Optional[str] = None
-    pre_number: Optional[int] = None
-    dev: Optional[int] = None
-
-
-@dataclass
-class PythonVersion:
-    major: int
-    minor: int
-    micro: int
-    releaselevel: str
-    serial: int
-
-
-@dataclass
 class Info:
-    robot_version: RobotVersion
     robot_version_string: str
     robot_env: Dict[str, str]
-    python_version: PythonVersion
+    robotcode_version_string: str
     python_version_string: str
     machine: str
     processor: str
     platform: str
     system: str
     system_version: str
 
@@ -682,36 +674,41 @@
 
     \b
     Examples:
     ```
     robotcode discover info
     ```
     """
+    import pprint
+
     from robot.version import get_version as get_version
+    from robotcode.core.dataclasses import as_dict
+
+    from ...__version__ import __version__
 
     robot_env: Dict[str, str] = {}
     if "ROBOT_OPTIONS" in os.environ:
         robot_env["ROBOT_OPTIONS"] = os.environ["ROBOT_OPTIONS"]
     if "ROBOT_SYSLOG_FILE" in os.environ:
         robot_env["ROBOT_SYSLOG_FILE"] = os.environ["ROBOT_SYSLOG_FILE"]
     if "ROBOT_SYSLOG_LEVEL" in os.environ:
         robot_env["ROBOT_SYSLOG_LEVEL"] = os.environ["ROBOT_SYSLOG_LEVEL"]
     if "ROBOT_INTERNAL_TRACES" in os.environ:
         robot_env["ROBOT_INTERNAL_TRACES"] = os.environ["ROBOT_INTERNAL_TRACES"]
 
     info = Info(
-        RobotVersion(*get_robot_version()),
         get_version(),
         robot_env,
-        PythonVersion(*sys.version_info),
+        __version__,
         platform.python_version(),
         platform.machine(),
         platform.processor(),
         sys.platform,
         platform.system(),
         platform.version(),
     )
 
     if app.config.output_format is None or app.config.output_format == OutputFormat.TEXT:
-        app.print_data(info, remove_defaults=True)
+        app.echo_via_pager(pprint.pformat(as_dict(info, remove_defaults=True), compact=True, sort_dicts=False))
+        # app.print_data(info, remove_defaults=True)
     else:
         app.print_data(info, remove_defaults=True)
```

### Comparing `robotcode_runner-0.47.5/.gitignore` & `robotcode_runner-0.48.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.47.5/LICENSE.txt` & `robotcode_runner-0.48.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.47.5/README.md` & `robotcode_runner-0.48.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.47.5/pyproject.toml` & `robotcode_runner-0.48.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -24,17 +24,17 @@
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dynamic = ["version"]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-robot==0.47.5",
-  "robotcode-modifiers==0.47.5",
-  "robotcode==0.47.5",
+  "robotcode-robot==0.48.0",
+  "robotcode-modifiers==0.48.0",
+  "robotcode==0.48.0",
 ]
 
 [project.entry-points.robotcode]
 runner = "robotcode.runner.hooks"
 
 [project.urls]
 Homepage = "https://robotcode.io"
```

### Comparing `robotcode_runner-0.47.5/PKG-INFO` & `robotcode_runner-0.48.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-runner
-Version: 0.47.5
+Version: 0.48.0
 Summary: RobotCode runner plugin for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,17 +21,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-modifiers==0.47.5
-Requires-Dist: robotcode-robot==0.47.5
-Requires-Dist: robotcode==0.47.5
+Requires-Dist: robotcode-modifiers==0.48.0
+Requires-Dist: robotcode-robot==0.48.0
+Requires-Dist: robotcode==0.48.0
 Requires-Dist: robotframework>=4.1.0
 Description-Content-Type: text/markdown
 
 # robotcode-runner
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-runner.svg)](https://pypi.org/project/robotcode-runner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-runner.svg)](https://pypi.org/project/robotcode-runner)
```

