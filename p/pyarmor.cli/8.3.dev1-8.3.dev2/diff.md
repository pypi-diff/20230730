# Comparing `tmp/pyarmor.cli-8.3.dev1.zip` & `tmp/pyarmor.cli-8.3.dev2.zip`

## zipinfo {}

```diff
@@ -1,33 +1,36 @@
-Zip file size: 52148 bytes, number of entries: 31
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 20:58 pyarmor.cli-8.3.dev1/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 20:58 pyarmor.cli-8.3.dev1/pyarmor/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 20:58 pyarmor.cli-8.3.dev1/pyarmor.cli.egg-info/
--rw-r--r--  2.0 unx     2852 b- defN 23-Jul-23 20:58 pyarmor.cli-8.3.dev1/PKG-INFO
--rw-r--r--  2.0 unx     1829 b- defN 23-Jul-19 09:23 pyarmor.cli-8.3.dev1/setup.py
--rw-r--r--  2.0 unx       38 b- defN 23-Jul-23 20:58 pyarmor.cli-8.3.dev1/setup.cfg
--rw-r--r--  2.0 unx     1598 b- defN 23-Mar-04 17:07 pyarmor.cli-8.3.dev1/README.rst
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 20:58 pyarmor.cli-8.3.dev1/pyarmor/cli/
--rw-r--r--  2.0 unx     7036 b- defN 23-Jun-21 23:40 pyarmor.cli-8.3.dev1/pyarmor/cli/bootstrap.py
--rw-r--r--  2.0 unx     7184 b- defN 23-May-31 08:47 pyarmor.cli-8.3.dev1/pyarmor/cli/merge.py
--rw-r--r--  2.0 unx    10726 b- defN 23-May-31 08:18 pyarmor.cli-8.3.dev1/pyarmor/cli/config.py
--rw-r--r--  2.0 unx    18993 b- defN 23-Jul-23 15:37 pyarmor.cli-8.3.dev1/pyarmor/cli/register.py
--rw-r--r--  2.0 unx     5835 b- defN 23-May-22 18:36 pyarmor.cli-8.3.dev1/pyarmor/cli/generate.py
--rw-r--r--  2.0 unx     2193 b- defN 23-Feb-22 22:43 pyarmor.cli-8.3.dev1/pyarmor/cli/shell.py
--rw-r--r--  2.0 unx     7158 b- defN 23-May-07 11:39 pyarmor.cli-8.3.dev1/pyarmor/cli/resource.py
--rw-r--r--  2.0 unx     1526 b- defN 23-Jul-19 09:21 pyarmor.cli-8.3.dev1/pyarmor/cli/__init__.py
--rw-r--r--  2.0 unx     4594 b- defN 23-Jun-30 13:25 pyarmor.cli-8.3.dev1/pyarmor/cli/docker.py
--rw-r--r--  2.0 unx    19470 b- defN 23-Jul-20 10:16 pyarmor.cli-8.3.dev1/pyarmor/cli/context.py
--rw-r--r--  2.0 unx     3137 b- defN 23-Jun-25 16:00 pyarmor.cli-8.3.dev1/pyarmor/cli/group.py
--rw-r--r--  2.0 unx     7718 b- defN 23-Jun-09 14:11 pyarmor.cli-8.3.dev1/pyarmor/cli/plugin.py
--rw-r--r--  2.0 unx     3956 b- defN 23-Apr-20 15:02 pyarmor.cli-8.3.dev1/pyarmor/cli/mixer.py
--rw-r--r--  2.0 unx     2487 b- defN 23-Mar-26 06:51 pyarmor.cli-8.3.dev1/pyarmor/cli/public_capsule.zip
--rw-r--r--  2.0 unx     9133 b- defN 23-Jul-20 10:08 pyarmor.cli-8.3.dev1/pyarmor/cli/default.cfg
--rw-r--r--  2.0 unx    23065 b- defN 23-Jun-30 23:02 pyarmor.cli-8.3.dev1/pyarmor/cli/__main__.py
--rw-r--r--  2.0 unx    16099 b- defN 23-Jun-21 23:40 pyarmor.cli-8.3.dev1/pyarmor/cli/repack.py
--rw-r--r--  2.0 unx     2852 b- defN 23-Jul-23 20:58 pyarmor.cli-8.3.dev1/pyarmor.cli.egg-info/PKG-INFO
--rw-r--r--  2.0 unx      626 b- defN 23-Jul-23 20:58 pyarmor.cli-8.3.dev1/pyarmor.cli.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       55 b- defN 23-Jul-23 20:58 pyarmor.cli-8.3.dev1/pyarmor.cli.egg-info/entry_points.txt
--rw-r--r--  2.0 unx       27 b- defN 23-Jul-23 20:58 pyarmor.cli-8.3.dev1/pyarmor.cli.egg-info/requires.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-23 20:58 pyarmor.cli-8.3.dev1/pyarmor.cli.egg-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-23 20:58 pyarmor.cli-8.3.dev1/pyarmor.cli.egg-info/dependency_links.txt
-31 files, 160196 bytes uncompressed, 47148 bytes compressed:  70.6%
+Zip file size: 427734 bytes, number of entries: 34
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 18:11 pyarmor.cli-8.3.dev2/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 18:11 pyarmor.cli-8.3.dev2/pyarmor/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 18:11 pyarmor.cli-8.3.dev2/pyarmor.cli.egg-info/
+-rw-r--r--  2.0 unx     2852 b- defN 23-Jul-30 18:11 pyarmor.cli-8.3.dev2/PKG-INFO
+-rw-r--r--  2.0 unx     1841 b- defN 23-Jul-29 08:08 pyarmor.cli-8.3.dev2/setup.py
+-rw-r--r--  2.0 unx       38 b- defN 23-Jul-30 18:11 pyarmor.cli-8.3.dev2/setup.cfg
+-rw-r--r--  2.0 unx     1598 b- defN 23-Mar-04 17:07 pyarmor.cli-8.3.dev2/README.rst
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-30 18:11 pyarmor.cli-8.3.dev2/pyarmor/cli/
+-rw-r--r--  2.0 unx     7036 b- defN 23-Jun-21 23:40 pyarmor.cli-8.3.dev2/pyarmor/cli/bootstrap.py
+-rw-r--r--  2.0 unx     7184 b- defN 23-May-31 08:47 pyarmor.cli-8.3.dev2/pyarmor/cli/merge.py
+-rw-r--r--  2.0 unx   132120 b- defN 23-Jul-30 17:45 pyarmor.cli-8.3.dev2/pyarmor/cli/core.data.2
+-rw-r--r--  2.0 unx    10726 b- defN 23-May-31 08:18 pyarmor.cli-8.3.dev2/pyarmor/cli/config.py
+-rw-r--r--  2.0 unx    55974 b- defN 23-Jul-30 17:45 pyarmor.cli-8.3.dev2/pyarmor/cli/core.data.3
+-rw-r--r--  2.0 unx    18993 b- defN 23-Jul-23 15:37 pyarmor.cli-8.3.dev2/pyarmor/cli/register.py
+-rw-r--r--  2.0 unx     5835 b- defN 23-May-22 18:36 pyarmor.cli-8.3.dev2/pyarmor/cli/generate.py
+-rw-r--r--  2.0 unx     2193 b- defN 23-Feb-22 22:43 pyarmor.cli-8.3.dev2/pyarmor/cli/shell.py
+-rw-r--r--  2.0 unx     7158 b- defN 23-May-07 11:39 pyarmor.cli-8.3.dev2/pyarmor/cli/resource.py
+-rw-r--r--  2.0 unx     1156 b- defN 23-Jul-30 16:59 pyarmor.cli-8.3.dev2/pyarmor/cli/__init__.py
+-rw-r--r--  2.0 unx     4594 b- defN 23-Jun-30 13:25 pyarmor.cli-8.3.dev2/pyarmor/cli/docker.py
+-rw-r--r--  2.0 unx    19926 b- defN 23-Jul-28 17:10 pyarmor.cli-8.3.dev2/pyarmor/cli/context.py
+-rw-r--r--  2.0 unx   186837 b- defN 23-Jul-30 17:45 pyarmor.cli-8.3.dev2/pyarmor/cli/core.data.1
+-rw-r--r--  2.0 unx     3137 b- defN 23-Jun-25 16:00 pyarmor.cli-8.3.dev2/pyarmor/cli/group.py
+-rw-r--r--  2.0 unx     7718 b- defN 23-Jun-09 14:11 pyarmor.cli-8.3.dev2/pyarmor/cli/plugin.py
+-rw-r--r--  2.0 unx     3956 b- defN 23-Apr-20 15:02 pyarmor.cli-8.3.dev2/pyarmor/cli/mixer.py
+-rw-r--r--  2.0 unx     2487 b- defN 23-Mar-26 06:51 pyarmor.cli-8.3.dev2/pyarmor/cli/public_capsule.zip
+-rw-r--r--  2.0 unx     9190 b- defN 23-Jul-29 08:15 pyarmor.cli-8.3.dev2/pyarmor/cli/default.cfg
+-rw-r--r--  2.0 unx    23065 b- defN 23-Jun-30 23:02 pyarmor.cli-8.3.dev2/pyarmor/cli/__main__.py
+-rw-r--r--  2.0 unx    16099 b- defN 23-Jun-21 23:40 pyarmor.cli-8.3.dev2/pyarmor/cli/repack.py
+-rw-r--r--  2.0 unx     2852 b- defN 23-Jul-30 18:11 pyarmor.cli-8.3.dev2/pyarmor.cli.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx      698 b- defN 23-Jul-30 18:11 pyarmor.cli-8.3.dev2/pyarmor.cli.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx       55 b- defN 23-Jul-30 18:11 pyarmor.cli-8.3.dev2/pyarmor.cli.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx       24 b- defN 23-Jul-30 18:11 pyarmor.cli-8.3.dev2/pyarmor.cli.egg-info/requires.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-30 18:11 pyarmor.cli-8.3.dev2/pyarmor.cli.egg-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-30 18:11 pyarmor.cli-8.3.dev2/pyarmor.cli.egg-info/dependency_links.txt
+34 files, 535351 bytes uncompressed, 422242 bytes compressed:  21.1%
```

## zipnote {}

```diff
@@ -1,94 +1,103 @@
-Filename: pyarmor.cli-8.3.dev1/
+Filename: pyarmor.cli-8.3.dev2/
 Comment: 
 
-Filename: pyarmor.cli-8.3.dev1/pyarmor/
+Filename: pyarmor.cli-8.3.dev2/pyarmor/
 Comment: 
 
-Filename: pyarmor.cli-8.3.dev1/pyarmor.cli.egg-info/
+Filename: pyarmor.cli-8.3.dev2/pyarmor.cli.egg-info/
 Comment: 
 
-Filename: pyarmor.cli-8.3.dev1/PKG-INFO
+Filename: pyarmor.cli-8.3.dev2/PKG-INFO
 Comment: 
 
-Filename: pyarmor.cli-8.3.dev1/setup.py
+Filename: pyarmor.cli-8.3.dev2/setup.py
 Comment: 
 
-Filename: pyarmor.cli-8.3.dev1/setup.cfg
+Filename: pyarmor.cli-8.3.dev2/setup.cfg
 Comment: 
 
-Filename: pyarmor.cli-8.3.dev1/README.rst
+Filename: pyarmor.cli-8.3.dev2/README.rst
 Comment: 
 
-Filename: pyarmor.cli-8.3.dev1/pyarmor/cli/
+Filename: pyarmor.cli-8.3.dev2/pyarmor/cli/
 Comment: 
 
-Filename: pyarmor.cli-8.3.dev1/pyarmor/cli/bootstrap.py
+Filename: pyarmor.cli-8.3.dev2/pyarmor/cli/bootstrap.py
 Comment: 
 
-Filename: pyarmor.cli-8.3.dev1/pyarmor/cli/merge.py
+Filename: pyarmor.cli-8.3.dev2/pyarmor/cli/merge.py
 Comment: 
 
-Filename: pyarmor.cli-8.3.dev1/pyarmor/cli/config.py
+Filename: pyarmor.cli-8.3.dev2/pyarmor/cli/core.data.2
 Comment: 
 
-Filename: pyarmor.cli-8.3.dev1/pyarmor/cli/register.py
+Filename: pyarmor.cli-8.3.dev2/pyarmor/cli/config.py
 Comment: 
 
-Filename: pyarmor.cli-8.3.dev1/pyarmor/cli/generate.py
+Filename: pyarmor.cli-8.3.dev2/pyarmor/cli/core.data.3
 Comment: 
 
-Filename: pyarmor.cli-8.3.dev1/pyarmor/cli/shell.py
+Filename: pyarmor.cli-8.3.dev2/pyarmor/cli/register.py
 Comment: 
 
-Filename: pyarmor.cli-8.3.dev1/pyarmor/cli/resource.py
+Filename: pyarmor.cli-8.3.dev2/pyarmor/cli/generate.py
 Comment: 
 
-Filename: pyarmor.cli-8.3.dev1/pyarmor/cli/__init__.py
+Filename: pyarmor.cli-8.3.dev2/pyarmor/cli/shell.py
 Comment: 
 
-Filename: pyarmor.cli-8.3.dev1/pyarmor/cli/docker.py
+Filename: pyarmor.cli-8.3.dev2/pyarmor/cli/resource.py
 Comment: 
 
-Filename: pyarmor.cli-8.3.dev1/pyarmor/cli/context.py
+Filename: pyarmor.cli-8.3.dev2/pyarmor/cli/__init__.py
 Comment: 
 
-Filename: pyarmor.cli-8.3.dev1/pyarmor/cli/group.py
+Filename: pyarmor.cli-8.3.dev2/pyarmor/cli/docker.py
 Comment: 
 
-Filename: pyarmor.cli-8.3.dev1/pyarmor/cli/plugin.py
+Filename: pyarmor.cli-8.3.dev2/pyarmor/cli/context.py
 Comment: 
 
-Filename: pyarmor.cli-8.3.dev1/pyarmor/cli/mixer.py
+Filename: pyarmor.cli-8.3.dev2/pyarmor/cli/core.data.1
 Comment: 
 
-Filename: pyarmor.cli-8.3.dev1/pyarmor/cli/public_capsule.zip
+Filename: pyarmor.cli-8.3.dev2/pyarmor/cli/group.py
 Comment: 
 
-Filename: pyarmor.cli-8.3.dev1/pyarmor/cli/default.cfg
+Filename: pyarmor.cli-8.3.dev2/pyarmor/cli/plugin.py
 Comment: 
 
-Filename: pyarmor.cli-8.3.dev1/pyarmor/cli/__main__.py
+Filename: pyarmor.cli-8.3.dev2/pyarmor/cli/mixer.py
 Comment: 
 
-Filename: pyarmor.cli-8.3.dev1/pyarmor/cli/repack.py
+Filename: pyarmor.cli-8.3.dev2/pyarmor/cli/public_capsule.zip
 Comment: 
 
-Filename: pyarmor.cli-8.3.dev1/pyarmor.cli.egg-info/PKG-INFO
+Filename: pyarmor.cli-8.3.dev2/pyarmor/cli/default.cfg
 Comment: 
 
-Filename: pyarmor.cli-8.3.dev1/pyarmor.cli.egg-info/SOURCES.txt
+Filename: pyarmor.cli-8.3.dev2/pyarmor/cli/__main__.py
 Comment: 
 
-Filename: pyarmor.cli-8.3.dev1/pyarmor.cli.egg-info/entry_points.txt
+Filename: pyarmor.cli-8.3.dev2/pyarmor/cli/repack.py
 Comment: 
 
-Filename: pyarmor.cli-8.3.dev1/pyarmor.cli.egg-info/requires.txt
+Filename: pyarmor.cli-8.3.dev2/pyarmor.cli.egg-info/PKG-INFO
 Comment: 
 
-Filename: pyarmor.cli-8.3.dev1/pyarmor.cli.egg-info/top_level.txt
+Filename: pyarmor.cli-8.3.dev2/pyarmor.cli.egg-info/SOURCES.txt
 Comment: 
 
-Filename: pyarmor.cli-8.3.dev1/pyarmor.cli.egg-info/dependency_links.txt
+Filename: pyarmor.cli-8.3.dev2/pyarmor.cli.egg-info/entry_points.txt
+Comment: 
+
+Filename: pyarmor.cli-8.3.dev2/pyarmor.cli.egg-info/requires.txt
+Comment: 
+
+Filename: pyarmor.cli-8.3.dev2/pyarmor.cli.egg-info/top_level.txt
+Comment: 
+
+Filename: pyarmor.cli-8.3.dev2/pyarmor.cli.egg-info/dependency_links.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `pyarmor.cli-8.3.dev1/PKG-INFO` & `pyarmor.cli-8.3.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyarmor.cli
-Version: 8.3.dev1
+Version: 8.3.dev2
 Summary: A comand line tool to obfuscate python scripts
 Home-page: https://github.com/dashingsoft/pyarmor
 Author: Jondy Zhao
 Author-email: pyarmor@163.com
 License: Free To Use But Restricted
 Description: Protect Python Scripts By Pyarmor
         =================================
```

## Comparing `pyarmor.cli-8.3.dev1/setup.py` & `pyarmor.cli-8.3.dev2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-__VERSION__ = ' 8.3.dev1'
+__VERSION__ = ' 8.3.dev2'
 
 with open('README.rst') as f:
     long_description = f.read()
 
 setup(
     name="pyarmor.cli",
 
@@ -43,18 +43,18 @@
     # project page. What does your project relate to?
     #
     # Note that this is a string of words separated by whitespace, not a list.
     keywords="protect obfuscate encrypt obfuscation distribute",
 
     packages=["pyarmor.cli"],
     package_dir={"pyarmor.cli": "pyarmor/cli"},
-    package_data={"pyarmor.cli": ["default.cfg", "public_capsule.zip"]},
+    package_data={"pyarmor.cli": ["default.cfg", "public_capsule.zip", "core.data.*"]},
 
     install_requires=[
-        'pyarmor.cli.core~=4.3.dev1'
+        'pyarmor.cli.core~=4.3.0'
     ],
 
     entry_points={
         'console_scripts': [
             'pyarmor=pyarmor.cli.__main__:main',
         ],
     },
```

## Comparing `pyarmor.cli-8.3.dev1/README.rst` & `pyarmor.cli-8.3.dev2/README.rst`

 * *Files identical despite different names*

## Comparing `pyarmor.cli-8.3.dev1/pyarmor/cli/bootstrap.py` & `pyarmor.cli-8.3.dev2/pyarmor/cli/bootstrap.py`

 * *Files identical despite different names*

## Comparing `pyarmor.cli-8.3.dev1/pyarmor/cli/merge.py` & `pyarmor.cli-8.3.dev2/pyarmor/cli/merge.py`

 * *Files identical despite different names*

## Comparing `pyarmor.cli-8.3.dev1/pyarmor/cli/config.py` & `pyarmor.cli-8.3.dev2/pyarmor/cli/config.py`

 * *Files identical despite different names*

## Comparing `pyarmor.cli-8.3.dev1/pyarmor/cli/register.py` & `pyarmor.cli-8.3.dev2/pyarmor/cli/register.py`

 * *Files identical despite different names*

## Comparing `pyarmor.cli-8.3.dev1/pyarmor/cli/generate.py` & `pyarmor.cli-8.3.dev2/pyarmor/cli/generate.py`

 * *Files identical despite different names*

## Comparing `pyarmor.cli-8.3.dev1/pyarmor/cli/shell.py` & `pyarmor.cli-8.3.dev2/pyarmor/cli/shell.py`

 * *Files identical despite different names*

## Comparing `pyarmor.cli-8.3.dev1/pyarmor/cli/resource.py` & `pyarmor.cli-8.3.dev2/pyarmor/cli/resource.py`

 * *Files identical despite different names*

## Comparing `pyarmor.cli-8.3.dev1/pyarmor/cli/docker.py` & `pyarmor.cli-8.3.dev2/pyarmor/cli/docker.py`

 * *Files identical despite different names*

## Comparing `pyarmor.cli-8.3.dev1/pyarmor/cli/context.py` & `pyarmor.cli-8.3.dev2/pyarmor/cli/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -637,7 +637,27 @@
                 with open(filename, encoding=encoding) as f:
                     return f.read()
 
     def runtime_plugin(self, source, target, platforms):
         for plugin in self.plugins:
             if hasattr(plugin, 'post_runtime'):
                 plugin.post_runtime(self, source, target, platforms)
+
+    #
+    # Core data, new in 8.3
+    #
+    def _core_data(self, name):
+        n = __file__.find('context.py')
+        with open(__file__[:n] + name, 'rb') as f:
+            return f.read()
+
+    @property
+    def core_data_1(self):
+        return self._core_data('core.data.1')
+
+    @property
+    def core_data_2(self):
+        return self._core_data('core.data.2')
+
+    @property
+    def core_data_3(self):
+        return self._core_data('core.data.3')
```

## Comparing `pyarmor.cli-8.3.dev1/pyarmor/cli/group.py` & `pyarmor.cli-8.3.dev2/pyarmor/cli/group.py`

 * *Files identical despite different names*

## Comparing `pyarmor.cli-8.3.dev1/pyarmor/cli/plugin.py` & `pyarmor.cli-8.3.dev2/pyarmor/cli/plugin.py`

 * *Files identical despite different names*

## Comparing `pyarmor.cli-8.3.dev1/pyarmor/cli/mixer.py` & `pyarmor.cli-8.3.dev2/pyarmor/cli/mixer.py`

 * *Files identical despite different names*

## Comparing `pyarmor.cli-8.3.dev1/pyarmor/cli/public_capsule.zip` & `pyarmor.cli-8.3.dev2/pyarmor/cli/public_capsule.zip`

 * *Files identical despite different names*

## Comparing `pyarmor.cli-8.3.dev1/pyarmor/cli/default.cfg` & `pyarmor.cli-8.3.dev2/pyarmor/cli/default.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [pyarmor]
 
 ;; Pyarmor version
 major = 8
 minor = 3
-patch = dev1
+patch = dev2
 
 ;; Core version
-cli.core = 4.3.dev1
+cli.core = 4.3.0
 
 ;; Deprecated since Pyarmor 8.2.5
 ; cli.runtime = 3.2.5
 
 ;; Default timeout when send request to remote server for
 ;;     check Pyarmor license
 ;;     register Pyarmor license
@@ -323,15 +323,15 @@
 cc = clang.exe
 cflags = --target=i686-elf-linux -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fno-stack-protector -fPIC -mno-sse -std=c99 -c
 
 [linux.x86_64.bcc]
 cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fPIC -fno-stack-protector -c
 
 [linux.aarch64.bcc]
-cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fPIC -fno-stack-protector -shared -nostdlib -Tlinux.aarch64.ldscript
+cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fPIC -fno-stack-protector -shared -nostdlib -DENABLE_BCC_MEMSET -Tlinux.aarch64.ldscript
 
 [linux.x86.bcc]
 cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fno-stack-protector -fPIC -c
 
 [linux.armv7.bcc]
 cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fno-stack-protector -shared -nostdlib -Tlinux.armv7.ldscript
 
@@ -341,23 +341,23 @@
 [darwin.aarch64.bcc]
 cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables --target=arm64-macho-darwin -fPIC -fno-addrsig -fno-stack-protector -shared -nostdlib -lsystem
 
 [android.x86_64.bcc]
 cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fPIC -fno-stack-protector -c
 
 [android.aarch64.bcc]
-cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fPIC -fno-stack-protector -shared -nostdlib -Tlinux.aarch64.ldscript
+cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fPIC -fno-stack-protector -shared -nostdlib -DENABLE_BCC_MEMSET -Tlinux.aarch64.ldscript
 
 [android.x86.bcc]
 cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fno-stack-protector -fPIC -c
 
 [android.armv7.bcc]
 cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fno-stack-protector -shared -nostdlib -Tlinux.armv7.ldscript
 
 [alpine.x86_64.bcc]
 cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fPIC -fno-stack-protector -c
 
 [alpine.aarch64.bcc]
-cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fPIC -fno-stack-protector -shared -nostdlib -Tlinux.aarch64.ldscript
+cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fPIC -fno-stack-protector -shared -nostdlib -DENABLE_BCC_MEMSET -Tlinux.aarch64.ldscript
 
 [freebsd.x86_64.bcc]
 cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fPIC -fno-stack-protector -c
```

## Comparing `pyarmor.cli-8.3.dev1/pyarmor/cli/__main__.py` & `pyarmor.cli-8.3.dev2/pyarmor/cli/__main__.py`

 * *Files identical despite different names*

## Comparing `pyarmor.cli-8.3.dev1/pyarmor/cli/repack.py` & `pyarmor.cli-8.3.dev2/pyarmor/cli/repack.py`

 * *Files identical despite different names*

## Comparing `pyarmor.cli-8.3.dev1/pyarmor.cli.egg-info/PKG-INFO` & `pyarmor.cli-8.3.dev2/pyarmor.cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyarmor.cli
-Version: 8.3.dev1
+Version: 8.3.dev2
 Summary: A comand line tool to obfuscate python scripts
 Home-page: https://github.com/dashingsoft/pyarmor
 Author: Jondy Zhao
 Author-email: pyarmor@163.com
 License: Free To Use But Restricted
 Description: Protect Python Scripts By Pyarmor
         =================================
```

## Comparing `pyarmor.cli-8.3.dev1/pyarmor.cli.egg-info/SOURCES.txt` & `pyarmor.cli-8.3.dev2/pyarmor.cli.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 pyarmor.cli.egg-info/requires.txt
 pyarmor.cli.egg-info/top_level.txt
 pyarmor/cli/__init__.py
 pyarmor/cli/__main__.py
 pyarmor/cli/bootstrap.py
 pyarmor/cli/config.py
 pyarmor/cli/context.py
+pyarmor/cli/core.data.1
+pyarmor/cli/core.data.2
+pyarmor/cli/core.data.3
 pyarmor/cli/default.cfg
 pyarmor/cli/docker.py
 pyarmor/cli/generate.py
 pyarmor/cli/group.py
 pyarmor/cli/merge.py
 pyarmor/cli/mixer.py
 pyarmor/cli/plugin.py
```

