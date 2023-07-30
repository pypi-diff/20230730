# Comparing `tmp/garth-0.3.1.tar.gz` & `tmp/garth-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garth-0.3.1.tar", last modified: Fri Jul 28 15:03:11 2023, max compression
+gzip compressed data, was "garth-0.3.2.tar", last modified: Sun Jul 30 00:46:26 2023, max compression
```

## Comparing `garth-0.3.1.tar` & `garth-0.3.2.tar`

### file list

```diff
@@ -1,42 +1,50 @@
--rw-r--r--   0        0        0     1071 2023-07-20 12:44:00.130760 garth-0.3.1/LICENSE
--rw-r--r--   0        0        0     9446 2023-07-28 15:02:39.347778 garth-0.3.1/README.md
--rw-r--r--   0        0        0      448 2023-07-28 02:46:53.365386 garth-0.3.1/garth/__init__.py
--rw-r--r--   0        0        0      931 2023-07-28 12:08:41.094670 garth-0.3.1/garth/auth_token.py
--rw-r--r--   0        0        0      145 2023-07-18 22:32:58.010661 garth-0.3.1/garth/exc.py
--rw-r--r--   0        0        0     4673 2023-07-28 12:13:51.131928 garth-0.3.1/garth/http.py
--rw-r--r--   0        0        0        0 2023-07-27 13:16:10.642595 garth-0.3.1/garth/py.typed
--rw-r--r--   0        0        0      157 2023-07-28 02:46:53.365687 garth-0.3.1/garth/resources/__init__.py
--rw-r--r--   0        0        0     3508 2023-07-28 12:23:42.498445 garth-0.3.1/garth/resources/sleep.py
--rw-r--r--   0        0        0      616 2023-07-27 13:31:20.421792 garth-0.3.1/garth/resources/stress.py
--rw-r--r--   0        0        0     3767 2023-07-28 12:13:50.747670 garth-0.3.1/garth/sso.py
--rw-r--r--   0        0        0     1610 2023-07-27 13:31:20.421985 garth-0.3.1/garth/stats.py
--rw-r--r--   0        0        0     1294 2023-07-28 02:46:53.372554 garth-0.3.1/garth/utils.py
--rw-r--r--   0        0        0       22 2023-07-28 15:02:55.210356 garth-0.3.1/garth/version.py
--rw-r--r--   0        0        0     1069 2023-07-28 15:03:11.356228 garth-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2386 2023-07-22 11:39:14.617674 garth-0.3.1/tests/cassettes/test_client_get.yaml
--rw-r--r--   0        0        0     2425 2023-07-22 11:39:14.746057 garth-0.3.1/tests/cassettes/test_client_post.yaml
--rw-r--r--   0        0        0   100962 2023-07-22 11:22:15.428262 garth-0.3.1/tests/cassettes/test_client_request.yaml
--rw-r--r--   0        0        0     2331 2023-07-28 03:35:21.644342 garth-0.3.1/tests/cassettes/test_connectapi.yaml
--rw-r--r--   0        0        0     4564 2023-07-28 03:35:21.644997 garth-0.3.1/tests/cassettes/test_connectapi_refresh.yaml
--rw-r--r--   0        0        0     3231 2023-07-28 03:35:21.645581 garth-0.3.1/tests/cassettes/test_exchange.yaml
--rw-r--r--   0        0        0    10962 2023-07-23 13:53:16.232082 garth-0.3.1/tests/cassettes/test_get_username.yaml
--rw-r--r--   0        0        0    50551 2023-07-22 15:27:42.274531 garth-0.3.1/tests/cassettes/test_login_email_password_fail.yaml
--rw-r--r--   0        0        0    91847 2023-07-23 13:50:32.012417 garth-0.3.1/tests/cassettes/test_login_success.yaml
--rw-r--r--   0        0        0     2270 2023-07-28 03:35:21.646057 garth-0.3.1/tests/cassettes/test_refresh.yaml
--rw-r--r--   0        0        0     2963 2023-07-28 03:35:21.646600 garth-0.3.1/tests/cassettes/test_refresh_expired.yaml
--rw-r--r--   0        0        0     3080 2023-07-28 12:57:32.501754 garth-0.3.1/tests/conftest.py
--rw-r--r--   0        0        0     3098 2023-07-28 03:35:40.317256 garth-0.3.1/tests/resources/cassettes/test_daily_sleep.yaml
--rw-r--r--   0        0        0     6252 2023-07-28 03:35:40.317752 garth-0.3.1/tests/resources/cassettes/test_daily_stress.yaml
--rw-r--r--   0        0        0    44427 2023-07-28 03:35:40.318411 garth-0.3.1/tests/resources/cassettes/test_daily_stress_pagination.yaml
--rw-r--r--   0        0        0     3652 2023-07-28 12:21:13.363000 garth-0.3.1/tests/resources/cassettes/test_sleep_data_get.yaml
--rw-r--r--   0        0        0    77468 2023-07-28 12:22:31.103002 garth-0.3.1/tests/resources/cassettes/test_sleep_data_list.yaml
--rw-r--r--   0        0        0     4717 2023-07-28 03:35:40.318832 garth-0.3.1/tests/resources/cassettes/test_weekly_stress.yaml
--rw-r--r--   0        0        0    16221 2023-07-28 03:35:40.319518 garth-0.3.1/tests/resources/cassettes/test_weekly_stress_beyond_data.yaml
--rw-r--r--   0        0        0     7522 2023-07-28 03:35:40.320026 garth-0.3.1/tests/resources/cassettes/test_weekly_stress_pagination.yaml
--rw-r--r--   0        0        0      849 2023-07-28 12:22:22.098284 garth-0.3.1/tests/resources/test_sleep.py
--rw-r--r--   0        0        0     1437 2023-07-27 13:31:20.424008 garth-0.3.1/tests/resources/test_stress.py
--rw-r--r--   0        0        0     1808 2023-07-23 13:40:52.098938 garth-0.3.1/tests/test_auth_token.py
--rw-r--r--   0        0        0     4097 2023-07-28 12:02:46.585315 garth-0.3.1/tests/test_http.py
--rw-r--r--   0        0        0     2570 2023-07-28 12:10:36.895963 garth-0.3.1/tests/test_sso.py
--rw-r--r--   0        0        0      531 2023-07-27 13:16:10.645234 garth-0.3.1/tests/test_utils.py
--rw-r--r--   0        0        0     9858 1970-01-01 00:00:00.000000 garth-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-20 12:44:00.130760 garth-0.3.2/LICENSE
+-rw-r--r--   0        0        0    12322 2023-07-29 23:44:50.244943 garth-0.3.2/README.md
+-rw-r--r--   0        0        0      653 2023-07-29 23:23:30.395971 garth-0.3.2/garth/__init__.py
+-rw-r--r--   0        0        0      931 2023-07-28 12:08:41.094670 garth-0.3.2/garth/auth_token.py
+-rw-r--r--   0        0        0      145 2023-07-18 22:32:58.010661 garth-0.3.2/garth/exc.py
+-rw-r--r--   0        0        0     4673 2023-07-28 12:13:51.131928 garth-0.3.2/garth/http.py
+-rw-r--r--   0        0        0        0 2023-07-27 13:16:10.642595 garth-0.3.2/garth/py.typed
+-rw-r--r--   0        0        0      392 2023-07-29 23:23:57.760715 garth-0.3.2/garth/resources/__init__.py
+-rw-r--r--   0        0        0      612 2023-07-29 23:28:46.923483 garth-0.3.2/garth/resources/intensity_minutes.py
+-rw-r--r--   0        0        0     3536 2023-07-29 23:32:07.004688 garth-0.3.2/garth/resources/sleep.py
+-rw-r--r--   0        0        0      654 2023-07-29 23:30:44.232250 garth-0.3.2/garth/resources/steps.py
+-rw-r--r--   0        0        0      653 2023-07-29 23:30:50.433149 garth-0.3.2/garth/resources/stress.py
+-rw-r--r--   0        0        0     3767 2023-07-28 12:13:50.747670 garth-0.3.2/garth/sso.py
+-rw-r--r--   0        0        0     1529 2023-07-29 23:29:30.202390 garth-0.3.2/garth/stats.py
+-rw-r--r--   0        0        0     1294 2023-07-28 02:46:53.372554 garth-0.3.2/garth/utils.py
+-rw-r--r--   0        0        0       22 2023-07-30 00:45:53.783018 garth-0.3.2/garth/version.py
+-rw-r--r--   0        0        0     1146 2023-07-30 00:46:26.427362 garth-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2386 2023-07-22 11:39:14.617674 garth-0.3.2/tests/cassettes/test_client_get.yaml
+-rw-r--r--   0        0        0     2425 2023-07-22 11:39:14.746057 garth-0.3.2/tests/cassettes/test_client_post.yaml
+-rw-r--r--   0        0        0   100962 2023-07-22 11:22:15.428262 garth-0.3.2/tests/cassettes/test_client_request.yaml
+-rw-r--r--   0        0        0     2331 2023-07-28 03:35:21.644342 garth-0.3.2/tests/cassettes/test_connectapi.yaml
+-rw-r--r--   0        0        0     4564 2023-07-28 03:35:21.644997 garth-0.3.2/tests/cassettes/test_connectapi_refresh.yaml
+-rw-r--r--   0        0        0     3231 2023-07-28 03:35:21.645581 garth-0.3.2/tests/cassettes/test_exchange.yaml
+-rw-r--r--   0        0        0    10962 2023-07-23 13:53:16.232082 garth-0.3.2/tests/cassettes/test_get_username.yaml
+-rw-r--r--   0        0        0    50551 2023-07-22 15:27:42.274531 garth-0.3.2/tests/cassettes/test_login_email_password_fail.yaml
+-rw-r--r--   0        0        0    91847 2023-07-23 13:50:32.012417 garth-0.3.2/tests/cassettes/test_login_success.yaml
+-rw-r--r--   0        0        0     2270 2023-07-28 03:35:21.646057 garth-0.3.2/tests/cassettes/test_refresh.yaml
+-rw-r--r--   0        0        0     2963 2023-07-28 03:35:21.646600 garth-0.3.2/tests/cassettes/test_refresh_expired.yaml
+-rw-r--r--   0        0        0     3080 2023-07-28 12:57:32.501754 garth-0.3.2/tests/conftest.py
+-rw-r--r--   0        0        0     4197 2023-07-29 23:34:06.394173 garth-0.3.2/tests/resources/cassettes/test_daily_intensity_minutes.yaml
+-rw-r--r--   0        0        0     3098 2023-07-28 03:35:40.317256 garth-0.3.2/tests/resources/cassettes/test_daily_sleep.yaml
+-rw-r--r--   0        0        0     4179 2023-07-29 17:52:20.398786 garth-0.3.2/tests/resources/cassettes/test_daily_steps.yaml
+-rw-r--r--   0        0        0     6252 2023-07-28 03:35:40.317752 garth-0.3.2/tests/resources/cassettes/test_daily_stress.yaml
+-rw-r--r--   0        0        0    44427 2023-07-28 03:35:40.318411 garth-0.3.2/tests/resources/cassettes/test_daily_stress_pagination.yaml
+-rw-r--r--   0        0        0     3652 2023-07-28 12:21:13.363000 garth-0.3.2/tests/resources/cassettes/test_sleep_data_get.yaml
+-rw-r--r--   0        0        0    77468 2023-07-28 12:22:31.103002 garth-0.3.2/tests/resources/cassettes/test_sleep_data_list.yaml
+-rw-r--r--   0        0        0     3349 2023-07-29 23:35:28.845204 garth-0.3.2/tests/resources/cassettes/test_weekly_intensity_minutes.yaml
+-rw-r--r--   0        0        0    13052 2023-07-29 17:52:45.776274 garth-0.3.2/tests/resources/cassettes/test_weekly_steps.yaml
+-rw-r--r--   0        0        0     4717 2023-07-28 03:35:40.318832 garth-0.3.2/tests/resources/cassettes/test_weekly_stress.yaml
+-rw-r--r--   0        0        0    16221 2023-07-28 03:35:40.319518 garth-0.3.2/tests/resources/cassettes/test_weekly_stress_beyond_data.yaml
+-rw-r--r--   0        0        0     7522 2023-07-28 03:35:40.320026 garth-0.3.2/tests/resources/cassettes/test_weekly_stress_pagination.yaml
+-rw-r--r--   0        0        0      748 2023-07-29 23:40:27.912636 garth-0.3.2/tests/resources/test_intensity_minutes.py
+-rw-r--r--   0        0        0      849 2023-07-28 12:22:22.098284 garth-0.3.2/tests/resources/test_sleep.py
+-rw-r--r--   0        0        0      667 2023-07-29 17:53:35.423973 garth-0.3.2/tests/resources/test_steps.py
+-rw-r--r--   0        0        0     1437 2023-07-27 13:31:20.424008 garth-0.3.2/tests/resources/test_stress.py
+-rw-r--r--   0        0        0     1808 2023-07-23 13:40:52.098938 garth-0.3.2/tests/test_auth_token.py
+-rw-r--r--   0        0        0     4097 2023-07-28 12:02:46.585315 garth-0.3.2/tests/test_http.py
+-rw-r--r--   0        0        0     2570 2023-07-28 12:10:36.895963 garth-0.3.2/tests/test_sso.py
+-rw-r--r--   0        0        0      531 2023-07-27 13:16:10.645234 garth-0.3.2/tests/test_utils.py
+-rw-r--r--   0        0        0    12734 1970-01-01 00:00:00.000000 garth-0.3.2/PKG-INFO
```

### Comparing `garth-0.3.1/LICENSE` & `garth-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `garth-0.3.1/README.md` & `garth-0.3.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,34 @@
 [![CI](https://github.com/matin/garth/workflows/CI/badge.svg?event=push)](https://github.com/matin/garth/actions?query=event%3Apush+branch%3Amain+workflow%3ACI)
 [![codecov](https://codecov.io/gh/matin/garth/branch/main/graph/badge.svg?token=0EFFYJNFIL)](https://codecov.io/gh/matin/garth)
 
 Garmin SSO auth + Connect client
 
 ## Google Colabs
 
-[Graph 28-day rolling average of daily stress](https://colab.research.google.com/github/matin/garth/blob/main/colabs/stress.ipynb)
+### [Stress: 28-day rolling average](https://colab.research.google.com/github/matin/garth/blob/main/colabs/stress.ipynb)
+
+Stress levels from one day to another can vary by extremes, but there's always
+a general trend. Using a scatter plot with a rolling average shows both the
+individual days and the trend. The Colab retrieves up to three years of daily
+data. If there's less than three years of data, it retrieves whatever is
+available.
+
+![Stress: Garph of 28-day rolling average](https://github.com/matin/garth/assets/98985/868ecf25-4644-4879-b28f-ed0706a9e7b9)
+
+### [Sleep stages over 90 days](https://colab.research.google.com/github/matin/garth/blob/main/colabs/sleep.ipynb)
+
+The Garmin Connect app only shows a maximum of seven days for sleep
+stages—making it hard to see trends. The Connect API supports retrieving
+daily sleep quality in 28-day pages, but that doesn't show details. Using
+`SleedData.list()` gives us the ability to retrieve an arbitrary number of
+day with enough detail to product a stacked bar graph of the daily sleep
+stages.
+
+![Sleep stages over 90 days](https://github.com/matin/garth/assets/98985/2e43d68e-b882-4a5e-839a-a1326ed7c61e)
 
 ## Background
 
 Garth is meant for personal use and follows the philosiphy that your data is
 your data. You should be able to download it and analyze it in the way that
 you'd like. In my case, that means processing with Google Colab, Pandas,
 Matplotlib, etc.
@@ -96,15 +115,15 @@
     garth.client.auth_token.refresh()
 except (GarthException, HTTPError):
     # Session is expired. You'll need to log in again
 ```
 
 ## Connect API
 
-### Wellness
+### Daily details
 
 ```python
 sleep = garth.connectapi(
     f"/wellness-service/wellness/dailySleepData/{garth.client.username}",
     params={"date": "2023-07-05", "nonSleepBufferMinutes": 60),
 )
 list(sleep.keys())
@@ -121,15 +140,15 @@
     "wellnessSpO2SleepSummaryDTO",
     "wellnessEpochSPO2DataDTOList",
     "wellnessEpochRespirationDataDTOList",
     "sleepStress"
 ]
 ```
 
-### Usersummary
+### Stats
 
 ```python
 stress =  garth.connectapi(f"/usersummary-service/stats/stress/weekly/2023-07-05/52")
 ```
 
 ```json
 {
@@ -184,14 +203,114 @@
 ```python
 [
     WeeklyStress(calendar_date=datetime.date(2023, 7, 10), value=33),
     WeeklyStress(calendar_date=datetime.date(2023, 7, 17), value=32)
 ]
 ```
 
+### Steps
+
+Daily steps
+
+```python
+garth.DailySteps.list(period=2)
+```
+
+```python
+[
+    DailySteps(
+        calendar_date=datetime.date(2023, 7, 28),
+        total_steps=6510,
+        total_distance=5552,
+        step_goal=8090
+    ),
+    DailySteps(
+        calendar_date=datetime.date(2023, 7, 29),
+        total_steps=7218,
+        total_distance=6002,
+        step_goal=7940
+    )
+]
+```
+
+Weekly steps
+
+```python
+garth.WeeklySteps.list(period=2)
+```
+
+```python
+[
+    WeeklySteps(
+        calendar_date=datetime.date(2023, 7, 16),
+        total_steps=42339,
+        average_steps=6048.428571428572,
+        average_distance=5039.285714285715,
+        total_distance=35275.0,
+        wellness_data_days_count=7
+    ),
+    WeeklySteps(
+        calendar_date=datetime.date(2023, 7, 23),
+        total_steps=56420,
+        average_steps=8060.0,
+        average_distance=7198.142857142857,
+        total_distance=50387.0,
+        wellness_data_days_count=7
+    )
+]
+```
+
+### Intensity Minutes
+
+Daily intensity minutes
+
+```python
+garth.DailyIntensityMinutes.list(period=2)
+```
+
+```python
+[
+    DailyIntensityMinutes(
+        calendar_date=datetime.date(2023, 7, 28),
+        weekly_goal=150,
+        moderate_value=0,
+        vigorous_value=0
+    ),
+    DailyIntensityMinutes(
+        calendar_date=datetime.date(2023, 7, 29),
+        weekly_goal=150,
+        moderate_value=0,
+        vigorous_value=0
+    )
+]
+```
+
+Weekly intensity minutes
+
+```python
+garth.WeeklyIntensityMinutes.list(period=2)
+```
+
+```python
+[
+    WeeklyIntensityMinutes(
+        calendar_date=datetime.date(2023, 7, 17),
+        weekly_goal=150,
+        moderate_value=103,
+        vigorous_value=9
+    ),
+    WeeklyIntensityMinutes(
+        calendar_date=datetime.date(2023, 7, 24),
+        weekly_goal=150,
+        moderate_value=101,
+        vigorous_value=105
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

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `garth-0.3.1/garth/auth_token.py` & `garth-0.3.2/garth/auth_token.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.1/garth/http.py` & `garth-0.3.2/garth/http.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.1/garth/resources/sleep.py` & `garth-0.3.2/garth/resources/sleep.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 from ..utils import camel_to_snake_dict, date_range, format_end_date
 
 
 @dataclass(frozen=True)
 class DailySleep(Stats):
     value: int
 
-    _path: ClassVar[str] = "/wellness-service/stats/daily/sleep/score"
+    _path: ClassVar[
+        str
+    ] = "/wellness-service/stats/daily/sleep/score/{start}/{end}"
     _page_size: ClassVar[int] = 28
 
 
 @dataclass(frozen=True)
 class Score:
     qualifier_key: str
     optimal_start: Optional[float] = None
```

### Comparing `garth-0.3.1/garth/resources/stress.py` & `garth-0.3.2/garth/resources/stress.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 class DailyStress(Stats):
     overall_stress_level: int
     rest_stress_duration: int | None
     low_stress_duration: int | None
     medium_stress_duration: int | None
     high_stress_duration: int | None
 
-    _path: ClassVar[str] = f"{BASE_PATH}/daily"
+    _path: ClassVar[str] = f"{BASE_PATH}/daily/{{start}}/{{end}}"
     _page_size: ClassVar[int] = 28
 
 
 @dataclass(frozen=True)
 class WeeklyStress(Stats):
     value: int
 
-    _path: ClassVar[str] = f"{BASE_PATH}/weekly"
+    _path: ClassVar[str] = f"{BASE_PATH}/weekly/{{end}}/{{period}}"
     _page_size: ClassVar[int] = 52
```

### Comparing `garth-0.3.1/garth/sso.py` & `garth-0.3.2/garth/sso.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.1/garth/stats.py` & `garth-0.3.2/garth/stats.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,17 +38,14 @@
                     period - cls._page_size,
                     client=client,
                 )
                 + page
             )
             return page
 
-        if period_type == "weeks":
-            path = f"{cls._path}/{end}/{period}"
-        else:
-            start = end - timedelta(**{period_type: period - 1})
-            path = f"{cls._path}/{start}/{end}"
+        start = end - timedelta(**{period_type: period - 1})
+        path = cls._path.format(start=start, end=end, period=period)
         page_dirs = client.connectapi(path)
         if page_dirs and "values" in page_dirs[0]:
             page_dirs = [stat | stat.pop("values") for stat in page_dirs]
         page_dirs = [camel_to_snake_dict(stat) for stat in page_dirs]
         return [cls(**stat) for stat in page_dirs]
```

### Comparing `garth-0.3.1/garth/utils.py` & `garth-0.3.2/garth/utils.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.1/pyproject.toml` & `garth-0.3.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -12,34 +12,39 @@
 requires-python = ">=3.10"
 readme = "README.md"
 classifiers = [
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
 ]
-version = "0.3.1"
+packages = [
+    { include = "garth" },
+]
+version = "0.3.2"
 
 [project.license]
 text = "MIT"
 
-[project.packages]
-include = [
-    { from = ".", include = "garth" },
-    { from = "garth", include = "py.typed" },
-]
-
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.pytest.ini_options]
 addopts = "--ignore=__pypackages__ --ignore-glob=*.yaml"
 
+[tool.isort]
+multi_line_output = 3
+include_trailing_comma = true
+force_grid_wrap = 0
+use_parentheses = true
+line_length = 79
+known_first_party = "garth"
+
 [tool.pdm.version]
 source = "file"
 path = "garth/version.py"
 
 [tool.pdm.dev-dependencies]
 dev = [
     "ipython",
```

### Comparing `garth-0.3.1/tests/cassettes/test_client_get.yaml` & `garth-0.3.2/tests/cassettes/test_client_get.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.1/tests/cassettes/test_client_post.yaml` & `garth-0.3.2/tests/cassettes/test_client_post.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.1/tests/cassettes/test_client_request.yaml` & `garth-0.3.2/tests/cassettes/test_client_request.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.1/tests/cassettes/test_connectapi.yaml` & `garth-0.3.2/tests/cassettes/test_connectapi.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.1/tests/cassettes/test_connectapi_refresh.yaml` & `garth-0.3.2/tests/cassettes/test_connectapi_refresh.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.1/tests/cassettes/test_exchange.yaml` & `garth-0.3.2/tests/cassettes/test_exchange.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.1/tests/cassettes/test_get_username.yaml` & `garth-0.3.2/tests/cassettes/test_get_username.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.1/tests/cassettes/test_login_email_password_fail.yaml` & `garth-0.3.2/tests/cassettes/test_login_email_password_fail.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.1/tests/cassettes/test_login_success.yaml` & `garth-0.3.2/tests/cassettes/test_login_success.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.1/tests/cassettes/test_refresh.yaml` & `garth-0.3.2/tests/cassettes/test_refresh.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.1/tests/cassettes/test_refresh_expired.yaml` & `garth-0.3.2/tests/cassettes/test_refresh_expired.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.1/tests/conftest.py` & `garth-0.3.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.1/tests/resources/cassettes/test_daily_sleep.yaml` & `garth-0.3.2/tests/resources/cassettes/test_daily_sleep.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.1/tests/resources/cassettes/test_daily_stress.yaml` & `garth-0.3.2/tests/resources/cassettes/test_daily_stress.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.1/tests/resources/cassettes/test_daily_stress_pagination.yaml` & `garth-0.3.2/tests/resources/cassettes/test_daily_stress_pagination.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.1/tests/resources/cassettes/test_sleep_data_get.yaml` & `garth-0.3.2/tests/resources/cassettes/test_sleep_data_get.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.1/tests/resources/cassettes/test_sleep_data_list.yaml` & `garth-0.3.2/tests/resources/cassettes/test_sleep_data_list.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.1/tests/resources/cassettes/test_weekly_stress.yaml` & `garth-0.3.2/tests/resources/cassettes/test_weekly_stress.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.1/tests/resources/cassettes/test_weekly_stress_beyond_data.yaml` & `garth-0.3.2/tests/resources/cassettes/test_weekly_stress_beyond_data.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.1/tests/resources/cassettes/test_weekly_stress_pagination.yaml` & `garth-0.3.2/tests/resources/cassettes/test_weekly_stress_pagination.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.1/tests/resources/test_sleep.py` & `garth-0.3.2/tests/resources/test_sleep.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.1/tests/resources/test_stress.py` & `garth-0.3.2/tests/resources/test_stress.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.1/tests/test_auth_token.py` & `garth-0.3.2/tests/test_auth_token.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.1/tests/test_http.py` & `garth-0.3.2/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.1/tests/test_sso.py` & `garth-0.3.2/tests/test_sso.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.1/tests/test_utils.py` & `garth-0.3.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.1/PKG-INFO` & `garth-0.3.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garth
-Version: 0.3.1
+Version: 0.3.2
 Summary: Garmin SSO auth + Connect client
 Author-Email: Matin Tamizi <mtamizi@duck.com>
 License: MIT
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
@@ -17,15 +17,34 @@
 [![CI](https://github.com/matin/garth/workflows/CI/badge.svg?event=push)](https://github.com/matin/garth/actions?query=event%3Apush+branch%3Amain+workflow%3ACI)
 [![codecov](https://codecov.io/gh/matin/garth/branch/main/graph/badge.svg?token=0EFFYJNFIL)](https://codecov.io/gh/matin/garth)
 
 Garmin SSO auth + Connect client
 
 ## Google Colabs
 
-[Graph 28-day rolling average of daily stress](https://colab.research.google.com/github/matin/garth/blob/main/colabs/stress.ipynb)
+### [Stress: 28-day rolling average](https://colab.research.google.com/github/matin/garth/blob/main/colabs/stress.ipynb)
+
+Stress levels from one day to another can vary by extremes, but there's always
+a general trend. Using a scatter plot with a rolling average shows both the
+individual days and the trend. The Colab retrieves up to three years of daily
+data. If there's less than three years of data, it retrieves whatever is
+available.
+
+![Stress: Garph of 28-day rolling average](https://github.com/matin/garth/assets/98985/868ecf25-4644-4879-b28f-ed0706a9e7b9)
+
+### [Sleep stages over 90 days](https://colab.research.google.com/github/matin/garth/blob/main/colabs/sleep.ipynb)
+
+The Garmin Connect app only shows a maximum of seven days for sleep
+stages—making it hard to see trends. The Connect API supports retrieving
+daily sleep quality in 28-day pages, but that doesn't show details. Using
+`SleedData.list()` gives us the ability to retrieve an arbitrary number of
+day with enough detail to product a stacked bar graph of the daily sleep
+stages.
+
+![Sleep stages over 90 days](https://github.com/matin/garth/assets/98985/2e43d68e-b882-4a5e-839a-a1326ed7c61e)
 
 ## Background
 
 Garth is meant for personal use and follows the philosiphy that your data is
 your data. You should be able to download it and analyze it in the way that
 you'd like. In my case, that means processing with Google Colab, Pandas,
 Matplotlib, etc.
@@ -110,15 +129,15 @@
     garth.client.auth_token.refresh()
 except (GarthException, HTTPError):
     # Session is expired. You'll need to log in again
 ```
 
 ## Connect API
 
-### Wellness
+### Daily details
 
 ```python
 sleep = garth.connectapi(
     f"/wellness-service/wellness/dailySleepData/{garth.client.username}",
     params={"date": "2023-07-05", "nonSleepBufferMinutes": 60),
 )
 list(sleep.keys())
@@ -135,15 +154,15 @@
     "wellnessSpO2SleepSummaryDTO",
     "wellnessEpochSPO2DataDTOList",
     "wellnessEpochRespirationDataDTOList",
     "sleepStress"
 ]
 ```
 
-### Usersummary
+### Stats
 
 ```python
 stress =  garth.connectapi(f"/usersummary-service/stats/stress/weekly/2023-07-05/52")
 ```
 
 ```json
 {
@@ -198,14 +217,114 @@
 ```python
 [
     WeeklyStress(calendar_date=datetime.date(2023, 7, 10), value=33),
     WeeklyStress(calendar_date=datetime.date(2023, 7, 17), value=32)
 ]
 ```
 
+### Steps
+
+Daily steps
+
+```python
+garth.DailySteps.list(period=2)
+```
+
+```python
+[
+    DailySteps(
+        calendar_date=datetime.date(2023, 7, 28),
+        total_steps=6510,
+        total_distance=5552,
+        step_goal=8090
+    ),
+    DailySteps(
+        calendar_date=datetime.date(2023, 7, 29),
+        total_steps=7218,
+        total_distance=6002,
+        step_goal=7940
+    )
+]
+```
+
+Weekly steps
+
+```python
+garth.WeeklySteps.list(period=2)
+```
+
+```python
+[
+    WeeklySteps(
+        calendar_date=datetime.date(2023, 7, 16),
+        total_steps=42339,
+        average_steps=6048.428571428572,
+        average_distance=5039.285714285715,
+        total_distance=35275.0,
+        wellness_data_days_count=7
+    ),
+    WeeklySteps(
+        calendar_date=datetime.date(2023, 7, 23),
+        total_steps=56420,
+        average_steps=8060.0,
+        average_distance=7198.142857142857,
+        total_distance=50387.0,
+        wellness_data_days_count=7
+    )
+]
+```
+
+### Intensity Minutes
+
+Daily intensity minutes
+
+```python
+garth.DailyIntensityMinutes.list(period=2)
+```
+
+```python
+[
+    DailyIntensityMinutes(
+        calendar_date=datetime.date(2023, 7, 28),
+        weekly_goal=150,
+        moderate_value=0,
+        vigorous_value=0
+    ),
+    DailyIntensityMinutes(
+        calendar_date=datetime.date(2023, 7, 29),
+        weekly_goal=150,
+        moderate_value=0,
+        vigorous_value=0
+    )
+]
+```
+
+Weekly intensity minutes
+
+```python
+garth.WeeklyIntensityMinutes.list(period=2)
+```
+
+```python
+[
+    WeeklyIntensityMinutes(
+        calendar_date=datetime.date(2023, 7, 17),
+        weekly_goal=150,
+        moderate_value=103,
+        vigorous_value=9
+    ),
+    WeeklyIntensityMinutes(
+        calendar_date=datetime.date(2023, 7, 24),
+        weekly_goal=150,
+        moderate_value=101,
+        vigorous_value=105
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

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

