# Comparing `tmp/seldom-3.2.2.tar.gz` & `tmp/seldom-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seldom-3.2.2.tar", last modified: Tue May  9 16:56:34 2023, max compression
+gzip compressed data, was "seldom-3.2.3.tar", last modified: Sun Jul 30 07:16:31 2023, max compression
```

## Comparing `seldom-3.2.2.tar` & `seldom-3.2.3.tar`

### file list

```diff
@@ -1,112 +1,113 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 16:56:34.050982 seldom-3.2.2/
--rw-rw-rw-   0        0        0    11565 2022-12-06 15:57:51.000000 seldom-3.2.2/LICENSE
--rw-rw-rw-   0        0        0       44 2022-12-06 15:57:51.000000 seldom-3.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1041 2023-05-09 16:56:34.049980 seldom-3.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     9716 2023-05-05 15:56:59.000000 seldom-3.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 16:56:33.936361 seldom-3.2.2/demo/
--rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.2/demo/__init__.py
--rw-rw-rw-   0        0        0     1164 2023-01-11 15:24:10.000000 seldom-3.2.2/demo/confrun.py
--rw-rw-rw-   0        0        0     1583 2022-12-06 15:57:51.000000 seldom-3.2.2/demo/run.py
-drwxrwxrwx   0        0        0        0 2023-05-09 16:56:33.937359 seldom-3.2.2/demo/test_dir/
--rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.2/demo/test_dir/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 16:56:33.939355 seldom-3.2.2/demo/test_dir/api_case/
--rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.2/demo/test_dir/api_case/__init__.py
--rw-rw-rw-   0        0        0     3713 2023-01-11 15:24:10.000000 seldom-3.2.2/demo/test_dir/api_case/test_http_demo.py
-drwxrwxrwx   0        0        0        0 2023-05-09 16:56:33.944366 seldom-3.2.2/demo/test_dir/app_case/
--rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.2/demo/test_dir/app_case/__init__.py
--rw-rw-rw-   0        0        0      994 2022-12-06 15:57:51.000000 seldom-3.2.2/demo/test_dir/app_case/test_first_demo.py
--rw-rw-rw-   0        0        0     1231 2023-03-19 02:35:00.000000 seldom-3.2.2/demo/test_dir/app_case/test_po_demo.py
--rw-rw-rw-   0        0        0      875 2023-03-14 15:43:32.000000 seldom-3.2.2/demo/test_dir/app_case/test_u2_demo.py
-drwxrwxrwx   0        0        0        0 2023-05-09 16:56:33.952991 seldom-3.2.2/demo/test_dir/web_case/
--rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.2/demo/test_dir/web_case/__init__.py
--rw-rw-rw-   0        0        0      579 2022-12-06 15:57:51.000000 seldom-3.2.2/demo/test_dir/web_case/test_data_demo.py
--rw-rw-rw-   0        0        0     4287 2023-01-11 15:24:10.000000 seldom-3.2.2/demo/test_dir/web_case/test_ddt_demo.py
--rw-rw-rw-   0        0        0      589 2023-01-11 15:24:10.000000 seldom-3.2.2/demo/test_dir/web_case/test_first_demo.py
--rw-rw-rw-   0        0        0      846 2022-12-06 15:57:51.000000 seldom-3.2.2/demo/test_dir/web_case/test_fixture_demo.py
--rw-rw-rw-   0        0        0      953 2023-01-11 15:24:10.000000 seldom-3.2.2/demo/test_dir/web_case/test_playwright_demo.py
--rw-rw-rw-   0        0        0     1194 2023-03-19 02:31:03.000000 seldom-3.2.2/demo/test_dir/web_case/test_po_demo.py
-drwxrwxrwx   0        0        0        0 2023-05-09 16:56:33.958995 seldom-3.2.2/proj/
--rw-rw-rw-   0        0        0        0 2022-12-08 16:29:03.000000 seldom-3.2.2/proj/__init__.py
--rw-rw-rw-   0        0        0      110 2022-12-12 15:41:44.000000 seldom-3.2.2/proj/confrun.py
--rw-rw-rw-   0        0        0     1031 2022-12-12 15:42:40.000000 seldom-3.2.2/proj/loader.py
--rw-rw-rw-   0        0        0      293 2022-12-12 15:41:28.000000 seldom-3.2.2/proj/run.py
-drwxrwxrwx   0        0        0        0 2023-05-09 16:56:33.969980 seldom-3.2.2/seldom/
--rw-rw-rw-   0        0        0     1305 2023-05-09 16:52:08.000000 seldom-3.2.2/seldom/__init__.py
--rw-rw-rw-   0        0        0     5373 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/appdriver.py
-drwxrwxrwx   0        0        0        0 2023-05-09 16:56:33.984991 seldom-3.2.2/seldom/appium_lab/
--rw-rw-rw-   0        0        0     1669 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/appium_lab/__init__.py
--rw-rw-rw-   0        0        0     3909 2023-03-13 16:12:23.000000 seldom-3.2.2/seldom/appium_lab/action.py
--rw-rw-rw-   0        0        0     7248 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/appium_lab/find.py
--rw-rw-rw-   0        0        0     2997 2023-03-13 16:12:23.000000 seldom-3.2.2/seldom/appium_lab/keyboard.py
--rw-rw-rw-   0        0        0     1721 2023-03-13 16:12:23.000000 seldom-3.2.2/seldom/appium_lab/switch.py
--rw-rw-rw-   0        0        0    11006 2023-03-13 16:12:38.000000 seldom-3.2.2/seldom/case.py
--rw-rw-rw-   0        0        0    13177 2022-12-16 17:09:13.000000 seldom-3.2.2/seldom/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-09 16:56:33.993015 seldom-3.2.2/seldom/db_operation/
--rw-rw-rw-   0        0        0       64 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/db_operation/__init__.py
--rw-rw-rw-   0        0        0     1698 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/db_operation/base_db.py
--rw-rw-rw-   0        0        0      715 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/db_operation/mongo_db.py
--rw-rw-rw-   0        0        0     4084 2023-05-04 15:57:05.000000 seldom-3.2.2/seldom/db_operation/mssql_db.py
--rw-rw-rw-   0        0        0     4329 2023-05-04 15:55:58.000000 seldom-3.2.2/seldom/db_operation/mysql_db.py
--rw-rw-rw-   0        0        0     3206 2023-05-04 15:54:53.000000 seldom-3.2.2/seldom/db_operation/sqlite_db.py
--rw-rw-rw-   0        0        0     5665 2023-03-14 15:43:32.000000 seldom-3.2.2/seldom/driver.py
-drwxrwxrwx   0        0        0        0 2023-05-09 16:56:33.996015 seldom-3.2.2/seldom/har2case/
--rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/har2case/__init__.py
--rw-rw-rw-   0        0        0     4014 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/har2case/core.py
--rw-rw-rw-   0        0        0     1171 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/har2case/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-09 16:56:33.999991 seldom-3.2.2/seldom/logging/
--rw-rw-rw-   0        0        0       48 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/logging/__init__.py
--rw-rw-rw-   0        0        0     1101 2023-01-02 07:33:41.000000 seldom-3.2.2/seldom/logging/exceptions.py
--rw-rw-rw-   0        0        0     1887 2023-03-16 00:03:22.000000 seldom-3.2.2/seldom/logging/log.py
--rw-rw-rw-   0        0        0    11842 2023-03-19 02:45:19.000000 seldom-3.2.2/seldom/request.py
-drwxrwxrwx   0        0        0        0 2023-05-09 16:56:34.010991 seldom-3.2.2/seldom/running/
--rw-rw-rw-   0        0        0     2477 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/running/DebugTestRunner.py
--rw-rw-rw-   0        0        0      803 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/running/__init__.py
--rw-rw-rw-   0        0        0      561 2023-03-14 15:43:32.000000 seldom-3.2.2/seldom/running/config.py
--rw-rw-rw-   0        0        0     1467 2022-12-07 17:25:01.000000 seldom-3.2.2/seldom/running/loader.py
--rw-rw-rw-   0        0        0     7450 2022-12-15 14:14:22.000000 seldom-3.2.2/seldom/running/loader_extend.py
--rw-rw-rw-   0        0        0     1006 2022-12-12 16:47:54.000000 seldom-3.2.2/seldom/running/loader_hook.py
--rw-rw-rw-   0        0        0    14707 2023-05-09 15:45:14.000000 seldom-3.2.2/seldom/running/runner.py
--rw-rw-rw-   0        0        0     3119 2023-05-09 15:45:14.000000 seldom-3.2.2/seldom/skip.py
-drwxrwxrwx   0        0        0        0 2023-05-09 16:56:34.016991 seldom-3.2.2/seldom/testdata/
--rw-rw-rw-   0        0        0       28 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/testdata/__init__.py
--rw-rw-rw-   0        0        0     4164 2023-03-13 16:12:23.000000 seldom-3.2.2/seldom/testdata/conversion.py
--rw-rw-rw-   0        0        0    10749 2023-04-03 16:11:58.000000 seldom-3.2.2/seldom/testdata/parameterization.py
--rw-rw-rw-   0        0        0    18847 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/testdata/random_data.py
--rw-rw-rw-   0        0        0    11986 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/testdata/random_func.py
-drwxrwxrwx   0        0        0        0 2023-05-09 16:56:34.034003 seldom-3.2.2/seldom/utils/
--rw-rw-rw-   0        0        0      263 2023-05-09 15:45:14.000000 seldom-3.2.2/seldom/utils/__init__.py
--rw-rw-rw-   0        0        0     5564 2023-04-01 06:05:16.000000 seldom-3.2.2/seldom/utils/cache.py
--rw-rw-rw-   0        0        0     1067 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/utils/curlify.py
--rw-rw-rw-   0        0        0     2395 2023-03-13 16:12:38.000000 seldom-3.2.2/seldom/utils/diff.py
--rw-rw-rw-   0        0        0     3280 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/utils/file_extend.py
--rw-rw-rw-   0        0        0      438 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/utils/genson.py
--rw-rw-rw-   0        0        0      243 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/utils/jmespath.py
--rw-rw-rw-   0        0        0    10473 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/utils/jsonpath.py
--rw-rw-rw-   0        0        0     3964 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/utils/klook.py
--rw-rw-rw-   0        0        0     1500 2023-03-13 16:12:23.000000 seldom-3.2.2/seldom/utils/send_extend.py
--rw-rw-rw-   0        0        0     1577 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/utils/thread_lab.py
--rw-rw-rw-   0        0        0     1599 2023-05-09 15:45:14.000000 seldom-3.2.2/seldom/utils/tomorrow.py
--rw-rw-rw-   0        0        0     1543 2022-12-06 15:42:11.000000 seldom-3.2.2/seldom/utils/webdriver_manager_extend.py
--rw-rw-rw-   0        0        0    32336 2023-05-09 15:45:14.000000 seldom-3.2.2/seldom/webdriver.py
--rw-rw-rw-   0        0        0    10549 2022-12-06 15:57:51.000000 seldom-3.2.2/seldom/webdriver_chaining.py
-drwxrwxrwx   0        0        0        0 2023-05-09 16:56:33.978991 seldom-3.2.2/seldom.egg-info/
--rw-rw-rw-   0        0        0     1041 2023-05-09 16:56:33.000000 seldom-3.2.2/seldom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2465 2023-05-09 16:56:33.000000 seldom-3.2.2/seldom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 16:56:33.000000 seldom-3.2.2/seldom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-05-09 16:56:33.000000 seldom-3.2.2/seldom.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-09 16:56:22.000000 seldom-3.2.2/seldom.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      252 2023-05-09 16:56:33.000000 seldom-3.2.2/seldom.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-09 16:56:33.000000 seldom-3.2.2/seldom.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 16:56:34.050982 seldom-3.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1904 2023-05-05 16:01:28.000000 seldom-3.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-09 16:56:34.048991 seldom-3.2.2/test/
--rw-rw-rw-   0        0        0      594 2022-12-06 15:57:51.000000 seldom-3.2.2/test/test_cache.py
--rw-rw-rw-   0        0        0     8814 2023-04-13 16:38:59.000000 seldom-3.2.2/test/test_db_operation.py
--rw-rw-rw-   0        0        0      691 2022-12-06 15:57:51.000000 seldom-3.2.2/test/test_klook.py
--rw-rw-rw-   0        0        0     1062 2022-12-06 15:57:51.000000 seldom-3.2.2/test/test_log.py
--rw-rw-rw-   0        0        0      761 2023-04-01 06:05:16.000000 seldom-3.2.2/test/test_memory_cache.py
--rw-rw-rw-   0        0        0     2204 2022-12-06 15:57:51.000000 seldom-3.2.2/test/test_testdata.py
--rw-rw-rw-   0        0        0     1601 2023-05-09 15:45:14.000000 seldom-3.2.2/test/test_thread.py
--rw-rw-rw-   0        0        0      999 2022-12-06 15:57:51.000000 seldom-3.2.2/test/test_thread2.py
--rw-rw-rw-   0        0        0      776 2023-05-09 16:33:27.000000 seldom-3.2.2/test/test_thread_case.py
--rw-rw-rw-   0        0        0      520 2023-05-09 16:38:11.000000 seldom-3.2.2/test/test_thread_path.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:16:31.180286 seldom-3.2.3/
+-rw-rw-rw-   0        0        0    11565 2022-12-06 15:57:51.000000 seldom-3.2.3/LICENSE
+-rw-rw-rw-   0        0        0       44 2022-12-06 15:57:51.000000 seldom-3.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1048 2023-07-30 07:16:31.180286 seldom-3.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     9716 2023-05-10 17:08:36.000000 seldom-3.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 07:16:31.068817 seldom-3.2.3/demo/
+-rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.3/demo/__init__.py
+-rw-rw-rw-   0        0        0     1164 2023-01-11 15:24:10.000000 seldom-3.2.3/demo/confrun.py
+-rw-rw-rw-   0        0        0     1583 2022-12-06 15:57:51.000000 seldom-3.2.3/demo/run.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:16:31.069805 seldom-3.2.3/demo/test_dir/
+-rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.3/demo/test_dir/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:16:31.071817 seldom-3.2.3/demo/test_dir/api_case/
+-rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.3/demo/test_dir/api_case/__init__.py
+-rw-rw-rw-   0        0        0     3743 2023-05-10 16:55:57.000000 seldom-3.2.3/demo/test_dir/api_case/test_http_demo.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:16:31.077818 seldom-3.2.3/demo/test_dir/app_case/
+-rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.3/demo/test_dir/app_case/__init__.py
+-rw-rw-rw-   0        0        0      994 2022-12-06 15:57:51.000000 seldom-3.2.3/demo/test_dir/app_case/test_first_demo.py
+-rw-rw-rw-   0        0        0     1231 2023-03-19 02:35:00.000000 seldom-3.2.3/demo/test_dir/app_case/test_po_demo.py
+-rw-rw-rw-   0        0        0      875 2023-03-14 15:43:32.000000 seldom-3.2.3/demo/test_dir/app_case/test_u2_demo.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:16:31.085254 seldom-3.2.3/demo/test_dir/web_case/
+-rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.3/demo/test_dir/web_case/__init__.py
+-rw-rw-rw-   0        0        0      579 2022-12-06 15:57:51.000000 seldom-3.2.3/demo/test_dir/web_case/test_data_demo.py
+-rw-rw-rw-   0        0        0     4287 2023-01-11 15:24:10.000000 seldom-3.2.3/demo/test_dir/web_case/test_ddt_demo.py
+-rw-rw-rw-   0        0        0      589 2023-01-11 15:24:10.000000 seldom-3.2.3/demo/test_dir/web_case/test_first_demo.py
+-rw-rw-rw-   0        0        0      846 2022-12-06 15:57:51.000000 seldom-3.2.3/demo/test_dir/web_case/test_fixture_demo.py
+-rw-rw-rw-   0        0        0      953 2023-01-11 15:24:10.000000 seldom-3.2.3/demo/test_dir/web_case/test_playwright_demo.py
+-rw-rw-rw-   0        0        0     1194 2023-03-19 02:31:03.000000 seldom-3.2.3/demo/test_dir/web_case/test_po_demo.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:16:31.090252 seldom-3.2.3/proj/
+-rw-rw-rw-   0        0        0        0 2022-12-08 16:29:03.000000 seldom-3.2.3/proj/__init__.py
+-rw-rw-rw-   0        0        0      110 2022-12-12 15:41:44.000000 seldom-3.2.3/proj/confrun.py
+-rw-rw-rw-   0        0        0     1031 2022-12-12 15:42:40.000000 seldom-3.2.3/proj/loader.py
+-rw-rw-rw-   0        0        0      293 2022-12-12 15:41:28.000000 seldom-3.2.3/proj/run.py
+-rw-rw-rw-   0        0        0     1557 2023-07-30 07:11:47.000000 seldom-3.2.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-30 07:16:31.101254 seldom-3.2.3/seldom/
+-rw-rw-rw-   0        0        0     1305 2023-07-30 07:11:36.000000 seldom-3.2.3/seldom/__init__.py
+-rw-rw-rw-   0        0        0     5373 2022-12-06 15:57:51.000000 seldom-3.2.3/seldom/appdriver.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:16:31.115841 seldom-3.2.3/seldom/appium_lab/
+-rw-rw-rw-   0        0        0     1669 2022-12-06 15:57:51.000000 seldom-3.2.3/seldom/appium_lab/__init__.py
+-rw-rw-rw-   0        0        0     3909 2023-03-13 16:12:23.000000 seldom-3.2.3/seldom/appium_lab/action.py
+-rw-rw-rw-   0        0        0     7248 2022-12-06 15:57:51.000000 seldom-3.2.3/seldom/appium_lab/find.py
+-rw-rw-rw-   0        0        0     2996 2023-06-12 15:02:43.000000 seldom-3.2.3/seldom/appium_lab/keyboard.py
+-rw-rw-rw-   0        0        0     1721 2023-03-13 16:12:23.000000 seldom-3.2.3/seldom/appium_lab/switch.py
+-rw-rw-rw-   0        0        0    11144 2023-05-28 08:23:47.000000 seldom-3.2.3/seldom/case.py
+-rw-rw-rw-   0        0        0    13177 2022-12-16 17:09:13.000000 seldom-3.2.3/seldom/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:16:31.124827 seldom-3.2.3/seldom/db_operation/
+-rw-rw-rw-   0        0        0       64 2022-12-06 15:57:51.000000 seldom-3.2.3/seldom/db_operation/__init__.py
+-rw-rw-rw-   0        0        0     1698 2022-12-06 15:57:51.000000 seldom-3.2.3/seldom/db_operation/base_db.py
+-rw-rw-rw-   0        0        0      715 2022-12-06 15:57:51.000000 seldom-3.2.3/seldom/db_operation/mongo_db.py
+-rw-rw-rw-   0        0        0     4084 2023-05-04 15:57:05.000000 seldom-3.2.3/seldom/db_operation/mssql_db.py
+-rw-rw-rw-   0        0        0     4329 2023-05-04 15:55:58.000000 seldom-3.2.3/seldom/db_operation/mysql_db.py
+-rw-rw-rw-   0        0        0     3206 2023-05-04 15:54:53.000000 seldom-3.2.3/seldom/db_operation/sqlite_db.py
+-rw-rw-rw-   0        0        0     5619 2023-07-24 15:30:19.000000 seldom-3.2.3/seldom/driver.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:16:31.129543 seldom-3.2.3/seldom/har2case/
+-rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.3/seldom/har2case/__init__.py
+-rw-rw-rw-   0        0        0     4014 2022-12-06 15:57:51.000000 seldom-3.2.3/seldom/har2case/core.py
+-rw-rw-rw-   0        0        0     1171 2022-12-06 15:57:51.000000 seldom-3.2.3/seldom/har2case/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:16:31.132595 seldom-3.2.3/seldom/logging/
+-rw-rw-rw-   0        0        0       48 2022-12-06 15:57:51.000000 seldom-3.2.3/seldom/logging/__init__.py
+-rw-rw-rw-   0        0        0     1101 2023-01-02 07:33:41.000000 seldom-3.2.3/seldom/logging/exceptions.py
+-rw-rw-rw-   0        0        0     2018 2023-07-16 13:48:12.000000 seldom-3.2.3/seldom/logging/log.py
+-rw-rw-rw-   0        0        0    12738 2023-07-30 03:45:42.000000 seldom-3.2.3/seldom/request.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:16:31.141618 seldom-3.2.3/seldom/running/
+-rw-rw-rw-   0        0        0     2846 2023-05-10 16:59:39.000000 seldom-3.2.3/seldom/running/DebugTestRunner.py
+-rw-rw-rw-   0        0        0      803 2022-12-06 15:57:51.000000 seldom-3.2.3/seldom/running/__init__.py
+-rw-rw-rw-   0        0        0      561 2023-03-14 15:43:32.000000 seldom-3.2.3/seldom/running/config.py
+-rw-rw-rw-   0        0        0     1467 2022-12-07 17:25:01.000000 seldom-3.2.3/seldom/running/loader.py
+-rw-rw-rw-   0        0        0     7450 2022-12-15 14:14:22.000000 seldom-3.2.3/seldom/running/loader_extend.py
+-rw-rw-rw-   0        0        0     1038 2023-07-16 13:48:12.000000 seldom-3.2.3/seldom/running/loader_hook.py
+-rw-rw-rw-   0        0        0    14717 2023-05-28 08:23:47.000000 seldom-3.2.3/seldom/running/runner.py
+-rw-rw-rw-   0        0        0     3119 2023-05-09 15:45:14.000000 seldom-3.2.3/seldom/skip.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:16:31.147883 seldom-3.2.3/seldom/testdata/
+-rw-rw-rw-   0        0        0       28 2022-12-06 15:57:51.000000 seldom-3.2.3/seldom/testdata/__init__.py
+-rw-rw-rw-   0        0        0     4164 2023-03-13 16:12:23.000000 seldom-3.2.3/seldom/testdata/conversion.py
+-rw-rw-rw-   0        0        0    10747 2023-06-07 06:47:26.000000 seldom-3.2.3/seldom/testdata/parameterization.py
+-rw-rw-rw-   0        0        0    18847 2022-12-06 15:57:51.000000 seldom-3.2.3/seldom/testdata/random_data.py
+-rw-rw-rw-   0        0        0    11986 2022-12-06 15:57:51.000000 seldom-3.2.3/seldom/testdata/random_func.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:16:31.166399 seldom-3.2.3/seldom/utils/
+-rw-rw-rw-   0        0        0      263 2023-05-09 15:45:14.000000 seldom-3.2.3/seldom/utils/__init__.py
+-rw-rw-rw-   0        0        0     5564 2023-04-01 06:05:16.000000 seldom-3.2.3/seldom/utils/cache.py
+-rw-rw-rw-   0        0        0     1067 2022-12-06 15:57:51.000000 seldom-3.2.3/seldom/utils/curlify.py
+-rw-rw-rw-   0        0        0     2395 2023-03-13 16:12:38.000000 seldom-3.2.3/seldom/utils/diff.py
+-rw-rw-rw-   0        0        0     3280 2022-12-06 15:57:51.000000 seldom-3.2.3/seldom/utils/file_extend.py
+-rw-rw-rw-   0        0        0      438 2022-12-06 15:57:51.000000 seldom-3.2.3/seldom/utils/genson.py
+-rw-rw-rw-   0        0        0      243 2022-12-06 15:57:51.000000 seldom-3.2.3/seldom/utils/jmespath.py
+-rw-rw-rw-   0        0        0    10473 2022-12-06 15:57:51.000000 seldom-3.2.3/seldom/utils/jsonpath.py
+-rw-rw-rw-   0        0        0     3964 2022-12-06 15:57:51.000000 seldom-3.2.3/seldom/utils/klook.py
+-rw-rw-rw-   0        0        0     1500 2023-03-13 16:12:23.000000 seldom-3.2.3/seldom/utils/send_extend.py
+-rw-rw-rw-   0        0        0     1577 2022-12-06 15:57:51.000000 seldom-3.2.3/seldom/utils/thread_lab.py
+-rw-rw-rw-   0        0        0     1599 2023-05-09 15:45:14.000000 seldom-3.2.3/seldom/utils/tomorrow.py
+-rw-rw-rw-   0        0        0     2066 2023-07-30 03:09:02.000000 seldom-3.2.3/seldom/utils/webdriver_manager_extend.py
+-rw-rw-rw-   0        0        0    32060 2023-05-28 08:23:47.000000 seldom-3.2.3/seldom/webdriver.py
+-rw-rw-rw-   0        0        0    10549 2022-12-06 15:57:51.000000 seldom-3.2.3/seldom/webdriver_chaining.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:16:31.110254 seldom-3.2.3/seldom.egg-info/
+-rw-rw-rw-   0        0        0     1048 2023-07-30 07:16:30.000000 seldom-3.2.3/seldom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2480 2023-07-30 07:16:30.000000 seldom-3.2.3/seldom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 07:16:30.000000 seldom-3.2.3/seldom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-07-30 07:16:30.000000 seldom-3.2.3/seldom.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-09 16:56:22.000000 seldom-3.2.3/seldom.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      254 2023-07-30 07:16:30.000000 seldom-3.2.3/seldom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-30 07:16:30.000000 seldom-3.2.3/seldom.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 07:16:31.181285 seldom-3.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1913 2023-07-30 03:01:13.000000 seldom-3.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 07:16:31.179285 seldom-3.2.3/test/
+-rw-rw-rw-   0        0        0      594 2022-12-06 15:57:51.000000 seldom-3.2.3/test/test_cache.py
+-rw-rw-rw-   0        0        0     8814 2023-04-13 16:38:59.000000 seldom-3.2.3/test/test_db_operation.py
+-rw-rw-rw-   0        0        0      691 2022-12-06 15:57:51.000000 seldom-3.2.3/test/test_klook.py
+-rw-rw-rw-   0        0        0     1062 2022-12-06 15:57:51.000000 seldom-3.2.3/test/test_log.py
+-rw-rw-rw-   0        0        0      761 2023-04-01 06:05:16.000000 seldom-3.2.3/test/test_memory_cache.py
+-rw-rw-rw-   0        0        0     2204 2022-12-06 15:57:51.000000 seldom-3.2.3/test/test_testdata.py
+-rw-rw-rw-   0        0        0     1601 2023-05-09 15:45:14.000000 seldom-3.2.3/test/test_thread.py
+-rw-rw-rw-   0        0        0      999 2022-12-06 15:57:51.000000 seldom-3.2.3/test/test_thread2.py
+-rw-rw-rw-   0        0        0      776 2023-05-09 16:33:27.000000 seldom-3.2.3/test/test_thread_case.py
+-rw-rw-rw-   0        0        0      520 2023-05-09 16:38:11.000000 seldom-3.2.3/test/test_thread_path.py
```

### Comparing `seldom-3.2.2/LICENSE` & `seldom-3.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/PKG-INFO` & `seldom-3.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: seldom
-Version: 3.2.2
+Version: 3.2.3
 Summary: Seldom automation testing framework based on unittest.
 Home-page: https://github.com/seldomQA/seldom/
 Author: bugmaster
 Author-email: fnngj@126.com
-License: BSD
+License: Apache-2.0
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `seldom-3.2.2/README.md` & `seldom-3.2.3/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -280,28 +280,28 @@
 
 https://github.com/SeldomQA/seldom-web-testing
 
 基于seldom的接口自动化项目:
 
 https://github.com/defnngj/seldom-api-testing
 
+### Star History
+
+![Star History Chart](https://api.star-history.com/svg?repos=SeldomQA/seldom&type=Date)
+
 ### 感谢
 
 感谢从以下项目中得到思路和帮助。
 
 * [HTMLTestRunner_cn](https://github.com/GoverSky/HTMLTestRunner_cn)
 
 * [parameterized](https://github.com/wolever/parameterized)
 
 * [utx](https://github.com/jianbing/utx)
 
-### Star History
-
-![Star History Chart](https://api.star-history.com/svg?repos=SeldomQA/seldom&type=Date)
-
 ### 交流
 
 QQ群：948994709
 
 
 ## 🔥 company
```

### Comparing `seldom-3.2.2/demo/confrun.py` & `seldom-3.2.3/demo/confrun.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/demo/run.py` & `seldom-3.2.3/demo/run.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/demo/test_dir/api_case/test_http_demo.py` & `seldom-3.2.3/demo/test_dir/api_case/test_http_demo.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         self.assertStatusCode(200)
 
     def test_get_method(self):
         """
         test get request
         """
         payload = {'key1': 'value1', 'key2': 'value2'}
-        self.get("/get", params=payload)
+        self.get("/get", params= {'key1': 'value1', 'key2': 'value2'})
         self.assertStatusCode(200)
 
     def test_delete_method(self):
         """
         test delete request
         """
         self.delete('/delete')
```

### Comparing `seldom-3.2.2/demo/test_dir/app_case/test_first_demo.py` & `seldom-3.2.3/demo/test_dir/app_case/test_first_demo.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/demo/test_dir/app_case/test_po_demo.py` & `seldom-3.2.3/demo/test_dir/app_case/test_po_demo.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/demo/test_dir/app_case/test_u2_demo.py` & `seldom-3.2.3/demo/test_dir/app_case/test_u2_demo.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/demo/test_dir/web_case/test_data_demo.py` & `seldom-3.2.3/demo/test_dir/web_case/test_data_demo.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/demo/test_dir/web_case/test_ddt_demo.py` & `seldom-3.2.3/demo/test_dir/web_case/test_ddt_demo.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/demo/test_dir/web_case/test_first_demo.py` & `seldom-3.2.3/demo/test_dir/web_case/test_first_demo.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/demo/test_dir/web_case/test_fixture_demo.py` & `seldom-3.2.3/demo/test_dir/web_case/test_fixture_demo.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/demo/test_dir/web_case/test_playwright_demo.py` & `seldom-3.2.3/demo/test_dir/web_case/test_playwright_demo.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/demo/test_dir/web_case/test_po_demo.py` & `seldom-3.2.3/demo/test_dir/web_case/test_po_demo.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/proj/loader.py` & `seldom-3.2.3/proj/loader.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/seldom/__init__.py` & `seldom-3.2.3/seldom/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,10 +27,10 @@
 from .skip import *
 from .driver import *
 from .testdata.parameterization import *
 
 
 __author__ = "bugmaster"
 
-__version__ = "3.2.2"
+__version__ = "3.2.3"
 
 __description__ = "WebUI/HTTP automation testing framework based on unittest."
```

### Comparing `seldom-3.2.2/seldom/appdriver.py` & `seldom-3.2.3/seldom/appdriver.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/seldom/appium_lab/__init__.py` & `seldom-3.2.3/seldom/appium_lab/__init__.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/seldom/appium_lab/action.py` & `seldom-3.2.3/seldom/appium_lab/action.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/seldom/appium_lab/find.py` & `seldom-3.2.3/seldom/appium_lab/find.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/seldom/appium_lab/keyboard.py` & `seldom-3.2.3/seldom/appium_lab/keyboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,28 +37,28 @@
     'T': 48,
     'U': 49,
     'V': 50,
     'W': 51,
     'X': 52,
     'Y': 53,
     'Z': 54,
+    ',': 55,
+    '.': 56,
     ' ': 62,
     '*': 17,
     '#': 18,
-    ',': 55,
     '`': 68,
     '-': 69,
     '[': 71,
     ']': 72,
     '\\': 73,
     ';': 74,
     '/': 76,
     '@': 77,
     '=': 161,
-    '.': 158,
     '+': 157,
     'NUM_LOCK': 143,
     'CAPS_LOCK': 115,
     'HOME': 4,
     'BACK': 3,
 }
```

### Comparing `seldom-3.2.2/seldom/appium_lab/switch.py` & `seldom-3.2.3/seldom/appium_lab/switch.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/seldom/case.py` & `seldom-3.2.3/seldom/case.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,17 +63,24 @@
     def tearDown(self):
         self.end()
         # close appium
         if (Seldom.app_server is not None) and (Seldom.app_info is not None):
             Seldom.driver.quit()
 
     @property
+    def base_url(self):
+        """
+        return base url (http)
+        """
+        return Seldom.base_url
+
+    @property
     def driver(self):
         """
-        return browser driver
+        return browser driver (web)
         """
         return Seldom.driver
 
     @staticmethod
     def browser(name: str):
         """
         launch browser
```

### Comparing `seldom-3.2.2/seldom/cli.py` & `seldom-3.2.3/seldom/cli.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/seldom/db_operation/base_db.py` & `seldom-3.2.3/seldom/db_operation/base_db.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/seldom/db_operation/mongo_db.py` & `seldom-3.2.3/seldom/db_operation/mongo_db.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/seldom/db_operation/mssql_db.py` & `seldom-3.2.3/seldom/db_operation/mssql_db.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/seldom/db_operation/mysql_db.py` & `seldom-3.2.3/seldom/db_operation/mysql_db.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/seldom/db_operation/sqlite_db.py` & `seldom-3.2.3/seldom/db_operation/sqlite_db.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/seldom/driver.py` & `seldom-3.2.3/seldom/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 browser driver
 """
 from selenium import webdriver
-from selenium.webdriver import ChromeOptions
 from selenium.webdriver.common.desired_capabilities import DesiredCapabilities
 from selenium.webdriver.firefox.service import Service as fService
 from selenium.webdriver.ie.service import Service as iService
 from selenium.webdriver.edge.service import Service as eService
 from selenium.webdriver.chrome.service import Service as cService
 from webdriver_manager.firefox import GeckoDriverManager
 from webdriver_manager.microsoft import IEDriverManager
```

### Comparing `seldom-3.2.2/seldom/har2case/core.py` & `seldom-3.2.3/seldom/har2case/core.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/seldom/har2case/utils.py` & `seldom-3.2.3/seldom/har2case/utils.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/seldom/logging/exceptions.py` & `seldom-3.2.3/seldom/logging/exceptions.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/seldom/logging/log.py` & `seldom-3.2.3/seldom/logging/log.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,29 +11,34 @@
 stack_t = inspect.stack()
 ins = inspect.getframeinfo(stack_t[1][0])
 exec_dir = os.path.dirname(os.path.abspath(ins.filename))
 report_dir = os.path.join(exec_dir, "reports")
 if os.path.exists(report_dir) is False:
     os.mkdir(report_dir)
 
-now_time = time.strftime("%Y_%m_%d_%H_%M_%S")
+
+with open(os.path.join(report_dir, "seldom_log.log"), "w") as log:
+    log.truncate(0)
+
 if BrowserConfig.LOG_PATH is None:
     BrowserConfig.LOG_PATH = os.path.join(report_dir, "seldom_log.log")
+
 if BrowserConfig.REPORT_PATH is None:
+    now_time = time.strftime("%Y_%m_%d_%H_%M_%S")
     BrowserConfig.REPORT_PATH = os.path.join(report_dir, now_time + "_result.html")
 
 
 class LogConfig:
     """log config"""
 
     def __init__(self, level: str = "DEBUG", colorlog: bool = True):
         self.logger = logger
         self._colorlog = colorlog
-        self._console_format = "<green>{time:YYYY-MM-DD HH:mm:ss}</> {file} <level>| {level} | {message}</level>"
-        self._log_format = "{time: YYYY-MM-DD HH:mm:ss} {file} | {level} | {message}"
+        self._console_format = "<green>{time:YYYY-MM-DD HH:mm:ss}</> <level>| {level: <8} | {file} | {message}</level>"
+        self._log_format = "{time: YYYY-MM-DD HH:mm:ss} | <level>{level: <8}</level> | {file: <10} | {message}"
         self._level = level
         self.logfile = BrowserConfig.LOG_PATH
         self.set_level(self._colorlog, self._console_format, self._level)
 
     def set_level(self, colorlog: bool = True, format: str = None, level: str = "DEBUG"):
         """
         setting level
```

### Comparing `seldom-3.2.2/seldom/request.py` & `seldom-3.2.3/seldom/request.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,23 +2,30 @@
 seldom requests
 """
 import ast
 import json
 from typing import Any
 import requests
 from seldom.running.config import Seldom
+from seldom.running.loader_hook import loader
 from seldom.logging import log
 from seldom.utils import jsonpath as utils_jsonpath
 from seldom.utils import jmespath as utils_jmespath
 from seldom.utils.curlify import to_curl
 
 
 IMG = ["jpg", "jpeg", "gif", "bmp", "webp"]
 
 
+class ResponseResult:
+    status_code = 200
+    response = None
+    request = None
+
+
 def formatting(msg):
     """formatted message"""
     if isinstance(msg, dict):
         return json.dumps(msg, indent=2, ensure_ascii=False)
     return msg
 
 
@@ -36,32 +43,35 @@
 
         img_file = False
         file_type = url.split(".")[-1]
         if file_type in IMG:
             img_file = True
 
         log.info(f"[method]: {func_name.upper()}      [url]: {url} ")
-        auth = kwargs.get("auth", "")
-        headers = kwargs.get("headers", "")
-        cookies = kwargs.get("cookies", "")
-        params = kwargs.get("params", "")
-        data = kwargs.get("data", "")
-        json_ = kwargs.get("json", "")
-        if auth != "":
-            log.debug(f"[auth]:\n {auth}")
-        if headers != "":
-            log.debug(f"[headers]:\n {formatting(headers)}")
-        if cookies != "":
-            log.debug(f"[cookies]:\n {formatting(cookies)}")
-        if params != "":
-            log.debug(f"[params]:\n {formatting(params)}")
-        if data != "":
-            log.debug(f"[data]:\n {formatting(data)}")
-        if json_ != "":
-            log.debug(f"[json]:\n {formatting(json_)}")
+        auth = kwargs.get("auth", None)
+        headers = kwargs.get("headers", None)
+        cookies = kwargs.get("cookies", None)
+        params = kwargs.get("params", None)
+        data = kwargs.get("data", None)
+        json_ = kwargs.get("json", None)
+        files = kwargs.get("files", None)
+        if auth is not None:
+            log.debug(f"[auth]:\n{auth}")
+        if headers is not None:
+            log.debug(f"[headers]:\n{formatting(headers)}")
+        if cookies is not None:
+            log.debug(f"[cookies]:\n{formatting(cookies)}")
+        if params is not None:
+            log.debug(f"[params]:\n{formatting(params)}")
+        if data is not None:
+            log.debug(f"[data]:\n{formatting(data)}")
+        if json_ is not None:
+            log.debug(f"[json]:\n{formatting(json_)}")
+        if files is not None:
+            log.debug(f"[files]:\n{files}")
 
         # running function
         r = func(*args, **kwargs)
 
         ResponseResult.request = r.request
         ResponseResult.status_code = r.status_code
         log.info("-------------- Response ----------------[🛬️]")
@@ -88,51 +98,67 @@
                 ResponseResult.response = r.text
 
         return r
 
     return wrapper
 
 
-class ResponseResult:
-    status_code = 200
-    response = None
-    request = None
+def mock_url(url: str) -> str:
+    """
+    If the mock hook is set, replace it with the mock url
+    :param url:
+    """
+    configs = loader("mock_url") if loader("mock_url") is not None else None
+    if configs is None:
+        return url
+
+    replace_url = configs.get(url, "")
+    if replace_url == "":
+        return url
+
+    log.debug(f"mock url: {replace_url}")
+    return replace_url
 
 
 class HttpRequest:
     """seldom http request class"""
 
     @request
     def get(self, url, params=None, **kwargs):
         if (Seldom.base_url is not None) and (url.startswith("http") is False):
             url = Seldom.base_url + url
+        url = mock_url(url)
         return requests.get(url, params=params, **kwargs)
 
     @request
     def post(self, url, data=None, json=None, **kwargs):
         if (Seldom.base_url is not None) and (url.startswith("http") is False):
             url = Seldom.base_url + url
+        url = mock_url(url)
         return requests.post(url, data=data, json=json, **kwargs)
 
     @request
     def put(self, url, data=None, **kwargs):
         if (Seldom.base_url is not None) and (url.startswith("http") is False):
             url = Seldom.base_url + url
+        url = mock_url(url)
         return requests.put(url, data=data, **kwargs)
 
     @request
     def delete(self, url, **kwargs):
         if (Seldom.base_url is not None) and (url.startswith("http") is False):
             url = Seldom.base_url + url
+        url = mock_url(url)
         return requests.delete(url, **kwargs)
 
     @request
     def patch(self, url, data=None, **kwargs):
         if (Seldom.base_url is not None) and (url.startswith("http") is False):
             url = Seldom.base_url + url
+        url = mock_url(url)
         return requests.patch(url, data=data, **kwargs)
 
     @property
     def response(self) -> dict:
         """
         Returns the result of the response
         :return: response
@@ -196,14 +222,15 @@
             r"""Sends a GET request. Returns :class:`Response` object.
             :param url: URL for the new :class:`Request` object.
             :param \*\*kwargs: Optional arguments that ``request`` takes.
             :rtype: requests.Response
             """
             if (Seldom.base_url is not None) and (url.startswith("http") is False):
                 url = Seldom.base_url + url
+            url = mock_url(url)
             kwargs.setdefault('allow_redirects', True)
             return self.request('GET', url, **kwargs)
 
         @request
         def post(self, url, data=None, json=None, **kwargs):
             r"""Sends a POST request. Returns :class:`Response` object.
 
@@ -212,40 +239,43 @@
                 object to send in the body of the :class:`Request`.
             :param json: (optional) json to send in the body of the :class:`Request`.
             :param \*\*kwargs: Optional arguments that ``request`` takes.
             :rtype: requests.Response
             """
             if (Seldom.base_url is not None) and (url.startswith("http") is False):
                 url = Seldom.base_url + url
+            url = mock_url(url)
             return self.request('POST', url, data=data, json=json, **kwargs)
 
         @request
         def put(self, url, data=None, **kwargs):
             r"""Sends a PUT request. Returns :class:`Response` object.
 
             :param url: URL for the new :class:`Request` object.
             :param data: (optional) Dictionary, list of tuples, bytes, or file-like
                 object to send in the body of the :class:`Request`.
             :param \*\*kwargs: Optional arguments that ``request`` takes.
             :rtype: requests.Response
             """
             if (Seldom.base_url is not None) and (url.startswith("http") is False):
                 url = Seldom.base_url + url
+            url = mock_url(url)
             return self.request('PUT', url, data=data, **kwargs)
 
         @request
         def delete(self, url, **kwargs):
             r"""Sends a DELETE request. Returns :class:`Response` object.
 
             :param url: URL for the new :class:`Request` object.
             :param \*\*kwargs: Optional arguments that ``request`` takes.
             :rtype: requests.Response
             """
             if (Seldom.base_url is not None) and (url.startswith("http") is False):
                 url = Seldom.base_url + url
+            url = mock_url(url)
             return self.request('DELETE', url, **kwargs)
 
     @staticmethod
     def json_to_dict(data: str, replace_quotes: bool = True) -> dict:
         """
         json to dict
         :param data: json data.
```

### Comparing `seldom-3.2.2/seldom/running/DebugTestRunner.py` & `seldom-3.2.3/seldom/running/DebugTestRunner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
 Run tests in debug mode
 """
 import unittest
 import functools
+from concurrent.futures import ThreadPoolExecutor
+from XTestRunner.htmlrunner.result import _TestResult
 
 
 class DebugTestRunner(unittest.TextTestRunner):
     """Debug test runner"""
 
     def __init__(self, *args, **kwargs):
         """
@@ -59,9 +61,17 @@
                     skip_wrapper.__unittest_skip_why__ = f'label whitelist {self.whitelist}'
                 if len(self.blacklist) >= 1:
                     skip_wrapper.__unittest_skip_why__ = f'label blacklist {self.blacklist}'
                 setattr(test, test._testMethodName, skip_wrapper)
 
             suite.addTest(test)
 
+        # res = unittest.TestResult()
+        res = _TestResult()
+        with ThreadPoolExecutor(max_workers=3) as executor:
+            for s in suite:
+                executor.submit(s.run, result=res)
+
+        # print("res", res)
+        return res
         # Resume normal TextTestRunner function with the new test suite
-        super(DebugTestRunner, self).run(suite)
+        # super(DebugTestRunner, self).run(suite)
```

### Comparing `seldom-3.2.2/seldom/running/__init__.py` & `seldom-3.2.3/seldom/running/__init__.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/seldom/running/config.py` & `seldom-3.2.3/seldom/running/config.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/seldom/running/loader.py` & `seldom-3.2.3/seldom/running/loader.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/seldom/running/loader_extend.py` & `seldom-3.2.3/seldom/running/loader_extend.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/seldom/running/loader_hook.py` & `seldom-3.2.3/seldom/running/loader_hook.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import sys
 import importlib
 
 
-def loader(func_name: str, file_name: str = "confrun.py"):
+def loader(func_name: str, file_name: str = "confrun.py", *args, **kwargs):
     """
     Execute the hook function dynamically.
     :param func_name: function name
     :param file_name: hook file name
     """
     # By default, confrun.py files are searched in the current directory
     file_dir = os.getcwd()
@@ -19,15 +19,15 @@
     for module_name in all_hook_module:
         hooks.append(importlib.import_module(module_name))
 
     # Execute the function according to the  name
     for per_hook in hooks:
         try:
             func = getattr(per_hook, func_name)
-            return func()
+            return func(*args, **kwargs)
         except AttributeError:
             return None
 
 
 if __name__ == '__main__':
     browser = loader("browser")
     print(f"get browser name: {browser}")
```

### Comparing `seldom-3.2.2/seldom/running/runner.py` & `seldom-3.2.3/seldom/running/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             debug: bool = False,
             timeout: int = 10,
             app_server=None,
             app_info=None,
             report: str = None,
             title: str = "Seldom Test Report",
             tester: str = "Anonymous",
-            description: str = "Test case execution",
+            description: [str or list] = "Test case execution",
             rerun: int = 0,
             language: str = "en",
             whitelist: list = [],
             blacklist: list = [],
             open: bool = True,
             auto: bool = True):
         """
```

### Comparing `seldom-3.2.2/seldom/skip.py` & `seldom-3.2.3/seldom/skip.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/seldom/testdata/conversion.py` & `seldom-3.2.3/seldom/testdata/conversion.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/seldom/testdata/parameterization.py` & `seldom-3.2.3/seldom/testdata/parameterization.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         raise FileExistsError("File name does not exist.")
 
     stack_t = sys_inspect.stack()
     ins = sys_inspect.getframeinfo(stack_t[1][0])
     file_dir = os.path.dirname(os.path.abspath(ins.filename))
 
     file_path = find_file(file, file_dir)
-    if file_path is None:
+    if file_path == "":
         raise FileExistsError(f"No '{file}' data file found.")
 
     suffix = file.split(".")[-1]
     if suffix == "csv":
         data_list = conversion.csv_to_list(file_path, line=line, end_line=end_line)
     elif suffix == "xlsx":
         data_list = conversion.excel_to_list(file_path, sheet=sheet, line=line, end_line=end_line)
```

### Comparing `seldom-3.2.2/seldom/testdata/random_data.py` & `seldom-3.2.3/seldom/testdata/random_data.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/seldom/testdata/random_func.py` & `seldom-3.2.3/seldom/testdata/random_func.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/seldom/utils/cache.py` & `seldom-3.2.3/seldom/utils/cache.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/seldom/utils/curlify.py` & `seldom-3.2.3/seldom/utils/curlify.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/seldom/utils/diff.py` & `seldom-3.2.3/seldom/utils/diff.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/seldom/utils/file_extend.py` & `seldom-3.2.3/seldom/utils/file_extend.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/seldom/utils/jsonpath.py` & `seldom-3.2.3/seldom/utils/jsonpath.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/seldom/utils/klook.py` & `seldom-3.2.3/seldom/utils/klook.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/seldom/utils/send_extend.py` & `seldom-3.2.3/seldom/utils/send_extend.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/seldom/utils/thread_lab.py` & `seldom-3.2.3/seldom/utils/thread_lab.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/seldom/utils/tomorrow.py` & `seldom-3.2.3/seldom/utils/tomorrow.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/seldom/webdriver.py` & `seldom-3.2.3/seldom/webdriver.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,32 +59,35 @@
 
         self.by = LOCATOR_LIST.get(by)
         if self.by is None:
             raise ValueError(f"The find element is not supported: {by}. ")
         self.find_elem_info = None
         self.find_elem_warn = None
 
-    def get_elements(self, index: int = None):
+    def get_elements(self, index: int = None, empty=False):
         """
         Judge element positioning way, and returns the element.
         """
 
         for _ in range(Seldom.timeout):
             elems = Seldom.driver.find_elements(by=self.by, value=self.value)
             if len(elems) >= 1:
                 self.find_elem_info = f"Find {len(elems)} element: {self.by}={self.value} "
                 break
             time.sleep(1)
         else:
             self.find_elem_warn = f"❌ Find 0 element through: {self.by}={self.value}"
 
         elem = Seldom.driver.find_elements(self.by, self.value)
-        if len(elem) == 0:
+        if len(elem) == 0 and empty is False:
             raise NotFindElementError(self.find_elem_warn)
 
+        if len(elem) == 0 and empty is True:
+            return []
+
         if index is None:
             return elem
 
         return elem[index]
 
     @staticmethod
     def show_element(elem) -> None:
@@ -102,23 +105,14 @@
                 Seldom.driver.execute_script(style_red, elem)
                 time.sleep(0.2)
                 Seldom.driver.execute_script(style_blue, elem)
                 time.sleep(0.2)
             Seldom.driver.execute_script(style_blue, elem)
             time.sleep(0.2)
             Seldom.driver.execute_script(style_null, elem)
-        else:
-            for _ in range(2):
-                Seldom.driver.execute_script(style_red, elem)
-                time.sleep(0.1)
-                Seldom.driver.execute_script(style_blue, elem)
-                time.sleep(0.1)
-            Seldom.driver.execute_script(style_blue, elem)
-            time.sleep(0.3)
-            Seldom.driver.execute_script(style_null, elem)
 
     @property
     def info(self):
         """return element info"""
         return self.find_elem_info
 
     @property
@@ -942,15 +936,15 @@
         Get a set of elements
 
         Usage:
         ret = self.get_elements(css="#el")
         print(len(ret))
         """
         web_elem = WebElement(**kwargs)
-        elems = web_elem.get_elements()
+        elems = web_elem.get_elements(empty=True)
         if len(elems) == 0:
             log.warning(f"{web_elem.warn}.")
         else:
             log.info(f"✅ {web_elem.info}.")
         return elems
 
     @staticmethod
```

### Comparing `seldom-3.2.2/seldom/webdriver_chaining.py` & `seldom-3.2.3/seldom/webdriver_chaining.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/seldom.egg-info/PKG-INFO` & `seldom-3.2.3/seldom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: seldom
-Version: 3.2.2
+Version: 3.2.3
 Summary: Seldom automation testing framework based on unittest.
 Home-page: https://github.com/seldomQA/seldom/
 Author: bugmaster
 Author-email: fnngj@126.com
-License: BSD
+License: Apache-2.0
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `seldom-3.2.2/seldom.egg-info/SOURCES.txt` & `seldom-3.2.3/seldom.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.py
 demo/__init__.py
 demo/confrun.py
 demo/run.py
 demo/test_dir/__init__.py
 demo/test_dir/api_case/__init__.py
 demo/test_dir/api_case/test_http_demo.py
```

### Comparing `seldom-3.2.2/setup.py` & `seldom-3.2.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,33 +11,33 @@
         f.read().decode('utf-8')).group(1)))
 
 
 setup(
     name='seldom',
     version=version,
     url='https://github.com/seldomQA/seldom/',
-    license='BSD',
+    license='Apache-2.0',
     author='bugmaster',
     author_email='fnngj@126.com',
     description='Seldom automation testing framework based on unittest.',
     long_description=open(join(abspath(dirname(__file__)), "description.rst"), encoding='utf8').read(),
     packages=find_packages(),
     include_package_data=True,
     zip_safe=False,
     install_requires=[
-        'Appium-Python-Client>=2.1.0',
+        'Appium-Python-Client>=2.11.0',
         'XTestRunner>=1.7.0',
         'parameterized==0.8.1',
         'loguru==0.6.0',
         'openpyxl>=3.0.3',
-        'pyyaml>=5.1',
+        'pyyaml>=6.0',
         'requests>=2.22.0',
-        'jsonschema>=3.2.0',
+        'jsonschema>=4.10.0',
         'jmespath>=0.10.0',
-        'webdriver-manager==3.8.5',
+        'webdriver-manager~=4.0.0',
         'pymysql>=1.0.0',
         'genson==1.2.2',
         'click~=8.1.3',
         'python-dateutil==2.8.2'
     ],
     classifiers=[
         'Intended Audience :: Developers',
```

### Comparing `seldom-3.2.2/test/test_cache.py` & `seldom-3.2.3/test/test_cache.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/test/test_db_operation.py` & `seldom-3.2.3/test/test_db_operation.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/test/test_klook.py` & `seldom-3.2.3/test/test_klook.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/test/test_log.py` & `seldom-3.2.3/test/test_log.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/test/test_memory_cache.py` & `seldom-3.2.3/test/test_memory_cache.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/test/test_testdata.py` & `seldom-3.2.3/test/test_testdata.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/test/test_thread.py` & `seldom-3.2.3/test/test_thread.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/test/test_thread2.py` & `seldom-3.2.3/test/test_thread2.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/test/test_thread_case.py` & `seldom-3.2.3/test/test_thread_case.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.2/test/test_thread_path.py` & `seldom-3.2.3/test/test_thread_path.py`

 * *Files identical despite different names*

