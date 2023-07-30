# Comparing `tmp/problem180meridian-0.0.1.tar.gz` & `tmp/problem180meridian-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "problem180meridian-0.0.1.tar", last modified: Mon Jul 17 18:03:47 2023, max compression
+gzip compressed data, was "problem180meridian-0.1.0.tar", last modified: Sun Jul 30 14:24:23 2023, max compression
```

## Comparing `problem180meridian-0.0.1.tar` & `problem180meridian-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 18:03:47.727336 problem180meridian-0.0.1/
--rw-rw-rw-   0        0        0    11558 2023-07-17 17:29:47.000000 problem180meridian-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      858 2023-07-17 18:03:47.727336 problem180meridian-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       81 2023-07-06 15:07:17.000000 problem180meridian-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 18:03:47.715519 problem180meridian-0.0.1/problem180meridian/
--rw-rw-rw-   0        0        0      303 2023-07-17 16:51:43.000000 problem180meridian-0.0.1/problem180meridian/__init__.py
--rw-rw-rw-   0        0        0     7059 2023-07-17 16:29:54.000000 problem180meridian-0.0.1/problem180meridian/problem180meridian.py
-drwxrwxrwx   0        0        0        0 2023-07-17 18:03:47.727336 problem180meridian-0.0.1/problem180meridian.egg-info/
--rw-rw-rw-   0        0        0      858 2023-07-17 18:03:47.000000 problem180meridian-0.0.1/problem180meridian.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-07-17 18:03:47.000000 problem180meridian-0.0.1/problem180meridian.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 18:03:47.000000 problem180meridian-0.0.1/problem180meridian.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-17 18:03:47.000000 problem180meridian-0.0.1/problem180meridian.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 18:03:47.729585 problem180meridian-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1262 2023-07-17 18:03:41.000000 problem180meridian-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:24:23.479513 problem180meridian-0.1.0/
+-rw-rw-rw-   0        0        0    11558 2023-07-17 17:29:47.000000 problem180meridian-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2660 2023-07-30 14:24:23.480867 problem180meridian-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1839 2023-07-30 14:06:53.000000 problem180meridian-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 14:24:23.393700 problem180meridian-0.1.0/problem180meridian/
+-rw-rw-rw-   0        0        0      212 2023-07-30 13:57:13.000000 problem180meridian-0.1.0/problem180meridian/__init__.py
+-rw-rw-rw-   0        0        0     6958 2023-07-30 14:08:03.000000 problem180meridian-0.1.0/problem180meridian/problem180meridian.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:24:23.442660 problem180meridian-0.1.0/problem180meridian.egg-info/
+-rw-rw-rw-   0        0        0     2660 2023-07-30 14:24:22.000000 problem180meridian-0.1.0/problem180meridian.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-07-30 14:24:23.000000 problem180meridian-0.1.0/problem180meridian.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 14:24:22.000000 problem180meridian-0.1.0/problem180meridian.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-30 14:24:22.000000 problem180meridian-0.1.0/problem180meridian.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-30 14:24:22.000000 problem180meridian-0.1.0/problem180meridian.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 14:24:23.489383 problem180meridian-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1304 2023-07-30 13:57:13.000000 problem180meridian-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 14:24:23.478497 problem180meridian-0.1.0/test/
+-rw-rw-rw-   0        0        0      913 2023-07-29 16:05:14.000000 problem180meridian-0.1.0/test/test_Geometries.py
+-rw-rw-rw-   0        0        0     1875 2023-07-29 16:07:21.000000 problem180meridian-0.1.0/test/test_cross180.py
+-rw-rw-rw-   0        0        0     1163 2023-07-29 16:05:14.000000 problem180meridian-0.1.0/test/test_split180.py
```

### Comparing `problem180meridian-0.0.1/LICENSE` & `problem180meridian-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `problem180meridian-0.0.1/problem180meridian/problem180meridian.py` & `problem180meridian-0.1.0/problem180meridian/problem180meridian.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,212 +1,221 @@
 import numpy as np
-from osgeo import ogr
 
+try:
+    from osgeo import ogr
+except ImportError:
+    import ogr
 
-class GeometryHierarchyError(Exception):
+
+__all__ = [
+    'Geometries', 'check180', 'cross180', 'split180', 'split180_multipolygon'
+]
+
+
+class GeometriesError(Exception):
 
     def __init__(self, *args, **kwargs):
         pass
 
 
 # Arranges a set of polygons to find out which of them are within others
 # If any of them is within others they are cut off while creating a new
 # multipolygon
-class GeometryHierarchy:
+class Geometries:
 
-    def __init__(self, *geometries, main_geometry=None, level=0):
+    def __init__(self, *geom_tuple, main_geom=None, level=0):
 
-        assert (main_geometry is None) or isinstance(main_geometry, ogr.Geometry)
+        assert (main_geom is None) or isinstance(main_geom, ogr.Geometry)
 
-        self.main_geometry = main_geometry
+        self.main_geometry = main_geom
         self.level = level
         self.geometries = []
 
-        for geometry in geometries:
-            self.joinGeometry(geometry)
+        for geometry in geom_tuple:
+            self.join_geometry(geometry)
 
     def __str__(self):
 
         if self.main_geometry is None:
             main_wkt = 'No main geometry'
         else:
             main_wkt = self.main_geometry.ExportToWkt()
 
         tab = '\n\t' + self.level*'\t'
 
         return tab.join([main_wkt] + [str(h) for h in self.geometries])
 
-    def checkMainGeometry(self, geometry):
+    def check_main_geometry(self, geometry):
 
         if self.main_geometry is not None:
 
             if geometry.Within(self.main_geometry):
                 # print('Geometry within')
                 return 0
 
             elif self.main_geometry.Within(geometry):
                 # print('Hierarchy within')
                 return 2
 
             elif geometry.Intersects(self.main_geometry):
-                raise GeometryHierarchyError('Unexpected intersection')
+                raise GeometriesError('Unexpected intersection')
 
             else:
                 # print('Out of main geometry')
                 return 1
 
-    def joinGeometry(self, geometry):
+    def join_geometry(self, geometry):
 
         assert isinstance(geometry, ogr.Geometry)
 
-        main_geometry_check = self.checkMainGeometry(geometry)
+        main_geometry_check = self.check_main_geometry(geometry)
 
         if main_geometry_check:
             return main_geometry_check
 
-        new_hierarchy = GeometryHierarchy(main_geometry=geometry,
-                                          level=self.level + 1)
+        new_geoms = Geometries(main_geom=geometry, level=self.level + 1)
         separate = True
 
         for i in range(len(self.geometries)-1, -1, -1):
 
-            hierarchy = self.geometries[i]
-            separate = self.geometries[i].joinGeometry(geometry)
+            self_geoms = self.geometries[i]
+            separate = self.geometries[i].join_geometry(geometry)
 
             if separate == 0:
                 # print('Joined hierarchy')
                 return 0
 
             elif separate == 2:
-                # Doesn't check if there're intersections within new_hierarchy
+                # Doesn't check if there are intersections within new_geoms
                 # Need to fix if used for other polygons but raster footprints!
-                new_hierarchy.geometries.append(self.geometries.pop(i))
+                new_geoms.geometries.append(self.geometries.pop(i))
 
-            elif geometry.Intersects(hierarchy.main_geometry):
-                raise GeometryHierarchyError('Unexpected intersection')
+            elif geometry.Intersects(self_geoms.main_geometry):
+                raise GeometriesError('Unexpected intersection')
 
         if separate:
-            self.geometries.append(new_hierarchy)
+            self.geometries.append(new_geoms)
             return 0
 
-        raise GeometryHierarchyError('Geometry not processed')
+        raise GeometriesError('Geometry not processed')
 
-    def Multipolygon(self):
+    def multipolygon(self):
 
         if self.main_geometry is not None:
             multipolygon = self.main_geometry
-            for hierarhy in self.geometries:
-                multipolygon = multipolygon.Difference(hierarhy.Multipolygon())
+            for geoms in self.geometries:
+                multipolygon = multipolygon.Difference(geoms.multipolygon())
 
         elif len(self.geometries) != 0:
-            multipolygon = self.geometries[0].Multipolygon()
-            for hierarhy in self.geometries[1:]:
-                multipolygon = multipolygon.Union(hierarhy.Multipolygon())
+            multipolygon = self.geometries[0].multipolygon()
+            for geoms in self.geometries[1:]:
+                multipolygon = multipolygon.Union(geoms.multipolygon())
 
         else:
             multipolygon = ogr.Geometry(6)
 
         return multipolygon
 
 
 # Returns True if value is positive or zero and False if it is negative
-def arrayNotNegative(array):
+def array_not_negative(array):
     return np.sign(np.sign(array) + 1).astype(bool)
 
 
 # Checks if any segment in a pair of coordinates crosses 180th meridian
 # It's considered so if abs(x2 - x1) > abs(x2_1 - x1_1) where
 # xi_1 = xi + (xi < 0) * 360
 # If any crossing is found a check_array is returned where crossing pairs
 # are marked as True
-def check180lon(coordinates):
+def check180(coordinates):
 
     longitudes = np.array([p[0] for p in coordinates])
-    signs = arrayNotNegative(longitudes)
+    signs = array_not_negative(longitudes)
 
     if list(np.unique(signs)) == [0, 1]:
         distances = abs(longitudes[1:] - longitudes[:-1])
         longitudes_fixed = longitudes + ((signs == 0) * 360)
         distances_fixed = abs(longitudes_fixed[1:] - longitudes_fixed[:-1])
         # Need to add small value below to avoid Python calculation errors
-        check_array = arrayNotNegative(distances_fixed - distances + 0.000001)
+        check_array = array_not_negative(distances_fixed - distances + 0.000001)
         return True, check_array
     else:
         return False, None
 
 
-# Creates coordinates for two points in a segment crossing 180th meridian
-# Setting distance_from180lon one can separate them from each other and
+# Create coordinates for two points in a segment crossing 180th meridian
+# Setting lon_buffer one can separate them from each other and
 # the meridian itself
-def cross180lon(coord1, coord2, distance_from_180lon = 0):
+def cross180(coord1, coord2, lon_buffer=0):
 
     if coord1[0] > 0:
         assert coord2[0] < 0
         img_lon2 = coord2[0] + 360
-        new_lon1 = 180 - abs(distance_from_180lon)
+        new_lon1 = 180 - abs(lon_buffer)
     else:
         assert coord2[0] >= 0
         img_lon2 = coord2[0] - 360
-        new_lon1 = abs(distance_from_180lon) - 180
+        new_lon1 = abs(lon_buffer) - 180
 
     if (img_lon2 - coord1[0]) == 0:
-        angle_coef = 1
+        angle_coefficient = 1
     else:
-        angle_coef = (coord2[1] - coord1[1]) / (img_lon2 - coord1[0])
+        angle_coefficient = (coord2[1] - coord1[1]) / (img_lon2 - coord1[0])
 
     new_lon2 = (-1) * new_lon1
-    new_lat1 = coord1[1] + angle_coef * (new_lon1 - coord1[0])
-    new_lat2 = coord2[1] + angle_coef * (new_lon2 - coord2[0])
+    new_lat1 = coord1[1] + angle_coefficient * (new_lon1 - coord1[0])
+    new_lat2 = coord2[1] + angle_coefficient * (new_lon2 - coord2[0])
 
     return (new_lon1, new_lat1), (- new_lon1, new_lat2)
 
 
 # Split polygon geometry by the 180th meridian creating a multipolygon
-def split180lon(coordinates, check, distance_from_180lon=0):
+def split180(coordinates, check, lon_buffer=0):
 
     assert len(coordinates) - 1 == len(check)
     assert coordinates[0] == coordinates[-1]
-    chains=[[coordinates[0]]]
+    chains = [[coordinates[0]]]
 
     for i in range(len(check)):
 
         if check[i]:
             chains[-1].append(coordinates[i+1])
         else:
-            new_coord1, new_coord2 = cross180lon(*tuple(coordinates[i:i+2]),
-                                    distance_from_180lon=distance_from_180lon)
+            new_coord1, new_coord2 = cross180(
+                *tuple(coordinates[i:i + 2]),
+                lon_buffer=lon_buffer)
             chains[-1].append(new_coord1)
             chains.append([new_coord2, coordinates[i+1]])
 
     # need to finish all the polygon chains to make correct wkt
     if len(chains) > 1:
         chains[0].extend(chains.pop())
         for chain in chains[1:]:
             chain.append(chain[0])
 
     wkt_list = ['MULTIPOLYGON (((%s)))' % ','.join(['%f %f' %
                 (p[0], p[1]) for p in chain]) for chain in chains]
 
-    polygons = [ogr.Geometry(wkt = wkt) for wkt in wkt_list]
-    hierarchy = GeometryHierarchy(*polygons)
-    multipolygon = hierarchy.Multipolygon()
+    polygons = [ogr.Geometry(wkt=wkt) for wkt in wkt_list]
+    geoms = Geometries(*polygons)
+    multipolygon = geoms.multipolygon()
 
     return multipolygon
 
 
 # Split polygon/multipolygon geometry by the 180th meridian
-def split180lonMultipolygon(coordinates, distance_from_180lon=0):
+def split180_multipolygon(coordinates, lon_buffer=0):
 
-    hierarchy = GeometryHierarchy()
+    geoms = Geometries()
 
     for poly in coordinates:
 
-        cross, check = check180lon(coordinates[0])
+        cross, check = check180(coordinates[0])
 
         if cross:
-            hierarchy.joinGeometry(split180lon(poly, check,
-                            distance_from_180lon=distance_from_180lon))
+            geoms.join_geometry(split180(poly, check, lon_buffer=lon_buffer))
         else:
-            hierarchy.joinGeometry(ogr.Geometry(wkt='MULTIPOLYGON (((%s)))' %
-                            ','.join(['%f %f' % (p[0], p[1]) for p in poly])))
+            point_str = ','.join(['%f %f' % (p[0], p[1]) for p in poly])
+            wkt = f"MULTIPOLYGON ((({point_str})))"
+            geoms.join_geometry(ogr.Geometry(wkt=wkt))
 
-    return hierarchy.Multipolygon()
+    return geoms.multipolygon()
```

### Comparing `problem180meridian-0.0.1/setup.py` & `problem180meridian-0.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,45 +7,42 @@
 
 :authors: sergsadkov
 :license: Apache License, Version 2.0, see LICENSE file
 :copyright: (c) 2023 sergsadkov
 """
 
 
-version = '0.0.1'
+version = '0.1.0'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='problem180meridian',
     version=version,
 
     author='sergsadkov',
     author_email='sergsadkov@gmail.com',
 
-    description=(
-        u'Python module to fix 180 degree crossing issue for vector geodata',
-    ),
+    description=u'Fixes 180 degree crossing issue for vector geodata',
 
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     url='https://github.com/sergsadkov/problem180meridian',
     download_url='https://github.com/sergsadkov/problem180meridian/archive/main.zip',
 
     license='Apache License, Version 2.0, see LICENSE file',
 
     packages=['problem180meridian'],
-    install_requires=[],
+    install_requires=['numpy', 'GDAL'],
 
     classifiers=[
-
-
+        'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
         'Intended Audience :: End Users/Desktop',
         'Intended Audience :: Developers',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: Implementation :: CPython',
     ]
-)
+)
```

