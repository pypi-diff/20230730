# Comparing `tmp/nichord-0.1.8.tar.gz` & `tmp/nichord-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nichord-0.1.8.tar", last modified: Thu Jul 27 14:53:22 2023, max compression
+gzip compressed data, was "nichord-0.1.9.tar", last modified: Sun Jul 30 03:02:53 2023, max compression
```

## Comparing `nichord-0.1.8.tar` & `nichord-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 14:53:22.699819 nichord-0.1.8/
--rw-rw-rw-   0        0        0     1290 2023-07-27 14:53:22.698818 nichord-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0    10897 2023-07-23 20:57:39.000000 nichord-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 14:53:22.693817 nichord-0.1.8/nichord/
--rw-rw-rw-   0        0        0      756 2022-11-12 03:49:12.000000 nichord-0.1.8/nichord/__init__.py
--rw-rw-rw-   0        0        0    33895 2022-11-13 20:04:28.000000 nichord-0.1.8/nichord/chord.py
--rw-rw-rw-   0        0        0     4893 2022-11-13 19:54:36.000000 nichord-0.1.8/nichord/combine.py
--rw-rw-rw-   0        0        0      482 2022-05-22 13:31:30.000000 nichord-0.1.8/nichord/convert.py
--rw-rw-rw-   0        0        0     5639 2023-07-23 21:52:21.000000 nichord-0.1.8/nichord/coord_labeler.py
--rw-rw-rw-   0        0        0     5731 2022-11-12 03:52:39.000000 nichord-0.1.8/nichord/glassbrain.py
--rw-rw-rw-   0        0        0     2156 2023-07-24 20:52:49.000000 nichord-0.1.8/nichord/patch_RendererAgg.py
--rw-rw-rw-   0        0        0     8678 2023-07-23 21:52:21.000000 nichord-0.1.8/nichord/peak.py
-drwxrwxrwx   0        0        0        0 2023-07-27 14:53:22.697818 nichord-0.1.8/nichord.egg-info/
--rw-rw-rw-   0        0        0     1290 2023-07-27 14:53:22.000000 nichord-0.1.8/nichord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-07-27 14:53:22.000000 nichord-0.1.8/nichord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 14:53:22.000000 nichord-0.1.8/nichord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-07-27 14:53:22.000000 nichord-0.1.8/nichord.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-27 14:53:22.000000 nichord-0.1.8/nichord.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 14:53:22.699819 nichord-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1806 2023-07-27 14:51:12.000000 nichord-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 03:02:53.714777 nichord-0.1.9/
+-rw-rw-rw-   0        0        0     1269 2023-07-30 03:02:53.713777 nichord-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    10845 2023-07-30 01:34:33.000000 nichord-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 03:02:53.709775 nichord-0.1.9/nichord/
+-rw-rw-rw-   0        0        0      756 2022-11-12 03:49:12.000000 nichord-0.1.9/nichord/__init__.py
+-rw-rw-rw-   0        0        0    33895 2022-11-13 20:04:28.000000 nichord-0.1.9/nichord/chord.py
+-rw-rw-rw-   0        0        0     4893 2022-11-13 19:54:36.000000 nichord-0.1.9/nichord/combine.py
+-rw-rw-rw-   0        0        0      482 2022-05-22 13:31:30.000000 nichord-0.1.9/nichord/convert.py
+-rw-rw-rw-   0        0        0     5683 2023-07-30 02:58:52.000000 nichord-0.1.9/nichord/coord_labeler.py
+-rw-rw-rw-   0        0        0     5731 2022-11-12 03:52:39.000000 nichord-0.1.9/nichord/glassbrain.py
+-rw-rw-rw-   0        0        0     2156 2023-07-24 20:52:49.000000 nichord-0.1.9/nichord/patch_RendererAgg.py
+drwxrwxrwx   0        0        0        0 2023-07-30 03:02:53.712777 nichord-0.1.9/nichord.egg-info/
+-rw-rw-rw-   0        0        0     1269 2023-07-30 03:02:53.000000 nichord-0.1.9/nichord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-07-30 03:02:53.000000 nichord-0.1.9/nichord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 03:02:53.000000 nichord-0.1.9/nichord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-30 03:02:53.000000 nichord-0.1.9/nichord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-30 03:02:53.000000 nichord-0.1.9/nichord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 03:02:53.714777 nichord-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1877 2023-07-30 03:02:19.000000 nichord-0.1.9/setup.py
```

### Comparing `nichord-0.1.8/PKG-INFO` & `nichord-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: nichord
-Version: 0.1.8
+Version: 0.1.9
 Summary: Creates chord diagrams for connectivity/graph data
 Home-page: https://github.com/paulcbogdan/NiChord
 Author: paulcbogdan
 Author-email: paulcbogdan@gmail.com
 License: MIT
 Keywords: plotting,fmri,plotting,chord
-Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 
 `NiChord` is a Python package for visualizing functional connectivity data. This package was inspired by [NeuroMArVL](https://immersive.erc.monash.edu/neuromarvl/?example=40496078-effa-4ac3-9d3e-cb7f946e7dd1_137.147.133.145), an online visualization tool.
 
 The code can function with any configuration of edges and labels specified by the user.
 
 The glass brain diagrams (left & middle) rely on the plotting tools from [nilearn](https://nilearn.github.io/modules/generated/nilearn.plotting.plot_connectome.html), whereas the chord diagram (right) is made from scratch by drawing shapes in [matplotlib](https://matplotlib.org/). Most of the code, here, is dedicated to the chord diagrams.
 
 This package additionally provides code to help assign labels to nodes based on their anatomical location.
 
 To find out more about the package and see an example, see its [GitHub repo](https://github.com/paulcbogdan/NiChord).
-
```

### Comparing `nichord-0.1.8/README.md` & `nichord-0.1.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -32,53 +32,55 @@
 
 The examples above were constructed by saving separate images for the chord and
 glass brain diagrams and then combining the images.
 
 ### Input variables
 Edges are specified as a list of tuples, (i, j), where i and j are indices
 representing the two nodes making up the edge.
-```
+
+```Python
 edges = [(0, 1), (0, 2), (1, 5), (3, 5), (4, 6), (2, 7), (6, 7)]
 ```
 
 Each node index should also correspond to a coordinate in MNI space:
-```
+```Python
 coords = [[-24, -99, -12], [51, -3, -15], [-15, -70, 30], [21, 39, 39],
           [21, -66, 48], [54, 33, 12], [-33, 3, 3], [57, -45, 12]]
 ```
 
 These coordinates can be used to construct a dictionary, mapping each node index
 to a network label (by default, network labels are based on the 
 [Yeo et al. (2011) atlas](https://journals.physiology.org/doi/full/10.1152/jn.00338.2011)):
 
-```
+```Python
 from nichord.coord_labeler import get_idx_to_label
 idx_to_label = get_idx_to_label(coords, atlas='yeo')
 ```
 
 Or a dictionary can be defined manually:
 
-```
+```Python
 idx_to_label = {0: 'Visual', 1: 'DMN', 2: 'Visual', 3: 'DMN', 
                 4: 'DAN', 5: 'FPCN', 6: 'VAN', 7: 'VAN'}
 ```
 
 Each edge may be associated with a weight. Weights are defined as a list of 
 length equal to the number of edges (if `edge_weights = None`, then grey edges are.
 plotted).
 
-```
+```Python
 edge_weights = [-0.3, -0.5, 0.7, 0.5, -0.2, 0.3, 0.8]
 ```
 
 ### Plotting
 
 These variables and a filepath can then be 
 passed to create the chord diagram:
-```
+
+```Python
 from nichord.chord import plot_chord
 
 fp_chord = 'ex0_good.png' # if None, chord diagram can be opened in a matplotlib
                           # window with matplotlib.pyplot.show()
 plot_chord(idx_to_label, edges, edge_weights=edge_weights, 
     fp_chord=fp_chord,
     linewidths=15, alphas = 0.9, do_ROI_circles=True, 
@@ -91,28 +93,30 @@
   If no filepath is passed, the diagram will be opened in a matplotlib window.
 </p>
 
 
 Plotting the glass brain involves the same variables (note that the colors of 
 the glass brain nodes should correspond to the same colors as the chord network 
 labels)
-```
+
+```Python
 from nichord.glassbrain import plot_glassbrain
 
 fp_glass = 'ex0_glassbrain.png'
 plot_glassbrain(idx_to_label, edges, edge_weights, fp_glass,
                 coords, linewidths=15, node_size=17)
 ```
 
 <p align="center">
   <img src="example\glass\ex0_glass.png" />
 </p>
 
 Finally, to combine the figures above:
-```
+
+```Python
 from nichord.combine import combine_imgs
 
 fp_combined = 'ex0_combined.png'
 combine_imgs(fp_glass, fp_chord, fp_combined)
 ```
 
 Notably, these functions have many other optional variables (e.g., passing
@@ -130,95 +134,96 @@
 ### Plotting everything at once
 
 You can also use `combine.plot_and_combine` to do `plot_chord`, 
 `plot_glassbrain`, and `combine_image` with a single function. 
 `plot_and_combine` will create (if needed) and use directories `chord` and 
 `glass` wherever you specify the combined image to be made with `dir_out`.
 
-```
-    dir_out = 'example'
-    fn = 'ex1.png'
-    plot_and_combine(dir_out, fn, idx_to_label, edges,
-                     edge_weights=edge_weights, coords=power_coords,
-                     network_order=network_order, network_colors=network_colors,
-                     )
+```Python
+dir_out = 'example'
+fn = 'ex1.png'
+plot_and_combine(dir_out, fn, idx_to_label, edges,
+                 edge_weights=edge_weights, coords=power_coords,
+                 network_order=network_order, network_colors=network_colors,
+                 )
 ```
 
 You can pass `plot_and_combine` some `chord_kwargs=` or `glass_kwargs=` to 
 adjust the appearance of the chord diagram or glass brain, like above. These two
 examples here do this and also show new features added in November 2022. The
 one below shows how you can add a title and give the chord diagram a black 
 background:
-```
-    dir_out = 'example'
-    fn = r'ex1_black_BG.png'
-    chord_kwargs = {'black_BG': True}
-    plot_and_combine(dir_out, fn, idx_to_label, edges,
-                     edge_weights=edge_weights, coords=power_coords,
-                     network_order=network_order, network_colors=network_colors,
-                     chord_kwargs=chord_kwargs, title='Example 1b (black)')
+
+```Python
+dir_out = 'example'
+fn = r'ex1_black_BG.png'
+chord_kwargs = {'black_BG': True}
+plot_and_combine(dir_out, fn, idx_to_label, edges,
+                 edge_weights=edge_weights, coords=power_coords,
+                 network_order=network_order, network_colors=network_colors,
+                 chord_kwargs=chord_kwargs, title='Example 1b (black)')
 ```
 <p align="center">
   <img src="example\ex1_black_BG.png" />
 </p>
 
 Here is another example. This one shows how setting linewidth = 0 causes no 
 lines to be plotted on the glass brain. This may be useful in combination
 with setting a node sizes as a list, which casues nodes on the glassbrain to be
 plotted in sizes specified. 
 
-```
-    fn = r'ex1_count.png'
-    chord_kwargs = {'plot_count': True}
-    n_nodes = len(set([i for i, j in edges] + [j for i, j in edges]))
-    glass_kwargs = {'linewidths': 0.,
-                    'node_size': list(range(1, n_nodes+1))}
-    plot_and_combine(dir_out, fn, idx_to_label, edges,
-                     edge_weights=edge_weights, coords=power_coords,
-                     network_order=network_order, network_colors=network_colors,
-                     chord_kwargs=chord_kwargs, glass_kwargs=glass_kwargs,
-                     title='Example 1c (count)')
+```Python
+fn = r'ex1_count.png'
+chord_kwargs = {'plot_count': True}
+n_nodes = len(set([i for i, j in edges] + [j for i, j in edges]))
+glass_kwargs = {'linewidths': 0.,
+                'node_size': list(range(1, n_nodes+1))}
+plot_and_combine(dir_out, fn, idx_to_label, edges,
+                 edge_weights=edge_weights, coords=power_coords,
+                 network_order=network_order, network_colors=network_colors,
+                 chord_kwargs=chord_kwargs, glass_kwargs=glass_kwargs,
+                 title='Example 1c (count)')
 ```
 
 <p align="center">
   <img src="example\ex1_count.png" />
 </p>
 
 
 Final example, which shows other features (you can plot little circles on the
 chord diagrams where the arcs start): 
 
-```
-    fn = r'ex2.png'
-    edges = [(32, 12), (32, 48), (33, 48), (101, 105), (105, 219), (201, 33),
-             (32, 105)]
-    edge_weights = [-0.3, -0.5, 0.7, 0.5, -0.2, 0.3, 0.8]
-
-    chord_kwargs = {'alphas': 0.9, 'linewidths': 15, 'do_ROI_circles': True,
-                    'do_ROI_circles_specific': True, 'ROI_circle_radius': 0.02,
-                    'arc_setting': False}
-    glass_kwargs = {'linewidths': 15, 'node_size': 17}
-    plot_and_combine(dir_out, fn, idx_to_label, edges,
-                     edge_weights=edge_weights, coords=power_coords,
-                     network_order=network_order, network_colors=network_colors,
-                     chord_kwargs=chord_kwargs, glass_kwargs=glass_kwargs)
+```Python
+fn = r'ex2.png'
+edges = [(32, 12), (32, 48), (33, 48), (101, 105), (105, 219), (201, 33),
+         (32, 105)]
+edge_weights = [-0.3, -0.5, 0.7, 0.5, -0.2, 0.3, 0.8]
+
+chord_kwargs = {'alphas': 0.9, 'linewidths': 15, 'do_ROI_circles': True,
+                'do_ROI_circles_specific': True, 'ROI_circle_radius': 0.02,
+                'arc_setting': False}
+glass_kwargs = {'linewidths': 15, 'node_size': 17}
+plot_and_combine(dir_out, fn, idx_to_label, edges,
+                 edge_weights=edge_weights, coords=power_coords,
+                 network_order=network_order, network_colors=network_colors,
+                 chord_kwargs=chord_kwargs, glass_kwargs=glass_kwargs)
 ```
 
 <p align="center">
   <img src="example\ex2.png"/>
 </p>
 
 
 ### Convenience functions
 
 For convenience, the function `convert.convert_matrix(matrix)` is provided, which
 takes a matrix as input and returns two lists corresponding to edges and 
 edge_weights.
 
-```
+```Python
 from nichord.convert import convert_matrix
 
 matrix = [[0, 0.5, 0.2], [0.5, 0, -0.2], [0.2, -0.2, 0]]
 edges, edge_weights = convert_matrix(matrix)
 ```
 
 ### Note
```

### Comparing `nichord-0.1.8/nichord/__init__.py` & `nichord-0.1.9/nichord/__init__.py`

 * *Files identical despite different names*

### Comparing `nichord-0.1.8/nichord/chord.py` & `nichord-0.1.9/nichord/chord.py`

 * *Files identical despite different names*

### Comparing `nichord-0.1.8/nichord/combine.py` & `nichord-0.1.9/nichord/combine.py`

 * *Files identical despite different names*

### Comparing `nichord-0.1.8/nichord/coord_labeler.py` & `nichord-0.1.9/nichord/coord_labeler.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,16 +25,16 @@
     :param max_dist: If search_closest == True, max_dist corresponds to the
         distance that will be searched before using "Uncertain."
     :param must_have: used to filter what labels are considered valid. see
         find_closest(...)
     :return:
     """
 
-    from nichord.peak import read_atlas_peak # import statements here
-                                             # to speed things up
+    from atlasreader.atlasreader import read_atlas_peak # import statements here
+                                                        # to speed things up
     idx_to_label = {}
     if atlas.lower() == 'yeo':
         atlas = get_yeo_atlas()
 
     for idx, (x, y, z) in enumerate(coords):
         if search_closest:
             region, dist = find_closest(atlas, (x, y, z), max_dist=max_dist,
@@ -62,16 +62,16 @@
         else it will not be used. For example, if you are interested in getting
         Brodmann areas with the 'talairach_ba' atlas, you would pass
         must_have=["Brodmann"]
     :param max_dist: max_dist corresponds to the distance that will be
         searched before using "Uncertain."
     :return: the label and the distance from the coord to the label
     """
-    from nichord.peak import read_atlas_peak # import statements here
-                                             # to speed things up
+    from atlasreader.atlasreader import read_atlas_peak # import statements here
+                                                        # to speed things up
     from scipy.spatial import distance
 
     region = read_atlas_peak(atlas, coord, prob_thresh=0.01)
     if isinstance(region, float) and np.isnan(region):
         region = 'uncertain'
 
     bad_keys = ['uncertain', 'Background', 'Cerebral',
```

### Comparing `nichord-0.1.8/nichord/glassbrain.py` & `nichord-0.1.9/nichord/glassbrain.py`

 * *Files identical despite different names*

### Comparing `nichord-0.1.8/nichord/patch_RendererAgg.py` & `nichord-0.1.9/nichord/patch_RendererAgg.py`

 * *Files identical despite different names*

### Comparing `nichord-0.1.8/nichord.egg-info/PKG-INFO` & `nichord-0.1.9/nichord.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: nichord
-Version: 0.1.8
+Version: 0.1.9
 Summary: Creates chord diagrams for connectivity/graph data
 Home-page: https://github.com/paulcbogdan/NiChord
 Author: paulcbogdan
 Author-email: paulcbogdan@gmail.com
 License: MIT
 Keywords: plotting,fmri,plotting,chord
-Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 
 `NiChord` is a Python package for visualizing functional connectivity data. This package was inspired by [NeuroMArVL](https://immersive.erc.monash.edu/neuromarvl/?example=40496078-effa-4ac3-9d3e-cb7f946e7dd1_137.147.133.145), an online visualization tool.
 
 The code can function with any configuration of edges and labels specified by the user.
 
 The glass brain diagrams (left & middle) rely on the plotting tools from [nilearn](https://nilearn.github.io/modules/generated/nilearn.plotting.plot_connectome.html), whereas the chord diagram (right) is made from scratch by drawing shapes in [matplotlib](https://matplotlib.org/). Most of the code, here, is dedicated to the chord diagrams.
 
 This package additionally provides code to help assign labels to nodes based on their anatomical location.
 
 To find out more about the package and see an example, see its [GitHub repo](https://github.com/paulcbogdan/NiChord).
-
```

### Comparing `nichord-0.1.8/setup.py` & `nichord-0.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,21 +15,23 @@
 'To find out more about the package and see an example, see its [GitHub repo](https://github.com/paulcbogdan/NiChord).'
 
 setup(
     name="nichord",
     description="Creates chord diagrams for connectivity/graph data",
     long_description=desc,
     long_description_content_type="text/markdown",
-    version="v0.1.8",
+    version="v0.1.9",
     packages=["nichord"],
     python_requires=">=3.5",
     url="https://github.com/paulcbogdan/NiChord",
     author="paulcbogdan",
     author_email="paulcbogdan@gmail.com",
     install_requires=["nilearn",
+                      "pandas",
                       "matplotlib",
                       "numpy",
                       "scipy",
-                      "pillow"],
+                      "pillow",
+                      "atlasreader"],
     keywords=["plotting", "fmri", "plotting", "chord"],
     license="MIT"
 )
```

