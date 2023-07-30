# Comparing `tmp/yambs-2.2.0.tar.gz` & `tmp/yambs-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yambs-2.2.0.tar", last modified: Sat Jul 29 06:53:33 2023, max compression
+gzip compressed data, was "yambs-2.2.1.tar", last modified: Sun Jul 30 04:46:22 2023, max compression
```

## Comparing `yambs-2.2.0.tar` & `yambs-2.2.1.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.786966 yambs-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-29 06:52:19.000000 yambs-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-29 06:53:33.786966 yambs-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8840 2023-07-29 06:52:19.000000 yambs-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-29 06:52:19.000000 yambs-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 06:53:33.786966 yambs-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-29 06:52:19.000000 yambs-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.778967 yambs-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-29 06:52:19.000000 yambs-2.2.0/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-29 06:52:19.000000 yambs-2.2.0/tests/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.778967 yambs-2.2.0/yambs/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.782966 yambs-2.2.0/yambs/aggregation/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/aggregation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.782966 yambs-2.2.0/yambs/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/commands/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/commands/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/commands/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/commands/uf2conv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.782966 yambs-2.2.0/yambs/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/config/board.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/config/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/config/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.782966 yambs-2.2.0/yambs/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.782966 yambs-2.2.0/yambs/data/includes/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/includes/chips.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/includes/common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/includes/infineon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/includes/microchip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/native.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.782966 yambs-2.2.0/yambs/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/schemas/Architecture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/schemas/Board.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/schemas/Chip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/schemas/CommonConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/schemas/Dependency.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/schemas/Github.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/schemas/Native.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/schemas/Project.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/schemas/Toolchain.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/schemas/Variant.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/schemas/config_common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/schemas/entry_common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/schemas/toolchain_common.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.786966 yambs-2.2.0/yambs/data/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/templates/all.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/templates/architecture.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/templates/board.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/templates/build.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/templates/chip.ld.j2
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/templates/chip.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/templates/compile_commands.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/templates/native_all.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/templates/native_build.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/templates/native_rules.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/templates/rules.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/templates/toolchain.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/templates/variant.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/uf2families.json
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/data/yambs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.786966 yambs-2.2.0/yambs/dependency/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/dependency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/dependency/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/dependency/github.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.786966 yambs-2.2.0/yambs/dependency/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/dependency/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/dependency/handlers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/dependency/handlers/yambs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/dependency/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/dependency/state.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/dev_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.786966 yambs-2.2.0/yambs/dist/
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/dist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.786966 yambs-2.2.0/yambs/environment/
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/environment/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.786966 yambs-2.2.0/yambs/generate/
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/generate/architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/generate/boards.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/generate/chips.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/generate/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.786966 yambs-2.2.0/yambs/generate/ninja/
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/generate/ninja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/generate/ninja/format.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/generate/toolchains.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/generate/variants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.786966 yambs-2.2.0/yambs/github/
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.786966 yambs-2.2.0/yambs/translation/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/translation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.786966 yambs-2.2.0/yambs/uf2/
--rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-07-29 06:52:19.000000 yambs-2.2.0/yambs/uf2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 06:53:33.782966 yambs-2.2.0/yambs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-29 06:53:33.000000 yambs-2.2.0/yambs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-29 06:53:33.000000 yambs-2.2.0/yambs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 06:53:33.000000 yambs-2.2.0/yambs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-29 06:53:33.000000 yambs-2.2.0/yambs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-29 06:53:33.000000 yambs-2.2.0/yambs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 06:53:33.000000 yambs-2.2.0/yambs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:46:22.001957 yambs-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-30 04:45:05.000000 yambs-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-30 04:46:22.001957 yambs-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8840 2023-07-30 04:45:05.000000 yambs-2.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-30 04:45:05.000000 yambs-2.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 04:46:22.001957 yambs-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-30 04:45:05.000000 yambs-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:46:21.989957 yambs-2.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-30 04:45:05.000000 yambs-2.2.1/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-30 04:45:05.000000 yambs-2.2.1/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:46:21.993957 yambs-2.2.1/yambs/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:46:21.993957 yambs-2.2.1/yambs/aggregation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/aggregation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:46:21.993957 yambs-2.2.1/yambs/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/commands/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/commands/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/commands/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/commands/uf2conv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:46:21.993957 yambs-2.2.1/yambs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/config/board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/config/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/config/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:46:21.993957 yambs-2.2.1/yambs/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:46:21.997957 yambs-2.2.1/yambs/data/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/data/includes/chips.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/data/includes/common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/data/includes/infineon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/data/includes/microchip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/data/native.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:46:21.997957 yambs-2.2.1/yambs/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/data/schemas/Architecture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/data/schemas/Board.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/data/schemas/Chip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/data/schemas/CommonConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/data/schemas/Dependency.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/data/schemas/Github.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/data/schemas/Native.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/data/schemas/Project.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/data/schemas/Toolchain.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/data/schemas/Variant.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/data/schemas/config_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/data/schemas/entry_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/data/schemas/toolchain_common.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:46:21.997957 yambs-2.2.1/yambs/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/data/templates/all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/data/templates/architecture.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/data/templates/board.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/data/templates/build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/data/templates/chip.ld.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/data/templates/chip.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/data/templates/compile_commands.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/data/templates/native_all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/data/templates/native_build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/data/templates/native_rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/data/templates/rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/data/templates/toolchain.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/data/templates/variant.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/data/uf2families.json
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/data/yambs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:46:22.001957 yambs-2.2.1/yambs/dependency/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/dependency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/dependency/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/dependency/github.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:46:22.001957 yambs-2.2.1/yambs/dependency/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/dependency/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/dependency/handlers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/dependency/handlers/yambs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/dependency/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/dependency/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/dev_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:46:22.001957 yambs-2.2.1/yambs/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/dist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:46:22.001957 yambs-2.2.1/yambs/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/environment/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:46:22.001957 yambs-2.2.1/yambs/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/generate/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/generate/boards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/generate/chips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/generate/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:46:22.001957 yambs-2.2.1/yambs/generate/ninja/
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/generate/ninja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/generate/ninja/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/generate/toolchains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/generate/variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:46:22.001957 yambs-2.2.1/yambs/github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:46:22.001957 yambs-2.2.1/yambs/translation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/translation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:46:22.001957 yambs-2.2.1/yambs/uf2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-07-30 04:45:05.000000 yambs-2.2.1/yambs/uf2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 04:46:21.993957 yambs-2.2.1/yambs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-30 04:46:21.000000 yambs-2.2.1/yambs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-30 04:46:21.000000 yambs-2.2.1/yambs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 04:46:21.000000 yambs-2.2.1/yambs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-30 04:46:21.000000 yambs-2.2.1/yambs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-30 04:46:21.000000 yambs-2.2.1/yambs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-30 04:46:21.000000 yambs-2.2.1/yambs.egg-info/top_level.txt
```

### Comparing `yambs-2.2.0/LICENSE` & `yambs-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/PKG-INFO` & `yambs-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 2.2.0
+Version: 2.2.1
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
@@ -18,19 +18,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=9fd78d02f6bd1c0baddfb2fa7ba65d51
+    hash=2f414044223b7b56f2fb2a465aee095e
     =====================================
 -->
 
-# yambs ([2.2.0](https://pypi.org/project/yambs/))
+# yambs ([2.2.1](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-2.2.0/README.md` & `yambs-2.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=9fd78d02f6bd1c0baddfb2fa7ba65d51
+    hash=2f414044223b7b56f2fb2a465aee095e
     =====================================
 -->
 
-# yambs ([2.2.0](https://pypi.org/project/yambs/))
+# yambs ([2.2.1](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-2.2.0/pyproject.toml` & `yambs-2.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "yambs"
-version = "2.2.0"
+version = "2.2.1"
 description = "Yet another meta build-system."
 readme = "README.md"
 requires-python = ">=3.11"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `yambs-2.2.0/setup.py` & `yambs-2.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/tests/test_entry.py` & `yambs-2.2.1/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/aggregation/__init__.py` & `yambs-2.2.1/yambs/aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/app.py` & `yambs-2.2.1/yambs/app.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/commands/all.py` & `yambs-2.2.1/yambs/commands/all.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/commands/common.py` & `yambs-2.2.1/yambs/commands/common.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/commands/dist.py` & `yambs-2.2.1/yambs/commands/dist.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,22 +13,27 @@
 from vcorelib.args import CommandFunction as _CommandFunction
 from vcorelib.io import ARBITER
 from vcorelib.paths import create_hex_digest
 
 # internal
 from yambs.commands.common import add_config_arg
 from yambs.config.common import CommonConfig
+from yambs.dependency.manager import write_third_party_script
 from yambs.dist import copy_source_tree, dist_metadata, make_archives
 
 
 def dist_cmd(args: _Namespace) -> int:
     """Execute the dist command."""
 
     config = CommonConfig.load(path=args.config, root=args.dir)
 
+    # Ensure that the third-party build script doesn't contain any instructions
+    # to build third-party dependencies (that won't be present for linking).
+    write_third_party_script(config.third_party_script)
+
     # Prepare a temporary directory with project sources.
     with TemporaryDirectory() as tmp:
         path = Path(tmp)
 
         # Put everything under a directory named after the project slug (name
         # and version).
         base = path.joinpath(str(config.project))
```

### Comparing `yambs-2.2.0/yambs/commands/gen.py` & `yambs-2.2.1/yambs/commands/gen.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/commands/native.py` & `yambs-2.2.1/yambs/commands/native.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/commands/uf2conv.py` & `yambs-2.2.1/yambs/commands/uf2conv.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/config/__init__.py` & `yambs-2.2.1/yambs/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/config/board.py` & `yambs-2.2.1/yambs/config/board.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/config/common.py` & `yambs-2.2.1/yambs/config/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,31 +74,37 @@
     build_root: Path
     ninja_root: Path
     dist_root: Path
     third_party_root: Path
 
     file: Optional[Path]
 
-    def directory(self, name: str, mkdir: bool = True) -> Path:
+    dependencies: Set[Dependency]
+
+    def directory(
+        self, name: str, mkdir: bool = True, root: Path = None
+    ) -> Path:
         """Get a configurable directory."""
 
         name_root = Path(str(self.data[name]))
         if not name_root.is_absolute():
-            name_root = self.root.joinpath(name_root)
+            if root is None:
+                root = self.root
+            name_root = root.joinpath(name_root)
 
         if mkdir:
             name_root.mkdir(parents=True, exist_ok=True)
 
         return name_root
 
     def init(self, data: _JsonObject) -> None:
         """Initialize this instance."""
 
         self.data = data
-        self.root = Path()
+        self.root = Path(data["root"])  # type: ignore
 
         self.src_root = self.directory("src_root")
         self.build_root = self.directory("build_root")
         self.ninja_root = self.directory("ninja_out")
         self.dist_root = self.directory("dist_out")
         self.third_party_root = self.directory("third_party_root")
 
@@ -109,14 +115,19 @@
         # Collect project dependency data.
         self.dependencies: Set[Dependency] = set()
         for dep in data.get("dependencies", []):  # type: ignore
             new_dep = Dependency(data=dep, verify=False)  # type: ignore
             new_dep.github.setdefault("owner", self.project.owner)
             self.dependencies.add(new_dep)
 
+    @property
+    def third_party_script(self) -> Path:
+        """Get the path to the third-party build script."""
+        return self.ninja_root.joinpath("third_party.sh")
+
     @classmethod
     def load(
         cls: Type[T],
         path: Pathlike = DEFAULT_CONFIG,
         package_config: str = DEFAULT_CONFIG,
         root: Pathlike = None,
     ) -> T:
@@ -135,17 +146,16 @@
             ).data,
             _ARBITER.decode(path, includes_key=DEFAULT_INCLUDES_KEY).data,
             # Always allow the project-specific configuration to override
             # package data.
             expect_overwrite=True,
         )
 
+        if root is not None:
+            data["root"] = str(normalize(root))
+
         result = cls.create(data)
 
         if path.is_file():
             result.file = path
 
-        if root is not None:
-            result.root = normalize(root)
-            result.root.mkdir(parents=True, exist_ok=True)
-
         return result
```

### Comparing `yambs-2.2.0/yambs/data/includes/chips.yaml` & `yambs-2.2.1/yambs/data/includes/chips.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/data/includes/infineon.yaml` & `yambs-2.2.1/yambs/data/includes/infineon.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/data/includes/microchip.yaml` & `yambs-2.2.1/yambs/data/includes/microchip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/data/native.yaml` & `yambs-2.2.1/yambs/data/native.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/data/schemas/Chip.yaml` & `yambs-2.2.1/yambs/data/schemas/Chip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/data/schemas/Config.yaml` & `yambs-2.2.1/yambs/data/schemas/Config.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/data/schemas/Native.yaml` & `yambs-2.2.1/yambs/data/schemas/Native.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/data/schemas/config_common.yaml` & `yambs-2.2.1/yambs/data/schemas/config_common.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 ---
 properties:
+  root:
+    type: string
+    default: "."
+
   src_root:
     type: string
     default: src
 
   ninja_out:
     type: string
     default: ninja
```

### Comparing `yambs-2.2.0/yambs/data/templates/native_rules.ninja.j2` & `yambs-2.2.1/yambs/data/templates/native_rules.ninja.j2`

 * *Files 20% similar despite different names*

```diff
@@ -22,10 +22,10 @@
   command = ar rcs $out $in
 
 build_dir = {{build_root}}/$variant
 
 rule script
   command = /bin/bash $in $out
 
-build $build_dir/third_party.txt: script $third_party_dir/third_party.sh
+build $build_dir/third_party.txt: script $include_dir/third_party.sh
 
 build ${variant}_third_party: phony $build_dir/third_party.txt
```

### Comparing `yambs-2.2.0/yambs/data/templates/rules.ninja.j2` & `yambs-2.2.1/yambs/data/templates/rules.ninja.j2`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/data/uf2families.json` & `yambs-2.2.1/yambs/data/uf2families.json`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/dependency/config.py` & `yambs-2.2.1/yambs/dependency/config.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/dependency/github.py` & `yambs-2.2.1/yambs/dependency/github.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/dependency/handlers/types.py` & `yambs-2.2.1/yambs/dependency/handlers/types.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/dependency/handlers/yambs.py` & `yambs-2.2.1/yambs/dependency/handlers/yambs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """
 A module implementing a dependency handler for other yambs projects.
 """
 
 # built-in
 from pathlib import Path
+from typing import Set
 
 # third-party
 import requests
 from vcorelib.io.archive import extractall
-from vcorelib.paths import validate_hex_digest
+from vcorelib.paths import Pathlike, normalize, validate_hex_digest
 
 # internal
+from yambs.config.common import DEFAULT_CONFIG
+from yambs.config.native import load_native
 from yambs.dependency.config import (
     Dependency,
     DependencyData,
     DependencySource,
 )
 from yambs.dependency.github import GithubDependency
 from yambs.dependency.handlers.types import DependencyTask
@@ -109,14 +112,62 @@
     ):
         name_link.unlink(missing_ok=True)
         name_link.symlink_to(dest_dir.name)
 
     return name_link
 
 
+def check_nested_dependencies(
+    config: DependencyData, nested: Set[Dependency]
+) -> None:
+    """
+    Determine if a dependency's configuration specifies additional
+    dependencies. Add them to the provided set if so.
+    """
+
+    for dep in config.get("dependencies", []):
+        nested.add(Dependency.create(dep))
+
+
+def audit_config_load(
+    root: Path,
+    include: Path,
+    static: Path,
+    data: DependencyData,
+    config_path: Pathlike = DEFAULT_CONFIG,
+) -> DependencyData:
+    """
+    Load a dependency's configuration data (from disk if necessary) and
+    return the result.
+    """
+
+    if "dependencies" not in data:
+        config_path = normalize(config_path)
+        path = config_path
+        if not path.is_absolute():
+            path = root.joinpath(path)
+
+        assert path.is_file(), path
+
+        config = load_native(path=path, root=root)
+
+        # Ensure some directory linkages are set up ('static' and 'include').
+        config.third_party_root.mkdir(parents=True, exist_ok=True)
+
+        for source in [include, static]:
+            dest = config.third_party_root.joinpath(source.name)
+            if not dest.is_symlink():
+                dest.symlink_to(source)
+
+        # It's not necessary to keep track of the entire configuration.
+        data["dependencies"] = [x.asdict() for x in config.dependencies]
+
+    return data
+
+
 def yambs_handler(task: DependencyTask) -> DependencyState:
     """Handle a yambs dependency."""
 
     # No other source implementations currently.
     assert task.dep.source == DependencySource.GITHUB
 
     github = github_release(task.dep, task.data)
@@ -145,12 +196,15 @@
     task.link_flags.append(f"-l{task.data['slug']}")
 
     # Ensure the 'src' directory is linked within the include directory.
     src_include = task.include.joinpath(task.data["name"])
     if not src_include.is_symlink():
         src_include.symlink_to(Path("..", task.data["name"], "src"))
 
+    # Check if loading the project configuration data is necessary.
     # Read the project's configuration data to find any nested dependencies.
-    # task.root.joinpath("yambs.yaml"), look for data file?
-    # task.nested.add()
+    check_nested_dependencies(
+        audit_config_load(directory, task.include, task.static, task.data),
+        task.nested,
+    )
 
     return task.current
```

### Comparing `yambs-2.2.0/yambs/dependency/manager.py` & `yambs-2.2.1/yambs/dependency/manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,14 +14,38 @@
 # internal
 from yambs.dependency.config import Dependency, DependencyData
 from yambs.dependency.handlers import HANDLERS
 from yambs.dependency.handlers.types import DependencyTask
 from yambs.dependency.state import DependencyState
 
 
+def write_third_party_script(
+    path: Path, commands: List[List[str]] = None
+) -> None:
+    """
+    Create a simple shell script normally containing instructions to build
+    third-party commands.
+    """
+
+    if commands is None:
+        commands = []
+
+    with path.open("w") as script_fd:
+        script_fd.write("#!/bin/bash\n\n")
+
+        # Add build commands.
+        for command in commands:
+            script_fd.write(" ".join(command))
+            script_fd.write("\n")
+
+        script_fd.write("\ndate > $1\n")
+
+    set_exec_flags(path)
+
+
 class DependencyManager:
     """A class for managing project dependencies."""
 
     def __init__(self, root: Path) -> None:
         """Initialize this instance."""
 
         self.root = root
@@ -39,41 +63,33 @@
         # A list of commands to run that should build dependencies.
         self.build_commands: List[List[str]] = []
 
         # Aggregate compiler flags.
         self.compile_flags = ["-iquote", str(self.include)]
         self.link_flags = [f"-L{self.static}"]
 
+        # Keep track of dependencies that have been handled.
+        self.resolved: Set[Dependency] = set()
+
     def info(self, logger: LoggerType) -> None:
         """Log some information."""
 
         if self.build_commands:
             logger.info("Build commands: %s.", self.build_commands)
         logger.info("Third-party compile flags: %s.", self.compile_flags)
         logger.info("Third-party link flags: %s.", self.link_flags)
 
-    def save(self, logger: LoggerType = None) -> None:
+    def save(self, script: Path, logger: LoggerType = None) -> None:
         """Save state data and create the third-party build script."""
 
         ARBITER.encode(self.state_path, self.state)
         if logger is not None:
             self.info(logger)
 
-        script = self.root.joinpath("third_party.sh")
-        with script.open("w") as script_fd:
-            script_fd.write("#!/bin/bash\n\n")
-
-            # Add build commands.
-            for command in self.build_commands:
-                script_fd.write(" ".join(command))
-                script_fd.write("\n")
-
-            script_fd.write("\ndate > $1\n")
-
-        set_exec_flags(script)
+        write_third_party_script(script, commands=self.build_commands)
 
     def _create_task(self, dep: Dependency) -> DependencyTask:
         """Create a new task object."""
 
         dep_data: DependencyData = self.state.setdefault(
             str(dep),
             {},
@@ -92,26 +108,22 @@
             set(),
         )
 
     def audit(self, dep: Dependency) -> DependencyState:
         """Interact with a dependency if needed."""
 
         tasks = [self._create_task(dep)]
-        resolved: Set[Dependency] = set()
 
         while tasks:
             task = tasks.pop()
             state = HANDLERS[dep.kind](task)
-            resolved.add(task.dep)
+            self.resolved.add(task.dep)
 
             # Update state.
             task.data["state"] = str(state.value)
 
             # Handle any nested dependencies.
-            #
-            # Enable this soon!
-            #
-            # for nested in task.nested:
-            #     if nested not in resolved:
-            #         tasks.append(self._create_task(nested))
+            for nested in task.nested:
+                if nested not in self.resolved:
+                    tasks.append(self._create_task(nested))
 
         return state
```

### Comparing `yambs-2.2.0/yambs/dist/__init__.py` & `yambs-2.2.1/yambs/dist/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/entry.py` & `yambs-2.2.1/yambs/entry.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/environment/__init__.py` & `yambs-2.2.1/yambs/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/environment/native.py` & `yambs-2.2.1/yambs/environment/native.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,17 @@
 
         if not sources_only:
             # Audit dependencies.
             for dep in self.config.dependencies:
                 self.dependency_manager.audit(dep)
 
             # Create build script.
-            self.dependency_manager.save(logger=self.logger)
+            self.dependency_manager.save(
+                self.config.third_party_script, logger=self.logger
+            )
 
             # Handle compile and link flags generated by the third-party pass.
             self.config.data["common_cflags"].extend(
                 self.dependency_manager.compile_flags
             )
             self.config.data["common_ldflags"].extend(
                 self.dependency_manager.link_flags
```

### Comparing `yambs-2.2.0/yambs/generate/__init__.py` & `yambs-2.2.1/yambs/generate/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/generate/architectures.py` & `yambs-2.2.1/yambs/generate/architectures.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/generate/boards.py` & `yambs-2.2.1/yambs/generate/boards.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/generate/chips.py` & `yambs-2.2.1/yambs/generate/chips.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/generate/common.py` & `yambs-2.2.1/yambs/generate/common.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/generate/ninja/__init__.py` & `yambs-2.2.1/yambs/generate/ninja/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/generate/ninja/format.py` & `yambs-2.2.1/yambs/generate/ninja/format.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/generate/toolchains.py` & `yambs-2.2.1/yambs/generate/toolchains.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/generate/variants.py` & `yambs-2.2.1/yambs/generate/variants.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/github/__init__.py` & `yambs-2.2.1/yambs/github/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/schemas.py` & `yambs-2.2.1/yambs/schemas.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/translation/__init__.py` & `yambs-2.2.1/yambs/translation/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs/uf2/__init__.py` & `yambs-2.2.1/yambs/uf2/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.0/yambs.egg-info/PKG-INFO` & `yambs-2.2.1/yambs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 2.2.0
+Version: 2.2.1
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
@@ -18,19 +18,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=9fd78d02f6bd1c0baddfb2fa7ba65d51
+    hash=2f414044223b7b56f2fb2a465aee095e
     =====================================
 -->
 
-# yambs ([2.2.0](https://pypi.org/project/yambs/))
+# yambs ([2.2.1](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-2.2.0/yambs.egg-info/SOURCES.txt` & `yambs-2.2.1/yambs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

