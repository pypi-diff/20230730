# Comparing `tmp/pydantic-mermaid-0.2.0.tar.gz` & `tmp/pydantic-mermaid-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydantic-mermaid-0.2.0.tar", last modified: Sun Mar 19 16:21:51 2023, max compression
+gzip compressed data, was "dist/pydantic-mermaid-0.3.0.tar", last modified: Sun Jul 30 02:13:50 2023, max compression
```

## Comparing `pydantic-mermaid-0.2.0.tar` & `pydantic-mermaid-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 eric      (1000) eric      (1000)        0 2023-03-19 16:21:51.000000 pydantic-mermaid-0.2.0/
--rw-r--r--   0 eric      (1000) eric      (1000)     3069 2023-03-19 16:21:51.000000 pydantic-mermaid-0.2.0/PKG-INFO
--rw-r--r--   0 eric      (1000) eric      (1000)     2611 2023-03-19 13:23:50.000000 pydantic-mermaid-0.2.0/README.md
-drwxr-xr-x   0 eric      (1000) eric      (1000)        0 2023-03-19 16:21:51.000000 pydantic-mermaid-0.2.0/pydantic_mermaid/
--rw-r--r--   0 eric      (1000) eric      (1000)       83 2023-03-19 12:25:20.000000 pydantic-mermaid-0.2.0/pydantic_mermaid/__init__.py
--rw-r--r--   0 eric      (1000) eric      (1000)     2276 2023-03-19 16:13:44.000000 pydantic-mermaid-0.2.0/pydantic_mermaid/__main__.py
--rw-r--r--   0 eric      (1000) eric      (1000)     6434 2023-03-19 16:02:59.000000 pydantic-mermaid-0.2.0/pydantic_mermaid/mermaid_generator.py
--rw-r--r--   0 eric      (1000) eric      (1000)     1329 2023-03-19 15:58:46.000000 pydantic-mermaid-0.2.0/pydantic_mermaid/models.py
--rw-r--r--   0 eric      (1000) eric      (1000)        0 2023-03-18 12:31:31.000000 pydantic-mermaid-0.2.0/pydantic_mermaid/py.typed
-drwxr-xr-x   0 eric      (1000) eric      (1000)        0 2023-03-19 16:21:51.000000 pydantic-mermaid-0.2.0/pydantic_mermaid.egg-info/
--rw-r--r--   0 eric      (1000) eric      (1000)     3069 2023-03-19 16:21:51.000000 pydantic-mermaid-0.2.0/pydantic_mermaid.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) eric      (1000)      434 2023-03-19 16:21:51.000000 pydantic-mermaid-0.2.0/pydantic_mermaid.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) eric      (1000)        1 2023-03-19 16:21:51.000000 pydantic-mermaid-0.2.0/pydantic_mermaid.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) eric      (1000)       68 2023-03-19 16:21:51.000000 pydantic-mermaid-0.2.0/pydantic_mermaid.egg-info/entry_points.txt
--rw-r--r--   0 eric      (1000) eric      (1000)        9 2023-03-19 16:21:51.000000 pydantic-mermaid-0.2.0/pydantic_mermaid.egg-info/requires.txt
--rw-r--r--   0 eric      (1000) eric      (1000)       17 2023-03-19 16:21:51.000000 pydantic-mermaid-0.2.0/pydantic_mermaid.egg-info/top_level.txt
--rw-r--r--   0 eric      (1000) eric      (1000)       38 2023-03-19 16:21:51.000000 pydantic-mermaid-0.2.0/setup.cfg
--rw-r--r--   0 eric      (1000) eric      (1000)      933 2023-03-19 16:11:24.000000 pydantic-mermaid-0.2.0/setup.py
-drwxr-xr-x   0 eric      (1000) eric      (1000)        0 2023-03-19 16:21:51.000000 pydantic-mermaid-0.2.0/tests/
--rw-r--r--   0 eric      (1000) eric      (1000)      429 2023-03-19 15:53:51.000000 pydantic-mermaid-0.2.0/tests/test_basic_test.py
+drwxr-xr-x   0 eric      (1000) eric      (1000)        0 2023-07-30 02:13:50.000000 pydantic-mermaid-0.3.0/
+-rw-r--r--   0 eric      (1000) eric      (1000)     2926 2023-07-30 02:13:50.000000 pydantic-mermaid-0.3.0/PKG-INFO
+-rw-r--r--   0 eric      (1000) eric      (1000)     2468 2023-03-19 16:43:08.000000 pydantic-mermaid-0.3.0/README.md
+drwxr-xr-x   0 eric      (1000) eric      (1000)        0 2023-07-30 02:13:50.000000 pydantic-mermaid-0.3.0/pydantic_mermaid/
+-rw-r--r--   0 eric      (1000) eric      (1000)       83 2023-03-19 12:25:20.000000 pydantic-mermaid-0.3.0/pydantic_mermaid/__init__.py
+-rw-r--r--   0 eric      (1000) eric      (1000)     2276 2023-03-19 16:13:44.000000 pydantic-mermaid-0.3.0/pydantic_mermaid/__main__.py
+-rw-r--r--   0 eric      (1000) eric      (1000)     6437 2023-07-30 02:07:21.000000 pydantic-mermaid-0.3.0/pydantic_mermaid/mermaid_generator.py
+-rw-r--r--   0 eric      (1000) eric      (1000)     1329 2023-03-19 15:58:46.000000 pydantic-mermaid-0.3.0/pydantic_mermaid/models.py
+-rw-r--r--   0 eric      (1000) eric      (1000)        0 2023-03-18 12:31:31.000000 pydantic-mermaid-0.3.0/pydantic_mermaid/py.typed
+drwxr-xr-x   0 eric      (1000) eric      (1000)        0 2023-07-30 02:13:50.000000 pydantic-mermaid-0.3.0/pydantic_mermaid.egg-info/
+-rw-r--r--   0 eric      (1000) eric      (1000)     2926 2023-07-30 02:13:50.000000 pydantic-mermaid-0.3.0/pydantic_mermaid.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) eric      (1000)      434 2023-07-30 02:13:50.000000 pydantic-mermaid-0.3.0/pydantic_mermaid.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) eric      (1000)        1 2023-07-30 02:13:50.000000 pydantic-mermaid-0.3.0/pydantic_mermaid.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) eric      (1000)       68 2023-07-30 02:13:50.000000 pydantic-mermaid-0.3.0/pydantic_mermaid.egg-info/entry_points.txt
+-rw-r--r--   0 eric      (1000) eric      (1000)        9 2023-07-30 02:13:50.000000 pydantic-mermaid-0.3.0/pydantic_mermaid.egg-info/requires.txt
+-rw-r--r--   0 eric      (1000) eric      (1000)       17 2023-07-30 02:13:50.000000 pydantic-mermaid-0.3.0/pydantic_mermaid.egg-info/top_level.txt
+-rw-r--r--   0 eric      (1000) eric      (1000)       38 2023-07-30 02:13:50.000000 pydantic-mermaid-0.3.0/setup.cfg
+-rw-r--r--   0 eric      (1000) eric      (1000)      933 2023-07-30 02:13:41.000000 pydantic-mermaid-0.3.0/setup.py
+drwxr-xr-x   0 eric      (1000) eric      (1000)        0 2023-07-30 02:13:50.000000 pydantic-mermaid-0.3.0/tests/
+-rw-r--r--   0 eric      (1000) eric      (1000)      429 2023-03-19 15:53:51.000000 pydantic-mermaid-0.3.0/tests/test_basic_test.py
```

### Comparing `pydantic-mermaid-0.2.0/PKG-INFO` & `pydantic-mermaid-0.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-mermaid
-Version: 0.2.0
+Version: 0.3.0
 Summary: Convert pydantic classes to markdown mermaid class charts
 Home-page: https://github.com/EricWebsmith/pydantic_mermaid
 Author: Eric Websmith
 Author-email: eric.websmith@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -103,52 +103,47 @@
     Bird <|-- Eagle
 ```
 
 dependencies:
 
 ```mermaid
 classDiagram
-    class County {
+    class Place {
         name: str
         population: int
     }
 
+    class County {
+    }
+
     class Region {
-        name: str
-        population: int
         counties: List[County]
     }
 
     class Province {
-        name: str
-        population: int
         regions: List[Region]
     }
 
     class City {
-        name: str
-        population: int
         counties: List[County]
     }
 
     class Country {
-        name: str
-        population: int
         provinces: List[Province]
         cities: List[City]
     }
 
 
     Region ..> County
     Province ..> Region
     City ..> County
-    Country ..> City
     Country ..> Province
+    Country ..> City
 
-    Region --|> Place
-    County --|> Place
-    City --|> Place
-    Country --|> Place
-    Province --|> Place
+    Place <|-- City
+    Place <|-- County
+    Place <|-- Country
+    Place <|-- Province
+    Place <|-- Region
 ```
 
 For details, check examples/ folder.
```

### Comparing `pydantic-mermaid-0.2.0/README.md` & `pydantic-mermaid-0.3.0/pydantic_mermaid.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: pydantic-mermaid
+Version: 0.3.0
+Summary: Convert pydantic classes to markdown mermaid class charts
+Home-page: https://github.com/EricWebsmith/pydantic_mermaid
+Author: Eric Websmith
+Author-email: eric.websmith@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 # Pydantic Mermaid
 To convert Pydantic models to Mermaid charts, you can use the `pydantic-mermaid` library. This library allows you to generate Mermaid charts from your Pydantic models. Here are the steps to install and use pydantic-mermaid:
 
 # Use in terminal
 
 Install the `pydantic-mermaid` library using pip:
 
@@ -90,52 +103,47 @@
     Bird <|-- Eagle
 ```
 
 dependencies:
 
 ```mermaid
 classDiagram
-    class County {
+    class Place {
         name: str
         population: int
     }
 
+    class County {
+    }
+
     class Region {
-        name: str
-        population: int
         counties: List[County]
     }
 
     class Province {
-        name: str
-        population: int
         regions: List[Region]
     }
 
     class City {
-        name: str
-        population: int
         counties: List[County]
     }
 
     class Country {
-        name: str
-        population: int
         provinces: List[Province]
         cities: List[City]
     }
 
 
     Region ..> County
     Province ..> Region
     City ..> County
-    Country ..> City
     Country ..> Province
+    Country ..> City
 
-    Region --|> Place
-    County --|> Place
-    City --|> Place
-    Country --|> Place
-    Province --|> Place
+    Place <|-- City
+    Place <|-- County
+    Place <|-- Country
+    Place <|-- Province
+    Place <|-- Region
 ```
 
-For details, check examples/ folder.
+For details, check examples/ folder.
```

### Comparing `pydantic-mermaid-0.2.0/pydantic_mermaid/__main__.py` & `pydantic-mermaid-0.3.0/pydantic_mermaid/__main__.py`

 * *Files identical despite different names*

### Comparing `pydantic-mermaid-0.2.0/pydantic_mermaid/mermaid_generator.py` & `pydantic-mermaid-0.3.0/pydantic_mermaid/mermaid_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         """print inheritance for class chart"""
         s = ""
         for parent, children in self.parent_children.items():
             for child in children:
                 s += f"    {parent} <|-- {child}\n"
         return s
 
-    def generate_chart(self, root: str = "", relations: Relations = Relations.Dependency) -> str:
+    def generate_chart(self, *, root: str = "", relations: Relations = Relations.Dependency) -> str:
         """print class chart"""
         self.generate_allow_list(root)
 
         s = "```mermaid\nclassDiagram"
         for class_name, class_type in self.class_dict.items():
             if class_name not in self.allow_list:
                 continue
```

### Comparing `pydantic-mermaid-0.2.0/pydantic_mermaid/models.py` & `pydantic-mermaid-0.3.0/pydantic_mermaid/models.py`

 * *Files identical despite different names*

### Comparing `pydantic-mermaid-0.2.0/setup.py` & `pydantic-mermaid-0.3.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup  # type: ignore
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='pydantic-mermaid',
-    version='0.2.0',
+    version='0.3.0',
     description='Convert pydantic classes to markdown mermaid class charts',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Eric Websmith',
     author_email='eric.websmith@gmail.com',
     url='https://github.com/EricWebsmith/pydantic_mermaid',
     packages=['pydantic_mermaid'],
```

