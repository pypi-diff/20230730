# Comparing `tmp/garth-0.3.2.tar.gz` & `tmp/garth-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garth-0.3.2.tar", last modified: Sun Jul 30 00:46:26 2023, max compression
+gzip compressed data, was "garth-0.3.3.tar", last modified: Sun Jul 30 01:23:43 2023, max compression
```

## Comparing `garth-0.3.2.tar` & `garth-0.3.3.tar`

### file list

```diff
@@ -1,50 +1,53 @@
--rw-r--r--   0        0        0     1071 2023-07-20 12:44:00.130760 garth-0.3.2/LICENSE
--rw-r--r--   0        0        0    12322 2023-07-29 23:44:50.244943 garth-0.3.2/README.md
--rw-r--r--   0        0        0      653 2023-07-29 23:23:30.395971 garth-0.3.2/garth/__init__.py
--rw-r--r--   0        0        0      931 2023-07-28 12:08:41.094670 garth-0.3.2/garth/auth_token.py
--rw-r--r--   0        0        0      145 2023-07-18 22:32:58.010661 garth-0.3.2/garth/exc.py
--rw-r--r--   0        0        0     4673 2023-07-28 12:13:51.131928 garth-0.3.2/garth/http.py
--rw-r--r--   0        0        0        0 2023-07-27 13:16:10.642595 garth-0.3.2/garth/py.typed
--rw-r--r--   0        0        0      392 2023-07-29 23:23:57.760715 garth-0.3.2/garth/resources/__init__.py
--rw-r--r--   0        0        0      612 2023-07-29 23:28:46.923483 garth-0.3.2/garth/resources/intensity_minutes.py
--rw-r--r--   0        0        0     3536 2023-07-29 23:32:07.004688 garth-0.3.2/garth/resources/sleep.py
--rw-r--r--   0        0        0      654 2023-07-29 23:30:44.232250 garth-0.3.2/garth/resources/steps.py
--rw-r--r--   0        0        0      653 2023-07-29 23:30:50.433149 garth-0.3.2/garth/resources/stress.py
--rw-r--r--   0        0        0     3767 2023-07-28 12:13:50.747670 garth-0.3.2/garth/sso.py
--rw-r--r--   0        0        0     1529 2023-07-29 23:29:30.202390 garth-0.3.2/garth/stats.py
--rw-r--r--   0        0        0     1294 2023-07-28 02:46:53.372554 garth-0.3.2/garth/utils.py
--rw-r--r--   0        0        0       22 2023-07-30 00:45:53.783018 garth-0.3.2/garth/version.py
--rw-r--r--   0        0        0     1146 2023-07-30 00:46:26.427362 garth-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     2386 2023-07-22 11:39:14.617674 garth-0.3.2/tests/cassettes/test_client_get.yaml
--rw-r--r--   0        0        0     2425 2023-07-22 11:39:14.746057 garth-0.3.2/tests/cassettes/test_client_post.yaml
--rw-r--r--   0        0        0   100962 2023-07-22 11:22:15.428262 garth-0.3.2/tests/cassettes/test_client_request.yaml
--rw-r--r--   0        0        0     2331 2023-07-28 03:35:21.644342 garth-0.3.2/tests/cassettes/test_connectapi.yaml
--rw-r--r--   0        0        0     4564 2023-07-28 03:35:21.644997 garth-0.3.2/tests/cassettes/test_connectapi_refresh.yaml
--rw-r--r--   0        0        0     3231 2023-07-28 03:35:21.645581 garth-0.3.2/tests/cassettes/test_exchange.yaml
--rw-r--r--   0        0        0    10962 2023-07-23 13:53:16.232082 garth-0.3.2/tests/cassettes/test_get_username.yaml
--rw-r--r--   0        0        0    50551 2023-07-22 15:27:42.274531 garth-0.3.2/tests/cassettes/test_login_email_password_fail.yaml
--rw-r--r--   0        0        0    91847 2023-07-23 13:50:32.012417 garth-0.3.2/tests/cassettes/test_login_success.yaml
--rw-r--r--   0        0        0     2270 2023-07-28 03:35:21.646057 garth-0.3.2/tests/cassettes/test_refresh.yaml
--rw-r--r--   0        0        0     2963 2023-07-28 03:35:21.646600 garth-0.3.2/tests/cassettes/test_refresh_expired.yaml
--rw-r--r--   0        0        0     3080 2023-07-28 12:57:32.501754 garth-0.3.2/tests/conftest.py
--rw-r--r--   0        0        0     4197 2023-07-29 23:34:06.394173 garth-0.3.2/tests/resources/cassettes/test_daily_intensity_minutes.yaml
--rw-r--r--   0        0        0     3098 2023-07-28 03:35:40.317256 garth-0.3.2/tests/resources/cassettes/test_daily_sleep.yaml
--rw-r--r--   0        0        0     4179 2023-07-29 17:52:20.398786 garth-0.3.2/tests/resources/cassettes/test_daily_steps.yaml
--rw-r--r--   0        0        0     6252 2023-07-28 03:35:40.317752 garth-0.3.2/tests/resources/cassettes/test_daily_stress.yaml
--rw-r--r--   0        0        0    44427 2023-07-28 03:35:40.318411 garth-0.3.2/tests/resources/cassettes/test_daily_stress_pagination.yaml
--rw-r--r--   0        0        0     3652 2023-07-28 12:21:13.363000 garth-0.3.2/tests/resources/cassettes/test_sleep_data_get.yaml
--rw-r--r--   0        0        0    77468 2023-07-28 12:22:31.103002 garth-0.3.2/tests/resources/cassettes/test_sleep_data_list.yaml
--rw-r--r--   0        0        0     3349 2023-07-29 23:35:28.845204 garth-0.3.2/tests/resources/cassettes/test_weekly_intensity_minutes.yaml
--rw-r--r--   0        0        0    13052 2023-07-29 17:52:45.776274 garth-0.3.2/tests/resources/cassettes/test_weekly_steps.yaml
--rw-r--r--   0        0        0     4717 2023-07-28 03:35:40.318832 garth-0.3.2/tests/resources/cassettes/test_weekly_stress.yaml
--rw-r--r--   0        0        0    16221 2023-07-28 03:35:40.319518 garth-0.3.2/tests/resources/cassettes/test_weekly_stress_beyond_data.yaml
--rw-r--r--   0        0        0     7522 2023-07-28 03:35:40.320026 garth-0.3.2/tests/resources/cassettes/test_weekly_stress_pagination.yaml
--rw-r--r--   0        0        0      748 2023-07-29 23:40:27.912636 garth-0.3.2/tests/resources/test_intensity_minutes.py
--rw-r--r--   0        0        0      849 2023-07-28 12:22:22.098284 garth-0.3.2/tests/resources/test_sleep.py
--rw-r--r--   0        0        0      667 2023-07-29 17:53:35.423973 garth-0.3.2/tests/resources/test_steps.py
--rw-r--r--   0        0        0     1437 2023-07-27 13:31:20.424008 garth-0.3.2/tests/resources/test_stress.py
--rw-r--r--   0        0        0     1808 2023-07-23 13:40:52.098938 garth-0.3.2/tests/test_auth_token.py
--rw-r--r--   0        0        0     4097 2023-07-28 12:02:46.585315 garth-0.3.2/tests/test_http.py
--rw-r--r--   0        0        0     2570 2023-07-28 12:10:36.895963 garth-0.3.2/tests/test_sso.py
--rw-r--r--   0        0        0      531 2023-07-27 13:16:10.645234 garth-0.3.2/tests/test_utils.py
--rw-r--r--   0        0        0    12734 1970-01-01 00:00:00.000000 garth-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-20 12:44:00.130760 garth-0.3.3/LICENSE
+-rw-r--r--   0        0        0    13326 2023-07-30 01:22:39.496857 garth-0.3.3/README.md
+-rw-r--r--   0        0        0      683 2023-07-30 01:10:44.332019 garth-0.3.3/garth/__init__.py
+-rw-r--r--   0        0        0      931 2023-07-28 12:08:41.094670 garth-0.3.3/garth/auth_token.py
+-rw-r--r--   0        0        0      145 2023-07-18 22:32:58.010661 garth-0.3.3/garth/exc.py
+-rw-r--r--   0        0        0     4671 2023-07-30 00:47:33.469751 garth-0.3.3/garth/http.py
+-rw-r--r--   0        0        0        0 2023-07-27 13:16:10.642595 garth-0.3.3/garth/py.typed
+-rw-r--r--   0        0        0      434 2023-07-30 01:10:27.575730 garth-0.3.3/garth/resources/__init__.py
+-rw-r--r--   0        0        0     1167 2023-07-30 01:22:51.576888 garth-0.3.3/garth/resources/hrv.py
+-rw-r--r--   0        0        0      612 2023-07-29 23:28:46.923483 garth-0.3.3/garth/resources/intensity_minutes.py
+-rw-r--r--   0        0        0     3524 2023-07-30 01:09:43.261424 garth-0.3.3/garth/resources/sleep.py
+-rw-r--r--   0        0        0      654 2023-07-29 23:30:44.232250 garth-0.3.3/garth/resources/steps.py
+-rw-r--r--   0        0        0      653 2023-07-29 23:30:50.433149 garth-0.3.3/garth/resources/stress.py
+-rw-r--r--   0        0        0     3767 2023-07-28 12:13:50.747670 garth-0.3.3/garth/sso.py
+-rw-r--r--   0        0        0     1529 2023-07-29 23:29:30.202390 garth-0.3.3/garth/stats.py
+-rw-r--r--   0        0        0     1319 2023-07-30 01:09:15.596865 garth-0.3.3/garth/utils.py
+-rw-r--r--   0        0        0       22 2023-07-30 01:23:26.019284 garth-0.3.3/garth/version.py
+-rw-r--r--   0        0        0     1146 2023-07-30 01:23:43.441312 garth-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2386 2023-07-22 11:39:14.617674 garth-0.3.3/tests/cassettes/test_client_get.yaml
+-rw-r--r--   0        0        0     2425 2023-07-22 11:39:14.746057 garth-0.3.3/tests/cassettes/test_client_post.yaml
+-rw-r--r--   0        0        0   100962 2023-07-22 11:22:15.428262 garth-0.3.3/tests/cassettes/test_client_request.yaml
+-rw-r--r--   0        0        0     2331 2023-07-28 03:35:21.644342 garth-0.3.3/tests/cassettes/test_connectapi.yaml
+-rw-r--r--   0        0        0     4564 2023-07-28 03:35:21.644997 garth-0.3.3/tests/cassettes/test_connectapi_refresh.yaml
+-rw-r--r--   0        0        0     3231 2023-07-28 03:35:21.645581 garth-0.3.3/tests/cassettes/test_exchange.yaml
+-rw-r--r--   0        0        0    10962 2023-07-23 13:53:16.232082 garth-0.3.3/tests/cassettes/test_get_username.yaml
+-rw-r--r--   0        0        0    50551 2023-07-22 15:27:42.274531 garth-0.3.3/tests/cassettes/test_login_email_password_fail.yaml
+-rw-r--r--   0        0        0    91847 2023-07-23 13:50:32.012417 garth-0.3.3/tests/cassettes/test_login_success.yaml
+-rw-r--r--   0        0        0     2270 2023-07-28 03:35:21.646057 garth-0.3.3/tests/cassettes/test_refresh.yaml
+-rw-r--r--   0        0        0     2963 2023-07-28 03:35:21.646600 garth-0.3.3/tests/cassettes/test_refresh_expired.yaml
+-rw-r--r--   0        0        0     3080 2023-07-28 12:57:32.501754 garth-0.3.3/tests/conftest.py
+-rw-r--r--   0        0        0     8524 2023-07-30 01:16:56.595924 garth-0.3.3/tests/resources/cassettes/test_daily_hrv.yaml
+-rw-r--r--   0        0        0     4197 2023-07-29 23:34:06.394173 garth-0.3.3/tests/resources/cassettes/test_daily_intensity_minutes.yaml
+-rw-r--r--   0        0        0     3098 2023-07-28 03:35:40.317256 garth-0.3.3/tests/resources/cassettes/test_daily_sleep.yaml
+-rw-r--r--   0        0        0     4179 2023-07-29 17:52:20.398786 garth-0.3.3/tests/resources/cassettes/test_daily_steps.yaml
+-rw-r--r--   0        0        0     6252 2023-07-28 03:35:40.317752 garth-0.3.3/tests/resources/cassettes/test_daily_stress.yaml
+-rw-r--r--   0        0        0    44427 2023-07-28 03:35:40.318411 garth-0.3.3/tests/resources/cassettes/test_daily_stress_pagination.yaml
+-rw-r--r--   0        0        0     3652 2023-07-28 12:21:13.363000 garth-0.3.3/tests/resources/cassettes/test_sleep_data_get.yaml
+-rw-r--r--   0        0        0    77468 2023-07-28 12:22:31.103002 garth-0.3.3/tests/resources/cassettes/test_sleep_data_list.yaml
+-rw-r--r--   0        0        0     3349 2023-07-29 23:35:28.845204 garth-0.3.3/tests/resources/cassettes/test_weekly_intensity_minutes.yaml
+-rw-r--r--   0        0        0    13052 2023-07-29 17:52:45.776274 garth-0.3.3/tests/resources/cassettes/test_weekly_steps.yaml
+-rw-r--r--   0        0        0     4717 2023-07-28 03:35:40.318832 garth-0.3.3/tests/resources/cassettes/test_weekly_stress.yaml
+-rw-r--r--   0        0        0    16221 2023-07-28 03:35:40.319518 garth-0.3.3/tests/resources/cassettes/test_weekly_stress_beyond_data.yaml
+-rw-r--r--   0        0        0     7522 2023-07-28 03:35:40.320026 garth-0.3.3/tests/resources/cassettes/test_weekly_stress_pagination.yaml
+-rw-r--r--   0        0        0      346 2023-07-30 01:22:47.002975 garth-0.3.3/tests/resources/test_hrv.py
+-rw-r--r--   0        0        0      748 2023-07-29 23:40:27.912636 garth-0.3.3/tests/resources/test_intensity_minutes.py
+-rw-r--r--   0        0        0      849 2023-07-28 12:22:22.098284 garth-0.3.3/tests/resources/test_sleep.py
+-rw-r--r--   0        0        0      667 2023-07-29 17:53:35.423973 garth-0.3.3/tests/resources/test_steps.py
+-rw-r--r--   0        0        0     1437 2023-07-27 13:31:20.424008 garth-0.3.3/tests/resources/test_stress.py
+-rw-r--r--   0        0        0     1808 2023-07-23 13:40:52.098938 garth-0.3.3/tests/test_auth_token.py
+-rw-r--r--   0        0        0     4095 2023-07-30 01:09:06.802029 garth-0.3.3/tests/test_http.py
+-rw-r--r--   0        0        0     2570 2023-07-28 12:10:36.895963 garth-0.3.3/tests/test_sso.py
+-rw-r--r--   0        0        0      531 2023-07-27 13:16:10.645234 garth-0.3.3/tests/test_utils.py
+-rw-r--r--   0        0        0    13738 1970-01-01 00:00:00.000000 garth-0.3.3/PKG-INFO
```

### Comparing `garth-0.3.2/LICENSE` & `garth-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/README.md` & `garth-0.3.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -303,14 +303,57 @@
         weekly_goal=150,
         moderate_value=101,
         vigorous_value=105
     )
 ]
 ```
 
+### HRV
+
+Daily HRV
+
+```python
+garth.DailyHRV.list(period=2)
+```
+
+```python
+[
+    DailyHRV(
+        calendar_date=datetime.date(2023, 7, 28),
+        weekly_avg=39,
+        last_night_avg=36,
+        last_night_5_min_high=52,
+        baseline=HRVBaseline(
+            low_upper=36,
+            balanced_low=39,
+            balanced_upper=51,
+            marker_value=0.25
+        ),
+        status='BALANCED',
+        feedback_phrase='HRV_BALANCED_2',
+        create_time_stamp=datetime.datetime(2023, 7, 28, 12, 40, 16, 785000)
+    ),
+    DailyHRV(
+        calendar_date=datetime.date(2023, 7, 29),
+        weekly_avg=40,
+        last_night_avg=41,
+        last_night_5_min_high=76,
+        baseline=HRVBaseline(
+            low_upper=36,
+            balanced_low=39,
+            balanced_upper=51,
+            marker_value=0.2916565
+        ),
+        status='BALANCED',
+        feedback_phrase='HRV_BALANCED_8',
+        create_time_stamp=datetime.datetime(2023, 7, 29, 13, 45, 23, 479000)
+    )
+]
+```
+
 ### Sleep
 
 Daily sleep quality
 
 ```python
 garth.DailySleep.list("2023-07-23", 2)
 ```
```

### Comparing `garth-0.3.2/garth/__init__.py` & `garth-0.3.3/garth/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from .http import client
 from .resources import (
+    DailyHRV,
     DailyIntensityMinutes,
     DailySleep,
     DailySteps,
     DailyStress,
     SleepData,
     WeeklyIntensityMinutes,
     WeeklySteps,
     WeeklyStress,
 )
 from .version import __version__
 
 __all__ = [
+    "DailyHRV",
     "DailyIntensityMinutes",
     "DailySleep",
     "DailySteps",
     "DailyStress",
     "SleepData",
     "WeeklyIntensityMinutes",
     "WeeklySteps",
```

### Comparing `garth-0.3.2/garth/auth_token.py` & `garth-0.3.3/garth/auth_token.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/garth/http.py` & `garth-0.3.3/garth/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 
 class Client:
     sess: Session
     last_resp: Response
     domain: str = "garmin.com"
     auth_token: AuthToken | None = None
     timeout: int = 15
-    retries: int = 3
+    retries: int = 5
     status_forcelist: tuple[int, ...] = (429, 500, 502, 503, 504)
-    backoff_factor: float = 0.5
+    backoff_factor: float = 1
     _username: str | None = None
 
     def __init__(self, session: Session | None = None, **kwargs):
         self.sess = session if session else Session()
         self.sess.headers.update(USER_AGENT)
         self.configure(
             timeout=self.timeout,
```

### Comparing `garth-0.3.2/garth/resources/intensity_minutes.py` & `garth-0.3.3/garth/resources/intensity_minutes.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/garth/resources/sleep.py` & `garth-0.3.3/garth/resources/sleep.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import date, datetime
-from typing import ClassVar, List, Optional
+from typing import ClassVar, Optional
 
 from pydantic.dataclasses import dataclass
 
 from .. import http
 from ..stats import Stats
 from ..utils import camel_to_snake_dict, date_range, format_end_date
 
@@ -87,15 +87,15 @@
     end_gmt: datetime
     activity_level: float
 
 
 @dataclass(frozen=True)
 class SleepData:
     daily_sleep_dto: DailySleepDTO
-    sleep_movement: List[SleepMovement]
+    sleep_movement: list[SleepMovement]
 
     @classmethod
     def get(cls, day: date | str, *, client: Optional[http.Client] = None):
         client = client or http.client
         path = (
             f"/wellness-service/wellness/dailySleepData/{client.username}?"
             f"nonSleepBufferMinutes=60&date={day}"
@@ -103,18 +103,18 @@
         sleep_data = client.connectapi(path)
         sleep_data = camel_to_snake_dict(sleep_data)
         return cls(**sleep_data)
 
     @classmethod
     def list(
         cls,
-        end: Optional[date] | str = None,
+        end: date | str | None = None,
         days: int = 1,
         *,
-        client: Optional[http.Client] = None,
+        client: http.Client | None = None,
     ):
         client = client or http.client
         end = format_end_date(end)
         sleep_data = [
             cls.get(date_, client=client) for date_ in date_range(end, days)
         ]
         return sorted(
```

### Comparing `garth-0.3.2/garth/resources/steps.py` & `garth-0.3.3/garth/resources/steps.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/garth/resources/stress.py` & `garth-0.3.3/garth/resources/stress.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/garth/sso.py` & `garth-0.3.3/garth/sso.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/garth/stats.py` & `garth-0.3.3/garth/stats.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/garth/utils.py` & `garth-0.3.3/garth/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import re
 from datetime import date, timedelta
 from typing import Any
 
-CAMEL_TO_SNAKE = re.compile(r"((?<=[a-z0-9])[A-Z]|(?!^)[A-Z](?=[a-z]))")
+CAMEL_TO_SNAKE = re.compile(
+    r"((?<=[a-z0-9])[A-Z]|(?!^)[A-Z](?=[a-z])|(?<=[a-zA-Z])[0-9])"
+)
 
 
 def camel_to_snake(camel_str: str) -> str:
     snake_str = CAMEL_TO_SNAKE.sub(r"_\1", camel_str)
     return snake_str.lower()
```

### Comparing `garth-0.3.2/pyproject.toml` & `garth-0.3.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
 ]
 packages = [
     { include = "garth" },
 ]
-version = "0.3.2"
+version = "0.3.3"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `garth-0.3.2/tests/cassettes/test_client_get.yaml` & `garth-0.3.3/tests/cassettes/test_client_get.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/tests/cassettes/test_client_post.yaml` & `garth-0.3.3/tests/cassettes/test_client_post.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/tests/cassettes/test_client_request.yaml` & `garth-0.3.3/tests/cassettes/test_client_request.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/tests/cassettes/test_connectapi.yaml` & `garth-0.3.3/tests/cassettes/test_connectapi.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/tests/cassettes/test_connectapi_refresh.yaml` & `garth-0.3.3/tests/cassettes/test_connectapi_refresh.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/tests/cassettes/test_exchange.yaml` & `garth-0.3.3/tests/cassettes/test_exchange.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/tests/cassettes/test_get_username.yaml` & `garth-0.3.3/tests/cassettes/test_get_username.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/tests/cassettes/test_login_email_password_fail.yaml` & `garth-0.3.3/tests/cassettes/test_login_email_password_fail.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/tests/cassettes/test_login_success.yaml` & `garth-0.3.3/tests/cassettes/test_login_success.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/tests/cassettes/test_refresh.yaml` & `garth-0.3.3/tests/cassettes/test_refresh.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/tests/cassettes/test_refresh_expired.yaml` & `garth-0.3.3/tests/cassettes/test_refresh_expired.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/tests/conftest.py` & `garth-0.3.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/tests/resources/cassettes/test_daily_intensity_minutes.yaml` & `garth-0.3.3/tests/resources/cassettes/test_daily_intensity_minutes.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/tests/resources/cassettes/test_daily_sleep.yaml` & `garth-0.3.3/tests/resources/cassettes/test_daily_sleep.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/tests/resources/cassettes/test_daily_steps.yaml` & `garth-0.3.3/tests/resources/cassettes/test_daily_steps.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/tests/resources/cassettes/test_daily_stress.yaml` & `garth-0.3.3/tests/resources/cassettes/test_daily_stress.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/tests/resources/cassettes/test_daily_stress_pagination.yaml` & `garth-0.3.3/tests/resources/cassettes/test_daily_stress_pagination.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/tests/resources/cassettes/test_sleep_data_get.yaml` & `garth-0.3.3/tests/resources/cassettes/test_sleep_data_get.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/tests/resources/cassettes/test_sleep_data_list.yaml` & `garth-0.3.3/tests/resources/cassettes/test_sleep_data_list.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/tests/resources/cassettes/test_weekly_intensity_minutes.yaml` & `garth-0.3.3/tests/resources/cassettes/test_weekly_intensity_minutes.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/tests/resources/cassettes/test_weekly_steps.yaml` & `garth-0.3.3/tests/resources/cassettes/test_weekly_steps.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/tests/resources/cassettes/test_weekly_stress.yaml` & `garth-0.3.3/tests/resources/cassettes/test_weekly_stress.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/tests/resources/cassettes/test_weekly_stress_beyond_data.yaml` & `garth-0.3.3/tests/resources/cassettes/test_weekly_stress_beyond_data.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/tests/resources/cassettes/test_weekly_stress_pagination.yaml` & `garth-0.3.3/tests/resources/cassettes/test_weekly_stress_pagination.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/tests/resources/test_intensity_minutes.py` & `garth-0.3.3/tests/resources/test_intensity_minutes.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/tests/resources/test_sleep.py` & `garth-0.3.3/tests/resources/test_sleep.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/tests/resources/test_steps.py` & `garth-0.3.3/tests/resources/test_steps.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/tests/resources/test_stress.py` & `garth-0.3.3/tests/resources/test_stress.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/tests/test_auth_token.py` & `garth-0.3.3/tests/test_auth_token.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/tests/test_http.py` & `garth-0.3.3/tests/test_http.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 def test_configure_timeout(client: Client):
     assert client.timeout == 15
     client.configure(timeout=99)
     assert client.timeout == 99
 
 
 def test_configure_retry(client: Client):
-    assert client.retries == 3
+    assert client.retries == 5
     assert client.sess.adapters["https://"].max_retries.total == client.retries
     client.configure(retries=99)
     assert client.retries == 99
     assert client.sess.adapters["https://"].max_retries.total == 99
 
 
 def test_configure_status_forcelist(client: Client):
@@ -62,15 +62,15 @@
         == client.status_forcelist
     )
     client.configure(status_forcelist=(200, 201, 202))
     assert client.status_forcelist == (200, 201, 202)
 
 
 def test_backoff_factor(client: Client):
-    assert client.backoff_factor == 0.5
+    assert client.backoff_factor == 1
     assert (
         client.sess.adapters["https://"].max_retries.backoff_factor
         == client.backoff_factor
     )
     client.configure(backoff_factor=0.99)
     assert client.backoff_factor == 0.99
     assert (
```

### Comparing `garth-0.3.2/tests/test_sso.py` & `garth-0.3.3/tests/test_sso.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/tests/test_utils.py` & `garth-0.3.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.2/PKG-INFO` & `garth-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garth
-Version: 0.3.2
+Version: 0.3.3
 Summary: Garmin SSO auth + Connect client
 Author-Email: Matin Tamizi <mtamizi@duck.com>
 License: MIT
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
@@ -317,14 +317,57 @@
         weekly_goal=150,
         moderate_value=101,
         vigorous_value=105
     )
 ]
 ```
 
+### HRV
+
+Daily HRV
+
+```python
+garth.DailyHRV.list(period=2)
+```
+
+```python
+[
+    DailyHRV(
+        calendar_date=datetime.date(2023, 7, 28),
+        weekly_avg=39,
+        last_night_avg=36,
+        last_night_5_min_high=52,
+        baseline=HRVBaseline(
+            low_upper=36,
+            balanced_low=39,
+            balanced_upper=51,
+            marker_value=0.25
+        ),
+        status='BALANCED',
+        feedback_phrase='HRV_BALANCED_2',
+        create_time_stamp=datetime.datetime(2023, 7, 28, 12, 40, 16, 785000)
+    ),
+    DailyHRV(
+        calendar_date=datetime.date(2023, 7, 29),
+        weekly_avg=40,
+        last_night_avg=41,
+        last_night_5_min_high=76,
+        baseline=HRVBaseline(
+            low_upper=36,
+            balanced_low=39,
+            balanced_upper=51,
+            marker_value=0.2916565
+        ),
+        status='BALANCED',
+        feedback_phrase='HRV_BALANCED_8',
+        create_time_stamp=datetime.datetime(2023, 7, 29, 13, 45, 23, 479000)
+    )
+]
+```
+
 ### Sleep
 
 Daily sleep quality
 
 ```python
 garth.DailySleep.list("2023-07-23", 2)
 ```
```

