# Comparing `tmp/aco_routing-1.0.5.tar.gz` & `tmp/aco_routing-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aco_routing-1.0.5.tar", last modified: Sun Jul 30 15:02:42 2023, max compression
+gzip compressed data, was "aco_routing-1.0.6.tar", last modified: Sun Jul 30 15:19:33 2023, max compression
```

## Comparing `aco_routing-1.0.5.tar` & `aco_routing-1.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:02:42.734166 aco_routing-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-30 15:02:30.000000 aco_routing-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-07-30 15:02:42.734166 aco_routing-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-07-30 15:02:30.000000 aco_routing-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:02:42.730166 aco_routing-1.0.5/aco_routing/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-30 15:02:30.000000 aco_routing-1.0.5/aco_routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-07-30 15:02:30.000000 aco_routing-1.0.5/aco_routing/aco.py
--rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-07-30 15:02:30.000000 aco_routing-1.0.5/aco_routing/ant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-30 15:02:30.000000 aco_routing-1.0.5/aco_routing/dijkstra.py
--rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-07-30 15:02:30.000000 aco_routing-1.0.5/aco_routing/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:02:42.730166 aco_routing-1.0.5/aco_routing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-07-30 15:02:42.000000 aco_routing-1.0.5/aco_routing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-30 15:02:42.000000 aco_routing-1.0.5/aco_routing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 15:02:42.000000 aco_routing-1.0.5/aco_routing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-30 15:02:42.000000 aco_routing-1.0.5/aco_routing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 15:02:42.734166 aco_routing-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-30 15:02:30.000000 aco_routing-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:02:42.730166 aco_routing-1.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:02:30.000000 aco_routing-1.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-30 15:02:30.000000 aco_routing-1.0.5/tests/test_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:19:33.501070 aco_routing-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-30 15:19:23.000000 aco_routing-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-07-30 15:19:33.501070 aco_routing-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-07-30 15:19:23.000000 aco_routing-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:19:33.501070 aco_routing-1.0.6/aco_routing/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-30 15:19:23.000000 aco_routing-1.0.6/aco_routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-07-30 15:19:23.000000 aco_routing-1.0.6/aco_routing/aco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-07-30 15:19:23.000000 aco_routing-1.0.6/aco_routing/ant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-30 15:19:23.000000 aco_routing-1.0.6/aco_routing/dijkstra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-07-30 15:19:23.000000 aco_routing-1.0.6/aco_routing/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:19:33.501070 aco_routing-1.0.6/aco_routing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-07-30 15:19:33.000000 aco_routing-1.0.6/aco_routing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-30 15:19:33.000000 aco_routing-1.0.6/aco_routing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 15:19:33.000000 aco_routing-1.0.6/aco_routing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-30 15:19:33.000000 aco_routing-1.0.6/aco_routing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 15:19:33.501070 aco_routing-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-30 15:19:23.000000 aco_routing-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:19:33.501070 aco_routing-1.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:19:23.000000 aco_routing-1.0.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-30 15:19:23.000000 aco_routing-1.0.6/tests/test_graph.py
```

### Comparing `aco_routing-1.0.5/LICENSE` & `aco_routing-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aco_routing-1.0.5/PKG-INFO` & `aco_routing-1.0.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aco_routing
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Python package to find the shortest path in a graph using Ant Colony Optimization (ACO)
 Home-page: https://github.com/hasnainroopawalla/ant-colony-optimization
 Author: Hasnain Roopawalla
 Author-email: hasnain.roopawalla@gmail.com
 License: MIT
 Description: <h1 align="center">Ant Colony Optimization</h1>
         
@@ -32,22 +32,19 @@
         ### To install the package directly from PyPi:
         ```
         $ pip install aco_routing
         ```
         
         
         ## 🎈 Usage <a name="usage"></a>
-        > **_Check out:_** [aco_routing/example.py](https://github.com/hasnainroopawalla/Ant-Colony-Optimization/tree/master/aco_routing/example.py)
+        > **_Check out:_** [example.py](https://github.com/hasnainroopawalla/Ant-Colony-Optimization/blob/00cd068597ab9a69a8eb81c8a3fd984797d2eefd/example.py)
         
         Import all the dependencies.
         ```python
-        from aco_routing.utils.graph import Graph
-        from aco_routing.dijkstra import Dijkstra
-        from aco_routing.utils.simulator import Simulator
-        from aco_routing.aco import ACO
+        from aco_routing import Graph, Dijkstra, ACO
         ```
         
         Create a `Graph` object.
         ```python
         graph = Graph()
         ```
         
@@ -62,15 +59,15 @@
         graph.add_edge("G", "F", travel_time=1)
         graph.add_edge("F", "C", travel_time=1)
         graph.add_edge("C", "D", travel_time=10)
         graph.add_edge("E", "D", travel_time=2)
         graph.add_edge("G", "E", travel_time=2)
         ```
         
-        Define a `source` and `destination` as well create objects for the `Dijkstra` and `ACO` classes.
+        Define a `source` and `destination` as well as create objects for the `Dijkstra` and `ACO` classes.
         ```python
         source = "A"
         destination = "D"
         
         aco = ACO(graph)
         dijkstra = Dijkstra(graph)
         ```
@@ -80,57 +77,51 @@
         dijkstra_path, dijkstra_cost = dijkstra.find_shortest_path(source, destination)
         aco_path, aco_cost = aco.find_shortest_path(source, destination)
         
         print(f"ACO - path: {aco_path}, cost: {aco_cost}")
         print(f"Dijkstra - path: {dijkstra_path}, cost: {dijkstra_cost}")
         ```
         
-        Simulate a real-life scenario with various episodes of stochastically updating traffic conditions in a city.
-        ```python
-        Simulator(graph).simulate(source, destination, num_episodes=100, plot=True)
+        Output:
+        ```
+        ACO - path: ['A', 'H', 'G', 'E', 'D'], cost: 8.0
+        Dijkstra - path: ['A', 'H', 'G', 'E', 'D'], cost: 8.0
         ```
-        
         
         ## 📦 Contents <a name = "contents"></a>
         
         ### Graph
-        `aco_routing.utils.graph.Graph`
+        `aco_routing.Graph`
         - A Directed Graph class which consists of `Nodes` and `Edges`.
         - The `evaporation_rate` is initialized here.
         
         ### Node
-        `aco_routing.utils.graph.Node`
+        `aco_routing.Node`
         - A `Node` class which represents a node in the Graph and consists of various outgoing edges.
         
         ### Edge
-        `aco_routing.utils.graph.Edge`
+        `aco_routing.Edge`
         - An `Edge` class which represents a link between 2 nodes in the Graph.
         - Each `Edge` has 2 parameters:
             - `travel_time`: The amount of time it takes to traverse the edge. A high value indicates more traffic.
             - `pheromones`: A heuristic parameter i.e., the pheromone values deposited by the ants.
         
         ### Dijkstra
-        `aco_routing.dijkstra.Dijkstra`
+        `aco_routing.Dijkstra`
         - The baseline algorithm to compare the results of the candidate algorithm with.
         - The Dijkstra's algorithm ([source](https://en.wikipedia.org/wiki/Dijkstra%27s_algorithm)) returns the shortest path between any 2 nodes in a graph.
         
         ### Ant
-        `aco_routing.utils.ant.Ant`
+        `aco_routing.Ant`
         - The `Ant` class representing an ant that traverses the graph.
         
         ### ACO
-        `aco_routing.aco.ACO`
+        `aco_routing.ACO`
         - The traditional Ant Colony Optimization algorithm that spawns various ants at random nodes and tries to find the shortest path between the specified source and destination.
         
-        ### Simulator
-        `aco_routing.utils.simulator.Simulator`
-        - The simulator class is used to simulate and evaluate the performance of the candidate algorithm (ACO) with a baseline Dijkstra's Algorithm.
-        - It simulates a real-life city, where the traffic conditions change every episode in a conditionally stochastic manner.
-        - The ants continue to find the shortest path even after the traffic conditions change.
-        
         <hr>
         
         
         ## Contributing
         
         - Post any issues and suggestions on the GitHub [issues](https://github.com/hasnainroopawalla/Ant-Colony-Optimization/issues) page.
         - To contribute, fork the project and then create a pull request back to master.
```

### Comparing `aco_routing-1.0.5/README.md` & `aco_routing-1.0.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -24,22 +24,19 @@
 ### To install the package directly from PyPi:
 ```
 $ pip install aco_routing
 ```
 
 
 ## 🎈 Usage <a name="usage"></a>
-> **_Check out:_** [aco_routing/example.py](https://github.com/hasnainroopawalla/Ant-Colony-Optimization/tree/master/aco_routing/example.py)
+> **_Check out:_** [example.py](https://github.com/hasnainroopawalla/Ant-Colony-Optimization/blob/00cd068597ab9a69a8eb81c8a3fd984797d2eefd/example.py)
 
 Import all the dependencies.
 ```python
-from aco_routing.utils.graph import Graph
-from aco_routing.dijkstra import Dijkstra
-from aco_routing.utils.simulator import Simulator
-from aco_routing.aco import ACO
+from aco_routing import Graph, Dijkstra, ACO
 ```
 
 Create a `Graph` object.
 ```python
 graph = Graph()
 ```
 
@@ -54,15 +51,15 @@
 graph.add_edge("G", "F", travel_time=1)
 graph.add_edge("F", "C", travel_time=1)
 graph.add_edge("C", "D", travel_time=10)
 graph.add_edge("E", "D", travel_time=2)
 graph.add_edge("G", "E", travel_time=2)
 ```
 
-Define a `source` and `destination` as well create objects for the `Dijkstra` and `ACO` classes.
+Define a `source` and `destination` as well as create objects for the `Dijkstra` and `ACO` classes.
 ```python
 source = "A"
 destination = "D"
 
 aco = ACO(graph)
 dijkstra = Dijkstra(graph)
 ```
@@ -72,57 +69,51 @@
 dijkstra_path, dijkstra_cost = dijkstra.find_shortest_path(source, destination)
 aco_path, aco_cost = aco.find_shortest_path(source, destination)
 
 print(f"ACO - path: {aco_path}, cost: {aco_cost}")
 print(f"Dijkstra - path: {dijkstra_path}, cost: {dijkstra_cost}")
 ```
 
-Simulate a real-life scenario with various episodes of stochastically updating traffic conditions in a city.
-```python
-Simulator(graph).simulate(source, destination, num_episodes=100, plot=True)
+Output:
+```
+ACO - path: ['A', 'H', 'G', 'E', 'D'], cost: 8.0
+Dijkstra - path: ['A', 'H', 'G', 'E', 'D'], cost: 8.0
 ```
-
 
 ## 📦 Contents <a name = "contents"></a>
 
 ### Graph
-`aco_routing.utils.graph.Graph`
+`aco_routing.Graph`
 - A Directed Graph class which consists of `Nodes` and `Edges`.
 - The `evaporation_rate` is initialized here.
 
 ### Node
-`aco_routing.utils.graph.Node`
+`aco_routing.Node`
 - A `Node` class which represents a node in the Graph and consists of various outgoing edges.
 
 ### Edge
-`aco_routing.utils.graph.Edge`
+`aco_routing.Edge`
 - An `Edge` class which represents a link between 2 nodes in the Graph.
 - Each `Edge` has 2 parameters:
     - `travel_time`: The amount of time it takes to traverse the edge. A high value indicates more traffic.
     - `pheromones`: A heuristic parameter i.e., the pheromone values deposited by the ants.
 
 ### Dijkstra
-`aco_routing.dijkstra.Dijkstra`
+`aco_routing.Dijkstra`
 - The baseline algorithm to compare the results of the candidate algorithm with.
 - The Dijkstra's algorithm ([source](https://en.wikipedia.org/wiki/Dijkstra%27s_algorithm)) returns the shortest path between any 2 nodes in a graph.
 
 ### Ant
-`aco_routing.utils.ant.Ant`
+`aco_routing.Ant`
 - The `Ant` class representing an ant that traverses the graph.
 
 ### ACO
-`aco_routing.aco.ACO`
+`aco_routing.ACO`
 - The traditional Ant Colony Optimization algorithm that spawns various ants at random nodes and tries to find the shortest path between the specified source and destination.
 
-### Simulator
-`aco_routing.utils.simulator.Simulator`
-- The simulator class is used to simulate and evaluate the performance of the candidate algorithm (ACO) with a baseline Dijkstra's Algorithm.
-- It simulates a real-life city, where the traffic conditions change every episode in a conditionally stochastic manner.
-- The ants continue to find the shortest path even after the traffic conditions change.
-
 <hr>
 
 
 ## Contributing
 
 - Post any issues and suggestions on the GitHub [issues](https://github.com/hasnainroopawalla/Ant-Colony-Optimization/issues) page.
 - To contribute, fork the project and then create a pull request back to master.
```

### Comparing `aco_routing-1.0.5/aco_routing/aco.py` & `aco_routing-1.0.6/aco_routing/aco.py`

 * *Files identical despite different names*

### Comparing `aco_routing-1.0.5/aco_routing/ant.py` & `aco_routing-1.0.6/aco_routing/ant.py`

 * *Files identical despite different names*

### Comparing `aco_routing-1.0.5/aco_routing/dijkstra.py` & `aco_routing-1.0.6/aco_routing/dijkstra.py`

 * *Files identical despite different names*

### Comparing `aco_routing-1.0.5/aco_routing/graph.py` & `aco_routing-1.0.6/aco_routing/graph.py`

 * *Files identical despite different names*

### Comparing `aco_routing-1.0.5/aco_routing.egg-info/PKG-INFO` & `aco_routing-1.0.6/aco_routing.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aco-routing
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Python package to find the shortest path in a graph using Ant Colony Optimization (ACO)
 Home-page: https://github.com/hasnainroopawalla/ant-colony-optimization
 Author: Hasnain Roopawalla
 Author-email: hasnain.roopawalla@gmail.com
 License: MIT
 Description: <h1 align="center">Ant Colony Optimization</h1>
         
@@ -32,22 +32,19 @@
         ### To install the package directly from PyPi:
         ```
         $ pip install aco_routing
         ```
         
         
         ## 🎈 Usage <a name="usage"></a>
-        > **_Check out:_** [aco_routing/example.py](https://github.com/hasnainroopawalla/Ant-Colony-Optimization/tree/master/aco_routing/example.py)
+        > **_Check out:_** [example.py](https://github.com/hasnainroopawalla/Ant-Colony-Optimization/blob/00cd068597ab9a69a8eb81c8a3fd984797d2eefd/example.py)
         
         Import all the dependencies.
         ```python
-        from aco_routing.utils.graph import Graph
-        from aco_routing.dijkstra import Dijkstra
-        from aco_routing.utils.simulator import Simulator
-        from aco_routing.aco import ACO
+        from aco_routing import Graph, Dijkstra, ACO
         ```
         
         Create a `Graph` object.
         ```python
         graph = Graph()
         ```
         
@@ -62,15 +59,15 @@
         graph.add_edge("G", "F", travel_time=1)
         graph.add_edge("F", "C", travel_time=1)
         graph.add_edge("C", "D", travel_time=10)
         graph.add_edge("E", "D", travel_time=2)
         graph.add_edge("G", "E", travel_time=2)
         ```
         
-        Define a `source` and `destination` as well create objects for the `Dijkstra` and `ACO` classes.
+        Define a `source` and `destination` as well as create objects for the `Dijkstra` and `ACO` classes.
         ```python
         source = "A"
         destination = "D"
         
         aco = ACO(graph)
         dijkstra = Dijkstra(graph)
         ```
@@ -80,57 +77,51 @@
         dijkstra_path, dijkstra_cost = dijkstra.find_shortest_path(source, destination)
         aco_path, aco_cost = aco.find_shortest_path(source, destination)
         
         print(f"ACO - path: {aco_path}, cost: {aco_cost}")
         print(f"Dijkstra - path: {dijkstra_path}, cost: {dijkstra_cost}")
         ```
         
-        Simulate a real-life scenario with various episodes of stochastically updating traffic conditions in a city.
-        ```python
-        Simulator(graph).simulate(source, destination, num_episodes=100, plot=True)
+        Output:
+        ```
+        ACO - path: ['A', 'H', 'G', 'E', 'D'], cost: 8.0
+        Dijkstra - path: ['A', 'H', 'G', 'E', 'D'], cost: 8.0
         ```
-        
         
         ## 📦 Contents <a name = "contents"></a>
         
         ### Graph
-        `aco_routing.utils.graph.Graph`
+        `aco_routing.Graph`
         - A Directed Graph class which consists of `Nodes` and `Edges`.
         - The `evaporation_rate` is initialized here.
         
         ### Node
-        `aco_routing.utils.graph.Node`
+        `aco_routing.Node`
         - A `Node` class which represents a node in the Graph and consists of various outgoing edges.
         
         ### Edge
-        `aco_routing.utils.graph.Edge`
+        `aco_routing.Edge`
         - An `Edge` class which represents a link between 2 nodes in the Graph.
         - Each `Edge` has 2 parameters:
             - `travel_time`: The amount of time it takes to traverse the edge. A high value indicates more traffic.
             - `pheromones`: A heuristic parameter i.e., the pheromone values deposited by the ants.
         
         ### Dijkstra
-        `aco_routing.dijkstra.Dijkstra`
+        `aco_routing.Dijkstra`
         - The baseline algorithm to compare the results of the candidate algorithm with.
         - The Dijkstra's algorithm ([source](https://en.wikipedia.org/wiki/Dijkstra%27s_algorithm)) returns the shortest path between any 2 nodes in a graph.
         
         ### Ant
-        `aco_routing.utils.ant.Ant`
+        `aco_routing.Ant`
         - The `Ant` class representing an ant that traverses the graph.
         
         ### ACO
-        `aco_routing.aco.ACO`
+        `aco_routing.ACO`
         - The traditional Ant Colony Optimization algorithm that spawns various ants at random nodes and tries to find the shortest path between the specified source and destination.
         
-        ### Simulator
-        `aco_routing.utils.simulator.Simulator`
-        - The simulator class is used to simulate and evaluate the performance of the candidate algorithm (ACO) with a baseline Dijkstra's Algorithm.
-        - It simulates a real-life city, where the traffic conditions change every episode in a conditionally stochastic manner.
-        - The ants continue to find the shortest path even after the traffic conditions change.
-        
         <hr>
         
         
         ## Contributing
         
         - Post any issues and suggestions on the GitHub [issues](https://github.com/hasnainroopawalla/Ant-Colony-Optimization/issues) page.
         - To contribute, fork the project and then create a pull request back to master.
```

### Comparing `aco_routing-1.0.5/setup.py` & `aco_routing-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 repository_dir = os.path.dirname(__file__)
 
 with open(os.path.join(repository_dir, "README.md")) as fh:
     long_description = fh.read()
 
 setup(
     name="aco_routing",
-    version="1.0.5",
+    version="1.0.6",
     packages=find_packages(exclude="tests"),
     description="A Python package to find the shortest path in a graph using Ant Colony Optimization (ACO)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hasnainroopawalla/ant-colony-optimization",
     author="Hasnain Roopawalla",
     author_email="hasnain.roopawalla@gmail.com",
```

### Comparing `aco_routing-1.0.5/tests/test_graph.py` & `aco_routing-1.0.6/tests/test_graph.py`

 * *Files identical despite different names*

