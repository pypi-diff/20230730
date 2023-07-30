# Comparing `tmp/betwatch-1.0.8.tar.gz` & `tmp/betwatch-1.1.0.tar.gz`

## Comparing `betwatch-1.0.8.tar` & `betwatch-1.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 betwatch-1.0.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 betwatch-1.0.8/Makefile
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 betwatch-1.0.8/.github/dependabot.yml
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 betwatch-1.0.8/.github/workflows/test.yml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 betwatch-1.0.8/betwatch/__about__.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 betwatch-1.0.8/betwatch/__init__.py
--rw-r--r--   0        0        0     8765 2020-02-02 00:00:00.000000 betwatch-1.0.8/betwatch/client.py
--rw-r--r--   0        0        0    27637 2020-02-02 00:00:00.000000 betwatch-1.0.8/betwatch/client_async.py
--rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 betwatch-1.0.8/betwatch/queries.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 betwatch-1.0.8/betwatch/types/__init__.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 betwatch-1.0.8/betwatch/types/bookmakers.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 betwatch-1.0.8/betwatch/types/exceptions.py
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 betwatch-1.0.8/betwatch/types/filters.py
--rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 betwatch-1.0.8/betwatch/types/markets.py
--rw-r--r--   0        0        0    12482 2020-02-02 00:00:00.000000 betwatch-1.0.8/betwatch/types/race.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 betwatch-1.0.8/betwatch/types/updates.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 betwatch-1.0.8/examples/get_race_prices.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 betwatch-1.0.8/examples/get_race_prices_async.py
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 betwatch-1.0.8/examples/get_races.py
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 betwatch-1.0.8/examples/get_races_async.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 betwatch-1.0.8/examples/subscriptions.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 betwatch-1.0.8/examples/update_rated_prices.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 betwatch-1.0.8/tests/__init__.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 betwatch-1.0.8/tests/test_check_last_updated.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 betwatch-1.0.8/tests/test_get_race.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 betwatch-1.0.8/tests/test_get_race_async.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 betwatch-1.0.8/tests/test_get_races.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 betwatch-1.0.8/tests/test_get_races_async.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 betwatch-1.0.8/.gitignore
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 betwatch-1.0.8/LICENSE.txt
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 betwatch-1.0.8/README.md
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 betwatch-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 betwatch-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 betwatch-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 betwatch-1.1.0/Makefile
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 betwatch-1.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 betwatch-1.1.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 betwatch-1.1.0/betwatch/__about__.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 betwatch-1.1.0/betwatch/__init__.py
+-rw-r--r--   0        0        0     8765 2020-02-02 00:00:00.000000 betwatch-1.1.0/betwatch/client.py
+-rw-r--r--   0        0        0    28031 2020-02-02 00:00:00.000000 betwatch-1.1.0/betwatch/client_async.py
+-rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 betwatch-1.1.0/betwatch/queries.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 betwatch-1.1.0/betwatch/types/__init__.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 betwatch-1.1.0/betwatch/types/bookmakers.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 betwatch-1.1.0/betwatch/types/exceptions.py
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 betwatch-1.1.0/betwatch/types/filters.py
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 betwatch-1.1.0/betwatch/types/markets.py
+-rw-r--r--   0        0        0    12482 2020-02-02 00:00:00.000000 betwatch-1.1.0/betwatch/types/race.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 betwatch-1.1.0/betwatch/types/updates.py
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 betwatch-1.1.0/examples/get_race_prices.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 betwatch-1.1.0/examples/get_race_prices_async.py
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 betwatch-1.1.0/examples/get_races.py
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 betwatch-1.1.0/examples/get_races_async.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 betwatch-1.1.0/examples/subscriptions.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 betwatch-1.1.0/examples/update_rated_prices.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 betwatch-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 betwatch-1.1.0/tests/test_check_last_updated.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 betwatch-1.1.0/tests/test_get_race.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 betwatch-1.1.0/tests/test_get_race_async.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 betwatch-1.1.0/tests/test_get_races.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 betwatch-1.1.0/tests/test_get_races_async.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 betwatch-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 betwatch-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 betwatch-1.1.0/README.md
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 betwatch-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 betwatch-1.1.0/PKG-INFO
```

### Comparing `betwatch-1.0.8/.github/workflows/test.yml` & `betwatch-1.1.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.8/betwatch/__init__.py` & `betwatch-1.1.0/betwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.8/betwatch/client.py` & `betwatch-1.1.0/betwatch/client.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.8/betwatch/client_async.py` & `betwatch-1.1.0/betwatch/client_async.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from gql.transport.aiohttp import AIOHTTPTransport
 from gql.transport.aiohttp import log as aiohttp_logger
 from gql.transport.exceptions import TransportError, TransportQueryError
 from gql.transport.websockets import WebsocketsTransport
 from gql.transport.websockets import log as websockets_logger
 from graphql import DocumentNode
 from typedload.exceptions import TypedloadException
+from websockets.exceptions import ConnectionClosedError
 
 from betwatch.__about__ import __version__
 from betwatch.queries import (
     MUTATION_UPDATE_USER_EVENT_DATA,
     QUERY_GET_LAST_SUCCESSFUL_PRICE_UPDATE,
     SUBSCRIPTION_BETFAIR_UPDATES,
     SUBSCRIPTION_RACES_UPDATES,
@@ -522,14 +523,16 @@
             if "does not have access" in e.args[0]:
                 raise NotEntitledError(
                     "API key is not entitled to websocket subscriptions"
                 ) from e
         except asyncio.CancelledError:
             await self.unsubscribe_bookmaker_updates(race_id)
             return
+        except ConnectionClosedError as e:
+            logging.debug(f"Error on bookmaker prices subscription: {e}")
         except Exception as e:
             logging.debug(f"Error subscribing to bookmaker updates: {e}")
 
     async def unsubscribe_betfair_updates(self, race_id: str):
         if race_id not in self._subscriptions_betfair:
             logging.info(
                 f"Not subscribed to {race_id if race_id else 'all races'} betfair updates"
@@ -598,14 +601,16 @@
             if "does not have access" in e.args[0]:
                 raise NotEntitledError(
                     "API key is not entitled to websocket subscriptions"
                 ) from e
         except asyncio.CancelledError:
             await self.unsubscribe_betfair_updates(race_id)
             return
+        except ConnectionClosedError as e:
+            logging.debug(f"Error on betfair subscription: {e}")
 
     async def unsubscribe_race_updates(self, date_from: str, date_to: str):
         if (date_from, date_to) not in self._subscriptions_updates:
             logging.info(f"Not subscribed to races updates for {date_from} - {date_to}")
             return
 
         self._subscriptions_updates[(date_from, date_to)].cancel()
@@ -642,14 +647,16 @@
                     self._subscription_queue.put_nowait(update)
 
         except TransportError as e:
             logging.debug(f"Error subscribing to race updates: {e}")
         except asyncio.CancelledError:
             await self.unsubscribe_race_updates(date_from, date_to)
             return
+        except ConnectionClosedError as e:
+            logging.debug(f"Error on race updates subscription: {e}")
 
     @backoff.on_exception(backoff.expo, Exception, max_time=60, max_tries=5)
     async def _get_race_by_id(
         self,
         race_id: str,
         query: DocumentNode,
     ) -> Union[Race, None]:
```

### Comparing `betwatch-1.0.8/betwatch/queries.py` & `betwatch-1.1.0/betwatch/queries.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.8/betwatch/types/bookmakers.py` & `betwatch-1.1.0/betwatch/types/bookmakers.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.8/betwatch/types/filters.py` & `betwatch-1.1.0/betwatch/types/filters.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.8/betwatch/types/markets.py` & `betwatch-1.1.0/betwatch/types/markets.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.8/betwatch/types/race.py` & `betwatch-1.1.0/betwatch/types/race.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.8/examples/get_race_prices.py` & `betwatch-1.1.0/examples/get_race_prices.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def main():
     api_key = os.getenv("API_KEY")
     if not api_key:
         raise Exception("API_KEY not set in .env file")
 
     # client = betwatch.connect(api_key=api_key)
-    client = BetwatchClient(api_key=api_key, host="api.betwatch.localhost")
+    client = BetwatchClient(api_key=api_key)
 
     # define the projection of the returned data
     # we can filter out for certain bookmakers as well as define whether we want market data or flucs
     projection = RaceProjection(
         markets=True,
         flucs=True,
         bookmakers=[Bookmaker.SPORTSBET, Bookmaker.TAB],
```

### Comparing `betwatch-1.0.8/examples/get_race_prices_async.py` & `betwatch-1.1.0/examples/get_race_prices_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.8/examples/get_races.py` & `betwatch-1.1.0/examples/get_races.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.8/examples/get_races_async.py` & `betwatch-1.1.0/examples/get_races_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.8/examples/subscriptions.py` & `betwatch-1.1.0/examples/subscriptions.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.8/examples/update_rated_prices.py` & `betwatch-1.1.0/examples/update_rated_prices.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.8/tests/test_get_race.py` & `betwatch-1.1.0/tests/test_get_race.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.8/tests/test_get_race_async.py` & `betwatch-1.1.0/tests/test_get_race_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.8/tests/test_get_races.py` & `betwatch-1.1.0/tests/test_get_races.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.8/tests/test_get_races_async.py` & `betwatch-1.1.0/tests/test_get_races_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.8/.gitignore` & `betwatch-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.8/LICENSE.txt` & `betwatch-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.8/README.md` & `betwatch-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.8/pyproject.toml` & `betwatch-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -17,19 +17,19 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-    "gql[aiohttp,websockets,requests]==3.5.0b4",
-    "typedload==2.22",
-    "aiohttp==3.8.3",
+    "gql[aiohttp,websockets,requests]==3.5.0b5",
+    "typedload==2.24",
+    "aiohttp==3.8.5",
     "python-dateutil==2.8.2",
-    "urllib3>=1.26,<2",
+    "urllib3>=1.26,<3",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://github.com/betwatch/betwatch-sdk-python#readme"
 Issues = "https://github.com/betwatch/betwatch-sdk-python/issues"
 Source = "https://github.com/betwatch/betwatch-sdk-python"
```

### Comparing `betwatch-1.0.8/PKG-INFO` & `betwatch-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: betwatch
-Version: 1.0.8
+Version: 1.1.0
 Summary: A Python package for interacting with the Betwatch.com API
 Project-URL: Documentation, https://github.com/betwatch/betwatch-sdk-python#readme
 Project-URL: Issues, https://github.com/betwatch/betwatch-sdk-python/issues
 Project-URL: Source, https://github.com/betwatch/betwatch-sdk-python
 Project-URL: Betwatch.com, https://betwatch.com
 Author-email: Jamie Watts <jamie@betwatch.com>
-License-Expression: MIT
 License-File: LICENSE.txt
 Keywords: api,betting,betwatch,sdk,sports
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
-Requires-Dist: aiohttp==3.8.3
-Requires-Dist: gql[aiohttp,requests,websockets]==3.5.0b4
+Requires-Dist: aiohttp==3.8.5
+Requires-Dist: gql[aiohttp,requests,websockets]==3.5.0b5
 Requires-Dist: python-dateutil==2.8.2
-Requires-Dist: typedload==2.22
-Requires-Dist: urllib3<2,>=1.26
+Requires-Dist: typedload==2.24
+Requires-Dist: urllib3<3,>=1.26
 Description-Content-Type: text/markdown
 
 # Betwatch Python SDK
 
 [![PyPI - Version](https://img.shields.io/pypi/v/betwatch.svg)](https://pypi.org/project/betwatch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/betwatch.svg)](https://pypi.org/project/betwatch)
```

