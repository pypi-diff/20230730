# Comparing `tmp/geomancy-0.9.3.tar.gz` & `tmp/geomancy-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomancy-0.9.3.tar", last modified: Sat Jul 29 16:59:32 2023, max compression
+gzip compressed data, was "geomancy-0.9.4.tar", last modified: Sun Jul 30 02:41:10 2023, max compression
```

## Comparing `geomancy-0.9.3.tar` & `geomancy-0.9.4.tar`

### file list

```diff
@@ -1,86 +1,88 @@
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.052968 geomancy-0.9.3/
--rw-r--r--   0 jlorieau   (501) staff       (20)      345 2023-07-26 14:41:25.000000 geomancy-0.9.3/.editorconfig
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.026954 geomancy-0.9.3/.github/
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.033491 geomancy-0.9.3/.github/workflows/
--rw-r--r--   0 jlorieau   (501) staff       (20)      760 2023-07-29 16:55:41.000000 geomancy-0.9.3/.github/workflows/tests.yml
--rw-r--r--   0 jlorieau   (501) staff       (20)     1780 2023-07-24 22:25:03.000000 geomancy-0.9.3/.gitignore
--rw-r--r--   0 jlorieau   (501) staff       (20)      233 2023-07-25 16:40:32.000000 geomancy-0.9.3/.readthedocs.yaml
--rw-r--r--   0 jlorieau   (501) staff       (20)     1023 2023-07-26 00:50:48.000000 geomancy-0.9.3/LICENSE
--rw-r--r--   0 jlorieau   (501) staff       (20)     6029 2023-07-29 16:59:32.052605 geomancy-0.9.3/PKG-INFO
--rw-r--r--   0 jlorieau   (501) staff       (20)     4849 2023-07-29 16:55:41.000000 geomancy-0.9.3/README.md
--rw-r--r--   0 jlorieau   (501) staff       (20)     1711 2023-07-26 14:41:25.000000 geomancy-0.9.3/Taskfile.yaml
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.033913 geomancy-0.9.3/changelog/
--rw-r--r--   0 jlorieau   (501) staff       (20)      310 2023-07-25 18:53:41.000000 geomancy-0.9.3/changelog/changelog_template.jinja
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.035364 geomancy-0.9.3/docs/
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.036396 geomancy-0.9.3/docs/_static/
--rw-r--r--   0 jlorieau   (501) staff       (20)      466 2023-07-26 14:41:25.000000 geomancy-0.9.3/docs/_static/custom.css
--rw-r--r--   0 jlorieau   (501) staff       (20)    49829 2023-07-25 15:23:09.000000 geomancy-0.9.3/docs/_static/geomancy_logo.png
--rw-r--r--   0 jlorieau   (501) staff       (20)     6346 2023-07-28 19:38:01.000000 geomancy-0.9.3/docs/_static/geomancy_logo.svg
--rw-r--r--   0 jlorieau   (501) staff       (20)     3205 2023-07-29 16:57:58.000000 geomancy-0.9.3/docs/changelog.md
--rw-r--r--   0 jlorieau   (501) staff       (20)     2121 2023-07-29 16:55:41.000000 geomancy-0.9.3/docs/conf.py
--rw-r--r--   0 jlorieau   (501) staff       (20)      651 2023-07-28 19:38:01.000000 geomancy-0.9.3/docs/index.md
--rw-r--r--   0 jlorieau   (501) staff       (20)      121 2023-07-25 15:07:00.000000 geomancy-0.9.3/docs/quickstart.md
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.037336 geomancy-0.9.3/docs/usage/
--rw-r--r--   0 jlorieau   (501) staff       (20)     8813 2023-07-29 16:55:41.000000 geomancy-0.9.3/docs/usage/cmd_checks.md
--rw-r--r--   0 jlorieau   (501) staff       (20)     1437 2023-07-28 19:38:01.000000 geomancy-0.9.3/docs/usage/cmd_run.md
--rw-r--r--   0 jlorieau   (501) staff       (20)    11313 2023-07-29 16:55:41.000000 geomancy-0.9.3/docs/usage/format.md
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.038435 geomancy-0.9.3/examples/
--rw-r--r--   0 jlorieau   (501) staff       (20)     1483 2023-07-29 16:55:41.000000 geomancy-0.9.3/examples/geomancy.toml
--rw-r--r--   0 jlorieau   (501) staff       (20)     1278 2023-07-29 16:55:41.000000 geomancy-0.9.3/examples/geomancy.yaml
--rw-r--r--   0 jlorieau   (501) staff       (20)      272 2023-07-26 14:41:25.000000 geomancy-0.9.3/examples/geomancy_flat.yaml
--rw-r--r--   0 jlorieau   (501) staff       (20)      510 2023-07-29 16:55:41.000000 geomancy-0.9.3/examples/pyproject.toml
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.039006 geomancy-0.9.3/geomancy/
--rw-r--r--   0 jlorieau   (501) staff       (20)       59 2023-07-23 20:49:04.000000 geomancy-0.9.3/geomancy/__description__.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)      485 2023-07-29 16:59:23.000000 geomancy-0.9.3/geomancy/__init__.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.044252 geomancy-0.9.3/geomancy/checks/
--rw-r--r--   0 jlorieau   (501) staff       (20)      345 2023-07-24 12:18:52.000000 geomancy-0.9.3/geomancy/checks/__init__.py
--rw-r--r--   0 jlorieau   (501) staff       (20)    11987 2023-07-29 16:55:41.000000 geomancy-0.9.3/geomancy/checks/base.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     1696 2023-07-29 16:55:41.000000 geomancy-0.9.3/geomancy/checks/env.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     2426 2023-07-24 15:55:52.000000 geomancy-0.9.3/geomancy/checks/exec.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     1549 2023-07-23 16:57:23.000000 geomancy-0.9.3/geomancy/checks/path.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     3422 2023-07-29 02:10:42.000000 geomancy-0.9.3/geomancy/checks/python.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     5242 2023-07-29 16:55:41.000000 geomancy-0.9.3/geomancy/checks/utils.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     2336 2023-07-24 15:55:27.000000 geomancy-0.9.3/geomancy/checks/version.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.044912 geomancy-0.9.3/geomancy/cli/
--rw-r--r--   0 jlorieau   (501) staff       (20)       42 2023-07-27 16:55:31.000000 geomancy-0.9.3/geomancy/cli/__init__.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     6640 2023-07-29 16:55:41.000000 geomancy-0.9.3/geomancy/cli/term.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.045648 geomancy-0.9.3/geomancy/config/
--rw-r--r--   0 jlorieau   (501) staff       (20)      137 2023-07-22 15:14:01.000000 geomancy-0.9.3/geomancy/config/__init__.py
--rw-r--r--   0 jlorieau   (501) staff       (20)    13410 2023-07-28 19:38:01.000000 geomancy-0.9.3/geomancy/config/config.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.047940 geomancy-0.9.3/geomancy/entrypoints/
--rw-r--r--   0 jlorieau   (501) staff       (20)       47 2023-07-28 19:38:01.000000 geomancy-0.9.3/geomancy/entrypoints/__init__.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     3423 2023-07-29 16:55:41.000000 geomancy-0.9.3/geomancy/entrypoints/check.py
--rw-r--r--   0 jlorieau   (501) staff       (20)      546 2023-07-28 19:38:01.000000 geomancy-0.9.3/geomancy/entrypoints/config.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     4136 2023-07-28 19:38:01.000000 geomancy-0.9.3/geomancy/entrypoints/environment.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     1427 2023-07-28 19:38:01.000000 geomancy-0.9.3/geomancy/entrypoints/geo.py
--rw-r--r--   0 jlorieau   (501) staff       (20)      487 2023-07-28 19:38:01.000000 geomancy-0.9.3/geomancy/entrypoints/run.py
--rw-r--r--   0 jlorieau   (501) staff       (20)      904 2023-07-28 19:38:01.000000 geomancy-0.9.3/geomancy/entrypoints/utils.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.048606 geomancy-0.9.3/geomancy/environment/
--rw-r--r--   0 jlorieau   (501) staff       (20)      164 2023-07-29 16:55:41.000000 geomancy-0.9.3/geomancy/environment/__init__.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     8587 2023-07-29 16:55:41.000000 geomancy-0.9.3/geomancy/environment/dotenv.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.041086 geomancy-0.9.3/geomancy.egg-info/
--rw-r--r--   0 jlorieau   (501) staff       (20)     6029 2023-07-29 16:59:31.000000 geomancy-0.9.3/geomancy.egg-info/PKG-INFO
--rw-r--r--   0 jlorieau   (501) staff       (20)     1579 2023-07-29 16:59:32.000000 geomancy-0.9.3/geomancy.egg-info/SOURCES.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)        1 2023-07-29 16:59:31.000000 geomancy-0.9.3/geomancy.egg-info/dependency_links.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)       53 2023-07-29 16:59:31.000000 geomancy-0.9.3/geomancy.egg-info/entry_points.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)      167 2023-07-29 16:59:31.000000 geomancy-0.9.3/geomancy.egg-info/requires.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)        9 2023-07-29 16:59:31.000000 geomancy-0.9.3/geomancy.egg-info/top_level.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)     2836 2023-07-28 19:38:01.000000 geomancy-0.9.3/pyproject.toml
--rw-r--r--   0 jlorieau   (501) staff       (20)       38 2023-07-29 16:59:32.053070 geomancy-0.9.3/setup.cfg
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.048886 geomancy-0.9.3/tests/
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.050343 geomancy-0.9.3/tests/checks/
--rw-r--r--   0 jlorieau   (501) staff       (20)     5181 2023-07-29 16:55:41.000000 geomancy-0.9.3/tests/checks/test_base.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     2690 2023-07-29 16:55:41.000000 geomancy-0.9.3/tests/checks/test_env.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     1074 2023-07-29 02:10:42.000000 geomancy-0.9.3/tests/checks/test_exec.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     2193 2023-07-29 16:55:41.000000 geomancy-0.9.3/tests/checks/test_path.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     2442 2023-07-24 15:31:44.000000 geomancy-0.9.3/tests/checks/test_python.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.050960 geomancy-0.9.3/tests/config/
--rw-r--r--   0 jlorieau   (501) staff       (20)       73 2023-07-20 16:27:03.000000 geomancy-0.9.3/tests/config/config1.toml
--rw-r--r--   0 jlorieau   (501) staff       (20)     7826 2023-07-28 19:38:01.000000 geomancy-0.9.3/tests/config/test_config.py
--rw-r--r--   0 jlorieau   (501) staff       (20)      524 2023-07-25 04:11:09.000000 geomancy-0.9.3/tests/conftest.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.051367 geomancy-0.9.3/tests/data/
--rw-r--r--   0 jlorieau   (501) staff       (20)      159 2023-07-25 01:20:06.000000 geomancy-0.9.3/tests/data/test.env
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.051640 geomancy-0.9.3/tests/entrypoints/
--rw-r--r--   0 jlorieau   (501) staff       (20)     4417 2023-07-28 19:38:01.000000 geomancy-0.9.3/tests/entrypoints/test_geo.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-29 16:59:32.051905 geomancy-0.9.3/tests/environment/
--rw-r--r--   0 jlorieau   (501) staff       (20)     6043 2023-07-29 16:55:41.000000 geomancy-0.9.3/tests/environment/test_dotenv.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.367814 geomancy-0.9.4/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      345 2023-07-26 14:41:25.000000 geomancy-0.9.4/.editorconfig
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.342615 geomancy-0.9.4/.github/
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.350307 geomancy-0.9.4/.github/workflows/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      757 2023-07-30 02:36:10.000000 geomancy-0.9.4/.github/workflows/tests.yml
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1780 2023-07-24 22:25:03.000000 geomancy-0.9.4/.gitignore
+-rw-r--r--   0 jlorieau   (501) staff       (20)      233 2023-07-25 16:40:32.000000 geomancy-0.9.4/.readthedocs.yaml
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1023 2023-07-26 00:50:48.000000 geomancy-0.9.4/LICENSE
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6318 2023-07-30 02:41:10.367471 geomancy-0.9.4/PKG-INFO
+-rw-r--r--   0 jlorieau   (501) staff       (20)     5138 2023-07-30 02:40:03.000000 geomancy-0.9.4/README.md
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1711 2023-07-26 14:41:25.000000 geomancy-0.9.4/Taskfile.yaml
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.350979 geomancy-0.9.4/changelog/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      310 2023-07-25 18:53:41.000000 geomancy-0.9.4/changelog/changelog_template.jinja
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.352235 geomancy-0.9.4/docs/
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.353223 geomancy-0.9.4/docs/_static/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      466 2023-07-26 14:41:25.000000 geomancy-0.9.4/docs/_static/custom.css
+-rw-r--r--   0 jlorieau   (501) staff       (20)    49829 2023-07-25 15:23:09.000000 geomancy-0.9.4/docs/_static/geomancy_logo.png
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6346 2023-07-28 19:38:01.000000 geomancy-0.9.4/docs/_static/geomancy_logo.svg
+-rw-r--r--   0 jlorieau   (501) staff       (20)     3543 2023-07-30 02:36:10.000000 geomancy-0.9.4/docs/changelog.md
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2121 2023-07-29 16:55:41.000000 geomancy-0.9.4/docs/conf.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)      651 2023-07-28 19:38:01.000000 geomancy-0.9.4/docs/index.md
+-rw-r--r--   0 jlorieau   (501) staff       (20)      121 2023-07-25 15:07:00.000000 geomancy-0.9.4/docs/quickstart.md
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.354119 geomancy-0.9.4/docs/usage/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     8813 2023-07-29 16:55:41.000000 geomancy-0.9.4/docs/usage/cmd_checks.md
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1437 2023-07-28 19:38:01.000000 geomancy-0.9.4/docs/usage/cmd_run.md
+-rw-r--r--   0 jlorieau   (501) staff       (20)    13139 2023-07-30 02:36:10.000000 geomancy-0.9.4/docs/usage/format.md
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.355260 geomancy-0.9.4/examples/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1763 2023-07-30 02:36:10.000000 geomancy-0.9.4/examples/geomancy.toml
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1883 2023-07-30 02:36:10.000000 geomancy-0.9.4/examples/geomancy.yaml
+-rw-r--r--   0 jlorieau   (501) staff       (20)      272 2023-07-26 14:41:25.000000 geomancy-0.9.4/examples/geomancy_flat.yaml
+-rw-r--r--   0 jlorieau   (501) staff       (20)      369 2023-07-30 02:36:10.000000 geomancy-0.9.4/examples/pyproject.toml
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.355823 geomancy-0.9.4/geomancy/
+-rw-r--r--   0 jlorieau   (501) staff       (20)       59 2023-07-23 20:49:04.000000 geomancy-0.9.4/geomancy/__description__.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)      485 2023-07-30 02:40:59.000000 geomancy-0.9.4/geomancy/__init__.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.359986 geomancy-0.9.4/geomancy/checks/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      388 2023-07-30 02:36:10.000000 geomancy-0.9.4/geomancy/checks/__init__.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)    12445 2023-07-30 02:36:10.000000 geomancy-0.9.4/geomancy/checks/base.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1696 2023-07-29 16:55:41.000000 geomancy-0.9.4/geomancy/checks/env.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2426 2023-07-24 15:55:52.000000 geomancy-0.9.4/geomancy/checks/exec.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1549 2023-07-23 16:57:23.000000 geomancy-0.9.4/geomancy/checks/path.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2359 2023-07-30 02:36:10.000000 geomancy-0.9.4/geomancy/checks/platform.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1378 2023-07-30 02:36:10.000000 geomancy-0.9.4/geomancy/checks/python.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     5242 2023-07-29 16:55:41.000000 geomancy-0.9.4/geomancy/checks/utils.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2381 2023-07-30 02:36:10.000000 geomancy-0.9.4/geomancy/checks/version.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.360535 geomancy-0.9.4/geomancy/cli/
+-rw-r--r--   0 jlorieau   (501) staff       (20)       42 2023-07-27 16:55:31.000000 geomancy-0.9.4/geomancy/cli/__init__.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6640 2023-07-29 16:55:41.000000 geomancy-0.9.4/geomancy/cli/term.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.361091 geomancy-0.9.4/geomancy/config/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      137 2023-07-22 15:14:01.000000 geomancy-0.9.4/geomancy/config/__init__.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)    13410 2023-07-28 19:38:01.000000 geomancy-0.9.4/geomancy/config/config.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.363009 geomancy-0.9.4/geomancy/entrypoints/
+-rw-r--r--   0 jlorieau   (501) staff       (20)       47 2023-07-28 19:38:01.000000 geomancy-0.9.4/geomancy/entrypoints/__init__.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     3423 2023-07-29 16:55:41.000000 geomancy-0.9.4/geomancy/entrypoints/check.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)      546 2023-07-28 19:38:01.000000 geomancy-0.9.4/geomancy/entrypoints/config.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     4136 2023-07-28 19:38:01.000000 geomancy-0.9.4/geomancy/entrypoints/environment.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1427 2023-07-28 19:38:01.000000 geomancy-0.9.4/geomancy/entrypoints/geo.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)      487 2023-07-28 19:38:01.000000 geomancy-0.9.4/geomancy/entrypoints/run.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)      904 2023-07-28 19:38:01.000000 geomancy-0.9.4/geomancy/entrypoints/utils.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.363570 geomancy-0.9.4/geomancy/environment/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      164 2023-07-29 16:55:41.000000 geomancy-0.9.4/geomancy/environment/__init__.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     8587 2023-07-29 16:55:41.000000 geomancy-0.9.4/geomancy/environment/dotenv.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.357527 geomancy-0.9.4/geomancy.egg-info/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6318 2023-07-30 02:41:10.000000 geomancy-0.9.4/geomancy.egg-info/PKG-INFO
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1637 2023-07-30 02:41:10.000000 geomancy-0.9.4/geomancy.egg-info/SOURCES.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)        1 2023-07-30 02:41:10.000000 geomancy-0.9.4/geomancy.egg-info/dependency_links.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)       53 2023-07-30 02:41:10.000000 geomancy-0.9.4/geomancy.egg-info/entry_points.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)      167 2023-07-30 02:41:10.000000 geomancy-0.9.4/geomancy.egg-info/requires.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)        9 2023-07-30 02:41:10.000000 geomancy-0.9.4/geomancy.egg-info/top_level.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2836 2023-07-28 19:38:01.000000 geomancy-0.9.4/pyproject.toml
+-rw-r--r--   0 jlorieau   (501) staff       (20)       38 2023-07-30 02:41:10.367903 geomancy-0.9.4/setup.cfg
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.363848 geomancy-0.9.4/tests/
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.365505 geomancy-0.9.4/tests/checks/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     5181 2023-07-29 16:55:41.000000 geomancy-0.9.4/tests/checks/test_base.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2690 2023-07-29 16:55:41.000000 geomancy-0.9.4/tests/checks/test_env.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1074 2023-07-29 02:10:42.000000 geomancy-0.9.4/tests/checks/test_exec.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2193 2023-07-29 16:55:41.000000 geomancy-0.9.4/tests/checks/test_path.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)      612 2023-07-30 02:36:10.000000 geomancy-0.9.4/tests/checks/test_platform.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)      936 2023-07-30 02:36:10.000000 geomancy-0.9.4/tests/checks/test_python.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.366057 geomancy-0.9.4/tests/config/
+-rw-r--r--   0 jlorieau   (501) staff       (20)       73 2023-07-20 16:27:03.000000 geomancy-0.9.4/tests/config/config1.toml
+-rw-r--r--   0 jlorieau   (501) staff       (20)     7826 2023-07-28 19:38:01.000000 geomancy-0.9.4/tests/config/test_config.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)      524 2023-07-25 04:11:09.000000 geomancy-0.9.4/tests/conftest.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.366328 geomancy-0.9.4/tests/data/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      159 2023-07-25 01:20:06.000000 geomancy-0.9.4/tests/data/test.env
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.366602 geomancy-0.9.4/tests/entrypoints/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     4417 2023-07-28 19:38:01.000000 geomancy-0.9.4/tests/entrypoints/test_geo.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-30 02:41:10.366882 geomancy-0.9.4/tests/environment/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6043 2023-07-29 16:55:41.000000 geomancy-0.9.4/tests/environment/test_dotenv.py
```

### Comparing `geomancy-0.9.3/.github/workflows/tests.yml` & `geomancy-0.9.4/.github/workflows/tests.yml`

 * *Files 18% similar despite different names*

```diff
@@ -24,11 +24,11 @@
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          python -m pip install -e .[dev]
+          python -m pip install .[dev]
       - name: Test with pytest
         run: |
           pytest --log-level=DEBUG
```

### Comparing `geomancy-0.9.3/.gitignore` & `geomancy-0.9.4/.gitignore`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.3/LICENSE` & `geomancy-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.3/PKG-INFO` & `geomancy-0.9.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomancy
-Version: 0.9.3
+Version: 0.9.4
 Summary: Geomancy validates deployment and development environments
 Author: Justin Lorieau
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
@@ -46,15 +46,17 @@
 executables, the state of external dependencies, like LaTeX packages, or cloud
 resources, or for checking environments that use the
 [12-factor](http://12factor.net/) principles.
 <!-- end intro -->
 
 ## Quickstart
 <!-- start quickstart -->
-1. Create a ``.geomancy.yaml`` file with checks.
+1. Create a ``.geomancy.yaml`` file with checks. See
+   [examples/geomancy.yaml](https://github.com/jlorieau/geomancy/blob/main/examples/geomancy.yaml)
+   for an example of all checks.
 
     ```yaml
     checks:
       Environment:
         desc: Check environment variables common to all development environments
 
         Username:
@@ -103,27 +105,29 @@
     ``.geomancy.toml``, ``geomancy.toml`` and ``pyproject.toml``.)
 <!-- end quickstart -->
 
 ## Features
 <!-- start features -->
 Geomancy checks include:
 
+- __Operating systems__ meet the minimum required versions
+  ([checkOS](https://geomancy.readthedocs.io/en/latest/usage/format.html#checkplatform))
 - __Environment variables__ are properly set and, optionally,
   check that they have valid values with regular expressions
-  ([checkEnv](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkenv))
+  ([checkEnv](https://geomancy.readthedocs.io/en/latest/usage/format.html#checkenv))
 - __Paths__ exist and whether they're files or directories
-  ([checkPath](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkpath))
+  ([checkPath](https://geomancy.readthedocs.io/en/latest/usage/format.html#checkpath))
 - __Executables__ are available and, optionally, have the minimum or correct
   versions
-  ([checkExec](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkexec))
+  ([checkExec](https://geomancy.readthedocs.io/en/latest/usage/format.html#checkexec))
 - __Python packages__ are available and, optionally, have the minimum or
   correct versions
-  ([checkPythonPkg](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkpythonpkg))
+  ([checkPythonPkg](https://geomancy.readthedocs.io/en/latest/usage/format.html#checkpythonpkg))
 - __Group checks__ to nested groups of checks with conditional (all or any) pass
-  criteria ([groups of checks](https://geomancy.readthedocs.io/en/latest/usage/index.html#check-groups))
+  criteria ([groups of checks](https://geomancy.readthedocs.io/en/latest/usage/format.html#check-groups))
 
 Additionally, geomancy can:
 
 - __Load environment files__ for
   [checks](https://geomancy.readthedocs.io/en/latest/usage/cmd_checks.html#environment-files)
   or for [running](https://geomancy.readthedocs.io/en/latest/usage/cmd_run.html#running-environments)
   shell commands
```

### Comparing `geomancy-0.9.3/README.md` & `geomancy-0.9.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 executables, the state of external dependencies, like LaTeX packages, or cloud
 resources, or for checking environments that use the
 [12-factor](http://12factor.net/) principles.
 <!-- end intro -->
 
 ## Quickstart
 <!-- start quickstart -->
-1. Create a ``.geomancy.yaml`` file with checks.
+1. Create a ``.geomancy.yaml`` file with checks. See
+   [examples/geomancy.yaml](https://github.com/jlorieau/geomancy/blob/main/examples/geomancy.yaml)
+   for an example of all checks.
 
     ```yaml
     checks:
       Environment:
         desc: Check environment variables common to all development environments
 
         Username:
@@ -74,27 +76,29 @@
     ``.geomancy.toml``, ``geomancy.toml`` and ``pyproject.toml``.)
 <!-- end quickstart -->
 
 ## Features
 <!-- start features -->
 Geomancy checks include:
 
+- __Operating systems__ meet the minimum required versions
+  ([checkOS](https://geomancy.readthedocs.io/en/latest/usage/format.html#checkplatform))
 - __Environment variables__ are properly set and, optionally,
   check that they have valid values with regular expressions
-  ([checkEnv](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkenv))
+  ([checkEnv](https://geomancy.readthedocs.io/en/latest/usage/format.html#checkenv))
 - __Paths__ exist and whether they're files or directories
-  ([checkPath](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkpath))
+  ([checkPath](https://geomancy.readthedocs.io/en/latest/usage/format.html#checkpath))
 - __Executables__ are available and, optionally, have the minimum or correct
   versions
-  ([checkExec](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkexec))
+  ([checkExec](https://geomancy.readthedocs.io/en/latest/usage/format.html#checkexec))
 - __Python packages__ are available and, optionally, have the minimum or
   correct versions
-  ([checkPythonPkg](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkpythonpkg))
+  ([checkPythonPkg](https://geomancy.readthedocs.io/en/latest/usage/format.html#checkpythonpkg))
 - __Group checks__ to nested groups of checks with conditional (all or any) pass
-  criteria ([groups of checks](https://geomancy.readthedocs.io/en/latest/usage/index.html#check-groups))
+  criteria ([groups of checks](https://geomancy.readthedocs.io/en/latest/usage/format.html#check-groups))
 
 Additionally, geomancy can:
 
 - __Load environment files__ for
   [checks](https://geomancy.readthedocs.io/en/latest/usage/cmd_checks.html#environment-files)
   or for [running](https://geomancy.readthedocs.io/en/latest/usage/cmd_run.html#running-environments)
   shell commands
```

### Comparing `geomancy-0.9.3/Taskfile.yaml` & `geomancy-0.9.4/Taskfile.yaml`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.3/docs/_static/geomancy_logo.png` & `geomancy-0.9.4/docs/_static/geomancy_logo.png`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.3/docs/_static/geomancy_logo.svg` & `geomancy-0.9.4/docs/_static/geomancy_logo.svg`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.3/docs/changelog.md` & `geomancy-0.9.4/docs/changelog.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,27 @@
 Changes in API will only be introduced in major versions with notes in the
 deprecations section.
 
 % Do not edit below this line, as the changelog is managed by towncrier
 
 <!-- towncrier release notes start -->
 
+## [0.9.4](https://github.com/jlorieau/geomancy/tree/0.9.4) - 2023-07-29
+
+
+### Features
+
+- [#14](https://github.com/jlorieau/geomancy/issues/14). Added checkPlatform check for checking minimum OS versions
+
+
+### Improved Documentation
+
+- [#14](https://github.com/jlorieau/geomancy/issues/14). Added documentation for checkPlatform check
+
+
 ## [0.9.3](https://github.com/jlorieau/geomancy/tree/0.9.3) - 2023-07-29
 
 
 ### Features
 
 - [#25](https://github.com/jlorieau/geomancy/issues/25). Implement github action to test pushes and pull requests
 - [#26](https://github.com/jlorieau/geomancy/issues/26). Implemented environment.sub_env function for check values, allowing a more powerful environment variable substitution mechanism described in the docs for environment files
```

### Comparing `geomancy-0.9.3/docs/conf.py` & `geomancy-0.9.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.3/docs/index.md` & `geomancy-0.9.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.3/docs/usage/cmd_checks.md` & `geomancy-0.9.4/docs/usage/cmd_checks.md`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.3/docs/usage/cmd_run.md` & `geomancy-0.9.4/docs/usage/cmd_run.md`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.3/docs/usage/format.md` & `geomancy-0.9.4/docs/usage/format.md`

 * *Files 12% similar despite different names*

```diff
@@ -325,14 +325,83 @@
 ```toml
 [checks.Environment]
 Pyproject = { checkPath = "./pyproject.toml", type = "file" }
 ```
 :::
 ::::
 
+### checkPlatform
+
+Check the current platform and, optionally, its minimum version.
+
+:::{card}
+Parameters
+^^^
+`checkPlatform`: str
+: Operating system to check. Additionally, an optional version check can be added
+  with a test operator. <br>
+  __aliases__: ``checkOS``, ``checkPlatform``
+
+{{check_base_args}}
+:::
+
+::::{tab-set}
+:::{tab-item} Example 1 (yaml)
+The ``checkPlatform`` check in YAML format.
+```yaml
+check:
+  OperatingSystem:
+    desc: Check the minimum operating system versions
+    subchecks: any
+
+    checkMacOS:
+      desc: MacOS 10.9 or later (released 2013)
+      checkOS: "macOS >= 10.9"
+    checkLinuxOS:
+      desc: Linux 4.0 or later (released 2015)
+      checkOS: "Linux >= 3.0"
+    checkWindows:
+      desc: Windows 10 or later (released 2015)
+      checkOS: "Windows >= 10"
+```
+:::
+:::{tab-item} Example 2 (toml)
+The ``checkPlatfor`` check in TOML format.
+```toml
+[checks.OperatingSystem]
+desc = "Check the minimum operating system versions"
+subchecks = "any"
+
+    [checks.OperatingSystem.checkMacOS]
+    desc = "MacOS 10.9 or later (released 2013)"
+    checkOS = "macOS >= 10.9"
+
+    [checks.OperatingSystem.checkLinuxOS]
+    desc = "Linux 4.0 or later (released 2015)"
+    checkOS = "Linux >= 3.0"
+
+    [checks.OperatingSystem.checkWindows]
+    desc = "Windows 10 or later (released 2015)"
+    checkOS = "Windows >= 10"
+```
+:::
+:::{tab-item} Example 3 (toml)
+The ``checkPlatform`` check in abbreviated TOML format.
+```toml
+[checks.OperatingSystem]
+desc = "Check the minimum operating system versions"
+subchecks = "any"
+
+checkMacOS = {desc = "MacOS 10.9 or later (released 2013)", checkOS = "macOS >= 10.9"}
+checkLinuxOS = {desc = "Linux 4.0 or later (released 2015)", checkOS = "Linux >= 3.0"}
+checkWindows = {desc = "Windows 10 or later (released 2015)", checkOS = "Windows >= 10"}
+```
+:::
+::::
+
 ### checkPythonPkg
 
 Checks whether the python package is installed and, optionally, check its
 version.
 
 :::{card}
 Parameters
@@ -471,14 +540,14 @@
 ```yaml
 [MyOddFilename]
 checkpath='myfile$.txt'
 substitution=false
 ```
 :::
 :::{tab-item} Literal string (toml)
-Use triple (4) single quotes
+Use quadruple (4) single quotes
 ```yaml
 [MyOddFilename]
 checkpath=''''myfile$.txt''''
 ```
 :::
 ::::
```

### Comparing `geomancy-0.9.3/examples/geomancy.toml` & `geomancy-0.9.4/examples/geomancy.toml`

 * *Files 16% similar despite different names*

```diff
@@ -9,17 +9,25 @@
 desc = "Check environment variables common to all development environments"
 
     [checks.Environment.Path]
     desc = "Paths to search for executables"
     checkEnv = "$PATH"
 
     [checks.Environment.Username]
-    desc = "The current username"
-    checkEnv = "$USER"
-    regex = "[a-z_][a-z0-9_-]*[$]?"
+    subchecks = "any"
+
+        [checks.Environment.Username.UnixUsername]  # linux and macOS
+        desc = "The current username"
+        checkEnv = "$USER"
+        regex = "[a-z_][a-z0-9_-]*[$]?"
+
+        [checks.Environment.Username.WindowsUsername]  # windows
+        desc = "The current username"
+        checkEnv = "$USERNAME"
+        regex = "[a-z_][a-z0-9_-]*[$]?"
 
 [checks.Paths]
 desc = "Checks the existence of needed files and directories"
 
     [checks.Paths.ChecksFile]
     desc = "Checks that at least one checks file exists"
     subchecks = "any"
```

### Comparing `geomancy-0.9.3/geomancy/checks/base.py` & `geomancy-0.9.4/geomancy/checks/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,23 +260,35 @@
         # (value)
         d = dict()
         for cls_type in cls_types:
             # Skip abstract classes, which can't be instantiated
             if isabstract(cls_type):
                 continue
 
+            # Make sure class name isn't alreay in the dict
+            assert (
+                cls_type.__name__ not in d
+            ), f"class {cls_type.__name__} already registered class"
+
             # Add the class name directly
             d[cls_type.__name__] = cls_type
 
             # Add class name aliases
             aliases = cls_type.aliases if cls_type.aliases is not None else ()
             for alias in aliases:
                 # Aliases should not create name collisions
                 assert alias not in d, f"Duplicate alias name '{alias}'"
 
+                # Make sure the alias doesn't match a class that's already
+                # registered
+                assert (
+                    alias not in d
+                ), f"Alias {alias} already matches a registered class"
+
+                # Add alias
                 d[alias] = cls_type
         return d
 
     @classmethod
     def load(
         cls, d: dict, name: str, level: int = 1, max_level: t.Optional[int] = None
     ) -> t.Union["CheckBase", None]:
```

### Comparing `geomancy-0.9.3/geomancy/checks/env.py` & `geomancy-0.9.4/geomancy/checks/env.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.3/geomancy/checks/exec.py` & `geomancy-0.9.4/geomancy/checks/exec.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.3/geomancy/checks/path.py` & `geomancy-0.9.4/geomancy/checks/path.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.3/geomancy/checks/utils.py` & `geomancy-0.9.4/geomancy/checks/utils.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.3/geomancy/checks/version.py` & `geomancy-0.9.4/geomancy/checks/version.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,16 @@
 
     @value.setter
     def value(self, v):
         CheckBase.value.fset(self, v)
 
     @abstractmethod
     def get_current_version(self) -> t.Union[None, t.Tuple[int]]:
-        """Get the current version, or None if it can't be found."""
+        """Get the current version as a tuple of integers, or None if it can't
+        be found."""
         return None
 
     def check(self, level: int = 0) -> CheckResult:
         """Check whether the current version is compatible with the version
         specified in the value."""
         name, op, version = self.value
         current_version = self.get_current_version()
@@ -54,15 +55,15 @@
                 status = "present but current version unknown"
             elif (
                 version is not None
                 and current_version is not None
                 and op is not None
                 and not op(current_version, version)
             ):
-                status = f"version={'.'.join(map(str, current_version))}"
+                status = f"incorrect version=" f"{'.'.join(map(str, current_version))}"
             else:
                 status = "passed"
                 passed = True
 
         return CheckResult(
             passed=passed, msg=self.msg.format(check=self), status=status
         )
```

### Comparing `geomancy-0.9.3/geomancy/cli/term.py` & `geomancy-0.9.4/geomancy/cli/term.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.3/geomancy/config/config.py` & `geomancy-0.9.4/geomancy/config/config.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.3/geomancy/entrypoints/check.py` & `geomancy-0.9.4/geomancy/entrypoints/check.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.3/geomancy/entrypoints/config.py` & `geomancy-0.9.4/geomancy/entrypoints/config.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.3/geomancy/entrypoints/environment.py` & `geomancy-0.9.4/geomancy/entrypoints/environment.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.3/geomancy/entrypoints/geo.py` & `geomancy-0.9.4/geomancy/entrypoints/geo.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.3/geomancy/entrypoints/utils.py` & `geomancy-0.9.4/geomancy/entrypoints/utils.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.3/geomancy/environment/dotenv.py` & `geomancy-0.9.4/geomancy/environment/dotenv.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.3/geomancy.egg-info/PKG-INFO` & `geomancy-0.9.4/geomancy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomancy
-Version: 0.9.3
+Version: 0.9.4
 Summary: Geomancy validates deployment and development environments
 Author: Justin Lorieau
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
@@ -46,15 +46,17 @@
 executables, the state of external dependencies, like LaTeX packages, or cloud
 resources, or for checking environments that use the
 [12-factor](http://12factor.net/) principles.
 <!-- end intro -->
 
 ## Quickstart
 <!-- start quickstart -->
-1. Create a ``.geomancy.yaml`` file with checks.
+1. Create a ``.geomancy.yaml`` file with checks. See
+   [examples/geomancy.yaml](https://github.com/jlorieau/geomancy/blob/main/examples/geomancy.yaml)
+   for an example of all checks.
 
     ```yaml
     checks:
       Environment:
         desc: Check environment variables common to all development environments
 
         Username:
@@ -103,27 +105,29 @@
     ``.geomancy.toml``, ``geomancy.toml`` and ``pyproject.toml``.)
 <!-- end quickstart -->
 
 ## Features
 <!-- start features -->
 Geomancy checks include:
 
+- __Operating systems__ meet the minimum required versions
+  ([checkOS](https://geomancy.readthedocs.io/en/latest/usage/format.html#checkplatform))
 - __Environment variables__ are properly set and, optionally,
   check that they have valid values with regular expressions
-  ([checkEnv](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkenv))
+  ([checkEnv](https://geomancy.readthedocs.io/en/latest/usage/format.html#checkenv))
 - __Paths__ exist and whether they're files or directories
-  ([checkPath](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkpath))
+  ([checkPath](https://geomancy.readthedocs.io/en/latest/usage/format.html#checkpath))
 - __Executables__ are available and, optionally, have the minimum or correct
   versions
-  ([checkExec](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkexec))
+  ([checkExec](https://geomancy.readthedocs.io/en/latest/usage/format.html#checkexec))
 - __Python packages__ are available and, optionally, have the minimum or
   correct versions
-  ([checkPythonPkg](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkpythonpkg))
+  ([checkPythonPkg](https://geomancy.readthedocs.io/en/latest/usage/format.html#checkpythonpkg))
 - __Group checks__ to nested groups of checks with conditional (all or any) pass
-  criteria ([groups of checks](https://geomancy.readthedocs.io/en/latest/usage/index.html#check-groups))
+  criteria ([groups of checks](https://geomancy.readthedocs.io/en/latest/usage/format.html#check-groups))
 
 Additionally, geomancy can:
 
 - __Load environment files__ for
   [checks](https://geomancy.readthedocs.io/en/latest/usage/cmd_checks.html#environment-files)
   or for [running](https://geomancy.readthedocs.io/en/latest/usage/cmd_run.html#running-environments)
   shell commands
```

### Comparing `geomancy-0.9.3/geomancy.egg-info/SOURCES.txt` & `geomancy-0.9.4/geomancy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 geomancy.egg-info/requires.txt
 geomancy.egg-info/top_level.txt
 geomancy/checks/__init__.py
 geomancy/checks/base.py
 geomancy/checks/env.py
 geomancy/checks/exec.py
 geomancy/checks/path.py
+geomancy/checks/platform.py
 geomancy/checks/python.py
 geomancy/checks/utils.py
 geomancy/checks/version.py
 geomancy/cli/__init__.py
 geomancy/cli/term.py
 geomancy/config/__init__.py
 geomancy/config/config.py
@@ -51,13 +52,14 @@
 geomancy/environment/__init__.py
 geomancy/environment/dotenv.py
 tests/conftest.py
 tests/checks/test_base.py
 tests/checks/test_env.py
 tests/checks/test_exec.py
 tests/checks/test_path.py
+tests/checks/test_platform.py
 tests/checks/test_python.py
 tests/config/config1.toml
 tests/config/test_config.py
 tests/data/test.env
 tests/entrypoints/test_geo.py
 tests/environment/test_dotenv.py
```

### Comparing `geomancy-0.9.3/pyproject.toml` & `geomancy-0.9.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.3/tests/checks/test_base.py` & `geomancy-0.9.4/tests/checks/test_base.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.3/tests/checks/test_env.py` & `geomancy-0.9.4/tests/checks/test_env.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.3/tests/checks/test_exec.py` & `geomancy-0.9.4/tests/checks/test_exec.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.3/tests/checks/test_path.py` & `geomancy-0.9.4/tests/checks/test_path.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.3/tests/config/test_config.py` & `geomancy-0.9.4/tests/config/test_config.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.3/tests/conftest.py` & `geomancy-0.9.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.3/tests/entrypoints/test_geo.py` & `geomancy-0.9.4/tests/entrypoints/test_geo.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.9.3/tests/environment/test_dotenv.py` & `geomancy-0.9.4/tests/environment/test_dotenv.py`

 * *Files identical despite different names*

