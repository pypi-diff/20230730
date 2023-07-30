# Comparing `tmp/twscrape-0.6.0.tar.gz` & `tmp/twscrape-0.7.0.tar.gz`

## Comparing `twscrape-0.6.0.tar` & `twscrape-0.7.0.tar`

### file list

```diff
@@ -1,48 +1,51 @@
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 twscrape-0.6.0/.gitattributes
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 twscrape-0.6.0/Dockerfile-test
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 twscrape-0.6.0/Makefile
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 twscrape-0.6.0/_get_gql_ops.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 twscrape-0.6.0/.github/CODEOWNERS
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 twscrape-0.6.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 twscrape-0.6.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 twscrape-0.6.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 twscrape-0.6.0/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 twscrape-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 twscrape-0.6.0/tests/conftest.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 twscrape-0.6.0/tests/test_api.py
--rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 twscrape-0.6.0/tests/test_parser.py
--rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 twscrape-0.6.0/tests/test_pool.py
--rw-r--r--   0        0        0     4839 2020-02-02 00:00:00.000000 twscrape-0.6.0/tests/test_queue_client.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 twscrape-0.6.0/tests/test_utils.py
--rw-r--r--   0        0        0    47075 2020-02-02 00:00:00.000000 twscrape-0.6.0/tests/mocked-data/_issue_28.2.json
--rw-r--r--   0        0        0    43215 2020-02-02 00:00:00.000000 twscrape-0.6.0/tests/mocked-data/_issue_28.json
--rw-r--r--   0        0        0    65611 2020-02-02 00:00:00.000000 twscrape-0.6.0/tests/mocked-data/favoriters_raw.json
--rw-r--r--   0        0        0   249678 2020-02-02 00:00:00.000000 twscrape-0.6.0/tests/mocked-data/followers_raw.json
--rw-r--r--   0        0        0   265585 2020-02-02 00:00:00.000000 twscrape-0.6.0/tests/mocked-data/following_raw.json
--rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 twscrape-0.6.0/tests/mocked-data/manual_tweet_with_video_1.json
--rw-r--r--   0        0        0    84696 2020-02-02 00:00:00.000000 twscrape-0.6.0/tests/mocked-data/manual_tweet_with_video_2.json
--rw-r--r--   0        0        0    71891 2020-02-02 00:00:00.000000 twscrape-0.6.0/tests/mocked-data/retweeters_raw.json
--rw-r--r--   0        0        0   162255 2020-02-02 00:00:00.000000 twscrape-0.6.0/tests/mocked-data/search_raw.json
--rw-r--r--   0        0        0   124262 2020-02-02 00:00:00.000000 twscrape-0.6.0/tests/mocked-data/tweet_details_raw.json
--rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 twscrape-0.6.0/tests/mocked-data/user_by_id_raw.json
--rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 twscrape-0.6.0/tests/mocked-data/user_by_login_raw.json
--rw-r--r--   0        0        0   291032 2020-02-02 00:00:00.000000 twscrape-0.6.0/tests/mocked-data/user_tweets_and_replies_raw.json
--rw-r--r--   0        0        0   244343 2020-02-02 00:00:00.000000 twscrape-0.6.0/tests/mocked-data/user_tweets_raw.json
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 twscrape-0.6.0/twscrape/__init__.py
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 twscrape-0.6.0/twscrape/account.py
--rw-r--r--   0        0        0    12082 2020-02-02 00:00:00.000000 twscrape-0.6.0/twscrape/accounts_pool.py
--rw-r--r--   0        0        0    10052 2020-02-02 00:00:00.000000 twscrape-0.6.0/twscrape/api.py
--rw-r--r--   0        0        0     6501 2020-02-02 00:00:00.000000 twscrape-0.6.0/twscrape/cli.py
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 twscrape-0.6.0/twscrape/constants.py
--rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 twscrape-0.6.0/twscrape/db.py
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 twscrape-0.6.0/twscrape/imap.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 twscrape-0.6.0/twscrape/logger.py
--rw-r--r--   0        0        0     6950 2020-02-02 00:00:00.000000 twscrape-0.6.0/twscrape/login.py
--rw-r--r--   0        0        0    11686 2020-02-02 00:00:00.000000 twscrape-0.6.0/twscrape/models.py
--rw-r--r--   0        0        0     6182 2020-02-02 00:00:00.000000 twscrape-0.6.0/twscrape/queue_client.py
--rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 twscrape-0.6.0/twscrape/utils.py
--rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 twscrape-0.6.0/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 twscrape-0.6.0/LICENSE
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 twscrape-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     8473 2020-02-02 00:00:00.000000 twscrape-0.6.0/readme.md
--rw-r--r--   0        0        0     9495 2020-02-02 00:00:00.000000 twscrape-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 twscrape-0.7.0/.gitattributes
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 twscrape-0.7.0/Dockerfile-test
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 twscrape-0.7.0/Makefile
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 twscrape-0.7.0/_get_gql_ops.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 twscrape-0.7.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 twscrape-0.7.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 twscrape-0.7.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 twscrape-0.7.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 twscrape-0.7.0/.vscode/settings.json
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 twscrape-0.7.0/examples/parallel_search.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 twscrape-0.7.0/examples/parallel_search_with_limit.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 twscrape-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 twscrape-0.7.0/tests/conftest.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 twscrape-0.7.0/tests/test_api.py
+-rw-r--r--   0        0        0     7999 2020-02-02 00:00:00.000000 twscrape-0.7.0/tests/test_parser.py
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 twscrape-0.7.0/tests/test_pool.py
+-rw-r--r--   0        0        0     4839 2020-02-02 00:00:00.000000 twscrape-0.7.0/tests/test_queue_client.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 twscrape-0.7.0/tests/test_utils.py
+-rw-r--r--   0        0        0    43215 2020-02-02 00:00:00.000000 twscrape-0.7.0/tests/mocked-data/_issue_28_1.json
+-rw-r--r--   0        0        0    47075 2020-02-02 00:00:00.000000 twscrape-0.7.0/tests/mocked-data/_issue_28_2.json
+-rw-r--r--   0        0        0    22052 2020-02-02 00:00:00.000000 twscrape-0.7.0/tests/mocked-data/_issue_42.json
+-rw-r--r--   0        0        0    65611 2020-02-02 00:00:00.000000 twscrape-0.7.0/tests/mocked-data/favoriters_raw.json
+-rw-r--r--   0        0        0   249678 2020-02-02 00:00:00.000000 twscrape-0.7.0/tests/mocked-data/followers_raw.json
+-rw-r--r--   0        0        0   265585 2020-02-02 00:00:00.000000 twscrape-0.7.0/tests/mocked-data/following_raw.json
+-rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 twscrape-0.7.0/tests/mocked-data/manual_tweet_with_video_1.json
+-rw-r--r--   0        0        0    84696 2020-02-02 00:00:00.000000 twscrape-0.7.0/tests/mocked-data/manual_tweet_with_video_2.json
+-rw-r--r--   0        0        0    71891 2020-02-02 00:00:00.000000 twscrape-0.7.0/tests/mocked-data/retweeters_raw.json
+-rw-r--r--   0        0        0   162255 2020-02-02 00:00:00.000000 twscrape-0.7.0/tests/mocked-data/search_raw.json
+-rw-r--r--   0        0        0   124262 2020-02-02 00:00:00.000000 twscrape-0.7.0/tests/mocked-data/tweet_details_raw.json
+-rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 twscrape-0.7.0/tests/mocked-data/user_by_id_raw.json
+-rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 twscrape-0.7.0/tests/mocked-data/user_by_login_raw.json
+-rw-r--r--   0        0        0   291032 2020-02-02 00:00:00.000000 twscrape-0.7.0/tests/mocked-data/user_tweets_and_replies_raw.json
+-rw-r--r--   0        0        0   244343 2020-02-02 00:00:00.000000 twscrape-0.7.0/tests/mocked-data/user_tweets_raw.json
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 twscrape-0.7.0/twscrape/__init__.py
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 twscrape-0.7.0/twscrape/account.py
+-rw-r--r--   0        0        0    12475 2020-02-02 00:00:00.000000 twscrape-0.7.0/twscrape/accounts_pool.py
+-rw-r--r--   0        0        0     9832 2020-02-02 00:00:00.000000 twscrape-0.7.0/twscrape/api.py
+-rw-r--r--   0        0        0     6800 2020-02-02 00:00:00.000000 twscrape-0.7.0/twscrape/cli.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 twscrape-0.7.0/twscrape/constants.py
+-rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 twscrape-0.7.0/twscrape/db.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 twscrape-0.7.0/twscrape/imap.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 twscrape-0.7.0/twscrape/logger.py
+-rw-r--r--   0        0        0     7027 2020-02-02 00:00:00.000000 twscrape-0.7.0/twscrape/login.py
+-rw-r--r--   0        0        0    13828 2020-02-02 00:00:00.000000 twscrape-0.7.0/twscrape/models.py
+-rw-r--r--   0        0        0     6317 2020-02-02 00:00:00.000000 twscrape-0.7.0/twscrape/queue_client.py
+-rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 twscrape-0.7.0/twscrape/utils.py
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 twscrape-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 twscrape-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 twscrape-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     8473 2020-02-02 00:00:00.000000 twscrape-0.7.0/readme.md
+-rw-r--r--   0        0        0     9495 2020-02-02 00:00:00.000000 twscrape-0.7.0/PKG-INFO
```

### Comparing `twscrape-0.6.0/Dockerfile-test` & `twscrape-0.7.0/Dockerfile-test`

 * *Files identical despite different names*

### Comparing `twscrape-0.6.0/Makefile` & `twscrape-0.7.0/Makefile`

 * *Files identical despite different names*

### Comparing `twscrape-0.6.0/_get_gql_ops.py` & `twscrape-0.7.0/_get_gql_ops.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.6.0/.github/workflows/publish.yml` & `twscrape-0.7.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `twscrape-0.6.0/tests/conftest.py` & `twscrape-0.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.6.0/tests/test_api.py` & `twscrape-0.7.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.6.0/tests/test_parser.py` & `twscrape-0.7.0/tests/test_parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-import asyncio
 import json
 import os
 
-from twscrape import API, AccountsPool, gather
+from twscrape import API, gather
 from twscrape.logger import set_log_level
-from twscrape.models import Tweet, User
+from twscrape.models import Tweet, User, parse_tweet
 
 BASE_DIR = os.path.dirname(__file__)
 DATA_DIR = os.path.join(BASE_DIR, "mocked-data")
 os.makedirs(DATA_DIR, exist_ok=True)
 
 set_log_level("DEBUG")
 
@@ -96,14 +95,17 @@
                 assert x.thumbnailUrl is not None
                 assert x.duration is not None
                 for v in x.variants:
                     assert v.url is not None
                     assert v.bitrate is not None
                     assert v.contentType is not None
 
+    if doc.retweetedTweet is not None:
+        assert doc.rawContent.endswith(doc.retweetedTweet.rawContent), "content should be full"
+
     check_user(doc.user)
 
 
 def check_user(doc: User):
     assert doc.id is not None
     assert doc.id_str is not None
     assert isinstance(doc.id, int)
@@ -174,19 +176,19 @@
 
 
 async def test_tweet_details():
     api = API()
     mock_rep(api, "tweet_details_raw")
 
     doc = await api.tweet_details(1649191520250245121)
-    assert doc is not None
+    assert doc is not None, "tweet should not be None"
     check_tweet(doc)
 
     assert doc.id == 1649191520250245121
-    assert doc.user is not None
+    assert doc.user is not None, "tweet.user should not be None"
 
 
 async def test_followers():
     api = API()
     mock_gen(api, "followers_raw")
 
     users = await gather(api.followers(2244994945))
@@ -265,85 +267,46 @@
         assert doc is not None
         check_tweet(doc)
 
 
 async def test_issue_28():
     api = API()
 
-    mock_rep(api, "tweet_details_raw", "_issue_28")
+    mock_rep(api, "tweet_details_raw", "_issue_28_1")
     doc = await api.tweet_details(1658409412799737856)
     assert doc is not None
     check_tweet(doc)
 
     assert doc.id == 1658409412799737856
     assert doc.user is not None
 
     assert doc.retweetedTweet is not None
     assert doc.retweetedTweet.viewCount is not None
     assert doc.viewCount is not None  # views should come from retweetedTweet
     assert doc.viewCount == doc.retweetedTweet.viewCount
     check_tweet(doc.retweetedTweet)
 
-    mock_rep(api, "tweet_details_raw", "_issue_28.2")
+    mock_rep(api, "tweet_details_raw", "_issue_28_2")
     doc = await api.tweet_details(1658421690001502208)
     assert doc is not None
     check_tweet(doc)
     assert doc.id == 1658421690001502208
     assert doc.viewCount is not None
 
     assert doc.quotedTweet is not None
     assert doc.quotedTweet.id != doc.id
     check_tweet(doc.quotedTweet)
     assert doc.quotedTweet.viewCount is not None
 
 
-async def main():
-    # prepare mock files from real twitter replies
-    # you need to have some account to perform this
-    FRESH = False
-
-    pool = AccountsPool()
-    api = API(pool)
-
-    jobs = [
-        (Files.search_raw, lambda: api.search_raw("elon musk lang:en", limit=20)),
-        (Files.user_by_id_raw, lambda: api.user_by_id_raw(2244994945)),
-        (Files.user_by_login_raw, lambda: api.user_by_login_raw("twitterdev")),
-        (Files.tweet_details_raw, lambda: api.tweet_details_raw(1649191520250245121)),
-        (Files.followers_raw, lambda: api.followers_raw(2244994945)),
-        (Files.following_raw, lambda: api.following_raw(2244994945)),
-        (Files.retweeters_raw, lambda: api.retweeters_raw(1649191520250245121)),
-        (Files.favoriters_raw, lambda: api.favoriters_raw(1649191520250245121)),
-        (Files.user_tweets_raw, lambda: api.user_tweets_raw(2244994945)),
-        (Files.user_tweets_and_replies_raw, lambda: api.user_tweets_and_replies_raw(2244994945)),
-    ]
-
-    for filename, fn in jobs:
-        filename = os.path.join(DATA_DIR, f"{filename}")
-        print("-" * 20)
-        if os.path.exists(filename) and FRESH is False:
-            print(f"File {filename} already exists")
-            continue
-
-        print(f"Getting data for {filename}")
-
-        rep = fn()
-        is_coroutine = getattr(rep, "__aiter__", None) is None
-
-        data = None
-        if is_coroutine:
-            data = await rep
-        else:
-            async for x in rep:
-                data = x
-                break
-
-        if data is None:
-            print(f"Failed to get data for {filename}")
-            continue
-
-        with open(filename, "w") as fp:
-            fp.write(data.text)
+async def test_issue_42():
+    file = os.path.join(os.path.dirname(__file__), "mocked-data/_issue_42.json")
+    with open(file) as f:
+        data = json.load(f)
 
+    doc = parse_tweet(data, 1665951747842641921)
+    assert doc is not None
+    assert doc.retweetedTweet is not None
+    assert doc.rawContent is not None
+    assert doc.retweetedTweet.rawContent is not None
 
-if __name__ == "__main__":
-    asyncio.run(main())
+    assert doc.rawContent.endswith(doc.retweetedTweet.rawContent)
```

### Comparing `twscrape-0.6.0/tests/test_pool.py` & `twscrape-0.7.0/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.6.0/tests/test_queue_client.py` & `twscrape-0.7.0/tests/test_queue_client.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.6.0/tests/test_utils.py` & `twscrape-0.7.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.6.0/tests/mocked-data/_issue_28.2.json` & `twscrape-0.7.0/tests/mocked-data/_issue_28_2.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.6.0/tests/mocked-data/_issue_28.json` & `twscrape-0.7.0/tests/mocked-data/_issue_28_1.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.6.0/tests/mocked-data/favoriters_raw.json` & `twscrape-0.7.0/tests/mocked-data/favoriters_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.6.0/tests/mocked-data/followers_raw.json` & `twscrape-0.7.0/tests/mocked-data/followers_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.6.0/tests/mocked-data/following_raw.json` & `twscrape-0.7.0/tests/mocked-data/following_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.6.0/tests/mocked-data/manual_tweet_with_video_1.json` & `twscrape-0.7.0/tests/mocked-data/manual_tweet_with_video_1.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.6.0/tests/mocked-data/manual_tweet_with_video_2.json` & `twscrape-0.7.0/tests/mocked-data/manual_tweet_with_video_2.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.6.0/tests/mocked-data/retweeters_raw.json` & `twscrape-0.7.0/tests/mocked-data/retweeters_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.6.0/tests/mocked-data/search_raw.json` & `twscrape-0.7.0/tests/mocked-data/search_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.6.0/tests/mocked-data/tweet_details_raw.json` & `twscrape-0.7.0/tests/mocked-data/tweet_details_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.6.0/tests/mocked-data/user_by_id_raw.json` & `twscrape-0.7.0/tests/mocked-data/user_by_id_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.6.0/tests/mocked-data/user_by_login_raw.json` & `twscrape-0.7.0/tests/mocked-data/user_by_login_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.6.0/tests/mocked-data/user_tweets_and_replies_raw.json` & `twscrape-0.7.0/tests/mocked-data/user_tweets_and_replies_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.6.0/tests/mocked-data/user_tweets_raw.json` & `twscrape-0.7.0/tests/mocked-data/user_tweets_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.6.0/twscrape/account.py` & `twscrape-0.7.0/twscrape/account.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.6.0/twscrape/accounts_pool.py` & `twscrape-0.7.0/twscrape/accounts_pool.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,14 +90,15 @@
             proxy=proxy,
         )
 
         if "ct0" in account.cookies:
             account.active = True
 
         await self.save(account)
+        logger.info(f"Account {username} added successfully (active={account.active})")
 
     async def delete_accounts(self, usernames: str | list[str]):
         usernames = usernames if isinstance(usernames, list) else [usernames]
         usernames = list(set(usernames))
         if not usernames:
             logger.warning("No usernames provided")
             return
@@ -127,40 +128,40 @@
 
         qs = f"""
         INSERT INTO accounts ({",".join(cols)}) VALUES ({",".join([f":{x}" for x in cols])})
         ON CONFLICT(username) DO UPDATE SET {",".join([f"{x}=excluded.{x}" for x in cols])}
         """
         await execute(self._db_file, qs, data)
 
-    async def login(self, account: Account):
+    async def login(self, account: Account, email_first: bool = False):
         try:
-            await login(account)
+            await login(account, email_first=email_first)
             logger.info(f"Logged in to {account.username} successfully")
             return True
         except Exception as e:
             logger.error(f"Error logging in to {account.username}: {e}")
             return False
         finally:
             await self.save(account)
 
-    async def login_all(self):
+    async def login_all(self, email_first=False):
         qs = "SELECT * FROM accounts WHERE active = false AND error_msg IS NULL"
         rs = await fetchall(self._db_file, qs)
 
         accounts = [Account.from_rs(rs) for rs in rs]
         # await asyncio.gather(*[login(x) for x in self.accounts])
 
         counter = {"total": len(accounts), "success": 0, "failed": 0}
         for i, x in enumerate(accounts, start=1):
             logger.info(f"[{i}/{len(accounts)}] Logging in {x.username} - {x.email}")
-            status = await self.login(x)
+            status = await self.login(x, email_first=email_first)
             counter["success" if status else "failed"] += 1
         return counter
 
-    async def relogin(self, usernames: str | list[str]):
+    async def relogin(self, usernames: str | list[str], email_first=False):
         usernames = usernames if isinstance(usernames, list) else [usernames]
         usernames = list(set(usernames))
         if not usernames:
             logger.warning("No usernames provided")
             return
 
         qs = f"""
@@ -172,20 +173,20 @@
             headers = json_object(),
             cookies = json_object(),
             user_agent = "{UserAgent().safari}"
         WHERE username IN ({','.join([f'"{x}"' for x in usernames])})
         """
 
         await execute(self._db_file, qs)
-        await self.login_all()
+        await self.login_all(email_first=email_first)
 
-    async def relogin_failed(self):
+    async def relogin_failed(self, email_first=False):
         qs = "SELECT username FROM accounts WHERE active = false AND error_msg IS NOT NULL"
         rs = await fetchall(self._db_file, qs)
-        await self.relogin([x["username"] for x in rs])
+        await self.relogin([x["username"] for x in rs], email_first=email_first)
 
     async def reset_locks(self):
         qs = "UPDATE accounts SET locks = json_object()"
         await execute(self._db_file, qs)
 
     async def set_active(self, username: str, active: bool):
         qs = "UPDATE accounts SET active = :active WHERE username = :username"
@@ -245,25 +246,28 @@
 
             qs = f"SELECT * FROM accounts WHERE _tx = '{tx}'"
             rs = await fetchone(self._db_file, qs)
 
         return Account.from_rs(rs) if rs else None
 
     async def get_for_queue_or_wait(self, queue: str) -> Account:
-        msg_show = False
+        msg_shown = False
         while True:
             account = await self.get_for_queue(queue)
             if not account:
-                if not msg_show:
+                if not msg_shown:
                     nat = await self.next_available_at(queue)
                     msg = f'No account available for queue "{queue}". Next available at {nat}'
                     logger.info(msg)
-                    msg_show = True
+                    msg_shown = True
                 await asyncio.sleep(5)
                 continue
+            else:
+                if msg_shown:
+                    logger.info(f"Account available for queue {queue}")
 
             return account
 
     async def next_available_at(self, queue: str):
         qs = f"""
         SELECT json_extract(locks, '$."{queue}"') as lock_until
         FROM accounts
```

### Comparing `twscrape-0.6.0/twscrape/api.py` & `twscrape-0.7.0/twscrape/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # ruff: noqa: F405
 from httpx import Response
 
 from .accounts_pool import AccountsPool
 from .constants import *  # noqa: F403
 from .logger import set_log_level
-from .models import Tweet, User, get_tweets, get_users
+from .models import parse_tweet, parse_tweets, parse_user, parse_users
 from .queue_client import QueueClient
-from .utils import encode_params, find_obj, get_by_path, to_old_obj, to_old_rep
+from .utils import encode_params, find_obj, get_by_path
 
 SEARCH_FEATURES = {
     "tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled": True,
 }
 
 
 class API:
@@ -91,15 +91,15 @@
             **(kv or {}),
         }
         async for x in self._gql_items(op, kv, ft=SEARCH_FEATURES, limit=limit):
             yield x
 
     async def search(self, q: str, limit=-1, kv=None):
         async for rep in self.search_raw(q, limit=limit, kv=kv):
-            for x in get_tweets(rep.json(), limit):
+            for x in parse_tweets(rep.json(), limit):
                 yield x
 
     # user_by_id
 
     async def user_by_id_raw(self, uid: int, kv=None):
         op = OP_UserByRestId
         kv = {"userId": str(uid), "withSafetyModeUserFields": True, **(kv or {})}
@@ -108,16 +108,15 @@
             "highlights_tweets_tab_ui_enabled": True,
             "creator_subscriptions_tweet_preview_api_enabled": True,
         }
         return await self._gql_item(op, kv, ft)
 
     async def user_by_id(self, uid: int, kv=None):
         rep = await self.user_by_id_raw(uid, kv=kv)
-        res = rep.json()
-        return User.parse(to_old_obj(res["data"]["user"]["result"]))
+        return parse_user(rep)
 
     # user_by_login
 
     async def user_by_login_raw(self, login: str, kv=None):
         op = OP_UserByScreenName
         kv = {"screen_name": login, "withSafetyModeUserFields": True, **(kv or {})}
         ft = {
@@ -126,16 +125,15 @@
             "creator_subscriptions_tweet_preview_api_enabled": True,
             "subscriptions_verification_info_verified_since_enabled": True,
         }
         return await self._gql_item(op, kv, ft)
 
     async def user_by_login(self, login: str, kv=None):
         rep = await self.user_by_login_raw(login, kv=kv)
-        res = rep.json()
-        return User.parse(to_old_obj(res["data"]["user"]["result"]))
+        return parse_user(rep)
 
     # tweet_details
 
     async def tweet_details_raw(self, twid: int, kv=None):
         op = OP_TweetDetail
         kv = {
             "focalTweetId": str(twid),
@@ -159,68 +157,66 @@
             "longform_notetweets_richtext_consumption_enabled": True,
             **SEARCH_FEATURES,
         }
         return await self._gql_item(op, kv, ft)
 
     async def tweet_details(self, twid: int, kv=None):
         rep = await self.tweet_details_raw(twid, kv=kv)
-        obj = to_old_rep(rep.json())
-        doc = obj["tweets"].get(str(twid), None)
-        return Tweet.parse(doc, obj) if doc else None
+        return parse_tweet(rep, twid)
 
     # followers
 
     async def followers_raw(self, uid: int, limit=-1, kv=None):
         op = OP_Followers
         kv = {"userId": str(uid), "count": 20, "includePromotedContent": False, **(kv or {})}
         async for x in self._gql_items(op, kv, limit=limit):
             yield x
 
     async def followers(self, uid: int, limit=-1, kv=None):
         async for rep in self.followers_raw(uid, limit=limit, kv=kv):
-            for x in get_users(rep.json(), limit):
+            for x in parse_users(rep.json(), limit):
                 yield x
 
     # following
 
     async def following_raw(self, uid: int, limit=-1, kv=None):
         op = OP_Following
         kv = {"userId": str(uid), "count": 20, "includePromotedContent": False, **(kv or {})}
         async for x in self._gql_items(op, kv, limit=limit):
             yield x
 
     async def following(self, uid: int, limit=-1, kv=None):
         async for rep in self.following_raw(uid, limit=limit, kv=kv):
-            for x in get_users(rep.json(), limit):
+            for x in parse_users(rep.json(), limit):
                 yield x
 
     # retweeters
 
     async def retweeters_raw(self, twid: int, limit=-1, kv=None):
         op = OP_Retweeters
         kv = {"tweetId": str(twid), "count": 20, "includePromotedContent": True, **(kv or {})}
         async for x in self._gql_items(op, kv, limit=limit):
             yield x
 
     async def retweeters(self, twid: int, limit=-1, kv=None):
         async for rep in self.retweeters_raw(twid, limit=limit, kv=kv):
-            for x in get_users(rep.json(), limit):
+            for x in parse_users(rep.json(), limit):
                 yield x
 
     # favoriters
 
     async def favoriters_raw(self, twid: int, limit=-1, kv=None):
         op = OP_Favoriters
         kv = {"tweetId": str(twid), "count": 20, "includePromotedContent": True, **(kv or {})}
         async for x in self._gql_items(op, kv, limit=limit):
             yield x
 
     async def favoriters(self, twid: int, limit=-1, kv=None):
         async for rep in self.favoriters_raw(twid, limit=limit, kv=kv):
-            for x in get_users(rep.json(), limit):
+            for x in parse_users(rep.json(), limit):
                 yield x
 
     # user_tweets
 
     async def user_tweets_raw(self, uid: int, limit=-1, kv=None):
         op = OP_UserTweets
         kv = {
@@ -233,15 +229,15 @@
             **(kv or {}),
         }
         async for x in self._gql_items(op, kv, limit=limit):
             yield x
 
     async def user_tweets(self, uid: int, limit=-1, kv=None):
         async for rep in self.user_tweets_raw(uid, limit=limit, kv=kv):
-            for x in get_tweets(rep.json(), limit):
+            for x in parse_tweets(rep.json(), limit):
                 yield x
 
     # user_tweets_and_replies
 
     async def user_tweets_and_replies_raw(self, uid: int, limit=-1, kv=None):
         op = OP_UserTweetsAndReplies
         kv = {
@@ -254,15 +250,15 @@
             **(kv or {}),
         }
         async for x in self._gql_items(op, kv, limit=limit):
             yield x
 
     async def user_tweets_and_replies(self, uid: int, limit=-1, kv=None):
         async for rep in self.user_tweets_and_replies_raw(uid, limit=limit, kv=kv):
-            for x in get_tweets(rep.json(), limit):
+            for x in parse_tweets(rep.json(), limit):
                 yield x
 
     # list timeline
 
     async def list_timeline_raw(self, list_id: int, limit=-1, kv=None):
         op = OP_ListLatestTweetsTimeline
         kv = {
@@ -271,9 +267,9 @@
             **(kv or {}),
         }
         async for x in self._gql_items(op, kv, ft=SEARCH_FEATURES, limit=limit):
             yield x
 
     async def list_timeline(self, list_id: int, limit=-1, kv=None):
         async for rep in self.list_timeline_raw(list_id, limit=limit, kv=kv):
-            for x in get_tweets(rep, limit):
+            for x in parse_tweets(rep, limit):
                 yield x
```

### Comparing `twscrape-0.6.0/twscrape/cli.py` & `twscrape-0.7.0/twscrape/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,23 +76,24 @@
         return
 
     if args.command == "del_accounts":
         await pool.delete_accounts(args.usernames)
         return
 
     if args.command == "login_accounts":
-        print(await pool.login_all())
+        stats = await pool.login_all(email_first=args.email_first)
+        print(stats)
         return
 
     if args.command == "relogin_failed":
-        await pool.relogin_failed()
+        await pool.relogin_failed(email_first=args.email_first)
         return
 
     if args.command == "relogin":
-        await pool.relogin(args.usernames)
+        await pool.relogin(args.usernames, email_first=args.email_first)
         return
 
     if args.command == "reset_locks":
         await pool.reset_locks()
         return
 
     if args.command == "delete_inactive":
@@ -160,20 +161,23 @@
     add_accounts = subparsers.add_parser("add_accounts", help="Add accounts")
     add_accounts.add_argument("file_path", help="File with accounts")
     add_accounts.add_argument("line_format", help="args of Pool.add_account splited by same delim")
 
     del_accounts = subparsers.add_parser("del_accounts", help="Delete accounts")
     del_accounts.add_argument("usernames", nargs="+", default=[], help="Usernames to delete")
 
-    subparsers.add_parser("login_accounts", help="Login accounts")
-
+    login_cmd = subparsers.add_parser("login_accounts", help="Login accounts")
     relogin = subparsers.add_parser("relogin", help="Re-login selected accounts")
     relogin.add_argument("usernames", nargs="+", default=[], help="Usernames to re-login")
+    re_failed = subparsers.add_parser("relogin_failed", help="Retry login for failed accounts")
+
+    check_email = [login_cmd, relogin, re_failed]
+    for cmd in check_email:
+        cmd.add_argument("--email-first", action="store_true", help="Check email first")
 
-    subparsers.add_parser("relogin_failed", help="Retry login for failed accounts")
     subparsers.add_parser("reset_locks", help="Reset all locks")
     subparsers.add_parser("delete_inactive", help="Delete inactive accounts")
 
     c_lim("search", "Search for tweets", "query", "Search query")
     c_one("tweet_details", "Get tweet details", "tweet_id", "Tweet ID", int)
     c_lim("retweeters", "Get retweeters of a tweet", "tweet_id", "Tweet ID", int)
     c_lim("favoriters", "Get favoriters of a tweet", "tweet_id", "Tweet ID", int)
```

### Comparing `twscrape-0.6.0/twscrape/constants.py` & `twscrape-0.7.0/twscrape/constants.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.6.0/twscrape/db.py` & `twscrape-0.7.0/twscrape/db.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
     migrations = {
         1: v1,
         2: v2,
         3: v3,
     }
 
-    logger.debug(f"Current migration v{uv} (latest v{len(migrations)})")
+    # logger.debug(f"Current migration v{uv} (latest v{len(migrations)})")
     for i in range(uv + 1, len(migrations) + 1):
         logger.info(f"Running migration to v{i}")
         try:
             await migrations[i]()
         except sqlite3.OperationalError as e:
             if "duplicate column name" not in str(e):
                 raise e
```

### Comparing `twscrape-0.6.0/twscrape/imap.py` & `twscrape-0.7.0/twscrape/imap.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,22 +29,22 @@
 }
 
 
 def add_imap_mapping(email_domain: str, imap_domain: str):
     IMAP_MAPPING[email_domain] = imap_domain
 
 
-def get_imap_domain(email: str) -> str:
+def _get_imap_domain(email: str) -> str:
     email_domain = email.split("@")[1]
     if email_domain in IMAP_MAPPING:
         return IMAP_MAPPING[email_domain]
     return f"imap.{email_domain}"
 
 
-def search_email_code(imap: imaplib.IMAP4_SSL, count: int, min_t: datetime | None) -> str | None:
+def _wait_email_code(imap: imaplib.IMAP4_SSL, count: int, min_t: datetime | None) -> str | None:
     for i in range(count, 0, -1):
         _, rep = imap.fetch(str(i), "(RFC822)")
         for x in rep:
             if isinstance(x, tuple):
                 msg = emaillib.message_from_bytes(x[1])
 
                 msg_time = datetime.strptime(msg.get("Date", ""), "%a, %d %b %Y %H:%M:%S %z")
@@ -67,15 +67,15 @@
 ) -> str:
     try:
         start_time, was_count = time.time(), 0
         while True:
             _, rep = imap.select("INBOX")
             now_count = int(rep[0].decode("utf-8")) if len(rep) > 0 and rep[0] is not None else 0
             if now_count > was_count:
-                code = search_email_code(imap, now_count, min_t)
+                code = _wait_email_code(imap, now_count, min_t)
                 if code is not None:
                     return code
 
             logger.info(f"Waiting for confirmation code for {email}, msg_count: {now_count}")
             if MAX_WAIT_SEC < time.time() - start_time:
                 logger.info(f"Timeout waiting for confirmation code for {email}")
                 raise EmailCodeTimeoutError()
@@ -83,16 +83,16 @@
     except Exception as e:
         imap.select("INBOX")
         imap.close()
         logger.error(f"Error getting confirmation code for {email}: {e}")
         raise e
 
 
-async def imap_try_login(email: str, password: str):
-    domain = get_imap_domain(email)
+async def imap_login(email: str, password: str):
+    domain = _get_imap_domain(email)
     imap = imaplib.IMAP4_SSL(domain)
 
     try:
         imap.login(email, password)
     except imaplib.IMAP4.error as e:
         logger.error(f"Error logging into {email} on {domain}: {e}")
         imap.select("INBOX")
```

### Comparing `twscrape-0.6.0/twscrape/login.py` & `twscrape-0.7.0/twscrape/login.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import datetime, timedelta, timezone
 
 from httpx import AsyncClient, HTTPStatusError, Response
 
 from .account import Account
 from .constants import LOGIN_URL
-from .imap import imap_get_email_code, imap_try_login
+from .imap import imap_get_email_code, imap_login
 from .logger import logger
 from .utils import raise_for_status
 
 
 async def get_guest_token(client: AsyncClient):
     rep = await client.post("https://api.twitter.com/1.1/guest/activate.json")
     raise_for_status(rep, "guest_token")
@@ -113,14 +113,17 @@
 
     rep = await client.post(LOGIN_URL, json=payload)
     raise_for_status(rep, "login_confirm_email")
     return rep
 
 
 async def login_confirm_email_code(client: AsyncClient, acc: Account, prev: dict, imap):
+    if not imap:
+        imap = await imap_login(acc.email, acc.password)
+
     now_time = datetime.now(timezone.utc) - timedelta(seconds=30)
     value = await imap_get_email_code(imap, acc.email, now_time)
 
     payload = {
         "flow_token": prev["flow_token"],
         "subtask_inputs": [
             {
@@ -177,22 +180,24 @@
             acc.error_msg = f"login_step={task_id} err={e}"
             logger.error(f"Error in {task_id}: {e}")
             raise e
 
     return None
 
 
-async def login(acc: Account, fresh=False) -> Account:
+async def login(acc: Account, email_first=False) -> Account:
     log_id = f"{acc.username} - {acc.email}"
-    if acc.active and not fresh:
+    if acc.active:
         logger.info(f"account already active {log_id}")
         return acc
 
-    # check if email is valid first
-    imap = await imap_try_login(acc.email, acc.email_password)
+    if email_first:
+        imap = await imap_login(acc.email, acc.email_password)
+    else:
+        imap = None
 
     client = acc.make_client()
     guest_token = await get_guest_token(client)
     client.headers["x-guest-token"] = guest_token
 
     rep = await login_initiate(client)
     while True:
```

### Comparing `twscrape-0.6.0/twscrape/models.py` & `twscrape-0.7.0/twscrape/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 import email.utils
 import json
+import os
+import random
 import re
+import string
+import traceback
 from dataclasses import asdict, dataclass, field
 from datetime import datetime
 from typing import Generator, Optional
 
 import httpx
 
 from .logger import logger
@@ -105,14 +109,16 @@
     listedCount: int
     mediaCount: int
     location: str
     profileImageUrl: str
     profileBannerUrl: str | None = None
     protected: bool | None = None
     verified: bool | None = None
+    blue: bool | None = None
+    blueType: str | None = None
     descriptionLinks: list[TextLink] = field(default_factory=list)
     _type: str = "snscrape.modules.twitter.User"
 
     # todo:
     # link: typing.Optional[TextLink] = None
     # label: typing.Optional["UserLabel"] = None
 
@@ -132,14 +138,16 @@
             favouritesCount=obj["favourites_count"],
             listedCount=obj["listed_count"],
             mediaCount=obj["media_count"],
             location=obj["location"],
             profileImageUrl=obj["profile_image_url_https"],
             profileBannerUrl=obj.get("profile_banner_url"),
             verified=obj.get("verified"),
+            blue=obj.get("is_blue_verified"),
+            blueType=obj.get("verified_type"),
             protected=obj.get("protected"),
             descriptionLinks=_parse_links(obj, ["entities.description.urls", "entities.url.urls"]),
         )
 
 
 @dataclass
 class Tweet(JSONTrait):
@@ -183,22 +191,15 @@
 
         rt_id = _first(obj, ["retweeted_status_id_str", "retweeted_status_result.result.rest_id"])
         rt_obj = get_or(res, f"tweets.{rt_id}")
 
         qt_id = _first(obj, ["quoted_status_id_str", "quoted_status_result.result.rest_id"])
         qt_obj = get_or(res, f"tweets.{qt_id}")
 
-        # for development
-        # print()
-        # print("-" * 80)
-        # print(res["tweets"].keys())
-        # print(rt_id, rt_obj is not None)
-        # print(qt_id, qt_obj is not None)
-
-        return Tweet(
+        doc = Tweet(
             id=int(obj["id_str"]),
             id_str=obj["id_str"],
             url=f'https://twitter.com/{tw_usr.username}/status/{obj["id_str"]}',
             date=email.utils.parsedate_to_datetime(obj["created_at"]),
             user=tw_usr,
             lang=obj["lang"],
             rawContent=get_or(obj, "note_tweet.note_tweet_results.result.text", obj["full_text"]),
@@ -220,24 +221,32 @@
             inReplyToUser=_get_reply_user(obj, res),
             source=obj.get("source", None),
             sourceUrl=_get_source_url(obj),
             sourceLabel=_get_source_label(obj),
             media=Media.parse(obj),
         )
 
+        # issue #42 – restore full rt text
+        rt = doc.retweetedTweet
+        if rt is not None and rt.user is not None and doc.rawContent.endswith("…"):
+            prefix = f"RT @{rt.user.username}: "
+            rt_msg = f"{prefix}{rt.rawContent}"
+            if doc.rawContent != rt_msg and doc.rawContent.startswith(prefix):
+                doc.rawContent = rt_msg
+
+        return doc
+
 
 @dataclass
 class MediaPhoto(JSONTrait):
     url: str
 
     @staticmethod
     def parse(obj: dict):
-        return MediaPhoto(
-            url=obj["media_url_https"],
-        )
+        return MediaPhoto(url=obj["media_url_https"])
 
 
 @dataclass
 class MediaVideo(JSONTrait):
     thumbnailUrl: str
     variants: list["MediaVideoVariant"]
     duration: int
@@ -315,14 +324,17 @@
                 continue
 
             logger.warning(f"Unknown media type: {x['type']}: {json.dumps(x)}")
 
         return Media(photos=photos, videos=videos, animated=animated)
 
 
+# internal helpers
+
+
 def _get_reply_user(tw_obj: dict, res: dict):
     user_id = tw_obj.get("in_reply_to_user_id_str", None)
     if user_id is None:
         return None
 
     if user_id in res["users"]:
         return UserRef.parse(res["users"][user_id])
@@ -373,38 +385,87 @@
         for y in ["ext_views.count", "views.count"]:
             k = int_or_none(x, y)
             if k is not None:
                 return k
     return None
 
 
-# reply parsing
+def _write_dump(kind: str, e: Exception, x: dict, obj: dict):
+    uniq = "".join(random.choice(string.ascii_lowercase) for _ in range(5))
+    time = datetime.utcnow().strftime("%Y-%m-%d_%H-%M-%S")
+    dumpfile = f"/tmp/twscrape/twscrape_parse_error_{time}_{uniq}.txt"
+    os.makedirs(os.path.dirname(dumpfile), exist_ok=True)
+
+    with open(dumpfile, "w") as fp:
+        msg = [
+            f"Error parsing {kind}. Error: {type(e)}",
+            traceback.format_exc(),
+            json.dumps(x, default=str),
+            json.dumps(obj, default=str),
+        ]
+        fp.write("\n\n".join(msg))
+
+    logger.error(f"Failed to parse response of {kind}, writing dump to {dumpfile}")
 
 
-def get_items(rep: httpx.Response, kind: str, limit: int = -1):
+def _parse_items(rep: httpx.Response, kind: str, limit: int = -1):
     if kind == "user":
-        Cls = User
-        key = "users"
+        Cls, key = User, "users"
     elif kind == "tweet":
-        Cls = Tweet
-        key = "tweets"
+        Cls, key = Tweet, "tweets"
     else:
         raise ValueError(f"Invalid kind: {kind}")
 
+    # check for dict, because httpx.Response can be mocked in tests with different type
+    res = rep if isinstance(rep, dict) else rep.json()
+    obj = to_old_rep(res)
+
     ids = set()
-    obj = to_old_rep(rep.json() if "json" in rep else rep)  # type: ignore
     for x in obj[key].values():
         if limit != -1 and len(ids) >= limit:
-            break
+            # todo: move somewhere in configuration like force_limit
+            # https://github.com/vladkens/twscrape/issues/26#issuecomment-1656875132
+            # break
+            pass
+
+        try:
+            tmp = Cls.parse(x, obj)
+            if tmp.id not in ids:
+                ids.add(tmp.id)
+                yield tmp
+        except Exception as e:
+            _write_dump(kind, e, x, obj)
+            continue
 
-        tmp = Cls.parse(x, obj)
-        if tmp.id not in ids:
-            ids.add(tmp.id)
-            yield tmp
 
+# public helpers
 
-def get_tweets(rep: httpx.Response, limit: int = -1) -> Generator[Tweet, None, None]:
-    return get_items(rep, "tweet", limit)  # type: ignore
 
+def parse_tweets(rep: httpx.Response, limit: int = -1) -> Generator[Tweet, None, None]:
+    return _parse_items(rep, "tweet", limit)  # type: ignore
 
-def get_users(rep: httpx.Response, limit: int = -1) -> Generator[User, None, None]:
-    return get_items(rep, "user", limit)  # type: ignore
+
+def parse_users(rep: httpx.Response, limit: int = -1) -> Generator[User, None, None]:
+    return _parse_items(rep, "user", limit)  # type: ignore
+
+
+def parse_tweet(rep: httpx.Response, twid: int) -> Tweet | None:
+    try:
+        docs = list(parse_tweets(rep))
+        for x in docs:
+            if x.id == twid:
+                return x
+        return None
+    except Exception as e:
+        logger.error(f"Failed to parse tweet {twid} - {type(e)}:\n{traceback.format_exc()}")
+        return None
+
+
+def parse_user(rep: httpx.Response) -> User | None:
+    try:
+        docs = list(parse_users(rep))
+        if len(docs) == 1:
+            return docs[0]
+        return None
+    except Exception as e:
+        logger.error(f"Failed to parse user - {type(e)}:\n{traceback.format_exc()}")
+        return None
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `twscrape-0.6.0/twscrape/queue_client.py` & `twscrape-0.7.0/twscrape/queue_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,12 +186,15 @@
 
                 ctx.req_count += 1  # count only successful
                 retry_count = 0
                 return rep
             except (RateLimitError, BannedError):
                 # already handled
                 continue
+            except (httpx.ReadTimeout, httpx.ProxyError):
+                # http transport failed, just retry
+                continue
             except Exception as e:
                 retry_count += 1
                 if retry_count >= 3:
                     logger.warning(f"Unknown error {type(e)}: {e}")
                     await self._close_ctx(utc_ts() + 60 * 15)  # 15 minutes
```

### Comparing `twscrape-0.6.0/twscrape/utils.py` & `twscrape-0.7.0/twscrape/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,14 +189,17 @@
         val = base64.b64decode(val).decode()
     except Exception:
         pass
 
     try:
         try:
             res = json.loads(val)
+            if isinstance(res, dict) and "cookies" in res:
+                res = res["cookies"]
+
             if isinstance(res, list):
                 return {x["name"]: x["value"] for x in res}
             if isinstance(res, dict):
                 return res
         except json.JSONDecodeError:
             res = val.split("; ")
             res = [x.split("=") for x in res]
```

### Comparing `twscrape-0.6.0/.gitignore` & `twscrape-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `twscrape-0.6.0/LICENSE` & `twscrape-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twscrape-0.6.0/pyproject.toml` & `twscrape-0.7.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "twscrape"
-version = "0.6.0"
+version = "0.7.0"
 authors = [{name = "vladkens", email = "v.pronsky@gmail.com"}]
 description = "Twitter GraphQL and Search API implementation with SNScrape data models"
 readme = "readme.md"
 requires-python = ">=3.10"
 keywords = ["twitter", "scrape", "scrapper", "api", "snscrape"]
 license = {text = "MIT"}
 classifiers = [
```

### Comparing `twscrape-0.6.0/readme.md` & `twscrape-0.7.0/readme.md`

 * *Files identical despite different names*

### Comparing `twscrape-0.6.0/PKG-INFO` & `twscrape-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twscrape
-Version: 0.6.0
+Version: 0.7.0
 Summary: Twitter GraphQL and Search API implementation with SNScrape data models
 Project-URL: repository, https://github.com/vladkens/twscrape
 Author-email: vladkens <v.pronsky@gmail.com>
 License: MIT
 License-File: LICENSE
 Keywords: api,scrape,scrapper,snscrape,twitter
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: twscrape Version: 0.6.0 Summary: Twitter GraphQL
+Metadata-Version: 2.1 Name: twscrape Version: 0.7.0 Summary: Twitter GraphQL
 and Search API implementation with SNScrape data models Project-URL:
 repository, https://github.com/vladkens/twscrape Author-email: vladkens
 pronsky@gmail.com> License: MIT License-File: LICENSE Keywords:
 api,scrape,scrapper,snscrape,twitter Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10 Requires-Dist: aiosqlite==0.17.0 Requires-Dist: fake-
```

