# Comparing `tmp/pycomfort-0.0.8.tar.gz` & `tmp/pycomfort-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycomfort-0.0.8.tar", last modified: Wed Feb  9 21:41:00 2022, max compression
+gzip compressed data, was "pycomfort-0.0.9.tar", last modified: Sat Feb 12 11:31:59 2022, max compression
```

## Comparing `pycomfort-0.0.8.tar` & `pycomfort-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2022-02-09 21:41:00.650449 pycomfort-0.0.8/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)    11357 2021-12-16 16:50:44.000000 pycomfort-0.0.8/LICENSE
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      880 2022-02-09 21:41:00.650449 pycomfort-0.0.8/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      129 2021-12-22 21:42:51.000000 pycomfort-0.0.8/README.md
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2022-02-09 21:41:00.650449 pycomfort-0.0.8/pycomfort/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2021-12-16 16:51:51.000000 pycomfort-0.0.8/pycomfort/__init__.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1653 2022-02-09 21:37:08.000000 pycomfort-0.0.8/pycomfort/comfort.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4871 2022-02-09 21:39:50.000000 pycomfort-0.0.8/pycomfort/files.py
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2022-02-09 21:41:00.650449 pycomfort-0.0.8/pycomfort.egg-info/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      880 2022-02-09 21:41:00.000000 pycomfort-0.0.8/pycomfort.egg-info/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      288 2022-02-09 21:41:00.000000 pycomfort-0.0.8/pycomfort.egg-info/SOURCES.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2022-02-09 21:41:00.000000 pycomfort-0.0.8/pycomfort.egg-info/dependency_links.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      101 2022-02-09 21:41:00.000000 pycomfort-0.0.8/pycomfort.egg-info/entry_points.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       49 2022-02-09 21:41:00.000000 pycomfort-0.0.8/pycomfort.egg-info/requires.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       10 2022-02-09 21:41:00.000000 pycomfort-0.0.8/pycomfort.egg-info/top_level.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2022-02-09 21:41:00.650449 pycomfort-0.0.8/setup.cfg
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1453 2022-02-09 13:37:43.000000 pycomfort-0.0.8/setup.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2022-02-12 11:31:59.784242 pycomfort-0.0.9/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)    11357 2021-12-16 16:50:44.000000 pycomfort-0.0.9/LICENSE
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     2387 2022-02-12 11:31:59.784242 pycomfort-0.0.9/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1636 2022-02-12 11:31:45.000000 pycomfort-0.0.9/README.md
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2022-02-12 11:31:59.784242 pycomfort-0.0.9/pycomfort/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2021-12-16 16:51:51.000000 pycomfort-0.0.9/pycomfort/__init__.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1652 2022-02-12 11:19:28.000000 pycomfort-0.0.9/pycomfort/comfort.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4853 2022-02-12 11:24:06.000000 pycomfort-0.0.9/pycomfort/files.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2022-02-12 11:31:59.784242 pycomfort-0.0.9/pycomfort.egg-info/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     2387 2022-02-12 11:31:59.000000 pycomfort-0.0.9/pycomfort.egg-info/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      288 2022-02-12 11:31:59.000000 pycomfort-0.0.9/pycomfort.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2022-02-12 11:31:59.000000 pycomfort-0.0.9/pycomfort.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      101 2022-02-12 11:31:59.000000 pycomfort-0.0.9/pycomfort.egg-info/entry_points.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       49 2022-02-12 11:31:59.000000 pycomfort-0.0.9/pycomfort.egg-info/requires.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       10 2022-02-12 11:31:59.000000 pycomfort-0.0.9/pycomfort.egg-info/top_level.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2022-02-12 11:31:59.784242 pycomfort-0.0.9/setup.cfg
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1453 2022-02-12 11:19:28.000000 pycomfort-0.0.9/setup.py
```

### Comparing `pycomfort-0.0.8/LICENSE` & `pycomfort-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pycomfort-0.0.8/pycomfort/comfort.py` & `pycomfort-0.0.9/pycomfort/comfort.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 
 @click.command("replace_with_dictionary")
 @click.option('--file', type=click.Path(exists=True), help="rename file with substitution")
 @click.option('--dictionary', type=click.Path(exists=True), help="dictionary to load from")
 @click.option('--output', help="optional output, will rewrite --file is not output provided")
 @click.option('--verbose', type=click.BOOL, help="if we should output more to console")
-def replace_dict(file: str, dictionary: dict, output: Optional[str], verbose: bool = False):
+def replace_dict(file: str, dictionary: str, output: Optional[str], verbose: bool = False):
     print(f"replacing from {dict} in {file}")
     # reading the data from the file
     with Path(dictionary).open("r+") as f:
         data = f.read()
     js: dict = json.loads(data)
     print(f"substitutions dictionary is:")
     for k, v in js.items():
```

### Comparing `pycomfort-0.0.8/pycomfort/files.py` & `pycomfort-0.0.9/pycomfort/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,29 +115,30 @@
             return output
 
 
 def replace_from_dict_in_file(file: Path, replacement: dict, output: Optional[Path] = None, verbose: bool = False) -> Path:
     in_place = output is None
     with file.open("r+") as text_file:
         s: str = text_file.read()
-        for old, new in replacement.items():
-            if old in s:
-                if verbose:
-                    print(f"REPLACING {old}\n WITH {new}")
-                s = s.replace(old, new) # warning: mutation!
-        if in_place:
+    for old, new in replacement.items():
+        if old in s:
             if verbose:
-                print(f"editing {str(file)} in place")
-            text_file.write(s)
-            return file
-        else:
-            if verbose:
-                print(f"writing {str(file)} with replacements to {str(output)}")
-            output.write_text(s)
-            return output
+                print(f"REPLACING {old}\n WITH {new}")
+            s = s.replace(old, new) # warning: mutation!
+    if in_place:
+        if verbose:
+            print(f"editing {str(file)} in place")
+        with file.open("w") as rewrite:
+            rewrite.write(s)
+        return file
+    else:
+        if verbose:
+            print(f"writing {str(file)} with replacements to {str(output)}")
+        output.write_text(s)
+        return output
 
 
 
 def tprint(p: Path, prefix: str = "", debug: bool = False):
     """
     Pretty-print the content of the folder recursively
     :param p: path to print content for
```

### Comparing `pycomfort-0.0.8/setup.py` & `pycomfort-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'Pycomfort - Python helper methods to make life easier'
 LONG_DESCRIPTION = 'A package with python helper functions to make your life more comfortable'
 
 # Setting up
 setup(
     name="pycomfort",
     version=VERSION,
```

