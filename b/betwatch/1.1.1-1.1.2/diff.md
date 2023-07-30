# Comparing `tmp/betwatch-1.1.1.tar.gz` & `tmp/betwatch-1.1.2.tar.gz`

## Comparing `betwatch-1.1.1.tar` & `betwatch-1.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 betwatch-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 betwatch-1.1.1/Makefile
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 betwatch-1.1.1/.github/dependabot.yml
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 betwatch-1.1.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 betwatch-1.1.1/betwatch/__about__.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 betwatch-1.1.1/betwatch/__init__.py
--rw-r--r--   0        0        0     8765 2020-02-02 00:00:00.000000 betwatch-1.1.1/betwatch/client.py
--rw-r--r--   0        0        0    28031 2020-02-02 00:00:00.000000 betwatch-1.1.1/betwatch/client_async.py
--rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 betwatch-1.1.1/betwatch/queries.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 betwatch-1.1.1/betwatch/types/__init__.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 betwatch-1.1.1/betwatch/types/bookmakers.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 betwatch-1.1.1/betwatch/types/exceptions.py
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 betwatch-1.1.1/betwatch/types/filters.py
--rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 betwatch-1.1.1/betwatch/types/markets.py
--rw-r--r--   0        0        0    12482 2020-02-02 00:00:00.000000 betwatch-1.1.1/betwatch/types/race.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 betwatch-1.1.1/betwatch/types/updates.py
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 betwatch-1.1.1/examples/get_race_prices.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 betwatch-1.1.1/examples/get_race_prices_async.py
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 betwatch-1.1.1/examples/get_races.py
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 betwatch-1.1.1/examples/get_races_async.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 betwatch-1.1.1/examples/subscriptions.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 betwatch-1.1.1/examples/update_rated_prices.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 betwatch-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 betwatch-1.1.1/tests/test_check_last_updated.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 betwatch-1.1.1/tests/test_get_race.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 betwatch-1.1.1/tests/test_get_race_async.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 betwatch-1.1.1/tests/test_get_races.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 betwatch-1.1.1/tests/test_get_races_async.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 betwatch-1.1.1/.gitignore
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 betwatch-1.1.1/LICENSE.txt
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 betwatch-1.1.1/README.md
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 betwatch-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 betwatch-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 betwatch-1.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 betwatch-1.1.2/Makefile
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 betwatch-1.1.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 betwatch-1.1.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 betwatch-1.1.2/betwatch/__about__.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 betwatch-1.1.2/betwatch/__init__.py
+-rw-r--r--   0        0        0     8765 2020-02-02 00:00:00.000000 betwatch-1.1.2/betwatch/client.py
+-rw-r--r--   0        0        0    28031 2020-02-02 00:00:00.000000 betwatch-1.1.2/betwatch/client_async.py
+-rw-r--r--   0        0        0     5038 2020-02-02 00:00:00.000000 betwatch-1.1.2/betwatch/queries.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 betwatch-1.1.2/betwatch/types/__init__.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 betwatch-1.1.2/betwatch/types/bookmakers.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 betwatch-1.1.2/betwatch/types/exceptions.py
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 betwatch-1.1.2/betwatch/types/filters.py
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 betwatch-1.1.2/betwatch/types/markets.py
+-rw-r--r--   0        0        0    12569 2020-02-02 00:00:00.000000 betwatch-1.1.2/betwatch/types/race.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 betwatch-1.1.2/betwatch/types/updates.py
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 betwatch-1.1.2/examples/get_race_prices.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 betwatch-1.1.2/examples/get_race_prices_async.py
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 betwatch-1.1.2/examples/get_races.py
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 betwatch-1.1.2/examples/get_races_async.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 betwatch-1.1.2/examples/subscriptions.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 betwatch-1.1.2/examples/update_rated_prices.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 betwatch-1.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 betwatch-1.1.2/tests/test_check_last_updated.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 betwatch-1.1.2/tests/test_get_race.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 betwatch-1.1.2/tests/test_get_race_async.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 betwatch-1.1.2/tests/test_get_races.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 betwatch-1.1.2/tests/test_get_races_async.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 betwatch-1.1.2/.gitignore
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 betwatch-1.1.2/LICENSE.txt
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 betwatch-1.1.2/README.md
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 betwatch-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 betwatch-1.1.2/PKG-INFO
```

### Comparing `betwatch-1.1.1/.github/workflows/test.yml` & `betwatch-1.1.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.1/betwatch/__init__.py` & `betwatch-1.1.2/betwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.1/betwatch/client.py` & `betwatch-1.1.2/betwatch/client.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.1/betwatch/client_async.py` & `betwatch-1.1.2/betwatch/client_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.1/betwatch/queries.py` & `betwatch-1.1.2/betwatch/queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     )
 
     return (
         " id betfairMapping { win place } meeting { id location track type date } "
         + "classConditions name number status startTime results distance "
         + runners_gql
         + (
-            " links { bookmaker lastSuccessfulPriceUpdate navLink } "
+            " links { bookmaker lastSuccessfulPriceUpdate navLink fixedWin } "
             if projection.links
             else ""
         )
     )
 
 
 SUBSCRIPTION_RACES_UPDATES = gql(
```

### Comparing `betwatch-1.1.1/betwatch/types/bookmakers.py` & `betwatch-1.1.2/betwatch/types/bookmakers.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.1/betwatch/types/filters.py` & `betwatch-1.1.2/betwatch/types/filters.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.1/betwatch/types/markets.py` & `betwatch-1.1.2/betwatch/types/markets.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.1/betwatch/types/race.py` & `betwatch-1.1.2/betwatch/types/race.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,14 +215,15 @@
         return None
 
 
 @dataclass
 class RaceLink:
     _bookmaker: Union[Bookmaker, str] = field(metadata={"name": "bookmaker"})
     nav_link: Optional[str] = field(metadata={"name": "navLink"}, default=None)
+    fixed_win_link: Optional[str] = field(metadata={"name": "fixedWin"}, default=None)
     _last_successful_price_update: Optional[str] = field(
         metadata={"name": "lastSuccessfulPriceUpdate"}, default=None
     )
 
     def __post_init__(self):
         self.last_successful_price_update = (
             dateutil.parser.isoparse(self._last_successful_price_update)
```

### Comparing `betwatch-1.1.1/examples/get_race_prices.py` & `betwatch-1.1.2/examples/get_race_prices.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.1/examples/get_race_prices_async.py` & `betwatch-1.1.2/examples/get_race_prices_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.1/examples/get_races.py` & `betwatch-1.1.2/examples/get_races.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.1/examples/get_races_async.py` & `betwatch-1.1.2/examples/get_races_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.1/examples/subscriptions.py` & `betwatch-1.1.2/examples/subscriptions.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.1/examples/update_rated_prices.py` & `betwatch-1.1.2/examples/update_rated_prices.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.1/tests/test_get_race.py` & `betwatch-1.1.2/tests/test_get_race.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.1/tests/test_get_race_async.py` & `betwatch-1.1.2/tests/test_get_race_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.1/tests/test_get_races.py` & `betwatch-1.1.2/tests/test_get_races.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.1/tests/test_get_races_async.py` & `betwatch-1.1.2/tests/test_get_races_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.1/.gitignore` & `betwatch-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.1/LICENSE.txt` & `betwatch-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.1/README.md` & `betwatch-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.1/pyproject.toml` & `betwatch-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.1/PKG-INFO` & `betwatch-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betwatch
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Python package for interacting with the Betwatch.com API
 Project-URL: Documentation, https://github.com/betwatch/betwatch-sdk-python#readme
 Project-URL: Issues, https://github.com/betwatch/betwatch-sdk-python/issues
 Project-URL: Source, https://github.com/betwatch/betwatch-sdk-python
 Project-URL: Betwatch.com, https://betwatch.com
 Author-email: Jamie Watts <jamie@betwatch.com>
 License-File: LICENSE.txt
```

