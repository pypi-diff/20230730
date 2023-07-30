# Comparing `tmp/tfx-ann-ct-pipeline-0.0.1.tar.gz` & `tmp/tfx-ann-ct-pipeline-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tfx-ann-ct-pipeline-0.0.1.tar", last modified: Sun Jul 30 14:49:42 2023, max compression
+gzip compressed data, was "tfx-ann-ct-pipeline-0.0.2.tar", last modified: Sun Jul 30 15:17:46 2023, max compression
```

## Comparing `tfx-ann-ct-pipeline-0.0.1.tar` & `tfx-ann-ct-pipeline-0.0.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:49:42.051981 tfx-ann-ct-pipeline-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-30 14:49:42.047981 tfx-ann-ct-pipeline-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:49:42.043981 tfx-ann-ct-pipeline-0.0.1/cencus_consumer_complaint_executor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/cencus_consumer_complaint_executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/cencus_consumer_complaint_executor/zip_csv_executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:49:42.043981 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_component/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_component/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_component/data_ingestion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_component/data_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_component/data_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:49:42.043981 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_component/feature_engineering/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_component/feature_engineering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_component/feature_engineering/feature_engineering.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_component/model_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_component/model_pusher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_component/model_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:49:42.043981 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_component/model_training/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_component/model_training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_component/model_training/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:49:42.043981 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_config/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:49:42.043981 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_custom_component/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_custom_component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_custom_component/component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:49:42.043981 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_custom_component/example_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_custom_component/example_gen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:49:42.047981 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_custom_component/example_gen/remote_zip_csv_example_gen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_custom_component/example_gen/remote_zip_csv_example_gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_custom_component/example_gen/remote_zip_csv_example_gen/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_custom_component/example_gen/remote_zip_csv_example_gen/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_custom_component/example_gen/remote_zip_csv_example_gen/executor_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:49:42.047981 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_exception/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_exception/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:49:42.047981 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_orchestrator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_orchestrator/airflow_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_orchestrator/apache_beam_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_orchestrator/interactive_context_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_orchestrator/local_orchestrator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:49:42.047981 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_types/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:49:42.047981 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 14:49:42.051981 tfx-ann-ct-pipeline-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-30 14:49:28.000000 tfx-ann-ct-pipeline-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:49:42.047981 tfx-ann-ct-pipeline-0.0.1/tfx_ann_ct_pipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-30 14:49:42.000000 tfx-ann-ct-pipeline-0.0.1/tfx_ann_ct_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-30 14:49:42.000000 tfx-ann-ct-pipeline-0.0.1/tfx_ann_ct_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 14:49:42.000000 tfx-ann-ct-pipeline-0.0.1/tfx_ann_ct_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-30 14:49:42.000000 tfx-ann-ct-pipeline-0.0.1/tfx_ann_ct_pipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-30 14:49:42.000000 tfx-ann-ct-pipeline-0.0.1/tfx_ann_ct_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:17:46.917009 tfx-ann-ct-pipeline-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-30 15:17:46.917009 tfx-ann-ct-pipeline-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:17:46.905008 tfx-ann-ct-pipeline-0.0.2/cencus_consumer_complaint_executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/cencus_consumer_complaint_executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/cencus_consumer_complaint_executor/zip_csv_executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:17:46.905008 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_component/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_component/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_component/data_ingestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_component/data_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_component/data_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:17:46.913009 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_component/feature_engineering/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_component/feature_engineering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_component/feature_engineering/feature_engineering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_component/model_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_component/model_pusher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_component/model_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:17:46.913009 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_component/model_training/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_component/model_training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_component/model_training/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:17:46.913009 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_config/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:17:46.913009 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_custom_component/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_custom_component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_custom_component/component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:17:46.913009 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_custom_component/example_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_custom_component/example_gen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:17:46.913009 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_custom_component/example_gen/remote_zip_csv_example_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_custom_component/example_gen/remote_zip_csv_example_gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_custom_component/example_gen/remote_zip_csv_example_gen/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_custom_component/example_gen/remote_zip_csv_example_gen/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_custom_component/example_gen/remote_zip_csv_example_gen/executor_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:17:46.913009 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_exception/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_exception/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:17:46.913009 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_orchestrator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_orchestrator/airflow_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_orchestrator/apache_beam_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_orchestrator/interactive_context_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_orchestrator/local_orchestrator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:17:46.913009 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_types/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:17:46.913009 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 15:17:46.917009 tfx-ann-ct-pipeline-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-30 15:17:35.000000 tfx-ann-ct-pipeline-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:17:46.913009 tfx-ann-ct-pipeline-0.0.2/tfx_ann_ct_pipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-30 15:17:46.000000 tfx-ann-ct-pipeline-0.0.2/tfx_ann_ct_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-30 15:17:46.000000 tfx-ann-ct-pipeline-0.0.2/tfx_ann_ct_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 15:17:46.000000 tfx-ann-ct-pipeline-0.0.2/tfx_ann_ct_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-30 15:17:46.000000 tfx-ann-ct-pipeline-0.0.2/tfx_ann_ct_pipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-30 15:17:46.000000 tfx-ann-ct-pipeline-0.0.2/tfx_ann_ct_pipeline.egg-info/top_level.txt
```

### Comparing `tfx-ann-ct-pipeline-0.0.1/README.md` & `tfx-ann-ct-pipeline-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tfx-ann-ct-pipeline-0.0.1/cencus_consumer_complaint_executor/zip_csv_executor.py` & `tfx-ann-ct-pipeline-0.0.2/cencus_consumer_complaint_executor/zip_csv_executor.py`

 * *Files identical despite different names*

### Comparing `tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_component/component.py` & `tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_component/component.py`

 * *Files identical despite different names*

### Comparing `tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_component/data_ingestion.py` & `tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_component/data_ingestion.py`

 * *Files identical despite different names*

### Comparing `tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_component/data_preprocessing.py` & `tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_component/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_component/data_validation.py` & `tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_component/data_validation.py`

 * *Files identical despite different names*

### Comparing `tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_component/feature_engineering/feature_engineering.py` & `tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_component/feature_engineering/feature_engineering.py`

 * *Files identical despite different names*

### Comparing `tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_component/model_evaluation.py` & `tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_component/model_evaluation.py`

 * *Files identical despite different names*

### Comparing `tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_component/model_pusher.py` & `tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_component/model_pusher.py`

 * *Files identical despite different names*

### Comparing `tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_component/model_trainer.py` & `tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_component/model_trainer.py`

 * *Files identical despite different names*

### Comparing `tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_component/model_training/trainer.py` & `tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_component/model_training/trainer.py`

 * *Files identical despite different names*

### Comparing `tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_config/configuration.py` & `tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_config/configuration.py`

 * *Files identical despite different names*

### Comparing `tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_custom_component/component.py` & `tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_custom_component/component.py`

 * *Files identical despite different names*

### Comparing `tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_custom_component/example_gen/remote_zip_csv_example_gen/component.py` & `tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_custom_component/example_gen/remote_zip_csv_example_gen/component.py`

 * *Files identical despite different names*

### Comparing `tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_custom_component/example_gen/remote_zip_csv_example_gen/executor.py` & `tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_custom_component/example_gen/remote_zip_csv_example_gen/executor.py`

 * *Files identical despite different names*

### Comparing `tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_custom_component/example_gen/remote_zip_csv_example_gen/executor_test.py` & `tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_custom_component/example_gen/remote_zip_csv_example_gen/executor_test.py`

 * *Files identical despite different names*

### Comparing `tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_exception/exception.py` & `tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_exception/exception.py`

 * *Files identical despite different names*

### Comparing `tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_orchestrator/airflow_orchestrator.py` & `tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_orchestrator/airflow_orchestrator.py`

 * *Files identical despite different names*

### Comparing `tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_orchestrator/apache_beam_orchestrator.py` & `tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_orchestrator/apache_beam_orchestrator.py`

 * *Files identical despite different names*

### Comparing `tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_orchestrator/interactive_context_runner.py` & `tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_orchestrator/interactive_context_runner.py`

 * *Files identical despite different names*

### Comparing `tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_orchestrator/local_orchestrator.py` & `tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_orchestrator/local_orchestrator.py`

 * *Files identical despite different names*

### Comparing `tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_types/types.py` & `tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_types/types.py`

 * *Files identical despite different names*

### Comparing `tfx-ann-ct-pipeline-0.0.1/census_consumer_complaint_utils/utils.py` & `tfx-ann-ct-pipeline-0.0.2/census_consumer_complaint_utils/utils.py`

 * *Files identical despite different names*

### Comparing `tfx-ann-ct-pipeline-0.0.1/setup.py` & `tfx-ann-ct-pipeline-0.0.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
      name="tfx-ann-ct-pipeline",
     license="MIT",
-    version="0.0.1",
+    version="0.0.2",
     description="""
     This project is created to provide a simple way to
     ingest data from the Census API.
     https://files.consumerfinance.gov/ccdb/complaints.csv.zip
 
     Project provide prebuilt airflow DAG pipleine designed using TFX
     how to use this library
     ```
     from census_consumer_complaint_orchestrator.airflow_orchestrator import get_airflow_dag_pipeline
     dag = get_airflow_dag_pipeline()
     ```
     """,
-    long_description = "This is a test deployment",
+    long_description = "This is a test deployment", # long description is mandatory 
     author="Manjesh Kumar",
     packages=find_packages(),
     install_requires=['tfx==1.6.1', 'apache-beam[interactive]', 'apache-airflow']
 )
```

### Comparing `tfx-ann-ct-pipeline-0.0.1/tfx_ann_ct_pipeline.egg-info/SOURCES.txt` & `tfx-ann-ct-pipeline-0.0.2/tfx_ann_ct_pipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

