# Comparing `tmp/portablemc-4.0.0rc1.tar.gz` & `tmp/portablemc-4.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portablemc-4.0.0rc1.tar", max compression
+gzip compressed data, was "portablemc-4.0.0rc2.tar", max compression
```

## Comparing `portablemc-4.0.0rc1.tar` & `portablemc-4.0.0rc2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35149 2023-07-14 20:55:06.871777 portablemc-4.0.0rc1/LICENSE
--rw-r--r--   0        0        0    14683 2023-07-29 19:17:52.174139 portablemc-4.0.0rc1/README.md
--rw-r--r--   0        0        0      306 2023-07-22 19:03:05.137436 portablemc-4.0.0rc1/portablemc/__init__.py
--rw-r--r--   0        0        0      800 2023-07-14 20:55:06.888443 portablemc-4.0.0rc1/portablemc/__main__.py
--rw-r--r--   0        0        0    16930 2023-07-29 18:39:34.554294 portablemc-4.0.0rc1/portablemc/auth.py
--rw-r--r--   0        0        0    28227 2023-07-29 19:42:29.366986 portablemc-4.0.0rc1/portablemc/cli/__init__.py
--rw-r--r--   0        0        0    13780 2023-07-29 19:58:42.262680 portablemc-4.0.0rc1/portablemc/cli/lang.py
--rw-r--r--   0        0        0     9442 2023-07-29 20:10:30.949309 portablemc-4.0.0rc1/portablemc/cli/output.py
--rw-r--r--   0        0        0     7297 2023-07-29 19:06:02.641566 portablemc-4.0.0rc1/portablemc/cli/parse.py
--rw-r--r--   0        0        0     3034 2023-07-28 21:45:28.559579 portablemc-4.0.0rc1/portablemc/cli/util.py
--rw-r--r--   0        0        0    12222 2023-07-29 20:26:00.437021 portablemc-4.0.0rc1/portablemc/download.py
--rw-r--r--   0        0        0     5322 2023-07-29 16:13:33.741775 portablemc-4.0.0rc1/portablemc/fabric.py
--rw-r--r--   0        0        0    18738 2023-07-29 16:13:49.891610 portablemc-4.0.0rc1/portablemc/forge.py
--rw-r--r--   0        0        0     2373 2023-07-15 10:13:00.771725 portablemc-4.0.0rc1/portablemc/http.py
--rw-r--r--   0        0        0    75003 2023-07-29 19:33:08.560588 portablemc-4.0.0rc1/portablemc/standard.py
--rw-r--r--   0        0        0     5040 2023-07-23 13:48:34.873644 portablemc-4.0.0rc1/portablemc/util.py
--rw-r--r--   0        0        0      950 2023-07-22 19:08:50.757737 portablemc-4.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0    15730 1970-01-01 00:00:00.000000 portablemc-4.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-14 20:55:06.871777 portablemc-4.0.0rc2/LICENSE
+-rw-r--r--   0        0        0    14683 2023-07-29 19:17:52.174139 portablemc-4.0.0rc2/README.md
+-rw-r--r--   0        0        0      306 2023-07-29 21:27:01.773514 portablemc-4.0.0rc2/portablemc/__init__.py
+-rw-r--r--   0        0        0      800 2023-07-14 20:55:06.888443 portablemc-4.0.0rc2/portablemc/__main__.py
+-rw-r--r--   0        0        0    16930 2023-07-29 18:39:34.554294 portablemc-4.0.0rc2/portablemc/auth.py
+-rw-r--r--   0        0        0    28713 2023-07-29 22:06:41.150534 portablemc-4.0.0rc2/portablemc/cli/__init__.py
+-rw-r--r--   0        0        0    13780 2023-07-29 19:58:42.262680 portablemc-4.0.0rc2/portablemc/cli/lang.py
+-rw-r--r--   0        0        0     9442 2023-07-29 20:10:30.949309 portablemc-4.0.0rc2/portablemc/cli/output.py
+-rw-r--r--   0        0        0     7297 2023-07-29 19:06:02.641566 portablemc-4.0.0rc2/portablemc/cli/parse.py
+-rw-r--r--   0        0        0     3034 2023-07-28 21:45:28.559579 portablemc-4.0.0rc2/portablemc/cli/util.py
+-rw-r--r--   0        0        0    12222 2023-07-29 20:26:00.437021 portablemc-4.0.0rc2/portablemc/download.py
+-rw-r--r--   0        0        0     5322 2023-07-29 16:13:33.741775 portablemc-4.0.0rc2/portablemc/fabric.py
+-rw-r--r--   0        0        0    18738 2023-07-29 16:13:49.891610 portablemc-4.0.0rc2/portablemc/forge.py
+-rw-r--r--   0        0        0     2373 2023-07-15 10:13:00.771725 portablemc-4.0.0rc2/portablemc/http.py
+-rw-r--r--   0        0        0    75274 2023-07-29 21:36:43.490242 portablemc-4.0.0rc2/portablemc/standard.py
+-rw-r--r--   0        0        0     5040 2023-07-23 13:48:34.873644 portablemc-4.0.0rc2/portablemc/util.py
+-rw-r--r--   0        0        0      961 2023-07-30 10:28:46.744101 portablemc-4.0.0rc2/pyproject.toml
+-rw-r--r--   0        0        0    15730 1970-01-01 00:00:00.000000 portablemc-4.0.0rc2/PKG-INFO
```

### Comparing `portablemc-4.0.0rc1/LICENSE` & `portablemc-4.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `portablemc-4.0.0rc1/README.md` & `portablemc-4.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `portablemc-4.0.0rc1/portablemc/__main__.py` & `portablemc-4.0.0rc2/portablemc/__main__.py`

 * *Files identical despite different names*

### Comparing `portablemc-4.0.0rc1/portablemc/auth.py` & `portablemc-4.0.0rc2/portablemc/auth.py`

 * *Files identical despite different names*

### Comparing `portablemc-4.0.0rc1/portablemc/cli/__init__.py` & `portablemc-4.0.0rc2/portablemc/cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,24 @@
 EXIT_OK = 0
 EXIT_FAILURE = 1
 
 AUTH_DATABASE_FILE_NAME = "portablemc_auth.json"
 MANIFEST_CACHE_FILE_NAME = "portablemc_version_manifest.json"
 MICROSOFT_AZURE_APP_ID = "708e91b5-99f8-4a1d-80ec-e746cbb24771"
 
+DEFAULT_JVM_ARGS = [
+    "-Xmx2G",
+    "-XX:+UnlockExperimentalVMOptions",
+    "-XX:+UseG1GC",
+    "-XX:G1NewSizePercent=20",
+    "-XX:G1ReservePercent=20",
+    "-XX:MaxGCPauseMillis=50",
+    "-XX:G1HeapRegionSize=32M"
+]
+
 CommandHandler = Callable[[Any], Any]
 CommandTree = Dict[str, Union[CommandHandler, "CommandTree"]]
 
 
 def main(args: Optional[List[str]] = None):
     """Main entry point of the CLI. This function parses the input arguments and try to
     find a command handler to dispatch to. These command handlers are specified by the
@@ -323,14 +333,20 @@
                 for bin_path in ns.include_bin:
                     bin_path = Path(bin_path)
                     if not bin_path.is_file():
                         ns.out.task("FAILED", "start.additional_binary_not_found", path=bin_path)
                         ns.out.finish()
                         sys.exit(EXIT_FAILURE)
                     env.native_libs.append(bin_path)
+            
+            # Extend JVM arguments with given arguments, or defaults
+            if ns.jvm_args is None:
+                env.jvm_args.extend(DEFAULT_JVM_ARGS)
+            elif len(ns.jvm_args):
+                env.jvm_args.extend(ns.jvm_args.split())
 
             env.run(CliRunner(ns))
 
         sys.exit(EXIT_OK)
     
     except VersionNotFoundError as error:
         ns.out.task("FAILED", "start.version.not_found", version=error.version)
```

### Comparing `portablemc-4.0.0rc1/portablemc/cli/lang.py` & `portablemc-4.0.0rc2/portablemc/cli/lang.py`

 * *Files identical despite different names*

### Comparing `portablemc-4.0.0rc1/portablemc/cli/output.py` & `portablemc-4.0.0rc2/portablemc/cli/output.py`

 * *Files identical despite different names*

### Comparing `portablemc-4.0.0rc1/portablemc/cli/parse.py` & `portablemc-4.0.0rc2/portablemc/cli/parse.py`

 * *Files identical despite different names*

### Comparing `portablemc-4.0.0rc1/portablemc/cli/util.py` & `portablemc-4.0.0rc2/portablemc/cli/util.py`

 * *Files identical despite different names*

### Comparing `portablemc-4.0.0rc1/portablemc/download.py` & `portablemc-4.0.0rc2/portablemc/download.py`

 * *Files identical despite different names*

### Comparing `portablemc-4.0.0rc1/portablemc/fabric.py` & `portablemc-4.0.0rc2/portablemc/fabric.py`

 * *Files identical despite different names*

### Comparing `portablemc-4.0.0rc1/portablemc/forge.py` & `portablemc-4.0.0rc2/portablemc/forge.py`

 * *Files identical despite different names*

### Comparing `portablemc-4.0.0rc1/portablemc/http.py` & `portablemc-4.0.0rc2/portablemc/http.py`

 * *Files identical despite different names*

### Comparing `portablemc-4.0.0rc1/portablemc/standard.py` & `portablemc-4.0.0rc2/portablemc/standard.py`

 * *Files 1% similar despite different names*

```diff
@@ -871,15 +871,21 @@
 
             jvm_manifest["version"] = jvm_meta[0].get("version", {}).get("name")
 
             jvm_manifest_file.parent.mkdir(parents=True, exist_ok=True)
             with jvm_manifest_file.open("wt") as jvm_manifest_fp:
                 json.dump(jvm_manifest, jvm_manifest_fp)
         
-        self._jvm_path = jvm_dir.joinpath("bin", jvm_bin_filename)
+        # Special case for macOS because of weird directory structure.
+        if minecraft_os == "osx":
+            self.jvm_path = jvm_dir.joinpath("jre.bundle/Contents/Home/bin/java")
+        else:
+            self._jvm_path = jvm_dir.joinpath("bin", jvm_bin_filename)
+        
+        # This key is custom and set just above in code.
         self._jvm_version = jvm_manifest.get("version")
 
         jvm_files = jvm_manifest.get("files")
         if not isinstance(jvm_files, dict):
             raise ValueError("jvm manifest: /files must be an object")
 
         for jvm_file_path_prefix, jvm_file in jvm_files.items():
```

### Comparing `portablemc-4.0.0rc1/portablemc/util.py` & `portablemc-4.0.0rc2/portablemc/util.py`

 * *Files identical despite different names*

### Comparing `portablemc-4.0.0rc1/pyproject.toml` & `portablemc-4.0.0rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["poetry_core>=1.0.0"]
+requires = ["poetry_core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "portablemc"
-version = "4.0.0rc1"
+version = "4.0.0rc2"
 description = "PortableMC is a module that provides both an API for development of your custom launcher and an executable script to run PortableMC CLI."
 authors = ["Théo Rozier <contact@theorozier.fr>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/mindstorm38/portablemc"
 repository = "https://github.com/mindstorm38/portablemc"
 documentation = "https://github.com/mindstorm38/portablemc"
@@ -20,10 +20,11 @@
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 
 [tool.poetry.group.test.dependencies]
 pytest = "*"
+toml = "*"
 
 [tool.poetry.scripts]
 portablemc = "portablemc.cli:main"
```

### Comparing `portablemc-4.0.0rc1/PKG-INFO` & `portablemc-4.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portablemc
-Version: 4.0.0rc1
+Version: 4.0.0rc2
 Summary: PortableMC is a module that provides both an API for development of your custom launcher and an executable script to run PortableMC CLI.
 Home-page: https://github.com/mindstorm38/portablemc
 License: GPL-3.0-only
 Keywords: minecraft,launcher,portable,cli
 Author: Théo Rozier
 Author-email: contact@theorozier.fr
 Requires-Python: >=3.7
```

