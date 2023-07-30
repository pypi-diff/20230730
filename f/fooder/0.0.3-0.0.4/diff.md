# Comparing `tmp/fooder-0.0.3.tar.gz` & `tmp/fooder-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fooder-0.0.3.tar", last modified: Wed Apr 19 16:41:50 2023, max compression
+gzip compressed data, was "fooder-0.0.4.tar", last modified: Sun Jul 30 18:48:08 2023, max compression
```

## Comparing `fooder-0.0.3.tar` & `fooder-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 doman      (501) staff       (20)        0 2023-04-19 16:41:50.160477 fooder-0.0.3/
--rw-r--r--   0 doman      (501) staff       (20)    35149 2023-04-17 21:36:03.000000 fooder-0.0.3/LICENSE
--rw-r--r--   0 doman      (501) staff       (20)     2134 2023-04-19 16:41:50.160534 fooder-0.0.3/PKG-INFO
-drwxr-xr-x   0 doman      (501) staff       (20)        0 2023-04-19 16:41:50.158634 fooder-0.0.3/fooder.egg-info/
--rw-r--r--   0 doman      (501) staff       (20)     2134 2023-04-19 16:41:50.000000 fooder-0.0.3/fooder.egg-info/PKG-INFO
--rw-r--r--   0 doman      (501) staff       (20)      375 2023-04-19 16:41:50.000000 fooder-0.0.3/fooder.egg-info/SOURCES.txt
--rw-r--r--   0 doman      (501) staff       (20)        1 2023-04-19 16:41:50.000000 fooder-0.0.3/fooder.egg-info/dependency_links.txt
--rw-r--r--   0 doman      (501) staff       (20)       49 2023-04-19 16:41:50.000000 fooder-0.0.3/fooder.egg-info/entry_points.txt
--rw-r--r--   0 doman      (501) staff       (20)       40 2023-04-19 16:41:50.000000 fooder-0.0.3/fooder.egg-info/requires.txt
--rw-r--r--   0 doman      (501) staff       (20)       11 2023-04-19 16:41:50.000000 fooder-0.0.3/fooder.egg-info/top_level.txt
-drwxr-xr-x   0 doman      (501) staff       (20)        0 2023-04-19 16:41:50.160290 fooder-0.0.3/fooder_cli/
--rw-r--r--   0 doman      (501) staff       (20)        0 2023-04-17 21:36:03.000000 fooder-0.0.3/fooder_cli/__init__.py
--rw-r--r--   0 doman      (501) staff       (20)       63 2023-04-17 21:36:03.000000 fooder-0.0.3/fooder_cli/__main__.py
--rw-r--r--   0 doman      (501) staff       (20)     9704 2023-04-18 10:04:23.000000 fooder-0.0.3/fooder_cli/client.py
--rw-r--r--   0 doman      (501) staff       (20)     1626 2023-04-18 10:06:34.000000 fooder-0.0.3/fooder_cli/diary.py
--rw-r--r--   0 doman      (501) staff       (20)      675 2023-04-18 10:04:11.000000 fooder-0.0.3/fooder_cli/entry.py
--rw-r--r--   0 doman      (501) staff       (20)     3785 2023-04-19 16:39:05.000000 fooder-0.0.3/fooder_cli/main.py
--rw-r--r--   0 doman      (501) staff       (20)      719 2023-04-18 10:04:56.000000 fooder-0.0.3/fooder_cli/meal.py
--rw-r--r--   0 doman      (501) staff       (20)     2717 2023-04-18 10:05:40.000000 fooder-0.0.3/fooder_cli/product.py
--rw-r--r--   0 doman      (501) staff       (20)      100 2023-04-19 16:41:50.160833 fooder-0.0.3/setup.cfg
--rw-r--r--   0 doman      (501) staff       (20)      973 2023-04-19 16:39:48.000000 fooder-0.0.3/setup.py
+drwxr-xr-x   0 doman      (501) staff       (20)        0 2023-07-30 18:48:08.785587 fooder-0.0.4/
+-rw-r--r--   0 doman      (501) staff       (20)    35149 2023-04-17 21:36:03.000000 fooder-0.0.4/LICENSE
+-rw-r--r--   0 doman      (501) staff       (20)     2097 2023-07-30 18:48:08.785650 fooder-0.0.4/PKG-INFO
+drwxr-xr-x   0 doman      (501) staff       (20)        0 2023-07-30 18:48:08.783720 fooder-0.0.4/fooder.egg-info/
+-rw-r--r--   0 doman      (501) staff       (20)     2097 2023-07-30 18:48:08.000000 fooder-0.0.4/fooder.egg-info/PKG-INFO
+-rw-r--r--   0 doman      (501) staff       (20)      375 2023-07-30 18:48:08.000000 fooder-0.0.4/fooder.egg-info/SOURCES.txt
+-rw-r--r--   0 doman      (501) staff       (20)        1 2023-07-30 18:48:08.000000 fooder-0.0.4/fooder.egg-info/dependency_links.txt
+-rw-r--r--   0 doman      (501) staff       (20)       48 2023-07-30 18:48:08.000000 fooder-0.0.4/fooder.egg-info/entry_points.txt
+-rw-r--r--   0 doman      (501) staff       (20)       40 2023-07-30 18:48:08.000000 fooder-0.0.4/fooder.egg-info/requires.txt
+-rw-r--r--   0 doman      (501) staff       (20)       11 2023-07-30 18:48:08.000000 fooder-0.0.4/fooder.egg-info/top_level.txt
+drwxr-xr-x   0 doman      (501) staff       (20)        0 2023-07-30 18:48:08.785380 fooder-0.0.4/fooder_cli/
+-rw-r--r--   0 doman      (501) staff       (20)        0 2023-04-17 21:36:03.000000 fooder-0.0.4/fooder_cli/__init__.py
+-rw-r--r--   0 doman      (501) staff       (20)       63 2023-04-17 21:36:03.000000 fooder-0.0.4/fooder_cli/__main__.py
+-rw-r--r--   0 doman      (501) staff       (20)     9813 2023-07-30 18:42:38.000000 fooder-0.0.4/fooder_cli/client.py
+-rw-r--r--   0 doman      (501) staff       (20)     1626 2023-04-18 10:06:34.000000 fooder-0.0.4/fooder_cli/diary.py
+-rw-r--r--   0 doman      (501) staff       (20)      675 2023-04-18 10:04:11.000000 fooder-0.0.4/fooder_cli/entry.py
+-rw-r--r--   0 doman      (501) staff       (20)     3785 2023-04-19 16:39:05.000000 fooder-0.0.4/fooder_cli/main.py
+-rw-r--r--   0 doman      (501) staff       (20)      719 2023-04-18 10:04:56.000000 fooder-0.0.4/fooder_cli/meal.py
+-rw-r--r--   0 doman      (501) staff       (20)     2889 2023-07-30 18:42:19.000000 fooder-0.0.4/fooder_cli/product.py
+-rw-r--r--   0 doman      (501) staff       (20)      100 2023-07-30 18:48:08.785821 fooder-0.0.4/setup.cfg
+-rw-r--r--   0 doman      (501) staff       (20)      973 2023-07-30 18:43:08.000000 fooder-0.0.4/setup.py
```

### Comparing `fooder-0.0.3/LICENSE` & `fooder-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fooder-0.0.3/PKG-INFO` & `fooder-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: fooder
-Version: 0.0.3
+Version: 0.0.4
 Summary: Minimalistic cli diary for tracking calories
 Home-page: https://github.com/ickyicky/fooder-cli-client
 Author: Piotr Domanski
 Author-email: pi.domanski@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -52,9 +50,7 @@
 products database.
 
 [![](https://github.com/ickyicky/fooder-cli-client/blob/main/doc/menu.png?raw=true)](https://github.com/ickyicky/fooder-cli-client)
 
 Whole program is very simple TUI where in each view you can select action from available options, such as switching to diary from
 another day, adding meals, adding entries etc. It's just intuitive and since project is in alpha stage I'm not writting whole
 usage instruction just yet, before the finalized product is complete.
-
-
```

### Comparing `fooder-0.0.3/fooder.egg-info/PKG-INFO` & `fooder-0.0.4/fooder.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: fooder
-Version: 0.0.3
+Version: 0.0.4
 Summary: Minimalistic cli diary for tracking calories
 Home-page: https://github.com/ickyicky/fooder-cli-client
 Author: Piotr Domanski
 Author-email: pi.domanski@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -52,9 +50,7 @@
 products database.
 
 [![](https://github.com/ickyicky/fooder-cli-client/blob/main/doc/menu.png?raw=true)](https://github.com/ickyicky/fooder-cli-client)
 
 Whole program is very simple TUI where in each view you can select action from available options, such as switching to diary from
 another day, adding meals, adding entries etc. It's just intuitive and since project is in alpha stage I'm not writting whole
 usage instruction just yet, before the finalized product is complete.
-
-
```

### Comparing `fooder-0.0.3/fooder_cli/client.py` & `fooder-0.0.4/fooder_cli/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -233,28 +233,35 @@
     @validate_arguments
     def create_product(
         self,
         name: str,
         protein: float,
         carb: float,
         fat: float,
+        fiber: float,
     ) -> Dict:
         """create_product.
 
         :param name:
         :type name: str
         :param protein:
         :type protein: float
         :param carb:
         :type carb: float
         :param fat:
         :type fat: float
         :rtype: Dict
         """
-        data = {"name": name, "protein": protein, "carb": carb, "fat": fat}
+        data = {
+            "name": name,
+            "protein": protein,
+            "carb": carb,
+            "fat": fat,
+            "fiber": fiber,
+        }
         return self.post("/product", data=data)
 
     @validate_arguments
     def get_diary(self, date_: Optional[date] = None) -> Dict:
         """get_diary.
 
         :param date:
```

### Comparing `fooder-0.0.3/fooder_cli/diary.py` & `fooder-0.0.4/fooder_cli/diary.py`

 * *Files identical despite different names*

### Comparing `fooder-0.0.3/fooder_cli/entry.py` & `fooder-0.0.4/fooder_cli/entry.py`

 * *Files identical despite different names*

### Comparing `fooder-0.0.3/fooder_cli/main.py` & `fooder-0.0.4/fooder_cli/main.py`

 * *Files identical despite different names*

### Comparing `fooder-0.0.3/fooder_cli/meal.py` & `fooder-0.0.4/fooder_cli/meal.py`

 * *Files identical despite different names*

### Comparing `fooder-0.0.3/fooder_cli/product.py` & `fooder-0.0.4/fooder_cli/product.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,40 +50,44 @@
 
 def add_product(client):
     console = Console()
     name = Prompt.ask("Enter product name")
     protein = float(Prompt.ask("Enter protein"))
     carb = float(Prompt.ask("Enter carb"))
     fat = float(Prompt.ask("Enter fat"))
+    fiber = float(Prompt.ask("Enter fiber"))
 
-    calories = protein * 4 + carb * 4 + fat * 9
+    calories = protein * 4 + carb * 4 + fat * 9 + fiber * 2
 
     table = Table(title="Product")
     table.add_column("Name", style="cyan", no_wrap=True)
     table.add_column("Protein", justify="right", style="green")
     table.add_column("Carb", justify="right", style="blue")
     table.add_column("Fat", justify="right", style="red")
+    table.add_column("Fiber", justify="right", style="magenta")
     table.add_column("Kcal", justify="right", style="yellow")
 
     table.add_row(
         name,
         str(round(protein, 2)),
         str(round(carb, 2)),
         str(round(fat, 2)),
+        str(round(fiber, 2)),
         str(round(calories, 2)),
     )
 
     console.print(table, justify="left")
 
     proceed = Confirm.ask("Add this product?", default=True)
     if not proceed:
         return
 
     product = client.create_product(
         name=name,
         protein=protein,
         carb=carb,
         fat=fat,
+        fiber=fiber,
     )
 
     console.print(Text("Product added", style="bold green"))
     return product
```

### Comparing `fooder-0.0.3/setup.py` & `fooder-0.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read().splitlines()
 
 
 setup(
     name="fooder",
-    version="0.0.3",
+    version="0.0.4",
     author="Piotr Domanski",
     author_email="pi.domanski@gmail.com",
     description="Minimalistic cli diary for tracking calories",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ickyicky/fooder-cli-client",
     classifiers=[
```

