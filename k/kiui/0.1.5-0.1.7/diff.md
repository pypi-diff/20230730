# Comparing `tmp/kiui-0.1.5.tar.gz` & `tmp/kiui-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiui-0.1.5.tar", last modified: Wed Jun 14 04:56:19 2023, max compression
+gzip compressed data, was "kiui-0.1.7.tar", last modified: Sun Jul 30 14:56:34 2023, max compression
```

## Comparing `kiui-0.1.5.tar` & `kiui-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:56:19.687029 kiui-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 04:56:10.000000 kiui-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-14 04:56:19.687029 kiui-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-14 04:56:10.000000 kiui-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:56:19.687029 kiui-0.1.5/kiui/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-14 04:56:10.000000 kiui-0.1.5/kiui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-14 04:56:10.000000 kiui-0.1.5/kiui/bg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-06-14 04:56:10.000000 kiui-0.1.5/kiui/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    12513 2023-06-14 04:56:10.000000 kiui-0.1.5/kiui/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-14 04:56:10.000000 kiui-0.1.5/kiui/op.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-14 04:56:10.000000 kiui-0.1.5/kiui/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-06-14 04:56:10.000000 kiui-0.1.5/kiui/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:56:19.687029 kiui-0.1.5/kiui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-14 04:56:19.000000 kiui-0.1.5/kiui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-14 04:56:19.000000 kiui-0.1.5/kiui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 04:56:19.000000 kiui-0.1.5/kiui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-14 04:56:19.000000 kiui-0.1.5/kiui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-14 04:56:19.000000 kiui-0.1.5/kiui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 04:56:19.687029 kiui-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-14 04:56:10.000000 kiui-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:56:34.148046 kiui-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-30 14:56:21.000000 kiui-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-07-30 14:56:34.148046 kiui-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-30 14:56:21.000000 kiui-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:56:34.148046 kiui-0.1.7/kiui/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-30 14:56:21.000000 kiui-0.1.7/kiui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-07-30 14:56:21.000000 kiui-0.1.7/kiui/cam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-30 14:56:21.000000 kiui-0.1.7/kiui/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13075 2023-07-30 14:56:21.000000 kiui-0.1.7/kiui/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-30 14:56:21.000000 kiui-0.1.7/kiui/op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-07-30 14:56:21.000000 kiui-0.1.7/kiui/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-07-30 14:56:21.000000 kiui-0.1.7/kiui/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:56:34.148046 kiui-0.1.7/kiui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-07-30 14:56:34.000000 kiui-0.1.7/kiui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-30 14:56:34.000000 kiui-0.1.7/kiui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 14:56:34.000000 kiui-0.1.7/kiui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-30 14:56:34.000000 kiui-0.1.7/kiui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-30 14:56:34.000000 kiui-0.1.7/kiui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 14:56:34.148046 kiui-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-30 14:56:21.000000 kiui-0.1.7/setup.py
```

### Comparing `kiui-0.1.5/LICENSE` & `kiui-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kiui-0.1.5/PKG-INFO` & `kiui-0.1.7/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: kiui
-Version: 0.1.5
-Summary: self-use toolkits
-Home-page: https://github.com/ashawkey/kiuikit
-Author: kiui
-Author-email: ashawkey1999@gmail.com
-Keywords: utility
-Classifier: Programming Language :: Python :: 3 
-Description-Content-Type: text/markdown
-Provides-Extra: full
-License-File: LICENSE
-
 # kiui kit
 
 A toolkit for personal use.
 
 ### Install
 
 ```bash
@@ -59,16 +46,26 @@
 
 ### mesh utils
 from kiui.mesh import Mesh
 mesh = Mesh.load('model.obj')
 kiui.lo(mesh.v, mesh.f) # CUDA torch.Tensor suitable for nvdiffrast
 mesh.write('new.obj')
 
-### background removal utils
-from kiui.bg import remove, remove_file, remove_folder
-res = remove(img)
-remove_file('input.jpg', 'output.png')
-remove_file('input.jpg', 'output.png', post_process=True) # morphology opening
-remove_file('input.jpg', 'output.png', lcc=True) # largest connected component
-remove_file('input.jpg', 'mask.png', return_mask=True) # only save [h, w] mask
-remove_folder('input/', 'output/')
 ```
+
+CLI tools:
+```bash
+# background removal utils
+python -m kiui.cli.bg --help
+python -m kiui.cli.bg input.png output.png
+python -m kiui.cli.bg input_folder output_folder
+
+# openpose detector
+python -m kiui.cli.pose --help
+
+# hed edge detector
+python -m kiui.cli.hed --help
+
+# open a GUI to render a mesh (extra dependency: nvdiffrast)
+python -m kiui.cli.renderer --help
+python -m kiui.cli.renderer mesh.obj
+```
```

### Comparing `kiui-0.1.5/kiui/env.py` & `kiui-0.1.7/kiui/env.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,138 +1,152 @@
 import importlib
 import inspect
 
 
 LIBS = {
-    'base': [{
-        'os': 'os',
-        'glob': 'glob',
-        'math': 'math',
-        'time': 'time',
-        'random': 'random',
-        'argparse': 'argparse',
-    }, ()],
-
-    'utils': [{
-        'tqdm': 'tqdm',
-        'rich': 'rich',
-    }, ('base')], # dependency
-
-    'data': [{
-        'np': 'numpy', # alternatives
-        'cv2': 'cv2',
-        'plt': 'matplotlib.pyplot',
-        'Image': 'PIL.Image',
-        # 'vis': vis, # live object
-    }, ('base', 'utils')],
-
-    'torch': [{
-        'torch': 'torch',
-        'nn': 'torch.nn',
-        'F': 'torch.nn.functional',
-        'Dataset': ('torch.utils.data', 'Dataset'), # single class/function
-        'DataLoader': ('torch.utils.data', 'DataLoader'),
-    }, ('base', 'utils', 'data')],
-
+    "base": [
+        {
+            "os": "os",
+            "glob": "glob",
+            "math": "math",
+            "time": "time",
+            "random": "random",
+            "argparse": "argparse",
+        },
+        (),
+    ],
+    "utils": [
+        {
+            "tqdm": "tqdm",
+            "rich": "rich",
+        },
+        ("base"),
+    ],  # dependency
+    "data": [
+        {
+            "np": "numpy",  # alternatives
+            "cv2": "cv2",
+            "plt": "matplotlib.pyplot",
+            "Image": "PIL.Image",
+            # 'vis': vis, # live object
+        },
+        ("base", "utils"),
+    ],
+    "torch": [
+        {
+            "torch": "torch",
+            "nn": "torch.nn",
+            "F": "torch.nn.functional",
+            "Dataset": ("torch.utils.data", "Dataset"),  # single class/function
+            "DataLoader": ("torch.utils.data", "DataLoader"),
+        },
+        ("base", "utils", "data"),
+    ],
 }
 
-LIBS['all'] = [{}, tuple(LIBS.keys())]
+LIBS["all"] = [{}, tuple(LIBS.keys())]
 
 G = None
 
+
 def retrieve_globals(verbose=False):
     # locate and set G to the globals which directly `import kiui`. (only once)
     # ref: https://stackoverflow.com/questions/40652688/how-to-access-globals-of-parent-module-into-a-sub-module/50381748
     global G
     stack = inspect.stack()
-    frame_id = 1 
+    frame_id = 1
     while frame_id < len(stack):
         g = dict(inspect.getmembers(stack[frame_id][0]))["f_globals"]
-        if 'kiui' in g:
+        if "kiui" in g:
             G = g
             if verbose:
-                print(f'[KiuiKit-INFO] located global frame at {frame_id}')
+                print(f"[KiuiKit-INFO] located global frame at {frame_id}")
             break
         frame_id += 1
     if G is None:
-        raise RuntimeError('Cannot locate global frame, make sure you called exactly `import kiui`!')
+        raise RuntimeError(
+            "Cannot locate global frame, make sure you called exactly `import kiui`!"
+        )
 
 
 def try_import(target, sources, verbose=False):
 
     if G is None:
         retrieve_globals(verbose)
-    
+
     if target in G:
         if verbose:
-            print(f'[KiuiKit-INFO] {target} is already present, skipped.')
+            print(f"[KiuiKit-INFO] {target} is already present, skipped.")
         return
 
     if not isinstance(sources, list):
         sources = [sources]
 
     for source in sources:
         try:
             if verbose:
-                print(f'[KiuiKit-INFO] try to import {source}')
-            
+                print(f"[KiuiKit-INFO] try to import {source}")
+
             # (module, component) or ("module", component)
             if isinstance(source, tuple):
                 source_module, source_component = source
                 if isinstance(source_module, str):
                     source_module = importlib.import_module(source_module)
                 source = getattr(source_module, source_component)
             # "module"
             elif isinstance(source, str):
                 source = importlib.import_module(source)
             # module
             else:
                 pass
 
             G[target] = source
-            
+
             if verbose:
-                print(f'[KiuiKit-INFO] succeed to import {source} as {target}')
+                print(f"[KiuiKit-INFO] succeed to import {source} as {target}")
             break
 
         except ImportError as e:
-            print(f'[KiuiKit-WARN] failed to import {source} as {target}: {str(e)}')
-            
+            print(f"[KiuiKit-WARN] failed to import {source} as {target}: {str(e)}")
+
 
 def import_libs(pack, verbose=False):
     for k, v in LIBS[pack][0].items():
         try_import(k, v, verbose)
 
 
 """
 setup all import in one line.
 usage:
     kiui.env() # setup base env
     kiui.env('torch') # pytorch with all regular dependencies
     kiui.env('[torch]') # pytorch only
 """
+
+
 def env(*packs, verbose=False):
     if len(packs) == 0:
-        packs = ['base']
+        packs = ["base"]
 
     def check_pack(pack):
         if pack not in LIBS:
-            raise RuntimeError(f'[Kiui-ERROR] unknown pack {pack}, availables: {list(LIBS.keys())}')
+            raise RuntimeError(
+                f"[Kiui-ERROR] unknown pack {pack}, availables: {list(LIBS.keys())}"
+            )
 
     def resolve_env(packs):
         res = set()
         for pack in packs:
-            if pack[0] == '[' and pack[-1] == ']':
+            if pack[0] == "[" and pack[-1] == "]":
                 pack = pack[1:-1]
                 check_pack(pack)
                 res.add(pack)
             else:
                 check_pack(pack)
                 for dep in LIBS[pack][1]:
                     res.add(dep)
                 res.add(pack)
         return list(res)
-    
+
     packs = resolve_env(packs)
     for pack in packs:
         import_libs(pack, verbose)
-
```

### Comparing `kiui-0.1.5/kiui/mesh.py` & `kiui-0.1.7/kiui/mesh.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,219 +3,266 @@
 import torch
 import trimesh
 import numpy as np
 
 from .op import *
 
 
-class Mesh():
-
-    def __init__(self, v=None, f=None, vn=None, fn=None, vt=None, ft=None, albedo=None, device=None):
+class Mesh:
+    def __init__(
+        self,
+        v=None,
+        f=None,
+        vn=None,
+        fn=None,
+        vt=None,
+        ft=None,
+        albedo=None,
+        device=None,
+    ):
         self.device = device
         self.v = v
         self.vn = vn
         self.vt = vt
         self.f = f
         self.fn = fn
         self.ft = ft
         # only support a single albedo
         self.albedo = albedo
 
         self.ori_center = 0
         self.ori_scale = 1
-    
+
     @classmethod
     def load(cls, path=None, **kwargs):
         # assume init with kwargs
         if path is None:
             mesh = cls(**kwargs)
         # obj supports face uv
-        elif path.endswith('.obj'):
+        elif path.endswith(".obj"):
             mesh = cls.load_obj(path, **kwargs)
         # trimesh only supports vertex uv, but can load more formats
         else:
             mesh = cls.load_trimesh(path, **kwargs)
-        
+
         # auto-normalize
         mesh.auto_size()
-        print(f'[Mesh loading] v: {mesh.v.shape}, f: {mesh.f.shape}')
+        print(f"[Mesh loading] v: {mesh.v.shape}, f: {mesh.f.shape}")
         # auto-fix normal
         if mesh.vn is None:
             mesh.auto_normal()
-        print(f'[Mesh loading] vn: {mesh.vn.shape}, fn: {mesh.fn.shape}')
+        print(f"[Mesh loading] vn: {mesh.vn.shape}, fn: {mesh.fn.shape}")
         # auto-fix texture
         if mesh.vt is None:
             mesh.auto_uv(cache_path=path)
-        print(f'[Mesh loading] vt: {mesh.vt.shape}, ft: {mesh.ft.shape}')
-        
+        print(f"[Mesh loading] vt: {mesh.vt.shape}, ft: {mesh.ft.shape}")
+
         return mesh
 
     # load from obj file
     @classmethod
     def load_obj(cls, path, albedo_path=None, device=None, init_empty_tex=False):
 
-        assert os.path.splitext(path)[-1] == '.obj'
+        assert os.path.splitext(path)[-1] == ".obj"
 
         mesh = cls()
 
         # device
         if device is None:
-            device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
+            device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
         mesh.device = device
 
         # try to find texture from mtl file
         if albedo_path is None:
-            mtl_path = path.replace('.obj', '.mtl')
+            mtl_path = path.replace(".obj", ".mtl")
             if os.path.exists(mtl_path):
-                with open(mtl_path, 'r') as f:
+                with open(mtl_path, "r") as f:
                     lines = f.readlines()
                 for line in lines:
                     split_line = line.split()
                     # empty line
                     if len(split_line) == 0:
                         continue
                     prefix = split_line[0]
                     # NOTE: simply use the first map_Kd as albedo!
-                    if 'map_Kd' in prefix:
+                    if "map_Kd" in prefix:
                         albedo_path = os.path.join(os.path.dirname(path), split_line[1])
-                        print(f'[load_obj] use texture from: {albedo_path}')
+                        print(f"[load_obj] use texture from: {albedo_path}")
                         break
 
         if init_empty_tex or albedo_path is None or not os.path.exists(albedo_path):
             # init an empty texture
-            print(f'[load_obj] init empty albedo!')
+            print(f"[load_obj] init empty albedo!")
             # albedo = np.random.rand(1024, 1024, 3).astype(np.float32)
-            albedo = np.ones((1024, 1024, 3), dtype=np.float32) * np.array([0.5, 0.5, 0.5])  # default color
+            albedo = np.ones((1024, 1024, 3), dtype=np.float32) * np.array(
+                [0.5, 0.5, 0.5]
+            )  # default color
         else:
             albedo = cv2.imread(albedo_path, cv2.IMREAD_UNCHANGED)
             albedo = cv2.cvtColor(albedo, cv2.COLOR_BGR2RGB)
             albedo = albedo.astype(np.float32) / 255
-            print(f'[load_obj] load texture: {albedo.shape}')
+            print(f"[load_obj] load texture: {albedo.shape}")
 
             # import matplotlib.pyplot as plt
             # plt.imshow(albedo)
             # plt.show()
 
         mesh.albedo = torch.tensor(albedo, dtype=torch.float32, device=device)
 
         # load obj
-        with open(path, 'r') as f:
+        with open(path, "r") as f:
             lines = f.readlines()
 
         def parse_f_v(fv):
             # pass in a vertex term of a face, return {v, vt, vn} (-1 if not provided)
             # supported forms:
             # f v1 v2 v3
             # f v1/vt1 v2/vt2 v3/vt3
             # f v1/vt1/vn1 v2/vt2/vn2 v3/vt3/vn3
             # f v1//vn1 v2//vn2 v3//vn3
-            xs = [int(x) - 1 if x != '' else -1 for x in fv.split('/')]
+            xs = [int(x) - 1 if x != "" else -1 for x in fv.split("/")]
             xs.extend([-1] * (3 - len(xs)))
             return xs[0], xs[1], xs[2]
 
         # NOTE: we ignore usemtl, and assume the mesh ONLY uses one material (first in mtl)
         vertices, texcoords, normals = [], [], []
         faces, tfaces, nfaces = [], [], []
         for line in lines:
             split_line = line.split()
             # empty line
             if len(split_line) == 0:
                 continue
             # v/vn/vt
             prefix = split_line[0].lower()
-            if prefix == 'v':
+            if prefix == "v":
                 vertices.append([float(v) for v in split_line[1:]])
-            elif prefix == 'vn':
+            elif prefix == "vn":
                 normals.append([float(v) for v in split_line[1:]])
-            elif prefix == 'vt':
+            elif prefix == "vt":
                 val = [float(v) for v in split_line[1:]]
                 texcoords.append([val[0], 1.0 - val[1]])
-            elif prefix == 'f':
+            elif prefix == "f":
                 vs = split_line[1:]
                 nv = len(vs)
                 v0, t0, n0 = parse_f_v(vs[0])
                 for i in range(nv - 2):  # triangulate (assume vertices are ordered)
                     v1, t1, n1 = parse_f_v(vs[i + 1])
                     v2, t2, n2 = parse_f_v(vs[i + 2])
                     faces.append([v0, v1, v2])
                     tfaces.append([t0, t1, t2])
                     nfaces.append([n0, n1, n2])
 
         mesh.v = torch.tensor(vertices, dtype=torch.float32, device=device)
-        mesh.vt = torch.tensor(texcoords, dtype=torch.float32, device=device) if len(texcoords) > 0 else None
-        mesh.vn = torch.tensor(normals, dtype=torch.float32, device=device) if len(normals) > 0 else None
+        mesh.vt = (
+            torch.tensor(texcoords, dtype=torch.float32, device=device)
+            if len(texcoords) > 0
+            else None
+        )
+        mesh.vn = (
+            torch.tensor(normals, dtype=torch.float32, device=device)
+            if len(normals) > 0
+            else None
+        )
 
         mesh.f = torch.tensor(faces, dtype=torch.int32, device=device)
-        mesh.ft = torch.tensor(tfaces, dtype=torch.int32, device=device) if texcoords is not None else None
-        mesh.fn = torch.tensor(nfaces, dtype=torch.int32, device=device) if normals is not None else None
+        mesh.ft = (
+            torch.tensor(tfaces, dtype=torch.int32, device=device)
+            if texcoords is not None
+            else None
+        )
+        mesh.fn = (
+            torch.tensor(nfaces, dtype=torch.int32, device=device)
+            if normals is not None
+            else None
+        )
 
         return mesh
 
     @classmethod
     def load_trimesh(cls, path, device=None):
         mesh = cls()
 
         # device
         if device is None:
-            device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
+            device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
         mesh.device = device
 
         # use trimesh to load glb, assume only has one single RootMesh...
         _data = trimesh.load(path)
         if isinstance(_data, trimesh.Scene):
-                
+
             mesh_keys = list(_data.geometry.keys())
-            assert len(mesh_keys) == 1, f'{path} contains more than one meshes, not supported!'
+            assert (
+                len(mesh_keys) == 1
+            ), f"{path} contains more than one meshes, not supported!"
             _mesh = _data.geometry[mesh_keys[0]]
 
         elif isinstance(_data, trimesh.Trimesh):
             _mesh = _data
 
         else:
-            raise NotImplementedError(f'type {type(_data)} not supported!')
+            raise NotImplementedError(f"type {type(_data)} not supported!")
 
         # TODO: exception handling if no material
         _material = _mesh.visual.material
         if isinstance(_material, trimesh.visual.material.PBRMaterial):
             texture = np.array(_material.baseColorTexture).astype(np.float32) / 255
         elif isinstance(_material, trimesh.visual.material.SimpleMaterial):
-            texture = np.array(_material.to_pbr().baseColorTexture).astype(np.float32) / 255
+            texture = (
+                np.array(_material.to_pbr().baseColorTexture).astype(np.float32) / 255
+            )
         else:
-            raise NotImplementedError(f'material type {type(_material)} not supported!')
+            raise NotImplementedError(f"material type {type(_material)} not supported!")
 
-        print(f'[load_obj] load texture: {texture.shape}')
+        print(f"[load_obj] load texture: {texture.shape}")
         mesh.albedo = torch.tensor(texture, dtype=torch.float32, device=device)
 
         vertices = _mesh.vertices
         texcoords = _mesh.visual.uv
         texcoords[:, 1] = 1 - texcoords[:, 1]
         normals = _mesh.vertex_normals
 
         # trimesh only support vertex uv...
         faces = tfaces = nfaces = _mesh.faces
 
         mesh.v = torch.tensor(vertices, dtype=torch.float32, device=device)
-        mesh.vt = torch.tensor(texcoords, dtype=torch.float32, device=device) if len(texcoords) > 0 else None
-        mesh.vn = torch.tensor(normals, dtype=torch.float32, device=device) if len(normals) > 0 else None
+        mesh.vt = (
+            torch.tensor(texcoords, dtype=torch.float32, device=device)
+            if len(texcoords) > 0
+            else None
+        )
+        mesh.vn = (
+            torch.tensor(normals, dtype=torch.float32, device=device)
+            if len(normals) > 0
+            else None
+        )
 
         mesh.f = torch.tensor(faces, dtype=torch.int32, device=device)
-        mesh.ft = torch.tensor(tfaces, dtype=torch.int32, device=device) if texcoords is not None else None
-        mesh.fn = torch.tensor(nfaces, dtype=torch.int32, device=device) if normals is not None else None
+        mesh.ft = (
+            torch.tensor(tfaces, dtype=torch.int32, device=device)
+            if texcoords is not None
+            else None
+        )
+        mesh.fn = (
+            torch.tensor(nfaces, dtype=torch.int32, device=device)
+            if normals is not None
+            else None
+        )
 
         return mesh
-    
+
     # aabb
     def aabb(self):
         return torch.min(self.v, dim=0).values, torch.max(self.v, dim=0).values
 
     # unit size
     @torch.no_grad()
-    def auto_size(self): 
+    def auto_size(self):
         vmin, vmax = self.aabb()
         self.ori_center = (vmax + vmin) / 2
         self.ori_scale = 1.2 / torch.max(vmax - vmin).item()
         self.v = (self.v - self.ori_center) * self.ori_scale
 
     def auto_normal(self):
         i0, i1, i2 = self.f[:, 0].long(), self.f[:, 1].long(), self.f[:, 2].long()
@@ -226,32 +273,37 @@
         # Splat face normals to vertices
         vn = torch.zeros_like(self.v)
         vn.scatter_add_(0, i0[:, None].repeat(1, 3), face_normals)
         vn.scatter_add_(0, i1[:, None].repeat(1, 3), face_normals)
         vn.scatter_add_(0, i2[:, None].repeat(1, 3), face_normals)
 
         # Normalize, replace zero (degenerated) normals with some default value
-        vn = torch.where(dot(vn, vn) > 1e-20, vn, torch.tensor([0.0, 0.0, 1.0], dtype=torch.float32, device=vn.device))
+        vn = torch.where(
+            dot(vn, vn) > 1e-20,
+            vn,
+            torch.tensor([0.0, 0.0, 1.0], dtype=torch.float32, device=vn.device),
+        )
         vn = safe_normalize(vn)
 
         self.vn = vn
         self.fn = self.f
 
     def auto_uv(self, cache_path=None):
 
         # try to load cache
         if cache_path is not None:
-            cache_path = cache_path.replace('.obj', '_uv.npz')
+            cache_path = cache_path.replace(".obj", "_uv.npz")
 
         if cache_path is not None and os.path.exists(cache_path):
             data = np.load(cache_path)
-            vt_np, ft_np = data['vt'], data['ft']
+            vt_np, ft_np = data["vt"], data["ft"]
         else:
 
             import xatlas
+
             v_np = self.v.detach().cpu().numpy()
             f_np = self.f.detach().int().cpu().numpy()
             atlas = xatlas.Atlas()
             atlas.add_mesh(v_np, f_np)
             chart_options = xatlas.ChartOptions()
             chart_options.max_iterations = 4
             atlas.generate(chart_options=chart_options)
@@ -265,59 +317,59 @@
         ft = torch.from_numpy(ft_np.astype(np.int32)).to(self.device)
 
         self.vt = vt
         self.ft = ft
 
     def to(self, device):
         self.device = device
-        for name in ['v', 'f', 'vn', 'fn', 'vt', 'ft', 'albedo']:
+        for name in ["v", "f", "vn", "fn", "vt", "ft", "albedo"]:
             tensor = getattr(self, name)
             if tensor is not None:
                 setattr(self, name, tensor.to(device))
         return self
 
     # write to obj file
     def write(self, path):
 
-        mtl_path = path.replace('.obj', '.mtl')
-        albedo_path = path.replace('.obj', '_albedo.png')
+        mtl_path = path.replace(".obj", ".mtl")
+        albedo_path = path.replace(".obj", "_albedo.png")
 
         v_np = self.v.detach().cpu().numpy()
         vt_np = self.vt.detach().cpu().numpy() if self.vt is not None else None
         vn_np = self.vn.detach().cpu().numpy() if self.vn is not None else None
         f_np = self.f.detach().cpu().numpy()
         ft_np = self.ft.detach().cpu().numpy() if self.ft is not None else None
         fn_np = self.fn.detach().cpu().numpy() if self.fn is not None else None
 
         with open(path, "w") as fp:
-            fp.write(f'mtllib {os.path.basename(mtl_path)} \n')
+            fp.write(f"mtllib {os.path.basename(mtl_path)} \n")
 
             for v in v_np:
-                fp.write(f'v {v[0]} {v[1]} {v[2]} \n')
+                fp.write(f"v {v[0]} {v[1]} {v[2]} \n")
 
             for v in vt_np:
-                fp.write(f'vt {v[0]} {1 - v[1]} \n')
+                fp.write(f"vt {v[0]} {1 - v[1]} \n")
 
             for v in vn_np:
-                fp.write(f'vn {v[0]} {v[1]} {v[2]} \n')
+                fp.write(f"vn {v[0]} {v[1]} {v[2]} \n")
 
-            fp.write(f'usemtl defaultMat \n')
+            fp.write(f"usemtl defaultMat \n")
             for i in range(len(f_np)):
                 fp.write(
                     f'f {f_np[i, 0] + 1}/{ft_np[i, 0] + 1 if ft_np is not None else ""}/{fn_np[i, 0] + 1 if fn_np is not None else ""} \
                              {f_np[i, 1] + 1}/{ft_np[i, 1] + 1 if ft_np is not None else ""}/{fn_np[i, 1] + 1 if fn_np is not None else ""} \
                              {f_np[i, 2] + 1}/{ft_np[i, 2] + 1 if ft_np is not None else ""}/{fn_np[i, 2] + 1 if fn_np is not None else ""} \n'
                 )
 
         with open(mtl_path, "w") as fp:
-            fp.write(f'newmtl defaultMat \n')
-            fp.write(f'Ka 1 1 1 \n')
-            fp.write(f'Kd 1 1 1 \n')
-            fp.write(f'Ks 0 0 0 \n')
-            fp.write(f'Tr 1 \n')
-            fp.write(f'illum 1 \n')
-            fp.write(f'Ns 0 \n')
-            fp.write(f'map_Kd {os.path.basename(albedo_path)} \n')
+            fp.write(f"newmtl defaultMat \n")
+            fp.write(f"Ka 1 1 1 \n")
+            fp.write(f"Kd 1 1 1 \n")
+            fp.write(f"Ks 0 0 0 \n")
+            fp.write(f"Tr 1 \n")
+            fp.write(f"illum 1 \n")
+            fp.write(f"Ns 0 \n")
+            fp.write(f"map_Kd {os.path.basename(albedo_path)} \n")
 
         albedo = self.albedo.detach().cpu().numpy()
         albedo = (albedo * 255).astype(np.uint8)
-        cv2.imwrite(albedo_path, cv2.cvtColor(albedo, cv2.COLOR_RGB2BGR))
+        cv2.imwrite(albedo_path, cv2.cvtColor(albedo, cv2.COLOR_RGB2BGR))
```

### Comparing `kiui-0.1.5/kiui/vis.py` & `kiui-0.1.7/kiui/vis.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,35 +2,39 @@
 import numpy as np
 
 import matplotlib.cm as cm
 import matplotlib.pyplot as plt
 
 from .utils import lo
 
-def map_color(value, cmap_name='viridis', vmin=None, vmax=None):
+
+def map_color(value, cmap_name="viridis", vmin=None, vmax=None):
     # value: [N], float
     # return: RGB, [N, 3], float in [0, 1]
 
-    if vmin is None: vmin = value.min()
-    if vmax is None: vmax = value.max()
-    value = (value - vmin) / (vmax - vmin) # range in [0, 1]
-    cmap = cm.get_cmap(cmap_name) 
+    if vmin is None:
+        vmin = value.min()
+    if vmax is None:
+        vmax = value.max()
+    value = (value - vmin) / (vmax - vmin)  # range in [0, 1]
+    cmap = cm.get_cmap(cmap_name)
     rgb = cmap(value)[:, :3]  # will return rgba, we take only first 3 so we get rgb
     return rgb
 
+
 # visualize some 2D matrix, different from plot_image, this will keep the original range and plot channel-by-channel
 def plot_matrix(*xs):
     # x: [B, C, H, W], [C, H, W], or [H, W] torch.Tensor
     #    [B, H, W, C], [H, W, C], or [H, W] numpy.ndarray
 
     def _plot_matrix(matrix):
-            
+
         if isinstance(matrix, torch.Tensor):
             if len(matrix.shape) == 3:
-                matrix = matrix.permute(1,2,0).squeeze()
+                matrix = matrix.permute(1, 2, 0).squeeze()
             matrix = matrix.detach().cpu().numpy()
 
         lo(matrix)
 
         if len(matrix.shape) == 3:
             # per channel
             for i in range(matrix.shape[-1]):
@@ -42,38 +46,43 @@
 
     for x in xs:
         if len(x.shape) == 4:
             for i in range(x.shape[0]):
                 _plot_matrix(x[i])
         else:
             _plot_matrix(x)
-  
+
+
 # sequentially plot provided images
 def plot_image(*xs, normalize=False):
     # x: [B, 3, H, W], [3, H, W], [1, H, W] or [H, W] torch.Tensor
     #    [B, H, W, 3], [H, W, 3], [H, W, 1] or [H, W] numpy.ndarray
 
     def _plot_image(image):
 
         if isinstance(image, torch.Tensor):
             if len(image.shape) == 3:
-                image = image.permute(1,2,0).squeeze()
+                image = image.permute(1, 2, 0).squeeze()
             image = image.detach().cpu().numpy()
 
         lo(image)
 
         image = image.astype(np.float32)
-        
+
         # normalize
         if normalize:
-            image = (image - image.min(axis=0, keepdims=True)) / (image.max(axis=0, keepdims=True) - image.min(axis=0, keepdims=True) + 1e-8)
+            image = (image - image.min(axis=0, keepdims=True)) / (
+                image.max(axis=0, keepdims=True)
+                - image.min(axis=0, keepdims=True)
+                + 1e-8
+            )
 
         plt.imshow(image)
         plt.show()
-    
+
     for x in xs:
         if len(x.shape) == 4:
             for i in range(x.shape[0]):
                 _plot_image(x[i])
         else:
             _plot_image(x)
 
@@ -83,71 +92,86 @@
     # color: [N, 3/4]
 
     lo(pc)
 
     if color is None or color.shape[-1] == 3:
         # use o3d as it's better to control
         import open3d as o3d
+
         pcd = o3d.geometry.PointCloud()
         pcd.points = o3d.utility.Vector3dVector(pc)
         if color is not None:
             pcd.colors = o3d.utility.Vector3dVector(color)
         o3d.visualization.draw_geometries([pcd])
 
     else:
         import trimesh
+
         pc = trimesh.PointCloud(pc, color)
         # axis
         axes = trimesh.creation.axis(axis_length=4)
         # sphere
         box = trimesh.primitives.Box(extents=(2, 2, 2)).as_outline()
         box.colors = np.array([[128, 128, 128]] * len(box.entities))
 
         trimesh.Scene([pc, axes, box]).show()
-    
+
 
 def plot_poses(poses, size=0.05, bound=1, points=None, mesh=None):
     # poses: [B, 4, 4]
 
     lo(poses)
 
     import trimesh
+
     axes = trimesh.creation.axis(axis_length=4)
-    box = trimesh.primitives.Box(extents=[2*bound]*3).as_outline()
+    box = trimesh.primitives.Box(extents=[2 * bound] * 3).as_outline()
     box.colors = np.array([[128, 128, 128]] * len(box.entities))
     objects = [axes, box]
 
     if bound > 1:
-        unit_box = trimesh.primitives.Box(extents=[2]*3).as_outline()
+        unit_box = trimesh.primitives.Box(extents=[2] * 3).as_outline()
         unit_box.colors = np.array([[128, 128, 128]] * len(unit_box.entities))
         objects.append(unit_box)
 
     for pose in poses:
         # a camera is visualized with 8 line segments.
         pos = pose[:3, 3]
-        a = pos + size * pose[:3, 0] + size * pose[:3, 1] - size * pose[:3, 2]
-        b = pos - size * pose[:3, 0] + size * pose[:3, 1] - size * pose[:3, 2]
-        c = pos - size * pose[:3, 0] - size * pose[:3, 1] - size * pose[:3, 2]
-        d = pos + size * pose[:3, 0] - size * pose[:3, 1] - size * pose[:3, 2]
+        a = pos + size * pose[:3, 0] + size * pose[:3, 1] + size * pose[:3, 2]
+        b = pos - size * pose[:3, 0] + size * pose[:3, 1] + size * pose[:3, 2]
+        c = pos - size * pose[:3, 0] - size * pose[:3, 1] + size * pose[:3, 2]
+        d = pos + size * pose[:3, 0] - size * pose[:3, 1] + size * pose[:3, 2]
 
         dir = (a + b + c + d) / 4 - pos
         dir = dir / (np.linalg.norm(dir) + 1e-8)
         o = pos + dir * 3
 
-        segs = np.array([[pos, a], [pos, b], [pos, c], [pos, d], [a, b], [b, c], [c, d], [d, a], [pos, o]])
+        segs = np.array(
+            [
+                [pos, a],
+                [pos, b],
+                [pos, c],
+                [pos, d],
+                [a, b],
+                [b, c],
+                [c, d],
+                [d, a],
+                [pos, o],
+            ]
+        )
         segs = trimesh.load_path(segs)
         objects.append(segs)
 
     if points is not None:
 
         lo(points)
 
         colors = np.zeros((points.shape[0], 4), dtype=np.uint8)
-        colors[:, 2] = 255 # blue
-        colors[:, 3] = 30 # transparent
+        colors[:, 2] = 255  # blue
+        colors[:, 3] = 30  # transparent
         objects.append(trimesh.PointCloud(points, colors))
 
     if mesh is not None:
         objects.append(mesh)
 
     scene = trimesh.Scene(objects)
     scene.set_camera(distance=bound, center=[0, 0, 0])
```

