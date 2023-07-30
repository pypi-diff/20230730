# Comparing `tmp/betwatch-1.1.0.tar.gz` & `tmp/betwatch-1.1.1.tar.gz`

## Comparing `betwatch-1.1.0.tar` & `betwatch-1.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 betwatch-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 betwatch-1.1.0/Makefile
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 betwatch-1.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 betwatch-1.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 betwatch-1.1.0/betwatch/__about__.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 betwatch-1.1.0/betwatch/__init__.py
--rw-r--r--   0        0        0     8765 2020-02-02 00:00:00.000000 betwatch-1.1.0/betwatch/client.py
--rw-r--r--   0        0        0    28031 2020-02-02 00:00:00.000000 betwatch-1.1.0/betwatch/client_async.py
--rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 betwatch-1.1.0/betwatch/queries.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 betwatch-1.1.0/betwatch/types/__init__.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 betwatch-1.1.0/betwatch/types/bookmakers.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 betwatch-1.1.0/betwatch/types/exceptions.py
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 betwatch-1.1.0/betwatch/types/filters.py
--rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 betwatch-1.1.0/betwatch/types/markets.py
--rw-r--r--   0        0        0    12482 2020-02-02 00:00:00.000000 betwatch-1.1.0/betwatch/types/race.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 betwatch-1.1.0/betwatch/types/updates.py
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 betwatch-1.1.0/examples/get_race_prices.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 betwatch-1.1.0/examples/get_race_prices_async.py
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 betwatch-1.1.0/examples/get_races.py
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 betwatch-1.1.0/examples/get_races_async.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 betwatch-1.1.0/examples/subscriptions.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 betwatch-1.1.0/examples/update_rated_prices.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 betwatch-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 betwatch-1.1.0/tests/test_check_last_updated.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 betwatch-1.1.0/tests/test_get_race.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 betwatch-1.1.0/tests/test_get_race_async.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 betwatch-1.1.0/tests/test_get_races.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 betwatch-1.1.0/tests/test_get_races_async.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 betwatch-1.1.0/.gitignore
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 betwatch-1.1.0/LICENSE.txt
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 betwatch-1.1.0/README.md
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 betwatch-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 betwatch-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 betwatch-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 betwatch-1.1.1/Makefile
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 betwatch-1.1.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 betwatch-1.1.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 betwatch-1.1.1/betwatch/__about__.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 betwatch-1.1.1/betwatch/__init__.py
+-rw-r--r--   0        0        0     8765 2020-02-02 00:00:00.000000 betwatch-1.1.1/betwatch/client.py
+-rw-r--r--   0        0        0    28031 2020-02-02 00:00:00.000000 betwatch-1.1.1/betwatch/client_async.py
+-rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 betwatch-1.1.1/betwatch/queries.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 betwatch-1.1.1/betwatch/types/__init__.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 betwatch-1.1.1/betwatch/types/bookmakers.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 betwatch-1.1.1/betwatch/types/exceptions.py
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 betwatch-1.1.1/betwatch/types/filters.py
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 betwatch-1.1.1/betwatch/types/markets.py
+-rw-r--r--   0        0        0    12482 2020-02-02 00:00:00.000000 betwatch-1.1.1/betwatch/types/race.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 betwatch-1.1.1/betwatch/types/updates.py
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 betwatch-1.1.1/examples/get_race_prices.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 betwatch-1.1.1/examples/get_race_prices_async.py
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 betwatch-1.1.1/examples/get_races.py
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 betwatch-1.1.1/examples/get_races_async.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 betwatch-1.1.1/examples/subscriptions.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 betwatch-1.1.1/examples/update_rated_prices.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 betwatch-1.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 betwatch-1.1.1/tests/test_check_last_updated.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 betwatch-1.1.1/tests/test_get_race.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 betwatch-1.1.1/tests/test_get_race_async.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 betwatch-1.1.1/tests/test_get_races.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 betwatch-1.1.1/tests/test_get_races_async.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 betwatch-1.1.1/.gitignore
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 betwatch-1.1.1/LICENSE.txt
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 betwatch-1.1.1/README.md
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 betwatch-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 betwatch-1.1.1/PKG-INFO
```

### Comparing `betwatch-1.1.0/.github/workflows/test.yml` & `betwatch-1.1.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.0/betwatch/__init__.py` & `betwatch-1.1.1/betwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.0/betwatch/client.py` & `betwatch-1.1.1/betwatch/client.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.0/betwatch/client_async.py` & `betwatch-1.1.1/betwatch/client_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.0/betwatch/queries.py` & `betwatch-1.1.1/betwatch/queries.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.0/betwatch/types/bookmakers.py` & `betwatch-1.1.1/betwatch/types/bookmakers.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.0/betwatch/types/filters.py` & `betwatch-1.1.1/betwatch/types/filters.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.0/betwatch/types/markets.py` & `betwatch-1.1.1/betwatch/types/markets.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.0/betwatch/types/race.py` & `betwatch-1.1.1/betwatch/types/race.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.0/examples/get_race_prices.py` & `betwatch-1.1.1/examples/get_race_prices.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.0/examples/get_race_prices_async.py` & `betwatch-1.1.1/examples/get_race_prices_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.0/examples/get_races.py` & `betwatch-1.1.1/examples/get_races.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.0/examples/get_races_async.py` & `betwatch-1.1.1/examples/get_races_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.0/examples/subscriptions.py` & `betwatch-1.1.1/examples/subscriptions.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.0/examples/update_rated_prices.py` & `betwatch-1.1.1/examples/update_rated_prices.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.0/tests/test_get_race.py` & `betwatch-1.1.1/tests/test_get_race.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.0/tests/test_get_race_async.py` & `betwatch-1.1.1/tests/test_get_race_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.0/tests/test_get_races.py` & `betwatch-1.1.1/tests/test_get_races.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.0/tests/test_get_races_async.py` & `betwatch-1.1.1/tests/test_get_races_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.0/.gitignore` & `betwatch-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.0/LICENSE.txt` & `betwatch-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.0/README.md` & `betwatch-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.0/pyproject.toml` & `betwatch-1.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
     "gql[aiohttp,websockets,requests]==3.5.0b5",
     "typedload==2.24",
-    "aiohttp==3.8.5",
+    "aiohttp>=3.8.3",
     "python-dateutil==2.8.2",
     "urllib3>=1.26,<3",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://github.com/betwatch/betwatch-sdk-python#readme"
```

### Comparing `betwatch-1.1.0/PKG-INFO` & `betwatch-1.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betwatch
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python package for interacting with the Betwatch.com API
 Project-URL: Documentation, https://github.com/betwatch/betwatch-sdk-python#readme
 Project-URL: Issues, https://github.com/betwatch/betwatch-sdk-python/issues
 Project-URL: Source, https://github.com/betwatch/betwatch-sdk-python
 Project-URL: Betwatch.com, https://betwatch.com
 Author-email: Jamie Watts <jamie@betwatch.com>
 License-File: LICENSE.txt
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
-Requires-Dist: aiohttp==3.8.5
+Requires-Dist: aiohttp>=3.8.3
 Requires-Dist: gql[aiohttp,requests,websockets]==3.5.0b5
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: typedload==2.24
 Requires-Dist: urllib3<3,>=1.26
 Description-Content-Type: text/markdown
 
 # Betwatch Python SDK
```

