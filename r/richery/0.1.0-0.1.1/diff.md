# Comparing `tmp/richery-0.1.0.tar.gz` & `tmp/richery-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "richery-0.1.0.tar", last modified: Fri Jul 28 19:36:43 2023, max compression
+gzip compressed data, was "richery-0.1.1.tar", last modified: Sun Jul 30 16:36:24 2023, max compression
```

## Comparing `richery-0.1.0.tar` & `richery-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:36:43.682152 richery-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-28 19:36:30.000000 richery-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-28 19:36:43.682152 richery-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-28 19:36:30.000000 richery-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-28 19:36:30.000000 richery-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:36:43.682152 richery-0.1.0/richery/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-28 19:36:30.000000 richery-0.1.0/richery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-28 19:36:30.000000 richery-0.1.0/richery/ansitool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8995 2023-07-28 19:36:30.000000 richery-0.1.0/richery/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-07-28 19:36:30.000000 richery-0.1.0/richery/colordef.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-28 19:36:30.000000 richery-0.1.0/richery/textwork.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:36:43.682152 richery-0.1.0/richery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-28 19:36:43.000000 richery-0.1.0/richery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-28 19:36:43.000000 richery-0.1.0/richery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:36:43.000000 richery-0.1.0/richery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 19:36:43.000000 richery-0.1.0/richery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-28 19:36:43.000000 richery-0.1.0/richery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 19:36:43.682152 richery-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:36:24.393959 richery-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-30 16:36:13.000000 richery-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-30 16:36:24.393959 richery-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-30 16:36:13.000000 richery-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-30 16:36:13.000000 richery-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:36:24.393959 richery-0.1.1/richery/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-30 16:36:13.000000 richery-0.1.1/richery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-30 16:36:13.000000 richery-0.1.1/richery/ansitool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-07-30 16:36:13.000000 richery-0.1.1/richery/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-07-30 16:36:13.000000 richery-0.1.1/richery/colordef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-30 16:36:13.000000 richery-0.1.1/richery/textwork.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 16:36:24.393959 richery-0.1.1/richery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-30 16:36:24.000000 richery-0.1.1/richery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-30 16:36:24.000000 richery-0.1.1/richery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 16:36:24.000000 richery-0.1.1/richery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-30 16:36:24.000000 richery-0.1.1/richery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-30 16:36:24.000000 richery-0.1.1/richery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 16:36:24.393959 richery-0.1.1/setup.cfg
```

### Comparing `richery-0.1.0/LICENSE` & `richery-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `richery-0.1.0/richery/ansitool.py` & `richery-0.1.1/richery/ansitool.py`

 * *Files identical despite different names*

### Comparing `richery-0.1.0/richery/canvas.py` & `richery-0.1.1/richery/canvas.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         x0, y0, w0, h0 = base
         x1, y1 = target.xy
         return cls(x1 + x0, y1 + y0, w0, h0)
 
     def remap(self, *rect: "Rect") -> "Rect":
         """Remap this rectangle to another rectangle"""
         return reduce(self._remap, (self, *rect))
-    
+
     def __contains__(self, point: Tuple[int, int]) -> bool:
         _x, _y = point
         return (
             self.x <= _x <= self.x + self.w
             and self.y <= _y <= self.y + self.h
         )
 
@@ -140,23 +140,23 @@
 
     def find_relative_font(
         self, delta: int = 0, font: Optional[GenericFont] = None
     ) -> GenericFont:
         ext = tuple(x for x in self._tuple() if x is not None)
         _font = self.Regular if font is None else font
         found = ext.index(_font) + delta
-        return ext[max(0, min(len(ext), found))]
+        return ext[max(0, min(len(ext) - 1, found))]
 
     def __getitem__(self, _i: int) -> GenericFont:
         if 0 <= _i < 10:
             return self._select(_i)
         if 100 <= _i <= 900:
             return self._select(round(_i / 100))
         raise IndexError("font index only supports [0..9] and [100..900]")
-    
+
     def __add__(self, other: int) -> GenericFont:
         return self.find_relative_font(other)
 
 
 @dataclass
 class TextDrawState:
     land: Rect
@@ -292,8 +292,8 @@
 
     def text(
         self, state: TextDrawState, text: str,
         *,
         justify: bool = True
     ) -> None:
         for lns in text.splitlines():
-            self._text(state, lns, justify=justify)
+            self._text(state, lns, justify=justify)
```

### Comparing `richery-0.1.0/richery/colordef.py` & `richery-0.1.1/richery/colordef.py`

 * *Files identical despite different names*

### Comparing `richery-0.1.0/richery/textwork.py` & `richery-0.1.1/richery/textwork.py`

 * *Files identical despite different names*

