# Comparing `tmp/sourmash_plugin_venn-0.2.tar.gz` & `tmp/sourmash_plugin_venn-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sourmash_plugin_venn-0.2.tar", last modified: Tue Jul 25 20:39:05 2023, max compression
+gzip compressed data, was "sourmash_plugin_venn-0.3.tar", last modified: Sun Jul 30 10:35:07 2023, max compression
```

## Comparing `sourmash_plugin_venn-0.2.tar` & `sourmash_plugin_venn-0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-25 20:39:05.491703 sourmash_plugin_venn-0.2/
--rw-r--r--   0 t          (502) staff       (20)     1540 2023-07-24 20:57:14.000000 sourmash_plugin_venn-0.2/LICENSE
--rw-r--r--   0 t          (502) staff       (20)      583 2023-07-25 20:39:05.491562 sourmash_plugin_venn-0.2/PKG-INFO
--rw-r--r--   0 t          (502) staff       (20)      386 2023-07-25 20:32:07.000000 sourmash_plugin_venn-0.2/README.md
--rw-r--r--   0 t          (502) staff       (20)      381 2023-07-25 20:32:07.000000 sourmash_plugin_venn-0.2/pyproject.toml
--rw-r--r--   0 t          (502) staff       (20)       38 2023-07-25 20:39:05.491749 sourmash_plugin_venn-0.2/setup.cfg
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-25 20:39:05.489996 sourmash_plugin_venn-0.2/src/
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-25 20:39:05.491094 sourmash_plugin_venn-0.2/src/sourmash_plugin_venn.egg-info/
--rw-r--r--   0 t          (502) staff       (20)      583 2023-07-25 20:39:05.000000 sourmash_plugin_venn-0.2/src/sourmash_plugin_venn.egg-info/PKG-INFO
--rw-r--r--   0 t          (502) staff       (20)      380 2023-07-25 20:39:05.000000 sourmash_plugin_venn-0.2/src/sourmash_plugin_venn.egg-info/SOURCES.txt
--rw-r--r--   0 t          (502) staff       (20)        1 2023-07-25 20:39:05.000000 sourmash_plugin_venn-0.2/src/sourmash_plugin_venn.egg-info/dependency_links.txt
--rw-r--r--   0 t          (502) staff       (20)       68 2023-07-25 20:39:05.000000 sourmash_plugin_venn-0.2/src/sourmash_plugin_venn.egg-info/entry_points.txt
--rw-r--r--   0 t          (502) staff       (20)       46 2023-07-25 20:39:05.000000 sourmash_plugin_venn-0.2/src/sourmash_plugin_venn.egg-info/requires.txt
--rw-r--r--   0 t          (502) staff       (20)       21 2023-07-25 20:39:05.000000 sourmash_plugin_venn-0.2/src/sourmash_plugin_venn.egg-info/top_level.txt
--rw-r--r--   0 t          (502) staff       (20)     2809 2023-07-25 20:32:07.000000 sourmash_plugin_venn-0.2/src/sourmash_plugin_venn.py
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-25 20:39:05.491241 sourmash_plugin_venn-0.2/tests/
--rw-r--r--   0 t          (502) staff       (20)      446 2023-07-24 20:57:14.000000 sourmash_plugin_venn-0.2/tests/test_sourmash_plugin.py
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-30 10:35:07.121432 sourmash_plugin_venn-0.3/
+-rw-r--r--   0 t          (502) staff       (20)     1540 2023-07-24 20:57:14.000000 sourmash_plugin_venn-0.3/LICENSE
+-rw-r--r--   0 t          (502) staff       (20)     1093 2023-07-30 10:35:07.121286 sourmash_plugin_venn-0.3/PKG-INFO
+-rw-r--r--   0 t          (502) staff       (20)      896 2023-07-30 10:32:56.000000 sourmash_plugin_venn-0.3/README.md
+-rw-r--r--   0 t          (502) staff       (20)      381 2023-07-30 10:32:14.000000 sourmash_plugin_venn-0.3/pyproject.toml
+-rw-r--r--   0 t          (502) staff       (20)       38 2023-07-30 10:35:07.121723 sourmash_plugin_venn-0.3/setup.cfg
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-30 10:35:07.116501 sourmash_plugin_venn-0.3/src/
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-30 10:35:07.118886 sourmash_plugin_venn-0.3/src/sourmash_plugin_venn.egg-info/
+-rw-r--r--   0 t          (502) staff       (20)     1093 2023-07-30 10:35:07.000000 sourmash_plugin_venn-0.3/src/sourmash_plugin_venn.egg-info/PKG-INFO
+-rw-r--r--   0 t          (502) staff       (20)      380 2023-07-30 10:35:07.000000 sourmash_plugin_venn-0.3/src/sourmash_plugin_venn.egg-info/SOURCES.txt
+-rw-r--r--   0 t          (502) staff       (20)        1 2023-07-30 10:35:07.000000 sourmash_plugin_venn-0.3/src/sourmash_plugin_venn.egg-info/dependency_links.txt
+-rw-r--r--   0 t          (502) staff       (20)       68 2023-07-30 10:35:07.000000 sourmash_plugin_venn-0.3/src/sourmash_plugin_venn.egg-info/entry_points.txt
+-rw-r--r--   0 t          (502) staff       (20)       46 2023-07-30 10:35:07.000000 sourmash_plugin_venn-0.3/src/sourmash_plugin_venn.egg-info/requires.txt
+-rw-r--r--   0 t          (502) staff       (20)       21 2023-07-30 10:35:07.000000 sourmash_plugin_venn-0.3/src/sourmash_plugin_venn.egg-info/top_level.txt
+-rw-r--r--   0 t          (502) staff       (20)     3189 2023-07-30 10:27:30.000000 sourmash_plugin_venn-0.3/src/sourmash_plugin_venn.py
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-30 10:35:07.120251 sourmash_plugin_venn-0.3/tests/
+-rw-r--r--   0 t          (502) staff       (20)      446 2023-07-24 20:57:14.000000 sourmash_plugin_venn-0.3/tests/test_sourmash_plugin.py
```

### Comparing `sourmash_plugin_venn-0.2/LICENSE` & `sourmash_plugin_venn-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_venn-0.2/src/sourmash_plugin_venn.py` & `sourmash_plugin_venn-0.3/src/sourmash_plugin_venn.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 "Create and write out a pairwise Venn diagram."
 import sys
 
 import pylab
-from matplotlib_venn import venn2
+from matplotlib_venn import venn2, venn3
 
 import sourmash
 from sourmash import sourmash_args
 from sourmash.logging import debug_literal, error, notify
 from sourmash.plugins import CommandLinePlugin
 from sourmash.cli.utils import (add_ksize_arg, add_moltype_args)
 
@@ -14,29 +14,31 @@
 
 #
 # CLI plugin - supports 'sourmash scripts venn'
 #
 
 class Command_Venn(CommandLinePlugin):
     command = 'venn'
-    description = "makes a venn diagram of the overlap between two sketches"
+    description = "makes a venn diagram of the overlap between two or three sketches"
 
     def __init__(self, subparser):
         super().__init__(subparser)
         # add argparse arguments here.
         debug_literal('RUNNING cmd venn __init__')
         subparser.add_argument('sketches', nargs='+',
-                               help="file(s) containing exactly two sketches")
+                               help="file(s) containing two or three sketches")
         subparser.add_argument('-o', '--output', default=None,
                                help="save Venn diagram image to this file",
                                required=True)
         subparser.add_argument('--name1', default=None,
                                help="override name for first sketch")
         subparser.add_argument('--name2', default=None,
                                help="override name for second sketch")
+        subparser.add_argument('--name3', default=None,
+                               help="override name for (optional) third sketch")
         add_ksize_arg(subparser)
         add_moltype_args(subparser)
 
     def main(self, args):
         # code that we actually run.
         super().main(args)
         moltype = sourmash_args.calculate_moltype(args)
@@ -51,27 +53,33 @@
             x = list(sourmash.load_file_as_signatures(filename,
                                                       ksize=args.ksize,
                                                       select_moltype=moltype))
             notify(f"...loaded {len(x)} sketches from {filename}.")
             sketches.extend(x)
 
         if not len(sketches):
-            error("ERROR: no sketches found. Must supply exactly 2.")
+            error("ERROR: no sketches found. Must supply 2 or 3.")
             sys.exit(-1)
         elif len(sketches) == 1:
-            error("ERROR: only found one sketch. Must supply exactly 2.")
+            error("ERROR: only found one sketch. Must supply 2 or 3.")
             sys.exit(-1)
-        elif len(sketches) > 2:
-            error("ERROR: found more than one sketch. Must supply exactly 2.")
+        elif len(sketches) > 3:
+            error("ERROR: found more than three sketches. Must supply 2 or 3.")
             sys.exit(-1)
 
-        sketch1, sketch2 = sketches
-        hashes1 = set(sketch1.minhash.hashes)
-        hashes2 = set(sketch2.minhash.hashes)
+        hashes1 = set(sketches[0].minhash.hashes)
+        hashes2 = set(sketches[1].minhash.hashes)
             
         label1 = args.name1 or sketches[0].name
         label2 = args.name2 or sketches[1].name
 
-        venn2([hashes1, hashes2], set_labels=(label1, label2))
+        if len(sketches) == 2:
+            venn2([hashes1, hashes2], set_labels=(label1, label2))
+
+        elif len(sketches) == 3:
+            hashes3 = set(sketches[2].minhash.hashes)
+            label3 = args.name3 or sketches[2].name
+            venn3([hashes1, hashes2,hashes3], set_labels=(label1, label2, label3))
+
         if args.output:
             print(f"saving to '{args.output}'")
             pylab.savefig(args.output)
```

