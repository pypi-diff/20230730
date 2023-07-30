# Comparing `tmp/mcsrv-xImAnton-1.2.0.tar.gz` & `tmp/mcsrv-xImAnton-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcsrv-xImAnton-1.2.0.tar", last modified: Thu Dec 22 17:32:01 2022, max compression
+gzip compressed data, was "mcsrv-xImAnton-1.3.0.tar", last modified: Sun Jul 30 12:20:22 2023, max compression
```

## Comparing `mcsrv-xImAnton-1.2.0.tar` & `mcsrv-xImAnton-1.3.0.tar`

### file list

```diff
@@ -1,20 +1,32 @@
-drwxrwxrwx   0        0        0        0 2022-12-22 17:32:01.925588 mcsrv-xImAnton-1.2.0/
--rw-rw-rw-   0        0        0      652 2022-12-22 17:32:01.925588 mcsrv-xImAnton-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      105 2022-10-07 09:49:53.000000 mcsrv-xImAnton-1.2.0/README.md
--rw-rw-rw-   0        0        0       88 2022-04-03 09:36:19.000000 mcsrv-xImAnton-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      868 2022-12-22 17:32:01.936338 mcsrv-xImAnton-1.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-12-22 17:32:01.855744 mcsrv-xImAnton-1.2.0/src/
-drwxrwxrwx   0        0        0        0 2022-12-22 17:32:01.887764 mcsrv-xImAnton-1.2.0/src/mcsrv/
--rw-rw-rw-   0        0        0       28 2022-04-03 11:36:44.000000 mcsrv-xImAnton-1.2.0/src/mcsrv/__init__.py
--rw-rw-rw-   0        0        0       73 2022-04-03 11:08:34.000000 mcsrv-xImAnton-1.2.0/src/mcsrv/__main__.py
--rw-rw-rw-   0        0        0     6868 2022-12-22 17:00:35.000000 mcsrv-xImAnton-1.2.0/src/mcsrv/cli.py
--rw-rw-rw-   0        0        0     3025 2022-12-22 17:14:12.000000 mcsrv-xImAnton-1.2.0/src/mcsrv/javaexecutable.py
--rw-rw-rw-   0        0        0     8416 2022-12-22 17:28:26.000000 mcsrv-xImAnton-1.2.0/src/mcsrv/server.py
--rw-rw-rw-   0        0        0     1380 2022-12-22 17:25:02.000000 mcsrv-xImAnton-1.2.0/src/mcsrv/util.py
-drwxrwxrwx   0        0        0        0 2022-12-22 17:32:01.923543 mcsrv-xImAnton-1.2.0/src/mcsrv_xImAnton.egg-info/
--rw-rw-rw-   0        0        0      652 2022-12-22 17:32:01.000000 mcsrv-xImAnton-1.2.0/src/mcsrv_xImAnton.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      415 2022-12-22 17:32:01.000000 mcsrv-xImAnton-1.2.0/src/mcsrv_xImAnton.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-22 17:32:01.000000 mcsrv-xImAnton-1.2.0/src/mcsrv_xImAnton.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2022-12-22 17:32:01.000000 mcsrv-xImAnton-1.2.0/src/mcsrv_xImAnton.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       59 2022-12-22 17:32:01.000000 mcsrv-xImAnton-1.2.0/src/mcsrv_xImAnton.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-12-22 17:32:01.000000 mcsrv-xImAnton-1.2.0/src/mcsrv_xImAnton.egg-info/top_level.txt
+drwxrwxr-x   0 fritz     (1000) fritz     (1000)        0 2023-07-30 12:20:22.116021 mcsrv-xImAnton-1.3.0/
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)     1053 2023-07-30 12:20:22.116021 mcsrv-xImAnton-1.3.0/PKG-INFO
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)      520 2023-07-30 12:07:58.000000 mcsrv-xImAnton-1.3.0/README.md
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)       85 2023-03-26 11:35:36.000000 mcsrv-xImAnton-1.3.0/pyproject.toml
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)      862 2023-07-30 12:20:22.116021 mcsrv-xImAnton-1.3.0/setup.cfg
+drwxrwxr-x   0 fritz     (1000) fritz     (1000)        0 2023-07-30 12:20:22.112021 mcsrv-xImAnton-1.3.0/src/
+drwxrwxr-x   0 fritz     (1000) fritz     (1000)        0 2023-07-30 12:20:22.112021 mcsrv-xImAnton-1.3.0/src/mcsrv/
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)       27 2023-03-26 11:35:36.000000 mcsrv-xImAnton-1.3.0/src/mcsrv/__init__.py
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)       68 2023-03-26 11:35:36.000000 mcsrv-xImAnton-1.3.0/src/mcsrv/__main__.py
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)      609 2023-07-26 10:35:26.000000 mcsrv-xImAnton-1.3.0/src/mcsrv/api.py
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)    10859 2023-07-30 12:07:58.000000 mcsrv-xImAnton-1.3.0/src/mcsrv/cli.py
+drwxrwxr-x   0 fritz     (1000) fritz     (1000)        0 2023-07-30 12:20:22.112021 mcsrv-xImAnton-1.3.0/src/mcsrv/commands/
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)       64 2023-06-11 09:38:46.000000 mcsrv-xImAnton-1.3.0/src/mcsrv/commands/__init__.py
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)     3596 2023-07-30 11:54:19.000000 mcsrv-xImAnton-1.3.0/src/mcsrv/commands/create.py
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)      779 2023-06-11 09:22:40.000000 mcsrv-xImAnton-1.3.0/src/mcsrv/commands/start.py
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)     2930 2023-03-26 11:35:36.000000 mcsrv-xImAnton-1.3.0/src/mcsrv/javaexecutable.py
+drwxrwxr-x   0 fritz     (1000) fritz     (1000)        0 2023-07-30 12:20:22.112021 mcsrv-xImAnton-1.3.0/src/mcsrv/launch/
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)      220 2023-03-26 13:41:11.000000 mcsrv-xImAnton-1.3.0/src/mcsrv/launch/__init__.py
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)     1326 2023-03-27 15:30:09.000000 mcsrv-xImAnton-1.3.0/src/mcsrv/launch/forge.py
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)     1075 2023-03-27 15:30:09.000000 mcsrv-xImAnton-1.3.0/src/mcsrv/launch/jar.py
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)     1268 2023-03-27 15:30:09.000000 mcsrv-xImAnton-1.3.0/src/mcsrv/launch/launch.py
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)     2467 2023-07-30 12:11:38.000000 mcsrv-xImAnton-1.3.0/src/mcsrv/prompt.py
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)     1726 2023-06-11 10:38:07.000000 mcsrv-xImAnton-1.3.0/src/mcsrv/properties.py
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)    10465 2023-07-30 11:56:48.000000 mcsrv-xImAnton-1.3.0/src/mcsrv/server.py
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)     2637 2023-07-22 12:54:45.000000 mcsrv-xImAnton-1.3.0/src/mcsrv/util.py
+drwxrwxr-x   0 fritz     (1000) fritz     (1000)        0 2023-07-30 12:20:22.116021 mcsrv-xImAnton-1.3.0/src/mcsrv_xImAnton.egg-info/
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)     1053 2023-07-30 12:20:22.000000 mcsrv-xImAnton-1.3.0/src/mcsrv_xImAnton.egg-info/PKG-INFO
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)      670 2023-07-30 12:20:22.000000 mcsrv-xImAnton-1.3.0/src/mcsrv_xImAnton.egg-info/SOURCES.txt
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)        1 2023-07-30 12:20:22.000000 mcsrv-xImAnton-1.3.0/src/mcsrv_xImAnton.egg-info/dependency_links.txt
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)       41 2023-07-30 12:20:22.000000 mcsrv-xImAnton-1.3.0/src/mcsrv_xImAnton.egg-info/entry_points.txt
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)       89 2023-07-30 12:20:22.000000 mcsrv-xImAnton-1.3.0/src/mcsrv_xImAnton.egg-info/requires.txt
+-rw-rw-r--   0 fritz     (1000) fritz     (1000)        6 2023-07-30 12:20:22.000000 mcsrv-xImAnton-1.3.0/src/mcsrv_xImAnton.egg-info/top_level.txt
```

### Comparing `mcsrv-xImAnton-1.2.0/src/mcsrv/javaexecutable.py` & `mcsrv-xImAnton-1.3.0/src/mcsrv/javaexecutable.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-import os.path
-import pathlib
-import shlex
-import shutil
-import subprocess
-from typing import Union
-
-import click
-import inquirer
-from click import echo
-from colorama import Fore, Back
-
-RC_PATH = pathlib.Path("~/.javaversions").expanduser()
-
-
-def prompt_java_version():
-    installations = JavaExecutable.get_known_java_installations()
-
-    if len(installations) == 0:
-        echo(f"{Fore.RED}There are no registered Java installations")
-        raise click.exceptions.Exit(code=1)
-
-    if len(installations) == 1:
-        echo(f"{Fore.YELLOW}Nothing changed, there is only one registered Java version ({installations[0]})")
-        return
-
-    options = [(f"{j.version} ({j.path})", j.path) for j in installations]
-
-    answer = inquirer.prompt([inquirer.List("java_ver", message="Which Java version should be used?", choices=options)])
-
-    if not answer:
-        raise click.exceptions.Exit(code=1)
-
-    return answer["java_ver"]
-
-
-class JavaExecutable:
-    @classmethod
-    def get_known_java_installations(cls, return_paths: bool = False) -> list[Union["JavaExecutable", str]]:
-        if not RC_PATH.is_file():
-            return []
-
-        with RC_PATH.open("r") as f:
-            map_func = str.strip if return_paths else cls
-            return list(map(map_func, f.readlines()))
-
-    @classmethod
-    def get_default_version(cls) -> "JavaExecutable":
-        installs = cls.get_known_java_installations(True)
-
-        if len(installs) == 0:
-            print(f"{Fore.RED}No registered java versions. Set the default version using"
-                  f"{Fore.WHITE}{Back.BLUE}mcsrv java set")
-            raise click.exceptions.Exit(code=1)
-
-        return JavaExecutable(installs[0])
-
-    def __init__(self, path: str):
-        self.path: str = path.strip()
-        self.version: str = self.get_version()
-
-    def get_version(self) -> str:
-        path = shutil.which(self.path)
-        if not path:
-            echo(f"{Fore.RED}File {self.path!r} is not a valid java installation")
-            raise ValueError(f"file {self.path!r} is not a valid java installation")
-
-        self.path = path
-
-        version = subprocess.getoutput(shlex.join([self.path, "--version"])).split("\n")[0]
-
-        if not version.startswith("Unrecognized option: --version"):
-            return version
-
-        return subprocess.getoutput(shlex.join([self.path, "-version"])).split("\n")[0]
-
-    def register(self):
-        # check if already registered
-
-        javas = self.get_known_java_installations()
-
-        for java in javas:
-            if os.path.samefile(java.path, self.path):
-                return self
-
-        with RC_PATH.open("a" if RC_PATH.is_file() else "w") as f:
-            f.write(f"{self.path}\n")
-
-        return self
-
-    def __str__(self):
-        return f"Java Version {self.version!r} at {self.path!r}"
-
-    def __repr__(self):
-        return f"<JavaExecutable version={self.version!r} path={self.path!r}>"
+import os.path
+import pathlib
+import shlex
+import shutil
+import subprocess
+from typing import Union
+
+import click
+import inquirer
+from click import echo
+from colorama import Fore, Back
+
+RC_PATH = pathlib.Path("~/.javaversions").expanduser()
+
+
+def prompt_java_version():
+    installations = JavaExecutable.get_known_java_installations()
+
+    if len(installations) == 0:
+        echo(f"{Fore.RED}There are no registered Java installations")
+        raise click.exceptions.Exit(code=1)
+
+    if len(installations) == 1:
+        echo(f"{Fore.YELLOW}Nothing changed, there is only one registered Java version ({installations[0]})")
+        return
+
+    options = [(f"{j.version} ({j.path})", j.path) for j in installations]
+
+    answer = inquirer.prompt([inquirer.List("java_ver", message="Which Java version should be used?", choices=options)])
+
+    if not answer:
+        raise click.exceptions.Exit(code=1)
+
+    return answer["java_ver"]
+
+
+class JavaExecutable:
+    @classmethod
+    def get_known_java_installations(cls, return_paths: bool = False) -> list[Union["JavaExecutable", str]]:
+        if not RC_PATH.is_file():
+            return []
+
+        with RC_PATH.open("r") as f:
+            map_func = str.strip if return_paths else cls
+            return list(map(map_func, f.readlines()))
+
+    @classmethod
+    def get_default_version(cls) -> "JavaExecutable":
+        installs = cls.get_known_java_installations(True)
+
+        if len(installs) == 0:
+            print(f"{Fore.RED}No registered java versions. Set the default version using"
+                  f"{Fore.WHITE}{Back.BLUE}mcsrv java set")
+            raise click.exceptions.Exit(code=1)
+
+        return JavaExecutable(installs[0])
+
+    def __init__(self, path: str):
+        self.path: str = path.strip()
+        self.version: str = self.get_version()
+
+    def get_version(self) -> str:
+        path = shutil.which(self.path)
+        if not path:
+            echo(f"{Fore.RED}File {self.path!r} is not a valid java installation")
+            raise ValueError(f"file {self.path!r} is not a valid java installation")
+
+        self.path = path
+
+        version = subprocess.getoutput(shlex.join([self.path, "--version"])).split("\n")[0]
+
+        if not version.startswith("Unrecognized option: --version"):
+            return version
+
+        return subprocess.getoutput(shlex.join([self.path, "-version"])).split("\n")[0]
+
+    def register(self):
+        # check if already registered
+
+        javas = self.get_known_java_installations()
+
+        for java in javas:
+            if os.path.samefile(java.path, self.path):
+                return self
+
+        with RC_PATH.open("a" if RC_PATH.is_file() else "w") as f:
+            f.write(f"{self.path}\n")
+
+        return self
+
+    def __str__(self):
+        return f"Java Version {self.version!r} at {self.path!r}"
+
+    def __repr__(self):
+        return f"<JavaExecutable version={self.version!r} path={self.path!r}>"
```

