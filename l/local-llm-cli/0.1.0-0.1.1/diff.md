# Comparing `tmp/local_llm_cli-0.1.0.tar.gz` & `tmp/local_llm_cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "local_llm_cli-0.1.0.tar", last modified: Sun Jul 30 05:24:17 2023, max compression
+gzip compressed data, was "local_llm_cli-0.1.1.tar", last modified: Sun Jul 30 05:30:23 2023, max compression
```

## Comparing `local_llm_cli-0.1.0.tar` & `local_llm_cli-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 05:24:16.998892 local_llm_cli-0.1.0/
--rw-rw-rw-   0        0        0      321 2023-07-30 05:24:16.997895 local_llm_cli-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-30 05:24:16.977840 local_llm_cli-0.1.0/local_llm_cli/
--rw-rw-rw-   0        0        0       41 2023-07-30 05:19:47.000000 local_llm_cli-0.1.0/local_llm_cli/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 05:24:16.995894 local_llm_cli-0.1.0/local_llm_cli/converse/
--rw-rw-rw-   0        0        0       35 2023-07-30 05:19:30.000000 local_llm_cli-0.1.0/local_llm_cli/converse/__init__.py
--rw-rw-rw-   0        0        0      742 2023-07-30 05:21:42.000000 local_llm_cli-0.1.0/local_llm_cli/converse/chat.py
-drwxrwxrwx   0        0        0        0 2023-07-30 05:24:16.992361 local_llm_cli-0.1.0/local_llm_cli.egg-info/
--rw-rw-rw-   0        0        0      321 2023-07-30 05:24:16.000000 local_llm_cli-0.1.0/local_llm_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-07-30 05:24:16.000000 local_llm_cli-0.1.0/local_llm_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 05:24:16.000000 local_llm_cli-0.1.0/local_llm_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-30 05:24:16.000000 local_llm_cli-0.1.0/local_llm_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-30 05:24:16.000000 local_llm_cli-0.1.0/local_llm_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-30 05:24:16.999888 local_llm_cli-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      493 2023-07-30 05:22:47.000000 local_llm_cli-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 05:30:23.346207 local_llm_cli-0.1.1/
+-rw-rw-rw-   0        0        0      321 2023-07-30 05:30:23.345207 local_llm_cli-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1700 2023-07-30 05:30:06.000000 local_llm_cli-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 05:30:23.323188 local_llm_cli-0.1.1/local_llm_cli/
+-rw-rw-rw-   0        0        0       41 2023-07-30 05:19:47.000000 local_llm_cli-0.1.1/local_llm_cli/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 05:30:23.343188 local_llm_cli-0.1.1/local_llm_cli/converse/
+-rw-rw-rw-   0        0        0       35 2023-07-30 05:19:30.000000 local_llm_cli-0.1.1/local_llm_cli/converse/__init__.py
+-rw-rw-rw-   0        0        0      742 2023-07-30 05:21:42.000000 local_llm_cli-0.1.1/local_llm_cli/converse/chat.py
+drwxrwxrwx   0        0        0        0 2023-07-30 05:30:23.338189 local_llm_cli-0.1.1/local_llm_cli.egg-info/
+-rw-rw-rw-   0        0        0      321 2023-07-30 05:30:22.000000 local_llm_cli-0.1.1/local_llm_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-07-30 05:30:23.000000 local_llm_cli-0.1.1/local_llm_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 05:30:22.000000 local_llm_cli-0.1.1/local_llm_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-30 05:30:22.000000 local_llm_cli-0.1.1/local_llm_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-30 05:30:22.000000 local_llm_cli-0.1.1/local_llm_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 05:30:23.346207 local_llm_cli-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      493 2023-07-30 05:28:18.000000 local_llm_cli-0.1.1/setup.py
```

### Comparing `local_llm_cli-0.1.0/local_llm_cli/converse/chat.py` & `local_llm_cli-0.1.1/local_llm_cli/converse/chat.py`

 * *Files identical despite different names*

