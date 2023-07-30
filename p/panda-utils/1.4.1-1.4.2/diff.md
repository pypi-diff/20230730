# Comparing `tmp/panda_utils-1.4.1.tar.gz` & `tmp/panda_utils-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panda_utils-1.4.1.tar", last modified: Fri Jul 28 09:46:45 2023, max compression
+gzip compressed data, was "panda_utils-1.4.2.tar", last modified: Sun Jul 30 11:22:31 2023, max compression
```

## Comparing `panda_utils-1.4.1.tar` & `panda_utils-1.4.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-28 09:46:45.679729 panda_utils-1.4.1/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1085 2023-07-07 08:54:13.000000 panda_utils-1.4.1/LICENSE
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2206 2023-07-28 09:46:45.679729 panda_utils-1.4.1/PKG-INFO
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1476 2023-07-11 16:19:27.000000 panda_utils-1.4.1/README.md
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      327 2023-06-11 07:33:25.000000 panda_utils-1.4.1/config_example.ini
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-28 09:46:45.676396 panda_utils-1.4.1/panda_utils/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.4.1/panda_utils/__init__.py
--rwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)     6345 2023-06-11 07:03:04.000000 panda_utils-1.4.1/panda_utils/__main__.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-28 09:46:45.679729 panda_utils-1.4.1/panda_utils/assetpipeline/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 07:03:50.000000 panda_utils-1.4.1/panda_utils/assetpipeline/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5056 2023-07-28 09:29:44.000000 panda_utils-1.4.1/panda_utils/assetpipeline/__main__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      247 2023-07-28 09:44:44.000000 panda_utils-1.4.1/panda_utils/assetpipeline/imports.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      807 2023-07-26 20:53:08.000000 panda_utils-1.4.1/panda_utils/assetpipeline/misc.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    14512 2023-07-28 09:44:44.000000 panda_utils-1.4.1/panda_utils/assetpipeline/models.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      785 2023-06-13 10:37:09.000000 panda_utils-1.4.1/panda_utils/assetpipeline/textures.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-28 09:46:45.679729 panda_utils-1.4.1/panda_utils/blender/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 08:19:46.000000 panda_utils-1.4.1/panda_utils/blender/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      615 2023-07-28 09:44:44.000000 panda_utils-1.4.1/panda_utils/blender/export_glb.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1797 2023-07-28 09:44:44.000000 panda_utils-1.4.1/panda_utils/blender/export_with_yabee.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      527 2023-07-28 09:44:44.000000 panda_utils-1.4.1/panda_utils/blender/import_model.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      454 2023-07-11 08:56:38.000000 panda_utils-1.4.1/panda_utils/blender/patch_paths.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-28 09:46:45.679729 panda_utils-1.4.1/panda_utils/eggtree/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-09-19 11:38:19.000000 panda_utils-1.4.1/panda_utils/eggtree/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5632 2023-07-28 09:44:44.000000 panda_utils-1.4.1/panda_utils/eggtree/eggparse.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      762 2023-07-25 21:42:36.000000 panda_utils-1.4.1/panda_utils/eggtree/operations.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-28 09:46:45.679729 panda_utils-1.4.1/panda_utils/tools/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.4.1/panda_utils/tools/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1449 2023-06-10 09:05:07.000000 panda_utils-1.4.1/panda_utils/tools/animconvert.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5397 2023-06-12 17:52:50.000000 panda_utils-1.4.1/panda_utils/tools/convert.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3686 2023-06-13 10:30:48.000000 panda_utils-1.4.1/panda_utils/tools/downscale.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3201 2023-06-13 12:07:52.000000 panda_utils-1.4.1/panda_utils/tools/palettize.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1373 2023-06-10 09:05:07.000000 panda_utils-1.4.1/panda_utils/tools/toontown.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3332 2023-07-08 05:28:59.000000 panda_utils-1.4.1/panda_utils/util.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-28 09:46:45.676396 panda_utils-1.4.1/panda_utils.egg-info/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2206 2023-07-28 09:46:45.000000 panda_utils-1.4.1/panda_utils.egg-info/PKG-INFO
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      991 2023-07-28 09:46:45.000000 panda_utils-1.4.1/panda_utils.egg-info/SOURCES.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        1 2023-07-28 09:46:45.000000 panda_utils-1.4.1/panda_utils.egg-info/dependency_links.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      274 2023-07-28 09:46:45.000000 panda_utils-1.4.1/panda_utils.egg-info/requires.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       12 2023-07-28 09:46:45.000000 panda_utils-1.4.1/panda_utils.egg-info/top_level.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1023 2023-07-28 09:44:37.000000 panda_utils-1.4.1/pyproject.toml
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       66 2023-06-11 07:37:00.000000 panda_utils-1.4.1/requirements.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       38 2023-07-28 09:46:45.679729 panda_utils-1.4.1/setup.cfg
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-30 11:22:31.879986 panda_utils-1.4.2/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1085 2023-07-07 08:54:13.000000 panda_utils-1.4.2/LICENSE
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2206 2023-07-30 11:22:31.879986 panda_utils-1.4.2/PKG-INFO
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1476 2023-07-11 16:19:27.000000 panda_utils-1.4.2/README.md
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      327 2023-06-11 07:33:25.000000 panda_utils-1.4.2/config_example.ini
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-30 11:22:31.876653 panda_utils-1.4.2/panda_utils/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.4.2/panda_utils/__init__.py
+-rwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)     6345 2023-06-11 07:03:04.000000 panda_utils-1.4.2/panda_utils/__main__.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-30 11:22:31.879986 panda_utils-1.4.2/panda_utils/assetpipeline/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 07:03:50.000000 panda_utils-1.4.2/panda_utils/assetpipeline/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     4820 2023-07-30 10:55:48.000000 panda_utils-1.4.2/panda_utils/assetpipeline/__main__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      247 2023-07-28 09:44:44.000000 panda_utils-1.4.2/panda_utils/assetpipeline/imports.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      747 2023-07-30 10:56:09.000000 panda_utils-1.4.2/panda_utils/assetpipeline/misc.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    14659 2023-07-30 11:01:49.000000 panda_utils-1.4.2/panda_utils/assetpipeline/models.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      785 2023-06-13 10:37:09.000000 panda_utils-1.4.2/panda_utils/assetpipeline/textures.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-30 11:22:31.879986 panda_utils-1.4.2/panda_utils/blender/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 08:19:46.000000 panda_utils-1.4.2/panda_utils/blender/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      615 2023-07-28 09:44:44.000000 panda_utils-1.4.2/panda_utils/blender/export_glb.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1797 2023-07-28 09:44:44.000000 panda_utils-1.4.2/panda_utils/blender/export_with_yabee.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      527 2023-07-28 09:44:44.000000 panda_utils-1.4.2/panda_utils/blender/import_model.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      454 2023-07-11 08:56:38.000000 panda_utils-1.4.2/panda_utils/blender/patch_paths.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-30 11:22:31.879986 panda_utils-1.4.2/panda_utils/eggtree/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-09-19 11:38:19.000000 panda_utils-1.4.2/panda_utils/eggtree/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5632 2023-07-28 09:44:44.000000 panda_utils-1.4.2/panda_utils/eggtree/eggparse.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      762 2023-07-25 21:42:36.000000 panda_utils-1.4.2/panda_utils/eggtree/operations.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-30 11:22:31.879986 panda_utils-1.4.2/panda_utils/tools/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.4.2/panda_utils/tools/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1449 2023-06-10 09:05:07.000000 panda_utils-1.4.2/panda_utils/tools/animconvert.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5397 2023-06-12 17:52:50.000000 panda_utils-1.4.2/panda_utils/tools/convert.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3686 2023-06-13 10:30:48.000000 panda_utils-1.4.2/panda_utils/tools/downscale.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3201 2023-06-13 12:07:52.000000 panda_utils-1.4.2/panda_utils/tools/palettize.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1373 2023-06-10 09:05:07.000000 panda_utils-1.4.2/panda_utils/tools/toontown.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3332 2023-07-08 05:28:59.000000 panda_utils-1.4.2/panda_utils/util.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-30 11:22:31.879986 panda_utils-1.4.2/panda_utils.egg-info/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2206 2023-07-30 11:22:31.000000 panda_utils-1.4.2/panda_utils.egg-info/PKG-INFO
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      991 2023-07-30 11:22:31.000000 panda_utils-1.4.2/panda_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        1 2023-07-30 11:22:31.000000 panda_utils-1.4.2/panda_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      274 2023-07-30 11:22:31.000000 panda_utils-1.4.2/panda_utils.egg-info/requires.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       12 2023-07-30 11:22:31.000000 panda_utils-1.4.2/panda_utils.egg-info/top_level.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1023 2023-07-30 11:22:22.000000 panda_utils-1.4.2/pyproject.toml
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       66 2023-06-11 07:37:00.000000 panda_utils-1.4.2/requirements.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       38 2023-07-30 11:22:31.879986 panda_utils-1.4.2/setup.cfg
```

### Comparing `panda_utils-1.4.1/LICENSE` & `panda_utils-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.1/PKG-INFO` & `panda_utils-1.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda_utils
-Version: 1.4.1
+Version: 1.4.2
 Summary: PandaUtils includes multiple tools for basic Panda3D automation
 Author-email: "Toontown: Event Horizon" <development@toontowneventhorizon.com>
 Project-URL: homepage, https://github.com/toontown-event-horizon/panda-utils
 Project-URL: bugtracker, https://github.com/toontown-event-horizon/panda-utils/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `panda_utils-1.4.1/README.md` & `panda_utils-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.1/panda_utils/__main__.py` & `panda_utils-1.4.2/panda_utils/__main__.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.1/panda_utils/assetpipeline/__main__.py` & `panda_utils-1.4.2/panda_utils/assetpipeline/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,16 +28,15 @@
         self.name = self.model_name.replace("-", " ").replace("_", " ").title()
 
         self.intermediate_path = f"{OUTPUT_PARENT}/{output_phase}/models/{output_folder}/{self.model_name}"
         self.output_model_rel = f"{output_phase}/models/{output_folder}"
         self.output_model = os.path.abspath(os.path.dirname(self.intermediate_path))
         self.output_texture = os.path.abspath(f"{OUTPUT_PARENT}/{output_phase}/maps")
         self.eggs = None
-        self.path_overrides = {}
-        self.post_remove = set()
+        self.copy_ignores = set()
 
     def cache_eggs(self):
         if self.eggs is not None:
             return
 
         self.eggs = {}
         for file in self.files:
@@ -88,22 +87,14 @@
         if isinstance(args, dict):
             action(self, **args)
         elif isinstance(args, str):
             action(self, args)
         else:
             logger.warning("%s: Invalid configured arguments: %s (expected dict, or str)", self.name, type(args))
 
-    @staticmethod
-    def reverse_rmdir(path):
-        while not os.listdir(path):
-            path.rmdir()
-            path = path.parent
-            if path[-1] == OUTPUT_PARENT:
-                break
-
 
 def main(enable_logging=False):
     if enable_logging:
         console = logging.StreamHandler()
         console.setLevel(logging.INFO)
         formatter = logging.Formatter("%(name)-12s: %(levelname)-8s %(message)s")
         console.setFormatter(formatter)
```

### Comparing `panda_utils-1.4.1/panda_utils/assetpipeline/misc.py` & `panda_utils-1.4.2/panda_utils/assetpipeline/misc.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,18 +8,17 @@
 
 def action_script(ctx, script_file):
     logger.info("%s: Running script %s", ctx.name, script_file)
     mod = importlib.import_module(f"scripts.{script_file}")
     mod.run(ctx)
 
 
-def action_cts(ctx, injection_name, copy_path):
+def action_cts(ctx, injection_name):
     inject_path = ctx.get_injection_path(injection_name)
     if inject_path is None:
         logger.warning("%s: Unable to find common texture set: %s", ctx.name, injection_name)
         return
 
     for file_name in os.listdir(inject_path):
-        ctx.path_overrides[file_name] = copy_path
-        ctx.post_remove.add(file_name)
+        ctx.copy_ignores.add(file_name)
         shutil.copy(inject_path / file_name, file_name)
     logger.info("%s: Copied common texture set %s", ctx.name, injection_name)
```

### Comparing `panda_utils-1.4.1/panda_utils/assetpipeline/models.py` & `panda_utils-1.4.2/panda_utils/assetpipeline/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -356,42 +356,39 @@
 def action_egg2bam(ctx, all_textures=""):
     all_textures = all_textures.lower() not in ("", "0", "false")
 
     files = []
     # if followed by palettize we wont have eggs here
     ctx.cache_eggs()
 
-    copied_files = set()
+    copied_files = {}
     for file, eggtree in ctx.eggs.items():
         logger.info("%s: Copying %s into the dist directory", ctx.name, file)
         files.append(file)
         operations.set_texture_prefix(eggtree, f"{ctx.output_phase}/maps")
         for tex in eggtree.findall("Texture"):
-            filename = eggparse.sanitize_string(tex.get_child(0).value).split("/")[-1]
-            copied_files.add(filename)
+            full_path = eggparse.sanitize_string(tex.get_child(0).value)
+            filename = full_path.split("/")[-1]
+            # The first two components of full_path we can safely ignore because they're phase_X/maps
+            copied_files[filename] = pathlib.Path(pathlib.PurePosixPath(full_path.split("/", 2)[2]))
 
     if all_textures:
-        copied_files.clear()
+        # By default, we will be copying the textures into the `phase_X/maps/` folder
+        # But if the egg file tells us to copy them into `phase_X/maps/subfolder/` then so be it
         for filename in ctx.files:
-            if image_regex.match(filename):
-                copied_files.add(filename)
+            if filename not in copied_files and image_regex.match(filename):
+                copied_files[filename] = filename
 
-    copied_files = {cf: ctx.path_overrides.get(cf) for cf in copied_files}
-    delete_paths = set()
-    delete_parents = set()
-    for filename, target_path in copied_files.items():
-        if target_path is None:
-            copy_path = pathlib.Path(ctx.output_texture, filename)
-        else:
-            copy_path = pathlib.Path(ctx.output_texture, target_path, filename)
+    # Under no circumstances, we will be copying common texture set into the built/ folder.
+    # This should be done by some other thing *before* we run the pipeline.
+    copied_files = {cf: target for cf, target in copied_files.items() if cf not in ctx.copy_ignores}
+    for filename, target in copied_files.items():
+        copy_path = pathlib.Path(ctx.output_texture, target)
         copy_path.parent.mkdir(parents=True, exist_ok=True)
         shutil.copy(filename, copy_path)
-        if filename in ctx.post_remove:
-            delete_paths.add(copy_path)
-            delete_parents.add(copy_path.parent)
 
     ctx.uncache_eggs()
     for file in ctx.files:
         if file.endswith(".egg"):
             shutil.copy(file, pathlib.Path(ctx.output_model, file))
 
     os.chdir(ctx.output_model)
@@ -400,11 +397,7 @@
     for file in files:
         if file.endswith(".egg"):
             logger.info("%s: Converting %s to bam", ctx.name, file)
             egg2bam(ctx.putil_ctx, ctx.output_model_rel + "/" + file)
             os.unlink(f"{ctx.output_model}/{file}")
     os.chdir(ctx.cwd)
     ctx.putil_ctx.working_path = ctx.cwd
-    for dp in delete_paths:
-        os.unlink(dp)
-    for folder in delete_parents:
-        ctx.reverse_rmdir(folder)
```

### Comparing `panda_utils-1.4.1/panda_utils/assetpipeline/textures.py` & `panda_utils-1.4.2/panda_utils/assetpipeline/textures.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.1/panda_utils/blender/export_glb.py` & `panda_utils-1.4.2/panda_utils/blender/export_glb.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.1/panda_utils/blender/export_with_yabee.py` & `panda_utils-1.4.2/panda_utils/blender/export_with_yabee.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.1/panda_utils/blender/import_model.py` & `panda_utils-1.4.2/panda_utils/blender/import_model.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.1/panda_utils/eggtree/eggparse.py` & `panda_utils-1.4.2/panda_utils/eggtree/eggparse.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.1/panda_utils/eggtree/operations.py` & `panda_utils-1.4.2/panda_utils/eggtree/operations.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.1/panda_utils/tools/animconvert.py` & `panda_utils-1.4.2/panda_utils/tools/animconvert.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.1/panda_utils/tools/convert.py` & `panda_utils-1.4.2/panda_utils/tools/convert.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.1/panda_utils/tools/downscale.py` & `panda_utils-1.4.2/panda_utils/tools/downscale.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.1/panda_utils/tools/palettize.py` & `panda_utils-1.4.2/panda_utils/tools/palettize.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.1/panda_utils/tools/toontown.py` & `panda_utils-1.4.2/panda_utils/tools/toontown.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.1/panda_utils/util.py` & `panda_utils-1.4.2/panda_utils/util.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.1/panda_utils.egg-info/PKG-INFO` & `panda_utils-1.4.2/panda_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda-utils
-Version: 1.4.1
+Version: 1.4.2
 Summary: PandaUtils includes multiple tools for basic Panda3D automation
 Author-email: "Toontown: Event Horizon" <development@toontowneventhorizon.com>
 Project-URL: homepage, https://github.com/toontown-event-horizon/panda-utils
 Project-URL: bugtracker, https://github.com/toontown-event-horizon/panda-utils/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `panda_utils-1.4.1/panda_utils.egg-info/SOURCES.txt` & `panda_utils-1.4.2/panda_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.1/pyproject.toml` & `panda_utils-1.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=60", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "panda_utils"
-version = "1.4.1"
+version = "1.4.2"
 authors = [
     {name = "Toontown: Event Horizon", email = "development@toontowneventhorizon.com"}
 ]
 description = "PandaUtils includes multiple tools for basic Panda3D automation"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

