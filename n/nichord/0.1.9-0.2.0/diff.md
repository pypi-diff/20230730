# Comparing `tmp/nichord-0.1.9.tar.gz` & `tmp/nichord-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nichord-0.1.9.tar", last modified: Sun Jul 30 03:02:53 2023, max compression
+gzip compressed data, was "nichord-0.2.0.tar", last modified: Sun Jul 30 18:16:36 2023, max compression
```

## Comparing `nichord-0.1.9.tar` & `nichord-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 03:02:53.714777 nichord-0.1.9/
--rw-rw-rw-   0        0        0     1269 2023-07-30 03:02:53.713777 nichord-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0    10845 2023-07-30 01:34:33.000000 nichord-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 03:02:53.709775 nichord-0.1.9/nichord/
--rw-rw-rw-   0        0        0      756 2022-11-12 03:49:12.000000 nichord-0.1.9/nichord/__init__.py
--rw-rw-rw-   0        0        0    33895 2022-11-13 20:04:28.000000 nichord-0.1.9/nichord/chord.py
--rw-rw-rw-   0        0        0     4893 2022-11-13 19:54:36.000000 nichord-0.1.9/nichord/combine.py
--rw-rw-rw-   0        0        0      482 2022-05-22 13:31:30.000000 nichord-0.1.9/nichord/convert.py
--rw-rw-rw-   0        0        0     5683 2023-07-30 02:58:52.000000 nichord-0.1.9/nichord/coord_labeler.py
--rw-rw-rw-   0        0        0     5731 2022-11-12 03:52:39.000000 nichord-0.1.9/nichord/glassbrain.py
--rw-rw-rw-   0        0        0     2156 2023-07-24 20:52:49.000000 nichord-0.1.9/nichord/patch_RendererAgg.py
-drwxrwxrwx   0        0        0        0 2023-07-30 03:02:53.712777 nichord-0.1.9/nichord.egg-info/
--rw-rw-rw-   0        0        0     1269 2023-07-30 03:02:53.000000 nichord-0.1.9/nichord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-07-30 03:02:53.000000 nichord-0.1.9/nichord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 03:02:53.000000 nichord-0.1.9/nichord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-30 03:02:53.000000 nichord-0.1.9/nichord.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-30 03:02:53.000000 nichord-0.1.9/nichord.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-30 03:02:53.714777 nichord-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1877 2023-07-30 03:02:19.000000 nichord-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 18:16:36.529254 nichord-0.2.0/
+-rw-rw-rw-   0        0        0     1269 2023-07-30 18:16:36.528254 nichord-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9235 2023-07-30 18:11:26.000000 nichord-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 18:16:36.522252 nichord-0.2.0/nichord/
+-rw-rw-rw-   0        0        0      756 2022-11-12 03:49:12.000000 nichord-0.2.0/nichord/__init__.py
+-rw-rw-rw-   0        0        0    34573 2023-07-30 17:47:59.000000 nichord-0.2.0/nichord/chord.py
+-rw-rw-rw-   0        0        0     4893 2022-11-13 19:54:36.000000 nichord-0.2.0/nichord/combine.py
+-rw-rw-rw-   0        0        0      482 2022-05-22 13:31:30.000000 nichord-0.2.0/nichord/convert.py
+-rw-rw-rw-   0        0        0     5683 2023-07-30 02:58:52.000000 nichord-0.2.0/nichord/coord_labeler.py
+-rw-rw-rw-   0        0        0     5731 2022-11-12 03:52:39.000000 nichord-0.2.0/nichord/glassbrain.py
+-rw-rw-rw-   0        0        0     2156 2023-07-24 20:52:49.000000 nichord-0.2.0/nichord/patch_RendererAgg.py
+drwxrwxrwx   0        0        0        0 2023-07-30 18:16:36.527254 nichord-0.2.0/nichord.egg-info/
+-rw-rw-rw-   0        0        0     1269 2023-07-30 18:16:36.000000 nichord-0.2.0/nichord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-07-30 18:16:36.000000 nichord-0.2.0/nichord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 18:16:36.000000 nichord-0.2.0/nichord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-30 18:16:36.000000 nichord-0.2.0/nichord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-30 18:16:36.000000 nichord-0.2.0/nichord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 18:16:36.529254 nichord-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1877 2023-07-30 17:38:21.000000 nichord-0.2.0/setup.py
```

### Comparing `nichord-0.1.9/PKG-INFO` & `nichord-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nichord
-Version: 0.1.9
+Version: 0.2.0
 Summary: Creates chord diagrams for connectivity/graph data
 Home-page: https://github.com/paulcbogdan/NiChord
 Author: paulcbogdan
 Author-email: paulcbogdan@gmail.com
 License: MIT
 Keywords: plotting,fmri,plotting,chord
 Requires-Python: >=3.5
```

### Comparing `nichord-0.1.9/README.md` & `nichord-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,120 +1,109 @@
 # NiChord
 
 `NiChord` is a Python package for visualizing functional connectivity data. 
 This package was inspired by [NeuroMArVL](https://immersive.erc.monash.edu/neuromarvl/?example=40496078-effa-4ac3-9d3e-cb7f946e7dd1_137.147.133.145),
-an online visualization tool. With just a few lines of Python code, `NiChord`
- can create figures like these:
-  
- <p align="center">
-  <img src="example\ex_1_and_2.png" />
-</p>
-
-The code can function with any configuration of edges and labels specified by
-the user. 
+an online visualization tool. Although the code was designed for neuroscience
+research, it can be used with any configuration of edge and label data.
 
-The glass brain diagrams (left & middle) rely on the plotting tools from 
-[nilearn](https://nilearn.github.io/modules/generated/nilearn.plotting.plot_connectome.html), 
-whereas the chord diagram (right) is made from scratch by drawing shapes in 
-[matplotlib](https://matplotlib.org/). Most of the code, here, is dedicated to 
-the chord diagrams. 
-  
- This package additionally provides code to help assign labels to nodes based
- on their anatomical location. 
+<p align="center">
+  <img src="example\outside_chord_example.png"  width="600" />
+</p>
 
 ## Installation
 `NiChord` (requires Python 3.5+) can be installed via pip:
 
 ```
 $ pip install nichord
 ```
 
-## Usage example
+## Examples
 
-The examples above were constructed by saving separate images for the chord and
-glass brain diagrams and then combining the images.
+Here, we cover the code provided in `example.example.py`. 
 
 ### Input variables
 Edges are specified as a list of tuples, (i, j), where i and j are indices
-representing the two nodes making up the edge.
+representing the two nodes making up the edge. For this example, the list 
+represents seven edges among eight nodes.
 
 ```Python
 edges = [(0, 1), (0, 2), (1, 5), (3, 5), (4, 6), (2, 7), (6, 7)]
 ```
 
 Each node index should also correspond to a coordinate in MNI space:
 ```Python
 coords = [[-24, -99, -12], [51, -3, -15], [-15, -70, 30], [21, 39, 39],
           [21, -66, 48], [54, 33, 12], [-33, 3, 3], [57, -45, 12]]
 ```
 
 These coordinates can be used to construct a dictionary, mapping each node index
-to a network label (by default, network labels are based on the 
-[Yeo et al. (2011) atlas](https://journals.physiology.org/doi/full/10.1152/jn.00338.2011)):
+to a network label. This package provides functions to help assign labels to 
+nodes given their anatomical location. By default, network labels are based on the 
+[Yeo et al. (2011) atlas](https://journals.physiology.org/doi/full/10.1152/jn.00338.2011):
 
 ```Python
 from nichord.coord_labeler import get_idx_to_label
 idx_to_label = get_idx_to_label(coords, atlas='yeo')
 ```
 
-Or a dictionary can be defined manually:
+`idx_to_label` can alternatively be defined manually:
 
 ```Python
 idx_to_label = {0: 'Visual', 1: 'DMN', 2: 'Visual', 3: 'DMN', 
                 4: 'DAN', 5: 'FPCN', 6: 'VAN', 7: 'VAN'}
 ```
 
-Each edge may be associated with a weight. Weights are defined as a list of 
-length equal to the number of edges (if `edge_weights = None`, then grey edges are.
-plotted).
+You may assign each edge a weight. Weights are defined as a list of 
+length equal to the number of edges (e.g., 8 weights for this example). 
+If `edge_weights = None`, then grey edges are plotted, unless an aggregation
+feature is used (see `plot_count=True` below).
 
 ```Python
 edge_weights = [-0.3, -0.5, 0.7, 0.5, -0.2, 0.3, 0.8]
 ```
 
 ### Plotting
 
-These variables and a filepath can then be 
-passed to create the chord diagram:
+These variables and an optional filepath can then be passed to create a chord diagram:
 
 ```Python
 from nichord.chord import plot_chord
 
-fp_chord = 'ex0_good.png' # if None, chord diagram can be opened in a matplotlib
-                          # window with matplotlib.pyplot.show()
-plot_chord(idx_to_label, edges, edge_weights=edge_weights, 
-    fp_chord=fp_chord,
-    linewidths=15, alphas = 0.9, do_ROI_circles=True, 
-    do_ROI_circles_specific=True, ROI_circle_radius=0.02)
+# If the filepath is left None, the chord diagram can be opened in a matplotlib with plt.show()
+fp_chord = 'ex0_chord.png'
+plot_chord(idx_to_label, edges, edge_weights=edge_weights, fp_chord=fp_chord, 
+           linewidths=15, alphas=0.9, do_ROI_circles=True, label_fontsize=70, 
+           # July 2023 update allows changing label fontsize
+           do_ROI_circles_specific=True, ROI_circle_radius=0.02)
+
 ```
 
 <p align="center">
   <img src="example\chord\ex0_chord.png" width="600" />
   <br>
   If no filepath is passed, the diagram will be opened in a matplotlib window.
 </p>
 
 
-Plotting the glass brain involves the same variables (note that the colors of 
-the glass brain nodes should correspond to the same colors as the chord network 
-labels)
+Plotting the glass brain involves the same variables. Note that the colors of 
+the glass brain nodes correspond to the network colors in the chord diagram.
 
 ```Python
 from nichord.glassbrain import plot_glassbrain
 
 fp_glass = 'ex0_glassbrain.png'
 plot_glassbrain(idx_to_label, edges, edge_weights, fp_glass,
                 coords, linewidths=15, node_size=17)
 ```
 
 <p align="center">
   <img src="example\glass\ex0_glass.png" />
 </p>
 
-Finally, to combine the figures above:
+You can combine the figures above into a single figure.
 
 ```Python
 from nichord.combine import combine_imgs
 
 fp_combined = 'ex0_combined.png'
 combine_imgs(fp_glass, fp_chord, fp_combined)
 ```
@@ -143,18 +132,17 @@
 fn = 'ex1.png'
 plot_and_combine(dir_out, fn, idx_to_label, edges,
                  edge_weights=edge_weights, coords=power_coords,
                  network_order=network_order, network_colors=network_colors,
                  )
 ```
 
-You can pass `plot_and_combine` some `chord_kwargs=` or `glass_kwargs=` to 
-adjust the appearance of the chord diagram or glass brain, like above. These two
-examples here do this and also show new features added in November 2022. The
-one below shows how you can add a title and give the chord diagram a black 
+To `plot_and_combine`, you can pass `chord_kwargs` and/or `glass_kwargs` to 
+adjust the appearance of the chord diagram or glass brain, like above. The
+example below also shows how you can add a title and give the chord diagram a black 
 background:
 
 ```Python
 dir_out = 'example'
 fn = r'ex1_black_BG.png'
 chord_kwargs = {'black_BG': True}
 plot_and_combine(dir_out, fn, idx_to_label, edges,
@@ -162,15 +150,15 @@
                  network_order=network_order, network_colors=network_colors,
                  chord_kwargs=chord_kwargs, title='Example 1b (black)')
 ```
 <p align="center">
   <img src="example\ex1_black_BG.png" />
 </p>
 
-Here is another example. This one shows how setting linewidth = 0 causes no 
+Here is another example. This one shows how setting `linewidth = 0` causes no 
 lines to be plotted on the glass brain. This may be useful in combination
 with setting a node sizes as a list, which casues nodes on the glassbrain to be
 plotted in sizes specified. 
 
 ```Python
 fn = r'ex1_count.png'
 chord_kwargs = {'plot_count': True}
@@ -185,16 +173,19 @@
 ```
 
 <p align="center">
   <img src="example\ex1_count.png" />
 </p>
 
 
-Final example, which shows other features (you can plot little circles on the
-chord diagrams where the arcs start): 
+This example shows other features. With `do_ROI_cicles=True`, you can plot 
+little circles on the chord diagrams where the arcs start with.
+With `only1glass=True`, you can the sagittal glass brain only. These arguments
+are not specific to `plot_and_combine`. They can also be passed to 
+`plot_chord` and `plot_glassbrain`, respectively.
 
 ```Python
 fn = r'ex2.png'
 edges = [(32, 12), (32, 48), (33, 48), (101, 105), (105, 219), (201, 33),
          (32, 105)]
 edge_weights = [-0.3, -0.5, 0.7, 0.5, -0.2, 0.3, 0.8]
 
@@ -222,48 +213,29 @@
 ```Python
 from nichord.convert import convert_matrix
 
 matrix = [[0, 0.5, 0.2], [0.5, 0, -0.2], [0.2, -0.2, 0]]
 edges, edge_weights = convert_matrix(matrix)
 ```
 
-### Note
+
+## Note
 There is seemingly a bug in matplotlib.backend_agg.RenderAgg, which makes 
 rotated text not look ideal when plotting character by character, as is being
 done here. I submitted a [bug report](https://github.com/matplotlib/matplotlib/issues/23021)
 to matplotlib, along with a potential
 solution. It has not been accepted yet, so for now I am "monkey patching" the
 malfunctioning code in `nichord.patch_RenderAgg.py`. The patch is automatically 
-applied when calling `chord.plot_chord_diagram(...)` unless 
-`do_monkeypatch=False`. 
-
-## Update (November 10, 2022)
-Additions:
-* added `combine.plot_and_combine` to do `plot_chord`, `plot_glassbrain`, and `combine_image` with a single function. See new examples above
-* updated to allow titles for `combine_image` (new `title=` argument; `''` by default)
-* updated to allow `black_BG` for `plot_chord` (new `black_BG=` argument; `false` by default, which causes a white BG). See the example below. Note: `black_BG=true` with the new `'turbo'` default looks much better for extremely dense chord diagrams (1000+ edges)
-
-<p align="center">
-  <img src="example\ex1_chord_black_BG.png"  width="600" />
-</p>
-
-<p align="center">
-  <img src="example\outside_chord_example.png"  width="600" />
-</p>
-
-* updated to allow `plot_chord` to average all edges between a pair of networks (new `plot_count=` argument; default is `false`). Helpful when there are a lot of edges otherwise. See the example below, which is a `plot_count=True` version of the chord diagram immediately above. For `plot_count=True`, the arc color is the average of all edge weights for edges between a pair of networks. Arc thickness corresponds to the number of edges between the pair of networks
-
-<p align="center">
-  <img src="example\outside_chord_example_count.png"  width="600" />
-</p>
+applied when calling `chord.plot_chord_diagram(...)` with the default argument 
+`do_monkeypatch=True`. 
 
-Changed:
-* Default plotting colormap from matplotlib's `'Spectral_r'` to its `'turbo'`. The middle end is much more visible now and the colors overall pop more
-* `plot_chord `to now plots the arcs in order of the absolute value of edge_weights or for plot_count in order of the count (thicker edges are now on top)
-* The hinting for `plot_glassbrain` to specify that node_size can be a list or ndarray. Passing a list or ndarray of length = #nodes or #nonzero_nodes will cause the nodes to be plotted the different sizes specified
+The glass brain diagrams rely on the plotting tools from 
+[`nilearn`](https://nilearn.github.io/modules/generated/nilearn.plotting.plot_connectome.html), 
+whereas the chord diagrams is made from scratch by drawing shapes in 
+[`matplotlib`](https://matplotlib.org/).
 
 ## Authors
 `NiChord` was created by Paul C. Bogdan with help from [Jonathan
  Shobrook](https://github.com/shobrook) as part of our research in the 
  [Dolcos Lab](https://dolcoslab.beckman.illinois.edu/) at the Beckman Institute
  for Advanced Science and Technology and the University of Illinois at 
  Urbana-Champaign.
```

### Comparing `nichord-0.1.9/nichord/__init__.py` & `nichord-0.2.0/nichord/__init__.py`

 * *Files identical despite different names*

### Comparing `nichord-0.1.9/nichord/chord.py` & `nichord-0.2.0/nichord/chord.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,15 @@
                coords: Union[list, np.ndarray] = None,
                arc_setting: bool = True,
                cbar: Union[None, plt.colorbar] = None,
                do_ROI_circles: bool = False,
                do_ROI_circles_specific: bool = True,
                ROI_circle_radius: float = 0.005,
                black_BG: bool = False,
+               label_fontsize: int = 60,
                do_monkeypatch: bool = True,
                vmin: Union[None, int, float] = None,
                vmax: Union[None, int, float] = None,
                plot_count: bool = False,
                plot_abs_sum: bool = False,
                norm_thickness: bool = False,
                dpi: int = 400) -> None:
@@ -132,15 +133,16 @@
     if coords is None:
         coords = np.random.random(size=(len(idx_to_label), 3))
 
     plt.figure(figsize=(15, 15))
     radius = 0.6
     network_low_high, network_counts, network_centers, network_starts_ends = \
         plot_rim_and_labels(idx_to_label, network_order, network_colors, radius,
-                            black_BG=black_BG, do_monkeypatch=do_monkeypatch)
+                            black_BG=black_BG, label_fontsize=label_fontsize,
+                            do_monkeypatch=do_monkeypatch)
 
 
     vmin, vmax = plot_arcs(edges, idx_to_label, network_low_high, network_counts,
                            edge_weights, network_centers, network_starts_ends,
                            radius, cmap, coords, linewidths=linewidths,
                            seven_point_arc=arc_setting, colors=colors,
                            alphas=alphas, vmin=vmin, vmax=vmax,
@@ -176,16 +178,17 @@
     if fp_chord is not None:
         plt.savefig(fp_chord, dpi=dpi)
         plt.clf()
 
 
 def plot_rim_and_labels(idx_to_label: dict, network_order: list,
                         network_colors: dict, radius: Union[float, int],
-                        rim_border: Union[float, int]=1.0,
-                        black_BG: bool=False,
+                        rim_border: Union[float, int] = 1.0,
+                        black_BG: bool = False,
+                        label_fontsize: int = 60,
                         do_monkeypatch: bool = True) -> Tuple[dict, dict,
                                                               dict, dict]:
     """
     Plots the chord diagram rims and labels. Each rim is plotted separately
 
     :param idx_to_label: dict mapping each ROI index to its chord label
     :param network_order: list specifying the order of the labels (rims)
@@ -215,14 +218,15 @@
         degree_st = circle_consumed / num_ROIs * 360
         degree_end = (circle_consumed + cnt) / num_ROIs * 360
         plot_rim(degree_st, degree_end, rim_border=rim_border, radius=radius,
                  color=network_colors[network])
         plot_rim_label(degree_st, degree_end, network, rim_border=rim_border,
                        radius=radius,
                        color=network_colors[network],
+                       label_fontsize=label_fontsize,
                        do_monkeypatch=do_monkeypatch)
         network_low_high[network] = (
             degree_st + rim_border, degree_end - rim_border)
         network_center[network] = (circle_consumed + cnt * 0.5) / num_ROIs * 360
         network_starts_ends[network] = (degree_st, degree_end)
         circle_consumed += cnt
     if black_BG:
@@ -267,23 +271,31 @@
         char1_transparent = plt.text(0, 0, char1, rotation=0,
                                      rotation_mode='anchor', ha='center',
                                      alpha=0, **font_kwargs)
         bb1 = char1_transparent.get_window_extent(renderer=r).transformed(
             ax.transData.inverted())
 
         width = bb0.width / 2 + bb1.width / 2
+        width *= 1.1
         boost = 1
         if 'fontname' in font_kwargs and \
                 font_kwargs['fontname'].lower() == 'monospace':
-            if char1 in ['D',
-                         'P']:  # given the shapes of these letters, they look
-                                # a bit better when pushed to be closer
-                boost -= .4     # to the previous/following letter in the text.
-            if char0 in ['A']:
+            # Given the shapes of some letters, they look a bit better when
+            # pushed to be closer to the previous/following letter in the text.
+            if char1 in ['D', 'P', 'C']:
                 boost -= .4
+            elif char0 in ['A']:
+                boost -= .8
+            elif char1 in ['A']:
+                boost += .4
+            # Somebody who understands kerning please help me.
+            # I've invested substantial effort into trying to get this right,
+            # and this is the best that I've got. It works fine for the Yeo
+            # atlas labels and for a few other label sets I tested, but
+            # there could be label sets out there where it doesn't look good.
 
         char_deg += width / arc_len * (degree_end - degree_st) + boost
         if char_deg > degree_end - degree_st - rim_border * 2:
             text = text[:len(char_degs) - 1] + '.'
             break
         char_degs.append(char_deg)
 
@@ -305,49 +317,50 @@
     return char_degs, text
 
 
 def plot_rim_label(degree_st: Union[float, int], degree_end: Union[float, int],
                    text: str,
                    rim_border: Union[float, int] = 1, radius: float = 0.55,
                    color: Union[str, tuple] = 'black',
-                   fontsize: Union[float, int] = 40,
+                   label_fontsize: Union[float, int] = 60,
                    do_monkeypatch: bool = True):
     """
     Adds the label for its corresponding rim.
 
     :param degree_st: Starting degree of the rim (whitespace included)
     :param degree_end: Ending degree of the rim (whitespace included)
     :param text: The string written around the rim
     :param rim_border: Float specifying the degrees/2 between each rim
                        (i.e., the amount of white spacing between rims)
     :param radius: radius of the chord diagram
     :param color: label color
-    :param fontsize: label fontsize
+    :param label_fontsize: label fontsize
     :param do_monkeypatch: I think there is a bug in matplotlib, which prevents
         characters from being rotated properly. patch_RendererAgg.py contains
         code that attempts to fix this. Setting do_monkeypatch == True applies
         this fix, while this script is running (to be clear, running this
         code will not permanently change your matplotlib files)
     """
     if do_monkeypatch:
         from nichord import patch_RendererAgg
         patch_RendererAgg.do_monkey_patch()
+
     # monospace is the easiest font to work with
     # although future work can try playing around with
     # the code to get non-monospace fonts working
     # (non-monospace is difficult to position).
-    font_kwargs = {'fontname': 'monospace', 'fontsize': fontsize}
+    font_kwargs = {'fontname': 'monospace', 'fontsize': label_fontsize}
     char_degrees, text = get_character_degree_locations(text, degree_st,
                                                         degree_end, rim_border,
                                                         font_kwargs)
 
     text = text[::-1]  # The text must be flipped so that the text reads
                  # left-to-right (note that the last character must have
                  # the lowest degree angle.
-
+    # spacing_incrament
     for deg, char in zip(char_degrees, text):
         trans_deg = deg
         trans_deg270 = deg + 270
         x = np.cos(trans_deg / 360 * 2 * np.pi) * (radius)
         y = np.sin(trans_deg / 360 * 2 * np.pi) * (radius)
         plt.text(x, y, char, rotation=trans_deg270, rotation_mode='anchor',
                  va='bottom',
```

### Comparing `nichord-0.1.9/nichord/combine.py` & `nichord-0.2.0/nichord/combine.py`

 * *Files identical despite different names*

### Comparing `nichord-0.1.9/nichord/coord_labeler.py` & `nichord-0.2.0/nichord/coord_labeler.py`

 * *Files identical despite different names*

### Comparing `nichord-0.1.9/nichord/glassbrain.py` & `nichord-0.2.0/nichord/glassbrain.py`

 * *Files identical despite different names*

### Comparing `nichord-0.1.9/nichord/patch_RendererAgg.py` & `nichord-0.2.0/nichord/patch_RendererAgg.py`

 * *Files identical despite different names*

### Comparing `nichord-0.1.9/nichord.egg-info/PKG-INFO` & `nichord-0.2.0/nichord.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nichord
-Version: 0.1.9
+Version: 0.2.0
 Summary: Creates chord diagrams for connectivity/graph data
 Home-page: https://github.com/paulcbogdan/NiChord
 Author: paulcbogdan
 Author-email: paulcbogdan@gmail.com
 License: MIT
 Keywords: plotting,fmri,plotting,chord
 Requires-Python: >=3.5
```

### Comparing `nichord-0.1.9/setup.py` & `nichord-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 'To find out more about the package and see an example, see its [GitHub repo](https://github.com/paulcbogdan/NiChord).'
 
 setup(
     name="nichord",
     description="Creates chord diagrams for connectivity/graph data",
     long_description=desc,
     long_description_content_type="text/markdown",
-    version="v0.1.9",
+    version="v0.2.0",
     packages=["nichord"],
     python_requires=">=3.5",
     url="https://github.com/paulcbogdan/NiChord",
     author="paulcbogdan",
     author_email="paulcbogdan@gmail.com",
     install_requires=["nilearn",
                       "pandas",
```

