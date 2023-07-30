# Comparing `tmp/Logbook-1.5.3.tar.gz` & `tmp/Logbook-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Logbook-1.5.3.tar", last modified: Wed Oct 16 18:00:25 2019, max compression
+gzip compressed data, was "Logbook-1.6.0.tar", last modified: Sun Jul 30 20:08:32 2023, max compression
```

## Comparing `Logbook-1.5.3.tar` & `Logbook-1.6.0.tar`

### file list

```diff
@@ -1,66 +1,129 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-16 18:00:25.000000 Logbook-1.5.3/
--rw-rw-r--   0 travis    (2000) travis    (2000)    10892 2019-10-16 17:59:35.000000 Logbook-1.5.3/CHANGES
--rw-rw-r--   0 travis    (2000) travis    (2000)     1556 2019-10-16 17:59:35.000000 Logbook-1.5.3/LICENSE
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-16 18:00:25.000000 Logbook-1.5.3/Logbook.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2502 2019-10-16 18:00:25.000000 Logbook-1.5.3/Logbook.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1295 2019-10-16 18:00:25.000000 Logbook-1.5.3/Logbook.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-10-16 18:00:25.000000 Logbook-1.5.3/Logbook.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-10-16 18:00:25.000000 Logbook-1.5.3/Logbook.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      286 2019-10-16 18:00:25.000000 Logbook-1.5.3/Logbook.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2019-10-16 18:00:25.000000 Logbook-1.5.3/Logbook.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      151 2019-10-16 17:59:35.000000 Logbook-1.5.3/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      727 2019-10-16 17:59:35.000000 Logbook-1.5.3/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)     2502 2019-10-16 18:00:25.000000 Logbook-1.5.3/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1299 2019-10-16 17:59:35.000000 Logbook-1.5.3/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-16 18:00:25.000000 Logbook-1.5.3/logbook/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1772 2019-10-16 17:59:35.000000 Logbook-1.5.3/logbook/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2019-10-16 17:59:35.000000 Logbook-1.5.3/logbook/__version__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8112 2019-10-16 17:59:35.000000 Logbook-1.5.3/logbook/_fallback.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9480 2019-10-16 17:59:35.000000 Logbook-1.5.3/logbook/_speedups.pyx
--rw-rw-r--   0 travis    (2000) travis    (2000)     1138 2019-10-16 17:59:35.000000 Logbook-1.5.3/logbook/_termcolors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41344 2019-10-16 17:59:35.000000 Logbook-1.5.3/logbook/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10377 2019-10-16 17:59:35.000000 Logbook-1.5.3/logbook/compat.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6257 2019-10-16 17:59:35.000000 Logbook-1.5.3/logbook/concurrency.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    71534 2019-10-16 17:59:35.000000 Logbook-1.5.3/logbook/handlers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8384 2019-10-16 17:59:35.000000 Logbook-1.5.3/logbook/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19776 2019-10-16 17:59:35.000000 Logbook-1.5.3/logbook/more.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12035 2019-10-16 17:59:35.000000 Logbook-1.5.3/logbook/notifiers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24663 2019-10-16 17:59:35.000000 Logbook-1.5.3/logbook/queues.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19231 2019-10-16 17:59:35.000000 Logbook-1.5.3/logbook/ticketing.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5783 2019-10-16 17:59:35.000000 Logbook-1.5.3/logbook/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-16 18:00:25.000000 Logbook-1.5.3/scripts/
--rw-rw-r--   0 travis    (2000) travis    (2000)      364 2019-10-16 17:59:35.000000 Logbook-1.5.3/scripts/test_setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      156 2019-10-16 18:00:25.000000 Logbook-1.5.3/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     7211 2019-10-16 17:59:35.000000 Logbook-1.5.3/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-16 18:00:25.000000 Logbook-1.5.3/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-16 17:59:35.000000 Logbook-1.5.3/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2673 2019-10-16 17:59:35.000000 Logbook-1.5.3/tests/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      801 2019-10-16 17:59:35.000000 Logbook-1.5.3/tests/test_asyncio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      474 2019-10-16 17:59:35.000000 Logbook-1.5.3/tests/test_ci.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      986 2019-10-16 17:59:35.000000 Logbook-1.5.3/tests/test_deadlock.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9790 2019-10-16 17:59:35.000000 Logbook-1.5.3/tests/test_file_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2633 2019-10-16 17:59:35.000000 Logbook-1.5.3/tests/test_fingers_crossed_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1073 2019-10-16 17:59:35.000000 Logbook-1.5.3/tests/test_flags.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2285 2019-10-16 17:59:35.000000 Logbook-1.5.3/tests/test_groups.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1543 2019-10-16 17:59:35.000000 Logbook-1.5.3/tests/test_handler_errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4628 2019-10-16 17:59:35.000000 Logbook-1.5.3/tests/test_handlers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1138 2019-10-16 17:59:35.000000 Logbook-1.5.3/tests/test_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1280 2019-10-16 17:59:35.000000 Logbook-1.5.3/tests/test_log_record.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1126 2019-10-16 17:59:35.000000 Logbook-1.5.3/tests/test_logbook.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1181 2019-10-16 17:59:35.000000 Logbook-1.5.3/tests/test_logger.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2823 2019-10-16 17:59:35.000000 Logbook-1.5.3/tests/test_logging_api.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3123 2019-10-16 17:59:35.000000 Logbook-1.5.3/tests/test_logging_compat.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2921 2019-10-16 17:59:35.000000 Logbook-1.5.3/tests/test_logging_times.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8642 2019-10-16 17:59:35.000000 Logbook-1.5.3/tests/test_mail_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7053 2019-10-16 17:59:35.000000 Logbook-1.5.3/tests/test_more.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1943 2019-10-16 17:59:35.000000 Logbook-1.5.3/tests/test_nteventlog_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1701 2019-10-16 17:59:35.000000 Logbook-1.5.3/tests/test_null_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3368 2019-10-16 17:59:35.000000 Logbook-1.5.3/tests/test_processors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11304 2019-10-16 17:59:35.000000 Logbook-1.5.3/tests/test_queues.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2146 2019-10-16 17:59:35.000000 Logbook-1.5.3/tests/test_syslog_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1535 2019-10-16 17:59:35.000000 Logbook-1.5.3/tests/test_test_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2211 2019-10-16 17:59:35.000000 Logbook-1.5.3/tests/test_ticketing.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2187 2019-10-16 17:59:35.000000 Logbook-1.5.3/tests/test_unicode.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5496 2019-10-16 17:59:35.000000 Logbook-1.5.3/tests/test_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2507 2019-10-16 17:59:35.000000 Logbook-1.5.3/tests/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      879 2019-10-16 17:59:35.000000 Logbook-1.5.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:08:32.159198 Logbook-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-30 20:08:17.000000 Logbook-1.6.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11565 2023-07-30 20:08:17.000000 Logbook-1.6.0/CHANGES
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-30 20:08:17.000000 Logbook-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-30 20:08:17.000000 Logbook-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-30 20:08:17.000000 Logbook-1.6.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-30 20:08:32.159198 Logbook-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-30 20:08:17.000000 Logbook-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:08:32.147197 Logbook-1.6.0/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-30 20:08:17.000000 Logbook-1.6.0/benchmark/bench_disabled_introspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-30 20:08:17.000000 Logbook-1.6.0/benchmark/bench_disabled_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-30 20:08:17.000000 Logbook-1.6.0/benchmark/bench_enabled_introspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-30 20:08:17.000000 Logbook-1.6.0/benchmark/bench_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-30 20:08:17.000000 Logbook-1.6.0/benchmark/bench_file_handler_unicode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-30 20:08:17.000000 Logbook-1.6.0/benchmark/bench_logger_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-30 20:08:17.000000 Logbook-1.6.0/benchmark/bench_logger_level_low.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-30 20:08:17.000000 Logbook-1.6.0/benchmark/bench_logging_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-30 20:08:17.000000 Logbook-1.6.0/benchmark/bench_logging_file_handler_unicode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-30 20:08:17.000000 Logbook-1.6.0/benchmark/bench_logging_logger_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-30 20:08:17.000000 Logbook-1.6.0/benchmark/bench_logging_logger_level_low.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-30 20:08:17.000000 Logbook-1.6.0/benchmark/bench_logging_noop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-30 20:08:17.000000 Logbook-1.6.0/benchmark/bench_logging_noop_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-30 20:08:17.000000 Logbook-1.6.0/benchmark/bench_logging_stream_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-30 20:08:17.000000 Logbook-1.6.0/benchmark/bench_noop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-30 20:08:17.000000 Logbook-1.6.0/benchmark/bench_noop_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-30 20:08:17.000000 Logbook-1.6.0/benchmark/bench_noop_filter_on_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-30 20:08:17.000000 Logbook-1.6.0/benchmark/bench_redirect_from_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-30 20:08:17.000000 Logbook-1.6.0/benchmark/bench_redirect_to_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-30 20:08:17.000000 Logbook-1.6.0/benchmark/bench_stack_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-30 20:08:17.000000 Logbook-1.6.0/benchmark/bench_stream_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-30 20:08:17.000000 Logbook-1.6.0/benchmark/bench_test_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-30 20:08:17.000000 Logbook-1.6.0/benchmark/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:08:32.151198 Logbook-1.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-07-30 20:08:17.000000 Logbook-1.6.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:08:32.151198 Logbook-1.6.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   255890 2023-07-30 20:08:17.000000 Logbook-1.6.0/docs/_static/logbook-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:08:32.151198 Logbook-1.6.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-30 20:08:17.000000 Logbook-1.6.0/docs/api/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-30 20:08:17.000000 Logbook-1.6.0/docs/api/compat.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-30 20:08:17.000000 Logbook-1.6.0/docs/api/handlers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-30 20:08:17.000000 Logbook-1.6.0/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-30 20:08:17.000000 Logbook-1.6.0/docs/api/internal.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-30 20:08:17.000000 Logbook-1.6.0/docs/api/more.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-30 20:08:17.000000 Logbook-1.6.0/docs/api/notifiers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-30 20:08:17.000000 Logbook-1.6.0/docs/api/queues.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-30 20:08:17.000000 Logbook-1.6.0/docs/api/ticketing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-30 20:08:17.000000 Logbook-1.6.0/docs/api/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-30 20:08:17.000000 Logbook-1.6.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-30 20:08:17.000000 Logbook-1.6.0/docs/compat.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-30 20:08:17.000000 Logbook-1.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-30 20:08:17.000000 Logbook-1.6.0/docs/cookbook.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10248 2023-07-30 20:08:17.000000 Logbook-1.6.0/docs/designdefense.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-07-30 20:08:17.000000 Logbook-1.6.0/docs/designexplained.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-07-30 20:08:17.000000 Logbook-1.6.0/docs/features.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-30 20:08:17.000000 Logbook-1.6.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-30 20:08:17.000000 Logbook-1.6.0/docs/libraries.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-07-30 20:08:17.000000 Logbook-1.6.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-07-30 20:08:17.000000 Logbook-1.6.0/docs/performance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-07-30 20:08:17.000000 Logbook-1.6.0/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-07-30 20:08:17.000000 Logbook-1.6.0/docs/setups.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:08:32.151198 Logbook-1.6.0/docs/sheet/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-30 20:08:17.000000 Logbook-1.6.0/docs/sheet/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:08:32.151198 Logbook-1.6.0/docs/sheet/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-30 20:08:17.000000 Logbook-1.6.0/docs/sheet/static/background.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-30 20:08:17.000000 Logbook-1.6.0/docs/sheet/static/sheet.css_t
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-30 20:08:17.000000 Logbook-1.6.0/docs/sheet/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-07-30 20:08:17.000000 Logbook-1.6.0/docs/stacks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-30 20:08:17.000000 Logbook-1.6.0/docs/ticketing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-30 20:08:17.000000 Logbook-1.6.0/docs/unittesting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-30 20:08:17.000000 Logbook-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-30 20:08:32.159198 Logbook-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-30 20:08:17.000000 Logbook-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:08:32.143197 Logbook-1.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:08:32.155197 Logbook-1.6.0/src/Logbook.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-30 20:08:32.000000 Logbook-1.6.0/src/Logbook.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-30 20:08:32.000000 Logbook-1.6.0/src/Logbook.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 20:08:32.000000 Logbook-1.6.0/src/Logbook.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 20:08:31.000000 Logbook-1.6.0/src/Logbook.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-30 20:08:32.000000 Logbook-1.6.0/src/Logbook.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-30 20:08:32.000000 Logbook-1.6.0/src/Logbook.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:08:32.155197 Logbook-1.6.0/src/cython/
+-rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-07-30 20:08:17.000000 Logbook-1.6.0/src/cython/speedups.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:08:32.155197 Logbook-1.6.0/src/logbook/
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-30 20:08:17.000000 Logbook-1.6.0/src/logbook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-30 20:08:17.000000 Logbook-1.6.0/src/logbook/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-07-30 20:08:17.000000 Logbook-1.6.0/src/logbook/_fallback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-30 20:08:17.000000 Logbook-1.6.0/src/logbook/_termcolors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40578 2023-07-30 20:08:17.000000 Logbook-1.6.0/src/logbook/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9798 2023-07-30 20:08:17.000000 Logbook-1.6.0/src/logbook/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-07-30 20:08:17.000000 Logbook-1.6.0/src/logbook/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70813 2023-07-30 20:08:17.000000 Logbook-1.6.0/src/logbook/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-07-30 20:08:17.000000 Logbook-1.6.0/src/logbook/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19446 2023-07-30 20:08:17.000000 Logbook-1.6.0/src/logbook/more.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-07-30 20:08:17.000000 Logbook-1.6.0/src/logbook/notifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24465 2023-07-30 20:08:17.000000 Logbook-1.6.0/src/logbook/queues.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19139 2023-07-30 20:08:17.000000 Logbook-1.6.0/src/logbook/ticketing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-30 20:08:17.000000 Logbook-1.6.0/src/logbook/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 20:08:32.159198 Logbook-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 20:08:17.000000 Logbook-1.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-30 20:08:17.000000 Logbook-1.6.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-30 20:08:17.000000 Logbook-1.6.0/tests/test_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-30 20:08:17.000000 Logbook-1.6.0/tests/test_deadlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-07-30 20:08:17.000000 Logbook-1.6.0/tests/test_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-30 20:08:17.000000 Logbook-1.6.0/tests/test_fingers_crossed_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-30 20:08:17.000000 Logbook-1.6.0/tests/test_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-30 20:08:17.000000 Logbook-1.6.0/tests/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-30 20:08:17.000000 Logbook-1.6.0/tests/test_handler_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-07-30 20:08:17.000000 Logbook-1.6.0/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-30 20:08:17.000000 Logbook-1.6.0/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-30 20:08:17.000000 Logbook-1.6.0/tests/test_log_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-30 20:08:17.000000 Logbook-1.6.0/tests/test_logbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-30 20:08:17.000000 Logbook-1.6.0/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-30 20:08:17.000000 Logbook-1.6.0/tests/test_logging_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-30 20:08:17.000000 Logbook-1.6.0/tests/test_logging_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-30 20:08:17.000000 Logbook-1.6.0/tests/test_logging_times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-07-30 20:08:17.000000 Logbook-1.6.0/tests/test_mail_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-07-30 20:08:17.000000 Logbook-1.6.0/tests/test_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-30 20:08:17.000000 Logbook-1.6.0/tests/test_nteventlog_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-30 20:08:17.000000 Logbook-1.6.0/tests/test_null_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-30 20:08:17.000000 Logbook-1.6.0/tests/test_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11321 2023-07-30 20:08:17.000000 Logbook-1.6.0/tests/test_queues.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-30 20:08:17.000000 Logbook-1.6.0/tests/test_speedups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-30 20:08:17.000000 Logbook-1.6.0/tests/test_syslog_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-30 20:08:17.000000 Logbook-1.6.0/tests/test_test_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-30 20:08:17.000000 Logbook-1.6.0/tests/test_ticketing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-30 20:08:17.000000 Logbook-1.6.0/tests/test_unicode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-07-30 20:08:17.000000 Logbook-1.6.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-30 20:08:17.000000 Logbook-1.6.0/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-30 20:08:17.000000 Logbook-1.6.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `Logbook-1.5.3/CHANGES` & `Logbook-1.6.0/CHANGES`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,39 @@
 Logbook Changelog
 =================
 
+Version 1.6.0
+-------------
+
+Released on July 30th, 2023
+
+- Dropped support for Python 2.7, 3.5, and 3.6.
+- Uses pyproject.toml based build.
+- Added nteventlog extra for NTEventLogHandler.
+- Supports SQLAlchemy 1.4 and 2.0.
+- Fix various deprecation warnings.
+- exc_info arg may be a BaseException instance (thanks Mattijs Ugen)
+- FileHandler supports path-like objects.
+- Fixed bug which prevented compilation on Cython 3
+- Wheels are generated for more platforms and architectures
+
+Version 1.5.3
+-------------
+
+Released on October 16th, 2019
+
+- Fixed deprecated imports from collections module.
+
+Version 1.5.2
+-------------
+
+Released on August 21st, 2019
+
+- No changes
+
 Version 1.5.1
 -------------
 
 Released on August 20th, 2019
 
 - Added support for asyncio and contextvars
 
@@ -219,15 +248,15 @@
 
 Version 0.4.1
 -------------
 
 Released on December 12th. Codename "121212"
 
 - Fixed several outstanding encoding problems, thanks to @dvarazzo.
-- Merged in minor pull requests (see https://github.com/mitsuhiko/logbook/pulls?&state=closed)
+- Merged in minor pull requests (see https://github.com/getlogbook/logbook/pulls?q=is%3Aclosed)
 
 Version 0.4
 -----------
 
 Released on October 24th.  Codename "Phoenix"
 
 - Added preliminary RabbitMQ and CouchDB support.
```

### Comparing `Logbook-1.5.3/LICENSE` & `Logbook-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Logbook-1.5.3/Makefile` & `Logbook-1.6.0/Makefile`

 * *Files identical despite different names*

### Comparing `Logbook-1.5.3/logbook/__init__.py` & `Logbook-1.6.0/src/logbook/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,71 @@
-# -*- coding: utf-8 -*-
 """
     logbook
     ~~~~~~~
 
     Simple logging library that aims to support desktop, command line
     and web applications alike.
 
     :copyright: (c) 2010 by Armin Ronacher, Georg Brandl.
     :license: BSD, see LICENSE for more details.
 """
 
 import os
+
 from .base import (
-    LogRecord, Logger, LoggerGroup, NestedSetup,  Processor, Flags,
-    get_level_name, lookup_level, dispatch_record, CRITICAL, ERROR, WARNING,
-    NOTICE, INFO, DEBUG, TRACE, NOTSET, set_datetime_format)
+    CRITICAL,
+    DEBUG,
+    ERROR,
+    INFO,
+    NOTICE,
+    NOTSET,
+    TRACE,
+    WARNING,
+    Flags,
+    Logger,
+    LoggerGroup,
+    LogRecord,
+    NestedSetup,
+    Processor,
+    dispatch_record,
+    get_level_name,
+    lookup_level,
+    set_datetime_format,
+)
 from .handlers import (
-    Handler, StreamHandler, FileHandler, MonitoringFileHandler, StderrHandler,
-    RotatingFileHandler, TimedRotatingFileHandler, TestHandler, MailHandler,
-    GMailHandler, SyslogHandler, NullHandler, NTEventLogHandler,
-    create_syshandler, StringFormatter, StringFormatterHandlerMixin,
-    HashingHandlerMixin, LimitingHandlerMixin, WrapperHandler,
-    FingersCrossedHandler, GroupHandler, GZIPCompressionHandler, BrotliCompressionHandler)
-from . import compat
+    BrotliCompressionHandler,
+    FileHandler,
+    FingersCrossedHandler,
+    GMailHandler,
+    GroupHandler,
+    GZIPCompressionHandler,
+    Handler,
+    HashingHandlerMixin,
+    LimitingHandlerMixin,
+    MailHandler,
+    MonitoringFileHandler,
+    NTEventLogHandler,
+    NullHandler,
+    RotatingFileHandler,
+    StderrHandler,
+    StreamHandler,
+    StringFormatter,
+    StringFormatterHandlerMixin,
+    SyslogHandler,
+    TestHandler,
+    TimedRotatingFileHandler,
+    WrapperHandler,
+    create_syshandler,
+)
 
+from . import compat  # isort: skip
 
 # create an anonymous default logger and provide all important
 # methods of that logger as global functions
-_default_logger = Logger('Generic')
+_default_logger = Logger("Generic")
 _default_logger.suppress_dispatcher = True
 trace = _default_logger.trace
 debug = _default_logger.debug
 info = _default_logger.info
 warn = _default_logger.warn
 warning = _default_logger.warning
 notice = _default_logger.notice
@@ -40,12 +74,12 @@
 catch_exceptions = _default_logger.catch_exceptions
 critical = _default_logger.critical
 log = _default_logger.log
 del _default_logger
 
 
 # install a default global handler
-if os.environ.get('LOGBOOK_INSTALL_DEFAULT_HANDLER'):
+if os.environ.get("LOGBOOK_INSTALL_DEFAULT_HANDLER"):
     default_handler = StderrHandler()
     default_handler.push_application()
 
 from .__version__ import __version__
```

### Comparing `Logbook-1.5.3/logbook/_fallback.py` & `Logbook-1.6.0/src/logbook/_fallback.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,65 +1,74 @@
-# -*- coding: utf-8 -*-
 """
     logbook._fallback
     ~~~~~~~~~~~~~~~~~
 
     Fallback implementations in case speedups is not around.
 
     :copyright: (c) 2010 by Armin Ronacher, Georg Brandl.
     :license: BSD, see LICENSE for more details.
 """
 from itertools import count
-from logbook.helpers import get_iterator_next_method
+
 from logbook.concurrency import (
-    thread_get_ident, greenlet_get_ident, thread_local, greenlet_local,
-    ThreadLock, GreenletRLock, is_gevent_enabled, ContextVar, context_get_ident,
-    is_context_enabled)
+    ContextVar,
+    GreenletRLock,
+    ThreadLock,
+    context_get_ident,
+    greenlet_get_ident,
+    greenlet_local,
+    is_context_enabled,
+    is_gevent_enabled,
+    thread_get_ident,
+    thread_local,
+)
+from logbook.helpers import get_iterator_next_method
 
 _missing = object()
 _MAX_CONTEXT_OBJECT_CACHE = 256
 
 
 def group_reflected_property(name, default, fallback=_missing):
     """Returns a property for a given name that falls back to the
     value of the group if set.  If there is no such group, the
     provided default is used.
     """
+
     def _get(self):
-        rv = getattr(self, '_' + name, _missing)
+        rv = getattr(self, "_" + name, _missing)
         if rv is not _missing and rv != fallback:
             return rv
         if self.group is None:
             return default
         return getattr(self.group, name)
 
     def _set(self, value):
-        setattr(self, '_' + name, value)
+        setattr(self, "_" + name, value)
 
     def _del(self):
-        delattr(self, '_' + name)
-    return property(_get, _set, _del)
+        delattr(self, "_" + name)
 
+    return property(_get, _set, _del)
 
-class _StackBound(object):
 
+class _StackBound:
     def __init__(self, obj, push, pop):
         self.__obj = obj
         self.__push = push
         self.__pop = pop
 
     def __enter__(self):
         self.__push()
         return self.__obj
 
     def __exit__(self, exc_type, exc_value, tb):
         self.__pop()
 
 
-class StackedObject(object):
+class StackedObject:
     """Baseclass for all objects that provide stack manipulation
     operations.
     """
 
     def push_greenlet(self):
         """Pushes the stacked object to the greenlet stack."""
         raise NotImplementedError()
@@ -127,52 +136,52 @@
     def applicationbound(self, _cls=_StackBound):
         """Can be used in combination with the `with` statement to
         execute code while the object is bound to the application.
         """
         return _cls(self, self.push_application, self.pop_application)
 
 
-class ContextStackManager(object):
+class ContextStackManager:
     """Helper class for context objects that manages a stack of
     objects.
     """
 
     def __init__(self):
         self._global = []
         self._thread_context_lock = ThreadLock()
         self._thread_context = thread_local()
         self._greenlet_context_lock = GreenletRLock()
         self._greenlet_context = greenlet_local()
-        self._context_stack = ContextVar('stack')
+        self._context_stack = ContextVar("stack")
         self._cache = {}
         self._stackop = get_iterator_next_method(count())
 
     def iter_context_objects(self):
         """Returns an iterator over all objects for the combined
         application and context cache.
         """
         use_gevent = is_gevent_enabled()
         use_context = is_context_enabled()
 
-        if use_gevent:
-            tid = greenlet_get_ident()
-        elif use_context:
+        if use_context:
             tid = context_get_ident()
+        elif use_gevent:
+            tid = greenlet_get_ident()
         else:
             tid = thread_get_ident()
 
         objects = self._cache.get(tid)
         if objects is None:
             if len(self._cache) > _MAX_CONTEXT_OBJECT_CACHE:
                 self._cache.clear()
             objects = self._global[:]
-            objects.extend(getattr(self._thread_context, 'stack', ()))
+            objects.extend(getattr(self._thread_context, "stack", ()))
 
             if use_gevent:
-                objects.extend(getattr(self._greenlet_context, 'stack', ()))
+                objects.extend(getattr(self._greenlet_context, "stack", ()))
 
             if use_context:
                 objects.extend(self._context_stack.get([]))
 
             objects.sort(reverse=True)
             objects = [x[1] for x in objects]
             self._cache[tid] = objects
@@ -180,29 +189,29 @@
 
     def push_greenlet(self, obj):
         self._greenlet_context_lock.acquire()
         try:
             # remote chance to conflict with thread ids
             self._cache.pop(greenlet_get_ident(), None)
             item = (self._stackop(), obj)
-            stack = getattr(self._greenlet_context, 'stack', None)
+            stack = getattr(self._greenlet_context, "stack", None)
             if stack is None:
                 self._greenlet_context.stack = [item]
             else:
                 stack.append(item)
         finally:
             self._greenlet_context_lock.release()
 
     def pop_greenlet(self):
         self._greenlet_context_lock.acquire()
         try:
             # remote chance to conflict with thread ids
             self._cache.pop(greenlet_get_ident(), None)
-            stack = getattr(self._greenlet_context, 'stack', None)
-            assert stack, 'no objects on stack'
+            stack = getattr(self._greenlet_context, "stack", None)
+            assert stack, "no objects on stack"
             return stack.pop()[1]
         finally:
             self._greenlet_context_lock.release()
 
     def push_context(self, obj):
         self._cache.pop(context_get_ident(), None)
         item = (self._stackop(), obj)
@@ -212,42 +221,42 @@
             self._context_stack.set(stack)
         else:
             stack.append(item)
 
     def pop_context(self):
         self._cache.pop(context_get_ident(), None)
         stack = self._context_stack.get(None)
-        assert stack, 'no objects on stack'
+        assert stack, "no objects on stack"
         return stack.pop()[1]
 
     def push_thread(self, obj):
         self._thread_context_lock.acquire()
         try:
             self._cache.pop(thread_get_ident(), None)
             item = (self._stackop(), obj)
-            stack = getattr(self._thread_context, 'stack', None)
+            stack = getattr(self._thread_context, "stack", None)
             if stack is None:
                 self._thread_context.stack = [item]
             else:
                 stack.append(item)
         finally:
             self._thread_context_lock.release()
 
     def pop_thread(self):
         self._thread_context_lock.acquire()
         try:
             self._cache.pop(thread_get_ident(), None)
-            stack = getattr(self._thread_context, 'stack', None)
-            assert stack, 'no objects on stack'
+            stack = getattr(self._thread_context, "stack", None)
+            assert stack, "no objects on stack"
             return stack.pop()[1]
         finally:
             self._thread_context_lock.release()
 
     def push_application(self, obj):
         self._global.append((self._stackop(), obj))
         self._cache.clear()
 
     def pop_application(self):
-        assert self._global, 'no objects on application stack'
+        assert self._global, "no objects on application stack"
         popped = self._global.pop()[1]
         self._cache.clear()
         return popped
```

### Comparing `Logbook-1.5.3/logbook/_speedups.pyx` & `Logbook-1.6.0/src/cython/speedups.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,39 @@
-# -*- coding: utf-8 -*-
-# cython: language_level=2
 """
     logbook._speedups
     ~~~~~~~~~~~~~~~~~
 
     Cython implementation of some core objects.
 
     :copyright: (c) 2010 by Armin Ronacher, Georg Brandl.
     :license: BSD, see LICENSE for more details.
 """
 
 
-from logbook.concurrency import (is_gevent_enabled, thread_get_ident, greenlet_get_ident, thread_local,
-                                 GreenletRLock, greenlet_local, ContextVar, context_get_ident, is_context_enabled)
+from logbook.concurrency import (
+    ContextVar,
+    GreenletRLock,
+    context_get_ident,
+    greenlet_get_ident,
+    greenlet_local,
+    is_context_enabled,
+    is_gevent_enabled,
+    thread_get_ident,
+    thread_local,
+)
 
 from cpython.dict cimport PyDict_Clear, PyDict_SetItem
-from cpython.list cimport PyList_Append, PyList_Sort, PyList_GET_SIZE
-
-from cpython.pythread cimport PyThread_type_lock, PyThread_allocate_lock, \
-     PyThread_release_lock, PyThread_acquire_lock, WAIT_LOCK
+from cpython.list cimport PyList_Append, PyList_GET_SIZE, PyList_Sort
+from cpython.pythread cimport (
+    WAIT_LOCK,
+    PyThread_acquire_lock,
+    PyThread_allocate_lock,
+    PyThread_release_lock,
+    PyThread_type_lock,
+)
 
 _missing = object()
 
 cdef enum:
     _MAX_CONTEXT_OBJECT_CACHE = 256
 
 
@@ -47,15 +58,15 @@
         if obj.group is None:
             return self.default
         return getattr(obj.group, self.name)
 
     def __set__(self, obj, value):
         setattr(obj, self._name, value)
 
-    def __del__(self, obj):
+    def __delete__(self, obj):
         delattr(obj, self._name)
 
 
 cdef class _StackItem:
     cdef int id
     cdef readonly object val
 
@@ -194,18 +205,18 @@
         self._stackcnt += 1
         return self._stackcnt
 
     cpdef iter_context_objects(self):
         use_gevent = is_gevent_enabled()
         use_context = is_context_enabled()
 
-        if use_gevent:
-            tid = greenlet_get_ident()
-        elif use_context:
+        if use_context:
             tid = context_get_ident()
+        elif use_gevent:
+            tid = greenlet_get_ident()
         else:
             tid = thread_get_ident()
 
         objects = self._cache.get(tid)
         if objects is None:
             if PyList_GET_SIZE(self._cache) > _MAX_CONTEXT_OBJECT_CACHE:
                 PyDict_Clear(self._cache)
```

### Comparing `Logbook-1.5.3/logbook/_termcolors.py` & `Logbook-1.6.0/src/logbook/_termcolors.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,41 @@
-# -*- coding: utf-8 -*-
 """
     logbook._termcolors
     ~~~~~~~~~~~~~~~~~~~
 
     Provides terminal color mappings.
 
     :copyright: (c) 2010 by Armin Ronacher, Georg Brandl.
     :license: BSD, see LICENSE for more details.
 """
 
 esc = "\x1b["
 
 codes = {"": "", "reset": esc + "39;49;00m"}
 
-dark_colors = ["black", "darkred", "darkgreen", "brown", "darkblue",
-               "purple", "teal", "lightgray"]
-light_colors = ["darkgray", "red", "green", "yellow", "blue",
-                "fuchsia", "turquoise", "white"]
+dark_colors = [
+    "black",
+    "darkred",
+    "darkgreen",
+    "brown",
+    "darkblue",
+    "purple",
+    "teal",
+    "lightgray",
+]
+light_colors = [
+    "darkgray",
+    "red",
+    "green",
+    "yellow",
+    "blue",
+    "fuchsia",
+    "turquoise",
+    "white",
+]
 
 x = 30
 for d, l in zip(dark_colors, light_colors):
     codes[d] = esc + "%im" % x
     codes[l] = esc + "%i;01m" % x
     x += 1
 
@@ -31,14 +46,15 @@
 codes["fuscia"] = codes["fuchsia"]
 
 
 def _str_to_type(obj, strtype):
     """Helper for ansiformat and colorize"""
     if isinstance(obj, type(strtype)):
         return obj
-    return obj.encode('ascii')
+    return obj.encode("ascii")
 
 
 def colorize(color_key, text):
     """Returns an ANSI formatted text with the given color."""
-    return (_str_to_type(codes[color_key], text) + text +
-            _str_to_type(codes["reset"], text))
+    return (
+        _str_to_type(codes[color_key], text) + text + _str_to_type(codes["reset"], text)
+    )
```

### Comparing `Logbook-1.5.3/logbook/base.py` & `Logbook-1.6.0/src/logbook/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
     logbook.base
     ~~~~~~~~~~~~
 
     Base implementation for logbook.
 
     :copyright: (c) 2010 by Armin Ronacher, Georg Brandl.
@@ -12,33 +11,37 @@
 import sys
 import traceback
 from collections import defaultdict
 from datetime import datetime
 from itertools import chain
 from weakref import ref as weakref
 
-from logbook.concurrency import (greenlet_get_ident, thread_get_ident,
-                                 thread_get_name)
-
-from logbook.helpers import (PY2, cached_property, integer_types, iteritems,
-                             parse_iso8601, string_types, to_safe_json, u,
-                             xrange)
+from logbook.concurrency import greenlet_get_ident, thread_get_ident, thread_get_name
+from logbook.helpers import cached_property, parse_iso8601, to_safe_json
 
 _has_speedups = False
 try:
-    if os.environ.get('DISABLE_LOGBOOK_CEXT_AT_RUNTIME'):
+    if os.environ.get("DISABLE_LOGBOOK_CEXT_AT_RUNTIME"):
         raise ImportError("Speedups disabled via DISABLE_LOGBOOK_CEXT_AT_RUNTIME")
 
     from logbook._speedups import (
-        _missing, group_reflected_property, ContextStackManager, StackedObject)
+        ContextStackManager,
+        StackedObject,
+        _missing,
+        group_reflected_property,
+    )
 
     _has_speedups = True
 except ImportError:
     from logbook._fallback import (
-        _missing, group_reflected_property, ContextStackManager, StackedObject)
+        ContextStackManager,
+        StackedObject,
+        _missing,
+        group_reflected_property,
+    )
 
 _datetime_factory = datetime.utcnow
 
 
 def set_datetime_format(datetime_format):
     """
     Set the format for the datetime objects created, which are then
@@ -56,16 +59,15 @@
              :py:attr:`LogRecord.time` will be a datetime in local time zone
              (but not time zone aware)
          A `callable` returning datetime instances
             :py:attr:`LogRecord.time` will be a datetime created by
             :py:obj:`datetime_format` (possibly time zone aware)
 
     This function defaults to creating datetime objects in UTC time,
-    using `datetime.utcnow()
-    <http://docs.python.org/3/library/datetime.html#datetime.datetime.utcnow>`_,
+    using :func:`datetime.utcnow`,
     so that logbook logs all times in UTC time by default.  This is
     recommended in case you have multiple software modules or
     instances running in different servers in different time zones, as
     it makes it simple and less error prone to correlate logging
     across the different servers.
 
     On the other hand if all your software modules are running in the
@@ -75,15 +77,15 @@
     logging can be enabled like this::
 
        import logbook
        from datetime import datetime
        logbook.set_datetime_format("local")
 
     Other uses rely on your supplied :py:obj:`datetime_format`.
-    Using `pytz <https://pypi.org/pypi/pytz>`_ for example::
+    Using `pytz <https://pypi.org/project/pytz>`_ for example::
 
         from datetime import datetime
         import logbook
         import pytz
 
         def utc_tz():
             return datetime.now(tz=pytz.utc)
@@ -94,106 +96,98 @@
     if datetime_format == "utc":
         _datetime_factory = datetime.utcnow
     elif datetime_format == "local":
         _datetime_factory = datetime.now
     elif callable(datetime_format):
         inst = datetime_format()
         if not isinstance(inst, datetime):
-            raise ValueError("Invalid callable value, valid callable "
-                             "should return datetime.datetime instances, "
-                             "not %r" % (type(inst),))
+            raise ValueError(
+                "Invalid callable value, valid callable "
+                "should return datetime.datetime instances, "
+                "not %r" % (type(inst),)
+            )
         _datetime_factory = datetime_format
     else:
-        raise ValueError("Invalid value %r.  Valid values are 'utc' and "
-                         "'local'." % (datetime_format,))
+        raise ValueError(
+            "Invalid value %r.  Valid values are 'utc' and "
+            "'local'." % (datetime_format,)
+        )
+
 
 # make sure to sync these up with _speedups.pyx
 CRITICAL = 15
 ERROR = 14
 WARNING = 13
 NOTICE = 12
 INFO = 11
 DEBUG = 10
 TRACE = 9
 NOTSET = 0
 
 _level_names = {
-    CRITICAL:   'CRITICAL',
-    ERROR:      'ERROR',
-    WARNING:    'WARNING',
-    NOTICE:     'NOTICE',
-    INFO:       'INFO',
-    DEBUG:      'DEBUG',
-    TRACE:      'TRACE',
-    NOTSET:     'NOTSET'
+    CRITICAL: "CRITICAL",
+    ERROR: "ERROR",
+    WARNING: "WARNING",
+    NOTICE: "NOTICE",
+    INFO: "INFO",
+    DEBUG: "DEBUG",
+    TRACE: "TRACE",
+    NOTSET: "NOTSET",
 }
-_reverse_level_names = dict((v, k) for (k, v) in iteritems(_level_names))
+_reverse_level_names = {v: k for (k, v) in _level_names.items()}
 _missing = object()
 
 
-# on python 3 we can savely assume that frame filenames will be in
-# unicode, on Python 2 we have to apply a trick.
-if PY2:
-    def _convert_frame_filename(fn):
-        if isinstance(fn, unicode):
-            fn = fn.decode(sys.getfilesystemencoding() or 'utf-8',
-                           'replace')
-        return fn
-else:
-    def _convert_frame_filename(fn):
-        return fn
-
-
 def level_name_property():
     """Returns a property that reflects the level as name from
     the internal level attribute.
     """
 
     def _get_level_name(self):
         return get_level_name(self.level)
 
     def _set_level_name(self, level):
         self.level = lookup_level(level)
-    return property(_get_level_name, _set_level_name,
-                    doc='The level as unicode string')
+
+    return property(_get_level_name, _set_level_name, doc="The level as unicode string")
 
 
 def lookup_level(level):
     """Return the integer representation of a logging level."""
-    if isinstance(level, integer_types):
+    if isinstance(level, int):
         return level
     try:
         return _reverse_level_names[level]
     except KeyError:
-        raise LookupError('unknown level name %s' % level)
+        raise LookupError("unknown level name %s" % level)
 
 
 def get_level_name(level):
     """Return the textual representation of logging level 'level'."""
     try:
         return _level_names[level]
     except KeyError:
-        raise LookupError('unknown level')
+        raise LookupError("unknown level")
 
 
-class _ExceptionCatcher(object):
+class _ExceptionCatcher:
     """Helper for exception caught blocks."""
 
     def __init__(self, logger, args, kwargs):
         self.logger = logger
         self.args = args
         self.kwargs = kwargs
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, tb):
         if exc_type is not None:
             kwargs = self.kwargs.copy()
-            kwargs['exc_info'] = (exc_type, exc_value, tb)
+            kwargs["exc_info"] = (exc_type, exc_value, tb)
             self.logger.exception(*self.args, **kwargs)
         return True
 
 
 class ContextObject(StackedObject):
     """An object that can be bound to a context.  It is managed by the
     :class:`ContextStackManager`"""
@@ -206,42 +200,42 @@
     def push_greenlet(self):
         """Pushes the context object to the greenlet stack."""
         self.stack_manager.push_greenlet(self)
 
     def pop_greenlet(self):
         """Pops the context object from the stack."""
         popped = self.stack_manager.pop_greenlet()
-        assert popped is self, 'popped unexpected object'
+        assert popped is self, "popped unexpected object"
 
     def push_context(self):
         """Pushes the context object to the context stack."""
         self.stack_manager.push_context(self)
 
     def pop_context(self):
         """Pops the context object from the stack."""
         popped = self.stack_manager.pop_context()
-        assert popped is self, 'popped unexpected object'
+        assert popped is self, "popped unexpected object"
 
     def push_thread(self):
         """Pushes the context object to the thread stack."""
         self.stack_manager.push_thread(self)
 
     def pop_thread(self):
         """Pops the context object from the stack."""
         popped = self.stack_manager.pop_thread()
-        assert popped is self, 'popped unexpected object'
+        assert popped is self, "popped unexpected object"
 
     def push_application(self):
         """Pushes the context object to the application stack."""
         self.stack_manager.push_application(self)
 
     def pop_application(self):
         """Pops the context object from the stack."""
         popped = self.stack_manager.pop_application()
-        assert popped is self, 'popped unexpected object'
+        assert popped is self, "popped unexpected object"
 
 
 class NestedSetup(StackedObject):
     """A nested setup can be used to configure multiple handlers
     and processors at once.
     """
 
@@ -302,22 +296,24 @@
         """Called with the log record that should be overridden.  The default
         implementation calls :attr:`callback` if it is not `None`.
         """
         if self.callback is not None:
             self.callback(record)
 
 
-class _InheritedType(object):
+class _InheritedType:
     __slots__ = ()
 
     def __repr__(self):
-        return 'Inherit'
+        return "Inherit"
 
     def __reduce__(self):
-        return 'Inherit'
+        return "Inherit"
+
+
 Inherit = _InheritedType()
 
 
 class Flags(ContextObject):
     """Allows flags to be pushed on a flag stack.  Currently two flags
     are available:
 
@@ -342,14 +338,15 @@
         not be available when introspection is disabled.
 
     Example usage::
 
         with Flags(errors='silent'):
             ...
     """
+
     stack_manager = ContextStackManager()
 
     def __init__(self, **flags):
         self.__dict__.update(flags)
 
     @staticmethod
     def get_flag(flag, default=None):
@@ -364,27 +361,39 @@
 def _create_log_record(cls, dict):
     """Extra function for reduce because on Python 3 unbound methods
     can no longer be pickled.
     """
     return cls.from_dict(dict)
 
 
-class LogRecord(object):
+class LogRecord:
     """A LogRecord instance represents an event being logged.
 
     LogRecord instances are created every time something is logged. They
     contain all the information pertinent to the event being logged. The
     main information passed in is in msg and args
     """
-    _pullable_information = frozenset((
-        'func_name', 'module', 'filename', 'lineno', 'process_name', 'thread',
-        'thread_name', 'greenlet', 'formatted_exception', 'message',
-        'exception_name', 'exception_message'
-    ))
-    _noned_on_close = frozenset(('exc_info', 'frame', 'calling_frame'))
+
+    _pullable_information = frozenset(
+        (
+            "func_name",
+            "module",
+            "filename",
+            "lineno",
+            "process_name",
+            "thread",
+            "thread_name",
+            "greenlet",
+            "formatted_exception",
+            "message",
+            "exception_name",
+            "exception_message",
+        )
+    )
+    _noned_on_close = frozenset(("exc_info", "frame", "calling_frame"))
 
     #: can be overriden by a handler to not close the record.  This could
     #: lead to memory leaks so it should be used carefully.
     keep_open = False
 
     #: the time of the log record creation as :class:`datetime.datetime`
     #: object.  This information is unavailable until the record was
@@ -398,17 +407,27 @@
     #: a flag that is `True` when heavy initialization is no longer possible
     late = False
 
     #: a flag that is `True` when all the information was pulled from the
     #: information that becomes unavailable on close.
     information_pulled = False
 
-    def __init__(self, channel, level, msg, args=None, kwargs=None,
-                 exc_info=None, extra=None, frame=None, dispatcher=None,
-                 frame_correction=0):
+    def __init__(
+        self,
+        channel,
+        level,
+        msg,
+        args=None,
+        kwargs=None,
+        exc_info=None,
+        extra=None,
+        frame=None,
+        dispatcher=None,
+        frame_correction=0,
+    ):
         #: the name of the logger that created it or any other textual
         #: channel description.  This is a descriptive name and can be
         #: used for filtering.
         self.channel = channel
         #: The message of the log record as new-style format string.
         self.msg = msg
         #: the positional arguments for the format string.
@@ -427,16 +446,15 @@
             # theory, and it should be the same as exc_info=None
             exc_info = None
         self.exc_info = exc_info
         #: optional extra information as dictionary.  This is the place
         #: where custom log processors can attach custom context sensitive
         #: data.
 
-        # TODO: Replace the lambda with str when we remove support for python 2
-        self.extra = defaultdict(lambda: u'', extra or ())
+        self.extra = defaultdict(str, extra or ())
         #: If available, optionally the interpreter frame that pulled the
         #: heavy init.  This usually points to somewhere in the dispatcher.
         #: Might not be available for all calls and is removed when the log
         #: record is closed.
         self.frame = frame
         #: A positive integer telling the number of frames to go back from
         #: the frame which triggered the log entry. This is mainly useful
@@ -456,22 +474,28 @@
         date information will be for example.
 
         This is internally used by the record dispatching system and usually
         something not to worry about.
         """
         if self.heavy_initialized:
             return
-        assert not self.late, 'heavy init is no longer possible'
+        assert not self.late, "heavy init is no longer possible"
         self.heavy_initialized = True
         self.process = os.getpid()
         self.time = _datetime_factory()
-        if self.frame is None and Flags.get_flag('introspection', True):
+        if self.frame is None and Flags.get_flag("introspection", True):
             self.frame = sys._getframe(1)
         if self.exc_info is True:
             self.exc_info = sys.exc_info()
+        if isinstance(self.exc_info, BaseException):
+            self.exc_info = (
+                type(self.exc_info),
+                self.exc_info,
+                self.exc_info.__traceback__,
+            )
 
     def pull_information(self):
         """A helper function that pulls all frame-related information into
         the object so that this information is available after the log
         record was closed.
         """
         if self.information_pulled:
@@ -500,19 +524,19 @@
     def to_dict(self, json_safe=False):
         """Exports the log record into a dictionary without the information
         that cannot be safely serialized like interpreter frames and
         tracebacks.
         """
         self.pull_information()
         rv = {}
-        for key, value in iteritems(self.__dict__):
-            if key[:1] != '_' and key not in self._noned_on_close:
+        for key, value in self.__dict__.items():
+            if key[:1] != "_" and key not in self._noned_on_close:
                 rv[key] = value
         # the extra dict is exported as regular dict
-        rv['extra'] = dict(rv['extra'])
+        rv["extra"] = dict(rv["extra"])
         if json_safe:
             return to_safe_json(rv)
         return rv
 
     @classmethod
     def from_dict(cls, d):
         """Creates a log record from an exported dictionary.  This also
@@ -527,19 +551,18 @@
         instance in place.  Helpful for constructors.
         """
         self.__dict__.update(d)
         for key in self._noned_on_close:
             setattr(self, key, None)
         self._information_pulled = True
         self._channel = None
-        if isinstance(self.time, string_types):
+        if isinstance(self.time, str):
             self.time = parse_iso8601(self.time)
 
-        # TODO: Replace the lambda with str when we remove support for python 2`
-        self.extra = defaultdict(lambda: u'', self.extra)
+        self.extra = defaultdict(str, self.extra)
         return self
 
     def _format_message(self, msg, *args, **kwargs):
         """Called if the record's message needs to be formatted.
         Subclasses can implement their own formatting.
         """
         return msg.format(*args, **kwargs)
@@ -547,65 +570,68 @@
     @cached_property
     def message(self):
         """The formatted message."""
         if not (self.args or self.kwargs):
             return self.msg
         try:
             try:
-                return self._format_message(self.msg, *self.args,
-                                            **self.kwargs)
+                return self._format_message(self.msg, *self.args, **self.kwargs)
             except UnicodeDecodeError:
                 # Assume an unicode message but mixed-up args
-                msg = self.msg.encode('utf-8', 'replace')
+                msg = self.msg.encode("utf-8", "replace")
                 return self._format_message(msg, *self.args, **self.kwargs)
             except (UnicodeEncodeError, AttributeError):
                 # we catch AttributeError since if msg is bytes,
                 # it won't have the 'format' method
-                if (sys.exc_info()[0] is AttributeError
-                        and (PY2 or not isinstance(self.msg, bytes))):
+                if sys.exc_info()[0] is AttributeError and not isinstance(
+                    self.msg, bytes
+                ):
                     # this is not the case we thought it is...
                     raise
                 # Assume encoded message with unicode args.
                 # The assumption of utf8 as input encoding is just a guess,
                 # but this codepath is unlikely (if the message is a constant
                 # string in the caller's source file)
-                msg = self.msg.decode('utf-8', 'replace')
+                msg = self.msg.decode("utf-8", "replace")
                 return self._format_message(msg, *self.args, **self.kwargs)
 
         except Exception:
             # this obviously will not give a proper error message if the
             # information was not pulled and the log record no longer has
             # access to the frame.  But there is not much we can do about
             # that.
             e = sys.exc_info()[1]
-            errormsg = ('Could not format message with provided '
-                        'arguments: {err}\n  msg={msg!r}\n  '
-                        'args={args!r} \n  kwargs={kwargs!r}.\n'
-                        'Happened in file {file}, line {lineno}').format(
-                err=e, msg=self.msg, args=self.args,
-                kwargs=self.kwargs, file=self.filename,
-                lineno=self.lineno
+            errormsg = (
+                "Could not format message with provided "
+                "arguments: {err}\n  msg={msg!r}\n  "
+                "args={args!r} \n  kwargs={kwargs!r}.\n"
+                "Happened in file {file}, line {lineno}"
+            ).format(
+                err=e,
+                msg=self.msg,
+                args=self.args,
+                kwargs=self.kwargs,
+                file=self.filename,
+                lineno=self.lineno,
             )
-            if PY2:
-                errormsg = errormsg.encode('utf-8')
             raise TypeError(errormsg)
 
     level_name = level_name_property()
 
     @cached_property
     def calling_frame(self):
         """The frame in which the record has been created.  This only
         exists for as long the log record is not closed.
         """
         frm = self.frame
         globs = globals()
         while frm is not None and frm.f_globals is globs:
             frm = frm.f_back
 
-        for _ in xrange(self.frame_correction):
+        for _ in range(self.frame_correction):
             if frm is None:
                 break
 
             frm = frm.f_back
 
         return frm
 
@@ -623,27 +649,27 @@
     def module(self):
         """The name of the module that triggered the log call if
         available.  Requires a frame or that :meth:`pull_information`
         was called before.
         """
         cf = self.calling_frame
         if cf is not None:
-            return cf.f_globals.get('__name__')
+            return cf.f_globals.get("__name__")
 
     @cached_property
     def filename(self):
         """The filename of the module in which the record has been created.
         Requires a frame or that :meth:`pull_information` was called before.
         """
         cf = self.calling_frame
         if cf is not None:
             fn = cf.f_code.co_filename
-            if fn[:1] == '<' and fn[-1:] == '>':
+            if fn[:1] == "<" and fn[-1:] == ">":
                 return fn
-            return _convert_frame_filename(os.path.abspath(fn))
+            return os.path.abspath(fn)
 
     @cached_property
     def lineno(self):
         """The line number of the file in which the record has been created.
         Requires a frame or that :meth:`pull_information` was called before.
         """
         cf = self.calling_frame
@@ -677,70 +703,62 @@
     @cached_property
     def process_name(self):
         """The name of the process in which the record has been created."""
         # Errors may occur if multiprocessing has not finished loading
         # yet - e.g. if a custom import hook causes third-party code
         # to run when multiprocessing calls import. See issue 8200
         # for an example
-        mp = sys.modules.get('multiprocessing')
+        mp = sys.modules.get("multiprocessing")
         if mp is not None:  # pragma: no cover
             try:
                 return mp.current_process().name
             except Exception:
                 pass
 
     @cached_property
     def formatted_exception(self):
         """The formatted exception which caused this record to be created
         in case there was any.
         """
         if self.exc_info is not None and self.exc_info != (None, None, None):
-            rv = ''.join(traceback.format_exception(*self.exc_info))
-            if PY2:
-                rv = rv.decode('utf-8', 'replace')
+            rv = "".join(traceback.format_exception(*self.exc_info))
             return rv.rstrip()
 
     @cached_property
     def exception_name(self):
         """The name of the exception."""
         if self.exc_info is not None:
             cls = self.exc_info[0]
-            return u(cls.__module__ + '.' + cls.__name__)
+            return cls.__module__ + "." + cls.__name__
 
     @property
     def exception_shortname(self):
         """An abbreviated exception name (no import path)"""
-        return self.exception_name.rsplit('.')[-1]
+        return self.exception_name.rsplit(".")[-1]
 
     @cached_property
     def exception_message(self):
         """The message of the exception."""
         if self.exc_info is not None:
             val = self.exc_info[1]
-            try:
-                if PY2:
-                    return unicode(val)
-                else:
-                    return str(val)
-            except UnicodeError:
-                return str(val).decode('utf-8', 'replace')
+            return str(val)
 
     @property
     def dispatcher(self):
         """The dispatcher that created the log record.  Might not exist because
         a log record does not have to be created from a logger or other
         dispatcher to be handled by logbook.  If this is set, it will point to
         an object that implements the :class:`~logbook.base.RecordDispatcher`
         interface.
         """
         if self._dispatcher is not None:
             return self._dispatcher()
 
 
-class LoggerMixin(object):
+class LoggerMixin:
     """This mixin class defines and implements the "usual" logger
     interface (i.e. the descriptive logging functions).
 
     Classes using this mixin have to implement a :meth:`!handle` method which
     takes a :class:`~logbook.LogRecord` and passes it along.
     """
 
@@ -798,19 +816,19 @@
     def exception(self, *args, **kwargs):
         """Works exactly like :meth:`error` just that the message
         is optional and exception information is recorded.
         """
         if self.disabled or ERROR < self.level:
             return
         if not args:
-            args = ('Uncaught exception occurred',)
-        if 'exc_info' not in kwargs:
+            args = ("Uncaught exception occurred",)
+        if "exc_info" not in kwargs:
             exc_info = sys.exc_info()
-            assert exc_info[0] is not None, 'no exception occurred'
-            kwargs.setdefault('exc_info', sys.exc_info())
+            assert exc_info[0] is not None, "no exception occurred"
+            kwargs.setdefault("exc_info", sys.exc_info())
         return self.error(*args, **kwargs)
 
     def critical(self, *args, **kwargs):
         """Logs a :class:`~logbook.LogRecord` with the level set
         to :data:`~logbook.CRITICAL`.
         """
         if not self.disabled and CRITICAL >= self.level:
@@ -833,52 +851,53 @@
 
         .. code-block:: python
 
             with logger.catch_exceptions():
                 execute_code_that_might_fail()
         """
         if not args:
-            args = ('Uncaught exception occurred',)
+            args = ("Uncaught exception occurred",)
         return _ExceptionCatcher(self, args, kwargs)
 
     def enable(self):
         """Convenience method to enable this logger.
 
         :raises AttributeError: The disabled property is read-only, typically
                                 because it was overridden in a subclass.
 
         .. versionadded:: 1.0
         """
         try:
             self.disabled = False
         except AttributeError:
-            raise AttributeError('The disabled property is read-only.')
+            raise AttributeError("The disabled property is read-only.")
 
     def disable(self):
         """Convenience method to disable this logger.
 
         :raises AttributeError: The disabled property is read-only, typically
                                 because it was overridden in a subclass.
 
         .. versionadded:: 1.0
         """
         try:
             self.disabled = True
         except AttributeError:
-            raise AttributeError('The disabled property is read-only.')
+            raise AttributeError("The disabled property is read-only.")
 
     def _log(self, level, args, kwargs):
-        exc_info = kwargs.pop('exc_info', None)
-        extra = kwargs.pop('extra', None)
-        frame_correction = kwargs.pop('frame_correction', 0)
-        self.make_record_and_handle(level, args[0], args[1:], kwargs,
-                                    exc_info, extra, frame_correction)
+        exc_info = kwargs.pop("exc_info", None)
+        extra = kwargs.pop("extra", None)
+        frame_correction = kwargs.pop("frame_correction", 0)
+        self.make_record_and_handle(
+            level, args[0], args[1:], kwargs, exc_info, extra, frame_correction
+        )
 
 
-class RecordDispatcher(object):
+class RecordDispatcher:
     """A record dispatcher is the internal base class that implements
     the logic used by the :class:`~logbook.Logger`.
     """
 
     #: If this is set to `True` the dispatcher information will be suppressed
     #: for log records emitted from this logger.
     suppress_dispatcher = False
@@ -889,44 +908,55 @@
         #: list of handlers specific for this record dispatcher
         self.handlers = []
         #: optionally the name of the group this logger belongs to
         self.group = None
         #: the level of the record dispatcher as integer
         self.level = level
 
-    disabled = group_reflected_property('disabled', False)
-    level = group_reflected_property('level', NOTSET, fallback=NOTSET)
+    disabled = group_reflected_property("disabled", False)
+    level = group_reflected_property("level", NOTSET, fallback=NOTSET)
 
     def handle(self, record):
         """Call the handlers for the specified record.  This is
         invoked automatically when a record should be handled.
         The default implementation checks if the dispatcher is disabled
         and if the record level is greater than the level of the
         record dispatcher.  In that case it will call the handlers
         (:meth:`call_handlers`).
         """
         if not self.disabled and record.level >= self.level:
             self.call_handlers(record)
 
-    def make_record_and_handle(self, level, msg, args, kwargs, exc_info,
-                               extra, frame_correction):
+    def make_record_and_handle(
+        self, level, msg, args, kwargs, exc_info, extra, frame_correction
+    ):
         """Creates a record from some given arguments and heads it
         over to the handling system.
         """
         # The channel information can be useful for some use cases which is
         # why we keep it on there.  The log record however internally will
         # only store a weak reference to the channel, so it might disappear
         # from one instruction to the other.  It will also disappear when
         # a log record is transmitted to another process etc.
         channel = None
         if not self.suppress_dispatcher:
             channel = self
 
-        record = LogRecord(self.name, level, msg, args, kwargs, exc_info,
-                           extra, None, channel, frame_correction)
+        record = LogRecord(
+            self.name,
+            level,
+            msg,
+            args,
+            kwargs,
+            exc_info,
+            extra,
+            None,
+            channel,
+            frame_correction,
+        )
 
         # after handling the log record is closed which will remove some
         # referenes that would require a GC run on cpython.  This includes
         # the current stack frame, exception information.  However there are
         # some use cases in keeping the records open for a little longer.
         # For example the test handler keeps log records open until the
         # test handler is closed to allow assertions based on stack frames
@@ -953,16 +983,17 @@
         # and processed if at least one of the handlers has a higher
         # level than the record and that handler is not a black hole.
         record_initialized = False
 
         # Both logger attached handlers as well as context specific
         # handlers are handled one after another.  The latter also
         # include global handlers.
-        for handler in chain(self.handlers,
-                             Handler.stack_manager.iter_context_objects()):
+        for handler in chain(
+            self.handlers, Handler.stack_manager.iter_context_objects()
+        ):
             # skip records that this handler is not interested in based
             # on the record and handler level or in case this method was
             # overridden on some custom logic.
             if not handler.should_handle(record):
                 continue
 
             # first case of blackhole (without filter).
@@ -981,16 +1012,15 @@
                 record_initialized = True
 
             # a filter can still veto the handling of the record.  This
             # however is already operating on an initialized and processed
             # record.  The impact is that filters are slower than the
             # handler's should_handle function in case there is no default
             # handler that would handle the record (delayed init).
-            if (handler.filter is not None
-                    and not handler.filter(record, handler)):
+            if handler.filter is not None and not handler.filter(record, handler):
                 continue
 
             # We might have a filter, so now that we know we *should* handle
             # this record, we should consider the case of us being a black hole...
             if handler.blackhole:
                 break
 
@@ -1022,15 +1052,15 @@
     A logger internally is a subclass of a
     :class:`~logbook.base.RecordDispatcher` that implements the actual
     logic.  If you want to implement a custom logger class, have a look
     at the interface of that class as well.
     """
 
 
-class LoggerGroup(object):
+class LoggerGroup:
     """A LoggerGroup represents a group of loggers.  It cannot emit log
     messages on its own but it can be used to set the disabled flag and
     log level of all loggers in the group.
 
     Furthermore the :meth:`process_record` method of the group is called
     by any logger in the group which by default calls into the
     :attr:`processor` callback function.
@@ -1053,15 +1083,15 @@
         self.disabled = False
         #: an optional callback function that is executed to process
         #: the log records of all loggers in the group.
         self.processor = processor
 
     def add_logger(self, logger):
         """Adds a logger to this group."""
-        assert logger.group is None, 'Logger already belongs to a group'
+        assert logger.group is None, "Logger already belongs to a group"
         logger.group = self
         self.loggers.append(logger)
 
     def remove_logger(self, logger):
         """Removes a logger from the group."""
         self.loggers.remove(logger)
         logger.group = None
@@ -1084,15 +1114,15 @@
                                 overridden in a subclass.
 
         .. versionadded:: 1.0
         """
         self.disabled = False
         if force:
             for logger in self.loggers:
-                rv = getattr(logger, '_disabled', _missing)
+                rv = getattr(logger, "_disabled", _missing)
                 if rv is not _missing:
                     logger.enable()
 
     def disable(self, force=False):
         """Convenience method to disable this group.
 
         :param force: Force disable loggers that were explicitly set.
@@ -1102,24 +1132,25 @@
                                 overridden in a subclass.
 
         .. versionadded:: 1.0
         """
         self.disabled = True
         if force:
             for logger in self.loggers:
-                rv = getattr(logger, '_disabled', _missing)
+                rv = getattr(logger, "_disabled", _missing)
                 if rv is not _missing:
                     logger.disable()
 
 
 _default_dispatcher = RecordDispatcher()
 
 
 def dispatch_record(record):
     """Passes a record on to the handlers on the stack.  This is useful when
     log records are created programmatically and already have all the
     information attached and should be dispatched independent of a logger.
     """
     _default_dispatcher.call_handlers(record)
 
+
 # at that point we are safe to import handler
-from logbook.handlers import Handler # isort:skip
+from logbook.handlers import Handler  # isort:skip
```

### Comparing `Logbook-1.5.3/logbook/compat.py` & `Logbook-1.6.0/src/logbook/compat.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,24 @@
-# -*- coding: utf-8 -*-
 """
     logbook.compat
     ~~~~~~~~~~~~~~
 
     Backwards compatibility with stdlib's logging package and the
     warnings module.
 
     :copyright: (c) 2010 by Armin Ronacher, Georg Brandl.
     :license: BSD, see LICENSE for more details.
 """
-import collections
 import logging
 import sys
 import warnings
-from datetime import date, datetime
+from collections.abc import Mapping
+from datetime import date, datetime, timezone
 
 import logbook
-from logbook.helpers import u, string_types, iteritems, collections_abc
-
-_epoch_ord = date(1970, 1, 1).toordinal()
 
 
 def redirect_logging(set_root_logger_level=True):
     """Permanently redirects logging to the stdlib.  This also
     removes all otherwise registered handlers on root logger of
     the logging system but leaves the other loggers untouched.
 
@@ -32,23 +28,24 @@
     """
     del logging.root.handlers[:]
     logging.root.addHandler(RedirectLoggingHandler())
     if set_root_logger_level:
         logging.root.setLevel(logging.DEBUG)
 
 
-class redirected_logging(object):
+class redirected_logging:
     """Temporarily redirects logging for all threads and reverts
     it later to the old handlers.  Mainly used by the internal
     unittests::
 
         from logbook.compat import redirected_logging
         with redirected_logging():
             ...
     """
+
     def __init__(self, set_root_logger_level=True):
         self.old_handlers = logging.root.handlers[:]
         self.old_level = logging.root.level
         self.set_root_logger_level = set_root_logger_level
 
     def start(self):
         redirect_logging(self.set_root_logger_level)
@@ -58,15 +55,14 @@
         logging.root.setLevel(self.old_level)
 
     __enter__ = start
     __exit__ = end
 
 
 class LoggingCompatRecord(logbook.LogRecord):
-
     def _format_message(self, msg, *args, **kwargs):
         if kwargs:
             assert not args
             return msg % kwargs
         else:
             assert not kwargs
             return msg % tuple(args)
@@ -98,29 +94,48 @@
 
     def find_extra(self, old_record):
         """Tries to find custom data from the old logging record.  The
         return value is a dictionary that is merged with the log record
         extra dictionaries.
         """
         rv = vars(old_record).copy()
-        for key in ('name', 'msg', 'args', 'levelname', 'levelno',
-                    'pathname', 'filename', 'module', 'exc_info',
-                    'exc_text', 'lineno', 'funcName', 'created',
-                    'msecs', 'relativeCreated', 'thread', 'threadName',
-                    'greenlet', 'processName', 'process'):
+        for key in (
+            "name",
+            "msg",
+            "args",
+            "levelname",
+            "levelno",
+            "pathname",
+            "filename",
+            "module",
+            "exc_info",
+            "exc_text",
+            "lineno",
+            "funcName",
+            "created",
+            "msecs",
+            "relativeCreated",
+            "thread",
+            "threadName",
+            "greenlet",
+            "processName",
+            "process",
+        ):
             rv.pop(key, None)
         return rv
 
     def find_caller(self, old_record):
         """Tries to find the caller that issued the call."""
         frm = sys._getframe(2)
         while frm is not None:
-            if (frm.f_globals is globals() or
-                    frm.f_globals is logbook.base.__dict__ or
-                    frm.f_globals is logging.__dict__):
+            if (
+                frm.f_globals is globals()
+                or frm.f_globals is logbook.base.__dict__
+                or frm.f_globals is logging.__dict__
+            ):
                 frm = frm.f_back
             else:
                 return frm
 
     def convert_time(self, timestamp):
         """Converts the UNIX timestamp of the old record into a
         datetime object as used by logbook.
@@ -129,23 +144,27 @@
 
     def convert_record(self, old_record):
         """Converts an old logging record into a logbook log record."""
         args = old_record.args
         kwargs = None
 
         # Logging allows passing a mapping object, in which case args will be a mapping.
-        if isinstance(args, collections_abc.Mapping):
+        if isinstance(args, Mapping):
             kwargs = args
             args = None
-        record = LoggingCompatRecord(old_record.name,
-                                     self.convert_level(old_record.levelno),
-                                     old_record.msg, args,
-                                     kwargs, old_record.exc_info,
-                                     self.find_extra(old_record),
-                                     self.find_caller(old_record))
+        record = LoggingCompatRecord(
+            old_record.name,
+            self.convert_level(old_record.levelno),
+            old_record.msg,
+            args,
+            kwargs,
+            old_record.exc_info,
+            self.find_extra(old_record),
+            self.find_caller(old_record),
+        )
         record.time = self.convert_time(old_record.created)
         return record
 
     def emit(self, record):
         logbook.dispatch_record(self.convert_record(record))
 
 
@@ -160,20 +179,19 @@
     Example usage::
 
         from logbook.compat import LoggingHandler, warn
         with LoggingHandler():
             warn('This goes to logging')
     """
 
-    def __init__(self, logger=None, level=logbook.NOTSET, filter=None,
-                 bubble=False):
+    def __init__(self, logger=None, level=logbook.NOTSET, filter=None, bubble=False):
         logbook.Handler.__init__(self, level, filter, bubble)
         if logger is None:
             logger = logging.getLogger()
-        elif isinstance(logger, string_types):
+        elif isinstance(logger, str):
             logger = logging.getLogger(logger)
         self.logger = logger
 
     def get_logger(self, record):
         """Returns the logger to use for this record.  This implementation
         always return :attr:`logger`.
         """
@@ -189,36 +207,32 @@
             return logging.WARNING
         if level >= logbook.INFO:
             return logging.INFO
         return logging.DEBUG
 
     def convert_time(self, dt):
         """Converts a datetime object into a timestamp."""
-        year, month, day, hour, minute, second = dt.utctimetuple()[:6]
-        days = date(year, month, 1).toordinal() - _epoch_ord + day - 1
-        hours = days * 24 + hour
-        minutes = hours * 60 + minute
-        seconds = minutes * 60 + second
-        return seconds
+        if dt.tzinfo is None:
+            # Logbook uses naive datetimes to represent UTC (utcnow)
+            return dt.replace(tzinfo=timezone.utc).timestamp()
+        return dt.timestamp()
 
     def convert_record(self, old_record):
         """Converts a record from logbook to logging."""
-        if sys.version_info >= (2, 5):
-            # make sure 2to3 does not screw this up
-            optional_kwargs = {'func': getattr(old_record, 'func_name')}
-        else:
-            optional_kwargs = {}
-        record = logging.LogRecord(old_record.channel,
-                                   self.convert_level(old_record.level),
-                                   old_record.filename,
-                                   old_record.lineno,
-                                   old_record.message,
-                                   (), old_record.exc_info,
-                                   **optional_kwargs)
-        for key, value in iteritems(old_record.extra):
+        record = logging.LogRecord(
+            old_record.channel,
+            self.convert_level(old_record.level),
+            old_record.filename,
+            old_record.lineno,
+            old_record.message,
+            (),
+            old_record.exc_info,
+            func=old_record.func_name,
+        )
+        for key, value in old_record.extra.items():
             record.__dict__.setdefault(key, value)
         record.created = self.convert_time(old_record.time)
         return record
 
     def emit(self, record):
         self.get_logger(record).handle(self.convert_record(record))
 
@@ -231,15 +245,15 @@
 
         from logbook.compat import redirect_warnings
         redirect_warnings()
     """
     redirected_warnings().__enter__()
 
 
-class redirected_warnings(object):
+class redirected_warnings:
     """A context manager that copies and restores the warnings filter upon
     exiting the context, and logs warnings using the logbook system.
 
     The :attr:`~logbook.LogRecord.channel` attribute of the log record will be
     the import name of the warning.
 
     Example usage:
@@ -253,23 +267,20 @@
             warn(DeprecationWarning('logging should be deprecated'))
     """
 
     def __init__(self):
         self._entered = False
 
     def message_to_unicode(self, message):
-        try:
-            return u(str(message))
-        except UnicodeError:
-            return str(message).decode('utf-8', 'replace')
+        return str(message)
 
     def make_record(self, message, exception, filename, lineno):
         category = exception.__name__
-        if exception.__module__ not in ('exceptions', 'builtins'):
-            category = exception.__module__ + '.' + category
+        if exception.__module__ not in ("exceptions", "builtins"):
+            category = exception.__module__ + "." + category
         rv = logbook.LogRecord(category, logbook.WARNING, message)
         # we don't know the caller, but we get that information from the
         # warning system.  Just attach them.
         rv.filename = filename
         rv.lineno = lineno
         return rv
 
@@ -277,19 +288,19 @@
         if self._entered:  # pragma: no cover
             raise RuntimeError("Cannot enter %r twice" % self)
         self._entered = True
         self._filters = warnings.filters
         warnings.filters = self._filters[:]
         self._showwarning = warnings.showwarning
 
-        def showwarning(message, category, filename, lineno,
-                        file=None, line=None):
+        def showwarning(message, category, filename, lineno, file=None, line=None):
             message = self.message_to_unicode(message)
             record = self.make_record(message, category, filename, lineno)
             logbook.dispatch_record(record)
+
         warnings.showwarning = showwarning
 
     def end(self, etype=None, evalue=None, tb=None):
         if not self._entered:  # pragma: no cover
             raise RuntimeError("Cannot exit %r without entering first" % self)
         warnings.filters = self._filters
         warnings.showwarning = self._showwarning
```

### Comparing `Logbook-1.5.3/logbook/concurrency.py` & `Logbook-1.6.0/src/logbook/concurrency.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+from contextvars import ContextVar
+from itertools import count
+from threading import current_thread
+
 has_gevent = True
 use_gevent = False
 try:
     import gevent
 
     def enable_gevent():
         global use_gevent
@@ -10,57 +14,58 @@
     def _disable_gevent():  # for testing
         global use_gevent
         use_gevent = False
 
     def is_gevent_enabled():
         global use_gevent
         return use_gevent
+
 except ImportError:
     has_gevent = False
 
     def enable_gevent():
         pass
 
     def _disable_gevent():
         pass
 
     def is_gevent_enabled():
         return False
 
 
+def thread_get_name():
+    return current_thread().name
+
+
 if has_gevent:
     from gevent.monkey import get_original as _get_original
-    ThreadLock = _get_original('threading', 'Lock')
-    ThreadRLock = _get_original('threading', 'RLock')
-    try:
-        thread_get_ident = _get_original('threading', 'get_ident')
-    except AttributeError:
-        # In 2.7, this is called _get_ident
-        thread_get_ident = _get_original('threading', '_get_ident')
-    thread_local = _get_original('threading', 'local')
 
-    from gevent.thread import get_ident as greenlet_get_ident
+    ThreadLock = _get_original("threading", "Lock")
+    ThreadRLock = _get_original("threading", "RLock")
+    thread_get_ident = _get_original("threading", "get_ident")
+    thread_local = _get_original("threading", "local")
+
     from gevent.local import local as greenlet_local
     from gevent.lock import BoundedSemaphore
-    from gevent.threading import __threading__
-
-    def thread_get_name():
-        return __threading__.currentThread().getName()
+    from gevent.thread import get_ident as greenlet_get_ident
 
-    class GreenletRLock(object):
+    class GreenletRLock:
         def __init__(self):
             self._thread_local = thread_local()
             self._owner = None
             self._wait_queue = []
             self._count = 0
 
         def __repr__(self):
             owner = self._owner
-            return "<%s owner=%r count=%d>" % (self.__class__.__name__, owner,
-                                               self._count)
+            return "<%s owner=%r count=%d>" % (
+                self.__class__.__name__,
+                owner,
+                self._count,
+            )
 
         def acquire(self, blocking=1):
             tid = thread_get_ident()
             gid = greenlet_get_ident()
             tid_gid = (tid, gid)
 
             # We trust the GIL here so we can do this comparison w/o locking.
@@ -115,40 +120,34 @@
 
         __enter__ = acquire
 
         def __exit__(self, t, v, tb):
             self.release()
 
         def _get_greenlet_lock(self):
-            if not hasattr(self._thread_local, 'greenlet_lock'):
+            if not hasattr(self._thread_local, "greenlet_lock"):
                 greenlet_lock = self._thread_local.greenlet_lock = BoundedSemaphore(1)
             else:
                 greenlet_lock = self._thread_local.greenlet_lock
             return greenlet_lock
 
         def _is_owned(self):
             return self._owner == (thread_get_ident(), greenlet_get_ident())
-else:
-    from threading import (
-        Lock as ThreadLock, RLock as ThreadRLock, currentThread)
-    try:
-        from thread import (
-            get_ident as thread_get_ident, _local as thread_local)
-    except ImportError:
-        from _thread import (
-            get_ident as thread_get_ident, _local as thread_local)
 
-    def thread_get_name():
-        return currentThread().getName()
+else:
+    from threading import Lock as ThreadLock
+    from threading import RLock as ThreadRLock
+    from threading import get_ident as thread_get_ident
+    from threading import local as thread_local
 
     greenlet_get_ident = thread_get_ident
 
     greenlet_local = thread_local
 
-    class GreenletRLock(object):
+    class GreenletRLock:
         def acquire(self):
             pass
 
         def release(self):
             pass
 
         def __enter__(self):
@@ -162,55 +161,26 @@
     global use_gevent
     if use_gevent:
         return GreenletRLock()
     else:
         return ThreadRLock()
 
 
-has_contextvars = True
-try:
-    import contextvars
-except ImportError:
-    has_contextvars = False
-
-if has_contextvars:
-    from contextvars import ContextVar
-    from itertools import count
-
-    context_ident_counter = count()
-    context_ident = ContextVar('context_ident')
-
-    def context_get_ident():
-        try:
-            return context_ident.get()
-        except LookupError:
-            ident = 'context-%s' % next(context_ident_counter)
-            context_ident.set(ident)
-            return ident
-
-    def is_context_enabled():
-        try:
-            context_ident.get()
-            return True
-        except LookupError:
-            return False
-
-else:
-    class ContextVar(object):
-        def __init__(self, name):
-            self.name = name
-            self.local = thread_local()
-
-        def set(self, value):
-            self.local = value
+context_ident_counter = count()
+context_ident = ContextVar("context_ident")
 
-        def get(self, default=None):
-            if self.local is None:
-                return default
 
-            return default
+def context_get_ident():
+    try:
+        return context_ident.get()
+    except LookupError:
+        ident = "context-%s" % next(context_ident_counter)
+        context_ident.set(ident)
+        return ident
 
-    def context_get_ident():
-        return 1
 
-    def is_context_enabled():
+def is_context_enabled():
+    try:
+        context_ident.get()
+        return True
+    except LookupError:
         return False
```

### Comparing `Logbook-1.5.3/logbook/handlers.py` & `Logbook-1.6.0/src/logbook/handlers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,124 +1,143 @@
-# -*- coding: utf-8 -*-
 """
     logbook.handlers
     ~~~~~~~~~~~~~~~~
 
     The handler interface and builtin handlers.
 
     :copyright: (c) 2010 by Armin Ronacher, Georg Brandl.
     :license: BSD, see LICENSE for more details.
 """
-import io
-import os
-import re
-import sys
-import stat
 import errno
-import socket
 import gzip
 import math
-try:
-    from hashlib import sha1
-except ImportError:
-    from sha import new as sha1
+import os
+import re
+import socket
+import stat
+import sys
 import traceback
-import collections
-from datetime import datetime, timedelta
 from collections import deque
+from collections.abc import Iterable, Mapping
+from datetime import datetime, timedelta
+from hashlib import sha1
 from textwrap import dedent
 
 from logbook.base import (
-    CRITICAL, ERROR, WARNING, NOTICE, INFO, DEBUG, TRACE, NOTSET, level_name_property,
-    _missing, lookup_level, Flags, ContextObject, ContextStackManager,
-    _datetime_factory)
-from logbook.helpers import (
-    rename, b, _is_text_stream, is_unicode, PY2, zip, xrange, string_types, collections_abc,
-    integer_types, reraise, u, with_metaclass)
+    CRITICAL,
+    DEBUG,
+    ERROR,
+    INFO,
+    NOTICE,
+    NOTSET,
+    TRACE,
+    WARNING,
+    ContextObject,
+    ContextStackManager,
+    Flags,
+    _datetime_factory,
+    _missing,
+    level_name_property,
+    lookup_level,
+)
 from logbook.concurrency import new_fine_grained_lock
+from logbook.helpers import rename
 
-DEFAULT_FORMAT_STRING = u(
-    '[{record.time:%Y-%m-%d %H:%M:%S.%f%z}] '
-    '{record.level_name}: {record.channel}: {record.message}')
+DEFAULT_FORMAT_STRING = (
+    "[{record.time:%Y-%m-%d %H:%M:%S.%f%z}] "
+    "{record.level_name}: {record.channel}: {record.message}"
+)
 
-SYSLOG_FORMAT_STRING = u('{record.channel}: {record.message}')
-NTLOG_FORMAT_STRING = dedent(u('''
+SYSLOG_FORMAT_STRING = "{record.channel}: {record.message}"
+NTLOG_FORMAT_STRING = dedent(
+    """
     Message Level: {record.level_name}
     Location: {record.filename}:{record.lineno}
     Module: {record.module}
     Function: {record.func_name}
     Exact Time: {record.time:%Y-%m-%d %H:%M:%S}
 
     Event provided Message:
 
     {record.message}
-    ''')).lstrip()
+    """
+).lstrip()
 
-TEST_FORMAT_STRING = u('[{record.level_name}] {record.channel}: {record.message}')
-MAIL_FORMAT_STRING = dedent(u('''
+TEST_FORMAT_STRING = "[{record.level_name}] {record.channel}: {record.message}"
+MAIL_FORMAT_STRING = dedent(
+    """
     Subject: {handler.subject}
 
     Message type:       {record.level_name}
     Location:           {record.filename}:{record.lineno}
     Module:             {record.module}
     Function:           {record.func_name}
     Time:               {record.time:%Y-%m-%d %H:%M:%S}
 
     Message:
 
     {record.message}
-    ''')).lstrip()
+    """
+).lstrip()
 
-MAIL_RELATED_FORMAT_STRING = dedent(u('''
+MAIL_RELATED_FORMAT_STRING = dedent(
+    """
     Message type:       {record.level_name}
     Location:           {record.filename}:{record.lineno}
     Module:             {record.module}
     Function:           {record.func_name}
     {record.message}
-    ''')).lstrip()
+    """
+).lstrip()
 
 SYSLOG_PORT = 514
 
 REGTYPE = type(re.compile("I'm a regular expression!"))
 
 
 def create_syshandler(application_name, level=NOTSET):
     """Creates the handler the operating system provides.  On Unix systems
     this creates a :class:`SyslogHandler`, on Windows sytems it will
     create a :class:`NTEventLogHandler`.
     """
-    if os.name == 'nt':
+    if os.name == "nt":
         return NTEventLogHandler(application_name, level=level)
     return SyslogHandler(application_name, level=level)
 
 
 class _HandlerType(type):
     """The metaclass of handlers injects a destructor if the class has an
     overridden close method.  This makes it possible that the default
     handler class as well as all subclasses that don't need cleanup to be
     collected with less overhead.
     """
 
     def __new__(cls, name, bases, d):
         # aha, that thing has a custom close method.  We will need a magic
         # __del__ for it to be called on cleanup.
-        if (bases != (ContextObject,) and 'close' in d and '__del__' not in d
-                and not any(hasattr(x, '__del__') for x in bases)):
+        if (
+            bases != (ContextObject,)
+            and "close" in d
+            and "__del__" not in d
+            and not any(hasattr(x, "__del__") for x in bases)
+        ):
+
             def _magic_del(self):
                 try:
                     self.close()
                 except Exception:
                     # del is also invoked when init fails, so we better just
                     # ignore any exception that might be raised here
                     pass
-            d['__del__'] = _magic_del
+
+            d["__del__"] = _magic_del
         return type.__new__(cls, name, bases, d)
 
 
-class Handler(with_metaclass(_HandlerType), ContextObject):
+class Handler(ContextObject, metaclass=_HandlerType):
     """Handler instances dispatch logging events to specific destinations.
 
     The base handler class. Acts as a placeholder which defines the Handler
     interface. Handlers can optionally use Formatter instances to format
     records as desired. By default, no formatter is specified; in this case,
     the 'raw' message as determined by record.message is logged.
 
@@ -153,14 +172,15 @@
     on the handler itself if not using gevent::
 
         with handler:
             ...
 
     If gevent is enabled, the handler is aliased to `greenletbound`.
     """
+
     stack_manager = ContextStackManager()
 
     #: a flag for this handler that can be set to `True` for handlers that
     #: are consuming log records but are not actually displaying it.  This
     #: flag is set for the :class:`NullHandler` for instance.
     blackhole = False
 
@@ -286,70 +306,73 @@
     def handle_error(self, record, exc_info):
         """Handle errors which occur during an emit() call.  The behaviour of
         this function depends on the current `errors` setting.
 
         Check :class:`Flags` for more information.
         """
         try:
-            behaviour = Flags.get_flag('errors', 'print')
-            if behaviour == 'raise':
-                reraise(exc_info[0], exc_info[1], exc_info[2])
-            elif behaviour == 'print':
+            behaviour = Flags.get_flag("errors", "print")
+            if behaviour == "raise":
+                raise exc_info[1]
+            elif behaviour == "print":
                 traceback.print_exception(*(exc_info + (None, sys.stderr)))
-                sys.stderr.write('Logged from file %s, line %s\n' % (
-                                 record.filename, record.lineno))
-        except IOError:
+                sys.stderr.write(
+                    "Logged from file {}, line {}\n".format(
+                        record.filename, record.lineno
+                    )
+                )
+        except OSError:
             pass
 
 
 class NullHandler(Handler):
     """A handler that does nothing.
 
     Useful to silence logs above a certain location in the handler stack::
 
         handler = NullHandler()
         handler.push_application()
 
     NullHandlers swallow all logs sent to them, and do not bubble them onwards.
 
     """
+
     blackhole = True
 
     def __init__(self, level=NOTSET, filter=None):
-        super(NullHandler, self).__init__(level=level, filter=filter,
-                                          bubble=False)
+        super().__init__(level=level, filter=filter, bubble=False)
 
 
 class WrapperHandler(Handler):
     """A class that can wrap another handler and redirect all calls to the
     wrapped handler::
 
         handler = WrapperHandler(other_handler)
 
     Subclasses should override the :attr:`_direct_attrs` attribute as
     necessary.
     """
 
     #: a set of direct attributes that are not forwarded to the inner
     #: handler.  This has to be extended as necessary.
-    _direct_attrs = frozenset(['handler'])
+    _direct_attrs = frozenset(["handler"])
 
     def __init__(self, handler):
         self.handler = handler
 
     def __getattr__(self, name):
         return getattr(self.handler, name)
 
     def __setattr__(self, name, value):
         if name in self._direct_attrs:
             return Handler.__setattr__(self, name, value)
         setattr(self.handler, name, value)
 
 
-class StringFormatter(object):
+class StringFormatter:
     """Many handlers format the log entries to text format.  This is done
     by a callable that is passed a log record and returns an unicode
     string.  The default formatter for this is implemented as a class so
     that it becomes possible to hook into every aspect of the formatting
     process.
     """
 
@@ -368,34 +391,34 @@
 
     def format_record(self, record, handler):
         try:
             return self._formatter.format(record=record, handler=handler)
         except UnicodeEncodeError:
             # self._formatter is a str, but some of the record items
             # are unicode
-            fmt = self._formatter.decode('ascii', 'replace')
+            fmt = self._formatter.decode("ascii", "replace")
             return fmt.format(record=record, handler=handler)
         except UnicodeDecodeError:
             # self._formatter is unicode, but some of the record items
             # are non-ascii str
-            fmt = self._formatter.encode('ascii', 'replace')
+            fmt = self._formatter.encode("ascii", "replace")
             return fmt.format(record=record, handler=handler)
 
     def format_exception(self, record):
         return record.formatted_exception
 
     def __call__(self, record, handler):
         line = self.format_record(record, handler)
         exc = self.format_exception(record)
         if exc:
-            line += u('\n') + exc
+            line += "\n" + exc
         return line
 
 
-class StringFormatterHandlerMixin(object):
+class StringFormatterHandlerMixin:
     """A mixin for handlers that provides a default integration for the
     :class:`~logbook.StringFormatter` class.  This is used for all handlers
     by default that log text to a destination.
     """
 
     #: a class attribute for the default format string to use if the
     #: constructor was invoked with `None`.
@@ -422,37 +445,35 @@
         else:
             self.formatter = self.formatter_class(value)
 
     format_string = property(_get_format_string, _set_format_string)
     del _get_format_string, _set_format_string
 
 
-class HashingHandlerMixin(object):
+class HashingHandlerMixin:
     """Mixin class for handlers that are hashing records."""
 
     def hash_record_raw(self, record):
         """Returns a hashlib object with the hash of the record."""
         hash = sha1()
-        hash.update(('%d\x00' % record.level).encode('ascii'))
-        hash.update((record.channel or u('')).encode('utf-8') + b('\x00'))
-        hash.update(record.filename.encode('utf-8') + b('\x00'))
-        hash.update(b(str(record.lineno)))
+        hash.update(("%d\x00" % record.level).encode("ascii"))
+        hash.update((record.channel or "").encode("utf-8") + b"\x00")
+        hash.update(record.filename.encode("utf-8") + b"\x00")
+        hash.update(str(record.lineno).encode("utf-8"))
         return hash
 
     def hash_record(self, record):
         """Returns a hash for a record to keep it apart from other records.
         This is used for the `record_limit` feature.  By default
         The level, channel, filename and location are hashed.
 
         Calls into :meth:`hash_record_raw`.
         """
         return self.hash_record_raw(record).hexdigest()
 
-_NUMBER_TYPES = integer_types + (float,)
-
 
 class LimitingHandlerMixin(HashingHandlerMixin):
     """Mixin class for handlers that want to limit emitting records.
 
     In the default setting it delivers all log records but it can be set up
     to not send more than n mails for the same record each hour to not
     overload an inbox and the network in case a message is triggered multiple
@@ -465,15 +486,15 @@
 
     def __init__(self, record_limit, record_delta):
         self.record_limit = record_limit
         self._limit_lock = new_fine_grained_lock()
         self._record_limits = {}
         if record_delta is None:
             record_delta = timedelta(seconds=60)
-        elif isinstance(record_delta, _NUMBER_TYPES):
+        elif isinstance(record_delta, (int, float)):
             record_delta = timedelta(seconds=record_delta)
         self.record_delta = record_delta
 
     def check_delivery(self, record):
         """Helper function to check if data should be delivered by this
         handler.  It returns a tuple in the form ``(suppression_count,
         allow)``.  The first one is the number of items that were not delivered
@@ -492,19 +513,20 @@
                 last_count, suppression_count = self._record_limits[hash]
                 if last_count + self.record_delta < now:
                     allow_delivery = True
                 else:
                     first_count = last_count
                     old_count = suppression_count
 
-            if (not suppression_count and
-                    len(self._record_limits) >= self.max_record_cache):
+            if (
+                not suppression_count
+                and len(self._record_limits) >= self.max_record_cache
+            ):
                 cache_items = sorted(self._record_limits.items())
-                del cache_items[:int(self._record_limits)
-                                * self.record_cache_prune]
+                del cache_items[: int(self._record_limits) * self.record_cache_prune]
                 self._record_limits = dict(cache_items)
 
             self._record_limits[hash] = (first_count, old_count + 1)
 
             if allow_delivery is None:
                 allow_delivery = old_count < self.record_limit
             return suppression_count, allow_delivery
@@ -525,16 +547,23 @@
 
     .. admonition:: Notes on the encoding
 
        On Python 3, the encoding parameter is only used if a stream was
        passed that was opened in binary mode.
     """
 
-    def __init__(self, stream, level=NOTSET, format_string=None,
-                 encoding=None, filter=None, bubble=False):
+    def __init__(
+        self,
+        stream,
+        level=NOTSET,
+        format_string=None,
+        encoding=None,
+        filter=None,
+        bubble=False,
+    ):
         Handler.__init__(self, level, filter, bubble)
         StringFormatterHandlerMixin.__init__(self, format_string)
         self.encoding = encoding
         self.lock = new_fine_grained_lock()
         if stream is not _missing:
             self.stream = stream
 
@@ -555,28 +584,20 @@
         """The default stream handler implementation is not to close
         the wrapped stream but to flush it.
         """
         self.flush()
 
     def flush(self):
         """Flushes the inner stream."""
-        if self.stream is not None and hasattr(self.stream, 'flush'):
+        if self.stream is not None and hasattr(self.stream, "flush"):
             self.stream.flush()
 
     def encode(self, msg):
         """Encodes the message to the stream encoding."""
-        stream = self.stream
-        rv = msg + '\n'
-        if ((PY2 and is_unicode(rv)) or
-                not (PY2 or is_unicode(rv) or _is_text_stream(stream))):
-            enc = self.encoding
-            if enc is None:
-                enc = getattr(stream, 'encoding', None) or 'utf-8'
-            rv = rv.encode(enc, 'replace')
-        return rv
+        return msg + "\n"
 
     def write(self, item):
         """Writes a bytestring to the stream."""
         self.stream.write(item)
 
     def emit(self, record):
         msg = self.format(record)
@@ -598,31 +619,41 @@
     By default the file is opened right away, but you can also `delay`
     the open to the point where the first message is written.
 
     This is useful when the handler is used with a
     :class:`~logbook.FingersCrossedHandler` or something similar.
     """
 
-    def __init__(self, filename, mode='a', encoding=None, level=NOTSET,
-                 format_string=None, delay=False, filter=None, bubble=False):
+    def __init__(
+        self,
+        filename,
+        mode="a",
+        encoding=None,
+        level=NOTSET,
+        format_string=None,
+        delay=False,
+        filter=None,
+        bubble=False,
+    ):
         if encoding is None:
-            encoding = 'utf-8'
-        StreamHandler.__init__(self, None, level, format_string,
-                               encoding, filter, bubble)
-        self._filename = filename
+            encoding = "utf-8"
+        StreamHandler.__init__(
+            self, None, level, format_string, encoding, filter, bubble
+        )
+        self._filename = os.fspath(filename)
         self._mode = mode
         if delay:
             self.stream = None
         else:
             self._open()
 
     def _open(self, mode=None):
         if mode is None:
             mode = self._mode
-        self.stream = io.open(self._filename, mode, encoding=self.encoding)
+        self.stream = open(self._filename, mode, encoding=self.encoding)
 
     def write(self, item):
         self.ensure_stream_is_open()
         if isinstance(item, bytes):
             self.stream.buffer.write(item)
         else:
             self.stream.write(item)
@@ -645,102 +676,149 @@
 
     def ensure_stream_is_open(self):
         if self.stream is None:
             self._open()
 
 
 class GZIPCompressionHandler(FileHandler):
-    def __init__(self, filename, encoding=None, level=NOTSET,
-                 format_string=None, delay=False, filter=None, bubble=False, compression_quality=9):
-
+    def __init__(
+        self,
+        filename,
+        encoding=None,
+        level=NOTSET,
+        format_string=None,
+        delay=False,
+        filter=None,
+        bubble=False,
+        compression_quality=9,
+    ):
         self._compression_quality = compression_quality
-        super(GZIPCompressionHandler, self).__init__(filename, mode='wb', encoding=encoding, level=level,
-                             format_string=format_string, delay=delay, filter=filter, bubble=bubble)
+        super().__init__(
+            filename,
+            mode="wb",
+            encoding=encoding,
+            level=level,
+            format_string=format_string,
+            delay=delay,
+            filter=filter,
+            bubble=bubble,
+        )
 
     def _open(self, mode=None):
         if mode is None:
             mode = self._mode
-        self.stream = gzip.open(self._filename, mode, compresslevel=self._compression_quality)
+        self.stream = gzip.open(
+            self._filename, mode, compresslevel=self._compression_quality
+        )
 
     def write(self, item):
         if isinstance(item, str):
             item = item.encode(encoding=self.encoding)
         self.ensure_stream_is_open()
         self.stream.write(item)
 
     def should_flush(self):
         # gzip manages writes independently. Flushing prematurely could mean
         # duplicate flushes and thus bloated files
         return False
 
 
 class BrotliCompressionHandler(FileHandler):
-    def __init__(self, filename, encoding=None, level=NOTSET,
-                 format_string=None, delay=False, filter=None, bubble=False,
-                 compression_window_size=4*1024**2, compression_quality=11):
-        super(BrotliCompressionHandler, self).__init__(filename, mode='wb', encoding=encoding, level=level,
-                             format_string=format_string, delay=delay, filter=filter, bubble=bubble)
+    def __init__(
+        self,
+        filename,
+        encoding=None,
+        level=NOTSET,
+        format_string=None,
+        delay=False,
+        filter=None,
+        bubble=False,
+        compression_window_size=4 * 1024**2,
+        compression_quality=11,
+    ):
+        super().__init__(
+            filename,
+            mode="wb",
+            encoding=encoding,
+            level=level,
+            format_string=format_string,
+            delay=delay,
+            filter=filter,
+            bubble=bubble,
+        )
         try:
             from brotli import Compressor
         except ImportError:
-            raise RuntimeError('The brotli library is required for '
-                               'the BrotliCompressionHandler.')
+            raise RuntimeError(
+                "The brotli library is required for the BrotliCompressionHandler."
+            )
 
         max_window_size = int(math.log(compression_window_size, 2))
-        self._compressor = Compressor(quality=compression_quality, lgwin=max_window_size)
+        self._compressor = Compressor(
+            quality=compression_quality, lgwin=max_window_size
+        )
 
     def _open(self, mode=None):
         if mode is None:
             mode = self._mode
-        self.stream = io.open(self._filename, mode)
+        self.stream = open(self._filename, mode)
 
     def write(self, item):
         if isinstance(item, str):
             item = item.encode(encoding=self.encoding)
         ret = self._compressor.process(item)
         if ret:
             self.ensure_stream_is_open()
             self.stream.write(ret)
-            super(BrotliCompressionHandler, self).flush()
+            super().flush()
 
     def should_flush(self):
         return False
 
     def flush(self):
         if self._compressor is not None:
             ret = self._compressor.flush()
             if ret:
                 self.ensure_stream_is_open()
                 self.stream.write(ret)
-        super(BrotliCompressionHandler, self).flush()
+        super().flush()
 
     def close(self):
         if self._compressor is not None:
             self.ensure_stream_is_open()
             self.stream.write(self._compressor.finish())
             self._compressor = None
-        super(BrotliCompressionHandler, self).close()
+        super().close()
 
 
 class MonitoringFileHandler(FileHandler):
     """A file handler that will check if the file was moved while it was
     open.  This might happen on POSIX systems if an application like
     logrotate moves the logfile over.
 
     Because of different IO concepts on Windows, this handler will not
     work on a windows system.
     """
 
-    def __init__(self, filename, mode='a', encoding='utf-8', level=NOTSET,
-                 format_string=None, delay=False, filter=None, bubble=False):
-        FileHandler.__init__(self, filename, mode, encoding, level,
-                             format_string, delay, filter, bubble)
-        if os.name == 'nt':
-            raise RuntimeError('MonitoringFileHandler '
-                               'does not support Windows')
+    def __init__(
+        self,
+        filename,
+        mode="a",
+        encoding="utf-8",
+        level=NOTSET,
+        format_string=None,
+        delay=False,
+        filter=None,
+        bubble=False,
+    ):
+        FileHandler.__init__(
+            self, filename, mode, encoding, level, format_string, delay, filter, bubble
+        )
+        if os.name == "nt":
+            raise RuntimeError("MonitoringFileHandler does not support Windows")
         self._query_fd()
 
     def _query_fd(self):
         if self.stream is None:
             self._last_stat = None, None
         else:
             try:
@@ -776,18 +854,18 @@
     glace this appears to just be a :class:`StreamHandler` with the stream
     set to :data:`sys.stderr` but there is a difference: if the handler is
     created globally and :data:`sys.stderr` changes later, this handler will
     point to the current `stderr`, whereas a stream handler would still
     point to the old one.
     """
 
-    def __init__(self, level=NOTSET, format_string=None, filter=None,
-                 bubble=False):
-        StreamHandler.__init__(self, _missing, level, format_string,
-                               None, filter, bubble)
+    def __init__(self, level=NOTSET, format_string=None, filter=None, bubble=False):
+        StreamHandler.__init__(
+            self, _missing, level, format_string, None, filter, bubble
+        )
 
     @property
     def stream(self):
         return sys.stderr
 
 
 class RotatingFileHandler(FileHandler):
@@ -800,41 +878,51 @@
 
     The default number of backups is 5.  Unlike a similar logger from
     the logging package, the backup count is mandatory because just
     reopening the file is dangerous as it deletes the log without
     asking on rollover.
     """
 
-    def __init__(self, filename, mode='a', encoding='utf-8', level=NOTSET,
-                 format_string=None, delay=False, max_size=1024 * 1024,
-                 backup_count=5, filter=None, bubble=False):
-        FileHandler.__init__(self, filename, mode, encoding, level,
-                             format_string, delay, filter, bubble)
+    def __init__(
+        self,
+        filename,
+        mode="a",
+        encoding="utf-8",
+        level=NOTSET,
+        format_string=None,
+        delay=False,
+        max_size=1024 * 1024,
+        backup_count=5,
+        filter=None,
+        bubble=False,
+    ):
+        FileHandler.__init__(
+            self, filename, mode, encoding, level, format_string, delay, filter, bubble
+        )
         self.max_size = max_size
         self.backup_count = backup_count
-        assert backup_count > 0, ('at least one backup file has to be '
-                                  'specified')
+        assert backup_count > 0, "at least one backup file has to be specified"
 
     def should_rollover(self, record, bytes):
         self.stream.seek(0, 2)
         return self.stream.tell() + bytes >= self.max_size
 
     def perform_rollover(self):
         self.stream.close()
-        for x in xrange(self.backup_count - 1, 0, -1):
-            src = '%s.%d' % (self._filename, x)
-            dst = '%s.%d' % (self._filename, x + 1)
+        for x in range(self.backup_count - 1, 0, -1):
+            src = "%s.%d" % (self._filename, x)
+            dst = "%s.%d" % (self._filename, x + 1)
             try:
                 rename(src, dst)
             except OSError:
                 e = sys.exc_info()[1]
                 if e.errno != errno.ENOENT:
                     raise
-        rename(self._filename, self._filename + '.1')
-        self._open('w')
+        rename(self._filename, self._filename + ".1")
+        self._open("w")
 
     def emit(self, record):
         msg = self.format(record)
         self.lock.acquire()
         try:
             msg = self.encode(msg)
             if self.should_rollover(record, len(msg)):
@@ -881,99 +969,105 @@
         ...
 
     Finally, an optional argument `timed_filename_for_current` may be set to
     false if you wish to have the current log file match the supplied filename
     until it is rolled over
     """
 
-    def __init__(self, filename, mode='a', encoding='utf-8', level=NOTSET,
-                 format_string=None, date_format='%Y-%m-%d',
-                 backup_count=0, filter=None, bubble=False,
-                 timed_filename_for_current=True,
-                 rollover_format='{basename}-{timestamp}{ext}'):
+    def __init__(
+        self,
+        filename,
+        mode="a",
+        encoding="utf-8",
+        level=NOTSET,
+        format_string=None,
+        date_format="%Y-%m-%d",
+        backup_count=0,
+        filter=None,
+        bubble=False,
+        timed_filename_for_current=True,
+        rollover_format="{basename}-{timestamp}{ext}",
+    ):
         self.date_format = date_format
         self.backup_count = backup_count
 
         self.rollover_format = rollover_format
 
         self.original_filename = filename
         self.basename, self.ext = os.path.splitext(os.path.abspath(filename))
         self.timed_filename_for_current = timed_filename_for_current
 
         self._timestamp = self._get_timestamp(_datetime_factory())
         if self.timed_filename_for_current:
             filename = self.generate_timed_filename(self._timestamp)
         elif os.path.exists(filename):
             self._timestamp = self._get_timestamp(
-                datetime.fromtimestamp(
-                    os.stat(filename).st_mtime
-                )
+                datetime.fromtimestamp(os.stat(filename).st_mtime)
             )
 
-        FileHandler.__init__(self, filename, mode, encoding, level,
-                             format_string, True, filter, bubble)
+        FileHandler.__init__(
+            self, filename, mode, encoding, level, format_string, True, filter, bubble
+        )
 
     def _get_timestamp(self, datetime):
         """
         Fetches a formatted string witha timestamp of the given datetime
         """
         return datetime.strftime(self.date_format)
 
     def generate_timed_filename(self, timestamp):
         """
         Produces a filename that includes a timestamp in the format supplied
         to the handler at init time.
         """
         timed_filename = self.rollover_format.format(
-            basename=self.basename,
-            timestamp=timestamp,
-            ext=self.ext)
+            basename=self.basename, timestamp=timestamp, ext=self.ext
+        )
         return timed_filename
 
     def files_to_delete(self):
         """Returns a list with the files that have to be deleted when
         a rollover occours.
         """
         directory = os.path.dirname(self._filename)
         files = []
-        rollover_regex = re.compile(self.rollover_format.format(
-            basename=re.escape(self.basename),
-            timestamp='.+',
-            ext=re.escape(self.ext),
-        ))
+        rollover_regex = re.compile(
+            self.rollover_format.format(
+                basename=re.escape(self.basename),
+                timestamp=".+",
+                ext=re.escape(self.ext),
+            )
+        )
         for filename in os.listdir(directory):
             filename = os.path.join(directory, filename)
             if rollover_regex.match(filename):
                 files.append((os.path.getmtime(filename), filename))
         files.sort()
         if self.backup_count > 1:
-            return files[:-self.backup_count + 1]
+            return files[: -self.backup_count + 1]
         else:
             return files[:]
 
     def perform_rollover(self, new_timestamp):
         if self.stream is not None:
             self.stream.close()
 
-        if (
-                not self.timed_filename_for_current
-                and os.path.exists(self._filename)
-        ):
+        if not self.timed_filename_for_current and os.path.exists(self._filename):
             filename = self.generate_timed_filename(self._timestamp)
             os.rename(self._filename, filename)
 
         if self.backup_count > 0:
             for time, filename in self.files_to_delete():
                 os.remove(filename)
 
         if self.timed_filename_for_current:
             self._filename = self.generate_timed_filename(new_timestamp)
         self._timestamp = new_timestamp
 
-        self._open('w')
+        self._open("w")
 
     def emit(self, record):
         msg = self.format(record)
         self.lock.acquire()
         try:
             new_timestamp = self._get_timestamp(record.time)
             if new_timestamp != self._timestamp:
@@ -992,18 +1086,25 @@
 
         def my_test():
             with logbook.TestHandler() as handler:
                 logger.warn('A warning')
                 assert logger.has_warning('A warning')
                 ...
     """
+
     default_format_string = TEST_FORMAT_STRING
 
-    def __init__(self, level=NOTSET, format_string=None, filter=None,
-                 bubble=False, force_heavy_init=False):
+    def __init__(
+        self,
+        level=NOTSET,
+        format_string=None,
+        filter=None,
+        bubble=False,
+        force_heavy_init=False,
+    ):
         Handler.__init__(self, level, filter, bubble)
         StringFormatterHandlerMixin.__init__(self, format_string)
         #: captures the :class:`LogRecord`\s as instances
         self.records = []
         self._formatted_records = []
         self._formatted_record_cache = []
         self._force_heavy_init = force_heavy_init
@@ -1021,17 +1122,17 @@
         if self._force_heavy_init:
             record.heavy_init()
         self.records.append(record)
 
     @property
     def formatted_records(self):
         """Captures the formatted log records as unicode strings."""
-        if (len(self._formatted_record_cache) != len(self.records) or
-                any(r1 != r2 for r1, r2 in
-                    zip(self.records, self._formatted_record_cache))):
+        if len(self._formatted_record_cache) != len(self.records) or any(
+            r1 != r2 for r1, r2 in zip(self.records, self._formatted_record_cache)
+        ):
             self._formatted_records = [self.format(r) for r in self.records]
             self._formatted_record_cache = list(self.records)
         return self._formatted_records
 
     @property
     def has_criticals(self):
         """`True` if any :data:`CRITICAL` records were found."""
@@ -1068,86 +1169,86 @@
         return any(r.level == TRACE for r in self.records)
 
     def has_critical(self, *args, **kwargs):
         """`True` if a specific :data:`CRITICAL` log record exists.
 
         See :ref:`probe-log-records` for more information.
         """
-        kwargs['level'] = CRITICAL
+        kwargs["level"] = CRITICAL
         return self._test_for(*args, **kwargs)
 
     def has_error(self, *args, **kwargs):
         """`True` if a specific :data:`ERROR` log record exists.
 
         See :ref:`probe-log-records` for more information.
         """
-        kwargs['level'] = ERROR
+        kwargs["level"] = ERROR
         return self._test_for(*args, **kwargs)
 
     def has_warning(self, *args, **kwargs):
         """`True` if a specific :data:`WARNING` log record exists.
 
         See :ref:`probe-log-records` for more information.
         """
-        kwargs['level'] = WARNING
+        kwargs["level"] = WARNING
         return self._test_for(*args, **kwargs)
 
     def has_notice(self, *args, **kwargs):
         """`True` if a specific :data:`NOTICE` log record exists.
 
         See :ref:`probe-log-records` for more information.
         """
-        kwargs['level'] = NOTICE
+        kwargs["level"] = NOTICE
         return self._test_for(*args, **kwargs)
 
     def has_info(self, *args, **kwargs):
         """`True` if a specific :data:`INFO` log record exists.
 
         See :ref:`probe-log-records` for more information.
         """
-        kwargs['level'] = INFO
+        kwargs["level"] = INFO
         return self._test_for(*args, **kwargs)
 
     def has_debug(self, *args, **kwargs):
         """`True` if a specific :data:`DEBUG` log record exists.
 
         See :ref:`probe-log-records` for more information.
         """
-        kwargs['level'] = DEBUG
+        kwargs["level"] = DEBUG
         return self._test_for(*args, **kwargs)
 
     def has_trace(self, *args, **kwargs):
         """`True` if a specific :data:`TRACE` log record exists.
 
         See :ref:`probe-log-records` for more information.
         """
-        kwargs['level'] = TRACE
+        kwargs["level"] = TRACE
         return self._test_for(*args, **kwargs)
 
     def _test_for(self, message=None, channel=None, level=None):
         def _match(needle, haystack):
             """Matches both compiled regular expressions and strings"""
             if isinstance(needle, REGTYPE) and needle.search(haystack):
                 return True
             if needle == haystack:
                 return True
             return False
+
         for record in self.records:
             if level is not None and record.level != level:
                 continue
             if channel is not None and record.channel != channel:
                 continue
             if message is not None and not _match(message, record.message):
                 continue
             return True
         return False
 
 
-class MailHandler(Handler, StringFormatterHandlerMixin,
-                  LimitingHandlerMixin):
+class MailHandler(Handler, StringFormatterHandlerMixin, LimitingHandlerMixin):
     """A handler that sends error mails.  The format string used by this
     handler are the contents of the mail plus the headers.  This is handy
     if you want to use a custom subject or ``X-`` header::
 
         handler = MailHandler(format_string='''\
         Subject: {record.level_name} on My Application
 
@@ -1202,31 +1303,44 @@
 
     .. versionchanged:: 1.0
        `credentials` parameter can now be a dictionary of keyword arguments.
 
     .. versionchanged:: 1.0
        `secure` can now be a dictionary or boolean in addition to to a tuple.
     """
+
     default_format_string = MAIL_FORMAT_STRING
     default_related_format_string = MAIL_RELATED_FORMAT_STRING
-    default_subject = u('Server Error in Application')
+    default_subject = "Server Error in Application"
 
     #: the maximum number of record hashes in the cache for the limiting
     #: feature.  Afterwards, record_cache_prune percent of the oldest
     #: entries are removed
     max_record_cache = 512
 
     #: the number of items to prune on a cache overflow in percent.
     record_cache_prune = 0.333
 
-    def __init__(self, from_addr, recipients, subject=None,
-                 server_addr=None, credentials=None, secure=None,
-                 record_limit=None, record_delta=None, level=NOTSET,
-                 format_string=None, related_format_string=None,
-                 filter=None, bubble=False, starttls=True):
+    def __init__(
+        self,
+        from_addr,
+        recipients,
+        subject=None,
+        server_addr=None,
+        credentials=None,
+        secure=None,
+        record_limit=None,
+        record_delta=None,
+        level=NOTSET,
+        format_string=None,
+        related_format_string=None,
+        filter=None,
+        bubble=False,
+        starttls=True,
+    ):
         Handler.__init__(self, level, filter, bubble)
         StringFormatterHandlerMixin.__init__(self, format_string)
         LimitingHandlerMixin.__init__(self, record_limit, record_delta)
         self.from_addr = from_addr
         self.recipients = recipients
         if subject is None:
             subject = self.default_subject
@@ -1244,101 +1358,106 @@
             return self.related_formatter.format_string
 
     def _set_related_format_string(self, value):
         if value is None:
             self.related_formatter = None
         else:
             self.related_formatter = self.formatter_class(value)
-    related_format_string = property(_get_related_format_string,
-                                     _set_related_format_string)
+
+    related_format_string = property(
+        _get_related_format_string, _set_related_format_string
+    )
     del _get_related_format_string, _set_related_format_string
 
     def get_recipients(self, record):
         """Returns the recipients for a record.  By default the
         :attr:`recipients` attribute is returned for all records.
         """
         return self.recipients
 
     def message_from_record(self, record, suppressed):
         """Creates a new message for a record as email message object
         (:class:`email.message.Message`).  `suppressed` is the number
         of mails not sent if the `record_limit` feature is active.
         """
-        from email.message import Message
         from email.header import Header
+        from email.message import Message
+
         msg = Message()
-        msg.set_charset('utf-8')
+        msg.set_charset("utf-8")
         lineiter = iter(self.format(record).splitlines())
         for line in lineiter:
             if not line:
                 break
-            h, v = line.split(':', 1)
+            h, v = line.split(":", 1)
             # We could probably just encode everything. For the moment encode
             # only what really needed to avoid breaking a couple of tests.
             try:
-                v.encode('ascii')
+                v.encode("ascii")
             except UnicodeEncodeError:
-                msg[h.strip()] = Header(v.strip(), 'utf-8')
+                msg[h.strip()] = Header(v.strip(), "utf-8")
             else:
                 msg[h.strip()] = v.strip()
 
-        msg.replace_header('Content-Transfer-Encoding', '8bit')
+        msg.replace_header("Content-Transfer-Encoding", "8bit")
 
-        body = '\r\n'.join(lineiter)
+        body = "\r\n".join(lineiter)
         if suppressed:
-            body += ('\r\n\r\nThis message occurred additional %d '
-                     'time(s) and was suppressed' % suppressed)
-
-        # inconsistency in Python 2.5
-        # other versions correctly return msg.get_payload() as str
-        if sys.version_info < (2, 6) and isinstance(body, unicode):
-            body = body.encode('utf-8')
+            body += (
+                "\r\n\r\nThis message occurred additional %d "
+                "time(s) and was suppressed" % suppressed
+            )
 
-        msg.set_payload(body, 'UTF-8')
+        msg.set_payload(body, "UTF-8")
         return msg
 
     def format_related_record(self, record):
         """Used for format the records that led up to another record or
         records that are related into strings.  Used by the batch formatter.
         """
         return self.related_formatter(record, self)
 
     def generate_mail(self, record, suppressed=0):
         """Generates the final email (:class:`email.message.Message`)
         with headers and date.  `suppressed` is the number of mails
         that were not send if the `record_limit` feature is active.
         """
         from email.utils import formatdate
+
         msg = self.message_from_record(record, suppressed)
-        msg['From'] = self.from_addr
-        msg['Date'] = formatdate()
+        msg["From"] = self.from_addr
+        msg["Date"] = formatdate()
         return msg
 
     def collapse_mails(self, mail, related, reason):
-        """When escaling or grouped mails are """
+        """When escaling or grouped mails are"""
         if not related:
             return mail
-        if reason == 'group':
-            title = 'Other log records in the same group'
+        if reason == "group":
+            title = "Other log records in the same group"
         else:
-            title = 'Log records that led up to this one'
-        mail.set_payload('%s\r\n\r\n\r\n%s:\r\n\r\n%s' % (
-            mail.get_payload(),
-            title,
-            '\r\n\r\n'.join(body.rstrip() for body in related)
-        ), 'UTF-8')
+            title = "Log records that led up to this one"
+        mail.set_payload(
+            "{}\r\n\r\n\r\n{}:\r\n\r\n{}".format(
+                mail.get_payload(),
+                title,
+                "\r\n\r\n".join(body.rstrip() for body in related),
+            ),
+            "UTF-8",
+        )
         return mail
 
     def get_connection(self):
         """Returns an SMTP connection.  By default it reconnects for
         each sent mail.
         """
-        from smtplib import SMTP, SMTP_SSL, SMTP_PORT, SMTP_SSL_PORT
+        from smtplib import SMTP, SMTP_PORT, SMTP_SSL, SMTP_SSL_PORT
+
         if self.server_addr is None:
-            host = '127.0.0.1'
+            host = "127.0.0.1"
             port = self.secure and SMTP_SSL_PORT or SMTP_PORT
         else:
             try:
                 host, port = self.server_addr
             except ValueError:
                 # If server_addr is a string, the tuple unpacking will raise
                 # ValueError, and we can use the default port.
@@ -1351,18 +1470,18 @@
         #
         # The changes below allow passing:
         # - secure=True for secure connection without checking identity.
         # - dictionary with keys 'keyfile' and 'certfile'.
         # - tuple to be unpacked to variables keyfile and certfile.
         # - secure=() equivalent to secure=True for backwards compatibility.
         # - secure=False equivalent to secure=None to disable.
-        if isinstance(self.secure, collections_abc.Mapping):
-            keyfile = self.secure.get('keyfile', None)
-            certfile = self.secure.get('certfile', None)
-        elif isinstance(self.secure, collections_abc.Iterable):
+        if isinstance(self.secure, Mapping):
+            keyfile = self.secure.get("keyfile", None)
+            certfile = self.secure.get("certfile", None)
+        elif isinstance(self.secure, Iterable):
             # Allow empty tuple for backwards compatibility
             if len(self.secure) == 0:
                 keyfile = certfile = None
             else:
                 keyfile, certfile = self.secure
         else:
             keyfile = certfile = None
@@ -1377,15 +1496,15 @@
             secure = self.secure
             if self.starttls and secure is not None and secure is not False:
                 con.ehlo()
                 con.starttls(keyfile=keyfile, certfile=certfile)
                 con.ehlo()
 
             # Allow credentials to be a tuple or dict.
-            if isinstance(self.credentials, collections_abc.Mapping):
+            if isinstance(self.credentials, Mapping):
                 credentials_args = ()
                 credentials_kwargs = self.credentials
             else:
                 credentials_args = self.credentials
                 credentials_kwargs = dict()
 
             con.login(*credentials_args, **credentials_kwargs)
@@ -1411,37 +1530,39 @@
 
     def emit(self, record):
         suppressed = 0
         if self.record_limit is not None:
             suppressed, allow_delivery = self.check_delivery(record)
             if not allow_delivery:
                 return
-        self.deliver(self.generate_mail(record, suppressed),
-                     self.get_recipients(record))
+        self.deliver(
+            self.generate_mail(record, suppressed), self.get_recipients(record)
+        )
 
     def emit_batch(self, records, reason):
-        if reason not in ('escalation', 'group'):
+        if reason not in ("escalation", "group"):
             raise RuntimeError("reason must be either 'escalation' or 'group'")
         records = list(records)
         if not records:
             return
 
-        trigger = records.pop(reason == 'escalation' and -1 or 0)
+        trigger = records.pop(reason == "escalation" and -1 or 0)
         suppressed = 0
         if self.record_limit is not None:
             suppressed, allow_delivery = self.check_delivery(trigger)
             if not allow_delivery:
                 return
 
         trigger_mail = self.generate_mail(trigger, suppressed)
-        related = [self.format_related_record(record)
-                   for record in records]
+        related = [self.format_related_record(record) for record in records]
 
-        self.deliver(self.collapse_mails(trigger_mail, related, reason),
-                     self.get_recipients(trigger))
+        self.deliver(
+            self.collapse_mails(trigger_mail, related, reason),
+            self.get_recipients(trigger),
+        )
 
 
 class GMailHandler(MailHandler):
     """
     A customized mail handler class for sending emails via GMail (or Google
     Apps mail)::
 
@@ -1449,192 +1570,209 @@
            "my_user@gmail.com", "mypassword", ["to_user@some_mail.com"],
            ...) # other arguments same as MailHandler
 
     .. versionadded:: 0.6.0
     """
 
     def __init__(self, account_id, password, recipients, **kw):
-        super(GMailHandler, self).__init__(
-            account_id, recipients, secure=True,
+        super().__init__(
+            account_id,
+            recipients,
+            secure=True,
             server_addr=("smtp.gmail.com", 587),
-            credentials=(account_id, password), **kw)
+            credentials=(account_id, password),
+            **kw,
+        )
 
 
 class SyslogHandler(Handler, StringFormatterHandlerMixin):
     """A handler class which sends formatted logging records to a
     syslog server.  By default it will send to it via unix socket.
     """
+
     default_format_string = SYSLOG_FORMAT_STRING
 
     # priorities
-    LOG_EMERG = 0       # system is unusable
-    LOG_ALERT = 1       # action must be taken immediately
-    LOG_CRIT = 2       # critical conditions
-    LOG_ERR = 3       # error conditions
-    LOG_WARNING = 4       # warning conditions
-    LOG_NOTICE = 5       # normal but significant condition
-    LOG_INFO = 6       # informational
-    LOG_DEBUG = 7       # debug-level messages
+    LOG_EMERG = 0  # system is unusable
+    LOG_ALERT = 1  # action must be taken immediately
+    LOG_CRIT = 2  # critical conditions
+    LOG_ERR = 3  # error conditions
+    LOG_WARNING = 4  # warning conditions
+    LOG_NOTICE = 5  # normal but significant condition
+    LOG_INFO = 6  # informational
+    LOG_DEBUG = 7  # debug-level messages
 
     # facility codes
-    LOG_KERN = 0       # kernel messages
-    LOG_USER = 1       # random user-level messages
-    LOG_MAIL = 2       # mail system
-    LOG_DAEMON = 3       # system daemons
-    LOG_AUTH = 4       # security/authorization messages
-    LOG_SYSLOG = 5       # messages generated internally by syslogd
-    LOG_LPR = 6       # line printer subsystem
-    LOG_NEWS = 7       # network news subsystem
-    LOG_UUCP = 8       # UUCP subsystem
-    LOG_CRON = 9       # clock daemon
-    LOG_AUTHPRIV = 10      # security/authorization messages (private)
-    LOG_FTP = 11      # FTP daemon
+    LOG_KERN = 0  # kernel messages
+    LOG_USER = 1  # random user-level messages
+    LOG_MAIL = 2  # mail system
+    LOG_DAEMON = 3  # system daemons
+    LOG_AUTH = 4  # security/authorization messages
+    LOG_SYSLOG = 5  # messages generated internally by syslogd
+    LOG_LPR = 6  # line printer subsystem
+    LOG_NEWS = 7  # network news subsystem
+    LOG_UUCP = 8  # UUCP subsystem
+    LOG_CRON = 9  # clock daemon
+    LOG_AUTHPRIV = 10  # security/authorization messages (private)
+    LOG_FTP = 11  # FTP daemon
 
     # other codes through 15 reserved for system use
-    LOG_LOCAL0 = 16      # reserved for local use
-    LOG_LOCAL1 = 17      # reserved for local use
-    LOG_LOCAL2 = 18      # reserved for local use
-    LOG_LOCAL3 = 19      # reserved for local use
-    LOG_LOCAL4 = 20      # reserved for local use
-    LOG_LOCAL5 = 21      # reserved for local use
-    LOG_LOCAL6 = 22      # reserved for local use
-    LOG_LOCAL7 = 23      # reserved for local use
+    LOG_LOCAL0 = 16  # reserved for local use
+    LOG_LOCAL1 = 17  # reserved for local use
+    LOG_LOCAL2 = 18  # reserved for local use
+    LOG_LOCAL3 = 19  # reserved for local use
+    LOG_LOCAL4 = 20  # reserved for local use
+    LOG_LOCAL5 = 21  # reserved for local use
+    LOG_LOCAL6 = 22  # reserved for local use
+    LOG_LOCAL7 = 23  # reserved for local use
 
     facility_names = {
-        'auth':     LOG_AUTH,
-        'authpriv': LOG_AUTHPRIV,
-        'cron':     LOG_CRON,
-        'daemon':   LOG_DAEMON,
-        'ftp':      LOG_FTP,
-        'kern':     LOG_KERN,
-        'lpr':      LOG_LPR,
-        'mail':     LOG_MAIL,
-        'news':     LOG_NEWS,
-        'syslog':   LOG_SYSLOG,
-        'user':     LOG_USER,
-        'uucp':     LOG_UUCP,
-        'local0':   LOG_LOCAL0,
-        'local1':   LOG_LOCAL1,
-        'local2':   LOG_LOCAL2,
-        'local3':   LOG_LOCAL3,
-        'local4':   LOG_LOCAL4,
-        'local5':   LOG_LOCAL5,
-        'local6':   LOG_LOCAL6,
-        'local7':   LOG_LOCAL7,
+        "auth": LOG_AUTH,
+        "authpriv": LOG_AUTHPRIV,
+        "cron": LOG_CRON,
+        "daemon": LOG_DAEMON,
+        "ftp": LOG_FTP,
+        "kern": LOG_KERN,
+        "lpr": LOG_LPR,
+        "mail": LOG_MAIL,
+        "news": LOG_NEWS,
+        "syslog": LOG_SYSLOG,
+        "user": LOG_USER,
+        "uucp": LOG_UUCP,
+        "local0": LOG_LOCAL0,
+        "local1": LOG_LOCAL1,
+        "local2": LOG_LOCAL2,
+        "local3": LOG_LOCAL3,
+        "local4": LOG_LOCAL4,
+        "local5": LOG_LOCAL5,
+        "local6": LOG_LOCAL6,
+        "local7": LOG_LOCAL7,
     }
 
     level_priority_map = {
-        DEBUG:      LOG_DEBUG,
-        INFO:       LOG_INFO,
-        NOTICE:     LOG_NOTICE,
-        WARNING:    LOG_WARNING,
-        ERROR:      LOG_ERR,
-        CRITICAL:   LOG_CRIT
+        DEBUG: LOG_DEBUG,
+        INFO: LOG_INFO,
+        NOTICE: LOG_NOTICE,
+        WARNING: LOG_WARNING,
+        ERROR: LOG_ERR,
+        CRITICAL: LOG_CRIT,
     }
 
-    def __init__(self, application_name=None, address=None,
-                 facility='user', socktype=socket.SOCK_DGRAM,
-                 level=NOTSET, format_string=None, filter=None,
-                 bubble=False, record_delimiter=None):
+    def __init__(
+        self,
+        application_name=None,
+        address=None,
+        facility="user",
+        socktype=socket.SOCK_DGRAM,
+        level=NOTSET,
+        format_string=None,
+        filter=None,
+        bubble=False,
+        record_delimiter=None,
+    ):
         Handler.__init__(self, level, filter, bubble)
         StringFormatterHandlerMixin.__init__(self, format_string)
         self.application_name = application_name
 
         if address is None:
-            if sys.platform == 'darwin':
-                address = '/var/run/syslog'
+            if sys.platform == "darwin":
+                address = "/var/run/syslog"
             else:
-                address = '/dev/log'
+                address = "/dev/log"
 
         self.remote_address = self.address = address
         self.facility = facility
         self.socktype = socktype
 
-        if isinstance(address, string_types):
+        if isinstance(address, str):
             self._connect_unixsocket()
             self.enveloper = self.unix_envelope
-            default_delimiter = u'\x00'
+            default_delimiter = "\x00"
         else:
             self._connect_netsocket()
             self.enveloper = self.net_envelope
-            default_delimiter = u'\n'
+            default_delimiter = "\n"
 
-        self.record_delimiter = default_delimiter \
-            if record_delimiter is None else record_delimiter
+        self.record_delimiter = (
+            default_delimiter if record_delimiter is None else record_delimiter
+        )
 
         self.connection_exception = getattr(
-            __builtins__, 'BrokenPipeError', socket.error)
+            __builtins__, "BrokenPipeError", socket.error
+        )
 
     def _connect_unixsocket(self):
         self.unixsocket = True
         self.socket = socket.socket(socket.AF_UNIX, socket.SOCK_DGRAM)
         try:
             self.socket.connect(self.address)
-        except socket.error:
+        except OSError:
             self.socket.close()
             self.socket = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
             self.socket.connect(self.address)
 
     def _connect_netsocket(self):
         self.unixsocket = False
         self.socket = socket.socket(socket.AF_INET, self.socktype)
         if self.socktype == socket.SOCK_STREAM:
             self.socket.connect(self.remote_address)
             self.address = self.socket.getsockname()
 
     def encode_priority(self, record):
         facility = self.facility_names[self.facility]
-        priority = self.level_priority_map.get(record.level,
-                                               self.LOG_WARNING)
+        priority = self.level_priority_map.get(record.level, self.LOG_WARNING)
         return (facility << 3) | priority
 
     def wrap_segments(self, record, before):
         msg = self.format(record)
         segments = [segment for segment in msg.split(self.record_delimiter)]
-        return (before + segment + self.record_delimiter
-                for segment in segments)
-        
+        return (before + segment + self.record_delimiter for segment in segments)
+
     def unix_envelope(self, record):
-        before = u'<{}>{}'.format(
+        before = "<{}>{}".format(
             self.encode_priority(record),
-            self.application_name + ':' if self.application_name else '')
+            self.application_name + ":" if self.application_name else "",
+        )
         return self.wrap_segments(record, before)
 
     def net_envelope(self, record):
         # Gross but effective
         try:
             format_string = self.format_string
             application_name = self.application_name
-            if not application_name and record.channel and \
-               '{record.channel}: ' in format_string:
-                self.format_string = format_string.replace(
-                    '{record.channel}: ', '')
+            if (
+                not application_name
+                and record.channel
+                and "{record.channel}: " in format_string
+            ):
+                self.format_string = format_string.replace("{record.channel}: ", "")
                 self.application_name = record.channel
             # RFC 5424: <PRIVAL>version timestamp hostname app-name procid
             #           msgid structured-data message
-            before = u'<{}>1 {}Z {} {} {} - - '.format(
+            before = "<{}>1 {}Z {} {} {} - - ".format(
                 self.encode_priority(record),
                 record.time.isoformat(),
                 socket.gethostname(),
-                self.application_name if self.application_name else '-',
-                record.process)
+                self.application_name if self.application_name else "-",
+                record.process,
+            )
             return self.wrap_segments(record, before)
         finally:
             self.format_string = format_string
             self.application_name = application_name
 
     def emit(self, record):
         for segment in self.enveloper(record):
-            self.send_to_socket(segment.encode('utf-8'))
+            self.send_to_socket(segment.encode("utf-8"))
 
     def send_to_socket(self, data):
         if self.unixsocket:
             try:
                 self.socket.send(data)
-            except socket.error:
+            except OSError:
                 self._connect_unixsocket()
                 self.socket.send(data)
         elif self.socktype == socket.SOCK_DGRAM:
             # the flags are no longer optional on Python 3
             self.socket.sendto(data, 0, self.address)
         else:
             try:
@@ -1645,61 +1783,69 @@
 
     def close(self):
         self.socket.close()
 
 
 class NTEventLogHandler(Handler, StringFormatterHandlerMixin):
     """A handler that sends to the NT event log system."""
+
     dllname = None
     default_format_string = NTLOG_FORMAT_STRING
 
-    def __init__(self, application_name, log_type='Application',
-                 level=NOTSET, format_string=None, filter=None,
-                 bubble=False):
+    def __init__(
+        self,
+        application_name,
+        log_type="Application",
+        level=NOTSET,
+        format_string=None,
+        filter=None,
+        bubble=False,
+    ):
         Handler.__init__(self, level, filter, bubble)
         StringFormatterHandlerMixin.__init__(self, format_string)
 
-        if os.name != 'nt':
-            raise RuntimeError('NTLogEventLogHandler requires a Windows '
-                               'operating system.')
+        if os.name != "nt":
+            raise RuntimeError(
+                "NTLogEventLogHandler requires a Windows operating system."
+            )
 
         try:
-            import win32evtlogutil
             import win32evtlog
+            import win32evtlogutil
         except ImportError:
-            raise RuntimeError('The pywin32 library is required '
-                               'for the NTEventLogHandler.')
+            raise RuntimeError(
+                "The pywin32 library is required for the NTEventLogHandler."
+            )
 
         self.application_name = application_name
         self._welu = win32evtlogutil
         dllname = self.dllname
         if not dllname:
-            dllname = os.path.join(os.path.dirname(self._welu.__file__),
-                                   '../win32service.pyd')
+            dllname = os.path.join(
+                os.path.dirname(self._welu.__file__), "../win32service.pyd"
+            )
         self.log_type = log_type
-        self._welu.AddSourceToRegistry(self.application_name, dllname,
-                                       log_type)
+        self._welu.AddSourceToRegistry(self.application_name, dllname, log_type)
 
         self._default_type = win32evtlog.EVENTLOG_INFORMATION_TYPE
         self._type_map = {
-            DEBUG:      win32evtlog.EVENTLOG_INFORMATION_TYPE,
-            INFO:       win32evtlog.EVENTLOG_INFORMATION_TYPE,
-            NOTICE:     win32evtlog.EVENTLOG_INFORMATION_TYPE,
-            WARNING:    win32evtlog.EVENTLOG_WARNING_TYPE,
-            ERROR:      win32evtlog.EVENTLOG_ERROR_TYPE,
-            CRITICAL:   win32evtlog.EVENTLOG_ERROR_TYPE
+            DEBUG: win32evtlog.EVENTLOG_INFORMATION_TYPE,
+            INFO: win32evtlog.EVENTLOG_INFORMATION_TYPE,
+            NOTICE: win32evtlog.EVENTLOG_INFORMATION_TYPE,
+            WARNING: win32evtlog.EVENTLOG_WARNING_TYPE,
+            ERROR: win32evtlog.EVENTLOG_ERROR_TYPE,
+            CRITICAL: win32evtlog.EVENTLOG_ERROR_TYPE,
         }
 
     def unregister_logger(self):
         """Removes the application binding from the registry.  If you call
         this, the log viewer will no longer be able to provide any
         information about the message.
         """
-        self._welu.RemoveSourceFromRegistry(self.application_name,
-                                            self.log_type)
+        self._welu.RemoveSourceFromRegistry(self.application_name, self.log_type)
 
     def get_event_type(self, record):
         return self._type_map.get(record.level, self._default_type)
 
     def get_event_category(self, record):
         """Returns the event category for the record. Override this if you want
         to specify your own categories. This version returns 0.
@@ -1712,16 +1858,17 @@
         """
         return 1
 
     def emit(self, record):
         id = self.get_message_id(record)
         cat = self.get_event_category(record)
         type = self.get_event_type(record)
-        self._welu.ReportEvent(self.application_name, id, cat, type,
-                               [self.format(record)])
+        self._welu.ReportEvent(
+            self.application_name, id, cat, type, [self.format(record)]
+        )
 
 
 class FingersCrossedHandler(Handler):
     """This handler wraps another handler and will log everything in
     memory until a certain level (`action_level`, defaults to `ERROR`)
     is exceeded.  When that happens the fingers crossed handler will
     activate forever and log all buffered records as well as records
@@ -1763,15 +1910,15 @@
 
     Due to how the handler is implemented, the filter, bubble and level
     flags of the wrapped handler are ignored.
 
     .. versionchanged:: 0.3
 
     The default behaviour is to buffer up records and then invoke another
-    handler when a severity theshold was reached with the buffer emitting.
+    handler when a severity threshold was reached with the buffer emitting.
     This now enables this logger to be properly used with the
     :class:`~logbook.MailHandler`.  You will now only get one mail for
     each buffered record.  However once the threshold was reached you would
     still get a mail for each record which is why the `reset` flag was added.
 
     When set to `True`, the handler will instantly reset to the untriggered
     state and start buffering again::
@@ -1784,19 +1931,26 @@
        The `reset` flag was added.
     """
 
     #: the reason to be used for the batch emit.  The default is
     #: ``'escalation'``.
     #:
     #: .. versionadded:: 0.3
-    batch_emit_reason = 'escalation'
+    batch_emit_reason = "escalation"
 
-    def __init__(self, handler, action_level=ERROR, buffer_size=0,
-                 pull_information=True, reset=False, filter=None,
-                 bubble=False):
+    def __init__(
+        self,
+        handler,
+        action_level=ERROR,
+        buffer_size=0,
+        pull_information=True,
+        reset=False,
+        filter=None,
+        bubble=False,
+    ):
         Handler.__init__(self, NOTSET, filter, bubble)
         self.lock = new_fine_grained_lock()
         self._level = action_level
         if isinstance(handler, Handler):
             self._handler = handler
             self._handler_factory = None
         else:
@@ -1824,24 +1978,23 @@
             record.pull_information()
         if self._action_triggered:
             self._handler.emit(record)
         else:
             self.buffered_records.append(record)
             if self._buffer_full:
                 self.buffered_records.popleft()
-            elif (self.buffer_size and
-                    len(self.buffered_records) >= self.buffer_size):
+            elif self.buffer_size and len(self.buffered_records) >= self.buffer_size:
                 self._buffer_full = True
             return record.level >= self._level
         return False
 
     def rollover(self, record):
         if self._handler is None:
             self._handler = self._handler_factory(record, self)
-        self._handler.emit_batch(iter(self.buffered_records), 'escalation')
+        self._handler.emit_batch(iter(self.buffered_records), "escalation")
         self.buffered_records.clear()
         self._action_triggered = not self._reset
 
     @property
     def triggered(self):
         """This attribute is `True` when the action was triggered.  From
         this point onwards the finger crossed handler transparently
@@ -1876,24 +2029,24 @@
     thus forwarding all attributes of the wrapper handler.
 
     Notice that this handler really only emit the records when the handler
     is popped from the stack.
 
     .. versionadded:: 0.3
     """
-    _direct_attrs = frozenset(['handler', 'pull_information',
-                               'buffered_records'])
+
+    _direct_attrs = frozenset(["handler", "pull_information", "buffered_records"])
 
     def __init__(self, handler, pull_information=True):
         WrapperHandler.__init__(self, handler)
         self.pull_information = pull_information
         self.buffered_records = []
 
     def rollover(self):
-        self.handler.emit_batch(self.buffered_records, 'group')
+        self.handler.emit_batch(self.buffered_records, "group")
         self.buffered_records = []
 
     def pop_application(self):
         Handler.pop_application(self)
         self.rollover()
 
     def pop_thread(self):
```

### Comparing `Logbook-1.5.3/logbook/helpers.py` & `Logbook-1.6.0/src/logbook/helpers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,163 +1,93 @@
-# -*- coding: utf-8 -*-
 """
     logbook.helpers
     ~~~~~~~~~~~~~~~
 
     Various helper functions
 
     :copyright: (c) 2010 by Armin Ronacher, Georg Brandl.
     :license: BSD, see LICENSE for more details.
 """
+import errno
 import os
+import random
 import re
 import sys
-import errno
 import time
-import random
 from datetime import datetime, timedelta
 
-PY2 = sys.version_info[0] == 2
-
-if PY2:
-    import __builtin__ as _builtins
-    import collections as collections_abc
-else:
-    import builtins as _builtins
-    import collections.abc as collections_abc
-
-try:
-    import json
-except ImportError:
-    import simplejson as json
-
-if PY2:
-    from cStringIO import StringIO
-    iteritems = dict.iteritems
-    from itertools import izip as zip
-    xrange = _builtins.xrange
-else:
-    from io import StringIO
-    zip = _builtins.zip
-    xrange = range
-    iteritems = dict.items
-
-_IDENTITY = lambda obj: obj
-
-if PY2:
-    def u(s):
-        return unicode(s, "unicode_escape")
-else:
-    u = _IDENTITY
-
-if PY2:
-    integer_types = (int, long)
-    string_types = (basestring,)
-else:
-    integer_types = (int,)
-    string_types = (str,)
-
-if PY2:
-    import httplib as http_client
-else:
-    from http import client as http_client
-
-if PY2:
-    # Yucky, but apparently that's the only way to do this
-    exec("""
-def reraise(tp, value, tb=None):
-    raise tp, value, tb
-""", locals(), globals())
-else:
-    def reraise(tp, value, tb=None):
-        if value.__traceback__ is not tb:
-            raise value.with_traceback(tb)
-        raise value
-
-
 # this regexp also matches incompatible dates like 20070101 because
 # some libraries (like the python xmlrpclib modules) use this
 _iso8601_re = re.compile(
     # date
-    r'(\d{4})(?:-?(\d{2})(?:-?(\d{2}))?)?'
+    r"(\d{4})(?:-?(\d{2})(?:-?(\d{2}))?)?"
     # time
-    r'(?:T(\d{2}):(\d{2})(?::(\d{2}(?:\.\d+)?))?(Z|[+-]\d{2}:\d{2})?)?$'
+    r"(?:T(\d{2}):(\d{2})(?::(\d{2}(?:\.\d+)?))?(Z|[+-]\d{2}:\d{2})?)?$"
 )
 _missing = object()
-if PY2:
-    def b(x):
-        return x
-
-    def _is_text_stream(x):
-        return True
-else:
-    import io
-
-    def b(x):
-        return x.encode('ascii')
-
-    def _is_text_stream(stream):
-        return isinstance(stream, io.TextIOBase)
 
 
 can_rename_open_file = False
-if os.name == 'nt':
+if os.name == "nt":
     try:
         import ctypes
 
         _MOVEFILE_REPLACE_EXISTING = 0x1
         _MOVEFILE_WRITE_THROUGH = 0x8
         _MoveFileEx = ctypes.windll.kernel32.MoveFileExW
 
         def _rename(src, dst):
-            if PY2:
-                if not isinstance(src, unicode):
-                    src = unicode(src, sys.getfilesystemencoding())
-                if not isinstance(dst, unicode):
-                    dst = unicode(dst, sys.getfilesystemencoding())
             if _rename_atomic(src, dst):
                 return True
             retry = 0
             rv = False
             while not rv and retry < 100:
-                rv = _MoveFileEx(src, dst, _MOVEFILE_REPLACE_EXISTING |
-                                 _MOVEFILE_WRITE_THROUGH)
+                rv = _MoveFileEx(
+                    src, dst, _MOVEFILE_REPLACE_EXISTING | _MOVEFILE_WRITE_THROUGH
+                )
                 if not rv:
                     time.sleep(0.001)
                     retry += 1
             return rv
 
         # new in Vista and Windows Server 2008
         _CreateTransaction = ctypes.windll.ktmw32.CreateTransaction
         _CommitTransaction = ctypes.windll.ktmw32.CommitTransaction
         _MoveFileTransacted = ctypes.windll.kernel32.MoveFileTransactedW
         _CloseHandle = ctypes.windll.kernel32.CloseHandle
         can_rename_open_file = True
 
         def _rename_atomic(src, dst):
-            ta = _CreateTransaction(None, 0, 0, 0, 0, 1000, 'Logbook rename')
+            ta = _CreateTransaction(None, 0, 0, 0, 0, 1000, "Logbook rename")
             if ta == -1:
                 return False
             try:
                 retry = 0
                 rv = False
                 while not rv and retry < 100:
-                    rv = _MoveFileTransacted(src, dst, None, None,
-                                             _MOVEFILE_REPLACE_EXISTING |
-                                             _MOVEFILE_WRITE_THROUGH, ta)
+                    rv = _MoveFileTransacted(
+                        src,
+                        dst,
+                        None,
+                        None,
+                        _MOVEFILE_REPLACE_EXISTING | _MOVEFILE_WRITE_THROUGH,
+                        ta,
+                    )
                     if rv:
                         rv = _CommitTransaction(ta)
                         break
                     else:
                         time.sleep(0.001)
                         retry += 1
                 return rv
             finally:
                 _CloseHandle(ta)
+
     except Exception:
+
         def _rename(src, dst):
             return False
 
         def _rename_atomic(src, dst):
             return False
 
     def rename(src, dst):
@@ -167,110 +97,111 @@
         # Fall back to "move away and replace"
         try:
             os.rename(src, dst)
         except OSError:
             e = sys.exc_info()[1]
             if e.errno not in (errno.EEXIST, errno.EACCES):
                 raise
-            old = "%s-%08x" % (dst, random.randint(0, 2 ** 31 - 1))
+            old = f"{dst}-{random.randint(0, 2**31 - 1):08x}"
             os.rename(dst, old)
             os.rename(src, dst)
             try:
                 os.unlink(old)
             except Exception:
                 pass
+
 else:
     rename = os.rename
     can_rename_open_file = True
 
-_JSON_SIMPLE_TYPES = (bool, float) + integer_types + string_types
+_JSON_SIMPLE_TYPES = (bool, float, int, str)
 
 
 def to_safe_json(data):
     """Makes a data structure safe for JSON silently discarding invalid
     objects from nested structures.  This also converts dates.
     """
+
     def _convert(obj):
         if obj is None:
             return None
-        elif PY2 and isinstance(obj, str):
-            return obj.decode('utf-8', 'replace')
         elif isinstance(obj, _JSON_SIMPLE_TYPES):
             return obj
         elif isinstance(obj, datetime):
             return format_iso8601(obj)
         elif isinstance(obj, list):
             return [_convert(x) for x in obj]
         elif isinstance(obj, tuple):
             return tuple(_convert(x) for x in obj)
         elif isinstance(obj, dict):
             rv = {}
-            for key, value in iteritems(obj):
-                if not isinstance(key, string_types):
+            for key, value in obj.items():
+                if not isinstance(key, str):
                     key = str(key)
-                if not is_unicode(key):
-                    key = u(key)
+                if not isinstance(key, str):
+                    key = key
                 rv[key] = _convert(value)
             return rv
+
     return _convert(data)
 
 
 def format_iso8601(d=None):
     """Returns a date in iso8601 format."""
     if d is None:
         d = datetime.utcnow()
-    rv = d.strftime('%Y-%m-%dT%H:%M:%S')
+    rv = d.strftime("%Y-%m-%dT%H:%M:%S")
     if d.microsecond:
-        rv += '.' + str(d.microsecond)
-    return rv + 'Z'
+        rv += "." + str(d.microsecond)
+    return rv + "Z"
 
 
 def parse_iso8601(value):
     """Parse an iso8601 date into a datetime object.  The timezone is
     normalized to UTC.
     """
     m = _iso8601_re.match(value)
     if m is None:
-        raise ValueError('not a valid iso8601 date value')
+        raise ValueError("not a valid iso8601 date value")
 
     groups = m.groups()
     args = []
     for group in groups[:-2]:
         if group is not None:
             group = int(group)
         args.append(group)
     seconds = groups[-2]
     if seconds is not None:
-        if '.' in seconds:
-            sec, usec = seconds.split('.')
+        if "." in seconds:
+            sec, usec = seconds.split(".")
             args.append(int(sec))
-            args.append(int(usec.ljust(6, '0')))
+            args.append(int(usec.ljust(6, "0")))
         else:
             args.append(int(seconds))
 
     rv = datetime(*args)
     tz = groups[-1]
-    if tz and tz != 'Z':
-        args = [int(x) for x in tz[1:].split(':')]
+    if tz and tz != "Z":
+        args = [int(x) for x in tz[1:].split(":")]
         delta = timedelta(hours=args[0], minutes=args[1])
-        if tz[0] == '+':
+        if tz[0] == "+":
             rv -= delta
         else:
             rv += delta
 
     return rv
 
 
 def get_application_name():
     if not sys.argv or not sys.argv[0]:
-        return 'Python'
+        return "Python"
     return os.path.basename(sys.argv[0]).title()
 
 
-class cached_property(object):
+class cached_property:
     """A property that is lazily calculated and then cached."""
 
     def __init__(self, func, name=None, doc=None):
         self.__name__ = name or func.__name__
         self.__module__ = func.__module__
         self.__doc__ = doc or func.__doc__
         self.func = func
@@ -283,27 +214,7 @@
             value = self.func(obj)
             obj.__dict__[self.__name__] = value
         return value
 
 
 def get_iterator_next_method(it):
     return lambda: next(it)
-
-
-# python 2 support functions and aliases
-def is_unicode(x):
-    if PY2:
-        return isinstance(x, unicode)
-    return isinstance(x, str)
-
-if PY2:
-    exec("""def with_metaclass(meta):
-    class _WithMetaclassBase(object):
-        __metaclass__ = meta
-    return _WithMetaclassBase
-""")
-else:
-    exec("""def with_metaclass(meta):
-    class _WithMetaclassBase(object, metaclass=meta):
-        pass
-    return _WithMetaclassBase
-""")
```

### Comparing `Logbook-1.5.3/logbook/more.py` & `Logbook-1.6.0/src/logbook/more.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,99 +1,91 @@
-# -*- coding: utf-8 -*-
 """
     logbook.more
     ~~~~~~~~~~~~
 
     Fancy stuff for logbook.
 
     :copyright: (c) 2010 by Armin Ronacher, Georg Brandl.
     :license: BSD, see LICENSE for more details.
 """
-import re
 import os
 import platform
-
+import re
 from collections import defaultdict
 from functools import partial
+from urllib.parse import parse_qsl, urlencode
 
-from logbook.base import (
-    RecordDispatcher, dispatch_record, NOTSET, ERROR, NOTICE)
-from logbook.handlers import (
-    Handler, StringFormatter, StringFormatterHandlerMixin, StderrHandler)
 from logbook._termcolors import colorize
-from logbook.helpers import PY2, string_types, iteritems, u
-from logbook.ticketing import TicketingHandler as DatabaseHandler
+from logbook.base import ERROR, NOTICE, NOTSET, RecordDispatcher, dispatch_record
+from logbook.handlers import (
+    Handler,
+    StderrHandler,
+    StringFormatter,
+    StringFormatterHandlerMixin,
+)
 from logbook.ticketing import BackendBase
+from logbook.ticketing import TicketingHandler as DatabaseHandler
 
 try:
     import riemann_client.client
     import riemann_client.transport
 except ImportError:
     riemann_client = None
-    #from riemann_client.transport import TCPTransport, UDPTransport, BlankTransport
+    # from riemann_client.transport import TCPTransport, UDPTransport, BlankTransport
 
-
-if PY2:
-    from urllib import urlencode
-    from urlparse import parse_qsl
-else:
-    from urllib.parse import parse_qsl, urlencode
-
-_ws_re = re.compile(r'(\s+)', re.UNICODE)
-TWITTER_FORMAT_STRING = u(
-    '[{record.channel}] {record.level_name}: {record.message}')
-TWITTER_ACCESS_TOKEN_URL = 'https://twitter.com/oauth/access_token'
-NEW_TWEET_URL = 'https://api.twitter.com/1/statuses/update.json'
+_ws_re = re.compile(r"(\s+)", re.UNICODE)
+TWITTER_FORMAT_STRING = "[{record.channel}] {record.level_name}: {record.message}"
+TWITTER_ACCESS_TOKEN_URL = "https://twitter.com/oauth/access_token"
+NEW_TWEET_URL = "https://api.twitter.com/1/statuses/update.json"
 
 
 class CouchDBBackend(BackendBase):
-    """Implements a backend that writes into a CouchDB database.
-    """
+    """Implements a backend that writes into a CouchDB database."""
+
     def setup_backend(self):
         from couchdb import Server
 
-        uri = self.options.pop('uri', u(''))
+        uri = self.options.pop("uri", "")
         couch = Server(uri)
-        db_name = self.options.pop('db')
+        db_name = self.options.pop("db")
         self.database = couch[db_name]
 
     def record_ticket(self, record, data, hash, app_id):
-        """Records a log record as ticket.
-        """
+        """Records a log record as ticket."""
         db = self.database
 
         ticket = record.to_dict()
         ticket["time"] = ticket["time"].isoformat() + "Z"
         ticket_id, _ = db.save(ticket)
 
         db.save(ticket)
 
 
 class TwitterFormatter(StringFormatter):
     """Works like the standard string formatter and is used by the
     :class:`TwitterHandler` unless changed.
     """
+
     max_length = 140
 
     def format_exception(self, record):
-        return u('%s: %s') % (record.exception_shortname,
-                              record.exception_message)
+        return f"{record.exception_shortname}: {record.exception_message}"
 
     def __call__(self, record, handler):
         formatted = StringFormatter.__call__(self, record, handler)
         rv = []
         length = 0
         for piece in _ws_re.split(formatted):
             length += len(piece)
             if length > self.max_length:
                 if length - len(piece) < self.max_length:
-                    rv.append(u('…'))
+                    rv.append("…")
                 break
             rv.append(piece)
-        return u('').join(rv)
+        return "".join(rv)
 
 
 class TaggingLogger(RecordDispatcher):
     """A logger that attaches a tag to each record.  This is an alternative
     record dispatcher that does not use levels but tags to keep log
     records apart.  It is constructed with a descriptive name and at least
     one tag.  The tags are up for you to define::
@@ -111,26 +103,27 @@
     The tags themselves are stored as list named ``'tags'`` in the
     :attr:`~logbook.LogRecord.extra` dictionary.
     """
 
     def __init__(self, name=None, tags=None):
         RecordDispatcher.__init__(self, name)
         # create a method for each tag named
-        for tag in (tags or ()):
+        for tag in tags or ():
             setattr(self, tag, partial(self.log, tag))
 
     def log(self, tags, msg, *args, **kwargs):
-        if isinstance(tags, string_types):
+        if isinstance(tags, str):
             tags = [tags]
-        exc_info = kwargs.pop('exc_info', None)
-        extra = kwargs.pop('extra', {})
-        extra['tags'] = list(tags)
-        frame_correction = kwargs.pop('frame_correction', 0)
-        return self.make_record_and_handle(NOTSET, msg, args, kwargs,
-                                           exc_info, extra, frame_correction)
+        exc_info = kwargs.pop("exc_info", None)
+        extra = kwargs.pop("extra", {})
+        extra["tags"] = list(tags)
+        frame_correction = kwargs.pop("frame_correction", 0)
+        return self.make_record_and_handle(
+            NOTSET, msg, args, kwargs, exc_info, extra, frame_correction
+        )
 
 
 class TaggingHandler(Handler):
     """A handler that logs for tags and dispatches based on those.
 
     Example::
 
@@ -142,135 +135,153 @@
             warning=AnotherHandler()
         ))
     """
 
     def __init__(self, handlers, filter=None, bubble=False):
         Handler.__init__(self, NOTSET, filter, bubble)
         assert isinstance(handlers, dict)
-        self._handlers = dict(
-            (tag, isinstance(handler, Handler) and [handler] or handler)
-            for (tag, handler) in iteritems(handlers))
+        self._handlers = {
+            tag: isinstance(handler, Handler) and [handler] or handler
+            for (tag, handler) in handlers.items()
+        }
 
     def emit(self, record):
-        for tag in record.extra.get('tags', ()):
+        for tag in record.extra.get("tags", ()):
             for handler in self._handlers.get(tag, ()):
                 handler.handle(record)
 
 
 class TwitterHandler(Handler, StringFormatterHandlerMixin):
     """A handler that logs to twitter.  Requires that you sign up an
     application on twitter and request xauth support.  Furthermore the
     oauth2 library has to be installed.
 
     If you don't want to register your own application and request xauth
     credentials, there are a couple of leaked consumer key and secret
     pairs from application explicitly whitelisted at Twitter
-    (`leaked secrets <http://bit.ly/leaked-secrets>`_).
+    (`leaked secrets <https://bit.ly/leaked-secrets>`_).
     """
+
     default_format_string = TWITTER_FORMAT_STRING
     formatter_class = TwitterFormatter
 
-    def __init__(self, consumer_key, consumer_secret, username,
-                 password, level=NOTSET, format_string=None, filter=None,
-                 bubble=False):
+    def __init__(
+        self,
+        consumer_key,
+        consumer_secret,
+        username,
+        password,
+        level=NOTSET,
+        format_string=None,
+        filter=None,
+        bubble=False,
+    ):
         Handler.__init__(self, level, filter, bubble)
         StringFormatterHandlerMixin.__init__(self, format_string)
         self.consumer_key = consumer_key
         self.consumer_secret = consumer_secret
         self.username = username
         self.password = password
 
         try:
             import oauth2
         except ImportError:
-            raise RuntimeError('The python-oauth2 library is required for '
-                               'the TwitterHandler.')
+            raise RuntimeError(
+                "The python-oauth2 library is required for the TwitterHandler."
+            )
 
         self._oauth = oauth2
         self._oauth_token = None
         self._oauth_token_secret = None
-        self._consumer = oauth2.Consumer(consumer_key,
-                                         consumer_secret)
+        self._consumer = oauth2.Consumer(consumer_key, consumer_secret)
         self._client = oauth2.Client(self._consumer)
 
     def get_oauth_token(self):
         """Returns the oauth access token."""
         if self._oauth_token is None:
             resp, content = self._client.request(
-                TWITTER_ACCESS_TOKEN_URL + '?', 'POST',
-                body=urlencode({
-                    'x_auth_username':  self.username.encode('utf-8'),
-                    'x_auth_password':  self.password.encode('utf-8'),
-                    'x_auth_mode':      'client_auth'
-                }),
-                headers={'Content-Type': 'application/x-www-form-urlencoded'}
+                TWITTER_ACCESS_TOKEN_URL + "?",
+                "POST",
+                body=urlencode(
+                    {
+                        "x_auth_username": self.username.encode("utf-8"),
+                        "x_auth_password": self.password.encode("utf-8"),
+                        "x_auth_mode": "client_auth",
+                    }
+                ),
+                headers={"Content-Type": "application/x-www-form-urlencoded"},
             )
-            if resp['status'] != '200':
-                raise RuntimeError('unable to login to Twitter')
+            if resp["status"] != "200":
+                raise RuntimeError("unable to login to Twitter")
             data = dict(parse_qsl(content))
-            self._oauth_token = data['oauth_token']
-            self._oauth_token_secret = data['oauth_token_secret']
-        return self._oauth.Token(self._oauth_token,
-                                 self._oauth_token_secret)
+            self._oauth_token = data["oauth_token"]
+            self._oauth_token_secret = data["oauth_token_secret"]
+        return self._oauth.Token(self._oauth_token, self._oauth_token_secret)
 
     def make_client(self):
         """Creates a new oauth client auth a new access token."""
         return self._oauth.Client(self._consumer, self.get_oauth_token())
 
     def tweet(self, status):
         """Tweets a given status.  Status must not exceed 140 chars."""
         client = self.make_client()
         resp, content = client.request(
-            NEW_TWEET_URL, 'POST',
-            body=urlencode({'status': status.encode('utf-8')}),
-            headers={'Content-Type': 'application/x-www-form-urlencoded'})
-        return resp['status'] == '200'
+            NEW_TWEET_URL,
+            "POST",
+            body=urlencode({"status": status.encode("utf-8")}),
+            headers={"Content-Type": "application/x-www-form-urlencoded"},
+        )
+        return resp["status"] == "200"
 
     def emit(self, record):
         self.tweet(self.format(record))
 
 
 class SlackHandler(Handler, StringFormatterHandlerMixin):
 
     """A handler that logs to slack.  Requires that you sign up an
     application on slack and request an api token.  Furthermore the
     slacker library has to be installed.
     """
 
-    def __init__(self, api_token, channel, level=NOTSET, format_string=None, filter=None,
-                 bubble=False):
-
+    def __init__(
+        self,
+        api_token,
+        channel,
+        level=NOTSET,
+        format_string=None,
+        filter=None,
+        bubble=False,
+    ):
         Handler.__init__(self, level, filter, bubble)
         StringFormatterHandlerMixin.__init__(self, format_string)
         self.api_token = api_token
 
         try:
             from slacker import Slacker
         except ImportError:
-            raise RuntimeError('The slacker library is required for '
-                               'the SlackHandler.')
+            raise RuntimeError("The slacker library is required for the SlackHandler.")
 
         self.channel = channel
         self.slack = Slacker(api_token)
 
     def emit(self, record):
         self.slack.chat.post_message(channel=self.channel, text=self.format(record))
 
 
-class JinjaFormatter(object):
+class JinjaFormatter:
     """A formatter object that makes it easy to format using a Jinja 2
     template instead of a format string.
     """
 
     def __init__(self, template):
         try:
             from jinja2 import Template
         except ImportError:
-            raise RuntimeError('The jinja2 library is required for '
-                               'the JinjaFormatter.')
+            raise RuntimeError("The jinja2 library is required for the JinjaFormatter.")
         self.template = Template(template)
 
     def __call__(self, record, handler):
         return self.template.render(record=record, handler=handler)
 
 
 class ExternalApplicationHandler(Handler):
@@ -289,88 +300,92 @@
     recommended to combine this handler with the
     :class:`logbook.ThreadedWrapperHandler` to move the execution into
     a background thread.
 
     .. versionadded:: 0.3
     """
 
-    def __init__(self, arguments, stdin_format=None,
-                 encoding='utf-8', level=NOTSET, filter=None,
-                 bubble=False):
+    def __init__(
+        self,
+        arguments,
+        stdin_format=None,
+        encoding="utf-8",
+        level=NOTSET,
+        filter=None,
+        bubble=False,
+    ):
         Handler.__init__(self, level, filter, bubble)
         self.encoding = encoding
         self._arguments = list(arguments)
         if stdin_format is not None:
             stdin_format = stdin_format
         self._stdin_format = stdin_format
         import subprocess
+
         self._subprocess = subprocess
 
     def emit(self, record):
-        args = [arg.format(record=record)
-                for arg in self._arguments]
+        args = [arg.format(record=record) for arg in self._arguments]
         if self._stdin_format is not None:
-            stdin_data = (self._stdin_format.format(record=record)
-                          .encode(self.encoding))
+            stdin_data = self._stdin_format.format(record=record).encode(self.encoding)
             stdin = self._subprocess.PIPE
         else:
             stdin = None
         c = self._subprocess.Popen(args, stdin=stdin)
         if stdin is not None:
             c.communicate(stdin_data)
         c.wait()
 
 
-class ColorizingStreamHandlerMixin(object):
+class ColorizingStreamHandlerMixin:
     """A mixin class that does colorizing.
 
     .. versionadded:: 0.3
     .. versionchanged:: 1.0.0
        Added Windows support if `colorama`_ is installed.
 
-    .. _`colorama`: https://pypi.org/pypi/colorama
+    .. _`colorama`: https://pypi.org/project/colorama
     """
+
     _use_color = None
 
     def force_color(self):
-        """Force colorizing the stream (`should_colorize` will return True)
-        """
+        """Force colorizing the stream (`should_colorize` will return True)"""
         self._use_color = True
 
     def forbid_color(self):
-        """Forbid colorizing the stream (`should_colorize` will return False)
-        """
+        """Forbid colorizing the stream (`should_colorize` will return False)"""
         self._use_color = False
 
     def should_colorize(self, record):
         """Returns `True` if colorizing should be applied to this
         record.  The default implementation returns `True` if the
         stream is a tty. If we are executing on Windows, colorama must be
         installed.
         """
-        if os.name == 'nt':
+        if os.name == "nt":
             try:
                 import colorama
             except ImportError:
                 return False
         if self._use_color is not None:
             return self._use_color
-        isatty = getattr(self.stream, 'isatty', None)
+        isatty = getattr(self.stream, "isatty", None)
         return isatty and isatty()
 
     def get_color(self, record):
         """Returns the color for this record."""
         if record.level >= ERROR:
-            return 'red'
+            return "red"
         elif record.level >= NOTICE:
-            return 'yellow'
-        return 'lightgray'
+            return "yellow"
+        return "lightgray"
 
     def format(self, record):
-        rv = super(ColorizingStreamHandlerMixin, self).format(record)
+        rv = super().format(record)
         if self.should_colorize(record):
             color = self.get_color(record)
             if color:
                 rv = colorize(color, rv)
         return rv
 
 
@@ -379,40 +394,45 @@
     colorize if a terminal was detected.  Note that this handler does
     not colorize on Windows systems.
 
     .. versionadded:: 0.3
     .. versionchanged:: 1.0
        Added Windows support if `colorama`_ is installed.
 
-    .. _`colorama`: https://pypi.org/pypi/colorama
+    .. _`colorama`: https://pypi.org/project/colorama
     """
+
     def __init__(self, *args, **kwargs):
         StderrHandler.__init__(self, *args, **kwargs)
 
         # Try import colorama so that we work on Windows. colorama.init is a
         # noop on other operating systems.
         try:
             import colorama
         except ImportError:
             pass
         else:
             colorama.init()
 
 
 # backwards compat.  Should go away in some future releases
-from logbook.handlers import (
-    FingersCrossedHandler as FingersCrossedHandlerBase)
+from logbook.handlers import FingersCrossedHandler as FingersCrossedHandlerBase
 
 
 class FingersCrossedHandler(FingersCrossedHandlerBase):
     def __init__(self, *args, **kwargs):
         FingersCrossedHandlerBase.__init__(self, *args, **kwargs)
         from warnings import warn
-        warn(PendingDeprecationWarning('fingers crossed handler changed '
-             'location.  It\'s now a core component of Logbook.'))
+
+        warn(
+            PendingDeprecationWarning(
+                "fingers crossed handler changed "
+                "location.  It's now a core component of Logbook."
+            )
+        )
 
 
 class ExceptionHandler(Handler, StringFormatterHandlerMixin):
     """An exception handler which raises exceptions of the given `exc_type`.
     This is especially useful if you set a specific error `level` e.g. to treat
     warnings as exceptions::
 
@@ -421,16 +441,18 @@
         class ApplicationWarning(Exception):
             pass
 
         exc_handler = ExceptionHandler(ApplicationWarning, level='WARNING')
 
     .. versionadded:: 0.3
     """
-    def __init__(self, exc_type, level=NOTSET, format_string=None,
-                 filter=None, bubble=False):
+
+    def __init__(
+        self, exc_type, level=NOTSET, format_string=None, filter=None, bubble=False
+    ):
         Handler.__init__(self, level, filter, bubble)
         StringFormatterHandlerMixin.__init__(self, format_string)
         self.exc_type = exc_type
 
     def handle(self, record):
         if self.should_handle(record):
             raise self.exc_type(self.format(record))
@@ -450,17 +472,18 @@
             logbook.error('foo')
 
     The expected output:::
 
        message repeated 2 times: foo
        message repeated 1 times: bar
     """
-    def __init__(self,
-                 format_string='message repeated {count} times: {message}',
-                 *args, **kwargs):
+
+    def __init__(
+        self, format_string="message repeated {count} times: {message}", *args, **kwargs
+    ):
         Handler.__init__(self, bubble=False, *args, **kwargs)
         self._format_string = format_string
         self.clear()
 
     def clear(self):
         self._message_to_count = defaultdict(int)
         self._unique_ordered_records = []
@@ -486,16 +509,16 @@
             self._unique_ordered_records.append(record)
         self._message_to_count[record.message] += 1
         return True
 
     def flush(self):
         for record in self._unique_ordered_records:
             record.message = self._format_string.format(
-                message=record.message,
-                count=self._message_to_count[record.message])
+                message=record.message, count=self._message_to_count[record.message]
+            )
             # record.dispatcher is the logger who created the message,
             # it's sometimes supressed (by logbook.info for example)
             if record.dispatcher is not None:
                 dispatch = record.dispatcher.call_handlers
             else:
                 dispatch = dispatch_record
             dispatch(record)
@@ -504,72 +527,80 @@
 
 class RiemannHandler(Handler):
 
     """
     A handler that sends logs as events to Riemann.
     """
 
-    def __init__(self,
-                 host,
-                 port,
-                 message_type="tcp",
-                 ttl=60,
-                 flush_threshold=10,
-                 bubble=False,
-                 filter=None,
-                 level=NOTSET):
+    def __init__(
+        self,
+        host,
+        port,
+        message_type="tcp",
+        ttl=60,
+        flush_threshold=10,
+        bubble=False,
+        filter=None,
+        level=NOTSET,
+    ):
         """
         :param host: riemann host
         :param port: riemann port
         :param message_type: selects transport. Currently available 'tcp' and 'udp'
         :param ttl: defines time to live in riemann
         :param flush_threshold: count of events after which we send to riemann
         """
         if riemann_client is None:
-            raise NotImplementedError("The Riemann handler requires the riemann_client package") # pragma: no cover
+            raise NotImplementedError(
+                "The Riemann handler requires the riemann_client package"
+            )  # pragma: no cover
         Handler.__init__(self, level, filter, bubble)
         self.host = host
         self.port = port
         self.ttl = ttl
         self.queue = []
         self.flush_threshold = flush_threshold
         if message_type == "tcp":
             self.transport = riemann_client.transport.TCPTransport
         elif message_type == "udp":
             self.transport = riemann_client.transport.UDPTransport
         elif message_type == "test":
             self.transport = riemann_client.transport.BlankTransport
         else:
-            msg = ("Currently supported message types for RiemannHandler are: {0}. \
-                    {1} is not supported."
-                   .format(",".join(["tcp", "udp", "test"]), message_type))
+            msg = "Currently supported message types for RiemannHandler are: {}. \
+                    {} is not supported.".format(
+                ",".join(["tcp", "udp", "test"]), message_type
+            )
             raise RuntimeError(msg)
 
     def record_to_event(self, record):
         from time import time
+
         tags = ["log", record.level_name]
         msg = str(record.exc_info[1]) if record.exc_info else record.msg
         channel_name = str(record.channel) if record.channel else "unknown"
-        if any([record.level_name == keywords
-                for keywords in ["ERROR", "EXCEPTION"]]):
+        if any([record.level_name == keywords for keywords in ["ERROR", "EXCEPTION"]]):
             state = "error"
         else:
             state = "ok"
-        return {"metric_f": 1.0,
-                "tags": tags,
-                "description": msg,
-                "time": int(time()),
-                "ttl": self.ttl,
-                "host": platform.node(),
-                "service": "{0}.{1}".format(channel_name, os.getpid()),
-                "state": state
-                }
+        return {
+            "metric_f": 1.0,
+            "tags": tags,
+            "description": msg,
+            "time": int(time()),
+            "ttl": self.ttl,
+            "host": platform.node(),
+            "service": f"{channel_name}.{os.getpid()}",
+            "state": state,
+        }
 
     def _flush_events(self):
-        with riemann_client.client.QueuedClient(self.transport(self.host, self.port)) as cl:
+        with riemann_client.client.QueuedClient(
+            self.transport(self.host, self.port)
+        ) as cl:
             for event in self.queue:
                 cl.event(**event)
             cl.flush()
         self.queue = []
 
     def emit(self, record):
         self.queue.append(self.record_to_event(record))
```

### Comparing `Logbook-1.5.3/logbook/notifiers.py` & `Logbook-1.6.0/src/logbook/notifiers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,105 +1,127 @@
-# -*- coding: utf-8 -*-
 """
     logbook.notifiers
     ~~~~~~~~~~~~~~~~~
 
     System notify handlers for OSX and Linux.
 
     :copyright: (c) 2010 by Armin Ronacher, Christopher Grebs.
     :license: BSD, see LICENSE for more details.
 """
+import base64
 import os
 import sys
-import base64
+from http import client as http_client
 from time import time
+from urllib.parse import urlencode
 
-from logbook.base import NOTSET, ERROR, WARNING
+from logbook.base import ERROR, NOTSET, WARNING
 from logbook.handlers import Handler, LimitingHandlerMixin
-from logbook.helpers import get_application_name, PY2, http_client, u
-
-if PY2:
-    from urllib import urlencode
-else:
-    from urllib.parse import urlencode
+from logbook.helpers import get_application_name
 
 
-def create_notification_handler(application_name=None, level=NOTSET,
-                                icon=None):
+def create_notification_handler(application_name=None, level=NOTSET, icon=None):
     """Creates a handler perfectly fit the current platform.  On Linux
     systems this creates a :class:`LibNotifyHandler`, on OS X systems it
     will create a :class:`GrowlHandler`.
     """
-    if sys.platform == 'darwin':
+    if sys.platform == "darwin":
         return GrowlHandler(application_name, level=level, icon=icon)
     return LibNotifyHandler(application_name, level=level, icon=icon)
 
 
 class NotificationBaseHandler(Handler, LimitingHandlerMixin):
     """Baseclass for notification handlers."""
 
-    def __init__(self, application_name=None, record_limit=None,
-                 record_delta=None, level=NOTSET, filter=None, bubble=False):
+    def __init__(
+        self,
+        application_name=None,
+        record_limit=None,
+        record_delta=None,
+        level=NOTSET,
+        filter=None,
+        bubble=False,
+    ):
         Handler.__init__(self, level, filter, bubble)
         LimitingHandlerMixin.__init__(self, record_limit, record_delta)
         if application_name is None:
             application_name = get_application_name()
         self.application_name = application_name
 
     def make_title(self, record):
         """Called to get the title from the record."""
-        return u('%s: %s') % (record.channel, record.level_name.title())
+        return f"{record.channel}: {record.level_name.title()}"
 
     def make_text(self, record):
         """Called to get the text of the record."""
         return record.message
 
 
 class GrowlHandler(NotificationBaseHandler):
     """A handler that dispatches to Growl.  Requires that either growl-py or
     py-Growl are installed.
     """
 
-    def __init__(self, application_name=None, icon=None, host=None,
-                 password=None, record_limit=None, record_delta=None,
-                 level=NOTSET, filter=None, bubble=False):
-        NotificationBaseHandler.__init__(self, application_name, record_limit,
-                                         record_delta, level, filter, bubble)
+    def __init__(
+        self,
+        application_name=None,
+        icon=None,
+        host=None,
+        password=None,
+        record_limit=None,
+        record_delta=None,
+        level=NOTSET,
+        filter=None,
+        bubble=False,
+    ):
+        NotificationBaseHandler.__init__(
+            self, application_name, record_limit, record_delta, level, filter, bubble
+        )
 
         # growl is using the deprecated md5 module, but we really don't need
         # to see that deprecation warning
         from warnings import filterwarnings
-        filterwarnings(module='Growl', category=DeprecationWarning,
-                       action='ignore')
+
+        filterwarnings(module="Growl", category=DeprecationWarning, action="ignore")
 
         try:
             import Growl
+
             self._growl = Growl
         except ImportError:
-            raise RuntimeError('The growl module is not available.  You have '
-                               'to install either growl-py or py-Growl to '
-                               'use the GrowlHandler.')
+            raise RuntimeError(
+                "The growl module is not available.  You have "
+                "to install either growl-py or py-Growl to "
+                "use the GrowlHandler."
+            )
 
         if icon is not None:
             if not os.path.isfile(icon):
-                raise IOError('Filename to an icon expected.')
+                raise OSError("Filename to an icon expected.")
             icon = self._growl.Image.imageFromPath(icon)
         else:
             try:
                 icon = self._growl.Image.imageWithIconForCurrentApplication()
             except TypeError:
                 icon = None
 
         self._notifier = self._growl.GrowlNotifier(
             applicationName=self.application_name,
             applicationIcon=icon,
-            notifications=['Notset', 'Debug', 'Info', 'Notice', 'Warning',
-                           'Error', 'Critical'],
+            notifications=[
+                "Notset",
+                "Debug",
+                "Info",
+                "Notice",
+                "Warning",
+                "Error",
+                "Critical",
+            ],
             hostname=host,
-            password=password
+            password=password,
         )
         self._notifier.register()
 
     def is_sticky(self, record):
         """Returns `True` if the sticky flag should be set for this record.
         The default implementation marks errors and criticals sticky.
         """
@@ -115,50 +137,63 @@
         elif record.level == WARNING:
             return 1
         return 0
 
     def emit(self, record):
         if not self.check_delivery(record)[1]:
             return
-        self._notifier.notify(record.level_name.title(),
-                              self.make_title(record),
-                              self.make_text(record),
-                              sticky=self.is_sticky(record),
-                              priority=self.get_priority(record))
+        self._notifier.notify(
+            record.level_name.title(),
+            self.make_title(record),
+            self.make_text(record),
+            sticky=self.is_sticky(record),
+            priority=self.get_priority(record),
+        )
 
 
 class LibNotifyHandler(NotificationBaseHandler):
     """A handler that dispatches to libnotify.  Requires pynotify installed.
     If `no_init` is set to `True` the initialization of libnotify is skipped.
     """
 
-    def __init__(self, application_name=None, icon=None, no_init=False,
-                 record_limit=None, record_delta=None, level=NOTSET,
-                 filter=None, bubble=False):
-        NotificationBaseHandler.__init__(self, application_name, record_limit,
-                                         record_delta, level, filter, bubble)
+    def __init__(
+        self,
+        application_name=None,
+        icon=None,
+        no_init=False,
+        record_limit=None,
+        record_delta=None,
+        level=NOTSET,
+        filter=None,
+        bubble=False,
+    ):
+        NotificationBaseHandler.__init__(
+            self, application_name, record_limit, record_delta, level, filter, bubble
+        )
 
         try:
             import pynotify
+
             self._pynotify = pynotify
         except ImportError:
-            raise RuntimeError('The pynotify library is required for '
-                               'the LibNotifyHandler.')
+            raise RuntimeError(
+                "The pynotify library is required for the LibNotifyHandler."
+            )
 
         self.icon = icon
         if not no_init:
             pynotify.init(self.application_name)
 
     def set_notifier_icon(self, notifier, icon):
         """Used to attach an icon on a notifier object."""
         try:
             from gtk import gdk
         except ImportError:
             # TODO: raise a warning?
-            raise RuntimeError('The gtk.gdk module is required to set an icon.')
+            raise RuntimeError("The gtk.gdk module is required to set an icon.")
 
         if icon is not None:
             if not isinstance(icon, gdk.Pixbuf):
                 icon = gdk.pixbuf_new_from_file(icon)
             notifier.set_icon_from_pixbuf(icon)
 
     def get_expires(self, record):
@@ -179,106 +214,148 @@
         elif record.level == WARNING:
             return pn.URGENCY_NORMAL
         return pn.URGENCY_LOW
 
     def emit(self, record):
         if not self.check_delivery(record)[1]:
             return
-        notifier = self._pynotify.Notification(self.make_title(record),
-                                               self.make_text(record))
+        notifier = self._pynotify.Notification(
+            self.make_title(record), self.make_text(record)
+        )
         notifier.set_urgency(self.get_urgency(record))
         notifier.set_timeout(self.get_expires(record))
         self.set_notifier_icon(notifier, self.icon)
         notifier.show()
 
 
 class BoxcarHandler(NotificationBaseHandler):
     """Sends notifications to boxcar.io.  Can be forwarded to your iPhone or
     other compatible device.
     """
-    api_url = 'https://boxcar.io/notifications/'
 
-    def __init__(self, email, password, record_limit=None, record_delta=None,
-                 level=NOTSET, filter=None, bubble=False):
-        NotificationBaseHandler.__init__(self, None, record_limit,
-                                         record_delta, level, filter, bubble)
+    api_url = "https://boxcar.io/notifications/"
+
+    def __init__(
+        self,
+        email,
+        password,
+        record_limit=None,
+        record_delta=None,
+        level=NOTSET,
+        filter=None,
+        bubble=False,
+    ):
+        NotificationBaseHandler.__init__(
+            self, None, record_limit, record_delta, level, filter, bubble
+        )
         self.email = email
         self.password = password
 
     def get_screen_name(self, record):
         """Returns the value of the screen name field."""
         return record.level_name.title()
 
     def emit(self, record):
         if not self.check_delivery(record)[1]:
             return
-        body = urlencode({
-            'notification[from_screen_name]':
-                self.get_screen_name(record).encode('utf-8'),
-            'notification[message]':
-                self.make_text(record).encode('utf-8'),
-            'notification[from_remote_service_id]': str(int(time() * 100))
-        })
-        con = http_client.HTTPSConnection('boxcar.io')
-        con.request('POST', '/notifications/', headers={
-            'Authorization': 'Basic ' +
-            base64.b64encode((u('%s:%s') % (self.email, self.password))
-                             .encode('utf-8')).strip(),
-        }, body=body)
+        body = urlencode(
+            {
+                "notification[from_screen_name]": self.get_screen_name(record).encode(
+                    "utf-8"
+                ),
+                "notification[message]": self.make_text(record).encode("utf-8"),
+                "notification[from_remote_service_id]": str(int(time() * 100)),
+            }
+        )
+        con = http_client.HTTPSConnection("boxcar.io")
+        con.request(
+            "POST",
+            "/notifications/",
+            headers={
+                "Authorization": "Basic "
+                + base64.b64encode(f"{self.email}:{self.password}".encode()).strip(),
+            },
+            body=body,
+        )
         con.close()
 
 
 class NotifoHandler(NotificationBaseHandler):
     """Sends notifications to notifo.com.  Can be forwarded to your Desktop,
     iPhone, or other compatible device.
     """
 
-    def __init__(self, application_name=None, username=None, secret=None,
-                 record_limit=None, record_delta=None, level=NOTSET,
-                 filter=None, bubble=False, hide_level=False):
+    def __init__(
+        self,
+        application_name=None,
+        username=None,
+        secret=None,
+        record_limit=None,
+        record_delta=None,
+        level=NOTSET,
+        filter=None,
+        bubble=False,
+        hide_level=False,
+    ):
         try:
             import notifo
         except ImportError:
             raise RuntimeError(
-                'The notifo module is not available.  You have '
-                'to install notifo to use the NotifoHandler.'
+                "The notifo module is not available.  You have "
+                "to install notifo to use the NotifoHandler."
             )
-        NotificationBaseHandler.__init__(self, None, record_limit,
-                                         record_delta, level, filter, bubble)
+        NotificationBaseHandler.__init__(
+            self, None, record_limit, record_delta, level, filter, bubble
+        )
         self._notifo = notifo
         self.application_name = application_name
         self.username = username
         self.secret = secret
         self.hide_level = hide_level
 
     def emit(self, record):
-
         if self.hide_level:
             _level_name = None
         else:
             _level_name = self.level_name
 
-        self._notifo.send_notification(self.username, self.secret, None,
-                                       record.message, self.application_name,
-                                       _level_name, None)
+        self._notifo.send_notification(
+            self.username,
+            self.secret,
+            None,
+            record.message,
+            self.application_name,
+            _level_name,
+            None,
+        )
 
 
 class PushoverHandler(NotificationBaseHandler):
     """Sends notifications to pushover.net.  Can be forwarded to your Desktop,
     iPhone, or other compatible device. If `priority` is not one of -2, -1, 0,
     or 1, it is set to 0 automatically.
     """
 
-    def __init__(self, application_name=None, apikey=None, userkey=None,
-                 device=None, priority=0, sound=None, record_limit=None,
-                 record_delta=None, level=NOTSET, filter=None, bubble=False,
-                 max_title_len=100, max_message_len=512):
-
-        super(PushoverHandler, self).__init__(None, record_limit, record_delta,
-                                              level, filter, bubble)
+    def __init__(
+        self,
+        application_name=None,
+        apikey=None,
+        userkey=None,
+        device=None,
+        priority=0,
+        sound=None,
+        record_limit=None,
+        record_delta=None,
+        level=NOTSET,
+        filter=None,
+        bubble=False,
+        max_title_len=100,
+        max_message_len=512,
+    ):
+        super().__init__(None, record_limit, record_delta, level, filter, bubble)
 
         self.application_name = application_name
         self.apikey = apikey
         self.userkey = userkey
         self.device = device
         self.priority = priority
         self.sound = sound
@@ -292,32 +369,32 @@
             self.title = self._crop(self.application_name, self.max_title_len)
 
         if self.priority not in [-2, -1, 0, 1]:
             self.priority = 0
 
     def _crop(self, msg, max_len):
         if max_len is not None and max_len > 0 and len(msg) > max_len:
-            return "%s..." % (msg[:max_len-3],)
+            return f"{msg[: max_len - 3]}..."
         else:
             return msg
 
     def emit(self, record):
         message = self._crop(record.message, self.max_message_len)
 
         body_dict = {
-            'token': self.apikey,
-            'user': self.userkey,
-            'message': message,
-            'priority': self.priority
+            "token": self.apikey,
+            "user": self.userkey,
+            "message": message,
+            "priority": self.priority,
         }
 
         if self.title is not None:
-            body_dict['title'] = self.title
+            body_dict["title"] = self.title
         if self.device is not None:
-            body_dict['device'] = self.device
+            body_dict["device"] = self.device
         if self.sound is not None:
-            body_dict['sound'] = self.sound
+            body_dict["sound"] = self.sound
 
         body = urlencode(body_dict)
-        con = http_client.HTTPSConnection('api.pushover.net')
-        con.request('POST', '/1/messages.json', body=body)
+        con = http_client.HTTPSConnection("api.pushover.net")
+        con.request("POST", "/1/messages.json", body=body)
         con.close()
```

### Comparing `Logbook-1.5.3/logbook/queues.py` & `Logbook-1.6.0/src/logbook/queues.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,25 @@
-# -*- coding: utf-8 -*-
 """
     logbook.queues
     ~~~~~~~~~~~~~~
 
     This module implements queue backends.
 
     :copyright: (c) 2010 by Armin Ronacher, Georg Brandl.
     :license: BSD, see LICENSE for more details.
 """
 import json
-import threading
-from threading import Thread, Lock
 import platform
+import threading
+from queue import Empty, Full
+from queue import Queue as ThreadQueue
+from threading import Lock, Thread
+
 from logbook.base import NOTSET, LogRecord, dispatch_record
 from logbook.handlers import Handler, WrapperHandler
-from logbook.helpers import PY2, u
-
-if PY2:
-    from Queue import Empty, Full, Queue as ThreadQueue
-else:
-    from queue import Empty, Full, Queue as ThreadQueue
 
 
 class RedisHandler(Handler):
     """A handler that sends log messages to a Redis instance.
 
     It publishes each record as json dump. Requires redis module.
 
@@ -38,52 +34,62 @@
 
     Example::
 
         handler = RedisHandler(password='your_redis_password')
 
     More info about the default buffer size: wp.me/p3tYJu-3b
     """
-    def __init__(self, host='127.0.0.1', port=6379, key='redis',
-                 extra_fields=None, flush_threshold=128, flush_time=1,
-                 level=NOTSET, filter=None, password=False, bubble=True,
-                 context=None, push_method='rpush'):
+
+    def __init__(
+        self,
+        host="127.0.0.1",
+        port=6379,
+        key="redis",
+        extra_fields=None,
+        flush_threshold=128,
+        flush_time=1,
+        level=NOTSET,
+        filter=None,
+        password=False,
+        bubble=True,
+        context=None,
+        push_method="rpush",
+    ):
         Handler.__init__(self, level, filter, bubble)
         try:
             import redis
             from redis import ResponseError
         except ImportError:
-            raise RuntimeError('The redis library is required for '
-                               'the RedisHandler')
+            raise RuntimeError("The redis library is required for the RedisHandler")
 
-        self.redis = redis.Redis(host=host, port=port, password=password,
-                                 decode_responses=True)
+        self.redis = redis.Redis(
+            host=host, port=port, password=password, decode_responses=True
+        )
         try:
             self.redis.ping()
         except ResponseError:
-            raise ResponseError(
-                'The password provided is apparently incorrect')
+            raise ResponseError("The password provided is apparently incorrect")
         self.key = key
         self.extra_fields = extra_fields or {}
         self.flush_threshold = flush_threshold
         self.queue = []
         self.lock = Lock()
         self.push_method = push_method
 
         # Set up a thread that flushes the queue every specified seconds
         self._stop_event = threading.Event()
-        self._flushing_t = threading.Thread(target=self._flush_task,
-                                            args=(flush_time,
-                                                  self._stop_event))
+        self._flushing_t = threading.Thread(
+            target=self._flush_task, args=(flush_time, self._stop_event)
+        )
         self._flushing_t.daemon = True
         self._flushing_t.start()
 
     def _flush_task(self, time, stop_event):
-        """Calls the method _flush_buffer every certain time.
-        """
-        while not self._stop_event.isSet():
+        """Calls the method _flush_buffer every certain time."""
+        while not self._stop_event.is_set():
             with self.lock:
                 self._flush_buffer()
             self._stop_event.wait(time)
 
     def _flush_buffer(self):
         """Flushes the messaging queue into Redis.
 
@@ -107,18 +113,20 @@
         """Emits a pair (key, value) to redis.
 
         The key is the one provided when creating the handler, or redis if none
         was provided. The value contains both the message and the hostname.
         Extra values are also appended to the message.
         """
         with self.lock:
-            r = {"message": record.msg,
-                 "host": platform.node(),
-                 "level": record.level_name,
-                 "time": record.time.isoformat()}
+            r = {
+                "message": record.msg,
+                "host": platform.node(),
+                "level": record.level_name,
+                "time": record.time.isoformat(),
+            }
             r.update(self.extra_fields)
             r.update(record.kwargs)
             self.queue.append(json.dumps(r))
             if len(self.queue) == self.flush_threshold:
                 self._flush_buffer()
 
     def close(self):
@@ -145,33 +153,34 @@
     For MongoDB (requires pymongo)::
 
         handler = MessageQueueHandler('mongodb://localhost:27017/logging')
 
     Several other backends are also supported.
     Refer to the `kombu`_ documentation
 
-    .. _kombu: http://kombu.readthedocs.org/en/latest/introduction.html
+    .. _kombu: https://docs.celeryq.dev/projects/kombu/en/latest/introduction.html
     """
 
-    def __init__(self, uri=None, queue='logging', level=NOTSET,
-                 filter=None, bubble=False):
+    def __init__(
+        self, uri=None, queue="logging", level=NOTSET, filter=None, bubble=False
+    ):
         Handler.__init__(self, level, filter, bubble)
         try:
             import kombu
         except ImportError:
-            raise RuntimeError('The kombu library is required for '
-                               'the RabbitMQSubscriber.')
+            raise RuntimeError(
+                "The kombu library is required for the RabbitMQSubscriber."
+            )
         if uri:
             connection = kombu.Connection(uri)
 
         self.queue = connection.SimpleQueue(queue)
 
     def export_record(self, record):
-        """Exports the record into a dictionary ready for JSON dumping.
-        """
+        """Exports the record into a dictionary ready for JSON dumping."""
         return record.to_dict(json_safe=True)
 
     def emit(self, record):
         self.queue.put(self.export_record(record))
 
     def close(self):
         self.queue.close()
@@ -194,22 +203,28 @@
 
 
     Example setup::
 
         handler = ZeroMQHandler('tcp://127.0.0.1:5000')
     """
 
-    def __init__(self, uri=None, level=NOTSET, filter=None, bubble=False,
-                 context=None, multi=False):
+    def __init__(
+        self,
+        uri=None,
+        level=NOTSET,
+        filter=None,
+        bubble=False,
+        context=None,
+        multi=False,
+    ):
         Handler.__init__(self, level, filter, bubble)
         try:
             import zmq
         except ImportError:
-            raise RuntimeError('The pyzmq library is required for '
-                               'the ZeroMQHandler.')
+            raise RuntimeError("The pyzmq library is required for the ZeroMQHandler.")
         #: the zero mq context
         self.context = context or zmq.Context()
 
         if multi:
             #: the zero mq socket.
             self.socket = self.context.socket(zmq.PUSH)
             if uri is not None:
@@ -221,31 +236,31 @@
                 self.socket.bind(uri)
 
     def export_record(self, record):
         """Exports the record into a dictionary ready for JSON dumping."""
         return record.to_dict(json_safe=True)
 
     def emit(self, record):
-        self.socket.send(json.dumps(
-            self.export_record(record)).encode("utf-8"))
+        self.socket.send(json.dumps(self.export_record(record)).encode("utf-8"))
 
     def close(self, linger=-1):
         self.socket.close(linger)
 
     def __del__(self):
         # When the Handler is deleted we must close our socket in a
         # non-blocking fashion (using linger).
         # Otherwise it can block indefinitely, for example if the Subscriber is
         # not reachable.
         # If messages are pending on the socket, we wait 100ms for them to be
         # sent then we discard them.
-        self.close(linger=100)
+        if hasattr(self, "socket"):
+            self.close(linger=100)
 
 
-class ThreadController(object):
+class ThreadController:
     """A helper class used by queue subscribers to control the background
     thread.  This is usually created and started in one go by
     :meth:`~logbook.queues.ZeroMQSubscriber.dispatch_in_background` or
     a comparable function.
     """
 
     def __init__(self, subscriber, setup=None):
@@ -254,15 +269,15 @@
         self.running = False
         self._thread = None
 
     def start(self):
         """Starts the task thread."""
         self.running = True
         self._thread = Thread(target=self._target)
-        self._thread.setDaemon(True)
+        self._thread.daemon = True
         self._thread.start()
 
     def stop(self):
         """Stops the task thread."""
         if self.running:
             self.running = False
             self._thread.join()
@@ -275,15 +290,15 @@
             while self.running:
                 self.subscriber.dispatch_once(timeout=0.05)
         finally:
             if self.setup is not None:
                 self.setup.pop_thread()
 
 
-class SubscriberBase(object):
+class SubscriberBase:
     """Baseclass for all subscribers."""
 
     def recv(self, timeout=None):
         """Receives a single record from the socket.  Timeout of 0 means
         nonblocking, `None` means blocking and otherwise it's a timeout in
         seconds after which the function just returns with `None`.
 
@@ -344,19 +359,20 @@
         controller = subscriber.dispatch_in_background(target_handler)
 
     The controller returned can be used to shut down the background
     thread::
 
         controller.stop()
     """
-    def __init__(self, uri=None, queue='logging'):
+
+    def __init__(self, uri=None, queue="logging"):
         try:
             import kombu
         except ImportError:
-            raise RuntimeError('The kombu library is required.')
+            raise RuntimeError("The kombu library is required.")
         if uri:
             connection = kombu.Connection(uri)
 
         self.queue = connection.SimpleQueue(queue)
 
     def __del__(self):
         try:
@@ -424,16 +440,17 @@
     single subscriber to dispatch multiple handlers.
     """
 
     def __init__(self, uri=None, context=None, multi=False):
         try:
             import zmq
         except ImportError:
-            raise RuntimeError('The pyzmq library is required for '
-                               'the ZeroMQSubscriber.')
+            raise RuntimeError(
+                "The pyzmq library is required for the ZeroMQSubscriber."
+            )
         self._zmq = zmq
 
         #: the zero mq context
         self.context = context or zmq.Context()
 
         if multi:
             #: the zero mq socket.
@@ -441,15 +458,15 @@
             if uri is not None:
                 self.socket.bind(uri)
         else:
             #: the zero mq socket.
             self.socket = self.context.socket(zmq.SUB)
             if uri is not None:
                 self.socket.connect(uri)
-            self.socket.setsockopt_unicode(zmq.SUBSCRIBE, u(''))
+            self.socket.setsockopt_unicode(zmq.SUBSCRIBE, "")
 
     def __del__(self):
         try:
             self.close()
         except AttributeError:
             # subscriber partially created
             pass
@@ -469,28 +486,28 @@
             rv = self.socket.recv(self._zmq.NOBLOCK)
             if rv is None:
                 return
         else:
             if not self._zmq.select([self.socket], [], [], timeout)[0]:
                 return
             rv = self.socket.recv(self._zmq.NOBLOCK)
-        if not PY2:
-            rv = rv.decode("utf-8")
+        rv = rv.decode("utf-8")
         return LogRecord.from_dict(json.loads(rv))
 
 
 def _fix_261_mplog():
     """necessary for older python's to disable a broken monkeypatch
     in the logging module.  See multiprocessing/util.py for the
     hasattr() check.  At least in Python 2.6.1 the multiprocessing
     module is not imported by logging and as such the test in
     the util fails.
     """
     import logging
     import multiprocessing
+
     logging.multiprocessing = multiprocessing
 
 
 class MultiProcessingHandler(Handler):
     """Implements a handler that dispatches over a queue to a different
     process.  It is connected to a subscriber with a
     :class:`multiprocessing.Queue`::
@@ -549,14 +566,15 @@
         subscriber = MultiProcessingSubscriber()
         handler = MultiProcessingHandler(subscriber.queue)
     """
 
     def __init__(self, queue=None):
         if queue is None:
             from multiprocessing import Queue
+
             queue = Queue(-1)
         self.queue = queue
         _fix_261_mplog()
 
     def recv(self, timeout=None):
         if timeout is None:
             rv = self.queue.get()
@@ -595,52 +613,53 @@
             return None
         except (self.channel.TimeoutError, EOFError):
             return None
         else:
             return LogRecord.from_dict(rv)
 
 
-class TWHThreadController(object):
+class TWHThreadController:
     """A very basic thread controller that pulls things in from a
     queue and sends it to a handler.  Both queue and handler are
     taken from the passed :class:`ThreadedWrapperHandler`.
     """
-    class Command(object):
+
+    class Command:
         stop = object()
         emit = object()
         emit_batch = object()
 
     def __init__(self, wrapper_handler):
         self.wrapper_handler = wrapper_handler
         self.running = False
         self._thread = None
 
     def start(self):
         """Starts the task thread."""
         self.running = True
         self._thread = Thread(target=self._target)
-        self._thread.setDaemon(True)
+        self._thread.daemon = True
         self._thread.start()
 
     def stop(self):
         """Stops the task thread."""
         if self.running:
-            self.wrapper_handler.queue.put_nowait((self.Command.stop, ))
+            self.wrapper_handler.queue.put_nowait((self.Command.stop,))
             self._thread.join()
             self._thread = None
 
     def _target(self):
         while 1:
             item = self.wrapper_handler.queue.get()
             command, data = item[0], item[1:]
             if command is self.Command.stop:
                 self.running = False
                 break
             elif command is self.Command.emit:
-                (record, ) = data
+                (record,) = data
                 self.wrapper_handler.handler.emit(record)
             elif command is self.Command.emit_batch:
                 record, reason = data
                 self.wrapper_handler.handler.emit_batch(record, reason)
 
 
 class ThreadedWrapperHandler(WrapperHandler):
@@ -655,15 +674,16 @@
 
     >>> twh = ThreadedWrapperHandler(TestHandler())
     >>> from logbook import WARNING
     >>> twh.level_name = 'WARNING'
     >>> twh.handler.level_name
     'WARNING'
     """
-    _direct_attrs = frozenset(['handler', 'queue', 'controller'])
+
+    _direct_attrs = frozenset(["handler", "queue", "controller"])
 
     def __init__(self, handler, maxsize=0):
         WrapperHandler.__init__(self, handler)
         self.queue = ThreadQueue(maxsize)
         self.controller = TWHThreadController(self)
         self.controller.start()
 
@@ -720,14 +740,15 @@
         subscribers = SubscriberGroup([
             MultiProcessingSubscriber(queue),
             ZeroMQSubscriber('tcp://127.0.0.1:5000')
         ])
         with target_handler:
             subscribers.dispatch_forever()
     """
+
     def __init__(self, subscribers=None, queue_limit=10):
         self.members = []
         self.queue = ThreadQueue(queue_limit)
         for subscriber in subscribers or []:
             self.add(subscriber)
 
     def add(self, subscriber):
```

### Comparing `Logbook-1.5.3/logbook/ticketing.py` & `Logbook-1.6.0/src/logbook/ticketing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# -*- coding: utf-8 -*-
 """
     logbook.ticketing
     ~~~~~~~~~~~~~~~~~
 
     Implements long handlers that write to remote data stores and assign
     each logging message a ticket id.
 
     :copyright: (c) 2010 by Armin Ronacher, Georg Brandl.
     :license: BSD, see LICENSE for more details.
 """
-from time import time
 import json
-from logbook.base import NOTSET, level_name_property, LogRecord
+from time import time
+
+from logbook.base import NOTSET, LogRecord, level_name_property
 from logbook.handlers import Handler, HashingHandlerMixin
-from logbook.helpers import cached_property, b, PY2, u
+from logbook.helpers import cached_property
 
 
-class Ticket(object):
+class Ticket:
     """Represents a ticket from the database."""
 
     level_name = level_name_property()
 
     def __init__(self, db, row):
         self.db = db
-        self.__dict__.update(row)
+        self.__dict__.update(row._mapping)
 
     @cached_property
     def last_occurrence(self):
         """The last occurrence."""
         rv = self.get_occurrences(limit=1)
         if rv:
             return rv[0]
 
-    def get_occurrences(self, order_by='-time', limit=50, offset=0):
+    def get_occurrences(self, order_by="-time", limit=50, offset=0):
         """Returns the occurrences for this ticket."""
         return self.db.get_occurrences(self.ticket_id, order_by, limit, offset)
 
     def solve(self):
         """Marks this ticket as solved."""
         self.db.solve_ticket(self.ticket_id)
         self.solved = True
@@ -60,22 +60,22 @@
         return not self.__eq__(other)
 
 
 class Occurrence(LogRecord):
     """Represents an occurrence of a ticket."""
 
     def __init__(self, db, row):
-        self.update_from_dict(json.loads(row['data']))
+        self.update_from_dict(json.loads(row.data))
         self.db = db
-        self.time = row['time']
-        self.ticket_id = row['ticket_id']
-        self.occurrence_id = row['occurrence_id']
+        self.time = row.time
+        self.ticket_id = row.ticket_id
+        self.occurrence_id = row.occurrence_id
 
 
-class BackendBase(object):
+class BackendBase:
     """Provides an abstract interface to various databases."""
 
     def __init__(self, **options):
         self.options = options
         self.setup_backend()
 
     def setup_backend(self):
@@ -86,16 +86,15 @@
         """Records a log record as ticket."""
         raise NotImplementedError()
 
     def count_tickets(self):
         """Returns the number of tickets."""
         raise NotImplementedError()
 
-    def get_tickets(self, order_by='-last_occurrence_time',
-                    limit=50, offset=0):
+    def get_tickets(self, order_by="-last_occurrence_time", limit=50, offset=0):
         """Selects tickets from the database."""
         raise NotImplementedError()
 
     def solve_ticket(self, ticket_id):
         """Marks a ticket as solved."""
         raise NotImplementedError()
 
@@ -103,15 +102,15 @@
         """Deletes a ticket from the database."""
         raise NotImplementedError()
 
     def get_ticket(self, ticket_id):
         """Return a single ticket with all occurrences."""
         raise NotImplementedError()
 
-    def get_occurrences(self, ticket, order_by='-time', limit=50, offset=0):
+    def get_occurrences(self, ticket, order_by="-time", limit=50, offset=0):
         """Selects occurrences from the database for a ticket."""
         raise NotImplementedError()
 
 
 class SQLAlchemyBackend(BackendBase):
     """Implements a backend that is writing into a database SQLAlchemy can
     interface.
@@ -128,28 +127,28 @@
     `autocreate_tables`
         can be set to `False` to disable the automatic
         creation of the logbook tables.
 
     """
 
     def setup_backend(self):
-        from sqlalchemy import create_engine, MetaData
-        from sqlalchemy.orm import sessionmaker, scoped_session
-        engine_or_uri = self.options.pop('uri', None)
-        metadata = self.options.pop('metadata', None)
-        table_prefix = self.options.pop('table_prefix', 'logbook_')
+        from sqlalchemy import MetaData, create_engine
+        from sqlalchemy.orm import scoped_session, sessionmaker
+
+        engine_or_uri = self.options.pop("uri", None)
+        metadata = self.options.pop("metadata", None)
+        table_prefix = self.options.pop("table_prefix", "logbook_")
 
-        if hasattr(engine_or_uri, 'execute'):
+        if hasattr(engine_or_uri, "execute"):
             self.engine = engine_or_uri
         else:
             # Pool recycle keeps connections from going stale,
             # which happens in MySQL Databases
             # Pool size is more custom for out stack
-            self.engine = create_engine(engine_or_uri, convert_unicode=True,
-                                        pool_recycle=360, pool_size=1000)
+            self.engine = create_engine(engine_or_uri, pool_recycle=360, pool_size=1000)
 
             # Create session factory using session maker
             session = sessionmaker()
 
             # Bind to the engined
             session.configure(bind=self.engine)
 
@@ -158,174 +157,212 @@
             self.session = scoped_session(session)
 
         if metadata is None:
             metadata = MetaData()
         self.table_prefix = table_prefix
         self.metadata = metadata
         self.create_tables()
-        if self.options.get('autocreate_tables', True):
+        if self.options.get("autocreate_tables", True):
             self.metadata.create_all(bind=self.engine)
 
     def create_tables(self):
         """Creates the tables required for the handler on the class and
         metadata.
         """
         import sqlalchemy as db
 
         def table(name, *args, **kwargs):
-            return db.Table(self.table_prefix + name, self.metadata,
-                            *args, **kwargs)
-        self.tickets = table('tickets',
-                             db.Column('ticket_id', db.Integer,
-                                       primary_key=True),
-                             db.Column('record_hash', db.String(40),
-                                       unique=True),
-                             db.Column('level', db.Integer),
-                             db.Column('channel', db.String(120)),
-                             db.Column('location', db.String(512)),
-                             db.Column('module', db.String(256)),
-                             db.Column('last_occurrence_time', db.DateTime),
-                             db.Column('occurrence_count', db.Integer),
-                             db.Column('solved', db.Boolean),
-                             db.Column('app_id', db.String(80)))
-        self.occurrences = table('occurrences',
-                                 db.Column('occurrence_id',
-                                           db.Integer, primary_key=True),
-                                 db.Column('ticket_id', db.Integer,
-                                           db.ForeignKey(self.table_prefix +
-                                                         'tickets.ticket_id')),
-                                 db.Column('time', db.DateTime),
-                                 db.Column('data', db.Text),
-                                 db.Column('app_id', db.String(80)))
+            return db.Table(self.table_prefix + name, self.metadata, *args, **kwargs)
+
+        self.tickets = table(
+            "tickets",
+            db.Column("ticket_id", db.Integer, primary_key=True),
+            db.Column("record_hash", db.String(40), unique=True),
+            db.Column("level", db.Integer),
+            db.Column("channel", db.String(120)),
+            db.Column("location", db.String(512)),
+            db.Column("module", db.String(256)),
+            db.Column("last_occurrence_time", db.DateTime),
+            db.Column("occurrence_count", db.Integer),
+            db.Column("solved", db.Boolean),
+            db.Column("app_id", db.String(80)),
+        )
+        self.occurrences = table(
+            "occurrences",
+            db.Column("occurrence_id", db.Integer, primary_key=True),
+            db.Column(
+                "ticket_id",
+                db.Integer,
+                db.ForeignKey(self.table_prefix + "tickets.ticket_id"),
+            ),
+            db.Column("time", db.DateTime),
+            db.Column("data", db.Text),
+            db.Column("app_id", db.String(80)),
+        )
 
     def _order(self, q, table, order_by):
-        if order_by[0] == '-':
+        if order_by[0] == "-":
             return q.order_by(table.c[order_by[1:]].desc())
         return q.order_by(table.c[order_by])
 
     def record_ticket(self, record, data, hash, app_id):
         """Records a log record as ticket."""
         # Can use the session instead engine.connection and transaction
         s = self.session
         try:
-            q = self.tickets.select(self.tickets.c.record_hash == hash)
-            row = s.execute(q).fetchone()
+            q = self.tickets.select().where(self.tickets.c.record_hash == hash)
+            row = s.execute(q).one_or_none()
             if row is None:
-                row = s.execute(self.tickets.insert().values(
-                    record_hash=hash,
-                    level=record.level,
-                    channel=record.channel or u(''),
-                    location=u('%s:%d') % (record.filename, record.lineno),
-                    module=record.module or u('<unknown>'),
-                    occurrence_count=0,
-                    solved=False,
-                    app_id=app_id
-                ))
+                row = s.execute(
+                    self.tickets.insert().values(
+                        record_hash=hash,
+                        level=record.level,
+                        channel=record.channel or "",
+                        location="%s:%d" % (record.filename, record.lineno),
+                        module=record.module or "<unknown>",
+                        occurrence_count=0,
+                        solved=False,
+                        app_id=app_id,
+                    )
+                )
                 ticket_id = row.inserted_primary_key[0]
             else:
-                ticket_id = row['ticket_id']
-            s.execute(self.occurrences.insert()
-                      .values(ticket_id=ticket_id,
-                              time=record.time,
-                              app_id=app_id,
-                              data=json.dumps(data)))
+                ticket_id = row.ticket_id
+            s.execute(
+                self.occurrences.insert().values(
+                    ticket_id=ticket_id,
+                    time=record.time,
+                    app_id=app_id,
+                    data=json.dumps(data),
+                )
+            )
             s.execute(
                 self.tickets.update()
                 .where(self.tickets.c.ticket_id == ticket_id)
-                .values(occurrence_count=self.tickets.c.occurrence_count + 1,
-                        last_occurrence_time=record.time,
-                        solved=False))
+                .values(
+                    occurrence_count=self.tickets.c.occurrence_count + 1,
+                    last_occurrence_time=record.time,
+                    solved=False,
+                )
+            )
             s.commit()
         except Exception:
             s.rollback()
             raise
         # Closes the session and removes it from the pool
         s.remove()
 
     def count_tickets(self):
         """Returns the number of tickets."""
-        return self.engine.execute(self.tickets.count()).fetchone()[0]
+        from sqlalchemy import func, select
 
-    def get_tickets(self, order_by='-last_occurrence_time', limit=50,
-                    offset=0):
+        with self.engine.begin() as conn:
+            return conn.scalar(select(func.count()).select_from(self.tickets))
+
+    def get_tickets(self, order_by="-last_occurrence_time", limit=50, offset=0):
         """Selects tickets from the database."""
-        return [Ticket(self, row) for row in self.engine.execute(
-            self._order(self.tickets.select(), self.tickets, order_by)
-            .limit(limit).offset(offset)).fetchall()]
+        with self.engine.begin() as conn:
+            return [
+                Ticket(self, row)
+                for row in conn.execute(
+                    self._order(self.tickets.select(), self.tickets, order_by)
+                    .limit(limit)
+                    .offset(offset)
+                )
+            ]
 
     def solve_ticket(self, ticket_id):
         """Marks a ticket as solved."""
-        self.engine.execute(self.tickets.update()
-                            .where(self.tickets.c.ticket_id == ticket_id)
-                            .values(solved=True))
+        with self.engine.begin() as conn:
+            conn.execute(
+                self.tickets.update()
+                .where(self.tickets.c.ticket_id == ticket_id)
+                .values(solved=True)
+            )
 
     def delete_ticket(self, ticket_id):
         """Deletes a ticket from the database."""
-        self.engine.execute(self.occurrences.delete()
-                            .where(self.occurrences.c.ticket_id == ticket_id))
-        self.engine.execute(self.tickets.delete()
-                            .where(self.tickets.c.ticket_id == ticket_id))
+        with self.engine.begin() as conn:
+            conn.execute(
+                self.occurrences.delete().where(
+                    self.occurrences.c.ticket_id == ticket_id
+                )
+            )
+            conn.execute(
+                self.tickets.delete().where(self.tickets.c.ticket_id == ticket_id)
+            )
 
     def get_ticket(self, ticket_id):
         """Return a single ticket with all occurrences."""
-        row = self.engine.execute(self.tickets.select().where(
-            self.tickets.c.ticket_id == ticket_id)).fetchone()
+        with self.engine.begin() as conn:
+            row = conn.execute(
+                self.tickets.select().where(self.tickets.c.ticket_id == ticket_id)
+            ).one_or_none()
         if row is not None:
             return Ticket(self, row)
 
-    def get_occurrences(self, ticket, order_by='-time', limit=50, offset=0):
+    def get_occurrences(self, ticket, order_by="-time", limit=50, offset=0):
         """Selects occurrences from the database for a ticket."""
-        return [Occurrence(self, row) for row in
-                self.engine.execute(self._order(
-                    self.occurrences.select()
-                    .where(self.occurrences.c.ticket_id == ticket),
-                    self.occurrences, order_by)
-                .limit(limit).offset(offset)).fetchall()]
+        with self.engine.begin() as conn:
+            return [
+                Occurrence(self, row)
+                for row in conn.execute(
+                    self._order(
+                        self.occurrences.select().where(
+                            self.occurrences.c.ticket_id == ticket
+                        ),
+                        self.occurrences,
+                        order_by,
+                    )
+                    .limit(limit)
+                    .offset(offset)
+                )
+            ]
 
 
 class MongoDBBackend(BackendBase):
     """Implements a backend that writes into a MongoDB database."""
 
     class _FixedTicketClass(Ticket):
         @property
         def ticket_id(self):
             return self._id
 
     class _FixedOccurrenceClass(Occurrence):
         def __init__(self, db, row):
-            self.update_from_dict(json.loads(row['data']))
+            self.update_from_dict(json.loads(row["data"]))
             self.db = db
-            self.time = row['time']
-            self.ticket_id = row['ticket_id']
-            self.occurrence_id = row['_id']
+            self.time = row["time"]
+            self.ticket_id = row["ticket_id"]
+            self.occurrence_id = row["_id"]
 
     # TODO: Update connection setup once PYTHON-160 is solved.
     def setup_backend(self):
         from pymongo import ASCENDING, DESCENDING
         from pymongo.connection import Connection
 
         try:
-                from pymongo.uri_parser import parse_uri
+            from pymongo.uri_parser import parse_uri
         except ImportError:
-                from pymongo.connection import _parse_uri as parse_uri
+            from pymongo.connection import _parse_uri as parse_uri
 
         from pymongo.errors import AutoReconnect
 
         _connection = None
-        uri = self.options.pop('uri', u(''))
+        uri = self.options.pop("uri", "")
         _connection_attempts = 0
 
         parsed_uri = parse_uri(uri, Connection.PORT)
 
         if type(parsed_uri) is tuple:
-                # pymongo < 2.0
-                database = parsed_uri[1]
+            # pymongo < 2.0
+            database = parsed_uri[1]
         else:
-                # pymongo >= 2.0
-                database = parsed_uri['database']
+            # pymongo >= 2.0
+            database = parsed_uri["database"]
 
         # Handle auto reconnect signals properly
         while _connection_attempts < 5:
             try:
                 if _connection is None:
                     _connection = Connection(uri)
                 database = _connection[database]
@@ -333,102 +370,104 @@
             except AutoReconnect:
                 _connection_attempts += 1
                 time.sleep(0.1)
 
         self.database = database
 
         # setup correct indexes
-        database.tickets.ensure_index([('record_hash', ASCENDING)],
-                                      unique=True)
-        database.tickets.ensure_index([('solved', ASCENDING),
-                                      ('level', ASCENDING)])
-        database.occurrences.ensure_index([('time', DESCENDING)])
+        database.tickets.ensure_index([("record_hash", ASCENDING)], unique=True)
+        database.tickets.ensure_index([("solved", ASCENDING), ("level", ASCENDING)])
+        database.occurrences.ensure_index([("time", DESCENDING)])
 
     def _order(self, q, order_by):
         from pymongo import ASCENDING, DESCENDING
-        col = '%s' % (order_by[0] == '-' and order_by[1:] or order_by)
-        if order_by[0] == '-':
+
+        col = "%s" % (order_by[0] == "-" and order_by[1:] or order_by)
+        if order_by[0] == "-":
             return q.sort(col, DESCENDING)
         return q.sort(col, ASCENDING)
 
     def _oid(self, ticket_id):
         from pymongo.objectid import ObjectId
+
         return ObjectId(ticket_id)
 
     def record_ticket(self, record, data, hash, app_id):
         """Records a log record as ticket."""
         db = self.database
-        ticket = db.tickets.find_one({'record_hash': hash})
+        ticket = db.tickets.find_one({"record_hash": hash})
         if not ticket:
             doc = {
-                'record_hash':      hash,
-                'level':            record.level,
-                'channel':          record.channel or u(''),
-                'location':         u('%s:%d') % (record.filename,
-                                                  record.lineno),
-                'module':           record.module or u('<unknown>'),
-                'occurrence_count': 0,
-                'solved':           False,
-                'app_id':           app_id,
+                "record_hash": hash,
+                "level": record.level,
+                "channel": record.channel or "",
+                "location": "%s:%d" % (record.filename, record.lineno),
+                "module": record.module or "<unknown>",
+                "occurrence_count": 0,
+                "solved": False,
+                "app_id": app_id,
             }
             ticket_id = db.tickets.insert(doc)
         else:
-            ticket_id = ticket['_id']
+            ticket_id = ticket["_id"]
 
-        db.tickets.update({'_id': ticket_id}, {
-            '$inc': {
-                'occurrence_count': 1
+        db.tickets.update(
+            {"_id": ticket_id},
+            {
+                "$inc": {"occurrence_count": 1},
+                "$set": {"last_occurrence_time": record.time, "solved": False},
             },
-            '$set': {
-                'last_occurrence_time': record.time,
-                'solved':               False
-            }
-        })
+        )
         # We store occurrences in a seperate collection so that
         # we can make it a capped collection optionally.
-        db.occurrences.insert({
-            'ticket_id':    self._oid(ticket_id),
-            'app_id':       app_id,
-            'time':         record.time,
-            'data':         json.dumps(data),
-        })
+        db.occurrences.insert(
+            {
+                "ticket_id": self._oid(ticket_id),
+                "app_id": app_id,
+                "time": record.time,
+                "data": json.dumps(data),
+            }
+        )
 
     def count_tickets(self):
         """Returns the number of tickets."""
         return self.database.tickets.count()
 
-    def get_tickets(self, order_by='-last_occurrence_time', limit=50,
-                    offset=0):
+    def get_tickets(self, order_by="-last_occurrence_time", limit=50, offset=0):
         """Selects tickets from the database."""
-        query = (self._order(self.database.tickets.find(), order_by)
-                 .limit(limit).skip(offset))
+        query = (
+            self._order(self.database.tickets.find(), order_by)
+            .limit(limit)
+            .skip(offset)
+        )
         return [self._FixedTicketClass(self, obj) for obj in query]
 
     def solve_ticket(self, ticket_id):
         """Marks a ticket as solved."""
-        self.database.tickets.update({'_id': self._oid(ticket_id)},
-                                     {'solved': True})
+        self.database.tickets.update({"_id": self._oid(ticket_id)}, {"solved": True})
 
     def delete_ticket(self, ticket_id):
         """Deletes a ticket from the database."""
-        self.database.occurrences.remove({'ticket_id': self._oid(ticket_id)})
-        self.database.tickets.remove({'_id': self._oid(ticket_id)})
+        self.database.occurrences.remove({"ticket_id": self._oid(ticket_id)})
+        self.database.tickets.remove({"_id": self._oid(ticket_id)})
 
     def get_ticket(self, ticket_id):
         """Return a single ticket with all occurrences."""
-        ticket = self.database.tickets.find_one({'_id': self._oid(ticket_id)})
+        ticket = self.database.tickets.find_one({"_id": self._oid(ticket_id)})
         if ticket:
             return Ticket(self, ticket)
 
-    def get_occurrences(self, ticket, order_by='-time', limit=50, offset=0):
+    def get_occurrences(self, ticket, order_by="-time", limit=50, offset=0):
         """Selects occurrences from the database for a ticket."""
         collection = self.database.occurrences
-        occurrences = self._order(collection.find(
-            {'ticket_id': self._oid(ticket)}
-        ), order_by).limit(limit).skip(offset)
+        occurrences = (
+            self._order(collection.find({"ticket_id": self._oid(ticket)}), order_by)
+            .limit(limit)
+            .skip(offset)
+        )
         return [self._FixedOccurrenceClass(self, obj) for obj in occurrences]
 
 
 class TicketingBaseHandler(Handler, HashingHandlerMixin):
     """Baseclass for ticketing handlers.  This can be used to interface
     ticketing systems that do not necessarily provide an interface that
     would be compatible with the :class:`BackendBase` interface.
@@ -439,17 +478,16 @@
         self.hash_salt = hash_salt
 
     def hash_record_raw(self, record):
         """Returns the unique hash of a record."""
         hash = HashingHandlerMixin.hash_record_raw(self, record)
         if self.hash_salt is not None:
             hash_salt = self.hash_salt
-            if not PY2 or isinstance(hash_salt, unicode):
-                hash_salt = hash_salt.encode('utf-8')
-            hash.update(b('\x00') + hash_salt)
+            hash_salt = hash_salt.encode("utf-8")
+            hash.update(b"\x00" + hash_salt)
         return hash
 
 
 class TicketingHandler(TicketingBaseHandler):
     """A handler that writes log records into a remote database.  This
     database can be connected to from different dispatchers which makes
     this a nice setup for web applications::
@@ -469,23 +507,31 @@
     """
 
     #: The default backend that is being used when no backend is specified.
     #: Unless overriden by a subclass this will be the
     #: :class:`SQLAlchemyBackend`.
     default_backend = SQLAlchemyBackend
 
-    def __init__(self, uri, app_id='generic', level=NOTSET,
-                 filter=None, bubble=False, hash_salt=None, backend=None,
-                 **db_options):
+    def __init__(
+        self,
+        uri,
+        app_id="generic",
+        level=NOTSET,
+        filter=None,
+        bubble=False,
+        hash_salt=None,
+        backend=None,
+        **db_options,
+    ):
         if hash_salt is None:
-            hash_salt = u('apphash-') + app_id
+            hash_salt = "apphash-" + app_id
         TicketingBaseHandler.__init__(self, hash_salt, level, filter, bubble)
         if backend is None:
             backend = self.default_backend
-        db_options['uri'] = uri
+        db_options["uri"] = uri
         self.set_backend(backend, **db_options)
         self.app_id = app_id
 
     def set_backend(self, cls, **options):
         self.db = cls(**options)
 
     def process_record(self, record, hash):
@@ -498,10 +544,10 @@
         """Record either a new ticket or a new occurrence for a
         ticket based on the hash.
         """
         self.db.record_ticket(record, data, hash, self.app_id)
 
     def emit(self, record):
         """Emits a single record and writes it to the database."""
-        hash = self.hash_record(record).encode('utf-8')
+        hash = self.hash_record(record).encode("utf-8")
         data = self.process_record(record, hash)
         self.record_ticket(record, data, hash)
```

### Comparing `Logbook-1.5.3/logbook/utils.py` & `Logbook-1.6.0/src/logbook/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-from contextlib import contextmanager
 import functools
 import sys
 import threading
+from contextlib import contextmanager
 
-from .base import Logger, DEBUG
-from .helpers import string_types
-
+from .base import DEBUG, Logger
 
-class _SlowContextNotifier(object):
 
+class _SlowContextNotifier:
     def __init__(self, threshold, func):
         self.timer = threading.Timer(threshold, func)
 
     def __enter__(self):
         self.timer.start()
         return self
 
     def __exit__(self, *_):
         self.timer.cancel()
 
 
-_slow_logger = Logger('Slow')
+_slow_logger = Logger("Slow")
 
 
 def logged_if_slow(*args, **kwargs):
     """Context manager that logs if operations within take longer than
     `threshold` seconds.
 
     :param threshold: Number of seconds (or fractions thereof) allwoed before
@@ -33,32 +31,35 @@
                    logger.
     :param level: Log level. The default is `DEBUG`.
     :param func: (Deprecated). Function to call to perform logging.
 
     The remaining parameters are passed to the
     :meth:`~logbook.base.LoggerMixin.log` method.
     """
-    threshold = kwargs.pop('threshold', 1)
-    func = kwargs.pop('func', None)
+    threshold = kwargs.pop("threshold", 1)
+    func = kwargs.pop("func", None)
     if func is None:
-        logger = kwargs.pop('logger', _slow_logger)
-        level = kwargs.pop('level', DEBUG)
+        logger = kwargs.pop("logger", _slow_logger)
+        level = kwargs.pop("level", DEBUG)
         func = functools.partial(logger.log, level, *args, **kwargs)
     else:
-        if 'logger' in kwargs or 'level' in kwargs:
-            raise TypeError("If using deprecated func parameter, 'logger' and"
-                            " 'level' arguments cannot be passed.")
+        if "logger" in kwargs or "level" in kwargs:
+            raise TypeError(
+                "If using deprecated func parameter, 'logger' and"
+                " 'level' arguments cannot be passed."
+            )
         func = functools.partial(func, *args, **kwargs)
 
     return _SlowContextNotifier(threshold, func)
 
 
 class _Local(threading.local):
     enabled = True
 
+
 _local = _Local()
 
 
 @contextmanager
 def suppressed_deprecations():
     """Disables deprecation messages temporarily
 
@@ -82,79 +83,78 @@
 def forget_deprecation_locations():
     _deprecation_locations.clear()
 
 
 def _write_deprecations_if_needed(message, frame_correction):
     if not _local.enabled:
         return
-    caller_location = _get_caller_location(frame_correction=frame_correction+1)
+    caller_location = _get_caller_location(frame_correction=frame_correction + 1)
     if caller_location not in _deprecation_locations:
-        _deprecation_logger.warning(message, frame_correction=frame_correction+1)
+        _deprecation_logger.warning(message, frame_correction=frame_correction + 1)
         _deprecation_locations.add(caller_location)
 
 
 def log_deprecation_message(message, frame_correction=0):
-    _write_deprecations_if_needed("Deprecation message: {0}".format(message), frame_correction=frame_correction+1)
-
+    _write_deprecations_if_needed(
+        f"Deprecation message: {message}", frame_correction=frame_correction + 1
+    )
 
-class _DeprecatedFunction(object):
 
+class _DeprecatedFunction:
     def __init__(self, func, message, obj=None, objtype=None):
-        super(_DeprecatedFunction, self).__init__()
+        super().__init__()
         self._func = func
         self._message = message
         self._obj = obj
         self._objtype = objtype
 
     def _get_underlying_func(self):
         returned = self._func
         if isinstance(returned, classmethod):
-            if hasattr(returned, '__func__'):
+            if hasattr(returned, "__func__"):
                 returned = returned.__func__
             else:
                 returned = returned.__get__(self._objtype).__func__
         return returned
 
     def __call__(self, *args, **kwargs):
         func = self._get_underlying_func()
-        warning = "{0} is deprecated.".format(self._get_func_str())
+        warning = f"{self._get_func_str()} is deprecated."
         if self._message is not None:
-            warning += " {0}".format(self._message)
+            warning += f" {self._message}"
         _write_deprecations_if_needed(warning, frame_correction=+1)
         if self._obj is not None:
             return func(self._obj, *args, **kwargs)
         elif self._objtype is not None:
             return func(self._objtype, *args, **kwargs)
         return func(*args, **kwargs)
 
     def _get_func_str(self):
         func = self._get_underlying_func()
         if self._objtype is not None:
-            return '{0}.{1}'.format(self._objtype.__name__, func.__name__)
-        return '{0}.{1}'.format(func.__module__, func.__name__)
+            return f"{self._objtype.__name__}.{func.__name__}"
+        return f"{func.__module__}.{func.__name__}"
 
     def __get__(self, obj, objtype):
         return self.bound_to(obj, objtype)
 
     def bound_to(self, obj, objtype):
-        return _DeprecatedFunction(self._func, self._message, obj=obj,
-                                   objtype=objtype)
+        return _DeprecatedFunction(self._func, self._message, obj=obj, objtype=objtype)
 
     @property
     def __name__(self):
         return self._get_underlying_func().__name__
 
     @property
     def __doc__(self):
         returned = self._get_underlying_func().__doc__
         if returned:  # pylint: disable=no-member
             returned += "\n.. deprecated\n"  # pylint: disable=no-member
             if self._message:
-                returned += "   {0}".format(
-                    self._message)  # pylint: disable=no-member
+                returned += f"   {self._message}"  # pylint: disable=no-member
         return returned
 
     @__doc__.setter
     def __doc__(self, doc):
         self._get_underlying_func().__doc__ = doc
 
 
@@ -167,15 +167,15 @@
     ...     pass
 
     This will cause a warning log to be emitted when the function gets called,
     with the correct filename/lineno.
 
     .. versionadded:: 0.12
     """
-    if isinstance(func, string_types):
+    if isinstance(func, str):
         assert message is None
         message = func
         func = None
 
     if func is None:
         return functools.partial(deprecated, message=message)
```

### Comparing `Logbook-1.5.3/tests/conftest.py` & `Logbook-1.6.0/tests/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import sys
+from pathlib import Path
 
-import logbook
 import pytest
 
+import logbook
+
 logbook.StderrHandler().push_application()
 
 
 @pytest.fixture
 def logger():
-    return logbook.Logger('testlogger')
+    return logbook.Logger("testlogger")
 
 
 @pytest.fixture
 def active_handler(request, test_handler, activation_strategy):
-
     s = activation_strategy(test_handler)
     s.activate()
 
     @request.addfinalizer
     def deactivate():
         s.deactivate()
 
@@ -25,18 +25,17 @@
 
 
 @pytest.fixture
 def test_handler():
     return logbook.TestHandler()
 
 
-class ActivationStrategy(object):
-
+class ActivationStrategy:
     def __init__(self, handler):
-        super(ActivationStrategy, self).__init__()
+        super().__init__()
         self.handler = handler
 
     def activate(self):
         raise NotImplementedError()  # pragma: no cover
 
     def deactivate(self):
         raise NotImplementedError()  # pragma: no cover
@@ -46,72 +45,81 @@
         return self.handler
 
     def __exit__(self, *_):
         self.deactivate()
 
 
 class ContextEnteringStrategy(ActivationStrategy):
-
     def activate(self):
         self.handler.__enter__()
 
     def deactivate(self):
         self.handler.__exit__(None, None, None)
 
 
 class PushingStrategy(ActivationStrategy):
-
     def activate(self):
         from logbook.concurrency import is_gevent_enabled
+
         if is_gevent_enabled():
             self.handler.push_greenlet()
         else:
             self.handler.push_thread()
 
     def deactivate(self):
         from logbook.concurrency import is_gevent_enabled
+
         if is_gevent_enabled():
             self.handler.pop_greenlet()
         else:
             self.handler.pop_thread()
 
 
 @pytest.fixture(params=[ContextEnteringStrategy, PushingStrategy])
 def activation_strategy(request):
     return request.param
 
 
-@pytest.fixture
-def logfile(tmpdir):
-    return str(tmpdir.join('logfile.log'))
+class CustomPathLike:
+    def __init__(self, path):
+        self.path = path
+
+    def __fspath__(self):
+        return self.path
+
+
+@pytest.fixture(params=[Path, str, CustomPathLike])
+def logfile(tmp_path, request):
+    path = str(tmp_path / "logfile.log")
+    return request.param(path)
 
 
 @pytest.fixture
 def default_handler(request):
     returned = logbook.StderrHandler()
     returned.push_application()
     request.addfinalizer(returned.pop_application)
     return returned
 
+
 try:
     import gevent
 except ImportError:
     pass
 else:
-    @pytest.fixture(scope="module", autouse=True, params=[False, True])
+
+    @pytest.fixture(
+        scope="module", autouse=True, params=[False, True], ids=["nogevent", "gevent"]
+    )
     def gevent(request):
-        module_name = getattr(request.module, '__name__', '')
-        if (not any(s in module_name for s in ('queues', 'processors'))
-                and request.param):
-            from logbook.concurrency import enable_gevent, _disable_gevent
+        module_name = getattr(request.module, "__name__", "")
+        if (
+            not any(s in module_name for s in ("queues", "processors"))
+            and request.param
+        ):
+            from logbook.concurrency import _disable_gevent, enable_gevent
+
             enable_gevent()
 
             @request.addfinalizer
             def fin():
                 _disable_gevent()
-
-
-def pytest_ignore_collect(path, config):
-    if 'test_asyncio.py' in path.basename and (sys.version_info.major < 3 or sys.version_info.minor < 5):
-        return True
-
-    return False
```

### Comparing `Logbook-1.5.3/tests/test_asyncio.py` & `Logbook-1.6.0/tests/test_asyncio.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import pytest
-import logbook
 import asyncio
-from logbook.concurrency import has_contextvars
+
+import logbook
 
 ITERATIONS = 100
 
 
-@pytest.mark.skipif(not has_contextvars, reason="Contexvars not available")
 def test_asyncio_context_management(logger):
     h1 = logbook.TestHandler()
     h2 = logbook.TestHandler()
 
     async def task(handler, msg):
         for _ in range(ITERATIONS):
             with handler.contextbound():
                 logger.info(msg)
 
             await asyncio.sleep(0)  # allow for context switch
 
-    asyncio.get_event_loop().run_until_complete(asyncio.gather(task(h1, 'task1'), task(h2, 'task2')))
+    asyncio.get_event_loop().run_until_complete(
+        asyncio.gather(task(h1, "task1"), task(h2, "task2"))
+    )
 
     assert len(h1.records) == ITERATIONS
-    assert all(['task1' == r.msg for r in h1.records])
+    assert all(["task1" == r.msg for r in h1.records])
 
     assert len(h2.records) == ITERATIONS
-    assert all(['task2' == r.msg for r in h2.records])
+    assert all(["task2" == r.msg for r in h2.records])
```

### Comparing `Logbook-1.5.3/tests/test_file_handler.py` & `Logbook-1.6.0/tests/test_file_handler.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,242 +1,246 @@
+import gzip
 import os
-import pytest
 import time
 from datetime import datetime
 
-import logbook
-from logbook.helpers import u, xrange
-import gzip
 import brotli
-from .utils import capturing_stderr_context, LETTERS
+import pytest
+
+import logbook
+
+from .utils import LETTERS, capturing_stderr_context
 
 
 def test_file_handler(logfile, activation_strategy, logger):
     handler = logbook.FileHandler(
         logfile,
-        format_string='{record.level_name}:{record.channel}:{record.message}',)
+        format_string="{record.level_name}:{record.channel}:{record.message}",
+    )
     with activation_strategy(handler):
-        logger.warn('warning message')
+        logger.warn("warning message")
     handler.close()
     with open(logfile) as f:
-        assert f.readline() == 'WARNING:testlogger:warning message\n'
+        assert f.readline() == "WARNING:testlogger:warning message\n"
 
 
 def test_file_handler_unicode(logfile, activation_strategy, logger):
     with capturing_stderr_context() as captured:
         with activation_strategy(logbook.FileHandler(logfile)):
-            logger.info(u('\u0431'))
-    assert (not captured.getvalue())
+            logger.info("\u0431")
+    assert not captured.getvalue()
 
 
 def test_file_handler_delay(logfile, activation_strategy, logger):
     handler = logbook.FileHandler(
         logfile,
-        format_string='{record.level_name}:{record.channel}:{record.message}',
-        delay=True)
-    assert (not os.path.isfile(logfile))
+        format_string="{record.level_name}:{record.channel}:{record.message}",
+        delay=True,
+    )
+    assert not os.path.isfile(logfile)
     with activation_strategy(handler):
-        logger.warn('warning message')
+        logger.warn("warning message")
     handler.close()
 
     with open(logfile) as f:
-        assert f.readline() == 'WARNING:testlogger:warning message\n'
+        assert f.readline() == "WARNING:testlogger:warning message\n"
 
 
 def test_monitoring_file_handler(logfile, activation_strategy, logger):
-    if os.name == 'nt':
-        pytest.skip(
-            'unsupported on windows due to different IO (also unneeded)')
+    if os.name == "nt":
+        pytest.skip("unsupported on windows due to different IO (also unneeded)")
     handler = logbook.MonitoringFileHandler(
         logfile,
-        format_string='{record.level_name}:{record.channel}:{record.message}',
-        delay=True)
+        format_string="{record.level_name}:{record.channel}:{record.message}",
+        delay=True,
+    )
     with activation_strategy(handler):
-        logger.warn('warning message')
-        os.rename(logfile, logfile + '.old')
-        logger.warn('another warning message')
+        logger.warn("warning message")
+        os.rename(logfile, os.fspath(logfile) + ".old")
+        logger.warn("another warning message")
     handler.close()
     with open(logfile) as f:
-        assert f.read().strip() == 'WARNING:testlogger:another warning message'
+        assert f.read().strip() == "WARNING:testlogger:another warning message"
 
 
 def test_custom_formatter(activation_strategy, logfile, logger):
     def custom_format(record, handler):
-        return record.level_name + ':' + record.message
+        return record.level_name + ":" + record.message
 
     handler = logbook.FileHandler(logfile)
     with activation_strategy(handler):
         handler.formatter = custom_format
-        logger.warn('Custom formatters are awesome')
+        logger.warn("Custom formatters are awesome")
 
     with open(logfile) as f:
-        assert f.readline() == 'WARNING:Custom formatters are awesome\n'
+        assert f.readline() == "WARNING:Custom formatters are awesome\n"
 
 
 def test_rotating_file_handler(logfile, activation_strategy, logger):
     basename = os.path.basename(logfile)
-    handler = logbook.RotatingFileHandler(logfile, max_size=2048,
-                                          backup_count=3,
-                                          )
-    handler.format_string = '{record.message}'
+    handler = logbook.RotatingFileHandler(
+        logfile,
+        max_size=2048,
+        backup_count=3,
+    )
+    handler.format_string = "{record.message}"
     with activation_strategy(handler):
-        for c, x in zip(LETTERS, xrange(32)):
+        for c, x in zip(LETTERS, range(32)):
             logger.warn(c * 256)
-    files = [x for x in os.listdir(os.path.dirname(logfile))
-             if x.startswith(basename)]
+    files = [x for x in os.listdir(os.path.dirname(logfile)) if x.startswith(basename)]
     files.sort()
 
-    assert files == [basename, basename +
-                     '.1', basename + '.2', basename + '.3']
+    assert files == [basename, basename + ".1", basename + ".2", basename + ".3"]
     with open(logfile) as f:
-        assert f.readline().rstrip() == ('C' * 256)
-        assert f.readline().rstrip() == ('D' * 256)
-        assert f.readline().rstrip() == ('E' * 256)
-        assert f.readline().rstrip() == ('F' * 256)
+        assert f.readline().rstrip() == ("C" * 256)
+        assert f.readline().rstrip() == ("D" * 256)
+        assert f.readline().rstrip() == ("E" * 256)
+        assert f.readline().rstrip() == ("F" * 256)
 
 
 @pytest.mark.parametrize("backup_count", [1, 3])
 def test_timed_rotating_file_handler(tmpdir, activation_strategy, backup_count):
-    basename = str(tmpdir.join('trot.log'))
-    handler = logbook.TimedRotatingFileHandler(
-        basename, backup_count=backup_count)
-    handler.format_string = '[{record.time:%H:%M}] {record.message}'
+    basename = str(tmpdir.join("trot.log"))
+    handler = logbook.TimedRotatingFileHandler(basename, backup_count=backup_count)
+    handler.format_string = "[{record.time:%H:%M}] {record.message}"
 
-    def fake_record(message, year, month, day, hour=0,
-                    minute=0, second=0):
-        lr = logbook.LogRecord('Test Logger', logbook.WARNING,
-                               message)
+    def fake_record(message, year, month, day, hour=0, minute=0, second=0):
+        lr = logbook.LogRecord("Test Logger", logbook.WARNING, message)
         lr.time = datetime(year, month, day, hour, minute, second)
         return lr
 
     with activation_strategy(handler):
-        for x in xrange(10):
-            handler.handle(fake_record('First One', 2010, 1, 5, x + 1))
-        for x in xrange(20):
-            handler.handle(fake_record('Second One', 2010, 1, 6, x + 1))
-        for x in xrange(10):
-            handler.handle(fake_record('Third One', 2010, 1, 7, x + 1))
-        for x in xrange(20):
-            handler.handle(fake_record('Last One', 2010, 1, 8, x + 1))
-
-    files = sorted(x for x in os.listdir(str(tmpdir)) if x.startswith('trot'))
-
-    assert files == ['trot-2010-01-0{0}.log'.format(i)
-                     for i in xrange(5, 9)][-backup_count:]
-    with open(str(tmpdir.join('trot-2010-01-08.log'))) as f:
-        assert f.readline().rstrip() == '[01:00] Last One'
-        assert f.readline().rstrip() == '[02:00] Last One'
+        for x in range(10):
+            handler.handle(fake_record("First One", 2010, 1, 5, x + 1))
+        for x in range(20):
+            handler.handle(fake_record("Second One", 2010, 1, 6, x + 1))
+        for x in range(10):
+            handler.handle(fake_record("Third One", 2010, 1, 7, x + 1))
+        for x in range(20):
+            handler.handle(fake_record("Last One", 2010, 1, 8, x + 1))
+
+    files = sorted(x for x in os.listdir(str(tmpdir)) if x.startswith("trot"))
+
+    assert files == [f"trot-2010-01-0{i}.log" for i in range(5, 9)][-backup_count:]
+    with open(str(tmpdir.join("trot-2010-01-08.log"))) as f:
+        assert f.readline().rstrip() == "[01:00] Last One"
+        assert f.readline().rstrip() == "[02:00] Last One"
     if backup_count > 1:
-        with open(str(tmpdir.join('trot-2010-01-07.log'))) as f:
-            assert f.readline().rstrip() == '[01:00] Third One'
-            assert f.readline().rstrip() == '[02:00] Third One'
+        with open(str(tmpdir.join("trot-2010-01-07.log"))) as f:
+            assert f.readline().rstrip() == "[01:00] Third One"
+            assert f.readline().rstrip() == "[02:00] Third One"
+
 
 @pytest.mark.parametrize("backup_count", [1, 3])
-def test_timed_rotating_file_handler__rollover_format(tmpdir, activation_strategy, backup_count):
-    basename = str(tmpdir.join('trot.log'))
+def test_timed_rotating_file_handler__rollover_format(
+    tmpdir, activation_strategy, backup_count
+):
+    basename = str(tmpdir.join("trot.log"))
     handler = logbook.TimedRotatingFileHandler(
-        basename, backup_count=backup_count,
-        rollover_format='{basename}{ext}.{timestamp}',
+        basename,
+        backup_count=backup_count,
+        rollover_format="{basename}{ext}.{timestamp}",
     )
-    handler.format_string = '[{record.time:%H:%M}] {record.message}'
+    handler.format_string = "[{record.time:%H:%M}] {record.message}"
 
-    def fake_record(message, year, month, day, hour=0,
-                    minute=0, second=0):
-        lr = logbook.LogRecord('Test Logger', logbook.WARNING,
-                               message)
+    def fake_record(message, year, month, day, hour=0, minute=0, second=0):
+        lr = logbook.LogRecord("Test Logger", logbook.WARNING, message)
         lr.time = datetime(year, month, day, hour, minute, second)
         return lr
 
     with activation_strategy(handler):
-        for x in xrange(10):
-            handler.handle(fake_record('First One', 2010, 1, 5, x + 1))
-        for x in xrange(20):
-            handler.handle(fake_record('Second One', 2010, 1, 6, x + 1))
-        for x in xrange(10):
-            handler.handle(fake_record('Third One', 2010, 1, 7, x + 1))
-        for x in xrange(20):
-            handler.handle(fake_record('Last One', 2010, 1, 8, x + 1))
-
-    files = sorted(x for x in os.listdir(str(tmpdir)) if x.startswith('trot'))
-
-    assert files == ['trot.log.2010-01-0{0}'.format(i)
-                     for i in xrange(5, 9)][-backup_count:]
-    with open(str(tmpdir.join('trot.log.2010-01-08'))) as f:
-        assert f.readline().rstrip() == '[01:00] Last One'
-        assert f.readline().rstrip() == '[02:00] Last One'
+        for x in range(10):
+            handler.handle(fake_record("First One", 2010, 1, 5, x + 1))
+        for x in range(20):
+            handler.handle(fake_record("Second One", 2010, 1, 6, x + 1))
+        for x in range(10):
+            handler.handle(fake_record("Third One", 2010, 1, 7, x + 1))
+        for x in range(20):
+            handler.handle(fake_record("Last One", 2010, 1, 8, x + 1))
+
+    files = sorted(x for x in os.listdir(str(tmpdir)) if x.startswith("trot"))
+
+    assert files == [f"trot.log.2010-01-0{i}" for i in range(5, 9)][-backup_count:]
+    with open(str(tmpdir.join("trot.log.2010-01-08"))) as f:
+        assert f.readline().rstrip() == "[01:00] Last One"
+        assert f.readline().rstrip() == "[02:00] Last One"
     if backup_count > 1:
-        with open(str(tmpdir.join('trot.log.2010-01-07'))) as f:
-            assert f.readline().rstrip() == '[01:00] Third One'
-            assert f.readline().rstrip() == '[02:00] Third One'
+        with open(str(tmpdir.join("trot.log.2010-01-07"))) as f:
+            assert f.readline().rstrip() == "[01:00] Third One"
+            assert f.readline().rstrip() == "[02:00] Third One"
 
 
 @pytest.mark.parametrize("backup_count", [1, 3])
 @pytest.mark.parametrize("preexisting_file", [True, False])
 def test_timed_rotating_file_handler__not_timed_filename_for_current(
-        tmpdir, activation_strategy, backup_count, preexisting_file
+    tmpdir, activation_strategy, backup_count, preexisting_file
 ):
-    basename = str(tmpdir.join('trot.log'))
+    basename = str(tmpdir.join("trot.log"))
 
     if preexisting_file:
-        with open(basename, 'w') as file:
-            file.write('contents')
+        with open(basename, "w") as file:
+            file.write("contents")
         jan_first = time.mktime(datetime(2010, 1, 1).timetuple())
         os.utime(basename, (jan_first, jan_first))
 
     handler = logbook.TimedRotatingFileHandler(
         basename,
-        format_string='[{record.time:%H:%M}] {record.message}',
+        format_string="[{record.time:%H:%M}] {record.message}",
         backup_count=backup_count,
-        rollover_format='{basename}{ext}.{timestamp}',
+        rollover_format="{basename}{ext}.{timestamp}",
         timed_filename_for_current=False,
     )
 
-    def fake_record(message, year, month, day, hour=0,
-                    minute=0, second=0):
-        lr = logbook.LogRecord('Test Logger', logbook.WARNING,
-                               message)
+    def fake_record(message, year, month, day, hour=0, minute=0, second=0):
+        lr = logbook.LogRecord("Test Logger", logbook.WARNING, message)
         lr.time = datetime(year, month, day, hour, minute, second)
         return lr
 
     with activation_strategy(handler):
-        for x in xrange(10):
-            handler.handle(fake_record('First One', 2010, 1, 5, x + 1))
-        for x in xrange(20):
-            handler.handle(fake_record('Second One', 2010, 1, 6, x + 1))
-        for x in xrange(10):
-            handler.handle(fake_record('Third One', 2010, 1, 7, x + 1))
-        for x in xrange(20):
-            handler.handle(fake_record('Last One', 2010, 1, 8, x + 1))
-
-    computed_files = [x for x in os.listdir(str(tmpdir)) if x.startswith('trot')]
-
-    expected_files = ['trot.log.2010-01-01'] if preexisting_file else []
-    expected_files += ['trot.log.2010-01-0{0}'.format(i) for i in xrange(5, 8)]
-    expected_files += ['trot.log']
+        for x in range(10):
+            handler.handle(fake_record("First One", 2010, 1, 5, x + 1))
+        for x in range(20):
+            handler.handle(fake_record("Second One", 2010, 1, 6, x + 1))
+        for x in range(10):
+            handler.handle(fake_record("Third One", 2010, 1, 7, x + 1))
+        for x in range(20):
+            handler.handle(fake_record("Last One", 2010, 1, 8, x + 1))
+
+    computed_files = [x for x in os.listdir(str(tmpdir)) if x.startswith("trot")]
+
+    expected_files = ["trot.log.2010-01-01"] if preexisting_file else []
+    expected_files += [f"trot.log.2010-01-0{i}" for i in range(5, 8)]
+    expected_files += ["trot.log"]
     expected_files = expected_files[-backup_count:]
 
     assert sorted(computed_files) == sorted(expected_files)
 
-    with open(str(tmpdir.join('trot.log'))) as f:
-        assert f.readline().rstrip() == '[01:00] Last One'
-        assert f.readline().rstrip() == '[02:00] Last One'
+    with open(str(tmpdir.join("trot.log"))) as f:
+        assert f.readline().rstrip() == "[01:00] Last One"
+        assert f.readline().rstrip() == "[02:00] Last One"
     if backup_count > 1:
-        with open(str(tmpdir.join('trot.log.2010-01-07'))) as f:
-            assert f.readline().rstrip() == '[01:00] Third One'
-            assert f.readline().rstrip() == '[02:00] Third One'
+        with open(str(tmpdir.join("trot.log.2010-01-07"))) as f:
+            assert f.readline().rstrip() == "[01:00] Third One"
+            assert f.readline().rstrip() == "[02:00] Third One"
+
 
 def _decompress(input_file_name, use_gzip=True):
     if use_gzip:
-        with gzip.open(input_file_name, 'rb') as in_f:
+        with gzip.open(input_file_name, "rb") as in_f:
             return in_f.read().decode()
     else:
-        with open(input_file_name, 'rb') as in_f:
+        with open(input_file_name, "rb") as in_f:
             return brotli.decompress(in_f.read()).decode()
 
+
 @pytest.mark.parametrize("use_gzip", [True, False])
 def test_compression_file_handler(logfile, activation_strategy, logger, use_gzip):
-    handler = logbook.GZIPCompressionHandler(logfile) if use_gzip else logbook.BrotliCompressionHandler(logfile)
-    handler.format_string = '{record.level_name}:{record.channel}:{record.message}'
+    handler = (
+        logbook.GZIPCompressionHandler(logfile)
+        if use_gzip
+        else logbook.BrotliCompressionHandler(logfile)
+    )
+    handler.format_string = "{record.level_name}:{record.channel}:{record.message}"
     with activation_strategy(handler):
-        logger.warn('warning message')
+        logger.warn("warning message")
     handler.close()
-    assert  _decompress(logfile, use_gzip) == 'WARNING:testlogger:warning message\n'
+    assert _decompress(logfile, use_gzip) == "WARNING:testlogger:warning message\n"
```

### Comparing `Logbook-1.5.3/tests/test_fingers_crossed_handler.py` & `Logbook-1.6.0/tests/test_fingers_crossed_handler.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,77 +1,77 @@
 import logbook
 
 from .utils import capturing_stderr_context
 
 
 def test_fingerscrossed(activation_strategy, logger, default_handler):
-    handler = logbook.FingersCrossedHandler(default_handler,
-                                            logbook.WARNING)
+    handler = logbook.FingersCrossedHandler(default_handler, logbook.WARNING)
 
     # if no warning occurs, the infos are not logged
     with activation_strategy(handler):
         with capturing_stderr_context() as captured:
-            logger.info('some info')
-        assert captured.getvalue() == ''
-        assert (not handler.triggered)
+            logger.info("some info")
+        assert captured.getvalue() == ""
+        assert not handler.triggered
 
     # but if it does, all log messages are output
     with activation_strategy(handler):
         with capturing_stderr_context() as captured:
-            logger.info('some info')
-            logger.warning('something happened')
-            logger.info('something else happened')
+            logger.info("some info")
+            logger.warning("something happened")
+            logger.info("something else happened")
         logs = captured.getvalue()
-        assert 'some info' in logs
-        assert 'something happened' in logs
-        assert 'something else happened' in logs
+        assert "some info" in logs
+        assert "something happened" in logs
+        assert "something else happened" in logs
         assert handler.triggered
 
 
 def test_fingerscrossed_factory(activation_strategy, logger):
     handlers = []
 
     def handler_factory(record, fch):
         handler = logbook.TestHandler()
         handlers.append(handler)
         return handler
 
     def make_fch():
-        return logbook.FingersCrossedHandler(handler_factory,
-                                             logbook.WARNING)
+        return logbook.FingersCrossedHandler(handler_factory, logbook.WARNING)
 
     fch = make_fch()
     with activation_strategy(fch):
-        logger.info('some info')
+        logger.info("some info")
         assert len(handlers) == 0
-        logger.warning('a warning')
+        logger.warning("a warning")
         assert len(handlers) == 1
-        logger.error('an error')
+        logger.error("an error")
         assert len(handlers) == 1
         assert handlers[0].has_infos
         assert handlers[0].has_warnings
         assert handlers[0].has_errors
-        assert (not handlers[0].has_notices)
-        assert (not handlers[0].has_criticals)
-        assert (not handlers[0].has_debugs)
+        assert not handlers[0].has_notices
+        assert not handlers[0].has_criticals
+        assert not handlers[0].has_debugs
 
     fch = make_fch()
     with activation_strategy(fch):
-        logger.info('some info')
-        logger.warning('a warning')
+        logger.info("some info")
+        logger.warning("a warning")
         assert len(handlers) == 2
 
 
 def test_fingerscrossed_buffer_size(activation_strategy):
-    logger = logbook.Logger('Test')
+    logger = logbook.Logger("Test")
     test_handler = logbook.TestHandler()
     handler = logbook.FingersCrossedHandler(test_handler, buffer_size=3)
 
     with activation_strategy(handler):
-        logger.info('Never gonna give you up')
-        logger.warn('Aha!')
-        logger.warn('Moar!')
-        logger.error('Pure hate!')
-
-    assert test_handler.formatted_records == ['[WARNING] Test: Aha!',
-                                              '[WARNING] Test: Moar!',
-                                              '[ERROR] Test: Pure hate!']
+        logger.info("Never gonna give you up")
+        logger.warn("Aha!")
+        logger.warn("Moar!")
+        logger.error("Pure hate!")
+
+    assert test_handler.formatted_records == [
+        "[WARNING] Test: Aha!",
+        "[WARNING] Test: Moar!",
+        "[ERROR] Test: Pure hate!",
+    ]
```

### Comparing `Logbook-1.5.3/tests/test_flags.py` & `Logbook-1.6.0/tests/test_flags.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-import logbook
-
 import pytest
 
+import logbook
+
 from .utils import capturing_stderr_context
 
 
 def test_error_flag(logger):
     with capturing_stderr_context() as captured:
-        with logbook.Flags(errors='print'):
-            with logbook.Flags(errors='silent'):
-                logger.warn('Foo {42}', 'aha')
-        assert captured.getvalue() == ''
-
-        with logbook.Flags(errors='silent'):
-            with logbook.Flags(errors='print'):
-                logger.warn('Foo {42}', 'aha')
-        assert captured.getvalue() != ''
+        with logbook.Flags(errors="print"):
+            with logbook.Flags(errors="silent"):
+                logger.warn("Foo {42}", "aha")
+        assert captured.getvalue() == ""
+
+        with logbook.Flags(errors="silent"):
+            with logbook.Flags(errors="print"):
+                logger.warn("Foo {42}", "aha")
+        assert captured.getvalue() != ""
 
         with pytest.raises(Exception) as caught:
-            with logbook.Flags(errors='raise'):
-                logger.warn('Foo {42}', 'aha')
-        assert 'Could not format message with provided arguments' in str(
-            caught.value)
+            with logbook.Flags(errors="raise"):
+                logger.warn("Foo {42}", "aha")
+        assert "Could not format message with provided arguments" in str(caught.value)
 
 
 def test_disable_introspection(logger):
     with logbook.Flags(introspection=False):
         with logbook.TestHandler() as h:
-            logger.warn('Testing')
+            logger.warn("Testing")
             assert h.records[0].frame is None
             assert h.records[0].calling_frame is None
             assert h.records[0].module is None
```

### Comparing `Logbook-1.5.3/tests/test_groups.py` & `Logbook-1.6.0/tests/test_groups.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,91 +1,92 @@
 import logbook
 
 
 def test_groups(logger):
     def inject_extra(record):
-        record.extra['foo'] = 'bar'
+        record.extra["foo"] = "bar"
+
     group = logbook.LoggerGroup(processor=inject_extra)
     group.level = logbook.ERROR
     group.add_logger(logger)
     with logbook.TestHandler() as handler:
-        logger.warn('A warning')
-        logger.error('An error')
-    assert (not handler.has_warning('A warning'))
-    assert handler.has_error('An error')
-    assert handler.records[0].extra['foo'] == 'bar'
+        logger.warn("A warning")
+        logger.error("An error")
+    assert not handler.has_warning("A warning")
+    assert handler.has_error("An error")
+    assert handler.records[0].extra["foo"] == "bar"
 
 
 def test_group_disabled():
     group = logbook.LoggerGroup()
-    logger1 = logbook.Logger('testlogger1')
-    logger2 = logbook.Logger('testlogger2')
+    logger1 = logbook.Logger("testlogger1")
+    logger2 = logbook.Logger("testlogger2")
 
     group.add_logger(logger1)
     group.add_logger(logger2)
 
     # Test group disable
 
     group.disable()
 
     with logbook.TestHandler() as handler:
-        logger1.warn('Warning 1')
-        logger2.warn('Warning 2')
+        logger1.warn("Warning 1")
+        logger2.warn("Warning 2")
 
     assert not handler.has_warnings
 
     # Test group enable
 
     group.enable()
 
     with logbook.TestHandler() as handler:
-        logger1.warn('Warning 1')
-        logger2.warn('Warning 2')
+        logger1.warn("Warning 1")
+        logger2.warn("Warning 2")
 
-    assert handler.has_warning('Warning 1')
-    assert handler.has_warning('Warning 2')
+    assert handler.has_warning("Warning 1")
+    assert handler.has_warning("Warning 2")
 
     # Test group disabled, but logger explicitly enabled
 
     group.disable()
 
     logger1.enable()
 
     with logbook.TestHandler() as handler:
-        logger1.warn('Warning 1')
-        logger2.warn('Warning 2')
+        logger1.warn("Warning 1")
+        logger2.warn("Warning 2")
 
-    assert handler.has_warning('Warning 1')
-    assert not handler.has_warning('Warning 2')
+    assert handler.has_warning("Warning 1")
+    assert not handler.has_warning("Warning 2")
 
     # Logger 1 will be enabled by using force=True
 
     group.disable(force=True)
 
     with logbook.TestHandler() as handler:
-        logger1.warn('Warning 1')
-        logger2.warn('Warning 2')
+        logger1.warn("Warning 1")
+        logger2.warn("Warning 2")
 
-    assert not handler.has_warning('Warning 1')
-    assert not handler.has_warning('Warning 2')
+    assert not handler.has_warning("Warning 1")
+    assert not handler.has_warning("Warning 2")
 
     # Enabling without force means logger 1 will still be disabled.
 
     group.enable()
 
     with logbook.TestHandler() as handler:
-        logger1.warn('Warning 1')
-        logger2.warn('Warning 2')
+        logger1.warn("Warning 1")
+        logger2.warn("Warning 2")
 
-    assert not handler.has_warning('Warning 1')
-    assert handler.has_warning('Warning 2')
+    assert not handler.has_warning("Warning 1")
+    assert handler.has_warning("Warning 2")
 
     # Force logger 1 enabled.
 
     group.enable(force=True)
 
     with logbook.TestHandler() as handler:
-        logger1.warn('Warning 1')
-        logger2.warn('Warning 2')
+        logger1.warn("Warning 1")
+        logger2.warn("Warning 2")
 
-    assert handler.has_warning('Warning 1')
-    assert handler.has_warning('Warning 2')
+    assert handler.has_warning("Warning 1")
+    assert handler.has_warning("Warning 2")
```

### Comparing `Logbook-1.5.3/tests/test_handler_errors.py` & `Logbook-1.6.0/tests/test_handler_errors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,55 @@
 import re
 import sys
 
-import logbook
-
 import pytest
 
+import logbook
+
 from .utils import capturing_stderr_context
 
 __file_without_pyc__ = __file__
-if __file_without_pyc__.endswith('.pyc'):
+if __file_without_pyc__.endswith(".pyc"):
     __file_without_pyc__ = __file_without_pyc__[:-1]
 
 
 def test_handler_exception(activation_strategy, logger):
     class ErroringHandler(logbook.TestHandler):
-
         def emit(self, record):
-            raise RuntimeError('something bad happened')
+            raise RuntimeError("something bad happened")
 
     with capturing_stderr_context() as stderr:
         with activation_strategy(ErroringHandler()):
-            logger.warn('I warn you.')
-    assert 'something bad happened' in stderr.getvalue()
-    assert 'I warn you' not in stderr.getvalue()
+            logger.warn("I warn you.")
+    assert "something bad happened" in stderr.getvalue()
+    assert "I warn you" not in stderr.getvalue()
 
 
 def test_formatting_exception():
     def make_record():
-        return logbook.LogRecord('Test Logger', logbook.WARNING,
-                                 'Hello {foo:invalid}',
-                                 kwargs={'foo': 42},
-                                 frame=sys._getframe())
+        return logbook.LogRecord(
+            "Test Logger",
+            logbook.WARNING,
+            "Hello {foo:invalid}",
+            kwargs={"foo": 42},
+            frame=sys._getframe(),
+        )
+
     record = make_record()
     with pytest.raises(TypeError) as caught:
         record.message
 
     errormsg = str(caught.value)
     assert re.search(
-        'Could not format message with provided arguments: Invalid '
-        '(?:format specifier)|(?:conversion specification)|(?:format spec)',
-        errormsg, re.M | re.S)
+        "Could not format message with provided arguments: Invalid "
+        "(?:format specifier)|(?:conversion specification)|(?:format spec)",
+        errormsg,
+        re.M | re.S,
+    )
     assert "msg='Hello {foo:invalid}'" in errormsg
-    assert 'args=()' in errormsg
+    assert "args=()" in errormsg
     assert "kwargs={'foo': 42}" in errormsg
     assert re.search(
-        r'Happened in file .*%s, line \d+' % re.escape(__file_without_pyc__),
-        errormsg, re.M | re.S)
+        r"Happened in file .*%s, line \d+" % re.escape(__file_without_pyc__),
+        errormsg,
+        re.M | re.S,
+    )
```

### Comparing `Logbook-1.5.3/tests/test_handlers.py` & `Logbook-1.6.0/tests/test_handlers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,137 +1,138 @@
 import logbook
 
 from .utils import capturing_stderr_context, make_fake_mail_handler
 
 
 def test_custom_logger(activation_strategy, logger):
-    client_ip = '127.0.0.1'
+    client_ip = "127.0.0.1"
 
     class CustomLogger(logbook.Logger):
-
         def process_record(self, record):
-            record.extra['ip'] = client_ip
+            record.extra["ip"] = client_ip
 
-    custom_log = CustomLogger('awesome logger')
-    fmt = ('[{record.level_name}] {record.channel}: '
-           '{record.message} [{record.extra[ip]}]')
+    custom_log = CustomLogger("awesome logger")
+    fmt = (
+        "[{record.level_name}] {record.channel}: "
+        "{record.message} [{record.extra[ip]}]"
+    )
     handler = logbook.TestHandler(format_string=fmt)
     assert handler.format_string == fmt
 
     with activation_strategy(handler):
-        custom_log.warn('Too many sounds')
+        custom_log.warn("Too many sounds")
         logger.warn('"Music" playing')
 
     assert handler.formatted_records == [
-        '[WARNING] awesome logger: Too many sounds [127.0.0.1]',
-        '[WARNING] testlogger: "Music" playing []']
+        "[WARNING] awesome logger: Too many sounds [127.0.0.1]",
+        '[WARNING] testlogger: "Music" playing []',
+    ]
 
 
 def test_custom_handling(activation_strategy, logger):
     class MyTestHandler(logbook.TestHandler):
         def handle(self, record):
-            if record.extra.get('flag') != 'testing':
+            if record.extra.get("flag") != "testing":
                 return False
             return logbook.TestHandler.handle(self, record)
 
     # Check metaclass (== cls.__class__)
     assert logbook.Handler.__class__ == logbook.handlers._HandlerType
 
     class MyLogger(logbook.Logger):
         def process_record(self, record):
             logbook.Logger.process_record(self, record)
-            record.extra['flag'] = 'testing'
+            record.extra["flag"] = "testing"
 
     log = MyLogger()
     handler = MyTestHandler()
     with capturing_stderr_context() as captured:
         with activation_strategy(handler):
-            log.warn('From my logger')
-            logger.warn('From another logger')
-        assert handler.has_warning('From my logger')
-        assert 'From another logger' in captured.getvalue()
+            log.warn("From my logger")
+            logger.warn("From another logger")
+        assert handler.has_warning("From my logger")
+        assert "From another logger" in captured.getvalue()
 
 
 def test_nested_setups(activation_strategy):
     with capturing_stderr_context() as captured:
-        logger = logbook.Logger('App')
-        test_handler = logbook.TestHandler(level='WARNING')
+        logger = logbook.Logger("App")
+        test_handler = logbook.TestHandler(level="WARNING")
         mail_handler = make_fake_mail_handler(bubble=True)
 
-        handlers = logbook.NestedSetup([
-            logbook.NullHandler(),
-            test_handler,
-            mail_handler
-        ])
+        handlers = logbook.NestedSetup(
+            [logbook.NullHandler(), test_handler, mail_handler]
+        )
 
         with activation_strategy(handlers):
-            logger.warn('This is a warning')
-            logger.error('This is also a mail')
+            logger.warn("This is a warning")
+            logger.error("This is also a mail")
             try:
                 1 / 0
             except Exception:
                 logger.exception()
-        logger.warn('And here we go straight back to stderr')
+        logger.warn("And here we go straight back to stderr")
 
-        assert test_handler.has_warning('This is a warning')
-        assert test_handler.has_error('This is also a mail')
+        assert test_handler.has_warning("This is a warning")
+        assert test_handler.has_error("This is also a mail")
         assert len(mail_handler.mails) == 2
-        assert 'This is also a mail' in mail_handler.mails[0][2]
-        assert '1 / 0' in mail_handler.mails[1][2]
-        assert 'And here we go straight back to stderr' in captured.getvalue()
+        assert "This is also a mail" in mail_handler.mails[0][2]
+        assert "1 / 0" in mail_handler.mails[1][2]
+        assert "And here we go straight back to stderr" in captured.getvalue()
 
         with activation_strategy(handlers):
-            logger.warn('threadbound warning')
+            logger.warn("threadbound warning")
 
         handlers.push_application()
         try:
-            logger.warn('applicationbound warning')
+            logger.warn("applicationbound warning")
         finally:
             handlers.pop_application()
 
 
 def test_filtering(activation_strategy):
-    logger1 = logbook.Logger('Logger1')
-    logger2 = logbook.Logger('Logger2')
+    logger1 = logbook.Logger("Logger1")
+    logger2 = logbook.Logger("Logger2")
     handler = logbook.TestHandler()
     outer_handler = logbook.TestHandler()
 
     def only_1(record, handler):
         return record.dispatcher is logger1
+
     handler.filter = only_1
 
     with activation_strategy(outer_handler):
         with activation_strategy(handler):
-            logger1.warn('foo')
-            logger2.warn('bar')
+            logger1.warn("foo")
+            logger2.warn("bar")
 
-    assert handler.has_warning('foo', channel='Logger1')
-    assert (not handler.has_warning('bar', channel='Logger2'))
-    assert (not outer_handler.has_warning('foo', channel='Logger1'))
-    assert outer_handler.has_warning('bar', channel='Logger2')
+    assert handler.has_warning("foo", channel="Logger1")
+    assert not handler.has_warning("bar", channel="Logger2")
+    assert not outer_handler.has_warning("foo", channel="Logger1")
+    assert outer_handler.has_warning("bar", channel="Logger2")
 
 
 def test_different_context_pushing(activation_strategy):
     h1 = logbook.TestHandler(level=logbook.DEBUG)
     h2 = logbook.TestHandler(level=logbook.INFO)
     h3 = logbook.TestHandler(level=logbook.WARNING)
-    logger = logbook.Logger('Testing')
+    logger = logbook.Logger("Testing")
 
     with activation_strategy(h1):
         with activation_strategy(h2):
             with activation_strategy(h3):
-                logger.warn('Wuuu')
-                logger.info('still awesome')
-                logger.debug('puzzled')
-
-    assert h1.has_debug('puzzled')
-    assert h2.has_info('still awesome')
-    assert h3.has_warning('Wuuu')
+                logger.warn("Wuuu")
+                logger.info("still awesome")
+                logger.debug("puzzled")
+
+    assert h1.has_debug("puzzled")
+    assert h2.has_info("still awesome")
+    assert h3.has_warning("Wuuu")
     for handler in h1, h2, h3:
         assert len(handler.records) == 1
 
 
 def test_default_handlers(logger):
     with capturing_stderr_context() as stream:
-        logger.warn('Aha!')
+        logger.warn("Aha!")
         captured = stream.getvalue()
-    assert 'WARNING: testlogger: Aha!' in captured
+    assert "WARNING: testlogger: Aha!" in captured
```

### Comparing `Logbook-1.5.3/tests/test_log_record.py` & `Logbook-1.6.0/tests/test_log_record.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,42 +4,55 @@
 
 from .utils import capturing_stderr_context
 
 
 def test_exc_info_when_no_exceptions_exist(logger):
     with capturing_stderr_context() as captured:
         with logbook.StreamHandler(sys.stderr):
-            logger.debug('message', exc_info=True)
-    assert 'Traceback' not in captured.getvalue()
+            logger.debug("message", exc_info=True)
+    assert "Traceback" not in captured.getvalue()
 
 
 def test_exc_info_false():
     with logbook.handlers.TestHandler() as handler:
-        logbook.debug('message here', exc_info=False)
+        logbook.debug("message here", exc_info=False)
     [record] = handler.records
     assert not record.formatted_exception
 
 
+def test_exc_info_exception_instance(logger):
+    with logbook.handlers.TestHandler() as handler:
+        try:
+            raise ValueError("error here")
+        except Exception as e:
+            error = e
+        logger.exception(exc_info=error)
+    [record] = handler.records
+    assert isinstance(record.exc_info, tuple)
+    assert len(record.exc_info) == 3
+    assert "Traceback" in record.formatted_exception
+
+
 def test_extradict(active_handler, logger):
-    logger.warn('Test warning')
+    logger.warn("Test warning")
     record = active_handler.records[0]
-    record.extra['existing'] = 'foo'
-    assert record.extra['nonexisting'] == ''
-    assert record.extra['existing'] == 'foo'
+    record.extra["existing"] = "foo"
+    assert record.extra["nonexisting"] == ""
+    assert record.extra["existing"] == "foo"
 
 
 def test_calling_frame(active_handler, logger):
-    logger.warn('test')
+    logger.warn("test")
     assert active_handler.records[0].calling_frame == sys._getframe()
 
 
 def test_frame_correction(active_handler, logger):
     def inner():
-        logger.warn('test', frame_correction=+1)
+        logger.warn("test", frame_correction=+1)
 
     inner()
     assert active_handler.records[0].calling_frame == sys._getframe()
 
 
 def test_dispatcher(active_handler, logger):
-    logger.warn('Logbook is too awesome for stdlib')
+    logger.warn("Logbook is too awesome for stdlib")
     assert active_handler.records[0].dispatcher == logger
```

### Comparing `Logbook-1.5.3/tests/test_logger.py` & `Logbook-1.6.0/tests/test_logger.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-import logbook
 import pytest
 
+import logbook
+
 
 def test_level_properties(logger):
     assert logger.level == logbook.NOTSET
-    assert logger.level_name == 'NOTSET'
-    logger.level_name = 'WARNING'
+    assert logger.level_name == "NOTSET"
+    logger.level_name = "WARNING"
     assert logger.level == logbook.WARNING
     logger.level = logbook.ERROR
-    assert logger.level_name == 'ERROR'
+    assert logger.level_name == "ERROR"
 
 
 def test_reflected_properties(logger):
     group = logbook.LoggerGroup()
     group.add_logger(logger)
     assert logger.group == group
     group.level = logbook.ERROR
     assert logger.level == logbook.ERROR
-    assert logger.level_name == 'ERROR'
+    assert logger.level_name == "ERROR"
     group.level = logbook.WARNING
     assert logger.level == logbook.WARNING
-    assert logger.level_name == 'WARNING'
+    assert logger.level_name == "WARNING"
     logger.level = logbook.CRITICAL
     group.level = logbook.DEBUG
     assert logger.level == logbook.CRITICAL
-    assert logger.level_name == 'CRITICAL'
+    assert logger.level_name == "CRITICAL"
     group.remove_logger(logger)
     assert logger.group is None
 
 
 def test_disabled_property():
     class MyLogger(logbook.Logger):
         @property
```

### Comparing `Logbook-1.5.3/tests/test_logging_api.py` & `Logbook-1.6.0/tests/test_logging_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,93 +1,90 @@
 import pickle
 import sys
 
-import logbook
-from logbook.helpers import iteritems, xrange, u
-
 import pytest
 
+import logbook
+
 
 def test_basic_logging(active_handler, logger):
-    logger.warn('This is a warning.  Nice hah?')
+    logger.warn("This is a warning.  Nice hah?")
 
-    assert active_handler.has_warning('This is a warning.  Nice hah?')
+    assert active_handler.has_warning("This is a warning.  Nice hah?")
     assert active_handler.formatted_records == [
-        '[WARNING] testlogger: This is a warning.  Nice hah?']
+        "[WARNING] testlogger: This is a warning.  Nice hah?"
+    ]
 
 
 def test_exception_catching(active_handler, logger):
     assert not active_handler.has_error()
     try:
         1 / 0
     except Exception:
         logger.exception()
     try:
         1 / 0
     except Exception:
-        logger.exception('Awesome')
-    assert active_handler.has_error('Uncaught exception occurred')
-    assert active_handler.has_error('Awesome')
+        logger.exception("Awesome")
+    assert active_handler.has_error("Uncaught exception occurred")
+    assert active_handler.has_error("Awesome")
     assert active_handler.records[0].exc_info is not None
-    assert '1 / 0' in active_handler.records[0].formatted_exception
+    assert "1 / 0" in active_handler.records[0].formatted_exception
 
 
 def test_exception_catching_with_unicode():
-    """ See https://github.com/getlogbook/logbook/issues/104
-    """
+    """See https://github.com/getlogbook/logbook/issues/104"""
     try:
-        raise Exception(u('\u202a test \u202c'))
+        raise Exception("\u202a test \u202c")
     except:
-        r = logbook.LogRecord('channel', 'DEBUG', 'test',
-                              exc_info=sys.exc_info())
+        r = logbook.LogRecord("channel", "DEBUG", "test", exc_info=sys.exc_info())
     r.exception_message
 
 
-@pytest.mark.parametrize('as_tuple', [True, False])
+@pytest.mark.parametrize("as_tuple", [True, False])
 def test_exc_info(as_tuple, logger, active_handler):
     try:
         1 / 0
     except Exception:
         exc_info = sys.exc_info()
-        logger.info("Exception caught",
-                    exc_info=exc_info if as_tuple else True)
+        logger.info("Exception caught", exc_info=exc_info if as_tuple else True)
     assert active_handler.records[0].exc_info is not None
     assert active_handler.records[0].exc_info == exc_info
 
 
 def test_to_dict(logger, active_handler):
     try:
         1 / 0
     except Exception:
         logger.exception()
         record = active_handler.records[0]
 
     exported = record.to_dict()
     record.close()
     imported = logbook.LogRecord.from_dict(exported)
-    for key, value in iteritems(record.__dict__):
-        if key[0] == '_':
+    for key, value in record.__dict__.items():
+        if key[0] == "_":
             continue
         assert value == getattr(imported, key)
 
 
 def test_pickle(active_handler, logger):
     try:
         1 / 0
     except Exception:
         logger.exception()
         record = active_handler.records[0]
     record.pull_information()
     record.close()
 
-    for p in xrange(pickle.HIGHEST_PROTOCOL):
+    for p in range(pickle.HIGHEST_PROTOCOL):
         exported = pickle.dumps(record, p)
         imported = pickle.loads(exported)
-        for key, value in iteritems(record.__dict__):
-            if key[0] == '_':
+        for key, value in record.__dict__.items():
+            if key[0] == "_":
                 continue
             imported_value = getattr(imported, key)
             if isinstance(value, ZeroDivisionError):
                 # in Python 3.2, ZeroDivisionError(x) != ZeroDivisionError(x)
                 assert type(value) is type(imported_value)
                 assert value.args == imported_value.args
             else:
```

### Comparing `Logbook-1.5.3/tests/test_logging_times.py` & `Logbook-1.6.0/tests/test_logging_times.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,95 +1,100 @@
 from datetime import datetime, timedelta, tzinfo
 
-import logbook
-
 import pytest
 
-from .utils import get_total_delta_seconds
+import logbook
 
 
 def test_timedate_format(activation_strategy, logger):
     """
     tests the logbook.set_datetime_format() function
     """
-    FORMAT_STRING = '{record.time:%H:%M:%S.%f} {record.message}'
+    FORMAT_STRING = "{record.time:%H:%M:%S.%f} {record.message}"
     handler = logbook.TestHandler(format_string=FORMAT_STRING)
     with activation_strategy(handler):
-        logbook.set_datetime_format('utc')
+        logbook.set_datetime_format("utc")
         try:
-            logger.warn('This is a warning.')
+            logger.warn("This is a warning.")
             time_utc = handler.records[0].time
-            logbook.set_datetime_format('local')
-            logger.warn('This is a warning.')
+            logbook.set_datetime_format("local")
+            logger.warn("This is a warning.")
             time_local = handler.records[1].time
         finally:
             # put back the default time factory
-            logbook.set_datetime_format('utc')
+            logbook.set_datetime_format("utc")
 
     # get the expected difference between local and utc time
     t1 = datetime.now()
     t2 = datetime.utcnow()
 
-    tz_minutes_diff = get_total_delta_seconds(t1 - t2)/60.0
+    tz_minutes_diff = (t1 - t2).total_seconds() / 60.0
 
     if abs(tz_minutes_diff) < 1:
-        pytest.skip('Cannot test utc/localtime differences '
-                    'if they vary by less than one minute...')
+        pytest.skip(
+            "Cannot test utc/localtime differences "
+            "if they vary by less than one minute..."
+        )
 
     # get the difference between LogRecord local and utc times
-    logbook_minutes_diff = get_total_delta_seconds(time_local - time_utc)/60.0
+    logbook_minutes_diff = (time_local - time_utc).total_seconds() / 60.0
     assert abs(logbook_minutes_diff) > 1, (
-        'Localtime does not differ from UTC by more than 1 '
-        'minute (Local: %s, UTC: %s)' % (time_local, time_utc))
+        "Localtime does not differ from UTC by more than 1 "
+        "minute (Local: %s, UTC: %s)" % (time_local, time_utc)
+    )
 
     ratio = logbook_minutes_diff / tz_minutes_diff
 
     assert ratio > 0.99
     assert ratio < 1.01
 
 
 def test_tz_aware(activation_strategy, logger):
     """
     tests logbook.set_datetime_format() with a time zone aware time factory
     """
+
     class utc(tzinfo):
         def tzname(self, dt):
-            return 'UTC'
+            return "UTC"
+
         def utcoffset(self, dt):
             return timedelta(seconds=0)
+
         def dst(self, dt):
             return timedelta(seconds=0)
 
     utc = utc()
 
     def utc_tz():
         return datetime.now(tz=utc)
 
-    FORMAT_STRING = '{record.time:%H:%M:%S.%f%z} {record.message}'
+    FORMAT_STRING = "{record.time:%H:%M:%S.%f%z} {record.message}"
     handler = logbook.TestHandler(format_string=FORMAT_STRING)
     with activation_strategy(handler):
         logbook.set_datetime_format(utc_tz)
         try:
-            logger.warn('this is a warning.')
+            logger.warn("this is a warning.")
             record = handler.records[0]
         finally:
             # put back the default time factory
-            logbook.set_datetime_format('utc')
+            logbook.set_datetime_format("utc")
 
     assert record.time.tzinfo is not None
 
 
 def test_invalid_time_factory():
     """
     tests logbook.set_datetime_format() with an invalid time factory callable
     """
+
     def invalid_factory():
         return False
 
     with pytest.raises(ValueError) as e:
         try:
             logbook.set_datetime_format(invalid_factory)
         finally:
             # put back the default time factory
-            logbook.set_datetime_format('utc')
+            logbook.set_datetime_format("utc")
 
-    assert 'Invalid callable value' in str(e.value)
+    assert "Invalid callable value" in str(e.value)
```

### Comparing `Logbook-1.5.3/tests/test_mail_handler.py` & `Logbook-1.6.0/tests/test_mail_handler.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,234 +1,232 @@
 import base64
 import re
-import sys
+from unittest.mock import call, patch
 
 import logbook
-from logbook.helpers import u
 
 from .utils import capturing_stderr_context, make_fake_mail_handler
 
-try:
-    from unittest.mock import Mock, call, patch
-except ImportError:
-    from mock import Mock, call, patch
-
 __file_without_pyc__ = __file__
-if __file_without_pyc__.endswith('.pyc'):
+if __file_without_pyc__.endswith(".pyc"):
     __file_without_pyc__ = __file_without_pyc__[:-1]
 
 
 def test_mail_handler(activation_strategy, logger):
-    subject = u('\xf8nicode')
+    subject = "\xf8nicode"
     handler = make_fake_mail_handler(subject=subject)
     with capturing_stderr_context() as fallback:
         with activation_strategy(handler):
-            logger.warn('This is not mailed')
+            logger.warn("This is not mailed")
             try:
                 1 / 0
             except Exception:
-                logger.exception(u('Viva la Espa\xf1a'))
+                logger.exception("Viva la Espa\xf1a")
 
         if not handler.mails:
             # if sending the mail failed, the reason should be on stderr
             assert False, fallback.getvalue()
 
         assert len(handler.mails) == 1
         sender, receivers, mail = handler.mails[0]
-        mail = mail.replace('\r', '')
+        mail = mail.replace("\r", "")
         assert sender == handler.from_addr
-        assert '=?utf-8?q?=C3=B8nicode?=' in mail
-        header, data = mail.split('\n\n', 1)
-        if 'Content-Transfer-Encoding: base64' in header:
-            data = base64.b64decode(data).decode('utf-8')
-        assert re.search(r'Message type:\s+ERROR', data)
-        assert re.search(r'Location:.*%s' %
-                         re.escape(__file_without_pyc__), data)
-        assert re.search(r'Module:\s+%s' % __name__, data)
-        assert re.search(r'Function:\s+test_mail_handler', data)
-        body = u('Viva la Espa\xf1a')
-        if sys.version_info < (3, 0):
-            body = body.encode('utf-8')
+        assert "=?utf-8?q?=C3=B8nicode?=" in mail
+        header, data = mail.split("\n\n", 1)
+        if "Content-Transfer-Encoding: base64" in header:
+            data = base64.b64decode(data).decode("utf-8")
+        assert re.search(r"Message type:\s+ERROR", data)
+        assert re.search(r"Location:.*%s" % re.escape(__file_without_pyc__), data)
+        assert re.search(r"Module:\s+%s" % __name__, data)
+        assert re.search(r"Function:\s+test_mail_handler", data)
+        body = "Viva la Espa\xf1a"
         assert body in data
-        assert '\nTraceback (most' in data
-        assert '1 / 0' in data
-        assert 'This is not mailed' in fallback.getvalue()
+        assert "\nTraceback (most" in data
+        assert "1 / 0" in data
+        assert "This is not mailed" in fallback.getvalue()
 
 
 def test_mail_handler_batching(activation_strategy, logger):
     mail_handler = make_fake_mail_handler()
     handler = logbook.FingersCrossedHandler(mail_handler, reset=True)
     with activation_strategy(handler):
-        logger.warn('Testing')
-        logger.debug('Even more')
-        logger.error('And this triggers it')
-        logger.info('Aha')
-        logger.error('And this triggers it again!')
+        logger.warn("Testing")
+        logger.debug("Even more")
+        logger.error("And this triggers it")
+        logger.info("Aha")
+        logger.error("And this triggers it again!")
 
     assert len(mail_handler.mails) == 2
     mail = mail_handler.mails[0][2]
 
-    pieces = mail.split('Log records that led up to this one:')
+    pieces = mail.split("Log records that led up to this one:")
     assert len(pieces) == 2
     body, rest = pieces
-    rest = rest.replace('\r', '')
+    rest = rest.replace("\r", "")
 
-    assert re.search(r'Message type:\s+ERROR', body)
-    assert re.search(r'Module:\s+%s' % __name__, body)
-    assert re.search(r'Function:\s+test_mail_handler_batching', body)
+    assert re.search(r"Message type:\s+ERROR", body)
+    assert re.search(r"Module:\s+%s" % __name__, body)
+    assert re.search(r"Function:\s+test_mail_handler_batching", body)
 
-    related = rest.strip().split('\n\n')
+    related = rest.strip().split("\n\n")
     assert len(related) == 2
-    assert re.search(r'Message type:\s+WARNING', related[0])
-    assert re.search(r'Message type:\s+DEBUG', related[1])
+    assert re.search(r"Message type:\s+WARNING", related[0])
+    assert re.search(r"Message type:\s+DEBUG", related[1])
 
-    assert 'And this triggers it again' in mail_handler.mails[1][2]
+    assert "And this triggers it again" in mail_handler.mails[1][2]
 
 
 def test_group_handler_mail_combo(activation_strategy, logger):
     mail_handler = make_fake_mail_handler(level=logbook.DEBUG)
     handler = logbook.GroupHandler(mail_handler)
     with activation_strategy(handler):
-        logger.error('The other way round')
-        logger.warn('Testing')
-        logger.debug('Even more')
+        logger.error("The other way round")
+        logger.warn("Testing")
+        logger.debug("Even more")
         assert mail_handler.mails == []
 
     assert len(mail_handler.mails) == 1
     mail = mail_handler.mails[0][2]
 
-    pieces = mail.split('Other log records in the same group:')
+    pieces = mail.split("Other log records in the same group:")
     assert len(pieces) == 2
     body, rest = pieces
-    rest = rest.replace('\r', '')
+    rest = rest.replace("\r", "")
 
-    assert re.search(r'Message type:\s+ERROR', body)
-    assert re.search(r'Module:\s+' + __name__, body)
-    assert re.search(r'Function:\s+test_group_handler_mail_combo', body)
+    assert re.search(r"Message type:\s+ERROR", body)
+    assert re.search(r"Module:\s+" + __name__, body)
+    assert re.search(r"Function:\s+test_group_handler_mail_combo", body)
 
-    related = rest.strip().split('\n\n')
+    related = rest.strip().split("\n\n")
     assert len(related) == 2
-    assert re.search(r'Message type:\s+WARNING', related[0])
-    assert re.search(r'Message type:\s+DEBUG', related[1])
+    assert re.search(r"Message type:\s+WARNING", related[0])
+    assert re.search(r"Message type:\s+DEBUG", related[1])
 
 
 def test_mail_handler_arguments():
-    with patch('smtplib.SMTP', autospec=True) as mock_smtp:
-
+    with patch("smtplib.SMTP", autospec=True) as mock_smtp:
         # Test the mail handler with supported arguments before changes to
         # secure, credentials, and starttls
         mail_handler = logbook.MailHandler(
-            from_addr='from@example.com',
-            recipients='to@example.com',
-            server_addr=('server.example.com', 465),
-            credentials=('username', 'password'),
-            secure=('keyfile', 'certfile'))
+            from_addr="from@example.com",
+            recipients="to@example.com",
+            server_addr=("server.example.com", 465),
+            credentials=("username", "password"),
+            secure=("keyfile", "certfile"),
+        )
 
         mail_handler.get_connection()
 
-        assert mock_smtp.call_args == call('server.example.com', 465)
+        assert mock_smtp.call_args == call("server.example.com", 465)
         assert mock_smtp.method_calls[1] == call().starttls(
-            keyfile='keyfile', certfile='certfile')
-        assert mock_smtp.method_calls[3] == call().login('username', 'password')
+            keyfile="keyfile", certfile="certfile"
+        )
+        assert mock_smtp.method_calls[3] == call().login("username", "password")
 
         # Test secure=()
         mail_handler = logbook.MailHandler(
-            from_addr='from@example.com',
-            recipients='to@example.com',
-            server_addr=('server.example.com', 465),
-            credentials=('username', 'password'),
-            secure=())
+            from_addr="from@example.com",
+            recipients="to@example.com",
+            server_addr=("server.example.com", 465),
+            credentials=("username", "password"),
+            secure=(),
+        )
 
         mail_handler.get_connection()
 
-        assert mock_smtp.call_args == call('server.example.com', 465)
-        assert mock_smtp.method_calls[5] == call().starttls(
-            certfile=None, keyfile=None)
-        assert mock_smtp.method_calls[7] == call().login('username', 'password')
+        assert mock_smtp.call_args == call("server.example.com", 465)
+        assert mock_smtp.method_calls[5] == call().starttls(certfile=None, keyfile=None)
+        assert mock_smtp.method_calls[7] == call().login("username", "password")
 
         # Test implicit port with string server_addr, dictionary credentials,
         # dictionary secure.
         mail_handler = logbook.MailHandler(
-            from_addr='from@example.com',
-            recipients='to@example.com',
-            server_addr='server.example.com',
-            credentials={'user': 'username', 'password': 'password'},
-            secure={'certfile': 'certfile2', 'keyfile': 'keyfile2'})
+            from_addr="from@example.com",
+            recipients="to@example.com",
+            server_addr="server.example.com",
+            credentials={"user": "username", "password": "password"},
+            secure={"certfile": "certfile2", "keyfile": "keyfile2"},
+        )
 
         mail_handler.get_connection()
 
-        assert mock_smtp.call_args == call('server.example.com', 465)
+        assert mock_smtp.call_args == call("server.example.com", 465)
         assert mock_smtp.method_calls[9] == call().starttls(
-            certfile='certfile2', keyfile='keyfile2')
+            certfile="certfile2", keyfile="keyfile2"
+        )
         assert mock_smtp.method_calls[11] == call().login(
-            user='username', password='password')
+            user="username", password="password"
+        )
 
         # Test secure=True
         mail_handler = logbook.MailHandler(
-            from_addr='from@example.com',
-            recipients='to@example.com',
-            server_addr=('server.example.com', 465),
-            credentials=('username', 'password'),
-            secure=True)
+            from_addr="from@example.com",
+            recipients="to@example.com",
+            server_addr=("server.example.com", 465),
+            credentials=("username", "password"),
+            secure=True,
+        )
 
         mail_handler.get_connection()
 
-        assert mock_smtp.call_args == call('server.example.com', 465)
+        assert mock_smtp.call_args == call("server.example.com", 465)
         assert mock_smtp.method_calls[13] == call().starttls(
-            certfile=None, keyfile=None)
-        assert mock_smtp.method_calls[15] == call().login('username', 'password')
+            certfile=None, keyfile=None
+        )
+        assert mock_smtp.method_calls[15] == call().login("username", "password")
         assert len(mock_smtp.method_calls) == 16
 
         # Test secure=False
         mail_handler = logbook.MailHandler(
-            from_addr='from@example.com',
-            recipients='to@example.com',
-            server_addr=('server.example.com', 465),
-            credentials=('username', 'password'),
-            secure=False)
+            from_addr="from@example.com",
+            recipients="to@example.com",
+            server_addr=("server.example.com", 465),
+            credentials=("username", "password"),
+            secure=False,
+        )
 
         mail_handler.get_connection()
 
         # starttls not called because we check len of method_calls before and
         # after this test.
-        assert mock_smtp.call_args == call('server.example.com', 465)
-        assert mock_smtp.method_calls[16] == call().login('username', 'password')
+        assert mock_smtp.call_args == call("server.example.com", 465)
+        assert mock_smtp.method_calls[16] == call().login("username", "password")
         assert len(mock_smtp.method_calls) == 17
 
-    with patch('smtplib.SMTP_SSL', autospec=True) as mock_smtp_ssl:
+    with patch("smtplib.SMTP_SSL", autospec=True) as mock_smtp_ssl:
         # Test starttls=False
         mail_handler = logbook.MailHandler(
-            from_addr='from@example.com',
-            recipients='to@example.com',
-            server_addr='server.example.com',
-            credentials={'user': 'username', 'password': 'password'},
-            secure={'certfile': 'certfile', 'keyfile': 'keyfile'},
-            starttls=False)
+            from_addr="from@example.com",
+            recipients="to@example.com",
+            server_addr="server.example.com",
+            credentials={"user": "username", "password": "password"},
+            secure={"certfile": "certfile", "keyfile": "keyfile"},
+            starttls=False,
+        )
 
         mail_handler.get_connection()
 
         assert mock_smtp_ssl.call_args == call(
-            'server.example.com', 465, keyfile='keyfile', certfile='certfile')
+            "server.example.com", 465, keyfile="keyfile", certfile="certfile"
+        )
         assert mock_smtp_ssl.method_calls[0] == call().login(
-            user='username', password='password')
+            user="username", password="password"
+        )
 
         # Test starttls=False with secure=True
         mail_handler = logbook.MailHandler(
-            from_addr='from@example.com',
-            recipients='to@example.com',
-            server_addr='server.example.com',
-            credentials={'user': 'username', 'password': 'password'},
+            from_addr="from@example.com",
+            recipients="to@example.com",
+            server_addr="server.example.com",
+            credentials={"user": "username", "password": "password"},
             secure=True,
-            starttls=False)
+            starttls=False,
+        )
 
         mail_handler.get_connection()
 
         assert mock_smtp_ssl.call_args == call(
-            'server.example.com', 465, keyfile=None, certfile=None)
+            "server.example.com", 465, keyfile=None, certfile=None
+        )
         assert mock_smtp_ssl.method_calls[1] == call().login(
-            user='username', password='password')
-
-
-
-
-
-
+            user="username", password="password"
+        )
```

### Comparing `Logbook-1.5.3/tests/test_more.py` & `Logbook-1.6.0/tests/test_more.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,106 +1,111 @@
 import sys
-
-import logbook
-from logbook.helpers import StringIO
+from io import StringIO
 
 import pytest
 
+import logbook
+
 from .utils import capturing_stderr_context, missing, require_module
 
 
-@require_module('jinja2')
+@require_module("jinja2")
 def test_jinja_formatter(logger):
     from logbook.more import JinjaFormatter
-    fmter = JinjaFormatter('{{ record.channel }}/{{ record.level_name }}')
+
+    fmter = JinjaFormatter("{{ record.channel }}/{{ record.level_name }}")
     handler = logbook.TestHandler()
     handler.formatter = fmter
     with handler:
-        logger.info('info')
-    assert 'testlogger/INFO' in handler.formatted_records
+        logger.info("info")
+    assert "testlogger/INFO" in handler.formatted_records
 
 
-@missing('jinja2')
+@missing("jinja2")
 def test_missing_jinja2():
     from logbook.more import JinjaFormatter
+
     # check the RuntimeError is raised
     with pytest.raises(RuntimeError):
-        JinjaFormatter('dummy')
+        JinjaFormatter("dummy")
 
 
 def test_colorizing_support(logger):
     from logbook.more import ColorizedStderrHandler
 
     class TestColorizingHandler(ColorizedStderrHandler):
         def __init__(self, *args, **kwargs):
-            super(TestColorizingHandler, self).__init__(*args, **kwargs)
+            super().__init__(*args, **kwargs)
             self._obj_stream = StringIO()
 
         @property
         def stream(self):
             return self._obj_stream
 
-    with TestColorizingHandler(format_string='{record.message}') as handler:
+    with TestColorizingHandler(format_string="{record.message}") as handler:
         handler.force_color()
-        logger.error('An error')
-        logger.warn('A warning')
-        logger.debug('A debug message')
-        lines = handler.stream.getvalue().rstrip('\n').splitlines()
+        logger.error("An error")
+        logger.warn("A warning")
+        logger.debug("A debug message")
+        lines = handler.stream.getvalue().rstrip("\n").splitlines()
         assert lines == [
-            '\x1b[31;01mAn error\x1b[39;49;00m',
-            '\x1b[33;01mA warning\x1b[39;49;00m',
-            '\x1b[37mA debug message\x1b[39;49;00m']
+            "\x1b[31;01mAn error\x1b[39;49;00m",
+            "\x1b[33;01mA warning\x1b[39;49;00m",
+            "\x1b[37mA debug message\x1b[39;49;00m",
+        ]
 
-    with TestColorizingHandler(format_string='{record.message}') as handler:
+    with TestColorizingHandler(format_string="{record.message}") as handler:
         handler.forbid_color()
-        logger.error('An error')
-        logger.warn('A warning')
-        logger.debug('A debug message')
-        lines = handler.stream.getvalue().rstrip('\n').splitlines()
-        assert lines == ['An error', 'A warning', 'A debug message']
-
+        logger.error("An error")
+        logger.warn("A warning")
+        logger.debug("A debug message")
+        lines = handler.stream.getvalue().rstrip("\n").splitlines()
+        assert lines == ["An error", "A warning", "A debug message"]
 
 
 def test_tagged(default_handler):
-    from logbook.more import TaggingLogger, TaggingHandler
+    from logbook.more import TaggingHandler, TaggingLogger
+
     stream = StringIO()
     second_handler = logbook.StreamHandler(stream)
 
-    logger = TaggingLogger('name', ['cmd'])
-    handler = TaggingHandler(dict(
-        info=default_handler,
-        cmd=second_handler,
-        both=[default_handler, second_handler],
-    ))
+    logger = TaggingLogger("name", ["cmd"])
+    handler = TaggingHandler(
+        dict(
+            info=default_handler,
+            cmd=second_handler,
+            both=[default_handler, second_handler],
+        )
+    )
     handler.bubble = False
 
     with handler:
         with capturing_stderr_context() as captured:
-            logger.log('info', 'info message')
-            logger.log('both', 'all message')
-            logger.cmd('cmd message')
+            logger.log("info", "info message")
+            logger.log("both", "all message")
+            logger.cmd("cmd message")
 
     stderr = captured.getvalue()
 
-    assert 'info message' in stderr
-    assert 'all message' in stderr
-    assert 'cmd message' not in stderr
+    assert "info message" in stderr
+    assert "all message" in stderr
+    assert "cmd message" not in stderr
 
     stringio = stream.getvalue()
 
-    assert 'info message' not in stringio
-    assert 'all message' in stringio
-    assert 'cmd message' in stringio
+    assert "info message" not in stringio
+    assert "all message" in stringio
+    assert "cmd message" in stringio
 
 
 def test_tagging_logger(default_handler):
     from logbook import StderrHandler
     from logbook.more import TaggingLogger
 
-    logger = TaggingLogger('tagged', ['a', 'b'])
+    logger = TaggingLogger("tagged", ["a", "b"])
     handler = StderrHandler(format_string="{record.msg}|{record.extra[tags]}")
 
     with handler:
         with capturing_stderr_context() as captured:
             logger.a("a")
             logger.b("b")
 
@@ -110,67 +115,80 @@
     assert "a|['b']" not in stderr
     assert "b|['b']" in stderr
     assert "b|['a']" not in stderr
 
 
 def test_external_application_handler(tmpdir, logger):
     from logbook.more import ExternalApplicationHandler as Handler
-    fn = tmpdir.join('tempfile')
-    handler = Handler([sys.executable, '-c', r'''if 1:
-    f = open(%(tempfile)s, 'w')
+
+    fn = tmpdir.join("tempfile")
+    handler = Handler(
+        [
+            sys.executable,
+            "-c",
+            r"""if 1:
+    f = open({tempfile}, 'w')
     try:
-        f.write('{record.message}\n')
+        f.write('{{record.message}}\n')
     finally:
         f.close()
-    ''' % {'tempfile': repr(str(fn))}])
+    """.format(
+                tempfile=repr(str(fn))
+            ),
+        ]
+    )
     with handler:
-        logger.error('this is a really bad idea')
+        logger.error("this is a really bad idea")
     with fn.open() as rf:
         contents = rf.read().strip()
-    assert contents == 'this is a really bad idea'
+    assert contents == "this is a really bad idea"
 
 
 def test_exception_handler(logger):
     from logbook.more import ExceptionHandler
 
     with ExceptionHandler(ValueError):
         with pytest.raises(ValueError) as caught:
-            logger.info('here i am')
-    assert 'INFO: testlogger: here i am' in caught.value.args[0]
+            logger.info("here i am")
+    assert "INFO: testlogger: here i am" in caught.value.args[0]
 
 
 def test_exception_handler_specific_level(logger):
     from logbook.more import ExceptionHandler
+
     with logbook.TestHandler() as test_handler:
         with pytest.raises(ValueError) as caught:
-            with ExceptionHandler(ValueError, level='WARNING'):
-                logger.info('this is irrelevant')
-                logger.warn('here i am')
-        assert 'WARNING: testlogger: here i am' in caught.value.args[0]
-    assert 'this is irrelevant' in test_handler.records[0].message
+            with ExceptionHandler(ValueError, level="WARNING"):
+                logger.info("this is irrelevant")
+                logger.warn("here i am")
+        assert "WARNING: testlogger: here i am" in caught.value.args[0]
+    assert "this is irrelevant" in test_handler.records[0].message
 
 
 def test_dedup_handler(logger):
     from logbook.more import DedupHandler
+
     with logbook.TestHandler() as test_handler:
         with DedupHandler():
-            logger.info('foo')
-            logger.info('bar')
-            logger.info('foo')
+            logger.info("foo")
+            logger.info("bar")
+            logger.info("foo")
     assert 2 == len(test_handler.records)
-    assert 'message repeated 2 times: foo' in test_handler.records[0].message
-    assert 'message repeated 1 times: bar' in test_handler.records[1].message
-
+    assert "message repeated 2 times: foo" in test_handler.records[0].message
+    assert "message repeated 1 times: bar" in test_handler.records[1].message
 
-class TestRiemannHandler(object):
 
+class TestRiemannHandler:
     @require_module("riemann_client")
     def test_happy_path(self, logger):
         from logbook.more import RiemannHandler
-        riemann_handler = RiemannHandler("127.0.0.1", 5555, message_type="test", level=logbook.INFO)
+
+        riemann_handler = RiemannHandler(
+            "127.0.0.1", 5555, message_type="test", level=logbook.INFO
+        )
         null_handler = logbook.NullHandler()
         with null_handler.applicationbound():
             with riemann_handler:
                 logger.error("Something bad has happened")
                 try:
                     raise RuntimeError("For example, a RuntimeError")
                 except Exception as ex:
@@ -185,25 +203,29 @@
         assert exc_event["description"] == "For example, a RuntimeError"
         info_event = q[2]
         assert info_event["state"] == "ok"
 
     @require_module("riemann_client")
     def test_incorrect_type(self):
         from logbook.more import RiemannHandler
+
         with pytest.raises(RuntimeError):
             RiemannHandler("127.0.0.1", 5555, message_type="fancy_type")
 
     @require_module("riemann_client")
     def test_flush(self, logger):
         from logbook.more import RiemannHandler
-        riemann_handler = RiemannHandler("127.0.0.1",
-                                         5555,
-                                         message_type="test",
-                                         flush_threshold=2,
-                                         level=logbook.INFO)
+
+        riemann_handler = RiemannHandler(
+            "127.0.0.1",
+            5555,
+            message_type="test",
+            flush_threshold=2,
+            level=logbook.INFO,
+        )
         null_handler = logbook.NullHandler()
         with null_handler.applicationbound():
             with riemann_handler:
                 logger.info("Msg #1")
                 logger.info("Msg #2")
                 logger.info("Msg #3")
```

### Comparing `Logbook-1.5.3/tests/test_nteventlog_handler.py` & `Logbook-1.6.0/tests/test_nteventlog_handler.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,60 @@
 import os
 
-import logbook
 import pytest
 
+import logbook
+
 from .utils import require_module
 
 
-@require_module('win32con')
-@require_module('win32evtlog')
-@require_module('win32evtlogutil')
-@pytest.mark.skipif(os.environ.get('ENABLE_LOGBOOK_NTEVENTLOG_TESTS') is None,
-                    reason="Don't clutter NT Event Log unless enabled.")
+@require_module("win32con")
+@require_module("win32evtlog")
+@require_module("win32evtlogutil")
+@pytest.mark.skipif(
+    os.environ.get("ENABLE_LOGBOOK_NTEVENTLOG_TESTS") is None,
+    reason="Don't clutter NT Event Log unless enabled.",
+)
 def test_nteventlog_handler():
     from win32con import (
-        EVENTLOG_ERROR_TYPE, EVENTLOG_INFORMATION_TYPE, EVENTLOG_WARNING_TYPE)
+        EVENTLOG_ERROR_TYPE,
+        EVENTLOG_INFORMATION_TYPE,
+        EVENTLOG_WARNING_TYPE,
+    )
     from win32evtlog import (
-        EVENTLOG_BACKWARDS_READ, EVENTLOG_SEQUENTIAL_READ, OpenEventLog,
-        ReadEventLog)
+        EVENTLOG_BACKWARDS_READ,
+        EVENTLOG_SEQUENTIAL_READ,
+        OpenEventLog,
+        ReadEventLog,
+    )
     from win32evtlogutil import SafeFormatMessage
 
-    logger = logbook.Logger('Test Logger')
+    logger = logbook.Logger("Test Logger")
 
-    with logbook.NTEventLogHandler('Logbook Test Suite'):
-        logger.info('The info log message.')
-        logger.warning('The warning log message.')
-        logger.error('The error log message.')
+    with logbook.NTEventLogHandler("Logbook Test Suite"):
+        logger.info("The info log message.")
+        logger.warning("The warning log message.")
+        logger.error("The error log message.")
 
     def iter_event_log(handle, flags, offset):
         while True:
             events = ReadEventLog(handle, flags, offset)
-            for event in events:
-                yield event
+            yield from events
             if not events:
                 break
 
-    handle = OpenEventLog(None, 'Application')
+    handle = OpenEventLog(None, "Application")
     flags = EVENTLOG_BACKWARDS_READ | EVENTLOG_SEQUENTIAL_READ
 
     for event in iter_event_log(handle, flags, 0):
         source = str(event.SourceName)
-        if source == 'Logbook Test Suite':
-            message = SafeFormatMessage(event, 'Application')
-            if 'Message Level: INFO' in message:
-                assert 'The info log message' in message
+        if source == "Logbook Test Suite":
+            message = SafeFormatMessage(event, "Application")
+            if "Message Level: INFO" in message:
+                assert "The info log message" in message
                 assert event.EventType == EVENTLOG_INFORMATION_TYPE
-            if 'Message Level: WARNING' in message:
-                assert 'The warning log message' in message
+            if "Message Level: WARNING" in message:
+                assert "The warning log message" in message
                 assert event.EventType == EVENTLOG_WARNING_TYPE
-            if 'Message Level: ERROR' in message:
-                assert 'The error log message' in message
+            if "Message Level: ERROR" in message:
+                assert "The error log message" in message
                 assert event.EventType == EVENTLOG_ERROR_TYPE
```

### Comparing `Logbook-1.5.3/tests/test_null_handler.py` & `Logbook-1.6.0/tests/test_null_handler.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,39 +2,41 @@
 
 from .utils import capturing_stderr_context
 
 
 def test_null_handler(activation_strategy, logger):
     with capturing_stderr_context() as captured:
         with activation_strategy(logbook.NullHandler()):
-            with activation_strategy(logbook.TestHandler(level='ERROR')) as handler:
-                logger.error('An error')
-                logger.warn('A warning')
-        assert captured.getvalue() == ''
-        assert (not handler.has_warning('A warning'))
-        assert handler.has_error('An error')
+            with activation_strategy(logbook.TestHandler(level="ERROR")) as handler:
+                logger.error("An error")
+                logger.warn("A warning")
+        assert captured.getvalue() == ""
+        assert not handler.has_warning("A warning")
+        assert handler.has_error("An error")
 
 
 def test_blackhole_setting(activation_strategy):
     null_handler = logbook.NullHandler()
     heavy_init = logbook.LogRecord.heavy_init
     with activation_strategy(null_handler):
+
         def new_heavy_init(self):
-            raise RuntimeError('should not be triggered')
+            raise RuntimeError("should not be triggered")
+
         logbook.LogRecord.heavy_init = new_heavy_init
         try:
             with activation_strategy(null_handler):
-                logbook.warn('Awesome')
+                logbook.warn("Awesome")
         finally:
             logbook.LogRecord.heavy_init = heavy_init
 
     null_handler.bubble = True
     with capturing_stderr_context() as captured:
-        logbook.warning('Not a blockhole')
-        assert captured.getvalue() != ''
+        logbook.warning("Not a blockhole")
+        assert captured.getvalue() != ""
 
 
 def test_null_handler_filtering(activation_strategy):
     logger1 = logbook.Logger("1")
     logger2 = logbook.Logger("2")
     outer = logbook.TestHandler()
     inner = logbook.NullHandler()
@@ -42,9 +44,9 @@
     inner.filter = lambda record, handler: record.dispatcher is logger1
 
     with activation_strategy(outer):
         with activation_strategy(inner):
             logger1.warn("1")
             logger2.warn("2")
 
-    assert outer.has_warning('2', channel='2')
-    assert (not outer.has_warning('1', channel='1'))
+    assert outer.has_warning("2", channel="2")
+    assert not outer.has_warning("1", channel="1")
```

### Comparing `Logbook-1.5.3/tests/test_processors.py` & `Logbook-1.6.0/tests/test_processors.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,99 +3,105 @@
 import logbook
 
 from .utils import make_fake_mail_handler
 
 
 def test_handler_filter_after_processor(activation_strategy, logger):
     handler = make_fake_mail_handler(
-        format_string=dedent('''
+        format_string=dedent(
+            """
             Subject: Application Error for {record.extra[path]} [{record.extra[method]}]
 
             Message type:       {record.level_name}
             Location:           {record.filename}:{record.lineno}
             Module:             {record.module}
             Function:           {record.func_name}
             Time:               {record.time:%Y-%m-%d %H:%M:%S}
             Remote IP:          {record.extra[ip]}
             Request:            {record.extra[path]} [{record.extra[method]}]
 
             Message:
 
             {record.message}
-            ''').lstrip(),
-        filter=lambda r, h: 'ip' in r.extra,
-        bubble=False)
-
-    class Request(object):
-        remote_addr = '127.0.0.1'
-        method = 'GET'
-        path = '/index.html'
+            """
+        ).lstrip(),
+        filter=lambda r, h: "ip" in r.extra,
+        bubble=False,
+    )
+
+    class Request:
+        remote_addr = "127.0.0.1"
+        method = "GET"
+        path = "/index.html"
 
     def handle_request(request):
         def inject_extra(record):
-            record.extra['ip'] = request.remote_addr
-            record.extra['method'] = request.method
-            record.extra['path'] = request.path
+            record.extra["ip"] = request.remote_addr
+            record.extra["method"] = request.method
+            record.extra["path"] = request.path
 
         processor = logbook.Processor(inject_extra)
         with activation_strategy(processor):
             handler.push_thread()
             try:
                 try:
                     1 / 0
                 except Exception:
-                    logger.exception('Exception happened during request')
+                    logger.exception("Exception happened during request")
             finally:
                 handler.pop_thread()
 
     handle_request(Request())
     assert len(handler.mails) == 1
     mail = handler.mails[0][2]
-    assert 'Subject: Application Error for /index.html [GET]' in mail
-    assert '1 / 0' in mail
+    assert "Subject: Application Error for /index.html [GET]" in mail
+    assert "1 / 0" in mail
 
 
 def test_handler_processors(activation_strategy, logger):
     handler = make_fake_mail_handler(
-        format_string=dedent('''
+        format_string=dedent(
+            """
             Subject: Application Error for {record.extra[path]} [{record.extra[method]}]
 
             Message type:       {record.level_name}
             Location:           {record.filename}:{record.lineno}
             Module:             {record.module}
             Function:           {record.func_name}
             Time:               {record.time:%Y-%m-%d %H:%M:%S}
             Remote IP:          {record.extra[ip]}
             Request:            {record.extra[path]} [{record.extra[method]}]
 
             Message:
 
             {record.message}
-            ''').lstrip())
-
-    class Request(object):
-        remote_addr = '127.0.0.1'
-        method = 'GET'
-        path = '/index.html'
+            """
+        ).lstrip()
+    )
+
+    class Request:
+        remote_addr = "127.0.0.1"
+        method = "GET"
+        path = "/index.html"
 
     def handle_request(request):
         def inject_extra(record):
-            record.extra['ip'] = request.remote_addr
-            record.extra['method'] = request.method
-            record.extra['path'] = request.path
+            record.extra["ip"] = request.remote_addr
+            record.extra["method"] = request.method
+            record.extra["path"] = request.path
 
         processor = logbook.Processor(inject_extra)
         with activation_strategy(processor):
             handler.push_thread()
             try:
                 try:
                     1 / 0
                 except Exception:
-                    logger.exception('Exception happened during request')
+                    logger.exception("Exception happened during request")
             finally:
                 handler.pop_thread()
 
     handle_request(Request())
     assert len(handler.mails) == 1
     mail = handler.mails[0][2]
-    assert 'Subject: Application Error for /index.html [GET]' in mail
-    assert '1 / 0' in mail
+    assert "Subject: Application Error for /index.html [GET]" in mail
+    assert "1 / 0" in mail
```

### Comparing `Logbook-1.5.3/tests/test_queues.py` & `Logbook-1.6.0/tests/test_queues.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,235 +1,252 @@
-# -*- coding: utf-8 -*-
 import os
 import socket
 import time
 
-from .utils import require_module, missing, LETTERS
+import pytest
 
 import logbook
-from logbook.helpers import u
 
-import pytest
+from .utils import LETTERS, missing, require_module
+
+REDIS_HOST = os.environ.get("REDIS_HOST", "localhost")
+REDIS_PORT = int(os.environ.get("REDIS_PORT", "6379"))
 
 
-@require_module('zmq')
+@require_module("zmq")
 def test_zeromq_handler(logger, handlers, subscriber):
     tests = [
-        u('Logging something'),
-        u('Something with umlauts äöü'),
-        u('Something else for good measure'),
+        "Logging something",
+        "Something with umlauts äöü",
+        "Something else for good measure",
     ]
     for test in tests:
         for handler in handlers:
             with handler:
                 logger.warn(test)
                 record = subscriber.recv()
                 assert record.message == test
                 assert record.channel == logger.name
 
 
-@require_module('zmq')
+@require_module("zmq")
 def test_zeromq_background_thread(logger, handlers, subscriber):
     test_handler = logbook.TestHandler()
     controller = subscriber.dispatch_in_background(test_handler)
 
     for handler in handlers:
         with handler:
-            logger.warn('This is a warning')
-            logger.error('This is an error')
+            logger.warn("This is a warning")
+            logger.error("This is an error")
 
     # stop the controller.  This will also stop the loop and join the
     # background process.  Before that we give it a fraction of a second
     # to get all results
     time.sleep(0.5)
     controller.stop()
 
-    assert test_handler.has_warning('This is a warning')
-    assert test_handler.has_error('This is an error')
+    assert test_handler.has_warning("This is a warning")
+    assert test_handler.has_error("This is an error")
 
 
-@missing('zmq')
+@missing("zmq")
 def test_missing_zeromq():
     from logbook.queues import ZeroMQHandler, ZeroMQSubscriber
+
     with pytest.raises(RuntimeError):
-        ZeroMQHandler('tcp://127.0.0.1:42000')
+        ZeroMQHandler("tcp://127.0.0.1:42000")
     with pytest.raises(RuntimeError):
-        ZeroMQSubscriber('tcp://127.0.0.1:42000')
+        ZeroMQSubscriber("tcp://127.0.0.1:42000")
 
 
-class MultiProcessingHandlerSendBack(object):
+class MultiProcessingHandlerSendBack:
     def __init__(self, queue):
         self.queue = queue
 
     def __call__(self):
         from logbook.queues import MultiProcessingHandler
+
         handler = MultiProcessingHandler(self.queue)
         handler.push_thread()
         try:
-            logbook.warn('Hello World')
+            logbook.warn("Hello World")
         finally:
             handler.pop_thread()
 
 
-@require_module('multiprocessing')
+@require_module("multiprocessing")
 def test_multi_processing_handler():
-    if os.getenv('APPVEYOR') == 'True':
-        pytest.skip('Test hangs on AppVeyor CI')
+    if os.getenv("APPVEYOR") == "True":
+        pytest.skip("Test hangs on AppVeyor CI")
     from multiprocessing import Process, Queue
+
     from logbook.queues import MultiProcessingSubscriber
+
     queue = Queue(-1)
     test_handler = logbook.TestHandler()
     subscriber = MultiProcessingSubscriber(queue)
 
     p = Process(target=MultiProcessingHandlerSendBack(queue))
     p.start()
     p.join()
 
     with test_handler:
         subscriber.dispatch_once()
-        assert test_handler.has_warning('Hello World')
+        assert test_handler.has_warning("Hello World")
 
 
 class BatchTestHandler(logbook.TestHandler):
     def __init__(self, *args, **kwargs):
-        super(BatchTestHandler, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self.batches = []
 
     def emit(self, record):
-        super(BatchTestHandler, self).emit(record)
+        super().emit(record)
         self.batches.append([record])
 
     def emit_batch(self, records, reason):
         for record in records:
-            super(BatchTestHandler, self).emit(record)
+            super().emit(record)
         self.batches.append(records)
 
 
 def test_threaded_wrapper_handler(logger):
     from logbook.queues import ThreadedWrapperHandler
+
     test_handler = BatchTestHandler()
     with ThreadedWrapperHandler(test_handler) as handler:
-        logger.warn('Just testing')
-        logger.error('More testing')
+        logger.warn("Just testing")
+        logger.error("More testing")
 
     # give it some time to sync up
     handler.close()
 
-    assert (not handler.controller.running)
+    assert not handler.controller.running
     assert len(test_handler.records) == 2
     assert len(test_handler.batches) == 2
-    assert all((len(records) == 1 for records in test_handler.batches))
-    assert test_handler.has_warning('Just testing')
-    assert test_handler.has_error('More testing')
+    assert all(len(records) == 1 for records in test_handler.batches)
+    assert test_handler.has_warning("Just testing")
+    assert test_handler.has_error("More testing")
 
 
 def test_threaded_wrapper_handler_emit():
     from logbook.queues import ThreadedWrapperHandler
+
     test_handler = BatchTestHandler()
     with ThreadedWrapperHandler(test_handler) as handler:
-        lr = logbook.LogRecord('Test Logger', logbook.WARNING, 'Just testing')
+        lr = logbook.LogRecord("Test Logger", logbook.WARNING, "Just testing")
         test_handler.emit(lr)
-        lr = logbook.LogRecord('Test Logger', logbook.ERROR, 'More testing')
+        lr = logbook.LogRecord("Test Logger", logbook.ERROR, "More testing")
         test_handler.emit(lr)
 
     # give it some time to sync up
     handler.close()
 
-    assert (not handler.controller.running)
+    assert not handler.controller.running
     assert len(test_handler.records) == 2
     assert len(test_handler.batches) == 2
-    assert all((len(records) == 1 for records in test_handler.batches))
-    assert test_handler.has_warning('Just testing')
-    assert test_handler.has_error('More testing')
+    assert all(len(records) == 1 for records in test_handler.batches)
+    assert test_handler.has_warning("Just testing")
+    assert test_handler.has_error("More testing")
 
 
 def test_threaded_wrapper_handler_emit_batched():
     from logbook.queues import ThreadedWrapperHandler
+
     test_handler = BatchTestHandler()
     with ThreadedWrapperHandler(test_handler) as handler:
-        test_handler.emit_batch([
-            logbook.LogRecord('Test Logger', logbook.WARNING, 'Just testing'),
-            logbook.LogRecord('Test Logger', logbook.ERROR, 'More testing'),
-        ], 'group')
+        test_handler.emit_batch(
+            [
+                logbook.LogRecord("Test Logger", logbook.WARNING, "Just testing"),
+                logbook.LogRecord("Test Logger", logbook.ERROR, "More testing"),
+            ],
+            "group",
+        )
 
     # give it some time to sync up
     handler.close()
 
-    assert (not handler.controller.running)
+    assert not handler.controller.running
     assert len(test_handler.records) == 2
     assert len(test_handler.batches) == 1
-    (records, ) = test_handler.batches
+    (records,) = test_handler.batches
     assert len(records) == 2
-    assert test_handler.has_warning('Just testing')
-    assert test_handler.has_error('More testing')
+    assert test_handler.has_warning("Just testing")
+    assert test_handler.has_error("More testing")
 
 
-@require_module('execnet')
+@require_module("execnet")
 def test_execnet_handler():
     def run_on_remote(channel):
         import logbook
         from logbook.queues import ExecnetChannelHandler
+
         handler = ExecnetChannelHandler(channel)
-        log = logbook.Logger('Execnet')
+        log = logbook.Logger("Execnet")
         handler.push_application()
-        log.info('Execnet works')
+        log.info("Execnet works")
 
     import execnet
+
     gw = execnet.makegateway()
     channel = gw.remote_exec(run_on_remote)
     from logbook.queues import ExecnetChannelSubscriber
+
     subscriber = ExecnetChannelSubscriber(channel)
     record = subscriber.recv()
-    assert record.msg == 'Execnet works'
+    assert record.msg == "Execnet works"
     gw.exit()
 
 
-class SubscriberGroupSendBack(object):
+class SubscriberGroupSendBack:
     def __init__(self, message, queue):
         self.message = message
         self.queue = queue
 
     def __call__(self):
         from logbook.queues import MultiProcessingHandler
+
         with MultiProcessingHandler(self.queue):
             logbook.warn(self.message)
 
 
-@require_module('multiprocessing')
+@require_module("multiprocessing")
 def test_subscriber_group():
-    if os.getenv('APPVEYOR') == 'True':
-        pytest.skip('Test hangs on AppVeyor CI')
+    if os.getenv("APPVEYOR") == "True":
+        pytest.skip("Test hangs on AppVeyor CI")
     from multiprocessing import Process, Queue
+
     from logbook.queues import MultiProcessingSubscriber, SubscriberGroup
+
     a_queue = Queue(-1)
     b_queue = Queue(-1)
-    subscriber = SubscriberGroup([
-        MultiProcessingSubscriber(a_queue),
-        MultiProcessingSubscriber(b_queue)
-    ])
+    subscriber = SubscriberGroup(
+        [MultiProcessingSubscriber(a_queue), MultiProcessingSubscriber(b_queue)]
+    )
 
     for _ in range(10):
-        p1 = Process(target=SubscriberGroupSendBack('foo', a_queue))
-        p2 = Process(target=SubscriberGroupSendBack('bar', b_queue))
+        p1 = Process(target=SubscriberGroupSendBack("foo", a_queue))
+        p2 = Process(target=SubscriberGroupSendBack("bar", b_queue))
         p1.start()
         p2.start()
         p1.join()
         p2.join()
         messages = [subscriber.recv().message for i in (1, 2)]
-        assert sorted(messages) == ['bar', 'foo']
+        assert sorted(messages) == ["bar", "foo"]
 
 
-@require_module('redis')
+@require_module("redis")
 def test_redis_handler():
     import redis
+
     from logbook.queues import RedisHandler
 
-    KEY = 'redis-{}'.format(os.getpid())
-    FIELDS = ['message', 'host']
-    r = redis.Redis(decode_responses=True)
+    KEY = f"redis-{os.getpid()}"
+    FIELDS = ["message", "host"]
+    r = redis.Redis(REDIS_HOST, REDIS_PORT, decode_responses=True)
     redis_handler = RedisHandler(key=KEY, level=logbook.INFO, bubble=True)
     # We don't want output for the tests, so we can wrap everything in a
     # NullHandler
     null_handler = logbook.NullHandler()
 
     # Check default values
     with null_handler.applicationbound():
@@ -240,103 +257,110 @@
     # Are all the fields in the record?
     for field in FIELDS:
         assert message.find(field)
     assert key == KEY
     assert message.find(LETTERS)
 
     # Change the key of the handler and check on redis
-    KEY = 'test_another_key-{}'.format(os.getpid())
+    KEY = f"test_another_key-{os.getpid()}"
     redis_handler.key = KEY
 
     with null_handler.applicationbound():
         with redis_handler:
             logbook.info(LETTERS)
 
     key, message = r.blpop(KEY)
     assert key == KEY
 
     # Check that extra fields are added if specified when creating the handler
-    FIELDS.append('type')
-    extra_fields = {'type': 'test'}
-    del(redis_handler)
-    redis_handler = RedisHandler(key=KEY, level=logbook.INFO,
-                                 extra_fields=extra_fields, bubble=True)
+    FIELDS.append("type")
+    extra_fields = {"type": "test"}
+    del redis_handler
+    redis_handler = RedisHandler(
+        key=KEY, level=logbook.INFO, extra_fields=extra_fields, bubble=True
+    )
 
     with null_handler.applicationbound():
         with redis_handler:
             logbook.info(LETTERS)
 
     key, message = r.blpop(KEY)
     for field in FIELDS:
         assert message.find(field)
-    assert message.find('test')
+    assert message.find("test")
 
     # And finally, check that fields are correctly added if appended to the
     # log message
-    FIELDS.append('more_info')
+    FIELDS.append("more_info")
     with null_handler.applicationbound():
         with redis_handler:
-            logbook.info(LETTERS, more_info='This works')
+            logbook.info(LETTERS, more_info="This works")
 
     key, message = r.blpop(KEY)
     for field in FIELDS:
         assert message.find(field)
-    assert message.find('This works')
+    assert message.find("This works")
 
 
-@require_module('redis')
+@require_module("redis")
 def test_redis_handler_lpush():
     """
     Test if lpush stores messages in the right order
     new items should be first on list
     """
     import redis
+
     from logbook.queues import RedisHandler
+
     null_handler = logbook.NullHandler()
 
-    KEY = 'lpushed-'.format(os.getpid())
-    redis_handler = RedisHandler(key=KEY, push_method='lpush',
-                                 level=logbook.INFO, bubble=True)
+    KEY = f"lpushed-"
+    redis_handler = RedisHandler(
+        key=KEY, push_method="lpush", level=logbook.INFO, bubble=True
+    )
 
     with null_handler.applicationbound():
         with redis_handler:
             logbook.info("old item")
             logbook.info("new item")
 
     time.sleep(1.5)
 
-    r = redis.Redis(decode_responses=True)
+    r = redis.Redis(REDIS_HOST, REDIS_PORT, decode_responses=True)
     logs = r.lrange(KEY, 0, -1)
     assert logs
     assert "new item" in logs[0]
     r.delete(KEY)
 
 
-@require_module('redis')
+@require_module("redis")
 def test_redis_handler_rpush():
     """
     Test if rpush stores messages in the right order
     old items should be first on list
     """
     import redis
+
     from logbook.queues import RedisHandler
+
     null_handler = logbook.NullHandler()
 
-    KEY = 'rpushed-' + str(os.getpid())
-    redis_handler = RedisHandler(key=KEY, push_method='rpush',
-                                 level=logbook.INFO, bubble=True)
+    KEY = "rpushed-" + str(os.getpid())
+    redis_handler = RedisHandler(
+        key=KEY, push_method="rpush", level=logbook.INFO, bubble=True
+    )
 
     with null_handler.applicationbound():
         with redis_handler:
             logbook.info("old item")
             logbook.info("new item")
 
     time.sleep(1.5)
 
-    r = redis.Redis(decode_responses=True)
+    r = redis.Redis(REDIS_HOST, REDIS_PORT, decode_responses=True)
     logs = r.lrange(KEY, 0, -1)
     assert logs
     assert "old item" in logs[0]
     r.delete(KEY)
 
 
 @pytest.fixture
@@ -351,26 +375,26 @@
 
 @pytest.fixture
 def handlers_subscriber(multi):
     from logbook.queues import ZeroMQHandler, ZeroMQSubscriber
 
     # Get an unused port
     tempsock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-    tempsock.bind(('127.0.0.1', 0))
+    tempsock.bind(("127.0.0.1", 0))
     host, unused_port = tempsock.getsockname()
     tempsock.close()
 
     # Retrieve the ZeroMQ handler and subscriber
-    uri = 'tcp://%s:%d' % (host, unused_port)
+    uri = "tcp://%s:%d" % (host, unused_port)
     if multi:
         handlers = [ZeroMQHandler(uri, multi=True) for _ in range(3)]
     else:
         handlers = [ZeroMQHandler(uri)]
     subscriber = ZeroMQSubscriber(uri, multi=multi)
     # Enough time to start
     time.sleep(0.1)
     return handlers, subscriber
 
 
-@pytest.fixture(params=[True, False])
+@pytest.fixture(params=[True, False], ids=["multi", "nomulti"])
 def multi(request):
     return request.param
```

### Comparing `Logbook-1.5.3/tests/test_syslog_handler.py` & `Logbook-1.6.0/tests/test_syslog_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,69 +1,76 @@
 import os
 import re
 import socket
 from contextlib import closing
 
-import logbook
 import pytest
 
+import logbook
+
 UNIX_SOCKET = "/tmp/__unixsock_logbook.test"
 
-DELIMITERS = {
-    socket.AF_INET: '\n'
-}
+DELIMITERS = {socket.AF_INET: "\n"}
 
 TO_TEST = [
-    (socket.AF_INET, socket.SOCK_DGRAM, ('127.0.0.1', 0)),
-    (socket.AF_INET, socket.SOCK_STREAM, ('127.0.0.1', 0)),
+    (socket.AF_INET, socket.SOCK_DGRAM, ("127.0.0.1", 0)),
+    (socket.AF_INET, socket.SOCK_STREAM, ("127.0.0.1", 0)),
 ]
 
-UNIX_SOCKET_AVAILABLE = hasattr(socket, 'AF_UNIX')
+UNIX_SOCKET_AVAILABLE = hasattr(socket, "AF_UNIX")
 
 if UNIX_SOCKET_AVAILABLE:
-    DELIMITERS[socket.AF_UNIX] = '\x00'
+    DELIMITERS[socket.AF_UNIX] = "\x00"
     TO_TEST.append((socket.AF_UNIX, socket.SOCK_DGRAM, UNIX_SOCKET))
 
 
 @pytest.mark.usefixtures("unix_sock_path")
 @pytest.mark.parametrize("sock_family,socktype,address", TO_TEST)
-@pytest.mark.parametrize("app_name", [None, 'Testing'])
-def test_syslog_handler(logger, activation_strategy, sock_family, socktype, address, app_name):
+@pytest.mark.parametrize("app_name", [None, "Testing"])
+def test_syslog_handler(
+    logger, activation_strategy, sock_family, socktype, address, app_name
+):
     delimiter = DELIMITERS[sock_family]
     with closing(socket.socket(sock_family, socktype)) as inc:
         inc.bind(address)
 
         if socktype == socket.SOCK_STREAM:
             inc.listen(0)
 
         inc.settimeout(1)
 
         if UNIX_SOCKET_AVAILABLE and sock_family == socket.AF_UNIX:
-            expected = (r'^<12>%stestlogger: Syslog is weird%s$' % (app_name + ':' if app_name else '', delimiter))
+            expected = r"^<12>{}testlogger: Syslog is weird{}$".format(
+                app_name + ":" if app_name else "", delimiter
+            )
         else:
-            expected = (r'^<12>1 \d{4}-\d\d-\d\dT\d\d:\d\d:\d\d(\.\d+)?Z %s %s %d - - %sSyslog is weird%s$' % (
-                socket.gethostname(),
-                app_name if app_name else 'testlogger',
-                os.getpid(), 'testlogger: ' if app_name else '',
-                delimiter))
+            expected = (
+                r"^<12>1 \d{4}-\d\d-\d\dT\d\d:\d\d:\d\d(\.\d+)?Z %s %s %d - - %sSyslog is weird%s$"
+                % (
+                    socket.gethostname(),
+                    app_name if app_name else "testlogger",
+                    os.getpid(),
+                    "testlogger: " if app_name else "",
+                    delimiter,
+                )
+            )
 
         handler = logbook.SyslogHandler(app_name, inc.getsockname(), socktype=socktype)
 
         with activation_strategy(handler):
-            logger.warn('Syslog is weird')
+            logger.warn("Syslog is weird")
 
         if socktype == socket.SOCK_STREAM:
             with closing(inc.accept()[0]) as inc2:
                 rv = inc2.recv(1024)
         else:
             rv = inc.recvfrom(1024)[0]
 
-        rv = rv.decode('utf-8')
-        assert re.match(expected, rv), \
-            'expected {}, got {}'.format(expected, rv)
+        rv = rv.decode("utf-8")
+        assert re.match(expected, rv), f"expected {expected}, got {rv}"
 
 
 @pytest.fixture
 def unix_sock_path():
     try:
         yield UNIX_SOCKET
     finally:
```

### Comparing `Logbook-1.5.3/tests/test_test_handler.py` & `Logbook-1.6.0/tests/test_test_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,54 @@
 import re
 
 import pytest
 
 
-@pytest.mark.parametrize("level, method", [
-    ("trace", "has_traces"),
-    ("debug", "has_debugs"),
-    ("info", "has_infos"),
-    ("notice", "has_notices"),
-    ("warning", "has_warnings"),
-    ("error", "has_errors"),
-    ("critical", "has_criticals"),
-])
+@pytest.mark.parametrize(
+    "level, method",
+    [
+        ("trace", "has_traces"),
+        ("debug", "has_debugs"),
+        ("info", "has_infos"),
+        ("notice", "has_notices"),
+        ("warning", "has_warnings"),
+        ("error", "has_errors"),
+        ("critical", "has_criticals"),
+    ],
+)
 def test_has_level(active_handler, logger, level, method):
     log = getattr(logger, level)
-    log('Hello World')
+    log("Hello World")
     assert getattr(active_handler, method)
 
 
-@pytest.mark.parametrize("level, method", [
-    ("trace", "has_trace"),
-    ("debug", "has_debug"),
-    ("info", "has_info"),
-    ("notice", "has_notice"),
-    ("warning", "has_warning"),
-    ("error", "has_error"),
-    ("critical", "has_critical"),
-])
+@pytest.mark.parametrize(
+    "level, method",
+    [
+        ("trace", "has_trace"),
+        ("debug", "has_debug"),
+        ("info", "has_info"),
+        ("notice", "has_notice"),
+        ("warning", "has_warning"),
+        ("error", "has_error"),
+        ("critical", "has_critical"),
+    ],
+)
 def test_regex_matching(active_handler, logger, level, method):
     log = getattr(logger, level)
-    log('Hello World')
+    log("Hello World")
     has_level_method = getattr(active_handler, method)
-    assert has_level_method(re.compile('^Hello'))
-    assert (not has_level_method(re.compile('world$')))
-    assert (not has_level_method('^Hello World'))
+    assert has_level_method(re.compile("^Hello"))
+    assert not has_level_method(re.compile("world$"))
+    assert not has_level_method("^Hello World")
 
 
 def test_test_handler_cache(active_handler, logger):
-    logger.warn('First line')
+    logger.warn("First line")
     assert len(active_handler.formatted_records) == 1
     # store cache, to make sure it is identifiable
     cache = active_handler.formatted_records
     assert len(active_handler.formatted_records) == 1
     assert cache is active_handler.formatted_records
-    logger.warn('Second line invalidates cache')
+    logger.warn("Second line invalidates cache")
     assert len(active_handler.formatted_records) == 2
-    assert (cache is not active_handler.formatted_records)
+    assert cache is not active_handler.formatted_records
```

### Comparing `Logbook-1.5.3/tests/test_ticketing.py` & `Logbook-1.6.0/tests/test_ticketing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,30 @@
 import os
-import sys
-
-try:
-    from thread import get_ident
-except ImportError:
-    from _thread import get_ident
+from threading import get_ident
 
 import logbook
-import pytest
-from logbook.helpers import xrange
 
 from .utils import require_module
 
 __file_without_pyc__ = __file__
 if __file_without_pyc__.endswith(".pyc"):
     __file_without_pyc__ = __file_without_pyc__[:-1]
 
-python_version = sys.version_info[:2]
-
 
-@pytest.mark.xfail(
-    os.name == 'nt' and (python_version == (3, 2) or python_version == (3, 3)),
-    reason='Problem with in-memory sqlite on Python 3.2, 3.3 and Windows')
-@require_module('sqlalchemy')
+@require_module("sqlalchemy")
 def test_basic_ticketing(logger):
-    from logbook.ticketing import TicketingHandler
     from time import sleep
-    with TicketingHandler('sqlite:///') as handler:
-        for x in xrange(5):
-            logger.warn('A warning')
+
+    from logbook.ticketing import TicketingHandler
+
+    with TicketingHandler("sqlite:///") as handler:
+        for x in range(5):
+            logger.warn("A warning")
             sleep(0.2)
-            logger.info('An error')
+            logger.info("An error")
             sleep(0.2)
             if x < 2:
                 try:
                     1 / 0
                 except Exception:
                     logger.exception()
 
@@ -52,19 +42,18 @@
     tickets[0].solve()
     assert tickets[0].solved
     tickets[0].delete()
 
     ticket = handler.db.get_ticket(tickets[1].ticket_id)
     assert ticket == tickets[1]
 
-    occurrences = handler.db.get_occurrences(tickets[2].ticket_id,
-                                             order_by='time')
+    occurrences = handler.db.get_occurrences(tickets[2].ticket_id, order_by="time")
     assert len(occurrences) == 2
     record = occurrences[0]
     assert __file_without_pyc__ in record.filename
     # avoid 2to3 destroying our assertion
-    assert getattr(record, 'func_name') == 'test_basic_ticketing'
+    assert getattr(record, "func_name") == "test_basic_ticketing"
     assert record.level == logbook.ERROR
     assert record.thread == get_ident()
     assert record.process == os.getpid()
-    assert record.channel == 'testlogger'
-    assert '1 / 0' in record.formatted_exception
+    assert record.channel == "testlogger"
+    assert "1 / 0" in record.formatted_exception
```

### Comparing `Logbook-1.5.3/tests/test_unicode.py` & `Logbook-1.6.0/tests/test_unicode.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,53 @@
-# -*- coding: utf-8 -*-
-from .utils import require_py3, capturing_stderr_context
-
 import logbook
 
+from .utils import capturing_stderr_context
+
 
-@require_py3
 def test_default_format_unicode(logger):
     with capturing_stderr_context() as stream:
-        logger.warn('\u2603')
-    assert 'WARNING: testlogger: \u2603' in stream.getvalue()
+        logger.warn("\u2603")
+    assert "WARNING: testlogger: \u2603" in stream.getvalue()
 
 
-@require_py3
 def test_default_format_encoded(logger):
     with capturing_stderr_context() as stream:
         # it's a string but it's in the right encoding so don't barf
-        logger.warn('\u2603')
-    assert 'WARNING: testlogger: \u2603' in stream.getvalue()
+        logger.warn("\u2603")
+    assert "WARNING: testlogger: \u2603" in stream.getvalue()
 
 
-@require_py3
 def test_default_format_bad_encoding(logger):
     with capturing_stderr_context() as stream:
         # it's a string, is wrong, but just dump it in the logger,
         # don't try to decode/encode it
-        logger.warn('Русский'.encode('koi8-r'))
+        logger.warn("Русский".encode("koi8-r"))
     expected = "WARNING: testlogger: b'\\xf2\\xd5\\xd3\\xd3\\xcb\\xc9\\xca'"
     assert expected in stream.getvalue()
 
 
-@require_py3
 def test_custom_unicode_format_unicode(logger):
-    format_string = ('[{record.level_name}] '
-                     '{record.channel}: {record.message}')
+    format_string = "[{record.level_name}] {record.channel}: {record.message}"
     with capturing_stderr_context() as stream:
         with logbook.StderrHandler(format_string=format_string):
             logger.warn("\u2603")
-    assert '[WARNING] testlogger: \u2603' in stream.getvalue()
+    assert "[WARNING] testlogger: \u2603" in stream.getvalue()
 
 
-@require_py3
 def test_custom_string_format_unicode(logger):
-    format_string = ('[{record.level_name}] '
-                     '{record.channel}: {record.message}')
+    format_string = "[{record.level_name}] {record.channel}: {record.message}"
     with capturing_stderr_context() as stream:
         with logbook.StderrHandler(format_string=format_string):
-            logger.warn('\u2603')
-    assert '[WARNING] testlogger: \u2603' in stream.getvalue()
+            logger.warn("\u2603")
+    assert "[WARNING] testlogger: \u2603" in stream.getvalue()
 
 
-@require_py3
 def test_unicode_message_encoded_params(logger):
     with capturing_stderr_context() as stream:
-        logger.warn("\u2603 {0}", "\u2603".encode('utf8'))
+        logger.warn("\u2603 {0}", "\u2603".encode())
     assert "WARNING: testlogger: \u2603 b'\\xe2\\x98\\x83'" in stream.getvalue()
 
 
-@require_py3
 def test_encoded_message_unicode_params(logger):
     with capturing_stderr_context() as stream:
-        logger.warn('\u2603 {0}'.encode('utf8'), '\u2603')
-    assert 'WARNING: testlogger: \u2603 \u2603' in stream.getvalue()
+        logger.warn("\u2603 {0}".encode(), "\u2603")
+    assert "WARNING: testlogger: \u2603 \u2603" in stream.getvalue()
```

### Comparing `Logbook-1.5.3/tests/test_utils.py` & `Logbook-1.6.0/tests/test_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,234 +1,229 @@
+from time import sleep
+from unittest.mock import Mock, call
+
 import pytest
-import logbook
 
+import logbook
 from logbook.utils import (
-    logged_if_slow, deprecated, forget_deprecation_locations,
-    suppressed_deprecations, log_deprecation_message)
-from time import sleep
+    deprecated,
+    forget_deprecation_locations,
+    log_deprecation_message,
+    logged_if_slow,
+    suppressed_deprecations,
+)
 
 _THRESHOLD = 0.1
 
-try:
-    from unittest.mock import Mock, call
-except ImportError:
-    from mock import Mock, call
-
 
+@pytest.mark.flaky(reruns=5)
 def test_logged_if_slow_reached(test_handler):
     with test_handler.applicationbound():
-        with logged_if_slow('checking...', threshold=_THRESHOLD):
+        with logged_if_slow("checking...", threshold=_THRESHOLD):
             sleep(2 * _THRESHOLD)
         assert len(test_handler.records) == 1
         [record] = test_handler.records
-        assert record.message == 'checking...'
+        assert record.message == "checking..."
 
 
+@pytest.mark.flaky(reruns=5)
 def test_logged_if_slow_did_not_reached(test_handler):
     with test_handler.applicationbound():
-        with logged_if_slow('checking...', threshold=_THRESHOLD):
+        with logged_if_slow("checking...", threshold=_THRESHOLD):
             sleep(_THRESHOLD / 2)
         assert len(test_handler.records) == 0
 
 
+@pytest.mark.flaky(reruns=5)
 def test_logged_if_slow_logger():
     logger = Mock()
 
-    with logged_if_slow('checking...', threshold=_THRESHOLD, logger=logger):
+    with logged_if_slow("checking...", threshold=_THRESHOLD, logger=logger):
         sleep(2 * _THRESHOLD)
 
-    assert logger.log.call_args == call(logbook.DEBUG, 'checking...')
+    assert logger.log.call_args == call(logbook.DEBUG, "checking...")
 
 
+@pytest.mark.flaky(reruns=5)
 def test_logged_if_slow_level(test_handler):
     with test_handler.applicationbound():
-        with logged_if_slow('checking...', threshold=_THRESHOLD,
-                            level=logbook.WARNING):
+        with logged_if_slow("checking...", threshold=_THRESHOLD, level=logbook.WARNING):
             sleep(2 * _THRESHOLD)
 
     assert test_handler.records[0].level == logbook.WARNING
 
 
+@pytest.mark.flaky(reruns=5)
 def test_logged_if_slow_deprecated(logger, test_handler):
     with test_handler.applicationbound():
-        with logged_if_slow('checking...', threshold=_THRESHOLD,
-                            func=logbook.error):
+        with logged_if_slow("checking...", threshold=_THRESHOLD, func=logbook.error):
             sleep(2 * _THRESHOLD)
 
     assert test_handler.records[0].level == logbook.ERROR
-    assert test_handler.records[0].message == 'checking...'
+    assert test_handler.records[0].message == "checking..."
 
     with pytest.raises(TypeError):
-        logged_if_slow('checking...', logger=logger, func=logger.error)
+        logged_if_slow("checking...", logger=logger, func=logger.error)
 
 
 def test_deprecated_func_called(capture):
     assert deprecated_func(1, 2) == 3
 
 
 def test_deprecation_message(capture):
     deprecated_func(1, 2)
 
     [record] = capture.records
     assert "deprecated" in record.message
-    assert 'deprecated_func' in record.message
+    assert "deprecated_func" in record.message
 
 
 def test_deprecation_with_message(capture):
-
     @deprecated("use something else instead")
     def func(a, b):
         return a + b
 
     func(1, 2)
 
     [record] = capture.records
     assert "use something else instead" in record.message
     assert "func is deprecated" in record.message
 
 
 def test_no_deprecations(capture):
-
-    @deprecated('msg')
+    @deprecated("msg")
     def func(a, b):
         return a + b
 
     with suppressed_deprecations():
         assert func(1, 2) == 3
     assert not capture.records
 
 
 def _no_decorator(func):
     return func
 
 
-@pytest.mark.parametrize('decorator', [_no_decorator, classmethod])
+@pytest.mark.parametrize("decorator", [_no_decorator, classmethod])
 def test_class_deprecation(capture, decorator):
-
-    class Bla(object):
-
-        @deprecated('reason')
+    class Bla:
+        @deprecated("reason")
         @classmethod
         def func(self, a, b):
             assert isinstance(self, Bla)
             return a + b
 
     assert Bla().func(2, 4) == 6
 
     [record] = capture.records
-    assert 'Bla.func is deprecated' in record.message
+    assert "Bla.func is deprecated" in record.message
 
 
 def test_deprecations_different_sources(capture):
-
     def f():
         deprecated_func(1, 2)
 
     def g():
         deprecated_func(1, 2)
 
     f()
     g()
     assert len(capture.records) == 2
 
 
 def test_deprecations_same_sources(capture):
-
     def f():
         deprecated_func(1, 2)
 
     f()
     f()
     assert len(capture.records) == 1
 
 
 def test_deprecation_message_different_sources(capture):
-
     def f(flag):
         if flag:
-            log_deprecation_message('first message type')
+            log_deprecation_message("first message type")
         else:
-            log_deprecation_message('second message type')
+            log_deprecation_message("second message type")
 
     f(True)
     f(False)
     assert len(capture.records) == 2
 
 
 def test_deprecation_message_same_sources(capture):
-
     def f(flag):
         if flag:
-            log_deprecation_message('first message type')
+            log_deprecation_message("first message type")
         else:
-            log_deprecation_message('second message type')
+            log_deprecation_message("second message type")
 
     f(True)
     f(True)
     assert len(capture.records) == 1
 
 
 def test_deprecation_message_full_warning(capture):
     def f():
-        log_deprecation_message('some_message')
+        log_deprecation_message("some_message")
+
     f()
 
     [record] = capture.records
-    assert record.message == 'Deprecation message: some_message'
+    assert record.message == "Deprecation message: some_message"
 
 
 def test_name_doc():
     @deprecated
     def some_func():
         """docstring here"""
         pass
 
-    assert some_func.__name__ == 'some_func'
-    assert 'docstring here' in some_func.__doc__
+    assert some_func.__name__ == "some_func"
+    assert "docstring here" in some_func.__doc__
 
 
 def test_doc_update():
-    @deprecated('some_message')
+    @deprecated("some_message")
     def some_func():
         """docstring here"""
         pass
 
-    some_func.__doc__ = 'new_docstring'
+    some_func.__doc__ = "new_docstring"
 
-    assert 'docstring here' not in some_func.__doc__
-    assert 'new_docstring' in some_func.__doc__
-    assert 'some_message' in some_func.__doc__
+    assert "docstring here" not in some_func.__doc__
+    assert "new_docstring" in some_func.__doc__
+    assert "some_message" in some_func.__doc__
 
 
 def test_deprecatd_docstring():
-
     message = "Use something else instead"
 
     @deprecated()
     def some_func():
-        """This is a function
-        """
+        """This is a function"""
 
     @deprecated(message)
     def other_func():
-        """This is another function
-        """
+        """This is another function"""
 
     assert ".. deprecated" in some_func.__doc__
-    assert ".. deprecated\n   {0}".format(message) in other_func.__doc__
+    assert f".. deprecated\n   {message}" in other_func.__doc__
 
 
 @pytest.fixture
 def capture(request):
     handler = logbook.TestHandler(level=logbook.WARNING)
     handler.push_application()
 
     @request.addfinalizer
     def pop():
         handler.pop_application()
+
     return handler
 
 
 @deprecated
 def deprecated_func(a, b):
     return a + b
```

### Comparing `Logbook-1.5.3/tests/utils.py` & `Logbook-1.6.0/tests/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,37 @@
-# -*- coding: utf-8 -*-
 """
     test utils for logbook
     ~~~~~~~~~~~~~~~~~~~~~~
 
     :copyright: (c) 2010 by Armin Ronacher, Georg Brandl.
     :license: BSD, see LICENSE for more details.
 """
 import functools
-import os
+import importlib
 import sys
 from contextlib import contextmanager
-
-import logbook
-from logbook.helpers import StringIO
+from io import StringIO
 
 import pytest
 
+import logbook
+
 _missing = object()
 
 LETTERS = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ"
 
 
-def get_total_delta_seconds(delta):
-    """
-    Replacement for datetime.timedelta.total_seconds() for Python 2.5, 2.6
-    and 3.1
-    """
-    return (delta.microseconds + (delta.seconds + delta.days * 24 * 3600) * 10**6) / 10**6
-
-
-require_py3 = pytest.mark.skipif(
-    sys.version_info[0] < 3, reason="Requires Python 3")
-
-appveyor = pytest.mark.skipif(
-    os.environ.get('APPVEYOR') != 'True', reason='AppVeyor CI test')
-
-travis = pytest.mark.skipif(
-    os.environ.get('TRAVIS') != 'true', reason='Travis CI test')
-
-
 def require_module(module_name):
     found = True
     try:
-        __import__(module_name)
+        importlib.import_module(module_name)
     except ImportError:
         found = False
 
-    return pytest.mark.skipif(
-        not found, reason='Module {0} is required'.format(module_name))
+    return pytest.mark.skipif(not found, reason=f"Module {module_name} is required")
 
 
 def make_fake_mail_handler(**kwargs):
     class FakeMailHandler(logbook.MailHandler):
         mails = []
 
         def get_connection(self):
@@ -59,16 +39,16 @@
 
         def close_connection(self, con):
             pass
 
         def sendmail(self, fromaddr, recipients, mail):
             self.mails.append((fromaddr, recipients, mail))
 
-    kwargs.setdefault('level', logbook.ERROR)
-    return FakeMailHandler('foo@example.com', ['bar@example.com'], **kwargs)
+    kwargs.setdefault("level", logbook.ERROR)
+    return FakeMailHandler("foo@example.com", ["bar@example.com"], **kwargs)
 
 
 def missing(name):
     def decorate(f):
         @functools.wraps(f)
         def wrapper(*args, **kwargs):
             old = sys.modules.get(name, _missing)
@@ -76,15 +56,17 @@
             try:
                 f(*args, **kwargs)
             finally:
                 if old is _missing:
                     del sys.modules[name]
                 else:
                     sys.modules[name] = old
+
         return wrapper
+
     return decorate
 
 
 def activate_via_with_statement(handler):
     return handler
```

