# Comparing `tmp/matan-0.1.5.2.9.tar.gz` & `tmp/matan-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matan-0.1.5.2.9.tar", last modified: Wed Jun 28 22:31:41 2023, max compression
+gzip compressed data, was "matan-0.1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `matan-0.1.5.2.9.tar` & `matan-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,42 @@
-drwxr-xr-x   0 uuu       (1000) uuu       (1000)        0 2023-06-28 22:31:41.238112 matan-0.1.5.2.9/
--rw-r--r--   0 uuu       (1000) uuu       (1000)    34670 2023-06-18 20:22:37.000000 matan-0.1.5.2.9/LICENSE
--rw-r--r--   0 uuu       (1000) uuu       (1000)     4342 2023-06-28 22:31:41.238112 matan-0.1.5.2.9/PKG-INFO
--rw-r--r--   0 uuu       (1000) uuu       (1000)     3373 2023-06-28 22:30:13.000000 matan-0.1.5.2.9/README.md
-drwxr-xr-x   0 uuu       (1000) uuu       (1000)        0 2023-06-28 22:31:41.238112 matan-0.1.5.2.9/matan/
--rw-r--r--   0 uuu       (1000) uuu       (1000)       84 2023-06-28 16:35:23.000000 matan-0.1.5.2.9/matan/__init__.py
--rw-r--r--   0 uuu       (1000) uuu       (1000)      156 2023-06-19 18:03:25.000000 matan-0.1.5.2.9/matan/_misc.py
--rw-r--r--   0 uuu       (1000) uuu       (1000)     4960 2023-06-19 18:03:25.000000 matan-0.1.5.2.9/matan/files.py
-drwxr-xr-x   0 uuu       (1000) uuu       (1000)        0 2023-06-28 22:31:41.238112 matan-0.1.5.2.9/matan/polymers/
--rw-r--r--   0 uuu       (1000) uuu       (1000)        0 2023-06-28 16:39:25.000000 matan-0.1.5.2.9/matan/polymers/__init__.py
-drwxr-xr-x   0 uuu       (1000) uuu       (1000)        0 2023-06-28 22:31:41.238112 matan-0.1.5.2.9/matan/polymers/charpy/
--rw-r--r--   0 uuu       (1000) uuu       (1000)      815 2023-06-28 16:39:25.000000 matan-0.1.5.2.9/matan/polymers/charpy/__init__.py
-drwxr-xr-x   0 uuu       (1000) uuu       (1000)        0 2023-06-28 22:31:41.238112 matan-0.1.5.2.9/matan/polymers/tensile/
-drwxr-xr-x   0 uuu       (1000) uuu       (1000)        0 2023-06-28 22:31:41.238112 matan-0.1.5.2.9/matan/polymers/tensile/ISO527/
--rw-r--r--   0 uuu       (1000) uuu       (1000)     2710 2023-06-28 16:39:25.000000 matan-0.1.5.2.9/matan/polymers/tensile/ISO527/__init__.py
--rw-r--r--   0 uuu       (1000) uuu       (1000)    13780 2023-06-28 16:39:25.000000 matan-0.1.5.2.9/matan/polymers/tensile/__init__.py
--rw-r--r--   0 uuu       (1000) uuu       (1000)       33 2023-06-28 16:39:25.000000 matan-0.1.5.2.9/matan/polymers/tensile/misc.py
--rw-r--r--   0 uuu       (1000) uuu       (1000)     7948 2023-06-28 16:39:25.000000 matan-0.1.5.2.9/matan/sample.py
-drwxr-xr-x   0 uuu       (1000) uuu       (1000)        0 2023-06-28 22:31:41.238112 matan-0.1.5.2.9/matan.egg-info/
--rw-r--r--   0 uuu       (1000) uuu       (1000)     4342 2023-06-28 22:31:41.000000 matan-0.1.5.2.9/matan.egg-info/PKG-INFO
--rw-r--r--   0 uuu       (1000) uuu       (1000)      413 2023-06-28 22:31:41.000000 matan-0.1.5.2.9/matan.egg-info/SOURCES.txt
--rw-r--r--   0 uuu       (1000) uuu       (1000)        1 2023-06-28 22:31:41.000000 matan-0.1.5.2.9/matan.egg-info/dependency_links.txt
--rw-r--r--   0 uuu       (1000) uuu       (1000)       17 2023-06-28 22:31:41.000000 matan-0.1.5.2.9/matan.egg-info/requires.txt
--rw-r--r--   0 uuu       (1000) uuu       (1000)        6 2023-06-28 22:31:41.000000 matan-0.1.5.2.9/matan.egg-info/top_level.txt
--rw-r--r--   0 uuu       (1000) uuu       (1000)      103 2023-06-28 22:31:41.242112 matan-0.1.5.2.9/setup.cfg
--rw-r--r--   0 uuu       (1000) uuu       (1000)     1775 2023-06-28 22:30:21.000000 matan-0.1.5.2.9/setup.py
+-rw-r--r--   0        0        0     3651 2023-07-29 12:04:42.656318 matan-0.1.6/.gitignore
+-rw-r--r--   0        0        0      798 2023-07-29 12:04:42.656318 matan-0.1.6/.woodpecker.yml
+-rw-r--r--   0        0        0    34670 2023-07-29 12:04:42.656318 matan-0.1.6/LICENSE
+-rw-r--r--   0        0        0     4846 2023-07-29 12:04:42.656318 matan-0.1.6/MANIFEST.org
+-rw-r--r--   0        0        0       99 2023-07-29 12:04:42.656318 matan-0.1.6/Makefile
+-rw-r--r--   0        0        0     3385 2023-07-29 12:04:42.660318 matan-0.1.6/README.md
+-rw-r--r--   0        0        0      638 2023-07-29 12:04:42.660318 matan-0.1.6/docs/Makefile
+-rw-r--r--   0        0        0      804 2023-07-29 12:04:42.660318 matan-0.1.6/docs/make.bat
+-rw-r--r--   0        0        0     3164 2023-07-29 12:04:42.660318 matan-0.1.6/docs/phinx-autogen
+-rw-r--r--   0        0        0   285099 2023-07-29 12:04:42.660318 matan-0.1.6/docs/source/_static/logo.png
+-rw-r--r--   0        0        0     1229 2023-07-29 12:04:42.660318 matan-0.1.6/docs/source/_templates/custom-module-template.rst
+-rw-r--r--   0        0        0       95 2023-07-29 12:04:42.660318 matan-0.1.6/docs/source/api.rst
+-rw-r--r--   0        0        0     1462 2023-07-29 12:04:42.660318 matan-0.1.6/docs/source/conf.py
+-rw-r--r--   0        0        0      103 2023-07-29 12:04:42.660318 matan-0.1.6/docs/source/examples.rst
+-rw-r--r--   0        0        0      267 2023-07-29 12:04:42.660318 matan-0.1.6/docs/source/future.rst
+-rw-r--r--   0        0        0       73 2023-07-29 12:04:42.660318 matan-0.1.6/docs/source/generated/matan.files.rst
+-rw-r--r--   0        0        0      192 2023-07-29 12:04:42.660318 matan-0.1.6/docs/source/generated/matan.rst
+-rw-r--r--   0        0        0      400 2023-07-29 12:04:42.660318 matan-0.1.6/docs/source/generated/matan.sample.rst
+-rw-r--r--   0        0        0     2104 2023-07-29 12:04:42.660318 matan-0.1.6/docs/source/index.rst
+-rw-r--r--   0        0        0      408 2023-07-29 12:04:42.660318 matan-0.1.6/docs/source/matan.rst
+-rw-r--r--   0        0        0       52 2023-07-29 12:04:42.660318 matan-0.1.6/docs/source/modules.rst
+-rw-r--r--   0        0        0     2561 2023-07-29 12:04:42.660318 matan-0.1.6/docs/source/usage.rst
+-rw-r--r--   0        0        0        0 2023-07-29 12:04:42.732318 matan-0.1.6/docs/source/whats_next.rst
+-rw-r--r--   0        0        0      388 2023-07-29 12:04:42.660318 matan-0.1.6/examples/composition.py
+-rw-r--r--   0        0        0       40 2023-07-29 12:04:42.660318 matan-0.1.6/examples/find_files.py
+-rw-r--r--   0        0        0       87 2023-07-29 12:04:42.660318 matan-0.1.6/examples/imp.py
+-rw-r--r--   0        0        0     2147 2023-07-29 12:04:42.660318 matan-0.1.6/examples/tensile_test.py
+-rw-r--r--   0        0        0      192 2023-07-29 12:04:42.660318 matan-0.1.6/is-uploaded.sh
+-rw-r--r--   0        0        0       87 2023-07-29 12:04:42.660318 matan-0.1.6/matan/__init__.py
+-rw-r--r--   0        0        0      168 2023-07-29 12:04:42.660318 matan-0.1.6/matan/_misc.py
+-rw-r--r--   0        0        0      300 2023-07-29 12:04:42.660318 matan-0.1.6/matan/fem/tensile/__init__.py
+-rw-r--r--   0        0        0     5191 2023-07-29 12:04:42.660318 matan-0.1.6/matan/files.py
+-rw-r--r--   0        0        0        0 2023-07-29 12:04:42.732318 matan-0.1.6/matan/polymers/__init__.py
+-rw-r--r--   0        0        0      812 2023-07-29 12:04:42.660318 matan-0.1.6/matan/polymers/charpy/__init__.py
+-rw-r--r--   0        0        0     2616 2023-07-29 12:04:42.660318 matan-0.1.6/matan/polymers/tensile/ISO527/__init__.py
+-rw-r--r--   0        0        0    12062 2023-07-29 12:04:42.664318 matan-0.1.6/matan/polymers/tensile/__init__.py
+-rw-r--r--   0        0        0       28 2023-07-29 12:04:42.664318 matan-0.1.6/matan/polymers/tensile/misc.py
+-rw-r--r--   0        0        0     7894 2023-07-29 12:04:42.664318 matan-0.1.6/matan/sample.py
+-rw-r--r--   0        0        0      340 2023-07-29 12:04:42.664318 matan-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      941 2023-07-29 12:04:42.664318 matan-0.1.6/setup.cfg
+-rw-r--r--   0        0        0      160 2023-07-29 12:04:42.664318 matan-0.1.6/tests/sample_project/__main__.py
+-rw-r--r--   0        0        0      224 1970-01-01 00:00:00.000000 matan-0.1.6/PKG-INFO
```

### Comparing `matan-0.1.5.2.9/LICENSE` & `matan-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `matan-0.1.5.2.9/README.md` & `matan-0.1.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,88 +1,89 @@
 **This package is still under development. Be aware of often updates!**
 # MaTan
 
-Shortcut comes from **Mat**erial **An**analysis - ultimately is should contains modules allowing user to calculate metals and polymers properties from tensile, HDT (polymers) and DSC tests, as well as the others. There are few similar  packages in PyPI, but none of them I found good to me, so I wrote new one. 
+Shortcut comes from **Mat**erial **An**analysis - ultimately is should contains modules allowing
+user to calculate metals and polymers properties from tensile, HDT (polymers) and DSC tests, as well
+as the others. There are few similar  packages in PyPI, but none of them I found good to me, so I
+wrote new one. 
 
 For now it includes:
 - ISO:527-1 (polymers analysis)
 
-# [Documentation](https://matan.codeberg.page)
-
+_**[Documentation](https://matan.codeberg.page)**_
 
 # Abstract
 
-Nowadays, Python is one of the most popular programming languages, even in non-informatics fields like mechanical engineering, due to its simplicity, and computer analysis solvers using FEM methods are part of almost all components, albeit access to material data is sometimes hard due to inadequate data in the datasheets, problems with calculations, inconsistent information, etc. To overcome this problem, the Python package was created, which allows to calculate the stress, strains, tensile modulus, and other properties from force and elongation data from a machine. For now, it includes only polymer tests according to the ISO-527-1 standard, but in the future, other standards should be included.
-
-Moreover, the package would need a graphical user interface, which could make it even simpler to use and, more importantly, allow users to upload their obtained results into OpenAccess databases and export plastic strains, tensile modulus, and other properties needed to perform FEM and other numerical analysis. That could make FEM methods even more accessible, which would lead to a decrease in the use of unnecessary materials and, due to this, less CO2 pollution.
+Nowadays, Python is one of the most popular programming languages, even in non-informatics fields
+like mechanical engineering, due to its simplicity, and computer analysis solvers using FEM methods
+are part of almost all components, albeit access to material data is sometimes hard due to
+inadequate data in the datasheets, problems with calculations, inconsistent information, etc. To
+overcome this problem, the Python package was created, which allows to calculate the stress,
+strains, tensile modulus, and other properties from force and elongation data from a machine. For
+now, it includes only polymer tests according to the ISO-527-1 standard, but in the future, other
+standards should be included.
+
+Moreover, the package would need a graphical user interface, which could make it even simpler to use
+and, more importantly, allow users to upload their obtained results into OpenAccess databases and
+export plastic strains, tensile modulus, and other properties needed to perform FEM and other
+numerical analysis. That could make FEM methods even more accessible, which would lead to a decrease
+in the use of unnecessary materials and, due to this, less CO2 pollution.
 
 
 # How to use it?
 
-Just simply put elongation and force arrays into sample
+Just simply put elongation and force arrays into sample.
 
-Be aware that sometimes csv files can have diffrent extension depends on machine manufacturer. To be sure just check it using simples notepad, or try to read it by pandas.
+Be aware that sometimes csv files can have diffrent extension depends on machine manufacturer. To be
+sure just check it using simples notepad, or try to read it by pandas.
 
 ```python
 import matan as mt
 import pandas as pd
 
 path_to_your_CSV = r"path/to/your/CSV"
 
-
-'''
-Be aware that somethimes some software machines uses diffrent encoding! Check the documentation of pandas.read_csv for more
-'''
+# BE AWARE
+# Somethimes some software machines uses diffrent encoding! Check the documentation of pandas.read_csv for more
 df = pd.read_csv(path_to_your_CSV)
 
 elongation_array=df["elongation"]
 force_array=df["force"]
 
 # This uses N ewtons and mm by default to ensure [N/mm^2] as it is equal to MPa
 # by default force units are Newtons and lenght units are mm
-example=mt.sample(name="your sample name",
-thickness = 5,
-width= 5,
-elongation_array=elongation_array,
-force_array=force_array
+example=mt.sample(
+    name="your sample name",
+    thickness = 5,
+    width= 5,
+    elongation_array=elongation_array,
+    force_array=force_array
 )
 
-
-
-
 #Use method below to convert engineering values into  real
 example.calculate_real_values()
 
 # tensile modulus values between engineering value and real value
-print(ext.eng_values.tensile_modulus,
-ext.real_values.tensile_modulus)
+print(ext.eng_values.tensile_modulus, ext.real_values.tensile_modulus)
+
+## Engineering values
 
-# Engineering values
 # Value of strenght
-print(ext.eng_values.strength.value,
-ext.eng_values.strength.strain)
+print(ext.eng_values.strength.value, ext.eng_values.strength.strain)
 
 # Values at break
-print(ext.eng_values.at_break.stress,
-ext.eng_values.at_break.strain)
+print(ext.eng_values.at_break.stress, ext.eng_values.at_break.strain)
 
 # Yield strenght values
-print(ext.eng_values.yield_strength.value,
-ext.eng_values.yield_strength.strain)
+print(ext.eng_values.yield_strength.value, ext.eng_values.yield_strength.strain)
+
+## Real values
 
-# Real values
 # Value of strenght
-print(ext.real_values.strength.value,
-ext.real_values.strength.strain)
+print(ext.real_values.strength.value, ext.real_values.strength.strain)
 
 # Values at break
-print(ext.real_values.at_break.stress,
-ext.real_values.at_break.strain)
+print(ext.real_values.at_break.stress, ext.real_values.at_break.strain)
 
 # Yield strenght values
-print(ext.real_values.yield_strength.value,
-ext.real_values.yield_strength.strain)
-
+print(ext.real_values.yield_strength.value, ext.real_values.yield_strength.strain)
 ```
-
-
-
```

### Comparing `matan-0.1.5.2.9/matan/files.py` & `matan-0.1.6/matan/files.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-import glob,os
+import glob, os
 import re
+
+
 class files:
     def __init(self):
         pass
-        
 
-    def find(self,path, extension:str,methods=None, mods=None):
+    def find(self, path, extension: str, methods=None, mods=None):
         """This class can manage the files as well as it's parameters
 
         This class helps managing he files, find their names/paths, extract the method of manufacturing or other
         parameters
 
         TODO: add automatically finding the method placement in names, by putting them in the method definition
-        
+
         Parameters
         ----------
         path : str
             This variable is used to put path to your files
         extension : str
             Extention is the extention of your files. If your file is .csv put csv in there, be aware and do not put the dot before your extention
         methods : str
@@ -26,39 +27,58 @@
         --------
         FIXME: Add docs.
 
         """
 
         methods = [method.upper() for method in methods]
         if extension.startswith("."):
-            extension=extension[1:]
-        
-        files=glob.glob(os.path.join(path, f"*.{extension}"))
+            extension = extension[1:]
+
+        files = glob.glob(os.path.join(path, f"*.{extension}"))
         # breakpoint()
         try:
-            self.files=[file for file in files if any(method in file for method in methods)] 
-            splitted = [os.path.split(file)[1] for file in self.files if any(method in file for method in methods)] #split to extract names
-            self.paths = [file for file in self.files if any(method in file for method in methods)]
+            self.files = [
+                file for file in files if any(method in file for method in methods)
+            ]
+            splitted = [
+                os.path.split(file)[1]
+                for file in self.files
+                if any(method in file for method in methods)
+            ]  # split to extract names
+            self.paths = [
+                file for file in self.files if any(method in file for method in methods)
+            ]
         except TypeError:
-            self.files=[file for file in self.files if any(method in file for method in methods)] 
-            splitted = [os.path.split(file)[1] for file in self.files if any(method in file for method in methods)]
+            self.files = [
+                file for file in self.files if any(method in file for method in methods)
+            ]
+            splitted = [
+                os.path.split(file)[1]
+                for file in self.files
+                if any(method in file for method in methods)
+            ]
             self.paths = [file for file in self.files]
-        self.names = [name.split(".")[0] for name  in splitted]
-        numbers = [name.split("_")[1] for name  in splitted]
-        self.numbers=[os.path.splitext(number)[0] for number in numbers]
-        self.comments= [self.find_comments(name)[0] for name in self.names]
-        self.clean_names=[self.find_comments(name)[1] for name in self.names]
+        self.names = [name.split(".")[0] for name in splitted]
+        numbers = [name.split("_")[1] for name in splitted]
+        self.numbers = [os.path.splitext(number)[0] for number in numbers]
+        self.comments = [self.find_comments(name)[0] for name in self.names]
+        self.clean_names = [self.find_comments(name)[1] for name in self.names]
         if methods is not None:
-            self.methods = [self.find_method(name, methods) for name in self.names ] #thats for
+            self.methods = [
+                self.find_method(name, methods) for name in self.names
+            ]  # thats for
         if mods is not None:
-            self.modifications = [self.find_modification(name, mods) for name in self.names]
-        self.composition=[self.find_composition(name.split("_")[0]) for name in self.names]
-    def find_method(self,name:str,
-                    methods:list,
-                    delimiter:str='-', ):
+            self.modifications = [
+                self.find_modification(name, mods) for name in self.names
+            ]
+        self.composition = [
+            self.find_composition(name.split("_")[0]) for name in self.names
+        ]
+
+    def find_method(self, name: str, delimiter: str = "-", placement: int = 0):
         """Find the technique how the material was created
 
         Find the method how the material was created, what methods were used to modify it, etc. To do so it is using
         first letters of filename, so for extruded parts you can use EXT, for annealed extruded parts you can use aEXT
         etc.
 
         Parameters
@@ -69,57 +89,56 @@
             what sign you wanna use to finish your method string. By default it is -
 
         Examples
         --------
         FIXME: Add docs.
 
         """
-        name=name.split(delimiter)[0]
-        for method in methods:
-            if method in name:
-                return method
-
-    
-    def find_modification(self, name, mods:list, place=0):
-        if not  isinstance(mods, list):
+        return name.split(delimiter)[0]
+
+    def find_modification(self, name, mods: list, place=0):
+        if not isinstance(mods, list):
             raise ValueError("Put list of modifications!")
         for mod in mods:
             letter = mod[0]
-            if name[place]==letter:
+            if name[place] == letter:
                 return mod
             else:
                 continue
         return None
-    
-    def find_composition(name,delimiter: str='-', percent_sign="p"):
+
+    def find_composition(name, delimiter: str = "-", percent_sign="p"):
         """
         TODODO baby shark
         method to obtain material ingridiens from name, as I usually name files extracted from machine with code allowing me to get that information from filename
         """
         # breakpoint()
-        splitted=name.split(delimiter)
-        comp={}
+        splitted = name.split(delimiter)
+        comp = {}
         for name in splitted[1:]:
             comp.update(_extract_info(name, percent_sign))
         return comp
 
-
-
-
-    def find_comments(self,s):
-
-        pattern = r'\[.*?\]'  # a regular expression pattern to match text between square brackets
-        matches = re.findall(pattern, s)  # find all matches of the pattern in the string
-        comments = ''.join(matches)  # concatenate all the matches into a single string
-        cleaned_text = re.sub(pattern, '', s)  # remove all the matches from the original string
-        comments = re.sub(r'[\[\]]', '', comments)  # remove square brackets from the removed text
+    def find_comments(self, s):
+        pattern = r"\[.*?\]"  # a regular expression pattern to match text between square brackets
+        matches = re.findall(
+            pattern, s
+        )  # find all matches of the pattern in the string
+        comments = "".join(matches)  # concatenate all the matches into a single string
+        cleaned_text = re.sub(
+            pattern, "", s
+        )  # remove all the matches from the original string
+        comments = re.sub(
+            r"[\[\]]", "", comments
+        )  # remove square brackets from the removed text
         return comments, cleaned_text
 
+
 def _extract_info(s, delimiter="p"):
-    pattern = rf'(\d+){delimiter}(.+)'
+    pattern = rf"(\d+){delimiter}(.+)"
     match = re.match(pattern, s)
     result = {}
     if match:
         result[match.group(2)] = [int(match.group(1))]
     # else:
     #     return None
-    return result    
+    return result
```

### Comparing `matan-0.1.5.2.9/matan/polymers/charpy/__init__.py` & `matan-0.1.6/matan/polymers/charpy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 class simple_charpy:
     def __init__(self, corrected_energy: float, thickness: float, width: float):
-        """Class for calculating the non-instrumented Charpy impact strength. 
+        """Class for calculating the non-instrumented Charpy impact strength.
 
         In general by using this class you can calculate both notched and unnotched samples. For notched you need to put
         remained width on notch place.
 
         For now it is only for non-instrumented tests
 
         Parameters
@@ -17,9 +17,9 @@
             width of the test specimen
 
         Examples
         --------
         FIXME: Add docs.
 
         """
-        
-        self.impact_strength=(corrected_energy)/(thickness*width)
+
+        self.impact_strength = (corrected_energy) / (thickness * width)
```

### Comparing `matan-0.1.5.2.9/matan/polymers/tensile/ISO527/__init__.py` & `matan-0.1.6/matan/polymers/tensile/ISO527/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,76 +1,72 @@
 import numpy as np
 from .... import _misc
 
 
 """
 According to ISO 527-1: https://cdn.standards.iteh.ai/samples/75824/61c480ef4bf0494aa6966bd4c2244c2e/ISO-527-1-2019.pdf
 """
+
+
 class tensile_modulus:
-    def __init__(self,
-                 stress,
-                 strain,
-                 percent_strain=False,
-                 lower_limit=0.05,
-                 upper_limit=0.25
-                 ):
+    def __init__(
+        self, stress, strain, percent_strain=False, lower_limit=0.05, upper_limit=0.25
+    ):
         """
         Tensile, or Young's modulus is the slope of strain/stress curve, between strains equals to 0.05 and 0.25 percent
         """
-        stress=np.array(stress)
-        strain=np.array(strain)
-        if not percent_strain:
-            strain=strain*100
-        module_strain=strain[(strain>lower_limit) & (strain<upper_limit)]
-        low_idx = np.where(strain==min(module_strain))[0][0]
-        upp_idx = np.where(strain==max(module_strain))[0][0]
-        module_stress = stress[low_idx:upp_idx+1]
+        stress = np.array(stress)
+        strain = np.array(strain)
         if not percent_strain:
-            module_strain=module_strain/100
+            upper_limit = upper_limit / 100
+            lower_limit = lower_limit / 100
+        module_strain = strain[(strain > lower_limit) & (strain < upper_limit)]
+
+        low_idx = np.where(strain == min(module_strain))[0][0]
+        upp_idx = np.where(strain == max(module_strain))[0][0]
+        module_stress = stress[low_idx : upp_idx + 1]
         array = np.vstack([module_strain, np.ones(len(module_strain))]).T
 
         E, c = np.linalg.lstsq(array, module_stress, rcond=-1)[0]
         r2 = 1 - c / (module_stress.size * module_stress.var())
-        self.r2 = round(r2,4)
-        self.tensile_modulus=_misc._round_sig(E, sig=3)
-        self.module_strain, self.module_stress =module_strain, module_stress
+        self.r2 = round(r2, 4)
+        self.tensile_modulus = _misc._round_sig(E, sig=3)
+        self.module_strain, self.module_stress = module_strain, module_stress
 
 
 class at_break:
     def __init__(self, stress, strain):
-        self.stress=_misc._round_sig(stress[len(stress)-1], sig=3)
-        self.strain=_misc._round_sig(strain[len(strain)-1])
-        
+        self.stress = _misc._round_sig(stress[len(stress) - 1], sig=3)
+        self.strain = _misc._round_sig(strain[len(strain) - 1])
+
+
 class strenght:
     def __init__(self, stress, strain):
-        self.value=_misc._round_sig(self.find_local_maximum(stress), sig=3)
-        self.strain=_misc._round_sig(strain[self.idx])
+        self.value = _misc._round_sig(self.find_local_maximum(stress), sig=3)
+        self.strain = _misc._round_sig(strain[self.idx])
+
     def find_local_maximum(self, stress):
-        for i in range(1, len(stress)-1):
-            if stress[i-1] < stress[i] > stress[i+1] and stress[i]>1:
-                self.idx=i
-                return  stress[i]
+        for i in range(1, len(stress) - 1):
+            if stress[i - 1] < stress[i] > stress[i + 1] and stress[i] > 1:
+                self.idx = i
+                return stress[i]
 
         print("Strength: Local maximum not found, gives max value")
-        self.idx=np.where(stress==np.max(stress))[0][0]
+        self.idx = np.where(stress == np.max(stress))[0][0]
         val = np.max(stress)
         return val
-                
+
 
 class yield_strenght:
-    def __init__(self,stress, strain):
-        self.value=_misc._round_sig(stress[self.find_idx(stress,strain)], sig=3)
-        self.strain=_misc._round_sig(strain[self.find_idx(stress,strain)])
-    def find_idx(self, stress,strain):
+    def __init__(self, stress, strain):
+        self.value = _misc._round_sig(stress[self.find_idx(stress, strain)], sig=3)
+        self.strain = _misc._round_sig(strain[self.find_idx(stress, strain)])
+
+    def find_idx(self, stress, strain):
         for i in range(1, len(strain)):
-            if strain[i] > strain[i-1] and stress[i] <= stress[i-1]:
-                if stress[i]>1:
+            if strain[i] > strain[i - 1] and stress[i] <= stress[i - 1]:
+                if stress[i] > 1:
                     return i
                 else:
                     continue
                     # exit()
-        return len(strain)-1
-
-        
-
-        
-            
+        return len(strain) - 1
```

### Comparing `matan-0.1.5.2.9/matan/polymers/tensile/__init__.py` & `matan-0.1.6/matan/polymers/tensile/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,355 +1,354 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from typing import Union
 import importlib
 
 
-
 class _engineering_values:
-        def __init__(self,
-                     width,
-                     thickness,
-                     name=None,
-                     elongation_array: Union[list, np.array] =None,
-                     force_array: Union[list, np.array] =None,
-                     force_units="N",
-                     length_units="mm",
-                   norm="ISO527"
-                     ):
-            global properties
-            properties = importlib.import_module(f".{norm}", package=__package__)
-            """initializer of engineering values class
+    def __init__(
+        self,
+        width: float,
+        thickness: float,
+        initial_length: Union[float, int] = None,
+        name=None,
+        elongation_array: Union[list, np.array] = None,
+        force_array: Union[list, np.array] = None,
+        force_units="N",
+        length_units="mm",
+        norm="ISO527",
+    ):
+        global properties
+        properties = importlib.import_module(f".{norm}", package=__package__)
+        """initializer of engineering values class
 
             This class is used to menage the properties of engineering values
 
             Parameters
             ----------
             name : str
                 name for your sample
 
             Examples
             --------
             FIXME: Add docs.
 
             """
-            
-            self.name=name
-            self.force_units = force_units
-            self.length_units=length_units
-            self.thickness=thickness,
-            self.width=width
-            self.stress, self.strain=None,None
-        def _calculate(self,
-                      thickness:float,
-                      width:float,
-                      elongation_array,
-                      force_array,
-                      ):
-            """Calculates the engineering stress and strain
 
-            This method is used to calculate engineering stress and strain from height
+        self.name = name
+        self.force_units = force_units
+        self.length_units = length_units
+        self.thickness = (thickness,)
+        self.width = width
+        self.stress, self.strain = None, None
+
+    def _calculate(
+        self,
+        thickness: float,
+        width: float,
+        initial_length: float,
+        elongation_array,
+        force_array,
+    ):
+        """Calculates the engineering stress and strain
+
+        This method is used to calculate engineering stress and strain from height
+
+        Parameters
+        ----------
+        thickness : float
+            smaller initial dimension of the rectangular cross-section in the central part of test specimen
+        width : float
+            larger initial dimension of the rectangular cross-section in the central part of the test specimen
+        elongation_array : list
+            list of the sample elongation
+        force_array : list
+            list of the forces from the machinge
+        force_units : str
+            Units used as force units. Newtons [N] by default. Use shorten strings, as it is used in output
+        length : str
+            Units used for lenght, mm by default. Use short strings, as they are used in output. If you wanna use percent, just use % sign or percent
+        """
+        elongation_array = [(elon / initial_length) for elon in elongation_array]
 
-            Parameters
-            ----------
-            thickness : float
-                smaller initial dimension of the rectangular cross-section in the central part of test specimen
-            width : float
-                larger initial dimension of the rectangular cross-section in the central part of the test specimen
-            elongation_array : list
-                list of the sample elongation
-            force_array : list
-                list of the forces from the machinge
-            force_units : str
-                Units used as force units. Newtons [N] by default. Use shorten strings, as it is used in output
-            length : str
-                Units used for lenght, mm by default. Use short strings, as they are used in output. If you wanna use percent, just use % sign or percent
-            """
-            
+        if self.length_units == "%" or self.length_units == "percent":
+            self.percent_strain = True
+        else:
+            self.percent_strain = False
 
-            if self.length_units=="%" or self.length_units=="percent":
-                self.percent_strain=True
+        # breakpoint()
+        if self.stress is None and self.strain is None:
+            initial_area = thickness * width
+            self.stress = [force / initial_area for force in force_array]
+            if self.percent_strain:
+                self.strain = [strain * 100 for strain in elongation_array]
             else:
-                self.percent_strain=False
+                self.strain = [strain for strain in elongation_array]
 
+        self.strength = self._calculate_strength(self.stress, self.strain)
 
-            if  self.stress is  None and self.strain is None:
-                initial_area=thickness*width
-                self.stress=[force/initial_area for force in force_array]
-                if self.percent_strain:
-                    self.strain=[strain for strain in elongation_array]
-                else:
-                    self.strain=[strain*0.01 for strain in elongation_array]
-
-            self.strength=self._calculate_strength(self.stress,
-                                                  self.strain)
-            
-            self.at_break=self._calculate_at_break(self.strain,
-                                                  self.stress)
-            
-            self.yield_strength=self._calculate_yield_strength(self.stress,
-                                                              self.strain)
-            self.tensile_modulus=self._calculate_tensile_modulus()
-
-        class _calculate_strength:
-            def __init__(self,strain: np.array,stress:np.array):
-                """Strenght is according to ISO-527-1 first maximum local value
-
-                Parameters
-                ----------
-                strain : np.array
-                    strain array
-                stress : np.array
-                    stress array
-
-                Examples
-                --------
-                FIXME: Add docs.
-
-                """
-                
-                strength = properties.strenght(strain,stress)
-                self.value=strength.value
-                self.strain=strength.strain
-
-        class _calculate_yield_strength:
-            def __init__(self, stress: np.array, strain: np.array):
-                """
-                Yield strenght  is according to ISO-527-1 strain increase without stress increase. 
-
-                Parameters
-                ----------
-                stress : np.array
-                    stress numpy array
-                strain : np.array
-                    strain numpy array
-
-                Examples
-                --------
-                FIXME: Add docs.
-
-                """
-                yield_strenght=properties.yield_strenght(stress, strain)
-                self.stress, self.strain=yield_strenght.value,yield_strenght.strain
-        class _calculate_at_break:
-            """
-            This class calculates values at the brain according to ISO 527-1
-            """
-            def __init__(self,stress, strain):
-                at_break=properties.at_break(stress, strain)
-                self.stress=at_break.stress
-                self.strain=at_break.strain
+        self.at_break = self._calculate_at_break(self.strain, self.stress)
 
+        self.yield_strength = self._calculate_yield_strength(self.stress, self.strain)
+        self.tensile_modulus = self._calculate_tensile_modulus()
 
-        def _calculate_tensile_modulus(self,
-                                      plot=False,
-                                      r2=True,
-                                      output=False,
-                                      lower_limit=0.05,
-                                      upper_limit=0.25
-                                      ):
-            """            Tensile, or Young's modulus is the slope of strain/stress curve, between strains equals to 0.05 and 0.25 percent according to DIN ISO 527-1
+    class _calculate_strength:
+        def __init__(self, strain: np.array, stress: np.array):
+            """Strenght is according to ISO-527-1 first maximum local value
 
             Parameters
             ----------
-            plot : bool
-                Put True for use pyplot on the tensile modulus part
-            r2 : Put coeffitient 	of determination into pyplot label
-                Put coeffitient of determination into pyplot label
-            output : bool
-                Print the output of this method
-            lower_limit : float
-                lower limit of the measurement boundary
-            upper_limit : float
-                upper limit of the measurement boundary
+            strain : np.array
+                strain array
+            stress : np.array
+                stress array
 
             Examples
             --------
             FIXME: Add docs.
 
             """
 
-            E=properties.tensile_modulus(self.stress,
-                                         self.strain,
-                                         percent_strain=self.percent_strain
-                                         )
-            if plot:
-                label=rf"Young's modulus {int(E.tensile_modulus)} $\left[\frac{{{self.force_units}}}{{{self.length}^2}}\right]$"
-                if r2:
-                    label+="\n"+rf"$R^{{{2}}}={E.r2}$"
-                    plt.plot(E.module_strain,
-                             E.module_stress,
-                             label=label
-                             )
-            if output:
-                print(f"Tensile modulus is equal to {int(E.tensile_modulus)} [{self.force_units}/{self.length}^2]")
-            return   E.tensile_modulus
-
-                
-        def set(self,
-                engineering_stress: Union[list, np.array] =None,
-                engineering_strain:Union[list, np.array] =None,
-                # TODO: gives TypeError: only size-1 arrays can be converted to Python scalars while using numpy array
-                # TODO: gives KeyKerrr None
-                # TODO: in general this method does not work yet!
-                ):
-            """Method to set engineering stress and engineering strain
+            strength = properties.strenght(strain, stress)
+            self.value = strength.value
+            self.strain = strength.strain
+
+    class _calculate_yield_strength:
+        def __init__(self, stress: np.array, strain: np.array):
+            """
+            Yield strenght  is according to ISO-527-1 strain increase without stress increase.
 
             Parameters
             ----------
-            engineering_stress : list
-                array of engineering stress
-            engineering_strain : list
-                array of engineering strain
+            stress : np.array
+                stress numpy array
+            strain : np.array
+                strain numpy array
 
             Examples
             --------
             FIXME: Add docs.
 
             """
-            
-            self.stress, self.strain=engineering_stress, engineering_strain
-            self._calculate(thickness=self.thickness,
-                           width=self.width,
-                           elongation_array=None,
-                           force_array=None)
-            
+            yield_strenght = properties.yield_strenght(stress, strain)
+            self.stress, self.strain = yield_strenght.value, yield_strenght.strain
 
-        def plot(self, show=False):
-            """Method for plotting the results
+    class _calculate_at_break:
+        """
+        This class calculates values at the brain according to ISO 527-1
+        """
+
+        def __init__(self, stress, strain):
+            at_break = properties.at_break(stress, strain)
+            self.stress = at_break.stress
+            self.strain = at_break.strain
+
+    def _calculate_tensile_modulus(
+        self, plot=False, r2=True, output=False, lower_limit=0.05, upper_limit=0.25
+    ):
+        """Tensile, or Young's modulus is the slope of strain/stress curve, between strains equals to 0.05 and 0.25 percent according to DIN ISO 527-1
+
+        Parameters
+        ----------
+        plot : bool
+            Put True for use pyplot on the tensile modulus part
+        r2 : Put coeffitient 	of determination into pyplot label
+            Put coeffitient of determination into pyplot label
+        output : bool
+            Print the output of this method
+        lower_limit : float
+            lower limit of the measurement boundary
+        upper_limit : float
+            upper limit of the measurement boundary
+
+        Examples
+        --------
+        FIXME: Add docs.
 
-            This method can be used to plot your engineering stress-strain curve. If you wanna show it instantly use
-            parameter show as True
-
-            Parameters
-            ----------
-            show : bool
-                It it equal to matplotlib.pyplot function show
-
-            Examples
-            --------
-            FIXME: Add docs.
+        """
 
-            """
-            plt.plot(self.strain,self.stress, label=self.name)
-            plt.title(self.name)
-            plt.ylabel(rf"Stress $\left[\frac{{{self.force_units}}}{{{self.length_units}^2}}\right]$")
-            plt.xlabel(f"Strain [{self.length_units}]")
-            plt.legend()
-            if show:
-                plt.show()
+        E = properties.tensile_modulus(
+            self.stress, self.strain, percent_strain=self.percent_strain
+        )
+        if plot:
+            label = rf"Young's modulus {int(E.tensile_modulus)} $\left[\frac{{{self.force_units}}}{{{self.length}^2}}\right]$"
+            if r2:
+                label += "\n" + rf"$R^{{{2}}}={E.r2}$"
+                plt.plot(E.module_strain, E.module_stress, label=label)
+        if output:
+            print(
+                f"Tensile modulus is equal to {int(E.tensile_modulus)} [{self.force_units}/{self.length}^2]"
+            )
+        return E.tensile_modulus
+
+    def set(
+        self,
+        engineering_stress: Union[list, np.array] = None,
+        engineering_strain: Union[list, np.array] = None,
+        # TODO: gives TypeError: only size-1 arrays can be converted to Python scalars while using numpy array
+        # TODO: gives KeyKerrr None
+        # TODO: in general this method does not work yet!
+    ):
+        """Method to set engineering stress and engineering strain
+
+        Parameters
+        ----------
+        engineering_stress : list
+            array of engineering stress
+        engineering_strain : list
+            array of engineering strain
+
+        Examples
+        --------
+        FIXME: Add docs.
+
+        """
+
+        self.stress, self.strain = engineering_stress, engineering_strain
+        self._calculate(
+            thickness=self.thickness,
+            width=self.width,
+            elongation_array=None,
+            force_array=None,
+        )
 
-class _real_values(_engineering_values):
+    def plot(self, show=False):
+        """Method for plotting the results
 
-        def __init__(self,
-                     name,
-                     thickness,
-                     width,
-                     stress,
-                     strain,
-                     force_units,
-                     length_units,
-                     ):
-            self.force_units=force_units
-            self.length_units=length_units
-            if length_units=="%" or length_units=="percent":
-                self.percent_strain=True
-            else:
-                self.percent_strain=False
+        This method can be used to plot your engineering stress-strain curve. If you wanna show it instantly use
+        parameter show as True
 
-    
-            _engineering_values.__init__(self,
-                                        name=name,
-                                        thickness=thickness,
-                                        width=width
-                                        )
-            self.name=name + " [real]"
-            width=self.width
-            thickness=self.thickness
-            super().__init__(self,
-                             name=self.name,
-                             thickness=self.thickness
-                             )
-            self._calculate(stress, strain)
+        Parameters
+        ----------
+        show : bool
+            It it equal to matplotlib.pyplot function show
+
+        Examples
+        --------
+        FIXME: Add docs.
+
+        """
+        plt.plot(self.strain, self.stress, label=self.name)
+        plt.title(self.name)
+        lu = self.length_units
+        if "%" in lu:
+            lu = rf"\{lu}"
+        plt.ylabel(rf"Stress $\left[\frac{{{self.force_units}}}{{{lu}^2}}\right]$")
+        plt.xlabel(f"Strain [{lu}]")
+        plt.legend()
+        if show:
+            plt.show()
 
-        def _calculate(self, stress, strain):
-            """
-                Calculates the true stress and strain, from engineering values.
-                Read more there:
-                        https://courses.ansys.com/index.php/courses/topics-in-metal-plasticity/lessons/how-to-define-a-multilinear-hardening-plasticity-model-lesson-1/
-            
-                Parameters:
-                        strain (array-like): An array of strain values.
-                        stress (array-like): An array of corresponding stress values.
-                        n: An count of chunks to divide stress/strain array
-            
-                Returns:
-                    A tuple (start_strain, end_strain) representing the proportional range of the stress-strain curve.
-            """
-            self.stress=[stress_val*(1+strain_val) for stress_val, strain_val in zip(stress, strain)]
-            self.strain=[np.log(1+strain_val) for strain_val in strain]
 
-            self.strength=self._calculate_strength(self.stress,
-                                                  self.strain)
-            
-            self.at_break=self._calculate_at_break(self.strain,
-                                                  self.stress)
-            
-            self.yield_strength=self._calculate_yield_strength(self.stress,
-                                                              self.strain)
-            self.tensile_modulus=self._calculate_tensile_modulus()            
+class _real_values(_engineering_values):
+    def __init__(
+        self,
+        name,
+        thickness,
+        width,
+        stress,
+        strain,
+        force_units,
+        length_units,
+    ):
+        self.force_units = force_units
+        self.length_units = length_units
+        if length_units == "%" or length_units == "percent":
+            self.percent_strain = True
+        else:
+            self.percent_strain = False
 
+        _engineering_values.__init__(self, name=name, thickness=thickness, width=width)
+        self.name = name + " [real]"
+        width = self.width
+        thickness = self.thickness
+        super().__init__(self, name=self.name, thickness=self.thickness)
+        self._calculate(stress, strain)
+
+    def _calculate(self, stress, strain):
+        """
+        Calculates the true stress and strain, from engineering values.
+        Read more there:
+                https://courses.ansys.com/index.php/courses/topics-in-metal-plasticity/lessons/how-to-define-a-multilinear-hardening-plasticity-model-lesson-1/
+
+        Parameters:
+                strain (array-like): An array of strain values.
+                stress (array-like): An array of corresponding stress values.
+                n: An count of chunks to divide stress/strain array
+
+        Returns:
+            A tuple (start_strain, end_strain) representing the proportional range of the stress-strain curve.
+        """
+        self.stress = [
+            stress_val * (1 + strain_val)
+            for stress_val, strain_val in zip(stress, strain)
+        ]
+        self.strain = [np.log(1 + strain_val) for strain_val in strain]
 
+        self.strength = self._calculate_strength(self.stress, self.strain)
 
+        self.at_break = self._calculate_at_break(self.strain, self.stress)
 
+        self.yield_strength = self._calculate_yield_strength(self.stress, self.strain)
+        self.tensile_modulus = self._calculate_tensile_modulus()
 
 
 class _tensile:
-    
-    def __init__(self,
-                 name: str,
-                 thickness: Union[float, int],
-                 width: Union[float, int],
-                 elongation_array: Union[list, np.array] = None,
-                 force_array: Union[list, np.array] = None,
-                 stress_array: Union[list, np.array] = None,
-                 strain_array: Union[list, np.array] = None,
-                 force_units: str = "N",
-                 length_units: str = "mm"
-                 ):
-        self.name, self.thickness, self.width=name, thickness, width
+    def __init__(
+        self,
+        name: str,
+        thickness: Union[float, int],
+        width: Union[float, int],
+        initial_length: Union[float, int] = None,
+        elongation_array: Union[list, np.array] = None,
+        force_array: Union[list, np.array] = None,
+        stress_array: Union[list, np.array] = None,
+        strain_array: Union[list, np.array] = None,
+        force_units: str = "N",
+        length_units: str = "mm",
+    ):
+        self.name, self.thickness, self.width = name, thickness, width
         self.engineering_values = _engineering_values(
             width=width,
             thickness=thickness,
+            initial_length=initial_length,
             name=name,
             elongation_array=elongation_array,
             force_array=force_array,
             force_units=force_units,
-            length_units=length_units
+            length_units=length_units,
         )
         self.force_units, self.length_units = force_units, length_units
         self.stress_units = f"{force_units}/{length_units}^2"
         self.strain_units = f"{length_units}/{length_units}"
         if stress_array is None and strain_array is None:
             if elongation_array is None and force_array is None:
-                raise ValueError("None of elongation/force or stress/strain arrays are defined!")
+                raise ValueError(
+                    "None of elongation/force or stress/strain arrays are defined!"
+                )
             elif thickness is None:
                 raise ValueError("Thickness is not defined!")
             elif width is None:
                 raise ValueError("Width is not defined!")
             else:
                 self.elongation_array = elongation_array
                 self.force_array = force_array
-                self.engineering_values._calculate(thickness, width, elongation_array, force_array)
+                self.engineering_values._calculate(
+                    thickness=thickness,
+                    width=width,
+                    initial_length=initial_length,
+                    elongation_array=elongation_array,
+                    force_array=force_array,
+                )
         else:
             self.engineering_values.set(stress_array, strain_array)
 
     def convert2real(self):
-        self.real_values = _real_values(self.name,
-                                        self.thickness,
-                                        self.width,
-                                        self.engineering_values.stress,
-                                        self.engineering_values.strain,
-                                        self.force_units,
-                                        self.length_units)
-
-
+        self.real_values = _real_values(
+            self.name,
+            self.thickness,
+            self.width,
+            self.engineering_values.stress,
+            self.engineering_values.strain,
+            self.force_units,
+            self.length_units,
+        )
```

### Comparing `matan-0.1.5.2.9/matan/sample.py` & `matan-0.1.6/matan/sample.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,159 +27,164 @@
         ----------
         name : str
         name of your sample for example "Neat PLA"
         manufactured_method : str
         how your sample was made, etc. by FDM or injection method, just for description
         comments : str
         any comments describing your sample
-    
+
     Examples
         --------
         elongation_array=df["elongation"]
         force_array=df["force"]
 
         # This uses N ewtons and mm by default to ensure [N/mm^2] as it is equal to MPa
         example=mt.sample(name="your sample name",
         thickness = 5,
         width= 5,
         elongation_array=elongation_array,
         force_array=force_array
         )
+    """
+
+    def __init__(
+        self,
+        name: str,
+        comments: str = None,
+        path: str = None,
+        manufactured_method: str = None,
+    ):
+        self.name = name
+        self.comments = comments
+
+    def define_tensile_test(
+        self,
+        thickness: float = None,
+        width: float = None,
+        initial_length: Union[float, int] = None,
+        elongation_array: Union[list, np.array] = None,
+        force_array: Union[list, np.array] = None,
+        stress_array: Union[list, np.array] = None,
+        strain_array: Union[list, np.array] = None,
+        force_units: str = "N",
+        length_units: str = "mm",
+        material="polymers",
+        norm="ISO527",
+    ):
         """
 
-    def __init__(self,name: str,
-                 comments: str=None,
-                 path: str= None,
-                 manufactured_method: str=None):
-            self.name=name
-            self.comments=comments
-        
-    def define_tensile_test(self,
-                            thickness:float = None,
-                            width:float = None,
-                            elongation_array: Union[list, np.array] =None,
-                            force_array: Union[list, np.array] =None,
-                            stress_array: Union[list, np.array] =None,
-                            strain_array: Union[list, np.array] =None,
-                            force_units: str="N",
-                            length_units: str="mm",
-                            material="polymers",
-                            norm="ISO527"):
-            """
+        That's function to calculate tensile test parameters
 
-    That's function to calculate tensile test parameters
+        Parameters
+            ----------
+            thickness : float
+            thickness of your sample
+            width : float
+            width of your sample
+            elongation_array : Union[list, np.array]
+            elongation array from your tensile machine
+            force_array : Union[list, np.array]
+            forces obtained from your tensile machine
+            stress_array : Union[list, np.array]
+            calculated stresses
+            strain_array : Union[list, np.array]
+            calculated strains
+            force_units : str
+            force units of your force array
+            lenght_units : str
+            length units of your force array
+
+        Raises
+            ------
+            ValueError
+            Raises ValueError while stress/strains or width/thickness are not defined
 
-    Parameters
-        ----------
-        thickness : float
-        thickness of your sample
-        width : float
-        width of your sample
-        elongation_array : Union[list, np.array]
-        elongation array from your tensile machine
-        force_array : Union[list, np.array]
-        forces obtained from your tensile machine
-        stress_array : Union[list, np.array]
-        calculated stresses
-        strain_array : Union[list, np.array]
-        calculated strains
-        force_units : str
-        force units of your force array
-        lenght_units : str
-        length units of your force array
-
-    Raises
-        ------
-        ValueError
-        Raises ValueError while stress/strains or width/thickness are not defined
-    
-    Examples
-        --------
-        elongation_array=df["elongation"]
-        force_array=df["force"]
+        Examples
+            --------
+            elongation_array=df["elongation"]
+            force_array=df["force"]
 
-        # This uses N ewtons and mm by default to ensure [N/mm^2] as it is equal to MPa
-        example=mt.sample(name="your sample name",
-        thickness = 5,
-        width= 5,
-        elongation_array=elongation_array,
-        force_array=force_array
-        )
+            # This uses N ewtons and mm by default to ensure [N/mm^2] as it is equal to MPa
+            example=mt.sample(name="your sample name",
+            thickness = 5,
+            width= 5,
+            elongation_array=elongation_array,
+            force_array=force_array
+            )
         """
 
-            self._test = importlib.import_module(".polymers.tensile", package=__package__)
-            
-            self.thickness, self.width= thickness,width
-            self.tensile=self._test._tensile(name=self.name,
-                                        elongation_array=elongation_array,
-                                        force_array=force_array,
-                                        force_units=force_units,
-                                        length_units=length_units,
-                                        stress_array=stress_array,
-                                        strain_array=strain_array,
-                                        thickness=thickness,
-                                        width=width
-                                        )
+        self._test = importlib.import_module(".polymers.tensile", package=__package__)
 
+        self.thickness, self.width = thickness, width
+        self.tensile = self._test._tensile(
+            name=self.name,
+            elongation_array=elongation_array,
+            initial_length=initial_length,
+            force_array=force_array,
+            force_units=force_units,
+            length_units=length_units,
+            stress_array=stress_array,
+            strain_array=strain_array,
+            thickness=thickness,
+            width=width,
+        )
 
     def calculate_real_values(self):
-        print(dir(self.tensile))
         # exit()
-        self.real_vals=self.tensile.convert2real()
+        self.real_vals = self.tensile.convert2real()
         # self.real_vals.calculate(self.eng_values.stress,
-        #                            self.eng_values.strain)            
+        #                            self.eng_values.strain)
+
     def plot(self, show=False):
         """Method for plotting the results
 
-            This method can be used to plot your engineering stress-strain curve. If you wanna show it instantly use
-            parameter show as True
+        This method can be used to plot your engineering stress-strain curve. If you wanna show it instantly use
+        parameter show as True
 
-            Parameters
-            ----------
-            show : bool
-                It it equal to matplotlib.pyplot function show
+        Parameters
+        ----------
+        show : bool
+            It it equal to matplotlib.pyplot function show
 
-            Examples
-            --------
-            FIXME: Add docs.
+        Examples
+        --------
+        FIXME: Add docs.
 
-            """
-        plt.plot(self.elongation_array,self.force_array, label=self.name)
+        """
+        plt.plot(self.elongation_array, self.force_array, label=self.name)
         plt.title(self.name)
         plt.ylabel(f"Force [{self.force_units}]")
         plt.xlabel(f"Strain [{self.lenght_units}]")
         plt.legend()
         if show:
-                plt.show()        
-
+            plt.show()
 
-                
-        
-    def composition_from_name(self, delimiter: str='-', percent_sign="p"):
+    def composition_from_name(self, delimiter: str = "-", percent_sign="p"):
         """Method to obtain material ingridiens from name, as I usually name files extracted from machine with code allowing me to get that information from filename. For example you can name you sample 10pFDM-20pPET, and it will mean there is 20percent of addition PET as well as 10 percent of Polyolefin Elastometer addition. It can be also 90pPC-10pPET.
-        Parameters:
-        delimiter: str
-            It is the sign that delimits your composition, in default it is - sign.
-        percent_sign: str
-            It is the sign takes everything before as percent, like in example 90pPC, so int before (90) will be int in your composition.
-        
-    Returns: 
-            Sets the composition variable into a dicts of your composition. For example from 90pPC-10pPET it will return a dict {PC: 90, PET: 10}
+            Parameters:
+            delimiter: str
+                It is the sign that delimits your composition, in default it is - sign.
+            percent_sign: str
+                It is the sign takes everything before as percent, like in example 90pPC, so int before (90) will be int in your composition.
+
+        Returns:
+                Sets the composition variable into a dicts of your composition. For example from 90pPC-10pPET it will return a dict {PC: 90, PET: 10}
         """
-        
+
         from .files import files
-        name=self.name
+
+        name = self.name
         self.composition = files.find_composition(name, delimiter, percent_sign)
         return self.composition
-        
-    def modification_from_name(self, mods: list, place: int=0):
+
+    def modification_from_name(self, mods: list, place: int = 0):
         """Function that finds if the sample was somehow modified, for example by thermal annealing
 
         This can be useful in case you are testing modified samples, and you marked your filename with the letter
-        describing it.  By default describing letter is 
+        describing it.  By default describing letter is
 
         Parameters
         ----------
         mods : list
             that is the list of potential modification you have used, for example A for annealing
         place : int
             That is placement of your describing letter in the modification name. By default it is 0,
@@ -187,18 +192,22 @@
 
         Examples
         --------
         FIXME: Add docs.
 
         """
         from files.files import find_modification
-        self.modification = find_modification(self.name, mods, place)
 
-    def method_from_name(methods: list, delimiter:str = '-'):
-                    """Find the technique how the material was created
+        try:
+            self.modification = find_modification(self.name, mods, place)
+        except NameError:
+            raise NameError("Sample name is not defined")
+
+    def method_from_name(self, delimiter: str = "-", placement: int = 0):
+        """Find the technique how the material was created
 
         Find the method how the material was created, what methods were used to modify it, etc. To do so it is using
         first letters of filename, so for extruded parts you can use EXT, for annealed extruded parts you can use aEXT
         etc.
                     For example if you obtained your material by FDM method containing 90pPET10prPET, you can use FDM-90pPET10prPET name, and it will set instance method variable to FDM
 
         Parameters
@@ -209,9 +218,12 @@
             what sign you wanna use to finish your method string. By default it is -
 
         Examples
         --------
         FIXME: Add docs.
 
         """
-
-
+        try:
+            self.method = self.name.split(delimiter)[placement]
+            return self.method
+        except NameError:
+            raise NameError("Sample name is not defined")
```

