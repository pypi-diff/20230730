# Comparing `tmp/dagshub-0.3.0.post4.tar.gz` & `tmp/dagshub-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagshub-0.3.0.post4.tar", last modified: Wed Jul 26 12:44:52 2023, max compression
+gzip compressed data, was "dagshub-0.3.1.tar", last modified: Sun Jul 30 12:22:18 2023, max compression
```

## Comparing `dagshub-0.3.0.post4.tar` & `dagshub-0.3.1.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.552173 dagshub-0.3.0.post4/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-26 12:44:52.552173 dagshub-0.3.0.post4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.528173 dagshub-0.3.0.post4/dagshub/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.532173 dagshub-0.3.0.post4/dagshub/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/auth/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/auth/token_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/auth/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.532173 dagshub-0.3.0.post4/dagshub/common/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/common/analytics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.532173 dagshub-0.3.0.post4/dagshub/common/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/common/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11947 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/common/api/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/common/api/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/common/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/common/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/common/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/common/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/common/init.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/common/logging_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/common/rich_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/common/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.532173 dagshub-0.3.0.post4/dagshub/data_engine/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.536173 dagshub-0.3.0.post4/dagshub/data_engine/annotation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/annotation/voxel_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.536173 dagshub-0.3.0.post4/dagshub/data_engine/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/client/data_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/client/gql_mutations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/client/gql_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.536173 dagshub-0.3.0.post4/dagshub/data_engine/client/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/client/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/client/loaders/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/client/loaders/tf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/client/loaders/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/client/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.536173 dagshub-0.3.0.post4/dagshub/data_engine/client/query_builder/
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/client/query_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/datasources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.540173 dagshub-0.3.0.post4/dagshub/data_engine/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/model/datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    26149 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/model/datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/model/datasource_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/model/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/model/query.py
--rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/model/query_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.540173 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.524173 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.540173 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.540173 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    42241 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/dagshub.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.540173 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/
--rw-r--r--   0 runner    (1001) docker     (123)   180750 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/index.umd.js
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/fiftyone.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.544173 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/routes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/routes/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/routes/datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/routes/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/routes/voxel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.544173 dagshub-0.3.0.post4/dagshub/fastai/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/fastai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/fastai/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.544173 dagshub-0.3.0.post4/dagshub/keras/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/keras/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/notebook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.544173 dagshub-0.3.0.post4/dagshub/pytorch_lightning/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/pytorch_lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/pytorch_lightning/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/pytorch_lightning/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.548173 dagshub-0.3.0.post4/dagshub/streaming/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/streaming/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/streaming/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    39148 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/streaming/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/streaming/mount.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.552173 dagshub-0.3.0.post4/dagshub/upload/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/upload/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    25355 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/upload/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.528173 dagshub-0.3.0.post4/dagshub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-26 12:44:52.000000 dagshub-0.3.0.post4/dagshub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-26 12:44:52.000000 dagshub-0.3.0.post4/dagshub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:44:52.000000 dagshub-0.3.0.post4/dagshub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-26 12:44:52.000000 dagshub-0.3.0.post4/dagshub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-26 12:44:52.000000 dagshub-0.3.0.post4/dagshub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-26 12:44:52.000000 dagshub-0.3.0.post4/dagshub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 12:44:52.552173 dagshub-0.3.0.post4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.552173 dagshub-0.3.0.post4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/tests/test_dagshub_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/tests/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:22:18.641880 dagshub-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-30 12:22:09.000000 dagshub-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-30 12:22:09.000000 dagshub-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8669 2023-07-30 12:22:18.641880 dagshub-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-07-30 12:22:09.000000 dagshub-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:22:18.625880 dagshub-0.3.1/dagshub/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:22:18.625880 dagshub-0.3.1/dagshub/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/auth/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/auth/token_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/auth/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:22:18.629880 dagshub-0.3.1/dagshub/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/common/analytics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:22:18.629880 dagshub-0.3.1/dagshub/common/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/common/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11947 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/common/api/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/common/api/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/common/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/common/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/common/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/common/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/common/logging_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/common/rich_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/common/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:22:18.629880 dagshub-0.3.1/dagshub/data_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:22:18.629880 dagshub-0.3.1/dagshub/data_engine/annotation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/annotation/voxel_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:22:18.633880 dagshub-0.3.1/dagshub/data_engine/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/client/data_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/client/gql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/client/gql_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:22:18.633880 dagshub-0.3.1/dagshub/data_engine/client/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/client/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/client/loaders/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/client/loaders/tf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/client/loaders/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/client/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:22:18.633880 dagshub-0.3.1/dagshub/data_engine/client/query_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/client/query_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/datasources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:22:18.633880 dagshub-0.3.1/dagshub/data_engine/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/model/datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26149 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/model/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/model/datasource_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/model/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/model/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/model/query_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:22:18.637880 dagshub-0.3.1/dagshub/data_engine/voxel_plugin_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/voxel_plugin_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/voxel_plugin_server/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/voxel_plugin_server/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:22:18.621880 dagshub-0.3.1/dagshub/data_engine/voxel_plugin_server/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:22:18.637880 dagshub-0.3.1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:22:18.637880 dagshub-0.3.1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    42241 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/dagshub.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:22:18.637880 dagshub-0.3.1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)   180750 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/index.umd.js
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/fiftyone.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:22:18.637880 dagshub-0.3.1/dagshub/data_engine/voxel_plugin_server/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/voxel_plugin_server/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/voxel_plugin_server/routes/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/voxel_plugin_server/routes/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/voxel_plugin_server/routes/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/voxel_plugin_server/routes/voxel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/voxel_plugin_server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/data_engine/voxel_plugin_server/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:22:18.637880 dagshub-0.3.1/dagshub/fastai/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/fastai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/fastai/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:22:18.637880 dagshub-0.3.1/dagshub/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/keras/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/notebook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:22:18.641880 dagshub-0.3.1/dagshub/pytorch_lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/pytorch_lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/pytorch_lightning/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/pytorch_lightning/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:22:18.641880 dagshub-0.3.1/dagshub/streaming/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/streaming/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/streaming/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39148 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/streaming/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/streaming/mount.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:22:18.641880 dagshub-0.3.1/dagshub/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/upload/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25349 2023-07-30 12:22:09.000000 dagshub-0.3.1/dagshub/upload/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:22:18.625880 dagshub-0.3.1/dagshub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8669 2023-07-30 12:22:18.000000 dagshub-0.3.1/dagshub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-30 12:22:18.000000 dagshub-0.3.1/dagshub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 12:22:18.000000 dagshub-0.3.1/dagshub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-30 12:22:18.000000 dagshub-0.3.1/dagshub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-30 12:22:18.000000 dagshub-0.3.1/dagshub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-30 12:22:18.000000 dagshub-0.3.1/dagshub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 12:22:18.641880 dagshub-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-30 12:22:09.000000 dagshub-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:22:18.641880 dagshub-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-30 12:22:09.000000 dagshub-0.3.1/tests/test_dagshub_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-30 12:22:09.000000 dagshub-0.3.1/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-30 12:22:09.000000 dagshub-0.3.1/tests/test_misc.py
```

### Comparing `dagshub-0.3.0.post4/LICENSE` & `dagshub-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/PKG-INFO` & `dagshub-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagshub
-Version: 0.3.0.post4
+Version: 0.3.1
 Summary: DagsHub client libraries
 Home-page: https://github.com/DagsHub/client
 Author: DagsHub
 Author-email: contact@dagshub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -53,15 +53,15 @@
 
 For more details on the different functions of the client, check out the docs segments:
 1. [Installation & Setup](https://github.com/DagsHub/client/blob/master/docs/index.md#installation-and-setup)
 2. [Data Streaming](https://github.com/DagsHub/client/blob/master/docs/index.md#data-streaming)
 3. [Data Upload](https://github.com/DagsHub/client/blob/master/docs/index.md#data-upload)
 4. [Experiment Tracking](https://github.com/DagsHub/client/blob/master/docs/index.md#experiment-tracking-logger)
     1. [Autologging](https://github.com/DagsHub/client/blob/master/docs/index.md#autologging-integrations-with-ml-frameworks)
-5. [Data Engine](https://github.com/DagsHub/client/blob/master/docs/data_engine.md)
+5. [Data Engine](https://github.com/DagsHub/client/blob/master/docs/data_engine.md) 
 
 Some functionality is supported only in Python.
 
 To read about some of the awesome use cases for Direct Data Access, check out
 the [relevant doc page](https://dagshub.com/docs/feature_guide/direct_data_access/#use-cases).
 
 ## Installation
@@ -91,13 +91,8 @@
 
 ## Next Steps
 You can dive into the expanded [documentation](docs/index.md), to learn more about data streaming, data upload and
 experiment tracking with DagsHub
 
 ---
 
-
-### Analytics
-To improve your experience, we collect analytics on client usage. If you want to disable analytics collection,
-set the `DAGSHUB_DISABLE_ANALYTICS` environment variable to any value.
-
 Made with 🐶 by [DagsHub](https://dagshub.com/).
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: dagshub Version: 0.3.0.post4 Summary: DagsHub
-client libraries Home-page: https://github.com/DagsHub/client Author: DagsHub
-Author-email: contact@dagshub.com Classifier: Programming Language :: Python ::
-3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
-System :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
+Metadata-Version: 2.1 Name: dagshub Version: 0.3.1 Summary: DagsHub client
+libraries Home-page: https://github.com/DagsHub/client Author: DagsHub Author-
+email: contact@dagshub.com Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE [![DagsHub Client](https://github.com/DagsHub/
 client/raw/master/dagshub_github.png)](https://dagshub.com)
    **** ð Launching Streaming and Upload of DVC versioned Data ð ****
 
 [![Tests](https://github.com/dagshub/client/actions/workflows/python-
 package.yml/badge.svg?branch=master)](https://github.com/DAGsHub/client/
 actions/workflows/python-package.yml) [![pip](https://img.shields.io/pypi/v/
@@ -66,11 +66,8 @@
 install_hooks install_hooks() ``` 3. Thatâs it! You now have streaming access
 to all your project files. **ð¤© Check out this colab to see an example of
 this Data Streaming work end to end:** [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1CtBmcDtZnxZKVIhNvPagX-8UFWHZ5HAg?usp=sharing)
 ## Next Steps You can dive into the expanded [documentation](docs/index.md), to
 learn more about data streaming, data upload and experiment tracking with
-DagsHub --- ### Analytics To improve your experience, we collect analytics on
-client usage. If you want to disable analytics collection, set the
-`DAGSHUB_DISABLE_ANALYTICS` environment variable to any value. Made with ð¶
-by [DagsHub](https://dagshub.com/).
+DagsHub --- Made with ð¶ by [DagsHub](https://dagshub.com/).
```

### Comparing `dagshub-0.3.0.post4/README.md` & `dagshub-0.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 For more details on the different functions of the client, check out the docs segments:
 1. [Installation & Setup](https://github.com/DagsHub/client/blob/master/docs/index.md#installation-and-setup)
 2. [Data Streaming](https://github.com/DagsHub/client/blob/master/docs/index.md#data-streaming)
 3. [Data Upload](https://github.com/DagsHub/client/blob/master/docs/index.md#data-upload)
 4. [Experiment Tracking](https://github.com/DagsHub/client/blob/master/docs/index.md#experiment-tracking-logger)
     1. [Autologging](https://github.com/DagsHub/client/blob/master/docs/index.md#autologging-integrations-with-ml-frameworks)
-5. [Data Engine](https://github.com/DagsHub/client/blob/master/docs/data_engine.md)
+5. [Data Engine](https://github.com/DagsHub/client/blob/master/docs/data_engine.md) 
 
 Some functionality is supported only in Python.
 
 To read about some of the awesome use cases for Direct Data Access, check out
 the [relevant doc page](https://dagshub.com/docs/feature_guide/direct_data_access/#use-cases).
 
 ## Installation
@@ -77,13 +77,8 @@
 
 ## Next Steps
 You can dive into the expanded [documentation](docs/index.md), to learn more about data streaming, data upload and
 experiment tracking with DagsHub
 
 ---
 
-
-### Analytics
-To improve your experience, we collect analytics on client usage. If you want to disable analytics collection,
-set the `DAGSHUB_DISABLE_ANALYTICS` environment variable to any value.
-
 Made with 🐶 by [DagsHub](https://dagshub.com/).
```

#### html2text {}

```diff
@@ -61,11 +61,8 @@
 install_hooks install_hooks() ``` 3. Thatâs it! You now have streaming access
 to all your project files. **ð¤© Check out this colab to see an example of
 this Data Streaming work end to end:** [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1CtBmcDtZnxZKVIhNvPagX-8UFWHZ5HAg?usp=sharing)
 ## Next Steps You can dive into the expanded [documentation](docs/index.md), to
 learn more about data streaming, data upload and experiment tracking with
-DagsHub --- ### Analytics To improve your experience, we collect analytics on
-client usage. If you want to disable analytics collection, set the
-`DAGSHUB_DISABLE_ANALYTICS` environment variable to any value. Made with ð¶
-by [DagsHub](https://dagshub.com/).
+DagsHub --- Made with ð¶ by [DagsHub](https://dagshub.com/).
```

### Comparing `dagshub-0.3.0.post4/dagshub/auth/oauth.py` & `dagshub-0.3.1/dagshub/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/auth/token_auth.py` & `dagshub-0.3.1/dagshub/auth/token_auth.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/auth/tokens.py` & `dagshub-0.3.1/dagshub/auth/tokens.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/common/analytics.py` & `dagshub-0.3.1/dagshub/common/analytics.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,17 +15,17 @@
         event_data = {}
     event_data["event"] = event_name
     if repo is not None:
         if type(repo) is int:
             event_data["repo_id"] = repo
         else:
             event_data["repo_id"] = repo.id
-    host = config.host
-    token = config.token or get_token(host=host)
-    t = Thread(target=_send, args=(event_data, host, token), daemon=True)
+    t = Thread(target=_send, args=(event_data,), daemon=True)
     t.start()
 
 
-def _send(event_data: Dict[str, Any], host: str, token: str):
+def _send(event_data: Dict[str, Any]):
+    host = config.host
+    token = config.token or get_token(host=host)
     url = f"{host}/api/internal/trackAnalyticsEvent"
 
     http_request("POST", url, data=event_data, auth=HTTPBearerAuth(token))
```

### Comparing `dagshub-0.3.0.post4/dagshub/common/api/repo.py` & `dagshub-0.3.1/dagshub/common/api/repo.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/common/api/responses.py` & `dagshub-0.3.1/dagshub/common/api/responses.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/common/cli.py` & `dagshub-0.3.1/dagshub/common/cli.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/common/config.py` & `dagshub-0.3.1/dagshub/common/config.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/common/download.py` & `dagshub-0.3.1/dagshub/common/download.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/common/helpers.py` & `dagshub-0.3.1/dagshub/common/helpers.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/common/init.py` & `dagshub-0.3.1/dagshub/common/init.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/common/logging_util.py` & `dagshub-0.3.1/dagshub/common/logging_util.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/common/util.py` & `dagshub-0.3.1/dagshub/common/util.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/data_engine/annotation/voxel_conversion.py` & `dagshub-0.3.1/dagshub/data_engine/annotation/voxel_conversion.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/data_engine/client/data_client.py` & `dagshub-0.3.1/dagshub/data_engine/client/data_client.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/data_engine/client/gql_mutations.py` & `dagshub-0.3.1/dagshub/data_engine/client/gql_mutations.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/data_engine/client/gql_queries.py` & `dagshub-0.3.1/dagshub/data_engine/client/gql_queries.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/data_engine/client/loaders/base.py` & `dagshub-0.3.1/dagshub/data_engine/client/loaders/base.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/data_engine/client/loaders/tf.py` & `dagshub-0.3.1/dagshub/data_engine/client/loaders/tf.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/data_engine/client/loaders/torch.py` & `dagshub-0.3.1/dagshub/data_engine/client/loaders/torch.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/data_engine/client/models.py` & `dagshub-0.3.1/dagshub/data_engine/client/models.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/data_engine/client/query_builder/__init__.py` & `dagshub-0.3.1/dagshub/data_engine/client/query_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/data_engine/datasets.py` & `dagshub-0.3.1/dagshub/data_engine/datasets.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/data_engine/datasources.py` & `dagshub-0.3.1/dagshub/data_engine/datasources.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/data_engine/model/datapoint.py` & `dagshub-0.3.1/dagshub/data_engine/model/datapoint.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/data_engine/model/datasource.py` & `dagshub-0.3.1/dagshub/data_engine/model/datasource.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/data_engine/model/datasource_state.py` & `dagshub-0.3.1/dagshub/data_engine/model/datasource_state.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/data_engine/model/errors.py` & `dagshub-0.3.1/dagshub/data_engine/model/errors.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/data_engine/model/query.py` & `dagshub-0.3.1/dagshub/data_engine/model/query.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/data_engine/model/query_result.py` & `dagshub-0.3.1/dagshub/data_engine/model/query_result.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/app.py` & `dagshub-0.3.1/dagshub/data_engine/voxel_plugin_server/app.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/models.py` & `dagshub-0.3.1/dagshub/data_engine/voxel_plugin_server/models.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/dagshub.svg` & `dagshub-0.3.1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/dagshub.svg`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/index.umd.js` & `dagshub-0.3.1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/index.umd.js`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/routes/annotation.py` & `dagshub-0.3.1/dagshub/data_engine/voxel_plugin_server/routes/annotation.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/routes/datasource.py` & `dagshub-0.3.1/dagshub/data_engine/voxel_plugin_server/routes/datasource.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/routes/util.py` & `dagshub-0.3.1/dagshub/data_engine/voxel_plugin_server/routes/util.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/routes/voxel.py` & `dagshub-0.3.1/dagshub/data_engine/voxel_plugin_server/routes/voxel.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/server.py` & `dagshub-0.3.1/dagshub/data_engine/voxel_plugin_server/server.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/utils.py` & `dagshub-0.3.1/dagshub/data_engine/voxel_plugin_server/utils.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/fastai/logger.py` & `dagshub-0.3.1/dagshub/fastai/logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/keras/logger.py` & `dagshub-0.3.1/dagshub/keras/logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/logger.py` & `dagshub-0.3.1/dagshub/logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/notebook.py` & `dagshub-0.3.1/dagshub/notebook.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/pytorch_lightning/logger.py` & `dagshub-0.3.1/dagshub/pytorch_lightning/logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/streaming/dataclasses.py` & `dagshub-0.3.1/dagshub/streaming/dataclasses.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/streaming/filesystem.py` & `dagshub-0.3.1/dagshub/streaming/filesystem.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/streaming/mount.py` & `dagshub-0.3.1/dagshub/streaming/mount.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/upload/errors.py` & `dagshub-0.3.1/dagshub/upload/errors.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/dagshub/upload/wrapper.py` & `dagshub-0.3.1/dagshub/upload/wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,17 +286,17 @@
         if new_branch is not None:
             data.update(
                 {
                     "commit_choice": "commit-to-new-branch",
                     "new_branch_name": new_branch,
                 }
             )
-        # elif self._api.is_mirror:
-        #     # If not uploading to a new branch, and we're in a mirror - wait for the sync to complete
-        #     self._poll_mirror_up_to_date()
+        elif self._api.is_mirror:
+            # If not uploading to a new branch, and we're in a mirror - wait for the sync to complete
+            self._poll_mirror_up_to_date()
 
         if force:
             data["last_commit"] = self._api.last_commit_sha(self.branch)
 
         log_message(f'Uploading files ({len(files)}) to "{self._api.full_name}"...', logger)
         res = s.put(
             self.get_request_url(directory_path),
```

### Comparing `dagshub-0.3.0.post4/dagshub.egg-info/PKG-INFO` & `dagshub-0.3.1/dagshub.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagshub
-Version: 0.3.0.post4
+Version: 0.3.1
 Summary: DagsHub client libraries
 Home-page: https://github.com/DagsHub/client
 Author: DagsHub
 Author-email: contact@dagshub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -53,15 +53,15 @@
 
 For more details on the different functions of the client, check out the docs segments:
 1. [Installation & Setup](https://github.com/DagsHub/client/blob/master/docs/index.md#installation-and-setup)
 2. [Data Streaming](https://github.com/DagsHub/client/blob/master/docs/index.md#data-streaming)
 3. [Data Upload](https://github.com/DagsHub/client/blob/master/docs/index.md#data-upload)
 4. [Experiment Tracking](https://github.com/DagsHub/client/blob/master/docs/index.md#experiment-tracking-logger)
     1. [Autologging](https://github.com/DagsHub/client/blob/master/docs/index.md#autologging-integrations-with-ml-frameworks)
-5. [Data Engine](https://github.com/DagsHub/client/blob/master/docs/data_engine.md)
+5. [Data Engine](https://github.com/DagsHub/client/blob/master/docs/data_engine.md) 
 
 Some functionality is supported only in Python.
 
 To read about some of the awesome use cases for Direct Data Access, check out
 the [relevant doc page](https://dagshub.com/docs/feature_guide/direct_data_access/#use-cases).
 
 ## Installation
@@ -91,13 +91,8 @@
 
 ## Next Steps
 You can dive into the expanded [documentation](docs/index.md), to learn more about data streaming, data upload and
 experiment tracking with DagsHub
 
 ---
 
-
-### Analytics
-To improve your experience, we collect analytics on client usage. If you want to disable analytics collection,
-set the `DAGSHUB_DISABLE_ANALYTICS` environment variable to any value.
-
 Made with 🐶 by [DagsHub](https://dagshub.com/).
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: dagshub Version: 0.3.0.post4 Summary: DagsHub
-client libraries Home-page: https://github.com/DagsHub/client Author: DagsHub
-Author-email: contact@dagshub.com Classifier: Programming Language :: Python ::
-3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
-System :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
+Metadata-Version: 2.1 Name: dagshub Version: 0.3.1 Summary: DagsHub client
+libraries Home-page: https://github.com/DagsHub/client Author: DagsHub Author-
+email: contact@dagshub.com Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE [![DagsHub Client](https://github.com/DagsHub/
 client/raw/master/dagshub_github.png)](https://dagshub.com)
    **** ð Launching Streaming and Upload of DVC versioned Data ð ****
 
 [![Tests](https://github.com/dagshub/client/actions/workflows/python-
 package.yml/badge.svg?branch=master)](https://github.com/DAGsHub/client/
 actions/workflows/python-package.yml) [![pip](https://img.shields.io/pypi/v/
@@ -66,11 +66,8 @@
 install_hooks install_hooks() ``` 3. Thatâs it! You now have streaming access
 to all your project files. **ð¤© Check out this colab to see an example of
 this Data Streaming work end to end:** [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1CtBmcDtZnxZKVIhNvPagX-8UFWHZ5HAg?usp=sharing)
 ## Next Steps You can dive into the expanded [documentation](docs/index.md), to
 learn more about data streaming, data upload and experiment tracking with
-DagsHub --- ### Analytics To improve your experience, we collect analytics on
-client usage. If you want to disable analytics collection, set the
-`DAGSHUB_DISABLE_ANALYTICS` environment variable to any value. Made with ð¶
-by [DagsHub](https://dagshub.com/).
+DagsHub --- Made with ð¶ by [DagsHub](https://dagshub.com/).
```

### Comparing `dagshub-0.3.0.post4/dagshub.egg-info/SOURCES.txt` & `dagshub-0.3.1/dagshub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/setup.py` & `dagshub-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/tests/test_dagshub_logger.py` & `dagshub-0.3.1/tests/test_dagshub_logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post4/tests/test_misc.py` & `dagshub-0.3.1/tests/test_misc.py`

 * *Files identical despite different names*

