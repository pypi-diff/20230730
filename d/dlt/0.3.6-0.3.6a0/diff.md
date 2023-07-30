# Comparing `tmp/dlt-0.3.6.tar.gz` & `tmp/dlt-0.3.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlt-0.3.6.tar", max compression
+gzip compressed data, was "dlt-0.3.6a0.tar", max compression
```

## Comparing `dlt-0.3.6.tar` & `dlt-0.3.6a0.tar`

### file list

```diff
@@ -1,225 +1,224 @@
--rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.3.6/LICENSE.txt
--rw-r--r--   0        0        0     4196 2023-07-21 12:57:39.118978 dlt-0.3.6/README.md
--rw-r--r--   0        0        0     1708 2023-07-08 12:23:15.759697 dlt-0.3.6/dlt/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 12:23:15.759697 dlt-0.3.6/dlt/cli/__init__.py
--rw-r--r--   0        0        0    17134 2023-07-26 18:57:08.058358 dlt-0.3.6/dlt/cli/_dlt.py
--rw-r--r--   0        0        0     3974 2023-07-08 12:23:15.759697 dlt-0.3.6/dlt/cli/config_toml_writer.py
--rw-r--r--   0        0        0    15153 2023-07-26 18:57:08.058358 dlt-0.3.6/dlt/cli/deploy_command.py
--rw-r--r--   0        0        0    14849 2023-07-08 12:23:15.759697 dlt-0.3.6/dlt/cli/deploy_command_helpers.py
--rw-r--r--   0        0        0     1944 2023-07-27 11:13:48.179808 dlt-0.3.6/dlt/cli/echo.py
--rw-r--r--   0        0        0      435 2023-07-08 12:23:15.759697 dlt-0.3.6/dlt/cli/exceptions.py
--rw-r--r--   0        0        0    19741 2023-07-27 11:13:48.189808 dlt-0.3.6/dlt/cli/init_command.py
--rw-r--r--   0        0        0    10508 2023-07-08 12:23:15.759697 dlt-0.3.6/dlt/cli/pipeline_command.py
--rw-r--r--   0        0        0     9939 2023-07-27 11:13:48.189808 dlt-0.3.6/dlt/cli/pipeline_files.py
--rw-r--r--   0        0        0     2523 2023-07-27 11:13:48.189808 dlt-0.3.6/dlt/cli/requirements.py
--rw-r--r--   0        0        0     4505 2023-07-08 12:23:15.759697 dlt-0.3.6/dlt/cli/source_detection.py
--rw-r--r--   0        0        0     1899 2023-07-08 12:23:15.759697 dlt-0.3.6/dlt/cli/telemetry_command.py
--rw-r--r--   0        0        0     2308 2023-07-20 14:41:03.294283 dlt-0.3.6/dlt/cli/utils.py
--rw-r--r--   0        0        0      307 2023-07-08 12:23:15.759697 dlt-0.3.6/dlt/common/__init__.py
--rw-r--r--   0        0        0     1265 2022-08-24 09:42:09.472789 dlt-0.3.6/dlt/common/arithmetics.py
--rw-r--r--   0        0        0      480 2023-07-13 09:09:29.104259 dlt-0.3.6/dlt/common/configuration/__init__.py
--rw-r--r--   0        0        0     5078 2023-07-08 12:23:15.759697 dlt-0.3.6/dlt/common/configuration/accessors.py
--rw-r--r--   0        0        0     3469 2023-07-08 12:23:15.759697 dlt-0.3.6/dlt/common/configuration/container.py
--rw-r--r--   0        0        0     6741 2023-07-08 12:23:15.759697 dlt-0.3.6/dlt/common/configuration/exceptions.py
--rw-r--r--   0        0        0     7912 2023-07-08 12:23:15.759697 dlt-0.3.6/dlt/common/configuration/inject.py
--rw-r--r--   0        0        0     1791 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/configuration/paths.py
--rw-r--r--   0        0        0      344 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/configuration/providers/__init__.py
--rw-r--r--   0        0        0      664 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/configuration/providers/airflow.py
--rw-r--r--   0        0        0     1116 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/configuration/providers/context.py
--rw-r--r--   0        0        0     1335 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/configuration/providers/dictionary.py
--rw-r--r--   0        0        0     1981 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/configuration/providers/environ.py
--rw-r--r--   0        0        0     3662 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/configuration/providers/google_secrets.py
--rw-r--r--   0        0        0     1306 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/configuration/providers/provider.py
--rw-r--r--   0        0        0    12880 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/configuration/providers/toml.py
--rw-r--r--   0        0        0    20347 2023-07-26 18:57:08.058358 dlt-0.3.6/dlt/common/configuration/resolve.py
--rw-r--r--   0        0        0     1002 2023-07-15 19:51:36.170686 dlt-0.3.6/dlt/common/configuration/specs/__init__.py
--rw-r--r--   0        0        0     1817 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/configuration/specs/api_credentials.py
--rw-r--r--   0        0        0     2128 2023-07-15 19:51:36.170686 dlt-0.3.6/dlt/common/configuration/specs/aws_credentials.py
--rw-r--r--   0        0        0    14214 2023-07-23 19:50:04.055755 dlt-0.3.6/dlt/common/configuration/specs/base_configuration.py
--rw-r--r--   0        0        0     5476 2023-07-15 19:51:36.170686 dlt-0.3.6/dlt/common/configuration/specs/config_providers_context.py
--rw-r--r--   0        0        0     3387 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/configuration/specs/config_section_context.py
--rw-r--r--   0        0        0     1818 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/configuration/specs/connection_string_credentials.py
--rw-r--r--   0        0        0     2125 2023-07-21 12:45:34.138978 dlt-0.3.6/dlt/common/configuration/specs/exceptions.py
--rw-r--r--   0        0        0    12537 2023-07-13 09:09:29.104259 dlt-0.3.6/dlt/common/configuration/specs/gcp_credentials.py
--rw-r--r--   0        0        0      725 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/configuration/specs/known_sections.py
--rw-r--r--   0        0        0     2712 2023-07-13 09:09:29.104259 dlt-0.3.6/dlt/common/configuration/specs/run_configuration.py
--rw-r--r--   0        0        0     6559 2023-07-20 23:10:47.941211 dlt-0.3.6/dlt/common/configuration/utils.py
--rw-r--r--   0        0        0      142 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/data_types/__init__.py
--rw-r--r--   0        0        0     6306 2023-07-15 10:14:14.845022 dlt-0.3.6/dlt/common/data_types/type_helpers.py
--rw-r--r--   0        0        0      214 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/data_types/typing.py
--rw-r--r--   0        0        0      260 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/data_writers/__init__.py
--rw-r--r--   0        0        0     6498 2023-07-27 11:13:48.189808 dlt-0.3.6/dlt/common/data_writers/buffered.py
--rw-r--r--   0        0        0     2727 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/data_writers/escape.py
--rw-r--r--   0        0        0      962 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/data_writers/exceptions.py
--rw-r--r--   0        0        0     8427 2023-07-27 11:13:48.189808 dlt-0.3.6/dlt/common/data_writers/writers.py
--rw-r--r--   0        0        0      189 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/destination/__init__.py
--rw-r--r--   0        0        0     3201 2023-07-21 12:58:04.898978 dlt-0.3.6/dlt/common/destination/capabilities.py
--rw-r--r--   0        0        0    13629 2023-07-30 20:32:44.418673 dlt-0.3.6/dlt/common/destination/reference.py
--rw-r--r--   0        0        0     8111 2023-07-15 19:51:36.170686 dlt-0.3.6/dlt/common/exceptions.py
--rw-r--r--   0        0        0     4954 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/git.py
--rw-r--r--   0        0        0     5253 2023-07-15 10:57:51.195021 dlt-0.3.6/dlt/common/json/__init__.py
--rw-r--r--   0        0        0     1802 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/json/_orjson.py
--rw-r--r--   0        0        0     2939 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/json/_simplejson.py
--rw-r--r--   0        0        0     1536 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/jsonpath.py
--rw-r--r--   0        0        0        0 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/libs/__init__.py
--rw-r--r--   0        0        0     1657 2023-07-15 19:51:36.170686 dlt-0.3.6/dlt/common/libs/pyarrow.py
--rw-r--r--   0        0        0      232 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/normalizers/__init__.py
--rw-r--r--   0        0        0     1197 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/normalizers/configuration.py
--rw-r--r--   0        0        0      472 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/normalizers/exceptions.py
--rw-r--r--   0        0        0     1644 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/normalizers/json/__init__.py
--rw-r--r--   0        0        0    13382 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/normalizers/json/relational.py
--rw-r--r--   0        0        0       64 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/normalizers/naming/__init__.py
--rw-r--r--   0        0        0      807 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/normalizers/naming/direct.py
--rw-r--r--   0        0        0     1069 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/normalizers/naming/duck_case.py
--rw-r--r--   0        0        0      792 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/normalizers/naming/exceptions.py
--rw-r--r--   0        0        0     3753 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/normalizers/naming/naming.py
--rw-r--r--   0        0        0     3002 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/normalizers/naming/snake_case.py
--rw-r--r--   0        0        0      358 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/normalizers/typing.py
--rw-r--r--   0        0        0     2337 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/normalizers/utils.py
--rw-r--r--   0        0        0      451 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/pendulum.py
--rw-r--r--   0        0        0    19564 2023-07-26 18:57:08.058358 dlt-0.3.6/dlt/common/pipeline.py
--rw-r--r--   0        0        0        0 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/reflection/__init__.py
--rw-r--r--   0        0        0      374 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/reflection/function_visitor.py
--rw-r--r--   0        0        0     4891 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/reflection/spec.py
--rw-r--r--   0        0        0     5069 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/reflection/utils.py
--rw-r--r--   0        0        0      174 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/runners/__init__.py
--rw-r--r--   0        0        0      705 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/runners/configuration.py
--rw-r--r--   0        0        0     2635 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/runners/pool_runner.py
--rw-r--r--   0        0        0     4046 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/runners/runnable.py
--rw-r--r--   0        0        0     3145 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/runners/stdout.py
--rw-r--r--   0        0        0     2137 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/runners/synth_pickle.py
--rw-r--r--   0        0        0      105 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/runners/typing.py
--rw-r--r--   0        0        0     5590 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/runners/venv.py
--rw-r--r--   0        0        0       36 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/runtime/__init__.py
--rw-r--r--   0        0        0    13923 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/runtime/collector.py
--rw-r--r--   0        0        0     5032 2023-07-26 18:57:08.058358 dlt-0.3.6/dlt/common/runtime/exec_info.py
--rw-r--r--   0        0        0      771 2023-07-13 09:09:29.104259 dlt-0.3.6/dlt/common/runtime/init.py
--rw-r--r--   0        0        0     4002 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/runtime/logger.py
--rw-r--r--   0        0        0     2052 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/runtime/prometheus.py
--rw-r--r--   0        0        0     7234 2023-07-20 14:41:03.304283 dlt-0.3.6/dlt/common/runtime/segment.py
--rw-r--r--   0        0        0     2492 2023-07-13 09:09:29.104259 dlt-0.3.6/dlt/common/runtime/sentry.py
--rw-r--r--   0        0        0     2027 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/runtime/signals.py
--rw-r--r--   0        0        0      616 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/runtime/slack.py
--rw-r--r--   0        0        0     2798 2023-07-20 14:41:03.304283 dlt-0.3.6/dlt/common/runtime/telemetry.py
--rw-r--r--   0        0        0      387 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/schema/__init__.py
--rw-r--r--   0        0        0     1927 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/schema/detections.py
--rw-r--r--   0        0        0     2974 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/schema/exceptions.py
--rw-r--r--   0        0        0    25586 2023-07-30 20:32:44.418673 dlt-0.3.6/dlt/common/schema/schema.py
--rw-r--r--   0        0        0     3004 2023-07-29 11:30:56.572443 dlt-0.3.6/dlt/common/schema/typing.py
--rw-r--r--   0        0        0    23933 2023-07-30 20:32:44.418673 dlt-0.3.6/dlt/common/schema/utils.py
--rw-r--r--   0        0        0     1467 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/source.py
--rw-r--r--   0        0        0      554 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/storages/__init__.py
--rw-r--r--   0        0        0     1649 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/storages/configuration.py
--rw-r--r--   0        0        0     2321 2023-07-27 11:13:48.189808 dlt-0.3.6/dlt/common/storages/data_item_storage.py
--rw-r--r--   0        0        0     3107 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/storages/exceptions.py
--rw-r--r--   0        0        0    11872 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/storages/file_storage.py
--rw-r--r--   0        0        0     2690 2023-07-20 16:42:01.694283 dlt-0.3.6/dlt/common/storages/live_schema_storage.py
--rw-r--r--   0        0        0    21812 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/storages/load_storage.py
--rw-r--r--   0        0        0     2409 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/storages/normalize_storage.py
--rw-r--r--   0        0        0     8600 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/storages/schema_storage.py
--rw-r--r--   0        0        0     9506 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/storages/transactional_file.py
--rw-r--r--   0        0        0     2525 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/storages/versioned_storage.py
--rw-r--r--   0        0        0     2634 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/time.py
--rw-r--r--   0        0        0     4736 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/typing.py
--rw-r--r--   0        0        0    14285 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/utils.py
--rw-r--r--   0        0        0     3686 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/validation.py
--rw-r--r--   0        0        0     1185 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/common/wei.py
--rw-r--r--   0        0        0        0 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/destinations/__init__.py
--rw-r--r--   0        0        0      437 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/destinations/bigquery/README.md
--rw-r--r--   0        0        0     2129 2023-07-30 20:32:44.418673 dlt-0.3.6/dlt/destinations/bigquery/__init__.py
--rw-r--r--   0        0        0    14652 2023-07-30 20:32:44.418673 dlt-0.3.6/dlt/destinations/bigquery/bigquery.py
--rw-r--r--   0        0        0     2019 2023-07-26 18:57:08.058358 dlt-0.3.6/dlt/destinations/bigquery/configuration.py
--rw-r--r--   0        0        0    10509 2023-07-15 19:51:36.170686 dlt-0.3.6/dlt/destinations/bigquery/sql_client.py
--rw-r--r--   0        0        0     2302 2023-07-30 20:32:44.418673 dlt-0.3.6/dlt/destinations/duckdb/__init__.py
--rw-r--r--   0        0        0     7342 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/destinations/duckdb/configuration.py
--rw-r--r--   0        0        0     4238 2023-07-30 20:32:44.418673 dlt-0.3.6/dlt/destinations/duckdb/duck.py
--rw-r--r--   0        0        0     6386 2023-07-30 20:32:44.418673 dlt-0.3.6/dlt/destinations/duckdb/sql_client.py
--rw-r--r--   0        0        0     1761 2023-07-15 19:51:36.170686 dlt-0.3.6/dlt/destinations/dummy/__init__.py
--rw-r--r--   0        0        0      736 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/destinations/dummy/configuration.py
--rw-r--r--   0        0        0     5105 2023-07-21 12:58:04.898978 dlt-0.3.6/dlt/destinations/dummy/dummy.py
--rw-r--r--   0        0        0     4759 2023-07-30 20:32:44.418673 dlt-0.3.6/dlt/destinations/exceptions.py
--rw-r--r--   0        0        0     1270 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/destinations/filesystem/__init__.py
--rw-r--r--   0        0        0     2935 2023-07-26 18:57:08.058358 dlt-0.3.6/dlt/destinations/filesystem/configuration.py
--rw-r--r--   0        0        0     5618 2023-07-30 20:32:44.418673 dlt-0.3.6/dlt/destinations/filesystem/filesystem.py
--rw-r--r--   0        0        0     1390 2023-07-26 18:57:08.058358 dlt-0.3.6/dlt/destinations/filesystem/filesystem_client.py
--rw-r--r--   0        0        0     4772 2023-07-30 20:32:44.418673 dlt-0.3.6/dlt/destinations/insert_job_client.py
--rw-r--r--   0        0        0    19938 2023-07-30 20:32:44.418673 dlt-0.3.6/dlt/destinations/job_client_impl.py
--rw-r--r--   0        0        0     2057 2023-07-15 19:51:36.180686 dlt-0.3.6/dlt/destinations/job_impl.py
--rw-r--r--   0        0        0     2246 2023-07-30 20:32:44.418673 dlt-0.3.6/dlt/destinations/motherduck/__init__.py
--rw-r--r--   0        0        0     2070 2023-07-26 18:57:08.058358 dlt-0.3.6/dlt/destinations/motherduck/configuration.py
--rw-r--r--   0        0        0      968 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/destinations/motherduck/motherduck.py
--rw-r--r--   0        0        0     1391 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/destinations/motherduck/sql_client.py
--rw-r--r--   0        0        0      251 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/destinations/postgres/README.md
--rw-r--r--   0        0        0     2305 2023-07-30 20:32:44.418673 dlt-0.3.6/dlt/destinations/postgres/__init__.py
--rw-r--r--   0        0        0     1649 2023-07-26 18:57:08.058358 dlt-0.3.6/dlt/destinations/postgres/configuration.py
--rw-r--r--   0        0        0     4188 2023-07-30 20:32:44.418673 dlt-0.3.6/dlt/destinations/postgres/postgres.py
--rw-r--r--   0        0        0     5484 2023-07-30 20:32:44.418673 dlt-0.3.6/dlt/destinations/postgres/sql_client.py
--rw-r--r--   0        0        0     1159 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/destinations/redshift/README.md
--rw-r--r--   0        0        0     2230 2023-07-30 20:32:44.418673 dlt-0.3.6/dlt/destinations/redshift/__init__.py
--rw-r--r--   0        0        0      894 2023-07-26 18:57:08.058358 dlt-0.3.6/dlt/destinations/redshift/configuration.py
--rw-r--r--   0        0        0     8521 2023-07-30 20:32:44.418673 dlt-0.3.6/dlt/destinations/redshift/redshift.py
--rw-r--r--   0        0        0     2241 2023-07-30 20:32:44.418673 dlt-0.3.6/dlt/destinations/snowflake/__init__.py
--rw-r--r--   0        0        0     4347 2023-07-26 18:57:08.058358 dlt-0.3.6/dlt/destinations/snowflake/configuration.py
--rw-r--r--   0        0        0     9851 2023-07-30 20:32:44.418673 dlt-0.3.6/dlt/destinations/snowflake/snowflake.py
--rw-r--r--   0        0        0     6820 2023-07-30 20:32:44.418673 dlt-0.3.6/dlt/destinations/snowflake/sql_client.py
--rw-r--r--   0        0        0     8198 2023-07-30 20:32:44.418673 dlt-0.3.6/dlt/destinations/sql_client.py
--rw-r--r--   0        0        0    12350 2023-07-30 20:32:44.418673 dlt-0.3.6/dlt/destinations/sql_jobs.py
--rw-r--r--   0        0        0     1931 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/destinations/typing.py
--rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.3.6/dlt/extract/__init__.py
--rw-r--r--   0        0        0    26516 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/extract/decorators.py
--rw-r--r--   0        0        0    12995 2023-07-15 16:23:33.345022 dlt-0.3.6/dlt/extract/exceptions.py
--rw-r--r--   0        0        0     9379 2023-07-29 11:30:56.572443 dlt-0.3.6/dlt/extract/extract.py
--rw-r--r--   0        0        0    19337 2023-07-20 14:41:03.304283 dlt-0.3.6/dlt/extract/incremental.py
--rw-r--r--   0        0        0    35424 2023-07-20 14:41:03.304283 dlt-0.3.6/dlt/extract/pipe.py
--rw-r--r--   0        0        0     9683 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/extract/schema.py
--rw-r--r--   0        0        0    38391 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/extract/source.py
--rw-r--r--   0        0        0     4308 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/extract/typing.py
--rw-r--r--   0        0        0      593 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/extract/utils.py
--rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.3.6/dlt/helpers/__init__.py
--rw-r--r--   0        0        0    13867 2023-07-20 14:41:03.304283 dlt-0.3.6/dlt/helpers/airflow_helper.py
--rw-r--r--   0        0        0     3167 2023-07-13 09:09:29.104259 dlt-0.3.6/dlt/helpers/dbt/__init__.py
--rw-r--r--   0        0        0     1220 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/helpers/dbt/configuration.py
--rw-r--r--   0        0        0     6669 2023-07-13 09:09:29.104259 dlt-0.3.6/dlt/helpers/dbt/dbt_utils.py
--rw-r--r--   0        0        0      758 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/helpers/dbt/exceptions.py
--rw-r--r--   0        0        0     5220 2023-07-13 09:09:29.104259 dlt-0.3.6/dlt/helpers/dbt/profiles.yml
--rw-r--r--   0        0        0    13214 2023-07-20 14:41:03.304283 dlt-0.3.6/dlt/helpers/dbt/runner.py
--rw-r--r--   0        0        0     2490 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/helpers/pandas_helper.py
--rw-r--r--   0        0        0    13378 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/helpers/streamlit_helper.py
--rw-r--r--   0        0        0       31 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/load/__init__.py
--rw-r--r--   0        0        0     1005 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/load/configuration.py
--rw-r--r--   0        0        0     1993 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/load/exceptions.py
--rw-r--r--   0        0        0    24642 2023-07-30 20:32:44.418673 dlt-0.3.6/dlt/load/load.py
--rw-r--r--   0        0        0       32 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/normalize/__init__.py
--rw-r--r--   0        0        0     1101 2023-07-08 12:23:15.769697 dlt-0.3.6/dlt/normalize/configuration.py
--rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.3.6/dlt/normalize/exceptions.py
--rw-r--r--   0        0        0    17202 2023-07-30 20:32:44.418673 dlt-0.3.6/dlt/normalize/normalize.py
--rw-r--r--   0        0        0    13834 2023-07-30 20:32:44.418673 dlt-0.3.6/dlt/pipeline/__init__.py
--rw-r--r--   0        0        0     2009 2023-07-15 19:51:36.180686 dlt-0.3.6/dlt/pipeline/configuration.py
--rw-r--r--   0        0        0      379 2023-07-08 12:23:15.779697 dlt-0.3.6/dlt/pipeline/current.py
--rw-r--r--   0        0        0     4829 2023-07-08 12:23:15.779697 dlt-0.3.6/dlt/pipeline/dbt.py
--rw-r--r--   0        0        0     3100 2023-07-08 12:23:15.779697 dlt-0.3.6/dlt/pipeline/exceptions.py
--rw-r--r--   0        0        0     8753 2023-07-21 12:58:04.908978 dlt-0.3.6/dlt/pipeline/helpers.py
--rw-r--r--   0        0        0      122 2023-07-08 12:23:15.779697 dlt-0.3.6/dlt/pipeline/mark.py
--rw-r--r--   0        0        0    65295 2023-07-30 20:32:44.418673 dlt-0.3.6/dlt/pipeline/pipeline.py
--rw-r--r--   0        0        0      985 2023-07-08 12:23:15.779697 dlt-0.3.6/dlt/pipeline/progress.py
--rw-r--r--   0        0        0     4186 2023-07-08 12:23:15.779697 dlt-0.3.6/dlt/pipeline/state_sync.py
--rw-r--r--   0        0        0     9132 2023-07-20 14:41:03.304283 dlt-0.3.6/dlt/pipeline/trace.py
--rw-r--r--   0        0        0     5060 2023-07-26 18:57:08.058358 dlt-0.3.6/dlt/pipeline/track.py
--rw-r--r--   0        0        0       91 2023-07-08 12:23:15.779697 dlt-0.3.6/dlt/pipeline/typing.py
--rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.3.6/dlt/py.typed
--rw-r--r--   0        0        0        0 2023-07-08 12:23:15.779697 dlt-0.3.6/dlt/reflection/__init__.py
--rw-r--r--   0        0        0      563 2023-07-08 12:23:15.779697 dlt-0.3.6/dlt/reflection/names.py
--rw-r--r--   0        0        0     5617 2023-07-08 12:23:15.779697 dlt-0.3.6/dlt/reflection/script_inspector.py
--rw-r--r--   0        0        0     6186 2023-07-08 12:23:15.779697 dlt-0.3.6/dlt/reflection/script_visitor.py
--rw-r--r--   0        0        0      124 2023-07-08 12:23:15.779697 dlt-0.3.6/dlt/sources/__init__.py
--rw-r--r--   0        0        0      320 2023-07-08 12:23:15.779697 dlt-0.3.6/dlt/sources/credentials.py
--rw-r--r--   0        0        0        0 2023-07-08 12:23:15.779697 dlt-0.3.6/dlt/sources/helpers/__init__.py
--rw-r--r--   0        0        0      832 2023-07-13 09:09:29.104259 dlt-0.3.6/dlt/sources/helpers/requests/__init__.py
--rw-r--r--   0        0        0    10837 2023-07-13 09:09:29.104259 dlt-0.3.6/dlt/sources/helpers/requests/retry.py
--rw-r--r--   0        0        0     1757 2023-07-13 09:09:29.104259 dlt-0.3.6/dlt/sources/helpers/requests/session.py
--rw-r--r--   0        0        0      234 2023-07-13 09:09:29.104259 dlt-0.3.6/dlt/sources/helpers/requests/typing.py
--rw-r--r--   0        0        0      679 2023-07-08 12:23:15.779697 dlt-0.3.6/dlt/sources/helpers/transform.py
--rw-r--r--   0        0        0     1125 2023-07-08 12:23:15.779697 dlt-0.3.6/dlt/version.py
--rw-r--r--   0        0        0     4459 2023-07-30 20:43:39.078673 dlt-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     7815 1970-01-01 00:00:00.000000 dlt-0.3.6/setup.py
--rw-r--r--   0        0        0     7800 1970-01-01 00:00:00.000000 dlt-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.3.6a0/LICENSE.txt
+-rw-r--r--   0        0        0     4196 2023-07-21 12:57:39.118978 dlt-0.3.6a0/README.md
+-rw-r--r--   0        0        0     1708 2023-07-08 12:23:15.759697 dlt-0.3.6a0/dlt/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:23:15.759697 dlt-0.3.6a0/dlt/cli/__init__.py
+-rw-r--r--   0        0        0    17134 2023-07-25 13:41:56.702222 dlt-0.3.6a0/dlt/cli/_dlt.py
+-rw-r--r--   0        0        0     3974 2023-07-08 12:23:15.759697 dlt-0.3.6a0/dlt/cli/config_toml_writer.py
+-rw-r--r--   0        0        0    15153 2023-07-25 13:41:56.712222 dlt-0.3.6a0/dlt/cli/deploy_command.py
+-rw-r--r--   0        0        0    14849 2023-07-08 12:23:15.759697 dlt-0.3.6a0/dlt/cli/deploy_command_helpers.py
+-rw-r--r--   0        0        0     1853 2023-07-08 12:23:15.759697 dlt-0.3.6a0/dlt/cli/echo.py
+-rw-r--r--   0        0        0      435 2023-07-08 12:23:15.759697 dlt-0.3.6a0/dlt/cli/exceptions.py
+-rw-r--r--   0        0        0    18756 2023-07-08 12:23:15.759697 dlt-0.3.6a0/dlt/cli/init_command.py
+-rw-r--r--   0        0        0    10508 2023-07-08 12:23:15.759697 dlt-0.3.6a0/dlt/cli/pipeline_command.py
+-rw-r--r--   0        0        0     9588 2023-07-08 12:23:15.759697 dlt-0.3.6a0/dlt/cli/pipeline_files.py
+-rw-r--r--   0        0        0     4505 2023-07-08 12:23:15.759697 dlt-0.3.6a0/dlt/cli/source_detection.py
+-rw-r--r--   0        0        0     1899 2023-07-08 12:23:15.759697 dlt-0.3.6a0/dlt/cli/telemetry_command.py
+-rw-r--r--   0        0        0     2308 2023-07-20 14:41:03.294283 dlt-0.3.6a0/dlt/cli/utils.py
+-rw-r--r--   0        0        0      307 2023-07-08 12:23:15.759697 dlt-0.3.6a0/dlt/common/__init__.py
+-rw-r--r--   0        0        0     1265 2022-08-24 09:42:09.472789 dlt-0.3.6a0/dlt/common/arithmetics.py
+-rw-r--r--   0        0        0      480 2023-07-13 09:09:29.104259 dlt-0.3.6a0/dlt/common/configuration/__init__.py
+-rw-r--r--   0        0        0     5078 2023-07-08 12:23:15.759697 dlt-0.3.6a0/dlt/common/configuration/accessors.py
+-rw-r--r--   0        0        0     3469 2023-07-08 12:23:15.759697 dlt-0.3.6a0/dlt/common/configuration/container.py
+-rw-r--r--   0        0        0     6741 2023-07-08 12:23:15.759697 dlt-0.3.6a0/dlt/common/configuration/exceptions.py
+-rw-r--r--   0        0        0     7912 2023-07-08 12:23:15.759697 dlt-0.3.6a0/dlt/common/configuration/inject.py
+-rw-r--r--   0        0        0     1791 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/configuration/paths.py
+-rw-r--r--   0        0        0      344 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/configuration/providers/__init__.py
+-rw-r--r--   0        0        0      664 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/configuration/providers/airflow.py
+-rw-r--r--   0        0        0     1116 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/configuration/providers/context.py
+-rw-r--r--   0        0        0     1335 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/configuration/providers/dictionary.py
+-rw-r--r--   0        0        0     1981 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/configuration/providers/environ.py
+-rw-r--r--   0        0        0     3662 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/configuration/providers/google_secrets.py
+-rw-r--r--   0        0        0     1306 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/configuration/providers/provider.py
+-rw-r--r--   0        0        0    12880 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/configuration/providers/toml.py
+-rw-r--r--   0        0        0    20347 2023-07-23 22:00:45.675755 dlt-0.3.6a0/dlt/common/configuration/resolve.py
+-rw-r--r--   0        0        0     1002 2023-07-15 19:51:36.170686 dlt-0.3.6a0/dlt/common/configuration/specs/__init__.py
+-rw-r--r--   0        0        0     1817 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/configuration/specs/api_credentials.py
+-rw-r--r--   0        0        0     2128 2023-07-15 19:51:36.170686 dlt-0.3.6a0/dlt/common/configuration/specs/aws_credentials.py
+-rw-r--r--   0        0        0    14214 2023-07-23 19:50:04.055755 dlt-0.3.6a0/dlt/common/configuration/specs/base_configuration.py
+-rw-r--r--   0        0        0     5476 2023-07-15 19:51:36.170686 dlt-0.3.6a0/dlt/common/configuration/specs/config_providers_context.py
+-rw-r--r--   0        0        0     3387 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/configuration/specs/config_section_context.py
+-rw-r--r--   0        0        0     1818 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/configuration/specs/connection_string_credentials.py
+-rw-r--r--   0        0        0     2125 2023-07-21 12:45:34.138978 dlt-0.3.6a0/dlt/common/configuration/specs/exceptions.py
+-rw-r--r--   0        0        0    12537 2023-07-13 09:09:29.104259 dlt-0.3.6a0/dlt/common/configuration/specs/gcp_credentials.py
+-rw-r--r--   0        0        0      725 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/configuration/specs/known_sections.py
+-rw-r--r--   0        0        0     2712 2023-07-13 09:09:29.104259 dlt-0.3.6a0/dlt/common/configuration/specs/run_configuration.py
+-rw-r--r--   0        0        0     6559 2023-07-20 23:10:47.941211 dlt-0.3.6a0/dlt/common/configuration/utils.py
+-rw-r--r--   0        0        0      142 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/data_types/__init__.py
+-rw-r--r--   0        0        0     6306 2023-07-15 10:14:14.845022 dlt-0.3.6a0/dlt/common/data_types/type_helpers.py
+-rw-r--r--   0        0        0      214 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/data_types/typing.py
+-rw-r--r--   0        0        0      260 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/data_writers/__init__.py
+-rw-r--r--   0        0        0     6203 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/data_writers/buffered.py
+-rw-r--r--   0        0        0     2727 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/data_writers/escape.py
+-rw-r--r--   0        0        0      962 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/data_writers/exceptions.py
+-rw-r--r--   0        0        0     8426 2023-07-20 16:41:36.924283 dlt-0.3.6a0/dlt/common/data_writers/writers.py
+-rw-r--r--   0        0        0      189 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/destination/__init__.py
+-rw-r--r--   0        0        0     3201 2023-07-21 12:58:04.898978 dlt-0.3.6a0/dlt/common/destination/capabilities.py
+-rw-r--r--   0        0        0    12397 2023-07-23 22:00:45.675755 dlt-0.3.6a0/dlt/common/destination/reference.py
+-rw-r--r--   0        0        0     8111 2023-07-15 19:51:36.170686 dlt-0.3.6a0/dlt/common/exceptions.py
+-rw-r--r--   0        0        0     4954 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/git.py
+-rw-r--r--   0        0        0     5253 2023-07-15 10:57:51.195021 dlt-0.3.6a0/dlt/common/json/__init__.py
+-rw-r--r--   0        0        0     1802 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/json/_orjson.py
+-rw-r--r--   0        0        0     2939 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/json/_simplejson.py
+-rw-r--r--   0        0        0     1536 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/jsonpath.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/libs/__init__.py
+-rw-r--r--   0        0        0     1657 2023-07-15 19:51:36.170686 dlt-0.3.6a0/dlt/common/libs/pyarrow.py
+-rw-r--r--   0        0        0      232 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/normalizers/__init__.py
+-rw-r--r--   0        0        0     1197 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/normalizers/configuration.py
+-rw-r--r--   0        0        0      472 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/normalizers/exceptions.py
+-rw-r--r--   0        0        0     1644 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/normalizers/json/__init__.py
+-rw-r--r--   0        0        0    13382 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/normalizers/json/relational.py
+-rw-r--r--   0        0        0       64 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/normalizers/naming/__init__.py
+-rw-r--r--   0        0        0      807 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/normalizers/naming/direct.py
+-rw-r--r--   0        0        0     1069 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/normalizers/naming/duck_case.py
+-rw-r--r--   0        0        0      792 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/normalizers/naming/exceptions.py
+-rw-r--r--   0        0        0     3753 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/normalizers/naming/naming.py
+-rw-r--r--   0        0        0     3002 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/normalizers/naming/snake_case.py
+-rw-r--r--   0        0        0      358 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/normalizers/typing.py
+-rw-r--r--   0        0        0     2337 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/normalizers/utils.py
+-rw-r--r--   0        0        0      451 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/pendulum.py
+-rw-r--r--   0        0        0    19564 2023-07-23 22:00:45.675755 dlt-0.3.6a0/dlt/common/pipeline.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/reflection/__init__.py
+-rw-r--r--   0        0        0      374 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/reflection/function_visitor.py
+-rw-r--r--   0        0        0     4891 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/reflection/spec.py
+-rw-r--r--   0        0        0     5069 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/reflection/utils.py
+-rw-r--r--   0        0        0      174 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/runners/__init__.py
+-rw-r--r--   0        0        0      705 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/runners/configuration.py
+-rw-r--r--   0        0        0     2635 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/runners/pool_runner.py
+-rw-r--r--   0        0        0     4046 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/runners/runnable.py
+-rw-r--r--   0        0        0     3145 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/runners/stdout.py
+-rw-r--r--   0        0        0     2137 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/runners/synth_pickle.py
+-rw-r--r--   0        0        0      105 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/runners/typing.py
+-rw-r--r--   0        0        0     5590 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/runners/venv.py
+-rw-r--r--   0        0        0       36 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/runtime/__init__.py
+-rw-r--r--   0        0        0    13923 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/runtime/collector.py
+-rw-r--r--   0        0        0     5032 2023-07-21 13:08:23.348978 dlt-0.3.6a0/dlt/common/runtime/exec_info.py
+-rw-r--r--   0        0        0      771 2023-07-13 09:09:29.104259 dlt-0.3.6a0/dlt/common/runtime/init.py
+-rw-r--r--   0        0        0     4002 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/runtime/logger.py
+-rw-r--r--   0        0        0     2052 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/runtime/prometheus.py
+-rw-r--r--   0        0        0     7234 2023-07-20 14:41:03.304283 dlt-0.3.6a0/dlt/common/runtime/segment.py
+-rw-r--r--   0        0        0     2492 2023-07-13 09:09:29.104259 dlt-0.3.6a0/dlt/common/runtime/sentry.py
+-rw-r--r--   0        0        0     2027 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/runtime/signals.py
+-rw-r--r--   0        0        0      616 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/runtime/slack.py
+-rw-r--r--   0        0        0     2798 2023-07-20 14:41:03.304283 dlt-0.3.6a0/dlt/common/runtime/telemetry.py
+-rw-r--r--   0        0        0      387 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/schema/__init__.py
+-rw-r--r--   0        0        0     1927 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/schema/detections.py
+-rw-r--r--   0        0        0     2974 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/schema/exceptions.py
+-rw-r--r--   0        0        0    25222 2023-07-23 14:19:47.065755 dlt-0.3.6a0/dlt/common/schema/schema.py
+-rw-r--r--   0        0        0     3004 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/schema/typing.py
+-rw-r--r--   0        0        0    23295 2023-07-15 19:51:36.170686 dlt-0.3.6a0/dlt/common/schema/utils.py
+-rw-r--r--   0        0        0     1467 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/source.py
+-rw-r--r--   0        0        0      554 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/storages/__init__.py
+-rw-r--r--   0        0        0     1649 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/storages/configuration.py
+-rw-r--r--   0        0        0     1906 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/storages/data_item_storage.py
+-rw-r--r--   0        0        0     3107 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/storages/exceptions.py
+-rw-r--r--   0        0        0    11872 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/storages/file_storage.py
+-rw-r--r--   0        0        0     2690 2023-07-20 16:42:01.694283 dlt-0.3.6a0/dlt/common/storages/live_schema_storage.py
+-rw-r--r--   0        0        0    21812 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/storages/load_storage.py
+-rw-r--r--   0        0        0     2409 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/storages/normalize_storage.py
+-rw-r--r--   0        0        0     8600 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/storages/schema_storage.py
+-rw-r--r--   0        0        0     9506 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/storages/transactional_file.py
+-rw-r--r--   0        0        0     2525 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/storages/versioned_storage.py
+-rw-r--r--   0        0        0     2634 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/time.py
+-rw-r--r--   0        0        0     4736 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/typing.py
+-rw-r--r--   0        0        0    14285 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/utils.py
+-rw-r--r--   0        0        0     3686 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/validation.py
+-rw-r--r--   0        0        0     1185 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/common/wei.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/destinations/__init__.py
+-rw-r--r--   0        0        0      437 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/destinations/bigquery/README.md
+-rw-r--r--   0        0        0     2136 2023-07-15 19:51:36.170686 dlt-0.3.6a0/dlt/destinations/bigquery/__init__.py
+-rw-r--r--   0        0        0    15192 2023-07-21 12:58:04.898978 dlt-0.3.6a0/dlt/destinations/bigquery/bigquery.py
+-rw-r--r--   0        0        0     2019 2023-07-23 22:00:45.675755 dlt-0.3.6a0/dlt/destinations/bigquery/configuration.py
+-rw-r--r--   0        0        0    10509 2023-07-15 19:51:36.170686 dlt-0.3.6a0/dlt/destinations/bigquery/sql_client.py
+-rw-r--r--   0        0        0     2300 2023-07-21 12:58:04.898978 dlt-0.3.6a0/dlt/destinations/duckdb/__init__.py
+-rw-r--r--   0        0        0     7342 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/destinations/duckdb/configuration.py
+-rw-r--r--   0        0        0     4284 2023-07-21 12:58:04.898978 dlt-0.3.6a0/dlt/destinations/duckdb/duck.py
+-rw-r--r--   0        0        0     6635 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/destinations/duckdb/sql_client.py
+-rw-r--r--   0        0        0     1761 2023-07-15 19:51:36.170686 dlt-0.3.6a0/dlt/destinations/dummy/__init__.py
+-rw-r--r--   0        0        0      736 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/destinations/dummy/configuration.py
+-rw-r--r--   0        0        0     5105 2023-07-21 12:58:04.898978 dlt-0.3.6a0/dlt/destinations/dummy/dummy.py
+-rw-r--r--   0        0        0     4184 2023-07-15 19:51:36.170686 dlt-0.3.6a0/dlt/destinations/exceptions.py
+-rw-r--r--   0        0        0     1270 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/destinations/filesystem/__init__.py
+-rw-r--r--   0        0        0     2935 2023-07-23 22:00:45.675755 dlt-0.3.6a0/dlt/destinations/filesystem/configuration.py
+-rw-r--r--   0        0        0     6445 2023-07-23 22:00:45.675755 dlt-0.3.6a0/dlt/destinations/filesystem/filesystem.py
+-rw-r--r--   0        0        0     1390 2023-07-23 22:00:45.675755 dlt-0.3.6a0/dlt/destinations/filesystem/filesystem_client.py
+-rw-r--r--   0        0        0     5216 2023-07-21 12:58:04.898978 dlt-0.3.6a0/dlt/destinations/insert_job_client.py
+-rw-r--r--   0        0        0    19525 2023-07-23 14:19:47.065755 dlt-0.3.6a0/dlt/destinations/job_client_impl.py
+-rw-r--r--   0        0        0     2057 2023-07-15 19:51:36.180686 dlt-0.3.6a0/dlt/destinations/job_impl.py
+-rw-r--r--   0        0        0     2244 2023-07-21 12:58:04.898978 dlt-0.3.6a0/dlt/destinations/motherduck/__init__.py
+-rw-r--r--   0        0        0     2070 2023-07-23 22:00:45.675755 dlt-0.3.6a0/dlt/destinations/motherduck/configuration.py
+-rw-r--r--   0        0        0      968 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/destinations/motherduck/motherduck.py
+-rw-r--r--   0        0        0     1391 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/destinations/motherduck/sql_client.py
+-rw-r--r--   0        0        0      251 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/destinations/postgres/README.md
+-rw-r--r--   0        0        0     2312 2023-07-15 19:51:36.180686 dlt-0.3.6a0/dlt/destinations/postgres/__init__.py
+-rw-r--r--   0        0        0     1649 2023-07-23 22:00:45.675755 dlt-0.3.6a0/dlt/destinations/postgres/configuration.py
+-rw-r--r--   0        0        0     4490 2023-07-21 12:58:04.898978 dlt-0.3.6a0/dlt/destinations/postgres/postgres.py
+-rw-r--r--   0        0        0     5781 2023-07-20 16:42:13.474283 dlt-0.3.6a0/dlt/destinations/postgres/sql_client.py
+-rw-r--r--   0        0        0     1159 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/destinations/redshift/README.md
+-rw-r--r--   0        0        0     2237 2023-07-15 19:51:36.180686 dlt-0.3.6a0/dlt/destinations/redshift/__init__.py
+-rw-r--r--   0        0        0      894 2023-07-23 22:00:45.675755 dlt-0.3.6a0/dlt/destinations/redshift/configuration.py
+-rw-r--r--   0        0        0     9085 2023-07-21 12:58:04.898978 dlt-0.3.6a0/dlt/destinations/redshift/redshift.py
+-rw-r--r--   0        0        0     2255 2023-07-15 19:51:36.180686 dlt-0.3.6a0/dlt/destinations/snowflake/__init__.py
+-rw-r--r--   0        0        0     4347 2023-07-23 22:00:45.675755 dlt-0.3.6a0/dlt/destinations/snowflake/configuration.py
+-rw-r--r--   0        0        0    10402 2023-07-21 12:58:04.898978 dlt-0.3.6a0/dlt/destinations/snowflake/snowflake.py
+-rw-r--r--   0        0        0     7069 2023-07-15 19:51:36.180686 dlt-0.3.6a0/dlt/destinations/snowflake/sql_client.py
+-rw-r--r--   0        0        0     8045 2023-07-21 12:58:04.898978 dlt-0.3.6a0/dlt/destinations/sql_client.py
+-rw-r--r--   0        0        0    12311 2023-07-21 12:58:04.898978 dlt-0.3.6a0/dlt/destinations/sql_jobs.py
+-rw-r--r--   0        0        0     1931 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/destinations/typing.py
+-rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.3.6a0/dlt/extract/__init__.py
+-rw-r--r--   0        0        0    26516 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/extract/decorators.py
+-rw-r--r--   0        0        0    12995 2023-07-15 16:23:33.345022 dlt-0.3.6a0/dlt/extract/exceptions.py
+-rw-r--r--   0        0        0     8312 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/extract/extract.py
+-rw-r--r--   0        0        0    19337 2023-07-20 14:41:03.304283 dlt-0.3.6a0/dlt/extract/incremental.py
+-rw-r--r--   0        0        0    35424 2023-07-20 14:41:03.304283 dlt-0.3.6a0/dlt/extract/pipe.py
+-rw-r--r--   0        0        0     9683 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/extract/schema.py
+-rw-r--r--   0        0        0    38391 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/extract/source.py
+-rw-r--r--   0        0        0     4308 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/extract/typing.py
+-rw-r--r--   0        0        0      593 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/extract/utils.py
+-rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.3.6a0/dlt/helpers/__init__.py
+-rw-r--r--   0        0        0    13867 2023-07-20 14:41:03.304283 dlt-0.3.6a0/dlt/helpers/airflow_helper.py
+-rw-r--r--   0        0        0     3167 2023-07-13 09:09:29.104259 dlt-0.3.6a0/dlt/helpers/dbt/__init__.py
+-rw-r--r--   0        0        0     1220 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/helpers/dbt/configuration.py
+-rw-r--r--   0        0        0     6669 2023-07-13 09:09:29.104259 dlt-0.3.6a0/dlt/helpers/dbt/dbt_utils.py
+-rw-r--r--   0        0        0      758 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/helpers/dbt/exceptions.py
+-rw-r--r--   0        0        0     5220 2023-07-13 09:09:29.104259 dlt-0.3.6a0/dlt/helpers/dbt/profiles.yml
+-rw-r--r--   0        0        0    13214 2023-07-20 14:41:03.304283 dlt-0.3.6a0/dlt/helpers/dbt/runner.py
+-rw-r--r--   0        0        0     2490 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/helpers/pandas_helper.py
+-rw-r--r--   0        0        0    13378 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/helpers/streamlit_helper.py
+-rw-r--r--   0        0        0       31 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/load/__init__.py
+-rw-r--r--   0        0        0     1005 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/load/configuration.py
+-rw-r--r--   0        0        0     1993 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/load/exceptions.py
+-rw-r--r--   0        0        0    22500 2023-07-23 22:00:45.675755 dlt-0.3.6a0/dlt/load/load.py
+-rw-r--r--   0        0        0       32 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/normalize/__init__.py
+-rw-r--r--   0        0        0     1101 2023-07-08 12:23:15.769697 dlt-0.3.6a0/dlt/normalize/configuration.py
+-rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.3.6a0/dlt/normalize/exceptions.py
+-rw-r--r--   0        0        0    16488 2023-07-20 16:42:34.194283 dlt-0.3.6a0/dlt/normalize/normalize.py
+-rw-r--r--   0        0        0    13633 2023-07-15 19:51:36.180686 dlt-0.3.6a0/dlt/pipeline/__init__.py
+-rw-r--r--   0        0        0     2009 2023-07-15 19:51:36.180686 dlt-0.3.6a0/dlt/pipeline/configuration.py
+-rw-r--r--   0        0        0      379 2023-07-08 12:23:15.779697 dlt-0.3.6a0/dlt/pipeline/current.py
+-rw-r--r--   0        0        0     4829 2023-07-08 12:23:15.779697 dlt-0.3.6a0/dlt/pipeline/dbt.py
+-rw-r--r--   0        0        0     3100 2023-07-08 12:23:15.779697 dlt-0.3.6a0/dlt/pipeline/exceptions.py
+-rw-r--r--   0        0        0     8753 2023-07-21 12:58:04.908978 dlt-0.3.6a0/dlt/pipeline/helpers.py
+-rw-r--r--   0        0        0      122 2023-07-08 12:23:15.779697 dlt-0.3.6a0/dlt/pipeline/mark.py
+-rw-r--r--   0        0        0    65184 2023-07-23 22:00:45.675755 dlt-0.3.6a0/dlt/pipeline/pipeline.py
+-rw-r--r--   0        0        0      985 2023-07-08 12:23:15.779697 dlt-0.3.6a0/dlt/pipeline/progress.py
+-rw-r--r--   0        0        0     4186 2023-07-08 12:23:15.779697 dlt-0.3.6a0/dlt/pipeline/state_sync.py
+-rw-r--r--   0        0        0     9132 2023-07-20 14:41:03.304283 dlt-0.3.6a0/dlt/pipeline/trace.py
+-rw-r--r--   0        0        0     5060 2023-07-23 22:00:45.675755 dlt-0.3.6a0/dlt/pipeline/track.py
+-rw-r--r--   0        0        0       91 2023-07-08 12:23:15.779697 dlt-0.3.6a0/dlt/pipeline/typing.py
+-rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.3.6a0/dlt/py.typed
+-rw-r--r--   0        0        0        0 2023-07-08 12:23:15.779697 dlt-0.3.6a0/dlt/reflection/__init__.py
+-rw-r--r--   0        0        0      563 2023-07-08 12:23:15.779697 dlt-0.3.6a0/dlt/reflection/names.py
+-rw-r--r--   0        0        0     5617 2023-07-08 12:23:15.779697 dlt-0.3.6a0/dlt/reflection/script_inspector.py
+-rw-r--r--   0        0        0     6186 2023-07-08 12:23:15.779697 dlt-0.3.6a0/dlt/reflection/script_visitor.py
+-rw-r--r--   0        0        0      124 2023-07-08 12:23:15.779697 dlt-0.3.6a0/dlt/sources/__init__.py
+-rw-r--r--   0        0        0      320 2023-07-08 12:23:15.779697 dlt-0.3.6a0/dlt/sources/credentials.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:23:15.779697 dlt-0.3.6a0/dlt/sources/helpers/__init__.py
+-rw-r--r--   0        0        0      832 2023-07-13 09:09:29.104259 dlt-0.3.6a0/dlt/sources/helpers/requests/__init__.py
+-rw-r--r--   0        0        0    10837 2023-07-13 09:09:29.104259 dlt-0.3.6a0/dlt/sources/helpers/requests/retry.py
+-rw-r--r--   0        0        0     1757 2023-07-13 09:09:29.104259 dlt-0.3.6a0/dlt/sources/helpers/requests/session.py
+-rw-r--r--   0        0        0      234 2023-07-13 09:09:29.104259 dlt-0.3.6a0/dlt/sources/helpers/requests/typing.py
+-rw-r--r--   0        0        0      679 2023-07-08 12:23:15.779697 dlt-0.3.6a0/dlt/sources/helpers/transform.py
+-rw-r--r--   0        0        0     1125 2023-07-08 12:23:15.779697 dlt-0.3.6a0/dlt/version.py
+-rw-r--r--   0        0        0     4461 2023-07-25 13:41:56.712222 dlt-0.3.6a0/pyproject.toml
+-rw-r--r--   0        0        0     7817 1970-01-01 00:00:00.000000 dlt-0.3.6a0/setup.py
+-rw-r--r--   0        0        0     7802 1970-01-01 00:00:00.000000 dlt-0.3.6a0/PKG-INFO
```

### Comparing `dlt-0.3.6/LICENSE.txt` & `dlt-0.3.6a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/README.md` & `dlt-0.3.6a0/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/__init__.py` & `dlt-0.3.6a0/dlt/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/cli/_dlt.py` & `dlt-0.3.6a0/dlt/cli/_dlt.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/cli/config_toml_writer.py` & `dlt-0.3.6a0/dlt/cli/config_toml_writer.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/cli/deploy_command.py` & `dlt-0.3.6a0/dlt/cli/deploy_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/cli/deploy_command_helpers.py` & `dlt-0.3.6a0/dlt/cli/deploy_command_helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/cli/echo.py` & `dlt-0.3.6a0/dlt/cli/echo.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,18 +26,14 @@
 style = click.style
 
 
 def bold(msg: str) -> str:
     return click.style(msg, bold=True, reset=True)
 
 
-def warning_style(msg: str) -> str:
-    return click.style(msg, fg="yellow", reset=True)
-
-
 def error(msg: str) -> None:
     click.secho("ERROR: " + msg, fg="red")
 
 
 def warning(msg: str) -> None:
     click.secho("WARNING: " + msg, fg="yellow")
```

### Comparing `dlt-0.3.6/dlt/cli/init_command.py` & `dlt-0.3.6a0/dlt/cli/init_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 from dlt.reflection.script_inspector import inspect_pipeline_script, load_script_module
 
 from dlt.cli import echo as fmt, pipeline_files as files_ops, source_detection
 from dlt.cli import utils
 from dlt.cli.config_toml_writer import WritableConfigValue, write_values
 from dlt.cli.pipeline_files import VerifiedSourceFiles, TVerifiedSourceFileEntry, TVerifiedSourceFileIndex
 from dlt.cli.exceptions import CliCommandException
-from dlt.cli.requirements import SourceRequirements
 
 DLT_INIT_DOCS_URL = "https://dlthub.com/docs/reference/command-line-interface#dlt-init"
 DEFAULT_VERIFIED_SOURCES_REPO = "https://github.com/dlt-hub/verified-sources.git"
 INIT_MODULE_NAME = "init"
 SOURCES_MODULE_NAME = "sources"
 
 
@@ -123,21 +122,20 @@
             fmt.echo("Verified source %s was updated to the newest version!" % fmt.bold(source_name))
 
     if is_new_source:
         fmt.echo("* Add credentials for %s and other secrets in %s" % (fmt.bold(destination_name), fmt.bold(make_dlt_settings_path(SECRETS_TOML))))
 
     if dependency_system:
         fmt.echo("* Add the required dependencies to %s:" % fmt.bold(dependency_system))
-        compiled_requirements = source_files.requirements.compiled()
-        for dep in compiled_requirements:
+        for dep in source_files.requirements:
             fmt.echo("  " + fmt.bold(dep))
         fmt.echo("  If the dlt dependency is already added, make sure you install the extra for %s to it" % fmt.bold(destination_name))
         if dependency_system == utils.REQUIREMENTS_TXT:
             qs = "' '"
-            fmt.echo("  To install with pip: %s" % fmt.bold(f"pip3 install '{qs.join(compiled_requirements)}'"))
+            fmt.echo("  To install with pip: %s" % fmt.bold(f"pip3 install '{qs.join(source_files.requirements)}'"))
         elif dependency_system == utils.PYPROJECT_TOML:
             fmt.echo("  If you are using poetry you may issue the following command:")
             fmt.echo(fmt.bold("  poetry add %s -E %s" % (DLT_PKG_NAME, destination_name)))
         fmt.echo()
     else:
         fmt.echo("* %s was created. Install it with:\npip3 install -r %s" % (fmt.bold(utils.REQUIREMENTS_TXT), utils.REQUIREMENTS_TXT))
 
@@ -146,20 +144,15 @@
     else:
         fmt.echo("* Read %s for more information" % fmt.bold("https://dlthub.com/docs/walkthroughs/add-a-verified-source"))
 
 
 def list_verified_sources_command(repo_location: str, branch: str = None) -> None:
     fmt.echo("Looking up for verified sources in %s..." % fmt.bold(repo_location))
     for source_name, source_files in _list_verified_sources(repo_location, branch).items():
-        reqs = source_files.requirements
-        dlt_req_string = str(reqs.dlt_requirement_base)
-        msg = "%s: %s" % (fmt.bold(source_name), source_files.doc)
-        if not reqs.is_installed_dlt_compatible():
-            msg += fmt.warning_style(" [needs update: %s]" % (dlt_req_string))
-        fmt.echo(msg)
+        fmt.echo("%s: %s" % (fmt.bold(source_name), source_files.doc))
 
 
 def init_command(source_name: str, destination_name: str, use_generic_template: bool, repo_location: str, branch: str = None) -> None:
     # try to import the destination and get config spec
     destination_reference = DestinationReference.from_name(destination_name)
     destination_spec = destination_reference.spec()
 
@@ -187,17 +180,15 @@
     # look for existing source
     source_files: VerifiedSourceFiles = None
     remote_index: TVerifiedSourceFileIndex = None
     if sources_storage.has_folder(source_name):
         # get pipeline files
         source_files = files_ops.get_verified_source_files(sources_storage, source_name)
         # get file index from remote verified source files being copied
-        remote_index = files_ops.get_remote_source_index(
-            source_files.storage.storage_path, source_files.files, source_files.requirements.dlt_version_constraint()
-        )
+        remote_index = files_ops.get_remote_source_index(source_files.storage.storage_path, source_files.files)
         # diff local and remote index to get modified and deleted files
         remote_new, remote_modified, remote_deleted = files_ops.gen_index_diff(local_index, remote_index)
         # find files that are modified locally
         conflict_modified, conflict_deleted = files_ops.find_conflict_files(local_index, remote_new, remote_modified, remote_deleted, dest_storage)
         # add new to modified
         remote_modified.update(remote_new)
         if conflict_modified or conflict_deleted:
@@ -221,33 +212,26 @@
     else:
         # normalize source name
         naming, _ = import_normalizers(default_normalizers())
         norm_source_name = naming.normalize_identifier(source_name)
         if norm_source_name != source_name:
             raise InvalidSchemaName(source_name, norm_source_name)
         dest_pipeline_script = norm_source_name + ".py"
-        source_files = VerifiedSourceFiles(True, init_storage, pipeline_script, dest_pipeline_script, template_files, SourceRequirements([]), "")
+        source_files = VerifiedSourceFiles(True, init_storage, pipeline_script, dest_pipeline_script, template_files, [], "")
         if dest_storage.has_file(dest_pipeline_script):
             fmt.warning("Pipeline script %s already exist, exiting" % dest_pipeline_script)
             return
 
     # add .dlt/*.toml files to be copied
     source_files.files.extend([make_dlt_settings_path(CONFIG_TOML), make_dlt_settings_path(SECRETS_TOML)])
 
     # add dlt extras line to requirements
-    source_files.requirements.update_dlt_extras(destination_name)
-
-    # Check compatibility with installed dlt
-    if not source_files.requirements.is_installed_dlt_compatible():
-        msg = f"This pipeline requires a newer version of dlt than your installed version ({source_files.requirements.current_dlt_version()}). " \
-            f"Pipeline requires '{source_files.requirements.dlt_requirement_base}'"
-        fmt.warning(msg)
-        if not fmt.confirm("Would you like to continue anyway? (you can update dlt after this step)", default=True):
-            fmt.echo(f'You can update dlt with: pip3 install -U "{source_files.requirements.dlt_requirement_base}"')
-            return
+    req_dep = f"{DLT_PKG_NAME}[{destination_name}]"
+    req_dep_line = f"{req_dep}>={pkg_version(DLT_PKG_NAME)}"
+    source_files.requirements.insert(0, req_dep_line)
 
     # read module source and parse it
     visitor = utils.parse_init_script("init", source_files.storage.load(source_files.pipeline_script), source_files.pipeline_script)
     if visitor.is_destination_imported:
         raise CliCommandException("init", f"The pipeline script {source_files.pipeline_script} import a destination from dlt.destinations. You should specify destinations by name when calling dlt.pipeline or dlt.run in init scripts.")
     if n.PIPELINE not in visitor.known_calls:
         raise CliCommandException("init", f"The pipeline script {source_files.pipeline_script} does not seem to initialize pipeline with dlt.pipeline. Please initialize pipeline explicitly in init scripts.")
@@ -356,9 +340,9 @@
     secrets_prov.write_toml()
     config_prov.write_toml()
 
     # telemetry_status_command()
 
     # if there's no dependency system write the requirements file
     if dependency_system is None:
-        requirements_txt = "\n".join(source_files.requirements.compiled())
+        requirements_txt = "\n".join(source_files.requirements)
         dest_storage.save(utils.REQUIREMENTS_TXT, requirements_txt)
```

### Comparing `dlt-0.3.6/dlt/cli/pipeline_command.py` & `dlt-0.3.6a0/dlt/cli/pipeline_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/cli/pipeline_files.py` & `dlt-0.3.6a0/dlt/cli/pipeline_files.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,45 +10,43 @@
 from dlt.common import git
 from dlt.common.configuration.paths import make_dlt_settings_path
 from dlt.common.storages import FileStorage
 
 from dlt.common.reflection.utils import get_module_docstring
 
 from dlt.cli import utils
-from dlt.cli.requirements import SourceRequirements
 
 
 SOURCES_INIT_INFO_ENGINE_VERSION = 1
 SOURCES_INIT_INFO_FILE = ".sources"
 IGNORE_FILES = ["*.py[cod]", "*$py.class", "__pycache__", "py.typed", "requirements.txt"]
 IGNORE_SOURCES = [".*", "_*"]
 
 
 class VerifiedSourceFiles(NamedTuple):
     is_template: bool
     storage: FileStorage
     pipeline_script: str
     dest_pipeline_script: str
     files: List[str]
-    requirements: SourceRequirements
+    requirements: List[str]
     doc: str
 
 
 class TVerifiedSourceFileEntry(TypedDict):
     commit_sha: str
     git_sha: str
     sha3_256: str
 
 
 class TVerifiedSourceFileIndex(TypedDict):
     is_dirty: bool
     last_commit_sha: str
     last_commit_timestamp: str
     files: Dict[str, TVerifiedSourceFileEntry]
-    dlt_version_constraint: str
 
 
 class TVerifiedSourcesFileIndex(TypedDict):
     engine_version: int
     sources: Dict[str, TVerifiedSourceFileIndex]
 
 
@@ -82,26 +80,24 @@
     # delete all deleted
     for deleted in remote_deleted:
         del local_index["files"][deleted]
     # update global info
     local_index["is_dirty"] = remote_index["is_dirty"]
     local_index["last_commit_sha"] = remote_index["last_commit_sha"]
     local_index["last_commit_timestamp"] = remote_index["last_commit_timestamp"]
-    local_index["dlt_version_constraint"] = remote_index["dlt_version_constraint"]
 
     return local_index
 
 
 def load_verified_sources_local_index(source_name: str) -> TVerifiedSourceFileIndex:
     return _load_dot_sources()["sources"].get(source_name, {
         "is_dirty": False,
         "last_commit_sha": None,
         "last_commit_timestamp": None,
-        "files": {},
-        "dlt_version_constraint": ">=0.1.0"
+        "files": {}
         }
     )
 
 
 def save_verified_source_local_index(
     source_name: str,
     remote_index: TVerifiedSourceFileIndex,
@@ -111,15 +107,15 @@
 
     all_sources = _load_dot_sources()
     local_index = all_sources["sources"].setdefault(source_name, remote_index)
     _merge_remote_index(local_index, remote_index, remote_modified, remote_deleted)
     _save_dot_sources(all_sources)
 
 
-def get_remote_source_index(repo_path: str, files: Sequence[str], dlt_version_constraint: str) -> TVerifiedSourceFileIndex:
+def get_remote_source_index(repo_path: str, files: Sequence[str]) -> TVerifiedSourceFileIndex:
 
     with git.get_repo(repo_path) as repo:
         tree = repo.tree()
         commit_sha = repo.head.commit.hexsha
         files_sha: Dict[str, TVerifiedSourceFileEntry] = {}
         for file in files:
             posix_file = os.path.join(repo_path, file)
@@ -139,16 +135,15 @@
                 "sha3_256":  hashlib.sha3_256(file_blob).hexdigest()
             }
 
         return {
             "is_dirty": git.is_dirty(repo),
             "last_commit_sha": commit_sha,
             "last_commit_timestamp": repo.head.commit.committed_datetime.isoformat(),
-            "files": files_sha,
-            "dlt_version_constraint": dlt_version_constraint
+            "files": files_sha
         }
 
 
 def get_verified_source_names(sources_storage: FileStorage) -> List[str]:
     candidates: List[str] = []
     for name in [n for n in sources_storage.list_folder_dirs(".", to_root=False) if not any(fnmatch.fnmatch(n, ignore) for ignore in IGNORE_SOURCES)]:
         # must contain at least one valid python script
@@ -179,17 +174,17 @@
     if sources_storage.has_file(init_py):
         docstring = get_module_docstring(sources_storage.load(init_py))
         if docstring:
             docstring = docstring.splitlines()[0]
     # read requirements
     requirements_path = os.path.join(source_name, utils.REQUIREMENTS_TXT)
     if sources_storage.has_file(requirements_path):
-        requirements = SourceRequirements.from_string(sources_storage.load(requirements_path))
+        requirements = sources_storage.load(requirements_path).splitlines()
     else:
-        requirements = SourceRequirements([])
+        requirements = []
     # find requirements
     return VerifiedSourceFiles(False, sources_storage, example_script, example_script, files, requirements, docstring)
 
 
 def gen_index_diff(
     local_index: TVerifiedSourceFileIndex,
     remote_index: TVerifiedSourceFileIndex
```

### Comparing `dlt-0.3.6/dlt/cli/source_detection.py` & `dlt-0.3.6a0/dlt/cli/source_detection.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/cli/telemetry_command.py` & `dlt-0.3.6a0/dlt/cli/telemetry_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/cli/utils.py` & `dlt-0.3.6a0/dlt/cli/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/arithmetics.py` & `dlt-0.3.6a0/dlt/common/arithmetics.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/configuration/accessors.py` & `dlt-0.3.6a0/dlt/common/configuration/accessors.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/configuration/container.py` & `dlt-0.3.6a0/dlt/common/configuration/container.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/configuration/exceptions.py` & `dlt-0.3.6a0/dlt/common/configuration/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/configuration/inject.py` & `dlt-0.3.6a0/dlt/common/configuration/inject.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/configuration/paths.py` & `dlt-0.3.6a0/dlt/common/configuration/paths.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/configuration/providers/airflow.py` & `dlt-0.3.6a0/dlt/common/configuration/providers/airflow.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/configuration/providers/context.py` & `dlt-0.3.6a0/dlt/common/configuration/providers/context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/configuration/providers/dictionary.py` & `dlt-0.3.6a0/dlt/common/configuration/providers/dictionary.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/configuration/providers/environ.py` & `dlt-0.3.6a0/dlt/common/configuration/providers/environ.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/configuration/providers/google_secrets.py` & `dlt-0.3.6a0/dlt/common/configuration/providers/google_secrets.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/configuration/providers/provider.py` & `dlt-0.3.6a0/dlt/common/configuration/providers/provider.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/configuration/providers/toml.py` & `dlt-0.3.6a0/dlt/common/configuration/providers/toml.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/configuration/resolve.py` & `dlt-0.3.6a0/dlt/common/configuration/resolve.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/configuration/specs/__init__.py` & `dlt-0.3.6a0/dlt/common/configuration/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/configuration/specs/api_credentials.py` & `dlt-0.3.6a0/dlt/common/configuration/specs/api_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/configuration/specs/aws_credentials.py` & `dlt-0.3.6a0/dlt/common/configuration/specs/aws_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/configuration/specs/base_configuration.py` & `dlt-0.3.6a0/dlt/common/configuration/specs/base_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/configuration/specs/config_providers_context.py` & `dlt-0.3.6a0/dlt/common/configuration/specs/config_providers_context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/configuration/specs/config_section_context.py` & `dlt-0.3.6a0/dlt/common/configuration/specs/config_section_context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/configuration/specs/connection_string_credentials.py` & `dlt-0.3.6a0/dlt/common/configuration/specs/connection_string_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/configuration/specs/exceptions.py` & `dlt-0.3.6a0/dlt/common/configuration/specs/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/configuration/specs/gcp_credentials.py` & `dlt-0.3.6a0/dlt/common/configuration/specs/gcp_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/configuration/specs/known_sections.py` & `dlt-0.3.6a0/dlt/common/configuration/specs/known_sections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/configuration/specs/run_configuration.py` & `dlt-0.3.6a0/dlt/common/configuration/specs/run_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/configuration/utils.py` & `dlt-0.3.6a0/dlt/common/configuration/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/data_types/type_helpers.py` & `dlt-0.3.6a0/dlt/common/data_types/type_helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/data_writers/buffered.py` & `dlt-0.3.6a0/dlt/common/data_writers/buffered.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,19 +86,14 @@
             # rotate on max file size
             if self.file_max_bytes and self._file.tell() >= self.file_max_bytes:
                 self._rotate_file()
             # rotate on max items
             elif self.file_max_items and self._writer.items_count >= self.file_max_items:
                 self._rotate_file()
 
-    def write_empty_file(self, columns: TTableSchemaColumns) -> None:
-        if columns is not None:
-            self._current_columns = dict(columns)
-        self._flush_items(allow_empty_file=True)
-
     def close(self) -> None:
         self._ensure_open()
         self._flush_and_close_file()
         self._closed = True
 
     @property
     def closed(self) -> bool:
@@ -110,28 +105,27 @@
     def __exit__(self, exc_type: Type[BaseException], exc_val: BaseException, exc_tb: Any) -> None:
         self.close()
 
     def _rotate_file(self) -> None:
         self._flush_and_close_file()
         self._file_name = self.file_name_template % uniq_id(5) + "." + self._file_format_spec.file_extension
 
-    def _flush_items(self, allow_empty_file: bool = False) -> None:
-        if len(self._buffered_items) > 0 or allow_empty_file:
+    def _flush_items(self) -> None:
+        if len(self._buffered_items) > 0:
             # we only open a writer when there are any items in the buffer and first flush is requested
             if not self._writer:
                 # create new writer and write header
                 if self._file_format_spec.is_binary_format:
                     self._file = self.open(self._file_name, "wb") # type: ignore
                 else:
                     self._file = self.open(self._file_name, "wt", encoding="utf-8") # type: ignore
                 self._writer = DataWriter.from_file_format(self.file_format, self._file, caps=self._caps)
                 self._writer.write_header(self._current_columns)
             # write buffer
-            if self._buffered_items:
-                self._writer.write_data(self._buffered_items)
+            self._writer.write_data(self._buffered_items)
             self._buffered_items.clear()
 
     def _flush_and_close_file(self) -> None:
         # if any buffered items exist, flush them
         self._flush_items()
         # if writer exists then close it
         if self._writer:
```

### Comparing `dlt-0.3.6/dlt/common/data_writers/escape.py` & `dlt-0.3.6a0/dlt/common/data_writers/escape.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/data_writers/exceptions.py` & `dlt-0.3.6a0/dlt/common/data_writers/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/data_writers/writers.py` & `dlt-0.3.6a0/dlt/common/data_writers/writers.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,16 +159,16 @@
             self._f.write(",\n")
 
         # write last row without separator so we can write footer eventually
         write_row(rows[-1])
         self._chunks_written += 1
 
     def write_footer(self) -> None:
-        if self._chunks_written > 0:
-            self._f.write(";")
+        assert self._chunks_written > 0
+        self._f.write(";")
 
     @classmethod
     def data_format(cls) -> TFileFormatSpec:
         return TFileFormatSpec(
             "insert_values",
             file_extension="insert_values",
             is_binary_format=False,
```

### Comparing `dlt-0.3.6/dlt/common/destination/capabilities.py` & `dlt-0.3.6a0/dlt/common/destination/capabilities.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/destination/reference.py` & `dlt-0.3.6a0/dlt/common/destination/reference.py`

 * *Files 4% similar despite different names*

```diff
@@ -169,33 +169,28 @@
             Optional[TSchemaTables]: Returns an update that was applied at the destination.
         """
         self._verify_schema()
         return expected_update
 
     @abstractmethod
     def start_file_load(self, table: TTableSchema, file_path: str, load_id: str) -> LoadJob:
-        """Creates and starts a load job for a particular `table` with content in `file_path`"""
+        """Creates a job for a particular `table` with content in `file_path`"""
         pass
 
     @abstractmethod
     def restore_file_load(self, file_path: str) -> LoadJob:
-        """Finds and restores already started loading job identified by `file_path` if destination supports it."""
         pass
 
-    def get_truncate_destination_table_dispositions(self) -> List[TWriteDisposition]:
-        # in the base job, all replace strategies are treated the same, see filesystem for example
-        return ["replace"]
-
+    @abstractmethod
     def create_table_chain_completed_followup_jobs(self, table_chain: Sequence[TTableSchema]) -> List[NewLoadJob]:
         """Creates a list of followup jobs that should be executed after a table chain is completed"""
         return []
 
     @abstractmethod
     def complete_load(self, load_id: str) -> None:
-        """Marks the load package with `load_id` as completed in the destination. Before such commit is done, the data with `load_id` is invalid."""
         pass
 
     @abstractmethod
     def __enter__(self) -> "JobClientBase":
         pass
 
     @abstractmethod
@@ -219,14 +214,15 @@
                         self.config.destination_name,
                         "column",
                         f"{table_name}.{column_name}",
                         self.capabilities.max_column_identifier_length
                     )
                 if not is_complete_column(column):
                     logger.warning(f"A column {column_name} in table {table_name} in schema {self.schema.name} is incomplete. It was not bound to the data during normalizations stage and its data type is unknown. Did you add this column manually in code ie. as a merge key?")
+                    table["columns"].pop(column_name)
 
     @staticmethod
     def make_dataset_name(schema: Schema, dataset_name: str, default_schema_name: str) -> str:
         """Builds full db dataset (dataset) name out of (normalized) default dataset and schema name"""
         if not schema.name:
             raise ValueError("schema_name is None or empty")
         if not dataset_name:
@@ -240,38 +236,35 @@
 
         return norm_name
 
 class StagingJobClientBase(JobClientBase):
 
     @abstractmethod
     def get_stage_dispositions(self) -> List[TWriteDisposition]:
-        """Returns a list of write dispositions that require staging dataset"""
         return []
 
     @abstractmethod
     def with_staging_dataset(self)-> ContextManager["JobClientBase"]:
-        """Executes job client methods on staging dataset"""
         return self
 
 
 TDestinationReferenceArg = Union["DestinationReference", ModuleType, None, str]
 
 
 class DestinationReference(Protocol):
     __name__: str
-    """Name of the destination"""
 
     def capabilities(self) -> DestinationCapabilitiesContext:
-        """Destination capabilities ie. supported loader file formats, identifier name lengths, naming conventions, escape function etc."""
+        ...
 
     def client(self, schema: Schema, initial_config: DestinationClientConfiguration = config.value) -> "JobClientBase":
-        """A job client responsible for starting and resuming load jobs"""
+        ...
 
     def spec(self) -> Type[DestinationClientConfiguration]:
-        """A spec of destination configuration that also contains destination credentials"""
+        ...
 
     @staticmethod
     def from_name(destination: TDestinationReferenceArg) -> "DestinationReference":
         if destination is None:
             return None
 
         # if destination is a str, get destination reference by dynamically importing module
@@ -280,22 +273,15 @@
                 if "." in destination:
                     # this is full module name
                     destination_ref = cast(DestinationReference, import_module(destination))
                 else:
                     # from known location
                     destination_ref = cast(DestinationReference, import_module(f"dlt.destinations.{destination}"))
             except ImportError:
-                if "." in destination:
-                    raise UnknownDestinationModule(destination)
-                else:
-                    # allow local external module imported without dot
-                    try:
-                        destination_ref = cast(DestinationReference, import_module(destination))
-                    except ImportError:
-                        raise UnknownDestinationModule(destination)
+                raise UnknownDestinationModule(destination)
         else:
             destination_ref = cast(DestinationReference, destination)
 
         # make sure the reference is correct
         try:
             c = destination_ref.spec()
             c.credentials
```

### Comparing `dlt-0.3.6/dlt/common/exceptions.py` & `dlt-0.3.6a0/dlt/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/git.py` & `dlt-0.3.6a0/dlt/common/git.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/json/__init__.py` & `dlt-0.3.6a0/dlt/common/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/json/_orjson.py` & `dlt-0.3.6a0/dlt/common/json/_orjson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/json/_simplejson.py` & `dlt-0.3.6a0/dlt/common/json/_simplejson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/jsonpath.py` & `dlt-0.3.6a0/dlt/common/jsonpath.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/libs/pyarrow.py` & `dlt-0.3.6a0/dlt/common/libs/pyarrow.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/normalizers/configuration.py` & `dlt-0.3.6a0/dlt/common/normalizers/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/normalizers/json/__init__.py` & `dlt-0.3.6a0/dlt/common/normalizers/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/normalizers/json/relational.py` & `dlt-0.3.6a0/dlt/common/normalizers/json/relational.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/normalizers/naming/direct.py` & `dlt-0.3.6a0/dlt/common/normalizers/naming/direct.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/normalizers/naming/duck_case.py` & `dlt-0.3.6a0/dlt/common/normalizers/naming/duck_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/normalizers/naming/exceptions.py` & `dlt-0.3.6a0/dlt/common/normalizers/naming/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/normalizers/naming/naming.py` & `dlt-0.3.6a0/dlt/common/normalizers/naming/naming.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/normalizers/naming/snake_case.py` & `dlt-0.3.6a0/dlt/common/normalizers/naming/snake_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/normalizers/utils.py` & `dlt-0.3.6a0/dlt/common/normalizers/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/pipeline.py` & `dlt-0.3.6a0/dlt/common/pipeline.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/reflection/spec.py` & `dlt-0.3.6a0/dlt/common/reflection/spec.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/reflection/utils.py` & `dlt-0.3.6a0/dlt/common/reflection/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/runners/configuration.py` & `dlt-0.3.6a0/dlt/common/runners/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/runners/pool_runner.py` & `dlt-0.3.6a0/dlt/common/runners/pool_runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/runners/runnable.py` & `dlt-0.3.6a0/dlt/common/runners/runnable.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/runners/stdout.py` & `dlt-0.3.6a0/dlt/common/runners/stdout.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/runners/synth_pickle.py` & `dlt-0.3.6a0/dlt/common/runners/synth_pickle.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/runners/venv.py` & `dlt-0.3.6a0/dlt/common/runners/venv.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/runtime/collector.py` & `dlt-0.3.6a0/dlt/common/runtime/collector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/runtime/exec_info.py` & `dlt-0.3.6a0/dlt/common/runtime/exec_info.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/runtime/init.py` & `dlt-0.3.6a0/dlt/common/runtime/init.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/runtime/logger.py` & `dlt-0.3.6a0/dlt/common/runtime/logger.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/runtime/prometheus.py` & `dlt-0.3.6a0/dlt/common/runtime/prometheus.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/runtime/segment.py` & `dlt-0.3.6a0/dlt/common/runtime/segment.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/runtime/sentry.py` & `dlt-0.3.6a0/dlt/common/runtime/sentry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/runtime/signals.py` & `dlt-0.3.6a0/dlt/common/runtime/signals.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/runtime/slack.py` & `dlt-0.3.6a0/dlt/common/runtime/slack.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/runtime/telemetry.py` & `dlt-0.3.6a0/dlt/common/runtime/telemetry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/schema/detections.py` & `dlt-0.3.6a0/dlt/common/schema/detections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/schema/exceptions.py` & `dlt-0.3.6a0/dlt/common/schema/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/schema/schema.py` & `dlt-0.3.6a0/dlt/common/schema/schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -199,15 +199,15 @@
         self._stored_version, self._stored_version_hash = version
         return version
 
     def filter_row_with_hint(self, table_name: str, hint_type: TColumnHint, row: StrAny) -> StrAny:
         rv_row: DictStrAny = {}
         column_prop: TColumnProp = utils.hint_to_column_prop(hint_type)
         try:
-            table = self.get_table_columns(table_name, include_incomplete=True)
+            table = self.get_table_columns(table_name)
             for column_name in table:
                 if column_name in row:
                     hint_value = table[column_name][column_prop]
                     if (hint_value and column_prop != "nullable") or (column_prop == "nullable" and not hint_value):
                         rv_row[column_name] = row[column_name]
         except KeyError:
             for k, v in row.items():
@@ -242,32 +242,32 @@
         if columns:
             for c in columns.values():
                 c["name"] = self.naming.normalize_path(c["name"])
             # re-index columns as the name changed
             table["columns"] = {c["name"]:c for c in columns.values()}
         return table
 
-    def get_new_table_columns(self, table_name: str, exiting_columns: TTableSchemaColumns, include_incomplete: bool = False) -> List[TColumnSchema]:
-        """Gets new columns to be added to `exiting_columns` to bring them to date with `table_name` schema. Optionally includes incomplete columns (without data type)"""
+    def get_new_complete_columns(self, table_name: str, t: TTableSchemaColumns) -> List[TColumnSchema]:
+        """Gets new columns to be added to "t" to bring up to date with stored schema. Exclude incomplete columns (without data type)"""
         diff_c: List[TColumnSchema] = []
-        s_t = self.get_table_columns(table_name, include_incomplete=include_incomplete)
+        s_t = self.get_table_columns(table_name, only_complete=True)
         for c in s_t.values():
-            if c["name"] not in exiting_columns:
+            if c["name"] not in t:
                 diff_c.append(c)
         return diff_c
 
     def get_table(self, table_name: str) -> TTableSchema:
         return self._schema_tables[table_name]
 
-    def get_table_columns(self, table_name: str, include_incomplete: bool = False) -> TTableSchemaColumns:
-        """Gets columns of `table_name`. Optionally includes incomplete columns """
-        if include_incomplete:
-            return self._schema_tables[table_name]["columns"]
-        else:
+    def get_table_columns(self, table_name: str, only_complete: bool = False) -> TTableSchemaColumns:
+        """Gets columns of `table_name`"""
+        if only_complete:
             return {k:v for k, v in self._schema_tables[table_name]["columns"].items() if utils.is_complete_column(v)}
+        else:
+            return self._schema_tables[table_name]["columns"]
 
     def data_tables(self, include_incomplete: bool = False) -> List[TTableSchema]:
         """Gets list of all tables, that hold the loaded data. Excludes dlt tables. Excludes incomplete tables (ie. without columns)"""
         return [t for t in self._schema_tables.values() if not t["name"].startswith("_dlt") and (len(t["columns"]) > 0 or include_incomplete)]
 
     def dlt_tables(self) -> List[TTableSchema]:
         """Gets dlt tables"""
@@ -293,20 +293,18 @@
         Returns:
             int: Stored schema version
         """
         return self._stored_version
 
     @property
     def version_hash(self) -> str:
-        """Current version hash of the schema, recomputed from the actual content"""
         return utils.bump_version_if_modified(self.to_dict())[1]
 
     @property
     def stored_version_hash(self) -> str:
-        """Version hash of the schema content form the time of schema loading/creation."""
         return self._stored_version_hash
 
     @property
     def name(self) -> str:
         return self._schema_name
 
     @property
```

### Comparing `dlt-0.3.6/dlt/common/schema/typing.py` & `dlt-0.3.6a0/dlt/common/schema/typing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Callable, Dict, List, Literal, Optional, Sequence, Set, Type, TypedDict, NewType, Union, get_args
 
 from dlt.common.data_types import TDataType
 from dlt.common.normalizers.typing import TNormalizersConfig
 
 # current version of schema engine
-SCHEMA_ENGINE_VERSION = 6
+SCHEMA_ENGINE_VERSION = 5
 
 # dlt tables
 VERSION_TABLE_NAME = "_dlt_version"
 LOADS_TABLE_NAME = "_dlt_loads"
 
 TColumnHint = Literal["not_null", "partition", "cluster", "primary_key", "foreign_key", "sort", "unique", "root_key", "merge_key"]
 TColumnProp = Literal["name", "data_type", "nullable", "partition", "cluster", "primary_key", "foreign_key", "sort", "unique", "merge_key", "root_key"]
```

### Comparing `dlt-0.3.6/dlt/common/schema/utils.py` & `dlt-0.3.6a0/dlt/common/schema/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,19 +254,14 @@
         schema_dict.setdefault("version_hash", "")
         from_engine = 4
     if from_engine == 4 and to_engine > 4:
         # replace schema versions table
         schema_dict["tables"][VERSION_TABLE_NAME] = version_table()
         schema_dict["tables"][LOADS_TABLE_NAME] = load_table()
         from_engine = 5
-    if from_engine == 5 and to_engine > 5:
-        # replace loads table
-        schema_dict["tables"][LOADS_TABLE_NAME] = load_table()
-        from_engine = 6
-
 
     schema_dict["engine_version"] = from_engine
     if from_engine != to_engine:
         raise SchemaEngineNoUpgradePathException(schema_dict["name"], schema_dict["engine_version"], from_engine, to_engine)
 
     return cast(TStoredSchema, schema_dict)
 
@@ -388,18 +383,18 @@
 
 def hint_to_column_prop(h: TColumnHint) -> TColumnProp:
     if h == "not_null":
         return "nullable"
     return h
 
 
-def get_columns_names_with_prop(table: TTableSchema, column_prop: TColumnProp, include_incomplete: bool = False) -> List[str]:
+def get_columns_names_with_prop(table: TTableSchema, column_prop: TColumnProp, only_completed: bool = False) -> List[str]:
     # column_prop: TColumnProp = hint_to_column_prop(hint_type)
     # default = column_prop != "nullable"  # default is true, only for nullable false
-    return [c["name"] for c in table["columns"].values() if bool(c.get(column_prop, False)) is True and (include_incomplete or is_complete_column(c))]
+    return [c["name"] for c in table["columns"].values() if c.get(column_prop, False) is True and (not only_completed or is_complete_column(c))]
 
 
 def merge_schema_updates(schema_updates: Sequence[TSchemaUpdate]) -> TSchemaTables:
     aggregated_update: TSchemaTables = {}
     for schema_update in schema_updates:
         for table_name, table_updates in schema_update.items():
             for partial_table in table_updates:
@@ -421,15 +416,15 @@
         return get_write_disposition(tables, parent)
 
     raise ValueError(f"No write disposition found in the chain of tables for '{table_name}'.")
 
 
 def table_schema_has_type(table: TTableSchema, _typ: TDataType) -> bool:
     """Checks if `table` schema contains column with type _typ"""
-    return any(c.get("data_type") == _typ for c in table["columns"].values())
+    return any(c["data_type"] == _typ for c in table["columns"].values())
 
 
 def get_top_level_table(tables: TSchemaTables, table_name: str) -> TTableSchema:
     """Finds top level (without parent) of a `table_name` following the ancestry hierarchy."""
     table = tables[table_name]
     parent = table.get("parent")
     if parent:
@@ -462,16 +457,14 @@
         if resource and (pattern is None or pattern.match(resource)):
             resource_tables = result.setdefault(resource, [])
             resource_tables.extend(get_child_tables(tables, table['name']))
     return result
 
 
 def version_table() -> TTableSchema:
-    # NOTE: always add new columns at the end of the table so we have identical layout
-    # after an update of existing tables (always at the end)
     table = new_table(VERSION_TABLE_NAME, columns=[
             add_missing_hints({
                 "name": "version",
                 "data_type": "bigint",
                 "nullable": False,
             }),
             add_missing_hints({
@@ -503,16 +496,14 @@
     )
     table["write_disposition"] = "skip"
     table["description"] = "Created by DLT. Tracks schema updates"
     return table
 
 
 def load_table() -> TTableSchema:
-    # NOTE: always add new columns at the end of the table so we have identical layout
-    # after an update of existing tables (always at the end)
     table = new_table(LOADS_TABLE_NAME, columns=[
             add_missing_hints({
                 "name": "load_id",
                 "data_type": "text",
                 "nullable": False
             }),
             add_missing_hints({
@@ -525,20 +516,15 @@
                 "data_type": "bigint",
                 "nullable": False
             }),
             add_missing_hints({
                 "name": "inserted_at",
                 "data_type": "timestamp",
                 "nullable": False
-            }),
-            add_missing_hints({
-                "name": "schema_version_hash",
-                "data_type": "text",
-                "nullable": True,
-            }),
+            })
         ]
     )
     table["write_disposition"] = "skip"
     table["description"] = "Created by DLT. Tracks completed loads"
     return table
```

### Comparing `dlt-0.3.6/dlt/common/source.py` & `dlt-0.3.6a0/dlt/common/source.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/storages/__init__.py` & `dlt-0.3.6a0/dlt/common/storages/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/storages/configuration.py` & `dlt-0.3.6a0/dlt/common/storages/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/storages/data_item_storage.py` & `dlt-0.3.6a0/dlt/common/storages/data_item_storage.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,34 +9,26 @@
 
 class DataItemStorage(ABC):
     def __init__(self, load_file_type: TLoaderFileFormat, *args: Any) -> None:
         self.loader_file_format = load_file_type
         self.buffered_writers: Dict[str, BufferedDataWriter] = {}
         super().__init__(*args)
 
-    def get_writer(self, load_id: str, schema_name: str, table_name: str) -> BufferedDataWriter:
+    def write_data_item(self, load_id: str, schema_name: str, table_name: str, item: TDataItems, columns: TTableSchemaColumns) -> None:
         # unique writer id
         writer_id = f"{load_id}.{schema_name}.{table_name}"
         writer = self.buffered_writers.get(writer_id, None)
         if not writer:
             # assign a jsonl writer for each table
             path = self._get_data_item_path_template(load_id, schema_name, table_name)
             writer = BufferedDataWriter(self.loader_file_format, path)
             self.buffered_writers[writer_id] = writer
-        return writer
-
-    def write_data_item(self, load_id: str, schema_name: str, table_name: str, item: TDataItems, columns: TTableSchemaColumns) -> None:
-        writer = self.get_writer(load_id, schema_name, table_name)
         # write item(s)
         writer.write_data_item(item, columns)
 
-    def write_empty_file(self, load_id: str, schema_name: str, table_name: str, columns: TTableSchemaColumns) -> None:
-        writer = self.get_writer(load_id, schema_name, table_name)
-        writer.write_empty_file(columns)
-
     def close_writers(self, extract_id: str) -> None:
         # flush and close all files
         for name, writer in self.buffered_writers.items():
             if name.startswith(extract_id):
                 logger.debug(f"Closing writer for {name} with file {writer._file} and actual name {writer._file_name}")
                 writer.close()
```

### Comparing `dlt-0.3.6/dlt/common/storages/exceptions.py` & `dlt-0.3.6a0/dlt/common/storages/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/storages/file_storage.py` & `dlt-0.3.6a0/dlt/common/storages/file_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/storages/live_schema_storage.py` & `dlt-0.3.6a0/dlt/common/storages/live_schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/storages/load_storage.py` & `dlt-0.3.6a0/dlt/common/storages/load_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/storages/normalize_storage.py` & `dlt-0.3.6a0/dlt/common/storages/normalize_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/storages/schema_storage.py` & `dlt-0.3.6a0/dlt/common/storages/schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/storages/transactional_file.py` & `dlt-0.3.6a0/dlt/common/storages/transactional_file.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/storages/versioned_storage.py` & `dlt-0.3.6a0/dlt/common/storages/versioned_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/time.py` & `dlt-0.3.6a0/dlt/common/time.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/typing.py` & `dlt-0.3.6a0/dlt/common/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/utils.py` & `dlt-0.3.6a0/dlt/common/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/validation.py` & `dlt-0.3.6a0/dlt/common/validation.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/common/wei.py` & `dlt-0.3.6a0/dlt/common/wei.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/destinations/bigquery/__init__.py` & `dlt-0.3.6a0/dlt/destinations/bigquery/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 def _configure(config: BigQueryClientConfiguration = config.value) -> BigQueryClientConfiguration:
     return config
 
 
 def capabilities() -> DestinationCapabilitiesContext:
     caps = DestinationCapabilitiesContext()
     caps.preferred_loader_file_format = "jsonl"
-    caps.supported_loader_file_formats = ["jsonl", "parquet"]
+    caps.supported_loader_file_formats = ["jsonl", "sql", "parquet"]
     caps.preferred_staging_file_format = "parquet"
     caps.supported_staging_file_formats = ["parquet", "jsonl"]
     caps.escape_identifier = escape_bigquery_identifier
     caps.escape_literal = None
     caps.decimal_precision = (DEFAULT_NUMERIC_PRECISION, DEFAULT_NUMERIC_SCALE)
     caps.wei_precision = (76, 38)
     caps.max_identifier_length = 1024
```

### Comparing `dlt-0.3.6/dlt/destinations/bigquery/bigquery.py` & `dlt-0.3.6a0/dlt/destinations/bigquery/bigquery.py`

 * *Files 5% similar despite different names*

```diff
@@ -182,17 +182,18 @@
         return job
 
     def start_file_load(self, table: TTableSchema, file_path: str, load_id: str) -> LoadJob:
         job = super().start_file_load(table, file_path, load_id)
 
         if not job:
             try:
+                disposition = table["write_disposition"]
                 job = BigQueryLoadJob(
                     FileStorage.get_file_name_from_file_path(file_path),
-                    self._create_load_job(table, file_path),
+                    self._create_load_job(table, disposition in self.get_stage_dispositions(), self._should_truncate_destination_table(disposition), file_path),
                     self.config.http_timeout,
                     self.config.retry_deadline
                 )
             except api_core_exceptions.GoogleAPICallError as gace:
                 reason = BigQuerySqlClient._get_reason_from_errors(gace)
                 if reason == "notFound":
                     # google.api_core.exceptions.NotFound: 404 - table not found
@@ -251,16 +252,17 @@
                     "partition": c.name == partition_field
                 }
                 schema_table[c.name] = schema_c
             return True, schema_table
         except gcp_exceptions.NotFound:
             return False, schema_table
 
-    def _create_load_job(self, table: TTableSchema, file_path: str) -> bigquery.LoadJob:
+    def _create_load_job(self, table: TTableSchema, use_staging_table: bool, _should_truncate_destination_table: bool, file_path: str) -> bigquery.LoadJob:
         # append to table for merge loads (append to stage) and regular appends
+        bq_wd = bigquery.WriteDisposition.WRITE_TRUNCATE if _should_truncate_destination_table else bigquery.WriteDisposition.WRITE_APPEND
         table_name = table["name"]
 
         # determine wether we load from local or uri
         bucket_path = None
         ext: str = os.path.splitext(file_path)[1][1:]
         if NewReferenceJob.is_reference_job(file_path):
             bucket_path = NewReferenceJob.resolve_reference(file_path)
@@ -273,41 +275,43 @@
             # if table contains complex types, we cannot load with parquet
             if table_schema_has_type(table, "complex"):
                 raise LoadJobTerminalException(file_path, "Bigquery cannot load into JSON data type from parquet. Use jsonl instead.")
             source_format = bigquery.SourceFormat.PARQUET
             # parquet needs NUMERIC type autodetection
             decimal_target_types = ["NUMERIC", "BIGNUMERIC"]
 
-        job_id = BigQueryLoadJob.get_job_id_from_file_path(file_path)
-        job_config = bigquery.LoadJobConfig(
-            autodetect=False,
-            write_disposition=bigquery.WriteDisposition.WRITE_APPEND,
-            create_disposition=bigquery.CreateDisposition.CREATE_NEVER,
-            source_format=source_format,
-            decimal_target_types=decimal_target_types,
-            ignore_unknown_values=False,
-            max_bad_records=0)
-
-        if bucket_path:
-            return self.sql_client.native_connection.load_table_from_uri(
-                    bucket_path,
-                    self.sql_client.make_qualified_table_name(table_name, escape=False),
-                    job_id=job_id,
-                    job_config=job_config,
-                    timeout=self.config.file_upload_timeout
-                )
-
-        with open(file_path, "rb") as f:
-            return self.sql_client.native_connection.load_table_from_file(
-                    f,
-                    self.sql_client.make_qualified_table_name(table_name, escape=False),
-                    job_id=job_id,
-                    job_config=job_config,
-                    timeout=self.config.file_upload_timeout
-                )
+        # if merge then load to staging
+        with self.sql_client.with_staging_dataset(use_staging_table):
+            job_id = BigQueryLoadJob.get_job_id_from_file_path(file_path)
+            job_config = bigquery.LoadJobConfig(
+                autodetect=False,
+                write_disposition=bq_wd,
+                create_disposition=bigquery.CreateDisposition.CREATE_NEVER,
+                source_format=source_format,
+                decimal_target_types=decimal_target_types,
+                ignore_unknown_values=False,
+                max_bad_records=0)
+
+            if bucket_path:
+                return self.sql_client.native_connection.load_table_from_uri(
+                        bucket_path,
+                        self.sql_client.make_qualified_table_name(table_name, escape=False),
+                        job_id=job_id,
+                        job_config=job_config,
+                        timeout=self.config.file_upload_timeout
+                    )
+
+            with open(file_path, "rb") as f:
+                return self.sql_client.native_connection.load_table_from_file(
+                        f,
+                        self.sql_client.make_qualified_table_name(table_name, escape=False),
+                        job_id=job_id,
+                        job_config=job_config,
+                        timeout=self.config.file_upload_timeout
+                    )
 
     def _retrieve_load_job(self, file_path: str) -> bigquery.LoadJob:
         job_id = BigQueryLoadJob.get_job_id_from_file_path(file_path)
         return cast(bigquery.LoadJob, self.sql_client.native_connection.get_job(job_id))
 
     @classmethod
     def _to_db_type(cls, sc_t: TDataType) -> str:
```

### Comparing `dlt-0.3.6/dlt/destinations/bigquery/configuration.py` & `dlt-0.3.6a0/dlt/destinations/bigquery/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/destinations/bigquery/sql_client.py` & `dlt-0.3.6a0/dlt/destinations/bigquery/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/destinations/duckdb/__init__.py` & `dlt-0.3.6a0/dlt/destinations/duckdb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 def _configure(config: DuckDbClientConfiguration = config.value) -> DuckDbClientConfiguration:
     return config
 
 
 def capabilities() -> DestinationCapabilitiesContext:
     caps = DestinationCapabilitiesContext()
     caps.preferred_loader_file_format = "insert_values"
-    caps.supported_loader_file_formats = ["insert_values", "parquet", "jsonl"]
+    caps.supported_loader_file_formats = ["insert_values", "parquet", "sql"]
     caps.preferred_staging_file_format = None
     caps.supported_staging_file_formats = []
     caps.escape_identifier = escape_postgres_identifier
     caps.escape_literal = escape_duckdb_literal
     caps.decimal_precision = (DEFAULT_NUMERIC_PRECISION, DEFAULT_NUMERIC_SCALE)
     caps.wei_precision = (DEFAULT_NUMERIC_PRECISION, 0)
     caps.max_identifier_length = 65536
```

### Comparing `dlt-0.3.6/dlt/destinations/duckdb/configuration.py` & `dlt-0.3.6a0/dlt/destinations/duckdb/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/destinations/duckdb/duck.py` & `dlt-0.3.6a0/dlt/destinations/duckdb/duck.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,27 +40,23 @@
 
 HINT_TO_POSTGRES_ATTR: Dict[TColumnHint, str] = {
     "unique": "UNIQUE"
 }
 
 
 class DuckDbCopyJob(LoadJob, FollowupJob):
-    def __init__(self, table_name: str, file_path: str, sql_client: DuckDbSqlClient) -> None:
+    def __init__(self, table_name: str, use_staging_table: bool, _should_truncate_destination_table: bool, file_path: str, sql_client: DuckDbSqlClient) -> None:
         super().__init__(FileStorage.get_file_name_from_file_path(file_path))
 
-        if file_path.endswith("parquet"):
-            source_format = "PARQUET"
-        elif file_path.endswith("jsonl"):
-            # NOTE: loading JSON does not work in practice on duckdb: the missing keys fail the load instead of being interpreted as NULL
-            source_format = "JSON"  # newline delimited, compression auto
-        else:
-            raise ValueError(file_path)
-        qualified_table_name = sql_client.make_qualified_table_name(table_name)
-        with sql_client.begin_transaction():
-            sql_client.execute_sql(f"COPY {qualified_table_name} FROM '{file_path}' ( FORMAT {source_format} );")
+        with sql_client.with_staging_dataset(use_staging_table):
+            qualified_table_name = sql_client.make_qualified_table_name(table_name)
+            with sql_client.begin_transaction():
+                if _should_truncate_destination_table:
+                    sql_client.execute_sql(f"TRUNCATE TABLE {qualified_table_name}")
+                sql_client.execute_sql(f"COPY {qualified_table_name} FROM '{file_path}' ( FORMAT PARQUET );")
 
 
     def state(self) -> TLoadJobState:
         return "completed"
 
     def exception(self) -> str:
         raise NotImplementedError()
@@ -76,18 +72,18 @@
         )
         super().__init__(schema, config, sql_client)
         self.config: DuckDbClientConfiguration = config
         self.sql_client: DuckDbSqlClient = sql_client  # type: ignore
         self.active_hints = HINT_TO_POSTGRES_ATTR if self.config.create_indexes else {}
 
     def start_file_load(self, table: TTableSchema, file_path: str, load_id: str) -> LoadJob:
-        job = super().start_file_load(table, file_path, load_id)
-        if not job:
-            job = DuckDbCopyJob(table["name"], file_path, self.sql_client)
-        return job
+        if file_path.endswith("parquet"):
+            disposition = table["write_disposition"]
+            return DuckDbCopyJob(table["name"], disposition in self.get_stage_dispositions(), self._should_truncate_destination_table(disposition), file_path, self.sql_client)
+        return super().start_file_load(table, file_path, load_id)
 
     def _get_column_def_sql(self, c: TColumnSchema) -> str:
         hints_str = " ".join(self.active_hints.get(h, "") for h in self.active_hints.keys() if c.get(h, False) is True)
         column_name = self.capabilities.escape_identifier(c["name"])
         return f"{column_name} {self._to_db_type(c['data_type'])} {hints_str} {self._gen_not_null(c['nullable'])}"
 
     @classmethod
```

### Comparing `dlt-0.3.6/dlt/destinations/duckdb/sql_client.py` & `dlt-0.3.6a0/dlt/destinations/duckdb/sql_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,14 +87,20 @@
     def rollback_transaction(self) -> None:
         self._conn.rollback()
 
     @property
     def native_connection(self) -> duckdb.DuckDBPyConnection:
         return self._conn
 
+    def create_dataset(self) -> None:
+        self.execute_sql("CREATE SCHEMA %s" % self.fully_qualified_dataset_name())
+
+    def drop_dataset(self) -> None:
+        self.execute_sql("DROP SCHEMA %s CASCADE;" % self.fully_qualified_dataset_name())
+
     def execute_sql(self, sql: AnyStr, *args: Any, **kwargs: Any) -> Optional[Sequence[Sequence[Any]]]:
         with self.execute_query(sql, *args, **kwargs) as curr:
             if curr.description is None:
                 return None
             else:
                 f = curr.fetchall()
                 return f
```

### Comparing `dlt-0.3.6/dlt/destinations/dummy/__init__.py` & `dlt-0.3.6a0/dlt/destinations/dummy/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/destinations/dummy/configuration.py` & `dlt-0.3.6a0/dlt/destinations/dummy/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/destinations/dummy/dummy.py` & `dlt-0.3.6a0/dlt/destinations/dummy/dummy.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/destinations/exceptions.py` & `dlt-0.3.6a0/dlt/destinations/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,22 +41,14 @@
 class DestinationSchemaWillNotUpdate(DestinationTerminalException):
     def __init__(self, table_name: str, columns: Sequence[str], msg: str) -> None:
         self.table_name = table_name
         self.columns = columns
         super().__init__(f"Schema for table {table_name} column(s) {columns} will not update: {msg}")
 
 
-class DestinationSchemaTampered(DestinationTerminalException):
-    def __init__(self, schema_name: str, version_hash: str, stored_version_hash: str) -> None:
-        self.version_hash = version_hash
-        self.stored_version_hash = stored_version_hash
-        super().__init__(f"Schema {schema_name} content was changed - by a loader or by destination code - from the moment it was retrieved by load package. "
-                         f"Such schema cannot reliably be updated or saved. Current version hash: {version_hash} != stored version hash {stored_version_hash}")
-
-
 class LoadJobNotExistsException(DestinationTerminalException):
     def __init__(self, job_id: str) -> None:
         super().__init__(f"Job with id/file name {job_id} not found")
 
 
 class LoadJobTerminalException(DestinationTerminalException):
     def __init__(self, file_path: str, message: str) -> None:
```

### Comparing `dlt-0.3.6/dlt/destinations/filesystem/__init__.py` & `dlt-0.3.6a0/dlt/destinations/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/destinations/filesystem/configuration.py` & `dlt-0.3.6a0/dlt/destinations/filesystem/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/destinations/filesystem/filesystem.py` & `dlt-0.3.6a0/dlt/destinations/filesystem/filesystem.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,15 +34,39 @@
         file_name = FileStorage.get_file_name_from_file_path(local_path)
         self.config = config
         self.dataset_path = dataset_path
         self.destination_file_name = LoadFilesystemJob.make_destination_filename(file_name, schema_name, load_id)
 
         super().__init__(file_name)
         fs_client, _ = client_from_config(config)
-        self.destination_file_name = LoadFilesystemJob.make_destination_filename(file_name, schema_name, load_id)
+
+        # fallback to replace for merge without any merge keys
+        if write_disposition == 'merge':
+            write_disposition = 'append' if has_merge_keys else 'replace'
+
+        # replace existing files. also check if dir exists for bucket storages that cannot create dirs
+        if write_disposition == 'replace' and fs_client.isdir(dataset_path):
+            job_info = LoadStorage.parse_job_file_name(file_name)
+            # remove those files
+            search_prefix = posixpath.join(dataset_path, f"{schema_name}.{job_info.table_name}.")
+            # but leave actual load id - files may be loaded from other threads
+            ignore_prefix = posixpath.join(dataset_path, f"{schema_name}.{job_info.table_name}.{load_id}.")
+            # NOTE: glob implementation in fsspec does not look thread safe, way better is to use ls and then filter
+            all_files: List[str] = fs_client.ls(dataset_path, detail=False, refresh=True)
+            items = [item for item in all_files if item.startswith(search_prefix) and not item.startswith(ignore_prefix)]
+            # NOTE: deleting in chunks on s3 does not raise on access denied, file non existing and probably other errors
+            # if items:
+            #     fs_client.rm(items[0])
+            for item in items:
+                # ignore file not found as we can have races from other deleting threads
+                try:
+                    fs_client.rm_file(item)
+                except FileNotFoundError:
+                    pass
+
         fs_client.put_file(local_path, self.make_remote_path())
 
     @staticmethod
     def make_destination_filename(file_name: str, schema_name: str, load_id: str) -> str:
         job_info = LoadStorage.parse_job_file_name(file_name)
         return f"{schema_name}.{job_info.table_name}.{load_id}.{job_info.file_id}.{job_info.file_format}"
 
@@ -78,26 +102,14 @@
         self.config: FilesystemClientConfiguration = config
 
     @property
     def dataset_path(self) -> str:
         return posixpath.join(self.fs_path, self.config.dataset_name)
 
     def initialize_storage(self, truncate_tables: Iterable[str] = None) -> None:
-        # clean up existing files for tables selected for truncating
-        if truncate_tables and self.fs_client.isdir(self.dataset_path):
-            all_files = self.fs_client.ls(self.dataset_path, detail=False, refresh=True)
-            for table in truncate_tables:
-                search_prefix = posixpath.join(self.dataset_path, f"{self.schema.name}.{table}.")
-                for item in all_files:
-                    # NOTE: glob implementation in fsspec does not look thread safe, way better is to use ls and then filter
-                    if item.startswith(search_prefix):
-                        # NOTE: deleting in chunks on s3 does not raise on access denied, file non existing and probably other errors
-                        self.fs_client.rm_file(item)
-
-        # create destination dir
         self.fs_client.makedirs(self.dataset_path, exist_ok=True)
 
     def is_storage_initialized(self) -> bool:
         return self.fs_client.isdir(self.dataset_path)  # type: ignore[no-any-return]
 
     def start_file_load(self, table: TTableSchema, file_path: str, load_id: str) -> LoadJob:
         cls = FollowupFilesystemJob if self.config.as_staging else LoadFilesystemJob
@@ -111,14 +123,18 @@
             schema_name=self.schema.name,
             load_id=load_id
         )
 
     def restore_file_load(self, file_path: str) -> LoadJob:
         return EmptyLoadJob.from_file_path(file_path, "completed")
 
+    def create_table_chain_completed_followup_jobs(self, table_chain: Sequence[TTableSchema]) -> List[NewLoadJob]:
+        """Creates a list of followup jobs that should be executed after a table chain is completed"""
+        return []
+
     def complete_load(self, load_id: str) -> None:
         schema_name = self.schema.name
         table_name = LOADS_TABLE_NAME
         file_name = f"{schema_name}.{table_name}.{load_id}"
         self.fs_client.touch(posixpath.join(self.dataset_path, file_name))
 
     def __enter__(self) -> "FilesystemClient":
```

### Comparing `dlt-0.3.6/dlt/destinations/filesystem/filesystem_client.py` & `dlt-0.3.6a0/dlt/destinations/filesystem/filesystem_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/destinations/insert_job_client.py` & `dlt-0.3.6a0/dlt/destinations/insert_job_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,40 +8,43 @@
 
 from dlt.destinations.sql_client import SqlClientBase
 from dlt.destinations.job_impl import EmptyLoadJob
 from dlt.destinations.job_client_impl import SqlJobClientBase
 
 
 class InsertValuesLoadJob(LoadJob, FollowupJob):
-    def __init__(self, table_name: str, file_path: str, sql_client: SqlClientBase[Any]) -> None:
+    def __init__(self, table_name: str, use_staging_table: bool, _should_truncate_destination_table: bool, file_path: str, sql_client: SqlClientBase[Any]) -> None:
         super().__init__(FileStorage.get_file_name_from_file_path(file_path))
         self._sql_client = sql_client
         # insert file content immediately
-        with self._sql_client.begin_transaction():
-            for fragments in self._insert(sql_client.make_qualified_table_name(table_name), file_path):
-                self._sql_client.execute_fragments(fragments)
+        with self._sql_client.with_staging_dataset(use_staging_table):
+            with self._sql_client.begin_transaction():
+                for fragments in self._insert(sql_client.make_qualified_table_name(table_name), _should_truncate_destination_table, file_path):
+                    self._sql_client.execute_fragments(fragments)
 
     def state(self) -> TLoadJobState:
         # this job is always done
         return "completed"
 
     def exception(self) -> str:
         # this part of code should be never reached
         raise NotImplementedError()
 
-    def _insert(self, qualified_table_name: str, file_path: str) -> Iterator[List[str]]:
+    def _insert(self, qualified_table_name: str, _should_truncate_destination_table: bool, file_path: str) -> Iterator[List[str]]:
         # WARNING: maximum redshift statement is 16MB https://docs.aws.amazon.com/redshift/latest/dg/c_redshift-sql.html
         # the procedure below will split the inserts into max_query_length // 2 packs
         with FileStorage.open_zipsafe_ro(file_path, "r", encoding="utf-8") as f:
             header = f.readline()
             values_mark = f.readline()
             # properly formatted file has a values marker at the beginning
             assert values_mark == "VALUES\n"
 
             insert_sql = []
+            if _should_truncate_destination_table:
+                insert_sql.append("DELETE FROM {};".format(qualified_table_name))
             while content := f.read(self._sql_client.capabilities.max_query_length // 2):
                 # write INSERT
                 insert_sql.extend([header.format(qualified_table_name), values_mark, content])
                 # read one more line in order to
                 # 1. complete the content which ends at "random" position, not an end line
                 # 2. to modify its ending without a need to re-allocating the 8MB of "content"
                 until_nl = f.readline()
@@ -85,20 +88,20 @@
             job = EmptyLoadJob.from_file_path(file_path, "completed")
         return job
 
     def start_file_load(self, table: TTableSchema, file_path: str, load_id: str) -> LoadJob:
         job = super().start_file_load(table, file_path, load_id)
         if not job:
             # this is using sql_client internally and will raise a right exception
-            if file_path.endswith("insert_values"):
-                job = InsertValuesLoadJob(table["name"], file_path, self.sql_client)
+            disposition = table["write_disposition"]
+            job = InsertValuesLoadJob(table["name"], disposition in self.get_stage_dispositions(), self._should_truncate_destination_table(disposition), file_path, self.sql_client)
         return job
 
-    # # TODO: implement indexes and primary keys for postgres
-    # def _get_in_table_constraints_sql(self, t: TTableSchema) -> str:
-    #     # get primary key
-    #     pass
-
-    # def _get_out_table_constrains_sql(self, t: TTableSchema) -> str:
-    #     # set non unique indexes
-    #     pass
+    # TODO: implement indexes and primary keys for postgres
+    def _get_in_table_constraints_sql(self, t: TTableSchema) -> str:
+        # get primary key
+        pass
+
+    def _get_out_table_constrains_sql(self, t: TTableSchema) -> str:
+        # set non unique indexes
+        pass
```

### Comparing `dlt-0.3.6/dlt/destinations/job_client_impl.py` & `dlt-0.3.6a0/dlt/destinations/job_client_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from dlt.common.data_types import TDataType
 from dlt.common.schema.typing import COLUMN_HINTS, LOADS_TABLE_NAME, VERSION_TABLE_NAME, TColumnSchemaBase, TTableSchema, TWriteDisposition
 from dlt.common.schema.utils import add_missing_hints
 from dlt.common.storages import FileStorage
 from dlt.common.schema import TColumnSchema, Schema, TTableSchemaColumns, TSchemaTables
 from dlt.common.destination.reference import DestinationClientConfiguration, DestinationClientDwhConfiguration, NewLoadJob, TLoadJobState, LoadJob, StagingJobClientBase, FollowupJob, DestinationClientStagingConfiguration, CredentialsConfiguration
 from dlt.common.utils import concat_strings_with_limit
-from dlt.destinations.exceptions import DatabaseUndefinedRelation, DestinationSchemaTampered, DestinationSchemaWillNotUpdate
+from dlt.destinations.exceptions import DatabaseUndefinedRelation, DestinationSchemaWillNotUpdate
 from dlt.destinations.job_impl import EmptyLoadJobWithoutFollowup, NewReferenceJob
 from dlt.destinations.sql_jobs import SqlMergeJob, SqlStagingCopyJob
 
 from dlt.destinations.typing import TNativeConn
 from dlt.destinations.sql_client import SqlClientBase
 
 
@@ -107,14 +107,15 @@
         if not self.is_storage_initialized():
             self.sql_client.create_dataset()
         else:
             # truncate requested tables
             if truncate_tables:
                 self.sql_client.truncate_tables(*truncate_tables)
 
+
     def is_storage_initialized(self) -> bool:
         return self.sql_client.has_dataset()
 
     def update_storage_schema(self, only_tables: Iterable[str] = None, expected_update: TSchemaTables = None) -> Optional[TSchemaTables]:
         super().update_storage_schema(only_tables, expected_update)
         applied_update: TSchemaTables = {}
         schema_info = self.get_schema_by_hash(self.schema.stored_version_hash)
@@ -151,18 +152,16 @@
         """Returns a list of dispositions that require staging tables to be populated"""
         dispositions: List[TWriteDisposition] = ["merge"]
         # if we have anything but the truncate-and-insert replace strategy, we need staging tables
         if self.config.replace_strategy in ["insert-from-staging", "staging-optimized"]:
             dispositions.append("replace")
         return dispositions
 
-    def get_truncate_destination_table_dispositions(self) -> List[TWriteDisposition]:
-        if self.config.replace_strategy == "truncate-and-insert":
-            return ["replace"]
-        return []
+    def _should_truncate_destination_table(self, disposition: TWriteDisposition) -> bool:
+        return disposition == "replace" and self.config.replace_strategy == "truncate-and-insert"
 
     def _create_merge_job(self, table_chain: Sequence[TTableSchema]) -> NewLoadJob:
         return SqlMergeJob.from_table_chain(table_chain, self.sql_client)
 
     # update destination tables from staging tables
     def _create_staging_copy_job(self, table_chain: Sequence[TTableSchema]) -> NewLoadJob:
         return SqlStagingCopyJob.from_table_chain(table_chain, self.sql_client)
@@ -208,17 +207,15 @@
             return EmptyLoadJobWithoutFollowup.from_file_path(file_path, "completed")
         return None
 
     def complete_load(self, load_id: str) -> None:
         name = self.sql_client.make_qualified_table_name(LOADS_TABLE_NAME)
         now_ts = pendulum.now()
         self.sql_client.execute_sql(
-            f"INSERT INTO {name}(load_id, schema_name, status, inserted_at, schema_version_hash) VALUES(%s, %s, %s, %s, %s);",
-            load_id, self.schema.name, 0, now_ts, self.schema.version_hash
-        )
+            f"INSERT INTO {name}(load_id, schema_name, status, inserted_at) VALUES(%s, %s, %s, %s);", load_id, self.schema.name, 0, now_ts)
 
     def __enter__(self) -> "SqlJobClientBase":
         self.sql_client.open_connection()
         return self
 
     def __exit__(self, exc_type: Type[BaseException], exc_val: BaseException, exc_tb: TracebackType) -> None:
         self.sql_client.close_connection()
@@ -355,17 +352,17 @@
     def _get_column_def_sql(self, c: TColumnSchema) -> str:
         pass
 
     @staticmethod
     def _gen_not_null(v: bool) -> str:
         return "NOT NULL" if not v else ""
 
-    def _create_table_update(self, table_name: str, storage_columns: TTableSchemaColumns) -> Sequence[TColumnSchema]:
+    def _create_table_update(self, table_name: str, storage_table: TTableSchemaColumns) -> Sequence[TColumnSchema]:
         # compare table with stored schema and produce delta
-        updates = self.schema.get_new_table_columns(table_name, storage_columns)
+        updates = self.schema.get_new_complete_columns(table_name, storage_table)
         logger.info(f"Found {len(updates)} updates for {table_name} in {self.schema.name}")
         return updates
 
     def _row_to_schema_info(self, query: str, *args: Any) -> StorageSchemaInfo:
         row: Tuple[Any,...] = None
         # if there's no dataset/schema return none info
         with contextlib.suppress(DatabaseUndefinedRelation):
@@ -396,18 +393,14 @@
         name = self.sql_client.make_qualified_table_name(VERSION_TABLE_NAME)
         self.sql_client.execute_sql(
             f"DELETE FROM {name} WHERE schema_name = %s;", schema.name
         )
         self._update_schema_in_storage(schema)
 
     def _update_schema_in_storage(self, schema: Schema) -> None:
-        # make sure that schema being saved was not modified from the moment it was loaded from storage
-        version_hash = schema.version_hash
-        if version_hash != schema.stored_version_hash:
-            raise DestinationSchemaTampered(schema.name, version_hash, schema.stored_version_hash)
         now_ts = str(pendulum.now())
         # get schema string or zip
         schema_str = json.dumps(schema.to_dict())
         # TODO: not all databases store data as utf-8 but this exception is mostly for redshift
         schema_bytes = schema_str.encode("utf-8")
         if len(schema_bytes) > self.capabilities.max_text_data_type_length:
             # compress and to base64
```

### Comparing `dlt-0.3.6/dlt/destinations/job_impl.py` & `dlt-0.3.6a0/dlt/destinations/job_impl.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/destinations/motherduck/__init__.py` & `dlt-0.3.6a0/dlt/destinations/motherduck/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 def _configure(config: MotherDuckClientConfiguration = config.value) -> MotherDuckClientConfiguration:
     return config
 
 
 def capabilities() -> DestinationCapabilitiesContext:
     caps = DestinationCapabilitiesContext()
     caps.preferred_loader_file_format = "parquet"
-    caps.supported_loader_file_formats = ["parquet", "insert_values", "jsonl"]
+    caps.supported_loader_file_formats = ["parquet", "insert_values", "sql"]
     caps.escape_identifier = escape_postgres_identifier
     caps.escape_literal = escape_duckdb_literal
     caps.decimal_precision = (DEFAULT_NUMERIC_PRECISION, DEFAULT_NUMERIC_SCALE)
     caps.wei_precision = (DEFAULT_NUMERIC_PRECISION, 0)
     caps.max_identifier_length = 65536
     caps.max_column_identifier_length = 65536
     caps.naming_convention = "duck_case"
```

### Comparing `dlt-0.3.6/dlt/destinations/motherduck/configuration.py` & `dlt-0.3.6a0/dlt/destinations/motherduck/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/destinations/motherduck/motherduck.py` & `dlt-0.3.6a0/dlt/destinations/motherduck/motherduck.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/destinations/motherduck/sql_client.py` & `dlt-0.3.6a0/dlt/destinations/motherduck/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/destinations/postgres/__init__.py` & `dlt-0.3.6a0/dlt/destinations/postgres/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     return config
 
 
 def capabilities() -> DestinationCapabilitiesContext:
     # https://www.postgresql.org/docs/current/limits.html
     caps = DestinationCapabilitiesContext()
     caps.preferred_loader_file_format = "insert_values"
-    caps.supported_loader_file_formats = ["insert_values"]
+    caps.supported_loader_file_formats = ["insert_values", "sql"]
     caps.preferred_staging_file_format = None
     caps.supported_staging_file_formats = []
     caps.escape_identifier = escape_postgres_identifier
     caps.escape_literal = escape_postgres_literal
     caps.decimal_precision = (DEFAULT_NUMERIC_PRECISION, DEFAULT_NUMERIC_SCALE)
     caps.wei_precision = (2*EVM_DECIMAL_PRECISION, EVM_DECIMAL_PRECISION)
     caps.max_identifier_length = 63
```

### Comparing `dlt-0.3.6/dlt/destinations/postgres/configuration.py` & `dlt-0.3.6a0/dlt/destinations/postgres/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/destinations/postgres/postgres.py` & `dlt-0.3.6a0/dlt/destinations/postgres/postgres.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,21 @@
-from typing import ClassVar, Dict, Optional, Sequence, List, Any
+import platform
 
 from dlt.common.wei import EVM_DECIMAL_PRECISION
+if platform.python_implementation() == "PyPy":
+    import psycopg2cffi as psycopg2
+    from psycopg2cffi.sql import SQL, Composed
+else:
+    import psycopg2
+    from psycopg2.sql import SQL, Composed
+
+
+from typing import ClassVar, Dict, Optional, Sequence, List, Any
+
+from dlt.common.arithmetics import DEFAULT_NUMERIC_PRECISION, DEFAULT_NUMERIC_SCALE
 from dlt.common.destination.reference import NewLoadJob
 from dlt.common.destination import DestinationCapabilitiesContext
 from dlt.common.data_types import TDataType
 from dlt.common.schema import TColumnSchema, TColumnHint, Schema
 from dlt.common.schema.typing import TTableSchema
 
 from dlt.destinations.sql_jobs import SqlStagingCopyJob
```

### Comparing `dlt-0.3.6/dlt/destinations/postgres/sql_client.py` & `dlt-0.3.6a0/dlt/destinations/postgres/sql_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import platform
 
 from dlt.common.destination import DestinationCapabilitiesContext
 
 if platform.python_implementation() == "PyPy":
     import psycopg2cffi as psycopg2
-    from psycopg2cffi.sql import SQL, Composed, Composable
+    from psycopg2cffi.sql import SQL, Identifier, Literal as SQLLiteral
 else:
     import psycopg2
-    from psycopg2.sql import SQL, Composed, Composable
+    from psycopg2.sql import SQL, Identifier, Literal as SQLLiteral, Composed, Composable
 
 from contextlib import contextmanager
 from typing import Any, AnyStr, ClassVar, Iterator, Optional, Sequence
 
 from dlt.destinations.exceptions import DatabaseTerminalException, DatabaseTransientException, DatabaseUndefinedRelation
 from dlt.destinations.typing import DBApi, DBApiCursor, DBTransaction
 from dlt.destinations.sql_client import DBApiCursorImpl, SqlClientBase, raise_database_error, raise_open_connection_error
@@ -64,14 +64,20 @@
         self._conn.rollback()
         self._conn.autocommit = True
 
     @property
     def native_connection(self) -> "psycopg2.connection":
         return self._conn
 
+    def create_dataset(self) -> None:
+        self.execute_sql("CREATE SCHEMA %s" % self.fully_qualified_dataset_name())
+
+    def drop_dataset(self) -> None:
+        self.execute_sql("DROP SCHEMA %s CASCADE;" % self.fully_qualified_dataset_name())
+
     # @raise_database_error
     def execute_sql(self, sql: AnyStr, *args: Any, **kwargs: Any) -> Optional[Sequence[Sequence[Any]]]:
         with self.execute_query(sql, *args, **kwargs) as curr:
             if curr.description is None:
                 return None
             else:
                 f = curr.fetchall()
```

### Comparing `dlt-0.3.6/dlt/destinations/redshift/README.md` & `dlt-0.3.6a0/dlt/destinations/redshift/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/destinations/redshift/__init__.py` & `dlt-0.3.6a0/dlt/destinations/redshift/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 def _configure(config: RedshiftClientConfiguration = config.value) -> RedshiftClientConfiguration:
     return config
 
 
 def capabilities() -> DestinationCapabilitiesContext:
     caps = DestinationCapabilitiesContext()
     caps.preferred_loader_file_format = "insert_values"
-    caps.supported_loader_file_formats = ["insert_values"]
+    caps.supported_loader_file_formats = ["insert_values", "sql"]
     caps.preferred_staging_file_format = "jsonl"
     caps.supported_staging_file_formats = ["jsonl", "parquet"]
     caps.escape_identifier = escape_redshift_identifier
     caps.escape_literal = escape_redshift_literal
     caps.decimal_precision = (DEFAULT_NUMERIC_PRECISION, DEFAULT_NUMERIC_SCALE)
     caps.wei_precision = (DEFAULT_NUMERIC_PRECISION, 0)
     caps.max_identifier_length = 127
```

### Comparing `dlt-0.3.6/dlt/destinations/redshift/configuration.py` & `dlt-0.3.6a0/dlt/destinations/redshift/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/destinations/redshift/redshift.py` & `dlt-0.3.6a0/dlt/destinations/redshift/redshift.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,17 +80,21 @@
         return None
 
 class RedshiftCopyFileLoadJob(CopyRemoteFileLoadJob):
 
     def __init__(self, table: TTableSchema,
                  file_path: str,
                  sql_client: SqlClientBase[Any],
+                 use_staging_table: bool,
+                 should_truncate_destination_table: bool,
                  staging_credentials: Optional[CredentialsConfiguration] = None,
                  staging_iam_role: str = None) -> None:
         self._staging_iam_role = staging_iam_role
+        self._use_staging_table = use_staging_table
+        self._should_truncate_destination_table = should_truncate_destination_table
         super().__init__(table, file_path, sql_client, staging_credentials)
 
     def execute(self, table: TTableSchema, bucket_path: str) -> None:
 
         # we assume s3 credentials where provided for the staging
         credentials = ""
         if self._staging_iam_role:
@@ -117,24 +121,27 @@
             # if table contains complex types then SUPER field will be used.
             # https://docs.aws.amazon.com/redshift/latest/dg/ingest-super.html
             if table_schema_has_type(table, "complex"):
                 file_type += " SERIALIZETOJSON"
         else:
             raise ValueError(f"Unsupported file type {ext} for Redshift.")
 
-        with self._sql_client.begin_transaction():
-            dataset_name = self._sql_client.dataset_name
-            # TODO: if we ever support csv here remember to add column names to COPY
-            self._sql_client.execute_sql(f"""
-                COPY {dataset_name}.{table_name}
-                FROM '{bucket_path}'
-                {file_type}
-                {dateformat}
-                {compression}
-                {credentials} MAXERROR 0;""")
+        with self._sql_client.with_staging_dataset(self._use_staging_table):
+            with self._sql_client.begin_transaction():
+                dataset_name = self._sql_client.dataset_name
+                if self._should_truncate_destination_table:
+                    self._sql_client.execute_sql(f"""TRUNCATE TABLE {table_name}""")
+                # TODO: if we ever support csv here remember to add column names to COPY
+                self._sql_client.execute_sql(f"""
+                    COPY {dataset_name}.{table_name}
+                    FROM '{bucket_path}'
+                    {file_type}
+                    {dateformat}
+                    {compression}
+                    {credentials} MAXERROR 0;""")
 
 
 
 
     def exception(self) -> str:
         # this part of code should be never reached
         raise NotImplementedError()
@@ -171,19 +178,18 @@
     def _get_column_def_sql(self, c: TColumnSchema) -> str:
         hints_str = " ".join(HINT_TO_REDSHIFT_ATTR.get(h, "") for h in HINT_TO_REDSHIFT_ATTR.keys() if c.get(h, False) is True)
         column_name = self.capabilities.escape_identifier(c["name"])
         return f"{column_name} {self._to_db_type(c['data_type'])} {hints_str} {self._gen_not_null(c['nullable'])}"
 
     def start_file_load(self, table: TTableSchema, file_path: str, load_id: str) -> LoadJob:
         """Starts SqlLoadJob for files ending with .sql or returns None to let derived classes to handle their specific jobs"""
-        job = super().start_file_load(table, file_path, load_id)
-        if not job:
-            assert NewReferenceJob.is_reference_job(file_path), "Redshift must use staging to load files"
-            job = RedshiftCopyFileLoadJob(table, file_path, self.sql_client, staging_credentials=self.config.staging_credentials, staging_iam_role=self.config.staging_iam_role)
-        return job
+        if NewReferenceJob.is_reference_job(file_path):
+            disposition = table["write_disposition"]
+            return RedshiftCopyFileLoadJob(table, file_path, self.sql_client, disposition in self.get_stage_dispositions(), self._should_truncate_destination_table(disposition), staging_credentials=self.config.staging_credentials, staging_iam_role=self.config.staging_iam_role)
+        return super().start_file_load(table, file_path, load_id)
 
     @classmethod
     def _to_db_type(cls, sc_t: TDataType) -> str:
         if sc_t == "wei":
             return SCT_TO_PGT["decimal"] % cls.capabilities.wei_precision
         if sc_t == "decimal":
             return SCT_TO_PGT["decimal"] % cls.capabilities.decimal_precision
```

### Comparing `dlt-0.3.6/dlt/destinations/snowflake/__init__.py` & `dlt-0.3.6a0/dlt/destinations/snowflake/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 def _configure(config: SnowflakeClientConfiguration = config.value) -> SnowflakeClientConfiguration:
     return config
 
 
 def capabilities() -> DestinationCapabilitiesContext:
     caps = DestinationCapabilitiesContext()
     caps.preferred_loader_file_format = "jsonl"
-    caps.supported_loader_file_formats = ["jsonl", "parquet"]
+    caps.supported_loader_file_formats = ["jsonl", "parquet", "sql"]
     caps.preferred_staging_file_format = "jsonl"
-    caps.supported_staging_file_formats = ["jsonl", "parquet"]
+    caps.supported_staging_file_formats = ["jsonl", "parquet", "sql"]
     caps.escape_identifier = escape_snowflake_identifier
     caps.decimal_precision = (DEFAULT_NUMERIC_PRECISION, DEFAULT_NUMERIC_SCALE)
     caps.wei_precision = (DEFAULT_NUMERIC_PRECISION, 0)
     caps.max_identifier_length = 255
     caps.max_column_identifier_length = 255
     caps.max_query_length = 2 * 1024 * 1024
     caps.is_max_query_length_in_bytes = True
```

### Comparing `dlt-0.3.6/dlt/destinations/snowflake/configuration.py` & `dlt-0.3.6a0/dlt/destinations/snowflake/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/destinations/snowflake/snowflake.py` & `dlt-0.3.6a0/dlt/destinations/snowflake/snowflake.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,71 +48,74 @@
     "BINARY": "binary",
     "VARIANT": "complex"
 }
 
 
 class SnowflakeLoadJob(LoadJob, FollowupJob):
     def __init__(
-            self, file_path: str, table_name: str, load_id: str, client: SnowflakeSqlClient,
+            self, file_path: str, table_name: str, use_staging_table: bool, _should_truncate_destination_table: bool, load_id: str, client: SnowflakeSqlClient,
             stage_name: Optional[str] = None, keep_staged_files: bool = True, staging_credentials: Optional[CredentialsConfiguration] = None
     ) -> None:
         file_name = FileStorage.get_file_name_from_file_path(file_path)
         super().__init__(file_name)
 
-        qualified_table_name = client.make_qualified_table_name(table_name)
+        with client.with_staging_dataset(use_staging_table):
+            qualified_table_name = client.make_qualified_table_name(table_name)
 
-        # extract and prepare some vars
-        bucket_path = NewReferenceJob.resolve_reference(file_path) if NewReferenceJob.is_reference_job(file_path) else ""
-        file_name = FileStorage.get_file_name_from_file_path(bucket_path) if bucket_path else file_name
-        from_clause = ""
-        credentials_clause = ""
-        files_clause = ""
-        stage_file_path = ""
-
-        if bucket_path:
-            # s3 credentials case
-            if bucket_path.startswith("s3://") and staging_credentials and isinstance(staging_credentials, AwsCredentialsWithoutDefaults):
-                credentials_clause = f"""CREDENTIALS=(AWS_KEY_ID='{staging_credentials.aws_access_key_id}' AWS_SECRET_KEY='{staging_credentials.aws_secret_access_key}')"""
-                from_clause = f"FROM '{bucket_path}'"
+            # extract and prepare some vars
+            bucket_path = NewReferenceJob.resolve_reference(file_path) if NewReferenceJob.is_reference_job(file_path) else ""
+            file_name = FileStorage.get_file_name_from_file_path(bucket_path) if bucket_path else file_name
+            from_clause = ""
+            credentials_clause = ""
+            files_clause = ""
+            stage_file_path = ""
+
+            if bucket_path:
+                # s3 credentials case
+                if bucket_path.startswith("s3://") and staging_credentials and isinstance(staging_credentials, AwsCredentialsWithoutDefaults):
+                    credentials_clause = f"""CREDENTIALS=(AWS_KEY_ID='{staging_credentials.aws_access_key_id}' AWS_SECRET_KEY='{staging_credentials.aws_secret_access_key}')"""
+                    from_clause = f"FROM '{bucket_path}'"
+                else:
+                    # ensure that gcs bucket path starts with gcs://, this is a requirement of snowflake
+                    bucket_path = bucket_path.replace("gs://", "gcs://")
+                    if not stage_name:
+                        # when loading from bucket stage must be given
+                        raise LoadJobTerminalException(file_path, f"Cannot load from bucket path {bucket_path} without a stage name. See https://dlthub.com/docs/dlt-ecosystem/destinations/snowflake for instructions on setting up the `stage_name`")
+                    from_clause = f"FROM @{stage_name}/"
+                    files_clause = f"FILES = ('{urlparse(bucket_path).path.lstrip('/')}')"
             else:
-                # ensure that gcs bucket path starts with gcs://, this is a requirement of snowflake
-                bucket_path = bucket_path.replace("gs://", "gcs://")
+                # this means we have a local file
                 if not stage_name:
-                    # when loading from bucket stage must be given
-                    raise LoadJobTerminalException(file_path, f"Cannot load from bucket path {bucket_path} without a stage name. See https://dlthub.com/docs/dlt-ecosystem/destinations/snowflake for instructions on setting up the `stage_name`")
-                from_clause = f"FROM @{stage_name}/"
-                files_clause = f"FILES = ('{urlparse(bucket_path).path.lstrip('/')}')"
-        else:
-            # this means we have a local file
-            if not stage_name:
-                # Use implicit table stage by default: "SCHEMA_NAME"."%TABLE_NAME"
-                stage_name = client.make_qualified_table_name('%'+table_name)
-            stage_file_path = f'@{stage_name}/"{load_id}"/{file_name}'
-            from_clause = f"FROM {stage_file_path}"
-
-        # decide on source format, stage_file_path will either be a local file or a bucket path
-        source_format = "( TYPE = 'JSON', BINARY_FORMAT = 'BASE64' )"
-        if file_name.endswith("parquet"):
-            source_format = "(TYPE = 'PARQUET', BINARY_AS_TEXT = FALSE)"
-
-        with client.begin_transaction():
-            # PUT and COPY in one tx if local file, otherwise only copy
-            if not bucket_path:
-                client.execute_sql(f'PUT file://{file_path} @{stage_name}/"{load_id}" OVERWRITE = TRUE, AUTO_COMPRESS = FALSE')
-            client.execute_sql(
-                f"""COPY INTO {qualified_table_name}
-                {from_clause}
-                {files_clause}
-                {credentials_clause}
-                FILE_FORMAT = {source_format}
-                MATCH_BY_COLUMN_NAME='CASE_INSENSITIVE'
-                """
-            )
-            if stage_file_path and not keep_staged_files:
-                client.execute_sql(f'REMOVE {stage_file_path}')
+                    # Use implicit table stage by default: "SCHEMA_NAME"."%TABLE_NAME"
+                    stage_name = client.make_qualified_table_name('%'+table_name)
+                stage_file_path = f'@{stage_name}/"{load_id}"/{file_name}'
+                from_clause = f"FROM {stage_file_path}"
+
+            # decide on source format, stage_file_path will either be a local file or a bucket path
+            source_format = "( TYPE = 'JSON', BINARY_FORMAT = 'BASE64' )"
+            if file_name.endswith("parquet"):
+                source_format = "(TYPE = 'PARQUET', BINARY_AS_TEXT = FALSE)"
+
+            with client.begin_transaction():
+                if _should_truncate_destination_table:
+                    client.execute_sql(f"TRUNCATE TABLE IF EXISTS {qualified_table_name}")
+                # PUT and COPY in one tx if local file, otherwise only copy
+                if not bucket_path:
+                    client.execute_sql(f'PUT file://{file_path} @{stage_name}/"{load_id}" OVERWRITE = TRUE, AUTO_COMPRESS = FALSE')
+                client.execute_sql(
+                    f"""COPY INTO {qualified_table_name}
+                    {from_clause}
+                    {files_clause}
+                    {credentials_clause}
+                    FILE_FORMAT = {source_format}
+                    MATCH_BY_COLUMN_NAME='CASE_INSENSITIVE'
+                    """
+                )
+                if stage_file_path and not keep_staged_files:
+                    client.execute_sql(f'REMOVE {stage_file_path}')
 
 
     def state(self) -> TLoadJobState:
         return "completed"
 
     def exception(self) -> str:
         raise NotImplementedError()
@@ -146,21 +149,18 @@
         self.config: SnowflakeClientConfiguration = config
         self.sql_client: SnowflakeSqlClient = sql_client  # type: ignore
 
     def start_file_load(self, table: TTableSchema, file_path: str, load_id: str) -> LoadJob:
         job = super().start_file_load(table, file_path, load_id)
 
         if not job:
+            disposition = table['write_disposition']
             job = SnowflakeLoadJob(
-                file_path,
-                table['name'],
-                load_id,
-                self.sql_client,
-                stage_name=self.config.stage_name,
-                keep_staged_files=self.config.keep_staged_files,
+                file_path, table['name'], disposition in self.get_stage_dispositions(), self._should_truncate_destination_table(disposition), load_id, self.sql_client,
+                stage_name=self.config.stage_name, keep_staged_files=self.config.keep_staged_files,
                 staging_credentials=self.config.staging_credentials
             )
         return job
 
     def restore_file_load(self, file_path: str) -> LoadJob:
         return EmptyLoadJob.from_file_path(file_path, "completed")
```

### Comparing `dlt-0.3.6/dlt/destinations/snowflake/sql_client.py` & `dlt-0.3.6a0/dlt/destinations/snowflake/sql_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,14 +67,20 @@
         self._conn.rollback()
         self._conn.autocommit(True)
 
     @property
     def native_connection(self) -> "snowflake_lib.SnowflakeConnection":
         return self._conn
 
+    def create_dataset(self) -> None:
+        self.execute_sql("CREATE SCHEMA %s" % self.fully_qualified_dataset_name())
+
+    def drop_dataset(self) -> None:
+        self.execute_sql("DROP SCHEMA %s CASCADE;" % self.fully_qualified_dataset_name())
+
     def drop_tables(self, *tables: str) -> None:
         # Tables are drop with `IF EXISTS`, but snowflake raises when the schema doesn't exist.
         # Multi statement exec is safe and the error can be ignored since all tables are in the same schema.
         with suppress(DatabaseUndefinedRelation):
             super().drop_tables(*tables)
 
     def execute_sql(self, sql: AnyStr, *args: Any, **kwargs: Any) -> Optional[Sequence[Sequence[Any]]]:
```

### Comparing `dlt-0.3.6/dlt/destinations/sql_client.py` & `dlt-0.3.6a0/dlt/destinations/sql_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,22 +61,24 @@
         db_params = self.fully_qualified_dataset_name(escape=False).split(".", 2)
         if len(db_params) == 2:
             query += " catalog_name = %s AND "
         query += "schema_name = %s"
         rows = self.execute_sql(query, *db_params)
         return len(rows) > 0
 
+    @abstractmethod
     def create_dataset(self) -> None:
-        self.execute_sql("CREATE SCHEMA %s" % self.fully_qualified_dataset_name())
+        pass
 
+    @abstractmethod
     def drop_dataset(self) -> None:
-        self.execute_sql("DROP SCHEMA %s CASCADE;" % self.fully_qualified_dataset_name())
+        pass
 
     def truncate_tables(self, *tables: str) -> None:
-        statements = [self._truncate_table_sql(self.make_qualified_table_name(t)) for t in tables]
+        statements = [f"TRUNCATE TABLE {self.make_qualified_table_name(t)};" for t in tables]
         self.execute_fragments(statements)
 
     def drop_tables(self, *tables: str) -> None:
         if not tables:
             return
         statements = [f"DROP TABLE IF EXISTS {self.make_qualified_table_name(table)};" for table in tables]
         self.execute_fragments(statements)
@@ -143,19 +145,19 @@
     @staticmethod
     def make_staging_dataset_name(dataset_name: str) -> str:
         return dataset_name + "_staging"
 
     #
     # generate sql statements
     #
-    def _truncate_table_sql(self, qualified_table_name: str) -> str:
+    def truncate_table_sql(self, table_name: str) -> str:
         if self.capabilities.supports_truncate_command:
-            return f"TRUNCATE TABLE {qualified_table_name};"
+            return f"TRUNCATE TABLE {table_name};"
         else:
-            return f"DELETE FROM {qualified_table_name} WHERE 1=1;"
+            return f"DELETE FROM {table_name};"
 
 
 class DBApiCursorImpl(DBApiCursor):
     """A DBApi Cursor wrapper with dataframes reading functionality"""
     def __init__(self, curr: DBApiCursor) -> None:
         self.native_cursor = curr
```

### Comparing `dlt-0.3.6/dlt/destinations/sql_jobs.py` & `dlt-0.3.6a0/dlt/destinations/sql_jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,16 +50,16 @@
     @classmethod
     def generate_sql(cls, table_chain: Sequence[TTableSchema], sql_client: SqlClientBase[Any]) -> List[str]:
         sql: List[str] = []
         for table in table_chain:
             with sql_client.with_staging_dataset(staging=True):
                 staging_table_name = sql_client.make_qualified_table_name(table["name"])
             table_name = sql_client.make_qualified_table_name(table["name"])
-            columns = ", ".join(map(sql_client.capabilities.escape_identifier, get_columns_names_with_prop(table, "name")))
-            sql.append(sql_client._truncate_table_sql(table_name))
+            columns = ", ".join(map(sql_client.capabilities.escape_identifier, table["columns"].keys()))
+            sql.append(sql_client.truncate_table_sql(table_name))
             sql.append(f"INSERT INTO {table_name}({columns}) SELECT {columns} FROM {staging_table_name};")
         return sql
 
 class SqlMergeJob(SqlBaseJob):
     """Generates a list of sql statements that merge the data from staging dataset into destination dataset."""
     failed_text: str = "Tried to generate a merge sql job for the following tables:"
 
@@ -181,15 +181,15 @@
                 sql.extend(create_insert_temp_table_sql)
 
         # insert from staging to dataset, truncate staging table
         for table in table_chain:
             table_name = sql_client.make_qualified_table_name(table["name"])
             with sql_client.with_staging_dataset(staging=True):
                 staging_table_name = sql_client.make_qualified_table_name(table["name"])
-            columns = ", ".join(map(sql_client.capabilities.escape_identifier, get_columns_names_with_prop(table, "name")))
+            columns = ", ".join(map(sql_client.capabilities.escape_identifier, table["columns"].keys()))
             insert_sql = f"INSERT INTO {table_name}({columns}) SELECT {columns} FROM {staging_table_name}"
             if len(primary_keys) > 0:
                 if len(table_chain) == 1:
                     insert_sql = f"""INSERT INTO {table_name}({columns})
                         WITH _dlt_dedup_numbered AS (
                             SELECT ROW_NUMBER() OVER (partition BY {", ".join(primary_keys)} ORDER BY (SELECT NULL)) AS _dlt_dedup_rn, {columns}
                             FROM {staging_table_name}
```

### Comparing `dlt-0.3.6/dlt/destinations/typing.py` & `dlt-0.3.6a0/dlt/destinations/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/extract/decorators.py` & `dlt-0.3.6a0/dlt/extract/decorators.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/extract/exceptions.py` & `dlt-0.3.6a0/dlt/extract/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/extract/extract.py` & `dlt-0.3.6a0/dlt/extract/extract.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import contextlib
 import os
-from typing import ClassVar, List, Set
+from typing import ClassVar, List
 
 from dlt.common.configuration.container import Container
 from dlt.common.configuration.resolve import inject_section
 from dlt.common.configuration.specs.config_section_context import ConfigSectionContext
 from dlt.common.pipeline import _reset_resource_state
 
 from dlt.common.runtime import signals
@@ -65,29 +65,23 @@
     max_parallel_items: int = None,
     workers: int = None,
     futures_poll_interval: float = None
 ) -> TSchemaUpdate:
 
     dynamic_tables: TSchemaUpdate = {}
     schema = source.schema
-    resources_with_items: Set[str] = set()
 
     with collector(f"Extract {source.name}"):
 
-        def _write_empty_file(table_name: str) -> None:
-            table_name = schema.naming.normalize_identifier(table_name)
-            storage.write_empty_file(extract_id, schema.name, table_name, None)
-
-        def _write_item(table_name: str, resource_name: str, item: TDataItems) -> None:
+        def _write_item(table_name: str, item: TDataItems) -> None:
             # normalize table name before writing so the name match the name in schema
             # note: normalize function should be cached so there's almost no penalty on frequent calling
             # note: column schema is not required for jsonl writer used here
             table_name = schema.naming.normalize_identifier(table_name)
             collector.update(table_name)
-            resources_with_items.add(resource_name)
             storage.write_data_item(extract_id, schema.name, table_name, item, None)
 
         def _write_dynamic_table(resource: DltResource, item: TDataItem) -> None:
             table_name = resource._table_name_hint_fun(item)
             existing_table = dynamic_tables.get(table_name)
             if existing_table is None:
                 dynamic_tables[table_name] = [resource.table_schema(item)]
@@ -97,15 +91,15 @@
                     new_table = resource.table_schema(item)
                     # this merges into existing table in place
                     utils.merge_tables(existing_table[0], new_table)
                 else:
                     # if there are no other dynamic hints besides name then we just leave the existing partial table
                     pass
             # write to storage with inferred table name
-            _write_item(table_name, resource.name, item)
+            _write_item(table_name, item)
 
         def _write_static_table(resource: DltResource, table_name: str) -> None:
             existing_table = dynamic_tables.get(table_name)
             if existing_table is None:
                 static_table = resource.table_schema()
                 static_table["name"] = table_name
                 dynamic_tables[table_name] = [static_table]
@@ -123,44 +117,31 @@
                     collector.update("Resources", delta)
 
                 signals.raise_if_signalled()
 
                 # TODO: many resources may be returned. if that happens the item meta must be present with table name and this name must match one of resources
                 # if meta contains table name
                 resource = source.resources.find_by_pipe(pipe_item.pipe)
-                table_name: str = None
                 if isinstance(pipe_item.meta, TableNameMeta):
                     table_name = pipe_item.meta.table_name
                     _write_static_table(resource, table_name)
-                    _write_item(table_name, resource.name, pipe_item.item)
+                    _write_item(table_name, pipe_item.item)
                 else:
                     # get partial table from table template
                     if resource._table_name_hint_fun:
                         if isinstance(pipe_item.item, List):
                             for item in pipe_item.item:
                                 _write_dynamic_table(resource, item)
                         else:
                             _write_dynamic_table(resource, pipe_item.item)
                     else:
                         # write item belonging to table with static name
                         table_name = resource.table_name
                         _write_static_table(resource, table_name)
-                        _write_item(table_name, resource.name, pipe_item.item)
-
-            # find defined resources that did not yield any pipeitems and create empty jobs for them
-            data_tables = {t["name"]: t for t in schema.data_tables()}
-            tables_by_resources = utils.group_tables_by_resource(data_tables)
-            for resource in source.resources.selected.values():
-                if resource.write_disposition != "replace" or resource.name in resources_with_items:
-                    continue
-                if resource.name not in tables_by_resources:
-                    continue
-                for table in tables_by_resources[resource.name]:
-                    _write_empty_file(table["name"])
-
+                        _write_item(table_name, pipe_item.item)
             if left_gens > 0:
                 # go to 100%
                 collector.update("Resources", left_gens)
 
         # flush all buffered writers
         storage.close_writers(extract_id)
```

### Comparing `dlt-0.3.6/dlt/extract/incremental.py` & `dlt-0.3.6a0/dlt/extract/incremental.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/extract/pipe.py` & `dlt-0.3.6a0/dlt/extract/pipe.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/extract/schema.py` & `dlt-0.3.6a0/dlt/extract/schema.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/extract/source.py` & `dlt-0.3.6a0/dlt/extract/source.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/extract/typing.py` & `dlt-0.3.6a0/dlt/extract/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/extract/utils.py` & `dlt-0.3.6a0/dlt/extract/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/helpers/airflow_helper.py` & `dlt-0.3.6a0/dlt/helpers/airflow_helper.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/helpers/dbt/__init__.py` & `dlt-0.3.6a0/dlt/helpers/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/helpers/dbt/configuration.py` & `dlt-0.3.6a0/dlt/helpers/dbt/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/helpers/dbt/dbt_utils.py` & `dlt-0.3.6a0/dlt/helpers/dbt/dbt_utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/helpers/dbt/exceptions.py` & `dlt-0.3.6a0/dlt/helpers/dbt/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/helpers/dbt/profiles.yml` & `dlt-0.3.6a0/dlt/helpers/dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/helpers/dbt/runner.py` & `dlt-0.3.6a0/dlt/helpers/dbt/runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/helpers/pandas_helper.py` & `dlt-0.3.6a0/dlt/helpers/pandas_helper.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/helpers/streamlit_helper.py` & `dlt-0.3.6a0/dlt/helpers/streamlit_helper.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/load/configuration.py` & `dlt-0.3.6a0/dlt/load/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/load/exceptions.py` & `dlt-0.3.6a0/dlt/load/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/load/load.py` & `dlt-0.3.6a0/dlt/load/load.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-import contextlib
-from copy import copy
 from functools import reduce
 import datetime  # noqa: 251
-from typing import Dict, List, Optional, Tuple, Set, Iterator
+from typing import Dict, List, Optional, Tuple
 from multiprocessing.pool import ThreadPool
 import os
 
 from dlt.common import sleep, logger
 from dlt.common.configuration import with_config, known_sections
 from dlt.common.configuration.accessors import config
 from dlt.common.pipeline import LoadInfo, SupportsPipeline
@@ -16,110 +14,89 @@
 from dlt.common.runners import TRunMetrics, Runnable, workermethod
 from dlt.common.runtime.collector import Collector, NULL_COLLECTOR
 from dlt.common.runtime.logger import pretty_format_exception
 from dlt.common.exceptions import TerminalValueError
 from dlt.common.schema import Schema
 from dlt.common.schema.typing import VERSION_TABLE_NAME, TTableSchema, TWriteDisposition
 from dlt.common.storages import LoadStorage
-from dlt.common.destination.reference import DestinationClientDwhConfiguration, FollowupJob, JobClientBase, StagingJobClientBase, DestinationReference, LoadJob, NewLoadJob, TLoadJobState, DestinationClientConfiguration
+from dlt.common.destination.reference import DestinationClientDwhConfiguration, FollowupJob, JobClientBase, StagingJobClientBase, DestinationReference, LoadJob, NewLoadJob, TLoadJobState, DestinationClientConfiguration, DestinationClientStagingConfiguration
+from dlt.destinations.filesystem.filesystem import LoadFilesystemJob
 
 from dlt.destinations.job_impl import EmptyLoadJob
 from dlt.destinations.exceptions import DestinationTerminalException, DestinationTransientException, LoadJobUnknownTableException
 
 from dlt.load.configuration import LoaderConfiguration
 from dlt.load.exceptions import LoadClientJobFailed, LoadClientJobRetry, LoadClientUnsupportedWriteDisposition, LoadClientUnsupportedFileFormats
 
 
 class Load(Runnable[ThreadPool]):
 
     @with_config(spec=LoaderConfiguration, sections=(known_sections.LOAD,))
     def __init__(
         self,
         destination: DestinationReference,
-        staging_destination: DestinationReference = None,
+        staging: DestinationReference = None,
         collector: Collector = NULL_COLLECTOR,
         is_storage_owner: bool = False,
         config: LoaderConfiguration = config.value,
         initial_client_config: DestinationClientConfiguration = config.value,
         initial_staging_client_config: DestinationClientConfiguration = config.value
     ) -> None:
         self.config = config
         self.collector = collector
         self.initial_client_config = initial_client_config
         self.initial_staging_client_config = initial_staging_client_config
         self.destination = destination
         self.capabilities = destination.capabilities()
-        self.staging_destination = staging_destination
+        self.staging = staging
         self.pool: ThreadPool = None
         self.load_storage: LoadStorage = self.create_storage(is_storage_owner)
         self._processed_load_ids: Dict[str, int] = {}
 
 
     def create_storage(self, is_storage_owner: bool) -> LoadStorage:
         supported_file_formats = self.capabilities.supported_loader_file_formats
-        if self.staging_destination:
-            supported_file_formats = self.staging_destination.capabilities().supported_loader_file_formats + ["reference"]
-        if isinstance(self.get_destination_client(Schema("test")), StagingJobClientBase):
-            supported_file_formats += ["sql"]
+        if self.staging:
+            supported_file_formats = self.staging.capabilities().supported_loader_file_formats + ["reference", "sql"]
         load_storage = LoadStorage(
             is_storage_owner,
             self.capabilities.preferred_loader_file_format,
             supported_file_formats,
             config=self.config._load_storage_config
         )
         return load_storage
 
     @staticmethod
     def get_load_table(schema: Schema, file_name: str) -> TTableSchema:
         table_name = LoadStorage.parse_job_file_name(file_name).table_name
         try:
-            # make a copy of the schema so modifications do not affect the original document
-            table = copy(schema.get_table(table_name))
+            table = schema.get_table(table_name)
             # add write disposition if not specified - in child tables
             if "write_disposition" not in table:
                 table["write_disposition"] = get_write_disposition(schema.tables, table_name)
             return table
         except KeyError:
             raise LoadJobUnknownTableException(table_name, file_name)
 
-    def get_destination_client(self, schema: Schema) -> JobClientBase:
-        return self.destination.client(schema, self.initial_client_config)
-
-    def get_staging_destination_client(self, schema: Schema) -> JobClientBase:
-        return self.staging_destination.client(schema, self.initial_staging_client_config)
-
-    def is_staging_destination_job(self, file_path: str) -> bool:
-        return self.staging_destination is not None and os.path.splitext(file_path)[1][1:] in self.staging_destination.capabilities().supported_loader_file_formats
-
-    @contextlib.contextmanager
-    def maybe_with_staging_dataset(self, job_client: JobClientBase, table: TTableSchema) -> Iterator[None]:
-        """Executes job client methods in context of staging dataset if `table` has `write_disposition` that requires it"""
-        if isinstance(job_client, StagingJobClientBase) and table["write_disposition"] in job_client.get_stage_dispositions():
-            with job_client.with_staging_dataset():
-                yield
-        else:
-            yield
-
     @staticmethod
     @workermethod
     def w_spool_job(self: "Load", file_path: str, load_id: str, schema: Schema) -> Optional[LoadJob]:
         job: LoadJob = None
         try:
             # if we have a staging destination and the file is not a reference, send to staging
-            job_client = self.get_staging_destination_client(schema) if self.is_staging_destination_job(file_path) else self.get_destination_client(schema)
-            with job_client as job_client:
+            client = self.get_staging_client(schema) if self.is_staging_job(file_path) else self.get_destination_client(schema)
+            with client as client:
                 job_info = self.load_storage.parse_job_file_name(file_path)
                 if job_info.file_format not in self.load_storage.supported_file_formats:
                     raise LoadClientUnsupportedFileFormats(job_info.file_format, self.capabilities.supported_loader_file_formats, file_path)
                 logger.info(f"Will load file {file_path} with table name {job_info.table_name}")
                 table = self.get_load_table(schema, file_path)
                 if table["write_disposition"] not in ["append", "replace", "merge"]:
                     raise LoadClientUnsupportedWriteDisposition(job_info.table_name, table["write_disposition"], file_path)
-                with self.maybe_with_staging_dataset(job_client, table):
-                    job = job_client.start_file_load(table, self.load_storage.storage.make_full_path(file_path), load_id)
+                job = client.start_file_load(table, self.load_storage.storage.make_full_path(file_path), load_id)
         except (DestinationTerminalException, TerminalValueError):
             # if job irreversibly cannot be started, mark it as failed
             logger.exception(f"Terminal problem when adding job {file_path}")
             job = EmptyLoadJob.from_file_path(file_path, "failed", pretty_format_exception())
         except (DestinationTransientException, Exception):
             # return no job so file stays in new jobs (root) folder
             logger.exception(f"Temporary problem when adding job {file_path}")
@@ -142,28 +119,31 @@
         param_chunk = [(id(self), file, load_id, schema) for file in load_files]
         # exceptions should not be raised, None as job is a temporary failure
         # other jobs should not be affected
         jobs: List[LoadJob] = self.pool.starmap(Load.w_spool_job, param_chunk)
         # remove None jobs and check the rest
         return file_count, [job for job in jobs if job is not None]
 
+    def is_staging_job(self, file_path: str) -> bool:
+        return self.staging is not None and os.path.splitext(file_path)[1][1:] in self.staging.capabilities().supported_loader_file_formats
+
     def retrieve_jobs(self, client: JobClientBase, load_id: str, staging_client: JobClientBase = None) -> Tuple[int, List[LoadJob]]:
         jobs: List[LoadJob] = []
 
         # list all files that were started but not yet completed
         started_jobs = self.load_storage.list_started_jobs(load_id)
 
         logger.info(f"Found {len(started_jobs)} that are already started and should be continued")
         if len(started_jobs) == 0:
             return 0, jobs
 
         for file_path in started_jobs:
             try:
                 logger.info(f"Will retrieve {file_path}")
-                client = staging_client if self.is_staging_destination_job(file_path) else client
+                client = staging_client if self.is_staging_job(file_path) else client
                 job = client.restore_file_load(file_path)
             except DestinationTerminalException:
                 logger.exception(f"Job retrieval for {file_path} failed, job will be terminated")
                 job = EmptyLoadJob.from_file_path(file_path, "failed", pretty_format_exception())
                 # proceed to appending job, do not reraise
             except (DestinationTransientException, Exception):
                 # raise on all temporary exceptions, typically network / server problems
@@ -176,40 +156,39 @@
         jobs_info: List[ParsedLoadJobFileName] = []
         new_job_files = self.load_storage.list_new_jobs(load_id)
         for job_file in new_job_files:
             if not dispositions or self.get_load_table(schema, job_file)["write_disposition"] in dispositions:
                 jobs_info.append(LoadStorage.parse_job_file_name(job_file))
         return jobs_info
 
-
     def get_completed_table_chain(self, load_id: str, schema: Schema, top_merged_table: TTableSchema, starting_job_id: str) -> List[TTableSchema]:
         """Gets a table chain starting from the `top_merged_table` containing only tables with completed/failed jobs. None is returned if there's any job that is not completed"""
         # returns ordered list of tables from parent to child leaf tables
         table_chain: List[TTableSchema] = []
         # make sure all the jobs for the table chain is completed
         for table in get_child_tables(schema.tables, top_merged_table["name"]):
             table_jobs = self.load_storage.list_jobs_for_table(load_id, table["name"])
+            # if no jobs for table then skip the table in the chain. we assume that if parent has no jobs, the child would also have no jobs
+            # so it will be eliminated by this loop as well
+            if not table_jobs:
+                continue
             # all jobs must be completed in order for merge to be created
             if any(job.state not in ("failed_jobs", "completed_jobs") and job.job_file_info.job_id() != starting_job_id for job in table_jobs):
                 return None
-            # if there are no jobs for the table, skip it, unless the write disposition is replace, as we need to create and clear the child tables
-            if not table_jobs and top_merged_table["write_disposition"] != "replace":
-                 continue
             table_chain.append(table)
-        # there must be at least table
+        # there must be at least 1 job
         assert len(table_chain) > 0
         return table_chain
 
     def create_followup_jobs(self, load_id: str, state: TLoadJobState, starting_job: LoadJob, schema: Schema) -> List[NewLoadJob]:
         jobs: List[NewLoadJob] = []
         if isinstance(starting_job, FollowupJob):
-            # check for merge jobs only for jobs executing on the destination, the staging destination jobs must be excluded
-            # NOTE: we may move that logic to the interface
+            # check for merge jobs only for non-staging jobs. we may move that logic to the interface
             starting_job_file_name = starting_job.file_name()
-            if state == "completed" and not self.is_staging_destination_job(starting_job_file_name):
+            if state == "completed" and not self.is_staging_job(starting_job_file_name):
                 client = self.destination.client(schema, self.initial_client_config)
                 top_job_table = get_top_level_table(schema.tables, self.get_load_table(schema, starting_job_file_name)["name"])
                 # if all tables of chain completed, create follow  up jobs
                 if table_chain := self.get_completed_table_chain(load_id, schema, top_job_table, starting_job.job_file_info().job_id()):
                     if follow_up_jobs := client.create_table_chain_completed_followup_jobs(table_chain):
                         jobs = jobs + follow_up_jobs
             jobs = jobs + starting_job.create_followup_jobs(state)
@@ -257,68 +236,56 @@
             if state in ["failed", "completed"]:
                 self.collector.update("Jobs")
                 if state == "failed":
                     self.collector.update("Jobs", 1, message="WARNING: Some of the jobs failed!", label="Failed")
 
         return remaining_jobs
 
+    def get_destination_client(self, schema: Schema) -> JobClientBase:
+        return self.destination.client(schema, self.initial_client_config)
+
     def complete_package(self, load_id: str, schema: Schema, aborted: bool = False) -> None:
         # do not commit load id for aborted packages
         if not aborted:
             with self.get_destination_client(schema) as job_client:
                 job_client.complete_load(load_id)
         self.load_storage.complete_load_package(load_id, aborted)
         logger.info(f"All jobs completed, archiving package {load_id} with aborted set to {aborted}")
         self._processed_load_ids[load_id] = 1
 
-    def get_table_chain_tables_for_write_disposition(self, load_id: str, schema: Schema, dispositions: List[TWriteDisposition]) -> Set[str]:
-        """Get all jobs for tables with given write disposition and resolve the table chain"""
-        result: Set[str] = set()
-        table_jobs = self.get_new_jobs_info(load_id, schema, dispositions)
-        for job in table_jobs:
-            top_job_table = get_top_level_table(schema.tables, self.get_load_table(schema, job.job_id())["name"])
-            table_chain = get_child_tables(schema.tables, top_job_table["name"])
-            for table in table_chain:
-                existing_jobs = self.load_storage.list_jobs_for_table(load_id, table["name"])
-                # only add tables for tables that have jobs unless the disposition is replace
-                if not existing_jobs and top_job_table["write_disposition"] != "replace":
-                    continue
-                result.add(table["name"])
-        return result
-
     def load_single_package(self, load_id: str, schema: Schema) -> None:
         # initialize analytical storage ie. create dataset required by passed schema
         job_client: JobClientBase
         with self.get_destination_client(schema) as job_client:
             expected_update = self.load_storage.begin_schema_update(load_id)
             if expected_update is not None:
                 # update the default dataset
                 logger.info(f"Client for {job_client.config.destination_name} will start initialize storage")
-                truncate_tables = self.get_table_chain_tables_for_write_disposition(load_id, schema, job_client.get_truncate_destination_table_dispositions())
-                job_client.initialize_storage(truncate_tables=truncate_tables)
+                job_client.initialize_storage()
                 logger.info(f"Client for {job_client.config.destination_name} will update schema to package schema")
                 all_jobs = self.get_new_jobs_info(load_id, schema)
                 all_tables = set(job.table_name for job in all_jobs)
                 dlt_tables = set(t["name"] for t in schema.dlt_tables())
                 # only update tables that are present in the load package
                 applied_update = job_client.update_storage_schema(only_tables=all_tables | dlt_tables, expected_update=expected_update)
                 # update the staging dataset if client supports this
                 if isinstance(job_client, StagingJobClientBase):
-                    if staging_tables := self.get_table_chain_tables_for_write_disposition(load_id, schema, job_client.get_stage_dispositions()):
+                    if staging_table_jobs := self.get_new_jobs_info(load_id, schema, job_client.get_stage_dispositions()):
                         with job_client.with_staging_dataset():
                             logger.info(f"Client for {job_client.config.destination_name} will start initialize STAGING storage")
                             job_client.initialize_storage()
                             logger.info(f"Client for {job_client.config.destination_name} will UPDATE STAGING SCHEMA to package schema")
+                            staging_tables = set(job.table_name for job in staging_table_jobs)
                             job_client.update_storage_schema(only_tables=staging_tables | {VERSION_TABLE_NAME}, expected_update=expected_update)
                             logger.info(f"Client for {job_client.config.destination_name} will TRUNCATE STAGING TABLES: {staging_tables}")
                             job_client.initialize_storage(truncate_tables=staging_tables)
                 self.load_storage.commit_schema_update(load_id, applied_update)
             # spool or retrieve unfinished jobs
-            if self.staging_destination:
-                with self.get_staging_destination_client(schema) as staging_client:
+            if self.staging:
+                with self.get_staging_client(schema) as staging_client:
                     jobs_count, jobs = self.retrieve_jobs(job_client, load_id, staging_client)
             else:
                 jobs_count, jobs = self.retrieve_jobs(job_client, load_id)
 
         if not jobs:
             # jobs count is a total number of jobs including those that could not be initialized
             jobs_count, jobs = self.spool_new_jobs(load_id, schema)
@@ -358,14 +325,17 @@
                 # this will raise on signal
                 sleep(1)
             except LoadClientJobFailed:
                 # the package is completed and skipped
                 self.complete_package(load_id, schema, True)
                 raise
 
+    def get_staging_client(self, schema: Schema) -> JobClientBase:
+        return self.staging.client(schema, self.initial_staging_client_config)
+
     def run(self, pool: ThreadPool) -> TRunMetrics:
         # store pool
         self.pool = pool
 
         logger.info("Running file loading")
         # get list of loads and order by name ASC to execute schema updates
         loads = self.load_storage.list_packages()
```

### Comparing `dlt-0.3.6/dlt/normalize/configuration.py` & `dlt-0.3.6a0/dlt/normalize/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/normalize/normalize.py` & `dlt-0.3.6a0/dlt/normalize/normalize.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from typing import Any, Callable, List, Dict, Sequence, Tuple, Set
+from typing import Any, Callable, List, Dict, Sequence, Tuple
 from multiprocessing.pool import AsyncResult, Pool as ProcessPool
 
 from dlt.common import pendulum, json, logger, sleep
 from dlt.common.configuration import with_config, known_sections
 from dlt.common.configuration.accessors import config
 from dlt.common.configuration.container import Container
 from dlt.common.destination import DestinationCapabilitiesContext, TLoaderFileFormat
@@ -48,14 +48,15 @@
 
     def create_storages(self) -> None:
         # pass initial normalize storage config embedded in normalize config
         self.normalize_storage = NormalizeStorage(True, config=self.config._normalize_storage_config)
         # normalize saves in preferred format but can read all supported formats
         self.load_storage = LoadStorage(True, self.config.destination_capabilities.preferred_loader_file_format, LoadStorage.ALL_SUPPORTED_FILE_FORMATS, config=self.config._load_storage_config)
 
+
     @staticmethod
     def load_or_create_schema(schema_storage: SchemaStorage, schema_name: str) -> Schema:
         try:
             schema = schema_storage.load_schema(schema_name)
             logger.info(f"Loaded schema with name {schema_name} with version {schema.stored_version}")
         except SchemaNotFoundError:
             schema = Schema(schema_name)
@@ -77,41 +78,29 @@
         # process all files with data items and write to buffered item storage
         with Container().injectable_context(destination_caps):
             schema = Schema.from_stored_schema(stored_schema)
             load_storage = LoadStorage(False, destination_caps.preferred_loader_file_format, LoadStorage.ALL_SUPPORTED_FILE_FORMATS, loader_storage_config)
             normalize_storage = NormalizeStorage(False, normalize_storage_config)
 
             try:
-                root_tables: Set[str] = set()
-                populated_root_tables: Set[str] = set()
                 for extracted_items_file in extracted_items_files:
                     line_no: int = 0
                     root_table_name = NormalizeStorage.parse_normalize_file_name(extracted_items_file).table_name
-                    root_tables.add(root_table_name)
                     logger.debug(f"Processing extracted items in {extracted_items_file} in load_id {load_id} with table name {root_table_name} and schema {schema.name}")
                     with normalize_storage.storage.open_file(extracted_items_file) as f:
                         # enumerate jsonl file line by line
-                        items_count = 0
                         for line_no, line in enumerate(f):
                             items: List[TDataItem] = json.loads(line)
                             partial_update, items_count = Normalize._w_normalize_chunk(load_storage, schema, load_id, root_table_name, items)
                             schema_updates.append(partial_update)
                             total_items += items_count
                             logger.debug(f"Processed {line_no} items from file {extracted_items_file}, items {items_count} of total {total_items}")
                         # if any item found in the file
                         if items_count > 0:
-                            populated_root_tables.add(root_table_name)
                             logger.debug(f"Processed total {line_no + 1} lines from file {extracted_items_file}, total items {total_items}")
-                # write empty jobs for tables without items if table exists in schema
-                for table_name in root_tables - populated_root_tables:
-                    if table_name not in schema.tables:
-                        continue
-                    logger.debug(f"Writing empty job for table {table_name}")
-                    columns = schema.get_table_columns(table_name)
-                    load_storage.write_empty_file(load_id, schema.name, table_name, columns)
             except Exception:
                 logger.exception(f"Exception when processing file {extracted_items_file}, line {line_no}")
                 raise
             finally:
                 load_storage.close_writers(load_id)
 
         logger.info(f"Processed total {total_items} items in {len(extracted_items_files)} files")
@@ -139,19 +128,19 @@
                     # theres a new table or new columns in existing table
                     if partial_table:
                         # update schema and save the change
                         schema.update_schema(partial_table)
                         table_updates = schema_update.setdefault(table_name, [])
                         table_updates.append(partial_table)
                         # update our columns
-                        column_schemas[table_name] = schema.get_table_columns(table_name)
+                        column_schemas[table_name] = schema.get_table_columns(table_name, only_complete=True)
                     # get current columns schema
                     columns = column_schemas.get(table_name)
                     if not columns:
-                        columns = schema.get_table_columns(table_name)
+                        columns = schema.get_table_columns(table_name, only_complete=True)
                         column_schemas[table_name] = columns
                     # store row
                     # TODO: it is possible to write to single file from many processes using this: https://gitlab.com/warsaw/flufl.lock
                     load_storage.write_data_item(load_id, schema_name, table_name, row, columns)
                     # count total items
                     items_count += 1
             signals.raise_if_signalled()
```

### Comparing `dlt-0.3.6/dlt/pipeline/__init__.py` & `dlt-0.3.6a0/dlt/pipeline/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,26 +144,24 @@
 
 @with_config(spec=PipelineConfiguration, auto_pipeline_section=True)
 def attach(
     pipeline_name: str = None,
     pipelines_dir: str = None,
     pipeline_salt: TSecretValue = None,
     full_refresh: bool = False,
-    credentials: Any = None,
     progress: TCollectorArg = _NULL_COLLECTOR,
     **kwargs: Any
 ) -> Pipeline:
-    """Attaches to the working folder of `pipeline_name` in `pipelines_dir` or in default directory. Requires that valid pipeline state exists in working folder."""
     ensure_correct_pipeline_kwargs(attach, **kwargs)
     # if working_dir not provided use temp folder
     if not pipelines_dir:
         pipelines_dir = get_dlt_pipelines_dir()
     progress = collector_from_name(progress)
     # create new pipeline instance
-    p = Pipeline(pipeline_name, pipelines_dir, pipeline_salt, None, None, None, credentials, None, None, full_refresh, progress, True, last_config(**kwargs), kwargs["runtime"])
+    p = Pipeline(pipeline_name, pipelines_dir, pipeline_salt, None, None, None, None, None, None, full_refresh, progress, True, last_config(**kwargs), kwargs["runtime"])
     # set it as current pipeline
     p.activate()
     return p
 
 
 def run(
     data: Any,
```

### Comparing `dlt-0.3.6/dlt/pipeline/configuration.py` & `dlt-0.3.6a0/dlt/pipeline/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/pipeline/dbt.py` & `dlt-0.3.6a0/dlt/pipeline/dbt.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/pipeline/exceptions.py` & `dlt-0.3.6a0/dlt/pipeline/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/pipeline/helpers.py` & `dlt-0.3.6a0/dlt/pipeline/helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/pipeline/pipeline.py` & `dlt-0.3.6a0/dlt/pipeline/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -363,15 +363,15 @@
         load_config = LoaderConfiguration(
             workers=workers,
             raise_on_failed_jobs=raise_on_failed_jobs,
             _load_storage_config=self._load_storage_config
         )
         load = Load(
             self.destination,
-            staging_destination=self.staging,
+            staging=self.staging,
             collector=self.collector,
             is_storage_owner=False,
             config=load_config,
             initial_client_config=client.config,
             initial_staging_client_config=staging_client.config if staging_client else None
         )
         try:
@@ -1155,17 +1155,16 @@
                     schema_info = job_client.get_newest_schema_from_storage()
                     if schema_info is None:
                         logger.info(f"The schema {schema_name} was not found in the destination {self.destination.__name__}:{job_client.sql_client.dataset_name}.")
                         # try to import schema
                         with contextlib.suppress(FileNotFoundError):
                             self._schema_storage.load_schema(schema_name)
                     else:
-                        schema = Schema.from_dict(json.loads(schema_info.schema))
-                        logger.info(f"The schema {schema_name} version {schema.version} hash {schema.stored_version_hash} was restored from the destination {self.destination.__name__}:{job_client.sql_client.dataset_name}")
-                        restored_schemas.append(schema)
+                        logger.info(f"The schema {schema_name} was restored from the destination {self.destination.__name__}:{job_client.sql_client.dataset_name}")
+                        restored_schemas.append(Schema.from_dict(json.loads(schema_info.schema)))
         return restored_schemas
 
     @contextmanager
     def managed_state(self, *, extract_state: bool = False) -> Iterator[TPipelineState]:
         # load or restore state
         state = self._get_state()
         # TODO: we should backup schemas here
```

### Comparing `dlt-0.3.6/dlt/pipeline/progress.py` & `dlt-0.3.6a0/dlt/pipeline/progress.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/pipeline/state_sync.py` & `dlt-0.3.6a0/dlt/pipeline/state_sync.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/pipeline/trace.py` & `dlt-0.3.6a0/dlt/pipeline/trace.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/pipeline/track.py` & `dlt-0.3.6a0/dlt/pipeline/track.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/reflection/names.py` & `dlt-0.3.6a0/dlt/reflection/names.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/reflection/script_inspector.py` & `dlt-0.3.6a0/dlt/reflection/script_inspector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/reflection/script_visitor.py` & `dlt-0.3.6a0/dlt/reflection/script_visitor.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/sources/helpers/requests/__init__.py` & `dlt-0.3.6a0/dlt/sources/helpers/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/sources/helpers/requests/retry.py` & `dlt-0.3.6a0/dlt/sources/helpers/requests/retry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/sources/helpers/requests/session.py` & `dlt-0.3.6a0/dlt/sources/helpers/requests/session.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/sources/helpers/transform.py` & `dlt-0.3.6a0/dlt/sources/helpers/transform.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/dlt/version.py` & `dlt-0.3.6a0/dlt/version.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.6/pyproject.toml` & `dlt-0.3.6a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dlt"
-version = "0.3.6"
+version = "0.3.6a0"
 description = "DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run."
 authors = ["dltHub Inc. <services@dlthub.com>"]
 maintainers = [ "Marcin Rudolf <marcin@dlthub.com>", "Adrian Brudaru <adrian@dlthub.com>", "Ty Dunn <ty@dlthub.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/dlt-hub"
 repository = "https://github.com/dlt-hub/dlt"
```

### Comparing `dlt-0.3.6/setup.py` & `dlt-0.3.6a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
  'snowflake': ['snowflake-connector-python[pandas]>=3.0.4,<4.0.0']}
 
 entry_points = \
 {'console_scripts': ['dlt = dlt.cli._dlt:_main']}
 
 setup_kwargs = {
     'name': 'dlt',
-    'version': '0.3.6',
+    'version': '0.3.6a0',
     'description': 'DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run.',
     'long_description': '<h1 align="center">\n    <strong>data load tool (dlt) — the open-source Python library for data loading</strong>\n</h1>\n<p align="center">\nBe it a Google Colab notebook, AWS Lambda function, an Airflow DAG, your local laptop,<br/>or a GPT-4 assisted development playground—<strong>dlt</strong> can be dropped in anywhere.\n</p>\n\n<div align="center">\n  <a target="_blank" href="https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g" style="background:none">\n    <img src="https://img.shields.io/badge/slack-join-dlt.svg?labelColor=191937&color=6F6FF7&logo=slack" />\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/v/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/pyversions/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n</div>\n\n## Installation\n\ndlt supports Python 3.8+.\n\n```bash\npip install dlt\n```\n\n## Quick Start\n\nLoad chess game data from chess.com API and save it in DuckDB:\n\n```python\nimport dlt\nimport requests\n# Create a dlt pipeline that will load\n# chess player data to the DuckDB destination\npipeline = dlt.pipeline(\n    pipeline_name=\'chess_pipeline\',\n    destination=\'duckdb\',\n    dataset_name=\'player_data\'\n)\n# Grab some player data from Chess.com API\ndata = []\nfor player in [\'magnuscarlsen\', \'rpragchess\']:\n    response = requests.get(f\'https://api.chess.com/pub/player/{player}\')\n    response.raise_for_status()\n    data.append(response.json())\n# Extract, normalize, and load the data\npipeline.run(data, table_name=\'player\')\n```\n\n\nTry it out in our **[Colab Demo](https://colab.research.google.com/drive/1NfSB1DpwbbHX9_t5vlalBTf13utwpMGx?usp=sharing)**\n\n## Features\n\n- **Automatic Schema:** Data structure inspection and schema creation for the destination.\n- **Data Normalization:** Consistent and verified data before loading.\n- **Seamless Integration:** Colab, AWS Lambda, Airflow, and local environments.\n- **Scalable:** Adapts to growing data needs in production.\n- **Easy Maintenance:** Clear data pipeline structure for updates.\n- **Rapid Exploration:** Quickly explore and gain insights from new data sources.\n- **Versatile Usage:** Suitable for ad-hoc exploration to advanced loading infrastructures.\n- **Start in Seconds with CLI:** Powerful CLI for managing, deploying and inspecting local pipelines.\n- **Incremental Loading:** Load only new or changed data and avoid loading old records again.\n- **Open Source:** Free and Apache 2.0 Licensed.\n\n## Ready to use Sources and Destinations\n\nExplore ready to use sources (e.g. Google Sheets) in the [Verified Sources docs](https://dlthub.com/docs/dlt-ecosystem/verified-sources) and supported destinations (e.g. DuckDB) in the [Destinations docs](https://dlthub.com/docs/dlt-ecosystem/destinations).\n\n## Documentation\n\nFor detailed usage and configuration, please refer to the [official documentation](https://dlthub.com/docs).\n\n## Examples\n\nYou can find examples for various use cases in the [examples](docs/examples) folder.\n\n## Get Involved\n\nThe dlt project is quickly growing, and we\'re excited to have you join our community! Here\'s how you can get involved:\n\n- **Connect with the Community**: Join other dlt users and contributors on our [Slack](https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g)\n- **Report issues and suggest features**: Please use the [GitHub Issues](https://github.com/dlt-hub/dlt/issues) to report bugs or suggest new features. Before creating a new issue, make sure to search the tracker for possible duplicates and add a comment if you find one.\n- **Contribute Verified Sources**: Contribute your custom sources to the [dlt-hub/verified-sources](https://github.com/dlt-hub/verified-sources) to help other folks in handling their data tasks.\n- **Contribute code**: Check out our [contributing guidelines](CONTRIBUTING.md) for information on how to make a pull request.\n- **Improve documentation**: Help us enhance the dlt documentation.\n\n## License\n\nDLT is released under the [Apache 2.0 License](LICENSE.txt).\n',
     'author': 'dltHub Inc.',
     'author_email': 'services@dlthub.com',
     'maintainer': 'Marcin Rudolf',
     'maintainer_email': 'marcin@dlthub.com',
     'url': 'https://github.com/dlt-hub',
```

### Comparing `dlt-0.3.6/PKG-INFO` & `dlt-0.3.6a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlt
-Version: 0.3.6
+Version: 0.3.6a0
 Summary: DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run.
 Home-page: https://github.com/dlt-hub
 License: Apache-2.0
 Keywords: etl
 Author: dltHub Inc.
 Author-email: services@dlthub.com
 Maintainer: Marcin Rudolf
```

