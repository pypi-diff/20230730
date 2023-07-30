# Comparing `tmp/moscot-0.3.0.tar.gz` & `tmp/moscot-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moscot-0.3.0.tar", last modified: Fri May 12 09:56:06 2023, max compression
+gzip compressed data, was "moscot-0.3.1.tar", last modified: Sun Jul 30 08:10:08 2023, max compression
```

## Comparing `moscot-0.3.0.tar` & `moscot-0.3.1.tar`

### file list

```diff
@@ -1,94 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.420514 moscot-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-12 09:54:41.000000 moscot-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-12 09:54:41.000000 moscot-0.3.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-12 09:54:41.000000 moscot-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-12 09:54:41.000000 moscot-0.3.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-12 09:54:41.000000 moscot-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-12 09:54:41.000000 moscot-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-12 09:56:06.420514 moscot-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-12 09:54:41.000000 moscot-0.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-12 09:54:41.000000 moscot-0.3.0/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8649 2023-05-12 09:54:41.000000 moscot-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 09:56:06.420514 moscot-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.408513 moscot-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.412513 moscot-0.3.0/src/moscot/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.412513 moscot-0.3.0/src/moscot/_docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/_docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15359 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/_docs/_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/_docs/_docs_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/_docs/_docs_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/_docs/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.412513 moscot-0.3.0/src/moscot/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.412513 moscot-0.3.0/src/moscot/backends/ott/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/backends/ott/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/backends/ott/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/backends/ott/output.py
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/backends/ott/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/backends/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.412513 moscot-0.3.0/src/moscot/base/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/base/cost.py
--rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/base/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.416514 moscot-0.3.0/src/moscot/base/problems/
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/base/problems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22166 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/base/problems/_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    25439 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/base/problems/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/base/problems/birth_death.py
--rw-r--r--   0 runner    (1001) docker     (123)    22334 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/base/problems/compound_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/base/problems/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    27779 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/base/problems/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     7346 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/base/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.416514 moscot-0.3.0/src/moscot/costs/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/costs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/costs/_costs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/costs/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15430 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.416514 moscot-0.3.0/src/moscot/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9075 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/plotting/_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    23707 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/plotting/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.416514 moscot-0.3.0/src/moscot/problems/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/problems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/problems/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.416514 moscot-0.3.0/src/moscot/problems/generic/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/problems/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/problems/generic/_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/problems/generic/_mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.416514 moscot-0.3.0/src/moscot/problems/space/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/problems/space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/problems/space/_alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/problems/space/_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    22205 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/problems/space/_mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.416514 moscot-0.3.0/src/moscot/problems/spatiotemporal/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/problems/spatiotemporal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/problems/spatiotemporal/_spatio_temporal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.416514 moscot-0.3.0/src/moscot/problems/time/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/problems/time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/problems/time/_lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)    31747 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/problems/time/_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.420514 moscot-0.3.0/src/moscot/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.420514 moscot-0.3.0/src/moscot/utils/_data/
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/utils/_data/allTFs_dmel.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11690 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/utils/_data/allTFs_hg38.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11726 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/utils/_data/allTFs_mm.txt
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/utils/_data/human_apoptosis.txt
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/utils/_data/human_proliferation.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/utils/_data/mouse_apoptosis.txt
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/utils/_data/mouse_proliferation.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/utils/subset_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/utils/tagged_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.412513 moscot-0.3.0/src/moscot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-12 09:56:06.000000 moscot-0.3.0/src/moscot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-12 09:56:06.000000 moscot-0.3.0/src/moscot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 09:56:06.000000 moscot-0.3.0/src/moscot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-12 09:56:06.000000 moscot-0.3.0/src/moscot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 09:56:06.000000 moscot-0.3.0/src/moscot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.389801 moscot-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-30 08:08:45.000000 moscot-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-30 08:08:45.000000 moscot-0.3.1/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-30 08:08:45.000000 moscot-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-30 08:08:45.000000 moscot-0.3.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-30 08:08:45.000000 moscot-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-30 08:08:45.000000 moscot-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-07-30 08:10:08.385801 moscot-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-07-30 08:08:45.000000 moscot-0.3.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-30 08:08:45.000000 moscot-0.3.1/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-07-30 08:08:45.000000 moscot-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 08:10:08.389801 moscot-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.377802 moscot-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.381801 moscot-0.3.1/src/moscot/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.381801 moscot-0.3.1/src/moscot/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.381801 moscot-0.3.1/src/moscot/backends/ott/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/backends/ott/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/backends/ott/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/backends/ott/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/backends/ott/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/backends/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.381801 moscot-0.3.1/src/moscot/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/base/cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13161 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/base/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.381801 moscot-0.3.1/src/moscot/base/problems/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/base/problems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22360 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/base/problems/_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25371 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/base/problems/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11187 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/base/problems/birth_death.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21112 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/base/problems/compound_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/base/problems/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31320 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/base/problems/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/base/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.385801 moscot-0.3.1/src/moscot/costs/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/costs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/costs/_costs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/costs/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15395 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.385801 moscot-0.3.1/src/moscot/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13977 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/plotting/_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23748 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/plotting/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.385801 moscot-0.3.1/src/moscot/problems/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/problems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/problems/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.385801 moscot-0.3.1/src/moscot/problems/cross_modality/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/problems/cross_modality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/problems/cross_modality/_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12773 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/problems/cross_modality/_translation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.385801 moscot-0.3.1/src/moscot/problems/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/problems/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21399 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/problems/generic/_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/problems/generic/_mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.385801 moscot-0.3.1/src/moscot/problems/space/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/problems/space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11090 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/problems/space/_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13883 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/problems/space/_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25427 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/problems/space/_mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.385801 moscot-0.3.1/src/moscot/problems/spatiotemporal/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/problems/spatiotemporal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/problems/spatiotemporal/_spatio_temporal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.385801 moscot-0.3.1/src/moscot/problems/time/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/problems/time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22380 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/problems/time/_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39311 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/problems/time/_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.385801 moscot-0.3.1/src/moscot/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.385801 moscot-0.3.1/src/moscot/utils/_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/utils/_data/allTFs_dmel.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11690 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/utils/_data/allTFs_hg38.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11726 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/utils/_data/allTFs_mm.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/utils/_data/human_apoptosis.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/utils/_data/human_proliferation.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/utils/_data/mouse_apoptosis.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/utils/_data/mouse_proliferation.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17299 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/utils/subset_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/utils/tagged_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.381801 moscot-0.3.1/src/moscot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-07-30 08:10:08.000000 moscot-0.3.1/src/moscot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-07-30 08:10:08.000000 moscot-0.3.1/src/moscot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 08:10:08.000000 moscot-0.3.1/src/moscot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-30 08:10:08.000000 moscot-0.3.1/src/moscot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-30 08:10:08.000000 moscot-0.3.1/src/moscot.egg-info/top_level.txt
```

### Comparing `moscot-0.3.0/.gitignore` & `moscot-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `moscot-0.3.0/.pre-commit-config.yaml` & `moscot-0.3.1/.pre-commit-config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -3,30 +3,30 @@
   python: python3
 default_stages:
   - commit
   - push
 minimum_pre_commit_version: 3.0.0
 repos:
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.1.1
+    rev: v1.4.1
     hooks:
       - id: mypy
-        additional_dependencies: [numpy>=1.21.0, jax]
+        additional_dependencies: [numpy>=1.25.0]
         files: ^src
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.7.0
     hooks:
       - id: black
         additional_dependencies: [toml]
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.0-alpha.6
+    rev: v3.0.0
     hooks:
       - id: prettier
         language_version: system
-  - repo: https://github.com/timothycrosley/isort
+  - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
         additional_dependencies: [toml]
         args: [--order-by-type]
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
@@ -38,32 +38,32 @@
       - id: mixed-line-ending
         args: [--fix=lf]
       - id: trailing-whitespace
       - id: check-docstring-first
       - id: check-yaml
       - id: check-toml
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.9.0
     hooks:
       - id: pyupgrade
         args: [--py3-plus, --py38-plus, --keep-runtime-typing]
   - repo: https://github.com/asottile/blacken-docs
-    rev: 1.13.0
+    rev: 1.15.0
     hooks:
       - id: blacken-docs
         additional_dependencies: [black==23.1.0]
   - repo: https://github.com/rstcheck/rstcheck
     rev: v6.1.2
     hooks:
       - id: rstcheck
         additional_dependencies: [tomli]
         args: [--config=pyproject.toml]
   - repo: https://github.com/PyCQA/doc8
     rev: v1.1.1
     hooks:
       - id: doc8
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
+  - repo: https://github.com/astral-sh/ruff-pre-commit
     # Ruff version.
-    rev: v0.0.257
+    rev: v0.0.280
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
```

### Comparing `moscot-0.3.0/LICENSE` & `moscot-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `moscot-0.3.0/PKG-INFO` & `moscot-0.3.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moscot
-Version: 0.3.0
+Version: 0.3.1
 Summary: Multi-omic single-cell optimal transport tools
 Author: Dominik Klein, Giovanni Palla, Michal Klein, Zoe Piran, Marius Lange
 Maintainer-email: Dominik Klein <dominik.klein@helmholtz-muenchen.de>, Giovanni Palla <giovanni.palla@helmholtz-muenchen.de>, Michal Klein <michal.klein@helmholtz-muenchen.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Theis Lab
         All rights reserved.
@@ -58,54 +58,73 @@
 Description-Content-Type: text/x-rst
 Provides-Extra: spatial
 Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE
 
-|Codecov|
+|PyPI| |Downloads| |CI| |Pre-commit| |Codecov| |Docs|
 
 moscot - multi-omic single-cell optimal transport tools
 =======================================================
 
 **moscot** is a scalable framework for Optimal Transport (OT) applications in
 single-cell genomics. It can be used for
-- temporal and spatio-temporal trajectory inference
-- spatial mapping
-- spatial alignment
+
+- trajectory inference (incorporating spatial and lineage information)
+- mapping cells to their spatial organisation
+- aligning spatial transcriptomics slides
+- translating modalities
 - prototyping of new OT models in single-cell genomics
 
 **moscot** is powered by
 `OTT <https://ott-jax.readthedocs.io>`_ which is a JAX-based Optimal
 Transport toolkit that supports just-in-time compilation, GPU acceleration, automatic
 differentiation and linear memory complexity for OT problems.
 
 Installation
 ------------
 You can install **moscot** via::
 
     pip install moscot
 
-In order to install **moscot** from source, run::
+In order to install **moscot** from in editable mode, run::
 
     git clone https://github.com/theislab/moscot
     cd moscot
-    pip install -e .'[dev]'
-
-If used with GPU, additionally run::
-
-    pip install --upgrade "jax[cuda]" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
+    pip install -e .
 
-
-.. |Codecov| image:: https://codecov.io/gh/theislab/moscot/branch/master/graph/badge.svg?token=Rgtm5Tsblo
-    :target: https://codecov.io/gh/theislab/moscot
-    :alt: Coverage
+For further instructions how to install jax, please refer to https://github.com/google/jax.
 
 Resources
 ---------
 
 Please have a look at our `documentation <https://moscot.readthedocs.io>`_
 
 Reference
 ---------
 
 Our preprint "Mapping cells through time and space with moscot" can be found `here <https://www.biorxiv.org/content/10.1101/2023.05.11.540374v1>`_.
+
+.. |Codecov| image:: https://codecov.io/gh/theislab/moscot/branch/master/graph/badge.svg?token=Rgtm5Tsblo
+    :target: https://codecov.io/gh/theislab/moscot
+    :alt: Coverage
+
+.. |PyPI| image:: https://img.shields.io/pypi/v/moscot.svg
+    :target: https://pypi.org/project/moscot/
+    :alt: PyPI
+
+.. |CI| image:: https://img.shields.io/github/actions/workflow/status/theislab/moscot/test.yml?branch=main
+    :target: https://github.com/theislab/moscot/actions
+    :alt: CI
+
+.. |Pre-commit| image:: https://results.pre-commit.ci/badge/github/theislab/moscot/main.svg
+   :target: https://results.pre-commit.ci/latest/github/theislab/moscot/main
+   :alt: pre-commit.ci status
+
+.. |Docs| image:: https://img.shields.io/readthedocs/moscot
+    :target: https://moscot.readthedocs.io/en/stable/
+    :alt: Documentation
+
+.. |Downloads| image:: https://pepy.tech/badge/moscot
+    :target: https://pepy.tech/project/moscot
+    :alt: Downloads
```

### Comparing `moscot-0.3.0/README.rst` & `moscot-0.3.1/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,66 @@
-|Codecov|
+|PyPI| |Downloads| |CI| |Pre-commit| |Codecov| |Docs|
 
 moscot - multi-omic single-cell optimal transport tools
 =======================================================
 
 **moscot** is a scalable framework for Optimal Transport (OT) applications in
 single-cell genomics. It can be used for
-- temporal and spatio-temporal trajectory inference
-- spatial mapping
-- spatial alignment
+
+- trajectory inference (incorporating spatial and lineage information)
+- mapping cells to their spatial organisation
+- aligning spatial transcriptomics slides
+- translating modalities
 - prototyping of new OT models in single-cell genomics
 
 **moscot** is powered by
 `OTT <https://ott-jax.readthedocs.io>`_ which is a JAX-based Optimal
 Transport toolkit that supports just-in-time compilation, GPU acceleration, automatic
 differentiation and linear memory complexity for OT problems.
 
 Installation
 ------------
 You can install **moscot** via::
 
     pip install moscot
 
-In order to install **moscot** from source, run::
+In order to install **moscot** from in editable mode, run::
 
     git clone https://github.com/theislab/moscot
     cd moscot
-    pip install -e .'[dev]'
-
-If used with GPU, additionally run::
-
-    pip install --upgrade "jax[cuda]" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
+    pip install -e .
 
-
-.. |Codecov| image:: https://codecov.io/gh/theislab/moscot/branch/master/graph/badge.svg?token=Rgtm5Tsblo
-    :target: https://codecov.io/gh/theislab/moscot
-    :alt: Coverage
+For further instructions how to install jax, please refer to https://github.com/google/jax.
 
 Resources
 ---------
 
 Please have a look at our `documentation <https://moscot.readthedocs.io>`_
 
 Reference
 ---------
 
 Our preprint "Mapping cells through time and space with moscot" can be found `here <https://www.biorxiv.org/content/10.1101/2023.05.11.540374v1>`_.
+
+.. |Codecov| image:: https://codecov.io/gh/theislab/moscot/branch/master/graph/badge.svg?token=Rgtm5Tsblo
+    :target: https://codecov.io/gh/theislab/moscot
+    :alt: Coverage
+
+.. |PyPI| image:: https://img.shields.io/pypi/v/moscot.svg
+    :target: https://pypi.org/project/moscot/
+    :alt: PyPI
+
+.. |CI| image:: https://img.shields.io/github/actions/workflow/status/theislab/moscot/test.yml?branch=main
+    :target: https://github.com/theislab/moscot/actions
+    :alt: CI
+
+.. |Pre-commit| image:: https://results.pre-commit.ci/badge/github/theislab/moscot/main.svg
+   :target: https://results.pre-commit.ci/latest/github/theislab/moscot/main
+   :alt: pre-commit.ci status
+
+.. |Docs| image:: https://img.shields.io/readthedocs/moscot
+    :target: https://moscot.readthedocs.io/en/stable/
+    :alt: Documentation
+
+.. |Downloads| image:: https://pepy.tech/badge/moscot
+    :target: https://pepy.tech/project/moscot
+    :alt: Downloads
```

### Comparing `moscot-0.3.0/pyproject.toml` & `moscot-0.3.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -43,23 +43,22 @@
     {name = "Michal Klein", email = "michal.klein@helmholtz-muenchen.de"}
 ]
 
 
 dependencies = [
     "numpy>=1.20.0",
     "scipy>=1.7.0",
-    "pandas<2.0",
+    "pandas>=2.0.1",
     "networkx>=2.6.3",
     # https://github.com/scverse/scanpy/issues/2411
     "matplotlib>=3.5.0",
-    "anndata>=0.8.0",
+    "anndata>=0.9.1",
     "scanpy>=1.9.3",
     "wrapt>=1.13.2",
-    "docrep>=0.3.2",
-    "ott-jax>=0.4.0",
+    "ott-jax==0.4.0",
     "cloudpickle>=2.2.0",
 ]
 
 [project.optional-dependencies]
 spatial = [
     "squidpy>=1.2.3"
 ]
@@ -75,17 +74,18 @@
     "coverage[toml]>=7",
 ]
 docs = [
     "sphinx>=5.1.1",
     "sphinx_copybutton>=0.5.0",
     "sphinxcontrib-bibtex>=2.3.0",
     "sphinxcontrib-spelling>=7.6.2",
+    "sphinx-autodoc-typehints",
     "furo>=2022.09.29",
+    "sphinx-tippy>=0.4.1",
     "myst-nb>=0.17.1",
-    "nbsphinx>=0.8.1",
     "ipython>=7.20.0",
     "sphinx_design>=0.3.0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/theislab/moscot"
 Download = "https://moscot.readthedocs.io/en/latest/installation.html"
@@ -147,43 +147,41 @@
 "tests/*" = ["D"]
 "*/__init__.py" = ["F401"]
 "docs/*" = ["D"]
 "src/moscot/constants.py" = ["D101"]
 "src/moscot/utils/subset_policy.py" = ["D101", "D102"]
 [tool.ruff.pydocstyle]
 convention = "numpy"
-[tool.ruff.pyupgrade]
-# Preserve types, even if a file imports `from __future__ import annotations`.
-keep-runtime-typing = true
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all"
 [tool.ruff.flake8-quotes]
 inline-quotes = "double"
 
 [tool.black]
 line-length = 120
 target-version = ['py38']
 include = '\.pyi?$'
 
 [tool.isort]
 profile = "black"
 include_trailing_comma = true
 multi_line_output = 3
-sections = ["FUTURE", "STDLIB", "THIRDPARTY", "NUMERIC", "PLOTTING", "BIO", "FIRSTPARTY", "LOCALFOLDER"]
+sections = ["FUTURE", "STDLIB", "THIRDPARTY", "GENERIC", "NUMERIC", "PLOTTING", "BIO", "FIRSTPARTY", "LOCALFOLDER"]
 # also contains what we import in notebooks
-known_numeric = ["numpy", "scipy", "jax", "ott", "pandas", "sklearn", "networkx"]
+known_generic = ["wrapt", "joblib"]
+known_numeric = ["numpy", "scipy", "jax", "ott", "pandas", "sklearn", "networkx", "statsmodels"]
 known_bio = ["anndata", "scanpy", "squidpy"]
 known_plotting = ["IPython", "matplotlib", "mpl_toolkits", "seaborn"]
 
 [tool.pytest.ini_options]
 markers = ["fast: marks tests as fask"]
 xfail_strict = true
 filterwarnings = [
-    "ignore:X.dtype being converted:FutureWarning",
     "ignore:No data for colormapping:UserWarning",
+    "ignore:The dtype argument will be deprecated in anndata:PendingDeprecationWarning"
 ]
 
 [tool.coverage.run]
 branch = true
 parallel = true
 source = ["src/"]
 omit = [
@@ -209,14 +207,15 @@
     "toctree",
     "currentmodule",
     "autosummary",
     "module",
     "automodule",
     "autoclass",
     "bibliography",
+    "glossary",
     "card",
     "grid",
 ]
 ignore_roles = [
     "mod",
 ]
 
@@ -246,15 +245,15 @@
 no_warn_no_return = true
 
 show_error_codes = true
 show_column_numbers = true
 error_summary = true
 ignore_missing_imports = true
 
-disable_error_code = ["assignment", "comparison-overlap", "no-untyped-def"]
+disable_error_code = ["assignment", "comparison-overlap", "no-untyped-def", "override"]
 
 [tool.doc8]
 max_line_length = 120
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
@@ -289,23 +288,23 @@
 commands =
     make linkcheck {posargs}
     # TODO(michalk8): uncomment after https://github.com/theislab/moscot/issues/490
     # make spelling {posargs}
 
 [testenv:clean-docs]
 description = Remove the documentation.
+deps =
 skip_install = true
 changedir = {tox_root}{/}docs
 allowlist_externals = make
 commands =
     make clean
 
 [testenv:build-docs]
 description = Build the documentation.
-use_develop = true
 deps =
 extras = docs
 allowlist_externals = make
 changedir = {tox_root}{/}docs
 commands =
     make html {posargs}
 commands_post =
```

### Comparing `moscot-0.3.0/src/moscot/_docs/_docs_mixins.py` & `moscot-0.3.1/src/moscot/problems/generic/_mixins.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,224 +1,251 @@
-from docrep import DocstringProcessor
+from typing import TYPE_CHECKING, Any, List, Literal, Optional, Protocol, Tuple, Union
 
-_cell_trans_params = """\
-source
-    Key identifying the source distribution.
-target
-    Key identifying the target distribution.
-source_groups
-    Can be one of the following:
-
-        - if `source_groups` is of type :class:`str` this should correspond to a key in
-          :attr:`anndata.AnnData.obs`. In this case, the categories in the transition matrix correspond to the
-          unique values in :attr:`anndata.AnnData.obs` ``['{source_groups}']``.
-        - if `target_groups` is of type :class:`dict`, its key should correspond to a key in
-          :attr:`anndata.AnnData.obs` and its value to a list containing a subset of categories present in
-          :attr:`anndata.AnnData.obs` ``['{source_groups.keys()[0]}']``. The order of the list determines the order
-          in the transition matrix.
-
-target_groups
-    Can be one of the following:
-
-        - if `target_groups` is of type :class:`str` this should correspond to a key in
-          :attr:`anndata.AnnData.obs`. In this case, the categories in the transition matrix correspond to the
-          unique values in :attr:`anndata.AnnData.obs` ``['{target_groups}']``.
-        - if `target_groups` is of :class:`dict`, its key should correspond to a key in
-          :attr:`anndata.AnnData.obs` and its value to a list containing a subset of categories present in
-          :attr:`anndata.AnnData.obs` ``['{target_groups.keys()[0]}']``. The order of the list determines the order
-          in the transition matrix.
-"""
-_key = """\
-key
-    Key in :attr:`anndata.AnnData.obs` allocating the cell to a certain cell distribution (e.g. batch)."""
-_aggregation_mode = """\
-aggregation_mode
-
-    - `group`: transition probabilities from the groups defined by `source_annotation` are returned.
-    - `cell`: the transition probabilities for each cell are returned.
-"""
-_other_key = """\
-other_key
-    Key in :attr:`anndata.AnnData.obs` allocating the cell to a certain cell distribution (e.g. batch).
-"""
-_other_adata = """\
-adata
-    Annotated data object.
-"""
-_ott_jax_batch_size = """\
-batch_size
-    number of data points the matrix-vector products are applied to at the same time. The larger, the more memory
-    is required.
-"""
-_key_added_plotting = """\
-key_added
-    Key in :attr:`anndata.AnnData.uns` and/or :attr:`anndata.AnnData.obs` where the results
-    for the corresponding plotting functions are stored.
-    See TODO Notebook for how :mod:`moscot.plotting` works.
-"""
-_return_cell_transition = "Transition matrix of cells or groups of cells."
-_notes_cell_transition = """\
-To visualize the results, see :func:`moscot.plotting.cell_transition`.
-"""
-_normalize = """\
-normalize
-    If `True` the transition matrix is normalized such that it is stochastic. If `forward` is `True`, the transition
-    matrix is row-stochastic, otherwise column-stochastic.
-"""
-_forward_cell_transition = """\
-forward
-    If `True` computes transition from `source_annotations` to `target_annotations`, otherwise backward.
-"""
-_return_data = """\
-return_data
-    Whether to return the data.
-"""
-_return_all = """\
-return_all
-    If `True` returns all the intermediate masses if pushed through multiple transport plans, returned as a
-    dictionary.
-"""
-_data = """\
-data
-    - If `data` is a :class:`str` this should correspond to a column in :attr:`anndata.AnnData.obs`.
-      The transport map is applied to the subset corresponding to the source distribution
-      (if `forward` is `True`) or target distribution (if `forward` is `False`) of that column.
-    - If `data` is a :class:`numpy.ndarray` the transport map is applied to `data`.
-    - If `data` is a :class:`dict` then the keys should correspond to the tuple defining a single optimal
-      transport map and the value should be one of the two cases described above.
-"""
-_subset = """\
-subset
-    Subset of :attr:`anndata.AnnData.obs` ``['{key}']`` values of which the policy is to be applied to.
-"""
-_source = """\
-source
-    Value in :attr:`anndata.AnnData.obs` defining the assignment to the source distribution.
-"""
-_target = """\
-target
-    Value in :attr:`anndata.AnnData.obs` defining the assignment to the target distribution.
-"""
-_scale_by_marginals = """\
-scale_by_marginals
-    If `True` the transport map is scaled to be a stochastic matrix by multiplying the resulting mass
-    by the inverse of the marginals, TODO maybe EXAMPLE.
-"""
-_return_push_pull = """
-Depending on `key_added` updates `adata` or returns the result:
-
-    - In the former case all intermediate results are saved in :attr:`anndata.AnnData.obs`.
-    - In the latter case all intermediate step results are returned if `return_all` is `True`,
-      otherwise only the distribution at `source` is returned.
-"""
-_restrict_to_existing = """\
-restrict_to_existing
-    TODO.
-"""
-_order_annotations = """\
-order_annotations
-    Order of the annotations in the final plot, from top to bottom.
-"""
-_threshold = """\
-threshold
-    If not `None`, set all entries below `threshold` to 0.
-"""
-_backend = """\
-backend
-    Which backend to use for solving Optimal Transport problems.
-"""
-_kwargs_divergence = """\
-kwargs
-    Keyword arguments to solve the underlying Optimal Transport problem, see example TODO.
-"""
-_start = """\
-start
-    Time point corresponding to the early distribution.
-"""
-_end = """\
-end
-    Time point corresponding to the late distribution.
-"""
-_intermediate = """\
-intermediate
-    Time point corresponding to the intermediate distribution.
-"""
-_intermediate_interpolation = """\
-intermediate
-    Time point corresponding to the intermediate distribution which is to be interpolated.
-"""
-_seed_sampling = """\
-seed
-    Random seed for sampling from the transport matrix.
-"""
-_interpolation_parameter = """\
-interpolation_parameter
-    Interpolation parameter determining the weight of the source and the target distribution. If `None`
-    it is linearly inferred from `source`, `intermediate`, and `target`.
-"""
-_account_for_unbalancedness = """\
-account_for_unbalancedness
-    If `True` unbalancedness is accounted for by assuming exponential growth and death of cells.
-"""
-_n_interpolated_cells = """\
-n_interpolated_cells
-    Number of generated interpolated cell. If `None` the number of data points in the `intermediate`
-    distribution is taken.
-"""
-_seed_interpolation = """\
-seed
-    Random seed for generating randomly interpolated cells.
-"""
-_time_batch_distance = """\
-time
-    Time point corresponding to the cell distribution which to compute the batch distances within.
-"""
-_batch_key_batch_distance = """\
-batch_key
-    Key in :attr:`anndata.AnnData.obs` storing which batch each cell belongs to.
-"""
-_use_posterior_marginals = """\
-posterior_marginals
-    Whether to use posterior marginals (posterior growth rates). This requires the problem to be solved.
-    If `False`, prior marginals are used.
-"""
-
-d_mixins = DocstringProcessor(
-    cell_trans_params=_cell_trans_params,
-    key=_key,
-    forward_cell_transition=_forward_cell_transition,
-    aggregation_mode=_aggregation_mode,
-    other_key=_other_key,
-    other_adata=_other_adata,
-    ott_jax_batch_size=_ott_jax_batch_size,
-    key_added_plotting=_key_added_plotting,
-    return_cell_transition=_return_cell_transition,
-    notes_cell_transition=_notes_cell_transition,
-    normalize=_normalize,
-    # TODO(MUCDK): duplicate
-    forward=_forward_cell_transition,
-    return_data=_return_data,
-    return_all=_return_all,
-    return_push_pull=_return_push_pull,
-    data=_data,
-    subset=_subset,
-    source=_source,
-    target=_target,
-    scale_by_marginals=_scale_by_marginals,
-    restrict_to_existing=_restrict_to_existing,
-    order_annotations=_order_annotations,
-    threshold=_threshold,
-    backend=_backend,
-    kwargs_divergence=_kwargs_divergence,
-    start=_start,
-    end=_end,
-    intermediate=_intermediate,
-    intermediate_interpolation=_intermediate_interpolation,
-    seed_sampling=_seed_sampling,
-    interpolation_parameter=_interpolation_parameter,
-    n_interpolated_cells=_n_interpolated_cells,
-    seed_interpolation=_seed_interpolation,
-    time_batch_distance=_time_batch_distance,
-    batch_key_batch_distance=_batch_key_batch_distance,
-    use_posterior_marginals=_use_posterior_marginals,
-    account_for_unbalancedness=_account_for_unbalancedness,
-)
+import pandas as pd
+
+from anndata import AnnData
+
+from moscot import _constants
+from moscot._types import ArrayLike, Str_Dict_t
+from moscot.base.problems._mixins import AnalysisMixin, AnalysisMixinProtocol
+from moscot.base.problems.compound_problem import ApplyOutput_t, B, K
+from moscot.plotting._utils import set_plotting_vars
+
+__all__ = ["GenericAnalysisMixin"]
+
+
+class GenericAnalysisMixinProtocol(AnalysisMixinProtocol[K, B], Protocol[K, B]):
+    """Protocol class."""
+
+    _batch_key: Optional[str]
+    batch_key: Optional[str]
+    adata: AnnData
+
+    def _cell_transition(
+        self: AnalysisMixinProtocol[K, B],
+        *args: Any,
+        **kwargs: Any,
+    ) -> pd.DataFrame:
+        ...
+
+
+class GenericAnalysisMixin(AnalysisMixin[K, B]):
+    """Generic Analysis Mixin."""
+
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        super().__init__(*args, **kwargs)
+        self._batch_key: Optional[str] = None
+
+    def cell_transition(
+        self: GenericAnalysisMixinProtocol[K, B],
+        source: K,
+        target: K,
+        source_groups: Optional[Str_Dict_t] = None,
+        target_groups: Optional[Str_Dict_t] = None,
+        aggregation_mode: Literal["annotation", "cell"] = "annotation",
+        forward: bool = False,
+        batch_size: Optional[int] = None,
+        normalize: bool = True,
+        key_added: Optional[str] = _constants.CELL_TRANSITION,
+    ) -> pd.DataFrame:
+        """Aggregate the transport matrix.
+
+        .. seealso::
+            - See :doc:`../notebooks/examples/plotting/200_cell_transitions`
+              on how to compute and plot the cell transitions.
+
+        Parameters
+        ----------
+        source
+            Key identifying the source distribution.
+        target
+            Key identifying the target distribution.
+        source_groups
+            Source groups used for aggregation. Valid options are:
+
+            - :class:`str` - key in :attr:`~anndata.AnnData.obs` where categorical data is stored.
+            - :class:`dict` - a dictionary with one key corresponding to a categorical column in
+              :attr:`~anndata.AnnData.obs` and values to a subset of categories.
+        target_groups
+            Target groups used for aggregation. Valid options are:
+
+            - :class:`str` - key in :attr:`~anndata.AnnData.obs` where categorical data is stored.
+            - :class:`dict` - a dictionary with one key corresponding to a categorical column in
+              :attr:`~anndata.AnnData.obs` and values to a subset of categories.
+        aggregation_mode
+            How to aggregate the cell-level transport maps. Valid options are:
+
+            - ``'annotation'`` - group the transitions by the ``source_groups`` and the ``target_groups``.
+            - ``'cell'`` - do not group by the ``source_groups`` or the ``target_groups``, depending on the ``forward``.
+        forward
+            If :obj:`True`, compute the transitions from the ``source_groups`` to the ``target_groups``.
+        batch_size
+            Number of rows/columns of the cost matrix to materialize during :meth:`push` or :meth:`pull`.
+            Larger value will require more memory.
+        normalize
+            If :obj:`True`, normalize the transition matrix. If ``forward = True``, the transition matrix
+            will be row-stochastic, otherwise column-stochastic.
+        key_added
+            Key in :attr:`~anndata.AnnData.uns` where to save the result.
+
+        Returns
+        -------
+        Depending on the ``key_added``:
+
+        - :obj:`None` - returns the transition matrix.
+        - :obj:`str` - returns nothing and saves the transition matrix to
+          :attr:`uns['moscot_results']['cell_transition']['{key_added}'] <anndata.AnnData.uns>`
+        """
+        if TYPE_CHECKING:
+            assert isinstance(self.batch_key, str)
+        # TODO(michalk8): modify the behavior to match with the docs
+        return self._cell_transition(
+            key=self.batch_key,
+            source=source,
+            target=target,
+            source_groups=source_groups,
+            target_groups=target_groups,
+            forward=forward,
+            aggregation_mode=aggregation_mode,
+            batch_size=batch_size,
+            normalize=normalize,
+            other_key=None,
+            key_added=key_added,
+        )
+
+    def push(
+        self: GenericAnalysisMixinProtocol[K, B],
+        source: K,
+        target: K,
+        data: Optional[Union[str, ArrayLike]] = None,
+        subset: Optional[Union[str, List[str], Tuple[int, int]]] = None,
+        scale_by_marginals: bool = True,
+        key_added: Optional[str] = _constants.PUSH,
+        return_all: bool = False,
+        **kwargs: Any,
+    ) -> Optional[ApplyOutput_t[K]]:
+        """Push mass from source to target.
+
+        Parameters
+        ----------
+        source
+            Source key in :attr:`solutions`.
+        target
+            Target key in :attr:`solutions`.
+        data
+            Initial data to push, see :meth:`~moscot.base.problems.OTProblem.push` for information.
+        subset
+            Push values contained only within the subset.
+        scale_by_marginals
+            Whether to scale by the source :term:`marginals`.
+        key_added
+            Key in :attr:`~anndata.AnnData.obs` where to add the result.
+        return_all
+            Whether to also return intermediate results. Always true if ``key_added != None``.
+        kwargs
+            Keyword arguments for the subproblems' :meth:`~moscot.base.problems.OTProblem.push` method.
+
+        Returns
+        -------
+        Depending on the ``key_added``:
+
+        - :obj:`None` - returns the result.
+        - :class:`str` - returns nothing and updates :attr:`obs['{key_added}'] <anndata.AnnData.obs>`
+          with the result.
+        """
+        result = self._apply(
+            source=source,
+            target=target,
+            data=data,
+            subset=subset,
+            forward=True,
+            return_all=return_all or key_added is not None,
+            scale_by_marginals=scale_by_marginals,
+            **kwargs,
+        )
+
+        if TYPE_CHECKING:
+            assert isinstance(result, dict)
+
+        if key_added is not None:
+            if TYPE_CHECKING:
+                assert isinstance(key_added, str)
+            plot_vars = {
+                "distribution_key": self.batch_key,
+            }
+            self.adata.obs[key_added] = self._flatten(result, key=self.batch_key)
+            set_plotting_vars(self.adata, _constants.PUSH, key=key_added, value=plot_vars)
+            return None
+        return result
+
+    def pull(
+        self: GenericAnalysisMixinProtocol[K, B],
+        source: K,
+        target: K,
+        data: Optional[Union[str, ArrayLike]] = None,
+        subset: Optional[Union[str, List[str], Tuple[int, int]]] = None,
+        scale_by_marginals: bool = True,
+        key_added: Optional[str] = _constants.PULL,
+        return_all: bool = False,
+        **kwargs: Any,
+    ) -> Optional[ApplyOutput_t[K]]:
+        """Pull mass from target to source.
+
+        Parameters
+        ----------
+        source
+            Source key in :attr:`solutions`.
+        target
+            Target key in :attr:`solutions`.
+        data
+            Initial data to pull, see :meth:`~moscot.base.problems.OTProblem.pull` for information.
+        subset
+            Pull values contained only within the subset.
+        scale_by_marginals
+            Whether to scale by the source :term:`marginals`.
+        key_added
+            Key in :attr:`~anndata.AnnData.obs` where to add the result.
+        return_all
+            Whether to also return intermediate results. Always true if ``key_added != None``.
+        kwargs
+            Keyword arguments for the subproblems' :meth:`~moscot.base.problems.OTProblem.pull` method.
+
+        Returns
+        -------
+        Depending on the ``key_added``:
+
+        - :obj:`None` - returns the result.
+        - :class:`str` - returns nothing and updates :attr:`obs['{key_added}'] <anndata.AnnData.obs>`
+          with the result.
+        """
+        result = self._apply(
+            source=source,
+            target=target,
+            data=data,
+            subset=subset,
+            forward=False,
+            return_all=return_all or key_added is not None,
+            scale_by_marginals=scale_by_marginals,
+            **kwargs,
+        )
+        if TYPE_CHECKING:
+            assert isinstance(result, dict)
+
+        if key_added is not None:
+            plot_vars = {
+                "key": self.batch_key,
+            }
+            self.adata.obs[key_added] = self._flatten(result, key=self.batch_key)
+            set_plotting_vars(self.adata, _constants.PULL, key=key_added, value=plot_vars)
+            return None
+        return result
+
+    @property
+    def batch_key(self: GenericAnalysisMixinProtocol[K, B]) -> Optional[str]:
+        """Batch key in :attr:`~anndata.AnnData.obs`."""
+        return self._batch_key
+
+    @batch_key.setter
+    def batch_key(self: GenericAnalysisMixinProtocol[K, B], key: Optional[str]) -> None:
+        if key is not None and key not in self.adata.obs:
+            raise KeyError(f"Unable to find batch data in `adata.obs[{key!r}]`.")
+        self._batch_key = key
```

### Comparing `moscot-0.3.0/src/moscot/_logging.py` & `moscot-0.3.1/src/moscot/_logging.py`

 * *Files identical despite different names*

### Comparing `moscot-0.3.0/src/moscot/_registry.py` & `moscot-0.3.1/src/moscot/_registry.py`

 * *Files identical despite different names*

### Comparing `moscot-0.3.0/src/moscot/_types.py` & `moscot-0.3.1/src/moscot/_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,39 +20,39 @@
 SinkFullRankInit = Literal["default", "gaussian", "sorting"]
 LRInitializer_t = Literal["random", "rank2", "k-means", "generalized-k-means"]
 
 SinkhornInitializer_t = Optional[Union[SinkFullRankInit, LRInitializer_t]]
 QuadInitializer_t = Optional[LRInitializer_t]
 
 Initializer_t = Union[SinkhornInitializer_t, LRInitializer_t]
-ProblemStage_t = Literal["initialized", "prepared", "solved"]
+ProblemStage_t = Literal["prepared", "solved"]
 Device_t = Union[Literal["cpu", "gpu", "tpu"], str]
 
 # TODO(michalk8): autogenerate from the enums
-ScaleCost_t = Optional[Union[float, Literal["mean", "max_cost", "max_bound", "max_norm", "median"]]]
+ScaleCost_t = Union[float, Literal["mean", "max_cost", "max_bound", "max_norm", "median"]]
 OttCostFn_t = Literal[
     "euclidean",
     "sq_euclidean",
     "cosine",
     "PNormP",
     "SqPNorm",
     "Euclidean",
     "SqEuclidean",
     "Cosine",
     "ElasticL1",
     "ElasticSTVS",
     "ElasticSqKOverlap",
 ]
-OttCostFnMap_t = Union[OttCostFn_t, Mapping[str, OttCostFn_t]]
+OttCostFnMap_t = Union[OttCostFn_t, Mapping[Literal["xy", "x", "y"], OttCostFn_t]]
 GenericCostFn_t = Literal["barcode_distance", "leaf_distance", "custom"]
 CostFn_t = Union[str, GenericCostFn_t, OttCostFn_t]
 CostFnMap_t = Union[Union[OttCostFn_t, GenericCostFn_t], Mapping[str, Union[OttCostFn_t, GenericCostFn_t]]]
 PathLike = Union[os.PathLike, str]
 Policy_t = Literal[
     "sequential",
     "star",
     "external_star",
+    "explicit",
     "triu",
     "tril",
-    "explicit",
 ]
 CostKwargs_t = Union[Mapping[str, Any], Mapping[Literal["x", "y", "xy"], Mapping[str, Any]]]
```

### Comparing `moscot-0.3.0/src/moscot/backends/ott/__init__.py` & `moscot-0.3.1/src/moscot/backends/ott/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from ott.geometry import costs
 
+from moscot.backends.ott._utils import sinkhorn_divergence
 from moscot.backends.ott.output import OTTOutput
 from moscot.backends.ott.solver import GWSolver, SinkhornSolver
 from moscot.costs import register_cost
 
-__all__ = ["OTTOutput", "GWSolver", "SinkhornSolver"]
+__all__ = ["OTTOutput", "GWSolver", "SinkhornSolver", "sinkhorn_divergence"]
 
 register_cost("euclidean", backend="ott")(costs.Euclidean)
 register_cost("sq_euclidean", backend="ott")(costs.SqEuclidean)
 register_cost("cosine", backend="ott")(costs.Cosine)
 register_cost("pnorm_p", backend="ott")(costs.PNormP)
 register_cost("sq_pnorm", backend="ott")(costs.SqPNorm)
 register_cost("elastic_l1", backend="ott")(costs.ElasticL1)
```

### Comparing `moscot-0.3.0/src/moscot/backends/ott/_utils.py` & `moscot-0.3.1/src/moscot/backends/ott/_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,87 @@
 from typing import Any, Optional
 
+import jax
 import jax.numpy as jnp
 import scipy.sparse as sp
-from ott.geometry.geometry import Geometry
-from ott.geometry.pointcloud import PointCloud
-from ott.tools.sinkhorn_divergence import sinkhorn_divergence
+from ott.geometry import geometry, pointcloud
+from ott.tools import sinkhorn_divergence as sdiv
 
 from moscot._logging import logger
 from moscot._types import ArrayLike, ScaleCost_t
 
+__all__ = ["sinkhorn_divergence"]
 
-def _compute_sinkhorn_divergence(
+
+def sinkhorn_divergence(
     point_cloud_1: ArrayLike,
     point_cloud_2: ArrayLike,
     a: Optional[ArrayLike] = None,
     b: Optional[ArrayLike] = None,
     epsilon: Optional[float] = 1e-1,
     scale_cost: ScaleCost_t = 1.0,
     **kwargs: Any,
 ) -> float:
     point_cloud_1 = jnp.asarray(point_cloud_1)
     point_cloud_2 = jnp.asarray(point_cloud_2)
     a = None if a is None else jnp.asarray(a)
     b = None if b is None else jnp.asarray(b)
 
-    output = sinkhorn_divergence(
-        PointCloud, x=point_cloud_1, y=point_cloud_2, a=a, b=b, epsilon=epsilon, scale_cost=scale_cost, **kwargs
+    output = sdiv.sinkhorn_divergence(
+        pointcloud.PointCloud,
+        x=point_cloud_1,
+        y=point_cloud_2,
+        a=a,
+        b=b,
+        epsilon=epsilon,
+        scale_cost=scale_cost,
+        **kwargs,
     )
     xy_conv, xx_conv, *yy_conv = output.converged
 
     if not xy_conv:
         logger.warning("Solver did not converge in the `x/y` term.")
     if not xx_conv:
         logger.warning("Solver did not converge in the `x/x` term.")
     if len(yy_conv) and not yy_conv[0]:
         logger.warning("Solver did not converge in the `y/y` term.")
 
     return float(output.divergence)
 
 
-def check_shapes(geom_x: Geometry, geom_y: Geometry, geom_xy: Geometry) -> None:
+def check_shapes(geom_x: geometry.Geometry, geom_y: geometry.Geometry, geom_xy: geometry.Geometry) -> None:
     n, m = geom_xy.shape
     n_, m_ = geom_x.shape[0], geom_y.shape[0]
     if n != n_:
         raise ValueError(f"Expected the first geometry to have `{n}` points, found `{n_}`.")
     if m != m_:
         raise ValueError(f"Expected the second geometry to have `{m}` points, found `{m_}`.")
 
 
 def alpha_to_fused_penalty(alpha: float) -> float:
+    """Convert."""
     if not (0 < alpha <= 1):
         raise ValueError(f"Expected `alpha` to be in interval `(0, 1]`, found `{alpha}`.")
     return (1 - alpha) / alpha
 
 
-def ensure_2d(arr: ArrayLike, *, reshape: bool = False) -> Optional[jnp.ndarray]:  # type: ignore[name-defined]
+def ensure_2d(arr: ArrayLike, *, reshape: bool = False) -> jax.Array:
+    """Ensure that an array is 2-dimensional.
+
+    Parameters
+    ----------
+    arr
+        Array to check.
+    reshape
+        Allow reshaping 1-dimensional array to ``[n, 1]``.
+
+    Returns
+    -------
+    2-dimensional :mod:`jax` array.
+    """
     if sp.issparse(arr):
         arr = arr.A  # type: ignore[attr-defined]
     arr = jnp.asarray(arr)
     if reshape and arr.ndim == 1:
         return jnp.reshape(arr, (-1, 1))
     if arr.ndim != 2:
         raise ValueError(f"Expected array to have 2 dimensions, found `{arr.ndim}`.")
```

### Comparing `moscot-0.3.0/src/moscot/backends/ott/output.py` & `moscot-0.3.1/src/moscot/backends/ott/output.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,114 +1,131 @@
 from typing import Any, Optional, Tuple, Union
 
 import jaxlib.xla_extension as xla_ext
 
 import jax
 import jax.numpy as jnp
 import numpy as np
-from ott.solvers.linear.sinkhorn import SinkhornOutput as OTTSinkhornOutput
-from ott.solvers.linear.sinkhorn_lr import LRSinkhornOutput as OTTLRSinkhornOutput
-from ott.solvers.quadratic.gromov_wasserstein import GWOutput as OTTGWOutput
+from ott.solvers.linear import sinkhorn, sinkhorn_lr
+from ott.solvers.quadratic import gromov_wasserstein
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 
-from moscot._docs._docs import d
 from moscot._types import ArrayLike, Device_t
 from moscot.base.output import BaseSolverOutput
 
 __all__ = ["OTTOutput"]
 
 
 class OTTOutput(BaseSolverOutput):
-    """Output of various optimal transport problems.
+    """Output of various :term:`OT` problems.
 
     Parameters
     ----------
     output
-        Output of :mod:`ott` backend.
+        Output of the :mod:`ott` backend.
     """
 
-    _NOT_COMPUTED = -1.0
+    _NOT_COMPUTED = -1.0  # sentinel value used in `ott`
 
-    def __init__(self, output: Union[OTTSinkhornOutput, OTTLRSinkhornOutput, OTTGWOutput]):
+    def __init__(
+        self, output: Union[sinkhorn.SinkhornOutput, sinkhorn_lr.LRSinkhornOutput, gromov_wasserstein.GWOutput]
+    ):
         super().__init__()
         self._output = output
-        self._costs = None if isinstance(output, OTTSinkhornOutput) else output.costs
+        self._costs = None if isinstance(output, sinkhorn.SinkhornOutput) else output.costs
         self._errors = output.errors
 
-    @d.get_sections(base="plot_costs", sections=["Parameters", "Returns"])
     def plot_costs(
         self,
         last: Optional[int] = None,
         title: Optional[str] = None,
         return_fig: bool = False,
+        ax: Optional[mpl.axes.Axes] = None,
         figsize: Optional[Tuple[float, float]] = None,
         dpi: Optional[int] = None,
         save: Optional[str] = None,
-        ax: Optional[mpl.axes.Axes] = None,
         **kwargs: Any,
     ) -> Optional[mpl.figure.Figure]:
-        """Plot regularized OT costs during the iterations.
+        """Plot regularized :term:`OT` costs during the iterations.
 
         Parameters
         ----------
         last
-            How many of the last steps of the algorithm to plot. If `None`, plot the full curve.
+            How many of the last steps of the algorithm to plot. If :obj:`None`, plot the full curve.
         title
-            Title of the plot. If `None`, it is determined automatically.
+            Title of the plot. If :obj:`None`, it is determined automatically.
+        return_fig
+            Whether to return the figure.
+        ax
+            Axes on which to plot.
         figsize
             Size of the figure.
         dpi
             Dots per inch.
         save
             Path where to save the figure.
-        return_fig
-            Whether to return the figure.
-        ax
-            Axes on which to plot.
         kwargs
-            Keyword arguments for :meth:`~matplotlib.axes.Axes.plot`.
+            Keyword arguments for :meth:`matplotlib.axes.Axes.plot`.
 
         Returns
         -------
-        The figure if ``return_fig = True``.
+        If ``return_fig = True``, return the figure.
         """
         if self._costs is None:
             raise RuntimeError("No costs to plot.")
 
         fig, ax = plt.subplots(figsize=figsize, dpi=dpi) if ax is None else (ax.get_figure(), ax)
         self._plot_lines(ax, np.asarray(self._costs), last=last, y_label="cost", title=title, **kwargs)
 
         if save is not None:
             fig.savefig(save)
         return fig if return_fig else None
 
-    @d.dedent
     def plot_errors(
         self,
         last: Optional[int] = None,
         title: Optional[str] = None,
         outer_iteration: int = -1,
         return_fig: bool = False,
         figsize: Optional[Tuple[float, float]] = None,
         dpi: Optional[int] = None,
         save: Optional[str] = None,
         ax: Optional[mpl.axes.Axes] = None,
         **kwargs: Any,
     ) -> Optional[mpl.figure.Figure]:
-        """Plot errors during the iterations.
+        """Plot errors along iterations.
 
         Parameters
         ----------
-        %(plot_costs.parameters)s
+        last
+            Number of errors corresponding at the ``last`` steps of the algorithm to plot. If :obj:`None`,
+            plot the full curve.
+        title
+            Title of the plot. If :obj:`None`, it is determined automatically.
+        outer_iteration
+            Which outermost iteration's errors to plot.
+            Only used when this is the solution to the :term:`quadratic problem`.
+        return_fig
+            Whether to return the figure.
+        ax
+            Axes on which to plot.
+        figsize
+            Size of the figure.
+        dpi
+            Dots per inch.
+        save
+            Path where to save the figure.
+        kwargs
+            Keyword arguments for :meth:`matplotlib.axes.Axes.plot`.
 
         Returns
         -------
-        %(plot_costs.returns)s
+        If ``return_fig = True``, return the figure.
         """
         if self._errors is None:
             raise RuntimeError("No errors to plot.")
 
         fig, ax = plt.subplots(figsize=figsize, dpi=dpi) if ax is None else (ax.get_figure(), ax)
         errors = np.asarray(self._errors)
         errors = errors[np.where(errors != self._NOT_COMPUTED)[0]]
@@ -151,27 +168,30 @@
     def _apply(self, x: ArrayLike, *, forward: bool) -> ArrayLike:
         if x.ndim == 1:
             return self._output.apply(x, axis=1 - forward)
         return self._output.apply(x.T, axis=1 - forward).T  # convert to batch first
 
     @property
     def shape(self) -> Tuple[int, int]:  # noqa: D102
-        if isinstance(self._output, OTTSinkhornOutput):
+        if isinstance(self._output, sinkhorn.SinkhornOutput):
             return self._output.f.shape[0], self._output.g.shape[0]
         return self._output.geom.shape
 
     @property
     def transport_matrix(self) -> ArrayLike:  # noqa: D102
         return self._output.matrix
 
     @property
     def is_linear(self) -> bool:  # noqa: D102
-        return isinstance(self._output, (OTTSinkhornOutput, OTTLRSinkhornOutput))
+        return isinstance(self._output, (sinkhorn.SinkhornOutput, sinkhorn_lr.LRSinkhornOutput))
 
     def to(self, device: Optional[Device_t] = None) -> "OTTOutput":  # noqa: D102
+        if device is None:
+            return OTTOutput(jax.device_put(self._output, device=device))
+
         if isinstance(device, str) and ":" in device:
             device, ix = device.split(":")
             idx = int(ix)
         else:
             idx = 0
 
         if not isinstance(device, xla_ext.Device):
@@ -180,28 +200,26 @@
             except IndexError:
                 raise IndexError(f"Unable to fetch the device with `id={idx}`.") from None
 
         return OTTOutput(jax.device_put(self._output, device))
 
     @property
     def cost(self) -> float:  # noqa: D102
-        if isinstance(self._output, (OTTSinkhornOutput, OTTLRSinkhornOutput)):
-            return float(self._output.reg_ot_cost)
-        return float(self._output.reg_gw_cost)
+        return float(self._output.reg_ot_cost if self.is_linear else self._output.reg_gw_cost)
 
     @property
     def converged(self) -> bool:  # noqa: D102
         return bool(self._output.converged)
 
     @property
     def potentials(self) -> Optional[Tuple[ArrayLike, ArrayLike]]:  # noqa: D102
-        if isinstance(self._output, OTTSinkhornOutput):
+        if isinstance(self._output, sinkhorn.SinkhornOutput):
             return self._output.f, self._output.g
         return None
 
     @property
     def rank(self) -> int:  # noqa: D102
         lin_output = self._output if self.is_linear else self._output.linear_state
-        return len(lin_output.g) if isinstance(lin_output, OTTLRSinkhornOutput) else -1
+        return len(lin_output.g) if isinstance(lin_output, sinkhorn_lr.LRSinkhornOutput) else -1
 
     def _ones(self, n: int) -> ArrayLike:  # noqa: D102
-        return jnp.ones((n,))  # type: ignore[return-value]
+        return jnp.ones((n,))
```

### Comparing `moscot-0.3.0/src/moscot/backends/ott/solver.py` & `moscot-0.3.1/src/moscot/backends/ott/solver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,59 +1,57 @@
 import abc
 import inspect
 import types
 from typing import Any, Literal, Mapping, Optional, Set, Tuple, Union
 
 import jax
-from ott.geometry import costs
-from ott.geometry.epsilon_scheduler import Epsilon
-from ott.geometry.geometry import Geometry
-from ott.geometry.pointcloud import PointCloud
-from ott.problems.linear.linear_problem import LinearProblem
-from ott.problems.quadratic.quadratic_problem import QuadraticProblem
-from ott.solvers.linear.sinkhorn import Sinkhorn
-from ott.solvers.linear.sinkhorn_lr import LRSinkhorn
-from ott.solvers.quadratic.gromov_wasserstein import GromovWasserstein
+from ott.geometry import costs, epsilon_scheduler, geometry, pointcloud
+from ott.problems.linear import linear_problem
+from ott.problems.quadratic import quadratic_problem
+from ott.solvers.linear import sinkhorn, sinkhorn_lr
+from ott.solvers.quadratic import gromov_wasserstein
 
 from moscot._types import ProblemKind_t, QuadInitializer_t, SinkhornInitializer_t
 from moscot.backends.ott._utils import alpha_to_fused_penalty, check_shapes, ensure_2d
 from moscot.backends.ott.output import OTTOutput
 from moscot.base.solver import OTSolver
 from moscot.costs import get_cost
 from moscot.utils.tagged_array import TaggedArray
 
 __all__ = ["SinkhornSolver", "GWSolver"]
 
+OTTSolver_t = Union[sinkhorn.Sinkhorn, sinkhorn_lr.LRSinkhorn, gromov_wasserstein.GromovWasserstein]
+OTTProblem_t = Union[linear_problem.LinearProblem, quadratic_problem.QuadraticProblem]
 Scale_t = Union[float, Literal["mean", "median", "max_cost", "max_norm", "max_bound"]]
 
 
 class OTTJaxSolver(OTSolver[OTTOutput], abc.ABC):
     """Base class for :mod:`ott` solvers :cite:`cuturi2022optimal`.
 
     Parameters
     ----------
     jit
-        Whether to jit the :attr:`solver`.
+        Whether to :func:`~jax.jit` the :attr:`solver`.
     """
 
     def __init__(self, jit: bool = True):
         super().__init__()
-        self._solver: Optional[Union[Sinkhorn, LRSinkhorn, GromovWasserstein]] = None
-        self._problem: Optional[Union[LinearProblem, QuadraticProblem]] = None
+        self._solver: Optional[OTTSolver_t] = None
+        self._problem: Optional[OTTProblem_t] = None
         self._jit = jit
 
     def _create_geometry(
         self,
         x: TaggedArray,
-        epsilon: Optional[Union[float, Epsilon]] = None,
+        epsilon: Optional[Union[float, epsilon_scheduler.Epsilon]] = None,
         relative_epsilon: Optional[bool] = None,
         scale_cost: Scale_t = 1.0,
         batch_size: Optional[int] = None,
         **kwargs: Any,
-    ) -> Geometry:
+    ) -> geometry.Geometry:
         if x.is_point_cloud:
             cost_fn = x.cost
             if cost_fn is None:
                 cost_fn = costs.SqEuclidean()
             elif isinstance(cost_fn, str):
                 cost_fn = get_cost(cost_fn, backend="ott", **kwargs)
             if not isinstance(cost_fn, costs.CostFn):
@@ -62,70 +60,74 @@
             y = None if x.data_tgt is None else ensure_2d(x.data_tgt, reshape=True)
             x = ensure_2d(x.data_src, reshape=True)
             if y is not None and x.shape[1] != y.shape[1]:
                 raise ValueError(
                     f"Expected `x/y` to have the same number of dimensions, found `{x.shape[1]}/{y.shape[1]}`."
                 )
 
-            return PointCloud(
+            return pointcloud.PointCloud(
                 x,
                 y=y,
                 cost_fn=cost_fn,
                 epsilon=epsilon,
                 relative_epsilon=relative_epsilon,
                 scale_cost=scale_cost,
                 batch_size=batch_size,
             )
 
         arr = ensure_2d(x.data_src, reshape=False)
         if x.is_cost_matrix:
-            return Geometry(cost_matrix=arr, epsilon=epsilon, relative_epsilon=relative_epsilon, scale_cost=scale_cost)
+            return geometry.Geometry(
+                cost_matrix=arr, epsilon=epsilon, relative_epsilon=relative_epsilon, scale_cost=scale_cost
+            )
         if x.is_kernel:
-            return Geometry(
+            return geometry.Geometry(
                 kernel_matrix=arr, epsilon=epsilon, relative_epsilon=relative_epsilon, scale_cost=scale_cost
             )
         raise NotImplementedError(f"Creating geometry from `tag={x.tag!r}` is not yet implemented.")
 
     def _solve(  # type: ignore[override]
         self,
-        prob: Union[LinearProblem, QuadraticProblem],
+        prob: OTTProblem_t,
         **kwargs: Any,
     ) -> OTTOutput:
         solver = jax.jit(self.solver) if self._jit else self.solver
         out = solver(prob, **kwargs)
         return OTTOutput(out)
 
     @property
-    def solver(self) -> Union[Sinkhorn, LRSinkhorn, GromovWasserstein]:
-        """Underlying :mod:`ott` solver."""
+    def solver(self) -> OTTSolver_t:
+        """:mod:`ott` solver."""
         return self._solver
 
     @property
     def rank(self) -> int:
         """Rank of the :attr:`solver`."""
         return getattr(self.solver, "rank", -1)
 
     @property
     def is_low_rank(self) -> bool:
         """Whether the :attr:`solver` is low-rank."""
         return self.rank > -1
 
 
 class SinkhornSolver(OTTJaxSolver):
-    """Linear optimal transport problem solver.
+    """Solver for the :term:`linear problem`.
 
-    The (Kantorovich relaxed) optimal transport problem is defined by two distributions in the same space.
+    The (Kantorovich relaxed) :term:`OT` problem is defined by two distributions in the same space.
     The aim is to obtain a probabilistic map from the source distribution to the target distribution such that
     the (weighted) sum of the distances between coupled data point in the source and the target distribution is
     minimized.
 
     Parameters
     ----------
+    jit
+        Whether to :func:`~jax.jit` the :attr:`solver`.
     rank
-        Rank of the linear solver. If `-1`, use :class:`~ott.solvers.linear.sinkhorn.Sinkhorn` :cite:`cuturi:2013`,
+        Rank of the solver. If `-1`, use :class:`~ott.solvers.linear.sinkhorn.Sinkhorn` :cite:`cuturi:2013`,
         otherwise, use :class:`~ott.solvers.linear.sinkhorn_lr.LRSinkhorn` :cite:`scetbon:21a`.
     epsilon
         Additional epsilon regularization for the low-rank approach.
     initializer
         Initializer for :class:`~ott.solvers.linear.sinkhorn.Sinkhorn` or
         :class:`~ott.solvers.linear.sinkhorn_lr.LRSinkhorn`, depending on the ``rank``.
     initializer_kwargs
@@ -145,86 +147,88 @@
         **kwargs: Any,
     ):
         super().__init__(jit=jit)
         if rank > -1:
             kwargs.setdefault("gamma", 10)
             kwargs.setdefault("gamma_rescale", True)
             initializer = "rank2" if initializer is None else initializer
-            self._solver = LRSinkhorn(
+            self._solver = sinkhorn_lr.LRSinkhorn(
                 rank=rank, epsilon=epsilon, initializer=initializer, kwargs_init=initializer_kwargs, **kwargs
             )
         else:
             initializer = "default" if initializer is None else initializer
-            self._solver = Sinkhorn(initializer=initializer, kwargs_init=initializer_kwargs, **kwargs)
+            self._solver = sinkhorn.Sinkhorn(initializer=initializer, kwargs_init=initializer_kwargs, **kwargs)
 
     def _prepare(
         self,
         xy: Optional[TaggedArray] = None,
         x: Optional[TaggedArray] = None,
         y: Optional[TaggedArray] = None,
         # geometry
-        epsilon: Optional[Union[float, Epsilon]] = None,
+        epsilon: Optional[Union[float, epsilon_scheduler.Epsilon]] = None,
         relative_epsilon: Optional[bool] = None,
         batch_size: Optional[int] = None,
         scale_cost: Scale_t = 1.0,
         cost_kwargs: Mapping[str, Any] = types.MappingProxyType({}),
         cost_matrix_rank: Optional[int] = None,
         # problem
         **kwargs: Any,
-    ) -> LinearProblem:
+    ) -> linear_problem.LinearProblem:
         del x, y
         if xy is None:
             raise ValueError(f"Unable to create geometry from `xy={xy}`.")
 
         geom = self._create_geometry(
             xy,
             epsilon=epsilon,
             relative_epsilon=relative_epsilon,
             batch_size=batch_size,
             scale_cost=scale_cost,
             **cost_kwargs,
         )
         if cost_matrix_rank is not None:
             geom = geom.to_LRCGeometry(rank=cost_matrix_rank)
-        self._problem = LinearProblem(geom, **kwargs)
+        self._problem = linear_problem.LinearProblem(geom, **kwargs)
         return self._problem
 
     @property
-    def xy(self) -> Optional[Geometry]:
+    def xy(self) -> Optional[geometry.Geometry]:
         """Geometry defining the linear term."""
         return None if self._problem is None else self._problem.geom
 
     @property
     def problem_kind(self) -> ProblemKind_t:  # noqa: D102
         return "linear"
 
     @classmethod
     def _call_kwargs(cls) -> Tuple[Set[str], Set[str]]:
         geom_kwargs = {"epsilon", "relative_epsilon", "batch_size", "scale_cost", "cost_kwargs", "cost_matrix_rank"}
-        problem_kwargs = set(inspect.signature(LinearProblem).parameters.keys())
+        problem_kwargs = set(inspect.signature(linear_problem.LinearProblem).parameters.keys())
         problem_kwargs -= {"geom"}
         return geom_kwargs | problem_kwargs, {"epsilon"}
 
 
 class GWSolver(OTTJaxSolver):
-    """Solver solving quadratic optimal transport problem.
+    """Solver for the :term:`quadratic problem` :cite:`memoli:2011`.
 
-    The Gromov-Wasserstein (GW) problem involves two distribution in possibly two different spaces.
-    Points in the source distribution are matched to points in the target distribution by comparing the relative
-    location of the points within each distribution.
+    The :term:`Gromov-Wasserstein (GW) <Gromov-Wasserstein>` problem involves two distribution in
+    possibly two different spaces. Points in the source distribution are matched to points in the target distribution
+    by comparing the relative location of the points within each distribution.
 
     Parameters
     ----------
+    jit
+        Whether to :func:`~jax.jit` the :attr:`solver`.
     rank
-        Rank of the quadratic solver. If `-1` use the full-rank GW :cite:`memoli:2011`,
+        Rank of the solver. If `-1` use the full-rank :term:`GW <Gromov-Wasserstein>` :cite:`peyre:2016`,
         otherwise, use the low-rank approach :cite:`scetbon:21b`.
     initializer
         Initializer for :class:`~ott.solvers.quadratic.gromov_wasserstein.GromovWasserstein`.
     initializer_kwargs
-        Keyword arguments for the initializer.
+        Keyword arguments for the ``initializer``.
     linear_solver_kwargs
         Keyword arguments for :class:`~ott.solvers.linear.sinkhorn.Sinkhorn` or
         :class:`~ott.solvers.linear.sinkhorn_lr.LRSinkhorn`, depending on the ``rank``.
     kwargs
         Keyword arguments for :class:`~ott.solvers.quadratic.gromov_wasserstein.GromovWasserstein` .
     """
 
@@ -238,43 +242,43 @@
         **kwargs: Any,
     ):
         super().__init__(jit=jit)
         if rank > -1:
             linear_solver_kwargs = dict(linear_solver_kwargs)
             linear_solver_kwargs.setdefault("gamma", 10)
             linear_solver_kwargs.setdefault("gamma_rescale", True)
-            linear_ot_solver = LRSinkhorn(rank=rank, **linear_solver_kwargs)
+            linear_ot_solver = sinkhorn_lr.LRSinkhorn(rank=rank, **linear_solver_kwargs)
             initializer = "rank2" if initializer is None else initializer
         else:
-            linear_ot_solver = Sinkhorn(**linear_solver_kwargs)
+            linear_ot_solver = sinkhorn.Sinkhorn(**linear_solver_kwargs)
             initializer = None
-        self._solver = GromovWasserstein(
+        self._solver = gromov_wasserstein.GromovWasserstein(
             rank=rank,
             linear_ot_solver=linear_ot_solver,
             quad_initializer=initializer,
             kwargs_init=initializer_kwargs,
             **kwargs,
         )
 
     def _prepare(
         self,
         xy: Optional[TaggedArray] = None,
         x: Optional[TaggedArray] = None,
         y: Optional[TaggedArray] = None,
         # geometry
-        epsilon: Optional[Union[float, Epsilon]] = None,
+        epsilon: Optional[Union[float, epsilon_scheduler.Epsilon]] = None,
         relative_epsilon: Optional[bool] = None,
         batch_size: Optional[int] = None,
         scale_cost: Scale_t = 1.0,
         cost_kwargs: Mapping[str, Any] = types.MappingProxyType({}),
         cost_matrix_rank: Optional[int] = None,
         # problem
         alpha: float = 0.5,
         **kwargs: Any,
-    ) -> QuadraticProblem:
+    ) -> quadratic_problem.QuadraticProblem:
         if x is None or y is None:
             raise ValueError(f"Unable to create geometry from `x={x}`, `y={y}`.")
         geom_kwargs: Any = {
             "epsilon": epsilon,
             "relative_epsilon": relative_epsilon,
             "batch_size": batch_size,
             "scale_cost": scale_cost,
@@ -287,41 +291,43 @@
             # arbitrary fused penalty; must be positive
             geom_xy, fused_penalty = None, 1.0
         else:  # FGW
             fused_penalty = alpha_to_fused_penalty(alpha)
             geom_xy = self._create_geometry(xy, **geom_kwargs)
             check_shapes(geom_xx, geom_yy, geom_xy)
 
-        self._problem = QuadraticProblem(geom_xx, geom_yy, geom_xy, fused_penalty=fused_penalty, **kwargs)
+        self._problem = quadratic_problem.QuadraticProblem(
+            geom_xx, geom_yy, geom_xy, fused_penalty=fused_penalty, **kwargs
+        )
         return self._problem
 
     @property
-    def x(self) -> Optional[Geometry]:
-        """First geometry defining the quadratic term."""
+    def x(self) -> Optional[geometry.Geometry]:
+        """The first geometry defining the quadratic term."""
         return None if self._problem is None else self._problem.geom_xx
 
     @property
-    def y(self) -> Geometry:
-        """Second geometry defining the quadratic term."""
+    def y(self) -> geometry.Geometry:
+        """The second geometry defining the quadratic term."""
         return None if self._problem is None else self._problem.geom_yy
 
     @property
-    def xy(self) -> Optional[Geometry]:
-        """Geometry defining the linear term in the fused case."""
+    def xy(self) -> Optional[geometry.Geometry]:
+        """Geometry defining the linear term in the :term:`FGW <fused Gromov-Wasserstein>`."""
         return None if self._problem is None else self._problem.geom_xy
 
     @property
     def is_fused(self) -> Optional[bool]:
-        """Whether the problem is fused."""
+        """Whether the solver is fused."""
         return None if self._problem is None else (self.xy is not None)
 
     @property
     def problem_kind(self) -> ProblemKind_t:  # noqa: D102
         return "quadratic"
 
     @classmethod
     def _call_kwargs(cls) -> Tuple[Set[str], Set[str]]:
         geom_kwargs = {"epsilon", "relative_epsilon", "batch_size", "scale_cost", "cost_kwargs", "cost_matrix_rank"}
-        problem_kwargs = set(inspect.signature(QuadraticProblem).parameters.keys())
+        problem_kwargs = set(inspect.signature(quadratic_problem.QuadraticProblem).parameters.keys())
         problem_kwargs -= {"geom_xx", "geom_yy", "geom_xy", "fused_penalty"}
         problem_kwargs |= {"alpha"}
         return geom_kwargs | problem_kwargs, {"epsilon"}
```

### Comparing `moscot-0.3.0/src/moscot/backends/utils.py` & `moscot-0.3.1/src/moscot/backends/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, Any, Literal, Tuple, Type, Union
+from typing import TYPE_CHECKING, Any, Callable, Literal, Tuple, Type, Union
 
 from moscot import _registry
 from moscot._types import ProblemKind_t
 
 if TYPE_CHECKING:
     from moscot.backends import ott
 
@@ -16,26 +16,38 @@
     """TODO."""
     if backend not in _REGISTRY:
         raise ValueError(f"Backend `{backend!r}` is not available.")
     solver_class = _REGISTRY[backend](problem_kind)
     return solver_class if return_class else solver_class(**kwargs)
 
 
-def register_solver(backend: str) -> Any:
-    """TODO."""
-    return _REGISTRY.register(backend)
+def register_solver(
+    backend: str,
+) -> Callable[[Literal["linear", "quadratic"]], Union[Type["ott.SinkhornSolver"], Type["ott.GWSolver"]]]:
+    """Register a solver for a specific backend.
+
+    Parameters
+    ----------
+    backend
+        Name of the backend.
+
+    Returns
+    -------
+    The decorated function which returns the type of the solver.
+    """
+    return _REGISTRY.register(backend)  # type: ignore[return-value]
 
 
-@register_solver("ott")
+@register_solver("ott")  # type: ignore[arg-type]
 def _(problem_kind: Literal["linear", "quadratic"]) -> Union[Type["ott.SinkhornSolver"], Type["ott.GWSolver"]]:
     from moscot.backends import ott
 
     if problem_kind == "linear":
         return ott.SinkhornSolver
     if problem_kind == "quadratic":
         return ott.GWSolver
     raise NotImplementedError(f"Unable to create solver for `{problem_kind!r}` problem.")
 
 
 def get_available_backends() -> Tuple[str, ...]:
-    """TODO."""
+    """Return all available backends."""
     return tuple(backend for backend in _REGISTRY)
```

### Comparing `moscot-0.3.0/src/moscot/base/cost.py` & `moscot-0.3.1/src/moscot/base/cost.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,69 @@
-from abc import ABC, abstractmethod
-from typing import Any, Tuple, Union
+import abc
+from typing import Any, Optional, Tuple, Union
 
 import numpy as np
 
 from anndata import AnnData
 
 from moscot._logging import logger
 from moscot._types import ArrayLike
 
 __all__ = ["BaseCost"]
 
 
-class BaseCost(ABC):
-    """Base class for all :mod:`moscot.costs`.
+class BaseCost(abc.ABC):
+    """Base class for :mod:`moscot.costs`.
 
     Parameters
     ----------
     adata
         Annotated data object.
     attr
-        Attribute of :class:`~anndata.AnnData` used when computing the cost.
+        Attribute of :class:`~anndata.AnnData`.
     key
-        Key in the ``attr`` of :class:`~anndata.AnnData` used when computing the cost.
+        Key in the attribute of :class:`~anndata.AnnData`.
     dist_key
-        Helper key which determines which distribution :attr:`adata` belongs to.
+        Key which determines into which source/target subset ``adata`` belongs.
+        Useful when :attr:`attr = 'uns' <anndata.AnnData.uns>`.
     """
 
-    def __init__(self, adata: AnnData, attr: str, key: str, dist_key: Union[Any, Tuple[Any, Any]]):
+    def __init__(self, adata: AnnData, attr: str, key: str, dist_key: Optional[Union[Any, Tuple[Any, Any]]] = None):
         self._adata = adata
         self._attr = attr
         self._key = key
         self._dist_key = dist_key
 
-    @abstractmethod
+    @abc.abstractmethod
     def _compute(self, *args: Any, **kwargs: Any) -> ArrayLike:
         pass
 
     def __call__(self, *args: Any, **kwargs: Any) -> ArrayLike:
-        """Compute a cost matrix from :attr:`adata`.
+        """Compute the cost matrix.
 
         Parameters
         ----------
         args
-            Positional arguments for computation.
+            Positional arguments.
         kwargs
-            Keyword arguments for computation.
+            Keyword arguments.
 
         Returns
         -------
-        The computed cost matrix.
+        The cost matrix.
         """
         cost = self._compute(*args, **kwargs)
         if np.any(np.isnan(cost)):
             maxx = np.nanmax(cost)
-            logger.warning(f"Cost matrix contains `NaN` values, setting them to the maximum value `{maxx}`.")
+            logger.warning(
+                f"Cost matrix contains `{np.sum(np.isnan(cost))}` NaN values, "
+                f"setting them to the maximum value `{maxx}`."
+            )
             cost = np.nan_to_num(cost, nan=maxx)  # type: ignore[call-overload]
         if np.any(cost < 0):
-            raise ValueError("Cost matrix contains negative values.")
+            raise ValueError(f"Cost matrix contains `{np.sum(cost < 0)}` negative values.")
         return cost
 
     @property
     def adata(self) -> AnnData:
         """Annotated data object."""
         return self._adata
-
-    # TODO(michalk8): don't require impl.
-    @property
-    @abstractmethod
-    def data(self) -> Any:
-        """Container containing the data."""
```

### Comparing `moscot-0.3.0/src/moscot/base/output.py` & `moscot-0.3.1/src/moscot/base/output.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,92 +1,89 @@
-from abc import ABC, abstractmethod
-from copy import copy
-from functools import partial
-from typing import Any, Callable, Iterable, List, Literal, Optional, Tuple
+import abc
+import copy
+import functools
+from typing import Any, Callable, Iterable, List, Literal, Optional, Tuple, Union
 
 import numpy as np
 import scipy.sparse as sp
 from scipy.sparse.linalg import LinearOperator
 
-from moscot._docs._docs import d
 from moscot._logging import logger
 from moscot._types import ArrayLike, Device_t, DTypeLike  # type: ignore[attr-defined]
 
 __all__ = ["BaseSolverOutput", "MatrixSolverOutput"]
 
 
-@d.dedent
-class BaseSolverOutput(ABC):
+class BaseSolverOutput(abc.ABC):
     """Base class for all solver outputs."""
 
-    @abstractmethod
+    @abc.abstractmethod
     def _apply(self, x: ArrayLike, *, forward: bool) -> ArrayLike:
-        pass
+        """Apply :attr:`transport_matrix` to an array of shape ``[n, d]`` or ``[m, d]``."""
 
     @property
-    @abstractmethod
+    @abc.abstractmethod
     def transport_matrix(self) -> ArrayLike:
         """Transport matrix of shape ``[n, m]``."""
 
     @property
-    @abstractmethod
+    @abc.abstractmethod
     def shape(self) -> Tuple[int, int]:
         """Shape of the :attr:`transport_matrix`."""
 
     @property
-    @abstractmethod
+    @abc.abstractmethod
     def cost(self) -> float:
-        """Regularized optimal transport cost."""
+        """Regularized :term:`OT` cost."""
 
     @property
-    @abstractmethod
+    @abc.abstractmethod
     def converged(self) -> bool:
-        """Whether the algorithm converged."""
+        """Whether the solver converged."""
 
     @property
-    @abstractmethod
+    @abc.abstractmethod
     def potentials(self) -> Optional[Tuple[ArrayLike, ArrayLike]]:
-        """Dual potentials :math:`f` and :math:`g`.
+        """:term:`Dual potentials` :math:`f` and :math:`g`.
 
-        Only valid for the Sinkhorn algorithm.
+        Only valid for the :term:`Sinkhorn` algorithm.
         """
 
     @property
-    @abstractmethod
+    @abc.abstractmethod
     def is_linear(self) -> bool:
-        """Whether the output is linear."""
+        """Whether the output is a solution to a :term:`linear problem`."""
 
-    @abstractmethod
+    @abc.abstractmethod
     def to(self, device: Optional[Device_t] = None) -> "BaseSolverOutput":
-        """Transfer self to another device using :func:`jax.device_put`.
+        """Transfer self to another compute device.
 
         Parameters
         ----------
         device
-            Device where to transfer the solver output. If `None`, use the default device.
+            Device where to transfer the solver output. If :obj:`None`, use the default device.
 
         Returns
         -------
         Self transferred to the ``device``.
         """
 
     @property
     def rank(self) -> int:
         """Rank of the :attr:`transport_matrix`."""
         return -1
 
     @property
     def is_low_rank(self) -> bool:
-        """Whether the :attr:`transport_matrix` is low-rank."""
+        """Whether the :attr:`transport_matrix` is :term:`low-rank`."""
         return self.rank > -1
 
-    # TODO(michalk8): mention in docs it needs to be broadcastable
-    @abstractmethod
+    @abc.abstractmethod
     def _ones(self, n: int) -> ArrayLike:
-        pass
+        """Generate vector of 1s of shape ``[n,]``."""
 
     def push(self, x: ArrayLike, scale_by_marginals: bool = False) -> ArrayLike:
         """Push mass through the :attr:`transport_matrix`.
 
         It is equivalent to :math:`T^T x` but without instantiating the transport matrix :math:`T`, if possible.
 
         Parameters
@@ -94,15 +91,15 @@
         x
             Array of shape ``[n,]`` or ``[n, d]`` to push.
         scale_by_marginals
             Whether to scale by the source marginals :attr:`a`.
 
         Returns
         -------
-        Array of shape ``[m,]`` or ``[m, d]``, depending on ``x``.
+        Array of shape ``[m,]`` or ``[m, d]``, depending on the shape of ``x``.
         """
         if x.ndim not in (1, 2):
             raise ValueError(f"Expected 1D or 2D array, found `{x.ndim}`.")
         if x.shape[0] != self.shape[0]:
             raise ValueError(f"Expected array to have shape `({self.shape[0]}, ...)`, found `{x.shape}`.")
         if scale_by_marginals:
             x = self._scale_by_marginals(x, forward=True)
@@ -118,15 +115,15 @@
         x
             Array of shape ``[m,]`` or ``[m, d]`` to pull.
         scale_by_marginals
             Whether to scale by the target marginals :attr:`b`.
 
         Returns
         -------
-        Array of shape ``[n,]`` or ``[n, d]``, depending on ``x``.
+        Array of shape ``[n,]`` or ``[n, d]``, depending on the shape of ``x``.
         """
         if x.ndim not in (1, 2):
             raise ValueError(f"Expected 1D or 2D array, found `{x.ndim}`.")
         if x.shape[0] != self.shape[1]:
             raise ValueError(f"Expected array to have shape `({self.shape[1]}, ...)`, found `{x.shape}`.")
         if scale_by_marginals:
             x = self._scale_by_marginals(x, forward=False)
@@ -134,35 +131,35 @@
 
     def as_linear_operator(self, scale_by_marginals: bool = False) -> LinearOperator:
         """Transform :attr:`transport_matrix` into a linear operator.
 
         Parameters
         ----------
         scale_by_marginals
-            Whether to scale by marginals.
+            Whether to scale by :term:`marginals`.
 
         Returns
         -------
         The :attr:`transport_matrix` as a linear operator.
         """
-        push = partial(self.push, scale_by_marginals=scale_by_marginals)
-        pull = partial(self.pull, scale_by_marginals=scale_by_marginals)
+        push = functools.partial(self.push, scale_by_marginals=scale_by_marginals)
+        pull = functools.partial(self.pull, scale_by_marginals=scale_by_marginals)
         # push: a @ X (rmatvec)
         # pull: X @ a (matvec)
         return LinearOperator(shape=self.shape, dtype=self.dtype, matvec=pull, rmatvec=push)
 
     def chain(self, outputs: Iterable["BaseSolverOutput"], scale_by_marginals: bool = False) -> LinearOperator:
         """Chain subsequent applications of :attr:`transport_matrix`.
 
         Parameters
         ----------
         outputs
             Sequence of transport matrices to chain.
         scale_by_marginals
-            Whether to scale by marginals.
+            Whether to scale by :term:`marginals`.
 
         Returns
         -------
         The chained transport matrices as a linear operator.
         """
         op = self.as_linear_operator(scale_by_marginals)
         for out in outputs:
@@ -176,101 +173,97 @@
         value: Optional[float] = None,
         batch_size: int = 1024,
         n_samples: Optional[int] = None,
         seed: Optional[int] = None,
     ) -> "MatrixSolverOutput":
         """Sparsify the :attr:`transport_matrix`.
 
-        This function sets all entries of the transport matrix below `threshold` to 0 and
-        returns an instance of the `MatrixSolverOutput` with the
-        sparsified transport matrix stored as a :class:`~scipy.sparse.csr_matrix`.
+        This function sets all entries of the transport matrix below a certain threshold to :math:`0` and
+        returns a :class:`~moscot.base.output.MatrixSolverOutput` with sparsified transport matrix stored
+        as a :class:`~scipy.sparse.csr_matrix`.
 
         .. warning::
-            This function only serves for interfacing software which has to instantiate the transport matrix. Methods in
-            :mod:`moscot` never use the sparsified transport matrix.
+            This function only serves for interfacing software which has to instantiate the transport matrix,
+            :mod:`moscot` never uses the sparsified transport matrix.
 
         Parameters
         ----------
         mode
-            How to determine the value below which entries are set to 0:
-
-                - 'threshold' - threshold below which entries are set to 0.
-                - 'percentile' - determine threshold by percentile below which entries are set to 0. Hence, between 0
-                  and 100.
-                - 'min_row' - choose the threshold such that each row has at least one non-zero entry.
+            How to determine the value below which entries are set to :math:`0`. Valid options are:
 
+            - `'threshold'` - ``value`` is the threshold below which entries are set to :math:`0`.
+            - `'percentile'` - ``value`` is the percentile in :math:`[0, 100]` of the :attr:`transport_matrix`.
+              below which entries are set to :math:`0`.
+            - `'min_row'` - ``value`` is not used, it is chosen such that each row has at least 1 non-zero entry.
         value
-            Value to use for sparsification depending on ``mode``:
-
-                - `'threshold'` - `value` sets the threshold below which entries are set to 0.
-                - `percentile` - `value` is the percentile below which entries are set to 0.
-                - `min_row` - `value` is not used.
+            Value to use for sparsification.
         batch_size
-            How many rows of the transport matrix to sparsify per batch.
+            How many rows to materialize when sparsifying the :attr:`transport_matrix`.
         n_samples
-            If ``mode = 'percentile'``, determine the number of samples based on which the percentile
-            is computed stochastically. Note this means that a matrix of shape
-            `[n_samples, min(transport_matrix.shape)]` has to be instantiated. If `None`, ``n_samples`` is set to
-            ``batch_size``.
+            If ``mode = 'percentile'``, determine the number of samples based on which the percentile is computed
+            stochastically. Note this means that a matrix of shape `[n_samples, min(transport_matrix.shape)]`
+            has to be instantiated. If `None`, ``n_samples`` is set to ``batch_size``.
         seed
             Random seed needed for sampling if ``mode = 'percentile'``.
 
         Returns
         -------
-        Solve output with a sparsified transport matrix.
+        Output with sparsified transport matrix.
         """
         n, m = self.shape
         if mode == "threshold":
             if value is None:
-                raise ValueError("If `mode` is `threshold`, `threshold` must not be `None`.")
+                raise ValueError("If `mode = 'threshold'`, `threshold` cannot be `None`.")
             thr = value
         elif mode == "percentile":
             if value is None:
-                raise ValueError("If `mode` is `percentile`, `threshold` must not be `None`.")
+                raise ValueError("If `mode = 'percentile'`, `threshold` cannot be `None`.")
             rng = np.random.RandomState(seed=seed)
             n_samples = n_samples if n_samples is not None else batch_size
             k = min(n_samples, n)
             x = np.zeros((m, k))
             rows = rng.choice(m, size=k)
             x[rows, np.arange(k)] = 1.0
             res = self.pull(x, scale_by_marginals=False)  # tmap @ indicator_vectors
             thr = np.percentile(res, value)
         elif mode == "min_row":
             thr = np.inf
             for batch in range(0, m, batch_size):
                 x = np.eye(m, min(batch_size, m - batch), -(min(batch, m)))
                 res = self.pull(x, scale_by_marginals=False)  # tmap @ indicator_vectors
-                thr = min(thr, res.max(axis=1).min())
+                thr = min(thr, float(res.max(axis=1).min()))
         else:
-            raise NotImplementedError(mode)
+            raise NotImplementedError(f"Mode `{mode}` is not yet implemented.")
 
         k, func, fn_stack = (n, self.push, sp.vstack) if n < m else (m, self.pull, sp.hstack)
         tmaps_sparse: List[sp.csr_matrix] = []
+
         for batch in range(0, k, batch_size):
-            x = np.eye(k, min(batch_size, k - batch), -(min(batch, k)))
-            res = func(x, scale_by_marginals=False)
-            res[res < thr] = 0
+            x = np.eye(k, min(batch_size, k - batch), -(min(batch, k)), dtype=float)
+            res = np.array(func(x, scale_by_marginals=False))
+            res[res < thr] = 0.0
             tmaps_sparse.append(sp.csr_matrix(res.T if n < m else res))
+
         return MatrixSolverOutput(
             transport_matrix=fn_stack(tmaps_sparse), cost=self.cost, converged=self.converged, is_linear=self.is_linear
         )
 
     @property
     def a(self) -> ArrayLike:
-        """Marginals of the source distribution.
+        """:term:`Marginals` of the source distribution.
 
-        If the output of an unbalanced OT problem, these are the posterior marginals.
+        If the output of an :term:`unbalanced OT problem`, these are the posterior marginals.
         """
         return self.pull(self._ones(self.shape[1]))
 
     @property
     def b(self) -> ArrayLike:
-        """Marginals of the target distribution.
+        """:term:`Marginals` of the target distribution.
 
-        If the output of an unbalanced OT problem, these are the posterior marginals.
+        If the output of an :term:`unbalanced OT problem`, these are the posterior marginals.
         """
         return self.push(self._ones(self.shape[0]))
 
     @property
     def dtype(self) -> DTypeLike:
         """Underlying data type."""
         return self.a.dtype
@@ -293,31 +286,36 @@
         return f"{self.__class__.__name__}[{self._format_params(repr)}]"
 
     def __str__(self) -> str:
         return f"{self.__class__.__name__}[{self._format_params(str)}]"
 
 
 class MatrixSolverOutput(BaseSolverOutput):
-    """Optimal transport output with materialized `transport_matrix`.
+    """:term:`OT` solution with a materialized transport matrix.
 
     Parameters
     ----------
     transport_matrix
         Transport matrix of shape ``[n, m]``.
     cost
-        TODO
+        Cost of an :term:`OT` problem.
     converged
-        TODO.
+        Whether the solution converged.
     is_linear
-        TODO.
+        Whether this is a solution to a :term:`linear problem`.
     """
 
     # TODO(michalk8): don't provide defaults?
     def __init__(
-        self, transport_matrix: ArrayLike, *, cost: float = np.nan, converged: bool = True, is_linear: bool = True
+        self,
+        transport_matrix: Union[ArrayLike, sp.spmatrix],
+        *,
+        cost: float = np.nan,
+        converged: bool = True,
+        is_linear: bool = True,
     ):
         super().__init__()
         self._transport_matrix = transport_matrix
         self._cost = cost
         self._converged = converged
         self._is_linear = is_linear
 
@@ -338,15 +336,15 @@
         self, device: Optional[Device_t] = None, dtype: Optional[DTypeLike] = None
     ) -> "BaseSolverOutput":
         if device is not None:
             logger.warning(f"`{self!r}` does not support the `device` argument, ignoring.")
         if dtype is None:
             return self
 
-        obj = copy(self)
+        obj = copy.copy(self)
         obj._transport_matrix = obj.transport_matrix.astype(dtype)
         return obj
 
     @property
     def cost(self) -> float:  # noqa: D102
         return self._cost
```

### Comparing `moscot-0.3.0/src/moscot/base/problems/__init__.py` & `moscot-0.3.1/src/moscot/base/problems/__init__.py`

 * *Files identical despite different names*

### Comparing `moscot-0.3.0/src/moscot/base/problems/_mixins.py` & `moscot-0.3.1/src/moscot/base/problems/_mixins.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 import pandas as pd
 from scipy.sparse.linalg import LinearOperator
 
 import scanpy as sc
 from anndata import AnnData
 
 from moscot import _constants
-from moscot._docs._docs import d
 from moscot._types import ArrayLike, Numeric_t, Str_Dict_t
 from moscot.base.output import BaseSolverOutput
 from moscot.base.problems._utils import (
     _check_argument_compatibility_cell_transition,
     _correlation_test,
     _get_df_cell_transition,
     _order_transition_matrix,
@@ -113,15 +112,17 @@
         source_groups: Str_Dict_t,
         target_groups: Str_Dict_t,
         aggregation_mode: Literal["annotation", "cell"] = "annotation",
         key_added: Optional[str] = _constants.CELL_TRANSITION,
         **kwargs: Any,
     ) -> pd.DataFrame:
         if aggregation_mode == "annotation" and (source_groups is None or target_groups is None):
-            raise ValueError("If `aggregation_mode=annotation`, `source_groups` and `target_groups` cannot be `None`.")
+            raise ValueError(
+                "If `aggregation_mode='annotation'`, `source_groups` and `target_groups` cannot be `None`."
+            )
         if aggregation_mode == "cell" and source_groups is None and target_groups is None:
             raise ValueError("At least one of `source_groups` and `target_group` must be specified.")
 
         _check_argument_compatibility_cell_transition(
             source_annotation=source_groups,
             target_annotation=target_groups,
             aggregation_mode=aggregation_mode,
@@ -136,19 +137,19 @@
             **kwargs,
         )
         if key_added is not None:
             forward = kwargs.pop("forward")
             if aggregation_mode == "cell" and "cell" in self.adata.obs:
                 raise KeyError(f"Aggregation is already present in `adata.obs[{aggregation_mode!r}]`.")
             plot_vars = {
-                "transition_matrix": tm,
                 "source": source,
                 "target": target,
                 "source_groups": source_groups if (not forward or aggregation_mode == "annotation") else "cell",
                 "target_groups": target_groups if (forward or aggregation_mode == "annotation") else "cell",
+                "transition_matrix": tm,
             }
             set_plotting_vars(
                 self.adata,
                 _constants.CELL_TRANSITION,
                 key=key_added,
                 value=plot_vars,
             )
@@ -391,15 +392,14 @@
                 data=annotation_key,
                 subset=subset,
                 normalize=True,
                 return_all=False,
                 scale_by_marginals=False,
                 split_mass=False,
                 key_added=None,
-                return_data=True,
             )
             df["distribution"] = result
             cell_dist = df[df[annotation_key].isin(annotations_2)].groupby(annotation_key).sum(numeric_only=True)
             cell_dist /= cell_dist.sum()
             tm.loc[subset, :] = [
                 cell_dist.loc[annotation, "distribution"] if annotation in cell_dist.distribution.index else 0
                 for annotation in annotations_2
@@ -430,112 +430,112 @@
                 data=None,
                 subset=(batch, batch_size),
                 normalize=True,
                 return_all=False,
                 scale_by_marginals=False,
                 split_mass=True,
                 key_added=None,
-                return_data=True,
             )
             current_cells = df_2.iloc[range(batch, min(batch + batch_size, len(df_2)))].index.tolist()
             df_1.loc[:, current_cells] = result
             to_app = df_1[df_1[annotation_key].isin(annotations_2)].groupby(annotation_key).sum().transpose()
             tm = pd.concat([tm, to_app], verify_integrity=True, axis=0)
             df_1 = df_1.drop(current_cells, axis=1)
         return tm
 
-    # adapted from CellRank (github.com/theislab/cellrank)
-    @d.dedent
+    # adapted from:
+    # https://github.com/theislab/cellrank/blob/master/cellrank/_utils/_utils.py#L392
     def compute_feature_correlation(
         self: AnalysisMixinProtocol[K, B],
         obs_key: str,
         corr_method: Literal["pearson", "spearman"] = "pearson",
-        significance_method: Literal["fischer", "perm_test"] = "fischer",
+        significance_method: Literal["fisher", "perm_test"] = "fisher",
         annotation: Optional[Dict[str, Iterable[str]]] = None,
         layer: Optional[str] = None,
         features: Optional[Union[List[str], Literal["human", "mouse", "drosophila"]]] = None,
         confidence_level: float = 0.95,
         n_perms: int = 1000,
         seed: Optional[int] = None,
         **kwargs: Any,
     ) -> pd.DataFrame:
-        """
-        Compute correlation of push or pull distribution with features.
+        """Compute correlation of push-forward or pull-back distribution with features.
+
+        Correlates a feature, e.g., counts of a gene, with probabilities of cells mapped to a set of cells such as
+        the push-forward or pull-back distributions.
 
-        Correlates a feature (e.g. counts of a gene) with probabilities of cells mapped to a set of cells, e.g.
-        a pull back or push forward distribution.
+        .. seealso::
+            - TODO: create and link an example
 
         Parameters
         ----------
         obs_key
-            Column of :attr:`anndata.AnnData.obs` containing push-forward or pull-back distributions.
+            Key in :attr:`~anndata.AnnData.obs` containing the push-forward or pull-back distribution.
         corr_method
-            Which type of correlation to compute, options are `pearson`, and `spearman`.
+            Which type of correlation to compute, either ``'pearson'`` or ``'spearman'``.
         significance_method
             Mode to use when calculating p-values and confidence intervals. Valid options are:
 
-                - `fischer` - use Fischer transformation :cite:`fischer:21`.
-                - `perm_test` - use permutation test.
-
+            - ``'fisher'`` - Fisher transformation :cite:`fisher:21`.
+            - ``'perm_test'`` - `permutation test <https://en.wikipedia.org/wiki/Permutation_test>`_.
         annotation
-            If not `None`, this defines the subset of data to be considered when computing the correlation.
-            Its key should correspond to a key in
-            :attr:`anndata.AnnData.obs` and its value to an iterable containing a subset of categories present in
-            :attr:`anndata.AnnData.obs` ``['{annotation.keys()[0]}']``.
+            How to subset the data when computing the correlation:
+
+            - :obj:`None` - do not subset the data.
+            - :class:`str` - key in :attr:`~anndata.AnnData.obs` where categorical data is stored.
+            - :class:`dict` - a dictionary with one key corresponding to a categorical column in
+              :attr:`~anndata.AnnData.obs` and values to a subset of categories.
         layer
-            Key from :attr:`anndata.AnnData.layers` from which to get the expression.
-            If `None`, use :attr:`anndata.AnnData.X`.
+            Key in :attr:`~anndata.AnnData.layers` from which to get the expression.
+            If :obj:`None`, use :attr:`~anndata.AnnData.X`.
         features
-            Features in :class:`anndata.AnnData` which the correlation
-            of ``anndata.AnnData.obs['{obs_key}']`` is computed with:
-
-                - If `None`, all features from :attr:`anndata.AnnData.var` will be taken into account.
-                - If of type :obj:`list`, the elements should be from :attr:`anndata.AnnData.var_names` or
-                  :attr:`anndata.AnnData.obs_names`.
-                - If `human`, `mouse`, or `drosophila`, the features are subsetted to transcription factors,
-                  see :func:`~moscot.utils.data.transcription_factors`.
+            Features in :class:`~anndata.AnnData` to correlate with
+            :attr:`obs['{obs_key}'] <anndata.AnnData.obs>`:
 
+            - :obj:`None` - all features from :attr:`~anndata.AnnData.var` will be taken into account.
+            - :obj:`list` - subset of :attr:`~anndata.AnnData.var_names` or :attr:`~anndata.AnnData.obs_names`.
+            - ``'human'``, ``'mouse'``, or ``'drosophila'`` - the features are subsetted to the transcription factors
+              from :func:`~moscot.utils.data.transcription_factors`.
         confidence_level
-            Confidence level for the confidence interval calculation. Must be in interval `[0, 1]`.
+            Confidence level for the confidence interval calculation. Must be in interval :math:`[0, 1]`.
         n_perms
-            Number of permutations to use when ``method = perm_test``.
+            Number of permutations to use when ``method = 'perm_test'``.
         seed
-            Random seed when ``method = perm_test``.
+            Random seed when ``method = 'perm_test'``.
         kwargs
-            Keyword arguments for parallelization, e.g., `n_jobs`. # TODO(michalk8): consider making the function public
+            Keyword arguments for parallelization, e.g., ``n_jobs``.
 
         Returns
         -------
-        Dataframe of shape ``(n_features, 5)`` containing the following columns, one for each lineage:
-
-            - `corr` - correlation between the count data and push/pull distributions.
-            - `pval` - calculated p-values for double-sided test.
-            - `qval` - corrected p-values using Benjamini-Hochberg method at level `0.05`.
-            - `ci_low` - lower bound of the ``confidence_level`` correlation confidence interval.
-            - `ci_high` - upper bound of the ``confidence_level`` correlation confidence interval.
+        Dataframe of shape ``(n_features, 5)`` containing the following columns, one for each feature:
 
+        - ``'corr'`` - correlation between the count data and push/pull distributions.
+        - ``'pval'`` - calculated p-values for double-sided test.
+        - ``'qval'`` - corrected p-values using the `Benjamini-Hochberg
+          <https://en.wikipedia.org/wiki/False_discovery_rate#Benjamini%E2%80%93Hochberg_procedure>`_ method
+          at :math:`0.05` level.
+        - ``'ci_low'`` - lower bound of the ``confidence_level`` correlation confidence interval.
+        - ``'ci_high'`` - upper bound of the ``confidence_level`` correlation confidence interval.
         """
         if obs_key not in self.adata.obs:
             raise KeyError(f"Unable to access data in `adata.obs[{obs_key!r}]`.")
 
         if annotation is not None:
             annotation_key, annotation_vals = next(iter(annotation.items()))
             if annotation_key not in self.adata.obs:
-                raise KeyError(f"Unable to access data in [{annotation_key!r}.")
+                raise KeyError(f"Unable to access data in `adata.obs[{annotation_key!r}]`.")
             if not isinstance(annotation_vals, Iterable):
-                raise TypeError("`annotation` expected to be dictionary of length 1 with value being a list.")
-
+                raise TypeError("`annotation` expected to be dictionary of length 1 with value being an iterable.")
             adata = self.adata[self.adata.obs[annotation_key].isin(annotation_vals)]
         else:
             adata = self.adata
 
         adata = adata[~adata.obs[obs_key].isnull()]
-        if adata.n_obs == 0:
+        if not adata.n_obs:
             raise ValueError(f"`adata.obs[{obs_key!r}]` only contains NaN values.")
-        distribution = adata.obs[[obs_key]]
+        distribution: pd.DataFrame = adata.obs[[obs_key]]
 
         if isinstance(features, str):
             tfs = transcription_factors(organism=features)
             features = list(set(tfs).intersection(adata.var_names))
             if not features:
                 raise KeyError("No common transcription factors found in the data base.")
         elif features is None:
```

### Comparing `moscot-0.3.0/src/moscot/base/problems/_utils.py` & `moscot-0.3.1/src/moscot/base/problems/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+import functools
+import multiprocessing
+import threading
+import types
 import warnings
-from functools import partial, update_wrapper
-from multiprocessing import Manager, cpu_count
-from threading import Thread
-from types import MappingProxyType
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     List,
     Literal,
@@ -15,33 +15,32 @@
     Sequence,
     Tuple,
     Type,
     Union,
 )
 
 import joblib as jl
-
-if TYPE_CHECKING:
-    from moscot.base.problems.compound_problem import BaseCompoundProblem
-    from moscot.base.problems.problem import BaseProblem
-
 import wrapt
-from statsmodels.stats.multitest import multipletests
 
 import numpy as np
 import pandas as pd
 import scipy.sparse as sp
-from scipy.stats import norm, rankdata
+import scipy.stats as st
+from statsmodels.stats.multitest import multipletests
 
 from anndata import AnnData
 
-from moscot._docs._docs import d
 from moscot._logging import logger
 from moscot._types import ArrayLike, Str_Dict_t
 
+if TYPE_CHECKING:
+    from moscot.base.problems.compound_problem import BaseCompoundProblem
+    from moscot.base.problems.problem import BaseProblem
+
+
 Callback = Callable[..., Any]
 
 
 def _validate_annotations(
     df_source: pd.DataFrame,
     df_target: pd.DataFrame,
     source_annotation_key: Optional[str] = None,
@@ -231,21 +230,20 @@
             row_order=annotations_ordered,
             col_order=annotations_ordered,
         )
 
     return tm if forward else tm.T
 
 
-@d.dedent
 def _correlation_test(
     X: Union[ArrayLike, sp.spmatrix],
     Y: pd.DataFrame,
     feature_names: Sequence[str],
     corr_method: Literal["pearson", "spearman"] = "pearson",
-    significance_method: Literal["fischer", "perm_test"] = "fischer",
+    significance_method: Literal["fisher", "perm_test"] = "fisher",
     confidence_level: float = 0.95,
     n_perms: Optional[int] = None,
     seed: Optional[int] = None,
     **kwargs: Any,
 ) -> pd.DataFrame:
     """
     Perform a statistical test for correlation between X and .
@@ -324,15 +322,15 @@
     # fmt: on
 
 
 def _correlation_test_helper(
     X: ArrayLike,
     Y: ArrayLike,
     corr_method: Literal["pearson", "spearman"] = "spearman",
-    significance_method: Literal["fischer", "perm_test"] = "fischer",
+    significance_method: Literal["fisher", "perm_test"] = "fisher",
     n_perms: Optional[int] = None,
     seed: Optional[int] = None,
     confidence_level: float = 0.95,
     **kwargs: Any,
 ) -> Tuple[ArrayLike, ArrayLike, ArrayLike, ArrayLike]:
     """
     Compute the correlation between rows in matrix ``X`` columns of matrix ``Y``.
@@ -379,27 +377,27 @@
     ql = 1 - confidence_level - (1 - confidence_level) / 2.0
     qh = confidence_level + (1 - confidence_level) / 2.0
 
     if sp.issparse(X):
         X = sp.csr_matrix(X)
 
     if corr_method == "spearman":
-        X, Y = rankdata(X, method="average", axis=0), rankdata(Y, method="average", axis=0)
+        X, Y = st.rankdata(X, method="average", axis=0), st.rankdata(Y, method="average", axis=0)
     corr = _pearson_mat_mat_corr_sparse(X, Y) if sp.issparse(X) else _pearson_mat_mat_corr_dense(X, Y)
 
-    if significance_method == "fischer":
+    if significance_method == "fisher":
         # see: https://en.wikipedia.org/wiki/Pearson_correlation_coefficient#Using_the_Fisher_transformation
         # for spearman see: https://www.sciencedirect.com/topics/mathematics/spearman-correlation
         mean, se = np.arctanh(corr), 1 / np.sqrt(n - 3)
         z_score = (np.arctanh(corr) - np.arctanh(0)) * np.sqrt(n - 3)
 
-        z = norm.ppf(qh)
+        z = st.norm.ppf(qh)
         corr_ci_low = np.tanh(mean - z * se)
         corr_ci_high = np.tanh(mean + z * se)
-        pvals = 2 * norm.cdf(-np.abs(z_score))
+        pvals = 2 * st.norm.cdf(-np.abs(z_score))
 
     elif significance_method == "perm_test":
         if not isinstance(n_perms, int):
             raise TypeError(f"Expected `n_perms` to be an integer, found `{type(n_perms).__name__}`.")
         if n_perms <= 0:
             raise ValueError(f"Expected `n_perms` to be positive, found `{n_perms}`.")
 
@@ -550,21 +548,21 @@
         return func
 
     def wrapper(instance: Any, *args: Any, **kwargs: Any) -> Any:
         typ = type(getattr(instance, str(attr)))
         return dispatch(typ)(instance, *args, **kwargs)
 
     if func is None:
-        return partial(attributedispatch, attr=attr)
+        return functools.partial(attributedispatch, attr=attr)
 
     registry: Dict[Type[Any], Callback] = {}
     wrapper.register = register  # type: ignore[attr-defined]
     wrapper.dispatch = dispatch  # type: ignore[attr-defined]
-    wrapper.registry = MappingProxyType(registry)  # type: ignore[attr-defined]
-    update_wrapper(wrapper, func)
+    wrapper.registry = types.MappingProxyType(registry)  # type: ignore[attr-defined]
+    functools.update_wrapper(wrapper, func)
 
     return wrapper
 
 
 def parallelize(
     callback: Callable[[Any], Any],
     collection: Union[sp.spmatrix, Sequence[Any]],
@@ -639,16 +637,16 @@
 
         if pbar is not None:
             pbar.close()
 
     def wrapper(*args, **kwargs):
         if pass_queue and show_progress_bar:
             pbar = None if tqdm is None else tqdm(total=col_len, unit=unit, mininterval=0.125)
-            queue = Manager().Queue()
-            thread = Thread(target=update, args=(pbar, queue, len(collections)))
+            queue = multiprocessing.Manager().Queue()
+            thread = threading.Thread(target=update, args=(pbar, queue, len(collections)))
             thread.start()
         else:
             pbar, queue, thread = None, None, None
 
         res = jl.Parallel(n_jobs=n_jobs, backend=backend)(
             jl.delayed(callback)(
                 *((i, cs) if use_ixs else (cs,)),
@@ -672,15 +670,15 @@
 
     if sp.issparse(collection):
         n_split = max(1, min(n_split, collection.shape[0]))  # type: ignore
         if n_split == collection.shape[0]:  # type: ignore[union-attr]
             collections = [collection[[ix], :] for ix in range(collection.shape[0])]  # type: ignore
         else:
             step = collection.shape[0] // n_split  # type: ignore[union-attr]
-            ixs = [np.arange(i * step, min((i + 1) * step, collection.shape[0])) for i in range(n_split)]  # type: ignore  # noqa: 501
+            ixs = [np.arange(i * step, min((i + 1) * step, collection.shape[0])) for i in range(n_split)]  # type: ignore  # noqa: E501
             ixs[-1] = np.append(ixs[-1], np.arange(ixs[-1][-1] + 1, collection.shape[0]))  # type: ignore
 
             collections = [collection[ix, :] for ix in filter(len, ixs)]  # type:ignore[call-overload]
     else:
         collections = list(filter(len, np.array_split(collection, n_split)))
 
     n_split = len(collections)
@@ -707,10 +705,10 @@
     Positive integer corresponding to how many cores to use.
     """
     if n_cores == 0:
         raise ValueError("Number of cores cannot be `0`.")
     if n_jobs == 1 or n_cores is None:
         return 1
     if n_cores < 0:
-        return cpu_count() + 1 + n_cores
+        return multiprocessing.cpu_count() + 1 + n_cores
 
     return n_cores
```

### Comparing `moscot-0.3.0/src/moscot/base/problems/birth_death.py` & `moscot-0.3.1/src/moscot/base/problems/birth_death.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,39 @@
-from types import MappingProxyType
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Literal,
-    Mapping,
     Optional,
     Protocol,
     Sequence,
     Union,
 )
 
 import numpy as np
 
 import scanpy as sc
 from anndata import AnnData
 
-from moscot._docs._docs import d
 from moscot._logging import logger
 from moscot._types import ArrayLike
 from moscot.base.problems.problem import OTProblem
 from moscot.utils.data import apoptosis_markers, proliferation_markers
 
 __all__ = ["BirthDeathProblem", "BirthDeathMixin"]
 
 
 class BirthDeathProtocol(Protocol):  # noqa: D101
     adata: AnnData
     proliferation_key: Optional[str]
     apoptosis_key: Optional[str]
-    _proliferation_key: Optional[str] = None
-    _apoptosis_key: Optional[str] = None
-    _scaling: float = 1.0
-    _prior_growth: Optional[ArrayLike] = None
+    _proliferation_key: Optional[str]
+    _apoptosis_key: Optional[str]
+    _scaling: float
+    _prior_growth: Optional[ArrayLike]
 
     def score_genes_for_marginals(  # noqa: D102
         self: "BirthDeathProtocol",
         gene_set_proliferation: Optional[Union[Literal["human", "mouse"], Sequence[str]]] = None,
         gene_set_apoptosis: Optional[Union[Literal["human", "mouse"], Sequence[str]]] = None,
         proliferation_key: str = "proliferation",
         apoptosis_key: str = "apoptosis",
@@ -49,73 +46,65 @@
     delta: float
     adata_tgt: AnnData
     a: Optional[ArrayLike]
     b: Optional[ArrayLike]
 
 
 class BirthDeathMixin:
-    """Mixin for biological problems based on :class:`~moscot.base.problems.BirthDeathProblem`."""
+    """Mixin class used to estimate cell proliferation and apoptosis.
+
+    Parameters
+    ----------
+    args
+        Positional arguments.
+    kwargs
+        Keyword arguments.
+    """
 
     def __init__(self, *args: Any, **kwargs: Any):
         super().__init__(*args, **kwargs)
         self._proliferation_key: Optional[str] = None
         self._apoptosis_key: Optional[str] = None
         self._scaling: float = 1.0
         self._prior_growth: Optional[ArrayLike] = None
 
-    @d.dedent
     def score_genes_for_marginals(
-        self: BirthDeathProtocol,
+        self,  # type: BirthDeathProblemProtocol
         gene_set_proliferation: Optional[Union[Literal["human", "mouse"], Sequence[str]]] = None,
         gene_set_apoptosis: Optional[Union[Literal["human", "mouse"], Sequence[str]]] = None,
         proliferation_key: str = "proliferation",
         apoptosis_key: str = "apoptosis",
         **kwargs: Any,
     ) -> "BirthDeathMixin":
         """Compute gene scores to obtain prior knowledge about proliferation and apoptosis.
 
-        This method computes gene scores using :func:`~scanpy.tl.score_genes`. Therefore, a list of genes corresponding
-        to proliferation and/or apoptosis must be passed.
-
-        Alternatively, proliferation and apoptosis genes for humans and mice are saved in :mod:`moscot`.
-        The gene scores will be used in :meth:`~moscot.base.problems.BaseCompoundProblem.prepare` to estimate
-        the initial growth rates as suggested in :cite:`schiebinger:19`
+        The gene scores can be used in :meth:`~moscot.base.problems.BirthDeathProblem.estimate_marginals`
+        to estimate the initial growth rates as suggested in :cite:`schiebinger:19`
 
         Parameters
         ----------
         gene_set_proliferation
-            Set of marker genes for proliferation used in the birth-death process. If marker genes from :mod:`moscot`
-            are to be used the corresponding organism must be passed.
+            Set of proliferation marker genes. If a :class:`str`, it should
+            correspond to the organism in :func:`~moscot.utils.data.proliferation_markers`.
         gene_set_apoptosis
-            Set of marker genes for apoptosis used in the birth-death process. If marker genes from :mod:`moscot` are
-            to be used the corresponding organism must be passed.
+            Set of apoptosis marker genes. If a :class:`str`, it should
+            correspond to the organism in :func:`~moscot.utils.data.apoptosis_markers`.
         proliferation_key
-            Key in :attr:`anndata.AnnData.obs` where to add the genes scores.
+            Key in :attr:`~anndata.AnnData.obs` where to store the proliferation scores.
         apoptosis_key
-            TODO.
+            Key in :attr:`~anndata.AnnData.obs` where to store the apoptosis scores.
         kwargs
             Keyword arguments for :func:`~scanpy.tl.score_genes`.
 
         Returns
         -------
-        Returns self and updates the following:
-
-            - :attr:`proliferation_key` - TODO: description
-            - :attr:`apoptosis_key` - TODO: description
+        Returns self and updates the following fields:
 
-        Notes
-        -----
-        The marker genes in :mod:`moscot` are taken from the following sources:
-
-            - human, proliferation - :cite:`tirosh:16:science`.
-            - human, apoptosis - `Hallmark Apoptosis,
-              MSigDB <https://www.gsea-msigdb.org/gsea/msigdb/cards/HALLMARK_APOPTOSIS>`_.
-            - mouse, proliferation - :cite:`tirosh:16:nature`.
-            - mouse, apoptosis - `Hallmark P53 Pathway, MSigDB
-              <https://www.gsea-msigdb.org/gsea/msigdb/cards/HALLMARK_P53_PATHWAY>`_.
+        - :attr:`proliferation_key` - key in :attr:`~anndata.AnnData.obs` where proliferation scores are stored.
+        - :attr:`apoptosis_key` - key in :attr:`~anndata.AnnData.obs` where apoptosis scores are stored.
         """
         if isinstance(gene_set_proliferation, str):
             gene_set_proliferation = proliferation_markers(gene_set_proliferation)  # type: ignore[arg-type]
         if gene_set_proliferation is not None:
             sc.tl.score_genes(self.adata, gene_set_proliferation, score_name=proliferation_key, **kwargs)
             self.proliferation_key = proliferation_key
         else:
@@ -145,113 +134,151 @@
     def proliferation_key(self: BirthDeathProtocol, key: Optional[str]) -> None:
         if key is not None and key not in self.adata.obs:
             raise KeyError(f"Unable to find proliferation data in `adata.obs[{key!r}]`.")
         self._proliferation_key = key
 
     @property
     def apoptosis_key(self) -> Optional[str]:
-        """Key in :attr:`anndata.AnnData.obs` where cell apoptosis is stored."""
+        """Key in :attr:`~anndata.AnnData.obs` where cell apoptosis is stored."""
         return self._apoptosis_key
 
     @apoptosis_key.setter
     def apoptosis_key(self: BirthDeathProtocol, key: Optional[str]) -> None:
         if key is not None and key not in self.adata.obs:
             raise KeyError(f"Unable to find apoptosis data in `adata.obs[{key!r}]`.")
         self._apoptosis_key = key
 
 
-@d.dedent
 class BirthDeathProblem(BirthDeathMixin, OTProblem):
-    """Optimal transport problem which allows to estimate the marginals with a birth-death process.
+    """:term:`OT` problem used to estimate the :term:`marginals` with the
+    `birth-death process <https://en.wikipedia.org/wiki/Birth%E2%80%93death_process>`_.
 
     Parameters
     ----------
-    %(adata_x)s
-    """
+    args
+        Positional arguments for :class:`~moscot.base.problems.OTProblem`.
+    kwargs
+        Keyword arguments for :class:`~moscot.base.problems.OTProblem`.
+    """  # noqa: D205
 
     def estimate_marginals(
-        self: BirthDeathProblemProtocol,
+        self,  # type: BirthDeathProblemProtocol
         adata: AnnData,
         source: bool,
         proliferation_key: Optional[str] = None,
         apoptosis_key: Optional[str] = None,
-        marginal_kwargs: Mapping[str, Any] = MappingProxyType({}),
-        **_: Any,
+        **kwargs: Any,
     ) -> ArrayLike:
-        """TODO."""
+        """Estimate the source or target :term:`marginals` based on marker genes, either with the
+        `birth-death process <https://en.wikipedia.org/wiki/Birth%E2%80%93death_process>`_,
+        as suggested in :cite:`schiebinger:19`, or with an exponential kernel.
+
+        See :meth:`score_genes_for_marginals` on how to compute the proliferation and apoptosis scores.
+
+        Parameters
+        ----------
+        adata
+            Annotated data object.
+        source
+            Whether to estimate the source or the target :term:`marginals`.
+        proliferation_key
+            Key in :attr:`~anndata.AnnData.obs` where proliferation scores are stored.
+        apoptosis_key
+            Key in :attr:`~anndata.AnnData.obs` where apoptosis scores are stored.
+        kwargs
+            Keyword arguments for :func:`~moscot.base.problems.birth_death.beta` and
+            :func:`~moscot.base.problems.birth_death.delta`.
+
+        Returns
+        -------
+        The estimated source or target marginals of shape ``[n,]`` or ``[m,]``, depending on the ``source``.
+        If ``source = True``, also updates the following fields:
+
+        - :attr:`prior_growth_rates` - prior estimate of the source growth rates.
+
+        Examples
+        --------
+        - See :doc:`../notebooks/examples/problems/800_score_genes_for_marginals`
+            on examples how to use :meth:`~moscot.problems.time.TemporalProblem.score_genes_for_marginals`.
+
+        """  # noqa: D205
 
         def estimate(key: Optional[str], *, fn: Callable[..., ArrayLike], **kwargs: Any) -> ArrayLike:
             if key is None:
                 return np.zeros(adata.n_obs, dtype=float)
             try:
                 return fn(adata.obs[key].values.astype(float), **kwargs)
             except KeyError:
-                raise KeyError(f"Unable to fetch data from `adata.obs[{key}!r]`.") from None
+                raise KeyError(f"Unable to get data from `adata.obs[{key}!r]`.") from None
 
         if proliferation_key is None and apoptosis_key is None:
-            raise ValueError("Either `proliferation_key` or `apoptosis_key` must be specified.")
+            raise ValueError("At least one of `proliferation_key` or `apoptosis_key` must be specified.")
+
+        # TODO(michalk8): why does this need to be set?
         self.proliferation_key = proliferation_key
         self.apoptosis_key = apoptosis_key
-        if "scaling" in marginal_kwargs:
-            beta_fn = delta_fn = lambda x, *args, **kwargs: x
-            scaling = marginal_kwargs["scaling"]
+
+        if "scaling" in kwargs:
+            beta_fn = delta_fn = lambda x, *_, **__: x
+            scaling = kwargs["scaling"]
         else:
             beta_fn, delta_fn = beta, delta
             scaling = 1.0
-        birth = estimate(proliferation_key, fn=beta_fn, **marginal_kwargs)
-        death = estimate(apoptosis_key, fn=delta_fn, **marginal_kwargs)
+        birth = estimate(proliferation_key, fn=beta_fn, **kwargs)
+        death = estimate(apoptosis_key, fn=delta_fn, **kwargs)
 
         prior_growth = np.exp((birth - death) * self.delta / scaling)
 
         scaling = np.sum(prior_growth)
         normalized_growth = prior_growth / scaling
         if source:
             self._scaling = scaling
             self._prior_growth = prior_growth
-        return normalized_growth if source else np.full(self.adata_tgt.n_obs, fill_value=np.mean(normalized_growth))
+            return normalized_growth
+
+        return np.full(self.adata_tgt.n_obs, fill_value=np.mean(normalized_growth))
 
-    # TODO(michalk8): temporary fix to satisfy the mixin, consider removing the mixin
     @property
     def adata(self) -> AnnData:
         """Annotated data object."""
         return self.adata_src
 
     @property
     def prior_growth_rates(self) -> Optional[ArrayLike]:
-        """Return the prior estimate of growth rates of the cells in the source distribution."""
+        """Prior estimate of the source growth rates."""
         if self._prior_growth is None:
             return None
-        return np.power(self._prior_growth, 1.0 / self.delta)
+        return np.asarray(np.power(self._prior_growth, 1.0 / self.delta))
 
     @property
     def posterior_growth_rates(self) -> Optional[ArrayLike]:
-        """Return the posterior estimate of growth rates of the cells in the source distribution."""
-        if self.solution.a is None:  # type: ignore[union-attr]
+        """Posterior estimate of the source growth rates."""
+        if self.solution is None:
             return None
         if self.delta is None:
             return self.solution.a * self.adata.n_obs
-        return np.power(self.solution.a * self._scaling, 1.0 / self.delta)  # type: ignore[union-attr]
+        return np.asarray(self.solution.a * self._scaling) ** (1.0 / self.delta)
 
     @property
     def delta(self) -> float:
-        """TODO."""
+        """Time difference between the source and the target."""
         if TYPE_CHECKING:
             assert isinstance(self._src_key, float)
             assert isinstance(self._tgt_key, float)
         return self._tgt_key - self._src_key
 
 
 def _logistic(x: ArrayLike, L: float, k: float, center: float = 0) -> ArrayLike:
     """Logistic function."""
     return L / (1 + np.exp(-k * (x - center)))
 
 
 def _gen_logistic(p: ArrayLike, sup: float, inf: float, center: float, width: float) -> ArrayLike:
     """Shifted logistic function."""
-    return inf + _logistic(p, L=sup - inf, k=4 / width, center=center)
+    return inf + _logistic(p, L=sup - inf, k=4.0 / width, center=center)
 
 
 def beta(
     p: ArrayLike,
     beta_max: float = 1.7,
     beta_min: float = 0.3,
     beta_center: float = 0.25,
```

### Comparing `moscot-0.3.0/src/moscot/base/problems/compound_problem.py` & `moscot-0.3.1/src/moscot/base/problems/compound_problem.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import abc
-import os
-from types import MappingProxyType
+import types
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Generic,
     Hashable,
@@ -15,21 +14,18 @@
     Sequence,
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 
-import cloudpickle
-
 import scipy.sparse as sp
 
 from anndata import AnnData
 
-from moscot._docs._docs import d
 from moscot._logging import logger
 from moscot._types import ArrayLike, Policy_t, ProblemStage_t
 from moscot.base.output import BaseSolverOutput
 from moscot.base.problems._utils import attributedispatch, require_prepare
 from moscot.base.problems.manager import ProblemManager
 from moscot.base.problems.problem import BaseProblem, OTProblem
 from moscot.utils.subset_policy import (
@@ -47,62 +43,86 @@
 
 K = TypeVar("K", bound=Hashable)
 B = TypeVar("B", bound=OTProblem)
 Callback_t = Callable[
     [Literal["xy", "x", "y"], AnnData, Optional[AnnData]], Mapping[Literal["xy", "x", "y"], TaggedArray]
 ]
 ApplyOutput_t = Union[ArrayLike, Dict[K, ArrayLike]]
-# TODO(michalk8): future behavior
-# ApplyOutput_t = Union[ArrayLike, Dict[Tuple[K, K], ArrayLike]]
 
 
-@d.get_sections(base="BaseCompoundProblem", sections=["Parameters", "Raises"])
-@d.dedent
 class BaseCompoundProblem(BaseProblem, abc.ABC, Generic[K, B]):
-    """
-    Base class for all biological problems.
+    """Base class for all biological problems.
 
-    This base class translates a biological problem to potentially multiple Optimal Transport problems.
+    This class translates a biological problem to multiple :term:`OT` problems.
 
     Parameters
     ----------
-    %(adata)s
-
-    Raises
-    ------
-    TypeError
-        If `base_problem_type` is not a subclass of :class:`~moscot.base.problems.OTProblem`.
+    adata
+        Annotated data object.
+    kwargs
+        Keyword arguments for :class:`~moscot.base.problems.BaseProblem`.
     """
 
     def __init__(self, adata: AnnData, **kwargs: Any):
         super().__init__(**kwargs)
         self._adata = adata
         self._problem_manager: Optional[ProblemManager[K, B]] = None
 
     @abc.abstractmethod
     def _create_problem(self, src: K, tgt: K, src_mask: ArrayLike, tgt_mask: ArrayLike, **kwargs: Any) -> B:
-        pass
+        """Create an :term:`OT` subproblem.
+
+        Parameters
+        ----------
+        src
+            Source key identifying the subproblem.
+        tgt
+            Target key identifying the subproblem.
+        src_mask
+            Source mask used to subset :attr:`adata`.
+        tgt_mask
+            Target mask used to subset :attr:`adata`.
+        kwargs
+            Additional keyword arguments.
+
+        Returns
+        -------
+        The subproblem.
+        """
 
     @abc.abstractmethod
     def _create_policy(
         self,
         policy: Policy_t,
         **kwargs: Any,
     ) -> SubsetPolicy[K]:
-        pass
+        """Create a policy used to split :attr:`adata`.
+
+        Only policies specified by :attr:`_valid_policies` will be passed to this function.
+
+        Parameters
+        ----------
+        policy
+            Name of the policy.
+        kwargs
+            Keyword arguments for :class:`~moscot.utils.subset_policy.SubsetPolicy`.
+
+        Returns
+        -------
+        The policy.
+        """
 
     @property
     @abc.abstractmethod
     def _valid_policies(self) -> Tuple[Policy_t, ...]:
-        pass
+        """Valid policies for this problem."""
 
-    # TODO(michalk8): refactor me
     def _callback_handler(
         self,
-        term: Literal["x", "y", "xy"],
+        term: Literal["xy", "x", "y"],
         key_1: K,
         key_2: K,
         problem: B,
         *,
         callback: Optional[Union[Literal["local-pca"], Callback_t]] = None,
         **kwargs: Any,
     ) -> Mapping[Literal["xy", "x", "y"], TaggedArray]:
@@ -114,30 +134,32 @@
                 if not isinstance(val, TaggedArray):
                     raise TypeError(f"Expected value for `{key}` to be a `TaggedArray`, found `{type(val)}`.")
 
         if callback is None:
             return {}
         if callback == "local-pca":
             callback = problem._local_pca_callback
+        if callback == "spatial-norm":
+            callback = problem._spatial_norm_callback
 
         if not callable(callback):
             raise TypeError("Callback is not a function.")
         data = callback(term, problem.adata_src, problem.adata_tgt, **kwargs)
         verify_data(data)
         return data
 
     # TODO(michalk8): refactor me
     def _create_problems(
         self,
         xy_callback: Optional[Union[Literal["local-pca"], Callback_t]] = None,
         x_callback: Optional[Union[Literal["local-pca"], Callback_t]] = None,
         y_callback: Optional[Union[Literal["local-pca"], Callback_t]] = None,
-        xy_callback_kwargs: Mapping[str, Any] = MappingProxyType({}),
-        x_callback_kwargs: Mapping[str, Any] = MappingProxyType({}),
-        y_callback_kwargs: Mapping[str, Any] = MappingProxyType({}),
+        xy_callback_kwargs: Mapping[str, Any] = types.MappingProxyType({}),
+        x_callback_kwargs: Mapping[str, Any] = types.MappingProxyType({}),
+        y_callback_kwargs: Mapping[str, Any] = types.MappingProxyType({}),
         **kwargs: Any,
     ) -> Dict[Tuple[K, K], B]:
         from moscot.base.problems.birth_death import BirthDeathProblem
 
         if TYPE_CHECKING:
             assert isinstance(self._policy, SubsetPolicy)
 
@@ -160,72 +182,88 @@
                 term="x", key_1=src, key_2=tgt, problem=problem, callback=x_callback, **x_callback_kwargs
             )
 
             y_data = self._callback_handler(
                 term="y", key_1=src, key_2=tgt, problem=problem, callback=y_callback, **y_callback_kwargs
             )
 
-            kws = {**kwargs, **xy_data, **x_data, **y_data}  # type: ignore[arg-type]
+            kws = {**kwargs, **xy_data, **x_data, **y_data}  # type: ignore[misc]
 
             if isinstance(problem, BirthDeathProblem):
                 kws["proliferation_key"] = self.proliferation_key  # type: ignore[attr-defined]
                 kws["apoptosis_key"] = self.apoptosis_key  # type: ignore[attr-defined]
             problems[src_name, tgt_name] = problem.prepare(**kws)
 
         return problems
 
-    @d.get_sections(base="BaseCompoundProblem_prepare", sections=["Parameters", "Raises"])
-    @d.dedent
     def prepare(
         self,
-        key: str,
-        policy: Policy_t = "sequential",
+        policy: Policy_t,
+        key: Optional[str],
         subset: Optional[Sequence[Tuple[K, K]]] = None,
         reference: Optional[Any] = None,
         xy_callback: Optional[Union[Literal["local-pca"], Callback_t]] = None,
         x_callback: Optional[Union[Literal["local-pca"], Callback_t]] = None,
         y_callback: Optional[Union[Literal["local-pca"], Callback_t]] = None,
-        xy_callback_kwargs: Mapping[str, Any] = MappingProxyType({}),
-        x_callback_kwargs: Mapping[str, Any] = MappingProxyType({}),
-        y_callback_kwargs: Mapping[str, Any] = MappingProxyType({}),
+        xy_callback_kwargs: Mapping[str, Any] = types.MappingProxyType({}),
+        x_callback_kwargs: Mapping[str, Any] = types.MappingProxyType({}),
+        y_callback_kwargs: Mapping[str, Any] = types.MappingProxyType({}),
         **kwargs: Any,
     ) -> "BaseCompoundProblem[K, B]":
-        """
-        Prepare the biological problem.
+        """Prepare the individual :term:`OT` subproblems.
+
+        .. seealso::
+            - See :doc:`../notebooks/examples/problems/400_subset_policy` on how to use different policies.
 
         Parameters
         ----------
-        %(key)s
-        %(policy)s
-        %(subset)s
-        %(reference)s
-        %(xy_callback)s
-        %(x_callback)s
-        %(y_callback)s
-        %(xy_callback_kwargs)s
-        %(x_callback_kwargs)s
-        %(y_callback_kwargs)s
-        %(a)s
-        %(b)s
+        policy
+            Rule which defines how to construct the subproblems.
+        key
+            Key in :attr:`~anndata.AnnData.obs` for the :class:`~moscot.utils.subset_policy.SubsetPolicy`.
+        subset
+            Subset of :attr:`obs['{key}'] <anndata.AnnData.obs>`
+            for the :class:`~moscot.utils.subset_policy.ExplicitPolicy`. Only used when ``policy = 'explicit'``.
+        reference
+            Reference for the :class:`~moscot.utils.subset_policy.SubsetPolicy`. Only used when ``policy = 'star'``.
+        xy_callback
+            Callback function used to prepare the data in the :term:`linear term`.
+        x_callback
+            Callback function used to prepare the data in the source :term:`quadratic term`.
+        y_callback
+            Callback function used to prepare the data in the target :term:`quadratic term`.
+        xy_callback_kwargs
+            Keyword arguments for the ``xy_callback``.
+        x_callback_kwargs
+            Keyword arguments for the ``x_callback``.
+        y_callback_kwargs
+            Keyword arguments for the ``y_callback``.
+        kwargs
+            Keyword arguments for the subproblems' :meth:`~moscot.base.problems.OTProblem.prepare` method.
 
         Returns
         -------
-        The prepared problem.
+        Returns self and updates the following fields:
+
+        - :attr:`problems` - the prepared subproblems.
+        - :attr:`solutions` - set to an empty :class:`dict`.
+        - :attr:`stage` - set to ``'prepared'``.
+        - :attr:`problem_kind` - kind of the :term:`OT` problem.
         """
         self._ensure_valid_policy(policy)
         policy = self._create_policy(policy=policy, key=key)
         if TYPE_CHECKING:
             assert isinstance(policy, SubsetPolicy)
 
         if isinstance(policy, ExplicitPolicy):
-            policy = policy(subset=subset)
+            policy = policy.create_graph(subset=subset)
         elif isinstance(policy, StarPolicy):
-            policy = policy(reference=reference)
+            policy = policy.create_graph(reference=reference)
         else:
-            policy = policy()
+            policy = policy.create_graph()
 
         # TODO(michalk8): manager must be currently instantiated first, since `_create_problems` accesses the policy
         # when refactoring the callback, consider changing this
         self._problem_manager = ProblemManager(self, policy=policy)
         problems = self._create_problems(
             xy_callback=xy_callback,
             x_callback=x_callback,
@@ -233,95 +271,100 @@
             xy_callback_kwargs=xy_callback_kwargs,
             x_callback_kwargs=x_callback_kwargs,
             y_callback_kwargs=y_callback_kwargs,
             **kwargs,
         )
         self._problem_manager.add_problems(problems)
 
+        # we assume that all subproblems are of the same kind
         for p in self.problems.values():
             self._problem_kind = p._problem_kind
+            self._stage = "prepared"
             break
         return self
 
     def solve(
         self,
         stage: Union[ProblemStage_t, Tuple[ProblemStage_t, ...]] = ("prepared", "solved"),
         **kwargs: Any,
-    ) -> "BaseCompoundProblem[K,B]":
-        """
-        Solve the biological problem.
+    ) -> "BaseCompoundProblem[K, B]":
+        """Solve the individual :term:`OT` subproblems.
+
+        .. seealso:
+            - See :doc:`../notebooks/examples/solvers/100_linear_problems_basic`
+            for an introduction on how to solve linear problems.
+            - See :doc:`../notebooks/examples/solvers/300_quad_problems_basic`
+            for an introduction on how to solve quadratic problems.
 
         Parameters
         ----------
         stage
-            Some stage TODO.
+            Stage by which to filter the :attr:`problems` to be solved.
         kwargs
-            Keyword arguments for :meth:`~moscot.base.problems.OTProblem.solve`.
+            Keyword arguments for the subproblems' :meth:`~moscot.base.problems.OTProblem.solve` method.
 
         Returns
         -------
-        The solver problem.
+        Returns self and updates the following fields:
+
+        - :attr:`solutions` - the :term:`OT` solutions for each subproblem.
+        - :attr:`stage` - set to ``'solved'``.
         """
         if TYPE_CHECKING:
             assert isinstance(self._problem_manager, ProblemManager)
         problems = self._problem_manager.get_problems(stage=stage)
 
         logger.info(f"Solving `{len(problems)}` problems")
-        for _, problem in problems.items():
+        for problem in problems.values():
             logger.info(f"Solving problem {problem}.")
             _ = problem.solve(**kwargs)
 
+        self._stage = "solved"
         return self
 
     @attributedispatch(attr="_policy")
-    def _apply(
-        self,
-        data: Optional[Union[str, ArrayLike]] = None,
-        forward: bool = True,
-        scale_by_marginals: bool = False,
-        **kwargs: Any,
-    ) -> ApplyOutput_t[K]:
+    def _apply(self, *_args: Any, **_kwargs: Any) -> ApplyOutput_t[K]:
         raise NotImplementedError(type(self._policy))
 
     @_apply.register(DummyPolicy)
     @_apply.register(StarPolicy)
     def _(
         self,
+        source: Optional[K] = None,
+        target: Optional[K] = None,
         data: Optional[Union[str, ArrayLike]] = None,
         forward: bool = True,
         scale_by_marginals: bool = False,
-        source: Optional[K] = None,
-        return_all: bool = True,
+        return_all: bool = False,
         **kwargs: Any,
     ) -> ApplyOutput_t[K]:
+        del target
         if TYPE_CHECKING:
             assert isinstance(self._policy, StarPolicy)
+
         res = {}
-        # TODO(michalk8): should use manager.plan (once implemented), as some problems may not be solved
-        # TODO: better check
         source = source if isinstance(source, list) else [source]
-        _ = kwargs.pop("target", None)  # make compatible with Explicit/Ordered policy
         for src, tgt in self._policy.plan(
             explicit_steps=kwargs.pop("explicit_steps", None),
             filter=source,  # type: ignore [arg-type]
         ):
             problem = self.problems[src, tgt]
             fun = problem.push if forward else problem.pull
-            res[src] = fun(data=data, scale_by_marginals=scale_by_marginals, **kwargs)
+            res[src] = fun(data=data, scale_by_marginals=scale_by_marginals)
         return res if return_all else res[src]
 
     @_apply.register(ExplicitPolicy)
     @_apply.register(OrderedPolicy)
     def _(
         self,
+        source: Optional[K] = None,
+        target: Optional[K] = None,
         data: Optional[Union[str, ArrayLike]] = None,
         forward: bool = True,
         scale_by_marginals: bool = False,
-        source: Optional[K] = None,
-        target: Optional[K] = None,
         return_all: bool = False,
         **kwargs: Any,
     ) -> ApplyOutput_t[K]:
         explicit_steps = kwargs.pop(
             "explicit_steps", [[source, target]] if isinstance(self._policy, ExplicitPolicy) else None
         )
         if TYPE_CHECKING:
@@ -331,232 +374,128 @@
             start=source,
             end=target,
             explicit_steps=explicit_steps,
         )
         problem = self.problems[src, tgt]
         adata = problem.adata_src if forward else problem.adata_tgt
         current_mass = problem._get_mass(adata, data=data, **kwargs)
-        # TODO(michlak8): future behavior
-        # res = {(None, src) if forward else (tgt, None): current_mass}
         res = {src if forward else tgt: current_mass}
         for _src, _tgt in [(src, tgt)] + rest:
             problem = self.problems[_src, _tgt]
             fun = problem.push if forward else problem.pull
-            res[_tgt if forward else _src] = current_mass = fun(
-                current_mass, scale_by_marginals=scale_by_marginals, **kwargs
-            )
+            res[_tgt if forward else _src] = current_mass = fun(current_mass, scale_by_marginals=scale_by_marginals)
 
         return res if return_all else current_mass
 
-    @d.get_sections(base="BaseCompoundProblem_push", sections=["Parameters", "Raises"])
-    @d.dedent  # TODO(@MUCDK) document private _apply
+    # TODO(michalk8): better description of `source/target` (also in other places).
     def push(self, *args: Any, **kwargs: Any) -> ApplyOutput_t[K]:
-        """
-        Push mass from `start` to `end`.
-
-        TODO: verify.
+        """Push mass from source to target.
 
-        Parameters
-        ----------
-        %(data)s
-        %(subset)s
-        %(normalize)s
-
-        return_all
-            If `True` and transport maps are applied consecutively only the final mass is returned.
-            Otherwise, all intermediate step results are returned, too.
-
-        %(scale_by_marginals)s
-
-        kwargs
-            keyword arguments for policy-specific `_apply` method of :class:`moscot.base.problems.CompoundProblem`.
-
-        Returns
-        -------
         TODO.
         """
         _ = kwargs.pop("return_data", None)
         _ = kwargs.pop("key_added", None)  # this should be handled by overriding method
         return self._apply(*args, forward=True, **kwargs)
 
-    @d.get_sections(base="BaseCompoundProblem_pull", sections=["Parameters", "Raises"])
-    @d.dedent  # TODO(@MUCDK) document private functions
-    def pull(self, *args: Any, **kwargs: Any) -> ApplyOutput_t[K]:
-        """
-        Pull mass from `end` to `start`.
-
-        TODO: expose kwargs.
-
-        Parameters
-        ----------
-        %(data)s
-        %(subset)s
-        %(normalize)s
-
-        return_all
-            If `True` and transport maps are applied consecutively only the final mass is returned. Otherwise,
-            all intermediate step results are returned, too.
-
-        %(scale_by_marginals)s
-
-        kwargs
-            keyword arguments for policy-specific `_apply` method of :class:`moscot.base.problems.CompoundProblem`.
+    def pull(
+        self,
+        *args: Any,
+        **kwargs: Any,
+    ) -> ApplyOutput_t[K]:
+        """Pull mass from target to source.
 
-        Returns
-        -------
-        TODO.
+        TODO
         """
         _ = kwargs.pop("return_data", None)
         _ = kwargs.pop("key_added", None)  # this should be handled by overriding method
         return self._apply(*args, forward=False, **kwargs)
 
     @property
     def problems(self) -> Dict[Tuple[K, K], B]:
-        """Return dictionary of OT problems which the biological problem consists of."""
+        """:term:`OT` subproblems that define the biological problem."""
         if self._problem_manager is None:
             return {}
         return self._problem_manager.problems
 
-    @d.dedent
     @require_prepare
     def add_problem(
         self,
         key: Tuple[K, K],
         problem: B,
         *,
         overwrite: bool = False,
         **kwargs: Any,
     ) -> "BaseCompoundProblem[K, B]":
         """Add a subproblem.
 
-        This function adds and prepares a problem, e.g. if it is not included by the initial
-        :class:`~moscot.utils.subset_policy.SubsetPolicy`.
+        .. seealso::
+            - See :doc:`../notebooks/examples/problems/300_adding_and_removing_problems` on how to add subproblems.
 
         Parameters
         ----------
-        %(key)s
-
+        key
+            Key in :attr:`problems` where to add the subproblem.
         problem
-            Instance of a :class:`~moscot.base.problems.OTProblem`.
+            Subproblem to add.
         overwrite
-            If `True` the problem will be reinitialized and prepared even if a problem with `key` exists.
+            Whether ot overwrite an existing subproblem in :attr:`problems`.
+        kwargs
+            Additional keyword arguments.
 
         Returns
         -------
-        The updated compound problem.
+        Self and updates the following fields:
+
+        - :attr:`problems`
         """
         if TYPE_CHECKING:
             assert isinstance(self._problem_manager, ProblemManager)
         self._problem_manager.add_problem(key, problem, overwrite=overwrite, **kwargs)
         return self
 
-    @d.dedent
     @require_prepare
     def remove_problem(self, key: Tuple[K, K]) -> "BaseCompoundProblem[K, B]":
         """Remove a subproblem.
 
+        .. seealso::
+            - See :doc:`../notebooks/examples/problems/300_adding_and_removing_problems` on how to remove subproblems.
+
         Parameters
         ----------
-        %(key)s
+        key
+            Key of the subproblem to remove.
 
         Returns
         -------
-        The updated compound problem.
+        Self and updates the following fields:
+
+        - :attr:`problems`
         """
         if TYPE_CHECKING:
             assert isinstance(self._problem_manager, ProblemManager)
         self._problem_manager.remove_problem(key)
         return self
 
-    # TODO(MUCKD): should be on the OT problem level as well
-    def save(
-        self,
-        dir_path: str,
-        file_prefix: Optional[str] = None,
-        overwrite: bool = False,
-    ) -> None:
-        """
-        Save the model.
-
-        As of now this method pickled the problem class instance. Modifications depend on the I/O of the backend.
-
-        Parameters
-        ----------
-        dir_path
-            Path to a directory, defaults to current directory
-        file_prefix
-            Prefix to prepend to the file name.
-        overwrite
-            Whether to overwrite existing data or not.
-
-        Returns
-        -------
-        Nothing, just saves the problem.
-        """
-        file_name = (
-            f"{file_prefix}_{self.__class__.__name__}.pkl"
-            if file_prefix is not None
-            else f"{self.__class__.__name__}.pkl"
-        )
-        file_dir = os.path.join(dir_path, file_name) if dir_path is not None else file_name
-
-        if not overwrite and os.path.exists(file_dir):
-            raise RuntimeError(f"Unable to save to an existing file `{file_dir}` use `overwrite=True` to overwrite it.")
-        with open(file_dir, "wb") as f:
-            cloudpickle.dump(self, f)
-
-        logger.info(f"Successfully saved the problem as `{file_dir}`")
-
-    # TODO(MUCKD): should be on the OT problem level as well
-    @classmethod
-    def load(
-        cls,
-        filename: str,
-    ) -> "BaseCompoundProblem[K, B]":
-        """
-        Instantiate a moscot problem from a saved output.
-
-        Parameters
-        ----------
-        filename
-            filename of the model to load
-
-        Returns
-        -------
-        Loaded instance of the model.
-
-        Examples
-        --------
-        #TODO(michalk8): make nicer
-        >>> problem = ProblemClass.load(filename) # use the name of the model class used to save
-        >>> problem.push....
-        """
-        with open(filename, "rb") as f:
-            problem = cloudpickle.load(f)
-        if type(problem) is not cls:
-            raise TypeError(f"Expected the problem to be type of `{cls}`, found `{type(problem)}`.")
-        return problem
-
     @property
     def solutions(self) -> Dict[Tuple[K, K], BaseSolverOutput]:
-        """Return dictionary of solutions of OT problems which the biological problem consists of."""
+        """Solutions to the :attr:`problems`."""
         if self._problem_manager is None:
             return {}
         return self._problem_manager.solutions
 
     @property
     def adata(self) -> AnnData:
         """Annotated data object."""
         return self._adata
 
     @property
     def _policy(self) -> Optional[SubsetPolicy[K]]:
         if self._problem_manager is None:
             return None
-        return self._problem_manager._policy
+        return self._problem_manager.policy
 
     def _ensure_valid_policy(self, policy: Policy_t) -> None:
         if self._valid_policies and policy not in self._valid_policies:
             raise ValueError(f"Invalid policy `{policy!r}`. Valid policies are: `{self._valid_policies}`.")
 
     def __getitem__(self, item: Tuple[K, K]) -> B:
         return self.problems[item]
@@ -573,25 +512,25 @@
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}{list(self.problems.keys())}"
 
     def __str__(self) -> str:
         return repr(self)
 
 
-@d.get_sections(base="CompoundProblem", sections=["Parameters", "Raises"])
-@d.dedent
 class CompoundProblem(BaseCompoundProblem[K, B], abc.ABC):
-    """Class handling biological problems composed of exactly one :class:`~anndata.AnnData` instance.
+    """Base class for all biological problems.
 
-    This class is needed to apply the `policy` to one :class:`~anndata.AnnData` objects and hence create the
-    Optimal Transport subproblems from the biological problem.
+    This class translates a biological problem to multiple :term:`OT` problems.
 
     Parameters
     ----------
-    %(BaseCompoundProblem.parameters)s
+    adata
+        Annotated data object.
+    kwargs
+        Keyword arguments for :class:`~moscot.base.problems.BaseCompoundProblem`.
     """
 
     @property
     @abc.abstractmethod
     def _base_problem_type(self) -> Type[B]:
         pass
 
@@ -616,16 +555,14 @@
         key_1: K,
         key_2: K,
         problem: B,
         *,
         callback: Optional[Union[Literal["local-pca", "cost-matrix"], Callback_t]] = None,
         **kwargs: Any,
     ) -> Mapping[Literal["xy", "x", "y"], TaggedArray]:
-        # TODO(michalk8): better name?
-
         if callback == "cost-matrix":
             return self._cost_matrix_callback(term=term, key_1=key_1, key_2=key_2, **kwargs)
         return super()._callback_handler(
             term=term, key_1=key_1, key_2=key_2, problem=problem, callback=callback, **kwargs
         )
 
     def _cost_matrix_callback(
```

### Comparing `moscot-0.3.0/src/moscot/base/problems/problem.py` & `moscot-0.3.1/src/moscot/base/problems/problem.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,132 @@
+import abc
+import pathlib
 import types
-from abc import ABC, abstractmethod
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     List,
     Literal,
     Mapping,
     Optional,
     Tuple,
     Union,
 )
 
+import cloudpickle
+
 import numpy as np
 import pandas as pd
 import scipy.sparse as sp
+from pandas.api import types as pd_types
 from sklearn.preprocessing import StandardScaler
 
 import scanpy as sc
 from anndata import AnnData
 
 from moscot import backends
-from moscot._docs._docs import d
 from moscot._logging import logger
-from moscot._types import ArrayLike, CostFn_t, Device_t, ProblemKind_t, ProblemStage_t
+from moscot._types import ArrayLike, CostFn_t, Device_t, ProblemKind_t
 from moscot.base.output import BaseSolverOutput, MatrixSolverOutput
 from moscot.base.problems._utils import require_solution, wrap_prepare, wrap_solve
 from moscot.base.solver import OTSolver
 from moscot.utils.tagged_array import Tag, TaggedArray
 
 __all__ = ["BaseProblem", "OTProblem"]
 
 
-@d.get_sections(base="BaseProblem", sections=["Parameters", "Raises"])
-@d.dedent
-class BaseProblem(ABC):
-    """Problem interface handling one optimal transport problem.
-
-    Parameters
-    ----------
-    kwargs
-        Metadata.
-    """
+class BaseProblem(abc.ABC):
+    """Base class for all :term:`OT` problems."""
 
-    def __init__(self, **kwargs: Any):
+    def __init__(self):
         self._problem_kind: ProblemKind_t = "unknown"
-        self._stage: ProblemStage_t = "initialized"
-        self._metadata = dict(kwargs)
+        self._stage: Literal["initialized", "prepared", "solved"] = "initialized"
 
-    @abstractmethod
+    @abc.abstractmethod
     def prepare(self, *args: Any, **kwargs: Any) -> "BaseProblem":
-        """Abstract prepare method."""
+        """Prepare the problem.
+
+        Parameters
+        ----------
+        args
+            Positional arguments.
+        kwargs
+            Keyword arguments.
+
+        Returns
+        -------
+        Self and updates the following fields:
 
-    @abstractmethod
+        - :attr:`stage` - set to ``'prepared'``.
+        - :attr:`problem_kind` - kind of the :term:`OT` problem.
+        """
+
+    @abc.abstractmethod
     def solve(self, *args: Any, **kwargs: Any) -> "BaseProblem":
-        """Abstract solve method."""
+        """Solve the problem.
+
+        Parameters
+        ----------
+        args
+            Positional arguments.
+        kwargs
+            Keyword arguments.
+
+        Returns
+        -------
+        Self and updates the following fields:
+
+        - :attr:`stage` - set to ``'solved'``.
+        - :attr:`problem_kind` - kind of the :term:`OT` problem.
+        """
+
+    def save(
+        self,
+        path: Union[str, pathlib.Path],
+        overwrite: bool = False,
+    ) -> None:
+        """Save the problem to a file.
+
+        Parameters
+        ----------
+        path
+            Path where to save the problem.
+        overwrite
+            Whether to overwrite an existing file.
+
+        Returns
+        -------
+        Nothing, just saves the problem using :mod:`cloudpickle <pickle>`.
+        """
+        path = pathlib.Path(path)
+        if not overwrite and path.is_file():
+            raise RuntimeError(
+                f"Unable to write the model to an existing file `{path}`, " f"use `overwrite=True` to overwrite it."
+            )
+        with open(path, "wb") as fout:
+            cloudpickle.dump(self, fout)
+
+    @staticmethod
+    def load(
+        path: Union[str, pathlib.Path],
+    ) -> "BaseProblem":
+        """Load the model from a file.
+
+        Parameters
+        ----------
+        path
+            Path where the model is stored.
+
+        Returns
+        -------
+        The problem.
+        """
+        with open(path, "rb") as fin:
+            return cloudpickle.load(fin)
 
     @staticmethod
     def _get_mass(
         adata: AnnData,
         data: Optional[Union[str, ArrayLike]] = None,
         subset: Optional[Union[str, List[str], Tuple[int, int]]] = None,
         normalize: bool = True,
@@ -85,51 +153,50 @@
                     raise IndexError(f"Expected starting index to be smaller than `{adata.n_obs}`, found `{start}`.")
                 data = np.zeros((adata.n_obs,), dtype=float)
                 data[range(start, min(start + offset, adata.n_obs))] = 1.0
             else:
                 raise TypeError(f"Unable to interpret subset of type `{type(subset)}`.")
         elif not hasattr(data, "shape"):
             if subset is None:  # allow for numeric values
-                data = np.asarray(adata.obs[data], dtype=float)
+                data = (
+                    np.asarray(adata.obs[data], dtype=float)
+                    if pd_types.is_numeric_dtype(adata.obs[data])
+                    else np.ones((adata.n_obs,), dtype=float)
+                )
             else:
                 sset = subset if isinstance(subset, list) else [subset]  # type:ignore[list-item]
                 data = np.asarray(adata.obs[data].isin(sset), dtype=float)
         else:
             data = np.asarray(data, dtype=float)
 
         if split_mass:
             data = _split_mass(data)
 
         if data.ndim != 2:
             data = np.reshape(data, (-1, 1))
         if data.shape[0] != adata.n_obs:
             raise ValueError(f"Expected array of shape `({adata.n_obs,}, ...)`, found `{data.shape}`.")
-        if np.any(data < 0.0):
-            raise ValueError("Some entries have negative mass.")
-        total = np.sum(data, axis=0, keepdims=True)
-        if np.any(total <= 0.0):
-            raise ValueError("Some measures have no mass.")
-        return (data / total) if normalize else data
+
+        if normalize:
+            return data / np.sum(data, axis=0, keepdims=True)
+        return data
 
     @property
-    def stage(self) -> ProblemStage_t:
+    def stage(self) -> Literal["initialized", "prepared", "solved"]:
         """Problem stage."""
         return self._stage
 
     @property
     def problem_kind(self) -> ProblemKind_t:
         """Kind of the underlying problem."""
         return self._problem_kind
 
 
-@d.get_sections(base="OTProblem", sections=["Parameters", "Raises"])
-@d.dedent
 class OTProblem(BaseProblem):
-    """
-    Base class for all optimal transport problems.
+    """Base class for all :term:`OT` problems.
 
     Parameters
     ----------
     adata
         Source annotated data object.
     adata_tgt
         Target annotated data object. If :obj:`None`, use ``adata``.
@@ -138,38 +205,35 @@
     tgt_obs_mask
         Target observation mask that defines :attr:`adata_tgt`.
     src_var_mask
         Source variable mask that defines :attr:`adata_src`.
     tgt_var_mask
         Target variable mask that defines :attr:`adata_tgt`.
     src_key
-        Source key name, usually supplied by :class:`~moscot.base.problems.BaseCompoundProblem`.
+        Source key name, usually supplied by the :class:`~moscot.base.problems.BaseCompoundProblem`.
     tgt_key
-        Target key name, usually supplied by :class:`~moscot.base.problems.BaseCompoundProblem`.
-    kwargs
-        Keyword arguments for :class:`~moscot.base.problems.BaseProblem`.
+        Target key name, usually supplied by the :class:`~moscot.base.problems.BaseCompoundProblem`.
 
     Notes
     -----
-    If any of the source/target masks are specified, :attr:`adata_src`/:attr:`adata_tgt` will be a view.
+    If source/target mask is specified, :attr:`adata_src`/:attr:`adata_tgt` will be a view.
     """
 
     def __init__(
         self,
         adata: AnnData,
         adata_tgt: Optional[AnnData] = None,
         src_obs_mask: Optional[ArrayLike] = None,
         tgt_obs_mask: Optional[ArrayLike] = None,
         src_var_mask: Optional[ArrayLike] = None,
         tgt_var_mask: Optional[ArrayLike] = None,
         src_key: Optional[Any] = None,
         tgt_key: Optional[Any] = None,
-        **kwargs: Any,
     ):
-        super().__init__(**kwargs)
+        super().__init__()
         self._adata_src = adata
         self._adata_tgt = adata if adata_tgt is None else adata_tgt
         self._src_obs_mask = src_obs_mask
         self._tgt_obs_mask = tgt_obs_mask
         self._src_var_mask = src_var_mask
         self._tgt_var_mask = tgt_var_mask
         self._src_key = src_key
@@ -203,74 +267,76 @@
             y_kwargs["cost"] = cost
         x_kwargs["tag"] = Tag.POINT_CLOUD
         y_kwargs["tag"] = Tag.POINT_CLOUD
 
         x_array = TaggedArray.from_adata(self.adata_src, dist_key=self._src_key, **x_kwargs)
         y_array = TaggedArray.from_adata(self.adata_tgt, dist_key=self._tgt_key, **y_kwargs)
 
-        # restich together
         return TaggedArray(data_src=x_array.data_src, data_tgt=y_array.data_src, tag=Tag.POINT_CLOUD, cost=x_array.cost)
 
     @wrap_prepare
     def prepare(
         self,
         xy: Union[Mapping[str, Any], TaggedArray] = types.MappingProxyType({}),
         x: Union[Mapping[str, Any], TaggedArray] = types.MappingProxyType({}),
         y: Union[Mapping[str, Any], TaggedArray] = types.MappingProxyType({}),
         a: Optional[Union[bool, str, ArrayLike]] = None,
         b: Optional[Union[bool, str, ArrayLike]] = None,
         **kwargs: Any,
     ) -> "OTProblem":
-        """Prepare optimal transport problem.
+        """Prepare the :term:`OT` problem.
 
-        Depending on which arguments are passed:
+        Depending on which arguments are passed, the :attr:`problem_kind` will be:
 
-        - if only ``xy`` is non-empty, :attr:`problem_kind` will be ``'linear'``.
-        - if only ``x`` and ``y`` are non-empty, :attr:`problem_kind` will be ``'quadratic'``.
-        - if all ``xy``, ``x`` and ``y`` are non-empty, :attr:`problem_kind` will be ``'quadratic'``.
+        - if only ``xy`` is non-empty, :attr:`problem_kind = 'linear' <problem_kind>`.
+        - if only ``x`` and ``y`` are non-empty, :attr:`problem_kind = 'quadratic' <problem_kind>`.
+        - if all ``xy``, ``x`` and ``y`` are non-empty, :attr:`problem_kind = 'quadratic' <problem_kind>`.
 
         Parameters
         ----------
         xy
             Geometry defining the linear term. If a non-empty :class:`dict`,
             :meth:`~moscot.utils.tagged_array.TaggedArray.from_adata` will be called.
         x
-            First geometry defining the quadratic term. If a non-empty :class:`dict`,
+            Geometry defining the source :term:`quadratic term`. If a non-empty :class:`dict`,
             :meth:`~moscot.utils.tagged_array.TaggedArray.from_adata` will be called.
         y
-            Second geometry defining the quadratic term. If a non-empty :class:`dict`,
+            Geometry defining the target :term:`quadratic term`. If a non-empty :class:`dict`,
             :meth:`~moscot.utils.tagged_array.TaggedArray.from_adata` will be called.
         a
-            Source marginals. Valid value are:
+            Source :term:`marginals`. Valid options are:
 
-            - :class:`str`: key in :attr:`adata_src` :attr:`~anndata.AnnData.obs` where the marginals are stored.
-            - :class:`bool`: if `True`, compute the marginals from :attr:`adata_src`, otherwise use uniform.
-            - :class:`~numpy.ndarray`: array of shape ``[n,]`` containing the source marginals.
-            - :obj:`None`: uniform marginals.
+            - :class:`str` - key in :attr:`~anndata.AnnData.obs` where the source marginals are stored.
+            - :class:`bool` - if :obj:`True`, :meth:`estimate the marginals <estimate_marginals>`
+              from :attr:`adata_src`, otherwise use uniform marginals.
+            - :class:`~numpy.ndarray` - array of shape ``[n,]`` containing the source marginals.
+            - :obj:`None` - uniform marginals.
         b
-            Target marginals. Valid options are:
+            Target :term:`marginals`. Valid options are:
 
-            - :class:`str`: key in :attr:`adata_tgt` :attr:`~anndata.AnnData.obs` where the marginals are stored.
-            - :class:`bool`: if `True`, compute the marginals from :attr:`adata_tgt`, otherwise use uniform.
-            - :class:`~numpy.ndarray`: array of shape ``[m,]`` containing the target marginals.
-            - :obj:`None`: uniform marginals.
+            - :class:`str` - key in :attr:`~anndata.AnnData.obs` where the target marginals are stored.
+            - :class:`bool` - if :obj:`True`, :meth:`estimate the marginals <estimate_marginals>`
+              from :attr:`adata_tgt`, otherwise use uniform marginals.
+            - :class:`~numpy.ndarray` - array of shape ``[m,]`` containing the target marginals.
+            - :obj:`None` - uniform marginals.
         kwargs
-            Keyword arguments when creating the source/target marginals.
+            Keyword arguments for :meth:`estimate_marginals` when ``a = True`` or ``b = True``.
 
         Returns
         -------
-        Self and modifies the following attributes:
+        Self and updates the following fields:
 
-        - :attr:`xy`: geometry of shape ``[n, m]`` defining the linear term.
-        - :attr:`x`: first geometry of shape ``[n, n]`` defining  the quadratic term.
-        - :attr:`y`: second geometry of shape ``[m, m]`` defining the quadratic term.
-        - :attr:`a`: source marginals of shape ``[n,]``.
-        - :attr:`b`: target marginals of shape ``[m,]``.
-        - :attr:`problem_kind`: kind of the optimal transport problem.
-        - :attr:`solution`: set to :obj:`None`.
+        - :attr:`xy` - geometry of shape ``[n, m]`` defining the :term:`linear term`.
+        - :attr:`x` - geometry of shape ``[n, n]`` defining the source :term:`quadratic term`.
+        - :attr:`y` - geometry of shape ``[m, m]`` defining the target :term:`quadratic term`.
+        - :attr:`a` -  source :term:`marginals` of shape ``[n,]``.
+        - :attr:`b` - target :term:`marginals` of shape ``[m,]``.
+        - :attr:`solution` - set to :obj:`None`.
+        - :attr:`stage` - set to ``'prepared'``.
+        - :attr:`problem_kind` - kind of the :term:`OT` problem.
         """
         self._x = self._y = self._xy = self._solution = None
         # TODO(michalk8): in the future, have a better dispatch
         # fmt: off
         if xy and not x and not y:
             self._problem_kind = "linear"
             self._xy = xy if isinstance(xy, TaggedArray) else self._handle_linear(**xy)
@@ -298,40 +364,40 @@
         else:
             raise ValueError("Unable to prepare the data. Either only supply `xy=...`, or `x=..., y=...`, or all.")
         # fmt: on
         self._a = self._create_marginals(self.adata_src, data=a, source=True, **kwargs)
         self._b = self._create_marginals(self.adata_tgt, data=b, source=False, **kwargs)
         return self
 
-    @d.get_sections(base="OTProblem_solve", sections=["Parameters", "Raises"])
     @wrap_solve
     def solve(
         self,
         backend: Literal["ott"] = "ott",
         device: Optional[Device_t] = None,
         **kwargs: Any,
     ) -> "OTProblem":
-        """Solve optimal transport problem.
+        """Solve the :term:`OT` problem.
 
         Parameters
         ----------
         backend
             Which backend to use, see :func:`~moscot.backends.utils.get_available_backends`.
         device
-            Device where to transfer the solution, see :meth:`moscot.base.output.BaseSolverOutput.to`.
+            Transfer the solution to a different device, see :meth:`~moscot.base.output.BaseSolverOutput.to`.
+            If :obj:`None`, keep the output on the original device.
         kwargs
-            Keyword arguments for :class:`moscot.base.solver.BaseSolver` or
-            :meth:`moscot.base.solver.BaseSolver.__call__`.
+            Keyword arguments for :class:`~moscot.base.solver.BaseSolver` or its
+            :meth:`__call__ <moscot.base.solver.BaseSolver.__call__>` method.
 
         Returns
         -------
-        Self and modifies the following attributes:
+        Self and updates the following fields:
 
-        - :attr:`solver`: optimal transport solver.
-        - :attr:`solution`: optimal transport solution.
+        - :attr:`solver` - the :term:`OT` solver.
+        - :attr:`solution` - the :term:`OT` solution.
         """
         solver_class = backends.get_solver(self.problem_kind, backend=backend, return_class=True)
         init_kwargs, call_kwargs = solver_class._partition_kwargs(**kwargs)
         self._solver = solver_class(**init_kwargs)
 
         self._solution = self._solver(  # type: ignore[misc]
             xy=self._xy,
@@ -348,104 +414,116 @@
     def push(
         self,
         data: Optional[Union[str, ArrayLike]] = None,
         subset: Optional[Union[str, List[str], Tuple[int, int]]] = None,
         normalize: bool = True,
         *,
         split_mass: bool = False,
-        **kwargs: Any,
+        scale_by_marginals: bool = False,
     ) -> ArrayLike:
-        """Push mass through the :attr:`~moscot.base.output.BaseSolverOutput.transport_matrix`.
+        r"""Push data through the :attr:`~moscot.base.output.BaseSolverOutput.transport_matrix`.
 
         Parameters
         ----------
         data
             Data to push through the transport matrix. Valid options are:
 
-            - :class:`str`: key in :attr:`adata_src` :attr:`~anndata.AnnData.obs`.
-            - :class:`~numpy.ndarray`: array of shape ``[n,]``.
-            - :obj:`None`: depending on the ``subset``:
-
-              - :class:`list`: observation names to push in :attr:`adata_src` :attr:`~anndata.AnnData.obs_names`.
-              - :class:`tuple`: start and offset indices defining the mask.
-              - :obj:`None`: uniform array of 1s.
+            - :class:`~numpy.ndarray` - array of shape ``[n,]`` or ``[n, d]``.
+            - :class:`str` - key in :attr:`adata_src.obs['{data}'] <adata_src>`. If ``subset`` is a :class:`list`,
+              the data will be a boolean mask determined by the subset. Useful for categorical data.
+            - :obj:`None` - the value depends on the ``subset``.
+
+              - :class:`list` - names in :attr:`adata_src.obs_names <adata_src>` to push.
+              - :class:`tuple` - start and offset indices :math:`(subset[0], subset[0] + subset[1])`.
+                that define a boolean mask to push.
+              - :obj:`None` - uniform array of :math:`1`.
         subset
             Push values contained only within the subset.
         normalize
-            Whether to normalize the columns of ``data`` to sum to 1.
+            Whether to normalize the columns of ``data`` to sum to :math:`1`.
         split_mass
             Whether to split non-zero values in ``data`` into separate columns.
+        scale_by_marginals
+            Whether to scale by the source :term`marginals` :attr:`a`.
 
         Returns
         -------
-        Array of shape ``[m, d]``.
+        The transported values, array of shape ``[m, d]``.
         """
         if TYPE_CHECKING:
             assert isinstance(self.solution, BaseSolverOutput)
         data = self._get_mass(self.adata_src, data=data, subset=subset, normalize=normalize, split_mass=split_mass)
-        return self.solution.push(data, **kwargs)
+        return self.solution.push(data, scale_by_marginals=scale_by_marginals)
 
     @require_solution
     def pull(
         self,
         data: Optional[Union[str, ArrayLike]] = None,
         subset: Optional[Union[str, List[str], Tuple[int, int]]] = None,
         normalize: bool = True,
         *,
         split_mass: bool = False,
-        **kwargs: Any,
+        scale_by_marginals: bool = False,
     ) -> ArrayLike:
-        """Pull mass through the :attr:`~moscot.base.output.BaseSolverOutput.transport_matrix`.
+        r"""Pull data through the :attr:`~moscot.base.output.BaseSolverOutput.transport_matrix`.
 
         Parameters
         ----------
         data
             Data to pull through the transport matrix. Valid options are:
 
-            - :class:`str`: key in :attr:`adata_tgt` :attr:`~anndata.AnnData.obs`.
-            - :class:`~numpy.ndarray`: array of shape ``[m,]``.
-            - :obj:`None`: depending on the ``subset``:
-
-              - :class:`list`: observation names to pull in :attr:`adata_tgt` :attr:`~anndata.AnnData.obs_names`.
-              - :class:`tuple`: start and offset indices defining the mask.
-              - :obj:`None`: uniform array of 1s.
+            - :class:`~numpy.ndarray` - array of shape ``[m,]`` or ``[m, d]``.
+            - :class:`str` - key in :attr:`adata_tgt.obs['{data}'] <adata_tgt>`. If ``subset`` is a :class:`list`,
+              the data will be a boolean mask determined by the subset. Useful for categorical data.
+            - :obj:`None` - the value depends on the ``subset``.
+
+              - :class:`list` - names in :attr:`adata_tgt.obs_names <adata_tgt>` to pull.
+              - :class:`tuple` - start and offset indices :math:`(subset[0], subset[0] + subset[1])`.
+                that define a boolean mask to pull.
+              - :obj:`None` - uniform array of :math:`1`.
         subset
             Pull values contained only within the subset.
         normalize
-            Whether to normalize the columns of ``data`` to sum to 1.
+            Whether to normalize the columns of ``data`` to sum to :math:`1`.
         split_mass
             Whether to split non-zero values in ``data`` into separate columns.
+        scale_by_marginals
+            Whether to scale by the target :term`marginals` :attr:`b`.
 
         Returns
         -------
-        Array of shape ``[n, d]``.
+        The transported values, array of shape ``[n, d]``.
         """
         if TYPE_CHECKING:
             assert isinstance(self.solution, BaseSolverOutput)
         data = self._get_mass(self.adata_tgt, data=data, subset=subset, normalize=normalize, split_mass=split_mass)
-        return self.solution.pull(data, **kwargs)
+        return self.solution.pull(data, scale_by_marginals=scale_by_marginals)
 
     def set_solution(
         self, solution: Union[ArrayLike, pd.DataFrame, BaseSolverOutput], *, overwrite: bool = False, **kwargs: Any
     ) -> "OTProblem":
-        """Set the :attr:`solution`.
+        """Set a :attr:`solution` to the :term:`OT` problem.
 
         Parameters
         ----------
         solution
-            Solution for this problem. If a :class:`~pandas.DataFrame` is passed, its index and columns
-            must match the indexes of :attr:`adata_src` and :attr:`adata_tgt`, respectively.
+            Solution for this problem. If a :class:`~pandas.DataFrame` is passed,
+            its index must be equal to :attr:`adata_src.obs_names <adata_src>`
+            and its columns to :attr:`adata_tgt.obs_names <adata_tgt>`.
         overwrite
             Whether to overwrite an existing solution.
         kwargs
             Keyword arguments for :class:`~moscot.base.output.MatrixSolverOutput`.
 
         Returns
         -------
-        Set :attr:`solution` and return self.
+        Self and updates the following fields:
+
+        - :attr:`solution` - the :term:`OT` solution.
+        - :attr:`stage` - set to ``'solved'``.
         """
         if not overwrite and self.solution is not None:
             raise ValueError(f"`{self}` already contains a solution, use `overwrite=True` to overwrite it.")
 
         if isinstance(solution, pd.DataFrame):
             pd.testing.assert_series_equal(self.adata_src.obs_names.to_series(), solution.index.to_series())
             pd.testing.assert_series_equal(self.adata_tgt.obs_names.to_series(), solution.columns.to_series())
@@ -506,20 +584,45 @@
             logger.info(f"Computing pca with `n_comps={n_comps}` for `{term}` using `{msg}`")
             x = sc.pp.pca(x, n_comps=n_comps, **kwargs)
             if scaler is not None:
                 x = scaler.fit_transform(x)
             return {term: TaggedArray(x, tag=Tag.POINT_CLOUD)}
         raise ValueError(f"Expected `term` to be one of `x`, `y`, or `xy`, found `{term!r}`.")
 
+    @staticmethod
+    def _spatial_norm_callback(
+        term: Literal["x", "y"],
+        adata: AnnData,
+        adata_y: Optional[AnnData] = None,
+        **kwargs: Any,
+    ) -> Dict[Literal["x", "y"], TaggedArray]:
+        spatial_key = kwargs["spatial_key"]
+        if term == "x":
+            spatial = adata.obsm[spatial_key]
+        if term == "y":
+            if adata_y is None:
+                raise ValueError("When `term` is `y`, `adata_y` cannot be `None`.")
+            spatial = adata_y.obsm[spatial_key]
+
+        logger.info(f"Normalizing spatial coordinates of `{term}`.")
+        spatial = (spatial - spatial.mean()) / spatial.std()
+        return {term: TaggedArray(spatial, tag=Tag.POINT_CLOUD)}
+
     def _create_marginals(
-        self, adata: AnnData, *, source: bool, data: Optional[Union[bool, str, ArrayLike]] = None, **kwargs: Any
+        self,
+        adata: AnnData,
+        *,
+        source: bool,
+        data: Optional[Union[bool, str, ArrayLike]] = None,
+        marginal_kwargs: Dict[str, Any] = types.MappingProxyType({}),
+        **kwargs: Any,
     ) -> ArrayLike:
         if data is True:
-            marginals = self.estimate_marginals(adata, source=source, **kwargs)
-        elif data in (False, None):
+            marginals = self.estimate_marginals(adata, source=source, **marginal_kwargs, **kwargs)
+        elif data is False or data is None:
             marginals = np.ones((adata.n_obs,), dtype=float) / adata.n_obs
         elif isinstance(data, str):
             try:
                 marginals = np.asarray(adata.obs[data], dtype=float)
             except KeyError:
                 raise KeyError(f"Unable to find data in `adata.obs[{data!r}]`.") from None
         else:
@@ -529,114 +632,117 @@
             raise ValueError(
                 f"Expected {'source' if source else 'target'} marginals "
                 f"to have shape `{adata.n_obs,}`, found `{marginals.shape}`."
             )
         return marginals
 
     def estimate_marginals(self, adata: AnnData, *, source: bool, **kwargs: Any) -> ArrayLike:
-        """TODO."""
+        """Estimate the source or target :term:`marginals`.
+
+        .. note::
+            This function returns uniform marginals.
+
+        Parameters
+        ----------
+        adata
+            Annotated data object.
+        source
+            Whether to estimate the source or target :term:`marginals`.
+        kwargs
+            Additional keyword arguments.
+
+        Returns
+        -------
+        The estimated source or target marginals of shape ``[n,]`` or ``[m,]``, depending on the ``source``.
+        """
+        del kwargs
         return np.ones((adata.n_obs,), dtype=float) / adata.n_obs
 
-    @d.dedent
+    # TODO(michalk8): extend for point-clouds as Union[pd.DataFrame, Tuple[pd.DataFrame, pd.DataFrame]]
+    # TODO(michalk8): allow this to be nullified
     def set_xy(
         self,
         data: pd.DataFrame,
         tag: Literal["cost", "kernel"],
     ) -> None:
-        """
-        Set a custom cost matrix/kernel in the linear term.
+        """Set a cost/kernel matrix for the :term:`linear term`.
 
         Parameters
         ----------
-        %(data_set)s
-        %(tag_set)s
+        data
+            Cost or kernel matrix. Its index must be equal to :attr:`adata_src.obs_names <adata_src>`
+            and its columns to :attr:`adata_tgt.obs_names <adata_tgt>`.
+        tag
+            Whether ``data`` is a cost or a kernel matrix.
 
         Returns
         -------
-        None
+        Nothing, just updates the following fields:
+
+        - :attr:`xy` - the :term:`linear term`.
+        - :attr:`stage` - set to ``'prepared'``.
         """
-        if data.shape != self.shape:
-            raise ValueError(f"`data` is expected to have shape {self.shape} but found {data.shape}.")
-        if not isinstance(data, pd.DataFrame):
-            raise TypeError("If the data is to be validated, the data must be of type pandas.DataFrame.")
-        if list(data.index) != list(self.adata_src.obs_names):
-            raise ValueError(
-                "The index names of `data` do not correspond to `adata.obs_names` of the source distribution."
-            )
-        if list(data.columns) != list(self.adata_tgt.obs_names):
-            raise ValueError(
-                "The column names of `data` do not correspond to `adata.obs_names` of the target distribution."
-            )
-        self._xy = TaggedArray(data_src=data.values, data_tgt=None, tag=Tag(tag), cost="cost")
+        pd.testing.assert_series_equal(self.adata_src.obs_names.to_series(), data.index.to_series())
+        pd.testing.assert_series_equal(self.adata_tgt.obs_names.to_series(), data.columns.to_series())
+
+        self._xy = TaggedArray(data_src=data.to_numpy(), data_tgt=None, tag=Tag(tag), cost="cost")
         self._stage = "prepared"
 
-    @d.dedent
     def set_x(self, data: pd.DataFrame, tag: Literal["cost", "kernel"]) -> None:
-        """
-        Set a custom cost matrix/kernel in the quadratic source term.
+        """Set a cost/kernel matrix for the source :term:`quadratic term`.
 
         Parameters
         ----------
-        %(data_set)s
-        %(tag_set)s
+        data
+            Cost or kernel matrix. Its index must be equal to :attr:`adata_src.obs_names <adata_src>`
+            and its columns to :attr:`adata_src.obs_names <adata_src>`.
+        tag
+            Whether ``data`` is a cost or a kernel matrix.
 
         Returns
         -------
-        None
+        Nothing, just updates the following fields:
+
+        - :attr:`x` - the source :term:`quadratic term`.
+        - :attr:`stage` - set to ``'prepared'``.
         """
+        pd.testing.assert_series_equal(self.adata_src.obs_names.to_series(), data.index.to_series())
+        pd.testing.assert_series_equal(self.adata_src.obs_names.to_series(), data.columns.to_series())
+
         if self.problem_kind == "linear":
-            logger.info(f"Changing the problem type from {self.problem_kind} to fused-quadratic.")
+            logger.info(f"Changing the problem type from {self.problem_kind!r} to 'quadratic (fused)'.")
             self._problem_kind = "quadratic"
-        expected_shape = self.shape[0], self.shape[0]
-        if data.shape != expected_shape:
-            raise ValueError(f"`data` is expected to have shape {expected_shape} but found {data.shape}.")
-        if not isinstance(data, pd.DataFrame):
-            raise TypeError("If the data is to be validated, the data must be of type pandas.DataFrame.")
-        if list(data.index) != list(self.adata_src.obs_names):
-            raise ValueError(
-                "The index names of `data` do not correspond to `adata.obs_names` of the source distribution."
-            )
-        if list(data.columns) != list(self.adata_src.obs_names):
-            raise ValueError(
-                "The column names of `data` do not correspond to `adata.obs_names` of the source distribution."
-            )
-        self._x = TaggedArray(data_src=data.values, data_tgt=None, tag=Tag(tag), cost="cost")
+        self._x = TaggedArray(data_src=data.to_numpy(), data_tgt=None, tag=Tag(tag), cost="cost")
         self._stage = "prepared"
 
-    @d.dedent
     def set_y(self, data: pd.DataFrame, tag: Literal["cost", "kernel"]) -> None:
-        """
-        Set a custom cost matrix/kernel in the quadratic target term.
+        """Set a cost/kernel matrix for the target :term:`quadratic term`.
 
         Parameters
         ----------
-        %(data_set)s
-        %(tag_set)s
+        data
+            Cost or kernel matrix. Its index must be equal to :attr:`adata_tgt.obs_names <adata_tgt>`
+            and its columns to :attr:`adata_tgt.obs_names <adata_tgt>`.
+        tag
+            Whether ``data`` is a cost or a kernel matrix.
 
         Returns
         -------
-        None
+        Nothing, just updates the following fields:
+
+        - :attr:`y` - the target :term:`quadratic term`.
+        - :attr:`stage` - set to ``'prepared'``.
         """
+        pd.testing.assert_series_equal(self.adata_tgt.obs_names.to_series(), data.index.to_series())
+        pd.testing.assert_series_equal(self.adata_tgt.obs_names.to_series(), data.columns.to_series())
+
         if self.problem_kind == "linear":
-            logger.info(f"Changing the problem type from {self.problem_kind} to fused-quadratic.")
+            logger.info(f"Changing the problem type from {self.problem_kind!r} to 'quadratic (fused)'.")
             self._problem_kind = "quadratic"
-        expected_shape = self.shape[1], self.shape[1]
-        if data.shape != expected_shape:
-            raise ValueError(f"`data` is expected to have shape {expected_shape} but found {data.shape}.")
-        if not isinstance(data, pd.DataFrame):
-            raise TypeError("If the data is to be validated, the data must be of type pandas.DataFrame.")
-        if list(data.index) != list(self.adata_tgt.obs_names):
-            raise ValueError(
-                "The index names of `data` do not correspond to `adata.obs_names` of the source distribution."
-            )
-        if list(data.columns) != list(self.adata_tgt.obs_names):
-            raise ValueError(
-                "The column names of `data` do not correspond to `adata.obs_names` of the source distribution."
-            )
-        self._y = TaggedArray(data_src=data.values, data_tgt=None, tag=Tag(tag), cost="cost")
+        self._y = TaggedArray(data_src=data.to_numpy(), data_tgt=None, tag=Tag(tag), cost="cost")
         self._stage = "prepared"
 
     @property
     def adata_src(self) -> AnnData:
         """Source annotated data object."""
         adata = self._adata_src if self._src_obs_mask is None else self._adata_src[self._src_obs_mask]
         if not adata.n_obs:
@@ -655,50 +761,50 @@
         adata = adata if self._tgt_var_mask is None else adata[:, self._tgt_var_mask]
         if not adata.n_vars:
             raise ValueError("No variables in the target `AnnData`.")
         return adata
 
     @property
     def shape(self) -> Tuple[int, int]:
-        """Shape of the optimal transport problem."""
+        """Shape of the :term:`OT` problem."""
         return self.adata_src.n_obs, self.adata_tgt.n_obs
 
     @property
     def solution(self) -> Optional[BaseSolverOutput]:
-        """Solution of the optimal transport problem."""
+        """Solution of the :term:`OT` problem."""
         return self._solution
 
     @property
     def solver(self) -> Optional[OTSolver[BaseSolverOutput]]:
-        """Optimal transport solver."""
+        """:term:`OT` solver."""
         return self._solver
 
     @property
     def xy(self) -> Optional[TaggedArray]:
-        """Geometry defining the linear term."""
+        """Geometry defining the :term:`linear term`."""
         return self._xy
 
     @property
     def x(self) -> Optional[TaggedArray]:
-        """First geometry defining the quadratic term."""
+        """Geometry defining the source :term:`quadratic term`."""
         return self._x
 
     @property
     def y(self) -> Optional[TaggedArray]:
-        """Second geometry defining the quadratic term."""
+        """Geometry defining the target :term:`quadratic term`."""
         return self._y
 
     @property
     def a(self) -> Optional[ArrayLike]:
-        """Source marginals."""
+        """Source :term:`marginals`."""
         return self._a
 
     @property
     def b(self) -> Optional[ArrayLike]:
-        """Target marginals."""
+        """Target :term:`marginals`."""
         return self._b
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}[stage={self.stage!r}, shape={self.shape!r}]"
 
     def __str__(self) -> str:
         return repr(self)
```

### Comparing `moscot-0.3.0/src/moscot/base/solver.py` & `moscot-0.3.1/src/moscot/base/solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     Optional,
     Set,
     Tuple,
     TypeVar,
     Union,
 )
 
-from moscot._docs._docs import d
 from moscot._logging import logger
 from moscot._types import ArrayLike, Device_t, ProblemKind_t
 from moscot.base.output import BaseSolverOutput
 from moscot.utils.tagged_array import Tag, TaggedArray
 
 __all__ = ["BaseSolver", "OTSolver"]
 
@@ -161,16 +160,14 @@
         call_kws, shared_kws = cls._call_kwargs()
         init_kwargs = {k: v for k, v in kwargs.items() if k not in call_kws or k in shared_kws}
         call_kwargs = {k: v for k, v in kwargs.items() if k in call_kws or k in shared_kws}
 
         return init_kwargs, call_kwargs
 
 
-@d.get_sections(base="OTSolver", sections=["Parameters", "Raises"])
-@d.dedent
 class OTSolver(TagConverter, BaseSolver[O], abc.ABC):
     """Base class for optimal transport solvers."""
 
     def __call__(
         self,
         xy: Optional[Union[TaggedArray, ArrayLike, Tuple[ArrayLike, ArrayLike]]] = None,
         x: Optional[Union[TaggedArray, ArrayLike]] = None,
```

### Comparing `moscot-0.3.0/src/moscot/costs/_costs.py` & `moscot-0.3.1/src/moscot/costs/_costs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,105 +1,141 @@
-from typing import Any, List, Mapping, Optional
+from typing import Any, Callable, Dict, List, Mapping, Optional, Union
 
 import networkx as nx
 import numpy as np
 
+from anndata import AnnData
+
 from moscot._logging import logger
 from moscot._types import ArrayLike
 from moscot.base.cost import BaseCost
 from moscot.costs._utils import register_cost
 
 __all__ = ["LeafDistance", "BarcodeDistance"]
 
 
 @register_cost("barcode_distance", backend="moscot")
 class BarcodeDistance(BaseCost):
-    """Barcode distance."""
+    """Scaled `Hamming distance <https://en.wikipedia.org/wiki/Hamming_distance>`_ between barcodes.
 
-    @property
-    def data(self) -> ArrayLike:
+    .. seealso::
+        - See :doc:`../notebooks/examples/problems/700_barcode_distance` on how to use this cost
+          in the :class:`~moscot.problems.time.LineageProblem`.
+
+    Parameters
+    ----------
+    adata
+        Annotated data object.
+    kwargs
+        Additional keyword arguments for the :class:`~moscot.base.cost.BaseCost`.
+    """
+
+    def __init__(self, adata: AnnData, **kwargs: Any):
+        super().__init__(adata, **kwargs)
         try:
-            container = getattr(self.adata, self._attr)
-            return container[self._key]
+            self._barcodes = getattr(self.adata, self._attr)[self._key].astype(np.int64)
         except AttributeError:
             raise AttributeError(f"`Anndata` has no attribute `{self._attr}`.") from None
         except KeyError:
             raise KeyError(f"Unable to find data in `adata.{self._attr}[{self._key!r}]`.") from None
 
     def _compute(
         self,
         *_: Any,
         **__: Any,
     ) -> ArrayLike:
         logger.info("Computing barcode distance")
-        barcodes = self.data
-        n_cells = barcodes.shape[0]
+        n_cells = self.barcodes.shape[0]
+
+        # TODO(michalk8): use numba
         distances = np.zeros((n_cells, n_cells))
         for i in range(n_cells):
             distances[i, i + 1 :] = [
-                self._scaled_hamming_dist(barcodes[i, :], barcodes[j, :]) for j in range(i + 1, n_cells)
+                _scaled_hamming_dist(self.barcodes[i, :], self.barcodes[j, :]) for j in range(i + 1, n_cells)
             ]
-        return distances + np.transpose(distances)
-
-    @staticmethod
-    def _scaled_hamming_dist(x: ArrayLike, y: ArrayLike) -> float:
-        """Adapted from `LineageOT <https://github.com/aforr/LineageOT/>`_."""
-        shared_indices = (x >= 0) & (y >= 0)
-        b1 = x[shared_indices]
-
-        # there may not be any sites where both were measured
-        if not len(b1):
-            return np.nan
-        b2 = y[shared_indices]
+        return distances + distances.T
 
-        differences = b1 != b2
-        double_scars = differences & (b1 != 0) & (b2 != 0)
-
-        return (np.sum(differences) + np.sum(double_scars)) / len(b1)
+    @property
+    def barcodes(self) -> ArrayLike:
+        """Barcodes."""
+        return self._barcodes
 
 
 @register_cost("leaf_distance", backend="moscot")
 class LeafDistance(BaseCost):
-    """Tree leaf distance."""
-
-    @property
-    def data(self) -> nx.Graph:
-        try:
-            if self._attr != "uns":
-                raise NotImplementedError(f"Extracting trees from `adata.{self._attr}` is not yet implemented.")
+    """`Shortest path <https://en.wikipedia.org/wiki/Shortest_path_problem>`_ distance on a weighted tree.
 
-            tree = self.adata.uns[self._key][self._dist_key]
-            if not isinstance(tree, nx.Graph):
-                raise TypeError(
-                    f"Expected the tree in `adata.uns[{self._key!r}][{self._dist_key!r}]` "
-                    f"to be a `networkx.DiGraph`, found `{type(tree)}`."
-                )
+    .. seealso::
+        - See :doc:`../notebooks/examples/problems/600_leaf_distance` on how to use this cost
+          in the :class:`~moscot.problems.time.LineageProblem`.
+
+    Parameters
+    ----------
+    adata
+        Annotated data object. The tree is always extracted from the :attr:`~anndata.AnnData.uns` attribute.
+    weight
+        If a :class:`str`, it is the edge weight attribute of the :attr:`tree`.
+        If a function, it must accept arguments as described in
+        :func:`~networkx.algorithms.shortest_paths.weighted.multi_source_dijkstra`.
+    kwargs
+        Keyword arguments for the :class:`~moscot.base.cost.BaseCost`.
+    """
+
+    def __init__(
+        self, adata: AnnData, weight: Union[str, Callable[[Any, Any, Dict[Any, Any]], float]] = "weight", **kwargs: Any
+    ):
+        kwargs["attr"] = "uns"
+        super().__init__(adata, **kwargs)
+        self._weight = weight
 
-            return tree
+        location = f"adata.{self._attr}[{self._key!r}][{self._dist_key!r}]"
+        try:
+            self._tree = getattr(self.adata, self._attr)[self._key][self._dist_key]
+            if not isinstance(self.tree, nx.Graph):
+                raise TypeError(f"Expected tree in `{location}` to be a `networkx.Graph`, found `{type(self.tree)}`.")
         except KeyError:
-            raise KeyError(f"Unable to find tree in `adata.{self._attr}[{self._key!r}][{self._dist_key!r}]`.") from None
+            raise KeyError(f"Unable to find tree in `{location}`.") from None
 
     def _compute(
         self,
         **kwargs: Any,
     ) -> ArrayLike:
         logger.info("Computing tree distance")
-        tree = self.data
-        undirected_tree = tree.to_undirected()
-        leaves = self._get_leaves(undirected_tree)
-        n_leaves = len(leaves)
+        undirected_tree = self.tree.to_undirected()
+        leaves = self._get_leaves()
+        distances = np.zeros((len(leaves), len(leaves)), dtype=float)
 
-        distances = np.zeros((n_leaves, n_leaves), dtype=np.float_)
         for i, leaf in enumerate(leaves):
             # TODO(@MUCDK): more efficient, problem: `target`in `multi_source_dijkstra` cannot be chosen as a subset
-            distance_dictionary = nx.multi_source_dijkstra(undirected_tree, [leaf], **kwargs)[0]
-            distances[i, :] = [distance_dictionary.get(leaf) for leaf in leaves]
+            dist, _ = nx.multi_source_dijkstra(undirected_tree, [leaf], weight=self._weight, **kwargs)
+            distances[i, :] = [dist.get(leaf) for leaf in leaves]
 
         return distances
 
-    def _get_leaves(self, tree: nx.Graph, cell_to_leaf: Optional[Mapping[str, Any]] = None) -> List[Any]:
-        leaves = [node for node in tree if tree.degree(node) == 1]
+    def _get_leaves(self, cell_to_leaf: Optional[Mapping[str, Any]] = None) -> List[Any]:
+        leaves = {node for node in self.tree if self.tree.degree(node) == 1}
         if not set(self.adata.obs_names).issubset(leaves):
             if cell_to_leaf is None:
                 raise ValueError("Leaves do not match `AnnData`'s observation names, please specify `cell_to_leaf`.")
-            return [cell_to_leaf[cell] for cell in self.adata.obs.index]
+            return [cell_to_leaf[cell] for cell in self.adata.obs_names]
         return [cell for cell in self.adata.obs_names if cell in leaves]
+
+    @property
+    def tree(self) -> nx.DiGraph:
+        """Tree."""
+        return self._tree
+
+
+def _scaled_hamming_dist(x: ArrayLike, y: ArrayLike) -> float:
+    # Adapted from `LineageOT <https://github.com/aforr/LineageOT/>`_.
+    shared_indices = (x >= 0) & (y >= 0)
+    b1 = x[shared_indices]
+
+    # there may not be any sites where both were measured
+    if not len(b1):
+        return np.nan
+    b2 = y[shared_indices]
+
+    differences = b1 != b2
+    double_scars = differences & (b1 != 0) & (b2 != 0)
+
+    return (np.sum(differences) + np.sum(double_scars)) / len(b1)
```

### Comparing `moscot-0.3.0/src/moscot/costs/_utils.py` & `moscot-0.3.1/src/moscot/costs/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 def get_available_costs(backend: Optional[str] = None) -> Dict[str, Tuple[str, ...]]:
     """Return available costs.
 
     Parameters
     ----------
     backend
-        Select cost specific to a backend. If ``None``, return costs for each backend.
+        Select cost specific to a backend. If :obj:`None`, return the costs for each backend.
 
     Returns
     -------
     Dictionary with keys as backend names and values as registered cost functions.
     """
     groups: Dict[str, List[str]] = collections.defaultdict(list)
     for key in _REGISTRY:
```

### Comparing `moscot-0.3.0/src/moscot/datasets.py` & `moscot-0.3.1/src/moscot/datasets.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import contextlib
 import os
 import pathlib
 import pickle
 import shutil
 import tempfile
 import urllib.request
-import warnings
 from types import MappingProxyType
 from typing import Any, Dict, List, Literal, Mapping, Optional, Tuple
 
 import networkx as nx
 import numpy as np
 import pandas as pd
 
+import anndata as ad
 from anndata import AnnData
 from scanpy import read
 
 from moscot._types import PathLike
 
 __all__ = [
     "mosta",
     "hspc",
     "drosophila",
     "c_elegans",
     "zebrafish",
+    "bone_marrow",
     "sim_align",
     "simulate_data",
-    "bone_marrow",
 ]
 
 
 def mosta(
     path: PathLike = "~/.cache/moscot/mosta.h5ad",
     force_download: bool = False,
     **kwargs: Any,
@@ -53,15 +53,15 @@
 
     Returns
     -------
     Annotated data object.
     """
     return _load_dataset_from_url(
         path,
-        backup_url="https://figshare.com/ndownloader/files/37953852",
+        backup_url="https://figshare.com/ndownloader/files/40569779",
         expected_shape=(54134, 2000),
         force_download=force_download,
         **kwargs,
     )
 
 
 def hspc(
@@ -87,21 +87,24 @@
     kwargs
         Keyword arguments for :func:`scanpy.read`.
 
     Returns
     -------
     Annotated data object.
     """
-    return _load_dataset_from_url(
+    dataset = _load_dataset_from_url(
         path,
         backup_url="https://figshare.com/ndownloader/files/37993503",
         expected_shape=(4000, 2000),
         force_download=force_download,
         **kwargs,
     )
+    dataset.obs["day"] = dataset.obs["day"].astype("category")  # better solution to this?
+
+    return dataset
 
 
 def drosophila(
     path: PathLike = "~/.cache/moscot/drosophila.h5ad",
     *,
     spatial: bool,
     force_download: bool = False,
@@ -183,15 +186,15 @@
 
 
 def zebrafish(
     path: PathLike = "~/.cache/moscot/zebrafish.h5ad",
     force_download: bool = False,
     **kwargs: Any,
 ) -> Tuple[AnnData, Dict[str, nx.DiGraph]]:
-    """Lineage-traced scRNA-seq time-series dataset of zebrafish heart regeneration :cite:`hu:22`.
+    """Lineage-traced scRNA-seq time-series dataset of Zebrafish heart regeneration :cite:`hu:22`.
 
     Contains gene expression vectors, LINNAEUS :cite:`spanjaard:18` reconstructed lineage trees,
     a low-dimensional embedding, and additional metadata.
 
     Parameters
     ----------
     path
@@ -254,15 +257,15 @@
             backup_url="https://figshare.com/ndownloader/files/40195114",
             expected_shape=(6224, 2000),
             force_download=force_download,
             **kwargs,
         )
     return _load_dataset_from_url(
         path + "_atac.h5ad",
-        backup_url="https://figshare.com/ndownloader/files/40195102",
+        backup_url="https://figshare.com/ndownloader/files/41013551",
         expected_shape=(6224, 8000),
         force_download=force_download,
         **kwargs,
     )
 
 
 def tedsim(
@@ -334,15 +337,15 @@
 
 
 def simulate_data(
     n_distributions: int = 2,
     cells_per_distribution: int = 20,
     n_genes: int = 60,
     key: Literal["day", "batch"] = "batch",
-    var: float = 1,
+    var: float = 1.0,
     obs_to_add: Mapping[str, Any] = MappingProxyType({"celltype": 3}),
     marginals: Optional[Tuple[str, str]] = None,
     seed: int = 0,
     quad_term: Optional[Literal["tree", "barcode", "spatial"]] = None,
     lin_cost_matrix: Optional[str] = None,
     quad_cost_matrix: Optional[str] = None,
     **kwargs: Any,
@@ -388,24 +391,20 @@
     adatas = [
         AnnData(
             X=rng.multivariate_normal(
                 mean=kwargs.pop("mean", np.arange(n_genes)),
                 cov=kwargs.pop("cov", var * np.diag(np.ones(n_genes))),
                 size=cells_per_distribution,
             ),
-            dtype=float,
         )
         for _ in range(n_distributions)
     ]
-    # remove once new `anndata` is release
-    with warnings.catch_warnings():
-        warnings.simplefilter("ignore", category=FutureWarning)
-        adata = adatas[0].concatenate(*adatas[1:], batch_key=key)
+    adata = ad.concat(adatas, label=key, index_unique="-")
     if key == "day":
-        adata.obs["day"] = pd.to_numeric(adata.obs["day"])
+        adata.obs["day"] = pd.to_numeric(adata.obs["day"]).astype("category")
     for k, val in obs_to_add.items():
         adata.obs[k] = rng.choice(range(val), len(adata))
     if marginals:
         adata.obs[marginals[0]] = rng.uniform(1e-5, 1, len(adata))
         adata.obs[marginals[1]] = rng.uniform(1e-5, 1, len(adata))
     if quad_term == "tree":
         adata.uns["trees"] = {}
```

### Comparing `moscot-0.3.0/src/moscot/plotting/_utils.py` & `moscot-0.3.1/src/moscot/plotting/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import collections
 import contextlib
 import copy
-from types import MappingProxyType
+import pathlib
+import types
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     List,
     Mapping,
     Optional,
@@ -206,16 +207,16 @@
     row_annotation_label: Optional[str] = None,
     col_annotation_label: Optional[str] = None,
     cont_cmap: Union[str, mpl.colors.Colormap] = "viridis",
     annotate_values: Optional[str] = "{x:.2f}",
     fontsize: float = 7.0,
     figsize: Optional[Tuple[float, float]] = None,
     dpi: Optional[int] = None,
-    save: Optional[str] = None,
-    cbar_kwargs: Mapping[str, Any] = MappingProxyType({}),
+    save: Optional[Union[str, pathlib.Path]] = None,
+    cbar_kwargs: Mapping[str, Any] = types.MappingProxyType({}),
     ax: Optional[mpl.axes.Axes] = None,
     **kwargs: Any,
 ) -> plt.Figure:
     cbar_kwargs = dict(cbar_kwargs)
 
     if ax is None:
         fig, ax = plt.subplots(constrained_layout=True, dpi=dpi, figsize=figsize)
@@ -391,15 +392,15 @@
     cont_cmap: Optional[Union[str, mpl.colors.Colormap]] = "viridis",
     title: Optional[Union[str, List[str]]] = None,
     suptitle: Optional[str] = None,
     figsize: Optional[Tuple[float, float]] = None,
     dpi: Optional[int] = None,
     dot_scale_factor: float = 2.0,
     na_color: str = "#e8ebe9",
-    save: Optional[str] = None,
+    save: Optional[Union[str, pathlib.Path]] = None,
     ax: Optional[mpl.axes.Axes] = None,
     suptitle_fontsize: Optional[float] = None,
     **kwargs: Any,
 ) -> Optional[plt.Figure]:
     if time_points is not None:
         time_points = sorted(time_points)
     if cont_cmap is None or isinstance(cont_cmap, str):
```

### Comparing `moscot-0.3.0/src/moscot/problems/_utils.py` & `moscot-0.3.1/src/moscot/problems/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,17 +52,15 @@
     xy: Mapping[str, Any] = types.MappingProxyType({}),
     x: Mapping[str, Any] = types.MappingProxyType({}),
     y: Mapping[str, Any] = types.MappingProxyType({}),
     cost: Optional[Union[CostFn_t, Mapping[str, CostFn_t]]] = None,
     cost_kwargs: CostKwargs_t = types.MappingProxyType({}),
     **_: Any,
 ) -> Tuple[Dict[str, Any], Dict[str, Any], Dict[str, Any]]:
-    x = dict(x)
-    y = dict(y)
-    xy = dict(xy)
+    xy, x, y = dict(xy), dict(x), dict(y)
     if cost is None:
         return xy, x, y
     if isinstance(cost, str):  # if cost is a str, we use it in all terms
         if xy and ("x_cost" not in xy or "y_cost" not in xy):
             xy["x_cost"] = xy["y_cost"] = cost
         if x and "cost" not in x:
             x["cost"] = cost
```

### Comparing `moscot-0.3.0/src/moscot/problems/space/_mixins.py` & `moscot-0.3.1/src/moscot/problems/space/_mixins.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,31 +8,27 @@
     Mapping,
     Optional,
     Sequence,
     Tuple,
     Union,
 )
 
+import networkx as nx
 import numpy as np
 import pandas as pd
 import scipy.sparse as sp
-from networkx import NetworkXNoPath
-from pandas.api.types import is_categorical_dtype
+import scipy.stats as st
 from scipy.linalg import svd
-from scipy.sparse.linalg import LinearOperator
 from scipy.spatial import ConvexHull
-from scipy.stats import pearsonr, spearmanr
 from sklearn.metrics import pairwise_distances
 from sklearn.neighbors import NearestNeighbors
 
 from anndata import AnnData
 
 from moscot import _constants
-from moscot._docs._docs import d
-from moscot._docs._docs_mixins import d_mixins
 from moscot._logging import logger
 from moscot._types import ArrayLike, Device_t, Str_Dict_t
 from moscot.base.problems._mixins import AnalysisMixin, AnalysisMixinProtocol
 from moscot.base.problems.compound_problem import B, K
 from moscot.utils.subset_policy import StarPolicy
 
 __all__ = ["SpatialAlignmentMixin", "SpatialMappingMixin"]
@@ -44,38 +40,26 @@
     spatial_key: Optional[str]
     _spatial_key: Optional[str]
     batch_key: Optional[str]
 
     def _subset_spatial(  # type:ignore[empty-body]
         self: "SpatialAlignmentMixinProtocol[K, B]",
         k: K,
-        spatial_key: Optional[str] = None,
+        spatial_key: str,
     ) -> ArrayLike:
         ...
 
     def _interpolate_scheme(  # type:ignore[empty-body]
         self: "SpatialAlignmentMixinProtocol[K, B]",
         reference: K,
         mode: Literal["warp", "affine"],
-        spatial_key: Optional[str] = None,
+        spatial_key: str,
     ) -> Tuple[Dict[K, ArrayLike], Optional[Dict[K, Optional[ArrayLike]]]]:
         ...
 
-    @staticmethod
-    def _affine(  # type:ignore[empty-body]
-        tmap: LinearOperator, src: ArrayLike, tgt: ArrayLike
-    ) -> Tuple[ArrayLike, ArrayLike]:
-        ...
-
-    @staticmethod
-    def _warp(  # type: ignore[empty-body]
-        tmap: LinearOperator, src: ArrayLike, _: ArrayLike
-    ) -> Tuple[ArrayLike, Optional[ArrayLike]]:
-        ...
-
     def _cell_transition(
         self: AnalysisMixinProtocol[K, B],
         *args: Any,
         **kwargs: Any,
     ) -> pd.DataFrame:
         ...
 
@@ -107,134 +91,173 @@
         self._spatial_key: Optional[str] = None
         self._batch_key: Optional[str] = None
 
     def _interpolate_scheme(  # type: ignore[misc]
         self: SpatialAlignmentMixinProtocol[K, B],
         reference: K,
         mode: Literal["warp", "affine"],
-        spatial_key: Optional[str] = None,
+        spatial_key: str,
     ) -> Tuple[Dict[K, ArrayLike], Optional[Dict[K, Optional[ArrayLike]]]]:
         """Scheme for interpolation."""
         # get reference
         src = self._subset_spatial(reference, spatial_key=spatial_key)
         transport_maps: Dict[K, ArrayLike] = {reference: src}
         transport_metadata: Dict[K, Optional[ArrayLike]] = {}
         if mode == "affine":
             src -= src.mean(0)
             transport_metadata = {reference: np.diag((1, 1))}  # 2d data
 
-        # get policy
+        # get the reference
         reference_ = [reference] if isinstance(reference, str) else reference
         full_steps = self._policy._graph
         starts = set(itertools.chain.from_iterable(full_steps)) - set(reference_)  # type: ignore[call-overload]
 
         if mode == "affine":
-            _transport = self._affine
+            _transport = _affine
         elif mode == "warp":
-            _transport = self._warp
+            _transport = _warp
         else:
             raise NotImplementedError(f"Alignment mode `{mode!r}` is not yet implemented.")
 
         steps = {}
         for start in starts:
             try:
                 steps[start, reference, True] = self._policy.plan(start=start, end=reference)
-            except NetworkXNoPath:
+            except nx.NetworkXNoPath:
                 steps[reference, start, False] = self._policy.plan(start=reference, end=start)
 
         for (start, end, forward), path in steps.items():
             tmap = self._interpolate_transport(path=path, scale_by_marginals=True)
             # make `tmap` to have shape `(m, n_ref)` and apply it to `src` of shape `(n_ref, d)`
             key, tmap = (start, tmap) if forward else (end, tmap.T)
             spatial_data = self._subset_spatial(key, spatial_key=spatial_key)
             transport_maps[key], transport_metadata[key] = _transport(tmap, src=src, tgt=spatial_data)
 
+        # TODO(michalk8): always return the metadata?
         return transport_maps, (transport_metadata if mode == "affine" else None)
 
-    @d.dedent
     def align(  # type: ignore[misc]
         self: SpatialAlignmentMixinProtocol[K, B],
-        reference: K,
+        reference: Optional[K] = None,
         mode: Literal["warp", "affine"] = "warp",
         spatial_key: Optional[str] = None,
-        inplace: bool = True,
-    ) -> Optional[Union[ArrayLike, Tuple[ArrayLike, Optional[Dict[K, Optional[ArrayLike]]]]]]:
-        """
-        Align spatial data.
+        key_added: Optional[str] = None,
+    ) -> Optional[Tuple[ArrayLike, Optional[Dict[K, Optional[ArrayLike]]]]]:
+        """Align the spatial data.
 
         Parameters
         ----------
         reference
-            Reference key.
+            Reference key. If a :class:`star policy <moscot.utils.subset_policy.StarPolicy>` was used,
+            its reference will always be used.
         mode
-            Alignment mode:
+            Alignment mode. Valid options are:
 
-                - "warp": warp the data to the reference.
-                - "affine": align the data to the reference using affine transformation.
-
-        %(inplace)s
+            - ``'warp'`` - warp the data to the ``reference``.
+            - ``'affine'`` - align the data to the ``reference`` using affine transformation.
+        spatial_key
+            Key in :attr:`~anndata.AnnData.obsm` where the spatial coordinates are stored.
+            If :obj:`None`, use :attr:`spatial_key`.
+        key_added
+            Key in :attr:`~anndata.AnnData.obsm` and :attr:`~anndata.AnnData.uns` where to store the alignment.
 
         Returns
         -------
-        %(alignment_mixin_returns)s
-        """
+        Depending on the ``key_added``:
+
+        - :obj:`None` - returns the aligned coordinates and metadata.
+          The metadata is :obj:`None` when ``mode != 'affine'``.
+        - :class:`str` - updates :attr:`adata` with the following fields:
+
+          - :attr:`obsm['{key_added}'] <anndata.AnnData.obsm>` - the aligned spatial coordinates.
+          - :attr:`uns['{key_added}']['alignment_metadata'] <anndata.AnnData.uns>` - the metadata.
+        """
+        if isinstance(self._policy, StarPolicy):
+            reference = self._policy.reference
+            logger.debug(f"Setting `reference={reference}`.")
+        if reference is None:
+            raise ValueError("Please specify `reference=...`.")
         if reference not in self._policy._cat:
-            raise ValueError(f"Reference `{reference}` is not in policy's categories: `{self._policy._cat}`.")
-        if isinstance(self._policy, StarPolicy) and reference != self._policy.reference:
-            # TODO(michalk8): just warn + optional reference?
-            raise ValueError(f"Expected reference to be `{self._policy.reference}`, found `{reference}`.")
+            raise ValueError(f"Reference `{reference}` is not in policy's categories `{self._policy._cat}`.")
+
+        if spatial_key is None:
+            spatial_key = self.spatial_key
+
         aligned_maps, aligned_metadata = self._interpolate_scheme(
-            reference=reference, mode=mode, spatial_key=spatial_key
+            reference=reference, mode=mode, spatial_key=spatial_key  # type: ignore[arg-type]
         )
         aligned_basis = np.vstack([aligned_maps[k] for k in self._policy._cat])
-        if mode == "affine":
-            if not inplace:
-                return aligned_basis, aligned_metadata
-            if self.spatial_key not in self.adata.uns:
-                self.adata.uns[self.spatial_key] = {}
-            self.adata.uns[self.spatial_key]["alignment_metadata"] = aligned_metadata
-        if not inplace:
-            return aligned_basis
-        self.adata.obsm[f"{self.spatial_key}_{mode}"] = aligned_basis  # noqa: RET503
 
-    @d_mixins.dedent
+        if key_added is None:
+            return aligned_basis, aligned_metadata
+
+        self.adata.obsm[key_added] = aligned_basis
+        if mode == "affine":  # noqa: RET503
+            self.adata.uns.setdefault(key_added, {})
+            self.adata.uns[key_added]["alignment_metadata"] = aligned_metadata  # noqa: RET503
+
     def cell_transition(  # type: ignore[misc]
         self: SpatialAlignmentMixinProtocol[K, B],
         source: K,
         target: K,
         source_groups: Optional[Str_Dict_t] = None,
         target_groups: Optional[Str_Dict_t] = None,
-        forward: bool = False,  # return value will be row-stochastic if forward=True, else column-stochastic
         aggregation_mode: Literal["annotation", "cell"] = "annotation",
+        forward: bool = False,
         batch_size: Optional[int] = None,
         normalize: bool = True,
         key_added: Optional[str] = _constants.CELL_TRANSITION,
     ) -> pd.DataFrame:
-        """
-        Compute a grouped cell transition matrix.
+        """Aggregate the transport matrix.
 
-        This function computes a transition matrix with entries corresponding to categories, e.g. cell types.
-        The transition matrix will be row-stochastic if `forward` is `True`, otherwise column-stochastic.
+        .. seealso::
+            - See :doc:`../notebooks/examples/plotting/200_cell_transitions` on how to
+              compute and plot the cell transitions.
 
         Parameters
         ----------
-        %(cell_trans_params)s
-        %(forward_cell_transition)s
-        %(aggregation_mode)s
-        %(ott_jax_batch_size)s
-        %(normalize)s
-        %(key_added_plotting)s
+        source
+            Key identifying the source distribution.
+        target
+            Key identifying the target distribution.
+        source_groups
+            Source groups used for aggregation. Valid options are:
+
+            - :class:`str` - key in :attr:`~anndata.AnnData.obs` where categorical data is stored.
+            - :class:`dict` - a dictionary with one key corresponding to a categorical column in
+              :attr:`~anndata.AnnData.obs` and values to a subset of categories.
+        target_groups
+            Target groups used for aggregation. Valid options are:
+
+            - :class:`str` - key in :attr:`~anndata.AnnData.obs` where categorical data is stored.
+            - :class:`dict` - a dictionary with one key corresponding to a categorical column in
+              :attr:`~anndata.AnnData.obs` and values to a subset of categories.
+        aggregation_mode
+            How to aggregate the cell-level transport maps. Valid options are:
+
+            - ``'annotation'`` - group the transitions by the ``source_groups`` and the ``target_groups``.
+            - ``'cell'`` - do not group by the ``source_groups`` or the ``target_groups``, depending on the ``forward``.
+        forward
+            If :obj:`True`, compute the transitions from the ``source_groups`` to the ``target_groups``.
+        batch_size
+            Number of rows/columns of the cost matrix to materialize during :meth:`push` or :meth:`pull`.
+            Larger value will require more memory.
+        normalize
+            If :obj:`True`, normalize the transition matrix. If ``forward = True``, the transition matrix
+            will be row-stochastic, otherwise column-stochastic.
+        key_added
+            Key in :attr:`~anndata.AnnData.uns` where to save the result.
 
         Returns
         -------
-        %(return_cell_transition)s
+        Depending on the ``key_added``:
 
-        Notes
-        -----
-        %(notes_cell_transition)s
+        - :obj:`None` - returns the transition matrix.
+        - :obj:`str` - returns nothing and saves the transition matrix to
+          :attr:`uns['moscot_results']['cell_transition']['{key_added}'] <anndata.AnnData.uns>`
         """
         if TYPE_CHECKING:
             assert isinstance(self.batch_key, str)
 
         return self._cell_transition(
             key=self.batch_key,
             source=source,
@@ -248,61 +271,41 @@
             batch_size=batch_size,
             normalize=normalize,
             key_added=key_added,
         )
 
     @property
     def spatial_key(self) -> Optional[str]:
-        """Spatial key in :attr:`anndata.AnnData.obsm`."""
+        """Spatial key in :attr:`~anndata.AnnData.obsm`."""
         return self._spatial_key
 
     @spatial_key.setter
     def spatial_key(self: SpatialAlignmentMixinProtocol[K, B], key: Optional[str]) -> None:  # type: ignore[misc]
         if key is not None and key not in self.adata.obsm:
             raise KeyError(f"Unable to find spatial data in `adata.obsm[{key!r}]`.")
         self._spatial_key = key
 
     @property
     def batch_key(self) -> Optional[str]:
-        """Batch key in :attr:`anndata.AnnData.obs`."""
+        """Batch key in :attr:`~anndata.AnnData.obs`."""
         return self._batch_key
 
     @batch_key.setter
     def batch_key(self, key: Optional[str]) -> None:
         if key is not None and key not in self.adata.obs:  # type: ignore[attr-defined]
             raise KeyError(f"Unable to find batch data in `adata.obs[{key!r}]`.")
         self._batch_key = key
 
     def _subset_spatial(  # type: ignore[misc]
-        self: SpatialAlignmentMixinProtocol[K, B], k: K, spatial_key: Optional[str] = None
+        self: SpatialAlignmentMixinProtocol[K, B],
+        k: K,
+        spatial_key: str,
     ) -> ArrayLike:
-        if spatial_key is None:
-            spatial_key = self.spatial_key
-        return self.adata[self.adata.obs[self._policy._subset_key] == k].obsm[spatial_key].astype(float, copy=True)
-
-    @staticmethod
-    def _affine(
-        tmap: LinearOperator,
-        src: ArrayLike,
-        tgt: ArrayLike,
-    ) -> Tuple[ArrayLike, ArrayLike]:
-        """Affine transformation."""
-        tgt -= tgt.mean(0)
-        out = tmap @ src
-        H = tgt.T.dot(out)
-        U, _, Vt = svd(H)
-        R = Vt.T.dot(U.T)
-        tgt = R.dot(tgt.T).T
-        return tgt, R
-
-    @staticmethod
-    def _warp(tmap: LinearOperator, src: ArrayLike, tgt: ArrayLike) -> Tuple[ArrayLike, None]:
-        """Warp transformation."""
-        del tgt
-        return tmap @ src, None
+        mask = self.adata.obs[self._policy.key] == k
+        return self.adata[mask].obsm[spatial_key].astype(float, copy=True)
 
 
 class SpatialMappingMixin(AnalysisMixin[K, B]):
     """Spatial mapping analysis mixin class."""
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
@@ -329,200 +332,222 @@
         if var_names.issubset(vars_sc) and var_names.issubset(vars_sp):  # type: ignore[attr-defined]
             return list(var_names)
 
         raise ValueError("Some variable are missing in the single-cell or the spatial `AnnData`.")
 
     def correlate(  # type: ignore[misc]
         self: SpatialMappingMixinProtocol[K, B],
-        var_names: Optional[List[str]] = None,
+        var_names: Optional[Sequence[str]] = None,
         corr_method: Literal["pearson", "spearman"] = "pearson",
     ) -> Mapping[Tuple[K, K], pd.Series]:
-        """
-        Calculate correlation between true and predicted gene expression.
+        """Correlate true and predicted gene expression.
+
+        .. warning::
+            Sparse matrices stored in :attr:`~anndata.AnnData.X` will be densified.
 
         Parameters
         ----------
         var_names
-            List of variable names.
+            Keys in :attr:`~anndata.AnnData.var_names`. If :obj:`None`, use all shared genes.
         corr_method
-            Correlation method:
+            Correlation method. Valid options are:
 
-                - 'pearson': Pearson correlation.
-                - 'spearman': Spearman correlation
+            - ``'pearson'`` - `Pearson correlation <https://en.wikipedia.org/wiki/Pearson_correlation_coefficient>`_.
+            - ``'spearman'`` - `Spearman's rank correlation
+              <https://en.wikipedia.org/wiki/Spearman%27s_rank_correlation_coefficient>`_.
 
         Returns
         -------
-        TODO
+        Correlation for each solution in :attr:`solutions`.
         """
         var_sc = self._filter_vars(var_names)
         if var_sc is None or not len(var_sc):
-            raise ValueError("No overlapping `var_names` between ` adata_sc` and `adata_sp`.")
+            raise ValueError("No overlapping `var_names` between spatial and gene expression data.")
 
         if corr_method == "pearson":
-            cor = pearsonr
+            corr = st.pearsonr
         elif corr_method == "spearman":
-            cor = spearmanr
+            corr = st.spearmanr
         else:
             raise NotImplementedError(f"Correlation method `{corr_method!r}` is not yet implemented.")
 
+        gexp_sc = self.adata_sc[:, var_sc].X
+        if sp.issparse(gexp_sc):
+            gexp_sc = gexp_sc.A
+
         corrs = {}
-        gexp_sc = self.adata_sc[:, var_sc].X if not sp.issparse(self.adata_sc.X) else self.adata_sc[:, var_sc].X.A
         for key, val in self.solutions.items():
             index_obs: List[Union[bool, int]] = (
-                self.adata_sp.obs[self._policy._subset_key] == key[0]
-                if self._policy._subset_key is not None
+                self.adata_sp.obs[self._policy.key] == key[0]
+                if self._policy.key is not None
                 else np.arange(self.adata_sp.shape[0])
             )
             gexp_sp = self.adata_sp[index_obs, var_sc].X
             if sp.issparse(gexp_sp):
-                # TODO(giovp): in the future, logg if too large
                 gexp_sp = gexp_sp.A
             gexp_pred_sp = val.pull(gexp_sc, scale_by_marginals=True)
-            corr_val = [cor(gexp_pred_sp[:, gi], gexp_sp[:, gi])[0] for gi, _ in enumerate(var_sc)]
+            corr_val = [corr(gexp_pred_sp[:, gi], gexp_sp[:, gi])[0] for gi, _ in enumerate(var_sc)]
             corrs[key] = pd.Series(corr_val, index=var_sc)
 
         return corrs
 
     def impute(  # type: ignore[misc]
         self: SpatialMappingMixinProtocol[K, B],
-        var_names: Optional[Sequence[Any]] = None,
+        var_names: Optional[Sequence[str]] = None,
         device: Optional[Device_t] = None,
     ) -> AnnData:
-        """Impute expression of specific genes.
+        """Impute the expression of specific genes.
 
         Parameters
         ----------
-        var_names:
-            TODO: don't use device from docstrings here, as different use
+        var_names
+            Genes in :attr:`~anndata.AnnData.var_names` to impute. If :obj:`None`, use all genes in :attr:`adata_sc`.
+        device
+            Device where to transfer the solutions, see :meth:`~moscot.base.output.BaseSolverOutput.to`.
 
         Returns
         -------
-        Annotated data object with imputed gene expression values.
+        Annotated data object with the imputed gene expression.
         """
         if var_names is None:
             var_names = self.adata_sc.var_names
-        gexp_sc = self.adata_sc[:, var_names].X if not sp.issparse(self.adata_sc.X) else self.adata_sc[:, var_names].X.A
-        pred_list = [
-            val.to(device=device).pull(gexp_sc, scale_by_marginals=True)
-            if device is not None
-            else val.pull(gexp_sc, scale_by_marginals=True)
-            for val in self.solutions.values()
-        ]
-        gexp_pred = np.nan_to_num(np.vstack(pred_list), nan=0.0, copy=False)
-        adata_pred = AnnData(gexp_pred, dtype=np.float_)
+
+        gexp_sc = self.adata_sc[:, var_names].X
+        if sp.issparse(gexp_sc):
+            gexp_sc = gexp_sc.A
+
+        predictions = [val.to(device=device).pull(gexp_sc, scale_by_marginals=True) for val in self.solutions.values()]
+
+        adata_pred = AnnData(np.nan_to_num(np.vstack(predictions), nan=0.0, copy=False))
         adata_pred.obs_names = self.adata_sp.obs_names
         adata_pred.var_names = var_names
         adata_pred.obsm = self.adata_sp.obsm.copy()
+
         return adata_pred
 
-    @d.dedent
     def spatial_correspondence(  # type: ignore[misc]
         self: SpatialMappingMixinProtocol[K, B],
-        interval: Union[ArrayLike, int] = 10,
+        interval: Union[int, ArrayLike] = 10,
         max_dist: Optional[int] = None,
-        attr: Optional[Dict[str, Any]] = None,
+        attr: Optional[Dict[str, Optional[str]]] = None,
     ) -> pd.DataFrame:
-        """
-        Compute structural correspondence between spatial and molecular distances.
+        """Compute structural correspondence between spatial and molecular distances.
 
         Parameters
         ----------
         interval
-            Interval for the spatial distance.
+            Interval for the spatial distance. If :class:`int`, it will be set from the data.
         max_dist
-            Maximum distance for the interval, if `None` it is set from data.
+            Maximum distance for the interval. If :obj:`None`, it will set from the data.
         attr
-            Specify the attributes from which to compute the correspondence.
+            How to extract the data for correspondence. Valid options are:
+
+            - :obj:`None` - use :attr:`~anndata.AnnData.X`.
+            - :class:`dict` - key corresponds to an attribute of :class:`~anndata.AnnData` and
+              value to a key in that attribute. If the value is :obj:`None`, only the attribute will be used.
 
         Returns
         -------
-        :class:`pandas.DataFrame` with columns:
+        A dataframe with the following columns:
 
-            - `spatial`: average spatial distance.
-            - `expression`: average expression distance.
-            - `index`: index of the interval.
-            - `batch_key`: key of the batch (slide).
+        - ``'features_distance'`` - average spatial distance.
+        - ``'index_interval'`` - index of the interval.
+        - ``'value_interval'`` - average expression distance.
+        - ``'{batch_key}'`` key of the batch (slide).
         """
 
         def _get_features(
             adata: AnnData,
             attr: Optional[Dict[str, Any]] = None,
         ) -> ArrayLike:
             attr = {"attr": "X"} if attr is None else attr
             att = attr.get("attr", None)
             key = attr.get("key", None)
 
             if key is not None:
                 return getattr(adata, att)[key]
             return getattr(adata, att)
 
-        if self.batch_key is not None:
-            out_list = []
-            if is_categorical_dtype(self.adata.obs[self.batch_key]):
-                categ = self.adata.obs[self.batch_key].cat.categories
-            else:
-                logger.info(f"adata_sp.obs[`{self.batch_key}`] is not `categorical`, using `unique()` method.")
-                categ = self.adata.obs[self.batch_key].unique()
-            if len(categ) > 1:
-                for c in categ:
-                    adata_subset = self.adata[self.adata.obs[self.batch_key] == c]
-                    spatial = adata_subset.obsm[self.spatial_key]
-                    features = _get_features(adata_subset, attr)
-                    out = _compute_correspondence(spatial, features, interval, max_dist)
-                    out[self.batch_key] = c
-                    out_list.append(out)
-            else:
-                spatial = self.adata.obsm[self.spatial_key]
-                features = _get_features(self.adata, attr)
-                out = _compute_correspondence(spatial, features, interval, max_dist)
-                out[self.batch_key] = categ[0]
-                out_list.append(out)
-            out = pd.concat(out_list, axis=0)
-            out[self.batch_key] = pd.Categorical(out[self.batch_key])
-            return out
-
-        spatial = self.adata.obsm[self.spatial_key]
-        features = _get_features(self.adata, attr)
-        return _compute_correspondence(spatial, features, interval, max_dist)
+        if self.batch_key is None:
+            spatial = self.adata.obsm[self.spatial_key]
+            features = _get_features(self.adata, attr)
+            return _compute_correspondence(spatial, features, interval, max_dist)
+
+        res = []
+        for c in self.adata.obs[self.batch_key].cat.categories:
+            adata_subset = self.adata[self.adata.obs[self.batch_key] == c]
+            spatial = adata_subset.obsm[self.spatial_key]
+            features = _get_features(adata_subset, attr)
+            out = _compute_correspondence(spatial, features, interval, max_dist)
+            out[self.batch_key] = c
+            res.append(out)
+
+        res = pd.concat(res, axis=0)
+        res[self.batch_key] = res[self.batch_key].astype("category")  # type: ignore[call-overload]
+        return res
 
-    @d_mixins.dedent
     def cell_transition(  # type: ignore[misc]
         self: SpatialMappingMixinProtocol[K, B],
         source: K,
         target: Optional[K] = None,
         source_groups: Optional[Str_Dict_t] = None,
         target_groups: Optional[Str_Dict_t] = None,
-        forward: bool = False,  # return value will be row-stochastic if forward=True, else column-stochastic
         aggregation_mode: Literal["annotation", "cell"] = "annotation",
+        forward: bool = False,
         batch_size: Optional[int] = None,
         normalize: bool = True,
         key_added: Optional[str] = _constants.CELL_TRANSITION,
     ) -> pd.DataFrame:
-        """
-        Compute a grouped cell transition matrix.
+        """Aggregate the transport matrix.
 
-        This function computes a transition matrix with entries corresponding to categories, e.g. cell types.
-        The transition matrix will be row-stochastic if `forward` is `True`, otherwise column-stochastic.
+        .. seealso::
+            - See :doc:`../notebooks/examples/plotting/200_cell_transitions`
+              on how to compute and plot the cell transitions.
 
         Parameters
         ----------
-        %(cell_trans_params)s
-        %(forward_cell_transition)s
-        %(aggregation_mode)s
-        %(ott_jax_batch_size)s
-        %(normalize)s
-        %(key_added_plotting)s
+        source
+            Key identifying the source distribution.
+        target
+            Key identifying the target distribution.
+        source_groups
+            Source groups used for aggregation. Valid options are:
+
+            - :class:`str` - key in :attr:`~anndata.AnnData.obs` where categorical data is stored.
+            - :class:`dict` - a dictionary with one key corresponding to a categorical column in
+              :attr:`~anndata.AnnData.obs` and values to a subset of categories.
+        target_groups
+            Target groups used for aggregation. Valid options are:
+
+            - :class:`str` - key in :attr:`~anndata.AnnData.obs` where categorical data is stored.
+            - :class:`dict` - a dictionary with one key corresponding to a categorical column in
+              :attr:`~anndata.AnnData.obs` and values to a subset of categories.
+        aggregation_mode
+            How to aggregate the cell-level transport maps. Valid options are:
+
+            - ``'annotation'`` - group the transitions by the ``source_groups`` and the ``target_groups``.
+            - ``'cell'`` - do not group by the ``source_groups`` or the ``target_groups``, depending on the ``forward``.
+        forward
+            If :obj:`True`, compute the transitions from the ``source_groups`` to the ``target_groups``.
+        batch_size
+            Number of rows/columns of the cost matrix to materialize during :meth:`push` or :meth:`pull`.
+            Larger value will require more memory.
+        normalize
+            If :obj:`True`, normalize the transition matrix. If ``forward = True``, the transition matrix
+            will be row-stochastic, otherwise column-stochastic.
+        key_added
+            Key in :attr:`~anndata.AnnData.uns` where to save the result.
 
         Returns
         -------
-        %(return_cell_transition)s
+        Depending on the ``key_added``:
 
-        Notes
-        -----
-        %(notes_cell_transition)s
+        - :obj:`None` - returns the transition matrix.
+        - :obj:`str` - returns nothing and saves the transition matrix to
+          :attr:`uns['moscot_results']['cell_transition']['{key_added}'] <anndata.AnnData.uns>`
         """
         if TYPE_CHECKING:
             assert self.batch_key is not None
         return self._cell_transition(
             key=self.batch_key,
             source=source,
             target=target,
@@ -535,63 +560,62 @@
             batch_size=batch_size,
             normalize=normalize,
             key_added=key_added,
         )
 
     @property
     def batch_key(self) -> Optional[str]:
-        """Batch key in :attr:`anndata.AnnData.obs`."""
+        """Batch key in :attr:`~anndata.AnnData.obs`."""
         return self._batch_key
 
     @batch_key.setter
     def batch_key(self, key: Optional[str]) -> None:
         if key is not None and key not in self.adata.obs:  # type: ignore[attr-defined]
             raise KeyError(f"Unable to find batch data in `adata.obs[{key!r}]`.")
         self._batch_key = key
 
     @property
     def spatial_key(self) -> Optional[str]:
-        """Spatial key in :attr:`anndata.AnnData.obsm`."""
+        """Spatial key in :attr:`~anndata.AnnData.obsm`."""
         return self._spatial_key
 
     @spatial_key.setter
     def spatial_key(self: SpatialAlignmentMixinProtocol[K, B], key: Optional[str]) -> None:  # type: ignore[misc]
         if key is not None and key not in self.adata.obsm:
             raise KeyError(f"Unable to find spatial data in `adata.obsm[{key!r}]`.")
         self._spatial_key = key
 
 
 def _compute_correspondence(
     spatial: ArrayLike,
     features: ArrayLike,
-    interval: Union[ArrayLike, int] = 10,
+    interval: Union[int, ArrayLike] = 10,
     max_dist: Optional[int] = None,
 ) -> pd.DataFrame:
     if isinstance(interval, int):
         # prepare support
         hull = ConvexHull(spatial)
         area = hull.volume
         if max_dist is None:
             max_dist = round(((area / 2) ** 0.5) / 2)
         support = np.linspace(max_dist / interval, max_dist, interval)
     else:
-        support = np.array(sorted(interval), dtype=np.float_, copy=True)
+        support = np.asarray(np.sort(interval), dtype=float)
 
     def pdist(row_idx: ArrayLike, col_idx: float, feat: ArrayLike) -> Any:
         if len(row_idx) > 0:
             return pairwise_distances(feat[row_idx, :], feat[[col_idx], :]).mean()  # type: ignore[index]
         return np.nan
 
+    # TODO(michalk8): vectorize using jax, this is just a for loop
     vpdist = np.vectorize(pdist, excluded=["feat"])
-    features = features.A if sp.issparse(features) else features  # type: ignore[attr-defined]
-
-    feat_arr = []
-    index_arr = []
-    support_arr = []
+    if sp.issparse(features):
+        features = features.A  # type: ignore[attr-defined]
 
+    feat_arr, index_arr, support_arr = [], [], []
     for ind, i in enumerate(support):
         tree = NearestNeighbors(radius=i).fit(spatial)
         _, idx = tree.radius_neighbors()
 
         feat_dist = vpdist(row_idx=idx, col_idx=np.arange(len(idx)), feat=features)
         feat_dist = feat_dist[~np.isnan(feat_dist)]
 
@@ -604,9 +628,28 @@
     support_arr = np.concatenate(support_arr)
 
     df = pd.DataFrame(
         np.vstack([feat_arr, index_arr, support_arr]).T,
         columns=["features_distance", "index_interval", "value_interval"],
     )
 
-    df["index_interval"] = pd.Categorical(df["index_interval"].astype(np.int_))
+    df["index_interval"] = df["index_interval"].astype(int).astype("category")
     return df
+
+
+def _affine(
+    tmap: sp.linalg.LinearOperator,
+    src: ArrayLike,
+    tgt: ArrayLike,
+) -> Tuple[ArrayLike, ArrayLike]:
+    tgt -= tgt.mean(0)
+    out = tmap @ src
+    H = tgt.T.dot(out)
+    U, _, Vt = svd(H)
+    R = Vt.T.dot(U.T)
+    tgt = R.dot(tgt.T).T
+    return tgt, R
+
+
+def _warp(tmap: sp.linalg.LinearOperator, src: ArrayLike, tgt: ArrayLike) -> Tuple[ArrayLike, None]:
+    del tgt
+    return tmap @ src, None
```

### Comparing `moscot-0.3.0/src/moscot/problems/time/_mixins.py` & `moscot-0.3.1/src/moscot/problems/time/_mixins.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,42 @@
 import itertools
-from pathlib import Path
+import pathlib
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     Iterable,
     Iterator,
     List,
     Literal,
     Optional,
     Protocol,
+    Sequence,
     Tuple,
     Union,
 )
 
 import numpy as np
 import pandas as pd
-from pandas.api.types import infer_dtype, is_numeric_dtype
+from pandas.api.types import infer_dtype, is_categorical_dtype, is_numeric_dtype
 
 from anndata import AnnData
 
 from moscot import _constants
-from moscot._docs._docs_mixins import d_mixins
-from moscot._types import ArrayLike, Numeric_t, Str_Dict_t
+from moscot._types import ArrayLike, Str_Dict_t
 from moscot.base.problems._mixins import AnalysisMixin, AnalysisMixinProtocol
 from moscot.base.problems.birth_death import BirthDeathProblem
 from moscot.base.problems.compound_problem import ApplyOutput_t, B, K
 from moscot.plotting._utils import set_plotting_vars
 from moscot.utils.tagged_array import Tag
 
 __all__ = ["TemporalMixin"]
 
 
-# TODO(@MUCDK, @michalk8): check for ignore[misc] in line below, might become redundant
-class TemporalMixinProtocol(AnalysisMixinProtocol[K, B], Protocol[K, B]):  # type:ignore
-    """Protocol class."""
-
+class TemporalMixinProtocol(AnalysisMixinProtocol[K, B], Protocol[K, B]):  # type: ignore[misc]
     adata: AnnData
     problems: Dict[Tuple[K, K], BirthDeathProblem]
     temporal_key: Optional[str]
     _temporal_key: Optional[str]
 
     def cell_transition(  # noqa: D102
         self: "TemporalMixinProtocol[K, B]",
@@ -51,19 +48,18 @@
         aggregation_mode: Literal["annotation", "cell"] = "annotation",
         batch_size: Optional[int] = None,
         normalize: bool = True,
         key_added: Optional[str] = _constants.CELL_TRANSITION,
     ) -> pd.DataFrame:
         ...
 
-    def push(self, *args: Any, **kwargs: Any) -> Optional[ApplyOutput_t[K]]:  # noqa: D102
+    def push(self, *args: Any, **kwargs: Any) -> Optional[ApplyOutput_t[K]]:
         ...
 
     def pull(self, *args: Any, **kwargs: Any) -> Optional[ApplyOutput_t[K]]:
-        """Pull."""
         ...
 
     def _cell_transition(
         self: AnalysisMixinProtocol[K, B],
         *args: Any,
         **kwargs: Any,
     ) -> pd.DataFrame:
@@ -74,28 +70,28 @@
         source: K,
         target: K,
         n_samples: int,
         source_dim: int,
         target_dim: int,
         batch_size: int = 256,
         account_for_unbalancedness: bool = False,
-        interpolation_parameter: Optional[Numeric_t] = None,
+        interpolation_parameter: Optional[float] = None,
         seed: Optional[int] = None,
     ) -> Tuple[List[Any], List[ArrayLike]]:
         ...
 
     def _compute_wasserstein_distance(
         self: "TemporalMixinProtocol[K, B]",
         point_cloud_1: ArrayLike,
         point_cloud_2: ArrayLike,
         a: Optional[ArrayLike] = None,
         b: Optional[ArrayLike] = None,
         backend: Literal["ott"] = "ott",
         **kwargs: Any,
-    ) -> Numeric_t:
+    ) -> float:
         ...
 
     def _interpolate_gex_with_ot(
         self: "TemporalMixinProtocol[K, B]",
         number_cells: int,
         source_data: ArrayLike,
         target_data: ArrayLike,
@@ -135,71 +131,95 @@
         data: Dict[K, ArrayLike],
         source: K,
         target: K,
         time_points: Optional[Iterable[K]] = None,
         basis: str = "umap",
         result_key: Optional[str] = None,
         fill_value: float = 0.0,
-        save: Optional[Union[str, Path]] = None,
+        save: Optional[Union[str, pathlib.Path]] = None,
         **kwargs: Any,
     ) -> None:
         ...
 
     @staticmethod
     def _get_interp_param(
         source: K, intermediate: K, target: K, interpolation_parameter: Optional[float] = None
-    ) -> Numeric_t:
+    ) -> float:
         ...
 
     def __iter__(self) -> Iterator[Tuple[K, K]]:
         ...
 
 
 class TemporalMixin(AnalysisMixin[K, B]):
     """Analysis Mixin for all problems involving a temporal dimension."""
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
         self._temporal_key: Optional[str] = None
 
-    @d_mixins.dedent
     def cell_transition(
         self: TemporalMixinProtocol[K, B],
         source: K,
         target: K,
         source_groups: Str_Dict_t,
         target_groups: Str_Dict_t,
-        forward: bool = False,  # return value will be row-stochastic if forward=True, else column-stochastic
+        forward: bool = False,
         aggregation_mode: Literal["annotation", "cell"] = "annotation",
         batch_size: Optional[int] = None,
         normalize: bool = True,
         key_added: Optional[str] = _constants.CELL_TRANSITION,
     ) -> Optional[pd.DataFrame]:
-        """
-        Compute a grouped cell transition matrix.
+        """Aggregate the transport matrix.
 
-        This function computes a transition matrix with entries corresponding to categories, e.g. cell types.
-        The transition matrix will be row-stochastic if `forward` is `True`, otherwise column-stochastic.
+        .. seealso::
+            - See :doc:`../notebooks/examples/plotting/200_cell_transitions` on how to
+              compute and :func:`plot <moscot.plotting.cell_transition>` the cell transitions.
 
         Parameters
         ----------
-        %(cell_trans_params)s
-        %(forward_cell_transition)s
-        %(aggregation_mode)s
-        %(ott_jax_batch_size)s
-        %(normalize)s
-        %(key_added_plotting)s
+        source
+            Key identifying the source distribution.
+        target
+            Key identifying the target distribution.
+        source_groups
+            Source groups used for aggregation. Valid options are:
+
+            - :class:`str` - key in :attr:`~anndata.AnnData.obs` where categorical data is stored.
+            - :class:`dict` - a dictionary with one key corresponding to a categorical column in
+              :attr:`~anndata.AnnData.obs` and values to a subset of categories.
+        target_groups
+            Target groups used for aggregation. Valid options are:
+
+            - :class:`str` - key in :attr:`~anndata.AnnData.obs` where categorical data is stored.
+            - :class:`dict` - a dictionary with one key corresponding to a categorical column in
+              :attr:`~anndata.AnnData.obs` and values to a subset of categories.
+        aggregation_mode
+            How to aggregate the cell-level transport maps. Valid options are:
+
+            - ``'annotation'`` - group the transitions by the ``source_groups`` and the ``target_groups``.
+            - ``'cell'`` - do not group by the ``source_groups`` or the ``target_groups``, depending on the ``forward``.
+        forward
+            If :obj:`True`, compute the transitions from the ``source_groups`` to the ``target_groups``.
+        batch_size
+            Number of rows/columns of the cost matrix to materialize during :meth:`push` or :meth:`pull`.
+            Larger value will require more memory.
+        normalize
+            If :obj:`True`, normalize the transition matrix. If ``forward = True``, the transition matrix
+            will be row-stochastic, otherwise column-stochastic.
+        key_added
+            Key in :attr:`~anndata.AnnData.uns` where to save the result.
 
         Returns
         -------
-        %(return_cell_transition)s
+        Depending on the ``key_added``:
 
-        Notes
-        -----
-        %(notes_cell_transition)s
+        - :obj:`None` - returns the transition matrix.
+        - :obj:`str` - returns nothing and saves the transition matrix to
+          :attr:`uns['moscot_results']['cell_transition']['{key_added}'] <anndata.AnnData.uns>`
         """
         if TYPE_CHECKING:
             assert isinstance(self.temporal_key, str)
         return self._cell_transition(
             key=self.temporal_key,
             source=source,
             target=target,
@@ -208,62 +228,89 @@
             forward=forward,
             aggregation_mode=aggregation_mode,
             size=batch_size,
             normalize=normalize,
             key_added=key_added,
         )
 
-    @d_mixins.dedent
     def sankey(
         self: "TemporalMixinProtocol[K, B]",
         source: K,
         target: K,
         source_groups: Str_Dict_t,
         target_groups: Str_Dict_t,
         threshold: Optional[float] = None,
         normalize: bool = False,
         forward: bool = True,
         restrict_to_existing: bool = True,
-        order_annotations: Optional[List[Any]] = None,
+        order_annotations: Optional[Sequence[str]] = None,
         key_added: Optional[str] = _constants.SANKEY,
-        return_data: bool = False,
+        **kwargs: Any,
     ) -> Optional[List[pd.DataFrame]]:
-        """
-        Draw a Sankey diagram visualising transitions of cells across time points.
+        """Compute a `Sankey diagram <https://en.wikipedia.org/wiki/Sankey_diagram>`_ between cells across time points.
+
+        .. seealso::
+            - See :doc:`../notebooks/examples/plotting/300_sankey` on how to
+              compute and :func:`plot <moscot.plotting.sankey>` the Sankey diagram.
 
         Parameters
         ----------
-        %(cell_trans_params)s
-        %(threshold)s
-        %(normalize)s
-        %(forward)s
-        %(restrict_to_existing)s
-        %(order_annotations)s
-        %(key_added_plotting)s
-        %(return_data)s
+        source
+            Key identifying the source distribution.
+        target
+            Key identifying the target distribution.
+        source_groups
+            Source groups used for aggregation. Valid options are:
+
+            - :class:`str` - key in :attr:`~anndata.AnnData.obs` where categorical data is stored.
+            - :class:`dict` - a dictionary with one key corresponding to a categorical column in
+              :attr:`~anndata.AnnData.obs` and values to a subset of categories.
+        target_groups
+            Target groups used for aggregation. Valid options are:
+
+            - :class:`str` - key in :attr:`~anndata.AnnData.obs` where categorical data is stored.
+            - :class:`dict` - a dictionary with one key corresponding to a categorical column in
+              :attr:`~anndata.AnnData.obs` and values to a subset of categories.
+        threshold
+            Set cell transitions lower than ``threshold`` to :math:`0`.
+        normalize
+            If :obj:`True`, normalize the transition matrix. If ``forward = True``, the transition matrix
+            will be row-stochastic, otherwise column-stochastic.
+        forward
+            If :obj:`True`, compute the transitions from the ``source_groups`` to the ``target_groups``.
+        restrict_to_existing
+            TODO(MUCDK)
+        order_annotations
+            Order of annotations from top to bottom. If :obj:`None`, use the order defined by the categories.
+        key_added
+            Key in :attr:`~anndata.AnnData.uns` where to save the result.
+        kwargs
+            Keyword arguments for :meth:`cell_transition`.
 
         Returns
         -------
-        Transition matrices of cells or groups of cells, as needed for a sankey.
+        Depending on the ``key_added``:
 
-        Notes
-        -----
-        To visualise the results, see :func:`moscot.plotting.sankey`.
+        - :obj:`None` - returns the cell transitions.
+        - :obj:`str` - returns nothing and saves the data for the diagram to
+          :attr:`uns['moscot_results']['sankey']['{key_added}'] <anndata.AnnData.uns>`
         """
         tuples = self._policy.plan(start=source, end=target)
         cell_transitions = []
         for src, tgt in tuples:
             cell_transitions.append(
                 self.cell_transition(
                     src,
                     tgt,
                     source_groups=source_groups,
                     target_groups=target_groups,
                     forward=forward,
                     normalize=normalize,
+                    key_added=None,
+                    **kwargs,
                 )
             )
 
         if len(cell_transitions) > 1 and restrict_to_existing:
             for i in range(len(cell_transitions[:-1])):
                 present_annotations = list(
                     set(cell_transitions[i + 1].index).intersection(set(cell_transitions[i].columns))
@@ -273,76 +320,83 @@
         if order_annotations is not None:
             cell_transitions_updated = []
             for ct in cell_transitions:
                 order_annotations_present_index = [ann for ann in order_annotations if ann in ct.index]
                 ct = ct.loc[order_annotations_present_index[::-1]]
                 order_annotations_present_columns = [ann for ann in order_annotations if ann in ct.columns]
                 ct = ct[order_annotations_present_columns[::-1]]
-            cell_transitions_updated.append(ct)
+                cell_transitions_updated.append(ct)
         else:
             cell_transitions_updated = cell_transitions
 
         if threshold is not None:
-            if threshold < 0:
-                raise ValueError(f"Expected threshold to be non-negative, found `{threshold}`.")
             for ct in cell_transitions:
                 ct[ct < threshold] = 0.0
 
+        if key_added is None:
+            return cell_transitions_updated
+
         if isinstance(source_groups, str):
             key = source_groups
         # TODO(MUCDK): should this be really `target_groups`?
         elif isinstance(target_groups, dict):
             key = list(target_groups.keys())[0]
         else:
             raise TypeError(f"Expected early cells to be either `str` or `dict`, found `{type(source_groups)}`.")
 
-        if key_added is not None:
-            plot_vars = {
-                "transition_matrices": cell_transitions_updated,
-                "key": key,
-                "source": source,
-                "target": target,
-                "source_groups": source_groups,
-                "target_groups": target_groups,
-                "captions": [str(t) for t in tuples],
-            }
-            set_plotting_vars(self.adata, _constants.SANKEY, key=key_added, value=plot_vars)
-        return cell_transitions_updated if return_data else None
+        plot_vars = {
+            "transition_matrices": cell_transitions_updated,
+            "key": key,
+            "source": source,
+            "target": target,
+            "source_groups": source_groups,
+            "target_groups": target_groups,
+            "captions": [str(t) for t in tuples],
+        }
+        set_plotting_vars(self.adata, _constants.SANKEY, key=key_added, value=plot_vars)  # noqa: RET503
 
-    @d_mixins.dedent
     def push(
         self: TemporalMixinProtocol[K, B],
         source: K,
         target: K,
         data: Optional[Union[str, ArrayLike]] = None,
         subset: Optional[Union[str, List[str], Tuple[int, int]]] = None,
         scale_by_marginals: bool = True,
         key_added: Optional[str] = _constants.PUSH,
         return_all: bool = False,
-        return_data: bool = False,
         **kwargs: Any,
     ) -> Optional[ApplyOutput_t[K]]:
-        """
-        Push distribution of cells through time.
+        """Push mass from source to target.
 
         Parameters
         ----------
-        %(source)s
-        %(target)s
-        %(data)s
-        %(subset)s
-        %(scale_by_marginals)s
-        %(key_added_plotting)s
-        %(return_all)s
-        %(return_data)s
-
-        Return
-        ------
-        %(return_push_pull)s
+        source
+            Source key in :attr:`solutions`.
+        target
+            Target key in :attr:`solutions`.
+        data
+            Initial data to push, see :meth:`~moscot.base.problems.OTProblem.push` for information.
+        subset
+            Push values contained only within the subset.
+        scale_by_marginals
+            Whether to scale by the source :term:`marginals`.
+        key_added
+            Key in :attr:`~anndata.AnnData.obs` where to add the result.
+        return_all
+            Whether to also return intermediate results. Always true if ``key_added != None``.
+        kwargs
+            Keyword arguments for the subproblems' :meth:`~moscot.base.problems.OTProblem.push` method.
 
+        Returns
+        -------
+        Depending on the ``key_added``:
+
+        - :obj:`None` - returns the result.
+        - :class:`str` - returns nothing and updates :attr:`obs['{key_added}'] <anndata.AnnData.obs>`
+          with the result.
         """
         result = self._apply(
             source=source,
             target=target,
             data=data,
             subset=subset,
             forward=True,
@@ -360,47 +414,56 @@
                 "target": target,
                 "temporal_key": self.temporal_key,
                 "data": data if isinstance(data, str) else None,
                 "subset": subset,
             }
             self.adata.obs[key_added] = self._flatten(result, key=self.temporal_key)
             set_plotting_vars(self.adata, _constants.PUSH, key=key_added, value=plot_vars)
-        return result if return_data else None
+            return None
+        return result
 
-    @d_mixins.dedent
     def pull(
         self: TemporalMixinProtocol[K, B],
         source: K,
         target: K,
         data: Optional[Union[str, ArrayLike]] = None,
         subset: Optional[Union[str, List[str], Tuple[int, int]]] = None,
         scale_by_marginals: bool = True,
         key_added: Optional[str] = _constants.PULL,
         return_all: bool = False,
-        return_data: bool = False,
         **kwargs: Any,
     ) -> Optional[ApplyOutput_t[K]]:
-        """
-        Pull distribution of cells through time.
+        """Pull mass from target to source.
 
         Parameters
         ----------
-        %(source)s
-        %(target)s
-        %(data)s
-        %(subset)s
-        %(scale_by_marginals)s
-        %(key_added_plotting)s
-        %(return_all)s
-        %(return_data)s
-
-        Return
-        ------
-        %(return_push_pull)s
+        source
+            Source key in :attr:`solutions`.
+        target
+            Target key in :attr:`solutions`.
+        data
+            Initial data to pull, see :meth:`~moscot.base.problems.OTProblem.pull` for information.
+        subset
+            Pull values contained only within the subset.
+        scale_by_marginals
+            Whether to scale by the source :term:`marginals`.
+        key_added
+            Key in :attr:`~anndata.AnnData.obs` where to add the result.
+        return_all
+            Whether to also return intermediate results. Always true if ``key_added != None``.
+        kwargs
+            Keyword arguments for the subproblems' :meth:`~moscot.base.problems.OTProblem.pull` method.
 
+        Returns
+        -------
+        Depending on the ``key_added``:
+
+        - :obj:`None` - returns the result.
+        - :class:`str` - returns nothing and updates :attr:`obs['{key_added}'] <anndata.AnnData.obs>`
+          with the result.
         """
         result = self._apply(
             source=source,
             target=target,
             data=data,
             subset=subset,
             forward=False,
@@ -417,19 +480,20 @@
                 "data": data if isinstance(data, str) else None,
                 "subset": subset,
                 "source": source,
                 "target": target,
             }
             self.adata.obs[key_added] = self._flatten(result, key=self.temporal_key)
             set_plotting_vars(self.adata, _constants.PULL, key=key_added, value=plot_vars)
-        return result if return_data else None
+            return None
+        return result
 
     @property
     def prior_growth_rates(self: TemporalMixinProtocol[K, B]) -> Optional[pd.DataFrame]:
-        """Return the prior estimate of growth rates of the cells in the source distribution."""
+        """Prior estimate of the source growth rates."""
         computed = [isinstance(p.prior_growth_rates, np.ndarray) for p in self.problems.values()]
         if not np.sum(computed):
             return None
 
         cols = ["prior_growth_rates"]
         df_list = [
             pd.DataFrame(problem.prior_growth_rates, index=problem.adata.obs_names, columns=cols)
@@ -439,15 +503,15 @@
         indices_remaining = set(self.adata.obs_names) - set(df_1.index)
         df_2 = pd.DataFrame(np.nan, index=list(indices_remaining), columns=cols)
 
         return pd.concat([df_1, df_2], verify_integrity=True)
 
     @property
     def posterior_growth_rates(self: TemporalMixinProtocol[K, B]) -> Optional[pd.DataFrame]:
-        """Return the posterior estimate of growth rates of the cells in the source distribution."""
+        """Posterior estimate of the source growth rates."""
         computed = [isinstance(p.posterior_growth_rates, np.ndarray) for p in self.problems.values()]
         if not np.sum(computed):
             return None
 
         cols = ["posterior_growth_rates"]
         df_list = [
             pd.DataFrame(problem.posterior_growth_rates, index=problem.adata.obs_names, columns=cols)
@@ -457,20 +521,24 @@
         indices_remaining = set(self.adata.obs_names) - set(df_1.index)
         df_2 = pd.DataFrame(np.nan, index=list(indices_remaining), columns=cols)
 
         return pd.concat([df_1, df_2], verify_integrity=True)
 
     @property
     def cell_costs_source(self: TemporalMixinProtocol[K, B]) -> Optional[pd.DataFrame]:
-        """Return the cost of a cell obtained by the potentials of the optimal transport solution."""
+        """Cell cost obtained by the :term:`first dual potential <dual potentials>`.
+
+        Only available for subproblems with :attr:`problem_kind = 'linear' <problem_kind>`.
+        """
         computed = [isinstance(s.potentials, tuple) for s in self.solutions.values()]
         if not np.sum(computed):
             return None
 
         cols = ["cell_cost_source"]
+        # TODO(michalk8): `[1]` will fail if potentials is None
         df_list = [
             pd.DataFrame(
                 np.asarray(problem.solution.potentials[0]),  # type: ignore[union-attr,index]
                 index=problem.adata_src.obs_names,
                 columns=cols,
             )
             for problem in self.problems.values()
@@ -478,34 +546,37 @@
         df_1 = pd.concat(df_list, verify_integrity=True)
         indices_remaining = set(self.adata.obs_names) - set(df_1.index)
         df_2 = pd.DataFrame(np.nan, index=list(indices_remaining), columns=cols)
         return pd.concat([df_1, df_2], verify_integrity=True)
 
     @property
     def cell_costs_target(self: TemporalMixinProtocol[K, B]) -> Optional[pd.DataFrame]:
-        """Return the cost of a cell obtained by the potentials of the optimal transport solution."""
+        """Cell cost obtained by the :term:`second dual potential <dual potentials>`.
+
+        Only available for subproblems with :attr:`problem_kind = 'linear' <problem_kind>`.
+        """
         computed = [isinstance(s.potentials, tuple) for s in self.solutions.values()]
         if not np.sum(computed):
             return None
 
         cols = ["cell_cost_target"]
+        # TODO(michalk8): `[1]` will fail if potentials is None
         df_list = [
             pd.DataFrame(
                 np.array(problem.solution.potentials[1]),  # type: ignore[union-attr,index]
                 index=problem.adata_tgt.obs_names,
                 columns=cols,
             )
             for problem in self.problems.values()
         ]
         df_1 = pd.concat(df_list, verify_integrity=True)
         indices_remaining = set(self.adata.obs_names) - set(df_1.index)
         df_2 = pd.DataFrame(np.nan, index=list(indices_remaining), columns=cols)
         return pd.concat([df_1, df_2], verify_integrity=True)
 
-    # TODO(michalk8): refactor me
     def _get_data(
         self: TemporalMixinProtocol[K, B],
         source: K,
         intermediate: Optional[K] = None,
         target: Optional[K] = None,
         posterior_marginals: bool = True,
         *,
@@ -547,62 +618,74 @@
             source_data,
             growth_rates_source,
             intermediate_data,
             intermediate_adata,
             target_data,
         )
 
-    @d_mixins.dedent
     def compute_interpolated_distance(
         self: TemporalMixinProtocol[K, B],
         source: K,
         intermediate: K,
         target: K,
         interpolation_parameter: Optional[float] = None,
         n_interpolated_cells: Optional[int] = None,
         account_for_unbalancedness: bool = False,
         batch_size: int = 256,
         posterior_marginals: bool = True,
         seed: Optional[int] = None,
         backend: Literal["ott"] = "ott",
         **kwargs: Any,
-    ) -> Numeric_t:
-        """
-        Compute the Wasserstein distance between the OT-interpolated distribution and the true cell distribution.
-
-        This is a validation method which interpolates the cell distributions corresponding to `start` and `end`
-        leveraging the OT coupling to obtain an approximation of the cell distribution at time point `intermediate`.
-        Therefore, the Wasserstein distance between the interpolated and the real distribution is computed.
+    ) -> float:
+        """Compute `Wasserstein distance <https://en.wikipedia.org/wiki/Wasserstein_metric>`_ between
+        :term:`OT`-interpolated and intermediate cells.
 
-        It is recommended to compare the Wasserstein distance to the ones obtained by
-        :meth:`compute_time_point_distances` and :meth:`compute_random_distance`.
-
-        This method does not instantiate the transport matrix if the solver output does not.
-
-        TODO: link to notebook
+        .. seealso::
+            - TODO(MUCDK): create an example showing the usage.
 
+        This is a validation method which interpolates cells between the ``source`` and ``target`` distributions
+        leveraging the :term:`OT` coupling to approximate cells at the ``intermediate`` time point.
 
         Parameters
         ----------
-        %(start)s
-        %(intermediate_interpolation)s
-        %(end)s
-        %(interpolation_parameter)s
-        %(n_interpolated_cells)s
-        %(account_for_unbalancedness)s
-        %(ott_jax_batch_size)s
-        %(use_posterior_marginals)s
-        %(seed_sampling)s
-        %(backend)s
-        %(kwargs_divergence)s
+        source
+            Key identifying the source distribution.
+        intermediate
+            Key identifying the intermediate distribution.
+        target
+            Key identifying the target distribution.
+        interpolation_parameter
+            Interpolation parameter in :math:`(0, 1)` defining the weight of the ``source`` and ``target``
+            distributions. If :obj:`None`, it is linearly interpolated.
+        n_interpolated_cells
+            Number of cells used for interpolation. If :obj:`None`, use the number of cells in the ``intermediate``
+            distribution.
+        account_for_unbalancedness
+            Whether to account for unbalancedness by assuming exponential cell growth and death.
+        batch_size
+            Number of rows/columns of the cost matrix to materialize during :meth:`push` or :meth:`pull`.
+            Larger value will require more memory.
+        posterior_marginals
+            Whether to use :attr:`posterior_growth_rates` or :attr:`prior_growth_rates`.
+            TODO(MUCDK): needs more explanation
+        seed
+            Random seed used when sampling the interpolated cells.
+        backend
+            Backend used for the distance computation.
+        kwargs
+            Keyword arguments for the distance function, depending on the ``backend``:
+
+            - ``'ott'`` - :func:`~ott.tools.sinkhorn_divergence.sinkhorn_divergence`.
 
         Returns
         -------
-        Wasserstein distance between OT-based interpolated distribution and the true cell distribution.
-        """
+        The distance between :term:`OT`-interpolated cells and cells at the ``intermediate`` time point.
+        It is recommended to compare this to the distances computed by :meth:`compute_time_point_distances` and
+        :meth:`compute_random_distance`.
+        """  # noqa: D205
         source_data, _, intermediate_data, _, target_data = self._get_data(  # type: ignore[misc]
             source,
             intermediate,
             target,
             posterior_marginals=posterior_marginals,
             only_start=False,
         )
@@ -617,57 +700,70 @@
             source=source,
             target=target,
             interpolation_parameter=interpolation_parameter,
             account_for_unbalancedness=account_for_unbalancedness,
             batch_size=batch_size,
             seed=seed,
         )
-        return self._compute_wasserstein_distance(
-            point_cloud_1=intermediate_data, point_cloud_2=interpolation, backend=backend, **kwargs
-        )
+        return self._compute_wasserstein_distance(intermediate_data, interpolation, backend=backend, **kwargs)
 
-    @d_mixins.dedent
     def compute_random_distance(
         self: TemporalMixinProtocol[K, B],
         source: K,
         intermediate: K,
         target: K,
         interpolation_parameter: Optional[float] = None,
         n_interpolated_cells: Optional[int] = None,
         account_for_unbalancedness: bool = False,
         posterior_marginals: bool = True,
         seed: Optional[int] = None,
-        backend: Literal["ott"] = "ott",  # TODO: not used
+        backend: Literal["ott"] = "ott",
         **kwargs: Any,
-    ) -> Numeric_t:
-        """
-        Compute the Wasserstein distance of a randomly interpolated cell distribution and the true cell distribution.
+    ) -> float:
+        """Compute `Wasserstein distance <https://en.wikipedia.org/wiki/Wasserstein_metric>`_ between randomly
+        interpolated and intermediate cells.
 
-        This method interpolates the cell trajectories at the `intermediate` time point using a random coupling and
-        computes the distance to the true cell distribution.
+        .. seealso::
+            - TODO(MUCDK): create an example showing the usage.
 
-        TODO: link to notebook
+        This function interpolates cells between the ``source`` and ``target`` distributions using a random
+        :term:`OT` coupling to approximate cells at the ``intermediate`` time point.
 
         Parameters
         ----------
-        %(start)s
-        %(intermediate_interpolation)s
-        %(end)s
-        %(interpolation_parameter)s
-        %(n_interpolated_cells)s
-        %(account_for_unbalancedness)s
-        %(use_posterior_marginals)s
-        %(seed_interpolation)s
-        %(backend)s
-        %(kwargs_divergence)s
+        source
+            Key identifying the source distribution.
+        intermediate
+            Key identifying the intermediate distribution.
+        target
+            Key identifying the target distribution.
+        interpolation_parameter
+            Interpolation parameter in :math:`(0, 1)` defining the weight of the ``source`` and ``target``
+            distributions. If :obj:`None`, it is linearly interpolated.
+        n_interpolated_cells
+            Number of cells used for interpolation. If :obj:`None`, use the number of cells in the ``intermediate``
+            distribution.
+        account_for_unbalancedness
+            Whether to account for unbalancedness by assuming exponential cell growth and death.
+        posterior_marginals
+            Whether to use :attr:`posterior_growth_rates` or :attr:`prior_growth_rates`.
+            TODO(MUCDK): needs more explanation
+        seed
+            Random seed used when sampling the interpolated cells.
+        backend
+            Backend used for the distance computation.
+        kwargs
+            Keyword arguments for the distance function, depending on the ``backend``:
+
+            - ``'ott'`` - :func:`~ott.tools.sinkhorn_divergence.sinkhorn_divergence`.
 
         Returns
         -------
-        The Wasserstein distance between a randomly interpolated cell distribution and the true cell distribution.
-        """
+        The distance between randomly interpolated cells and cells at the ``intermediate`` time point.
+        """  # noqa: D205
         source_data, growth_rates_source, intermediate_data, _, target_data = self._get_data(  # type: ignore[misc]
             source, intermediate, target, posterior_marginals=posterior_marginals, only_start=False
         )
 
         interpolation_parameter = self._get_interp_param(
             source, intermediate, target, interpolation_parameter=interpolation_parameter
         )
@@ -678,42 +774,52 @@
             n_interpolated_cells,
             source_data,
             target_data,
             interpolation_parameter=interpolation_parameter,
             growth_rates=growth_rates,
             seed=seed,
         )
-        return self._compute_wasserstein_distance(intermediate_data, random_interpolation, **kwargs)
+        return self._compute_wasserstein_distance(intermediate_data, random_interpolation, backend=backend, **kwargs)
 
-    @d_mixins.dedent
     def compute_time_point_distances(
         self: TemporalMixinProtocol[K, B],
         source: K,
         intermediate: K,
         target: K,
         posterior_marginals: bool = True,
         backend: Literal["ott"] = "ott",
         **kwargs: Any,
-    ) -> Tuple[Numeric_t, Numeric_t]:
-        """
-        Compute the Wasserstein distance of cell distributions between time points.
-
-        This method computes the Wasserstein distance between the cell distribution corresponding to `start` and `
-        intermediate` and `intermediate` and `end`, respectively.
+    ) -> Tuple[float, float]:
+        """Compute `Wasserstein distance <https://en.wikipedia.org/wiki/Wasserstein_metric>`_ between time points.
 
-        TODO: link to notebook
+        .. seealso::
+            - TODO(MUCDK): create an example showing the usage.
 
         Parameters
         ----------
-        %(start)s
-        %(intermediate)s
-        %(end)s
-        %(use_posterior_marginals)s
-        %(backend)s
-        %(kwargs_divergence)s
+        source
+            Key identifying the source distribution.
+        intermediate
+            Key identifying the intermediate distribution.
+        target
+            Key identifying the target distribution.
+        posterior_marginals
+            Whether to use :attr:`posterior_growth_rates` or :attr:`prior_growth_rates`.
+            TODO(MUCDK): needs more explanation
+        backend
+            Backend used for the distance computation.
+        kwargs
+            Keyword arguments for the distance function, depending on the ``backend``:
+
+            - ``'ott'`` - :func:`~ott.tools.sinkhorn_divergence.sinkhorn_divergence`.
+
+        Returns
+        -------
+        The distance between ``source`` and ``intermediate`` cells and
+        ``intermediate`` and ``target`` cells, respectively.
         """
         source_data, _, intermediate_data, _, target_data = self._get_data(  # type: ignore[misc]
             source,
             intermediate,
             target,
             posterior_marginals=posterior_marginals,
             only_start=False,
@@ -730,62 +836,73 @@
     def compute_batch_distances(
         self: TemporalMixinProtocol[K, B],
         time: K,
         batch_key: str,
         posterior_marginals: bool = True,
         backend: Literal["ott"] = "ott",
         **kwargs: Any,
-    ) -> np.float_:
-        """
-        Compute the mean Wasserstein distance between batches of a distribution corresponding to one time point.
+    ) -> float:
+        """Compute the average `Wasserstein distance <https://en.wikipedia.org/wiki/Wasserstein_metric>`_ between
+        batches for a specific time point.
+
+        .. seealso::
+            - TODO(MUCDK): create an example showing the usage.
 
         Parameters
         ----------
-        %(time_batch_distance)s
-        %(batch_key_batch_distance)s
-        %(use_posterior_marginals)s
-        %(backend)s
-        %(kwargs_divergence)
+        time
+            Time point for which to compute the distances.
+        batch_key
+            Key in :attr:`~anndata.AnnData.obs` where batches are stored.
+        posterior_marginals
+            Whether to use :attr:`posterior_growth_rates` or :attr:`prior_growth_rates`.
+            TODO(MUCDK): needs more explanation
+        backend
+            Backend used for the distance computation.
+        kwargs
+            Keyword arguments for the distance function, depending on the ``backend``:
+
+            - ``'ott'`` - :func:`~ott.tools.sinkhorn_divergence.sinkhorn_divergence`.
 
         Returns
         -------
-        The mean Wasserstein distance between batches of a distribution corresponding to one time point.
-        """
+        The average distance between batches for a specific time point.
+        """  # noqa: D205
         data, adata = self._get_data(time, posterior_marginals=posterior_marginals, only_start=True)  # type: ignore[misc] # noqa: E501
-        assert len(adata) == len(data), "TODO: wrong shapes"
-        dist: List[Numeric_t] = []
+        if len(data) != len(adata):
+            raise ValueError(f"Expected the `data` to have length `{len(adata)}`, found `{len(data)}`.")
+
+        dist: List[float] = []
         for batch_1, batch_2 in itertools.combinations(adata.obs[batch_key].unique(), 2):
             dist.append(
                 self._compute_wasserstein_distance(
-                    point_cloud_1=data[(adata.obs[batch_key] == batch_1).values, :],
-                    point_cloud_2=data[(adata.obs[batch_key] == batch_2).values, :],
+                    point_cloud_1=data[(adata.obs[batch_key] == batch_1).values],
+                    point_cloud_2=data[(adata.obs[batch_key] == batch_2).values],
                     backend=backend,
                     **kwargs,
                 )
             )
-        return np.mean(dist)
+        return np.mean(dist)  # type: ignore[return-value]
 
     # TODO(@MUCDK) possibly offer two alternatives, once exact EMD with POT backend and once approximate,
     # faster with same solver as used for original problems
     def _compute_wasserstein_distance(
         self: TemporalMixinProtocol[K, B],
         point_cloud_1: ArrayLike,
         point_cloud_2: ArrayLike,
         a: Optional[ArrayLike] = None,
         b: Optional[ArrayLike] = None,
         backend: Literal["ott"] = "ott",
         **kwargs: Any,
-    ) -> Numeric_t:
+    ) -> float:
         if backend == "ott":
-            from moscot.backends.ott._utils import _compute_sinkhorn_divergence
+            from moscot.backends.ott import sinkhorn_divergence
 
-            distance = _compute_sinkhorn_divergence(point_cloud_1, point_cloud_2, a, b, **kwargs)
-        else:
-            raise NotImplementedError("Only `ott` available as backend.")
-        return distance
+            return sinkhorn_divergence(point_cloud_1, point_cloud_2, a, b, **kwargs)
+        raise NotImplementedError("Only `ott` available as backend.")
 
     def _interpolate_gex_with_ot(
         self: TemporalMixinProtocol[K, B],
         number_cells: int,
         source_data: ArrayLike,
         target_data: ArrayLike,
         source: K,
@@ -831,15 +948,15 @@
             * (1 - interpolation_parameter)
             + target_data[rng.choice(len(target_data), size=number_cells), :] * interpolation_parameter
         )
 
     @staticmethod
     def _get_interp_param(
         source: K, intermediate: K, target: K, interpolation_parameter: Optional[float] = None
-    ) -> Numeric_t:
+    ) -> float:
         if TYPE_CHECKING:
             assert isinstance(source, float)
             assert isinstance(intermediate, float)
             assert isinstance(target, float)
         if interpolation_parameter is not None:
             if 0 < interpolation_parameter < 1:
                 return interpolation_parameter
@@ -851,20 +968,24 @@
             return (intermediate - source) / (target - source)
         raise ValueError(
             f"Expected intermediate time point to be in interval `({source}, {target})`, found `{intermediate}`."
         )
 
     @property
     def temporal_key(self) -> Optional[str]:
-        """Temporal key in :attr:`anndata.AnnData.obs`."""
+        """Temporal key in :attr:`~anndata.AnnData.obs`."""
         return self._temporal_key
 
     @temporal_key.setter
     def temporal_key(self: TemporalMixinProtocol[K, B], key: Optional[str]) -> None:
-        if key is not None and key not in self.adata.obs:
+        if key is None:
+            self._temporal_key = key
+            return
+        if key not in self.adata.obs:
             raise KeyError(f"Unable to find temporal key in `adata.obs[{key!r}]`.")
-        if key is not None and not is_numeric_dtype(self.adata.obs[key]):
+        col = self.adata.obs[key]
+        if not (is_categorical_dtype(col) and is_numeric_dtype(col.cat.categories)):
             raise TypeError(
-                "Temporal key has to be of numeric type."
-                f"Found `adata.obs[{key!r}]` to be of type `{infer_dtype(self.adata.obs[key])}`."
+                f"Expected `adata.obs[{key!r}]` to be categorical with numeric categories, "
+                f"found `{infer_dtype(col)}`."
             )
         self._temporal_key = key
```

### Comparing `moscot-0.3.0/src/moscot/utils/_data/allTFs_dmel.txt` & `moscot-0.3.1/src/moscot/utils/_data/allTFs_dmel.txt`

 * *Files identical despite different names*

### Comparing `moscot-0.3.0/src/moscot/utils/_data/allTFs_hg38.txt` & `moscot-0.3.1/src/moscot/utils/_data/allTFs_hg38.txt`

 * *Files identical despite different names*

### Comparing `moscot-0.3.0/src/moscot/utils/_data/allTFs_mm.txt` & `moscot-0.3.1/src/moscot/utils/_data/allTFs_mm.txt`

 * *Files identical despite different names*

### Comparing `moscot-0.3.0/src/moscot/utils/_data/human_apoptosis.txt` & `moscot-0.3.1/src/moscot/utils/_data/human_apoptosis.txt`

 * *Files identical despite different names*

### Comparing `moscot-0.3.0/src/moscot/utils/_data/human_proliferation.txt` & `moscot-0.3.1/src/moscot/utils/_data/human_proliferation.txt`

 * *Files identical despite different names*

### Comparing `moscot-0.3.0/src/moscot/utils/_data/mouse_apoptosis.txt` & `moscot-0.3.1/src/moscot/utils/_data/mouse_apoptosis.txt`

 * *Files identical despite different names*

### Comparing `moscot-0.3.0/src/moscot/utils/_data/mouse_proliferation.txt` & `moscot-0.3.1/src/moscot/utils/_data/mouse_proliferation.txt`

 * *Files identical despite different names*

### Comparing `moscot-0.3.0/src/moscot/utils/subset_policy.py` & `moscot-0.3.1/src/moscot/utils/subset_policy.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import networkx as nx
 import numpy as np
 import pandas as pd
 
 from anndata import AnnData
 
 from moscot import _constants
+from moscot._logging import logger
 from moscot._types import ArrayLike, Policy_t
 
 __all__ = [
     "SubsetPolicy",
     "OrderedPolicy",
     "StarPolicy",
     "ExternalStarPolicy",
@@ -47,15 +48,29 @@
 class FormatterMixin(abc.ABC):
     @abc.abstractmethod
     def _format(self, value: Any, *, is_source: bool) -> Any:
         pass
 
 
 class SubsetPolicy(Generic[K], abc.ABC):
-    """Policy class."""
+    r"""Base policy class.
+
+    Parameters
+    ----------
+    adata
+        Annotated data object or a categorical data.
+    key
+        Key in :attr:`~anndata.AnnData.obs` where the categorical data is stored.
+    verify_integrity
+        Whether to check that the data has :math:`\ge 2` categories.
+
+    Examples
+    --------
+    - See :doc:`../notebooks/examples/problems/400_subset_policy` on how to use different policies.
+    """
 
     def __init__(
         self,
         adata: Union[AnnData, pd.Series, pd.Categorical],
         key: Optional[str] = None,
         verify_integrity: bool = True,
     ):
@@ -69,78 +84,120 @@
         self._subset_key: Optional[str] = key
 
         if verify_integrity and len(self._cat) < 2:
             raise ValueError(f"Policy must contain at least `2` different values, found `{len(self._cat)}`.")
 
     @abc.abstractmethod
     def _create_graph(self, **kwargs: Any) -> Set[Tuple[K, K]]:
-        pass
+        """Create a policy graph."""
+
+    @abc.abstractmethod
+    def _plan(self, **kwargs: Any) -> Sequence[Tuple[K, K]]:
+        """Compute a sequence of steps based on the policy graph."""
+
+    def create_graph(self, **kwargs: Any) -> "SubsetPolicy[K]":
+        """Create a policy graph.
+
+        Parameters
+        ----------
+        kwargs
+            Keyword arguments.
+
+        Returns
+        -------
+        Return self.
+        """
+        graph = self._create_graph(**kwargs)
+        if not len(graph):
+            raise ValueError("The policy graph is empty.")
+        self._graph = graph
+        return self
 
     def plan(
         self,
         filter: Optional[Sequence[Tuple[K, K]]] = None,  # noqa: A002
         explicit_steps: Optional[Sequence[Tuple[K, K]]] = None,
         **kwargs: Any,
     ) -> Sequence[Tuple[K, K]]:
-        """Compute all pairs of distributions belonging to the policy.
+        """Compute a sequence of steps based on the policy graph.
+
+        Useful when calling :meth:`create_masks`.
 
         Parameters
         ----------
-        %(fitler)s
-        %(explicit_steps)s
-        %(kwargs_plan)s
+        filter
+            Steps to exclude. If :obj:`None`, keep all the steps.
+        explicit_steps
+            Precomputed sequence of steps to use.
+        kwargs
+            Additional keyword arguments.
 
         Returns
         -------
-        Sequence containing pairs of distributions.
+        Sequence of steps.
         """
         if explicit_steps is not None:
             G = nx.DiGraph()
             G.add_edges_from(explicit_steps)
             if not set(G.nodes).issubset(self._cat):
                 raise ValueError(
                     f"Explicitly specified steps `{set(explicit_steps)}` must be a subset of `{self._cat}`."
                 )
-            if not nx.has_path(G, explicit_steps[0][0], explicit_steps[-1][1]):
-                raise ValueError("Explicitly specified steps do not form a connected path.")
+            src = explicit_steps[0][0]
+            tgt = explicit_steps[-1][1]
+            if not nx.has_path(G, src, tgt):
+                raise ValueError(f"Explicitly specified steps do not form a connected path from `{src}` to `{tgt}`.")
             return explicit_steps
         plan = self._plan(**kwargs)
         # TODO(michalk8): ensure unique
         if filter is not None:
             plan = self._filter_plan(plan, filter=filter)
         if not len(plan):
             raise ValueError("Unable to create a plan, no steps were selected after filtering.")
         return plan
 
-    @abc.abstractmethod
-    def _plan(self, **kwargs: Any) -> Sequence[Tuple[K, K]]:
-        pass
-
-    def __call__(self, **kwargs: Any) -> "SubsetPolicy[K]":
-        graph = self._create_graph(**kwargs)
-        if not len(graph):
-            raise ValueError("The policy graph is empty.")
-        self._graph = graph
-        return self
-
     def _filter_plan(
         self, plan: Sequence[Tuple[K, K]], filter: Sequence[Tuple[K, K]]  # noqa: A002
     ) -> Sequence[Tuple[K, K]]:
         return [step for step in plan if step in filter]
 
     def create_mask(self, value: Union[K, Sequence[K]], *, allow_empty: bool = False) -> ArrayLike:
+        """Create a mask used to subset the data.
+
+        Parameters
+        ----------
+        value
+            Values in the data which determine the mask.
+        allow_empty
+            Whether to allow empty mask.
+
+        Returns
+        -------
+        Boolean mask of the same shape as the data.
+        """
         if isinstance(value, str) or not isinstance(value, Iterable):
             mask = self._data == value
         else:
             mask = self._data.isin(value)
         if not allow_empty and not np.sum(mask):
             raise ValueError("Unable to construct an empty mask, use `allow_empty=True` to override.")
         return np.asarray(mask)
 
     def create_masks(self, discard_empty: bool = True) -> Dict[Tuple[K, K], Tuple[ArrayLike, ArrayLike]]:
+        """Create masks based on the policy graph.
+
+        Parameters
+        ----------
+        discard_empty
+            Whether to remove empty masks.
+
+        Returns
+        -------
+        Masks for each edge in the policy graph.
+        """
         res = {}
         for a, b in self._graph:
             try:
                 mask_a = self.create_mask(a, allow_empty=not discard_empty)
                 mask_b = self.create_mask(b, allow_empty=not discard_empty)
                 res[a, b] = mask_a, mask_b
             except ValueError as e:
@@ -149,74 +206,78 @@
 
         if not res:
             # can only happen when `discard_empty=True`
             raise ValueError("All empty masks were discarded.")
 
         return res
 
-    def add_node(self, node: Tuple[K, K], only_existing: bool = False) -> None:
-        """
-        Add a node to the policy.
+    def add_node(self, node: Tuple[K, K], only_existing: bool = False) -> "SubsetPolicy[K]":
+        """Add a node to the policy graph.
 
         Parameters
         ----------
-        %(node)s
-        %(only_existing)s
+        node
+            Node to add.
+        only_existing
+            Whether to allow creating new nodes or only connect existing ones.
 
         Returns
         -------
-        None
+        Remove the ``node``, if present and return self.
         """
-        if self._graph is None:
-            raise RuntimeError("Construct the policy graph first.")
         src, tgt = node
         if src == tgt:
             raise ValueError(f"Unable to add `{src, tgt}` node, self connections are disallowed.")
         if only_existing and (src not in self._cat or tgt not in self._cat):
             raise ValueError(
                 f"Unable to add `{src}` or `{tgt}` node(s) that are not already present "
                 f"in the policy graph, use `only_existing=False` to override."
             )
         self._graph.add(node)
+        return self
 
-    def remove_node(self, node: Tuple[K, K]) -> None:
-        """
-        Remove a node from the policy graph.
+    def remove_node(self, node: Tuple[K, K]) -> "SubsetPolicy[K]":
+        """Remove a node from the policy graph.
 
         Parameters
         ----------
-        %(node)s
+        node
+            Node to remove.
 
         Returns
         -------
-        None
+        Remove the ``node``, if present and return self.
         """
-        if self._graph is None:
-            raise RuntimeError("Construct the policy graph first.")
         with contextlib.suppress(KeyError):
             self._graph.remove(node)
+        return self
+
+    @property
+    def key(self) -> Optional[str]:
+        """Key in :attr:`~anndata.AnnData.obs` defining the policy."""
+        return self._subset_key
 
 
 class OrderedPolicy(SubsetPolicy[K], abc.ABC):
-    """
-    Policy taking into account the order of nodes.
+    """Base ordered policy.
 
     Parameters
     ----------
-    %(adata_policy)s
-    %(kwargs_policy)s
-
-    Returns
-    -------
-    None
+    adata
+        Annotated data object or an ordered categorical data.
+    kwargs
+        Additional keyword arguments.
     """
 
     def __init__(self, adata: Union[AnnData, pd.Series, pd.Categorical], **kwargs: Any):
         super().__init__(adata, **kwargs)
-        # TODO(michalk8): verify whether they can be ordered (only numeric?) + warn (or just raise)
+        if not self._data.cat.ordered:
+            # TODO(michalk8, MUCDK): not order by default by us?
+            logger.info(f"Ordering {self._data.index} in ascending order.")
+            self._data.sort_values(ascending=True)
 
     def _plan(
         self, forward: bool = True, start: Optional[K] = None, end: Optional[K] = None, **_: Any
     ) -> Sequence[Tuple[K, K]]:
         if self._graph is None:
             raise RuntimeError("Construct the policy graph first.")
         if start is None and end is None:
@@ -235,112 +296,188 @@
             raise ValueError("Both start and end node are `None`.")
 
         path = nx.shortest_path(G, start, end)
         path = list(zip(path[:-1], path[1:]))
 
         return path if forward else path[::-1]
 
+    def reverse(self) -> "OrderedPolicy[K]":
+        """Reverse the policy."""
+        cats = self._data.cat.categories
+        data = self._data.cat.reorder_categories(list(reversed(cats)))
+        return type(self)(data, key=self.key, verify_integrity=False)
+
 
 class SimplePlanPolicy(SubsetPolicy[K], abc.ABC):
+    """Policy whose plan is just the underlying policy graph."""
+
     def _plan(self, **_: Any) -> Sequence[Tuple[K, K]]:
         return list(self._graph)
 
 
 class StarPolicy(SimplePlanPolicy[K]):
+    r"""Policy with a star topology.
+
+    Parameters
+    ----------
+    adata
+        Annotated data object or a categorical data.
+    key
+        Key in :attr:`~anndata.AnnData.obs` where the categorical data is stored.
+    verify_integrity
+        Whether to check that the data has :math:`\ge 2` categories.
+    """
+
     def _create_graph(self, reference: K, **kwargs: Any) -> Set[Tuple[K, K]]:  # type: ignore[override]
         if reference not in self._cat:
             raise ValueError(f"Reference `{reference}` is not in valid nodes: `{self._cat}`.")
         return {(c, reference) for c in self._cat if c != reference}
 
     def _filter_plan(
         self, plan: Sequence[Tuple[K, K]], filter: Sequence[Union[K, Tuple[K, K]]]  # noqa: A002
     ) -> Sequence[Tuple[K, K]]:
         filter = [src[0] if isinstance(src, tuple) else src for src in filter]  # noqa: A001
         return [(src, ref) for src, ref in plan if src in filter]
 
-    @property
-    def reference(self) -> K:
-        for _, ref in self._graph:
-            return ref
-        raise ValueError("Graph is empty.")
-
-    def add_node(self, node: Union[K, Tuple[K, K]], only_existing: bool = False) -> None:
+    def add_node(self, node: Union[K, Tuple[K, K]], only_existing: bool = False) -> "StarPolicy[K]":
         if not isinstance(node, tuple):
             node = (node, self.reference)
-        return super().add_node(node, only_existing=only_existing)  # type: ignore[arg-type]
+        return super().add_node(node, only_existing=only_existing)  # type: ignore[return-value, arg-type]
 
-    def remove_node(self, node: Union[K, Tuple[K, K]]) -> None:
+    def remove_node(self, node: Union[K, Tuple[K, K]]) -> "StarPolicy[K]":
         if not isinstance(node, tuple):
             node = (node, self.reference)
-        return super().remove_node(node)  # type: ignore[arg-type]
+        return super().remove_node(node)  # type: ignore[return-value, arg-type]
+
+    @property
+    def reference(self) -> K:
+        """Central node."""
+        for _, ref in self._graph:
+            return ref
+        raise ValueError("Graph is empty.")
 
 
 class ExternalStarPolicy(FormatterMixin, StarPolicy[K]):
-    """Policy with one central node connected to all other nodes."""
+    """Policy with star topology and external central node.
+
+    Parameters
+    ----------
+    adata
+        Annotated data object.
+    tgt_name
+        Name of the central node.
+    kwargs
+        Additional keyword arguments.
+    """
 
     _SENTINEL = object()
 
-    def __init__(self, adata: Union[AnnData, pd.Series, pd.Categorical], tgt_name: str = "ref", **kwargs: Any):
+    def __init__(self, adata: Union[AnnData, pd.Series, pd.Categorical], tgt_name: K = "ref", **kwargs: Any):
         super().__init__(adata, **kwargs)
-        self._tgt_name: K = tgt_name  # type: ignore [assignment]
+        self._tgt_name = tgt_name
 
     def _format(self, value: K, *, is_source: bool) -> K:
         if is_source:
             return value
         if value is self._SENTINEL:
             return self._tgt_name
         raise ValueError(f"Expected value to be `{self._SENTINEL}`, found `{value}`.")
 
     def _create_graph(self, **_: Any) -> Set[Tuple[K, object]]:  # type: ignore[override]
         return {(c, self._SENTINEL) for c in self._cat if c != self._SENTINEL}
 
     def _plan(self, **_: Any) -> Sequence[Tuple[K, K]]:
         return [(src, self._format(tgt, is_source=False)) for (src, tgt) in self._graph]
 
-    def add_node(self, node: Union[K, Tuple[K, K]], only_existing: bool = False) -> None:
-        """Add a node to the policy."""
+    def add_node(self, node: Union[K, Tuple[K, K]], only_existing: bool = False) -> "ExternalStarPolicy[K]":
         if isinstance(node, tuple):
             _, tgt = node
+        # TODO(michalk8): tgt can be undefined
         if tgt is self._tgt_name:
-            return None
-        return super().add_node(node, only_existing=only_existing)  # type: ignore[arg-type]
+            return self
+        return super().add_node(node, only_existing=only_existing)  # type: ignore[return-value, arg-type]
 
     def create_masks(self, discard_empty: bool = True) -> Dict[Tuple[K, K], Tuple[ArrayLike, ArrayLike]]:
+        del discard_empty
         return super().create_masks(discard_empty=False)
 
 
 class SequentialPolicy(OrderedPolicy[K]):
-    """Policy connecting subsequent nodes."""
+    """Policy which connects immediate successors.
+
+    Parameters
+    ----------
+    adata
+        Annotated data object.
+    upper
+        Whether to use subsequent nodes instead of the preceding ones.
+    kwargs
+        Additional keyword arguments.
+    """
 
     def _create_graph(self, *_: Any, **__: Any) -> Set[Tuple[K, K]]:
         return set(zip(self._cat[:-1], self._cat[1:]))
 
 
 class TriangularPolicy(OrderedPolicy[K]):
-    """Connect all nodes with all subsequent nodes."""
+    """Policy which connects all preceding/subsequent nodes.
+
+    Parameters
+    ----------
+    adata
+        Annotated data object.
+    upper
+        Whether to use subsequent nodes instead of the preceding ones.
+    kwargs
+        Additional keyword arguments.
+    """
 
     def __init__(self, adata: Union[AnnData, pd.Series, pd.Categorical], upper: bool = True, **kwargs: Any):
         super().__init__(adata, **kwargs)
-        self._compare = operator.lt if upper else operator.gt
+        self._comparator = operator.lt if upper else operator.gt
 
     def _create_graph(self, **__: Any) -> Set[Tuple[K, K]]:
-        return {(a, b) for a, b in itertools.product(self._cat, self._cat) if self._compare(a, b)}
+        return {(a, b) for a, b in itertools.product(self._cat, self._cat) if self._comparator(a, b)}
 
 
 class ExplicitPolicy(SimplePlanPolicy[K]):
-    """A policy specified by the user."""
+    r"""Explicitly specified policy.
+
+    The policy graph is passed directly in :meth:`create_graph`.
+
+    Parameters
+    ----------
+    adata
+        Annotated data object or a categorical data.
+    key
+        Key in :attr:`~anndata.AnnData.obs` where the categorical data is stored.
+    verify_integrity
+        Whether to check that the data has :math:`\ge 2` categories.
+    """
 
     def _create_graph(self, subset: Sequence[Tuple[K, K]], **_: Any) -> Set[Tuple[K, K]]:  # type: ignore[override]
         if subset is None:
             raise ValueError("No steps specifying the explicit policy.")
         return set(subset)  # pass-through, all checks are done later
 
 
 class DummyPolicy(FormatterMixin, SubsetPolicy[str]):
-    """Policy to handle sentinel values."""
+    """Policy TODO.
+
+    Parameters
+    ----------
+    adata
+        Annotated data object or a categorical data.
+    src_name
+        TODO.
+    tgt_name
+        TODO.
+    kwargs
+        Additional keyword arguments.
+    """
 
     _SENTINEL = object()
 
     def __init__(
         self,
         adata: Union[AnnData, pd.Series, pd.Categorical],
         src_name: Literal["src"] = "src",
@@ -373,34 +510,36 @@
     adata: Union[AnnData, pd.Series, pd.Categorical],
     **kwargs: Any,
 ) -> SubsetPolicy[K]:
     """Create a policy.
 
     Parameters
     ----------
-    %(policy_kind)s
-    %(adata)s
+    kind
+        What policy to create.
+    adata
+        Annotated data object.
     kwargs
-        Keyword arguments for a :class:`~moscot.utils.subset_policy.SubsetPolicy`.
+        Additional keyword arguments.
 
     Returns
     -------
     The policy.
 
     Notes
     -----
-    TODO: link policy example.
+    - See :doc:`../notebooks/examples/problems/400_subset_policy` on how to use different policies.
     """
     if kind == _constants.SEQUENTIAL:
         return SequentialPolicy(adata, **kwargs)
     if kind == _constants.STAR:
         return StarPolicy(adata, **kwargs)
     if kind == _constants.EXTERNAL_STAR:
         return ExternalStarPolicy(adata, **kwargs)
     if kind == _constants.TRIU:
         return TriangularPolicy(adata, **kwargs, upper=True)
     if kind == _constants.TRIL:
         return TriangularPolicy(adata, **kwargs, upper=False)
     if kind == _constants.EXPLICIT:
         return ExplicitPolicy(adata, **kwargs)
 
-    raise NotImplementedError(kind)
+    raise NotImplementedError(f"Policy `{kind}` is not yet implemented.")
```

### Comparing `moscot-0.3.0/src/moscot/utils/tagged_array.py` & `moscot-0.3.1/src/moscot/utils/tagged_array.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,43 +12,55 @@
 from moscot.costs import get_cost
 
 __all__ = ["Tag", "TaggedArray"]
 
 
 @enum.unique
 class Tag(str, enum.Enum):
-    """Tag used to interpret array-like data in a class:`TaggedArray`."""
+    """Tag in the :class:`~moscot.utils.tagged_array.TaggedArray`."""
 
     COST_MATRIX = "cost_matrix"  #: Cost matrix.
     KERNEL = "kernel"  #: Kernel matrix.
     POINT_CLOUD = "point_cloud"  #: Point cloud.
 
 
 @dataclass(frozen=True, repr=True)
 class TaggedArray:
-    """Tagged array."""
+    """Interface to interpret array-like data for :mod:`moscot.solvers`.
+
+    It is used to extract array-like data stored in :class:`~anndata.AnnData` and interpret it as either
+    :attr:`cost matrix <is_cost_matrix>`, :attr:`kernel matrix <is_kernel>` or
+    a :attr:`point cloud <is_point_cloud>`, depending on the :attr:`tag`.
+
+    Parameters
+    ----------
+    data_src
+        Source data.
+    data_tgt
+        Target data.
+    tag
+        How to interpret :attr:`data_src` and :attr:`data_tgt`.
+    cost
+        Cost function when ``tag = 'point_cloud'``.
+    """
 
     data_src: ArrayLike  #: Source data.
     data_tgt: Optional[ArrayLike] = None  #: Target data.
     tag: Tag = Tag.POINT_CLOUD  #: How to interpret :attr:`data_src` and :attr:`data_tgt`.
     cost: Optional[Union[str, Callable[..., Any]]] = None  #: Cost function when ``tag = 'point_cloud'``.
 
     @staticmethod
     def _extract_data(
         adata: AnnData,
         *,
         attr: Literal["X", "obsp", "obsm", "layers", "uns"],
         key: Optional[str] = None,
     ) -> ArrayLike:
         modifier = f"adata.{attr}" if key is None else f"adata.{attr}[{key!r}]"
-
-        try:
-            data = getattr(adata, attr)
-        except AttributeError:
-            raise AttributeError(f"Annotated data object has no attribute `{attr}`.") from None
+        data = getattr(adata, attr)
 
         try:
             if key is not None:
                 data = data[key]
         except KeyError:
             raise KeyError(f"Unable to fetch data from `{modifier}`.") from None
         except IndexError:
@@ -72,47 +84,44 @@
         key: Optional[str] = None,
         cost: CostFn_t = "sq_euclidean",
         backend: Literal["ott"] = "ott",
         **kwargs: Any,
     ) -> "TaggedArray":
         """Create tagged array from :class:`~anndata.AnnData`.
 
+        .. warning::
+            Sparse arrays will be always densified.
+
         Parameters
         ----------
         adata
             Annotated data object.
         dist_key
-            Helper key which determines into which subset ``adata`` belongs.
+            Key which determines into which source/target subset ``adata`` belongs.
         attr
             Attribute of :class:`~anndata.AnnData` used when extracting/computing the cost.
         tag
             Tag used to interpret the extracted data.
         key
             Key in the ``attr`` of :class:`~anndata.AnnData` used when extracting/computing the cost.
         cost
             Cost function to apply to the extracted array, depending on ``tag``:
 
             - if ``tag = 'point_cloud'``, it is extracted from the ``backend``.
             - if ``tag = 'cost'`` or ``tag = 'kernel'``, and ``cost = 'custom'``,
               the extracted array is already assumed to be a cost/kernel matrix.
               Otherwise, :class:`~moscot.base.cost.BaseCost` is used to compute the cost matrix.
-        cost_kwargs
-            Keyword arguments for TODO
         backend
             Which backend to use, see :func:`~moscot.backends.utils.get_available_backends`.
         kwargs
-            Keyword arguments for :class:`~moscot.base.cost.BaseCost` or any backend-specific cost.
+            Keyword arguments for the :class:`~moscot.base.cost.BaseCost` or any backend-specific cost.
 
         Returns
         -------
         The tagged array.
-
-        Notes
-        -----
-        Sparse arrays will be always densified.
         """
         if tag == Tag.COST_MATRIX:
             if cost == "custom":  # our custom cost functions
                 modifier = f"adata.{attr}" if key is None else f"adata.{attr}[{key!r}]"
                 data = cls._extract_data(adata, attr=attr, key=key)
                 if np.any(data < 0):
                     raise ValueError(f"Cost matrix in `{modifier}` contains negative values.")
@@ -144,9 +153,9 @@
     @property
     def is_kernel(self) -> bool:
         """Whether :attr:`data_src` is a kernel matrix."""
         return self.tag == Tag.KERNEL
 
     @property
     def is_point_cloud(self) -> bool:
-        """Whether :attr:`data_src` (and optionally) :attr:`data_tgt` is/are a point cloud."""
+        """Whether :attr:`data_src` (and optionally) :attr:`data_tgt` is a point cloud."""
         return self.tag == Tag.POINT_CLOUD
```

### Comparing `moscot-0.3.0/src/moscot.egg-info/PKG-INFO` & `moscot-0.3.1/src/moscot.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moscot
-Version: 0.3.0
+Version: 0.3.1
 Summary: Multi-omic single-cell optimal transport tools
 Author: Dominik Klein, Giovanni Palla, Michal Klein, Zoe Piran, Marius Lange
 Maintainer-email: Dominik Klein <dominik.klein@helmholtz-muenchen.de>, Giovanni Palla <giovanni.palla@helmholtz-muenchen.de>, Michal Klein <michal.klein@helmholtz-muenchen.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Theis Lab
         All rights reserved.
@@ -58,54 +58,73 @@
 Description-Content-Type: text/x-rst
 Provides-Extra: spatial
 Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE
 
-|Codecov|
+|PyPI| |Downloads| |CI| |Pre-commit| |Codecov| |Docs|
 
 moscot - multi-omic single-cell optimal transport tools
 =======================================================
 
 **moscot** is a scalable framework for Optimal Transport (OT) applications in
 single-cell genomics. It can be used for
-- temporal and spatio-temporal trajectory inference
-- spatial mapping
-- spatial alignment
+
+- trajectory inference (incorporating spatial and lineage information)
+- mapping cells to their spatial organisation
+- aligning spatial transcriptomics slides
+- translating modalities
 - prototyping of new OT models in single-cell genomics
 
 **moscot** is powered by
 `OTT <https://ott-jax.readthedocs.io>`_ which is a JAX-based Optimal
 Transport toolkit that supports just-in-time compilation, GPU acceleration, automatic
 differentiation and linear memory complexity for OT problems.
 
 Installation
 ------------
 You can install **moscot** via::
 
     pip install moscot
 
-In order to install **moscot** from source, run::
+In order to install **moscot** from in editable mode, run::
 
     git clone https://github.com/theislab/moscot
     cd moscot
-    pip install -e .'[dev]'
-
-If used with GPU, additionally run::
-
-    pip install --upgrade "jax[cuda]" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
+    pip install -e .
 
-
-.. |Codecov| image:: https://codecov.io/gh/theislab/moscot/branch/master/graph/badge.svg?token=Rgtm5Tsblo
-    :target: https://codecov.io/gh/theislab/moscot
-    :alt: Coverage
+For further instructions how to install jax, please refer to https://github.com/google/jax.
 
 Resources
 ---------
 
 Please have a look at our `documentation <https://moscot.readthedocs.io>`_
 
 Reference
 ---------
 
 Our preprint "Mapping cells through time and space with moscot" can be found `here <https://www.biorxiv.org/content/10.1101/2023.05.11.540374v1>`_.
+
+.. |Codecov| image:: https://codecov.io/gh/theislab/moscot/branch/master/graph/badge.svg?token=Rgtm5Tsblo
+    :target: https://codecov.io/gh/theislab/moscot
+    :alt: Coverage
+
+.. |PyPI| image:: https://img.shields.io/pypi/v/moscot.svg
+    :target: https://pypi.org/project/moscot/
+    :alt: PyPI
+
+.. |CI| image:: https://img.shields.io/github/actions/workflow/status/theislab/moscot/test.yml?branch=main
+    :target: https://github.com/theislab/moscot/actions
+    :alt: CI
+
+.. |Pre-commit| image:: https://results.pre-commit.ci/badge/github/theislab/moscot/main.svg
+   :target: https://results.pre-commit.ci/latest/github/theislab/moscot/main
+   :alt: pre-commit.ci status
+
+.. |Docs| image:: https://img.shields.io/readthedocs/moscot
+    :target: https://moscot.readthedocs.io/en/stable/
+    :alt: Documentation
+
+.. |Downloads| image:: https://pepy.tech/badge/moscot
+    :target: https://pepy.tech/project/moscot
+    :alt: Downloads
```

### Comparing `moscot-0.3.0/src/moscot.egg-info/SOURCES.txt` & `moscot-0.3.1/src/moscot.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -15,19 +15,14 @@
 src/moscot/datasets.py
 src/moscot/py.typed
 src/moscot.egg-info/PKG-INFO
 src/moscot.egg-info/SOURCES.txt
 src/moscot.egg-info/dependency_links.txt
 src/moscot.egg-info/requires.txt
 src/moscot.egg-info/top_level.txt
-src/moscot/_docs/__init__.py
-src/moscot/_docs/_docs.py
-src/moscot/_docs/_docs_mixins.py
-src/moscot/_docs/_docs_plot.py
-src/moscot/_docs/_utils.py
 src/moscot/backends/__init__.py
 src/moscot/backends/utils.py
 src/moscot/backends/ott/__init__.py
 src/moscot/backends/ott/_utils.py
 src/moscot/backends/ott/output.py
 src/moscot/backends/ott/solver.py
 src/moscot/base/__init__.py
@@ -45,14 +40,17 @@
 src/moscot/costs/_costs.py
 src/moscot/costs/_utils.py
 src/moscot/plotting/__init__.py
 src/moscot/plotting/_plotting.py
 src/moscot/plotting/_utils.py
 src/moscot/problems/__init__.py
 src/moscot/problems/_utils.py
+src/moscot/problems/cross_modality/__init__.py
+src/moscot/problems/cross_modality/_mixins.py
+src/moscot/problems/cross_modality/_translation.py
 src/moscot/problems/generic/__init__.py
 src/moscot/problems/generic/_generic.py
 src/moscot/problems/generic/_mixins.py
 src/moscot/problems/space/__init__.py
 src/moscot/problems/space/_alignment.py
 src/moscot/problems/space/_mapping.py
 src/moscot/problems/space/_mixins.py
```

