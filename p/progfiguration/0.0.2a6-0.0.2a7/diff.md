# Comparing `tmp/progfiguration-0.0.2a6.tar.gz` & `tmp/progfiguration-0.0.2a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "progfiguration-0.0.2a6.tar", last modified: Sat Jul 29 03:01:12 2023, max compression
+gzip compressed data, was "progfiguration-0.0.2a7.tar", last modified: Sun Jul 30 17:46:07 2023, max compression
```

## Comparing `progfiguration-0.0.2a6.tar` & `progfiguration-0.0.2a7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-29 03:01:12.087110 progfiguration-0.0.2a6/
--rw-------   0 mrled      (501) staff       (20)     1074 2023-07-24 04:31:40.000000 progfiguration-0.0.2a6/LICENSE
--rw-------   0 mrled      (501) staff       (20)     3109 2023-07-29 03:01:12.085823 progfiguration-0.0.2a6/PKG-INFO
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-29 03:01:12.066557 progfiguration-0.0.2a6/progfiguration/
--rw-------   0 mrled      (501) staff       (20)      518 2023-07-23 23:23:06.000000 progfiguration-0.0.2a6/progfiguration/__init__.py
--rw-------   0 mrled      (501) staff       (20)     3635 2023-07-23 21:17:36.000000 progfiguration-0.0.2a6/progfiguration/age.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-29 03:01:12.071053 progfiguration-0.0.2a6/progfiguration/builddata/
--rw-r--r--   0 mrled      (501) staff       (20)      253 2023-07-22 05:43:26.000000 progfiguration-0.0.2a6/progfiguration/builddata/__init__.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-29 03:01:12.074966 progfiguration-0.0.2a6/progfiguration/cli/
--rw-------   0 mrled      (501) staff       (20)       41 2023-07-23 22:36:36.000000 progfiguration-0.0.2a6/progfiguration/cli/__init__.py
--rw-------   0 mrled      (501) staff       (20)     6909 2023-07-29 02:11:37.000000 progfiguration-0.0.2a6/progfiguration/cli/progfiguration_core_cmd.py
--rw-r--r--   0 mrled      (501) staff       (20)    21296 2023-07-29 02:51:19.000000 progfiguration-0.0.2a6/progfiguration/cli/progfiguration_site_cmd.py
--rw-r--r--   0 mrled      (501) staff       (20)     5863 2023-07-23 23:10:02.000000 progfiguration-0.0.2a6/progfiguration/cli/util.py
--rw-------   0 mrled      (501) staff       (20)     5927 2023-07-22 05:27:56.000000 progfiguration-0.0.2a6/progfiguration/cmd.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-29 03:01:12.077529 progfiguration-0.0.2a6/progfiguration/inventory/
--rw-------   0 mrled      (501) staff       (20)    17726 2023-07-29 02:57:14.000000 progfiguration-0.0.2a6/progfiguration/inventory/__init__.py
--rw-------   0 mrled      (501) staff       (20)      874 2023-07-22 04:24:12.000000 progfiguration-0.0.2a6/progfiguration/inventory/nodes.py
--rw-------   0 mrled      (501) staff       (20)     4613 2023-07-23 23:21:39.000000 progfiguration-0.0.2a6/progfiguration/inventory/roles.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-29 03:01:12.080221 progfiguration-0.0.2a6/progfiguration/localhost/
--rw-------   0 mrled      (501) staff       (20)    11082 2023-07-23 23:21:13.000000 progfiguration-0.0.2a6/progfiguration/localhost/__init__.py
--rw-------   0 mrled      (501) staff       (20)     1184 2023-07-22 04:24:17.000000 progfiguration-0.0.2a6/progfiguration/localhost/authorized_keys.py
--rw-------   0 mrled      (501) staff       (20)     6056 2023-07-22 04:24:20.000000 progfiguration-0.0.2a6/progfiguration/localhost/disks.py
--rw-------   0 mrled      (501) staff       (20)     3044 2023-07-22 04:24:22.000000 progfiguration-0.0.2a6/progfiguration/localhost/localusers.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-29 03:01:12.080937 progfiguration-0.0.2a6/progfiguration/progfigbuild/
--rw-r--r--   0 mrled      (501) staff       (20)    17352 2023-07-25 04:49:02.000000 progfiguration-0.0.2a6/progfiguration/progfigbuild/__init__.py
--rw-r--r--   0 mrled      (501) staff       (20)     2505 2023-07-22 05:35:59.000000 progfiguration-0.0.2a6/progfiguration/progfigsite_validator.py
--rw-------   0 mrled      (501) staff       (20)      912 2023-07-22 05:36:48.000000 progfiguration-0.0.2a6/progfiguration/progfigtypes.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-29 03:01:12.081822 progfiguration-0.0.2a6/progfiguration/remotebrute/
--rw-------   0 mrled      (501) staff       (20)     3117 2023-07-22 04:24:58.000000 progfiguration-0.0.2a6/progfiguration/remotebrute/__init__.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-29 03:01:12.082503 progfiguration-0.0.2a6/progfiguration/sitewrapper/
--rw-r--r--   0 mrled      (501) staff       (20)     3972 2023-07-22 04:26:29.000000 progfiguration-0.0.2a6/progfiguration/sitewrapper/__init__.py
--rw-------   0 mrled      (501) staff       (20)     1804 2023-07-22 05:39:58.000000 progfiguration-0.0.2a6/progfiguration/ssh.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-29 03:01:12.083082 progfiguration-0.0.2a6/progfiguration/temple/
--rw-------   0 mrled      (501) staff       (20)      744 2023-06-28 22:11:55.000000 progfiguration-0.0.2a6/progfiguration/temple/__init__.py
--rw-r--r--   0 mrled      (501) staff       (20)     1832 2023-07-23 22:41:01.000000 progfiguration-0.0.2a6/progfiguration/util.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-29 03:01:12.070442 progfiguration-0.0.2a6/progfiguration.egg-info/
--rw-------   0 mrled      (501) staff       (20)     3109 2023-07-29 03:01:12.000000 progfiguration-0.0.2a6/progfiguration.egg-info/PKG-INFO
--rw-------   0 mrled      (501) staff       (20)     1108 2023-07-29 03:01:12.000000 progfiguration-0.0.2a6/progfiguration.egg-info/SOURCES.txt
--rw-------   0 mrled      (501) staff       (20)        1 2023-07-29 03:01:12.000000 progfiguration-0.0.2a6/progfiguration.egg-info/dependency_links.txt
--rw-------   0 mrled      (501) staff       (20)       83 2023-07-29 03:01:12.000000 progfiguration-0.0.2a6/progfiguration.egg-info/entry_points.txt
--rw-------   0 mrled      (501) staff       (20)      184 2023-07-29 03:01:12.000000 progfiguration-0.0.2a6/progfiguration.egg-info/requires.txt
--rw-------   0 mrled      (501) staff       (20)       15 2023-07-29 03:01:12.000000 progfiguration-0.0.2a6/progfiguration.egg-info/top_level.txt
--rw-------   0 mrled      (501) staff       (20)     1068 2023-07-29 03:00:47.000000 progfiguration-0.0.2a6/pyproject.toml
--rw-------   0 mrled      (501) staff       (20)     2718 2023-07-29 02:39:31.000000 progfiguration-0.0.2a6/readme.md
--rw-------   0 mrled      (501) staff       (20)       38 2023-07-29 03:01:12.087282 progfiguration-0.0.2a6/setup.cfg
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-29 03:01:12.084968 progfiguration-0.0.2a6/tests/
--rw-------   0 mrled      (501) staff       (20)     1293 2023-07-22 04:15:43.000000 progfiguration-0.0.2a6/tests/test_cmd.py
--rw-------   0 mrled      (501) staff       (20)     1778 2023-07-22 04:38:21.000000 progfiguration-0.0.2a6/tests/test_packaging.py
--rw-------   0 mrled      (501) staff       (20)     2321 2023-07-19 14:30:38.000000 progfiguration-0.0.2a6/tests/test_site.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-30 17:46:07.655598 progfiguration-0.0.2a7/
+-rw-------   0 mrled      (501) staff       (20)     1074 2023-07-24 04:31:40.000000 progfiguration-0.0.2a7/LICENSE
+-rw-------   0 mrled      (501) staff       (20)     3109 2023-07-30 17:46:07.655179 progfiguration-0.0.2a7/PKG-INFO
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-30 17:46:07.631877 progfiguration-0.0.2a7/progfiguration/
+-rw-------   0 mrled      (501) staff       (20)      518 2023-07-23 23:23:06.000000 progfiguration-0.0.2a7/progfiguration/__init__.py
+-rw-------   0 mrled      (501) staff       (20)     3635 2023-07-23 21:17:36.000000 progfiguration-0.0.2a7/progfiguration/age.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-30 17:46:07.635959 progfiguration-0.0.2a7/progfiguration/builddata/
+-rw-r--r--   0 mrled      (501) staff       (20)      253 2023-07-22 05:43:26.000000 progfiguration-0.0.2a7/progfiguration/builddata/__init__.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-30 17:46:07.640348 progfiguration-0.0.2a7/progfiguration/cli/
+-rw-------   0 mrled      (501) staff       (20)       41 2023-07-23 22:36:36.000000 progfiguration-0.0.2a7/progfiguration/cli/__init__.py
+-rw-------   0 mrled      (501) staff       (20)     6909 2023-07-29 02:11:37.000000 progfiguration-0.0.2a7/progfiguration/cli/progfiguration_core_cmd.py
+-rw-r--r--   0 mrled      (501) staff       (20)    21296 2023-07-29 02:51:19.000000 progfiguration-0.0.2a7/progfiguration/cli/progfiguration_site_cmd.py
+-rw-r--r--   0 mrled      (501) staff       (20)     5863 2023-07-23 23:10:02.000000 progfiguration-0.0.2a7/progfiguration/cli/util.py
+-rw-------   0 mrled      (501) staff       (20)     6669 2023-07-29 04:31:32.000000 progfiguration-0.0.2a7/progfiguration/cmd.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-30 17:46:07.643390 progfiguration-0.0.2a7/progfiguration/inventory/
+-rw-------   0 mrled      (501) staff       (20)    17726 2023-07-29 02:57:14.000000 progfiguration-0.0.2a7/progfiguration/inventory/__init__.py
+-rw-------   0 mrled      (501) staff       (20)      874 2023-07-22 04:24:12.000000 progfiguration-0.0.2a7/progfiguration/inventory/nodes.py
+-rw-------   0 mrled      (501) staff       (20)     4613 2023-07-23 23:21:39.000000 progfiguration-0.0.2a7/progfiguration/inventory/roles.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-30 17:46:07.647478 progfiguration-0.0.2a7/progfiguration/localhost/
+-rw-------   0 mrled      (501) staff       (20)    11082 2023-07-23 23:21:13.000000 progfiguration-0.0.2a7/progfiguration/localhost/__init__.py
+-rw-------   0 mrled      (501) staff       (20)     1184 2023-07-22 04:24:17.000000 progfiguration-0.0.2a7/progfiguration/localhost/authorized_keys.py
+-rw-------   0 mrled      (501) staff       (20)     6056 2023-07-22 04:24:20.000000 progfiguration-0.0.2a7/progfiguration/localhost/disks.py
+-rw-------   0 mrled      (501) staff       (20)     3044 2023-07-22 04:24:22.000000 progfiguration-0.0.2a7/progfiguration/localhost/localusers.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-30 17:46:07.648441 progfiguration-0.0.2a7/progfiguration/progfigbuild/
+-rw-r--r--   0 mrled      (501) staff       (20)    17264 2023-07-29 16:02:57.000000 progfiguration-0.0.2a7/progfiguration/progfigbuild/__init__.py
+-rw-r--r--   0 mrled      (501) staff       (20)     2505 2023-07-22 05:35:59.000000 progfiguration-0.0.2a7/progfiguration/progfigsite_validator.py
+-rw-------   0 mrled      (501) staff       (20)      912 2023-07-22 05:36:48.000000 progfiguration-0.0.2a7/progfiguration/progfigtypes.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-30 17:46:07.649708 progfiguration-0.0.2a7/progfiguration/remotebrute/
+-rw-------   0 mrled      (501) staff       (20)     3117 2023-07-22 04:24:58.000000 progfiguration-0.0.2a7/progfiguration/remotebrute/__init__.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-30 17:46:07.650638 progfiguration-0.0.2a7/progfiguration/sitewrapper/
+-rw-r--r--   0 mrled      (501) staff       (20)     3972 2023-07-22 04:26:29.000000 progfiguration-0.0.2a7/progfiguration/sitewrapper/__init__.py
+-rw-------   0 mrled      (501) staff       (20)     1804 2023-07-22 05:39:58.000000 progfiguration-0.0.2a7/progfiguration/ssh.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-30 17:46:07.651550 progfiguration-0.0.2a7/progfiguration/temple/
+-rw-------   0 mrled      (501) staff       (20)      744 2023-06-28 22:11:55.000000 progfiguration-0.0.2a7/progfiguration/temple/__init__.py
+-rw-r--r--   0 mrled      (501) staff       (20)     1832 2023-07-29 16:02:29.000000 progfiguration-0.0.2a7/progfiguration/util.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-30 17:46:07.635607 progfiguration-0.0.2a7/progfiguration.egg-info/
+-rw-------   0 mrled      (501) staff       (20)     3109 2023-07-30 17:46:07.000000 progfiguration-0.0.2a7/progfiguration.egg-info/PKG-INFO
+-rw-------   0 mrled      (501) staff       (20)     1108 2023-07-30 17:46:07.000000 progfiguration-0.0.2a7/progfiguration.egg-info/SOURCES.txt
+-rw-------   0 mrled      (501) staff       (20)        1 2023-07-30 17:46:07.000000 progfiguration-0.0.2a7/progfiguration.egg-info/dependency_links.txt
+-rw-------   0 mrled      (501) staff       (20)       83 2023-07-30 17:46:07.000000 progfiguration-0.0.2a7/progfiguration.egg-info/entry_points.txt
+-rw-------   0 mrled      (501) staff       (20)      184 2023-07-30 17:46:07.000000 progfiguration-0.0.2a7/progfiguration.egg-info/requires.txt
+-rw-------   0 mrled      (501) staff       (20)       15 2023-07-30 17:46:07.000000 progfiguration-0.0.2a7/progfiguration.egg-info/top_level.txt
+-rw-------   0 mrled      (501) staff       (20)     1068 2023-07-30 17:45:41.000000 progfiguration-0.0.2a7/pyproject.toml
+-rw-------   0 mrled      (501) staff       (20)     2718 2023-07-29 02:39:31.000000 progfiguration-0.0.2a7/readme.md
+-rw-------   0 mrled      (501) staff       (20)       38 2023-07-30 17:46:07.655737 progfiguration-0.0.2a7/setup.cfg
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-30 17:46:07.654225 progfiguration-0.0.2a7/tests/
+-rw-------   0 mrled      (501) staff       (20)     1293 2023-07-22 04:15:43.000000 progfiguration-0.0.2a7/tests/test_cmd.py
+-rw-------   0 mrled      (501) staff       (20)     1778 2023-07-22 04:38:21.000000 progfiguration-0.0.2a7/tests/test_packaging.py
+-rw-------   0 mrled      (501) staff       (20)     2321 2023-07-19 14:30:38.000000 progfiguration-0.0.2a7/tests/test_site.py
```

### Comparing `progfiguration-0.0.2a6/LICENSE` & `progfiguration-0.0.2a7/LICENSE`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a6/PKG-INFO` & `progfiguration-0.0.2a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progfiguration
-Version: 0.0.2a6
+Version: 0.0.2a7
 Summary: PROGramatic conFIGURATION for your infrastructure
 Author-email: Micah R Ledbetter <me@micahrl.com>
 License: MIT
 Project-URL: Homepage, https://github.com/mrled/progfiguration
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: development
```

### Comparing `progfiguration-0.0.2a6/progfiguration/__init__.py` & `progfiguration-0.0.2a7/progfiguration/__init__.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a6/progfiguration/age.py` & `progfiguration-0.0.2a7/progfiguration/age.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a6/progfiguration/cli/progfiguration_core_cmd.py` & `progfiguration-0.0.2a7/progfiguration/cli/progfiguration_core_cmd.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a6/progfiguration/cli/progfiguration_site_cmd.py` & `progfiguration-0.0.2a7/progfiguration/cli/progfiguration_site_cmd.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a6/progfiguration/cli/util.py` & `progfiguration-0.0.2a7/progfiguration/cli/util.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a6/progfiguration/cmd.py` & `progfiguration-0.0.2a7/progfiguration/cmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,14 +107,30 @@
             if stream.fileno() == stdout_fileno:
                 raise Exception("Exception on stdout")
             elif stream.fileno() == stderr_fileno:
                 raise Exception("Exception on stderr")
             else:
                 raise Exception(f"Unknown exception in select result. Fileno: {stream.fileno()}")
 
+    # Check for any remaining output after the process has exited.
+    # Without this, the last line of output may not be printed,
+    # if output is buffered (very normal)
+    # and the process doesn't explictly flush upon exit
+    # (also very normal, and will definitely happen if the process crashes or gets KILLed).
+    for stream in [process.stdout, process.stderr]:
+        for line in stream.readlines():
+            if stream.fileno() == stdout_fileno:
+                stdoutbuf.write(line)
+                if print_output:
+                    sys.stdout.write(line)
+            elif stream.fileno() == stderr_fileno:
+                stderrbuf.write(line)
+                if print_output:
+                    sys.stderr.write(line)
+
     # We'd like to just seek(0) on the stdout/stderr buffers, but "underlying stream is not seekable",
     # So we create new buffers above, write to them line by line, and replace the old ones with these.
     process.stdout.close()  # type: ignore
     stdoutbuf.seek(0)
     process.stdout = stdoutbuf
     process.stderr.close()  # type: ignore
     stderrbuf.seek(0)
```

### Comparing `progfiguration-0.0.2a6/progfiguration/inventory/__init__.py` & `progfiguration-0.0.2a7/progfiguration/inventory/__init__.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a6/progfiguration/inventory/nodes.py` & `progfiguration-0.0.2a7/progfiguration/inventory/nodes.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a6/progfiguration/inventory/roles.py` & `progfiguration-0.0.2a7/progfiguration/inventory/roles.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a6/progfiguration/localhost/__init__.py` & `progfiguration-0.0.2a7/progfiguration/localhost/__init__.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a6/progfiguration/localhost/authorized_keys.py` & `progfiguration-0.0.2a7/progfiguration/localhost/authorized_keys.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a6/progfiguration/localhost/disks.py` & `progfiguration-0.0.2a7/progfiguration/localhost/disks.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a6/progfiguration/localhost/localusers.py` & `progfiguration-0.0.2a7/progfiguration/localhost/localusers.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a6/progfiguration/progfigbuild/__init__.py` & `progfiguration-0.0.2a7/progfiguration/progfigbuild/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -373,15 +373,14 @@
 
     with ProgfigsitePythonPackagePreparer(
         progfigsite_filesystem_path,
         build_date=build_date,
         progfiguration_package_path=progfiguration_package_path,
         keep_injected_files=keep_injected_files,
     ) as preparer:
-        # built = builder_function(preparer.progfigsite_project_path, package_out_path)
         cmd = [
             "python",
             "-m",
             "build",
             "-s",
             "-o",
             package_out_path.as_posix(),
```

### Comparing `progfiguration-0.0.2a6/progfiguration/progfigsite_validator.py` & `progfiguration-0.0.2a7/progfiguration/progfigsite_validator.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a6/progfiguration/progfigtypes.py` & `progfiguration-0.0.2a7/progfiguration/progfigtypes.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a6/progfiguration/remotebrute/__init__.py` & `progfiguration-0.0.2a7/progfiguration/remotebrute/__init__.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a6/progfiguration/sitewrapper/__init__.py` & `progfiguration-0.0.2a7/progfiguration/sitewrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a6/progfiguration/ssh.py` & `progfiguration-0.0.2a7/progfiguration/ssh.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a6/progfiguration/temple/__init__.py` & `progfiguration-0.0.2a7/progfiguration/temple/__init__.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a6/progfiguration/util.py` & `progfiguration-0.0.2a7/progfiguration/util.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a6/progfiguration.egg-info/PKG-INFO` & `progfiguration-0.0.2a7/progfiguration.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progfiguration
-Version: 0.0.2a6
+Version: 0.0.2a7
 Summary: PROGramatic conFIGURATION for your infrastructure
 Author-email: Micah R Ledbetter <me@micahrl.com>
 License: MIT
 Project-URL: Homepage, https://github.com/mrled/progfiguration
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: development
```

### Comparing `progfiguration-0.0.2a6/progfiguration.egg-info/SOURCES.txt` & `progfiguration-0.0.2a7/progfiguration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a6/pyproject.toml` & `progfiguration-0.0.2a7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "progfiguration"
-version = "0.0.2a6"
+version = "0.0.2a7"
 description = "PROGramatic conFIGURATION for your infrastructure"
 license = { text = "MIT" }
 readme = "readme.md"
 requires-python = ">=3.10"
 
 [[project.authors]]
 name = "Micah R Ledbetter"
```

### Comparing `progfiguration-0.0.2a6/readme.md` & `progfiguration-0.0.2a7/readme.md`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a6/tests/test_cmd.py` & `progfiguration-0.0.2a7/tests/test_cmd.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a6/tests/test_packaging.py` & `progfiguration-0.0.2a7/tests/test_packaging.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a6/tests/test_site.py` & `progfiguration-0.0.2a7/tests/test_site.py`

 * *Files identical despite different names*

