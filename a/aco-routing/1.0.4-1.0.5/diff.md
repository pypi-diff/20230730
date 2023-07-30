# Comparing `tmp/aco_routing-1.0.4.tar.gz` & `tmp/aco_routing-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aco_routing-1.0.4.tar", last modified: Sat Jul 23 09:04:33 2022, max compression
+gzip compressed data, was "aco_routing-1.0.5.tar", last modified: Sun Jul 30 15:02:42 2023, max compression
```

## Comparing `aco_routing-1.0.4.tar` & `aco_routing-1.0.5.tar`

### file list

```diff
@@ -1,24 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 09:04:33.332529 aco_routing-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-07-23 09:04:22.000000 aco_routing-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7230 2022-07-23 09:04:33.332529 aco_routing-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5260 2022-07-23 09:04:22.000000 aco_routing-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 09:04:33.328529 aco_routing-1.0.4/aco_routing/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-23 09:04:22.000000 aco_routing-1.0.4/aco_routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4206 2022-07-23 09:04:22.000000 aco_routing-1.0.4/aco_routing/aco.py
--rw-r--r--   0 runner    (1001) docker     (121)     2151 2022-07-23 09:04:22.000000 aco_routing-1.0.4/aco_routing/dijkstra.py
--rw-r--r--   0 runner    (1001) docker     (121)      911 2022-07-23 09:04:22.000000 aco_routing-1.0.4/aco_routing/example.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 09:04:33.332529 aco_routing-1.0.4/aco_routing/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-23 09:04:22.000000 aco_routing-1.0.4/aco_routing/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6936 2022-07-23 09:04:22.000000 aco_routing-1.0.4/aco_routing/utils/ant.py
--rw-r--r--   0 runner    (1001) docker     (121)    10165 2022-07-23 09:04:22.000000 aco_routing-1.0.4/aco_routing/utils/graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     3532 2022-07-23 09:04:22.000000 aco_routing-1.0.4/aco_routing/utils/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 09:04:33.328529 aco_routing-1.0.4/aco_routing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7230 2022-07-23 09:04:33.000000 aco_routing-1.0.4/aco_routing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-07-23 09:04:33.000000 aco_routing-1.0.4/aco_routing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-23 09:04:33.000000 aco_routing-1.0.4/aco_routing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-07-23 09:04:33.000000 aco_routing-1.0.4/aco_routing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-23 09:04:33.332529 aco_routing-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1228 2022-07-23 09:04:22.000000 aco_routing-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 09:04:33.332529 aco_routing-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-23 09:04:22.000000 aco_routing-1.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-07-23 09:04:22.000000 aco_routing-1.0.4/tests/test_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:02:42.734166 aco_routing-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-30 15:02:30.000000 aco_routing-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-07-30 15:02:42.734166 aco_routing-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-07-30 15:02:30.000000 aco_routing-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:02:42.730166 aco_routing-1.0.5/aco_routing/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-30 15:02:30.000000 aco_routing-1.0.5/aco_routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-07-30 15:02:30.000000 aco_routing-1.0.5/aco_routing/aco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-07-30 15:02:30.000000 aco_routing-1.0.5/aco_routing/ant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-30 15:02:30.000000 aco_routing-1.0.5/aco_routing/dijkstra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-07-30 15:02:30.000000 aco_routing-1.0.5/aco_routing/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:02:42.730166 aco_routing-1.0.5/aco_routing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-07-30 15:02:42.000000 aco_routing-1.0.5/aco_routing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-30 15:02:42.000000 aco_routing-1.0.5/aco_routing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 15:02:42.000000 aco_routing-1.0.5/aco_routing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-30 15:02:42.000000 aco_routing-1.0.5/aco_routing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 15:02:42.734166 aco_routing-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-30 15:02:30.000000 aco_routing-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:02:42.730166 aco_routing-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:02:30.000000 aco_routing-1.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-30 15:02:30.000000 aco_routing-1.0.5/tests/test_graph.py
```

### Comparing `aco_routing-1.0.4/LICENSE` & `aco_routing-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aco_routing-1.0.4/PKG-INFO` & `aco_routing-1.0.5/aco_routing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: aco_routing
-Version: 1.0.4
-Summary: A Python package to find the shortest path in a graph using Ant Colony Optimization (ACO).
+Name: aco-routing
+Version: 1.0.5
+Summary: A Python package to find the shortest path in a graph using Ant Colony Optimization (ACO)
 Home-page: https://github.com/hasnainroopawalla/ant-colony-optimization
 Author: Hasnain Roopawalla
 Author-email: hasnain.roopawalla@gmail.com
 License: MIT
 Description: <h1 align="center">Ant Colony Optimization</h1>
```

### Comparing `aco_routing-1.0.4/README.md` & `aco_routing-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `aco_routing-1.0.4/aco_routing/aco.py` & `aco_routing-1.0.5/aco_routing/aco.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,65 @@
 from dataclasses import dataclass
 import random
 from typing import List, Tuple
 
-from aco_routing.utils.graph import Graph
-from aco_routing.utils.ant import Ant
+from aco_routing.graph import Graph
+from aco_routing.ant import Ant
 
 
 @dataclass
 class ACO:
     graph: Graph
 
     def _forward_ants(self, ants: List[Ant], max_iterations: int) -> None:
         """Deploys forward search ants in the graph.
 
         Args:
             ants (List[Ant]): A List of Ants.
-            max_iterations (int, optional): The maximum number of steps an ant is allowed is to take in order to reach the destination.
-                If it fails to find a path, it is tagged as unfit. Defaults to 50.
+            max_iterations (int): The maximum number of steps an ant is allowed is to take in order to reach the destination.
+                If it fails to find a path, it is tagged as unfit.
         """
-        for idx, ant in enumerate(ants):
-            for i in range(max_iterations):
+        for _, ant in enumerate(ants):
+            for _ in range(max_iterations):
                 if ant.reached_destination():
                     ant.is_fit = True
                     break
                 ant.take_step()
 
     def _backward_ants(self, ants: List[Ant]) -> None:
         """Sends the ants (which are fit) backwards towards the source while they drop pheromones on the path.
 
         Args:
             ants (List[Ant]): A List of Ants.
         """
-        for idx, ant in enumerate(ants):
+        for _, ant in enumerate(ants):
             if ant.is_fit:
                 self.graph.deposit_pheromones_along_path(ant.path)
 
     def _deploy_search_ants(
         self,
         source: str,
         destination: str,
         num_ants: int,
-        random_spawns: bool = False,
-        cycles: int = 100,
+        cycles: int,
+        random_spawns: bool,
         max_iterations: int = 50,
     ) -> None:
         """Deploys search ants which traverse the graph to find the shortest path.
 
         Args:
             source (str): The source node in the graph.
             destination (str): The destination node in the graph.
             num_ants (int): The number of ants to be spawned.
-            random_spawns (bool): A flag to determine if the ants should be spawned at random nodes or always at the source node.
-            cycles (int, optional): The number of cycles of generating and deploying ants (forward and backward). Defaults to 100.
-            max_iterations (int, optional): The maximum number of steps an ant is allowed is to take in order to reach the destination.
-                If it fails to find a path, it is tagged as unfit. Defaults to 50.
+            cycles (int): The number of cycles of generating and deploying ants (forward and backward).
+            random_spawns (bool): Indicates if the search ants should spawn at random nodes in the graph.
+            max_iterations (int, optional): The maximum number of steps an ant is allowed is to take in order to reach the destination,
+                after which it is tagged as unfit. Defaults to 50.
         """
-        for cycle in range(cycles):
+        for _ in range(cycles):
             ants: List[Ant] = []
             for _ in range(num_ants):
                 spawn_point = (
                     random.choice(self.graph.get_all_nodes())
                     if random_spawns
                     else source
                 )
@@ -75,28 +75,46 @@
             source (str): The source node in the graph.
             destination (str): The destination node in the graph.
 
         Returns:
             List[str]: The shortest path found by the ants (A list of node IDs).
         """
         # Spawn an ant which favors pheromone values over edge costs.
-        ant = Ant(self.graph, source, destination, alpha=0.99, beta=0.01)
+        ant = Ant(self.graph, source, destination, is_solution_ant=True)
         while not ant.reached_destination():
             ant.take_step()
         return ant.path
 
     def find_shortest_path(
-        self, source: str, destination: str
+        self,
+        source: str,
+        destination: str,
+        num_ants: int,
+        max_iterations: int,
+        cycles: int,
+        random_spawn: bool = True,
     ) -> Tuple[List[str], float]:
         """Finds the shortest path from the source to the destination in the graph using the traditional Ant Colony Optimization technique.
 
         Args:
             source (str): The source node in the graph.
             destination (str): The destination node in the graph.
+            num_ants (int): The number of search ants to be deployed.
+            max_iterations (int): The maximum number of steps an ant is allowed is to take in order to reach the destination,
+                after which it is tagged as unfit. Defaults to 50.
+            cycles (int): The number of cycles/waves of search ants to be deployed.
+            random_spawn (bool, optional): Indicates if the search ants should spawn at random nodes in the graph. Defaults to True.
 
         Returns:
-            List[str]: The shortest path found by the ants (A list of node IDs).
+            List[str]: The shortest path found by the ants (a list of node IDs).
             float: The total travel time of the shortest path.
         """
-        self._deploy_search_ants(source, destination, num_ants=20, random_spawns=True)
+        self._deploy_search_ants(
+            source,
+            destination,
+            num_ants=num_ants,
+            max_iterations=max_iterations,
+            cycles=cycles,
+            random_spawns=random_spawn,
+        )
         shortest_path = self._deploy_solution_ant(source, destination)
         return shortest_path, self.graph.compute_path_travel_time(shortest_path)
```

### Comparing `aco_routing-1.0.4/aco_routing/dijkstra.py` & `aco_routing-1.0.5/aco_routing/dijkstra.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from dataclasses import dataclass
 from typing import Dict, List, Tuple
 
-from aco_routing.utils.graph import Graph
+from aco_routing.graph import Graph
 
 
 @dataclass
 class Dijkstra:
-    """The basline Dijkstra's Algorithm to find the shortest path between 2 nodes in the graph.
+    """The basline Dijkstra's Algorithm to find the shortest path between two nodes in the graph.
     Reference: https://stackoverflow.com/a/61078380
     """
 
     graph: Graph
 
     def __post_init__(self) -> None:
         self.dijkstra_graph = self.graph.normalize_graph_for_dijkstra()
```

### Comparing `aco_routing-1.0.4/aco_routing/utils/ant.py` & `aco_routing-1.0.5/aco_routing/ant.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 from dataclasses import dataclass, field
 import random
 from typing import Dict, List, Set
 
-from aco_routing.utils.graph import Edge, Graph
+from aco_routing.graph import Edge, Graph
 
 
 @dataclass
 class Ant:
     """A class for an Ant that traverses the graph.
 
     Args:
         graph (Graph): The Graph object.
         source (str): The source node of the ant.
         destination (str): The destination node of the ant.
-        alpha (float): The amount of importance given to the pheromone by the ant. Defaults to 0.9.
-        beta (float): The amount of importance given to the travel time value by the ant. Defaults to 0.1.
-        visited_nodes (Set): A set of nodes that have been visited by the ant.
-        path (List[str]): A List of node IDs of the path taken by the ant so far.
-        is_fit (bool): A flag which indicates if the ant has reached the destination (fit) or not (unfit). Defaults to False.
+        alpha (float, optional): The amount of importance given to the pheromone by the ant. Defaults to 0.9.
+        beta (float, optional): The amount of importance given to the travel time value by the ant. Defaults to 0.1.
+        visited_nodes (Set, optional): A set of nodes that have been visited by the ant.
+        path (List[str], optional): A List of node IDs of the path taken by the ant so far.
+        is_fit (bool, optional): Indicates if the ant has reached the destination (fit) or not (unfit). Defaults to False.
+        is_solution_ant (bool, optional): Indicates if the ant is the final/solution ant. Defaults to False.
     """
 
     graph: Graph
     source: str
     destination: str
     alpha: float = 0.7
     beta: float = 0.3
     visited_nodes: Set = field(default_factory=set)
     path: List[str] = field(default_factory=list)
     is_fit: bool = False
+    is_solution_ant: bool = False
 
     def __post_init__(self) -> None:
         self.current_node = self.source
         self.path.append(self.source)
 
     def reached_destination(self) -> bool:
         """Checks if the ant has reached the destination node in the graph.
@@ -145,19 +147,27 @@
             unvisited_neighbors (Dict[str, Edge]): A set of unvisited neighbors of the current node.
             alpha (float): [description]: The alpha value.
             beta (float): [description]: The beta value.
 
         Returns:
             str: The ID of the next node to be visited by the ant.
         """
+        if self.is_solution_ant:
+            # The final/solution ant greedily chooses the next node with the highest pheromone value.
+            return max(
+                unvisited_neighbors, key=lambda k: unvisited_neighbors[k].pheromones
+            )
         edges_total = self._calculate_edges_total(unvisited_neighbors, alpha, beta)
+
         probabilities = self._calculate_edge_probabilites(
             unvisited_neighbors, edges_total, alpha, beta
         )
         sorted_probabilities = self._sort_edge_probabilites(probabilities)
+
+        # Pick the next node based on the Roulette Wheel selection technique.
         return self._choose_neighbor_using_roulette_wheel(sorted_probabilities)
 
     def take_step(self) -> None:
         """This method allows the ant to travel to a neighbor of the current node in the graph."""
         # Mark the node as visited.
         self.visited_nodes.add(self.current_node)
 
@@ -167,12 +177,15 @@
         # Check if the current node has no neighbors (isolated node).
         if len(all_neighbors) == 0:
             return
 
         # Find unvisited neighbors of the current node.
         unvisited_neighbors = self._get_unvisited_neighbors(all_neighbors)
 
-        # Pick the next node based on the Roulette Wheel selection technique.
+        # Pick the next node of the ant.
         next_node = self._pick_next_node(unvisited_neighbors, self.alpha, self.beta)
 
+        if not next_node:
+            return
+
         self.path.append(next_node)
         self.current_node = next_node
```

### Comparing `aco_routing-1.0.4/aco_routing/utils/graph.py` & `aco_routing-1.0.5/aco_routing/graph.py`

 * *Files identical despite different names*

### Comparing `aco_routing-1.0.4/aco_routing.egg-info/PKG-INFO` & `aco_routing-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: aco-routing
-Version: 1.0.4
-Summary: A Python package to find the shortest path in a graph using Ant Colony Optimization (ACO).
+Name: aco_routing
+Version: 1.0.5
+Summary: A Python package to find the shortest path in a graph using Ant Colony Optimization (ACO)
 Home-page: https://github.com/hasnainroopawalla/ant-colony-optimization
 Author: Hasnain Roopawalla
 Author-email: hasnain.roopawalla@gmail.com
 License: MIT
 Description: <h1 align="center">Ant Colony Optimization</h1>
```

### Comparing `aco_routing-1.0.4/setup.py` & `aco_routing-1.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 repository_dir = os.path.dirname(__file__)
 
 with open(os.path.join(repository_dir, "README.md")) as fh:
     long_description = fh.read()
 
 setup(
     name="aco_routing",
-    version="1.0.4",
+    version="1.0.5",
     packages=find_packages(exclude="tests"),
-    description="A Python package to find the shortest path in a graph using Ant Colony Optimization (ACO).",
+    description="A Python package to find the shortest path in a graph using Ant Colony Optimization (ACO)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hasnainroopawalla/ant-colony-optimization",
     author="Hasnain Roopawalla",
     author_email="hasnain.roopawalla@gmail.com",
     license="MIT",
     classifiers=[
```

### Comparing `aco_routing-1.0.4/tests/test_graph.py` & `aco_routing-1.0.5/tests/test_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from aco_routing.utils.graph import Graph
+from aco_routing import Graph
 
 G = Graph()
 
 G.add_node("A")
 G.add_node("B")
 G.add_node("C")
```

