# Comparing `tmp/jaal-0.1.3.tar.gz` & `tmp/jaal-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaal-0.1.3.tar", last modified: Sat Sep  3 11:10:40 2022, max compression
+gzip compressed data, was "jaal-0.1.4.tar", last modified: Sun Jul 30 06:08:14 2023, max compression
```

## Comparing `jaal-0.1.3.tar` & `jaal-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 11:10:40.932567 jaal-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-09-03 11:10:33.000000 jaal-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     8122 2022-09-03 11:10:40.932567 jaal-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6272 2022-09-03 11:10:33.000000 jaal-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 11:10:40.932567 jaal-0.1.3/jaal/
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-09-03 11:10:33.000000 jaal-0.1.3/jaal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 11:10:40.932567 jaal-0.1.3/jaal/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-09-03 11:10:33.000000 jaal-0.1.3/jaal/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      710 2022-09-03 11:10:33.000000 jaal-0.1.3/jaal/datasets/load_got.py
--rw-r--r--   0 runner    (1001) docker     (121)     3143 2022-09-03 11:10:33.000000 jaal-0.1.3/jaal/datasets/parse_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (121)    14648 2022-09-03 11:10:33.000000 jaal-0.1.3/jaal/jaal.py
--rw-r--r--   0 runner    (1001) docker     (121)    12198 2022-09-03 11:10:33.000000 jaal-0.1.3/jaal/layout.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 11:10:40.932567 jaal-0.1.3/jaal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8122 2022-09-03 11:10:40.000000 jaal-0.1.3/jaal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-09-03 11:10:40.000000 jaal-0.1.3/jaal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-03 11:10:40.000000 jaal-0.1.3/jaal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-09-03 11:10:40.000000 jaal-0.1.3/jaal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-03 11:10:40.000000 jaal-0.1.3/jaal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-03 11:10:40.932567 jaal-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1735 2022-09-03 11:10:33.000000 jaal-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:08:14.322129 jaal-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-30 06:07:56.000000 jaal-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-07-30 06:08:14.322129 jaal-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-07-30 06:07:56.000000 jaal-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:08:14.318129 jaal-0.1.4/jaal/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-30 06:07:56.000000 jaal-0.1.4/jaal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:08:14.322129 jaal-0.1.4/jaal/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-30 06:07:56.000000 jaal-0.1.4/jaal/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-30 06:07:56.000000 jaal-0.1.4/jaal/datasets/load_got.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-07-30 06:07:56.000000 jaal-0.1.4/jaal/datasets/parse_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14666 2023-07-30 06:07:56.000000 jaal-0.1.4/jaal/jaal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-07-30 06:07:56.000000 jaal-0.1.4/jaal/layout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 06:08:14.322129 jaal-0.1.4/jaal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-07-30 06:08:14.000000 jaal-0.1.4/jaal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-30 06:08:14.000000 jaal-0.1.4/jaal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 06:08:14.000000 jaal-0.1.4/jaal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-30 06:08:14.000000 jaal-0.1.4/jaal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-30 06:08:14.000000 jaal-0.1.4/jaal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 06:08:14.322129 jaal-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-30 06:07:56.000000 jaal-0.1.4/setup.py
```

### Comparing `jaal-0.1.3/LICENSE` & `jaal-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jaal-0.1.3/PKG-INFO` & `jaal-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: jaal
-Version: 0.1.3
+Version: 0.1.4
 Summary: jaal - your interactive network visualizer dashboard
 Home-page: https://github.com/imohitmayank/jaal
 Author: Mohit Mayank
 Author-email: mohitmayank1@gmail.com
 License: UNKNOWN
-Description: <img src="jaal/assest/logo.png" alt="jaal logo"/>
+Description: <img src="jaal/assets/logo.png" alt="jaal logo"/>
         
         ![PyPI](https://img.shields.io/pypi/v/jaal) [![PyPI dm](https://img.shields.io/pypi/dm/jaal.svg)](https://img.shields.io/pypi/jaal) [![Join the chat at https://gitter.im/imm-jaal/community](https://badges.gitter.im/imm-jaal/community.svg)](https://gitter.im/imm-jaal/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) ![GitHub](https://img.shields.io/github/license/imohitmayank/jaal) ![GitHub Repo stars](https://img.shields.io/github/stars/imohitmayank/jaal?style=social)
         
         *Your interactive network visualizing dashboard*
         
         Documentation: [Here](http://mohitmayank.com/jaal/)
         
@@ -60,60 +60,69 @@
         1. **edge_df:** its a pandas dataframe with atleast `from` and `to` column, which represents the edge relationship between the entities
         2. **node_df:** its an optional parameter, but should contains a `id` column with unique node names. 
         
         Note, edge_df is mandatory and node_df is optional. Also we can include additional columns in these files which are automatically considered as edge or node features respectively.
         
         After running the plot, the console will prompt the default localhost address (`127.0.0.1:8050`) where Jaal is running. Access it to see the following dashboard,
         
-        <img src="jaal/assest/dashboard.png" alt="dashboard"/>
+        <img src="jaal/assets/dashboard.png" alt="dashboard"/>
         
         ## 👉 Features
         
         At present, the dashboard consist of following sections,
         1. **Setting panel:** here we can play with the graph data, it further contain following sections:
             - **Search:** can be used to find a node in graph
             - **Filter:** supports pandas query language and can be used to filter the graph data based on nodes or edge features.
             - **Color:** can be used to color nodes or edges based on their categorical features. Note, currently only features with at max 20 cardinality are supported. 
             - **Size:** can be used to size nodes or edges based on their numerical features.
         2. **Graph:** the network graph in all its glory :)
         
         ## 👉 Examples
         
         ### 1. Searching
-        <img src="jaal/assest/jaal_search.gif" alt="dashboard"/>
+        <img src="jaal/assets/jaal_search.gif" alt="dashboard"/>
         
         ### 2. Filtering
-        <img src="jaal/assest/jaal_filter.gif" alt="dashboard"/>
+        <img src="jaal/assets/jaal_filter.gif" alt="dashboard"/>
         
         ### 3. Coloring
-        <img src="jaal/assest/jaal_color.gif" alt="dashboard"/>
+        <img src="jaal/assets/jaal_color.gif" alt="dashboard"/>
         
         ### 4. Size
-        <img src="jaal/assest/jaal_size.gif" alt="dashboard"/>
+        <img src="jaal/assets/jaal_size.gif" alt="dashboard"/>
         
         ## 👉 Extra settings
         
         ### Display edge label
         
         To display labels over edges, we need to add a `label` attribute (column) in the `edge_df`. Also, it has to be in `string` format. 
         For example, using the GoT dataset, by adding the following line before the `Jaal` call, we can display the edge labels.
         
         ```python
         # add edge labels
         edge_df.loc[:, 'label'] = edge_df.loc[:, 'weight'].astype(str)
         ```
+        ### Display image in node
+        
+        Currently it is possible to show image within node (with circular shape). For this, we need to put `node_image_url` column in the `node_df` with URLs for each node.
+        
+        <img src="jaal/assets/jaal_node_image.png" width="300" height="200" alt="dashboard"/>
         
         ### Directed edges
         
         By default, `Jaal` plot undirected edges. This setting can be changed by,
         
         ```python
         Jaal(edge_df, node_df).plot(directed=True)
         ```
         
+        ### Showing Tooltip
+        
+        By default, `nodeid` is shown as tooltip. To overwrite this, include a `title` column with the respective data.
+        
         ### Using vis.js settings
         
         We can tweak any of the `vis.js` related network visualization settings. An example is,
         
         ```python
         # init Jaal and run server
         Jaal(edge_df, node_df).plot(vis_opts={'height': '600px', # change height
```

### Comparing `jaal-0.1.3/README.md` & `jaal-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<img src="jaal/assest/logo.png" alt="jaal logo"/>
+<img src="jaal/assets/logo.png" alt="jaal logo"/>
 
 ![PyPI](https://img.shields.io/pypi/v/jaal) [![PyPI dm](https://img.shields.io/pypi/dm/jaal.svg)](https://img.shields.io/pypi/jaal) [![Join the chat at https://gitter.im/imm-jaal/community](https://badges.gitter.im/imm-jaal/community.svg)](https://gitter.im/imm-jaal/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) ![GitHub](https://img.shields.io/github/license/imohitmayank/jaal) ![GitHub Repo stars](https://img.shields.io/github/stars/imohitmayank/jaal?style=social)
 
 *Your interactive network visualizing dashboard*
 
 Documentation: [Here](http://mohitmayank.com/jaal/)
 
@@ -52,60 +52,69 @@
 1. **edge_df:** its a pandas dataframe with atleast `from` and `to` column, which represents the edge relationship between the entities
 2. **node_df:** its an optional parameter, but should contains a `id` column with unique node names. 
 
 Note, edge_df is mandatory and node_df is optional. Also we can include additional columns in these files which are automatically considered as edge or node features respectively.
 
 After running the plot, the console will prompt the default localhost address (`127.0.0.1:8050`) where Jaal is running. Access it to see the following dashboard,
 
-<img src="jaal/assest/dashboard.png" alt="dashboard"/>
+<img src="jaal/assets/dashboard.png" alt="dashboard"/>
 
 ## 👉 Features
 
 At present, the dashboard consist of following sections,
 1. **Setting panel:** here we can play with the graph data, it further contain following sections:
     - **Search:** can be used to find a node in graph
     - **Filter:** supports pandas query language and can be used to filter the graph data based on nodes or edge features.
     - **Color:** can be used to color nodes or edges based on their categorical features. Note, currently only features with at max 20 cardinality are supported. 
     - **Size:** can be used to size nodes or edges based on their numerical features.
 2. **Graph:** the network graph in all its glory :)
 
 ## 👉 Examples
 
 ### 1. Searching
-<img src="jaal/assest/jaal_search.gif" alt="dashboard"/>
+<img src="jaal/assets/jaal_search.gif" alt="dashboard"/>
 
 ### 2. Filtering
-<img src="jaal/assest/jaal_filter.gif" alt="dashboard"/>
+<img src="jaal/assets/jaal_filter.gif" alt="dashboard"/>
 
 ### 3. Coloring
-<img src="jaal/assest/jaal_color.gif" alt="dashboard"/>
+<img src="jaal/assets/jaal_color.gif" alt="dashboard"/>
 
 ### 4. Size
-<img src="jaal/assest/jaal_size.gif" alt="dashboard"/>
+<img src="jaal/assets/jaal_size.gif" alt="dashboard"/>
 
 ## 👉 Extra settings
 
 ### Display edge label
 
 To display labels over edges, we need to add a `label` attribute (column) in the `edge_df`. Also, it has to be in `string` format. 
 For example, using the GoT dataset, by adding the following line before the `Jaal` call, we can display the edge labels.
 
 ```python
 # add edge labels
 edge_df.loc[:, 'label'] = edge_df.loc[:, 'weight'].astype(str)
 ```
+### Display image in node
+
+Currently it is possible to show image within node (with circular shape). For this, we need to put `node_image_url` column in the `node_df` with URLs for each node.
+
+<img src="jaal/assets/jaal_node_image.png" width="300" height="200" alt="dashboard"/>
 
 ### Directed edges
 
 By default, `Jaal` plot undirected edges. This setting can be changed by,
 
 ```python
 Jaal(edge_df, node_df).plot(directed=True)
 ```
 
+### Showing Tooltip
+
+By default, `nodeid` is shown as tooltip. To overwrite this, include a `title` column with the respective data.
+
 ### Using vis.js settings
 
 We can tweak any of the `vis.js` related network visualization settings. An example is,
 
 ```python
 # init Jaal and run server
 Jaal(edge_df, node_df).plot(vis_opts={'height': '600px', # change height
```

### Comparing `jaal-0.1.3/jaal/datasets/load_got.py` & `jaal-0.1.4/jaal/datasets/load_got.py`

 * *Files identical despite different names*

### Comparing `jaal-0.1.3/jaal/datasets/parse_dataframe.py` & `jaal-0.1.4/jaal/datasets/parse_dataframe.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,18 +47,23 @@
         scaling_vars['node'] = compute_scaling_vars_for_numerical_cols(node_df)
     scaling_vars['edge'] = compute_scaling_vars_for_numerical_cols(edge_df)
     
     # create node list w.r.t. the presence of absence of node_df
     nodes = []
     if node_df is None:
         node_list = list(set(edge_df['from'].unique().tolist() + edge_df['to'].unique().tolist()))
-        nodes = [{'id': node_name, 'label': node_name, 'shape': 'dot', 'size': 7} for node_name in node_list]
+        nodes = [{'id': node_name, 'label': node_name, 'title': node_name, 'shape': 'dot', 'size': 7} for node_name in node_list]
     else:
         # convert the node id column to string
         node_df.loc[:, 'id'] = node_df.loc[:, 'id'].astype(str)
+        # remove blanks cols
+        node_df = node_df.dropna(axis=1)
+        # if title is not present, make it same as label
+        if 'title' not in node_df.columns:
+            node_df['title'] = node_df['id']
         # see if node imge url is present or not
         node_image_url_flag = 'node_image_url' in node_df.columns
         # create the node data
         for node in node_df.to_dict(orient='records'):
             if not node_image_url_flag:
                 nodes.append({**node, **{'label': node['id'], 'shape': 'dot', 'size': 7}})
             else:
```

### Comparing `jaal-0.1.3/jaal/jaal.py` & `jaal-0.1.4/jaal/jaal.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         print("Done")
 
     def _callback_search_graph(self, graph_data, search_text):
         """Only show the nodes which match the search text
         """
         nodes = graph_data['nodes']
         for node in nodes:
-            if search_text not in node['label'].lower():
+            if search_text.lower() not in node['label'].lower():
                 node['hidden'] = True
             else:
                 node['hidden'] = False
         graph_data['nodes'] = nodes
         return graph_data
 
     def _callback_filter_nodes(self, graph_data, filter_nodes_text):
@@ -212,15 +212,15 @@
 
         Returns
         -------
             app: dash.Dash
                 the Jaal app
         """
         # create the app
-        app = dash.Dash(external_stylesheets=[dbc.themes.BOOTSTRAP])
+        app = dash.Dash(__name__, external_stylesheets=[dbc.themes.BOOTSTRAP])
 
         # define layout
         app.layout = get_app_layout(self.data, color_legends=self.get_color_popover_legend_children(), directed=directed, vis_opts=vis_opts)
 
         # create callbacks to toggle legend popover
         @app.callback(
             Output("color-legend-popup", "is_open"),
```

### Comparing `jaal-0.1.3/jaal/layout.py` & `jaal-0.1.4/jaal/layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,15 +209,15 @@
     cat_edge_features = get_categorical_features(pd.DataFrame(graph_data['edges']).drop(columns=['color']), 20, ['color', 'from', 'to', 'id'])
     # Step 3-4: Get numerical features of nodes and edges
     num_node_features = get_numerical_features(pd.DataFrame(graph_data['nodes']))
     num_edge_features = get_numerical_features(pd.DataFrame(graph_data['edges']))
     # Step 5: create and return the layout
     # resolve path
     this_dir, _ = os.path.split(__file__)
-    image_filename = os.path.join(this_dir, "assest", "logo.png")
+    image_filename = os.path.join(this_dir, "assets", "logo.png")
     encoded_image = base64.b64encode(open(image_filename, 'rb').read())
     return html.Div([
             # create_row(html.H2(children="Jaal")), # Title
             create_row(html.Img(src='data:image/png;base64,{}'.format(encoded_image.decode()), width="80px")),
             create_row([
                 dbc.Col([
                     # setting panel
```

### Comparing `jaal-0.1.3/jaal.egg-info/PKG-INFO` & `jaal-0.1.4/jaal.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: jaal
-Version: 0.1.3
+Version: 0.1.4
 Summary: jaal - your interactive network visualizer dashboard
 Home-page: https://github.com/imohitmayank/jaal
 Author: Mohit Mayank
 Author-email: mohitmayank1@gmail.com
 License: UNKNOWN
-Description: <img src="jaal/assest/logo.png" alt="jaal logo"/>
+Description: <img src="jaal/assets/logo.png" alt="jaal logo"/>
         
         ![PyPI](https://img.shields.io/pypi/v/jaal) [![PyPI dm](https://img.shields.io/pypi/dm/jaal.svg)](https://img.shields.io/pypi/jaal) [![Join the chat at https://gitter.im/imm-jaal/community](https://badges.gitter.im/imm-jaal/community.svg)](https://gitter.im/imm-jaal/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) ![GitHub](https://img.shields.io/github/license/imohitmayank/jaal) ![GitHub Repo stars](https://img.shields.io/github/stars/imohitmayank/jaal?style=social)
         
         *Your interactive network visualizing dashboard*
         
         Documentation: [Here](http://mohitmayank.com/jaal/)
         
@@ -60,60 +60,69 @@
         1. **edge_df:** its a pandas dataframe with atleast `from` and `to` column, which represents the edge relationship between the entities
         2. **node_df:** its an optional parameter, but should contains a `id` column with unique node names. 
         
         Note, edge_df is mandatory and node_df is optional. Also we can include additional columns in these files which are automatically considered as edge or node features respectively.
         
         After running the plot, the console will prompt the default localhost address (`127.0.0.1:8050`) where Jaal is running. Access it to see the following dashboard,
         
-        <img src="jaal/assest/dashboard.png" alt="dashboard"/>
+        <img src="jaal/assets/dashboard.png" alt="dashboard"/>
         
         ## 👉 Features
         
         At present, the dashboard consist of following sections,
         1. **Setting panel:** here we can play with the graph data, it further contain following sections:
             - **Search:** can be used to find a node in graph
             - **Filter:** supports pandas query language and can be used to filter the graph data based on nodes or edge features.
             - **Color:** can be used to color nodes or edges based on their categorical features. Note, currently only features with at max 20 cardinality are supported. 
             - **Size:** can be used to size nodes or edges based on their numerical features.
         2. **Graph:** the network graph in all its glory :)
         
         ## 👉 Examples
         
         ### 1. Searching
-        <img src="jaal/assest/jaal_search.gif" alt="dashboard"/>
+        <img src="jaal/assets/jaal_search.gif" alt="dashboard"/>
         
         ### 2. Filtering
-        <img src="jaal/assest/jaal_filter.gif" alt="dashboard"/>
+        <img src="jaal/assets/jaal_filter.gif" alt="dashboard"/>
         
         ### 3. Coloring
-        <img src="jaal/assest/jaal_color.gif" alt="dashboard"/>
+        <img src="jaal/assets/jaal_color.gif" alt="dashboard"/>
         
         ### 4. Size
-        <img src="jaal/assest/jaal_size.gif" alt="dashboard"/>
+        <img src="jaal/assets/jaal_size.gif" alt="dashboard"/>
         
         ## 👉 Extra settings
         
         ### Display edge label
         
         To display labels over edges, we need to add a `label` attribute (column) in the `edge_df`. Also, it has to be in `string` format. 
         For example, using the GoT dataset, by adding the following line before the `Jaal` call, we can display the edge labels.
         
         ```python
         # add edge labels
         edge_df.loc[:, 'label'] = edge_df.loc[:, 'weight'].astype(str)
         ```
+        ### Display image in node
+        
+        Currently it is possible to show image within node (with circular shape). For this, we need to put `node_image_url` column in the `node_df` with URLs for each node.
+        
+        <img src="jaal/assets/jaal_node_image.png" width="300" height="200" alt="dashboard"/>
         
         ### Directed edges
         
         By default, `Jaal` plot undirected edges. This setting can be changed by,
         
         ```python
         Jaal(edge_df, node_df).plot(directed=True)
         ```
         
+        ### Showing Tooltip
+        
+        By default, `nodeid` is shown as tooltip. To overwrite this, include a `title` column with the respective data.
+        
         ### Using vis.js settings
         
         We can tweak any of the `vis.js` related network visualization settings. An example is,
         
         ```python
         # init Jaal and run server
         Jaal(edge_df, node_df).plot(vis_opts={'height': '600px', # change height
```

### Comparing `jaal-0.1.3/setup.py` & `jaal-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
-    package_data={'': ['datasets/*', 'assest/logo.png', 'datasets/got/*']},
+    package_data={'': ['datasets/*', 'assets/logo.png', 'datasets/got/*']},
     include_package_data=True,
     install_requires=['dash>=1.19.0', 
                       'visdcc>=0.0.40', 
                       'pandas>=1.2.1', 
                       'dash_core_components>=1.15.0', 
                       'dash_html_components>=1.1.2', 
                       'dash_bootstrap_components<1'],
```

