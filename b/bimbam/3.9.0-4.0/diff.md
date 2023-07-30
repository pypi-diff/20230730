# Comparing `tmp/bimbam-3.9.0.tar.gz` & `tmp/bimbam-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bimbam-3.9.0.tar", last modified: Fri Jul 28 12:19:27 2023, max compression
+gzip compressed data, was "bimbam-4.0.tar", last modified: Sun Jul 30 12:30:12 2023, max compression
```

## Comparing `bimbam-3.9.0.tar` & `bimbam-4.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-28 12:19:27.988488 bimbam-3.9.0/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      666 2023-07-28 12:19:27.988488 bimbam-3.9.0/PKG-INFO
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-28 12:19:27.976487 bimbam-3.9.0/bimbam.egg-info/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      666 2023-07-28 12:19:27.000000 bimbam-3.9.0/bimbam.egg-info/PKG-INFO
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2648 2023-07-28 12:19:27.000000 bimbam-3.9.0/bimbam.egg-info/SOURCES.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-07-28 12:19:27.000000 bimbam-3.9.0/bimbam.egg-info/dependency_links.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-07-28 12:19:27.000000 bimbam-3.9.0/bimbam.egg-info/requires.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-07-28 12:19:27.000000 bimbam-3.9.0/bimbam.egg-info/top_level.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       38 2023-07-28 12:19:27.988488 bimbam-3.9.0/setup.cfg
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1963 2023-07-28 12:19:08.000000 bimbam-3.9.0/setup.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-28 12:19:27.976487 bimbam-3.9.0/thonnycontrib/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1804 2023-07-26 19:04:33.000000 bimbam-3.9.0/thonnycontrib/ThonnyLogsGenerator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-28 12:19:27.980487 bimbam-3.9.0/thonnycontrib/backend/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/backend/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17887 2023-07-27 19:37:17.000000 bimbam-3.9.0/thonnycontrib/backend/ast_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    35564 2023-07-23 17:34:08.000000 bimbam-3.9.0/thonnycontrib/backend/doctest_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5015 2023-07-27 19:30:14.000000 bimbam-3.9.0/thonnycontrib/backend/evaluator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4508 2023-07-27 19:33:34.000000 bimbam-3.9.0/thonnycontrib/backend/l1test_backend.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7164 2023-07-27 19:31:40.000000 bimbam-3.9.0/thonnycontrib/backend/test_finder.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-28 12:19:27.980487 bimbam-3.9.0/thonnycontrib/backend/verdicts/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2379 2023-07-22 13:45:44.000000 bimbam-3.9.0/thonnycontrib/backend/verdicts/ExampleVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      475 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/backend/verdicts/ExceptionVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      735 2023-07-23 18:54:56.000000 bimbam-3.9.0/thonnycontrib/backend/verdicts/FailedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      644 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      371 2023-07-22 11:09:20.000000 bimbam-3.9.0/thonnycontrib/backend/verdicts/PassedSetupVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      429 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/backend/verdicts/PassedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/backend/verdicts/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-28 12:19:27.980487 bimbam-3.9.0/thonnycontrib/docs/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/docs/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-28 12:19:27.980487 bimbam-3.9.0/thonnycontrib/docs/res/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      912 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/docs/res/error_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1778 2023-07-27 18:28:42.000000 bimbam-3.9.0/thonnycontrib/docs/res/exception_red_chip.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1275 2023-07-27 19:02:02.000000 bimbam-3.9.0/thonnycontrib/docs/res/failed.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1647 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/docs/res/failed_red_chip.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2130 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/docs/res/l1test_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2086 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/docs/res/l1test_icon_old.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      628 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/docs/res/outline_class.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      578 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/docs/res/outline_method.gif
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1213 2023-07-27 19:01:55.000000 bimbam-3.9.0/thonnycontrib/docs/res/passed.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1531 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/docs/res/pending_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      997 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/docs/res/restart_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1625 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/docs/res/success_green_chip.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1073 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/docs/res/warning.png
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-28 12:19:27.984488 bimbam-3.9.0/thonnycontrib/docstring_generator/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      408 2023-07-23 13:51:19.000000 bimbam-3.9.0/thonnycontrib/docstring_generator/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    11803 2023-07-27 19:42:02.000000 bimbam-3.9.0/thonnycontrib/docstring_generator/doc_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7054 2023-07-22 09:12:15.000000 bimbam-3.9.0/thonnycontrib/docstring_generator/doc_template.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1058 2023-07-23 10:37:34.000000 bimbam-3.9.0/thonnycontrib/environement_vars.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3712 2023-07-27 21:16:38.000000 bimbam-3.9.0/thonnycontrib/exceptions.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-28 12:19:27.984488 bimbam-3.9.0/thonnycontrib/l1test_configuration/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/l1test_configuration/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2991 2023-07-23 10:41:36.000000 bimbam-3.9.0/thonnycontrib/l1test_configuration/l1test_options.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-28 12:19:27.984488 bimbam-3.9.0/thonnycontrib/l1test_frontend/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      754 2023-07-23 12:01:22.000000 bimbam-3.9.0/thonnycontrib/l1test_frontend/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2847 2023-07-20 20:39:26.000000 bimbam-3.9.0/thonnycontrib/l1test_frontend/l1test_error_view.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3986 2023-07-23 12:06:57.000000 bimbam-3.9.0/thonnycontrib/l1test_frontend/l1test_outliner_menu.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2749 2023-07-23 16:34:32.000000 bimbam-3.9.0/thonnycontrib/l1test_frontend/l1test_reporter.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    23084 2023-07-27 21:21:22.000000 bimbam-3.9.0/thonnycontrib/l1test_frontend/l1test_runner.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    41453 2023-07-28 11:09:46.000000 bimbam-3.9.0/thonnycontrib/l1test_frontend/l1test_treeview.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-28 12:19:27.984488 bimbam-3.9.0/thonnycontrib/main_generator/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-07-22 08:21:17.000000 bimbam-3.9.0/thonnycontrib/main_generator/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5295 2023-07-23 11:59:59.000000 bimbam-3.9.0/thonnycontrib/main_generator/main_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5332 2023-07-23 16:18:24.000000 bimbam-3.9.0/thonnycontrib/plugin_loader.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2962 2023-07-27 19:06:48.000000 bimbam-3.9.0/thonnycontrib/properties.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-28 12:19:27.984488 bimbam-3.9.0/thonnycontrib/tests/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/tests/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-28 12:19:27.984488 bimbam-3.9.0/thonnycontrib/tests/fixtures/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-24 19:06:13.000000 bimbam-3.9.0/thonnycontrib/tests/fixtures/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      348 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/tests/fixtures/backend_mock.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1767 2023-07-22 09:17:05.000000 bimbam-3.9.0/thonnycontrib/tests/fixtures/workbench_mock.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1991 2023-07-24 19:13:49.000000 bimbam-3.9.0/thonnycontrib/tests/tests_doc_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5767 2023-07-27 19:30:14.000000 bimbam-3.9.0/thonnycontrib/tests/tests_example_no_expected.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16504 2023-07-27 19:30:14.000000 bimbam-3.9.0/thonnycontrib/tests/tests_example_with_exception.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    21862 2023-07-27 19:30:14.000000 bimbam-3.9.0/thonnycontrib/tests/tests_example_with_expected.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7935 2023-07-27 19:56:06.000000 bimbam-3.9.0/thonnycontrib/tests/tests_l1TestRunner.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2030 2023-07-26 07:37:26.000000 bimbam-3.9.0/thonnycontrib/tests/tests_main_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6202 2023-07-27 19:30:14.000000 bimbam-3.9.0/thonnycontrib/tests/tests_test_finder.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    14861 2023-07-24 19:26:54.000000 bimbam-3.9.0/thonnycontrib/tests/tests_view.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    18025 2023-07-27 20:42:09.000000 bimbam-3.9.0/thonnycontrib/utils.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-30 12:30:12.320661 bimbam-4.0/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      664 2023-07-30 12:30:12.320661 bimbam-4.0/PKG-INFO
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-30 12:30:12.308660 bimbam-4.0/bimbam.egg-info/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      664 2023-07-30 12:30:12.000000 bimbam-4.0/bimbam.egg-info/PKG-INFO
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2648 2023-07-30 12:30:12.000000 bimbam-4.0/bimbam.egg-info/SOURCES.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-07-30 12:30:12.000000 bimbam-4.0/bimbam.egg-info/dependency_links.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-07-30 12:30:12.000000 bimbam-4.0/bimbam.egg-info/requires.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-07-30 12:30:12.000000 bimbam-4.0/bimbam.egg-info/top_level.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       38 2023-07-30 12:30:12.320661 bimbam-4.0/setup.cfg
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1961 2023-07-30 12:30:06.000000 bimbam-4.0/setup.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-30 12:30:12.308660 bimbam-4.0/thonnycontrib/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1804 2023-07-26 19:04:33.000000 bimbam-4.0/thonnycontrib/ThonnyLogsGenerator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-30 12:30:12.312661 bimbam-4.0/thonnycontrib/backend/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/backend/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17887 2023-07-27 19:37:17.000000 bimbam-4.0/thonnycontrib/backend/ast_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    35564 2023-07-23 17:34:08.000000 bimbam-4.0/thonnycontrib/backend/doctest_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5015 2023-07-27 19:30:14.000000 bimbam-4.0/thonnycontrib/backend/evaluator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4508 2023-07-27 19:33:34.000000 bimbam-4.0/thonnycontrib/backend/l1test_backend.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7164 2023-07-27 19:31:40.000000 bimbam-4.0/thonnycontrib/backend/test_finder.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-30 12:30:12.312661 bimbam-4.0/thonnycontrib/backend/verdicts/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2379 2023-07-22 13:45:44.000000 bimbam-4.0/thonnycontrib/backend/verdicts/ExampleVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      475 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/backend/verdicts/ExceptionVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      735 2023-07-23 18:54:56.000000 bimbam-4.0/thonnycontrib/backend/verdicts/FailedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      644 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      371 2023-07-22 11:09:20.000000 bimbam-4.0/thonnycontrib/backend/verdicts/PassedSetupVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      429 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/backend/verdicts/PassedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/backend/verdicts/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-30 12:30:12.312661 bimbam-4.0/thonnycontrib/docs/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/docs/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-30 12:30:12.316661 bimbam-4.0/thonnycontrib/docs/res/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      912 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/docs/res/error_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1778 2023-07-27 18:28:42.000000 bimbam-4.0/thonnycontrib/docs/res/exception_red_chip.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1275 2023-07-27 19:02:02.000000 bimbam-4.0/thonnycontrib/docs/res/failed.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1647 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/docs/res/failed_red_chip.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2130 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/docs/res/l1test_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2086 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/docs/res/l1test_icon_old.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      628 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/docs/res/outline_class.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      578 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/docs/res/outline_method.gif
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1213 2023-07-27 19:01:55.000000 bimbam-4.0/thonnycontrib/docs/res/passed.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1531 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/docs/res/pending_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      997 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/docs/res/restart_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1625 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/docs/res/success_green_chip.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1073 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/docs/res/warning.png
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-30 12:30:12.316661 bimbam-4.0/thonnycontrib/docstring_generator/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      585 2023-07-29 21:42:29.000000 bimbam-4.0/thonnycontrib/docstring_generator/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16159 2023-07-30 12:26:59.000000 bimbam-4.0/thonnycontrib/docstring_generator/doc_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7054 2023-07-22 09:12:15.000000 bimbam-4.0/thonnycontrib/docstring_generator/doc_template.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1058 2023-07-23 10:37:34.000000 bimbam-4.0/thonnycontrib/environement_vars.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3712 2023-07-27 21:16:38.000000 bimbam-4.0/thonnycontrib/exceptions.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-30 12:30:12.316661 bimbam-4.0/thonnycontrib/l1test_configuration/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/l1test_configuration/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2991 2023-07-23 10:41:36.000000 bimbam-4.0/thonnycontrib/l1test_configuration/l1test_options.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-30 12:30:12.316661 bimbam-4.0/thonnycontrib/l1test_frontend/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      754 2023-07-23 12:01:22.000000 bimbam-4.0/thonnycontrib/l1test_frontend/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2847 2023-07-20 20:39:26.000000 bimbam-4.0/thonnycontrib/l1test_frontend/l1test_error_view.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3986 2023-07-23 12:06:57.000000 bimbam-4.0/thonnycontrib/l1test_frontend/l1test_outliner_menu.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2749 2023-07-23 16:34:32.000000 bimbam-4.0/thonnycontrib/l1test_frontend/l1test_reporter.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    23084 2023-07-27 21:21:22.000000 bimbam-4.0/thonnycontrib/l1test_frontend/l1test_runner.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    41416 2023-07-28 15:24:19.000000 bimbam-4.0/thonnycontrib/l1test_frontend/l1test_treeview.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-30 12:30:12.320661 bimbam-4.0/thonnycontrib/main_generator/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-07-22 08:21:17.000000 bimbam-4.0/thonnycontrib/main_generator/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5301 2023-07-28 14:35:18.000000 bimbam-4.0/thonnycontrib/main_generator/main_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5469 2023-07-30 12:01:10.000000 bimbam-4.0/thonnycontrib/plugin_loader.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2962 2023-07-27 19:06:48.000000 bimbam-4.0/thonnycontrib/properties.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-30 12:30:12.320661 bimbam-4.0/thonnycontrib/tests/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/tests/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-30 12:30:12.320661 bimbam-4.0/thonnycontrib/tests/fixtures/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-24 19:06:13.000000 bimbam-4.0/thonnycontrib/tests/fixtures/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      348 2023-07-20 20:20:05.000000 bimbam-4.0/thonnycontrib/tests/fixtures/backend_mock.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1767 2023-07-22 09:17:05.000000 bimbam-4.0/thonnycontrib/tests/fixtures/workbench_mock.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2306 2023-07-29 22:32:55.000000 bimbam-4.0/thonnycontrib/tests/tests_doc_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5767 2023-07-27 19:30:14.000000 bimbam-4.0/thonnycontrib/tests/tests_example_no_expected.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16504 2023-07-27 19:30:14.000000 bimbam-4.0/thonnycontrib/tests/tests_example_with_exception.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    21862 2023-07-27 19:30:14.000000 bimbam-4.0/thonnycontrib/tests/tests_example_with_expected.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7935 2023-07-27 19:56:06.000000 bimbam-4.0/thonnycontrib/tests/tests_l1TestRunner.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2030 2023-07-26 07:37:26.000000 bimbam-4.0/thonnycontrib/tests/tests_main_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6202 2023-07-27 19:30:14.000000 bimbam-4.0/thonnycontrib/tests/tests_test_finder.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    14861 2023-07-24 19:26:54.000000 bimbam-4.0/thonnycontrib/tests/tests_view.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    20009 2023-07-30 12:00:21.000000 bimbam-4.0/thonnycontrib/utils.py
```

### Comparing `bimbam-3.9.0/PKG-INFO` & `bimbam-4.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bimbam
-Version: 3.9.0
+Version: 4.0
 Summary: A plug-in which adds a test framework
 Home-page: https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests
 Author: idtaleb
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Topic :: Education :: Testing
```

### Comparing `bimbam-3.9.0/bimbam.egg-info/PKG-INFO` & `bimbam-4.0/bimbam.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bimbam
-Version: 3.9.0
+Version: 4.0
 Summary: A plug-in which adds a test framework
 Home-page: https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests
 Author: idtaleb
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Topic :: Education :: Testing
```

### Comparing `bimbam-3.9.0/bimbam.egg-info/SOURCES.txt` & `bimbam-4.0/bimbam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/setup.py` & `bimbam-4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     return py_packs | other_packs
 
 setupdir = os.path.dirname(__file__)
 
 
 setup(
     name="bimbam",
-    version="3.9.0",
+    version="4.0",
     author="idtaleb",
     description="A plug-in which adds a test framework",
     long_description="""A plug-in for Thonny which allows you to test your doc examples
  
 More info: https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests""",
     url="https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests",
 #    keywords="IDE education programming tests in documentation",
```

### Comparing `bimbam-3.9.0/thonnycontrib/ThonnyLogsGenerator.py` & `bimbam-4.0/thonnycontrib/ThonnyLogsGenerator.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/backend/ast_parser.py` & `bimbam-4.0/thonnycontrib/backend/ast_parser.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/backend/doctest_parser.py` & `bimbam-4.0/thonnycontrib/backend/doctest_parser.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/backend/evaluator.py` & `bimbam-4.0/thonnycontrib/backend/evaluator.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/backend/l1test_backend.py` & `bimbam-4.0/thonnycontrib/backend/l1test_backend.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/backend/test_finder.py` & `bimbam-4.0/thonnycontrib/backend/test_finder.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/backend/verdicts/ExampleVerdict.py` & `bimbam-4.0/thonnycontrib/backend/verdicts/ExampleVerdict.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/backend/verdicts/FailedVerdict.py` & `bimbam-4.0/thonnycontrib/backend/verdicts/FailedVerdict.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py` & `bimbam-4.0/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/docs/res/error_icon.png` & `bimbam-4.0/thonnycontrib/docs/res/error_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/docs/res/exception_red_chip.png` & `bimbam-4.0/thonnycontrib/docs/res/exception_red_chip.png`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/docs/res/failed.png` & `bimbam-4.0/thonnycontrib/docs/res/failed.png`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/docs/res/failed_red_chip.png` & `bimbam-4.0/thonnycontrib/docs/res/failed_red_chip.png`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/docs/res/l1test_icon.png` & `bimbam-4.0/thonnycontrib/docs/res/l1test_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/docs/res/l1test_icon_old.png` & `bimbam-4.0/thonnycontrib/docs/res/l1test_icon_old.png`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/docs/res/outline_class.png` & `bimbam-4.0/thonnycontrib/docs/res/outline_class.png`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/docs/res/outline_method.gif` & `bimbam-4.0/thonnycontrib/docs/res/outline_method.gif`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/docs/res/passed.png` & `bimbam-4.0/thonnycontrib/docs/res/passed.png`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/docs/res/pending_icon.png` & `bimbam-4.0/thonnycontrib/docs/res/pending_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/docs/res/restart_icon.png` & `bimbam-4.0/thonnycontrib/docs/res/restart_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/docs/res/success_green_chip.png` & `bimbam-4.0/thonnycontrib/docs/res/success_green_chip.png`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/docs/res/warning.png` & `bimbam-4.0/thonnycontrib/docs/res/warning.png`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/docstring_generator/doc_generator.py` & `bimbam-4.0/thonnycontrib/docstring_generator/doc_generator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import re
 import sys
 import textwrap
+from typing import List
+
+from .doc_template import DocTemplate
 from ..backend.ast_parser import L1TestAstParser
 from .doc_template import *
 from ..properties import CANNOT_GENERATE_THE_DOCSTRING
 from thonny.tktextext import *  
 from ..exceptions import DocGeneratorParserException, FrontendException, NoFunctionSelectedToDocumentException
-from ..utils import replace_error_line, get_last_exception, assert_one_line_is_selected
+from ..utils import replace_error_line, get_last_exception
 from thonny.editors import EditorCodeViewText
 from ..ThonnyLogsGenerator import log_doc_in_thonny
 from thonny import get_workbench
 from .. l1test_frontend import get_l1test_runner
 from thonnycontrib import docstring_generator
 
 r""" Docstring Generator Module
@@ -82,58 +85,31 @@
         self._ast_parser.set_source(source)
         
     def get_source(self):
         return self._source 
     
     def set_ast_parser(self, parser) :
         self._ast_parser = parser
-       
-class DocGenerator(ABC):
-    def __init__(self, parser=DocParser(), template:DocTemplate=None):
-        docstring_generator._doc_generator = self
-        self._parser = parser
-        self._template = template
-        self._has_exception = False
+
+class DocGenerationStrategy(ABC):
+    _SIGNATURE_REGEX = r"\s*(?P<id>def|class)\s*.*\s*$"
     
-    def run(self, selected_lineno:int, text_widget:EditorCodeViewText):
-        try:
-            # get the content of the selected line
-            selected_sig = text_widget.get(str(selected_lineno)+".0", str(selected_lineno+1)+".0").strip("\n")
-            if selected_sig: 
-                filename = get_workbench().get_editor_notebook().get_current_editor().get_filename()
-                if not filename:
-                    filename = "<unknown>" 
-                
-                assert_one_line_is_selected(text_widget)
-                        
-                self.set_filename(filename)
-                self.generate(selected_sig, selected_lineno, text_widget)   
-                
-                # après la génération (réussie) on vérifie si docgen avait rencontré une exception avant. Si oui, 
-                # on supprime l'exception de docgen (car elle a été déja montrée).
-                if get_l1test_runner().has_exception() or self.has_exception(): # si docgen avait lancé une exception avant
-                    # si les deux ont lancé une exception, on affiche l'exception de docgen
-                    if get_l1test_runner().has_exception() and self.has_exception(): 
-                        get_l1test_runner().clean_error_view()
-                        get_l1test_runner().get_reporter().get_error_view().hide_view()
-                        get_l1test_runner().get_reporter().get_treeview().show_view()
-                    else:
-                        self._show_treeview()
-                
-                self.set_has_exception(False) # success
-        except NoFunctionSelectedToDocumentException as e:
-            pass # do nothing
-        except FrontendException as e: # parsing error
-            self.set_has_exception(True)
-            self._show_error(str(e))
-                      
-        # Cette ligne est importante pour reprendre le focus sur l'éditeur
-        get_workbench().get_editor_notebook().focus_set() 
+    def __init__(self, text_widget:EditorCodeViewText, parser:DocParser=DocParser()):
+        self._parser = parser 
+        self._text_widget = text_widget
+    
+    @abstractmethod
+    def can_generate(self, selected_lineno:int) -> bool:
+        pass
+    
+    @abstractmethod
+    def generate(self) -> None:
+        pass
     
-    def generate(self, signature:str, selected_lineno:int=None, text_widget:EditorCodeViewText=None) -> str:   
+    def _generate(self, signature:str, selected_lineno:int=None) -> str:   
         """Generate a docstring from a given signature (or prototype).
         
         Args:
             - signature(str): The signature for which the docstring will be generated.
             The signature should always be finished by a ":" caractere, otherwise the 
             docstring not will be generated. 
             - selected_lineno(int, Optional): This parameter is optional. It is the line number
@@ -151,34 +127,33 @@
             - NoFunctionSelectedToDocument: When a selected line don't corresponds to 
             a function declaration. 
             - DocGeneratorParserException: when the ast parser fails.
         """
         if signature is None: signature = ""
         
         # We should check that the line is a function declaration and that ends with ':' character. 
-        declaration_match = re.match(r"\s*(?P<id>def|class)\s*.*\s*:\s*$", signature)
+        declaration_match = re.match(self._SIGNATURE_REGEX, signature)
 
         if not declaration_match:
             raise NoFunctionSelectedToDocumentException("No signature is selected to document!\n")
         else:   
             id_signature = declaration_match.group("id") # c'est le tag <id> dans l'expression régulière
             
-            self._template = DocTemplateFactory.create_template(id_signature) \
-                                if not self._template else self._template
+            template:DocTemplate = DocTemplateFactory.create_template(id_signature) 
             
-            generated_temp = self.__get_generated_template(signature, selected_lineno)
+            generated_temp = self.__get_generated_template(template, signature, selected_lineno)
             
             indent = self.__compute_indent(signature)
             generated_doc = textwrap.indent(generated_temp, indent)
-            if text_widget:
+            if self._text_widget:
                 # c'est içi que la docstring est ajoutée à l'éditeur
-                text_widget.insert(str(selected_lineno + 1) + ".0", generated_doc)
+                self._text_widget.insert(str(selected_lineno + 1) + ".0", generated_doc)
             return generated_doc
-            
-    def __get_generated_template(self, signature:str, selected_lineno:int) -> str:
+    
+    def __get_generated_template(self, template:DocTemplate, signature:str, selected_lineno:int) -> str:
         """
         Creates a custom function with the given `signature` then parses this function and if the
         AST parser success so the docstring will be generated. If the AST parser fails, so the 
         reported exception will be raised.
 
         Args:
             signature (str): the signature for which the docstring will be generated.
@@ -201,15 +176,15 @@
         # -> see the doc
         self._parser.set_source(custom_func)
         node = self._parser.parse_source(selected_lineno)
         
         # Generate an event in Thonny with l1test/ThonnyLogsGenerator.log_doc_in_thonny
         log_doc_in_thonny(node)
         
-        return self._template.get_template(node)
+        return template.get_template(node)
 
     def __compute_indent(self, signature:str) -> int:
         """
         Get the indentation based on the whitespaces located in the given `signature`.
 
         Args:
             signature (str): a signature of a function
@@ -217,49 +192,189 @@
         Returns:
             int: returns the indentation based on the whitespaces located in the given `signature`.
         """
         space_match = re.search("^(\s+)", signature)
         python_indent = 4
         sig_indent = len(space_match.group(1)) if space_match else 0
         return " " * (sig_indent + python_indent)
+    
+    def _create_custom_body(self, signature:str):
+        signature = signature.strip()
+        # on supprime tous ce qu'il vient après les ":" dans la signature. Car, on veut juste la signature.
+        signature = re.sub(r"\s*(?P<id>def|class)(?P<signature>\s*.*\s*:)(?P<body>\s*.*)$", r"\g<id>\g<signature>", signature)
+        indent = " " * 4
+        return signature + "\n" + indent + "pass"
+    
+    def set_parser(self, parser: DocParser):
+        self._parser = parser
+        
+    def get_parser(self):
+        return self._parser
+    
+    def set_filename(self, filename):
+        self._parser.set_filename(filename)
+        
+    def set_text_widget(self, text_widget:EditorCodeViewText):
+        self._text_widget = text_widget
+    
+class AutoGenerationStrategy(DocGenerationStrategy):
+    def __init__(self, text_widget:EditorCodeViewText=None, parser=DocParser()):
+        super().__init__(text_widget, parser)
+        self.__selected_sig = None
+        self.__selected_lineno = None
+    
+    def can_generate(self, selected_lineno:int) -> bool:
+        selected_sig = self._text_widget.get(str(selected_lineno)+".0", str(selected_lineno+1)+".0").strip().strip("\n")
+        if selected_sig != "":
+            self.__selected_sig = selected_sig
+            self.__selected_lineno = selected_lineno
+        return self.__selected_sig != ""
+    
+    def generate(self):
+        return super()._generate(self.__selected_sig, self.__selected_lineno)
+        
+class ManualGenerationStrategy(DocGenerationStrategy):
+    _OUTLINER_REGEX = r"\s*(?P<type>def|class)[ ]+(?P<name>[\w]+)"
+    
+    def __init__(self, text_widget:EditorCodeViewText=None, parser=DocParser()):
+        super().__init__(text_widget, parser)
+        self.__nodes: List[SourceNode] = []
+        self.__selected_node = None
+    
+    def can_generate(self, selected_lineno:int) -> bool:
+        self.__nodes = self.__parse(self._text_widget.get("1.0", "end"))
+        self.__selected_node = next((node for node in self.__nodes if node.get_starting_lineno() <= selected_lineno <= node.get_ending_lineno()), None)
+        return self.__selected_node is not None
+    
+    def generate(self) -> str:
+        return super()._generate(self.__selected_node.get_signature(), self.__selected_node.get_starting_lineno())
+     
+    def __parse(self, source:str) :
+        """
+        Parses a source and returns a list of the outlined nodes. 
+        The outlined nodes are either a class or a function. For 
+        each outlined node an object of type `OutlinedNode` is built 
+        in which we store the type (class/function), the name and the lineno
+        of the outlined node.
+        """
+        current_node = None
+        lines = source.splitlines()
+        lineno = 1
+        last_non_empty_line = None
+        for line in lines:
+            match = re.match(self._OUTLINER_REGEX, line)
+            if match:
+                # If there was a previous outlined node, set its ending lineno.
+                if current_node:
+                    current_node.set_ending_lineno(last_non_empty_line or current_node.get_starting_lineno())
+                    yield current_node
+
+                # Create a new outlined node.
+                current_node = SourceNode(line, lineno, None)
+                last_non_empty_line = None  # Reset the last_non_empty_line for the new node.
+
+            elif line.strip():
+                last_non_empty_line = lineno  # Update last_non_empty_line.
+
+            lineno += 1
+
+        # Set the ending lineno for the last outlined node.
+        if current_node:
+            current_node.set_ending_lineno(last_non_empty_line or current_node.get_starting_lineno())
+            yield current_node
+    
+    def get_nodes(self):
+        return self.__nodes
+        
+class SourceNode():
+    """
+    This class represents an outlined node. An outlined node is either a class or a function.
+    """ 
+    def __init__(self, signature:str, starting_lineno:int, ending_lineno) -> None:
+        self.__signature = signature
+        self.__starting_lineno = starting_lineno
+        self.__ending_lineno = ending_lineno
+        
+    def get_starting_lineno(self):
+        return self.__starting_lineno  
+    
+    def get_ending_lineno(self):
+        return self.__ending_lineno
+    
+    def set_ending_lineno(self, ending_lineno):
+        self.__ending_lineno = ending_lineno
+        
+    def set_signature(self, signature):
+        self.__signature = signature
+    
+    def get_signature(self):
+        return self.__signature
+    
+    def __str__(self) -> str:
+        return f"signature: {self.__signature}, s_lineno: {self.__starting_lineno}, e_lineno: {self.__ending_lineno}" 
+    
+    
+class DocGenerator():
+    def __init__(self, strategy:DocGenerationStrategy=AutoGenerationStrategy()):
+        docstring_generator._doc_generator = self
+        self._has_exception = False 
+        self._strategy = strategy
+   
+    def run(self, selected_lineno:int, text_widget:EditorCodeViewText):
+        try:
+            self.__run(selected_lineno, text_widget)
+        except NoFunctionSelectedToDocumentException as e:
+            pass # do nothing
+        except FrontendException as e: # parsing error
+            self.set_has_exception(True)
+            self._show_error(str(e))
 
+    def __run(self, selected_lineno:int, text_widget:EditorCodeViewText):
+        self._strategy.set_text_widget(text_widget)
+        if self._strategy.can_generate(selected_lineno):
+            filename = get_workbench().get_editor_notebook().get_current_editor().get_filename()
+            if not filename:
+                filename = "<unknown>" 
+                    
+            self._strategy.set_filename(filename)
+            self._strategy.generate()   
+            
+            # après la génération (réussie) on vérifie si docgen avait rencontré une exception avant. Si oui, 
+            # on supprime l'exception de docgen (car elle a été déja montrée).
+            if get_l1test_runner().has_exception() or self.has_exception(): # si docgen avait lancé une exception avant
+                # si les deux ont lancé une exception, on affiche l'exception de docgen
+                if get_l1test_runner().has_exception() and self.has_exception(): 
+                    get_l1test_runner().clean_error_view()
+                    get_l1test_runner().get_reporter().get_error_view().hide_view()
+                    get_l1test_runner().get_reporter().get_treeview().show_view()
+                else:
+                    self._show_treeview()
+                
+                self.set_has_exception(False) # success
+    
     def _show_treeview(self):
         """
         Cleans the ErrorView and hides it. Retreives the Treeview and shows it.
         """
         get_l1test_runner().show_treeview()
     
     def _show_error(self, error_msg:str, error_title:str=CANNOT_GENERATE_THE_DOCSTRING):
         """
         Shows the error in the ErrorView if the docstring generator raises an exception.
         """
         l1test_runner = get_l1test_runner()
         if self.has_exception():
             l1test_runner.show_errors(exception_msg=error_msg, title=error_title)
             l1test_runner.get_reporter().get_error_view().show_view() 
-            l1test_runner.get_reporter().get_treeview().hide_view() 
-    
-    def _create_custom_body(self, signature:str):
-        signature = signature.strip()
-        indent = " " * 4
-        return  signature + "\n" + indent + "pass"    
-    
-    def set_parser(self, parser: DocParser):
-        self._parser = parser
-        
-    def get_parser(self):
-        return self._parser
-        
-    def set_template(self, template: DocTemplate):
-        self._template = template
-    
-    def get_template(self):
-        return self._template
-        
-    def set_filename(self, filename: str):
-        self._parser.set_filename(filename)
+            l1test_runner.get_reporter().get_treeview().hide_view()     
         
     def has_exception(self):
         return self._has_exception
     
     def set_has_exception(self, has_exception: bool):
-        self._has_exception = has_exception
+        self._has_exception = has_exception
+        
+    def get_strategy(self):
+        return self._strategy
+    
+    def set_strategy(self, strategy: DocGenerationStrategy):
+        self._strategy = strategy
```

### Comparing `bimbam-3.9.0/thonnycontrib/docstring_generator/doc_template.py` & `bimbam-4.0/thonnycontrib/docstring_generator/doc_template.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/environement_vars.py` & `bimbam-4.0/thonnycontrib/environement_vars.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/exceptions.py` & `bimbam-4.0/thonnycontrib/exceptions.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/l1test_configuration/l1test_options.py` & `bimbam-4.0/thonnycontrib/l1test_configuration/l1test_options.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/l1test_frontend/__init__.py` & `bimbam-4.0/thonnycontrib/l1test_frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/l1test_frontend/l1test_error_view.py` & `bimbam-4.0/thonnycontrib/l1test_frontend/l1test_error_view.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/l1test_frontend/l1test_outliner_menu.py` & `bimbam-4.0/thonnycontrib/l1test_frontend/l1test_outliner_menu.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/l1test_frontend/l1test_reporter.py` & `bimbam-4.0/thonnycontrib/l1test_frontend/l1test_reporter.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/l1test_frontend/l1test_runner.py` & `bimbam-4.0/thonnycontrib/l1test_frontend/l1test_runner.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/l1test_frontend/l1test_treeview.py` & `bimbam-4.0/thonnycontrib/l1test_frontend/l1test_treeview.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,95 +51,93 @@
 class L1TestTreeView(ttk.Frame):    
     def __init__(self, master=None):
         ttk.Frame.__init__(self, master, borderwidth=0, relief="flat")
         self.workbench = thonny.get_workbench()
         self._origin_l1doctests: List[L1DocTest] = dict()
         self._copy_l1doctests = self._origin_l1doctests.copy()
         
-        self._init_treeview()
-        
+        self.__init_treeview()
+        self.__init_workbench_bindings()
+    
+    def __init_workbench_bindings(self):
+        """
+        Binds the events to the workbench.
+        """
         # Le binding est censé augmenter/diminuer automatiquement la taille de la treeview
         self.workbench.bind("<Control-plus>", self.observe_font_changing, True)
         self.workbench.bind("<Control-minus>", self.observe_font_changing, True)
-                    
-    def _init_treeview(self):
+        self.workbench.bind(ALT_I, self.increase_row_height, True)
+        self.workbench.bind(ALT_D, self.decrease_row_height, True)
+        self.workbench.bind(ALT_F, self.update_font, True)
+        self.workbench.bind(ALT_U, self.expand_rows, True) 
+        self.workbench.bind(ALT_O, self.fold_rows, True)
+               
+    def __init_treeview(self):
         """
         Creates the treeview widget.
         """
         self.vert_scrollbar = ttk.Scrollbar(self, orient=tk.VERTICAL, style=scrollbar_style("Vertical"))
         self.vert_scrollbar.grid(row=0, column=1, sticky=tk.NSEW, rowspan=3)
-        
-        self.init_header(row=0, column=0)
-        
-        spacer = ttk.Frame(self, height=1)
-        spacer.grid(row=1, sticky="nsew")
-
+    
         self.treeview = ttk.Treeview(self,yscrollcommand=self.vert_scrollbar.set)
-        
         rows, columns = 2, 0
         self.treeview.grid(row=rows, column=columns, sticky=tk.NSEW)
         self.vert_scrollbar["command"] = self.treeview.yview
         self.columnconfigure(columns, weight=1)
         self.rowconfigure(rows, weight=1)
-        
-        # configure the only tree column
-        self.treeview.column("#0", anchor=tk.W, stretch=tk.YES)
-        
-        # self.tree.heading('#0', text='Item (type @ line)', anchor=tk.W)
+        self.treeview.column("#0", anchor=tk.W, stretch=tk.YES) # configure the only tree column
         self.treeview["show"] = ("tree",)
 
         for color_name, color in COLORS.items():
-            if color_name == "lightred":
+            if color_name == "lightred": # lightred is used for background (highlighting)
                 self.treeview.tag_configure(color_name, background=color)
             else:
                 self.treeview.tag_configure(color_name, foreground=color)
         
-        # définir un tag pour les test en exception: il faut les souligner (underline)
-        self.treeview.tag_configure("exception_as_link", foreground=COLORS["red"], 
-                                    font=tk_font.Font(underline=True, weight="normal", family=get_font_family_option(), size=get_font_size_option()))
-        self.treeview.tag_configure("exception_hovered", foreground=COLORS["red"], 
-                                    font=tk_font.Font(underline=True, 
-                                                    weight="bold", 
-                                                    family=get_font_family_option(), 
-                                                    size=get_font_size_option()))
+        # définir un tag pour les tests en exception: il faut les souligner (underline)
+        self.treeview.tag_configure(
+            "exception_as_link", 
+            foreground=COLORS["red"], 
+            font=tk_font.Font(underline=True, weight="normal", family=get_font_family_option(), size=get_font_size_option())
+        )
+        # définir un tag pour les tests en exception survolé: il faut les souligner (underline) et les mettre en gras (bold)
+        self.treeview.tag_configure(
+            "exception_hovered", 
+            foreground=COLORS["red"], 
+            font=tk_font.Font(underline=True, weight="bold", family=get_font_family_option(), size=get_font_size_option())
+        )
 
         # définir un style par défault pour la treeview
         self.style = ttk.Style()
         self.style_mapping = self.style.map('Treeview')
-        
         self.__update_tree_font(get_font_family_option(), get_font_size_option())
 
         # All the icons used in the treeview should be loaded here to keep thier references.
         # Otherwise, they will be garbage collected and the treeview will not show them.
         self.image_references = {flag.name: get_photoImage(flag.get_image()) for flag in L1DocTestFlag}
         self.image_references[PENDING_ICON] = get_photoImage(PENDING_ICON)
         self.image_references[ERROR_ICON] = get_photoImage(ERROR_ICON)
         self.image_references[RESTART_ICON] = get_photoImage(RESTART_ICON)
         self.image_references[FAILED_RED_CHIP] = get_photoImage(FAILED_RED_CHIP)
         self.image_references[EXCEPTION_RED_CHIP] = get_photoImage(EXCEPTION_RED_CHIP)
         self.image_references[SUCCESS_GREEN_CHIP] = get_photoImage(SUCCESS_GREEN_CHIP)
         
-        # add a menu to the treeview 
-        self.menu = tk.Menu(self.treeview, name="menu", tearoff=False)
-        
         self.treeview.tag_bind("clickable", "<<TreeviewSelect>>", self._on_select)
         self.treeview.tag_bind("nonClickable", "<<TreeviewSelect>>", self._remove_highlight_selection_effect)
         self.treeview.bind("<Motion>", self._on_hover_exception_test)
         self.treeview.bind("<Configure>", self.__wrap_tree_content) # Here we handle the motion event of the treeview 
         
-        self.workbench.bind(ALT_I, self.increase_row_height, True)
-        self.workbench.bind(ALT_D, self.decrease_row_height, True)
-        self.workbench.bind(ALT_F, self.update_font, True)
-        self.workbench.bind(ALT_U, self.expand_rows, True) 
-        self.workbench.bind(ALT_O, self.fold_rows, True)
+        # add a menu to the treeview 
+        self.menu = tk.Menu(self.treeview, name="menu", tearoff=False)        
+        self.init_header(row=0, column=0)
 
         self.__init_special_attributes()
         
     def __init_special_attributes(self):
-        """"
+        """
         Initializes the special attributes of the treeview.
         """
         self.__old_height = -1 # utilisé pour savoir si la hauteur de la treeview a changé
         self.__max_lines = 1 # le nombre de lignes du texte le plus long de la treeview
         self.__hovered_exception = None # l'exception test sur laquelle le curseur est en train de passer
      
     def _on_hover_exception_test(self, event):
```

### Comparing `bimbam-3.9.0/thonnycontrib/main_generator/main_generator.py` & `bimbam-4.0/thonnycontrib/main_generator/main_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         the __main__ will be generated. Defaults to "".
     """         
     def __init__(self, source=""):
         self._source = source
      
     def generate(self, text_widget:EditorCodeViewText=None, show_tooltip_info=True) -> str: 
         """
-        Generate the __main__ and insert it at the bottom of the editor widget.
+        Generate the __main__ and insert it at the bottom of the given `text_widget`.
 
         Args:
             text_widget (EditorCodeViewText, optional): The text widget to insert 
             the generated __main__ into. Set to `None` to not insert the generated 
             main function, this is useful for testing.
             
             show_tooltip_info (bool, optional): Set to True to show a message on a tooltip
```

### Comparing `bimbam-3.9.0/thonnycontrib/plugin_loader.py` & `bimbam-4.0/thonnycontrib/plugin_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from thonny.ui_utils import select_sequence
 from .docstring_generator.doc_generator import DocGenerator
 from .l1test_frontend.l1test_reporter import L1TestErrorView, L1TestTreeView
 from .main_generator.main_generator import MainGenerator
 from .exceptions import *
 from .properties import  ERROR_VIEW_LABEL, PLUGIN_NAME
 from .utils import (
+    assert_one_line_is_selected,
     get_focused_writable_text,
     get_selected_line, 
     get_image_path
 )
 from .l1test_configuration.l1test_options import *
 from .l1test_frontend import get_l1test_runner
 from .l1test_frontend import get_outliner
@@ -32,21 +33,25 @@
     Args:
         auto (bool):  Si True, alors la docstring sera générée automatiquement après un saut de ligne. 
         Sinon, la docstring sera générée quand le button `doc_generator` est cliqué.
         event (Any, optional): Si event est différent de None, alors un saut de ligne a été réalisé. 
         et donc la docstring sera générée automatiquement.
         Defaults to None.
     """
+    print("ed")
     if _writable_text_is_focused(): # on vérifie si la zone séléctionnée est une zone de l'éditeur
         text_widget = get_focused_writable_text()
         selected_line = get_selected_line(text_widget) 
-        docGenerator = get_doc_generator()  
+        docGenerator = get_doc_generator(auto)  
         docGenerator.run(selected_line - 1 if auto else selected_line, text_widget)
 
 def generate_main():
+    """
+    Generate the __main__ function.
+    """
     text_widget = get_focused_writable_text()
     main_generator = MainGenerator(text_widget.get("1.0", "end"))
     main_generator.generate(text_widget)
     del main_generator # destruction de l'objet en mémoire (for better performance)
     
 
 def _writable_text_is_focused():
@@ -84,15 +89,15 @@
     )
     
     # Création du bouton dans le menu 'Edit' pour lancer la génération de docstring
     get_workbench().add_command(command_id="doc_generator",
                                 menu_name="edit",  
                                 command_label="Generate a docstring",
                                 handler=partial(generate_docstring, auto=False), 
-                                tester=_writable_text_is_focused,
+                                tester=_writable_text_is_focused and assert_one_line_is_selected,
     )
      
     # Création du bouton dans le menu 'Edit' pour générer le main
     get_workbench().add_command(command_id="main_generator",
                                 menu_name="edit",  
                                 command_label="Generate a main",
                                 handler=generate_main,
```

### Comparing `bimbam-3.9.0/thonnycontrib/properties.py` & `bimbam-4.0/thonnycontrib/properties.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/tests/fixtures/workbench_mock.py` & `bimbam-4.0/thonnycontrib/tests/fixtures/workbench_mock.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/tests/tests_doc_generator.py` & `bimbam-4.0/thonnycontrib/tests/tests_doc_generator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 import unittest as ut
 from thonnycontrib.docstring_generator.doc_generator import *
 
+class MockDocGeneratorStrategy(DocGenerationStrategy):
+    def __init__(self):
+        super().__init__(text_widget=None)
+        
+    def can_generate(self) -> bool:
+        pass
+    
+    def generate(self) -> None:
+        pass
+    
 class TestDocGenerator(ut.TestCase):
     def setUp(self):
-        self.docGenerator = DocGenerator()
+        self.docGenerationStrategy = MockDocGeneratorStrategy()
     
     def tearDown(self) -> None:
-        del self.docGenerator
+        del self.docGenerationStrategy
     
     def test_doc_generator_when_ok(self):
         signature = "def func():"
-        generated = self.docGenerator.generate(signature)
+        generated = self.docGenerationStrategy._generate(signature)
         
         self.assertTrue(len(generated) > 0)
         
         expected_doc = \
 '''\
     """x_résumé_x
 
@@ -27,38 +37,38 @@
     """
 '''
         self.assertTrue(generated == expected_doc)
     
     def test_doc_generator_typing_support_case_1(self):
         arg_type, r_type = "str", "int"
         signature = "def func(a: %s) -> %s:" % (arg_type, r_type)
-        generated = self.docGenerator.generate(signature)
+        generated = self.docGenerationStrategy._generate(signature)
         
         self.assertTrue(len(generated) > 0)
         self.assertTrue(arg_type in generated)
         self.assertTrue(r_type in generated)
     
     def test_doc_generator_typing_support_case_2(self):
         arg_type = "str"
         signature = "def func(a: %s):" % arg_type
-        generated = self.docGenerator.generate(signature)
+        generated = self.docGenerationStrategy._generate(signature)
         
         self.assertTrue(len(generated) > 0)
         self.assertTrue(arg_type in generated)
     
     def test_doc_generator_when_syntax_error(self):
         signature = "def func):"
        
         with self.assertRaises(DocGeneratorParserException) as e:
-            self.docGenerator.generate(signature)
+            self.docGenerationStrategy._generate(signature)
         
         raised_exception = e.exception      
         self.assertTrue(SyntaxError.__name__ in str(raised_exception))
         
     def test_doc_generator_when_signature_doesnt_finish_with_colon(self):
         signature = "def func()"
         
         with self.assertRaises(NoFunctionSelectedToDocumentException) as e:
-            self.docGenerator.generate(signature)
+            self.docGenerationStrategy._generate(signature)
             
 if __name__ == '__main__':
     ut.main(verbosity=2)
```

### Comparing `bimbam-3.9.0/thonnycontrib/tests/tests_example_no_expected.py` & `bimbam-4.0/thonnycontrib/tests/tests_example_no_expected.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/tests/tests_example_with_exception.py` & `bimbam-4.0/thonnycontrib/tests/tests_example_with_exception.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/tests/tests_example_with_expected.py` & `bimbam-4.0/thonnycontrib/tests/tests_example_with_expected.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/tests/tests_l1TestRunner.py` & `bimbam-4.0/thonnycontrib/tests/tests_l1TestRunner.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/tests/tests_main_generator.py` & `bimbam-4.0/thonnycontrib/tests/tests_main_generator.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/tests/tests_test_finder.py` & `bimbam-4.0/thonnycontrib/tests/tests_test_finder.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/tests/tests_view.py` & `bimbam-4.0/thonnycontrib/tests/tests_view.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.9.0/thonnycontrib/utils.py` & `bimbam-4.0/thonnycontrib/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,14 +126,77 @@
         s.replace("\\", "\\\\")
          .replace("*", "\\*")
          .replace("`", "\\`")
          .replace("_", "\\_")
          .replace("..", "\\..")
     )
 
+import traceback
+import re
+from io import StringIO
+
+def get_last_exception(exc_info: tuple):
+    """
+    Formats exception information provided by ~exc_info~.
+    Extracts the last exception located in the last frame.
+
+    Args:
+        exc_info (tuple): The tuple must contain three elements:
+                        (type, value, traceback) as returned by sys.exc_info().
+
+    Returns:
+        str: Returns a string containing a traceback message for the given ~exc_info~.
+    """
+    exc_type, exc_val, exc_tb = exc_info
+
+    # Get a traceback message.
+    excout = StringIO()
+    traceback.print_exception(exc_type, exc_val, exc_tb, file=excout)
+
+    # Extract the last exception from the traceback frames.
+    content = excout.getvalue()
+    excout.close()
+    last_exception = extract_last_exception(content.rstrip("\n"))
+
+    # Remove multiple empty lines and preceding frames.
+    #last_exception = re.sub(r"\n+", "\n", last_exception)
+
+    return last_exception.strip()
+
+def extract_last_exception(traceback_content: str):
+    """
+    Extract the last exception from the traceback frames.
+
+    Args:
+        traceback_content (str): The returned traceback as a string.
+
+    Returns:
+        str: The lines representing the compilation error.
+    """
+   # Split the traceback into lines.
+    splitted = traceback_content.splitlines()
+
+    # Reverse the traceback frames and find the last frame containing the keyword "File."
+    last_frame_index = next((i for i, frame in enumerate(reversed(splitted)) if "File" in frame), 0)
+
+    # Get the last frame and its file name.
+    last_frame = splitted[-last_frame_index:]
+
+    # We don't want to display frames from the backend on thonny, as they are unnecessary and clutter the output.
+    frames_to_exclude = ["cpython_backend", os.path.join("thonny", "backend")]
+
+    for frame in last_frame:
+        if any(exclude in frame for exclude in frames_to_exclude):
+            last_frame_index = 0
+            break
+
+    # Get the error message from the last frame.
+    return "\n".join(last_frame[-last_frame_index:]).strip()
+
+
 def get_last_exception(exc_info:tuple):
     """
     Formats exception information provided by ~exc_info~.
     Extracts the last exception located in the last frame.
     
     Args:
         exc_info (tuple): The tuple must contain three elements: 
@@ -358,24 +421,23 @@
         int | tuple[int, int]: Returns (lineno, column). If `only_lineno` is True, 
         returns only lineno.
     """
     # A text is selected in the editor => can't tell the exact line of the test to run
     lineno, column = map(int, text_widget.index(tk.INSERT).split("."))
     return lineno if only_lineno else (lineno, column)
 
-def assert_one_line_is_selected(text: Text=None):
+def assert_one_line_is_selected() -> bool:
     """
-    Verify if only one line is selected, otherwise an exception is raised.
-    
-    Raises:
-        CannotSelectSeveralLines: when several lines are selected.
+    Returns True if only one line is selected, otherwise an exception is raised.
     """
-    text = get_focused_writable_text() if not text else text 
-    if len(text.tag_ranges("sel")) > 0:
-        raise CannotSelectSeveralLines("Several lines are selected !\nSelect only one line.")
+    text = get_focused_writable_text()
+    print("selected = ", text.tag_ranges("sel") if text else None)
+    if text :
+        return len(text.tag_ranges("sel")) == 0
+    return False
         
 def add_random_suffix(word):
     """Add a random suffix to the given word.
      
     The suffix is added in the following format 'word_suffix'. An underscore separates the two words.
     The suffix is assumed to be long(more than 9 caracters).
```

