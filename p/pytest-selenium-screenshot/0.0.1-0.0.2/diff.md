# Comparing `tmp/pytest_selenium_screenshot-0.0.1.tar.gz` & `tmp/pytest_selenium_screenshot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_selenium_screenshot-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pytest_selenium_screenshot-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest_selenium_screenshot-0.0.1.tar` & `pytest_selenium_screenshot-0.0.2.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0       29 2023-07-29 17:39:00.207580 pytest_selenium_screenshot-0.0.1/README.md
--rw-r--r--   0        0        0      475 2023-07-29 19:47:08.428758 pytest_selenium_screenshot-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-29 19:13:20.657092 pytest_selenium_screenshot-0.0.1/src/pytest_selenium_screenshot/__init__.py
--rw-r--r--   0        0        0      380 1970-01-01 00:00:00.000000 pytest_selenium_screenshot-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       29 2023-07-29 17:39:00.207580 pytest_selenium_screenshot-0.0.2/README.md
+-rw-r--r--   0        0        0      688 2023-07-30 05:59:38.006265 pytest_selenium_screenshot-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-29 19:13:20.657092 pytest_selenium_screenshot-0.0.2/src/pytest_selenium_screenshot/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 05:53:33.967578 pytest_selenium_screenshot-0.0.2/src/pytest_selenium_screenshot/plugin.py
+-rw-r--r--   0        0        0      522 1970-01-01 00:00:00.000000 pytest_selenium_screenshot-0.0.2/PKG-INFO
```

