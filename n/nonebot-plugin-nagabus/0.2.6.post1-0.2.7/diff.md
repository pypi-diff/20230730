# Comparing `tmp/nonebot_plugin_nagabus-0.2.6.post1.tar.gz` & `tmp/nonebot_plugin_nagabus-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nagabus-0.2.6.post1.tar", max compression
+gzip compressed data, was "nonebot_plugin_nagabus-0.2.7.tar", max compression
```

## Comparing `nonebot_plugin_nagabus-0.2.6.post1.tar` & `nonebot_plugin_nagabus-0.2.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448000 nonebot_plugin_nagabus-0.2.6.post1/LICENSE
--rw-r--r--   0        0        0     1485 2023-06-27 03:08:54.351266 nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/__init__.py
--rw-r--r--   0        0        0      129 2023-05-27 04:29:09.849196 nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/ac.py
--rw-r--r--   0        0        0     1364 2023-06-19 13:39:23.142435 nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/config.py
--rw-r--r--   0        0        0        4 2023-05-26 13:11:24.775555 nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/data/__init__.py
--rw-r--r--   0        0        0      116 2023-05-26 11:41:42.946553 nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/data/base.py
--rw-r--r--   0        0        0      317 2023-05-26 11:41:42.956553 nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/data/mjs.py
--rw-r--r--   0        0        0     1697 2023-06-19 13:39:23.142435 nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/data/naga.py
--rw-r--r--   0        0        0      775 2023-05-26 11:41:42.960551 nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/data/session.py
--rw-r--r--   0        0        0      715 2023-06-19 13:39:23.143434 nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/data/utils/__init__.py
--rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843000 nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/data/utils/utc_datetime.py
--rw-r--r--   0        0        0       43 2023-05-28 14:51:33.785849 nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/errors.py
--rw-r--r--   0        0        0       95 2023-05-28 01:19:53.575323 nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/matchers/__init__.py
--rw-r--r--   0        0        0      189 2023-05-30 02:32:55.940589 nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/matchers/errors.py
--rw-r--r--   0        0        0        0 2023-05-30 02:22:08.333037 nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/matchers/interceptors/__init__.py
--rw-r--r--   0        0        0     2874 2023-06-27 03:05:14.174566 nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/matchers/interceptors/handle_error.py
--rw-r--r--   0        0        0     4650 2023-06-19 13:39:23.144435 nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/matchers/naga_analyze.py
--rw-r--r--   0        0        0     2840 2023-06-27 03:07:21.048380 nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/matchers/naga_statistic.py
--rw-r--r--   0        0        0     2278 2023-05-27 02:48:33.707764 nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/migrations/24aec3c56623_.py
--rw-r--r--   0        0        0     1617 2023-06-19 13:39:23.145434 nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/migrations/70ff5fb4923e_.py
--rw-r--r--   0        0        0     1350 2023-05-27 07:17:07.623159 nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py
--rw-r--r--   0        0        0      998 2023-07-28 15:04:21.945700 nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/mjs/__init__.py
--rw-r--r--   0        0        0      178 2023-06-19 13:39:23.146434 nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/naga/__init__.py
--rw-r--r--   0        0        0     4102 2023-07-29 03:59:30.075477 nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/naga/api.py
--rw-r--r--   0        0        0      436 2023-06-19 13:39:23.147435 nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/naga/errors.py
--rw-r--r--   0        0        0     3669 2023-06-27 03:05:14.166569 nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/naga/fake_api.py
--rw-r--r--   0        0        0     1248 2023-06-19 13:39:23.148435 nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/naga/model.py
--rw-r--r--   0        0        0    21282 2023-06-27 03:05:14.157193 nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/naga/service.py
--rw-r--r--   0        0        0      347 2023-06-19 13:39:23.149434 nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/naga/utils.py
--rw-r--r--   0        0        0        0 2023-05-25 16:04:02.955709 nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/utils/__init__.py
--rw-r--r--   0        0        0     1092 2023-05-25 16:06:56.701500 nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/utils/integer.py
--rw-r--r--   0        0        0        0 2023-05-26 12:48:40.974521 nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/utils/mapping.py
--rw-r--r--   0        0        0      101 2023-05-25 08:09:22.247000 nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/utils/nonebot.py
--rw-r--r--   0        0        0       68 2023-05-26 15:50:47.559077 nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/utils/tz.py
--rw-r--r--   0        0        0     1002 2023-07-29 03:59:30.070481 nonebot_plugin_nagabus-0.2.6.post1/pyproject.toml
--rw-r--r--   0        0        0     1789 2023-05-28 03:26:24.309853 nonebot_plugin_nagabus-0.2.6.post1/README.md
--rw-r--r--   0        0        0     2670 1970-01-01 00:00:00.000000 nonebot_plugin_nagabus-0.2.6.post1/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448000 nonebot_plugin_nagabus-0.2.7/LICENSE
+-rw-r--r--   0        0        0     1485 2023-06-27 03:08:54.351266 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/__init__.py
+-rw-r--r--   0        0        0      129 2023-05-27 04:29:09.849196 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/ac.py
+-rw-r--r--   0        0        0     1364 2023-06-19 13:39:23.142435 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/config.py
+-rw-r--r--   0        0        0        4 2023-05-26 13:11:24.775555 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/data/__init__.py
+-rw-r--r--   0        0        0      116 2023-05-26 11:41:42.946553 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/data/base.py
+-rw-r--r--   0        0        0      317 2023-05-26 11:41:42.956553 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/data/mjs.py
+-rw-r--r--   0        0        0     1697 2023-06-19 13:39:23.142435 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/data/naga.py
+-rw-r--r--   0        0        0      775 2023-05-26 11:41:42.960551 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/data/session.py
+-rw-r--r--   0        0        0      715 2023-06-19 13:39:23.143434 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/data/utils/__init__.py
+-rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843000 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/data/utils/utc_datetime.py
+-rw-r--r--   0        0        0       43 2023-05-28 14:51:33.785849 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/errors.py
+-rw-r--r--   0        0        0       95 2023-05-28 01:19:53.575323 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/matchers/__init__.py
+-rw-r--r--   0        0        0      189 2023-05-30 02:32:55.940589 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/matchers/errors.py
+-rw-r--r--   0        0        0        0 2023-05-30 02:22:08.333037 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/matchers/interceptors/__init__.py
+-rw-r--r--   0        0        0     2874 2023-06-27 03:05:14.174566 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/matchers/interceptors/handle_error.py
+-rw-r--r--   0        0        0     4650 2023-06-19 13:39:23.144435 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/matchers/naga_analyze.py
+-rw-r--r--   0        0        0     2840 2023-06-27 03:07:21.048380 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/matchers/naga_statistic.py
+-rw-r--r--   0        0        0     2278 2023-05-27 02:48:33.707764 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/migrations/24aec3c56623_.py
+-rw-r--r--   0        0        0     1617 2023-06-19 13:39:23.145434 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/migrations/70ff5fb4923e_.py
+-rw-r--r--   0        0        0     1350 2023-05-27 07:17:07.623159 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py
+-rw-r--r--   0        0        0      998 2023-07-28 15:04:21.945700 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/mjs/__init__.py
+-rw-r--r--   0        0        0      178 2023-06-19 13:39:23.146434 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/naga/__init__.py
+-rw-r--r--   0        0        0     4617 2023-07-30 16:24:05.300757 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/naga/api.py
+-rw-r--r--   0        0        0      436 2023-06-19 13:39:23.147435 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/naga/errors.py
+-rw-r--r--   0        0        0     3669 2023-06-27 03:05:14.166569 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/naga/fake_api.py
+-rw-r--r--   0        0        0     1248 2023-06-19 13:39:23.148435 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/naga/model.py
+-rw-r--r--   0        0        0    21282 2023-06-27 03:05:14.157193 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/naga/service.py
+-rw-r--r--   0        0        0      347 2023-06-19 13:39:23.149434 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/naga/utils.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:04:02.955709 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/utils/__init__.py
+-rw-r--r--   0        0        0     1092 2023-05-25 16:06:56.701500 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/utils/integer.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:48:40.974521 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/utils/mapping.py
+-rw-r--r--   0        0        0      101 2023-05-25 08:09:22.247000 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/utils/nonebot.py
+-rw-r--r--   0        0        0       68 2023-05-26 15:50:47.559077 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/utils/tz.py
+-rw-r--r--   0        0        0      996 2023-07-30 16:24:28.982337 nonebot_plugin_nagabus-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     1789 2023-05-28 03:26:24.309853 nonebot_plugin_nagabus-0.2.7/README.md
+-rw-r--r--   0        0        0     2664 1970-01-01 00:00:00.000000 nonebot_plugin_nagabus-0.2.7/PKG-INFO
```

### Comparing `nonebot_plugin_nagabus-0.2.6.post1/LICENSE` & `nonebot_plugin_nagabus-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/__init__.py` & `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/config.py` & `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/data/naga.py` & `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/data/naga.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/data/session.py` & `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/data/session.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/data/utils/__init__.py` & `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/data/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/data/utils/utc_datetime.py` & `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/data/utils/utc_datetime.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/matchers/interceptors/handle_error.py` & `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/matchers/interceptors/handle_error.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/matchers/naga_analyze.py` & `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/matchers/naga_analyze.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/matchers/naga_statistic.py` & `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/matchers/naga_statistic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/migrations/24aec3c56623_.py` & `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/migrations/24aec3c56623_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/migrations/70ff5fb4923e_.py` & `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/migrations/70ff5fb4923e_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py` & `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/mjs/__init__.py` & `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/mjs/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/naga/api.py` & `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/naga/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,20 +28,25 @@
         "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36 Edg/113.0.1774.35",
     }
 
     def __init__(self, cookies: Dict[str, str]):
         self.cookies = Cookies(cookies)
 
         async def req_hook(request):
+            # 手动设置cookies
             self.cookies.set_cookie_header(request)
             logger.trace(f"Request: {request.method} {request.url} - Waiting for response")
 
         async def resp_hook(response):
             request = response.request
             logger.trace(f"Response: {request.method} {request.url} - Status {response.status_code}")
+
+            # 始终清除掉响应带的cookies
+            self.client.cookies = None
+
             response.raise_for_status()
 
         self.client: AsyncClient = AsyncClient(
             base_url=self._BASE_URL,
             headers=self._HEADER,
             follow_redirects=True,
             event_hooks={'request': [req_hook], 'response': [resp_hook]},
@@ -56,24 +61,33 @@
             headers={
                 "Referer": "https://naga.dmv.nico/naga_report/order_report_list/"
             },
             params={"year": year, "month": month}
         )
         return OrderReportList.parse_obj(resp.json())
 
+    async def _get_csrfmiddlewaretoken(self) -> str:
+        resp = await self.client.get(
+            "/order_form/"
+        )
+        mat = re.search(r"<input type=\"hidden\" name=\"csrfmiddlewaretoken\" value=\"(.*)\">", resp.text)
+        if mat is None:
+            raise RuntimeError("cannot get csrfmiddlewaretoken")
+        return mat.group(1)
+
     async def analyze_tenhou(self, haihu_id: str, seat: int,
                              rule: NagaGameRule,
                              model_type: Union[Sequence[NagaHanchanModelType],
                                                Sequence[NagaHanchanModelType]]) -> AnalyzeTenhou:
         data = {
             "haihu_id": haihu_id,
             "seat": seat,
             "reanalysis": 0,
             "player_types": model_type_to_str(model_type),
-            "csrfmiddlewaretoken": self.cookies["csrftoken"]
+            "csrfmiddlewaretoken": await self._get_csrfmiddlewaretoken()
         }
 
         resp = await self.client.post(
             "/api/url_analyze/",
             headers={
                 "Referer": "https://naga.dmv.nico/naga_report/order_form/"
             },
@@ -93,15 +107,15 @@
             data = json.dumps(data, ensure_ascii=False)
 
         res_data = {
             "json_data": data,
             "seat": seat,
             "game_type": rule.value,
             "player_types": model_type_to_str(model_type),
-            "csrfmiddlewaretoken": self.cookies["csrftoken"]
+            "csrfmiddlewaretoken": await self._get_csrfmiddlewaretoken()
         }
 
         await self.client.post(
             "/api/custom_haihu_analyze/",
             headers={
                 "Referer": "https://naga.dmv.nico/naga_report/order_form/"
             },
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/naga/fake_api.py` & `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/naga/fake_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/naga/model.py` & `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/naga/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/naga/service.py` & `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/naga/service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.6.post1/nonebot_plugin_nagabus/utils/integer.py` & `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/utils/integer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.6.post1/pyproject.toml` & `nonebot_plugin_nagabus-0.2.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-nagabus"
-version = "0.2.6.post1"
+version = "0.2.7"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 readme = "README.md"
 packages = [{ include = "nonebot_plugin_nagabus" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `nonebot_plugin_nagabus-0.2.6.post1/README.md` & `nonebot_plugin_nagabus-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.6.post1/PKG-INFO` & `nonebot_plugin_nagabus-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nagabus
-Version: 0.2.6.post1
+Version: 0.2.7
 Summary: 
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

