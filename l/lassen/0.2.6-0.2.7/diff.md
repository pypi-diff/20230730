# Comparing `tmp/lassen-0.2.6.tar.gz` & `tmp/lassen-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lassen-0.2.6.tar", max compression
+gzip compressed data, was "lassen-0.2.7.tar", max compression
```

## Comparing `lassen-0.2.6.tar` & `lassen-0.2.7.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0     1071 2023-06-06 18:13:43.336753 lassen-0.2.6/LICENSE
--rw-r--r--   0        0        0     3418 2023-07-23 17:12:41.829570 lassen-0.2.6/README.md
--rw-r--r--   0        0        0        0 2023-06-06 23:14:20.986429 lassen-0.2.6/lassen/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 23:14:20.986933 lassen-0.2.6/lassen/alembic/__init__.py
--rw-r--r--   0        0        0     3685 2023-06-06 23:14:20.987092 lassen-0.2.6/lassen/alembic/cli.py
--rw-r--r--   0        0        0     2839 2023-07-22 17:00:28.388594 lassen-0.2.6/lassen/alembic/io.py
--rw-r--r--   0        0        0     1043 2023-06-06 23:14:20.987305 lassen-0.2.6/lassen/alembic/runner.py
--rw-r--r--   0        0        0      174 2023-06-06 23:14:20.987414 lassen-0.2.6/lassen/assets/__init__.py
--rw-r--r--   0        0        0     1592 2023-06-06 23:14:20.987525 lassen-0.2.6/lassen/assets/alembic.ini
--rw-r--r--   0        0        0      494 2023-06-06 23:14:20.987634 lassen-0.2.6/lassen/assets/script.py.mako
--rw-r--r--   0        0        0        0 2023-06-06 23:14:20.987697 lassen-0.2.6/lassen/core/__init__.py
--rw-r--r--   0        0        0      153 2023-06-15 21:16:27.734730 lassen-0.2.6/lassen/core/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2487 2023-06-15 21:16:27.734981 lassen-0.2.6/lassen/core/__pycache__/config.cpython-310.pyc
--rw-r--r--   0        0        0     1862 2023-06-06 23:14:20.988497 lassen-0.2.6/lassen/core/config.py
--rw-r--r--   0        0        0        0 2023-06-15 21:16:27.735020 lassen-0.2.6/lassen/datasets/__init__.py
--rw-r--r--   0        0        0     2368 2023-06-15 22:39:22.170659 lassen-0.2.6/lassen/datasets/dataset_helpers.py
--rw-r--r--   0        0        0     3024 2023-06-15 22:26:02.922940 lassen-0.2.6/lassen/datasets/pyarrow_schemas.py
--rw-r--r--   0        0        0      240 2023-06-06 23:14:20.988685 lassen-0.2.6/lassen/db/__init__.py
--rw-r--r--   0        0        0      396 2023-06-15 21:16:27.735607 lassen-0.2.6/lassen/db/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      422 2023-07-22 17:00:28.388869 lassen-0.2.6/lassen/db/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      147 2023-06-06 23:14:20.989285 lassen-0.2.6/lassen/db/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0      293 2023-06-06 23:14:20.989436 lassen-0.2.6/lassen/db/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     1931 2023-06-15 21:16:27.735885 lassen-0.2.6/lassen/db/__pycache__/base_class.cpython-310.pyc
--rw-r--r--   0        0        0     2138 2023-07-23 15:46:35.701193 lassen-0.2.6/lassen/db/__pycache__/base_class.cpython-311.pyc
--rw-r--r--   0        0        0      839 2023-06-15 21:16:27.736092 lassen-0.2.6/lassen/db/__pycache__/session.cpython-310.pyc
--rw-r--r--   0        0        0     1296 2023-07-22 17:00:28.389524 lassen-0.2.6/lassen/db/__pycache__/session.cpython-311.pyc
--rw-r--r--   0        0        0     1437 2023-07-23 15:46:28.626071 lassen-0.2.6/lassen/db/base_class.py
--rw-r--r--   0        0        0      627 2023-06-06 23:14:20.990409 lassen-0.2.6/lassen/db/session.py
--rw-r--r--   0        0        0      302 2023-07-29 15:15:21.002859 lassen-0.2.6/lassen/enums.py
--rw-r--r--   0        0        0     1272 2023-07-22 17:00:28.389917 lassen-0.2.6/lassen/io.py
--rw-r--r--   0        0        0        0 2023-07-22 17:05:14.900856 lassen-0.2.6/lassen/py.typed
--rw-r--r--   0        0        0      210 2023-06-06 23:14:20.990522 lassen-0.2.6/lassen/schema.py
--rw-r--r--   0        0        0      227 2023-06-15 21:16:27.736193 lassen-0.2.6/lassen/shared.py
--rw-r--r--   0        0        0    10799 2023-07-29 15:15:21.003191 lassen-0.2.6/lassen/store.py
--rw-r--r--   0        0        0      201 2023-07-22 17:00:28.390303 lassen-0.2.6/lassen/stubs/__init__.py
--rw-r--r--   0        0        0     1294 2023-07-23 15:10:32.421607 lassen-0.2.6/lassen/stubs/base.py
--rw-r--r--   0        0        0      147 2023-07-23 04:25:54.115562 lassen-0.2.6/lassen/stubs/definition.py
--rw-r--r--   0        0        0     2448 2023-07-25 17:26:24.493945 lassen-0.2.6/lassen/stubs/field.py
--rw-r--r--   0        0        0     4086 2023-07-23 17:13:39.305496 lassen-0.2.6/lassen/stubs/generate.py
--rw-r--r--   0        0        0       96 2023-07-22 17:00:28.390790 lassen-0.2.6/lassen/stubs/generators/__init__.py
--rw-r--r--   0        0        0     9321 2023-07-23 17:11:00.299172 lassen-0.2.6/lassen/stubs/generators/common.py
--rw-r--r--   0        0        0     8064 2023-07-25 17:26:24.494192 lassen-0.2.6/lassen/stubs/generators/schema.py
--rw-r--r--   0        0        0    12675 2023-07-29 13:45:40.415095 lassen-0.2.6/lassen/stubs/generators/store.py
--rw-r--r--   0        0        0      177 2023-07-22 17:00:28.391343 lassen-0.2.6/lassen/stubs/templates/__init__.py
--rw-r--r--   0        0        0     1052 2023-07-22 17:00:28.391457 lassen-0.2.6/lassen/stubs/templates/schema.py.j2
--rw-r--r--   0        0        0      591 2023-07-23 15:31:38.606138 lassen-0.2.6/lassen/stubs/templates/sqlalchemy.py.j2
--rw-r--r--   0        0        0        0 2023-06-06 23:14:20.990727 lassen-0.2.6/lassen/tests/__init__.py
--rw-r--r--   0        0        0      154 2023-06-15 21:16:27.736415 lassen-0.2.6/lassen/tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1973 2023-06-15 21:31:07.938752 lassen-0.2.6/lassen/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1220 2023-06-06 23:14:20.991368 lassen-0.2.6/lassen/tests/__pycache__/fixtures.cpython-310.pyc
--rw-r--r--   0        0        0     5734 2023-06-15 21:16:27.736953 lassen-0.2.6/lassen/tests/__pycache__/test_store.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1901 2023-06-15 21:16:27.737091 lassen-0.2.6/lassen/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-06-15 21:16:27.737128 lassen-0.2.6/lassen/tests/datasets/__init__.py
--rw-r--r--   0        0        0     2243 2023-06-15 22:42:38.547093 lassen-0.2.6/lassen/tests/datasets/test_dataset_helpers.py
--rw-r--r--   0        0        0     1645 2023-06-15 22:26:02.923228 lassen-0.2.6/lassen/tests/datasets/test_pyarrow_schemas.py
--rw-r--r--   0        0        0      176 2023-06-06 23:14:20.991801 lassen-0.2.6/lassen/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     1181 2023-07-25 17:26:24.494365 lassen-0.2.6/lassen/tests/fixtures/stubs/expected_schema.py
--rw-r--r--   0        0        0      961 2023-07-25 17:26:24.494521 lassen-0.2.6/lassen/tests/fixtures/stubs/expected_schema_public.py
--rw-r--r--   0        0        0      926 2023-07-23 17:16:21.722018 lassen-0.2.6/lassen/tests/fixtures/stubs/expected_store.py
--rw-r--r--   0        0        0     1134 2023-07-25 17:26:24.494720 lassen-0.2.6/lassen/tests/fixtures/stubs/fixtures.py
--rw-r--r--   0        0        0      463 2023-06-06 23:14:20.991923 lassen-0.2.6/lassen/tests/fixtures/test_harness/README.md
--rw-r--r--   0        0        0      311 2023-06-06 23:14:20.992056 lassen-0.2.6/lassen/tests/fixtures/test_harness/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-06 23:14:20.992112 lassen-0.2.6/lassen/tests/fixtures/test_harness/test_harness/__init__.py
--rw-r--r--   0        0        0      691 2023-06-06 23:14:20.992321 lassen-0.2.6/lassen/tests/fixtures/test_harness/test_harness/migrations/62bf8def9fb1_new_migration.py
--rw-r--r--   0        0        0      653 2023-06-06 23:14:20.992456 lassen-0.2.6/lassen/tests/fixtures/test_harness/test_harness/migrations/96dbf6f6d068_add_name.py
--rw-r--r--   0        0        0      217 2023-06-06 23:14:20.992593 lassen-0.2.6/lassen/tests/fixtures/test_harness/test_harness/models.py
--rw-r--r--   0        0        0      521 2023-07-23 15:10:32.425116 lassen-0.2.6/lassen/tests/model_fixtures.py
--rw-r--r--   0        0        0        0 2023-07-22 17:00:28.392359 lassen-0.2.6/lassen/tests/stubs/__init__.py
--rw-r--r--   0        0        0        0 2023-07-22 17:00:28.392464 lassen-0.2.6/lassen/tests/stubs/generators/__init__.py
--rw-r--r--   0        0        0     3649 2023-07-23 17:15:13.423972 lassen-0.2.6/lassen/tests/stubs/generators/test_common.py
--rw-r--r--   0        0        0     1221 2023-07-23 15:10:32.425828 lassen-0.2.6/lassen/tests/stubs/generators/test_schema.py
--rw-r--r--   0        0        0     3581 2023-07-29 13:45:40.415389 lassen-0.2.6/lassen/tests/stubs/generators/test_store.py
--rw-r--r--   0        0        0     2560 2023-07-22 17:00:28.393152 lassen-0.2.6/lassen/tests/stubs/test_generate.py
--rw-r--r--   0        0        0     2252 2023-06-06 23:14:20.992858 lassen-0.2.6/lassen/tests/test_alembic.py
--rw-r--r--   0        0        0     5422 2023-07-29 15:15:21.003403 lassen-0.2.6/lassen/tests/test_store.py
--rw-r--r--   0        0        0     1423 2023-07-29 15:15:24.937776 lassen-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     5252 1970-01-01 00:00:00.000000 lassen-0.2.6/setup.py
--rw-r--r--   0        0        0     4389 1970-01-01 00:00:00.000000 lassen-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-06 18:13:43.336753 lassen-0.2.7/LICENSE
+-rw-r--r--   0        0        0     3418 2023-07-23 17:12:41.829570 lassen-0.2.7/README.md
+-rw-r--r--   0        0        0        0 2023-06-06 23:14:20.986429 lassen-0.2.7/lassen/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 23:14:20.986933 lassen-0.2.7/lassen/alembic/__init__.py
+-rw-r--r--   0        0        0     3685 2023-06-06 23:14:20.987092 lassen-0.2.7/lassen/alembic/cli.py
+-rw-r--r--   0        0        0     2839 2023-07-22 17:00:28.388594 lassen-0.2.7/lassen/alembic/io.py
+-rw-r--r--   0        0        0     1043 2023-06-06 23:14:20.987305 lassen-0.2.7/lassen/alembic/runner.py
+-rw-r--r--   0        0        0      174 2023-06-06 23:14:20.987414 lassen-0.2.7/lassen/assets/__init__.py
+-rw-r--r--   0        0        0     1592 2023-06-06 23:14:20.987525 lassen-0.2.7/lassen/assets/alembic.ini
+-rw-r--r--   0        0        0      494 2023-06-06 23:14:20.987634 lassen-0.2.7/lassen/assets/script.py.mako
+-rw-r--r--   0        0        0        0 2023-06-06 23:14:20.987697 lassen-0.2.7/lassen/core/__init__.py
+-rw-r--r--   0        0        0      153 2023-06-15 21:16:27.734730 lassen-0.2.7/lassen/core/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2487 2023-06-15 21:16:27.734981 lassen-0.2.7/lassen/core/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0        0        0     1862 2023-06-06 23:14:20.988497 lassen-0.2.7/lassen/core/config.py
+-rw-r--r--   0        0        0        0 2023-06-15 21:16:27.735020 lassen-0.2.7/lassen/datasets/__init__.py
+-rw-r--r--   0        0        0     2368 2023-06-15 22:39:22.170659 lassen-0.2.7/lassen/datasets/dataset_helpers.py
+-rw-r--r--   0        0        0     3024 2023-06-15 22:26:02.922940 lassen-0.2.7/lassen/datasets/pyarrow_schemas.py
+-rw-r--r--   0        0        0      240 2023-06-06 23:14:20.988685 lassen-0.2.7/lassen/db/__init__.py
+-rw-r--r--   0        0        0      396 2023-06-15 21:16:27.735607 lassen-0.2.7/lassen/db/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      422 2023-07-22 17:00:28.388869 lassen-0.2.7/lassen/db/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      147 2023-06-06 23:14:20.989285 lassen-0.2.7/lassen/db/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0      293 2023-06-06 23:14:20.989436 lassen-0.2.7/lassen/db/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     1931 2023-06-15 21:16:27.735885 lassen-0.2.7/lassen/db/__pycache__/base_class.cpython-310.pyc
+-rw-r--r--   0        0        0     2138 2023-07-23 15:46:35.701193 lassen-0.2.7/lassen/db/__pycache__/base_class.cpython-311.pyc
+-rw-r--r--   0        0        0      839 2023-06-15 21:16:27.736092 lassen-0.2.7/lassen/db/__pycache__/session.cpython-310.pyc
+-rw-r--r--   0        0        0     1296 2023-07-22 17:00:28.389524 lassen-0.2.7/lassen/db/__pycache__/session.cpython-311.pyc
+-rw-r--r--   0        0        0     1437 2023-07-23 15:46:28.626071 lassen-0.2.7/lassen/db/base_class.py
+-rw-r--r--   0        0        0      627 2023-06-06 23:14:20.990409 lassen-0.2.7/lassen/db/session.py
+-rw-r--r--   0        0        0      302 2023-07-29 15:15:21.002859 lassen-0.2.7/lassen/enums.py
+-rw-r--r--   0        0        0     1272 2023-07-22 17:00:28.389917 lassen-0.2.7/lassen/io.py
+-rw-r--r--   0        0        0        0 2023-07-22 17:05:14.900856 lassen-0.2.7/lassen/py.typed
+-rw-r--r--   0        0        0      210 2023-06-06 23:14:20.990522 lassen-0.2.7/lassen/schema.py
+-rw-r--r--   0        0        0      227 2023-06-15 21:16:27.736193 lassen-0.2.7/lassen/shared.py
+-rw-r--r--   0        0        0    10799 2023-07-29 15:15:21.003191 lassen-0.2.7/lassen/store.py
+-rw-r--r--   0        0        0      201 2023-07-22 17:00:28.390303 lassen-0.2.7/lassen/stubs/__init__.py
+-rw-r--r--   0        0        0     1294 2023-07-23 15:10:32.421607 lassen-0.2.7/lassen/stubs/base.py
+-rw-r--r--   0        0        0      147 2023-07-23 04:25:54.115562 lassen-0.2.7/lassen/stubs/definition.py
+-rw-r--r--   0        0        0     2448 2023-07-25 17:26:24.493945 lassen-0.2.7/lassen/stubs/field.py
+-rw-r--r--   0        0        0     4856 2023-07-30 15:57:55.862739 lassen-0.2.7/lassen/stubs/generate.py
+-rw-r--r--   0        0        0       96 2023-07-22 17:00:28.390790 lassen-0.2.7/lassen/stubs/generators/__init__.py
+-rw-r--r--   0        0        0     9627 2023-07-30 15:57:55.863156 lassen-0.2.7/lassen/stubs/generators/common.py
+-rw-r--r--   0        0        0     8064 2023-07-25 17:26:24.494192 lassen-0.2.7/lassen/stubs/generators/schema.py
+-rw-r--r--   0        0        0    13343 2023-07-30 15:57:55.863592 lassen-0.2.7/lassen/stubs/generators/store.py
+-rw-r--r--   0        0        0      177 2023-07-22 17:00:28.391343 lassen-0.2.7/lassen/stubs/templates/__init__.py
+-rw-r--r--   0        0        0     1052 2023-07-22 17:00:28.391457 lassen-0.2.7/lassen/stubs/templates/schema.py.j2
+-rw-r--r--   0        0        0      591 2023-07-23 15:31:38.606138 lassen-0.2.7/lassen/stubs/templates/sqlalchemy.py.j2
+-rw-r--r--   0        0        0        0 2023-06-06 23:14:20.990727 lassen-0.2.7/lassen/tests/__init__.py
+-rw-r--r--   0        0        0      154 2023-06-15 21:16:27.736415 lassen-0.2.7/lassen/tests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1973 2023-06-15 21:31:07.938752 lassen-0.2.7/lassen/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1220 2023-06-06 23:14:20.991368 lassen-0.2.7/lassen/tests/__pycache__/fixtures.cpython-310.pyc
+-rw-r--r--   0        0        0     5734 2023-06-15 21:16:27.736953 lassen-0.2.7/lassen/tests/__pycache__/test_store.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1901 2023-06-15 21:16:27.737091 lassen-0.2.7/lassen/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-15 21:16:27.737128 lassen-0.2.7/lassen/tests/datasets/__init__.py
+-rw-r--r--   0        0        0     2243 2023-06-15 22:42:38.547093 lassen-0.2.7/lassen/tests/datasets/test_dataset_helpers.py
+-rw-r--r--   0        0        0     1645 2023-06-15 22:26:02.923228 lassen-0.2.7/lassen/tests/datasets/test_pyarrow_schemas.py
+-rw-r--r--   0        0        0      176 2023-06-06 23:14:20.991801 lassen-0.2.7/lassen/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     1181 2023-07-25 17:26:24.494365 lassen-0.2.7/lassen/tests/fixtures/stubs/expected_schema.py
+-rw-r--r--   0        0        0      961 2023-07-25 17:26:24.494521 lassen-0.2.7/lassen/tests/fixtures/stubs/expected_schema_public.py
+-rw-r--r--   0        0        0      926 2023-07-23 17:16:21.722018 lassen-0.2.7/lassen/tests/fixtures/stubs/expected_store.py
+-rw-r--r--   0        0        0     1134 2023-07-25 17:26:24.494720 lassen-0.2.7/lassen/tests/fixtures/stubs/fixtures.py
+-rw-r--r--   0        0        0      463 2023-06-06 23:14:20.991923 lassen-0.2.7/lassen/tests/fixtures/test_harness/README.md
+-rw-r--r--   0        0        0      311 2023-06-06 23:14:20.992056 lassen-0.2.7/lassen/tests/fixtures/test_harness/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 23:14:20.992112 lassen-0.2.7/lassen/tests/fixtures/test_harness/test_harness/__init__.py
+-rw-r--r--   0        0        0      691 2023-06-06 23:14:20.992321 lassen-0.2.7/lassen/tests/fixtures/test_harness/test_harness/migrations/62bf8def9fb1_new_migration.py
+-rw-r--r--   0        0        0      653 2023-06-06 23:14:20.992456 lassen-0.2.7/lassen/tests/fixtures/test_harness/test_harness/migrations/96dbf6f6d068_add_name.py
+-rw-r--r--   0        0        0      217 2023-06-06 23:14:20.992593 lassen-0.2.7/lassen/tests/fixtures/test_harness/test_harness/models.py
+-rw-r--r--   0        0        0      521 2023-07-23 15:10:32.425116 lassen-0.2.7/lassen/tests/model_fixtures.py
+-rw-r--r--   0        0        0        0 2023-07-22 17:00:28.392359 lassen-0.2.7/lassen/tests/stubs/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-22 17:00:28.392464 lassen-0.2.7/lassen/tests/stubs/generators/__init__.py
+-rw-r--r--   0        0        0     3788 2023-07-30 15:57:55.863980 lassen-0.2.7/lassen/tests/stubs/generators/test_common.py
+-rw-r--r--   0        0        0     1221 2023-07-23 15:10:32.425828 lassen-0.2.7/lassen/tests/stubs/generators/test_schema.py
+-rw-r--r--   0        0        0     3792 2023-07-30 15:57:55.864327 lassen-0.2.7/lassen/tests/stubs/generators/test_store.py
+-rw-r--r--   0        0        0     2560 2023-07-22 17:00:28.393152 lassen-0.2.7/lassen/tests/stubs/test_generate.py
+-rw-r--r--   0        0        0     2252 2023-06-06 23:14:20.992858 lassen-0.2.7/lassen/tests/test_alembic.py
+-rw-r--r--   0        0        0     5422 2023-07-29 15:15:21.003403 lassen-0.2.7/lassen/tests/test_store.py
+-rw-r--r--   0        0        0     1423 2023-07-30 15:58:38.629922 lassen-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     5252 1970-01-01 00:00:00.000000 lassen-0.2.7/setup.py
+-rw-r--r--   0        0        0     4389 1970-01-01 00:00:00.000000 lassen-0.2.7/PKG-INFO
```

### Comparing `lassen-0.2.6/LICENSE` & `lassen-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/README.md` & `lassen-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/alembic/cli.py` & `lassen-0.2.7/lassen/alembic/cli.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/alembic/io.py` & `lassen-0.2.7/lassen/alembic/io.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/alembic/runner.py` & `lassen-0.2.7/lassen/alembic/runner.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/assets/alembic.ini` & `lassen-0.2.7/lassen/assets/alembic.ini`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/core/__pycache__/config.cpython-310.pyc` & `lassen-0.2.7/lassen/core/__pycache__/config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/core/config.py` & `lassen-0.2.7/lassen/core/config.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/datasets/dataset_helpers.py` & `lassen-0.2.7/lassen/datasets/dataset_helpers.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/datasets/pyarrow_schemas.py` & `lassen-0.2.7/lassen/datasets/pyarrow_schemas.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/db/__pycache__/base_class.cpython-310.pyc` & `lassen-0.2.7/lassen/db/__pycache__/base_class.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/db/__pycache__/base_class.cpython-311.pyc` & `lassen-0.2.7/lassen/db/__pycache__/base_class.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/db/__pycache__/session.cpython-310.pyc` & `lassen-0.2.7/lassen/db/__pycache__/session.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/db/__pycache__/session.cpython-311.pyc` & `lassen-0.2.7/lassen/db/__pycache__/session.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/db/base_class.py` & `lassen-0.2.7/lassen/db/base_class.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/db/session.py` & `lassen-0.2.7/lassen/db/session.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/io.py` & `lassen-0.2.7/lassen/io.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/store.py` & `lassen-0.2.7/lassen/store.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/stubs/base.py` & `lassen-0.2.7/lassen/stubs/base.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/stubs/field.py` & `lassen-0.2.7/lassen/stubs/field.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/stubs/generate.py` & `lassen-0.2.7/lassen/stubs/generate.py`

 * *Files 12% similar despite different names*

```diff
@@ -79,43 +79,62 @@
         for file in generator_output.iterdir():
             if file.is_file():
                 file.unlink()
 
         with open(generator_output / "__init__.py", "w") as f:
             f.write("")
 
-    for model, path, generators in model_generators:
-        # Extract the explicit import from the model and its user-defined parents
-        # Skip the lassen-internal base class itself since this won't have any imports
-        # that are relevant to the definitions
-        parent_paths = [
-            Path(inspect.getfile(model))
-            for model in model.__bases__
-            if model != BaseStub
-        ]
-        stub_imports = extract_stub_imports([path] + parent_paths)
+    try:
+        for model, path, generators in model_generators:
+            # Extract the explicit import from the model and its user-defined parents
+            # Skip the lassen-internal base class itself since this won't have any imports
+            # that are relevant to the definitions
+            parent_paths = [
+                Path(inspect.getfile(model))
+                for model in model.__bases__
+                if model != BaseStub
+            ]
+            stub_imports = extract_stub_imports([path] + parent_paths)
+
+            secho(f"Generating files for {model.__name__}")
+
+            for generator in generators:
+                generator_output = root_path / generator.output_directory
+                rendered = generator(model, import_hints=stub_imports)
+                with open(
+                    generator_output / f"{underscore(model.__name__)}.py", "w"
+                ) as f:
+                    f.write(rendered.content)
+
+                with open(generator_output / "__init__.py", "a") as f:
+                    formatted_class_names = ", ".join(rendered.created_classes)
+                    f.write(
+                        f"from .{underscore(model.__name__)} import {formatted_class_names} # noqa: 401\n"
+                    )
+
+            if generators:
+                secho(f"Generated files for {model.__name__}", fg="green")
+            else:
+                secho(f"No generators found for {model.__name__}", fg="yellow")
+    except Exception as e:
+        secho("Exception encountered, cleaning up filesystem...", fg="red")
 
-        secho(f"Generating files for {model.__name__}")
-
-        for generator in generators:
+        for generator in unique_generators:
             generator_output = root_path / generator.output_directory
-            rendered = generator(model, import_hints=stub_imports)
-            with open(generator_output / f"{underscore(model.__name__)}.py", "w") as f:
-                f.write(rendered.content)
-
-            with open(generator_output / "__init__.py", "a") as f:
-                formatted_class_names = ", ".join(rendered.created_classes)
-                f.write(
-                    f"from .{underscore(model.__name__)} import {formatted_class_names} # noqa: 401\n"
-                )
-
-        if generators:
-            secho(f"Generated files for {model.__name__}", fg="green")
-        else:
-            secho(f"No generators found for {model.__name__}", fg="yellow")
+            generator_output.mkdir(parents=True, exist_ok=True)
+
+            # Clear the old files, since the user might have deleted the underlying stubs in the meantime
+            for file in generator_output.iterdir():
+                if file.is_file():
+                    file.unlink()
+
+            with open(generator_output / "__init__.py", "w") as f:
+                f.write("")
+
+        raise e
 
     return [model for model, _ in stub_models]
 
 
 @command()
 def cli():
     generate_files()
```

### Comparing `lassen-0.2.6/lassen/stubs/generators/common.py` & `lassen-0.2.7/lassen/stubs/generators/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import types
 import typing
 from collections import deque
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, Callable, Iterable, get_args, get_origin
 
+import pydantic
+
 from lassen.stubs.base import BaseStub
 
 
 def format_import(cls):
     # Get module of the class
     module = inspect.getmodule(cls)
 
@@ -84,14 +86,21 @@
     if origin is None and not args:
         if isinstance(typehint, str):
             # Forward reference, we assume dependencies are taken care of with the
             # standard import pipline
             return f"'{typehint}'", []
         elif isinstance(typehint, typing.ForwardRef):
             return f"'{typehint.__forward_arg__}'", []
+        elif (
+            inspect.isclass(typehint)
+            and issubclass(typehint, pydantic.BaseModel)
+            and not issubclass(typehint, BaseStub)
+        ):
+            # Support non-stub pydantic schemas
+            return f"{typehint.__name__}", [format_import(typehint)]
         else:
             return typehint.__name__, [format_import(typehint)]
 
     # Handle case for generic types like List, Dict
     if origin is not None or args:
         if origin:
             typehint_name = origin.__name__
```

### Comparing `lassen-0.2.6/lassen/stubs/generators/schema.py` & `lassen-0.2.7/lassen/stubs/generators/schema.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/stubs/generators/store.py` & `lassen-0.2.7/lassen/stubs/generators/store.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import enum
 import inspect
 import types
 import typing
 from datetime import datetime
 from typing import Any, Dict, List, Type, get_args, get_origin
 
+import pydantic
 import sqlalchemy
 import sqlalchemy.ext.associationproxy
 import sqlalchemy.orm
 from inflection import underscore
 from jinja2 import Environment, FileSystemLoader, select_autoescape
 
 from lassen.db.base_class import Base as LassenBase
@@ -232,16 +233,17 @@
         instance_variable: list[tuple[str, Any]] = list(inspect.getmembers(model))
 
         return {id(field): name for name, field in instance_variable}
 
     def format_column_for_sqlalchemy(
         self, typehint: Any
     ) -> tuple[str, Any, list[str | None]]:
+        print("GOT TYPEHINT", typehint)
         if inspect.isclass(typehint) and issubclass(typehint, enum.Enum):
-            enum_handler = self.origin_mapping.get(enum.Enum, sqlalchemy.Enum)
+            enum_handler = self.origin_mapping[enum.Enum]
             return (
                 f"{enum_handler.__name__}({typehint.__name__})",
                 enum_handler(typehint),
                 [format_import(enum_handler)],
             )
         elif inspect.isclass(typehint) and issubclass(typehint, BaseStub):
             return (
@@ -253,33 +255,48 @@
             )
         elif typehint in [int, float, str, bool, datetime, Any]:
             raw_class = self.origin_mapping[typehint]
             return (f"{raw_class.__name__}()", raw_class(), [format_import(raw_class)])
         elif isinstance(typehint, str):
             # Forward reference, assume this is to another class
             return (f"'{typehint}'", typehint, [])
+        elif (
+            inspect.isclass(typehint)
+            and issubclass(typehint, pydantic.BaseModel)
+            and not issubclass(typehint, BaseStub)
+        ):
+            raw_class = self.origin_mapping[Any]
+            return (f"{raw_class.__name__}()", raw_class(), [format_import(raw_class)])
         elif typehint in self.origin_mapping and typehint not in DEFAULT_ORIGIN_MAPPING:
             # User defined typehint for another, unsupported class
             raw_class = self.origin_mapping[typehint]
             return (f"{raw_class.__name__}()", raw_class(), [format_import(raw_class)])
         else:
             origin = get_origin(typehint)
             args = get_args(typehint)
             if origin is list or origin is List:
                 # Verify a homogeneous list
                 unique_args = set(args)
                 if len(unique_args) > 1:
                     raise ValueError("Lists with multiple types are not supported")
-                if args and isinstance(args[0], type):
-                    list_handler = self.origin_mapping.get(list, sqlalchemy.ARRAY)
+                if (
+                    args
+                    and inspect.isclass(args[0])
+                    and issubclass(args[0], pydantic.BaseModel)
+                ):
+                    # If the sub-model is a pydantic value we should format as a regular json blob
+                    return self.format_column_for_sqlalchemy(Any)
+                elif args and isinstance(args[0], type):
+                    list_handler = self.origin_mapping[list]
                     (
                         cast_arg,
                         cast_class_arg,
                         dependencies,
                     ) = self.format_column_for_sqlalchemy(args[0])
+
                     return (
                         f"{list_handler.__name__}({cast_arg})",
                         list_handler(cast_class_arg),
                         [format_import(list_handler), *dependencies],
                     )
             elif origin is dict or origin is Dict:
                 raw_class = self.origin_mapping[dict]
```

### Comparing `lassen-0.2.6/lassen/stubs/templates/schema.py.j2` & `lassen-0.2.7/lassen/stubs/templates/schema.py.j2`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/stubs/templates/sqlalchemy.py.j2` & `lassen-0.2.7/lassen/stubs/templates/sqlalchemy.py.j2`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc` & `lassen-0.2.7/lassen/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/tests/__pycache__/fixtures.cpython-310.pyc` & `lassen-0.2.7/lassen/tests/__pycache__/fixtures.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/tests/__pycache__/test_store.cpython-310-pytest-7.3.1.pyc` & `lassen-0.2.7/lassen/tests/__pycache__/test_store.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/tests/conftest.py` & `lassen-0.2.7/lassen/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/tests/datasets/test_dataset_helpers.py` & `lassen-0.2.7/lassen/tests/datasets/test_dataset_helpers.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/tests/datasets/test_pyarrow_schemas.py` & `lassen-0.2.7/lassen/tests/datasets/test_pyarrow_schemas.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/tests/fixtures/stubs/expected_schema.py` & `lassen-0.2.7/lassen/tests/fixtures/stubs/expected_schema.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/tests/fixtures/stubs/expected_schema_public.py` & `lassen-0.2.7/lassen/tests/fixtures/stubs/expected_schema_public.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/tests/fixtures/stubs/expected_store.py` & `lassen-0.2.7/lassen/tests/fixtures/stubs/expected_store.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/tests/fixtures/stubs/fixtures.py` & `lassen-0.2.7/lassen/tests/fixtures/stubs/fixtures.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/tests/fixtures/test_harness/test_harness/migrations/62bf8def9fb1_new_migration.py` & `lassen-0.2.7/lassen/tests/fixtures/test_harness/test_harness/migrations/62bf8def9fb1_new_migration.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/tests/fixtures/test_harness/test_harness/migrations/96dbf6f6d068_add_name.py` & `lassen-0.2.7/lassen/tests/fixtures/test_harness/test_harness/migrations/96dbf6f6d068_add_name.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/tests/model_fixtures.py` & `lassen-0.2.7/lassen/tests/model_fixtures.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/tests/stubs/generators/test_common.py` & `lassen-0.2.7/lassen/tests/stubs/generators/test_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from datetime import datetime
 from enum import Enum
 from pathlib import Path
 from typing import Any, Callable, Dict, List
 
 import pytest
+from pydantic import BaseModel
 
 from lassen.stubs.generators.common import (
     extract_stub_imports,
     format_dict_as_kwargs,
     format_typehint_as_string,
     get_lambda_body,
     get_ordered_instance_variables,
@@ -16,25 +17,30 @@
 from lassen.tests.fixtures import get_fixture_path
 
 
 class SimpleEnum(Enum):
     TEST = "TEST"
 
 
+class SimplePydanticModel(BaseModel):
+    TEST: str
+
+
 @pytest.mark.parametrize(
     "typehint, expected",
     [
         (int, "int"),
         (float, "float"),
         (SimpleEnum, "SimpleEnum"),
         (list[str], "list[str]"),
         (str | None, "Union[str, None]"),
         (List[str], "list[str]"),
         (Dict[str, str], "dict[str, str]"),
         (dict[str, str], "dict[str, str]"),
+        (SimplePydanticModel, "SimplePydanticModel"),
     ],
 )
 def test_format_typehint_as_string(typehint, expected):
     formatted_typehint, dependencies = format_typehint_as_string(typehint)
     assert formatted_typehint == expected
     assert len(dependencies) > 0
```

### Comparing `lassen-0.2.6/lassen/tests/stubs/generators/test_schema.py` & `lassen-0.2.7/lassen/tests/stubs/generators/test_schema.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/tests/stubs/generators/test_store.py` & `lassen-0.2.7/lassen/tests/stubs/generators/test_store.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 import datetime
 from enum import Enum
 from typing import Any, Dict, List
 
 import pytest
 import sqlalchemy
+from pydantic import BaseModel
 
 from lassen.stubs.base import BaseStub
 from lassen.stubs.definition import UniqueDefinition
 from lassen.stubs.field import Field
 from lassen.stubs.generators.common import ExtractedStubImports
 from lassen.stubs.generators.store import DEFAULT_ORIGIN_MAPPING, StoreGenerator
 
 
 class SimpleEnum(Enum):
     TEST = "TEST"
 
 
+class SimplePydanticModel(BaseModel):
+    TEST: str
+
+
 @pytest.mark.parametrize(
     "typehint, expected_str, expected_class",
     [
         (int, "Integer()", sqlalchemy.Integer()),
         (float, "Float()", sqlalchemy.Float()),
         (SimpleEnum, "Enum(SimpleEnum)", sqlalchemy.Enum(SimpleEnum)),
         (list[str], "ARRAY(String())", sqlalchemy.ARRAY(sqlalchemy.String())),
         (List[str], "ARRAY(String())", sqlalchemy.ARRAY(sqlalchemy.String())),
         (str | None, "String()", sqlalchemy.String()),
         (Any, "JSON()", sqlalchemy.JSON()),
         (dict[str, str], "JSON()", sqlalchemy.JSON()),
         (Dict[str, str], "JSON()", sqlalchemy.JSON()),
+        (SimplePydanticModel, "JSON()", sqlalchemy.JSON()),
+        (list[SimplePydanticModel], "JSON()", sqlalchemy.JSON()),
     ],
 )
 def test_format_column_for_sqlalchemy(typehint, expected_str, expected_class):
     store_generator = StoreGenerator("test")
     (
         formatted_column,
         class_value,
```

### Comparing `lassen-0.2.6/lassen/tests/stubs/test_generate.py` & `lassen-0.2.7/lassen/tests/stubs/test_generate.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/tests/test_alembic.py` & `lassen-0.2.7/lassen/tests/test_alembic.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/lassen/tests/test_store.py` & `lassen-0.2.7/lassen/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `lassen-0.2.6/pyproject.toml` & `lassen-0.2.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lassen"
-version = "0.2.6"
+version = "0.2.7"
 description = "Common webapp scaffolding."
 authors = ["Pierce Freeman <pierce@freeman.vc>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 fastapi = "^0.99.0"
```

### Comparing `lassen-0.2.6/setup.py` & `lassen-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 entry_points = \
 {'console_scripts': ['generate-lassen = lassen.stubs.generate:cli',
                      'migrate = lassen.alembic.cli:main']}
 
 setup_kwargs = {
     'name': 'lassen',
-    'version': '0.2.6',
+    'version': '0.2.7',
     'description': 'Common webapp scaffolding.',
     'long_description': '# lassen\n\n**40.4881° N, 121.5049° W**\n\nCore utilities for MonkeySee web applications.\n\nNot guaranteed to be backwards compatible, use at your own risk.\n\n## Structure\n\n**Stores:** Each datamodel is expected to have its own store. Base classes that provide standard logic are provided by `lassen.store`\n- StoreBase: Base class for all stores\n- StoreFilterMixin: Mixin for filtering stores that specify an additional schema to use to filter\n\n**Schemas:** Each datamodel should define a Model class (SQLAlchemy base object) and a series of Schema objects (Pydantic) that allow the Store to serialize the models. These schemas are also often used for direct CRUD referencing in the API layer.\n\nWe use a base `Stub` file to generate these schemas from a centralized definition. When defining generators you should use a path that can be fully managed by lassen, since we will remove and regenerate these files on each run.\n\n```python\nSTORE_GENERATOR = StoreGenerator("models/auto")\nSCHEMA_GENERATOR = SchemaGenerator("schemas/auto")\n```\n\n```bash\npoetry run generate-lassen\n```\n\n**Datasets:** Optional huggingface `datasets` processing utilities. Only installed under the `lassen[datasets]` extra. These provide support for:\n\n- batch_to_examples: Iterate and manipulate each example separately, versus over nested key-based lists.\n- examples_to_batch: Takes the output of a typehinted element-wise batch and converts into the format needed for dataset insertion. If datasets can\'t automatically interpret the type of the fields, also provide automatic casting based on the typehinted dataclass.\n\n```python\nfrom lassen.datasets import batch_to_examples, examples_to_batch\nimport pandas as pd\n\n@dataclass\nclass BatchInsertion:\n    texts: list[str]\n\ndef batch_process(examples):\n    new_examples : list[BatchInsertion] = []\n    for example in batch_to_examples(examples):\n        new_examples.append(\n            BatchInsertion(\n                example["raw_text"].split()\n            )\n        )\n\n    # datasets won\'t be able to typehint a dataset that starts with an empty example, so we use our explicit schema to cast the data\n    return examples_to_batch(new_examples, BatchInsertion, explicit_schema=True)\n\ndf = pd.DataFrame(\n    [\n        {"raw_text": ""},\n        {"raw_text": "This is a test"},\n        {"raw_text": "This is another test"},\n    ]\n)\n\ndataset = Dataset.from_pandas(df)\n\ndataset = dataset.map(\n    batch_process,\n    batched=True,\n    batch_size=1,\n    num_proc=1,\n    remove_columns=dataset.column_names,\n)\n```\n\n**Migrations:** Lassen includes a templated alembic.init and env.py file. Client applications just need to have a `migrations` folder within their project root. After this you can swap `poetry run alembic` with `poetry run migrate`.\n\n```sh\npoetry run migrate upgrade head\n```\n\n**Settings:** Application settings should subclass our core settings. This provides a standard way to load settings from environment variables and includes common database keys.\n\n```python\nfrom lassen.core.config import CoreSettings, register_settings\n\n@register_settings\nclass ClientSettings(CoreSettings):\n    pass\n```\n\n**Schemas:** For helper schemas when returning results via API, see [lassen.schema](./lassen/schema.py).\n\n## Development\n\n```sh\npoetry install --extras "datasets"\n\ncreateuser lassen\ncreatedb -O lassen lassen_db\ncreatedb -O lassen lassen_test_db\n```\n\nUnit Tests:\n\n```sh\npoetry run pytest\n```\n',
     'author': 'Pierce Freeman',
     'author_email': 'pierce@freeman.vc',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `lassen-0.2.6/PKG-INFO` & `lassen-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lassen
-Version: 0.2.6
+Version: 0.2.7
 Summary: Common webapp scaffolding.
 Author: Pierce Freeman
 Author-email: pierce@freeman.vc
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: database
 Provides-Extra: datasets
```

