# Comparing `tmp/speedtools-0.3.0.tar.gz` & `tmp/speedtools-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedtools-0.3.0.tar", last modified: Sat Jul 15 20:58:21 2023, max compression
+gzip compressed data, was "speedtools-0.4.0.tar", last modified: Sun Jul 30 13:53:43 2023, max compression
```

## Comparing `speedtools-0.3.0.tar` & `speedtools-0.4.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:58:21.587999 speedtools-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-15 20:58:05.000000 speedtools-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-07-15 20:58:21.587999 speedtools-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-15 20:58:05.000000 speedtools-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-15 20:58:05.000000 speedtools-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 20:58:21.587999 speedtools-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-15 20:58:05.000000 speedtools-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:58:21.587999 speedtools-0.3.0/speedtools/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-15 20:58:05.000000 speedtools-0.3.0/speedtools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:58:21.587999 speedtools-0.3.0/speedtools/blender/
--rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-07-15 20:58:05.000000 speedtools-0.3.0/speedtools/blender/io_nfs4_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-07-15 20:58:05.000000 speedtools-0.3.0/speedtools/frd_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:58:21.587999 speedtools-0.3.0/speedtools/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-15 20:58:05.000000 speedtools-0.3.0/speedtools/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-15 20:58:05.000000 speedtools-0.3.0/speedtools/qfs_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-15 20:58:05.000000 speedtools-0.3.0/speedtools/refpack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:58:21.587999 speedtools-0.3.0/speedtools/specs/
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-07-15 20:58:05.000000 speedtools-0.3.0/speedtools/specs/fce.ksy
--rw-r--r--   0 runner    (1001) docker     (123)    13111 2023-07-15 20:58:05.000000 speedtools-0.3.0/speedtools/specs/frd.ksy
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-15 20:58:05.000000 speedtools-0.3.0/speedtools/specs/fsh.ksy
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-15 20:58:05.000000 speedtools-0.3.0/speedtools/specs/qfs.ksy
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-15 20:58:05.000000 speedtools-0.3.0/speedtools/specs/viv.ksy
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-15 20:58:05.000000 speedtools-0.3.0/speedtools/speedtool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-15 20:58:05.000000 speedtools-0.3.0/speedtools/tr_ini.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-07-15 20:58:05.000000 speedtools-0.3.0/speedtools/track_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-15 20:58:05.000000 speedtools-0.3.0/speedtools/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-15 20:58:05.000000 speedtools-0.3.0/speedtools/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-07-15 20:58:05.000000 speedtools-0.3.0/speedtools/viv_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:58:21.587999 speedtools-0.3.0/speedtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-07-15 20:58:21.000000 speedtools-0.3.0/speedtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-15 20:58:21.000000 speedtools-0.3.0/speedtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 20:58:21.000000 speedtools-0.3.0/speedtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-15 20:58:21.000000 speedtools-0.3.0/speedtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-15 20:58:21.000000 speedtools-0.3.0/speedtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-15 20:58:21.000000 speedtools-0.3.0/speedtools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:53:43.136143 speedtools-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-30 13:53:26.000000 speedtools-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-30 13:53:43.136143 speedtools-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-30 13:53:26.000000 speedtools-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-30 13:53:26.000000 speedtools-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 13:53:43.136143 speedtools-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-30 13:53:26.000000 speedtools-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:53:43.132143 speedtools-0.4.0/speedtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-30 13:53:26.000000 speedtools-0.4.0/speedtools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:53:43.132143 speedtools-0.4.0/speedtools/blender/
+-rw-r--r--   0 runner    (1001) docker     (123)    16372 2023-07-30 13:53:26.000000 speedtools-0.4.0/speedtools/blender/io_nfs4_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-07-30 13:53:26.000000 speedtools-0.4.0/speedtools/frd_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:53:43.132143 speedtools-0.4.0/speedtools/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-30 13:53:26.000000 speedtools-0.4.0/speedtools/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-30 13:53:26.000000 speedtools-0.4.0/speedtools/qfs_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-30 13:53:26.000000 speedtools-0.4.0/speedtools/refpack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:53:43.136143 speedtools-0.4.0/speedtools/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-07-30 13:53:26.000000 speedtools-0.4.0/speedtools/specs/fce.ksy
+-rw-r--r--   0 runner    (1001) docker     (123)    13111 2023-07-30 13:53:26.000000 speedtools-0.4.0/speedtools/specs/frd.ksy
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-30 13:53:26.000000 speedtools-0.4.0/speedtools/specs/fsh.ksy
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-30 13:53:26.000000 speedtools-0.4.0/speedtools/specs/qfs.ksy
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-30 13:53:26.000000 speedtools-0.4.0/speedtools/specs/viv.ksy
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-30 13:53:26.000000 speedtools-0.4.0/speedtools/speedtool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-30 13:53:26.000000 speedtools-0.4.0/speedtools/tr_ini.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-07-30 13:53:26.000000 speedtools-0.4.0/speedtools/track_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-30 13:53:26.000000 speedtools-0.4.0/speedtools/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-30 13:53:26.000000 speedtools-0.4.0/speedtools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-07-30 13:53:26.000000 speedtools-0.4.0/speedtools/viv_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 13:53:43.132143 speedtools-0.4.0/speedtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-30 13:53:43.000000 speedtools-0.4.0/speedtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-30 13:53:43.000000 speedtools-0.4.0/speedtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 13:53:43.000000 speedtools-0.4.0/speedtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-30 13:53:43.000000 speedtools-0.4.0/speedtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-30 13:53:43.000000 speedtools-0.4.0/speedtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-30 13:53:43.000000 speedtools-0.4.0/speedtools.egg-info/top_level.txt
```

### Comparing `speedtools-0.3.0/LICENSE` & `speedtools-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `speedtools-0.3.0/PKG-INFO` & `speedtools-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtools
-Version: 0.3.0
+Version: 0.4.0
 Summary: NFS4 HS (PC) resource utilities
 Author: Rafał Kuźnia
 Author-email: rafal.kuznia@protonmail.com
 License: GPL-3.0-or-later
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -59,11 +59,13 @@
 * [Kaitai Struct compiler][3]
 
 Make sure the binary directories are in your `PATH`.
 
 # Known issues and limitations
 
 * Tested only with PC tracks
+* Road lanes are missing
+* The bear has left the park!
 
 [1]: https://pypi.org/project/speedtools/
 [2]: https://github.com/e-rk/speedtools/blob/master/speedtools/blender/io_nfs4_import.py
 [3]: https://kaitai.io/
```

### Comparing `speedtools-0.3.0/README.md` & `speedtools-0.4.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -40,11 +40,13 @@
 * [Kaitai Struct compiler][3]
 
 Make sure the binary directories are in your `PATH`.
 
 # Known issues and limitations
 
 * Tested only with PC tracks
+* Road lanes are missing
+* The bear has left the park!
 
 [1]: https://pypi.org/project/speedtools/
 [2]: https://github.com/e-rk/speedtools/blob/master/speedtools/blender/io_nfs4_import.py
 [3]: https://kaitai.io/
```

### Comparing `speedtools-0.3.0/pyproject.toml` & `speedtools-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "speedtools"
-version = "0.3.0"
+version = "0.4.0"
 description = "NFS4 HS (PC) resource utilities"
 authors = [{ name = "Rafał Kuźnia" }, { email = "rafal.kuznia@protonmail.com" }]
 readme = { file = 'README.md', content-type = 'text/markdown' }
 dependencies = ["kaitaistruct", "pillow", "click", "more-itertools", "parse"]
 license = { text = "GPL-3.0-or-later" }
 classifiers = [
     'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
```

### Comparing `speedtools-0.3.0/setup.py` & `speedtools-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `speedtools-0.3.0/speedtools/blender/io_nfs4_import.py` & `speedtools-0.4.0/speedtools/blender/io_nfs4_import.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 from __future__ import annotations
 
 import logging
 from abc import ABCMeta, abstractmethod
 from collections.abc import Callable, Iterable
 from dataclasses import dataclass
 from functools import total_ordering
-from itertools import groupby
+from itertools import chain, groupby
 from pathlib import Path
 from typing import Any
 
 import bpy
 import mathutils
 from bpy.props import BoolProperty, EnumProperty, StringProperty
-from more_itertools import collapse
+from more_itertools import collapse, duplicates_everseen, unique_everseen
 
 from speedtools import TrackData, VivData
 from speedtools.types import (
     Animation,
     BaseMesh,
     DirectionalLight,
     DrawableMesh,
@@ -62,14 +62,38 @@
 
 
 class BaseImporter(metaclass=ABCMeta):
     def __init__(self, material_map: Callable[[Polygon], Resource]) -> None:
         self.materials: dict[ExtendedResource, bpy.types.Material] = {}
         self.material_map = material_map
 
+    @classmethod
+    def duplicate_common_vertices(cls, mesh: DrawableMesh) -> DrawableMesh:
+        unique_vert_polys = list(unique_everseen(mesh.polygons, key=lambda x: frozenset(x.face)))
+        duplicate_vert_polys = list(
+            duplicates_everseen(mesh.polygons, key=lambda x: frozenset(x.face))
+        )
+        faces = chain.from_iterable(poly.face for poly in duplicate_vert_polys)
+        verts_to_duplicate = frozenset(mesh.vertices[x] for x in faces)
+        mapping = {v: i for i, v in enumerate(verts_to_duplicate, start=len(mesh.vertices))}
+
+        def _make_polygon(polygon: Polygon) -> Polygon:
+            vertices = tuple(mesh.vertices[x] for x in polygon.face)
+            face = tuple(mapping[v] for v in vertices)
+            return Polygon(
+                face=face,
+                uv=polygon.uv,
+                material=polygon.material,
+                backface_culling=polygon.backface_culling,
+            )
+
+        polygons = unique_vert_polys + [_make_polygon(polygon) for polygon in duplicate_vert_polys]
+        vertices = list(mesh.vertices) + list(verts_to_duplicate)
+        return DrawableMesh(vertices=vertices, polygons=polygons, normals=mesh.normals)
+
     def _extender_resource_map(self, polygon: Polygon) -> ExtendedResource:
         resource = self.material_map(polygon)
         return ExtendedResource(resource=resource, backface_culling=polygon.backface_culling)
 
     def _make_material(self, ext_resource: ExtendedResource) -> bpy.types.Material:
         resource = ext_resource.resource
         images_dir = Path(bpy.path.abspath("//images"))
@@ -122,16 +146,17 @@
         ):
             mu_location = mathutils.Vector(location)
             mu_quaternion = mathutils.Quaternion(quaternion)
             mu_quaternion = mu_quaternion.normalized()
             mu_quaternion = mu_quaternion.inverted()
             obj.location = mu_location
             obj.rotation_quaternion = mu_quaternion  # type: ignore[assignment]
-            obj.keyframe_insert(data_path="location", frame=index * animation.delay)
-            obj.keyframe_insert(data_path="rotation_quaternion", frame=index * animation.delay)
+            interval = index * animation.delay
+            obj.keyframe_insert(data_path="location", frame=interval)
+            obj.keyframe_insert(data_path="rotation_quaternion", frame=interval)
         obj.animation_data.action.name = f"{obj.name}-loop"
 
     def make_drawable_object(self, name: str, mesh: DrawableMesh) -> bpy.types.Object:
         bpy_mesh = self.make_base_mesh(name=name, mesh=mesh)
         uv_layer = bpy_mesh.uv_layers.new()
         uvs = collapse(polygon.uv for polygon in mesh.polygons)
         uv_layer.data.foreach_set("uv", list(uvs))
@@ -181,23 +206,25 @@
     @abstractmethod
     def import_track(self, track: TrackData) -> None:
         pass
 
 
 class TrackImportSimple(TrackImportStrategy, BaseImporter):
     def import_track(self, track: TrackData) -> None:
+        bpy.context.scene.render.fps = track.ANIMATION_FPS
         track_collection = bpy.data.collections.new("Track segments")
         bpy.context.scene.collection.children.link(track_collection)
         for index, segment in enumerate(track.track_segments):
             name = f"Track segment {index}"
             bpy_obj = self.make_drawable_object(name=name, mesh=segment.mesh)
             track_collection.objects.link(bpy_obj)
         for index, obj in enumerate(track.objects):
             name = f"Track object {index}"
-            bpy_obj = self.make_drawable_object(name=name, mesh=obj.mesh)
+            mesh = self.duplicate_common_vertices(mesh=obj.mesh)
+            bpy_obj = self.make_drawable_object(name=name, mesh=mesh)
             if obj.location:
                 self.set_object_location(obj=bpy_obj, location=obj.location)
             if obj.animation:
                 self.set_object_animation(obj=bpy_obj, animation=obj.animation)
             track_collection.objects.link(bpy_obj)
         for index, light in enumerate(track.lights):
             name = f"Track light {index}"
@@ -207,14 +234,15 @@
         if directional_light:
             bpy_obj = self.make_directional_light_object(name="sun", light=directional_light)
             track_collection.objects.link(bpy_obj)
 
 
 class TrackImportAdvanced(TrackImportStrategy, BaseImporter):
     def import_track(self, track: TrackData) -> None:
+        bpy.context.scene.render.fps = track.ANIMATION_FPS
         track_collection = bpy.data.collections.new("Track segments")
         bpy.context.scene.collection.children.link(track_collection)
         for index, segment in enumerate(track.track_segments):
             name = f"Track segment {index}"
             bpy_obj = self.make_drawable_object(name=name, mesh=segment.mesh)
             track_collection.objects.link(bpy_obj)
             for collision_mesh in segment.collision_meshes:
@@ -223,15 +251,16 @@
                 )
                 bpy_mesh = self.make_base_mesh(name=name, mesh=collision_mesh)
                 bpy_obj = bpy.data.objects.new(name, bpy_mesh)
                 track_collection.objects.link(bpy_obj)
                 bpy_obj.hide_set(True)
         for index, obj in enumerate(track.objects):
             name = f"Track object {index}"
-            bpy_obj = self.make_drawable_object(name=name, mesh=obj.mesh)
+            mesh = self.duplicate_common_vertices(mesh=obj.mesh)
+            bpy_obj = self.make_drawable_object(name=name, mesh=mesh)
             if obj.location:
                 self.set_object_location(obj=bpy_obj, location=obj.location)
             if obj.animation:
                 self.set_object_animation(obj=bpy_obj, animation=obj.animation)
             track_collection.objects.link(bpy_obj)
         for index, light in enumerate(track.lights):
             name = f"Track light {index}"
```

### Comparing `speedtools-0.3.0/speedtools/frd_data.py` & `speedtools-0.4.0/speedtools/frd_data.py`

 * *Files identical despite different names*

### Comparing `speedtools-0.3.0/speedtools/qfs_data.py` & `speedtools-0.4.0/speedtools/qfs_data.py`

 * *Files identical despite different names*

### Comparing `speedtools-0.3.0/speedtools/refpack.py` & `speedtools-0.4.0/speedtools/refpack.py`

 * *Files identical despite different names*

### Comparing `speedtools-0.3.0/speedtools/specs/fce.ksy` & `speedtools-0.4.0/speedtools/specs/fce.ksy`

 * *Files identical despite different names*

### Comparing `speedtools-0.3.0/speedtools/specs/frd.ksy` & `speedtools-0.4.0/speedtools/specs/frd.ksy`

 * *Files identical despite different names*

### Comparing `speedtools-0.3.0/speedtools/specs/fsh.ksy` & `speedtools-0.4.0/speedtools/specs/fsh.ksy`

 * *Files identical despite different names*

### Comparing `speedtools-0.3.0/speedtools/specs/viv.ksy` & `speedtools-0.4.0/speedtools/specs/viv.ksy`

 * *Files identical despite different names*

### Comparing `speedtools-0.3.0/speedtools/speedtool.py` & `speedtools-0.4.0/speedtools/speedtool.py`

 * *Files identical despite different names*

### Comparing `speedtools-0.3.0/speedtools/tr_ini.py` & `speedtools-0.4.0/speedtools/tr_ini.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,19 +60,19 @@
     def glows(self) -> Iterator[LightAttributes]:
         return starmap(self._make_glow, self.parser["track glows"].items())
 
     @property
     def sun(self) -> SunIni | None:
         try:
             sun = self.parser["sun"]
-            if bool(sun["hasSun"]) is False:
+            if sun["hasSun"] == "0":
                 return None
             return SunIni(
                 angle_theta=float(sun["angleTheta"]),
                 angle_rho=float(sun["angleRho"]),
                 radius=float(sun["radius"]),
-                rotates=bool(sun.get("rotates", "0")),
-                additive=bool(sun.get("additive", "0")),
-                in_front=bool(sun.get("inFront", "0")),
+                rotates=sun.get("rotates", "0") != "0",
+                additive=sun.get("additive", "0") != "0",
+                in_front=sun.get("inFront", "0") != "0",
             )
         except KeyError:
             return None
```

### Comparing `speedtools-0.3.0/speedtools/track_data.py` & `speedtools-0.4.0/speedtools/track_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
 logger = logging.getLogger(__name__)
 T = TypeVar("T")
 
 
 class TrackData:
     SUN_DISTANCE = 3000
+    ANIMATION_FPS = 64
 
     def __init__(
         self, directory: Path, mirrored: bool = False, night: bool = False, weather: bool = False
     ) -> None:
         logger.debug(f"Opening directory {directory}")
         self.frd: FrdData = self.tr_open(
             constructor=FrdData.from_file,
```

### Comparing `speedtools-0.3.0/speedtools/types.py` & `speedtools-0.4.0/speedtools/types.py`

 * *Files identical despite different names*

### Comparing `speedtools-0.3.0/speedtools/utils.py` & `speedtools-0.4.0/speedtools/utils.py`

 * *Files identical despite different names*

### Comparing `speedtools-0.3.0/speedtools/viv_data.py` & `speedtools-0.4.0/speedtools/viv_data.py`

 * *Files identical despite different names*

### Comparing `speedtools-0.3.0/speedtools.egg-info/PKG-INFO` & `speedtools-0.4.0/speedtools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtools
-Version: 0.3.0
+Version: 0.4.0
 Summary: NFS4 HS (PC) resource utilities
 Author: Rafał Kuźnia
 Author-email: rafal.kuznia@protonmail.com
 License: GPL-3.0-or-later
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -59,11 +59,13 @@
 * [Kaitai Struct compiler][3]
 
 Make sure the binary directories are in your `PATH`.
 
 # Known issues and limitations
 
 * Tested only with PC tracks
+* Road lanes are missing
+* The bear has left the park!
 
 [1]: https://pypi.org/project/speedtools/
 [2]: https://github.com/e-rk/speedtools/blob/master/speedtools/blender/io_nfs4_import.py
 [3]: https://kaitai.io/
```

### Comparing `speedtools-0.3.0/speedtools.egg-info/SOURCES.txt` & `speedtools-0.4.0/speedtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

